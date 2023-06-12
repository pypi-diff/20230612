# Comparing `tmp/littletable-2.2.2.tar.gz` & `tmp/littletable-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "littletable-2.2.2.tar", last modified: Sun May 28 19:24:44 2023, max compression
+gzip compressed data, was "littletable-2.2.3.tar", last modified: Mon Jun 12 02:49:44 2023, max compression
```

## Comparing `littletable-2.2.2.tar` & `littletable-2.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-05-28 19:24:44.237011 littletable-2.2.2/
--rw-rw-r--   0 paul      (1000) paul      (1000)    36660 2023-05-28 19:24:38.000000 littletable-2.2.2/CHANGES
--rw-rw-r--   0 paul      (1000) paul      (1000)      247 2023-04-30 06:48:17.000000 littletable-2.2.2/HowToUseLittletable.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)     1080 2023-04-30 06:48:17.000000 littletable-2.2.2/LICENSE
--rw-rw-r--   0 paul      (1000) paul      (1000)      222 2023-04-30 06:48:17.000000 littletable-2.2.2/MANIFEST.in
--rw-rw-r--   0 paul      (1000) paul      (1000)     7510 2023-05-28 19:24:44.237011 littletable-2.2.2/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)     6449 2023-04-30 06:48:17.000000 littletable-2.2.2/README.md
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-05-28 19:24:44.237011 littletable-2.2.2/littletable.egg-info/
--rw-rw-r--   0 paul      (1000) paul      (1000)     7510 2023-05-28 19:24:44.000000 littletable-2.2.2/littletable.egg-info/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)      249 2023-05-28 19:24:44.000000 littletable-2.2.2/littletable.egg-info/SOURCES.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)        1 2023-05-28 19:24:44.000000 littletable-2.2.2/littletable.egg-info/dependency_links.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       12 2023-05-28 19:24:44.000000 littletable-2.2.2/littletable.egg-info/top_level.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)   163352 2023-05-28 19:24:38.000000 littletable-2.2.2/littletable.py
--rw-rw-r--   0 paul      (1000) paul      (1000)       38 2023-05-28 19:24:44.237011 littletable-2.2.2/setup.cfg
--rw-rw-r--   0 paul      (1000) paul      (1000)     1467 2023-04-30 06:48:17.000000 littletable-2.2.2/setup.py
--rw-rw-r--   0 paul      (1000) paul      (1000)   110775 2023-05-28 19:07:07.000000 littletable-2.2.2/unit_tests.py
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-06-12 02:49:44.377186 littletable-2.2.3/
+-rw-rw-r--   0 paul      (1000) paul      (1000)    37635 2023-06-12 02:49:33.000000 littletable-2.2.3/CHANGES
+-rw-rw-r--   0 paul      (1000) paul      (1000)      247 2023-04-30 06:48:17.000000 littletable-2.2.3/HowToUseLittletable.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1080 2023-04-30 06:48:17.000000 littletable-2.2.3/LICENSE
+-rw-rw-r--   0 paul      (1000) paul      (1000)      222 2023-04-30 06:48:17.000000 littletable-2.2.3/MANIFEST.in
+-rw-rw-r--   0 paul      (1000) paul      (1000)     7510 2023-06-12 02:49:44.377186 littletable-2.2.3/PKG-INFO
+-rw-rw-r--   0 paul      (1000) paul      (1000)     6449 2023-04-30 06:48:17.000000 littletable-2.2.3/README.md
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-06-12 02:49:44.377186 littletable-2.2.3/littletable.egg-info/
+-rw-rw-r--   0 paul      (1000) paul      (1000)     7510 2023-06-12 02:49:44.000000 littletable-2.2.3/littletable.egg-info/PKG-INFO
+-rw-rw-r--   0 paul      (1000) paul      (1000)      249 2023-06-12 02:49:44.000000 littletable-2.2.3/littletable.egg-info/SOURCES.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)        1 2023-06-12 02:49:44.000000 littletable-2.2.3/littletable.egg-info/dependency_links.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)       12 2023-06-12 02:49:44.000000 littletable-2.2.3/littletable.egg-info/top_level.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)   169142 2023-06-12 02:49:33.000000 littletable-2.2.3/littletable.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)       38 2023-06-12 02:49:44.377186 littletable-2.2.3/setup.cfg
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1467 2023-04-30 06:48:17.000000 littletable-2.2.3/setup.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)   114429 2023-06-12 02:49:33.000000 littletable-2.2.3/unit_tests.py
```

### Comparing `littletable-2.2.2/CHANGES` & `littletable-2.2.3/CHANGES`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,41 @@
 Change History
 ==============
 
-NOTE: Deprecated features will be removed in the 3.0 release of littletable:
-- DataObject class, replace with typing.SimpleNamespace, dict, namedtuple, or
+NOTE: Deprecated features will be removed in the 3.0 release of `littletable`:
+- `DataObject` class, replace with `typing.SimpleNamespace`, `dict`, `namedtuple`, or
   other user-defined class
-- Table.re_match(patt) comparator is deprecated, replace with
-  re.compile(patt).match
+- `Table.re_match(patt)` comparator is deprecated, replace with
+  `re.compile(patt).match`
+
+
+Version 2.2.3
+-------------
+- Fixed bug when calling `add_field` on an existing field that has been indexed, that
+  the index on that field would not reflect the new values.
+
+- Added support for optional named arguments to `csv_import`,
+  `tsv_import`, `json_import`, and `excel_import` methods when the import
+  source is an HTTP or HTTPS URL:
+  - `headers`: dict to be used as request headers
+  - `body`: bytes for request body
+  - `username`: str to be added for basic authentication
+  - `password`: str to be added for basic authentication (default='')
+  - `context`: SSL Context passed to urlopen (see the urlopen docs at
+    https://docs.python.org/3/library/urllib.request.html#urllib.request.urlopen);
+    `capath` and `cafile` may be used instead, but use of these arguments is
+    deprecated and so discouraged
+
+- Added `Table.as_dataframe()` method to make a pandas `DataFrame` from a
+  `littletable.Table`, and example `table_to_dataframe.py`.
+
 
 Version 2.2.2
 -------------
-- Fixed bug using datetime.UTC (only available under Python 3.11 - sorry!)
+- Fixed bug using `datetime.UTC` (only available under Python 3.11 - sorry!)
 
 
 Version 2.2.1
 -------------
 - Rewrote handling of multiple custom `JSONEncoder`s to use multiple
   inheritance instead of explicit call chaining.
```

### Comparing `littletable-2.2.2/LICENSE` & `littletable-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `littletable-2.2.2/PKG-INFO` & `littletable-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: littletable
-Version: 2.2.2
+Version: 2.2.3
 Summary: Python in-memory ORM database
 Home-page: https://github.com/ptmcg/littletable/
 Author: Paul McGuire
 Author-email: ptmcg@austin.rr.com
 License: MIT License
 Download-URL: https://pypi.org/project/littletable/
 Platform: UNKNOWN
```

### Comparing `littletable-2.2.2/README.md` & `littletable-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `littletable-2.2.2/littletable.egg-info/PKG-INFO` & `littletable-2.2.3/littletable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: littletable
-Version: 2.2.2
+Version: 2.2.3
 Summary: Python in-memory ORM database
 Home-page: https://github.com/ptmcg/littletable/
 Author: Paul McGuire
 Author-email: ptmcg@austin.rr.com
 License: MIT License
 Download-URL: https://pypi.org/project/littletable/
 Platform: UNKNOWN
```

### Comparing `littletable-2.2.2/littletable.py` & `littletable-2.2.3/littletable.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,15 @@
         print(item)
 
     # list all wishlist items in descending order by price
     for item in wishlists().sort("unitprice desc"):
         print(item)
 """
 
+import base64
 import copy
 import csv
 import datetime
 import functools
 import io
 import itertools
 import textwrap
@@ -153,22 +154,22 @@
     import rich
     from rich import box
 except ImportError:
     rich = None
     box = None
 
 version_info = namedtuple("version_info", "major minor micro release_level serial")
-__version_info__ = version_info(2, 2, 2, "final", 0)
+__version_info__ = version_info(2, 2, 3, "final", 0)
 __version__ = (
     "{}.{}.{}".format(*__version_info__[:3])
     + (f"{__version_info__.release_level[0]}{__version_info__.serial}", "")[
         __version_info__.release_level == "final"
     ]
 )
-__version_time__ = "28 May 2023 19:19 UTC"
+__version_time__ = "12 Jun 2023 02:47 UTC"
 __author__ = "Paul McGuire <ptmcg@austin.rr.com>"
 
 
 # custom Exception classes
 class SearchIndexInconsistentError(Exception):
     """
     Exception raised when using search method on table that has been
@@ -196,14 +197,44 @@
 
 class ReadonlyIndexAccessError(Exception):
     """
     Exception raised when trying to write to a readonly index.
     """
 
 
+class AuthenticationWarning(Warning):
+    """
+    Warning emitted when using authentication credentials with http:// URL.
+    """
+    def __str__(self):
+        return (
+            "Using Basic Authentication over HTTP can expose login credentials; HTTPS is recommended"
+        )
+
+
+def _emit_warning_with_user_frame(warning_message):
+    import warnings, sys
+    try:
+        cur = sys._getframe()
+    except AttributeError:
+        user_stack_level = 2
+    else:
+        # walk stack trace until outside of this module
+        user_stack_level = 0
+        while cur:
+            user_stack_level += 1
+            if cur.f_code.co_filename != __file__:
+                break
+            cur = cur.f_back
+        else:
+            user_stack_level = 2
+
+    warnings.warn(warning_message, stacklevel=user_stack_level)
+
+
 NL = os.linesep
 
 default_row_class = SimpleNamespace
 
 _numeric_type: tuple[type, ...] = (int, float)
 right_justify_types: tuple[type, ...] = (int, float, datetime.timedelta)
 
@@ -218,14 +249,15 @@
     import openpyxl
 except ImportError:
     openpyxl = None
 
 PredicateFunction = Callable[[Any], bool]
 
 __all__ = [
+    "AuthenticationWarning",
     "DataObject",
     "FixedWidthReader",
     "Table",
     "csv_import",
     "tsv_import",
     "json_import",
     "excel_import",
@@ -474,15 +506,15 @@
         else:
             try:
                 self.none_values.remove(obj)
             except ValueError:
                 pass
 
     def _clear(self):
-        self.obs.clear()
+        super()._clear()
         del self.none_values[:]
 
 
 class _ObjIndexWrapper:
     def __init__(self, ind, table):
         self._index = ind
         self._table: Table = table
@@ -711,50 +743,86 @@
     - a str URL (denoted by a leading "http")
     - a str file name (containing the data, or a compressed
       file containing data)
     - a path to a file
     - any iterable
     """
 
-    def __init__(self, seqobj: _ImportExportDataContainer, encoding: str = "utf-8"):
+    def __init__(
+            self,
+            seqobj: _ImportExportDataContainer,
+            encoding: str = "utf-8",
+            url_args: dict = None,
+    ):
         def _decoder(seq):
             for line in seq:
                 yield line.decode(encoding)
 
         self.type = None
         if isinstance(seqobj, Path):
             seqobj = str(seqobj)
             self.type = ImportSourceType.path
 
         self._iterobj: Iterable[str]
+        self._closeobj = None
 
         if isinstance(seqobj, str):
             if "\n" in seqobj:
                 self._iterobj = iter(StringIO(seqobj))
                 self.type = ImportSourceType.string
             elif seqobj.startswith(("http://", "https://")):
-                self._iterobj = _decoder(urllib.request.urlopen(seqobj))
+                url_args = url_args or {}
+                urlopen_args = {}
+
+                if not isinstance(url_args.get("data", b""), bytes):
+                    raise TypeError("'data' must be of type bytes")
+
+                if "username" in url_args:
+                    if seqobj.startswith("http://"):
+                        _emit_warning_with_user_frame(AuthenticationWarning())
+
+                    creds = f"{url_args.pop('username')}:{url_args.pop('password', '')}"
+                    auth = base64.b64encode(creds.encode('utf-8')).decode('utf-8')
+
+                    # Create the auth request header, and add to url_args["headers"]
+                    auth_header = {'Authorization': f'Basic {auth}'}
+                    url_args["headers"] = {
+                        **url_args.get("headers", {}),
+                        **auth_header,
+                    }
+
+                    # extract any SSL-related args
+                    urlopen_args = {
+                        k: url_args.pop(k, None)
+                        for k in "cafile capath context".split()
+                    }
+
+                data_request = urllib.request.Request(url=seqobj, **url_args)
+                self._closeobj = urllib.request.urlopen(data_request, **urlopen_args)
+                self._iterobj = _decoder(self._closeobj)
                 self.type = ImportSourceType.url
             else:
                 if seqobj.endswith(".gz"):
                     import gzip
 
-                    self._iterobj = _decoder(gzip.GzipFile(filename=seqobj))
+                    self._closeobj = gzip.GzipFile(filename=seqobj)
+                    self._iterobj = _decoder(self._closeobj)
                     self.type = ImportSourceType.gzip
                 elif seqobj.endswith((".xz", ".lzma")):
                     import lzma
 
                     self._iterobj = lzma.open(seqobj, "rt", encoding=encoding)
                     self.type = ImportSourceType.lzma
                 elif seqobj.endswith(".zip"):
                     import zipfile
 
                     # assume file name inside zip is the same as the zip file without the trailing ".zip"
                     inner_name = Path(seqobj).stem
-                    self._iterobj = _decoder(zipfile.ZipFile(seqobj).open(inner_name))
+                    self._closeobj = zipfile.ZipFile(seqobj).open(inner_name)
+                    self._iterobj = _decoder(self._closeobj)
                     self.type = ImportSourceType.zip
                 elif seqobj.endswith(".xlsx") or seqobj.endswith("xlsm"):
                     self._iterobj = open(seqobj, 'rb')
                     if self.type is None:
                         self.type = ImportSourceType.file
                 else:
                     self._iterobj = open(seqobj, encoding=encoding)
@@ -769,14 +837,16 @@
 
     def __next__(self):
         return next(self._iterobj)
 
     def close(self):
         if hasattr(self._iterobj, "close"):
             self._iterobj.close()
+        if self._closeobj is not None:
+            self._closeobj.close()
 
 
 FixedWidthParseSpec = Union[
     tuple[str, int],
     tuple[str, int, Optional[int]],
     tuple[str, int, Optional[int], Optional[Callable[[str], Any]]],
 ]
@@ -1391,15 +1461,15 @@
 
     def get_index(self, attr: str):
         return _ReadonlyObjIndexWrapper(self._indexes[attr], self.copy_template())
 
     NON_WORD_STRIPPER_RE = re.compile(r"[^\w_]?([\w._-]*)[^\w.]*")
     NON_WORD_STRIPPER2_RE = re.compile(r"[^\w_-]?((?:\w|[-_]\w)+)(!>_-)$")
     ACRONYM_WITH_PERIODS = re.compile(r"((?:\w\.){2,})(!>\.)$")
-    SIGNIFICANT_WORD_ENDING_RE = re.compile(rf".*({'|'.join(_significant_word_endings)})$")
+    SIGNIFICANT_WORD_ENDING_RE = re.compile(rf"[a-z]{{2,}}({'|'.join(_significant_word_endings)})$")
 
     PLURAL_ENDING_IN_IES = re.compile(r"(.*[^aeiouy])ies$")
     PLURAL_ENDING_IN_ES = re.compile(r"(.*(?:ch|ss|sh|x))es$")
     PLURAL_ENDING_IN_ES2 = re.compile(r"(.*(?:[bcdfghklmnprstuvwxz]|(qu))e)s$")
     PLURAL_ENDING_IN_S = re.compile(r"(.*[^aeious])s$")
     SINGULAR_ENDING_IN_S = re.compile(r"(.*(?:ness|ics))$")
 
@@ -1452,16 +1522,18 @@
                             s)
 
             if sing and sing != s:
                 yield sing
             yield s
 
             # # also add special ending words for code and documentation parsing
-            if s.endswith(_significant_word_endings):
-                yield Table.SIGNIFICANT_WORD_ENDING_RE.match(s)[1]
+            if (s.endswith(_significant_word_endings) and
+                (m := Table.SIGNIFICANT_WORD_ENDING_RE.match(s))
+            ):
+                yield m[1]
 
             return
 
         match_res = [
             # an acronym of 2 or more "X." sequences, such as G.E. or I.B.M.
             Table.ACRONYM_WITH_PERIODS,
             # words that may be hyphenated or snake-case
@@ -1614,14 +1686,17 @@
                 for kwd in self._normalize_word_gen(keyword[1:], stopwords):
                     plus_matches.pop(kwd, None)
                     if kwd not in minus_matches and kwd not in excl_matches:
                         minus_matches[kwd] = set(search_index.get(kwd, []))
 
             else:
                 for kwd in self._normalize_word_gen(keyword, stopwords):
+                    if m := Table.SIGNIFICANT_WORD_ENDING_RE.match(keyword):
+                        if kwd == m[1]:
+                            continue
                     if kwd in plus_matches or kwd in minus_matches:
                         continue
                     opt_matches[kwd] = set(search_index.get(kwd, []))
 
         # process word groups to determine correct set of reqd_matches
         if reqd_words:
             reqd_matches = set(range(len(self.obs)))
@@ -2008,14 +2083,17 @@
     def select(self, fields: Union[Iterable[str], str] = None, **exprs) -> "Table":
         """
         Create a new table containing a subset of attributes, with optionally
         newly-added fields computed from each rec in the original table.
 
         @param fields: list of strings, or single space-delimited string, listing attribute name to be included in the
         output
+         - names starting with '-' indicate to suppress that field
+         - '*' means include all other field names
+         - if no fields are specifically included, then all fields are used
         @type fields: list, or space-delimited string
         @param exprs: one or more named callable arguments, to compute additional fields using the given function
         @type exprs: C{name=callable}, callable takes the record as an argument, and returns the new attribute value
         If a string is passed as a callable, this string will be used using string formatting, given the record
         as a source of interpolation values.  For instance, C{fullName = '%(lastName)s, %(firstName)s'}
 
         """
@@ -2480,20 +2558,21 @@
         source: _ImportExportDataContainer,
         encoding: str = "utf-8",
         transforms: Optional[dict] = None,
         filters: Optional[dict] = None,
         reader=csv.DictReader,
         row_class: type = None,
         limit: int = None,
+        url_args: dict = None,
     ):
 
         if row_class is None:
             row_class = default_row_class
 
-        with closing(_MultiIterator(source, encoding)) as _srciter:
+        with closing(_MultiIterator(source, encoding, url_args)) as _srciter:
             csvdata = reader(_srciter)
 
             if transforms:
                 transformers = []
                 for k, v in transforms.items():
                     if isinstance(v, tuple):
                         v, default = v
@@ -2609,56 +2688,64 @@
             input files, to pre-screen only for data matching one or more filters
         @type filters: dict (optional)
         @param row_class: class to construct for each imported row when populating table (default=SimpleNamespace)
         @type row_class: type
         @param limit: number of records to import
         @type limit: int (optional)
         @param kwargs: additional constructor arguments for csv C{DictReader} objects, such as C{delimiter}
-            or C{fieldnames}; these are passed directly through to the csv C{DictReader} constructor
+            or C{fieldnames}; these are passed directly through to the csv C{DictReader} constructor. kwargs
+            may also contain any of the following if importing using a URL: C{headers}, C{data}, C{username},
+            C{password}
         @type kwargs: named arguments (optional)
         @param fieldnames: names for imported columns; used if there is no header line in the input file
         @type fieldnames: list[str] or str
         """
-        non_reader_args = "encoding csv_source transforms row_class limit".split()
+        non_reader_args = "encoding csv_source transforms row_class limit headers data username password cafile capath context".split()
+        url_arg_names = "headers data username password cafile capath context".split()
+        url_args = {k: kwargs.pop(k) for k in url_arg_names if k in kwargs}
         reader_args = {
             k: v for k, v in kwargs.items() if k not in non_reader_args
         }
         reader_args["fieldnames"] = fieldnames.split() if isinstance(fieldnames, str) else fieldnames
         return self._import(
             csv_source,
             encoding=encoding,
             transforms=transforms,
             filters=filters,
             reader=lambda src: csv.DictReader(src, **reader_args),
             row_class=row_class,
             limit=limit,
+            url_args=url_args,
         )
 
     def _xsv_import(
         self,
         xsv_source: _ImportExportDataContainer,
         encoding: str = "utf-8",
         transforms: dict = None,
         filters: dict = None,
         row_class: type = None,
         limit: int = None,
         **kwargs,
     ):
-        non_reader_args = "encoding xsv_source transforms row_class limit filters".split()
+        non_reader_args = "encoding xsv_source transforms row_class limit filters headers data username password cafile capath context".split()
+        url_arg_names = "headers data username password cafile capath context".split()
+        url_args = {k: kwargs.pop(k) for k in url_arg_names if k in kwargs}
         reader_args = {
             k: v for k, v in kwargs.items() if k not in non_reader_args
         }
         return self._import(
             xsv_source,
             encoding=encoding,
             transforms=transforms,
             filters=filters,
             reader=lambda src: csv.DictReader(src, **reader_args),
             row_class=row_class,
             limit=limit,
+            url_args=url_args,
         )
 
     def tsv_import(
         self,
         xsv_source: _ImportExportDataContainer,
         encoding: str = "utf-8",
         transforms: dict = None,
@@ -2723,21 +2810,25 @@
                 # check whether to include or omit the header
                 header = (reader_args.get("fieldnames")
                           or [str(cell.value) for cell in next(rows_iter)])
 
                 for row in rows_iter:
                     yield {key: cell.value for key, cell in zip(header, row)}
 
+        url_arg_names = "headers data username password cafile capath context".split()
+        url_args = {k: kwargs.pop(k) for k in url_arg_names if k in kwargs}
+
         return self._import(
             excel_source,
             transforms=transforms,
             filters=filters,
             reader=lambda src: excel_as_dict(src._iterobj, **kwargs),
             row_class=row_class,
             limit=limit,
+            url_args=url_args,
         )
 
     def excel_import(
         self,
         excel_source: _ImportExportDataContainer,
         transforms: dict = None,
         filters: dict = None,
@@ -2766,26 +2857,30 @@
             input files, to pre-screen only for data matching one or more filters
         @type filters: dict (optional)
         @param row_class: class to construct for each imported row when populating table (default=SimpleNamespace)
         @type row_class: type
         @param limit: number of records to import
         @type limit: int (optional)
         @param kwargs: additional arguments for the excel reader. Only available argument is "sheet" to select which
-            sheet to read (defaults to active sheet)
+            sheet to read (defaults to active sheet). kwargs may also contain any of the following if importing
+            using a URL: C{headers}, C{data}, C{username}, C{password}
         @type kwargs: named arguments (optional)
         @param fieldnames: names for imported columns; used if there is no header line in the input file
         @type fieldnames: list[str] or str
         """
         kwargs["fieldnames"] = fieldnames.split() if isinstance(fieldnames, str) else fieldnames
+        url_arg_names = "headers data username password".split()
+        url_args = {k: kwargs.pop(k) for k in url_arg_names if k in kwargs}
         return self._excel_import(
             excel_source,
             transforms=transforms,
             filters=filters,
             row_class=row_class,
             limit=limit,
+            url_args=url_args,
             **kwargs,
         )
 
     def csv_export(
         self,
         csv_dest: _ImportExportDataContainer = None,
         fieldnames: Iterable[str] = None,
@@ -2875,14 +2970,15 @@
         source: _ImportExportDataContainer,
         encoding: str = "UTF-8",
         transforms: dict = None,
         row_class: type = None,
         streaming: bool = False,
         path: str = "",
         json_decoder: json.JSONDecoder = None,
+        **kwargs,
     ) -> "Table":
         """
         Imports the contents of a JSON data file into this table.
         @param source: JSON data file - if a string is given, the file with that name will be
             opened, read, and closed; if a file object is given, then that object
             will be read as-is, and left for the caller to be closed.
         @type source: string or file
@@ -2946,20 +3042,25 @@
                     yield from obs
 
         if path and streaming:
             raise ValueError("cannot specify path and streaming=True")
 
         if row_class is None:
             row_class = default_row_class
+
+        url_arg_names = "headers data username password cafile capath context".split()
+        url_args = {k: kwargs.pop(k) for k in url_arg_names if k in kwargs}
+
         return self._import(
             source,
             encoding,
             transforms=transforms,
             reader=_JsonFileReader,
             row_class=row_class,
+            url_args=url_args,
         )
 
     def json_export(
         self,
         dest: Optional[_ImportExportDataContainer] = None,
         fieldnames: Union[Iterable[str], str] = None,
         encoding: str = "UTF-8",
@@ -3093,14 +3194,47 @@
             fieldnames = fieldnames.split()
         ws.append(fieldnames)
         # append data
         for o in self.obs:
             ws.append([v for v in _to_dict(o).values()])
         wb.save(excel_dest)
 
+    def as_dataframe(self, fields=None):
+        """
+        Export contents of the Table to a pandas DataFrame.
+        @param fields: list of strings, or single space-delimited string, listing
+        attribute name to be included in the output
+         - names starting with '-' indicate to suppress that field
+         - '*' means include all other field names
+         - if no fields are specifically included, then all fields are used
+        @type fields: list, or space-delimited string
+        """
+        try:
+            import pandas as pd
+        except ImportError:
+            print("pandas not installed", file=sys.stderr)
+            return None
+
+        if fields is None:
+            # assume all fields
+            fieldnames = self._attr_names()
+        else:
+            fieldnames = self._parse_fields_string(fields)
+
+        # operator.attrgetter is an efficient extractor of values from objects
+        extractor = operator.attrgetter(*fieldnames)
+
+        # build a DataFrame from the tuples returned by the extractor for
+        # each object in this Table
+        ret = pd.DataFrame(
+            map(extractor, self),
+            columns=fieldnames,
+        )
+        return ret
+
     def add_field(
         self, attrname: str, fn: Callable[[Any], Any], default: Any = None
     ) -> "Table":
         """
         Computes a new attribute for each object in table, or replaces an
         existing attribute in each record with a computed value
         @param attrname: attribute to compute for each object
@@ -3110,25 +3244,35 @@
 
             lambda ob : ob.commission_pct/100.0 * ob.gross_sales
 
         @type fn: function(obj) returns value
         @param default: value to use if an exception is raised while trying
         to evaluate fn
         """
+        if attrname in self._indexes:
+            idx = self._indexes[attrname]
+            idx._clear()
+            idx_setitem = idx.__setitem__
+        else:
+            # there is no index for this attr
+            idx_setitem = None
 
         try:
             for rec_ in self:
                 try:
                     val = fn(rec_)
                 except Exception:
                     val = default
                 if isinstance(rec_, DataObject):
                     rec_.__dict__[attrname] = val
                 else:
                     setattr(rec_, attrname, val)
+                # update index for this attribute, if there is one
+                if idx_setitem is not None:
+                    idx_setitem(val, rec_)
         except AttributeError:
             raise AttributeError(
                 f"cannot add/modify attribute {attrname!r} in table records"
             )
 
         self._contents_changed(invalidate_search_indexes=False)
         return self
```

### Comparing `littletable-2.2.2/setup.py` & `littletable-2.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `littletable-2.2.2/unit_tests.py` & `littletable-2.2.3/unit_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,6891 +34,7119 @@
 00000210: 2c20 6669 6c65 3d4e 6f6e 6529 3a0a 2020  , file=None):.  
 00000220: 2020 696d 706f 7274 2064 6174 6574 696d    import datetim
 00000230: 650a 0a20 2020 2072 6574 203d 2053 696d  e..    ret = Sim
 00000240: 706c 654e 616d 6573 7061 6365 2829 0a20  pleNamespace(). 
 00000250: 2020 2072 6574 2e73 7461 7274 203d 2064     ret.start = d
 00000260: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
 00000270: 2e6e 6f77 2829 2e61 7374 696d 657a 6f6e  .now().astimezon
-00000280: 6528 6461 7465 7469 6d65 2e55 5443 290a  e(datetime.UTC).
-00000290: 2020 2020 6966 206c 6162 656c 3a0a 2020      if label:.  
-000002a0: 2020 2020 2020 7072 696e 7428 6622 5374        print(f"St
-000002b0: 6172 7420 2d20 7b6c 6162 656c 7d3a 207b  art - {label}: {
-000002c0: 7265 742e 7374 6172 747d 222c 2066 696c  ret.start}", fil
-000002d0: 653d 6669 6c65 290a 2020 2020 7969 656c  e=file).    yiel
-000002e0: 6420 7265 740a 2020 2020 7265 742e 656e  d ret.    ret.en
-000002f0: 6420 3d20 6461 7465 7469 6d65 2e64 6174  d = datetime.dat
-00000300: 6574 696d 652e 6e6f 7728 292e 6173 7469  etime.now().asti
-00000310: 6d65 7a6f 6e65 2864 6174 6574 696d 652e  mezone(datetime.
-00000320: 5554 4329 0a20 2020 2072 6574 2e65 6c61  UTC).    ret.ela
-00000330: 7073 6564 203d 2072 6574 2e65 6e64 202d  psed = ret.end -
-00000340: 2072 6574 2e73 7461 7274 0a20 2020 2069   ret.start.    i
-00000350: 6620 6c61 6265 6c3a 0a20 2020 2020 2020  f label:.       
-00000360: 2070 7269 6e74 2866 2245 6e64 2020 202d   print(f"End   -
-00000370: 207b 6c61 6265 6c7d 3a20 7b72 6574 2e65   {label}: {ret.e
-00000380: 6e64 7d22 2c20 6669 6c65 3d66 696c 6529  nd}", file=file)
-00000390: 0a0a 0a69 6d70 6f72 7420 6461 7461 636c  ...import datacl
-000003a0: 6173 7365 730a 4064 6174 6163 6c61 7373  asses.@dataclass
-000003b0: 6573 2e64 6174 6163 6c61 7373 0a63 6c61  es.dataclass.cla
-000003c0: 7373 2044 6174 6144 6174 6163 6c61 7373  ss DataDataclass
-000003d0: 3a0a 2020 2020 613a 2069 6e74 0a20 2020  :.    a: int.   
-000003e0: 2062 3a20 696e 740a 2020 2020 633a 2069   b: int.    c: i
-000003f0: 6e74 0a0a 7472 793a 0a20 2020 2069 6d70  nt..try:.    imp
-00000400: 6f72 7420 7079 6461 6e74 6963 0a65 7863  ort pydantic.exc
-00000410: 6570 7420 496d 706f 7274 4572 726f 723a  ept ImportError:
-00000420: 0a20 2020 2070 7269 6e74 2822 7079 6461  .    print("pyda
-00000430: 6e74 6963 2074 6573 7473 2064 6973 6162  ntic tests disab
-00000440: 6c65 6422 290a 2020 2020 7079 6461 6e74  led").    pydant
-00000450: 6963 203d 204e 6f6e 650a 656c 7365 3a0a  ic = None.else:.
-00000460: 2020 2020 636c 6173 7320 4461 7461 5079      class DataPy
-00000470: 6461 6e74 6963 4d6f 6465 6c28 7079 6461  danticModel(pyda
-00000480: 6e74 6963 2e42 6173 654d 6f64 656c 293a  ntic.BaseModel):
-00000490: 0a20 2020 2020 2020 2061 3a20 4f70 7469  .        a: Opti
-000004a0: 6f6e 616c 5b55 6e69 6f6e 5b69 6e74 2c20  onal[Union[int, 
-000004b0: 7374 725d 5d0a 2020 2020 2020 2020 623a  str]].        b:
-000004c0: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
-000004d0: 696e 742c 2073 7472 5d5d 0a20 2020 2020  int, str]].     
-000004e0: 2020 2063 3a20 4f70 7469 6f6e 616c 5b55     c: Optional[U
-000004f0: 6e69 6f6e 5b69 6e74 2c20 7374 725d 5d0a  nion[int, str]].
-00000500: 0a20 2020 2063 6c61 7373 2044 6174 6150  .    class DataP
-00000510: 7964 616e 7469 6349 6d6d 7574 6162 6c65  ydanticImmutable
-00000520: 4d6f 6465 6c28 7079 6461 6e74 6963 2e42  Model(pydantic.B
-00000530: 6173 654d 6f64 656c 293a 0a20 2020 2020  aseModel):.     
-00000540: 2020 2063 6c61 7373 2043 6f6e 6669 673a     class Config:
-00000550: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
-00000560: 6f77 5f6d 7574 6174 696f 6e20 3d20 4661  ow_mutation = Fa
-00000570: 6c73 650a 0a20 2020 2020 2020 2061 3a20  lse..        a: 
-00000580: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b69  Optional[Union[i
-00000590: 6e74 2c20 7374 725d 5d0a 2020 2020 2020  nt, str]].      
-000005a0: 2020 623a 204f 7074 696f 6e61 6c5b 556e    b: Optional[Un
-000005b0: 696f 6e5b 696e 742c 2073 7472 5d5d 0a20  ion[int, str]]. 
-000005c0: 2020 2020 2020 2063 3a20 4f70 7469 6f6e         c: Option
-000005d0: 616c 5b55 6e69 6f6e 5b69 6e74 2c20 7374  al[Union[int, st
-000005e0: 725d 5d0a 0a20 2020 2063 6c61 7373 2044  r]]..    class D
-000005f0: 6174 6150 7964 616e 7469 634f 524d 4d6f  ataPydanticORMMo
-00000600: 6465 6c28 7079 6461 6e74 6963 2e42 6173  del(pydantic.Bas
-00000610: 654d 6f64 656c 293a 0a20 2020 2020 2020  eModel):.       
-00000620: 2063 6c61 7373 2043 6f6e 6669 673a 0a20   class Config:. 
-00000630: 2020 2020 2020 2020 2020 206f 726d 5f6d             orm_m
-00000640: 6f64 6520 3d20 5472 7565 0a0a 2020 2020  ode = True..    
-00000650: 2020 2020 613a 204f 7074 696f 6e61 6c5b      a: Optional[
-00000660: 556e 696f 6e5b 696e 742c 2073 7472 5d5d  Union[int, str]]
-00000670: 0a20 2020 2020 2020 2062 3a20 4f70 7469  .        b: Opti
-00000680: 6f6e 616c 5b55 6e69 6f6e 5b69 6e74 2c20  onal[Union[int, 
-00000690: 7374 725d 5d0a 2020 2020 2020 2020 633a  str]].        c:
-000006a0: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
-000006b0: 696e 742c 2073 7472 5d5d 0a0a 7472 793a  int, str]]..try:
-000006c0: 0a20 2020 2069 6d70 6f72 7420 6174 7472  .    import attr
-000006d0: 0a65 7863 6570 7420 496d 706f 7274 4572  .except ImportEr
-000006e0: 726f 723a 0a20 2020 2070 7269 6e74 2822  ror:.    print("
-000006f0: 6174 7472 7320 7465 7374 7320 6469 7361  attrs tests disa
-00000700: 626c 6564 2229 0a20 2020 2061 7474 7220  bled").    attr 
-00000710: 3d20 4e6f 6e65 0a65 6c73 653a 0a20 2020  = None.else:.   
-00000720: 2041 7474 7243 6c61 7373 203d 2061 7474   AttrClass = att
-00000730: 722e 6d61 6b65 5f63 6c61 7373 2822 4174  r.make_class("At
-00000740: 7472 436c 6173 7322 2c20 5b22 6122 2c20  trClass", ["a", 
-00000750: 2262 222c 2022 6322 5d29 0a0a 7472 793a  "b", "c"])..try:
-00000760: 0a20 2020 2069 6d70 6f72 7420 7472 6169  .    import trai
-00000770: 746c 6574 730a 6578 6365 7074 2049 6d70  tlets.except Imp
-00000780: 6f72 7445 7272 6f72 3a0a 2020 2020 7072  ortError:.    pr
-00000790: 696e 7428 2274 7261 6974 6c65 7473 2074  int("traitlets t
-000007a0: 6573 7473 2064 6973 6162 6c65 6422 290a  ests disabled").
-000007b0: 2020 2020 7472 6169 746c 6574 7320 3d20      traitlets = 
-000007c0: 4e6f 6e65 0a65 6c73 653a 0a20 2020 2063  None.else:.    c
-000007d0: 6c61 7373 2054 7261 6974 6c65 7473 436c  lass TraitletsCl
-000007e0: 6173 7328 6c74 2e48 6173 5472 6169 7473  ass(lt.HasTraits
-000007f0: 4d69 7869 6e2c 2074 7261 6974 6c65 7473  Mixin, traitlets
-00000800: 2e48 6173 5472 6169 7473 293a 0a20 2020  .HasTraits):.   
-00000810: 2020 2020 2061 203d 2074 7261 6974 6c65       a = traitle
-00000820: 7473 2e55 6e69 6f6e 285b 7472 6169 746c  ts.Union([traitl
-00000830: 6574 732e 496e 7428 292c 2074 7261 6974  ets.Int(), trait
-00000840: 6c65 7473 2e55 6e69 636f 6465 2829 5d2c  lets.Unicode()],
-00000850: 2061 6c6c 6f77 5f6e 6f6e 653d 5472 7565   allow_none=True
-00000860: 290a 2020 2020 2020 2020 6220 3d20 7472  ).        b = tr
-00000870: 6169 746c 6574 732e 556e 696f 6e28 5b74  aitlets.Union([t
-00000880: 7261 6974 6c65 7473 2e49 6e74 2829 2c20  raitlets.Int(), 
-00000890: 7472 6169 746c 6574 732e 556e 6963 6f64  traitlets.Unicod
-000008a0: 6528 295d 2c20 616c 6c6f 775f 6e6f 6e65  e()], allow_none
-000008b0: 3d54 7275 6529 0a20 2020 2020 2020 2063  =True).        c
-000008c0: 203d 2074 7261 6974 6c65 7473 2e55 6e69   = traitlets.Uni
-000008d0: 6f6e 285b 7472 6169 746c 6574 732e 496e  on([traitlets.In
-000008e0: 7428 292c 2074 7261 6974 6c65 7473 2e55  t(), traitlets.U
-000008f0: 6e69 636f 6465 2829 5d2c 2061 6c6c 6f77  nicode()], allow
-00000900: 5f6e 6f6e 653d 5472 7565 290a 0a20 2020  _none=True)..   
-00000910: 2020 2020 2064 6566 205f 5f69 6e69 745f       def __init_
-00000920: 5f28 7365 6c66 2c20 2a2a 6b77 6172 6773  _(self, **kwargs
-00000930: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00000940: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
-00000950: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-00000960: 7220 6b2c 2077 2069 6e20 6b77 6172 6773  r k, w in kwargs
-00000970: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00000980: 2020 2020 2020 2020 2020 7365 7461 7474            setatt
-00000990: 7228 7365 6c66 2c20 6b2c 2077 290a 0a20  r(self, k, w).. 
-000009a0: 2020 2020 2020 2064 6566 205f 5f72 6570         def __rep
-000009b0: 725f 5f28 7365 6c66 293a 0a20 2020 2020  r__(self):.     
-000009c0: 2020 2020 2020 2072 6574 7572 6e20 6622         return f"
-000009d0: 7b74 7970 6528 7365 6c66 292e 5f5f 6e61  {type(self).__na
-000009e0: 6d65 5f5f 7d3a 2861 3d7b 7365 6c66 2e61  me__}:(a={self.a
-000009f0: 7d2c 2062 3d7b 7365 6c66 2e62 7d2c 2063  }, b={self.b}, c
-00000a00: 3d7b 7365 6c66 2e63 7d29 220a 0a20 2020  ={self.c})"..   
-00000a10: 2020 2020 2064 6566 205f 5f64 6972 5f5f       def __dir__
-00000a20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00000a30: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00000a40: 7472 6169 745f 6e61 6d65 7328 290a 0a44  trait_names()..D
-00000a50: 6174 6154 7570 6c65 203d 206e 616d 6564  ataTuple = named
-00000a60: 7475 706c 6528 2244 6174 6154 7570 6c65  tuple("DataTuple
-00000a70: 222c 2022 6120 6220 6322 290a 0a0a 636c  ", "a b c")...cl
-00000a80: 6173 7320 5479 7069 6e67 4e61 6d65 6454  ass TypingNamedT
-00000a90: 7570 6c65 2874 7970 696e 672e 4e61 6d65  uple(typing.Name
-00000aa0: 6454 7570 6c65 293a 0a20 2020 2061 3a20  dTuple):.    a: 
-00000ab0: 696e 740a 2020 2020 623a 2069 6e74 0a20  int.    b: int. 
-00000ac0: 2020 2063 3a20 696e 740a 0a0a 2320 6966     c: int...# if
-00000ad0: 2072 6963 6820 6973 206e 6f74 2069 6e73   rich is not ins
-00000ae0: 7461 6c6c 6564 2c20 6469 7361 626c 6520  talled, disable 
-00000af0: 7461 626c 652e 7072 6573 656e 7428 2920  table.present() 
-00000b00: 6361 6c6c 730a 7472 793a 0a20 2020 2069  calls.try:.    i
-00000b10: 6d70 6f72 7420 7269 6368 0a65 7863 6570  mport rich.excep
-00000b20: 7420 496d 706f 7274 4572 726f 723a 0a20  t ImportError:. 
-00000b30: 2020 2072 6963 6820 3d20 4e6f 6e65 0a20     rich = None. 
-00000b40: 2020 2023 2064 6973 6162 6c65 2070 7265     # disable pre
-00000b50: 7365 6e74 2829 206d 6574 686f 642c 2073  sent() method, s
-00000b60: 696e 6365 2072 6963 6820 6973 206e 6f74  ince rich is not
-00000b70: 2061 7661 696c 6162 6c65 0a20 2020 206c   available.    l
-00000b80: 742e 5461 626c 652e 7072 6573 656e 7420  t.Table.present 
-00000b90: 3d20 6c61 6d62 6461 202a 6172 6773 2c20  = lambda *args, 
-00000ba0: 2a2a 6b77 6172 6773 3a20 4e6f 6e65 0a0a  **kwargs: None..
-00000bb0: 0a63 6c61 7373 2053 6c6f 7474 6564 3a0a  .class Slotted:.
-00000bc0: 2020 2020 5f5f 736c 6f74 735f 5f20 3d20      __slots__ = 
-00000bd0: 5b27 6127 2c20 2762 272c 2027 6327 5d0a  ['a', 'b', 'c'].
-00000be0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00000bf0: 5f28 7365 6c66 2c20 612c 2062 2c20 6329  _(self, a, b, c)
-00000c00: 3a0a 2020 2020 2020 2020 7365 6c66 2e61  :.        self.a
-00000c10: 203d 2061 0a20 2020 2020 2020 2073 656c   = a.        sel
-00000c20: 662e 6220 3d20 620a 2020 2020 2020 2020  f.b = b.        
-00000c30: 7365 6c66 2e63 203d 2063 0a0a 2020 2020  self.c = c..    
-00000c40: 6465 6620 5f5f 6571 5f5f 2873 656c 662c  def __eq__(self,
-00000c50: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-00000c60: 2072 6574 7572 6e20 2869 7369 6e73 7461   return (isinsta
-00000c70: 6e63 6528 6f74 6865 722c 2053 6c6f 7474  nce(other, Slott
-00000c80: 6564 2920 616e 640a 2020 2020 2020 2020  ed) and.        
-00000c90: 2020 2020 2020 2020 616c 6c28 6765 7461          all(geta
-00000ca0: 7474 7228 7365 6c66 2c20 6174 7472 2920  ttr(self, attr) 
-00000cb0: 3d3d 2067 6574 6174 7472 286f 7468 6572  == getattr(other
-00000cc0: 2c20 6174 7472 2920 666f 7220 6174 7472  , attr) for attr
-00000cd0: 2069 6e20 7365 6c66 2e5f 5f73 6c6f 7473   in self.__slots
-00000ce0: 5f5f 2929 0a0a 2020 2020 6465 6620 5f5f  __))..    def __
-00000cf0: 7265 7072 5f5f 2873 656c 6629 3a0a 2020  repr__(self):.  
-00000d00: 2020 2020 2020 7265 7475 726e 2066 227b        return f"{
-00000d10: 7479 7065 2873 656c 6629 2e5f 5f6e 616d  type(self).__nam
-00000d20: 655f 5f7d 3a28 613d 7b73 656c 662e 617d  e__}:(a={self.a}
-00000d30: 2c20 623d 7b73 656c 662e 627d 2c20 633d  , b={self.b}, c=
-00000d40: 7b73 656c 662e 637d 2922 0a0a 0a63 6c61  {self.c})"...cla
-00000d50: 7373 2053 6c6f 7474 6564 5769 7468 4469  ss SlottedWithDi
-00000d60: 6374 3a0a 2020 2020 5f5f 736c 6f74 735f  ct:.    __slots_
-00000d70: 5f20 3d20 7b27 6127 3a20 2761 272c 2027  _ = {'a': 'a', '
-00000d80: 6227 3a20 2762 272c 2027 6327 3a20 2763  b': 'b', 'c': 'c
-00000d90: 277d 0a0a 2020 2020 6465 6620 5f5f 696e  '}..    def __in
-00000da0: 6974 5f5f 2873 656c 662c 2061 2c20 622c  it__(self, a, b,
-00000db0: 2063 293a 0a20 2020 2020 2020 2073 656c   c):.        sel
-00000dc0: 662e 6120 3d20 610a 2020 2020 2020 2020  f.a = a.        
-00000dd0: 7365 6c66 2e62 203d 2062 0a20 2020 2020  self.b = b.     
-00000de0: 2020 2073 656c 662e 6320 3d20 630a 0a20     self.c = c.. 
-00000df0: 2020 2064 6566 205f 5f65 715f 5f28 7365     def __eq__(se
-00000e00: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
-00000e10: 2020 2020 7265 7475 726e 2028 6973 696e      return (isin
-00000e20: 7374 616e 6365 286f 7468 6572 2c20 536c  stance(other, Sl
-00000e30: 6f74 7465 6457 6974 6844 6963 7429 2061  ottedWithDict) a
-00000e40: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
-00000e50: 2020 2061 6c6c 2867 6574 6174 7472 2873     all(getattr(s
-00000e60: 656c 662c 2061 7474 7229 203d 3d20 6765  elf, attr) == ge
-00000e70: 7461 7474 7228 6f74 6865 722c 2061 7474  tattr(other, att
-00000e80: 7229 2066 6f72 2061 7474 7220 696e 2073  r) for attr in s
-00000e90: 656c 662e 5f5f 736c 6f74 735f 5f29 290a  elf.__slots__)).
-00000ea0: 0a20 2020 2064 6566 205f 5f72 6570 725f  .    def __repr_
-00000eb0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-00000ec0: 2072 6574 7572 6e20 6622 7b74 7970 6528   return f"{type(
-00000ed0: 7365 6c66 292e 5f5f 6e61 6d65 5f5f 7d3a  self).__name__}:
-00000ee0: 2861 3d7b 7365 6c66 2e61 7d2c 2062 3d7b  (a={self.a}, b={
-00000ef0: 7365 6c66 2e62 7d2c 2063 3d7b 7365 6c66  self.b}, c={self
-00000f00: 2e63 7d29 220a 0a0a 636c 6173 7320 5479  .c})"...class Ty
-00000f10: 7069 6e67 5479 7065 6444 6963 7428 7479  pingTypedDict(ty
-00000f20: 7069 6e67 2e54 7970 6564 4469 6374 293a  ping.TypedDict):
-00000f30: 0a20 2020 2061 3a20 696e 740a 2020 2020  .    a: int.    
-00000f40: 623a 2069 6e74 0a20 2020 2063 3a20 696e  b: int.    c: in
-00000f50: 740a 0a0a 636c 6173 7320 5465 7374 4461  t...class TestDa
-00000f60: 7461 4f62 6a65 6374 7328 756e 6974 7465  taObjects(unitte
-00000f70: 7374 2e54 6573 7443 6173 6529 3a0a 2020  st.TestCase):.  
-00000f80: 2020 6465 6620 7465 7374 5f73 6574 5f61    def test_set_a
-00000f90: 7474 7269 6275 7465 7328 7365 6c66 293a  ttributes(self):
-00000fa0: 0a20 2020 2020 2020 206f 6220 3d20 6c74  .        ob = lt
-00000fb0: 2e44 6174 614f 626a 6563 7428 290a 2020  .DataObject().  
-00000fc0: 2020 2020 2020 6f62 2e7a 203d 2032 3030        ob.z = 200
-00000fd0: 0a20 2020 2020 2020 206f 622e 6120 3d20  .        ob.a = 
-00000fe0: 3130 300a 2020 2020 2020 2020 7769 7468  100.        with
-00000ff0: 2073 656c 662e 7375 6254 6573 7428 2274   self.subTest("t
-00001000: 6573 7420 4461 7461 4f62 6a65 6374 2061  est DataObject a
-00001010: 7474 7269 6275 7465 2073 6574 7469 6e67  ttribute setting
-00001020: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00001030: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00001040: 285b 2827 6127 2c20 3130 3029 2c20 2827  ([('a', 100), ('
-00001050: 7a27 2c20 3230 3029 5d2c 2073 6f72 7465  z', 200)], sorte
-00001060: 6428 6f62 2e5f 5f64 6963 745f 5f2e 6974  d(ob.__dict__.it
-00001070: 656d 7328 2929 290a 0a20 2020 2020 2020  ems()))..       
-00001080: 2023 2074 6573 7420 7365 6d69 2d69 6d6d   # test semi-imm
-00001090: 7574 6162 696c 6974 7920 2863 616e 2774  utability (can't
-000010a0: 206f 7665 7277 7269 7465 2065 7869 7374   overwrite exist
-000010b0: 696e 6720 6174 7472 6962 7574 6573 290a  ing attributes).
-000010c0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-000010d0: 662e 7375 6254 6573 7428 2274 6573 7420  f.subTest("test 
-000010e0: 4461 7461 4f62 6a65 6374 2077 7269 7465  DataObject write
-000010f0: 2d6f 6e63 6520 2873 656d 692d 696d 6d75  -once (semi-immu
-00001100: 7461 6269 6c69 7479 2922 293a 0a20 2020  tability)"):.   
-00001110: 2020 2020 2020 2020 2077 6974 6820 7365           with se
-00001120: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
-00001130: 4174 7472 6962 7574 6545 7272 6f72 293a  AttributeError):
-00001140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001150: 206f 622e 6120 3d20 3130 310a 0a20 2020   ob.a = 101..   
-00001160: 2020 2020 2023 2065 7175 616c 6974 7920       # equality 
-00001170: 7465 7374 730a 2020 2020 2020 2020 7769  tests.        wi
-00001180: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00001190: 2274 6573 7420 4461 7461 4f62 6a65 6374  "test DataObject
-000011a0: 2065 7175 616c 6974 7922 293a 0a20 2020   equality"):.   
-000011b0: 2020 2020 2020 2020 206f 6232 203d 206c           ob2 = l
-000011c0: 742e 4461 7461 4f62 6a65 6374 282a 2a7b  t.DataObject(**{
-000011d0: 2761 273a 2031 3030 2c20 277a 273a 2032  'a': 100, 'z': 2
-000011e0: 3030 7d29 0a20 2020 2020 2020 2020 2020  00}).           
-000011f0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00001200: 6c28 6f62 322c 206f 6229 0a0a 2020 2020  l(ob2, ob)..    
-00001210: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-00001220: 6254 6573 7428 2274 6573 7420 4461 7461  bTest("test Data
-00001230: 4f62 6a65 6374 2069 6e65 7175 616c 6974  Object inequalit
-00001240: 7922 293a 0a20 2020 2020 2020 2020 2020  y"):.           
-00001250: 206f 6232 2e62 203d 2027 626c 6168 270a   ob2.b = 'blah'.
-00001260: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001270: 2e61 7373 6572 744e 6f74 4571 7561 6c28  .assertNotEqual(
-00001280: 6f62 2c20 6f62 3229 0a0a 2020 2020 2020  ob, ob2)..      
-00001290: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-000012a0: 6573 7428 2274 6573 7420 4461 7461 4f62  est("test DataOb
-000012b0: 6a65 6374 2065 7175 616c 6974 7920 6166  ject equality af
-000012c0: 7465 7220 7570 6461 7465 7322 293a 0a20  ter updates"):. 
-000012d0: 2020 2020 2020 2020 2020 2064 656c 206f             del o
-000012e0: 6232 2e62 0a20 2020 2020 2020 2020 2020  b2.b.           
-000012f0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00001300: 6c28 6f62 322c 206f 6229 0a0a 2020 2020  l(ob2, ob)..    
-00001310: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-00001320: 6254 6573 7428 2274 6573 7420 4461 7461  bTest("test Data
-00001330: 4f62 6a65 6374 204b 6579 4572 726f 7222  Object KeyError"
-00001340: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
-00001350: 656c 206f 6232 2e61 0a20 2020 2020 2020  el ob2.a.       
-00001360: 2020 2020 2064 656c 206f 6232 2e7a 0a0a       del ob2.z..
-00001370: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00001380: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
-00001390: 6573 284b 6579 4572 726f 7229 3a0a 2020  es(KeyError):.  
-000013a0: 2020 2020 2020 2020 2020 2020 2020 6f62                ob
-000013b0: 325b 2761 275d 0a20 2020 2020 2020 2020  2['a'].         
-000013c0: 2020 206f 6232 5b27 6127 5d20 3d20 3130     ob2['a'] = 10
-000013d0: 0a20 2020 2020 2020 2020 2020 206f 6232  .            ob2
-000013e0: 5b27 6127 5d0a 0a20 2020 2020 2020 2077  ['a']..        w
-000013f0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00001400: 2822 7465 7374 2044 6174 614f 626a 6563  ("test DataObjec
-00001410: 7420 4b65 7945 7272 6f72 2028 3229 2229  t KeyError (2)")
-00001420: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
-00001430: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
-00001440: 6973 6573 284b 6579 4572 726f 7229 3a0a  ises(KeyError):.
-00001450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001460: 6f62 325b 2761 275d 203d 2031 300a 0a20  ob2['a'] = 10.. 
-00001470: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00001480: 2e73 7562 5465 7374 2822 7465 7374 2044  .subTest("test D
-00001490: 6174 614f 626a 6563 7420 7265 7072 2229  ataObject repr")
-000014a0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000014b0: 6c66 2e61 7373 6572 7445 7175 616c 2822  lf.assertEqual("
-000014c0: 7b27 6127 3a20 3130 7d22 2c20 7265 7072  {'a': 10}", repr
-000014d0: 286f 6232 2929 0a0a 0a63 6c61 7373 2054  (ob2))...class T
-000014e0: 6573 7454 6162 6c65 5479 7065 7328 756e  estTableTypes(un
-000014f0: 6974 7465 7374 2e54 6573 7443 6173 6529  ittest.TestCase)
-00001500: 3a0a 2020 2020 6465 6620 7465 7374 5f74  :.    def test_t
-00001510: 7970 6573 2873 656c 6629 3a0a 0a20 2020  ypes(self):..   
-00001520: 2020 2020 2023 2063 6865 636b 2074 6861       # check tha
-00001530: 7420 5461 626c 6520 616e 6420 496e 6465  t Table and Inde
-00001540: 7820 6172 6520 7265 636f 676e 697a 6564  x are recognized
-00001550: 2061 7320 5365 7175 656e 6365 2061 6e64   as Sequence and
-00001560: 204d 6170 7069 6e67 2074 7970 6573 0a20   Mapping types. 
-00001570: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00001580: 2e73 7562 5465 7374 2822 6368 6563 6b20  .subTest("check 
-00001590: 7468 6174 2054 6162 6c65 2069 7320 7265  that Table is re
-000015a0: 636f 676e 697a 6564 2061 7320 5365 7175  cognized as Sequ
-000015b0: 656e 6365 2074 7970 6522 293a 0a20 2020  ence type"):.   
-000015c0: 2020 2020 2020 2020 2074 203d 206c 742e           t = lt.
-000015d0: 5461 626c 6528 290a 2020 2020 2020 2020  Table().        
-000015e0: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
-000015f0: 7275 6528 6973 696e 7374 616e 6365 2874  rue(isinstance(t
-00001600: 2c20 6c74 2e53 6571 7565 6e63 6529 290a  , lt.Sequence)).
-00001610: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00001620: 6c66 2e73 7562 5465 7374 2822 6368 6563  lf.subTest("chec
-00001630: 6b20 7468 6174 2049 6e64 6578 2069 7320  k that Index is 
-00001640: 7265 636f 676e 697a 6564 2061 7320 4d61  recognized as Ma
-00001650: 7070 696e 6720 7479 7065 2229 3a0a 2020  pping type"):.  
-00001660: 2020 2020 2020 2020 2020 742e 6372 6561            t.crea
-00001670: 7465 5f69 6e64 6578 2822 7822 290a 2020  te_index("x").  
-00001680: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00001690: 7373 6572 7454 7275 6528 6973 696e 7374  ssertTrue(isinst
-000016a0: 616e 6365 2874 2e67 6574 5f69 6e64 6578  ance(t.get_index
-000016b0: 2827 7827 292c 206c 742e 4d61 7070 696e  ('x'), lt.Mappin
-000016c0: 6729 290a 0a20 2020 2020 2020 2023 206d  g))..        # m
-000016d0: 616b 6520 7375 7265 2067 6574 5f69 6e64  ake sure get_ind
-000016e0: 6578 2072 6574 7572 6e73 2061 2072 6561  ex returns a rea
-000016f0: 642d 6f6e 6c79 2061 6363 6573 7320 746f  d-only access to
-00001700: 2074 6865 2075 6e64 6572 6c79 696e 6720   the underlying 
-00001710: 696e 6465 780a 2020 2020 2020 2020 7769  index.        wi
-00001720: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00001730: 2263 6865 636b 2074 6861 7420 6765 745f  "check that get_
-00001740: 696e 6465 7820 7265 7475 726e 7320 6120  index returns a 
-00001750: 7265 6164 2d6f 6e6c 7920 6163 6365 7373  read-only access
-00001760: 2074 6f20 7468 6520 756e 6465 726c 7969   to the underlyi
-00001770: 6e67 2069 6e64 6578 2229 3a0a 2020 2020  ng index"):.    
-00001780: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00001790: 662e 6173 7365 7274 5261 6973 6573 286c  f.assertRaises(l
-000017a0: 742e 5265 6164 6f6e 6c79 496e 6465 7841  t.ReadonlyIndexA
-000017b0: 6363 6573 7345 7272 6f72 293a 0a20 2020  ccessError):.   
-000017c0: 2020 2020 2020 2020 2020 2020 2074 2e67               t.g
-000017d0: 6574 5f69 6e64 6578 2822 7822 295b 2761  et_index("x")['a
-000017e0: 275d 203d 2031 3030 0a0a 0a64 6566 2061  '] = 100...def a
-000017f0: 6e6e 6f75 6e63 655f 7465 7374 2866 6e29  nnounce_test(fn)
-00001800: 3a0a 2020 2020 6465 6620 5f69 6e6e 6572  :.    def _inner
-00001810: 282a 6172 6773 293a 0a20 2020 2020 2020  (*args):.       
-00001820: 2070 7269 6e74 2822 5c6e 2220 2b20 222d   print("\n" + "-
-00001830: 2220 2a20 3530 290a 2020 2020 2020 2020  " * 50).        
-00001840: 7072 696e 7428 6622 7b74 7970 6528 6172  print(f"{type(ar
-00001850: 6773 5b30 5d29 2e5f 5f6e 616d 655f 5f7d  gs[0]).__name__}
-00001860: 2e7b 666e 2e5f 5f6e 616d 655f 5f7d 2229  .{fn.__name__}")
-00001870: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001880: 666e 282a 6172 6773 290a 0a20 2020 2072  fn(*args)..    r
-00001890: 6574 7572 6e20 5f69 6e6e 6572 0a0a 0a64  eturn _inner...d
-000018a0: 6566 206d 616b 655f 7465 7374 5f63 6c61  ef make_test_cla
-000018b0: 7373 282a 636c 6173 7365 7329 3a0a 0a20  ss(*classes):.. 
-000018c0: 2020 2063 6c61 7373 5f6e 616d 6520 3d20     class_name = 
-000018d0: 225f 222e 6a6f 696e 2863 2e5f 5f6e 616d  "_".join(c.__nam
-000018e0: 655f 5f20 666f 7220 6320 696e 2063 6c61  e__ for c in cla
-000018f0: 7373 6573 290a 2020 2020 6966 206e 6f74  sses).    if not
-00001900: 2069 7373 7562 636c 6173 7328 636c 6173   issubclass(clas
-00001910: 7365 735b 305d 2c20 756e 6974 7465 7374  ses[0], unittest
-00001920: 2e54 6573 7443 6173 6529 3a0a 2020 2020  .TestCase):.    
-00001930: 2020 2020 636c 7320 3d20 7479 7065 2863      cls = type(c
-00001940: 6c61 7373 5f6e 616d 652c 2028 756e 6974  lass_name, (unit
-00001950: 7465 7374 2e54 6573 7443 6173 652c 202a  test.TestCase, *
-00001960: 636c 6173 7365 7329 2c20 7b7d 290a 2020  classes), {}).  
-00001970: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00001980: 636c 7320 3d20 7479 7065 2863 6c61 7373  cls = type(class
-00001990: 5f6e 616d 652c 2074 7570 6c65 2863 6c61  _name, tuple(cla
-000019a0: 7373 6573 292c 207b 7d29 0a20 2020 2066  sses), {}).    f
-000019b0: 6f72 2061 7474 7220 696e 2064 6972 2863  or attr in dir(c
-000019c0: 6c73 293a 0a20 2020 2020 2020 2061 7474  ls):.        att
-000019d0: 7276 616c 7565 203d 2067 6574 6174 7472  rvalue = getattr
-000019e0: 2863 6c73 2c20 6174 7472 290a 2020 2020  (cls, attr).    
-000019f0: 2020 2020 6966 2061 7474 722e 7374 6172      if attr.star
-00001a00: 7473 7769 7468 2822 7465 7374 5f22 2920  tswith("test_") 
-00001a10: 616e 6420 6361 6c6c 6162 6c65 2861 7474  and callable(att
-00001a20: 7276 616c 7565 293a 0a20 2020 2020 2020  rvalue):.       
-00001a30: 2020 2020 2073 6574 6174 7472 2863 6c73       setattr(cls
-00001a40: 2c20 6174 7472 2c20 616e 6e6f 756e 6365  , attr, announce
-00001a50: 5f74 6573 7428 6174 7472 7661 6c75 6529  _test(attrvalue)
-00001a60: 290a 2020 2020 676c 6f62 616c 7328 295b  ).    globals()[
-00001a70: 636c 732e 5f5f 6e61 6d65 5f5f 5d20 3d20  cls.__name__] = 
-00001a80: 636c 730a 0a0a 6465 6620 6d61 6b65 5f74  cls...def make_t
-00001a90: 6573 745f 636c 6173 7365 7328 636c 7329  est_classes(cls)
-00001aa0: 3a0a 2020 2020 6d61 6b65 5f74 6573 745f  :.    make_test_
-00001ab0: 636c 6173 7328 636c 732c 2055 7369 6e67  class(cls, Using
-00001ac0: 4461 7461 4f62 6a65 6374 7329 0a20 2020  DataObjects).   
-00001ad0: 206d 616b 655f 7465 7374 5f63 6c61 7373   make_test_class
-00001ae0: 2863 6c73 2c20 5573 696e 674e 616d 6564  (cls, UsingNamed
-00001af0: 7475 706c 6573 290a 2020 2020 6d61 6b65  tuples).    make
-00001b00: 5f74 6573 745f 636c 6173 7328 636c 732c  _test_class(cls,
-00001b10: 2055 7369 6e67 5479 7069 6e67 4e61 6d65   UsingTypingName
-00001b20: 6454 7570 6c65 290a 2020 2020 6d61 6b65  dTuple).    make
-00001b30: 5f74 6573 745f 636c 6173 7328 636c 732c  _test_class(cls,
-00001b40: 2055 7369 6e67 536c 6f74 7465 644f 626a   UsingSlottedObj
-00001b50: 6563 7473 290a 2020 2020 6966 2053 6c6f  ects).    if Slo
-00001b60: 7474 6564 5769 7468 4469 6374 2069 7320  ttedWithDict is 
-00001b70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00001b80: 2020 6d61 6b65 5f74 6573 745f 636c 6173    make_test_clas
-00001b90: 7328 636c 732c 2055 7369 6e67 536c 6f74  s(cls, UsingSlot
-00001ba0: 7465 6457 6974 6844 6963 744f 626a 6563  tedWithDictObjec
-00001bb0: 7473 290a 2020 2020 6d61 6b65 5f74 6573  ts).    make_tes
-00001bc0: 745f 636c 6173 7328 636c 732c 2055 7369  t_class(cls, Usi
-00001bd0: 6e67 5369 6d70 6c65 4e61 6d65 7370 6163  ngSimpleNamespac
-00001be0: 6529 0a20 2020 2069 6620 6461 7461 636c  e).    if datacl
-00001bf0: 6173 7365 7320 6973 206e 6f74 204e 6f6e  asses is not Non
-00001c00: 653a 0a20 2020 2020 2020 206d 616b 655f  e:.        make_
-00001c10: 7465 7374 5f63 6c61 7373 2863 6c73 2c20  test_class(cls, 
-00001c20: 5573 696e 6744 6174 6163 6c61 7373 6573  UsingDataclasses
-00001c30: 290a 2020 2020 6966 2070 7964 616e 7469  ).    if pydanti
-00001c40: 6320 6973 206e 6f74 204e 6f6e 653a 0a20  c is not None:. 
-00001c50: 2020 2020 2020 206d 616b 655f 7465 7374         make_test
-00001c60: 5f63 6c61 7373 2863 6c73 2c20 5573 696e  _class(cls, Usin
-00001c70: 6750 7964 616e 7469 634d 6f64 656c 290a  gPydanticModel).
-00001c80: 2020 2020 2020 2020 6d61 6b65 5f74 6573          make_tes
-00001c90: 745f 636c 6173 7328 636c 732c 2055 7369  t_class(cls, Usi
-00001ca0: 6e67 5079 6461 6e74 6963 496d 6d75 7461  ngPydanticImmuta
-00001cb0: 626c 654d 6f64 656c 290a 2020 2020 2020  bleModel).      
-00001cc0: 2020 6d61 6b65 5f74 6573 745f 636c 6173    make_test_clas
-00001cd0: 7328 636c 732c 2055 7369 6e67 5079 6461  s(cls, UsingPyda
-00001ce0: 6e74 6963 4f52 4d4d 6f64 656c 290a 2020  nticORMModel).  
-00001cf0: 2020 6966 2061 7474 7220 6973 206e 6f74    if attr is not
-00001d00: 204e 6f6e 653a 0a20 2020 2020 2020 206d   None:.        m
-00001d10: 616b 655f 7465 7374 5f63 6c61 7373 2863  ake_test_class(c
-00001d20: 6c73 2c20 5573 696e 6741 7474 7243 6c61  ls, UsingAttrCla
-00001d30: 7373 290a 2020 2020 6966 2074 7261 6974  ss).    if trait
-00001d40: 6c65 7473 2069 7320 6e6f 7420 4e6f 6e65  lets is not None
-00001d50: 3a0a 2020 2020 2020 2020 6d61 6b65 5f74  :.        make_t
-00001d60: 6573 745f 636c 6173 7328 636c 732c 2055  est_class(cls, U
-00001d70: 7369 6e67 5472 6169 746c 6574 7343 6c61  singTraitletsCla
-00001d80: 7373 290a 2020 2020 6d61 6b65 5f74 6573  ss).    make_tes
-00001d90: 745f 636c 6173 7328 636c 732c 2055 7369  t_class(cls, Usi
-00001da0: 6e67 5479 7069 6e67 5479 7065 6444 6963  ngTypingTypedDic
-00001db0: 7429 0a0a 0a63 6c61 7373 2041 6273 7472  t)...class Abstr
-00001dc0: 6163 7443 6f6e 7465 6e74 5479 7065 4661  actContentTypeFa
-00001dd0: 6374 6f72 793a 0a20 2020 2064 6174 615f  ctory:.    data_
-00001de0: 6f62 6a65 6374 5f74 7970 653a 204f 7074  object_type: Opt
-00001df0: 696f 6e61 6c5b 7479 7065 5d20 3d20 4e6f  ional[type] = No
-00001e00: 6e65 0a0a 2020 2020 4063 6c61 7373 6d65  ne..    @classme
-00001e10: 7468 6f64 0a20 2020 2064 6566 206d 616b  thod.    def mak
-00001e20: 655f 6461 7461 5f6f 626a 6563 7428 636c  e_data_object(cl
-00001e30: 732c 2061 2c20 622c 2063 293a 0a20 2020  s, a, b, c):.   
-00001e40: 2020 2020 2072 6574 7572 6e20 636c 732e       return cls.
-00001e50: 6461 7461 5f6f 626a 6563 745f 7479 7065  data_object_type
-00001e60: 2861 3d61 2c20 623d 622c 2063 3d63 290a  (a=a, b=b, c=c).
-00001e70: 0a0a 636c 6173 7320 5573 696e 6744 6174  ..class UsingDat
-00001e80: 614f 626a 6563 7473 2841 6273 7472 6163  aObjects(Abstrac
-00001e90: 7443 6f6e 7465 6e74 5479 7065 4661 6374  tContentTypeFact
-00001ea0: 6f72 7929 3a0a 2020 2020 6461 7461 5f6f  ory):.    data_o
-00001eb0: 626a 6563 745f 7479 7065 203d 206c 742e  bject_type = lt.
-00001ec0: 4461 7461 4f62 6a65 6374 0a0a 0a63 6c61  DataObject...cla
-00001ed0: 7373 2055 7369 6e67 4e61 6d65 6474 7570  ss UsingNamedtup
-00001ee0: 6c65 7328 4162 7374 7261 6374 436f 6e74  les(AbstractCont
-00001ef0: 656e 7454 7970 6546 6163 746f 7279 293a  entTypeFactory):
-00001f00: 0a20 2020 2064 6174 615f 6f62 6a65 6374  .    data_object
-00001f10: 5f74 7970 6520 3d20 4461 7461 5475 706c  _type = DataTupl
-00001f20: 650a 0a0a 636c 6173 7320 5573 696e 6753  e...class UsingS
-00001f30: 6c6f 7474 6564 4f62 6a65 6374 7328 4162  lottedObjects(Ab
-00001f40: 7374 7261 6374 436f 6e74 656e 7454 7970  stractContentTyp
-00001f50: 6546 6163 746f 7279 293a 0a20 2020 2064  eFactory):.    d
-00001f60: 6174 615f 6f62 6a65 6374 5f74 7970 6520  ata_object_type 
-00001f70: 3d20 536c 6f74 7465 640a 0a0a 6966 2053  = Slotted...if S
-00001f80: 6c6f 7474 6564 5769 7468 4469 6374 2069  lottedWithDict i
-00001f90: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00001fa0: 636c 6173 7320 5573 696e 6753 6c6f 7474  class UsingSlott
-00001fb0: 6564 5769 7468 4469 6374 4f62 6a65 6374  edWithDictObject
-00001fc0: 7328 4162 7374 7261 6374 436f 6e74 656e  s(AbstractConten
-00001fd0: 7454 7970 6546 6163 746f 7279 293a 0a20  tTypeFactory):. 
-00001fe0: 2020 2020 2020 2064 6174 615f 6f62 6a65         data_obje
-00001ff0: 6374 5f74 7970 6520 3d20 536c 6f74 7465  ct_type = Slotte
-00002000: 6457 6974 6844 6963 740a 656c 7365 3a0a  dWithDict.else:.
-00002010: 2020 2020 5573 696e 6753 6c6f 7474 6564      UsingSlotted
-00002020: 5769 7468 4469 6374 4f62 6a65 6374 7320  WithDictObjects 
-00002030: 3d20 4162 7374 7261 6374 436f 6e74 656e  = AbstractConten
-00002040: 7454 7970 6546 6163 746f 7279 0a0a 0a63  tTypeFactory...c
-00002050: 6c61 7373 2055 7369 6e67 5369 6d70 6c65  lass UsingSimple
-00002060: 4e61 6d65 7370 6163 6528 4162 7374 7261  Namespace(Abstra
-00002070: 6374 436f 6e74 656e 7454 7970 6546 6163  ctContentTypeFac
-00002080: 746f 7279 293a 0a20 2020 2064 6174 615f  tory):.    data_
-00002090: 6f62 6a65 6374 5f74 7970 6520 3d20 5369  object_type = Si
-000020a0: 6d70 6c65 4e61 6d65 7370 6163 650a 0a0a  mpleNamespace...
-000020b0: 6966 2064 6174 6163 6c61 7373 6573 2069  if dataclasses i
-000020c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000020d0: 636c 6173 7320 5573 696e 6744 6174 6163  class UsingDatac
-000020e0: 6c61 7373 6573 2841 6273 7472 6163 7443  lasses(AbstractC
-000020f0: 6f6e 7465 6e74 5479 7065 4661 6374 6f72  ontentTypeFactor
-00002100: 7929 3a0a 2020 2020 2020 2020 6461 7461  y):.        data
-00002110: 5f6f 626a 6563 745f 7479 7065 203d 2044  _object_type = D
-00002120: 6174 6144 6174 6163 6c61 7373 0a65 6c73  ataDataclass.els
-00002130: 653a 0a20 2020 2055 7369 6e67 4461 7461  e:.    UsingData
-00002140: 636c 6173 7365 7320 3d20 4162 7374 7261  classes = Abstra
-00002150: 6374 436f 6e74 656e 7454 7970 6546 6163  ctContentTypeFac
-00002160: 746f 7279 0a0a 0a69 6620 7079 6461 6e74  tory...if pydant
-00002170: 6963 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ic is not None:.
-00002180: 2020 2020 636c 6173 7320 5573 696e 6750      class UsingP
-00002190: 7964 616e 7469 634d 6f64 656c 2841 6273  ydanticModel(Abs
-000021a0: 7472 6163 7443 6f6e 7465 6e74 5479 7065  tractContentType
-000021b0: 4661 6374 6f72 7929 3a0a 2020 2020 2020  Factory):.      
-000021c0: 2020 6461 7461 5f6f 626a 6563 745f 7479    data_object_ty
-000021d0: 7065 203d 2044 6174 6150 7964 616e 7469  pe = DataPydanti
-000021e0: 634d 6f64 656c 0a0a 2020 2020 636c 6173  cModel..    clas
-000021f0: 7320 5573 696e 6750 7964 616e 7469 6349  s UsingPydanticI
-00002200: 6d6d 7574 6162 6c65 4d6f 6465 6c28 4162  mmutableModel(Ab
-00002210: 7374 7261 6374 436f 6e74 656e 7454 7970  stractContentTyp
-00002220: 6546 6163 746f 7279 293a 0a20 2020 2020  eFactory):.     
-00002230: 2020 2064 6174 615f 6f62 6a65 6374 5f74     data_object_t
-00002240: 7970 6520 3d20 4461 7461 5079 6461 6e74  ype = DataPydant
-00002250: 6963 496d 6d75 7461 626c 654d 6f64 656c  icImmutableModel
-00002260: 0a0a 2020 2020 636c 6173 7320 5573 696e  ..    class Usin
-00002270: 6750 7964 616e 7469 634f 524d 4d6f 6465  gPydanticORMMode
-00002280: 6c28 4162 7374 7261 6374 436f 6e74 656e  l(AbstractConten
-00002290: 7454 7970 6546 6163 746f 7279 293a 0a20  tTypeFactory):. 
-000022a0: 2020 2020 2020 2064 6174 615f 6f62 6a65         data_obje
-000022b0: 6374 5f74 7970 6520 3d20 4461 7461 5079  ct_type = DataPy
-000022c0: 6461 6e74 6963 4f52 4d4d 6f64 656c 0a0a  danticORMModel..
-000022d0: 656c 7365 3a0a 2020 2020 5573 696e 6750  else:.    UsingP
-000022e0: 7964 616e 7469 634d 6f64 656c 203d 2041  ydanticModel = A
-000022f0: 6273 7472 6163 7443 6f6e 7465 6e74 5479  bstractContentTy
-00002300: 7065 4661 6374 6f72 790a 2020 2020 5573  peFactory.    Us
-00002310: 696e 6750 7964 616e 7469 6349 6d6d 7574  ingPydanticImmut
-00002320: 6162 6c65 4d6f 6465 6c20 3d20 4162 7374  ableModel = Abst
-00002330: 7261 6374 436f 6e74 656e 7454 7970 6546  ractContentTypeF
-00002340: 6163 746f 7279 0a20 2020 2055 7369 6e67  actory.    Using
-00002350: 5079 6461 6e74 6963 4f52 4d4d 6f64 656c  PydanticORMModel
-00002360: 203d 2041 6273 7472 6163 7443 6f6e 7465   = AbstractConte
-00002370: 6e74 5479 7065 4661 6374 6f72 790a 0a69  ntTypeFactory..i
-00002380: 6620 6174 7472 2069 7320 6e6f 7420 4e6f  f attr is not No
-00002390: 6e65 3a0a 2020 2020 636c 6173 7320 5573  ne:.    class Us
-000023a0: 696e 6741 7474 7243 6c61 7373 2841 6273  ingAttrClass(Abs
-000023b0: 7472 6163 7443 6f6e 7465 6e74 5479 7065  tractContentType
-000023c0: 4661 6374 6f72 7929 3a0a 2020 2020 2020  Factory):.      
-000023d0: 2020 6461 7461 5f6f 626a 6563 745f 7479    data_object_ty
-000023e0: 7065 203d 2041 7474 7243 6c61 7373 0a65  pe = AttrClass.e
-000023f0: 6c73 653a 0a20 2020 2055 7369 6e67 4174  lse:.    UsingAt
-00002400: 7472 436c 6173 7320 3d20 4162 7374 7261  trClass = Abstra
-00002410: 6374 436f 6e74 656e 7454 7970 6546 6163  ctContentTypeFac
-00002420: 746f 7279 0a0a 6966 2074 7261 6974 6c65  tory..if traitle
-00002430: 7473 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ts is not None:.
-00002440: 2020 2020 636c 6173 7320 5573 696e 6754      class UsingT
-00002450: 7261 6974 6c65 7473 436c 6173 7328 4162  raitletsClass(Ab
-00002460: 7374 7261 6374 436f 6e74 656e 7454 7970  stractContentTyp
-00002470: 6546 6163 746f 7279 293a 0a20 2020 2020  eFactory):.     
-00002480: 2020 2064 6174 615f 6f62 6a65 6374 5f74     data_object_t
-00002490: 7970 6520 3d20 5472 6169 746c 6574 7343  ype = TraitletsC
-000024a0: 6c61 7373 0a65 6c73 653a 0a20 2020 2055  lass.else:.    U
-000024b0: 7369 6e67 5472 6169 746c 6574 7343 6c61  singTraitletsCla
-000024c0: 7373 203d 2041 6273 7472 6163 7443 6f6e  ss = AbstractCon
-000024d0: 7465 6e74 5479 7065 4661 6374 6f72 790a  tentTypeFactory.
-000024e0: 0a63 6c61 7373 2055 7369 6e67 5479 7069  .class UsingTypi
-000024f0: 6e67 4e61 6d65 6454 7570 6c65 2841 6273  ngNamedTuple(Abs
-00002500: 7472 6163 7443 6f6e 7465 6e74 5479 7065  tractContentType
-00002510: 4661 6374 6f72 7929 3a0a 2020 2020 6461  Factory):.    da
-00002520: 7461 5f6f 626a 6563 745f 7479 7065 203d  ta_object_type =
-00002530: 2054 7970 696e 674e 616d 6564 5475 706c   TypingNamedTupl
-00002540: 650a 0a63 6c61 7373 2055 7369 6e67 5479  e..class UsingTy
-00002550: 7069 6e67 5479 7065 6444 6963 7428 4162  pingTypedDict(Ab
+00000280: 6528 6461 7465 7469 6d65 2e74 696d 657a  e(datetime.timez
+00000290: 6f6e 652e 7574 6329 0a20 2020 2069 6620  one.utc).    if 
+000002a0: 6c61 6265 6c3a 0a20 2020 2020 2020 2070  label:.        p
+000002b0: 7269 6e74 2866 2253 7461 7274 202d 207b  rint(f"Start - {
+000002c0: 6c61 6265 6c7d 3a20 7b72 6574 2e73 7461  label}: {ret.sta
+000002d0: 7274 7d22 2c20 6669 6c65 3d66 696c 6529  rt}", file=file)
+000002e0: 0a20 2020 2079 6965 6c64 2072 6574 0a20  .    yield ret. 
+000002f0: 2020 2072 6574 2e65 6e64 203d 2064 6174     ret.end = dat
+00000300: 6574 696d 652e 6461 7465 7469 6d65 2e6e  etime.datetime.n
+00000310: 6f77 2829 2e61 7374 696d 657a 6f6e 6528  ow().astimezone(
+00000320: 6461 7465 7469 6d65 2e74 696d 657a 6f6e  datetime.timezon
+00000330: 652e 7574 6329 0a20 2020 2072 6574 2e65  e.utc).    ret.e
+00000340: 6c61 7073 6564 203d 2072 6574 2e65 6e64  lapsed = ret.end
+00000350: 202d 2072 6574 2e73 7461 7274 0a20 2020   - ret.start.   
+00000360: 2069 6620 6c61 6265 6c3a 0a20 2020 2020   if label:.     
+00000370: 2020 2070 7269 6e74 2866 2245 6e64 2020     print(f"End  
+00000380: 202d 207b 6c61 6265 6c7d 3a20 7b72 6574   - {label}: {ret
+00000390: 2e65 6e64 7d22 2c20 6669 6c65 3d66 696c  .end}", file=fil
+000003a0: 6529 0a0a 0a69 6d70 6f72 7420 6461 7461  e)...import data
+000003b0: 636c 6173 7365 730a 4064 6174 6163 6c61  classes.@datacla
+000003c0: 7373 6573 2e64 6174 6163 6c61 7373 0a63  sses.dataclass.c
+000003d0: 6c61 7373 2044 6174 6144 6174 6163 6c61  lass DataDatacla
+000003e0: 7373 3a0a 2020 2020 613a 2069 6e74 0a20  ss:.    a: int. 
+000003f0: 2020 2062 3a20 696e 740a 2020 2020 633a     b: int.    c:
+00000400: 2069 6e74 0a0a 7472 793a 0a20 2020 2069   int..try:.    i
+00000410: 6d70 6f72 7420 7079 6461 6e74 6963 0a65  mport pydantic.e
+00000420: 7863 6570 7420 496d 706f 7274 4572 726f  xcept ImportErro
+00000430: 723a 0a20 2020 2070 7269 6e74 2822 7079  r:.    print("py
+00000440: 6461 6e74 6963 2074 6573 7473 2064 6973  dantic tests dis
+00000450: 6162 6c65 6422 290a 2020 2020 7079 6461  abled").    pyda
+00000460: 6e74 6963 203d 204e 6f6e 650a 656c 7365  ntic = None.else
+00000470: 3a0a 2020 2020 636c 6173 7320 4461 7461  :.    class Data
+00000480: 5079 6461 6e74 6963 4d6f 6465 6c28 7079  PydanticModel(py
+00000490: 6461 6e74 6963 2e42 6173 654d 6f64 656c  dantic.BaseModel
+000004a0: 293a 0a20 2020 2020 2020 2061 3a20 4f70  ):.        a: Op
+000004b0: 7469 6f6e 616c 5b55 6e69 6f6e 5b69 6e74  tional[Union[int
+000004c0: 2c20 7374 725d 5d0a 2020 2020 2020 2020  , str]].        
+000004d0: 623a 204f 7074 696f 6e61 6c5b 556e 696f  b: Optional[Unio
+000004e0: 6e5b 696e 742c 2073 7472 5d5d 0a20 2020  n[int, str]].   
+000004f0: 2020 2020 2063 3a20 4f70 7469 6f6e 616c       c: Optional
+00000500: 5b55 6e69 6f6e 5b69 6e74 2c20 7374 725d  [Union[int, str]
+00000510: 5d0a 0a20 2020 2063 6c61 7373 2044 6174  ]..    class Dat
+00000520: 6150 7964 616e 7469 6349 6d6d 7574 6162  aPydanticImmutab
+00000530: 6c65 4d6f 6465 6c28 7079 6461 6e74 6963  leModel(pydantic
+00000540: 2e42 6173 654d 6f64 656c 293a 0a20 2020  .BaseModel):.   
+00000550: 2020 2020 2063 6c61 7373 2043 6f6e 6669       class Confi
+00000560: 673a 0a20 2020 2020 2020 2020 2020 2061  g:.            a
+00000570: 6c6c 6f77 5f6d 7574 6174 696f 6e20 3d20  llow_mutation = 
+00000580: 4661 6c73 650a 0a20 2020 2020 2020 2061  False..        a
+00000590: 3a20 4f70 7469 6f6e 616c 5b55 6e69 6f6e  : Optional[Union
+000005a0: 5b69 6e74 2c20 7374 725d 5d0a 2020 2020  [int, str]].    
+000005b0: 2020 2020 623a 204f 7074 696f 6e61 6c5b      b: Optional[
+000005c0: 556e 696f 6e5b 696e 742c 2073 7472 5d5d  Union[int, str]]
+000005d0: 0a20 2020 2020 2020 2063 3a20 4f70 7469  .        c: Opti
+000005e0: 6f6e 616c 5b55 6e69 6f6e 5b69 6e74 2c20  onal[Union[int, 
+000005f0: 7374 725d 5d0a 0a20 2020 2063 6c61 7373  str]]..    class
+00000600: 2044 6174 6150 7964 616e 7469 634f 524d   DataPydanticORM
+00000610: 4d6f 6465 6c28 7079 6461 6e74 6963 2e42  Model(pydantic.B
+00000620: 6173 654d 6f64 656c 293a 0a20 2020 2020  aseModel):.     
+00000630: 2020 2063 6c61 7373 2043 6f6e 6669 673a     class Config:
+00000640: 0a20 2020 2020 2020 2020 2020 206f 726d  .            orm
+00000650: 5f6d 6f64 6520 3d20 5472 7565 0a0a 2020  _mode = True..  
+00000660: 2020 2020 2020 613a 204f 7074 696f 6e61        a: Optiona
+00000670: 6c5b 556e 696f 6e5b 696e 742c 2073 7472  l[Union[int, str
+00000680: 5d5d 0a20 2020 2020 2020 2062 3a20 4f70  ]].        b: Op
+00000690: 7469 6f6e 616c 5b55 6e69 6f6e 5b69 6e74  tional[Union[int
+000006a0: 2c20 7374 725d 5d0a 2020 2020 2020 2020  , str]].        
+000006b0: 633a 204f 7074 696f 6e61 6c5b 556e 696f  c: Optional[Unio
+000006c0: 6e5b 696e 742c 2073 7472 5d5d 0a0a 7472  n[int, str]]..tr
+000006d0: 793a 0a20 2020 2069 6d70 6f72 7420 6174  y:.    import at
+000006e0: 7472 0a65 7863 6570 7420 496d 706f 7274  tr.except Import
+000006f0: 4572 726f 723a 0a20 2020 2070 7269 6e74  Error:.    print
+00000700: 2822 6174 7472 7320 7465 7374 7320 6469  ("attrs tests di
+00000710: 7361 626c 6564 2229 0a20 2020 2061 7474  sabled").    att
+00000720: 7220 3d20 4e6f 6e65 0a65 6c73 653a 0a20  r = None.else:. 
+00000730: 2020 2041 7474 7243 6c61 7373 203d 2061     AttrClass = a
+00000740: 7474 722e 6d61 6b65 5f63 6c61 7373 2822  ttr.make_class("
+00000750: 4174 7472 436c 6173 7322 2c20 5b22 6122  AttrClass", ["a"
+00000760: 2c20 2262 222c 2022 6322 5d29 0a0a 7472  , "b", "c"])..tr
+00000770: 793a 0a20 2020 2069 6d70 6f72 7420 7472  y:.    import tr
+00000780: 6169 746c 6574 730a 6578 6365 7074 2049  aitlets.except I
+00000790: 6d70 6f72 7445 7272 6f72 3a0a 2020 2020  mportError:.    
+000007a0: 7072 696e 7428 2274 7261 6974 6c65 7473  print("traitlets
+000007b0: 2074 6573 7473 2064 6973 6162 6c65 6422   tests disabled"
+000007c0: 290a 2020 2020 7472 6169 746c 6574 7320  ).    traitlets 
+000007d0: 3d20 4e6f 6e65 0a65 6c73 653a 0a20 2020  = None.else:.   
+000007e0: 2063 6c61 7373 2054 7261 6974 6c65 7473   class Traitlets
+000007f0: 436c 6173 7328 6c74 2e48 6173 5472 6169  Class(lt.HasTrai
+00000800: 7473 4d69 7869 6e2c 2074 7261 6974 6c65  tsMixin, traitle
+00000810: 7473 2e48 6173 5472 6169 7473 293a 0a20  ts.HasTraits):. 
+00000820: 2020 2020 2020 2061 203d 2074 7261 6974         a = trait
+00000830: 6c65 7473 2e55 6e69 6f6e 285b 7472 6169  lets.Union([trai
+00000840: 746c 6574 732e 496e 7428 292c 2074 7261  tlets.Int(), tra
+00000850: 6974 6c65 7473 2e55 6e69 636f 6465 2829  itlets.Unicode()
+00000860: 5d2c 2061 6c6c 6f77 5f6e 6f6e 653d 5472  ], allow_none=Tr
+00000870: 7565 290a 2020 2020 2020 2020 6220 3d20  ue).        b = 
+00000880: 7472 6169 746c 6574 732e 556e 696f 6e28  traitlets.Union(
+00000890: 5b74 7261 6974 6c65 7473 2e49 6e74 2829  [traitlets.Int()
+000008a0: 2c20 7472 6169 746c 6574 732e 556e 6963  , traitlets.Unic
+000008b0: 6f64 6528 295d 2c20 616c 6c6f 775f 6e6f  ode()], allow_no
+000008c0: 6e65 3d54 7275 6529 0a20 2020 2020 2020  ne=True).       
+000008d0: 2063 203d 2074 7261 6974 6c65 7473 2e55   c = traitlets.U
+000008e0: 6e69 6f6e 285b 7472 6169 746c 6574 732e  nion([traitlets.
+000008f0: 496e 7428 292c 2074 7261 6974 6c65 7473  Int(), traitlets
+00000900: 2e55 6e69 636f 6465 2829 5d2c 2061 6c6c  .Unicode()], all
+00000910: 6f77 5f6e 6f6e 653d 5472 7565 290a 0a20  ow_none=True).. 
+00000920: 2020 2020 2020 2064 6566 205f 5f69 6e69         def __ini
+00000930: 745f 5f28 7365 6c66 2c20 2a2a 6b77 6172  t__(self, **kwar
+00000940: 6773 293a 0a20 2020 2020 2020 2020 2020  gs):.           
+00000950: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
+00000960: 5f28 290a 2020 2020 2020 2020 2020 2020  _().            
+00000970: 666f 7220 6b2c 2077 2069 6e20 6b77 6172  for k, w in kwar
+00000980: 6773 2e69 7465 6d73 2829 3a0a 2020 2020  gs.items():.    
+00000990: 2020 2020 2020 2020 2020 2020 7365 7461              seta
+000009a0: 7474 7228 7365 6c66 2c20 6b2c 2077 290a  ttr(self, k, w).
+000009b0: 0a20 2020 2020 2020 2064 6566 205f 5f72  .        def __r
+000009c0: 6570 725f 5f28 7365 6c66 293a 0a20 2020  epr__(self):.   
+000009d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000009e0: 6622 7b74 7970 6528 7365 6c66 292e 5f5f  f"{type(self).__
+000009f0: 6e61 6d65 5f5f 7d3a 2861 3d7b 7365 6c66  name__}:(a={self
+00000a00: 2e61 7d2c 2062 3d7b 7365 6c66 2e62 7d2c  .a}, b={self.b},
+00000a10: 2063 3d7b 7365 6c66 2e63 7d29 220a 0a20   c={self.c})".. 
+00000a20: 2020 2020 2020 2064 6566 205f 5f64 6972         def __dir
+00000a30: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+00000a40: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00000a50: 662e 7472 6169 745f 6e61 6d65 7328 290a  f.trait_names().
+00000a60: 0a44 6174 6154 7570 6c65 203d 206e 616d  .DataTuple = nam
+00000a70: 6564 7475 706c 6528 2244 6174 6154 7570  edtuple("DataTup
+00000a80: 6c65 222c 2022 6120 6220 6322 290a 0a0a  le", "a b c")...
+00000a90: 636c 6173 7320 5479 7069 6e67 4e61 6d65  class TypingName
+00000aa0: 6454 7570 6c65 2874 7970 696e 672e 4e61  dTuple(typing.Na
+00000ab0: 6d65 6454 7570 6c65 293a 0a20 2020 2061  medTuple):.    a
+00000ac0: 3a20 696e 740a 2020 2020 623a 2069 6e74  : int.    b: int
+00000ad0: 0a20 2020 2063 3a20 696e 740a 0a0a 2320  .    c: int...# 
+00000ae0: 6966 2072 6963 6820 6973 206e 6f74 2069  if rich is not i
+00000af0: 6e73 7461 6c6c 6564 2c20 6469 7361 626c  nstalled, disabl
+00000b00: 6520 7461 626c 652e 7072 6573 656e 7428  e table.present(
+00000b10: 2920 6361 6c6c 730a 7472 793a 0a20 2020  ) calls.try:.   
+00000b20: 2069 6d70 6f72 7420 7269 6368 0a65 7863   import rich.exc
+00000b30: 6570 7420 496d 706f 7274 4572 726f 723a  ept ImportError:
+00000b40: 0a20 2020 2072 6963 6820 3d20 4e6f 6e65  .    rich = None
+00000b50: 0a20 2020 2023 2064 6973 6162 6c65 2070  .    # disable p
+00000b60: 7265 7365 6e74 2829 206d 6574 686f 642c  resent() method,
+00000b70: 2073 696e 6365 2072 6963 6820 6973 206e   since rich is n
+00000b80: 6f74 2061 7661 696c 6162 6c65 0a20 2020  ot available.   
+00000b90: 206c 742e 5461 626c 652e 7072 6573 656e   lt.Table.presen
+00000ba0: 7420 3d20 6c61 6d62 6461 202a 6172 6773  t = lambda *args
+00000bb0: 2c20 2a2a 6b77 6172 6773 3a20 4e6f 6e65  , **kwargs: None
+00000bc0: 0a0a 0a63 6c61 7373 2053 6c6f 7474 6564  ...class Slotted
+00000bd0: 3a0a 2020 2020 5f5f 736c 6f74 735f 5f20  :.    __slots__ 
+00000be0: 3d20 5b27 6127 2c20 2762 272c 2027 6327  = ['a', 'b', 'c'
+00000bf0: 5d0a 0a20 2020 2064 6566 205f 5f69 6e69  ]..    def __ini
+00000c00: 745f 5f28 7365 6c66 2c20 612c 2062 2c20  t__(self, a, b, 
+00000c10: 6329 3a0a 2020 2020 2020 2020 7365 6c66  c):.        self
+00000c20: 2e61 203d 2061 0a20 2020 2020 2020 2073  .a = a.        s
+00000c30: 656c 662e 6220 3d20 620a 2020 2020 2020  elf.b = b.      
+00000c40: 2020 7365 6c66 2e63 203d 2063 0a0a 2020    self.c = c..  
+00000c50: 2020 6465 6620 5f5f 6571 5f5f 2873 656c    def __eq__(sel
+00000c60: 662c 206f 7468 6572 293a 0a20 2020 2020  f, other):.     
+00000c70: 2020 2072 6574 7572 6e20 2869 7369 6e73     return (isins
+00000c80: 7461 6e63 6528 6f74 6865 722c 2053 6c6f  tance(other, Slo
+00000c90: 7474 6564 2920 616e 640a 2020 2020 2020  tted) and.      
+00000ca0: 2020 2020 2020 2020 2020 616c 6c28 6765            all(ge
+00000cb0: 7461 7474 7228 7365 6c66 2c20 6174 7472  tattr(self, attr
+00000cc0: 2920 3d3d 2067 6574 6174 7472 286f 7468  ) == getattr(oth
+00000cd0: 6572 2c20 6174 7472 2920 666f 7220 6174  er, attr) for at
+00000ce0: 7472 2069 6e20 7365 6c66 2e5f 5f73 6c6f  tr in self.__slo
+00000cf0: 7473 5f5f 2929 0a0a 2020 2020 6465 6620  ts__))..    def 
+00000d00: 5f5f 7265 7072 5f5f 2873 656c 6629 3a0a  __repr__(self):.
+00000d10: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00000d20: 227b 7479 7065 2873 656c 6629 2e5f 5f6e  "{type(self).__n
+00000d30: 616d 655f 5f7d 3a28 613d 7b73 656c 662e  ame__}:(a={self.
+00000d40: 617d 2c20 623d 7b73 656c 662e 627d 2c20  a}, b={self.b}, 
+00000d50: 633d 7b73 656c 662e 637d 2922 0a0a 0a63  c={self.c})"...c
+00000d60: 6c61 7373 2053 6c6f 7474 6564 5769 7468  lass SlottedWith
+00000d70: 4469 6374 3a0a 2020 2020 5f5f 736c 6f74  Dict:.    __slot
+00000d80: 735f 5f20 3d20 7b27 6127 3a20 2761 272c  s__ = {'a': 'a',
+00000d90: 2027 6227 3a20 2762 272c 2027 6327 3a20   'b': 'b', 'c': 
+00000da0: 2763 277d 0a0a 2020 2020 6465 6620 5f5f  'c'}..    def __
+00000db0: 696e 6974 5f5f 2873 656c 662c 2061 2c20  init__(self, a, 
+00000dc0: 622c 2063 293a 0a20 2020 2020 2020 2073  b, c):.        s
+00000dd0: 656c 662e 6120 3d20 610a 2020 2020 2020  elf.a = a.      
+00000de0: 2020 7365 6c66 2e62 203d 2062 0a20 2020    self.b = b.   
+00000df0: 2020 2020 2073 656c 662e 6320 3d20 630a       self.c = c.
+00000e00: 0a20 2020 2064 6566 205f 5f65 715f 5f28  .    def __eq__(
+00000e10: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
+00000e20: 2020 2020 2020 7265 7475 726e 2028 6973        return (is
+00000e30: 696e 7374 616e 6365 286f 7468 6572 2c20  instance(other, 
+00000e40: 536c 6f74 7465 6457 6974 6844 6963 7429  SlottedWithDict)
+00000e50: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
+00000e60: 2020 2020 2061 6c6c 2867 6574 6174 7472       all(getattr
+00000e70: 2873 656c 662c 2061 7474 7229 203d 3d20  (self, attr) == 
+00000e80: 6765 7461 7474 7228 6f74 6865 722c 2061  getattr(other, a
+00000e90: 7474 7229 2066 6f72 2061 7474 7220 696e  ttr) for attr in
+00000ea0: 2073 656c 662e 5f5f 736c 6f74 735f 5f29   self.__slots__)
+00000eb0: 290a 0a20 2020 2064 6566 205f 5f72 6570  )..    def __rep
+00000ec0: 725f 5f28 7365 6c66 293a 0a20 2020 2020  r__(self):.     
+00000ed0: 2020 2072 6574 7572 6e20 6622 7b74 7970     return f"{typ
+00000ee0: 6528 7365 6c66 292e 5f5f 6e61 6d65 5f5f  e(self).__name__
+00000ef0: 7d3a 2861 3d7b 7365 6c66 2e61 7d2c 2062  }:(a={self.a}, b
+00000f00: 3d7b 7365 6c66 2e62 7d2c 2063 3d7b 7365  ={self.b}, c={se
+00000f10: 6c66 2e63 7d29 220a 0a0a 636c 6173 7320  lf.c})"...class 
+00000f20: 5479 7069 6e67 5479 7065 6444 6963 7428  TypingTypedDict(
+00000f30: 7479 7069 6e67 2e54 7970 6564 4469 6374  typing.TypedDict
+00000f40: 293a 0a20 2020 2061 3a20 696e 740a 2020  ):.    a: int.  
+00000f50: 2020 623a 2069 6e74 0a20 2020 2063 3a20    b: int.    c: 
+00000f60: 696e 740a 0a0a 636c 6173 7320 5465 7374  int...class Test
+00000f70: 4461 7461 4f62 6a65 6374 7328 756e 6974  DataObjects(unit
+00000f80: 7465 7374 2e54 6573 7443 6173 6529 3a0a  test.TestCase):.
+00000f90: 2020 2020 6465 6620 7465 7374 5f73 6574      def test_set
+00000fa0: 5f61 7474 7269 6275 7465 7328 7365 6c66  _attributes(self
+00000fb0: 293a 0a20 2020 2020 2020 206f 6220 3d20  ):.        ob = 
+00000fc0: 6c74 2e44 6174 614f 626a 6563 7428 290a  lt.DataObject().
+00000fd0: 2020 2020 2020 2020 6f62 2e7a 203d 2032          ob.z = 2
+00000fe0: 3030 0a20 2020 2020 2020 206f 622e 6120  00.        ob.a 
+00000ff0: 3d20 3130 300a 2020 2020 2020 2020 7769  = 100.        wi
+00001000: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+00001010: 2274 6573 7420 4461 7461 4f62 6a65 6374  "test DataObject
+00001020: 2061 7474 7269 6275 7465 2073 6574 7469   attribute setti
+00001030: 6e67 2229 3a0a 2020 2020 2020 2020 2020  ng"):.          
+00001040: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00001050: 616c 285b 2827 6127 2c20 3130 3029 2c20  al([('a', 100), 
+00001060: 2827 7a27 2c20 3230 3029 5d2c 2073 6f72  ('z', 200)], sor
+00001070: 7465 6428 6f62 2e5f 5f64 6963 745f 5f2e  ted(ob.__dict__.
+00001080: 6974 656d 7328 2929 290a 0a20 2020 2020  items()))..     
+00001090: 2020 2023 2074 6573 7420 7365 6d69 2d69     # test semi-i
+000010a0: 6d6d 7574 6162 696c 6974 7920 2863 616e  mmutability (can
+000010b0: 2774 206f 7665 7277 7269 7465 2065 7869  't overwrite exi
+000010c0: 7374 696e 6720 6174 7472 6962 7574 6573  sting attributes
+000010d0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+000010e0: 656c 662e 7375 6254 6573 7428 2274 6573  elf.subTest("tes
+000010f0: 7420 4461 7461 4f62 6a65 6374 2077 7269  t DataObject wri
+00001100: 7465 2d6f 6e63 6520 2873 656d 692d 696d  te-once (semi-im
+00001110: 6d75 7461 6269 6c69 7479 2922 293a 0a20  mutability)"):. 
+00001120: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00001130: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
+00001140: 7328 4174 7472 6962 7574 6545 7272 6f72  s(AttributeError
+00001150: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00001160: 2020 206f 622e 6120 3d20 3130 310a 0a20     ob.a = 101.. 
+00001170: 2020 2020 2020 2023 2065 7175 616c 6974         # equalit
+00001180: 7920 7465 7374 730a 2020 2020 2020 2020  y tests.        
+00001190: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+000011a0: 7428 2274 6573 7420 4461 7461 4f62 6a65  t("test DataObje
+000011b0: 6374 2065 7175 616c 6974 7922 293a 0a20  ct equality"):. 
+000011c0: 2020 2020 2020 2020 2020 206f 6232 203d             ob2 =
+000011d0: 206c 742e 4461 7461 4f62 6a65 6374 282a   lt.DataObject(*
+000011e0: 2a7b 2761 273a 2031 3030 2c20 277a 273a  *{'a': 100, 'z':
+000011f0: 2032 3030 7d29 0a20 2020 2020 2020 2020   200}).         
+00001200: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00001210: 7561 6c28 6f62 322c 206f 6229 0a0a 2020  ual(ob2, ob)..  
+00001220: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00001230: 7375 6254 6573 7428 2274 6573 7420 4461  subTest("test Da
+00001240: 7461 4f62 6a65 6374 2069 6e65 7175 616c  taObject inequal
+00001250: 6974 7922 293a 0a20 2020 2020 2020 2020  ity"):.         
+00001260: 2020 206f 6232 2e62 203d 2027 626c 6168     ob2.b = 'blah
+00001270: 270a 2020 2020 2020 2020 2020 2020 7365  '.            se
+00001280: 6c66 2e61 7373 6572 744e 6f74 4571 7561  lf.assertNotEqua
+00001290: 6c28 6f62 2c20 6f62 3229 0a0a 2020 2020  l(ob, ob2)..    
+000012a0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+000012b0: 6254 6573 7428 2274 6573 7420 4461 7461  bTest("test Data
+000012c0: 4f62 6a65 6374 2065 7175 616c 6974 7920  Object equality 
+000012d0: 6166 7465 7220 7570 6461 7465 7322 293a  after updates"):
+000012e0: 0a20 2020 2020 2020 2020 2020 2064 656c  .            del
+000012f0: 206f 6232 2e62 0a20 2020 2020 2020 2020   ob2.b.         
+00001300: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00001310: 7561 6c28 6f62 322c 206f 6229 0a0a 2020  ual(ob2, ob)..  
+00001320: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00001330: 7375 6254 6573 7428 2274 6573 7420 4461  subTest("test Da
+00001340: 7461 4f62 6a65 6374 204b 6579 4572 726f  taObject KeyErro
+00001350: 7222 293a 0a20 2020 2020 2020 2020 2020  r"):.           
+00001360: 2064 656c 206f 6232 2e61 0a20 2020 2020   del ob2.a.     
+00001370: 2020 2020 2020 2064 656c 206f 6232 2e7a         del ob2.z
+00001380: 0a0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
+00001390: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
+000013a0: 6973 6573 284b 6579 4572 726f 7229 3a0a  ises(KeyError):.
+000013b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013c0: 6f62 325b 2761 275d 0a20 2020 2020 2020  ob2['a'].       
+000013d0: 2020 2020 206f 6232 5b27 6127 5d20 3d20       ob2['a'] = 
+000013e0: 3130 0a20 2020 2020 2020 2020 2020 206f  10.            o
+000013f0: 6232 5b27 6127 5d0a 0a20 2020 2020 2020  b2['a']..       
+00001400: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+00001410: 7374 2822 7465 7374 2044 6174 614f 626a  st("test DataObj
+00001420: 6563 7420 4b65 7945 7272 6f72 2028 3229  ect KeyError (2)
+00001430: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00001440: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
+00001450: 5261 6973 6573 284b 6579 4572 726f 7229  Raises(KeyError)
+00001460: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00001470: 2020 6f62 325b 2761 275d 203d 2031 300a    ob2['a'] = 10.
+00001480: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+00001490: 6c66 2e73 7562 5465 7374 2822 7465 7374  lf.subTest("test
+000014a0: 2044 6174 614f 626a 6563 7420 7265 7072   DataObject repr
+000014b0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+000014c0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000014d0: 2822 7b27 6127 3a20 3130 7d22 2c20 7265  ("{'a': 10}", re
+000014e0: 7072 286f 6232 2929 0a0a 0a63 6c61 7373  pr(ob2))...class
+000014f0: 2054 6573 7454 6162 6c65 5479 7065 7328   TestTableTypes(
+00001500: 756e 6974 7465 7374 2e54 6573 7443 6173  unittest.TestCas
+00001510: 6529 3a0a 2020 2020 6465 6620 7465 7374  e):.    def test
+00001520: 5f74 7970 6573 2873 656c 6629 3a0a 0a20  _types(self):.. 
+00001530: 2020 2020 2020 2023 2063 6865 636b 2074         # check t
+00001540: 6861 7420 5461 626c 6520 616e 6420 496e  hat Table and In
+00001550: 6465 7820 6172 6520 7265 636f 676e 697a  dex are recogniz
+00001560: 6564 2061 7320 5365 7175 656e 6365 2061  ed as Sequence a
+00001570: 6e64 204d 6170 7069 6e67 2074 7970 6573  nd Mapping types
+00001580: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+00001590: 6c66 2e73 7562 5465 7374 2822 6368 6563  lf.subTest("chec
+000015a0: 6b20 7468 6174 2054 6162 6c65 2069 7320  k that Table is 
+000015b0: 7265 636f 676e 697a 6564 2061 7320 5365  recognized as Se
+000015c0: 7175 656e 6365 2074 7970 6522 293a 0a20  quence type"):. 
+000015d0: 2020 2020 2020 2020 2020 2074 203d 206c             t = l
+000015e0: 742e 5461 626c 6528 290a 2020 2020 2020  t.Table().      
+000015f0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00001600: 7454 7275 6528 6973 696e 7374 616e 6365  tTrue(isinstance
+00001610: 2874 2c20 6c74 2e53 6571 7565 6e63 6529  (t, lt.Sequence)
+00001620: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+00001630: 7365 6c66 2e73 7562 5465 7374 2822 6368  self.subTest("ch
+00001640: 6563 6b20 7468 6174 2049 6e64 6578 2069  eck that Index i
+00001650: 7320 7265 636f 676e 697a 6564 2061 7320  s recognized as 
+00001660: 4d61 7070 696e 6720 7479 7065 2229 3a0a  Mapping type"):.
+00001670: 2020 2020 2020 2020 2020 2020 742e 6372              t.cr
+00001680: 6561 7465 5f69 6e64 6578 2822 7822 290a  eate_index("x").
+00001690: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000016a0: 2e61 7373 6572 7454 7275 6528 6973 696e  .assertTrue(isin
+000016b0: 7374 616e 6365 2874 2e67 6574 5f69 6e64  stance(t.get_ind
+000016c0: 6578 2827 7827 292c 206c 742e 4d61 7070  ex('x'), lt.Mapp
+000016d0: 696e 6729 290a 0a20 2020 2020 2020 2023  ing))..        #
+000016e0: 206d 616b 6520 7375 7265 2067 6574 5f69   make sure get_i
+000016f0: 6e64 6578 2072 6574 7572 6e73 2061 2072  ndex returns a r
+00001700: 6561 642d 6f6e 6c79 2061 6363 6573 7320  ead-only access 
+00001710: 746f 2074 6865 2075 6e64 6572 6c79 696e  to the underlyin
+00001720: 6720 696e 6465 780a 2020 2020 2020 2020  g index.        
+00001730: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00001740: 7428 2263 6865 636b 2074 6861 7420 6765  t("check that ge
+00001750: 745f 696e 6465 7820 7265 7475 726e 7320  t_index returns 
+00001760: 6120 7265 6164 2d6f 6e6c 7920 6163 6365  a read-only acce
+00001770: 7373 2074 6f20 7468 6520 756e 6465 726c  ss to the underl
+00001780: 7969 6e67 2069 6e64 6578 2229 3a0a 2020  ying index"):.  
+00001790: 2020 2020 2020 2020 2020 7769 7468 2073            with s
+000017a0: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
+000017b0: 286c 742e 5265 6164 6f6e 6c79 496e 6465  (lt.ReadonlyInde
+000017c0: 7841 6363 6573 7345 7272 6f72 293a 0a20  xAccessError):. 
+000017d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000017e0: 2e67 6574 5f69 6e64 6578 2822 7822 295b  .get_index("x")[
+000017f0: 2761 275d 203d 2031 3030 0a0a 0a64 6566  'a'] = 100...def
+00001800: 2061 6e6e 6f75 6e63 655f 7465 7374 2866   announce_test(f
+00001810: 6e29 3a0a 2020 2020 6465 6620 5f69 6e6e  n):.    def _inn
+00001820: 6572 282a 6172 6773 293a 0a20 2020 2020  er(*args):.     
+00001830: 2020 2070 7269 6e74 2822 5c6e 2220 2b20     print("\n" + 
+00001840: 222d 2220 2a20 3530 290a 2020 2020 2020  "-" * 50).      
+00001850: 2020 7072 696e 7428 6622 7b74 7970 6528    print(f"{type(
+00001860: 6172 6773 5b30 5d29 2e5f 5f6e 616d 655f  args[0]).__name_
+00001870: 5f7d 2e7b 666e 2e5f 5f6e 616d 655f 5f7d  _}.{fn.__name__}
+00001880: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
+00001890: 6e20 666e 282a 6172 6773 290a 0a20 2020  n fn(*args)..   
+000018a0: 2072 6574 7572 6e20 5f69 6e6e 6572 0a0a   return _inner..
+000018b0: 0a64 6566 206d 616b 655f 7465 7374 5f63  .def make_test_c
+000018c0: 6c61 7373 282a 636c 6173 7365 7329 3a0a  lass(*classes):.
+000018d0: 0a20 2020 2063 6c61 7373 5f6e 616d 6520  .    class_name 
+000018e0: 3d20 225f 222e 6a6f 696e 2863 2e5f 5f6e  = "_".join(c.__n
+000018f0: 616d 655f 5f20 666f 7220 6320 696e 2063  ame__ for c in c
+00001900: 6c61 7373 6573 290a 2020 2020 6966 206e  lasses).    if n
+00001910: 6f74 2069 7373 7562 636c 6173 7328 636c  ot issubclass(cl
+00001920: 6173 7365 735b 305d 2c20 756e 6974 7465  asses[0], unitte
+00001930: 7374 2e54 6573 7443 6173 6529 3a0a 2020  st.TestCase):.  
+00001940: 2020 2020 2020 636c 7320 3d20 7479 7065        cls = type
+00001950: 2863 6c61 7373 5f6e 616d 652c 2028 756e  (class_name, (un
+00001960: 6974 7465 7374 2e54 6573 7443 6173 652c  ittest.TestCase,
+00001970: 202a 636c 6173 7365 7329 2c20 7b7d 290a   *classes), {}).
+00001980: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00001990: 2020 636c 7320 3d20 7479 7065 2863 6c61    cls = type(cla
+000019a0: 7373 5f6e 616d 652c 2074 7570 6c65 2863  ss_name, tuple(c
+000019b0: 6c61 7373 6573 292c 207b 7d29 0a20 2020  lasses), {}).   
+000019c0: 2066 6f72 2061 7474 7220 696e 2064 6972   for attr in dir
+000019d0: 2863 6c73 293a 0a20 2020 2020 2020 2061  (cls):.        a
+000019e0: 7474 7276 616c 7565 203d 2067 6574 6174  ttrvalue = getat
+000019f0: 7472 2863 6c73 2c20 6174 7472 290a 2020  tr(cls, attr).  
+00001a00: 2020 2020 2020 6966 2061 7474 722e 7374        if attr.st
+00001a10: 6172 7473 7769 7468 2822 7465 7374 5f22  artswith("test_"
+00001a20: 2920 616e 6420 6361 6c6c 6162 6c65 2861  ) and callable(a
+00001a30: 7474 7276 616c 7565 293a 0a20 2020 2020  ttrvalue):.     
+00001a40: 2020 2020 2020 2073 6574 6174 7472 2863         setattr(c
+00001a50: 6c73 2c20 6174 7472 2c20 616e 6e6f 756e  ls, attr, announ
+00001a60: 6365 5f74 6573 7428 6174 7472 7661 6c75  ce_test(attrvalu
+00001a70: 6529 290a 2020 2020 676c 6f62 616c 7328  e)).    globals(
+00001a80: 295b 636c 732e 5f5f 6e61 6d65 5f5f 5d20  )[cls.__name__] 
+00001a90: 3d20 636c 730a 0a0a 6465 6620 6d61 6b65  = cls...def make
+00001aa0: 5f74 6573 745f 636c 6173 7365 7328 636c  _test_classes(cl
+00001ab0: 7329 3a0a 2020 2020 6d61 6b65 5f74 6573  s):.    make_tes
+00001ac0: 745f 636c 6173 7328 636c 732c 2055 7369  t_class(cls, Usi
+00001ad0: 6e67 4461 7461 4f62 6a65 6374 7329 0a20  ngDataObjects). 
+00001ae0: 2020 206d 616b 655f 7465 7374 5f63 6c61     make_test_cla
+00001af0: 7373 2863 6c73 2c20 5573 696e 674e 616d  ss(cls, UsingNam
+00001b00: 6564 7475 706c 6573 290a 2020 2020 6d61  edtuples).    ma
+00001b10: 6b65 5f74 6573 745f 636c 6173 7328 636c  ke_test_class(cl
+00001b20: 732c 2055 7369 6e67 5479 7069 6e67 4e61  s, UsingTypingNa
+00001b30: 6d65 6454 7570 6c65 290a 2020 2020 6d61  medTuple).    ma
+00001b40: 6b65 5f74 6573 745f 636c 6173 7328 636c  ke_test_class(cl
+00001b50: 732c 2055 7369 6e67 536c 6f74 7465 644f  s, UsingSlottedO
+00001b60: 626a 6563 7473 290a 2020 2020 6966 2053  bjects).    if S
+00001b70: 6c6f 7474 6564 5769 7468 4469 6374 2069  lottedWithDict i
+00001b80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00001b90: 2020 2020 6d61 6b65 5f74 6573 745f 636c      make_test_cl
+00001ba0: 6173 7328 636c 732c 2055 7369 6e67 536c  ass(cls, UsingSl
+00001bb0: 6f74 7465 6457 6974 6844 6963 744f 626a  ottedWithDictObj
+00001bc0: 6563 7473 290a 2020 2020 6d61 6b65 5f74  ects).    make_t
+00001bd0: 6573 745f 636c 6173 7328 636c 732c 2055  est_class(cls, U
+00001be0: 7369 6e67 5369 6d70 6c65 4e61 6d65 7370  singSimpleNamesp
+00001bf0: 6163 6529 0a20 2020 2069 6620 6461 7461  ace).    if data
+00001c00: 636c 6173 7365 7320 6973 206e 6f74 204e  classes is not N
+00001c10: 6f6e 653a 0a20 2020 2020 2020 206d 616b  one:.        mak
+00001c20: 655f 7465 7374 5f63 6c61 7373 2863 6c73  e_test_class(cls
+00001c30: 2c20 5573 696e 6744 6174 6163 6c61 7373  , UsingDataclass
+00001c40: 6573 290a 2020 2020 6966 2070 7964 616e  es).    if pydan
+00001c50: 7469 6320 6973 206e 6f74 204e 6f6e 653a  tic is not None:
+00001c60: 0a20 2020 2020 2020 206d 616b 655f 7465  .        make_te
+00001c70: 7374 5f63 6c61 7373 2863 6c73 2c20 5573  st_class(cls, Us
+00001c80: 696e 6750 7964 616e 7469 634d 6f64 656c  ingPydanticModel
+00001c90: 290a 2020 2020 2020 2020 6d61 6b65 5f74  ).        make_t
+00001ca0: 6573 745f 636c 6173 7328 636c 732c 2055  est_class(cls, U
+00001cb0: 7369 6e67 5079 6461 6e74 6963 496d 6d75  singPydanticImmu
+00001cc0: 7461 626c 654d 6f64 656c 290a 2020 2020  tableModel).    
+00001cd0: 2020 2020 6d61 6b65 5f74 6573 745f 636c      make_test_cl
+00001ce0: 6173 7328 636c 732c 2055 7369 6e67 5079  ass(cls, UsingPy
+00001cf0: 6461 6e74 6963 4f52 4d4d 6f64 656c 290a  danticORMModel).
+00001d00: 2020 2020 6966 2061 7474 7220 6973 206e      if attr is n
+00001d10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00001d20: 206d 616b 655f 7465 7374 5f63 6c61 7373   make_test_class
+00001d30: 2863 6c73 2c20 5573 696e 6741 7474 7243  (cls, UsingAttrC
+00001d40: 6c61 7373 290a 2020 2020 6966 2074 7261  lass).    if tra
+00001d50: 6974 6c65 7473 2069 7320 6e6f 7420 4e6f  itlets is not No
+00001d60: 6e65 3a0a 2020 2020 2020 2020 6d61 6b65  ne:.        make
+00001d70: 5f74 6573 745f 636c 6173 7328 636c 732c  _test_class(cls,
+00001d80: 2055 7369 6e67 5472 6169 746c 6574 7343   UsingTraitletsC
+00001d90: 6c61 7373 290a 2020 2020 6d61 6b65 5f74  lass).    make_t
+00001da0: 6573 745f 636c 6173 7328 636c 732c 2055  est_class(cls, U
+00001db0: 7369 6e67 5479 7069 6e67 5479 7065 6444  singTypingTypedD
+00001dc0: 6963 7429 0a0a 0a63 6c61 7373 2041 6273  ict)...class Abs
+00001dd0: 7472 6163 7443 6f6e 7465 6e74 5479 7065  tractContentType
+00001de0: 4661 6374 6f72 793a 0a20 2020 2064 6174  Factory:.    dat
+00001df0: 615f 6f62 6a65 6374 5f74 7970 653a 204f  a_object_type: O
+00001e00: 7074 696f 6e61 6c5b 7479 7065 5d20 3d20  ptional[type] = 
+00001e10: 4e6f 6e65 0a20 2020 2073 746f 7261 6765  None.    storage
+00001e20: 5f73 7570 706f 7274 735f 6164 645f 6669  _supports_add_fi
+00001e30: 656c 6420 3d20 5472 7565 0a20 2020 2073  eld = True.    s
+00001e40: 746f 7261 6765 5f69 735f 6d75 7461 626c  torage_is_mutabl
+00001e50: 6520 3d20 5472 7565 0a0a 2020 2020 4063  e = True..    @c
+00001e60: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+00001e70: 6566 206d 616b 655f 6461 7461 5f6f 626a  ef make_data_obj
+00001e80: 6563 7428 636c 732c 2061 2c20 622c 2063  ect(cls, a, b, c
+00001e90: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00001ea0: 6e20 636c 732e 6461 7461 5f6f 626a 6563  n cls.data_objec
+00001eb0: 745f 7479 7065 2861 3d61 2c20 623d 622c  t_type(a=a, b=b,
+00001ec0: 2063 3d63 290a 0a0a 636c 6173 7320 5573   c=c)...class Us
+00001ed0: 696e 6744 6174 614f 626a 6563 7473 2841  ingDataObjects(A
+00001ee0: 6273 7472 6163 7443 6f6e 7465 6e74 5479  bstractContentTy
+00001ef0: 7065 4661 6374 6f72 7929 3a0a 2020 2020  peFactory):.    
+00001f00: 6461 7461 5f6f 626a 6563 745f 7479 7065  data_object_type
+00001f10: 203d 206c 742e 4461 7461 4f62 6a65 6374   = lt.DataObject
+00001f20: 0a20 2020 2073 746f 7261 6765 5f69 735f  .    storage_is_
+00001f30: 6d75 7461 626c 6520 3d20 4661 6c73 650a  mutable = False.
+00001f40: 0a0a 636c 6173 7320 5573 696e 674e 616d  ..class UsingNam
+00001f50: 6564 7475 706c 6573 2841 6273 7472 6163  edtuples(Abstrac
+00001f60: 7443 6f6e 7465 6e74 5479 7065 4661 6374  tContentTypeFact
+00001f70: 6f72 7929 3a0a 2020 2020 6461 7461 5f6f  ory):.    data_o
+00001f80: 626a 6563 745f 7479 7065 203d 2044 6174  bject_type = Dat
+00001f90: 6154 7570 6c65 0a20 2020 2073 746f 7261  aTuple.    stora
+00001fa0: 6765 5f73 7570 706f 7274 735f 6164 645f  ge_supports_add_
+00001fb0: 6669 656c 6420 3d20 4661 6c73 650a 2020  field = False.  
+00001fc0: 2020 7374 6f72 6167 655f 6973 5f6d 7574    storage_is_mut
+00001fd0: 6162 6c65 203d 2046 616c 7365 0a0a 0a63  able = False...c
+00001fe0: 6c61 7373 2055 7369 6e67 536c 6f74 7465  lass UsingSlotte
+00001ff0: 644f 626a 6563 7473 2841 6273 7472 6163  dObjects(Abstrac
+00002000: 7443 6f6e 7465 6e74 5479 7065 4661 6374  tContentTypeFact
+00002010: 6f72 7929 3a0a 2020 2020 6461 7461 5f6f  ory):.    data_o
+00002020: 626a 6563 745f 7479 7065 203d 2053 6c6f  bject_type = Slo
+00002030: 7474 6564 0a20 2020 2073 746f 7261 6765  tted.    storage
+00002040: 5f73 7570 706f 7274 735f 6164 645f 6669  _supports_add_fi
+00002050: 656c 6420 3d20 4661 6c73 650a 0a0a 6966  eld = False...if
+00002060: 2053 6c6f 7474 6564 5769 7468 4469 6374   SlottedWithDict
+00002070: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00002080: 2020 636c 6173 7320 5573 696e 6753 6c6f    class UsingSlo
+00002090: 7474 6564 5769 7468 4469 6374 4f62 6a65  ttedWithDictObje
+000020a0: 6374 7328 4162 7374 7261 6374 436f 6e74  cts(AbstractCont
+000020b0: 656e 7454 7970 6546 6163 746f 7279 293a  entTypeFactory):
+000020c0: 0a20 2020 2020 2020 2064 6174 615f 6f62  .        data_ob
+000020d0: 6a65 6374 5f74 7970 6520 3d20 536c 6f74  ject_type = Slot
+000020e0: 7465 6457 6974 6844 6963 740a 2020 2020  tedWithDict.    
+000020f0: 2020 2020 7374 6f72 6167 655f 7375 7070      storage_supp
+00002100: 6f72 7473 5f61 6464 5f66 6965 6c64 203d  orts_add_field =
+00002110: 2046 616c 7365 0a65 6c73 653a 0a20 2020   False.else:.   
+00002120: 2055 7369 6e67 536c 6f74 7465 6457 6974   UsingSlottedWit
+00002130: 6844 6963 744f 626a 6563 7473 203d 2041  hDictObjects = A
+00002140: 6273 7472 6163 7443 6f6e 7465 6e74 5479  bstractContentTy
+00002150: 7065 4661 6374 6f72 790a 0a0a 636c 6173  peFactory...clas
+00002160: 7320 5573 696e 6753 696d 706c 654e 616d  s UsingSimpleNam
+00002170: 6573 7061 6365 2841 6273 7472 6163 7443  espace(AbstractC
+00002180: 6f6e 7465 6e74 5479 7065 4661 6374 6f72  ontentTypeFactor
+00002190: 7929 3a0a 2020 2020 6461 7461 5f6f 626a  y):.    data_obj
+000021a0: 6563 745f 7479 7065 203d 2053 696d 706c  ect_type = Simpl
+000021b0: 654e 616d 6573 7061 6365 0a0a 0a69 6620  eNamespace...if 
+000021c0: 6461 7461 636c 6173 7365 7320 6973 206e  dataclasses is n
+000021d0: 6f74 204e 6f6e 653a 0a20 2020 2063 6c61  ot None:.    cla
+000021e0: 7373 2055 7369 6e67 4461 7461 636c 6173  ss UsingDataclas
+000021f0: 7365 7328 4162 7374 7261 6374 436f 6e74  ses(AbstractCont
+00002200: 656e 7454 7970 6546 6163 746f 7279 293a  entTypeFactory):
+00002210: 0a20 2020 2020 2020 2064 6174 615f 6f62  .        data_ob
+00002220: 6a65 6374 5f74 7970 6520 3d20 4461 7461  ject_type = Data
+00002230: 4461 7461 636c 6173 730a 656c 7365 3a0a  Dataclass.else:.
+00002240: 2020 2020 5573 696e 6744 6174 6163 6c61      UsingDatacla
+00002250: 7373 6573 203d 2041 6273 7472 6163 7443  sses = AbstractC
+00002260: 6f6e 7465 6e74 5479 7065 4661 6374 6f72  ontentTypeFactor
+00002270: 790a 0a0a 6966 2070 7964 616e 7469 6320  y...if pydantic 
+00002280: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00002290: 2063 6c61 7373 2055 7369 6e67 5079 6461   class UsingPyda
+000022a0: 6e74 6963 4d6f 6465 6c28 4162 7374 7261  nticModel(Abstra
+000022b0: 6374 436f 6e74 656e 7454 7970 6546 6163  ctContentTypeFac
+000022c0: 746f 7279 293a 0a20 2020 2020 2020 2064  tory):.        d
+000022d0: 6174 615f 6f62 6a65 6374 5f74 7970 6520  ata_object_type 
+000022e0: 3d20 4461 7461 5079 6461 6e74 6963 4d6f  = DataPydanticMo
+000022f0: 6465 6c0a 2020 2020 2020 2020 7374 6f72  del.        stor
+00002300: 6167 655f 7375 7070 6f72 7473 5f61 6464  age_supports_add
+00002310: 5f66 6965 6c64 203d 2046 616c 7365 0a0a  _field = False..
+00002320: 2020 2020 636c 6173 7320 5573 696e 6750      class UsingP
+00002330: 7964 616e 7469 6349 6d6d 7574 6162 6c65  ydanticImmutable
+00002340: 4d6f 6465 6c28 4162 7374 7261 6374 436f  Model(AbstractCo
+00002350: 6e74 656e 7454 7970 6546 6163 746f 7279  ntentTypeFactory
+00002360: 293a 0a20 2020 2020 2020 2064 6174 615f  ):.        data_
+00002370: 6f62 6a65 6374 5f74 7970 6520 3d20 4461  object_type = Da
+00002380: 7461 5079 6461 6e74 6963 496d 6d75 7461  taPydanticImmuta
+00002390: 626c 654d 6f64 656c 0a20 2020 2020 2020  bleModel.       
+000023a0: 2073 746f 7261 6765 5f73 7570 706f 7274   storage_support
+000023b0: 735f 6164 645f 6669 656c 6420 3d20 4661  s_add_field = Fa
+000023c0: 6c73 650a 2020 2020 2020 2020 7374 6f72  lse.        stor
+000023d0: 6167 655f 6973 5f6d 7574 6162 6c65 203d  age_is_mutable =
+000023e0: 2046 616c 7365 0a0a 2020 2020 636c 6173   False..    clas
+000023f0: 7320 5573 696e 6750 7964 616e 7469 634f  s UsingPydanticO
+00002400: 524d 4d6f 6465 6c28 4162 7374 7261 6374  RMModel(Abstract
+00002410: 436f 6e74 656e 7454 7970 6546 6163 746f  ContentTypeFacto
+00002420: 7279 293a 0a20 2020 2020 2020 2064 6174  ry):.        dat
+00002430: 615f 6f62 6a65 6374 5f74 7970 6520 3d20  a_object_type = 
+00002440: 4461 7461 5079 6461 6e74 6963 4f52 4d4d  DataPydanticORMM
+00002450: 6f64 656c 0a20 2020 2020 2020 2073 746f  odel.        sto
+00002460: 7261 6765 5f73 7570 706f 7274 735f 6164  rage_supports_ad
+00002470: 645f 6669 656c 6420 3d20 4661 6c73 650a  d_field = False.
+00002480: 0a65 6c73 653a 0a20 2020 2055 7369 6e67  .else:.    Using
+00002490: 5079 6461 6e74 6963 4d6f 6465 6c20 3d20  PydanticModel = 
+000024a0: 4162 7374 7261 6374 436f 6e74 656e 7454  AbstractContentT
+000024b0: 7970 6546 6163 746f 7279 0a20 2020 2055  ypeFactory.    U
+000024c0: 7369 6e67 5079 6461 6e74 6963 496d 6d75  singPydanticImmu
+000024d0: 7461 626c 654d 6f64 656c 203d 2041 6273  tableModel = Abs
+000024e0: 7472 6163 7443 6f6e 7465 6e74 5479 7065  tractContentType
+000024f0: 4661 6374 6f72 790a 2020 2020 5573 696e  Factory.    Usin
+00002500: 6750 7964 616e 7469 634f 524d 4d6f 6465  gPydanticORMMode
+00002510: 6c20 3d20 4162 7374 7261 6374 436f 6e74  l = AbstractCont
+00002520: 656e 7454 7970 6546 6163 746f 7279 0a0a  entTypeFactory..
+00002530: 6966 2061 7474 7220 6973 206e 6f74 204e  if attr is not N
+00002540: 6f6e 653a 0a20 2020 2063 6c61 7373 2055  one:.    class U
+00002550: 7369 6e67 4174 7472 436c 6173 7328 4162  singAttrClass(Ab
 00002560: 7374 7261 6374 436f 6e74 656e 7454 7970  stractContentTyp
-00002570: 6546 6163 746f 7279 293a 0a20 2020 2064  eFactory):.    d
-00002580: 6174 615f 6f62 6a65 6374 5f74 7970 6520  ata_object_type 
-00002590: 3d20 5479 7069 6e67 5479 7065 6444 6963  = TypingTypedDic
-000025a0: 740a 0a20 2020 2040 636c 6173 736d 6574  t..    @classmet
-000025b0: 686f 640a 2020 2020 6465 6620 6d61 6b65  hod.    def make
-000025c0: 5f64 6174 615f 6f62 6a65 6374 2863 6c73  _data_object(cls
-000025d0: 2c20 612c 2062 2c20 6329 3a0a 2020 2020  , a, b, c):.    
-000025e0: 2020 2020 7265 7475 726e 2053 696d 706c      return Simpl
-000025f0: 654e 616d 6573 7061 6365 2861 3d61 2c20  eNamespace(a=a, 
-00002600: 623d 622c 2063 3d63 290a 0a64 6566 206c  b=b, c=c)..def l
-00002610: 6f61 645f 7461 626c 6528 7461 626c 652c  oad_table(table,
-00002620: 2072 6563 5f66 6163 746f 7279 5f66 6e2c   rec_factory_fn,
-00002630: 2074 6162 6c65 5f73 697a 6529 3a0a 2020   table_size):.  
-00002640: 2020 7465 7374 5f73 697a 6520 3d20 7461    test_size = ta
-00002650: 626c 655f 7369 7a65 0a20 2020 2074 6162  ble_size.    tab
-00002660: 6c65 2e69 6e73 6572 745f 6d61 6e79 280a  le.insert_many(.
-00002670: 2020 2020 2020 2020 7265 635f 6661 6374          rec_fact
-00002680: 6f72 795f 666e 2861 612c 2062 622c 2063  ory_fn(aa, bb, c
-00002690: 6329 0a20 2020 2020 2020 2066 6f72 2061  c).        for a
-000026a0: 612c 2062 622c 2063 6320 696e 2069 7465  a, bb, cc in ite
-000026b0: 7274 6f6f 6c73 2e70 726f 6475 6374 2872  rtools.product(r
-000026c0: 616e 6765 2874 6573 745f 7369 7a65 292c  ange(test_size),
-000026d0: 2072 6570 6561 743d 3329 0a20 2020 2029   repeat=3).    )
-000026e0: 0a0a 0a64 6566 206d 616b 655f 7465 7374  ...def make_test
-000026f0: 5f74 6162 6c65 2872 6563 5f66 6163 746f  _table(rec_facto
-00002700: 7279 5f66 6e2c 2074 6162 6c65 5f73 697a  ry_fn, table_siz
-00002710: 6529 3a0a 2020 2020 7461 626c 6520 3d20  e):.    table = 
-00002720: 6c74 2e54 6162 6c65 2829 0a20 2020 206c  lt.Table().    l
-00002730: 6f61 645f 7461 626c 6528 7461 626c 652c  oad_table(table,
-00002740: 2072 6563 5f66 6163 746f 7279 5f66 6e2c   rec_factory_fn,
-00002750: 2074 6162 6c65 5f73 697a 6529 0a20 2020   table_size).   
-00002760: 2072 6574 7572 6e20 7461 626c 650a 0a0a   return table...
-00002770: 6465 6620 6d61 6b65 5f64 6174 616f 626a  def make_dataobj
-00002780: 6563 745f 6672 6f6d 5f6f 6228 7265 6329  ect_from_ob(rec)
-00002790: 3a0a 2020 2020 7265 7475 726e 2053 696d  :.    return Sim
-000027a0: 706c 654e 616d 6573 7061 6365 282a 2a7b  pleNamespace(**{
-000027b0: 6b3a 2067 6574 6174 7472 2872 6563 2c20  k: getattr(rec, 
-000027c0: 6b29 2066 6f72 206b 2069 6e20 6c74 2e5f  k) for k in lt._
-000027d0: 6f62 6a65 6374 5f61 7474 726e 616d 6573  object_attrnames
-000027e0: 2872 6563 297d 290a 0a0a 636c 6173 7320  (rec)})...class 
-000027f0: 5461 626c 6554 7970 6554 6573 7473 2875  TableTypeTests(u
-00002800: 6e69 7474 6573 742e 5465 7374 4361 7365  nittest.TestCase
-00002810: 293a 0a20 2020 2064 6566 2074 6573 745f  ):.    def test_
-00002820: 7479 7065 7328 7365 6c66 293a 0a20 2020  types(self):.   
-00002830: 2020 2020 2066 726f 6d20 636f 6c6c 6563       from collec
-00002840: 7469 6f6e 732e 6162 6320 696d 706f 7274  tions.abc import
-00002850: 2028 4361 6c6c 6162 6c65 2c20 436f 6e74   (Callable, Cont
-00002860: 6169 6e65 722c 2049 7465 7261 626c 652c  ainer, Iterable,
-00002870: 2043 6f6c 6c65 6374 696f 6e2c 204d 6170   Collection, Map
-00002880: 7069 6e67 2c20 5265 7665 7273 6962 6c65  ping, Reversible
-00002890: 2c20 5365 7175 656e 6365 2c20 5369 7a65  , Sequence, Size
-000028a0: 6429 0a0a 2020 2020 2020 2020 7462 6c20  d)..        tbl 
-000028b0: 3d20 6c74 2e54 6162 6c65 2829 0a20 2020  = lt.Table().   
-000028c0: 2020 2020 2074 626c 2e63 7265 6174 655f       tbl.create_
-000028d0: 696e 6465 7828 2269 6478 2229 0a0a 2020  index("idx")..  
-000028e0: 2020 2020 2020 666f 7220 7375 7065 7263        for superc
-000028f0: 6c61 7373 2069 6e20 2843 616c 6c61 626c  lass in (Callabl
-00002900: 652c 2053 697a 6564 2c20 4974 6572 6162  e, Sized, Iterab
-00002910: 6c65 2c20 436f 6e74 6169 6e65 722c 2043  le, Container, C
-00002920: 6f6c 6c65 6374 696f 6e2c 2052 6576 6572  ollection, Rever
-00002930: 7369 626c 652c 2053 6571 7565 6e63 6529  sible, Sequence)
-00002940: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
-00002950: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00002960: 7375 7065 7263 6c61 7373 3d73 7570 6572  superclass=super
-00002970: 636c 6173 7329 3a0a 2020 2020 2020 2020  class):.        
-00002980: 2020 2020 2020 2020 7072 696e 7428 7375          print(su
-00002990: 7065 7263 6c61 7373 2e5f 5f6e 616d 655f  perclass.__name_
-000029a0: 5f29 0a20 2020 2020 2020 2020 2020 2020  _).             
-000029b0: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-000029c0: 7565 2869 7369 6e73 7461 6e63 6528 7462  ue(isinstance(tb
-000029d0: 6c2c 2073 7570 6572 636c 6173 7329 290a  l, superclass)).
-000029e0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-000029f0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-00002a00: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00002a10: 2269 7369 6e73 7461 6e63 6528 5f4f 626a  "isinstance(_Obj
-00002a20: 496e 6465 782c 204d 6170 7069 6e67 2922  Index, Mapping)"
-00002a30: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00002a40: 6c66 2e61 7373 6572 7454 7275 6528 6973  lf.assertTrue(is
-00002a50: 696e 7374 616e 6365 2874 626c 2e5f 696e  instance(tbl._in
-00002a60: 6465 7865 735b 2269 6478 225d 2c20 4d61  dexes["idx"], Ma
-00002a70: 7070 696e 6729 290a 0a20 2020 2020 2020  pping))..       
-00002a80: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00002a90: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00002aa0: 2020 7072 696e 7428 2269 7369 6e73 7461    print("isinsta
-00002ab0: 6e63 6528 5f4f 626a 496e 6465 7857 7261  nce(_ObjIndexWra
-00002ac0: 7070 6572 2c20 4d61 7070 696e 6729 2229  pper, Mapping)")
-00002ad0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00002ae0: 662e 6173 7365 7274 5472 7565 2869 7369  f.assertTrue(isi
-00002af0: 6e73 7461 6e63 6528 7462 6c2e 6279 2e69  nstance(tbl.by.i
-00002b00: 6478 2c20 4d61 7070 696e 6729 290a 0a0a  dx, Mapping))...
-00002b10: 406d 616b 655f 7465 7374 5f63 6c61 7373  @make_test_class
-00002b20: 6573 0a63 6c61 7373 2054 6162 6c65 4372  es.class TableCr
-00002b30: 6561 7465 5465 7374 733a 0a20 2020 2064  eateTests:.    d
-00002b40: 6566 2074 6573 745f 696e 7365 7274 7328  ef test_inserts(
-00002b50: 7365 6c66 293a 0a20 2020 2020 2020 2074  self):.        t
-00002b60: 6162 6c65 203d 206c 742e 5461 626c 6528  able = lt.Table(
-00002b70: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
-00002b80: 696e 7365 7274 2873 656c 662e 6d61 6b65  insert(self.make
-00002b90: 5f64 6174 615f 6f62 6a65 6374 2831 2c20  _data_object(1, 
-00002ba0: 322c 2033 2929 0a20 2020 2020 2020 2074  2, 3)).        t
-00002bb0: 6162 6c65 2e69 6e73 6572 7428 7365 6c66  able.insert(self
-00002bc0: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
-00002bd0: 7428 342c 2035 2c20 3629 290a 2020 2020  t(4, 5, 6)).    
-00002be0: 2020 2020 7461 626c 652e 6372 6561 7465      table.create
-00002bf0: 5f69 6e64 6578 2827 6127 2c20 756e 6971  _index('a', uniq
-00002c00: 7565 3d54 7275 6529 0a20 2020 2020 2020  ue=True).       
-00002c10: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00002c20: 6c28 7365 6c66 2e6d 616b 655f 6461 7461  l(self.make_data
-00002c30: 5f6f 626a 6563 7428 342c 2035 2c20 3629  _object(4, 5, 6)
-00002c40: 2c20 7461 626c 652e 6279 2e61 5b34 5d29  , table.by.a[4])
-00002c50: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
-00002c60: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
-00002c70: 284b 6579 4572 726f 7229 3a0a 2020 2020  (KeyError):.    
-00002c80: 2020 2020 2020 2020 7461 626c 652e 696e          table.in
-00002c90: 7365 7274 2873 656c 662e 6d61 6b65 5f64  sert(self.make_d
-00002ca0: 6174 615f 6f62 6a65 6374 2834 2c20 312c  ata_object(4, 1,
-00002cb0: 2030 2929 0a0a 2020 2020 2020 2020 7769   0))..        wi
-00002cc0: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
-00002cd0: 6973 6573 284b 6579 4572 726f 7229 3a0a  ises(KeyError):.
-00002ce0: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
-00002cf0: 652e 696e 7365 7274 2873 656c 662e 6d61  e.insert(self.ma
-00002d00: 6b65 5f64 6174 615f 6f62 6a65 6374 284e  ke_data_object(N
-00002d10: 6f6e 652c 2031 2c20 3029 290a 0a20 2020  one, 1, 0))..   
-00002d20: 2020 2020 2074 6162 6c65 2e64 656c 6574       table.delet
-00002d30: 655f 696e 6465 7828 2761 2729 0a20 2020  e_index('a').   
-00002d40: 2020 2020 2074 6162 6c65 2e69 6e73 6572       table.inser
-00002d50: 7428 7365 6c66 2e6d 616b 655f 6461 7461  t(self.make_data
-00002d60: 5f6f 626a 6563 7428 342c 2031 2c20 3029  _object(4, 1, 0)
-00002d70: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
-00002d80: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
-00002d90: 7328 4b65 7945 7272 6f72 293a 0a20 2020  s(KeyError):.   
-00002da0: 2020 2020 2020 2020 2074 6162 6c65 2e63           table.c
-00002db0: 7265 6174 655f 696e 6465 7828 2761 272c  reate_index('a',
-00002dc0: 2075 6e69 7175 653d 5472 7565 290a 0a20   unique=True).. 
-00002dd0: 2020 2064 6566 2074 6573 745f 696e 7365     def test_inse
-00002de0: 7274 5f64 6963 7473 2873 656c 6629 3a0a  rt_dicts(self):.
-00002df0: 2020 2020 2020 2020 7461 626c 6520 3d20          table = 
-00002e00: 6c74 2e54 6162 6c65 2829 0a20 2020 2020  lt.Table().     
-00002e10: 2020 2074 6162 6c65 2e69 6e73 6572 7428     table.insert(
-00002e20: 7b22 6122 3a20 312c 2022 6222 3a20 322c  {"a": 1, "b": 2,
-00002e30: 2022 6322 3a20 337d 290a 2020 2020 2020   "c": 3}).      
-00002e40: 2020 7461 626c 652e 696e 7365 7274 287b    table.insert({
-00002e50: 2261 223a 2034 2c20 2262 223a 2035 2c20  "a": 4, "b": 5, 
-00002e60: 2263 223a 2036 7d29 0a20 2020 2020 2020  "c": 6}).       
-00002e70: 2074 6162 6c65 2e63 7265 6174 655f 696e   table.create_in
-00002e80: 6465 7828 2761 272c 2075 6e69 7175 653d  dex('a', unique=
-00002e90: 5472 7565 290a 2020 2020 2020 2020 7265  True).        re
-00002ea0: 6330 2c20 7265 6331 203d 2074 6162 6c65  c0, rec1 = table
-00002eb0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00002ec0: 7365 7274 4571 7561 6c28 7b22 6122 3a20  sertEqual({"a": 
-00002ed0: 312c 2022 6222 3a20 322c 2022 6322 3a20  1, "b": 2, "c": 
-00002ee0: 337d 2c20 7661 7273 2872 6563 3029 290a  3}, vars(rec0)).
-00002ef0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00002f00: 6572 7445 7175 616c 286c 742e 6465 6661  ertEqual(lt.defa
-00002f10: 756c 745f 726f 775f 636c 6173 732c 2074  ult_row_class, t
-00002f20: 7970 6528 7265 6330 2929 0a20 2020 2020  ype(rec0)).     
-00002f30: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00002f40: 7561 6c28 312c 2067 6574 6174 7472 2872  ual(1, getattr(r
-00002f50: 6563 302c 2022 6122 2929 0a0a 2020 2020  ec0, "a"))..    
-00002f60: 2020 2020 2320 696e 7365 7274 2061 206e      # insert a n
-00002f70: 6573 7465 6420 6469 6374 0a20 2020 2020  ested dict.     
-00002f80: 2020 2074 6162 6c65 2e63 6c65 6172 2829     table.clear()
-00002f90: 0a20 2020 2020 2020 2074 6162 6c65 2e69  .        table.i
-00002fa0: 6e73 6572 7428 7b22 6122 3a20 312c 2022  nsert({"a": 1, "
-00002fb0: 6222 3a20 322c 2022 6322 3a20 332c 2022  b": 2, "c": 3, "
-00002fc0: 6422 3a20 7b22 7822 3a20 3130 302c 2022  d": {"x": 100, "
-00002fd0: 7922 3a20 3230 307d 7d29 0a20 2020 2020  y": 200}}).     
-00002fe0: 2020 2074 6162 6c65 2e69 6e73 6572 7428     table.insert(
-00002ff0: 7b22 6122 3a20 342c 2022 6222 3a20 352c  {"a": 4, "b": 5,
-00003000: 2022 6322 3a20 362c 2022 6422 3a20 7b22   "c": 6, "d": {"
-00003010: 7822 3a20 3130 312c 2022 7922 3a20 3230  x": 101, "y": 20
-00003020: 317d 7d29 0a20 2020 2020 2020 2072 6563  1}}).        rec
-00003030: 302c 2072 6563 3120 3d20 7461 626c 650a  0, rec1 = table.
-00003040: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00003050: 6572 7445 7175 616c 2831 3030 2c20 7265  ertEqual(100, re
-00003060: 6330 2e64 2e78 290a 2020 2020 2020 2020  c0.d.x).        
-00003070: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00003080: 2831 3031 2c20 7265 6331 2e64 2e78 290a  (101, rec1.d.x).
-00003090: 0a20 2020 2064 6566 2074 6573 745f 7768  .    def test_wh
-000030a0: 6572 655f 6571 7561 6c73 2873 656c 6629  ere_equals(self)
-000030b0: 3a0a 2020 2020 2020 2020 7465 7374 5f73  :.        test_s
-000030c0: 697a 6520 3d20 3130 0a20 2020 2020 2020  ize = 10.       
-000030d0: 2074 6162 6c65 203d 206d 616b 655f 7465   table = make_te
-000030e0: 7374 5f74 6162 6c65 2873 656c 662e 6d61  st_table(self.ma
-000030f0: 6b65 5f64 6174 615f 6f62 6a65 6374 2c20  ke_data_object, 
-00003100: 7465 7374 5f73 697a 6529 0a0a 2020 2020  test_size)..    
-00003110: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00003120: 7175 616c 2874 6573 745f 7369 7a65 2a74  qual(test_size*t
-00003130: 6573 745f 7369 7a65 2c20 6c65 6e28 7461  est_size, len(ta
-00003140: 626c 652e 7768 6572 6528 613d 3529 2929  ble.where(a=5)))
-00003150: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00003160: 7365 7274 4571 7561 6c28 302c 206c 656e  sertEqual(0, len
-00003170: 2874 6162 6c65 2e77 6865 7265 2861 3d2d  (table.where(a=-
-00003180: 3129 2929 0a0a 2020 2020 6465 6620 7465  1)))..    def te
-00003190: 7374 5f77 6865 7265 5f65 7175 616c 735f  st_where_equals_
-000031a0: 6e6f 6e65 2873 656c 6629 3a0a 2020 2020  none(self):.    
-000031b0: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
-000031c0: 3130 0a20 2020 2020 2020 2074 6162 6c65  10.        table
-000031d0: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
-000031e0: 6c65 2873 656c 662e 6d61 6b65 5f64 6174  le(self.make_dat
-000031f0: 615f 6f62 6a65 6374 2c20 7465 7374 5f73  a_object, test_s
-00003200: 697a 6529 0a0a 2020 2020 2020 2020 7365  ize)..        se
-00003210: 6c66 2e61 7373 6572 7445 7175 616c 2830  lf.assertEqual(0
-00003220: 2c20 6c65 6e28 7461 626c 652e 7768 6572  , len(table.wher
-00003230: 6528 613d 352c 2062 3d74 6573 745f 7369  e(a=5, b=test_si
-00003240: 7a65 2929 290a 0a20 2020 2064 6566 2074  ze)))..    def t
-00003250: 6573 745f 7768 6572 655f 6571 7561 6c73  est_where_equals
-00003260: 5f77 6974 685f 696e 6465 7828 7365 6c66  _with_index(self
-00003270: 293a 0a20 2020 2020 2020 2074 6573 745f  ):.        test_
-00003280: 7369 7a65 203d 2031 300a 2020 2020 2020  size = 10.      
-00003290: 2020 7461 626c 6520 3d20 6d61 6b65 5f74    table = make_t
-000032a0: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
-000032b0: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
-000032c0: 2074 6573 745f 7369 7a65 290a 2020 2020   test_size).    
-000032d0: 2020 2020 7461 626c 652e 6372 6561 7465      table.create
-000032e0: 5f69 6e64 6578 2827 6127 290a 0a20 2020  _index('a')..   
-000032f0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00003300: 4571 7561 6c28 7465 7374 5f73 697a 652a  Equal(test_size*
-00003310: 7465 7374 5f73 697a 652c 206c 656e 2874  test_size, len(t
-00003320: 6162 6c65 2e77 6865 7265 2861 3d35 2929  able.where(a=5))
-00003330: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00003340: 7373 6572 7445 7175 616c 2830 2c20 6c65  ssertEqual(0, le
-00003350: 6e28 7461 626c 652e 7768 6572 6528 613d  n(table.where(a=
-00003360: 2d31 2929 290a 0a20 2020 2064 6566 2074  -1)))..    def t
-00003370: 6573 745f 7768 6572 655f 7261 6e67 6528  est_where_range(
-00003380: 7365 6c66 293a 0a20 2020 2020 2020 2074  self):.        t
-00003390: 6573 745f 7369 7a65 203d 2031 300a 2020  est_size = 10.  
-000033a0: 2020 2020 2020 7461 626c 6520 3d20 6d61        table = ma
-000033b0: 6b65 5f74 6573 745f 7461 626c 6528 7365  ke_test_table(se
-000033c0: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
-000033d0: 6563 742c 2074 6573 745f 7369 7a65 290a  ect, test_size).
-000033e0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-000033f0: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
-00003400: 697a 652a 7465 7374 5f73 697a 652c 206c  ize*test_size, l
-00003410: 656e 2874 6162 6c65 2e77 6865 7265 286c  en(table.where(l
-00003420: 616d 6264 6120 7265 633a 2072 6563 2e61  ambda rec: rec.a
-00003430: 203d 3d20 7265 632e 6229 2929 0a0a 2020   == rec.b)))..  
+00002570: 6546 6163 746f 7279 293a 0a20 2020 2020  eFactory):.     
+00002580: 2020 2064 6174 615f 6f62 6a65 6374 5f74     data_object_t
+00002590: 7970 6520 3d20 4174 7472 436c 6173 730a  ype = AttrClass.
+000025a0: 656c 7365 3a0a 2020 2020 5573 696e 6741  else:.    UsingA
+000025b0: 7474 7243 6c61 7373 203d 2041 6273 7472  ttrClass = Abstr
+000025c0: 6163 7443 6f6e 7465 6e74 5479 7065 4661  actContentTypeFa
+000025d0: 6374 6f72 790a 0a69 6620 7472 6169 746c  ctory..if traitl
+000025e0: 6574 7320 6973 206e 6f74 204e 6f6e 653a  ets is not None:
+000025f0: 0a20 2020 2063 6c61 7373 2055 7369 6e67  .    class Using
+00002600: 5472 6169 746c 6574 7343 6c61 7373 2841  TraitletsClass(A
+00002610: 6273 7472 6163 7443 6f6e 7465 6e74 5479  bstractContentTy
+00002620: 7065 4661 6374 6f72 7929 3a0a 2020 2020  peFactory):.    
+00002630: 2020 2020 6461 7461 5f6f 626a 6563 745f      data_object_
+00002640: 7479 7065 203d 2054 7261 6974 6c65 7473  type = Traitlets
+00002650: 436c 6173 730a 656c 7365 3a0a 2020 2020  Class.else:.    
+00002660: 5573 696e 6754 7261 6974 6c65 7473 436c  UsingTraitletsCl
+00002670: 6173 7320 3d20 4162 7374 7261 6374 436f  ass = AbstractCo
+00002680: 6e74 656e 7454 7970 6546 6163 746f 7279  ntentTypeFactory
+00002690: 0a0a 636c 6173 7320 5573 696e 6754 7970  ..class UsingTyp
+000026a0: 696e 674e 616d 6564 5475 706c 6528 4162  ingNamedTuple(Ab
+000026b0: 7374 7261 6374 436f 6e74 656e 7454 7970  stractContentTyp
+000026c0: 6546 6163 746f 7279 293a 0a20 2020 2064  eFactory):.    d
+000026d0: 6174 615f 6f62 6a65 6374 5f74 7970 6520  ata_object_type 
+000026e0: 3d20 5479 7069 6e67 4e61 6d65 6454 7570  = TypingNamedTup
+000026f0: 6c65 0a20 2020 2073 746f 7261 6765 5f73  le.    storage_s
+00002700: 7570 706f 7274 735f 6164 645f 6669 656c  upports_add_fiel
+00002710: 6420 3d20 4661 6c73 650a 2020 2020 7374  d = False.    st
+00002720: 6f72 6167 655f 6973 5f6d 7574 6162 6c65  orage_is_mutable
+00002730: 203d 2046 616c 7365 0a0a 636c 6173 7320   = False..class 
+00002740: 5573 696e 6754 7970 696e 6754 7970 6564  UsingTypingTyped
+00002750: 4469 6374 2841 6273 7472 6163 7443 6f6e  Dict(AbstractCon
+00002760: 7465 6e74 5479 7065 4661 6374 6f72 7929  tentTypeFactory)
+00002770: 3a0a 2020 2020 6461 7461 5f6f 626a 6563  :.    data_objec
+00002780: 745f 7479 7065 203d 2054 7970 696e 6754  t_type = TypingT
+00002790: 7970 6564 4469 6374 0a0a 2020 2020 4063  ypedDict..    @c
+000027a0: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+000027b0: 6566 206d 616b 655f 6461 7461 5f6f 626a  ef make_data_obj
+000027c0: 6563 7428 636c 732c 2061 2c20 622c 2063  ect(cls, a, b, c
+000027d0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+000027e0: 6e20 5369 6d70 6c65 4e61 6d65 7370 6163  n SimpleNamespac
+000027f0: 6528 613d 612c 2062 3d62 2c20 633d 6329  e(a=a, b=b, c=c)
+00002800: 0a0a 6465 6620 6c6f 6164 5f74 6162 6c65  ..def load_table
+00002810: 2874 6162 6c65 2c20 7265 635f 6661 6374  (table, rec_fact
+00002820: 6f72 795f 666e 2c20 7461 626c 655f 7369  ory_fn, table_si
+00002830: 7a65 293a 0a20 2020 2074 6573 745f 7369  ze):.    test_si
+00002840: 7a65 203d 2074 6162 6c65 5f73 697a 650a  ze = table_size.
+00002850: 2020 2020 7461 626c 652e 696e 7365 7274      table.insert
+00002860: 5f6d 616e 7928 0a20 2020 2020 2020 2072  _many(.        r
+00002870: 6563 5f66 6163 746f 7279 5f66 6e28 6161  ec_factory_fn(aa
+00002880: 2c20 6262 2c20 6363 290a 2020 2020 2020  , bb, cc).      
+00002890: 2020 666f 7220 6161 2c20 6262 2c20 6363    for aa, bb, cc
+000028a0: 2069 6e20 6974 6572 746f 6f6c 732e 7072   in itertools.pr
+000028b0: 6f64 7563 7428 7261 6e67 6528 7465 7374  oduct(range(test
+000028c0: 5f73 697a 6529 2c20 7265 7065 6174 3d33  _size), repeat=3
+000028d0: 290a 2020 2020 290a 0a0a 6465 6620 6d61  ).    )...def ma
+000028e0: 6b65 5f74 6573 745f 7461 626c 6528 7265  ke_test_table(re
+000028f0: 635f 6661 6374 6f72 795f 666e 2c20 7461  c_factory_fn, ta
+00002900: 626c 655f 7369 7a65 293a 0a20 2020 2074  ble_size):.    t
+00002910: 6162 6c65 203d 206c 742e 5461 626c 6528  able = lt.Table(
+00002920: 290a 2020 2020 6c6f 6164 5f74 6162 6c65  ).    load_table
+00002930: 2874 6162 6c65 2c20 7265 635f 6661 6374  (table, rec_fact
+00002940: 6f72 795f 666e 2c20 7461 626c 655f 7369  ory_fn, table_si
+00002950: 7a65 290a 2020 2020 7265 7475 726e 2074  ze).    return t
+00002960: 6162 6c65 0a0a 0a64 6566 206d 616b 655f  able...def make_
+00002970: 6461 7461 6f62 6a65 6374 5f66 726f 6d5f  dataobject_from_
+00002980: 6f62 2872 6563 293a 0a20 2020 2072 6574  ob(rec):.    ret
+00002990: 7572 6e20 5369 6d70 6c65 4e61 6d65 7370  urn SimpleNamesp
+000029a0: 6163 6528 2a2a 7b6b 3a20 6765 7461 7474  ace(**{k: getatt
+000029b0: 7228 7265 632c 206b 2920 666f 7220 6b20  r(rec, k) for k 
+000029c0: 696e 206c 742e 5f6f 626a 6563 745f 6174  in lt._object_at
+000029d0: 7472 6e61 6d65 7328 7265 6329 7d29 0a0a  trnames(rec)})..
+000029e0: 0a63 6c61 7373 2054 6162 6c65 5479 7065  .class TableType
+000029f0: 5465 7374 7328 756e 6974 7465 7374 2e54  Tests(unittest.T
+00002a00: 6573 7443 6173 6529 3a0a 2020 2020 6465  estCase):.    de
+00002a10: 6620 7465 7374 5f74 7970 6573 2873 656c  f test_types(sel
+00002a20: 6629 3a0a 2020 2020 2020 2020 6672 6f6d  f):.        from
+00002a30: 2063 6f6c 6c65 6374 696f 6e73 2e61 6263   collections.abc
+00002a40: 2069 6d70 6f72 7420 2843 616c 6c61 626c   import (Callabl
+00002a50: 652c 2043 6f6e 7461 696e 6572 2c20 4974  e, Container, It
+00002a60: 6572 6162 6c65 2c20 436f 6c6c 6563 7469  erable, Collecti
+00002a70: 6f6e 2c20 4d61 7070 696e 672c 2052 6576  on, Mapping, Rev
+00002a80: 6572 7369 626c 652c 2053 6571 7565 6e63  ersible, Sequenc
+00002a90: 652c 2053 697a 6564 290a 0a20 2020 2020  e, Sized)..     
+00002aa0: 2020 2074 626c 203d 206c 742e 5461 626c     tbl = lt.Tabl
+00002ab0: 6528 290a 2020 2020 2020 2020 7462 6c2e  e().        tbl.
+00002ac0: 6372 6561 7465 5f69 6e64 6578 2822 6964  create_index("id
+00002ad0: 7822 290a 0a20 2020 2020 2020 2066 6f72  x")..        for
+00002ae0: 2073 7570 6572 636c 6173 7320 696e 2028   superclass in (
+00002af0: 4361 6c6c 6162 6c65 2c20 5369 7a65 642c  Callable, Sized,
+00002b00: 2049 7465 7261 626c 652c 2043 6f6e 7461   Iterable, Conta
+00002b10: 696e 6572 2c20 436f 6c6c 6563 7469 6f6e  iner, Collection
+00002b20: 2c20 5265 7665 7273 6962 6c65 2c20 5365  , Reversible, Se
+00002b30: 7175 656e 6365 293a 0a20 2020 2020 2020  quence):.       
+00002b40: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+00002b50: 7562 5465 7374 2873 7570 6572 636c 6173  ubTest(superclas
+00002b60: 733d 7375 7065 7263 6c61 7373 293a 0a20  s=superclass):. 
+00002b70: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00002b80: 7269 6e74 2873 7570 6572 636c 6173 732e  rint(superclass.
+00002b90: 5f5f 6e61 6d65 5f5f 290a 2020 2020 2020  __name__).      
+00002ba0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00002bb0: 7373 6572 7454 7275 6528 6973 696e 7374  ssertTrue(isinst
+00002bc0: 616e 6365 2874 626c 2c20 7375 7065 7263  ance(tbl, superc
+00002bd0: 6c61 7373 2929 0a0a 2020 2020 2020 2020  lass))..        
+00002be0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00002bf0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+00002c00: 2070 7269 6e74 2822 6973 696e 7374 616e   print("isinstan
+00002c10: 6365 285f 4f62 6a49 6e64 6578 2c20 4d61  ce(_ObjIndex, Ma
+00002c20: 7070 696e 6729 2229 0a20 2020 2020 2020  pping)").       
+00002c30: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00002c40: 5472 7565 2869 7369 6e73 7461 6e63 6528  True(isinstance(
+00002c50: 7462 6c2e 5f69 6e64 6578 6573 5b22 6964  tbl._indexes["id
+00002c60: 7822 5d2c 204d 6170 7069 6e67 2929 0a0a  x"], Mapping))..
+00002c70: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00002c80: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+00002c90: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00002ca0: 6973 696e 7374 616e 6365 285f 4f62 6a49  isinstance(_ObjI
+00002cb0: 6e64 6578 5772 6170 7065 722c 204d 6170  ndexWrapper, Map
+00002cc0: 7069 6e67 2922 290a 2020 2020 2020 2020  ping)").        
+00002cd0: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+00002ce0: 7275 6528 6973 696e 7374 616e 6365 2874  rue(isinstance(t
+00002cf0: 626c 2e62 792e 6964 782c 204d 6170 7069  bl.by.idx, Mappi
+00002d00: 6e67 2929 0a0a 0a40 6d61 6b65 5f74 6573  ng))...@make_tes
+00002d10: 745f 636c 6173 7365 730a 636c 6173 7320  t_classes.class 
+00002d20: 5461 626c 6543 7265 6174 6554 6573 7473  TableCreateTests
+00002d30: 3a0a 2020 2020 6465 6620 7465 7374 5f69  :.    def test_i
+00002d40: 6e73 6572 7473 2873 656c 6629 3a0a 2020  nserts(self):.  
+00002d50: 2020 2020 2020 7461 626c 6520 3d20 6c74        table = lt
+00002d60: 2e54 6162 6c65 2829 0a20 2020 2020 2020  .Table().       
+00002d70: 2074 6162 6c65 2e69 6e73 6572 7428 7365   table.insert(se
+00002d80: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
+00002d90: 6563 7428 312c 2032 2c20 3329 290a 2020  ect(1, 2, 3)).  
+00002da0: 2020 2020 2020 7461 626c 652e 696e 7365        table.inse
+00002db0: 7274 2873 656c 662e 6d61 6b65 5f64 6174  rt(self.make_dat
+00002dc0: 615f 6f62 6a65 6374 2834 2c20 352c 2036  a_object(4, 5, 6
+00002dd0: 2929 0a20 2020 2020 2020 2074 6162 6c65  )).        table
+00002de0: 2e63 7265 6174 655f 696e 6465 7828 2761  .create_index('a
+00002df0: 272c 2075 6e69 7175 653d 5472 7565 290a  ', unique=True).
+00002e00: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00002e10: 6572 7445 7175 616c 2873 656c 662e 6d61  ertEqual(self.ma
+00002e20: 6b65 5f64 6174 615f 6f62 6a65 6374 2834  ke_data_object(4
+00002e30: 2c20 352c 2036 292c 2074 6162 6c65 2e62  , 5, 6), table.b
+00002e40: 792e 615b 345d 290a 0a20 2020 2020 2020  y.a[4])..       
+00002e50: 2077 6974 6820 7365 6c66 2e61 7373 6572   with self.asser
+00002e60: 7452 6169 7365 7328 4b65 7945 7272 6f72  tRaises(KeyError
+00002e70: 293a 0a20 2020 2020 2020 2020 2020 2074  ):.            t
+00002e80: 6162 6c65 2e69 6e73 6572 7428 7365 6c66  able.insert(self
+00002e90: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
+00002ea0: 7428 342c 2031 2c20 3029 290a 0a20 2020  t(4, 1, 0))..   
+00002eb0: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
+00002ec0: 7373 6572 7452 6169 7365 7328 4b65 7945  ssertRaises(KeyE
+00002ed0: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
+00002ee0: 2020 2074 6162 6c65 2e69 6e73 6572 7428     table.insert(
+00002ef0: 7365 6c66 2e6d 616b 655f 6461 7461 5f6f  self.make_data_o
+00002f00: 626a 6563 7428 4e6f 6e65 2c20 312c 2030  bject(None, 1, 0
+00002f10: 2929 0a0a 2020 2020 2020 2020 7461 626c  ))..        tabl
+00002f20: 652e 6465 6c65 7465 5f69 6e64 6578 2827  e.delete_index('
+00002f30: 6127 290a 2020 2020 2020 2020 7461 626c  a').        tabl
+00002f40: 652e 696e 7365 7274 2873 656c 662e 6d61  e.insert(self.ma
+00002f50: 6b65 5f64 6174 615f 6f62 6a65 6374 2834  ke_data_object(4
+00002f60: 2c20 312c 2030 2929 0a0a 2020 2020 2020  , 1, 0))..      
+00002f70: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
+00002f80: 7274 5261 6973 6573 284b 6579 4572 726f  rtRaises(KeyErro
+00002f90: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00002fa0: 7461 626c 652e 6372 6561 7465 5f69 6e64  table.create_ind
+00002fb0: 6578 2827 6127 2c20 756e 6971 7565 3d54  ex('a', unique=T
+00002fc0: 7275 6529 0a0a 2020 2020 6465 6620 7465  rue)..    def te
+00002fd0: 7374 5f69 6e73 6572 745f 6469 6374 7328  st_insert_dicts(
+00002fe0: 7365 6c66 293a 0a20 2020 2020 2020 2074  self):.        t
+00002ff0: 6162 6c65 203d 206c 742e 5461 626c 6528  able = lt.Table(
+00003000: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
+00003010: 696e 7365 7274 287b 2261 223a 2031 2c20  insert({"a": 1, 
+00003020: 2262 223a 2032 2c20 2263 223a 2033 7d29  "b": 2, "c": 3})
+00003030: 0a20 2020 2020 2020 2074 6162 6c65 2e69  .        table.i
+00003040: 6e73 6572 7428 7b22 6122 3a20 342c 2022  nsert({"a": 4, "
+00003050: 6222 3a20 352c 2022 6322 3a20 367d 290a  b": 5, "c": 6}).
+00003060: 2020 2020 2020 2020 7461 626c 652e 6372          table.cr
+00003070: 6561 7465 5f69 6e64 6578 2827 6127 2c20  eate_index('a', 
+00003080: 756e 6971 7565 3d54 7275 6529 0a20 2020  unique=True).   
+00003090: 2020 2020 2072 6563 302c 2072 6563 3120       rec0, rec1 
+000030a0: 3d20 7461 626c 650a 2020 2020 2020 2020  = table.        
+000030b0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000030c0: 287b 2261 223a 2031 2c20 2262 223a 2032  ({"a": 1, "b": 2
+000030d0: 2c20 2263 223a 2033 7d2c 2076 6172 7328  , "c": 3}, vars(
+000030e0: 7265 6330 2929 0a20 2020 2020 2020 2073  rec0)).        s
+000030f0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00003100: 6c74 2e64 6566 6175 6c74 5f72 6f77 5f63  lt.default_row_c
+00003110: 6c61 7373 2c20 7479 7065 2872 6563 3029  lass, type(rec0)
+00003120: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00003130: 7373 6572 7445 7175 616c 2831 2c20 6765  ssertEqual(1, ge
+00003140: 7461 7474 7228 7265 6330 2c20 2261 2229  tattr(rec0, "a")
+00003150: 290a 0a20 2020 2020 2020 2023 2069 6e73  )..        # ins
+00003160: 6572 7420 6120 6e65 7374 6564 2064 6963  ert a nested dic
+00003170: 740a 2020 2020 2020 2020 7461 626c 652e  t.        table.
+00003180: 636c 6561 7228 290a 2020 2020 2020 2020  clear().        
+00003190: 7461 626c 652e 696e 7365 7274 287b 2261  table.insert({"a
+000031a0: 223a 2031 2c20 2262 223a 2032 2c20 2263  ": 1, "b": 2, "c
+000031b0: 223a 2033 2c20 2264 223a 207b 2278 223a  ": 3, "d": {"x":
+000031c0: 2031 3030 2c20 2279 223a 2032 3030 7d7d   100, "y": 200}}
+000031d0: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
+000031e0: 696e 7365 7274 287b 2261 223a 2034 2c20  insert({"a": 4, 
+000031f0: 2262 223a 2035 2c20 2263 223a 2036 2c20  "b": 5, "c": 6, 
+00003200: 2264 223a 207b 2278 223a 2031 3031 2c20  "d": {"x": 101, 
+00003210: 2279 223a 2032 3031 7d7d 290a 2020 2020  "y": 201}}).    
+00003220: 2020 2020 7265 6330 2c20 7265 6331 203d      rec0, rec1 =
+00003230: 2074 6162 6c65 0a20 2020 2020 2020 2073   table.        s
+00003240: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00003250: 3130 302c 2072 6563 302e 642e 7829 0a20  100, rec0.d.x). 
+00003260: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00003270: 7274 4571 7561 6c28 3130 312c 2072 6563  rtEqual(101, rec
+00003280: 312e 642e 7829 0a0a 2020 2020 6465 6620  1.d.x)..    def 
+00003290: 7465 7374 5f77 6865 7265 5f65 7175 616c  test_where_equal
+000032a0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+000032b0: 2074 6573 745f 7369 7a65 203d 2031 300a   test_size = 10.
+000032c0: 2020 2020 2020 2020 7461 626c 6520 3d20          table = 
+000032d0: 6d61 6b65 5f74 6573 745f 7461 626c 6528  make_test_table(
+000032e0: 7365 6c66 2e6d 616b 655f 6461 7461 5f6f  self.make_data_o
+000032f0: 626a 6563 742c 2074 6573 745f 7369 7a65  bject, test_size
+00003300: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00003310: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
+00003320: 5f73 697a 652a 7465 7374 5f73 697a 652c  _size*test_size,
+00003330: 206c 656e 2874 6162 6c65 2e77 6865 7265   len(table.where
+00003340: 2861 3d35 2929 290a 2020 2020 2020 2020  (a=5))).        
+00003350: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00003360: 2830 2c20 6c65 6e28 7461 626c 652e 7768  (0, len(table.wh
+00003370: 6572 6528 613d 2d31 2929 290a 0a20 2020  ere(a=-1)))..   
+00003380: 2064 6566 2074 6573 745f 7768 6572 655f   def test_where_
+00003390: 6571 7561 6c73 5f6e 6f6e 6528 7365 6c66  equals_none(self
+000033a0: 293a 0a20 2020 2020 2020 2074 6573 745f  ):.        test_
+000033b0: 7369 7a65 203d 2031 300a 2020 2020 2020  size = 10.      
+000033c0: 2020 7461 626c 6520 3d20 6d61 6b65 5f74    table = make_t
+000033d0: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
+000033e0: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
+000033f0: 2074 6573 745f 7369 7a65 290a 0a20 2020   test_size)..   
+00003400: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00003410: 4571 7561 6c28 302c 206c 656e 2874 6162  Equal(0, len(tab
+00003420: 6c65 2e77 6865 7265 2861 3d35 2c20 623d  le.where(a=5, b=
+00003430: 7465 7374 5f73 697a 6529 2929 0a0a 2020  test_size)))..  
 00003440: 2020 6465 6620 7465 7374 5f77 6865 7265    def test_where
-00003450: 5f63 6f6d 7061 7261 746f 7228 7365 6c66  _comparator(self
-00003460: 293a 0a20 2020 2020 2020 2074 6573 745f  ):.        test_
-00003470: 7369 7a65 203d 2031 300a 2020 2020 2020  size = 10.      
-00003480: 2020 7461 626c 6520 3d20 6d61 6b65 5f74    table = make_t
-00003490: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
-000034a0: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
-000034b0: 2074 6573 745f 7369 7a65 290a 0a20 2020   test_size)..   
-000034c0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000034d0: 4571 7561 6c28 7465 7374 5f73 697a 652a  Equal(test_size*
-000034e0: 7465 7374 5f73 697a 652a 342c 206c 656e  test_size*4, len
-000034f0: 2874 6162 6c65 2e77 6865 7265 2861 3d6c  (table.where(a=l
-00003500: 742e 5461 626c 652e 6c74 2834 2929 2929  t.Table.lt(4))))
-00003510: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00003520: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
-00003530: 697a 652a 7465 7374 5f73 697a 652a 2834  ize*test_size*(4
-00003540: 2b31 292c 206c 656e 2874 6162 6c65 2e77  +1), len(table.w
-00003550: 6865 7265 2861 3d6c 742e 5461 626c 652e  here(a=lt.Table.
-00003560: 6c65 2834 2929 2929 0a20 2020 2020 2020  le(4)))).       
-00003570: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00003580: 6c28 7465 7374 5f73 697a 652a 7465 7374  l(test_size*test
-00003590: 5f73 697a 652a 2874 6573 745f 7369 7a65  _size*(test_size
-000035a0: 2d34 2d31 292c 206c 656e 2874 6162 6c65  -4-1), len(table
-000035b0: 2e77 6865 7265 2861 3d6c 742e 5461 626c  .where(a=lt.Tabl
-000035c0: 652e 6774 2834 2929 2929 0a20 2020 2020  e.gt(4)))).     
-000035d0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000035e0: 7561 6c28 7465 7374 5f73 697a 652a 7465  ual(test_size*te
-000035f0: 7374 5f73 697a 652a 2874 6573 745f 7369  st_size*(test_si
-00003600: 7a65 2d34 292c 206c 656e 2874 6162 6c65  ze-4), len(table
-00003610: 2e77 6865 7265 2861 3d6c 742e 5461 626c  .where(a=lt.Tabl
-00003620: 652e 6765 2834 2929 2929 0a20 2020 2020  e.ge(4)))).     
-00003630: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00003640: 7561 6c28 7465 7374 5f73 697a 652a 7465  ual(test_size*te
-00003650: 7374 5f73 697a 652a 2874 6573 745f 7369  st_size*(test_si
-00003660: 7a65 2d31 292c 206c 656e 2874 6162 6c65  ze-1), len(table
-00003670: 2e77 6865 7265 2861 3d6c 742e 5461 626c  .where(a=lt.Tabl
-00003680: 652e 6e65 2834 2929 2929 0a20 2020 2020  e.ne(4)))).     
-00003690: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000036a0: 7561 6c28 7465 7374 5f73 697a 652a 7465  ual(test_size*te
-000036b0: 7374 5f73 697a 652c 206c 656e 2874 6162  st_size, len(tab
-000036c0: 6c65 2e77 6865 7265 2861 3d6c 742e 5461  le.where(a=lt.Ta
-000036d0: 626c 652e 6571 2834 2929 2929 0a20 2020  ble.eq(4)))).   
-000036e0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000036f0: 4571 7561 6c28 7465 7374 5f73 697a 652c  Equal(test_size,
-00003700: 206c 656e 2874 6162 6c65 2e77 6865 7265   len(table.where
-00003710: 2861 3d6c 742e 5461 626c 652e 6571 2834  (a=lt.Table.eq(4
-00003720: 292c 2062 3d6c 742e 5461 626c 652e 6571  ), b=lt.Table.eq
-00003730: 2834 2929 2929 0a20 2020 2020 2020 2073  (4)))).        s
-00003740: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00003750: 7465 7374 5f73 697a 652a 7465 7374 5f73  test_size*test_s
-00003760: 697a 652a 342c 206c 656e 2874 6162 6c65  ize*4, len(table
-00003770: 2e77 6865 7265 2861 3d6c 742e 5461 626c  .where(a=lt.Tabl
-00003780: 652e 6265 7477 6565 6e28 332c 2038 2929  e.between(3, 8))
-00003790: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-000037a0: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
-000037b0: 5f73 697a 652a 7465 7374 5f73 697a 652a  _size*test_size*
-000037c0: 342c 206c 656e 2874 6162 6c65 2e77 6865  4, len(table.whe
-000037d0: 7265 2861 3d6c 742e 5461 626c 652e 7769  re(a=lt.Table.wi
-000037e0: 7468 696e 2832 2c20 3529 2929 290a 2020  thin(2, 5)))).  
-000037f0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00003800: 7445 7175 616c 2874 6573 745f 7369 7a65  tEqual(test_size
-00003810: 2a74 6573 745f 7369 7a65 2a33 2c20 6c65  *test_size*3, le
-00003820: 6e28 7461 626c 652e 7768 6572 6528 613d  n(table.where(a=
-00003830: 6c74 2e54 6162 6c65 2e69 6e5f 7261 6e67  lt.Table.in_rang
-00003840: 6528 322c 2035 2929 2929 0a20 2020 2020  e(2, 5)))).     
-00003850: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00003860: 7561 6c28 302c 206c 656e 2874 6162 6c65  ual(0, len(table
-00003870: 2e77 6865 7265 2861 3d6c 742e 5461 626c  .where(a=lt.Tabl
-00003880: 652e 6265 7477 6565 6e28 332c 2033 2929  e.between(3, 3))
-00003890: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-000038a0: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
-000038b0: 5f73 697a 652a 7465 7374 5f73 697a 652c  _size*test_size,
-000038c0: 206c 656e 2874 6162 6c65 2e77 6865 7265   len(table.where
-000038d0: 2861 3d6c 742e 5461 626c 652e 7769 7468  (a=lt.Table.with
-000038e0: 696e 2833 2c20 3329 2929 290a 2020 2020  in(3, 3)))).    
-000038f0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00003900: 7175 616c 2830 2c20 6c65 6e28 7461 626c  qual(0, len(tabl
-00003910: 652e 7768 6572 6528 613d 6c74 2e54 6162  e.where(a=lt.Tab
-00003920: 6c65 2e69 6e5f 7261 6e67 6528 332c 2033  le.in_range(3, 3
-00003930: 2929 2929 0a20 2020 2020 2020 2073 656c  )))).        sel
-00003940: 662e 6173 7365 7274 4571 7561 6c28 7465  f.assertEqual(te
-00003950: 7374 5f73 697a 652a 7465 7374 5f73 697a  st_size*test_siz
-00003960: 652a 342c 206c 656e 2874 6162 6c65 2e77  e*4, len(table.w
-00003970: 6865 7265 2861 3d6c 742e 5461 626c 652e  here(a=lt.Table.
-00003980: 6973 5f69 6e28 5b32 2c20 342c 2036 2c20  is_in([2, 4, 6, 
-00003990: 385d 2929 2929 0a20 2020 2020 2020 2073  8])))).        s
-000039a0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000039b0: 302c 206c 656e 2874 6162 6c65 2e77 6865  0, len(table.whe
-000039c0: 7265 2861 3d6c 742e 5461 626c 652e 6973  re(a=lt.Table.is
-000039d0: 5f69 6e28 5b5d 2929 2929 0a20 2020 2020  _in([])))).     
-000039e0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000039f0: 7561 6c28 7465 7374 5f73 697a 652a 7465  ual(test_size*te
-00003a00: 7374 5f73 697a 652a 2874 6573 745f 7369  st_size*(test_si
-00003a10: 7a65 2d34 292c 206c 656e 2874 6162 6c65  ze-4), len(table
-00003a20: 2e77 6865 7265 2861 3d6c 742e 5461 626c  .where(a=lt.Tabl
-00003a30: 652e 6e6f 745f 696e 285b 322c 2034 2c20  e.not_in([2, 4, 
-00003a40: 362c 2038 5d29 2929 290a 2020 2020 2020  6, 8])))).      
-00003a50: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00003a60: 616c 2874 6573 745f 7369 7a65 2a74 6573  al(test_size*tes
-00003a70: 745f 7369 7a65 2a74 6573 745f 7369 7a65  t_size*test_size
-00003a80: 2c20 6c65 6e28 7461 626c 652e 7768 6572  , len(table.wher
-00003a90: 6528 613d 6c74 2e54 6162 6c65 2e6e 6f74  e(a=lt.Table.not
-00003aa0: 5f69 6e28 5b5d 2929 2929 0a0a 2020 2020  _in([]))))..    
-00003ab0: 2020 2020 2320 6164 6420 6120 7265 636f      # add a reco
-00003ac0: 7264 2063 6f6e 7461 696e 696e 6720 6120  rd containing a 
-00003ad0: 4e6f 6e65 2076 616c 7565 2074 6f20 7465  None value to te
-00003ae0: 7374 2069 735f 6e6f 6e65 2061 6e64 2069  st is_none and i
-00003af0: 735f 6e6f 745f 6e6f 6e65 2063 6f6d 7061  s_not_none compa
-00003b00: 7261 746f 7273 0a20 2020 2020 2020 2074  rators.        t
-00003b10: 6162 6c65 2e69 6e73 6572 7428 7365 6c66  able.insert(self
-00003b20: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
-00003b30: 7428 613d 312c 2062 3d32 2c20 633d 4e6f  t(a=1, b=2, c=No
-00003b40: 6e65 2929 0a20 2020 2020 2020 2073 656c  ne)).        sel
-00003b50: 662e 6173 7365 7274 4571 7561 6c28 312c  f.assertEqual(1,
-00003b60: 206c 656e 2874 6162 6c65 2e77 6865 7265   len(table.where
-00003b70: 2863 3d6c 742e 5461 626c 652e 6973 5f6e  (c=lt.Table.is_n
-00003b80: 6f6e 6528 2929 2929 0a20 2020 2020 2020  one()))).       
-00003b90: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00003ba0: 6c28 7465 7374 5f73 697a 652a 7465 7374  l(test_size*test
-00003bb0: 5f73 697a 652a 7465 7374 5f73 697a 652c  _size*test_size,
-00003bc0: 206c 656e 2874 6162 6c65 2e77 6865 7265   len(table.where
-00003bd0: 2863 3d6c 742e 5461 626c 652e 6973 5f6e  (c=lt.Table.is_n
-00003be0: 6f74 5f6e 6f6e 6528 2929 2929 0a0a 2020  ot_none())))..  
-00003bf0: 2020 2020 2020 2320 6164 6420 6120 7265        # add a re
-00003c00: 636f 7264 2063 6f6e 7461 696e 696e 6720  cord containing 
-00003c10: 6120 6d69 7373 696e 6720 7661 6c75 6520  a missing value 
-00003c20: 746f 2074 6573 7420 6973 5f6e 756c 6c20  to test is_null 
-00003c30: 616e 6420 6973 5f6e 6f74 5f6e 756c 6c20  and is_not_null 
-00003c40: 636f 6d70 6172 6174 6f72 730a 2020 2020  comparators.    
-00003c50: 2020 2020 7461 626c 652e 696e 7365 7274      table.insert
-00003c60: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
-00003c70: 6f62 6a65 6374 2861 3d31 2c20 623d 322c  object(a=1, b=2,
-00003c80: 2063 3d22 2229 290a 2020 2020 2020 2020   c="")).        
-00003c90: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00003ca0: 2832 2c20 6c65 6e28 7461 626c 652e 7768  (2, len(table.wh
-00003cb0: 6572 6528 633d 6c74 2e54 6162 6c65 2e69  ere(c=lt.Table.i
-00003cc0: 735f 6e75 6c6c 2829 2929 290a 2020 2020  s_null()))).    
-00003cd0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00003ce0: 7175 616c 2874 6573 745f 7369 7a65 202a  qual(test_size *
-00003cf0: 2074 6573 745f 7369 7a65 202a 2074 6573   test_size * tes
-00003d00: 745f 7369 7a65 2c20 6c65 6e28 7461 626c  t_size, len(tabl
-00003d10: 652e 7768 6572 6528 633d 6c74 2e54 6162  e.where(c=lt.Tab
-00003d20: 6c65 2e69 735f 6e6f 745f 6e75 6c6c 2829  le.is_not_null()
-00003d30: 2929 290a 0a20 2020 2020 2020 2074 7279  )))..        try
-00003d40: 3a0a 2020 2020 2020 2020 2020 2020 7461  :.            ta
-00003d50: 626c 652e 696e 7365 7274 2873 656c 662e  ble.insert(self.
-00003d60: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
-00003d70: 2861 3d31 2c20 623d 3229 290a 2020 2020  (a=1, b=2)).    
-00003d80: 2020 2020 6578 6365 7074 2054 7970 6545      except TypeE
-00003d90: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
-00003da0: 2020 2320 6e6f 7420 616c 6c20 6461 7461    # not all data
-00003db0: 206f 626a 6563 7420 7479 7065 7320 6265   object types be
-00003dc0: 696e 6720 7465 7374 6564 2073 7570 706f  ing tested suppo
-00003dd0: 7274 206d 6973 7369 6e67 2061 7474 7269  rt missing attri
-00003de0: 6275 7465 730a 2020 2020 2020 2020 2020  butes.          
-00003df0: 2020 7061 7373 0a20 2020 2020 2020 2065    pass.        e
-00003e00: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00003e10: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00003e20: 6c28 332c 206c 656e 2874 6162 6c65 2e77  l(3, len(table.w
-00003e30: 6865 7265 2863 3d6c 742e 5461 626c 652e  here(c=lt.Table.
-00003e40: 6973 5f6e 756c 6c28 2929 2929 0a20 2020  is_null()))).   
-00003e50: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00003e60: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
-00003e70: 697a 6520 2a20 7465 7374 5f73 697a 6520  ize * test_size 
-00003e80: 2a20 7465 7374 5f73 697a 652c 206c 656e  * test_size, len
-00003e90: 2874 6162 6c65 2e77 6865 7265 2863 3d6c  (table.where(c=l
-00003ea0: 742e 5461 626c 652e 6973 5f6e 6f74 5f6e  t.Table.is_not_n
-00003eb0: 756c 6c28 2929 2929 0a0a 2020 2020 6465  ull())))..    de
-00003ec0: 6620 7465 7374 5f77 6865 7265 5f73 7472  f test_where_str
-00003ed0: 5f63 6f6d 7061 7261 746f 7228 7365 6c66  _comparator(self
-00003ee0: 293a 0a20 2020 2020 2020 2075 6e69 636f  ):.        unico
-00003ef0: 6465 5f6e 756d 6265 7273 203d 206c 742e  de_numbers = lt.
-00003f00: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
-00003f10: 7274 2874 6578 7477 7261 702e 6465 6465  rt(textwrap.dede
-00003f20: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
-00003f30: 2020 2020 6e61 6d65 2c63 6f64 655f 7661      name,code_va
-00003f40: 6c75 652c 6e75 6d65 7269 635f 7661 6c75  lue,numeric_valu
-00003f50: 650a 2020 2020 2020 2020 2020 2020 524f  e.            RO
-00003f60: 4d41 4e20 4e55 4d45 5241 4c20 4f4e 452c  MAN NUMERAL ONE,
-00003f70: 3835 3434 2c31 0a20 2020 2020 2020 2020  8544,1.         
-00003f80: 2020 2052 4f4d 414e 204e 554d 4552 414c     ROMAN NUMERAL
-00003f90: 2054 574f 2c38 3534 352c 320a 2020 2020   TWO,8545,2.    
-00003fa0: 2020 2020 2020 2020 524f 4d41 4e20 4e55          ROMAN NU
-00003fb0: 4d45 5241 4c20 5448 5245 452c 3835 3436  MERAL THREE,8546
-00003fc0: 2c33 0a20 2020 2020 2020 2020 2020 2052  ,3.            R
-00003fd0: 4f4d 414e 204e 554d 4552 414c 2046 4f55  OMAN NUMERAL FOU
-00003fe0: 522c 3835 3437 2c34 0a20 2020 2020 2020  R,8547,4.       
-00003ff0: 2020 2020 2052 4f4d 414e 204e 554d 4552       ROMAN NUMER
-00004000: 414c 2046 4956 452c 3835 3438 2c35 0a20  AL FIVE,8548,5. 
-00004010: 2020 2020 2020 2020 2020 2052 4f4d 414e             ROMAN
-00004020: 204e 554d 4552 414c 2053 4958 2c38 3534   NUMERAL SIX,854
-00004030: 392c 360a 2020 2020 2020 2020 2020 2020  9,6.            
-00004040: 524f 4d41 4e20 4e55 4d45 5241 4c20 5345  ROMAN NUMERAL SE
-00004050: 5645 4e2c 3835 3530 2c37 0a20 2020 2020  VEN,8550,7.     
-00004060: 2020 2020 2020 2052 4f4d 414e 204e 554d         ROMAN NUM
-00004070: 4552 414c 2045 4947 4854 2c38 3535 312c  ERAL EIGHT,8551,
-00004080: 380a 2020 2020 2020 2020 2020 2020 524f  8.            RO
-00004090: 4d41 4e20 4e55 4d45 5241 4c20 4e49 4e45  MAN NUMERAL NINE
-000040a0: 2c38 3535 322c 390a 2020 2020 2020 2020  ,8552,9.        
-000040b0: 2020 2020 524f 4d41 4e20 4e55 4d45 5241      ROMAN NUMERA
-000040c0: 4c20 5445 4e2c 3835 3533 2c31 300a 2020  L TEN,8553,10.  
-000040d0: 2020 2020 2020 2020 2020 5355 5045 5253            SUPERS
-000040e0: 4352 4950 5420 5457 4f2c 3137 382c 320a  CRIPT TWO,178,2.
-000040f0: 2020 2020 2020 2020 2020 2020 5355 5045              SUPE
-00004100: 5253 4352 4950 5420 5448 5245 452c 3137  RSCRIPT THREE,17
-00004110: 392c 330a 2020 2020 2020 2020 2020 2020  9,3.            
-00004120: 5355 5045 5253 4352 4950 5420 4f4e 452c  SUPERSCRIPT ONE,
-00004130: 3138 352c 310a 2020 2020 2020 2020 2020  185,1.          
-00004140: 2020 5355 5045 5253 4352 4950 5420 5a45    SUPERSCRIPT ZE
-00004150: 524f 2c38 3330 342c 300a 2020 2020 2020  RO,8304,0.      
-00004160: 2020 2020 2020 5355 5045 5253 4352 4950        SUPERSCRIP
-00004170: 5420 464f 5552 2c38 3330 382c 340a 2020  T FOUR,8308,4.  
-00004180: 2020 2020 2020 2020 2020 5355 5045 5253            SUPERS
-00004190: 4352 4950 5420 4649 5645 2c38 3330 392c  CRIPT FIVE,8309,
-000041a0: 350a 2020 2020 2020 2020 2020 2020 5355  5.            SU
-000041b0: 5045 5253 4352 4950 5420 5349 582c 3833  PERSCRIPT SIX,83
-000041c0: 3130 2c36 0a20 2020 2020 2020 2020 2020  10,6.           
-000041d0: 2053 5550 4552 5343 5249 5054 2053 4556   SUPERSCRIPT SEV
-000041e0: 454e 2c38 3331 312c 370a 2020 2020 2020  EN,8311,7.      
-000041f0: 2020 2020 2020 5355 5045 5253 4352 4950        SUPERSCRIP
-00004200: 5420 4549 4748 542c 3833 3132 2c38 0a20  T EIGHT,8312,8. 
-00004210: 2020 2020 2020 2020 2020 2053 5550 4552             SUPER
-00004220: 5343 5249 5054 204e 494e 452c 3833 3133  SCRIPT NINE,8313
-00004230: 2c39 0a20 2020 2020 2020 2020 2020 2043  ,9.            C
-00004240: 4952 434c 4544 2044 4947 4954 204f 4e45  IRCLED DIGIT ONE
-00004250: 2c39 3331 322c 310a 2020 2020 2020 2020  ,9312,1.        
-00004260: 2020 2020 4349 5243 4c45 4420 4449 4749      CIRCLED DIGI
-00004270: 5420 5457 4f2c 3933 3133 2c32 0a20 2020  T TWO,9313,2.   
-00004280: 2020 2020 2020 2020 2043 4952 434c 4544           CIRCLED
-00004290: 2044 4947 4954 2054 4852 4545 2c39 3331   DIGIT THREE,931
-000042a0: 342c 330a 2020 2020 2020 2020 2020 2020  4,3.            
-000042b0: 4349 5243 4c45 4420 4449 4749 5420 464f  CIRCLED DIGIT FO
-000042c0: 5552 2c39 3331 352c 340a 2020 2020 2020  UR,9315,4.      
-000042d0: 2020 2020 2020 4349 5243 4c45 4420 4449        CIRCLED DI
-000042e0: 4749 5420 4649 5645 2c39 3331 362c 350a  GIT FIVE,9316,5.
-000042f0: 2020 2020 2020 2020 2020 2020 4349 5243              CIRC
-00004300: 4c45 4420 4449 4749 5420 5349 582c 3933  LED DIGIT SIX,93
-00004310: 3137 2c36 0a20 2020 2020 2020 2020 2020  17,6.           
-00004320: 2043 4952 434c 4544 2044 4947 4954 2053   CIRCLED DIGIT S
-00004330: 4556 454e 2c39 3331 382c 370a 2020 2020  EVEN,9318,7.    
-00004340: 2020 2020 2020 2020 4349 5243 4c45 4420          CIRCLED 
-00004350: 4449 4749 5420 4549 4748 542c 3933 3139  DIGIT EIGHT,9319
-00004360: 2c38 0a20 2020 2020 2020 2020 2020 2043  ,8.            C
-00004370: 4952 434c 4544 2044 4947 4954 204e 494e  IRCLED DIGIT NIN
-00004380: 452c 3933 3230 2c39 0a20 2020 2020 2020  E,9320,9.       
-00004390: 2020 2020 2043 4952 434c 4544 2044 4947       CIRCLED DIG
-000043a0: 4954 205a 4552 4f2c 3934 3530 2c30 0a20  IT ZERO,9450,0. 
-000043b0: 2020 2020 2020 2020 2020 2022 2222 2929             """))
-000043c0: 0a0a 2020 2020 2020 2020 6f6e 6573 203d  ..        ones =
-000043d0: 2075 6e69 636f 6465 5f6e 756d 6265 7273   unicode_numbers
-000043e0: 2e77 6865 7265 286e 616d 653d 6c74 2e54  .where(name=lt.T
-000043f0: 6162 6c65 2e65 6e64 7377 6974 6828 224f  able.endswith("O
-00004400: 4e45 2229 290a 2020 2020 2020 2020 7365  NE")).        se
-00004410: 6c66 2e61 7373 6572 7445 7175 616c 2833  lf.assertEqual(3
-00004420: 2c20 6c65 6e28 6f6e 6573 2929 0a0a 2020  , len(ones))..  
-00004430: 2020 2020 2020 7375 7065 7273 203d 2075        supers = u
-00004440: 6e69 636f 6465 5f6e 756d 6265 7273 2e77  nicode_numbers.w
-00004450: 6865 7265 286e 616d 653d 6c74 2e54 6162  here(name=lt.Tab
-00004460: 6c65 2e73 7461 7274 7377 6974 6828 2253  le.startswith("S
-00004470: 5550 4552 5343 5249 5054 2229 290a 2020  UPERSCRIPT")).  
-00004480: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00004490: 7445 7175 616c 2831 302c 206c 656e 2873  tEqual(10, len(s
-000044a0: 7570 6572 7329 290a 0a20 2020 2020 2020  upers))..       
-000044b0: 2023 2069 6d70 6f72 7420 7265 0a20 2020   # import re.   
-000044c0: 2020 2020 2023 2073 6576 656e 7320 3d20       # sevens = 
-000044d0: 756e 6963 6f64 655f 6e75 6d62 6572 732e  unicode_numbers.
-000044e0: 7768 6572 6528 6c61 6d62 6461 2072 6563  where(lambda rec
-000044f0: 3a20 7265 2e63 6f6d 7069 6c65 2872 222e  : re.compile(r".
-00004500: 2a53 4556 454e 2422 292e 6d61 7463 6828  *SEVEN$").match(
-00004510: 7265 632e 6e61 6d65 2929 0a0a 2020 2020  rec.name))..    
-00004520: 2020 2020 7365 7665 6e73 203d 2075 6e69      sevens = uni
-00004530: 636f 6465 5f6e 756d 6265 7273 2e77 6865  code_numbers.whe
-00004540: 7265 286e 616d 653d 6c74 2e54 6162 6c65  re(name=lt.Table
-00004550: 2e72 655f 6d61 7463 6828 7222 2e2a 5345  .re_match(r".*SE
-00004560: 5645 4e24 2229 290a 2020 2020 2020 2020  VEN$")).        
-00004570: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00004580: 2833 2c20 6c65 6e28 7365 7665 6e73 2929  (3, len(sevens))
-00004590: 0a0a 2020 2020 2020 2020 2320 6d61 6b65  ..        # make
-000045a0: 206e 616d 6573 2061 6c6c 2074 6974 6c65   names all title
-000045b0: 2063 6173 650a 2020 2020 2020 2020 756e   case.        un
-000045c0: 6963 6f64 655f 6e75 6d62 6572 732e 6164  icode_numbers.ad
-000045d0: 645f 6669 656c 6428 226e 616d 6522 2c20  d_field("name", 
-000045e0: 6c61 6d62 6461 2072 6563 3a20 7265 632e  lambda rec: rec.
-000045f0: 6e61 6d65 2e74 6974 6c65 2829 290a 2020  name.title()).  
-00004600: 2020 2020 2020 2320 7573 6520 7265 6765        # use rege
-00004610: 7820 7769 7468 2072 6520 666c 6167 0a20  x with re flag. 
-00004620: 2020 2020 2020 2069 6d70 6f72 7420 7265         import re
-00004630: 0a20 2020 2020 2020 2063 6972 636c 6564  .        circled
-00004640: 203d 2075 6e69 636f 6465 5f6e 756d 6265   = unicode_numbe
-00004650: 7273 2e77 6865 7265 286e 616d 653d 6c74  rs.where(name=lt
-00004660: 2e54 6162 6c65 2e72 655f 6d61 7463 6828  .Table.re_match(
-00004670: 7222 6369 7263 6c65 6422 2c20 666c 6167  r"circled", flag
-00004680: 733d 7265 2e49 2929 0a20 2020 2020 2020  s=re.I)).       
-00004690: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-000046a0: 6c28 3130 2c20 6c65 6e28 6369 7263 6c65  l(10, len(circle
-000046b0: 6429 290a 0a20 2020 2064 6566 2074 6573  d))..    def tes
-000046c0: 745f 7768 6572 655f 6174 7472 5f66 756e  t_where_attr_fun
-000046d0: 6374 696f 6e28 7365 6c66 293a 0a20 2020  ction(self):.   
-000046e0: 2020 2020 2074 6573 745f 7369 7a65 203d       test_size =
-000046f0: 2038 0a20 2020 2020 2020 2074 6162 6c65   8.        table
-00004700: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
-00004710: 6c65 2873 656c 662e 6d61 6b65 5f64 6174  le(self.make_dat
-00004720: 615f 6f62 6a65 6374 2c20 7465 7374 5f73  a_object, test_s
-00004730: 697a 6529 0a0a 2020 2020 2020 2020 6465  ize)..        de
-00004740: 6620 6973 5f6f 6464 2878 293a 0a20 2020  f is_odd(x):.   
-00004750: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00004760: 626f 6f6c 2878 2025 2032 290a 0a20 2020  bool(x % 2)..   
-00004770: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00004780: 4571 7561 6c28 7465 7374 5f73 697a 652a  Equal(test_size*
-00004790: 7465 7374 5f73 697a 652a 7465 7374 5f73  test_size*test_s
-000047a0: 697a 652f 2f32 2c20 6c65 6e28 7461 626c  ize//2, len(tabl
-000047b0: 652e 7768 6572 6528 613d 6973 5f6f 6464  e.where(a=is_odd
-000047c0: 2929 290a 0a20 2020 2064 6566 2074 6573  )))..    def tes
-000047d0: 745f 6765 745f 736c 6963 6528 7365 6c66  t_get_slice(self
-000047e0: 293a 0a20 2020 2020 2020 2074 6573 745f  ):.        test_
-000047f0: 7369 7a65 203d 2031 300a 2020 2020 2020  size = 10.      
-00004800: 2020 7461 626c 6520 3d20 6d61 6b65 5f74    table = make_t
-00004810: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
-00004820: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
-00004830: 2074 6573 745f 7369 7a65 290a 0a20 2020   test_size)..   
-00004840: 2020 2020 2073 7562 7461 626c 6520 3d20       subtable = 
-00004850: 7461 626c 655b 303a 3a74 6573 745f 7369  table[0::test_si
-00004860: 7a65 5d0a 2020 2020 2020 2020 7365 6c66  ze].        self
-00004870: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
-00004880: 745f 7369 7a65 202a 2074 6573 745f 7369  t_size * test_si
-00004890: 7a65 2c20 6c65 6e28 7375 6274 6162 6c65  ze, len(subtable
-000048a0: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
-000048b0: 5f69 6e64 6578 696e 6728 7365 6c66 293a  _indexing(self):
-000048c0: 0a20 2020 2020 2020 2063 6861 7273 203d  .        chars =
-000048d0: 2022 4142 4344 4546 4748 494a 4b4c 4d4e   "ABCDEFGHIJKLMN
-000048e0: 4f50 5152 5354 5556 5758 595a 220a 2020  OPQRSTUVWXYZ".  
-000048f0: 2020 2020 2020 6d61 6b65 5f72 6563 203d        make_rec =
-00004900: 206c 616d 6264 6120 6161 2c20 6262 2c20   lambda aa, bb, 
-00004910: 6363 3a20 7365 6c66 2e6d 616b 655f 6461  cc: self.make_da
-00004920: 7461 5f6f 626a 6563 7428 6368 6172 735b  ta_object(chars[
-00004930: 6161 5d2c 2063 6861 7273 5b62 625d 2c20  aa], chars[bb], 
-00004940: 6368 6172 735b 6363 5d29 0a20 2020 2020  chars[cc]).     
-00004950: 2020 2074 6573 745f 7369 7a65 203d 2031     test_size = 1
-00004960: 300a 2020 2020 2020 2020 7461 626c 6520  0.        table 
-00004970: 3d20 6d61 6b65 5f74 6573 745f 7461 626c  = make_test_tabl
-00004980: 6528 6d61 6b65 5f72 6563 2c20 7465 7374  e(make_rec, test
-00004990: 5f73 697a 6529 0a20 2020 2020 2020 2074  _size).        t
-000049a0: 6162 6c65 2e63 7265 6174 655f 696e 6465  able.create_inde
-000049b0: 7828 2761 2729 0a0a 2020 2020 2020 2020  x('a')..        
-000049c0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-000049d0: 2741 2720 696e 2074 6162 6c65 2e62 792e  'A' in table.by.
-000049e0: 6129 0a20 2020 2020 2020 2073 656c 662e  a).        self.
-000049f0: 6173 7365 7274 5472 7565 2827 4141 2720  assertTrue('AA' 
-00004a00: 6e6f 7420 696e 2074 6162 6c65 2e62 792e  not in table.by.
-00004a10: 6129 0a20 2020 2020 2020 2073 656c 662e  a).        self.
-00004a20: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
-00004a30: 5f73 697a 6520 2a20 7465 7374 5f73 697a  _size * test_siz
-00004a40: 652c 206c 656e 2874 6162 6c65 2e62 792e  e, len(table.by.
-00004a50: 615b 2742 275d 2929 0a20 2020 2020 2020  a['B'])).       
-00004a60: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
-00004a70: 2869 7369 6e73 7461 6e63 6528 7461 626c  (isinstance(tabl
-00004a80: 652e 6279 2e61 5b27 4227 5d2c 206c 742e  e.by.a['B'], lt.
-00004a90: 5461 626c 6529 290a 2020 2020 2020 2020  Table)).        
-00004aa0: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
-00004ab0: 5261 6973 6573 2841 7474 7269 6275 7465  Raises(Attribute
-00004ac0: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
-00004ad0: 2020 2020 7461 626c 652e 6279 2e7a 0a0a      table.by.z..
-00004ae0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00004af0: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
-00004b00: 7a65 2c20 6c65 6e28 7461 626c 652e 6279  ze, len(table.by
-00004b10: 2e61 2e6b 6579 7328 2929 290a 0a20 2020  .a.keys()))..   
-00004b20: 2064 6566 2074 6573 745f 756e 6971 7565   def test_unique
-00004b30: 5f69 6e64 6578 696e 6728 7365 6c66 293a  _indexing(self):
-00004b40: 0a20 2020 2020 2020 2063 6861 7273 203d  .        chars =
-00004b50: 2022 4142 4344 4546 4748 494a 4b4c 4d4e   "ABCDEFGHIJKLMN
-00004b60: 4f50 5152 5354 5556 5758 595a 220a 2020  OPQRSTUVWXYZ".  
-00004b70: 2020 2020 2020 6d61 6b65 5f75 6e69 7175        make_uniqu
-00004b80: 655f 6b65 7920 3d20 6c61 6d62 6461 202a  e_key = lambda *
-00004b90: 6172 6773 3a20 2727 2e6a 6f69 6e28 6368  args: ''.join(ch
-00004ba0: 6172 735b 6172 675d 2066 6f72 2061 7267  ars[arg] for arg
-00004bb0: 2069 6e20 6172 6773 290a 2020 2020 2020   in args).      
-00004bc0: 2020 6d61 6b65 5f72 6563 203d 206c 616d    make_rec = lam
-00004bd0: 6264 6120 6161 2c20 6262 2c20 6363 3a20  bda aa, bb, cc: 
-00004be0: 7365 6c66 2e6d 616b 655f 6461 7461 5f6f  self.make_data_o
-00004bf0: 626a 6563 7428 6d61 6b65 5f75 6e69 7175  bject(make_uniqu
-00004c00: 655f 6b65 7928 6161 2c20 6262 2c20 6363  e_key(aa, bb, cc
-00004c10: 292c 2063 6861 7273 5b62 625d 2c20 6368  ), chars[bb], ch
-00004c20: 6172 735b 6363 5d29 0a20 2020 2020 2020  ars[cc]).       
-00004c30: 2074 6573 745f 7369 7a65 203d 2031 300a   test_size = 10.
-00004c40: 2020 2020 2020 2020 7461 626c 6520 3d20          table = 
-00004c50: 6d61 6b65 5f74 6573 745f 7461 626c 6528  make_test_table(
-00004c60: 6d61 6b65 5f72 6563 2c20 7465 7374 5f73  make_rec, test_s
-00004c70: 697a 6529 2822 5461 626c 655f 3122 290a  ize)("Table_1").
-00004c80: 2020 2020 2020 2020 7461 626c 652e 6372          table.cr
-00004c90: 6561 7465 5f69 6e64 6578 2827 6127 2c20  eate_index('a', 
-00004ca0: 756e 6971 7565 3d54 7275 6529 0a20 2020  unique=True).   
-00004cb0: 2020 2020 2072 6563 5f74 7970 6520 3d20       rec_type = 
-00004cc0: 7479 7065 2873 656c 662e 6d61 6b65 5f64  type(self.make_d
-00004cd0: 6174 615f 6f62 6a65 6374 2830 2c20 302c  ata_object(0, 0,
-00004ce0: 2030 2929 0a0a 2020 2020 2020 2020 7365   0))..        se
-00004cf0: 6c66 2e61 7373 6572 7454 7275 6528 2741  lf.assertTrue('A
-00004d00: 4141 2720 696e 2074 6162 6c65 2e62 792e  AA' in table.by.
-00004d10: 6129 0a20 2020 2020 2020 2073 656c 662e  a).        self.
-00004d20: 6173 7365 7274 5472 7565 2827 4141 2720  assertTrue('AA' 
-00004d30: 6e6f 7420 696e 2074 6162 6c65 2e62 792e  not in table.by.
-00004d40: 6129 0a20 2020 2020 2020 2073 656c 662e  a).        self.
-00004d50: 6173 7365 7274 5472 7565 2869 7369 6e73  assertTrue(isins
-00004d60: 7461 6e63 6528 7461 626c 652e 6279 2e61  tance(table.by.a
-00004d70: 5b27 4241 4127 5d2c 2072 6563 5f74 7970  ['BAA'], rec_typ
-00004d80: 6529 290a 2020 2020 2020 2020 7769 7468  e)).        with
-00004d90: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
-00004da0: 6573 284b 6579 4572 726f 7229 3a0a 2020  es(KeyError):.  
-00004db0: 2020 2020 2020 2020 2020 7461 626c 652e            table.
-00004dc0: 696e 7365 7274 2873 656c 662e 6d61 6b65  insert(self.make
-00004dd0: 5f64 6174 615f 6f62 6a65 6374 284e 6f6e  _data_object(Non
-00004de0: 652c 204e 6f6e 652c 204e 6f6e 6529 290a  e, None, None)).
-00004df0: 0a20 2020 2020 2020 2023 2063 7265 6174  .        # creat
-00004e00: 6520 6475 706c 6963 6174 6520 696e 6465  e duplicate inde
-00004e10: 780a 2020 2020 2020 2020 7769 7468 2073  x.        with s
-00004e20: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
-00004e30: 2856 616c 7565 4572 726f 7229 3a0a 2020  (ValueError):.  
-00004e40: 2020 2020 2020 2020 2020 7461 626c 652e            table.
-00004e50: 6372 6561 7465 5f69 6e64 6578 2827 6127  create_index('a'
-00004e60: 2c20 756e 6971 7565 3d54 7275 652c 2061  , unique=True, a
-00004e70: 6363 6570 745f 6e6f 6e65 3d54 7275 6529  ccept_none=True)
-00004e80: 0a0a 2020 2020 2020 2020 2320 6372 6561  ..        # crea
-00004e90: 7465 2075 6e69 7175 6520 696e 6465 7820  te unique index 
-00004ea0: 7468 6174 2061 6c6c 6f77 7320 4e6f 6e65  that allows None
-00004eb0: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
-00004ec0: 7461 626c 652e 6465 6c65 7465 5f69 6e64  table.delete_ind
-00004ed0: 6578 2827 6127 290a 2020 2020 2020 2020  ex('a').        
-00004ee0: 7461 626c 652e 6372 6561 7465 5f69 6e64  table.create_ind
-00004ef0: 6578 2827 6127 2c20 756e 6971 7565 3d54  ex('a', unique=T
-00004f00: 7275 652c 2061 6363 6570 745f 6e6f 6e65  rue, accept_none
-00004f10: 3d54 7275 6529 0a20 2020 2020 2020 2074  =True).        t
-00004f20: 6162 6c65 2e69 6e73 6572 7428 7365 6c66  able.insert(self
-00004f30: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
-00004f40: 7428 4e6f 6e65 2c20 4e6f 6e65 2c20 2741  t(None, None, 'A
-00004f50: 2729 290a 0a20 2020 2020 2020 2073 7472  '))..        str
-00004f60: 5f6e 6f6e 655f 636f 6d70 6172 6520 3d20  _none_compare = 
-00004f70: 6c61 6d62 6461 2078 3a20 7820 6966 2069  lambda x: x if i
-00004f80: 7369 6e73 7461 6e63 6528 782c 2073 7472  sinstance(x, str
-00004f90: 2920 656c 7365 2063 6872 2832 3535 292a  ) else chr(255)*
-00004fa0: 3130 300a 2020 2020 2020 2020 7365 6c66  100.        self
-00004fb0: 2e61 7373 6572 7445 7175 616c 2873 6f72  .assertEqual(sor
-00004fc0: 7465 6428 7461 626c 652e 6279 2e61 2e6b  ted(table.by.a.k
-00004fd0: 6579 7328 292c 206b 6579 3d73 7472 5f6e  eys(), key=str_n
-00004fe0: 6f6e 655f 636f 6d70 6172 6529 2c0a 2020  one_compare),.  
-00004ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005000: 2020 2020 2020 2073 6f72 7465 6428 7461         sorted(ta
-00005010: 626c 652e 616c 6c2e 612c 206b 6579 3d73  ble.all.a, key=s
-00005020: 7472 5f6e 6f6e 655f 636f 6d70 6172 6529  tr_none_compare)
-00005030: 290a 0a20 2020 2020 2020 2023 206e 6f77  )..        # now
-00005040: 2064 726f 7020 696e 6465 7820 616e 6420   drop index and 
-00005050: 7265 6372 6561 7465 206e 6f74 2070 6572  recreate not per
-00005060: 6d69 7474 696e 6720 4e6f 6e65 2c20 7368  mitting None, sh
-00005070: 6f75 6c64 2072 6169 7365 2065 7863 6570  ould raise excep
-00005080: 7469 6f6e 0a20 2020 2020 2020 2074 6162  tion.        tab
-00005090: 6c65 2e64 656c 6574 655f 696e 6465 7828  le.delete_index(
-000050a0: 2761 2729 0a20 2020 2020 2020 2077 6974  'a').        wit
-000050b0: 6820 7365 6c66 2e61 7373 6572 7452 6169  h self.assertRai
-000050c0: 7365 7328 4b65 7945 7272 6f72 293a 0a20  ses(KeyError):. 
-000050d0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-000050e0: 2e63 7265 6174 655f 696e 6465 7828 2761  .create_index('a
-000050f0: 272c 2075 6e69 7175 653d 5472 7565 2c20  ', unique=True, 
-00005100: 6163 6365 7074 5f6e 6f6e 653d 4661 6c73  accept_none=Fals
-00005110: 6529 0a0a 2020 2020 2020 2020 7461 626c  e)..        tabl
-00005120: 652e 6372 6561 7465 5f69 6e64 6578 2827  e.create_index('
-00005130: 6127 2c20 756e 6971 7565 3d54 7275 652c  a', unique=True,
-00005140: 2061 6363 6570 745f 6e6f 6e65 3d54 7275   accept_none=Tru
-00005150: 6529 0a20 2020 2020 2020 2074 6162 6c65  e).        table
-00005160: 2e63 7265 6174 655f 696e 6465 7828 2763  .create_index('c
-00005170: 2729 0a0a 2020 2020 2020 2020 696d 706f  ')..        impo
-00005180: 7274 2070 7072 696e 740a 2020 2020 2020  rt pprint.      
-00005190: 2020 696e 666f 203d 2074 6162 6c65 2e69    info = table.i
-000051a0: 6e66 6f28 290a 2020 2020 2020 2020 7070  nfo().        pp
-000051b0: 7269 6e74 2e70 7072 696e 7428 696e 666f  rint.pprint(info
-000051c0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-000051d0: 7373 6572 7445 7175 616c 2827 5461 626c  ssertEqual('Tabl
-000051e0: 655f 3127 2c20 696e 666f 5b27 6e61 6d65  e_1', info['name
-000051f0: 275d 290a 2020 2020 2020 2020 7365 6c66  ']).        self
-00005200: 2e61 7373 6572 7445 7175 616c 285b 2761  .assertEqual(['a
-00005210: 272c 2027 6227 2c20 2763 275d 2c20 6c69  ', 'b', 'c'], li
-00005220: 7374 2873 6f72 7465 6428 696e 666f 5b27  st(sorted(info['
-00005230: 6669 656c 6473 275d 2929 290a 2020 2020  fields']))).    
-00005240: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00005250: 7175 616c 285b 2827 6127 2c20 5472 7565  qual([('a', True
-00005260: 292c 2028 2763 272c 2046 616c 7365 295d  ), ('c', False)]
-00005270: 2c20 6c69 7374 2873 6f72 7465 6428 696e  , list(sorted(in
-00005280: 666f 5b27 696e 6465 7865 7327 5d29 2929  fo['indexes'])))
-00005290: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-000052a0: 7365 7274 4571 7561 6c28 3130 3031 2c20  sertEqual(1001, 
-000052b0: 696e 666f 5b27 6c65 6e27 5d29 0a0a 2020  info['len'])..  
-000052c0: 2020 6465 6620 7465 7374 5f63 6861 696e    def test_chain
-000052d0: 6564 5f69 6e64 6578 696e 6728 7365 6c66  ed_indexing(self
-000052e0: 293a 0a20 2020 2020 2020 2063 6861 7273  ):.        chars
-000052f0: 203d 2022 4142 4344 4546 4748 494a 4b4c   = "ABCDEFGHIJKL
-00005300: 4d4e 4f50 5152 5354 5556 5758 595a 220a  MNOPQRSTUVWXYZ".
-00005310: 2020 2020 2020 2020 6d61 6b65 5f72 6563          make_rec
-00005320: 203d 206c 616d 6264 6120 6161 2c20 6262   = lambda aa, bb
-00005330: 2c20 6363 3a20 7365 6c66 2e6d 616b 655f  , cc: self.make_
-00005340: 6461 7461 5f6f 626a 6563 7428 6368 6172  data_object(char
-00005350: 735b 6161 2025 206c 656e 2863 6861 7273  s[aa % len(chars
-00005360: 295d 2c0a 2020 2020 2020 2020 2020 2020  )],.            
-00005370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053a0: 6368 6172 735b 6262 2025 206c 656e 2863  chars[bb % len(c
-000053b0: 6861 7273 295d 2c0a 2020 2020 2020 2020  hars)],.        
-000053c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053f0: 2020 2020 6368 6172 735b 6363 2025 206c      chars[cc % l
-00005400: 656e 2863 6861 7273 295d 290a 2020 2020  en(chars)]).    
-00005410: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
-00005420: 3130 0a20 2020 2020 2020 2074 6162 6c65  10.        table
-00005430: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
-00005440: 6c65 286d 616b 655f 7265 632c 2074 6573  le(make_rec, tes
-00005450: 745f 7369 7a65 290a 2020 2020 2020 2020  t_size).        
-00005460: 7461 626c 652e 6372 6561 7465 5f69 6e64  table.create_ind
-00005470: 6578 2827 6127 290a 2020 2020 2020 2020  ex('a').        
-00005480: 7461 626c 652e 6372 6561 7465 5f69 6e64  table.create_ind
-00005490: 6578 2827 6227 290a 2020 2020 2020 2020  ex('b').        
-000054a0: 7461 626c 652e 6372 6561 7465 5f69 6e64  table.create_ind
-000054b0: 6578 2827 6327 290a 0a20 2020 2020 2020  ex('c')..       
-000054c0: 2063 6861 696e 6564 5f74 6162 6c65 203d   chained_table =
-000054d0: 2074 6162 6c65 2e62 792e 625b 2741 275d   table.by.b['A']
-000054e0: 2e62 792e 635b 2743 275d 0a20 2020 2020  .by.c['C'].     
-000054f0: 2020 2066 6f72 2072 6563 2069 6e20 6368     for rec in ch
-00005500: 6169 6e65 645f 7461 626c 653a 0a20 2020  ained_table:.   
-00005510: 2020 2020 2020 2020 2070 7269 6e74 2872           print(r
-00005520: 6563 290a 0a20 2020 2020 2020 2073 656c  ec)..        sel
-00005530: 662e 6173 7365 7274 4571 7561 6c28 7465  f.assertEqual(te
-00005540: 7374 5f73 697a 652c 206c 656e 2863 6861  st_size, len(cha
-00005550: 696e 6564 5f74 6162 6c65 2929 0a0a 2020  ined_table))..  
-00005560: 2020 6465 6620 7465 7374 5f70 6172 7365    def test_parse
-00005570: 5f64 6174 6574 696d 655f 7472 616e 7366  _datetime_transf
-00005580: 6f72 6d28 7365 6c66 293a 0a20 2020 2020  orm(self):.     
-00005590: 2020 2069 6d70 6f72 7420 6461 7465 7469     import dateti
-000055a0: 6d65 0a0a 2020 2020 2020 2020 6461 7461  me..        data
-000055b0: 203d 2074 6578 7477 7261 702e 6465 6465   = textwrap.dede
-000055c0: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
-000055d0: 612c 622c 630a 2020 2020 2020 2020 3230  a,b,c.        20
-000055e0: 3031 2d30 312d 3031 2030 303a 3334 3a35  01-01-01 00:34:5
-000055f0: 362c 412c 3130 300a 2020 2020 2020 2020  6,A,100.        
-00005600: 3230 3031 2d30 312d 3032 2030 313a 3334  2001-01-02 01:34
-00005610: 3a35 362c 422c 3130 310a 2020 2020 2020  :56,B,101.      
-00005620: 2020 3230 3031 2d30 322d 3330 2030 323a    2001-02-30 02:
-00005630: 3334 3a35 362c 432c 3130 320a 2020 2020  34:56,C,102.    
-00005640: 2020 2020 2c44 2c31 3033 0a20 2020 2020      ,D,103.     
-00005650: 2020 2022 2222 290a 2020 2020 2020 2020     """).        
-00005660: 7465 7374 5f6b 7761 7267 7320 3d20 5b0a  test_kwargs = [.
-00005670: 2020 2020 2020 2020 2020 2020 7b27 656d              {'em
-00005680: 7074 7927 3a20 2727 2c20 276f 6e5f 6572  pty': '', 'on_er
-00005690: 726f 7227 3a20 4e6f 6e65 7d2c 0a20 2020  ror': None},.   
-000056a0: 2020 2020 2020 2020 207b 2765 6d70 7479           {'empty
-000056b0: 273a 2027 4e2f 4127 2c20 276f 6e5f 6572  ': 'N/A', 'on_er
-000056c0: 726f 7227 3a20 6461 7465 7469 6d65 2e64  ror': datetime.d
-000056d0: 6174 6574 696d 652e 6d69 6e7d 2c0a 2020  atetime.min},.  
-000056e0: 2020 2020 2020 2020 2020 7b27 656d 7074            {'empt
-000056f0: 7927 3a20 6461 7465 7469 6d65 2e64 6174  y': datetime.dat
-00005700: 6574 696d 652e 6d69 6e2c 2027 6f6e 5f65  etime.min, 'on_e
-00005710: 7272 6f72 273a 2027 277d 2c0a 2020 2020  rror': ''},.    
-00005720: 2020 2020 5d0a 2020 2020 2020 2020 666f      ].        fo
-00005730: 7220 6b77 6172 6773 2069 6e20 7465 7374  r kwargs in test
-00005740: 5f6b 7761 7267 733a 0a20 2020 2020 2020  _kwargs:.       
-00005750: 2020 2020 2074 626c 203d 206c 742e 5461       tbl = lt.Ta
-00005760: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
-00005770: 2864 6174 612c 0a20 2020 2020 2020 2020  (data,.         
-00005780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005790: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000057a0: 7261 6e73 666f 726d 733d 7b27 6127 3a20  ransforms={'a': 
-000057b0: 6c74 2e54 6162 6c65 2e70 6172 7365 5f64  lt.Table.parse_d
-000057c0: 6174 6574 696d 6528 2725 592d 256d 2d25  atetime('%Y-%m-%
-000057d0: 6420 2548 3a25 4d3a 2553 272c 0a20 2020  d %H:%M:%S',.   
-000057e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005820: 2020 2020 2020 2020 2020 2020 2020 2a2a                **
-00005830: 6b77 6172 6773 297d 290a 2020 2020 2020  kwargs)}).      
-00005840: 2020 2020 2020 7072 696e 7428 5b73 7472        print([str
-00005850: 2861 2920 666f 7220 6120 696e 2074 626c  (a) for a in tbl
-00005860: 2e61 6c6c 2e61 5d29 0a0a 2020 2020 2020  .all.a])..      
-00005870: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00005880: 7375 6254 6573 7428 2274 6573 7420 5461  subTest("test Ta
-00005890: 626c 652e 7061 7273 655f 6461 7465 5f74  ble.parse_date_t
-000058a0: 696d 6520 6572 726f 7273 222c 202a 2a6b  ime errors", **k
-000058b0: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
-000058c0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-000058d0: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
-000058e0: 2020 2020 2020 2020 2020 2020 2020 5b6b                [k
-000058f0: 7761 7267 735b 226f 6e5f 6572 726f 7222  wargs["on_error"
-00005900: 5d2c 206b 7761 7267 735b 2265 6d70 7479  ], kwargs["empty
-00005910: 225d 5d2c 0a20 2020 2020 2020 2020 2020  "]],.           
-00005920: 2020 2020 2020 2020 206c 6973 7428 7462           list(tb
-00005930: 6c2e 616c 6c2e 6129 5b2d 323a 5d0a 2020  l.all.a)[-2:].  
-00005940: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00005950: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00005960: 6820 7365 6c66 2e73 7562 5465 7374 2822  h self.subTest("
-00005970: 7465 7374 2054 6162 6c65 2e70 6172 7365  test Table.parse
-00005980: 5f64 6174 655f 7469 6d65 2076 616c 6964  _date_time valid
-00005990: 222c 202a 2a6b 7761 7267 7329 3a0a 2020  ", **kwargs):.  
-000059a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000059b0: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
-000059c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059d0: 2020 2020 5b64 6174 6574 696d 652e 6461      [datetime.da
-000059e0: 7465 7469 6d65 2832 3030 312c 2031 2c20  tetime(2001, 1, 
-000059f0: 312c 2030 2c20 3334 2c20 3536 292c 0a20  1, 0, 34, 56),. 
+00003450: 5f65 7175 616c 735f 7769 7468 5f69 6e64  _equals_with_ind
+00003460: 6578 2873 656c 6629 3a0a 2020 2020 2020  ex(self):.      
+00003470: 2020 7465 7374 5f73 697a 6520 3d20 3130    test_size = 10
+00003480: 0a20 2020 2020 2020 2074 6162 6c65 203d  .        table =
+00003490: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
+000034a0: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
+000034b0: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
+000034c0: 6529 0a20 2020 2020 2020 2074 6162 6c65  e).        table
+000034d0: 2e63 7265 6174 655f 696e 6465 7828 2761  .create_index('a
+000034e0: 2729 0a0a 2020 2020 2020 2020 7365 6c66  ')..        self
+000034f0: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
+00003500: 745f 7369 7a65 2a74 6573 745f 7369 7a65  t_size*test_size
+00003510: 2c20 6c65 6e28 7461 626c 652e 7768 6572  , len(table.wher
+00003520: 6528 613d 3529 2929 0a20 2020 2020 2020  e(a=5))).       
+00003530: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00003540: 6c28 302c 206c 656e 2874 6162 6c65 2e77  l(0, len(table.w
+00003550: 6865 7265 2861 3d2d 3129 2929 0a0a 2020  here(a=-1)))..  
+00003560: 2020 6465 6620 7465 7374 5f77 6865 7265    def test_where
+00003570: 5f72 616e 6765 2873 656c 6629 3a0a 2020  _range(self):.  
+00003580: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
+00003590: 3d20 3130 0a20 2020 2020 2020 2074 6162  = 10.        tab
+000035a0: 6c65 203d 206d 616b 655f 7465 7374 5f74  le = make_test_t
+000035b0: 6162 6c65 2873 656c 662e 6d61 6b65 5f64  able(self.make_d
+000035c0: 6174 615f 6f62 6a65 6374 2c20 7465 7374  ata_object, test
+000035d0: 5f73 697a 6529 0a0a 2020 2020 2020 2020  _size)..        
+000035e0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000035f0: 2874 6573 745f 7369 7a65 2a74 6573 745f  (test_size*test_
+00003600: 7369 7a65 2c20 6c65 6e28 7461 626c 652e  size, len(table.
+00003610: 7768 6572 6528 6c61 6d62 6461 2072 6563  where(lambda rec
+00003620: 3a20 7265 632e 6120 3d3d 2072 6563 2e62  : rec.a == rec.b
+00003630: 2929 290a 0a20 2020 2064 6566 2074 6573  )))..    def tes
+00003640: 745f 7768 6572 655f 636f 6d70 6172 6174  t_where_comparat
+00003650: 6f72 2873 656c 6629 3a0a 2020 2020 2020  or(self):.      
+00003660: 2020 7465 7374 5f73 697a 6520 3d20 3130    test_size = 10
+00003670: 0a20 2020 2020 2020 2074 6162 6c65 203d  .        table =
+00003680: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
+00003690: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
+000036a0: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
+000036b0: 6529 0a0a 2020 2020 2020 2020 7365 6c66  e)..        self
+000036c0: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
+000036d0: 745f 7369 7a65 2a74 6573 745f 7369 7a65  t_size*test_size
+000036e0: 2a34 2c20 6c65 6e28 7461 626c 652e 7768  *4, len(table.wh
+000036f0: 6572 6528 613d 6c74 2e54 6162 6c65 2e6c  ere(a=lt.Table.l
+00003700: 7428 3429 2929 290a 2020 2020 2020 2020  t(4)))).        
+00003710: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00003720: 2874 6573 745f 7369 7a65 2a74 6573 745f  (test_size*test_
+00003730: 7369 7a65 2a28 342b 3129 2c20 6c65 6e28  size*(4+1), len(
+00003740: 7461 626c 652e 7768 6572 6528 613d 6c74  table.where(a=lt
+00003750: 2e54 6162 6c65 2e6c 6528 3429 2929 290a  .Table.le(4)))).
+00003760: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00003770: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
+00003780: 7a65 2a74 6573 745f 7369 7a65 2a28 7465  ze*test_size*(te
+00003790: 7374 5f73 697a 652d 342d 3129 2c20 6c65  st_size-4-1), le
+000037a0: 6e28 7461 626c 652e 7768 6572 6528 613d  n(table.where(a=
+000037b0: 6c74 2e54 6162 6c65 2e67 7428 3429 2929  lt.Table.gt(4)))
+000037c0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+000037d0: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
+000037e0: 7369 7a65 2a74 6573 745f 7369 7a65 2a28  size*test_size*(
+000037f0: 7465 7374 5f73 697a 652d 3429 2c20 6c65  test_size-4), le
+00003800: 6e28 7461 626c 652e 7768 6572 6528 613d  n(table.where(a=
+00003810: 6c74 2e54 6162 6c65 2e67 6528 3429 2929  lt.Table.ge(4)))
+00003820: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00003830: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
+00003840: 7369 7a65 2a74 6573 745f 7369 7a65 2a28  size*test_size*(
+00003850: 7465 7374 5f73 697a 652d 3129 2c20 6c65  test_size-1), le
+00003860: 6e28 7461 626c 652e 7768 6572 6528 613d  n(table.where(a=
+00003870: 6c74 2e54 6162 6c65 2e6e 6528 3429 2929  lt.Table.ne(4)))
+00003880: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00003890: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
+000038a0: 7369 7a65 2a74 6573 745f 7369 7a65 2c20  size*test_size, 
+000038b0: 6c65 6e28 7461 626c 652e 7768 6572 6528  len(table.where(
+000038c0: 613d 6c74 2e54 6162 6c65 2e65 7128 3429  a=lt.Table.eq(4)
+000038d0: 2929 290a 2020 2020 2020 2020 7365 6c66  ))).        self
+000038e0: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
+000038f0: 745f 7369 7a65 2c20 6c65 6e28 7461 626c  t_size, len(tabl
+00003900: 652e 7768 6572 6528 613d 6c74 2e54 6162  e.where(a=lt.Tab
+00003910: 6c65 2e65 7128 3429 2c20 623d 6c74 2e54  le.eq(4), b=lt.T
+00003920: 6162 6c65 2e65 7128 3429 2929 290a 2020  able.eq(4)))).  
+00003930: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00003940: 7445 7175 616c 2874 6573 745f 7369 7a65  tEqual(test_size
+00003950: 2a74 6573 745f 7369 7a65 2a34 2c20 6c65  *test_size*4, le
+00003960: 6e28 7461 626c 652e 7768 6572 6528 613d  n(table.where(a=
+00003970: 6c74 2e54 6162 6c65 2e62 6574 7765 656e  lt.Table.between
+00003980: 2833 2c20 3829 2929 290a 2020 2020 2020  (3, 8)))).      
+00003990: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000039a0: 616c 2874 6573 745f 7369 7a65 2a74 6573  al(test_size*tes
+000039b0: 745f 7369 7a65 2a34 2c20 6c65 6e28 7461  t_size*4, len(ta
+000039c0: 626c 652e 7768 6572 6528 613d 6c74 2e54  ble.where(a=lt.T
+000039d0: 6162 6c65 2e77 6974 6869 6e28 322c 2035  able.within(2, 5
+000039e0: 2929 2929 0a20 2020 2020 2020 2073 656c  )))).        sel
+000039f0: 662e 6173 7365 7274 4571 7561 6c28 7465  f.assertEqual(te
+00003a00: 7374 5f73 697a 652a 7465 7374 5f73 697a  st_size*test_siz
+00003a10: 652a 332c 206c 656e 2874 6162 6c65 2e77  e*3, len(table.w
+00003a20: 6865 7265 2861 3d6c 742e 5461 626c 652e  here(a=lt.Table.
+00003a30: 696e 5f72 616e 6765 2832 2c20 3529 2929  in_range(2, 5)))
+00003a40: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00003a50: 7373 6572 7445 7175 616c 2830 2c20 6c65  ssertEqual(0, le
+00003a60: 6e28 7461 626c 652e 7768 6572 6528 613d  n(table.where(a=
+00003a70: 6c74 2e54 6162 6c65 2e62 6574 7765 656e  lt.Table.between
+00003a80: 2833 2c20 3329 2929 290a 2020 2020 2020  (3, 3)))).      
+00003a90: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00003aa0: 616c 2874 6573 745f 7369 7a65 2a74 6573  al(test_size*tes
+00003ab0: 745f 7369 7a65 2c20 6c65 6e28 7461 626c  t_size, len(tabl
+00003ac0: 652e 7768 6572 6528 613d 6c74 2e54 6162  e.where(a=lt.Tab
+00003ad0: 6c65 2e77 6974 6869 6e28 332c 2033 2929  le.within(3, 3))
+00003ae0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00003af0: 6173 7365 7274 4571 7561 6c28 302c 206c  assertEqual(0, l
+00003b00: 656e 2874 6162 6c65 2e77 6865 7265 2861  en(table.where(a
+00003b10: 3d6c 742e 5461 626c 652e 696e 5f72 616e  =lt.Table.in_ran
+00003b20: 6765 2833 2c20 3329 2929 290a 2020 2020  ge(3, 3)))).    
+00003b30: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00003b40: 7175 616c 2874 6573 745f 7369 7a65 2a74  qual(test_size*t
+00003b50: 6573 745f 7369 7a65 2a34 2c20 6c65 6e28  est_size*4, len(
+00003b60: 7461 626c 652e 7768 6572 6528 613d 6c74  table.where(a=lt
+00003b70: 2e54 6162 6c65 2e69 735f 696e 285b 322c  .Table.is_in([2,
+00003b80: 2034 2c20 362c 2038 5d29 2929 290a 2020   4, 6, 8])))).  
+00003b90: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00003ba0: 7445 7175 616c 2830 2c20 6c65 6e28 7461  tEqual(0, len(ta
+00003bb0: 626c 652e 7768 6572 6528 613d 6c74 2e54  ble.where(a=lt.T
+00003bc0: 6162 6c65 2e69 735f 696e 285b 5d29 2929  able.is_in([])))
+00003bd0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00003be0: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
+00003bf0: 7369 7a65 2a74 6573 745f 7369 7a65 2a28  size*test_size*(
+00003c00: 7465 7374 5f73 697a 652d 3429 2c20 6c65  test_size-4), le
+00003c10: 6e28 7461 626c 652e 7768 6572 6528 613d  n(table.where(a=
+00003c20: 6c74 2e54 6162 6c65 2e6e 6f74 5f69 6e28  lt.Table.not_in(
+00003c30: 5b32 2c20 342c 2036 2c20 385d 2929 2929  [2, 4, 6, 8]))))
+00003c40: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00003c50: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
+00003c60: 697a 652a 7465 7374 5f73 697a 652a 7465  ize*test_size*te
+00003c70: 7374 5f73 697a 652c 206c 656e 2874 6162  st_size, len(tab
+00003c80: 6c65 2e77 6865 7265 2861 3d6c 742e 5461  le.where(a=lt.Ta
+00003c90: 626c 652e 6e6f 745f 696e 285b 5d29 2929  ble.not_in([])))
+00003ca0: 290a 0a20 2020 2020 2020 2023 2061 6464  )..        # add
+00003cb0: 2061 2072 6563 6f72 6420 636f 6e74 6169   a record contai
+00003cc0: 6e69 6e67 2061 204e 6f6e 6520 7661 6c75  ning a None valu
+00003cd0: 6520 746f 2074 6573 7420 6973 5f6e 6f6e  e to test is_non
+00003ce0: 6520 616e 6420 6973 5f6e 6f74 5f6e 6f6e  e and is_not_non
+00003cf0: 6520 636f 6d70 6172 6174 6f72 730a 2020  e comparators.  
+00003d00: 2020 2020 2020 7461 626c 652e 696e 7365        table.inse
+00003d10: 7274 2873 656c 662e 6d61 6b65 5f64 6174  rt(self.make_dat
+00003d20: 615f 6f62 6a65 6374 2861 3d31 2c20 623d  a_object(a=1, b=
+00003d30: 322c 2063 3d4e 6f6e 6529 290a 2020 2020  2, c=None)).    
+00003d40: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00003d50: 7175 616c 2831 2c20 6c65 6e28 7461 626c  qual(1, len(tabl
+00003d60: 652e 7768 6572 6528 633d 6c74 2e54 6162  e.where(c=lt.Tab
+00003d70: 6c65 2e69 735f 6e6f 6e65 2829 2929 290a  le.is_none()))).
+00003d80: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00003d90: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
+00003da0: 7a65 2a74 6573 745f 7369 7a65 2a74 6573  ze*test_size*tes
+00003db0: 745f 7369 7a65 2c20 6c65 6e28 7461 626c  t_size, len(tabl
+00003dc0: 652e 7768 6572 6528 633d 6c74 2e54 6162  e.where(c=lt.Tab
+00003dd0: 6c65 2e69 735f 6e6f 745f 6e6f 6e65 2829  le.is_not_none()
+00003de0: 2929 290a 0a20 2020 2020 2020 2023 2061  )))..        # a
+00003df0: 6464 2061 2072 6563 6f72 6420 636f 6e74  dd a record cont
+00003e00: 6169 6e69 6e67 2061 206d 6973 7369 6e67  aining a missing
+00003e10: 2076 616c 7565 2074 6f20 7465 7374 2069   value to test i
+00003e20: 735f 6e75 6c6c 2061 6e64 2069 735f 6e6f  s_null and is_no
+00003e30: 745f 6e75 6c6c 2063 6f6d 7061 7261 746f  t_null comparato
+00003e40: 7273 0a20 2020 2020 2020 2074 6162 6c65  rs.        table
+00003e50: 2e69 6e73 6572 7428 7365 6c66 2e6d 616b  .insert(self.mak
+00003e60: 655f 6461 7461 5f6f 626a 6563 7428 613d  e_data_object(a=
+00003e70: 312c 2062 3d32 2c20 633d 2222 2929 0a20  1, b=2, c="")). 
+00003e80: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00003e90: 7274 4571 7561 6c28 322c 206c 656e 2874  rtEqual(2, len(t
+00003ea0: 6162 6c65 2e77 6865 7265 2863 3d6c 742e  able.where(c=lt.
+00003eb0: 5461 626c 652e 6973 5f6e 756c 6c28 2929  Table.is_null())
+00003ec0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00003ed0: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
+00003ee0: 5f73 697a 6520 2a20 7465 7374 5f73 697a  _size * test_siz
+00003ef0: 6520 2a20 7465 7374 5f73 697a 652c 206c  e * test_size, l
+00003f00: 656e 2874 6162 6c65 2e77 6865 7265 2863  en(table.where(c
+00003f10: 3d6c 742e 5461 626c 652e 6973 5f6e 6f74  =lt.Table.is_not
+00003f20: 5f6e 756c 6c28 2929 2929 0a0a 2020 2020  _null())))..    
+00003f30: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00003f40: 2020 2020 2074 6162 6c65 2e69 6e73 6572       table.inser
+00003f50: 7428 7365 6c66 2e6d 616b 655f 6461 7461  t(self.make_data
+00003f60: 5f6f 626a 6563 7428 613d 312c 2062 3d32  _object(a=1, b=2
+00003f70: 2929 0a20 2020 2020 2020 2065 7863 6570  )).        excep
+00003f80: 7420 5479 7065 4572 726f 723a 0a20 2020  t TypeError:.   
+00003f90: 2020 2020 2020 2020 2023 206e 6f74 2061           # not a
+00003fa0: 6c6c 2064 6174 6120 6f62 6a65 6374 2074  ll data object t
+00003fb0: 7970 6573 2062 6569 6e67 2074 6573 7465  ypes being teste
+00003fc0: 6420 7375 7070 6f72 7420 6d69 7373 696e  d support missin
+00003fd0: 6720 6174 7472 6962 7574 6573 0a20 2020  g attributes.   
+00003fe0: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
+00003ff0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00004000: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00004010: 6572 7445 7175 616c 2833 2c20 6c65 6e28  ertEqual(3, len(
+00004020: 7461 626c 652e 7768 6572 6528 633d 6c74  table.where(c=lt
+00004030: 2e54 6162 6c65 2e69 735f 6e75 6c6c 2829  .Table.is_null()
+00004040: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+00004050: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00004060: 2874 6573 745f 7369 7a65 202a 2074 6573  (test_size * tes
+00004070: 745f 7369 7a65 202a 2074 6573 745f 7369  t_size * test_si
+00004080: 7a65 2c20 6c65 6e28 7461 626c 652e 7768  ze, len(table.wh
+00004090: 6572 6528 633d 6c74 2e54 6162 6c65 2e69  ere(c=lt.Table.i
+000040a0: 735f 6e6f 745f 6e75 6c6c 2829 2929 290a  s_not_null()))).
+000040b0: 0a20 2020 2064 6566 2074 6573 745f 7768  .    def test_wh
+000040c0: 6572 655f 7374 725f 636f 6d70 6172 6174  ere_str_comparat
+000040d0: 6f72 2873 656c 6629 3a0a 2020 2020 2020  or(self):.      
+000040e0: 2020 756e 6963 6f64 655f 6e75 6d62 6572    unicode_number
+000040f0: 7320 3d20 6c74 2e54 6162 6c65 2829 2e63  s = lt.Table().c
+00004100: 7376 5f69 6d70 6f72 7428 7465 7874 7772  sv_import(textwr
+00004110: 6170 2e64 6564 656e 7428 2222 225c 0a20  ap.dedent("""\. 
+00004120: 2020 2020 2020 2020 2020 206e 616d 652c             name,
+00004130: 636f 6465 5f76 616c 7565 2c6e 756d 6572  code_value,numer
+00004140: 6963 5f76 616c 7565 0a20 2020 2020 2020  ic_value.       
+00004150: 2020 2020 2052 4f4d 414e 204e 554d 4552       ROMAN NUMER
+00004160: 414c 204f 4e45 2c38 3534 342c 310a 2020  AL ONE,8544,1.  
+00004170: 2020 2020 2020 2020 2020 524f 4d41 4e20            ROMAN 
+00004180: 4e55 4d45 5241 4c20 5457 4f2c 3835 3435  NUMERAL TWO,8545
+00004190: 2c32 0a20 2020 2020 2020 2020 2020 2052  ,2.            R
+000041a0: 4f4d 414e 204e 554d 4552 414c 2054 4852  OMAN NUMERAL THR
+000041b0: 4545 2c38 3534 362c 330a 2020 2020 2020  EE,8546,3.      
+000041c0: 2020 2020 2020 524f 4d41 4e20 4e55 4d45        ROMAN NUME
+000041d0: 5241 4c20 464f 5552 2c38 3534 372c 340a  RAL FOUR,8547,4.
+000041e0: 2020 2020 2020 2020 2020 2020 524f 4d41              ROMA
+000041f0: 4e20 4e55 4d45 5241 4c20 4649 5645 2c38  N NUMERAL FIVE,8
+00004200: 3534 382c 350a 2020 2020 2020 2020 2020  548,5.          
+00004210: 2020 524f 4d41 4e20 4e55 4d45 5241 4c20    ROMAN NUMERAL 
+00004220: 5349 582c 3835 3439 2c36 0a20 2020 2020  SIX,8549,6.     
+00004230: 2020 2020 2020 2052 4f4d 414e 204e 554d         ROMAN NUM
+00004240: 4552 414c 2053 4556 454e 2c38 3535 302c  ERAL SEVEN,8550,
+00004250: 370a 2020 2020 2020 2020 2020 2020 524f  7.            RO
+00004260: 4d41 4e20 4e55 4d45 5241 4c20 4549 4748  MAN NUMERAL EIGH
+00004270: 542c 3835 3531 2c38 0a20 2020 2020 2020  T,8551,8.       
+00004280: 2020 2020 2052 4f4d 414e 204e 554d 4552       ROMAN NUMER
+00004290: 414c 204e 494e 452c 3835 3532 2c39 0a20  AL NINE,8552,9. 
+000042a0: 2020 2020 2020 2020 2020 2052 4f4d 414e             ROMAN
+000042b0: 204e 554d 4552 414c 2054 454e 2c38 3535   NUMERAL TEN,855
+000042c0: 332c 3130 0a20 2020 2020 2020 2020 2020  3,10.           
+000042d0: 2053 5550 4552 5343 5249 5054 2054 574f   SUPERSCRIPT TWO
+000042e0: 2c31 3738 2c32 0a20 2020 2020 2020 2020  ,178,2.         
+000042f0: 2020 2053 5550 4552 5343 5249 5054 2054     SUPERSCRIPT T
+00004300: 4852 4545 2c31 3739 2c33 0a20 2020 2020  HREE,179,3.     
+00004310: 2020 2020 2020 2053 5550 4552 5343 5249         SUPERSCRI
+00004320: 5054 204f 4e45 2c31 3835 2c31 0a20 2020  PT ONE,185,1.   
+00004330: 2020 2020 2020 2020 2053 5550 4552 5343           SUPERSC
+00004340: 5249 5054 205a 4552 4f2c 3833 3034 2c30  RIPT ZERO,8304,0
+00004350: 0a20 2020 2020 2020 2020 2020 2053 5550  .            SUP
+00004360: 4552 5343 5249 5054 2046 4f55 522c 3833  ERSCRIPT FOUR,83
+00004370: 3038 2c34 0a20 2020 2020 2020 2020 2020  08,4.           
+00004380: 2053 5550 4552 5343 5249 5054 2046 4956   SUPERSCRIPT FIV
+00004390: 452c 3833 3039 2c35 0a20 2020 2020 2020  E,8309,5.       
+000043a0: 2020 2020 2053 5550 4552 5343 5249 5054       SUPERSCRIPT
+000043b0: 2053 4958 2c38 3331 302c 360a 2020 2020   SIX,8310,6.    
+000043c0: 2020 2020 2020 2020 5355 5045 5253 4352          SUPERSCR
+000043d0: 4950 5420 5345 5645 4e2c 3833 3131 2c37  IPT SEVEN,8311,7
+000043e0: 0a20 2020 2020 2020 2020 2020 2053 5550  .            SUP
+000043f0: 4552 5343 5249 5054 2045 4947 4854 2c38  ERSCRIPT EIGHT,8
+00004400: 3331 322c 380a 2020 2020 2020 2020 2020  312,8.          
+00004410: 2020 5355 5045 5253 4352 4950 5420 4e49    SUPERSCRIPT NI
+00004420: 4e45 2c38 3331 332c 390a 2020 2020 2020  NE,8313,9.      
+00004430: 2020 2020 2020 4349 5243 4c45 4420 4449        CIRCLED DI
+00004440: 4749 5420 4f4e 452c 3933 3132 2c31 0a20  GIT ONE,9312,1. 
+00004450: 2020 2020 2020 2020 2020 2043 4952 434c             CIRCL
+00004460: 4544 2044 4947 4954 2054 574f 2c39 3331  ED DIGIT TWO,931
+00004470: 332c 320a 2020 2020 2020 2020 2020 2020  3,2.            
+00004480: 4349 5243 4c45 4420 4449 4749 5420 5448  CIRCLED DIGIT TH
+00004490: 5245 452c 3933 3134 2c33 0a20 2020 2020  REE,9314,3.     
+000044a0: 2020 2020 2020 2043 4952 434c 4544 2044         CIRCLED D
+000044b0: 4947 4954 2046 4f55 522c 3933 3135 2c34  IGIT FOUR,9315,4
+000044c0: 0a20 2020 2020 2020 2020 2020 2043 4952  .            CIR
+000044d0: 434c 4544 2044 4947 4954 2046 4956 452c  CLED DIGIT FIVE,
+000044e0: 3933 3136 2c35 0a20 2020 2020 2020 2020  9316,5.         
+000044f0: 2020 2043 4952 434c 4544 2044 4947 4954     CIRCLED DIGIT
+00004500: 2053 4958 2c39 3331 372c 360a 2020 2020   SIX,9317,6.    
+00004510: 2020 2020 2020 2020 4349 5243 4c45 4420          CIRCLED 
+00004520: 4449 4749 5420 5345 5645 4e2c 3933 3138  DIGIT SEVEN,9318
+00004530: 2c37 0a20 2020 2020 2020 2020 2020 2043  ,7.            C
+00004540: 4952 434c 4544 2044 4947 4954 2045 4947  IRCLED DIGIT EIG
+00004550: 4854 2c39 3331 392c 380a 2020 2020 2020  HT,9319,8.      
+00004560: 2020 2020 2020 4349 5243 4c45 4420 4449        CIRCLED DI
+00004570: 4749 5420 4e49 4e45 2c39 3332 302c 390a  GIT NINE,9320,9.
+00004580: 2020 2020 2020 2020 2020 2020 4349 5243              CIRC
+00004590: 4c45 4420 4449 4749 5420 5a45 524f 2c39  LED DIGIT ZERO,9
+000045a0: 3435 302c 300a 2020 2020 2020 2020 2020  450,0.          
+000045b0: 2020 2222 2229 290a 0a20 2020 2020 2020    """))..       
+000045c0: 206f 6e65 7320 3d20 756e 6963 6f64 655f   ones = unicode_
+000045d0: 6e75 6d62 6572 732e 7768 6572 6528 6e61  numbers.where(na
+000045e0: 6d65 3d6c 742e 5461 626c 652e 656e 6473  me=lt.Table.ends
+000045f0: 7769 7468 2822 4f4e 4522 2929 0a20 2020  with("ONE")).   
+00004600: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00004610: 4571 7561 6c28 332c 206c 656e 286f 6e65  Equal(3, len(one
+00004620: 7329 290a 0a20 2020 2020 2020 2073 7570  s))..        sup
+00004630: 6572 7320 3d20 756e 6963 6f64 655f 6e75  ers = unicode_nu
+00004640: 6d62 6572 732e 7768 6572 6528 6e61 6d65  mbers.where(name
+00004650: 3d6c 742e 5461 626c 652e 7374 6172 7473  =lt.Table.starts
+00004660: 7769 7468 2822 5355 5045 5253 4352 4950  with("SUPERSCRIP
+00004670: 5422 2929 0a20 2020 2020 2020 2073 656c  T")).        sel
+00004680: 662e 6173 7365 7274 4571 7561 6c28 3130  f.assertEqual(10
+00004690: 2c20 6c65 6e28 7375 7065 7273 2929 0a0a  , len(supers))..
+000046a0: 2020 2020 2020 2020 2320 696d 706f 7274          # import
+000046b0: 2072 650a 2020 2020 2020 2020 2320 7365   re.        # se
+000046c0: 7665 6e73 203d 2075 6e69 636f 6465 5f6e  vens = unicode_n
+000046d0: 756d 6265 7273 2e77 6865 7265 286c 616d  umbers.where(lam
+000046e0: 6264 6120 7265 633a 2072 652e 636f 6d70  bda rec: re.comp
+000046f0: 696c 6528 7222 2e2a 5345 5645 4e24 2229  ile(r".*SEVEN$")
+00004700: 2e6d 6174 6368 2872 6563 2e6e 616d 6529  .match(rec.name)
+00004710: 290a 0a20 2020 2020 2020 2073 6576 656e  )..        seven
+00004720: 7320 3d20 756e 6963 6f64 655f 6e75 6d62  s = unicode_numb
+00004730: 6572 732e 7768 6572 6528 6e61 6d65 3d6c  ers.where(name=l
+00004740: 742e 5461 626c 652e 7265 5f6d 6174 6368  t.Table.re_match
+00004750: 2872 222e 2a53 4556 454e 2422 2929 0a20  (r".*SEVEN$")). 
+00004760: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00004770: 7274 4571 7561 6c28 332c 206c 656e 2873  rtEqual(3, len(s
+00004780: 6576 656e 7329 290a 0a20 2020 2020 2020  evens))..       
+00004790: 2023 206d 616b 6520 6e61 6d65 7320 616c   # make names al
+000047a0: 6c20 7469 746c 6520 6361 7365 0a20 2020  l title case.   
+000047b0: 2020 2020 2075 6e69 636f 6465 5f6e 756d       unicode_num
+000047c0: 6265 7273 2e61 6464 5f66 6965 6c64 2822  bers.add_field("
+000047d0: 6e61 6d65 222c 206c 616d 6264 6120 7265  name", lambda re
+000047e0: 633a 2072 6563 2e6e 616d 652e 7469 746c  c: rec.name.titl
+000047f0: 6528 2929 0a20 2020 2020 2020 2023 2075  e()).        # u
+00004800: 7365 2072 6567 6578 2077 6974 6820 7265  se regex with re
+00004810: 2066 6c61 670a 2020 2020 2020 2020 696d   flag.        im
+00004820: 706f 7274 2072 650a 2020 2020 2020 2020  port re.        
+00004830: 6369 7263 6c65 6420 3d20 756e 6963 6f64  circled = unicod
+00004840: 655f 6e75 6d62 6572 732e 7768 6572 6528  e_numbers.where(
+00004850: 6e61 6d65 3d6c 742e 5461 626c 652e 7265  name=lt.Table.re
+00004860: 5f6d 6174 6368 2872 2263 6972 636c 6564  _match(r"circled
+00004870: 222c 2066 6c61 6773 3d72 652e 4929 290a  ", flags=re.I)).
+00004880: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00004890: 6572 7445 7175 616c 2831 302c 206c 656e  ertEqual(10, len
+000048a0: 2863 6972 636c 6564 2929 0a0a 2020 2020  (circled))..    
+000048b0: 6465 6620 7465 7374 5f77 6865 7265 5f61  def test_where_a
+000048c0: 7474 725f 6675 6e63 7469 6f6e 2873 656c  ttr_function(sel
+000048d0: 6629 3a0a 2020 2020 2020 2020 7465 7374  f):.        test
+000048e0: 5f73 697a 6520 3d20 380a 2020 2020 2020  _size = 8.      
+000048f0: 2020 7461 626c 6520 3d20 6d61 6b65 5f74    table = make_t
+00004900: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
+00004910: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
+00004920: 2074 6573 745f 7369 7a65 290a 0a20 2020   test_size)..   
+00004930: 2020 2020 2064 6566 2069 735f 6f64 6428       def is_odd(
+00004940: 7829 3a0a 2020 2020 2020 2020 2020 2020  x):.            
+00004950: 7265 7475 726e 2062 6f6f 6c28 7820 2520  return bool(x % 
+00004960: 3229 0a0a 2020 2020 2020 2020 7365 6c66  2)..        self
+00004970: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
+00004980: 745f 7369 7a65 2a74 6573 745f 7369 7a65  t_size*test_size
+00004990: 2a74 6573 745f 7369 7a65 2f2f 322c 206c  *test_size//2, l
+000049a0: 656e 2874 6162 6c65 2e77 6865 7265 2861  en(table.where(a
+000049b0: 3d69 735f 6f64 6429 2929 0a0a 2020 2020  =is_odd)))..    
+000049c0: 6465 6620 7465 7374 5f67 6574 5f73 6c69  def test_get_sli
+000049d0: 6365 2873 656c 6629 3a0a 2020 2020 2020  ce(self):.      
+000049e0: 2020 7465 7374 5f73 697a 6520 3d20 3130    test_size = 10
+000049f0: 0a20 2020 2020 2020 2074 6162 6c65 203d  .        table =
+00004a00: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
+00004a10: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
+00004a20: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
+00004a30: 6529 0a0a 2020 2020 2020 2020 7375 6274  e)..        subt
+00004a40: 6162 6c65 203d 2074 6162 6c65 5b30 3a3a  able = table[0::
+00004a50: 7465 7374 5f73 697a 655d 0a20 2020 2020  test_size].     
+00004a60: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00004a70: 7561 6c28 7465 7374 5f73 697a 6520 2a20  ual(test_size * 
+00004a80: 7465 7374 5f73 697a 652c 206c 656e 2873  test_size, len(s
+00004a90: 7562 7461 626c 6529 290a 0a20 2020 2064  ubtable))..    d
+00004aa0: 6566 2074 6573 745f 696e 6465 7869 6e67  ef test_indexing
+00004ab0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00004ac0: 6368 6172 7320 3d20 2241 4243 4445 4647  chars = "ABCDEFG
+00004ad0: 4849 4a4b 4c4d 4e4f 5051 5253 5455 5657  HIJKLMNOPQRSTUVW
+00004ae0: 5859 5a22 0a20 2020 2020 2020 206d 616b  XYZ".        mak
+00004af0: 655f 7265 6320 3d20 6c61 6d62 6461 2061  e_rec = lambda a
+00004b00: 612c 2062 622c 2063 633a 2073 656c 662e  a, bb, cc: self.
+00004b10: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
+00004b20: 2863 6861 7273 5b61 615d 2c20 6368 6172  (chars[aa], char
+00004b30: 735b 6262 5d2c 2063 6861 7273 5b63 635d  s[bb], chars[cc]
+00004b40: 290a 2020 2020 2020 2020 7465 7374 5f73  ).        test_s
+00004b50: 697a 6520 3d20 3130 0a20 2020 2020 2020  ize = 10.       
+00004b60: 2074 6162 6c65 203d 206d 616b 655f 7465   table = make_te
+00004b70: 7374 5f74 6162 6c65 286d 616b 655f 7265  st_table(make_re
+00004b80: 632c 2074 6573 745f 7369 7a65 290a 2020  c, test_size).  
+00004b90: 2020 2020 2020 7461 626c 652e 6372 6561        table.crea
+00004ba0: 7465 5f69 6e64 6578 2827 6127 290a 0a20  te_index('a').. 
+00004bb0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00004bc0: 7274 5472 7565 2827 4127 2069 6e20 7461  rtTrue('A' in ta
+00004bd0: 626c 652e 6279 2e61 290a 2020 2020 2020  ble.by.a).      
+00004be0: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+00004bf0: 6528 2741 4127 206e 6f74 2069 6e20 7461  e('AA' not in ta
+00004c00: 626c 652e 6279 2e61 290a 2020 2020 2020  ble.by.a).      
+00004c10: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00004c20: 616c 2874 6573 745f 7369 7a65 202a 2074  al(test_size * t
+00004c30: 6573 745f 7369 7a65 2c20 6c65 6e28 7461  est_size, len(ta
+00004c40: 626c 652e 6279 2e61 5b27 4227 5d29 290a  ble.by.a['B'])).
+00004c50: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00004c60: 6572 7454 7275 6528 6973 696e 7374 616e  ertTrue(isinstan
+00004c70: 6365 2874 6162 6c65 2e62 792e 615b 2742  ce(table.by.a['B
+00004c80: 275d 2c20 6c74 2e54 6162 6c65 2929 0a20  '], lt.Table)). 
+00004c90: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00004ca0: 2e61 7373 6572 7452 6169 7365 7328 4174  .assertRaises(At
+00004cb0: 7472 6962 7574 6545 7272 6f72 293a 0a20  tributeError):. 
+00004cc0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+00004cd0: 2e62 792e 7a0a 0a20 2020 2020 2020 2073  .by.z..        s
+00004ce0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00004cf0: 7465 7374 5f73 697a 652c 206c 656e 2874  test_size, len(t
+00004d00: 6162 6c65 2e62 792e 612e 6b65 7973 2829  able.by.a.keys()
+00004d10: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
+00004d20: 5f75 6e69 7175 655f 696e 6465 7869 6e67  _unique_indexing
+00004d30: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00004d40: 6368 6172 7320 3d20 2241 4243 4445 4647  chars = "ABCDEFG
+00004d50: 4849 4a4b 4c4d 4e4f 5051 5253 5455 5657  HIJKLMNOPQRSTUVW
+00004d60: 5859 5a22 0a20 2020 2020 2020 206d 616b  XYZ".        mak
+00004d70: 655f 756e 6971 7565 5f6b 6579 203d 206c  e_unique_key = l
+00004d80: 616d 6264 6120 2a61 7267 733a 2027 272e  ambda *args: ''.
+00004d90: 6a6f 696e 2863 6861 7273 5b61 7267 5d20  join(chars[arg] 
+00004da0: 666f 7220 6172 6720 696e 2061 7267 7329  for arg in args)
+00004db0: 0a20 2020 2020 2020 206d 616b 655f 7265  .        make_re
+00004dc0: 6320 3d20 6c61 6d62 6461 2061 612c 2062  c = lambda aa, b
+00004dd0: 622c 2063 633a 2073 656c 662e 6d61 6b65  b, cc: self.make
+00004de0: 5f64 6174 615f 6f62 6a65 6374 286d 616b  _data_object(mak
+00004df0: 655f 756e 6971 7565 5f6b 6579 2861 612c  e_unique_key(aa,
+00004e00: 2062 622c 2063 6329 2c20 6368 6172 735b   bb, cc), chars[
+00004e10: 6262 5d2c 2063 6861 7273 5b63 635d 290a  bb], chars[cc]).
+00004e20: 2020 2020 2020 2020 7465 7374 5f73 697a          test_siz
+00004e30: 6520 3d20 3130 0a20 2020 2020 2020 2074  e = 10.        t
+00004e40: 6162 6c65 203d 206d 616b 655f 7465 7374  able = make_test
+00004e50: 5f74 6162 6c65 286d 616b 655f 7265 632c  _table(make_rec,
+00004e60: 2074 6573 745f 7369 7a65 2928 2254 6162   test_size)("Tab
+00004e70: 6c65 5f31 2229 0a20 2020 2020 2020 2074  le_1").        t
+00004e80: 6162 6c65 2e63 7265 6174 655f 696e 6465  able.create_inde
+00004e90: 7828 2761 272c 2075 6e69 7175 653d 5472  x('a', unique=Tr
+00004ea0: 7565 290a 2020 2020 2020 2020 7265 635f  ue).        rec_
+00004eb0: 7479 7065 203d 2074 7970 6528 7365 6c66  type = type(self
+00004ec0: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
+00004ed0: 7428 302c 2030 2c20 3029 290a 0a20 2020  t(0, 0, 0))..   
+00004ee0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00004ef0: 5472 7565 2827 4141 4127 2069 6e20 7461  True('AAA' in ta
+00004f00: 626c 652e 6279 2e61 290a 2020 2020 2020  ble.by.a).      
+00004f10: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+00004f20: 6528 2741 4127 206e 6f74 2069 6e20 7461  e('AA' not in ta
+00004f30: 626c 652e 6279 2e61 290a 2020 2020 2020  ble.by.a).      
+00004f40: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+00004f50: 6528 6973 696e 7374 616e 6365 2874 6162  e(isinstance(tab
+00004f60: 6c65 2e62 792e 615b 2742 4141 275d 2c20  le.by.a['BAA'], 
+00004f70: 7265 635f 7479 7065 2929 0a20 2020 2020  rec_type)).     
+00004f80: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
+00004f90: 6572 7452 6169 7365 7328 4b65 7945 7272  ertRaises(KeyErr
+00004fa0: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+00004fb0: 2074 6162 6c65 2e69 6e73 6572 7428 7365   table.insert(se
+00004fc0: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
+00004fd0: 6563 7428 4e6f 6e65 2c20 4e6f 6e65 2c20  ect(None, None, 
+00004fe0: 4e6f 6e65 2929 0a0a 2020 2020 2020 2020  None))..        
+00004ff0: 2320 6372 6561 7465 2064 7570 6c69 6361  # create duplica
+00005000: 7465 2069 6e64 6578 0a20 2020 2020 2020  te index.       
+00005010: 2077 6974 6820 7365 6c66 2e61 7373 6572   with self.asser
+00005020: 7452 6169 7365 7328 5661 6c75 6545 7272  tRaises(ValueErr
+00005030: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+00005040: 2074 6162 6c65 2e63 7265 6174 655f 696e   table.create_in
+00005050: 6465 7828 2761 272c 2075 6e69 7175 653d  dex('a', unique=
+00005060: 5472 7565 2c20 6163 6365 7074 5f6e 6f6e  True, accept_non
+00005070: 653d 5472 7565 290a 0a20 2020 2020 2020  e=True)..       
+00005080: 2023 2063 7265 6174 6520 756e 6971 7565   # create unique
+00005090: 2069 6e64 6578 2074 6861 7420 616c 6c6f   index that allo
+000050a0: 7773 204e 6f6e 6520 7661 6c75 6573 0a20  ws None values. 
+000050b0: 2020 2020 2020 2074 6162 6c65 2e64 656c         table.del
+000050c0: 6574 655f 696e 6465 7828 2761 2729 0a20  ete_index('a'). 
+000050d0: 2020 2020 2020 2074 6162 6c65 2e63 7265         table.cre
+000050e0: 6174 655f 696e 6465 7828 2761 272c 2075  ate_index('a', u
+000050f0: 6e69 7175 653d 5472 7565 2c20 6163 6365  nique=True, acce
+00005100: 7074 5f6e 6f6e 653d 5472 7565 290a 2020  pt_none=True).  
+00005110: 2020 2020 2020 7461 626c 652e 696e 7365        table.inse
+00005120: 7274 2873 656c 662e 6d61 6b65 5f64 6174  rt(self.make_dat
+00005130: 615f 6f62 6a65 6374 284e 6f6e 652c 204e  a_object(None, N
+00005140: 6f6e 652c 2027 4127 2929 0a0a 2020 2020  one, 'A'))..    
+00005150: 2020 2020 7374 725f 6e6f 6e65 5f63 6f6d      str_none_com
+00005160: 7061 7265 203d 206c 616d 6264 6120 783a  pare = lambda x:
+00005170: 2078 2069 6620 6973 696e 7374 616e 6365   x if isinstance
+00005180: 2878 2c20 7374 7229 2065 6c73 6520 6368  (x, str) else ch
+00005190: 7228 3235 3529 2a31 3030 0a20 2020 2020  r(255)*100.     
+000051a0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000051b0: 7561 6c28 736f 7274 6564 2874 6162 6c65  ual(sorted(table
+000051c0: 2e62 792e 612e 6b65 7973 2829 2c20 6b65  .by.a.keys(), ke
+000051d0: 793d 7374 725f 6e6f 6e65 5f63 6f6d 7061  y=str_none_compa
+000051e0: 7265 292c 0a20 2020 2020 2020 2020 2020  re),.           
+000051f0: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00005200: 7274 6564 2874 6162 6c65 2e61 6c6c 2e61  rted(table.all.a
+00005210: 2c20 6b65 793d 7374 725f 6e6f 6e65 5f63  , key=str_none_c
+00005220: 6f6d 7061 7265 2929 0a0a 2020 2020 2020  ompare))..      
+00005230: 2020 2320 6e6f 7720 6472 6f70 2069 6e64    # now drop ind
+00005240: 6578 2061 6e64 2072 6563 7265 6174 6520  ex and recreate 
+00005250: 6e6f 7420 7065 726d 6974 7469 6e67 204e  not permitting N
+00005260: 6f6e 652c 2073 686f 756c 6420 7261 6973  one, should rais
+00005270: 6520 6578 6365 7074 696f 6e0a 2020 2020  e exception.    
+00005280: 2020 2020 7461 626c 652e 6465 6c65 7465      table.delete
+00005290: 5f69 6e64 6578 2827 6127 290a 2020 2020  _index('a').    
+000052a0: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
+000052b0: 7365 7274 5261 6973 6573 284b 6579 4572  sertRaises(KeyEr
+000052c0: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
+000052d0: 2020 7461 626c 652e 6372 6561 7465 5f69    table.create_i
+000052e0: 6e64 6578 2827 6127 2c20 756e 6971 7565  ndex('a', unique
+000052f0: 3d54 7275 652c 2061 6363 6570 745f 6e6f  =True, accept_no
+00005300: 6e65 3d46 616c 7365 290a 0a20 2020 2020  ne=False)..     
+00005310: 2020 2074 6162 6c65 2e63 7265 6174 655f     table.create_
+00005320: 696e 6465 7828 2761 272c 2075 6e69 7175  index('a', uniqu
+00005330: 653d 5472 7565 2c20 6163 6365 7074 5f6e  e=True, accept_n
+00005340: 6f6e 653d 5472 7565 290a 2020 2020 2020  one=True).      
+00005350: 2020 7461 626c 652e 6372 6561 7465 5f69    table.create_i
+00005360: 6e64 6578 2827 6327 290a 0a20 2020 2020  ndex('c')..     
+00005370: 2020 2069 6d70 6f72 7420 7070 7269 6e74     import pprint
+00005380: 0a20 2020 2020 2020 2069 6e66 6f20 3d20  .        info = 
+00005390: 7461 626c 652e 696e 666f 2829 0a20 2020  table.info().   
+000053a0: 2020 2020 2070 7072 696e 742e 7070 7269       pprint.ppri
+000053b0: 6e74 2869 6e66 6f29 0a20 2020 2020 2020  nt(info).       
+000053c0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000053d0: 6c28 2754 6162 6c65 5f31 272c 2069 6e66  l('Table_1', inf
+000053e0: 6f5b 276e 616d 6527 5d29 0a20 2020 2020  o['name']).     
+000053f0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00005400: 7561 6c28 5b27 6127 2c20 2762 272c 2027  ual(['a', 'b', '
+00005410: 6327 5d2c 206c 6973 7428 736f 7274 6564  c'], list(sorted
+00005420: 2869 6e66 6f5b 2766 6965 6c64 7327 5d29  (info['fields'])
+00005430: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00005440: 6173 7365 7274 4571 7561 6c28 5b28 2761  assertEqual([('a
+00005450: 272c 2054 7275 6529 2c20 2827 6327 2c20  ', True), ('c', 
+00005460: 4661 6c73 6529 5d2c 206c 6973 7428 736f  False)], list(so
+00005470: 7274 6564 2869 6e66 6f5b 2769 6e64 6578  rted(info['index
+00005480: 6573 275d 2929 290a 2020 2020 2020 2020  es']))).        
+00005490: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000054a0: 2831 3030 312c 2069 6e66 6f5b 276c 656e  (1001, info['len
+000054b0: 275d 290a 0a20 2020 2064 6566 2074 6573  '])..    def tes
+000054c0: 745f 6368 6169 6e65 645f 696e 6465 7869  t_chained_indexi
+000054d0: 6e67 2873 656c 6629 3a0a 2020 2020 2020  ng(self):.      
+000054e0: 2020 6368 6172 7320 3d20 2241 4243 4445    chars = "ABCDE
+000054f0: 4647 4849 4a4b 4c4d 4e4f 5051 5253 5455  FGHIJKLMNOPQRSTU
+00005500: 5657 5859 5a22 0a20 2020 2020 2020 206d  VWXYZ".        m
+00005510: 616b 655f 7265 6320 3d20 6c61 6d62 6461  ake_rec = lambda
+00005520: 2061 612c 2062 622c 2063 633a 2073 656c   aa, bb, cc: sel
+00005530: 662e 6d61 6b65 5f64 6174 615f 6f62 6a65  f.make_data_obje
+00005540: 6374 2863 6861 7273 5b61 6120 2520 6c65  ct(chars[aa % le
+00005550: 6e28 6368 6172 7329 5d2c 0a20 2020 2020  n(chars)],.     
+00005560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005590: 2020 2020 2020 2063 6861 7273 5b62 6220         chars[bb 
+000055a0: 2520 6c65 6e28 6368 6172 7329 5d2c 0a20  % len(chars)],. 
+000055b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055e0: 2020 2020 2020 2020 2020 2063 6861 7273             chars
+000055f0: 5b63 6320 2520 6c65 6e28 6368 6172 7329  [cc % len(chars)
+00005600: 5d29 0a20 2020 2020 2020 2074 6573 745f  ]).        test_
+00005610: 7369 7a65 203d 2031 300a 2020 2020 2020  size = 10.      
+00005620: 2020 7461 626c 6520 3d20 6d61 6b65 5f74    table = make_t
+00005630: 6573 745f 7461 626c 6528 6d61 6b65 5f72  est_table(make_r
+00005640: 6563 2c20 7465 7374 5f73 697a 6529 0a20  ec, test_size). 
+00005650: 2020 2020 2020 2074 6162 6c65 2e63 7265         table.cre
+00005660: 6174 655f 696e 6465 7828 2761 2729 0a20  ate_index('a'). 
+00005670: 2020 2020 2020 2074 6162 6c65 2e63 7265         table.cre
+00005680: 6174 655f 696e 6465 7828 2762 2729 0a20  ate_index('b'). 
+00005690: 2020 2020 2020 2074 6162 6c65 2e63 7265         table.cre
+000056a0: 6174 655f 696e 6465 7828 2763 2729 0a0a  ate_index('c')..
+000056b0: 2020 2020 2020 2020 6368 6169 6e65 645f          chained_
+000056c0: 7461 626c 6520 3d20 7461 626c 652e 6279  table = table.by
+000056d0: 2e62 5b27 4127 5d2e 6279 2e63 5b27 4327  .b['A'].by.c['C'
+000056e0: 5d0a 2020 2020 2020 2020 666f 7220 7265  ].        for re
+000056f0: 6320 696e 2063 6861 696e 6564 5f74 6162  c in chained_tab
+00005700: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+00005710: 7072 696e 7428 7265 6329 0a0a 2020 2020  print(rec)..    
+00005720: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00005730: 7175 616c 2874 6573 745f 7369 7a65 2c20  qual(test_size, 
+00005740: 6c65 6e28 6368 6169 6e65 645f 7461 626c  len(chained_tabl
+00005750: 6529 290a 0a20 2020 2064 6566 2074 6573  e))..    def tes
+00005760: 745f 7061 7273 655f 6461 7465 7469 6d65  t_parse_datetime
+00005770: 5f74 7261 6e73 666f 726d 2873 656c 6629  _transform(self)
+00005780: 3a0a 2020 2020 2020 2020 696d 706f 7274  :.        import
+00005790: 2064 6174 6574 696d 650a 0a20 2020 2020   datetime..     
+000057a0: 2020 2064 6174 6120 3d20 7465 7874 7772     data = textwr
+000057b0: 6170 2e64 6564 656e 7428 2222 225c 0a20  ap.dedent("""\. 
+000057c0: 2020 2020 2020 2061 2c62 2c63 0a20 2020         a,b,c.   
+000057d0: 2020 2020 2032 3030 312d 3031 2d30 3120       2001-01-01 
+000057e0: 3030 3a33 343a 3536 2c41 2c31 3030 0a20  00:34:56,A,100. 
+000057f0: 2020 2020 2020 2032 3030 312d 3031 2d30         2001-01-0
+00005800: 3220 3031 3a33 343a 3536 2c42 2c31 3031  2 01:34:56,B,101
+00005810: 0a20 2020 2020 2020 2032 3030 312d 3032  .        2001-02
+00005820: 2d33 3020 3032 3a33 343a 3536 2c43 2c31  -30 02:34:56,C,1
+00005830: 3032 0a20 2020 2020 2020 202c 442c 3130  02.        ,D,10
+00005840: 330a 2020 2020 2020 2020 2222 2229 0a20  3.        """). 
+00005850: 2020 2020 2020 2074 6573 745f 6b77 6172         test_kwar
+00005860: 6773 203d 205b 0a20 2020 2020 2020 2020  gs = [.         
+00005870: 2020 207b 2765 6d70 7479 273a 2027 272c     {'empty': '',
+00005880: 2027 6f6e 5f65 7272 6f72 273a 204e 6f6e   'on_error': Non
+00005890: 657d 2c0a 2020 2020 2020 2020 2020 2020  e},.            
+000058a0: 7b27 656d 7074 7927 3a20 274e 2f41 272c  {'empty': 'N/A',
+000058b0: 2027 6f6e 5f65 7272 6f72 273a 2064 6174   'on_error': dat
+000058c0: 6574 696d 652e 6461 7465 7469 6d65 2e6d  etime.datetime.m
+000058d0: 696e 7d2c 0a20 2020 2020 2020 2020 2020  in},.           
+000058e0: 207b 2765 6d70 7479 273a 2064 6174 6574   {'empty': datet
+000058f0: 696d 652e 6461 7465 7469 6d65 2e6d 696e  ime.datetime.min
+00005900: 2c20 276f 6e5f 6572 726f 7227 3a20 2727  , 'on_error': ''
+00005910: 7d2c 0a20 2020 2020 2020 205d 0a20 2020  },.        ].   
+00005920: 2020 2020 2066 6f72 206b 7761 7267 7320       for kwargs 
+00005930: 696e 2074 6573 745f 6b77 6172 6773 3a0a  in test_kwargs:.
+00005940: 2020 2020 2020 2020 2020 2020 7462 6c20              tbl 
+00005950: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
+00005960: 5f69 6d70 6f72 7428 6461 7461 2c0a 2020  _import(data,.  
+00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005990: 2020 2020 2020 7472 616e 7366 6f72 6d73        transforms
+000059a0: 3d7b 2761 273a 206c 742e 5461 626c 652e  ={'a': lt.Table.
+000059b0: 7061 7273 655f 6461 7465 7469 6d65 2827  parse_datetime('
+000059c0: 2559 2d25 6d2d 2564 2025 483a 254d 3a25  %Y-%m-%d %H:%M:%
+000059d0: 5327 2c0a 2020 2020 2020 2020 2020 2020  S',.            
+000059e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a10: 2020 2020 6461 7465 7469 6d65 2e64 6174      datetime.dat
-00005a20: 6574 696d 6528 3230 3031 2c20 312c 2032  etime(2001, 1, 2
-00005a30: 2c20 312c 2033 342c 2035 3629 5d2c 0a20  , 1, 34, 56)],. 
-00005a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a50: 2020 206c 6973 7428 7462 6c2e 616c 6c2e     list(tbl.all.
-00005a60: 6129 5b3a 325d 0a20 2020 2020 2020 2020  a)[:2].         
-00005a70: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-00005a80: 6620 7465 7374 5f70 6172 7365 5f64 6174  f test_parse_dat
-00005a90: 655f 7472 616e 7366 6f72 6d28 7365 6c66  e_transform(self
-00005aa0: 293a 0a20 2020 2020 2020 2069 6d70 6f72  ):.        impor
-00005ab0: 7420 6461 7465 7469 6d65 0a0a 2020 2020  t datetime..    
-00005ac0: 2020 2020 6461 7461 203d 2074 6578 7477      data = textw
-00005ad0: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
-00005ae0: 2020 2020 2020 2020 612c 622c 630a 2020          a,b,c.  
-00005af0: 2020 2020 2020 3230 3031 2d30 312d 3031        2001-01-01
-00005b00: 2030 303a 3334 3a35 362c 412c 3130 300a   00:34:56,A,100.
-00005b10: 2020 2020 2020 2020 3230 3031 2d30 312d          2001-01-
-00005b20: 3032 2030 313a 3334 3a35 362c 422c 3130  02 01:34:56,B,10
-00005b30: 310a 2020 2020 2020 2020 3230 3031 2d30  1.        2001-0
-00005b40: 322d 3330 2030 323a 3334 3a35 362c 432c  2-30 02:34:56,C,
-00005b50: 3130 320a 2020 2020 2020 2020 2c44 2c31  102.        ,D,1
-00005b60: 3033 0a20 2020 2020 2020 2022 2222 290a  03.        """).
-00005b70: 2020 2020 2020 2020 7465 7374 5f6b 7761          test_kwa
-00005b80: 7267 7320 3d20 5b0a 2020 2020 2020 2020  rgs = [.        
-00005b90: 2020 2020 7b27 656d 7074 7927 3a20 2727      {'empty': ''
-00005ba0: 2c20 276f 6e5f 6572 726f 7227 3a20 4e6f  , 'on_error': No
-00005bb0: 6e65 7d2c 0a20 2020 2020 2020 2020 2020  ne},.           
-00005bc0: 207b 2765 6d70 7479 273a 2027 4e2f 4127   {'empty': 'N/A'
-00005bd0: 2c20 276f 6e5f 6572 726f 7227 3a20 6461  , 'on_error': da
-00005be0: 7465 7469 6d65 2e64 6174 652e 6d69 6e7d  tetime.date.min}
-00005bf0: 2c0a 2020 2020 2020 2020 2020 2020 7b27  ,.            {'
-00005c00: 656d 7074 7927 3a20 6461 7465 7469 6d65  empty': datetime
-00005c10: 2e64 6174 652e 6d69 6e2c 2027 6f6e 5f65  .date.min, 'on_e
-00005c20: 7272 6f72 273a 2027 277d 2c0a 2020 2020  rror': ''},.    
-00005c30: 2020 2020 5d0a 2020 2020 2020 2020 666f      ].        fo
-00005c40: 7220 6b77 6172 6773 2069 6e20 7465 7374  r kwargs in test
-00005c50: 5f6b 7761 7267 733a 0a20 2020 2020 2020  _kwargs:.       
-00005c60: 2020 2020 2074 626c 203d 206c 742e 5461       tbl = lt.Ta
-00005c70: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
-00005c80: 2864 6174 612c 0a20 2020 2020 2020 2020  (data,.         
-00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ca0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00005cb0: 7261 6e73 666f 726d 733d 7b27 6127 3a20  ransforms={'a': 
-00005cc0: 6c74 2e54 6162 6c65 2e70 6172 7365 5f64  lt.Table.parse_d
-00005cd0: 6174 6528 2725 592d 256d 2d25 6420 2548  ate('%Y-%m-%d %H
-00005ce0: 3a25 4d3a 2553 272c 0a20 2020 2020 2020  :%M:%S',.       
-00005cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d30: 2020 2020 2020 2a2a 6b77 6172 6773 297d        **kwargs)}
-00005d40: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00005d50: 696e 7428 5b73 7472 2861 2920 666f 7220  int([str(a) for 
-00005d60: 6120 696e 2074 626c 2e61 6c6c 2e61 5d29  a in tbl.all.a])
-00005d70: 0a0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-00005d80: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00005d90: 2274 6573 7420 5461 626c 652e 7061 7273  "test Table.pars
-00005da0: 655f 6461 7465 5f74 696d 6520 6572 726f  e_date_time erro
-00005db0: 7273 222c 202a 2a6b 7761 7267 7329 3a0a  rs", **kwargs):.
-00005dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005dd0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00005de0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00005df0: 2020 2020 2020 5b6b 7761 7267 735b 226f        [kwargs["o
-00005e00: 6e5f 6572 726f 7222 5d2c 206b 7761 7267  n_error"], kwarg
-00005e10: 735b 2265 6d70 7479 225d 5d2c 0a20 2020  s["empty"]],.   
-00005e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e30: 206c 6973 7428 7462 6c2e 616c 6c2e 6129   list(tbl.all.a)
-00005e40: 5b2d 323a 5d0a 2020 2020 2020 2020 2020  [-2:].          
-00005e50: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00005e60: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-00005e70: 7562 5465 7374 2822 7465 7374 2054 6162  ubTest("test Tab
-00005e80: 6c65 2e70 6172 7365 5f64 6174 655f 7469  le.parse_date_ti
-00005e90: 6d65 2076 616c 6964 222c 202a 2a6b 7761  me valid", **kwa
-00005ea0: 7267 7329 3a0a 2020 2020 2020 2020 2020  rgs):.          
-00005eb0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00005ec0: 7445 7175 616c 280a 2020 2020 2020 2020  tEqual(.        
-00005ed0: 2020 2020 2020 2020 2020 2020 5b64 6174              [dat
-00005ee0: 6574 696d 652e 6461 7465 2832 3030 312c  etime.date(2001,
-00005ef0: 2031 2c20 3129 2c0a 2020 2020 2020 2020   1, 1),.        
-00005f00: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-00005f10: 6574 696d 652e 6461 7465 2832 3030 312c  etime.date(2001,
-00005f20: 2031 2c20 3229 5d2c 0a20 2020 2020 2020   1, 2)],.       
-00005f30: 2020 2020 2020 2020 2020 2020 206c 6973               lis
-00005f40: 7428 7462 6c2e 616c 6c2e 6129 5b3a 325d  t(tbl.all.a)[:2]
-00005f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005f60: 2029 0a0a 2020 2020 6465 6620 7465 7374   )..    def test
-00005f70: 5f70 6172 7365 5f74 696d 6564 656c 7461  _parse_timedelta
-00005f80: 5f74 7261 6e73 666f 726d 2873 656c 6629  _transform(self)
-00005f90: 3a0a 2020 2020 2020 2020 696d 706f 7274  :.        import
-00005fa0: 2064 6174 6574 696d 650a 0a20 2020 2020   datetime..     
-00005fb0: 2020 2070 726f 6365 7373 5f64 6174 6120     process_data 
-00005fc0: 3d20 7465 7874 7772 6170 2e64 6564 656e  = textwrap.deden
-00005fd0: 7428 2222 225c 0a20 2020 2020 2020 2020  t("""\.         
-00005fe0: 2020 2065 6c61 7073 6564 5f74 696d 652c     elapsed_time,
-00005ff0: 6571 7074 2c65 7665 6e74 2c6c 6f74 2c70  eqpt,event,lot,p
-00006000: 6965 6365 730a 2020 2020 2020 2020 2020  ieces.          
-00006010: 2020 303a 3030 3a30 302c 4452 494c 4c30    0:00:00,DRILL0
-00006020: 312c 4c6f 7453 7461 7274 2c50 4342 3134  1,LotStart,PCB14
-00006030: 362c 310a 2020 2020 2020 2020 2020 2020  6,1.            
-00006040: 303a 3030 3a34 302c 4452 494c 4c30 312c  0:00:40,DRILL01,
-00006050: 546f 6f6c 312c 5043 4231 3436 2c32 0a20  Tool1,PCB146,2. 
-00006060: 2020 2020 2020 2020 2020 2030 3a30 333a             0:03:
-00006070: 3435 2c44 5249 4c4c 3031 2c54 6f6f 6c32  45,DRILL01,Tool2
-00006080: 2c50 4342 3134 362c 340a 2020 2020 2020  ,PCB146,4.      
-00006090: 2020 2020 2020 303a 3036 3a31 362c 4452        0:06:16,DR
-000060a0: 494c 4c30 312c 4c6f 7445 6e64 2c50 4342  ILL01,LotEnd,PCB
-000060b0: 3134 362c 380a 2020 2020 2020 2020 2020  146,8.          
-000060c0: 2020 2222 2229 0a0a 2020 2020 2020 2020    """)..        
-000060d0: 7472 616e 7366 6f72 6d73 203d 207b 2765  transforms = {'e
-000060e0: 6c61 7073 6564 5f74 696d 6527 3a20 6c74  lapsed_time': lt
-000060f0: 2e54 6162 6c65 2e70 6172 7365 5f74 696d  .Table.parse_tim
-00006100: 6564 656c 7461 2822 2548 3a25 4d3a 2553  edelta("%H:%M:%S
-00006110: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-00006120: 2020 2020 2020 2020 2020 2770 6965 6365            'piece
-00006130: 7327 3a20 696e 747d 0a20 2020 2020 2020  s': int}.       
-00006140: 2064 6174 6120 3d20 6c74 2e54 6162 6c65   data = lt.Table
-00006150: 2866 2250 726f 6365 7373 2073 7465 7020  (f"Process step 
-00006160: 656c 6170 7365 6420 7469 6d65 7322 292e  elapsed times").
-00006170: 6373 765f 696d 706f 7274 2870 726f 6365  csv_import(proce
-00006180: 7373 5f64 6174 612c 2074 7261 6e73 666f  ss_data, transfo
-00006190: 726d 733d 7472 616e 7366 6f72 6d73 290a  rms=transforms).
-000061a0: 2020 2020 2020 2020 6461 7461 2e63 7265          data.cre
-000061b0: 6174 655f 696e 6465 7828 2265 6c61 7073  ate_index("elaps
-000061c0: 6564 5f74 696d 6522 290a 0a20 2020 2020  ed_time")..     
-000061d0: 2020 205f 3030 5f30 315f 3330 203d 2064     _00_01_30 = d
-000061e0: 6174 6574 696d 652e 7469 6d65 6465 6c74  atetime.timedelt
-000061f0: 6128 7365 636f 6e64 733d 3930 290a 2020  a(seconds=90).  
-00006200: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00006210: 7445 7175 616c 2833 2c20 7375 6d28 6461  tEqual(3, sum(da
-00006220: 7461 2e62 792e 656c 6170 7365 645f 7469  ta.by.elapsed_ti
-00006230: 6d65 5b3a 5f30 305f 3031 5f33 305d 2e61  me[:_00_01_30].a
-00006240: 6c6c 2e70 6965 6365 7329 290a 0a20 2020  ll.pieces))..   
-00006250: 2064 6566 2074 6573 745f 736c 6963 6564   def test_sliced
-00006260: 5f69 6e64 6578 696e 6728 7365 6c66 293a  _indexing(self):
-00006270: 0a20 2020 2020 2020 2074 7261 6e73 666f  .        transfo
-00006280: 726d 7320 3d20 7b0a 2020 2020 2020 2020  rms = {.        
-00006290: 2020 2020 2770 6f70 273a 2069 6e74 2c0a      'pop': int,.
-000062a0: 2020 2020 2020 2020 2020 2020 2765 6c65              'ele
-000062b0: 7627 3a20 696e 742c 0a20 2020 2020 2020  v': int,.       
-000062c0: 2020 2020 2027 6c61 7427 3a20 666c 6f61       'lat': floa
-000062d0: 742c 0a20 2020 2020 2020 2020 2020 2027  t,.            '
-000062e0: 6c6f 6e67 273a 2066 6c6f 6174 2c0a 2020  long': float,.  
-000062f0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00006300: 7573 5f70 706c 203d 206c 742e 5461 626c  us_ppl = lt.Tabl
-00006310: 6528 292e 6373 765f 696d 706f 7274 2822  e().csv_import("
-00006320: 6578 616d 706c 6573 2f75 735f 7070 6c2e  examples/us_ppl.
-00006330: 6373 7622 2c0a 2020 2020 2020 2020 2020  csv",.          
-00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006350: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-00006360: 6e73 666f 726d 733d 7472 616e 7366 6f72  nsforms=transfor
-00006370: 6d73 2c0a 2020 2020 2020 2020 2020 2020  ms,.            
-00006380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006390: 2020 2020 2020 2020 2020 2029 2e73 656c             ).sel
-000063a0: 6563 7428 2269 6420 6e61 6d65 2065 6c65  ect("id name ele
-000063b0: 7620 6c61 7420 6c6f 6e67 2070 6f70 2229  v lat long pop")
-000063c0: 0a20 2020 2020 2020 2070 7269 6e74 2875  .        print(u
-000063d0: 735f 7070 6c2e 696e 666f 2829 290a 2020  s_ppl.info()).  
-000063e0: 2020 2020 2020 7573 5f70 706c 2e63 7265        us_ppl.cre
-000063f0: 6174 655f 696e 6465 7828 226e 616d 6522  ate_index("name"
-00006400: 290a 2020 2020 2020 2020 7573 5f70 706c  ).        us_ppl
-00006410: 2e63 7265 6174 655f 696e 6465 7828 2265  .create_index("e
-00006420: 6c65 7622 290a 0a20 2020 2020 2020 2074  lev")..        t
-00006430: 6573 7420 3d20 2265 6c65 7620 3c20 3022  est = "elev < 0"
-00006440: 0a20 2020 2020 2020 206c 6f77 5f70 706c  .        low_ppl
-00006450: 5f77 6865 7265 203d 2075 735f 7070 6c2e  _where = us_ppl.
-00006460: 7768 6572 6528 656c 6576 3d6c 742e 5461  where(elev=lt.Ta
-00006470: 626c 652e 6c74 2830 2929 2874 6573 7429  ble.lt(0))(test)
-00006480: 0a20 2020 2020 2020 206c 6f77 5f70 706c  .        low_ppl
-00006490: 5f73 6c69 6365 203d 2075 735f 7070 6c2e  _slice = us_ppl.
-000064a0: 6279 2e65 6c65 765b 3a30 5d28 6622 7b74  by.elev[:0](f"{t
-000064b0: 6573 747d 2028 736c 6963 6564 2922 290a  est} (sliced)").
-000064c0: 2020 2020 2020 2020 6c6f 775f 7070 6c5f          low_ppl_
-000064d0: 736c 6963 652e 7072 6573 656e 7428 290a  slice.present().
-000064e0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-000064f0: 6572 7445 7175 616c 286c 6973 7428 6c6f  ertEqual(list(lo
-00006500: 775f 7070 6c5f 7768 6572 652e 616c 6c2e  w_ppl_where.all.
-00006510: 6964 292c 206c 6973 7428 6c6f 775f 7070  id), list(low_pp
-00006520: 6c5f 736c 6963 652e 616c 6c2e 6964 2929  l_slice.all.id))
-00006530: 0a0a 2020 2020 2020 2020 7465 7374 203d  ..        test =
-00006540: 2022 656c 6576 203e 3d20 3130 3030 220a   "elev >= 1000".
-00006550: 2020 2020 2020 2020 6869 5f70 706c 5f77          hi_ppl_w
-00006560: 6865 7265 203d 2075 735f 7070 6c2e 7768  here = us_ppl.wh
-00006570: 6572 6528 656c 6576 3d6c 742e 5461 626c  ere(elev=lt.Tabl
-00006580: 652e 6765 2831 3030 3029 2928 7465 7374  e.ge(1000))(test
-00006590: 290a 2020 2020 2020 2020 6869 5f70 706c  ).        hi_ppl
-000065a0: 5f73 6c69 6365 203d 2075 735f 7070 6c2e  _slice = us_ppl.
-000065b0: 6279 2e65 6c65 765b 3130 3030 3a5d 2866  by.elev[1000:](f
-000065c0: 227b 7465 7374 7d20 2873 6c69 6365 6429  "{test} (sliced)
-000065d0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-000065e0: 6173 7365 7274 4571 7561 6c28 6c69 7374  assertEqual(list
-000065f0: 2868 695f 7070 6c5f 7768 6572 652e 616c  (hi_ppl_where.al
-00006600: 6c2e 6964 292c 206c 6973 7428 6869 5f70  l.id), list(hi_p
-00006610: 706c 5f73 6c69 6365 2e61 6c6c 2e69 6429  pl_slice.all.id)
-00006620: 290a 0a20 2020 2020 2020 2074 6573 7420  )..        test 
-00006630: 3d20 2230 203c 3d20 656c 6576 203c 2031  = "0 <= elev < 1
-00006640: 3030 220a 2020 2020 2020 2020 6c6f 775f  00".        low_
-00006650: 7070 6c5f 7768 6572 6520 3d20 7573 5f70  ppl_where = us_p
-00006660: 706c 2e77 6865 7265 2865 6c65 763d 6c74  pl.where(elev=lt
-00006670: 2e54 6162 6c65 2e67 6528 3029 292e 7768  .Table.ge(0)).wh
-00006680: 6572 6528 656c 6576 3d6c 742e 5461 626c  ere(elev=lt.Tabl
-00006690: 652e 6c74 2831 3030 2929 2874 6573 7429  e.lt(100))(test)
-000066a0: 0a20 2020 2020 2020 206c 6f77 5f70 706c  .        low_ppl
-000066b0: 5f73 6c69 6365 203d 2075 735f 7070 6c2e  _slice = us_ppl.
-000066c0: 6279 2e65 6c65 765b 303a 3130 305d 2866  by.elev[0:100](f
-000066d0: 227b 7465 7374 7d20 2873 6c69 6365 6429  "{test} (sliced)
-000066e0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-000066f0: 6173 7365 7274 4571 7561 6c28 6c69 7374  assertEqual(list
-00006700: 286c 6f77 5f70 706c 5f77 6865 7265 2e61  (low_ppl_where.a
-00006710: 6c6c 2e69 6429 2c20 6c69 7374 286c 6f77  ll.id), list(low
-00006720: 5f70 706c 5f73 6c69 6365 2e61 6c6c 2e69  _ppl_slice.all.i
-00006730: 6429 290a 0a20 2020 2020 2020 2061 5f70  d))..        a_p
-00006740: 706c 5f77 6865 7265 203d 2075 735f 7070  pl_where = us_pp
-00006750: 6c2e 7768 6572 6528 6e61 6d65 3d6c 742e  l.where(name=lt.
-00006760: 5461 626c 652e 6765 2822 4122 2929 2e77  Table.ge("A")).w
-00006770: 6865 7265 286e 616d 653d 6c74 2e54 6162  here(name=lt.Tab
-00006780: 6c65 2e6c 7428 2243 2229 290a 2020 2020  le.lt("C")).    
-00006790: 2020 2020 615f 7070 6c5f 736c 6963 6520      a_ppl_slice 
-000067a0: 3d20 7573 5f70 706c 2e62 792e 6e61 6d65  = us_ppl.by.name
-000067b0: 5b22 4122 3a22 4322 5d0a 2020 2020 2020  ["A":"C"].      
-000067c0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000067d0: 616c 286c 6973 7428 615f 7070 6c5f 7768  al(list(a_ppl_wh
-000067e0: 6572 652e 616c 6c2e 6964 292c 206c 6973  ere.all.id), lis
-000067f0: 7428 615f 7070 6c5f 736c 6963 652e 616c  t(a_ppl_slice.al
-00006800: 6c2e 6964 2929 0a0a 2020 2020 6465 6620  l.id))..    def 
-00006810: 7465 7374 5f6e 6f6e 5f69 6e74 6567 6572  test_non_integer
-00006820: 5f73 6c69 6365 645f 696e 6465 7869 6e67  _sliced_indexing
-00006830: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00006840: 696d 706f 7274 2064 6174 6574 696d 650a  import datetime.
-00006850: 0a20 2020 2020 2020 2073 616c 6573 5f64  .        sales_d
-00006860: 6174 6120 3d20 7465 7874 7772 6170 2e64  ata = textwrap.d
-00006870: 6564 656e 7428 2222 225c 0a20 2020 2020  edent("""\.     
-00006880: 2020 2020 2020 2064 6174 652c 6375 7374         date,cust
-00006890: 6f6d 6572 2c73 6b75 2c71 7479 0a20 2020  omer,sku,qty.   
-000068a0: 2020 2020 2020 2020 2032 3030 302f 3031           2000/01
-000068b0: 2f30 312c 3030 3230 2c41 4e56 494c 2d30  /01,0020,ANVIL-0
-000068c0: 3031 2c31 0a20 2020 2020 2020 2020 2020  01,1.           
-000068d0: 2032 3030 302f 3031 2f30 312c 3030 3230   2000/01/01,0020
-000068e0: 2c42 5244 5344 2d30 3031 2c32 0a20 2020  ,BRDSD-001,2.   
-000068f0: 2020 2020 2020 2020 2032 3030 302f 3032           2000/02
-00006900: 2f31 352c 3030 3230 2c42 5244 5344 2d30  /15,0020,BRDSD-0
-00006910: 3031 2c34 0a20 2020 2020 2020 2020 2020  01,4.           
-00006920: 2032 3030 302f 3033 2f33 312c 3030 3230   2000/03/31,0020
-00006930: 2c42 5244 5344 2d30 3031 2c38 0a20 2020  ,BRDSD-001,8.   
-00006940: 2020 2020 2020 2020 2032 3030 302f 3033           2000/03
-00006950: 2f33 312c 3030 3230 2c4d 4147 4e54 2d30  /31,0020,MAGNT-0
-00006960: 3031 2c31 360a 2020 2020 2020 2020 2020  01,16.          
-00006970: 2020 3230 3030 2f30 342f 3031 2c30 3032    2000/04/01,002
-00006980: 302c 524f 424f 542d 3030 312c 3332 0a20  0,ROBOT-001,32. 
-00006990: 2020 2020 2020 2020 2020 2032 3030 302f             2000/
-000069a0: 3034 2f31 352c 3030 3230 2c42 5244 5344  04/15,0020,BRDSD
-000069b0: 2d30 3031 2c36 340a 2020 2020 2020 2020  -001,64.        
-000069c0: 2020 2020 2222 2229 0a0a 2020 2020 2020      """)..      
-000069d0: 2020 7472 616e 7366 6f72 6d73 203d 207b    transforms = {
-000069e0: 2764 6174 6527 3a20 6c74 2e54 6162 6c65  'date': lt.Table
-000069f0: 2e70 6172 7365 5f64 6174 6528 2225 592f  .parse_date("%Y/
-00006a00: 256d 2f25 6422 292c 0a20 2020 2020 2020  %m/%d"),.       
-00006a10: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00006a20: 7174 7927 3a20 696e 747d 0a20 2020 2020  qty': int}.     
-00006a30: 2020 2073 616c 6573 203d 206c 742e 5461     sales = lt.Ta
-00006a40: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
-00006a50: 2873 616c 6573 5f64 6174 612c 0a20 2020  (sales_data,.   
-00006a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a80: 2020 2074 7261 6e73 666f 726d 733d 7472     transforms=tr
-00006a90: 616e 7366 6f72 6d73 2c29 0a0a 2020 2020  ansforms,)..    
-00006aa0: 2020 2020 7361 6c65 732e 6372 6561 7465      sales.create
-00006ab0: 5f69 6e64 6578 2822 6461 7465 2229 0a20  _index("date"). 
-00006ac0: 2020 2020 2020 206a 616e 5f30 3120 3d20         jan_01 = 
-00006ad0: 6461 7465 7469 6d65 2e64 6174 6528 3230  datetime.date(20
-00006ae0: 3030 2c20 312c 2031 290a 2020 2020 2020  00, 1, 1).      
-00006af0: 2020 6170 725f 3031 203d 2064 6174 6574    apr_01 = datet
-00006b00: 696d 652e 6461 7465 2832 3030 302c 2034  ime.date(2000, 4
-00006b10: 2c20 3129 0a20 2020 2020 2020 2066 6972  , 1).        fir
-00006b20: 7374 5f71 7472 5f73 616c 6573 203d 2073  st_qtr_sales = s
-00006b30: 616c 6573 2e62 792e 6461 7465 5b6a 616e  ales.by.date[jan
-00006b40: 5f30 313a 2061 7072 5f30 315d 0a20 2020  _01: apr_01].   
-00006b50: 2020 2020 2066 6972 7374 5f71 7472 5f73       first_qtr_s
-00006b60: 616c 6573 2e70 7265 7365 6e74 2829 0a20  ales.present(). 
-00006b70: 2020 2020 2020 2070 7269 6e74 286c 6973         print(lis
-00006b80: 7428 6669 7273 745f 7174 725f 7361 6c65  t(first_qtr_sale
-00006b90: 732e 616c 6c2e 736b 7529 290a 0a20 2020  s.all.sku))..   
-00006ba0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00006bb0: 4571 7561 6c28 6c69 7374 2866 6972 7374  Equal(list(first
-00006bc0: 5f71 7472 5f73 616c 6573 2e61 6c6c 2e73  _qtr_sales.all.s
-00006bd0: 6b75 292c 0a20 2020 2020 2020 2020 2020  ku),.           
-00006be0: 2020 2020 2020 2020 2020 2020 2020 5b27                ['
-00006bf0: 414e 5649 4c2d 3030 3127 2c20 2742 5244  ANVIL-001', 'BRD
-00006c00: 5344 2d30 3031 272c 2027 4252 4453 442d  SD-001', 'BRDSD-
-00006c10: 3030 3127 2c20 2742 5244 5344 2d30 3031  001', 'BRDSD-001
-00006c20: 272c 2027 4d41 474e 542d 3030 3127 5d2c  ', 'MAGNT-001'],
-00006c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006c40: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00006c50: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00006c60: 7175 616c 2833 312c 2073 756d 2866 6972  qual(31, sum(fir
-00006c70: 7374 5f71 7472 5f73 616c 6573 2e61 6c6c  st_qtr_sales.all
-00006c80: 2e71 7479 2929 0a0a 2020 2020 2020 2020  .qty))..        
-00006c90: 2320 7573 6520 6461 7465 2073 7472 696e  # use date strin
-00006ca0: 6773 2061 7320 7261 6e67 6520 7661 6c75  gs as range valu
-00006cb0: 6573 0a20 2020 2020 2020 2074 7261 6e73  es.        trans
-00006cc0: 666f 726d 7320 3d20 7b27 7174 7927 3a20  forms = {'qty': 
-00006cd0: 696e 747d 0a20 2020 2020 2020 2073 616c  int}.        sal
-00006ce0: 6573 203d 206c 742e 5461 626c 6528 292e  es = lt.Table().
-00006cf0: 6373 765f 696d 706f 7274 2873 616c 6573  csv_import(sales
-00006d00: 5f64 6174 612c 0a20 2020 2020 2020 2020  _data,.         
-00006d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d20: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-00006d30: 6e73 666f 726d 733d 7472 616e 7366 6f72  nsforms=transfor
-00006d40: 6d73 2c29 0a0a 2020 2020 2020 2020 7361  ms,)..        sa
-00006d50: 6c65 732e 6372 6561 7465 5f69 6e64 6578  les.create_index
-00006d60: 2822 6461 7465 2229 0a20 2020 2020 2020  ("date").       
-00006d70: 2066 6972 7374 5f71 7472 5f73 616c 6573   first_qtr_sales
-00006d80: 203d 2073 616c 6573 2e62 792e 6461 7465   = sales.by.date
-00006d90: 5b22 3230 3030 2f30 312f 3031 223a 2022  ["2000/01/01": "
-00006da0: 3230 3030 2f30 342f 3031 225d 0a20 2020  2000/04/01"].   
-00006db0: 2020 2020 2066 6972 7374 5f71 7472 5f73       first_qtr_s
-00006dc0: 616c 6573 2e70 7265 7365 6e74 2829 0a20  ales.present(). 
-00006dd0: 2020 2020 2020 2070 7269 6e74 286c 6973         print(lis
-00006de0: 7428 6669 7273 745f 7174 725f 7361 6c65  t(first_qtr_sale
-00006df0: 732e 616c 6c2e 736b 7529 290a 0a20 2020  s.all.sku))..   
-00006e00: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00006e10: 4571 7561 6c28 6c69 7374 2866 6972 7374  Equal(list(first
-00006e20: 5f71 7472 5f73 616c 6573 2e61 6c6c 2e73  _qtr_sales.all.s
-00006e30: 6b75 292c 0a20 2020 2020 2020 2020 2020  ku),.           
-00006e40: 2020 2020 2020 2020 2020 2020 2020 5b27                ['
-00006e50: 414e 5649 4c2d 3030 3127 2c20 2742 5244  ANVIL-001', 'BRD
-00006e60: 5344 2d30 3031 272c 2027 4252 4453 442d  SD-001', 'BRDSD-
-00006e70: 3030 3127 2c20 2742 5244 5344 2d30 3031  001', 'BRDSD-001
-00006e80: 272c 2027 4d41 474e 542d 3030 3127 5d2c  ', 'MAGNT-001'],
-00006e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006ea0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00006eb0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00006ec0: 7175 616c 2833 312c 2073 756d 2866 6972  qual(31, sum(fir
-00006ed0: 7374 5f71 7472 5f73 616c 6573 2e61 6c6c  st_qtr_sales.all
-00006ee0: 2e71 7479 2929 0a0a 2020 2020 2020 2020  .qty))..        
-00006ef0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00006f00: 2833 312c 2073 756d 2873 616c 6573 2e62  (31, sum(sales.b
-00006f10: 792e 6461 7465 5b3a 2232 3030 302f 3034  y.date[:"2000/04
-00006f20: 2f30 3122 5d2e 616c 6c2e 7174 7929 290a  /01"].all.qty)).
-00006f30: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00006f40: 6572 7445 7175 616c 2839 362c 2073 756d  ertEqual(96, sum
-00006f50: 2873 616c 6573 2e62 792e 6461 7465 5b22  (sales.by.date["
-00006f60: 3230 3030 2f30 342f 3031 223a 5d2e 616c  2000/04/01":].al
-00006f70: 6c2e 7174 7929 290a 0a20 2020 2064 6566  l.qty))..    def
-00006f80: 2074 6573 745f 696e 6465 785f 6469 7228   test_index_dir(
-00006f90: 7365 6c66 293a 0a20 2020 2020 2020 2063  self):.        c
-00006fa0: 6861 7273 203d 2022 4142 4344 4546 4748  hars = "ABCDEFGH
-00006fb0: 494a 4b4c 4d4e 4f50 5152 5354 5556 5758  IJKLMNOPQRSTUVWX
-00006fc0: 595a 220a 2020 2020 2020 2020 6d61 6b65  YZ".        make
-00006fd0: 5f72 6563 203d 206c 616d 6264 6120 6161  _rec = lambda aa
-00006fe0: 2c20 6262 2c20 6363 3a20 7365 6c66 2e6d  , bb, cc: self.m
-00006ff0: 616b 655f 6461 7461 5f6f 626a 6563 7428  ake_data_object(
-00007000: 6368 6172 735b 6161 2025 206c 656e 2863  chars[aa % len(c
-00007010: 6861 7273 295d 2c0a 2020 2020 2020 2020  hars)],.        
-00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a20: 2020 2020 202a 2a6b 7761 7267 7329 7d29       **kwargs)})
+00005a30: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00005a40: 6e74 285b 7374 7228 6129 2066 6f72 2061  nt([str(a) for a
+00005a50: 2069 6e20 7462 6c2e 616c 6c2e 615d 290a   in tbl.all.a]).
+00005a60: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00005a70: 6820 7365 6c66 2e73 7562 5465 7374 2822  h self.subTest("
+00005a80: 7465 7374 2054 6162 6c65 2e70 6172 7365  test Table.parse
+00005a90: 5f64 6174 655f 7469 6d65 2065 7272 6f72  _date_time error
+00005aa0: 7322 2c20 2a2a 6b77 6172 6773 293a 0a20  s", **kwargs):. 
+00005ab0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005ac0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00005ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005ae0: 2020 2020 205b 6b77 6172 6773 5b22 6f6e       [kwargs["on
+00005af0: 5f65 7272 6f72 225d 2c20 6b77 6172 6773  _error"], kwargs
+00005b00: 5b22 656d 7074 7922 5d5d 2c0a 2020 2020  ["empty"]],.    
+00005b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b20: 6c69 7374 2874 626c 2e61 6c6c 2e61 295b  list(tbl.all.a)[
+00005b30: 2d32 3a5d 0a20 2020 2020 2020 2020 2020  -2:].           
+00005b40: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00005b50: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+00005b60: 6254 6573 7428 2274 6573 7420 5461 626c  bTest("test Tabl
+00005b70: 652e 7061 7273 655f 6461 7465 5f74 696d  e.parse_date_tim
+00005b80: 6520 7661 6c69 6422 2c20 2a2a 6b77 6172  e valid", **kwar
+00005b90: 6773 293a 0a20 2020 2020 2020 2020 2020  gs):.           
+00005ba0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00005bb0: 4571 7561 6c28 0a20 2020 2020 2020 2020  Equal(.         
+00005bc0: 2020 2020 2020 2020 2020 205b 6461 7465             [date
+00005bd0: 7469 6d65 2e64 6174 6574 696d 6528 3230  time.datetime(20
+00005be0: 3031 2c20 312c 2031 2c20 302c 2033 342c  01, 1, 1, 0, 34,
+00005bf0: 2035 3629 2c0a 2020 2020 2020 2020 2020   56),.          
+00005c00: 2020 2020 2020 2020 2020 2064 6174 6574             datet
+00005c10: 696d 652e 6461 7465 7469 6d65 2832 3030  ime.datetime(200
+00005c20: 312c 2031 2c20 322c 2031 2c20 3334 2c20  1, 1, 2, 1, 34, 
+00005c30: 3536 295d 2c0a 2020 2020 2020 2020 2020  56)],.          
+00005c40: 2020 2020 2020 2020 2020 6c69 7374 2874            list(t
+00005c50: 626c 2e61 6c6c 2e61 295b 3a32 5d0a 2020  bl.all.a)[:2].  
+00005c60: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00005c70: 0a20 2020 2064 6566 2074 6573 745f 7061  .    def test_pa
+00005c80: 7273 655f 6461 7465 5f74 7261 6e73 666f  rse_date_transfo
+00005c90: 726d 2873 656c 6629 3a0a 2020 2020 2020  rm(self):.      
+00005ca0: 2020 696d 706f 7274 2064 6174 6574 696d    import datetim
+00005cb0: 650a 0a20 2020 2020 2020 2064 6174 6120  e..        data 
+00005cc0: 3d20 7465 7874 7772 6170 2e64 6564 656e  = textwrap.deden
+00005cd0: 7428 2222 225c 0a20 2020 2020 2020 2061  t("""\.        a
+00005ce0: 2c62 2c63 0a20 2020 2020 2020 2032 3030  ,b,c.        200
+00005cf0: 312d 3031 2d30 3120 3030 3a33 343a 3536  1-01-01 00:34:56
+00005d00: 2c41 2c31 3030 0a20 2020 2020 2020 2032  ,A,100.        2
+00005d10: 3030 312d 3031 2d30 3220 3031 3a33 343a  001-01-02 01:34:
+00005d20: 3536 2c42 2c31 3031 0a20 2020 2020 2020  56,B,101.       
+00005d30: 2032 3030 312d 3032 2d33 3020 3032 3a33   2001-02-30 02:3
+00005d40: 343a 3536 2c43 2c31 3032 0a20 2020 2020  4:56,C,102.     
+00005d50: 2020 202c 442c 3130 330a 2020 2020 2020     ,D,103.      
+00005d60: 2020 2222 2229 0a20 2020 2020 2020 2074    """).        t
+00005d70: 6573 745f 6b77 6172 6773 203d 205b 0a20  est_kwargs = [. 
+00005d80: 2020 2020 2020 2020 2020 207b 2765 6d70             {'emp
+00005d90: 7479 273a 2027 272c 2027 6f6e 5f65 7272  ty': '', 'on_err
+00005da0: 6f72 273a 204e 6f6e 657d 2c0a 2020 2020  or': None},.    
+00005db0: 2020 2020 2020 2020 7b27 656d 7074 7927          {'empty'
+00005dc0: 3a20 274e 2f41 272c 2027 6f6e 5f65 7272  : 'N/A', 'on_err
+00005dd0: 6f72 273a 2064 6174 6574 696d 652e 6461  or': datetime.da
+00005de0: 7465 2e6d 696e 7d2c 0a20 2020 2020 2020  te.min},.       
+00005df0: 2020 2020 207b 2765 6d70 7479 273a 2064       {'empty': d
+00005e00: 6174 6574 696d 652e 6461 7465 2e6d 696e  atetime.date.min
+00005e10: 2c20 276f 6e5f 6572 726f 7227 3a20 2727  , 'on_error': ''
+00005e20: 7d2c 0a20 2020 2020 2020 205d 0a20 2020  },.        ].   
+00005e30: 2020 2020 2066 6f72 206b 7761 7267 7320       for kwargs 
+00005e40: 696e 2074 6573 745f 6b77 6172 6773 3a0a  in test_kwargs:.
+00005e50: 2020 2020 2020 2020 2020 2020 7462 6c20              tbl 
+00005e60: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
+00005e70: 5f69 6d70 6f72 7428 6461 7461 2c0a 2020  _import(data,.  
+00005e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ea0: 2020 2020 2020 7472 616e 7366 6f72 6d73        transforms
+00005eb0: 3d7b 2761 273a 206c 742e 5461 626c 652e  ={'a': lt.Table.
+00005ec0: 7061 7273 655f 6461 7465 2827 2559 2d25  parse_date('%Y-%
+00005ed0: 6d2d 2564 2025 483a 254d 3a25 5327 2c0a  m-%d %H:%M:%S',.
+00005ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f20: 2020 2020 2020 2020 2020 2020 202a 2a6b               **k
+00005f30: 7761 7267 7329 7d29 0a20 2020 2020 2020  wargs)}).       
+00005f40: 2020 2020 2070 7269 6e74 285b 7374 7228       print([str(
+00005f50: 6129 2066 6f72 2061 2069 6e20 7462 6c2e  a) for a in tbl.
+00005f60: 616c 6c2e 615d 290a 0a20 2020 2020 2020  all.a])..       
+00005f70: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+00005f80: 7562 5465 7374 2822 7465 7374 2054 6162  ubTest("test Tab
+00005f90: 6c65 2e70 6172 7365 5f64 6174 655f 7469  le.parse_date_ti
+00005fa0: 6d65 2065 7272 6f72 7322 2c20 2a2a 6b77  me errors", **kw
+00005fb0: 6172 6773 293a 0a20 2020 2020 2020 2020  args):.         
+00005fc0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00005fd0: 7274 4571 7561 6c28 0a20 2020 2020 2020  rtEqual(.       
+00005fe0: 2020 2020 2020 2020 2020 2020 205b 6b77               [kw
+00005ff0: 6172 6773 5b22 6f6e 5f65 7272 6f72 225d  args["on_error"]
+00006000: 2c20 6b77 6172 6773 5b22 656d 7074 7922  , kwargs["empty"
+00006010: 5d5d 2c0a 2020 2020 2020 2020 2020 2020  ]],.            
+00006020: 2020 2020 2020 2020 6c69 7374 2874 626c          list(tbl
+00006030: 2e61 6c6c 2e61 295b 2d32 3a5d 0a20 2020  .all.a)[-2:].   
+00006040: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+00006050: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00006060: 2073 656c 662e 7375 6254 6573 7428 2274   self.subTest("t
+00006070: 6573 7420 5461 626c 652e 7061 7273 655f  est Table.parse_
+00006080: 6461 7465 5f74 696d 6520 7661 6c69 6422  date_time valid"
+00006090: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+000060a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000060b0: 662e 6173 7365 7274 4571 7561 6c28 0a20  f.assertEqual(. 
+000060c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060d0: 2020 205b 6461 7465 7469 6d65 2e64 6174     [datetime.dat
+000060e0: 6528 3230 3031 2c20 312c 2031 292c 0a20  e(2001, 1, 1),. 
+000060f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006100: 2020 2020 6461 7465 7469 6d65 2e64 6174      datetime.dat
+00006110: 6528 3230 3031 2c20 312c 2032 295d 2c0a  e(2001, 1, 2)],.
+00006120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006130: 2020 2020 6c69 7374 2874 626c 2e61 6c6c      list(tbl.all
+00006140: 2e61 295b 3a32 5d0a 2020 2020 2020 2020  .a)[:2].        
+00006150: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+00006160: 6566 2074 6573 745f 7061 7273 655f 7469  ef test_parse_ti
+00006170: 6d65 6465 6c74 615f 7472 616e 7366 6f72  medelta_transfor
+00006180: 6d28 7365 6c66 293a 0a20 2020 2020 2020  m(self):.       
+00006190: 2069 6d70 6f72 7420 6461 7465 7469 6d65   import datetime
+000061a0: 0a0a 2020 2020 2020 2020 7072 6f63 6573  ..        proces
+000061b0: 735f 6461 7461 203d 2074 6578 7477 7261  s_data = textwra
+000061c0: 702e 6465 6465 6e74 2822 2222 5c0a 2020  p.dedent("""\.  
+000061d0: 2020 2020 2020 2020 2020 656c 6170 7365            elapse
+000061e0: 645f 7469 6d65 2c65 7170 742c 6576 656e  d_time,eqpt,even
+000061f0: 742c 6c6f 742c 7069 6563 6573 0a20 2020  t,lot,pieces.   
+00006200: 2020 2020 2020 2020 2030 3a30 303a 3030           0:00:00
+00006210: 2c44 5249 4c4c 3031 2c4c 6f74 5374 6172  ,DRILL01,LotStar
+00006220: 742c 5043 4231 3436 2c31 0a20 2020 2020  t,PCB146,1.     
+00006230: 2020 2020 2020 2030 3a30 303a 3430 2c44         0:00:40,D
+00006240: 5249 4c4c 3031 2c54 6f6f 6c31 2c50 4342  RILL01,Tool1,PCB
+00006250: 3134 362c 320a 2020 2020 2020 2020 2020  146,2.          
+00006260: 2020 303a 3033 3a34 352c 4452 494c 4c30    0:03:45,DRILL0
+00006270: 312c 546f 6f6c 322c 5043 4231 3436 2c34  1,Tool2,PCB146,4
+00006280: 0a20 2020 2020 2020 2020 2020 2030 3a30  .            0:0
+00006290: 363a 3136 2c44 5249 4c4c 3031 2c4c 6f74  6:16,DRILL01,Lot
+000062a0: 456e 642c 5043 4231 3436 2c38 0a20 2020  End,PCB146,8.   
+000062b0: 2020 2020 2020 2020 2022 2222 290a 0a20           """).. 
+000062c0: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+000062d0: 7320 3d20 7b27 656c 6170 7365 645f 7469  s = {'elapsed_ti
+000062e0: 6d65 273a 206c 742e 5461 626c 652e 7061  me': lt.Table.pa
+000062f0: 7273 655f 7469 6d65 6465 6c74 6128 2225  rse_timedelta("%
+00006300: 483a 254d 3a25 5322 292c 0a20 2020 2020  H:%M:%S"),.     
+00006310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006320: 2027 7069 6563 6573 273a 2069 6e74 7d0a   'pieces': int}.
+00006330: 2020 2020 2020 2020 6461 7461 203d 206c          data = l
+00006340: 742e 5461 626c 6528 6622 5072 6f63 6573  t.Table(f"Proces
+00006350: 7320 7374 6570 2065 6c61 7073 6564 2074  s step elapsed t
+00006360: 696d 6573 2229 2e63 7376 5f69 6d70 6f72  imes").csv_impor
+00006370: 7428 7072 6f63 6573 735f 6461 7461 2c20  t(process_data, 
+00006380: 7472 616e 7366 6f72 6d73 3d74 7261 6e73  transforms=trans
+00006390: 666f 726d 7329 0a20 2020 2020 2020 2064  forms).        d
+000063a0: 6174 612e 6372 6561 7465 5f69 6e64 6578  ata.create_index
+000063b0: 2822 656c 6170 7365 645f 7469 6d65 2229  ("elapsed_time")
+000063c0: 0a0a 2020 2020 2020 2020 5f30 305f 3031  ..        _00_01
+000063d0: 5f33 3020 3d20 6461 7465 7469 6d65 2e74  _30 = datetime.t
+000063e0: 696d 6564 656c 7461 2873 6563 6f6e 6473  imedelta(seconds
+000063f0: 3d39 3029 0a20 2020 2020 2020 2073 656c  =90).        sel
+00006400: 662e 6173 7365 7274 4571 7561 6c28 332c  f.assertEqual(3,
+00006410: 2073 756d 2864 6174 612e 6279 2e65 6c61   sum(data.by.ela
+00006420: 7073 6564 5f74 696d 655b 3a5f 3030 5f30  psed_time[:_00_0
+00006430: 315f 3330 5d2e 616c 6c2e 7069 6563 6573  1_30].all.pieces
+00006440: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
+00006450: 5f73 6c69 6365 645f 696e 6465 7869 6e67  _sliced_indexing
+00006460: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00006470: 7472 616e 7366 6f72 6d73 203d 207b 0a20  transforms = {. 
+00006480: 2020 2020 2020 2020 2020 2027 706f 7027             'pop'
+00006490: 3a20 696e 742c 0a20 2020 2020 2020 2020  : int,.         
+000064a0: 2020 2027 656c 6576 273a 2069 6e74 2c0a     'elev': int,.
+000064b0: 2020 2020 2020 2020 2020 2020 276c 6174              'lat
+000064c0: 273a 2066 6c6f 6174 2c0a 2020 2020 2020  ': float,.      
+000064d0: 2020 2020 2020 276c 6f6e 6727 3a20 666c        'long': fl
+000064e0: 6f61 742c 0a20 2020 2020 2020 207d 0a20  oat,.        }. 
+000064f0: 2020 2020 2020 2075 735f 7070 6c20 3d20         us_ppl = 
+00006500: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
+00006510: 6d70 6f72 7428 2265 7861 6d70 6c65 732f  mport("examples/
+00006520: 7573 5f70 706c 2e63 7376 222c 0a20 2020  us_ppl.csv",.   
+00006530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006550: 2020 2020 7472 616e 7366 6f72 6d73 3d74      transforms=t
+00006560: 7261 6e73 666f 726d 732c 0a20 2020 2020  ransforms,.     
+00006570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006590: 2020 292e 7365 6c65 6374 2822 6964 206e    ).select("id n
+000065a0: 616d 6520 656c 6576 206c 6174 206c 6f6e  ame elev lat lon
+000065b0: 6720 706f 7022 290a 2020 2020 2020 2020  g pop").        
+000065c0: 7072 696e 7428 7573 5f70 706c 2e69 6e66  print(us_ppl.inf
+000065d0: 6f28 2929 0a20 2020 2020 2020 2075 735f  o()).        us_
+000065e0: 7070 6c2e 6372 6561 7465 5f69 6e64 6578  ppl.create_index
+000065f0: 2822 6e61 6d65 2229 0a20 2020 2020 2020  ("name").       
+00006600: 2075 735f 7070 6c2e 6372 6561 7465 5f69   us_ppl.create_i
+00006610: 6e64 6578 2822 656c 6576 2229 0a0a 2020  ndex("elev")..  
+00006620: 2020 2020 2020 7465 7374 203d 2022 656c        test = "el
+00006630: 6576 203c 2030 220a 2020 2020 2020 2020  ev < 0".        
+00006640: 6c6f 775f 7070 6c5f 7768 6572 6520 3d20  low_ppl_where = 
+00006650: 7573 5f70 706c 2e77 6865 7265 2865 6c65  us_ppl.where(ele
+00006660: 763d 6c74 2e54 6162 6c65 2e6c 7428 3029  v=lt.Table.lt(0)
+00006670: 2928 7465 7374 290a 2020 2020 2020 2020  )(test).        
+00006680: 6c6f 775f 7070 6c5f 736c 6963 6520 3d20  low_ppl_slice = 
+00006690: 7573 5f70 706c 2e62 792e 656c 6576 5b3a  us_ppl.by.elev[:
+000066a0: 305d 2866 227b 7465 7374 7d20 2873 6c69  0](f"{test} (sli
+000066b0: 6365 6429 2229 0a20 2020 2020 2020 206c  ced)").        l
+000066c0: 6f77 5f70 706c 5f73 6c69 6365 2e70 7265  ow_ppl_slice.pre
+000066d0: 7365 6e74 2829 0a20 2020 2020 2020 2073  sent().        s
+000066e0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000066f0: 6c69 7374 286c 6f77 5f70 706c 5f77 6865  list(low_ppl_whe
+00006700: 7265 2e61 6c6c 2e69 6429 2c20 6c69 7374  re.all.id), list
+00006710: 286c 6f77 5f70 706c 5f73 6c69 6365 2e61  (low_ppl_slice.a
+00006720: 6c6c 2e69 6429 290a 0a20 2020 2020 2020  ll.id))..       
+00006730: 2074 6573 7420 3d20 2265 6c65 7620 3e3d   test = "elev >=
+00006740: 2031 3030 3022 0a20 2020 2020 2020 2068   1000".        h
+00006750: 695f 7070 6c5f 7768 6572 6520 3d20 7573  i_ppl_where = us
+00006760: 5f70 706c 2e77 6865 7265 2865 6c65 763d  _ppl.where(elev=
+00006770: 6c74 2e54 6162 6c65 2e67 6528 3130 3030  lt.Table.ge(1000
+00006780: 2929 2874 6573 7429 0a20 2020 2020 2020  ))(test).       
+00006790: 2068 695f 7070 6c5f 736c 6963 6520 3d20   hi_ppl_slice = 
+000067a0: 7573 5f70 706c 2e62 792e 656c 6576 5b31  us_ppl.by.elev[1
+000067b0: 3030 303a 5d28 6622 7b74 6573 747d 2028  000:](f"{test} (
+000067c0: 736c 6963 6564 2922 290a 2020 2020 2020  sliced)").      
+000067d0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000067e0: 616c 286c 6973 7428 6869 5f70 706c 5f77  al(list(hi_ppl_w
+000067f0: 6865 7265 2e61 6c6c 2e69 6429 2c20 6c69  here.all.id), li
+00006800: 7374 2868 695f 7070 6c5f 736c 6963 652e  st(hi_ppl_slice.
+00006810: 616c 6c2e 6964 2929 0a0a 2020 2020 2020  all.id))..      
+00006820: 2020 7465 7374 203d 2022 3020 3c3d 2065    test = "0 <= e
+00006830: 6c65 7620 3c20 3130 3022 0a20 2020 2020  lev < 100".     
+00006840: 2020 206c 6f77 5f70 706c 5f77 6865 7265     low_ppl_where
+00006850: 203d 2075 735f 7070 6c2e 7768 6572 6528   = us_ppl.where(
+00006860: 656c 6576 3d6c 742e 5461 626c 652e 6765  elev=lt.Table.ge
+00006870: 2830 2929 2e77 6865 7265 2865 6c65 763d  (0)).where(elev=
+00006880: 6c74 2e54 6162 6c65 2e6c 7428 3130 3029  lt.Table.lt(100)
+00006890: 2928 7465 7374 290a 2020 2020 2020 2020  )(test).        
+000068a0: 6c6f 775f 7070 6c5f 736c 6963 6520 3d20  low_ppl_slice = 
+000068b0: 7573 5f70 706c 2e62 792e 656c 6576 5b30  us_ppl.by.elev[0
+000068c0: 3a31 3030 5d28 6622 7b74 6573 747d 2028  :100](f"{test} (
+000068d0: 736c 6963 6564 2922 290a 2020 2020 2020  sliced)").      
+000068e0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000068f0: 616c 286c 6973 7428 6c6f 775f 7070 6c5f  al(list(low_ppl_
+00006900: 7768 6572 652e 616c 6c2e 6964 292c 206c  where.all.id), l
+00006910: 6973 7428 6c6f 775f 7070 6c5f 736c 6963  ist(low_ppl_slic
+00006920: 652e 616c 6c2e 6964 2929 0a0a 2020 2020  e.all.id))..    
+00006930: 2020 2020 615f 7070 6c5f 7768 6572 6520      a_ppl_where 
+00006940: 3d20 7573 5f70 706c 2e77 6865 7265 286e  = us_ppl.where(n
+00006950: 616d 653d 6c74 2e54 6162 6c65 2e67 6528  ame=lt.Table.ge(
+00006960: 2241 2229 292e 7768 6572 6528 6e61 6d65  "A")).where(name
+00006970: 3d6c 742e 5461 626c 652e 6c74 2822 4322  =lt.Table.lt("C"
+00006980: 2929 0a20 2020 2020 2020 2061 5f70 706c  )).        a_ppl
+00006990: 5f73 6c69 6365 203d 2075 735f 7070 6c2e  _slice = us_ppl.
+000069a0: 6279 2e6e 616d 655b 2241 223a 2243 225d  by.name["A":"C"]
+000069b0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+000069c0: 7365 7274 4571 7561 6c28 6c69 7374 2861  sertEqual(list(a
+000069d0: 5f70 706c 5f77 6865 7265 2e61 6c6c 2e69  _ppl_where.all.i
+000069e0: 6429 2c20 6c69 7374 2861 5f70 706c 5f73  d), list(a_ppl_s
+000069f0: 6c69 6365 2e61 6c6c 2e69 6429 290a 0a20  lice.all.id)).. 
+00006a00: 2020 2064 6566 2074 6573 745f 6e6f 6e5f     def test_non_
+00006a10: 696e 7465 6765 725f 736c 6963 6564 5f69  integer_sliced_i
+00006a20: 6e64 6578 696e 6728 7365 6c66 293a 0a20  ndexing(self):. 
+00006a30: 2020 2020 2020 2069 6d70 6f72 7420 6461         import da
+00006a40: 7465 7469 6d65 0a0a 2020 2020 2020 2020  tetime..        
+00006a50: 7361 6c65 735f 6461 7461 203d 2074 6578  sales_data = tex
+00006a60: 7477 7261 702e 6465 6465 6e74 2822 2222  twrap.dedent("""
+00006a70: 5c0a 2020 2020 2020 2020 2020 2020 6461  \.            da
+00006a80: 7465 2c63 7573 746f 6d65 722c 736b 752c  te,customer,sku,
+00006a90: 7174 790a 2020 2020 2020 2020 2020 2020  qty.            
+00006aa0: 3230 3030 2f30 312f 3031 2c30 3032 302c  2000/01/01,0020,
+00006ab0: 414e 5649 4c2d 3030 312c 310a 2020 2020  ANVIL-001,1.    
+00006ac0: 2020 2020 2020 2020 3230 3030 2f30 312f          2000/01/
+00006ad0: 3031 2c30 3032 302c 4252 4453 442d 3030  01,0020,BRDSD-00
+00006ae0: 312c 320a 2020 2020 2020 2020 2020 2020  1,2.            
+00006af0: 3230 3030 2f30 322f 3135 2c30 3032 302c  2000/02/15,0020,
+00006b00: 4252 4453 442d 3030 312c 340a 2020 2020  BRDSD-001,4.    
+00006b10: 2020 2020 2020 2020 3230 3030 2f30 332f          2000/03/
+00006b20: 3331 2c30 3032 302c 4252 4453 442d 3030  31,0020,BRDSD-00
+00006b30: 312c 380a 2020 2020 2020 2020 2020 2020  1,8.            
+00006b40: 3230 3030 2f30 332f 3331 2c30 3032 302c  2000/03/31,0020,
+00006b50: 4d41 474e 542d 3030 312c 3136 0a20 2020  MAGNT-001,16.   
+00006b60: 2020 2020 2020 2020 2032 3030 302f 3034           2000/04
+00006b70: 2f30 312c 3030 3230 2c52 4f42 4f54 2d30  /01,0020,ROBOT-0
+00006b80: 3031 2c33 320a 2020 2020 2020 2020 2020  01,32.          
+00006b90: 2020 3230 3030 2f30 342f 3135 2c30 3032    2000/04/15,002
+00006ba0: 302c 4252 4453 442d 3030 312c 3634 0a20  0,BRDSD-001,64. 
+00006bb0: 2020 2020 2020 2020 2020 2022 2222 290a             """).
+00006bc0: 0a20 2020 2020 2020 2074 7261 6e73 666f  .        transfo
+00006bd0: 726d 7320 3d20 7b27 6461 7465 273a 206c  rms = {'date': l
+00006be0: 742e 5461 626c 652e 7061 7273 655f 6461  t.Table.parse_da
+00006bf0: 7465 2822 2559 2f25 6d2f 2564 2229 2c0a  te("%Y/%m/%d"),.
+00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c10: 2020 2020 2020 2771 7479 273a 2069 6e74        'qty': int
+00006c20: 7d0a 2020 2020 2020 2020 7361 6c65 7320  }.        sales 
+00006c30: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
+00006c40: 5f69 6d70 6f72 7428 7361 6c65 735f 6461  _import(sales_da
+00006c50: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+00006c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c70: 2020 2020 2020 2020 2020 7472 616e 7366            transf
+00006c80: 6f72 6d73 3d74 7261 6e73 666f 726d 732c  orms=transforms,
+00006c90: 290a 0a20 2020 2020 2020 2073 616c 6573  )..        sales
+00006ca0: 2e63 7265 6174 655f 696e 6465 7828 2264  .create_index("d
+00006cb0: 6174 6522 290a 2020 2020 2020 2020 6a61  ate").        ja
+00006cc0: 6e5f 3031 203d 2064 6174 6574 696d 652e  n_01 = datetime.
+00006cd0: 6461 7465 2832 3030 302c 2031 2c20 3129  date(2000, 1, 1)
+00006ce0: 0a20 2020 2020 2020 2061 7072 5f30 3120  .        apr_01 
+00006cf0: 3d20 6461 7465 7469 6d65 2e64 6174 6528  = datetime.date(
+00006d00: 3230 3030 2c20 342c 2031 290a 2020 2020  2000, 4, 1).    
+00006d10: 2020 2020 6669 7273 745f 7174 725f 7361      first_qtr_sa
+00006d20: 6c65 7320 3d20 7361 6c65 732e 6279 2e64  les = sales.by.d
+00006d30: 6174 655b 6a61 6e5f 3031 3a20 6170 725f  ate[jan_01: apr_
+00006d40: 3031 5d0a 2020 2020 2020 2020 6669 7273  01].        firs
+00006d50: 745f 7174 725f 7361 6c65 732e 7072 6573  t_qtr_sales.pres
+00006d60: 656e 7428 290a 2020 2020 2020 2020 7072  ent().        pr
+00006d70: 696e 7428 6c69 7374 2866 6972 7374 5f71  int(list(first_q
+00006d80: 7472 5f73 616c 6573 2e61 6c6c 2e73 6b75  tr_sales.all.sku
+00006d90: 2929 0a0a 2020 2020 2020 2020 7365 6c66  ))..        self
+00006da0: 2e61 7373 6572 7445 7175 616c 286c 6973  .assertEqual(lis
+00006db0: 7428 6669 7273 745f 7174 725f 7361 6c65  t(first_qtr_sale
+00006dc0: 732e 616c 6c2e 736b 7529 2c0a 2020 2020  s.all.sku),.    
+00006dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006de0: 2020 2020 205b 2741 4e56 494c 2d30 3031       ['ANVIL-001
+00006df0: 272c 2027 4252 4453 442d 3030 3127 2c20  ', 'BRDSD-001', 
+00006e00: 2742 5244 5344 2d30 3031 272c 2027 4252  'BRDSD-001', 'BR
+00006e10: 4453 442d 3030 3127 2c20 274d 4147 4e54  DSD-001', 'MAGNT
+00006e20: 2d30 3031 275d 2c0a 2020 2020 2020 2020  -001'],.        
+00006e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e40: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
+00006e50: 6173 7365 7274 4571 7561 6c28 3331 2c20  assertEqual(31, 
+00006e60: 7375 6d28 6669 7273 745f 7174 725f 7361  sum(first_qtr_sa
+00006e70: 6c65 732e 616c 6c2e 7174 7929 290a 0a20  les.all.qty)).. 
+00006e80: 2020 2020 2020 2023 2075 7365 2064 6174         # use dat
+00006e90: 6520 7374 7269 6e67 7320 6173 2072 616e  e strings as ran
+00006ea0: 6765 2076 616c 7565 730a 2020 2020 2020  ge values.      
+00006eb0: 2020 7472 616e 7366 6f72 6d73 203d 207b    transforms = {
+00006ec0: 2771 7479 273a 2069 6e74 7d0a 2020 2020  'qty': int}.    
+00006ed0: 2020 2020 7361 6c65 7320 3d20 6c74 2e54      sales = lt.T
+00006ee0: 6162 6c65 2829 2e63 7376 5f69 6d70 6f72  able().csv_impor
+00006ef0: 7428 7361 6c65 735f 6461 7461 2c0a 2020  t(sales_data,.  
+00006f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f20: 2020 2020 7472 616e 7366 6f72 6d73 3d74      transforms=t
+00006f30: 7261 6e73 666f 726d 732c 290a 0a20 2020  ransforms,)..   
+00006f40: 2020 2020 2073 616c 6573 2e63 7265 6174       sales.creat
+00006f50: 655f 696e 6465 7828 2264 6174 6522 290a  e_index("date").
+00006f60: 2020 2020 2020 2020 6669 7273 745f 7174          first_qt
+00006f70: 725f 7361 6c65 7320 3d20 7361 6c65 732e  r_sales = sales.
+00006f80: 6279 2e64 6174 655b 2232 3030 302f 3031  by.date["2000/01
+00006f90: 2f30 3122 3a20 2232 3030 302f 3034 2f30  /01": "2000/04/0
+00006fa0: 3122 5d0a 2020 2020 2020 2020 6669 7273  1"].        firs
+00006fb0: 745f 7174 725f 7361 6c65 732e 7072 6573  t_qtr_sales.pres
+00006fc0: 656e 7428 290a 2020 2020 2020 2020 7072  ent().        pr
+00006fd0: 696e 7428 6c69 7374 2866 6972 7374 5f71  int(list(first_q
+00006fe0: 7472 5f73 616c 6573 2e61 6c6c 2e73 6b75  tr_sales.all.sku
+00006ff0: 2929 0a0a 2020 2020 2020 2020 7365 6c66  ))..        self
+00007000: 2e61 7373 6572 7445 7175 616c 286c 6973  .assertEqual(lis
+00007010: 7428 6669 7273 745f 7174 725f 7361 6c65  t(first_qtr_sale
+00007020: 732e 616c 6c2e 736b 7529 2c0a 2020 2020  s.all.sku),.    
 00007030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007050: 2020 2020 6368 6172 735b 6262 2025 206c      chars[bb % l
-00007060: 656e 2863 6861 7273 295d 2c0a 2020 2020  en(chars)],.    
-00007070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007040: 2020 2020 205b 2741 4e56 494c 2d30 3031       ['ANVIL-001
+00007050: 272c 2027 4252 4453 442d 3030 3127 2c20  ', 'BRDSD-001', 
+00007060: 2742 5244 5344 2d30 3031 272c 2027 4252  'BRDSD-001', 'BR
+00007070: 4453 442d 3030 3127 2c20 274d 4147 4e54  DSD-001', 'MAGNT
+00007080: 2d30 3031 275d 2c0a 2020 2020 2020 2020  -001'],.        
 00007090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070a0: 2020 2020 2020 2020 6368 6172 735b 6363          chars[cc
-000070b0: 2025 206c 656e 2863 6861 7273 295d 290a   % len(chars)]).
-000070c0: 2020 2020 2020 2020 7465 7374 5f73 697a          test_siz
-000070d0: 6520 3d20 3130 0a20 2020 2020 2020 2074  e = 10.        t
-000070e0: 6162 6c65 203d 206d 616b 655f 7465 7374  able = make_test
-000070f0: 5f74 6162 6c65 286d 616b 655f 7265 632c  _table(make_rec,
-00007100: 2074 6573 745f 7369 7a65 290a 2020 2020   test_size).    
-00007110: 2020 2020 7461 626c 652e 6372 6561 7465      table.create
-00007120: 5f69 6e64 6578 2827 6127 290a 2020 2020  _index('a').    
-00007130: 2020 2020 7461 626c 652e 6372 6561 7465      table.create
-00007140: 5f69 6e64 6578 2827 6227 290a 0a20 2020  _index('b')..   
-00007150: 2020 2020 2064 6972 5f6c 6973 7420 3d20       dir_list = 
-00007160: 6469 7228 7461 626c 652e 6279 290a 2020  dir(table.by).  
-00007170: 2020 2020 2020 7072 696e 7428 5b61 7474        print([att
-00007180: 7220 666f 7220 6174 7472 2069 6e20 6469  r for attr in di
-00007190: 725f 6c69 7374 2069 6620 6e6f 7420 6174  r_list if not at
-000071a0: 7472 2e73 7461 7274 7377 6974 6828 225f  tr.startswith("_
-000071b0: 2229 5d29 0a0a 2020 2020 2020 2020 7365  ")])..        se
-000071c0: 6c66 2e61 7373 6572 7454 7275 6528 2827  lf.assertTrue(('
-000071d0: 6127 2069 6e20 6469 725f 6c69 7374 2920  a' in dir_list) 
-000071e0: 616e 6420 2827 6227 2069 6e20 6469 725f  and ('b' in dir_
-000071f0: 6c69 7374 2920 616e 6420 2827 6327 206e  list) and ('c' n
-00007200: 6f74 2069 6e20 6469 725f 6c69 7374 2929  ot in dir_list))
-00007210: 0a0a 2020 2020 6465 6620 7465 7374 5f64  ..    def test_d
-00007220: 656c 6574 655f 6279 5f66 696c 7465 7228  elete_by_filter(
-00007230: 7365 6c66 293a 0a20 2020 2020 2020 2074  self):.        t
-00007240: 6573 745f 7369 7a65 203d 2031 300a 2020  est_size = 10.  
-00007250: 2020 2020 2020 7461 626c 6520 3d20 6d61        table = ma
-00007260: 6b65 5f74 6573 745f 7461 626c 6528 7365  ke_test_table(se
-00007270: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
-00007280: 6563 742c 2074 6573 745f 7369 7a65 290a  ect, test_size).
-00007290: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-000072a0: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
-000072b0: 697a 652a 7465 7374 5f73 697a 652c 2074  ize*test_size, t
-000072c0: 6162 6c65 2e64 656c 6574 6528 623d 3529  able.delete(b=5)
-000072d0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-000072e0: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
-000072f0: 7369 7a65 2a74 6573 745f 7369 7a65 2a28  size*test_size*(
-00007300: 7465 7374 5f73 697a 652d 3129 2c20 6c65  test_size-1), le
-00007310: 6e28 7461 626c 6529 290a 2020 2020 2020  n(table)).      
-00007320: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00007330: 616c 2830 2c20 7461 626c 652e 6465 6c65  al(0, table.dele
-00007340: 7465 2862 3d2d 3129 290a 2020 2020 2020  te(b=-1)).      
-00007350: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00007360: 616c 2830 2c20 7461 626c 652e 6465 6c65  al(0, table.dele
-00007370: 7465 2829 290a 0a20 2020 2064 6566 2074  te())..    def t
-00007380: 6573 745f 7265 6d6f 7665 5f6d 616e 7928  est_remove_many(
-00007390: 7365 6c66 293a 0a20 2020 2020 2020 2074  self):.        t
-000073a0: 6573 745f 7369 7a65 203d 2031 300a 2020  est_size = 10.  
-000073b0: 2020 2020 2020 7461 626c 6520 3d20 6d61        table = ma
-000073c0: 6b65 5f74 6573 745f 7461 626c 6528 7365  ke_test_table(se
-000073d0: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
-000073e0: 6563 742c 2074 6573 745f 7369 7a65 290a  ect, test_size).
-000073f0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00007400: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
-00007410: 697a 652a 7465 7374 5f73 697a 652a 7465  ize*test_size*te
-00007420: 7374 5f73 697a 652f 322c 206c 656e 2874  st_size/2, len(t
-00007430: 6162 6c65 2e77 6865 7265 286c 616d 6264  able.where(lambd
-00007440: 6120 743a 2074 2e61 2025 2032 2929 290a  a t: t.a % 2))).
-00007450: 2020 2020 2020 2020 7461 626c 652e 7265          table.re
-00007460: 6d6f 7665 5f6d 616e 7928 7461 626c 652e  move_many(table.
-00007470: 7768 6572 6528 6c61 6d62 6461 2074 3a20  where(lambda t: 
-00007480: 742e 6120 2520 3229 290a 2020 2020 2020  t.a % 2)).      
-00007490: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000074a0: 616c 2874 6573 745f 7369 7a65 2a74 6573  al(test_size*tes
-000074b0: 745f 7369 7a65 2a74 6573 745f 7369 7a65  t_size*test_size
-000074c0: 2f32 2c20 6c65 6e28 7461 626c 6529 290a  /2, len(table)).
-000074d0: 2020 2020 2020 2020 7461 626c 655f 6c65          table_le
-000074e0: 6e20 3d20 6c65 6e28 7461 626c 6529 0a20  n = len(table). 
-000074f0: 2020 2020 2020 2074 6162 6c65 2e72 656d         table.rem
-00007500: 6f76 6528 7461 626c 655b 315d 290a 2020  ove(table[1]).  
-00007510: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00007520: 7445 7175 616c 2874 6162 6c65 5f6c 656e  tEqual(table_len
-00007530: 2d31 2c20 6c65 6e28 7461 626c 6529 290a  -1, len(table)).
-00007540: 0a20 2020 2064 6566 2074 6573 745f 6164  .    def test_ad
-00007550: 645f 6e65 775f 6669 656c 6428 7365 6c66  d_new_field(self
-00007560: 293a 0a20 2020 2020 2020 2074 6573 745f  ):.        test_
-00007570: 7369 7a65 203d 2031 300a 2020 2020 2020  size = 10.      
-00007580: 2020 7461 626c 6520 3d20 6d61 6b65 5f74    table = make_t
-00007590: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
-000075a0: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
-000075b0: 2074 6573 745f 7369 7a65 290a 0a20 2020   test_size)..   
-000075c0: 2020 2020 2023 206f 6e6c 7920 4461 7461       # only Data
-000075d0: 4f62 6a65 6374 7320 6172 6520 6d75 7461  Objects are muta
-000075e0: 626c 6520 696e 2074 6865 7365 2074 6573  ble in these tes
-000075f0: 7473 0a20 2020 2020 2020 2069 6620 6973  ts.        if is
-00007600: 696e 7374 616e 6365 2874 6162 6c65 5b30  instance(table[0
-00007610: 5d2c 206c 742e 4461 7461 4f62 6a65 6374  ], lt.DataObject
-00007620: 293a 0a20 2020 2020 2020 2020 2020 2074  ):.            t
-00007630: 6162 6c65 2e61 6464 5f66 6965 6c64 2827  able.add_field('
-00007640: 6427 2c20 6c61 6d62 6461 2072 6563 3a20  d', lambda rec: 
-00007650: 7265 632e 612b 7265 632e 622b 7265 632e  rec.a+rec.b+rec.
-00007660: 6329 0a0a 2020 2020 2020 2020 2020 2020  c)..            
-00007670: 7461 626c 652e 6372 6561 7465 5f69 6e64  table.create_ind
-00007680: 6578 2827 6427 290a 2020 2020 2020 2020  ex('d').        
-00007690: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-000076a0: 7175 616c 286c 656e 2872 616e 6765 2830  qual(len(range(0
-000076b0: 2c20 3237 2b31 2929 2c20 6c65 6e28 7461  , 27+1)), len(ta
-000076c0: 626c 652e 6279 2e64 2e6b 6579 7328 2929  ble.by.d.keys())
-000076d0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-000076e0: 6164 645f 7477 6f5f 7461 626c 6573 2873  add_two_tables(s
-000076f0: 656c 6629 3a0a 2020 2020 2020 2020 7465  elf):.        te
-00007700: 7374 5f73 697a 6520 3d20 3130 0a20 2020  st_size = 10.   
-00007710: 2020 2020 2074 3120 3d20 6d61 6b65 5f74       t1 = make_t
-00007720: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
-00007730: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
-00007740: 2074 6573 745f 7369 7a65 290a 2020 2020   test_size).    
-00007750: 2020 2020 6d61 6b65 5f72 6563 203d 206c      make_rec = l
-00007760: 616d 6264 6120 612c 622c 633a 2073 656c  ambda a,b,c: sel
-00007770: 662e 6d61 6b65 5f64 6174 615f 6f62 6a65  f.make_data_obje
-00007780: 6374 2861 2b74 6573 745f 7369 7a65 2c20  ct(a+test_size, 
-00007790: 622c 2063 290a 2020 2020 2020 2020 7432  b, c).        t2
-000077a0: 203d 206d 616b 655f 7465 7374 5f74 6162   = make_test_tab
-000077b0: 6c65 286d 616b 655f 7265 632c 2074 6573  le(make_rec, tes
-000077c0: 745f 7369 7a65 290a 0a20 2020 2020 2020  t_size)..       
-000077d0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-000077e0: 6c28 7465 7374 5f73 697a 652a 7465 7374  l(test_size*test
-000077f0: 5f73 697a 652a 7465 7374 5f73 697a 652a  _size*test_size*
-00007800: 322c 206c 656e 2874 312b 7432 2929 0a20  2, len(t1+t2)). 
-00007810: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00007820: 7274 4571 7561 6c28 7465 7374 5f73 697a  rtEqual(test_siz
-00007830: 6520 2a20 7465 7374 5f73 697a 6520 2a20  e * test_size * 
-00007840: 7465 7374 5f73 697a 652c 206c 656e 2874  test_size, len(t
-00007850: 3129 290a 0a20 2020 2020 2020 2074 3120  1))..        t1 
-00007860: 2b3d 2074 320a 2020 2020 2020 2020 7365  += t2.        se
-00007870: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
-00007880: 6573 745f 7369 7a65 202a 2074 6573 745f  est_size * test_
-00007890: 7369 7a65 202a 2074 6573 745f 7369 7a65  size * test_size
-000078a0: 202a 2032 2c20 6c65 6e28 7431 2929 0a0a   * 2, len(t1))..
-000078b0: 2020 2020 2020 2020 6f66 6673 6574 203d          offset =
-000078c0: 2074 6573 745f 7369 7a65 202a 2074 6573   test_size * tes
-000078d0: 745f 7369 7a65 0a20 2020 2020 2020 2074  t_size.        t
-000078e0: 3320 3d20 7431 202b 2028 7365 6c66 2e6d  3 = t1 + (self.m
-000078f0: 616b 655f 6461 7461 5f6f 626a 6563 7428  ake_data_object(
-00007900: 7265 632e 612b 6f66 6673 6574 2c20 7265  rec.a+offset, re
-00007910: 632e 622c 2072 6563 2e63 2920 666f 7220  c.b, rec.c) for 
-00007920: 7265 6320 696e 2074 3229 0a20 2020 2020  rec in t2).     
-00007930: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00007940: 7561 6c28 7465 7374 5f73 697a 6520 2a20  ual(test_size * 
-00007950: 7465 7374 5f73 697a 6520 2a20 7465 7374  test_size * test
-00007960: 5f73 697a 6520 2a20 332c 206c 656e 2874  _size * 3, len(t
-00007970: 3329 290a 0a20 2020 2064 6566 2074 6573  3))..    def tes
-00007980: 745f 7461 626c 655f 696e 666f 2873 656c  t_table_info(sel
-00007990: 6629 3a0a 2020 2020 2020 2020 7465 7374  f):.        test
-000079a0: 5f73 697a 6520 3d20 3130 0a20 2020 2020  _size = 10.     
-000079b0: 2020 2077 6974 6820 7469 6d65 7374 616d     with timestam
-000079c0: 705f 7374 6172 745f 656e 6428 2920 6173  p_start_end() as
-000079d0: 2074 696d 696e 673a 0a20 2020 2020 2020   timing:.       
-000079e0: 2020 2020 2074 3120 3d20 6d61 6b65 5f74       t1 = make_t
-000079f0: 6573 745f 7461 626c 6528 7365 6c66 2e6d  est_table(self.m
-00007a00: 616b 655f 6461 7461 5f6f 626a 6563 742c  ake_data_object,
-00007a10: 2074 6573 745f 7369 7a65 2928 2769 6e66   test_size)('inf
-00007a20: 6f5f 7465 7374 2729 0a0a 2020 2020 2020  o_test')..      
-00007a30: 2020 7431 2e63 7265 6174 655f 696e 6465    t1.create_inde
-00007a40: 7828 2762 2729 0a20 2020 2020 2020 2074  x('b').        t
-00007a50: 315f 696e 666f 203d 2074 312e 696e 666f  1_info = t1.info
-00007a60: 2829 0a20 2020 2020 2020 2023 206d 7573  ().        # mus
-00007a70: 7420 736f 7274 2066 6965 6c64 7320 616e  t sort fields an
-00007a80: 6420 696e 6465 7865 7320 7661 6c75 6573  d indexes values
-00007a90: 2c20 666f 7220 7465 7374 2063 6f6d 7061  , for test compa
-00007aa0: 7269 736f 6e73 0a20 2020 2020 2020 2074  risons.        t
-00007ab0: 315f 696e 666f 5b27 6669 656c 6473 275d  1_info['fields']
-00007ac0: 2e73 6f72 7428 290a 2020 2020 2020 2020  .sort().        
-00007ad0: 7431 5f69 6e66 6f5b 2769 6e64 6578 6573  t1_info['indexes
-00007ae0: 275d 2e73 6f72 7428 290a 2020 2020 2020  '].sort().      
-00007af0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00007b00: 616c 284e 6f6e 652c 2074 315f 696e 666f  al(None, t1_info
-00007b10: 2e70 6f70 2822 6c61 7374 5f69 6d70 6f72  .pop("last_impor
-00007b20: 7422 2929 0a20 2020 2020 2020 2073 656c  t")).        sel
-00007b30: 662e 6173 7365 7274 5472 7565 2874 696d  f.assertTrue(tim
-00007b40: 696e 672e 7374 6172 7420 3c3d 2074 315f  ing.start <= t1_
-00007b50: 696e 666f 2e70 6f70 2822 6372 6561 7465  info.pop("create
-00007b60: 6422 2920 3c3d 2074 696d 696e 672e 656e  d") <= timing.en
-00007b70: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
-00007b80: 6173 7365 7274 5472 7565 2874 696d 696e  assertTrue(timin
-00007b90: 672e 7374 6172 7420 3c3d 2074 315f 696e  g.start <= t1_in
-00007ba0: 666f 2e70 6f70 2822 6d6f 6469 6669 6564  fo.pop("modified
-00007bb0: 2229 203c 3d20 7469 6d69 6e67 2e65 6e64  ") <= timing.end
-00007bc0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00007bd0: 7373 6572 7445 7175 616c 287b 2766 6965  ssertEqual({'fie
-00007be0: 6c64 7327 3a20 5b27 6127 2c20 2762 272c  lds': ['a', 'b',
-00007bf0: 2027 6327 5d2c 0a20 2020 2020 2020 2020   'c'],.         
-00007c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c10: 2027 696e 6465 7865 7327 3a20 5b28 2762   'indexes': [('b
-00007c20: 272c 2046 616c 7365 295d 2c0a 2020 2020  ', False)],.    
-00007c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c40: 2020 2020 2020 276c 656e 273a 2031 3030        'len': 100
-00007c50: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-00007c60: 2020 2020 2020 2020 2020 2020 2027 6e61               'na
-00007c70: 6d65 273a 2027 696e 666f 5f74 6573 7427  me': 'info_test'
-00007c80: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00007c90: 2020 2020 2020 2020 2020 2020 7431 5f69              t1_i
-00007ca0: 6e66 6f2c 2022 696e 7661 6c69 6420 696e  nfo, "invalid in
-00007cb0: 666f 2072 6573 756c 7473 2229 0a0a 0a40  fo results")...@
-00007cc0: 6d61 6b65 5f74 6573 745f 636c 6173 7365  make_test_classe
-00007cd0: 730a 636c 6173 7320 5461 626c 654c 6973  s.class TableLis
-00007ce0: 7454 6573 7473 3a0a 2020 2020 6465 6620  tTests:.    def 
-00007cf0: 5f74 6573 745f 696e 6974 2873 656c 6629  _test_init(self)
-00007d00: 3a0a 2020 2020 2020 2020 7365 6c66 2e74  :.        self.t
-00007d10: 6573 745f 7369 7a65 203d 2033 0a20 2020  est_size = 3.   
-00007d20: 2020 2020 2073 656c 662e 7431 203d 206d       self.t1 = m
-00007d30: 616b 655f 7465 7374 5f74 6162 6c65 2873  ake_test_table(s
-00007d40: 656c 662e 6d61 6b65 5f64 6174 615f 6f62  elf.make_data_ob
-00007d50: 6a65 6374 2c20 7365 6c66 2e74 6573 745f  ject, self.test_
-00007d60: 7369 7a65 290a 2020 2020 2020 2020 7365  size).        se
-00007d70: 6c66 2e74 6573 745f 7265 6320 3d20 7365  lf.test_rec = se
-00007d80: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
-00007d90: 6563 7428 312c 2031 2c20 3129 0a0a 2020  ect(1, 1, 1)..  
-00007da0: 2020 6465 6620 7465 7374 5f63 6f6e 7461    def test_conta
-00007db0: 696e 7328 7365 6c66 293a 0a20 2020 2020  ins(self):.     
-00007dc0: 2020 2073 656c 662e 5f74 6573 745f 696e     self._test_in
-00007dd0: 6974 2829 0a20 2020 2020 2020 2073 656c  it().        sel
-00007de0: 662e 6173 7365 7274 5472 7565 2873 656c  f.assertTrue(sel
-00007df0: 662e 7465 7374 5f72 6563 2069 6e20 7365  f.test_rec in se
-00007e00: 6c66 2e74 312c 2022 6661 696c 6564 2027  lf.t1, "failed '
-00007e10: 696e 2720 2863 6f6e 7461 696e 7329 2074  in' (contains) t
-00007e20: 6573 7422 290a 0a20 2020 2064 6566 2074  est")..    def t
-00007e30: 6573 745f 696e 6465 785f 6669 6e64 2873  est_index_find(s
-00007e40: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-00007e50: 6c66 2e5f 7465 7374 5f69 6e69 7428 290a  lf._test_init().
-00007e60: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00007e70: 6572 7445 7175 616c 2831 332c 2073 656c  ertEqual(13, sel
-00007e80: 662e 7431 2e69 6e64 6578 2873 656c 662e  f.t1.index(self.
-00007e90: 7465 7374 5f72 6563 292c 2022 6661 696c  test_rec), "fail
-00007ea0: 6564 2027 696e 6465 783b 2074 6573 7420  ed 'index; test 
-00007eb0: 2865 7869 7374 7329 2229 0a20 2020 2020  (exists)").     
-00007ec0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00007ed0: 2873 656c 662e 7465 7374 5f72 6563 2c20  (self.test_rec, 
-00007ee0: 5369 6d70 6c65 4e61 6d65 7370 6163 6529  SimpleNamespace)
-00007ef0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00007f00: 6c66 2e61 7373 6572 7445 7175 616c 2831  lf.assertEqual(1
-00007f10: 332c 2073 656c 662e 7431 2e69 6e64 6578  3, self.t1.index
-00007f20: 2876 6172 7328 7365 6c66 2e74 6573 745f  (vars(self.test_
-00007f30: 7265 6329 292c 2022 6661 696c 6564 2027  rec)), "failed '
-00007f40: 696e 6465 783b 2074 6573 7420 2865 7869  index; test (exi
-00007f50: 7374 7329 2229 0a0a 2020 2020 2020 2020  sts)")..        
-00007f60: 6e6f 5f73 7563 685f 7265 6320 3d20 7365  no_such_rec = se
-00007f70: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
-00007f80: 6563 7428 7365 6c66 2e74 6573 745f 7369  ect(self.test_si
-00007f90: 7a65 2b31 2c20 7365 6c66 2e74 6573 745f  ze+1, self.test_
-00007fa0: 7369 7a65 2b31 2c20 7365 6c66 2e74 6573  size+1, self.tes
-00007fb0: 745f 7369 7a65 2b31 290a 2020 2020 2020  t_size+1).      
-00007fc0: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
-00007fd0: 7274 5261 6973 6573 2856 616c 7565 4572  rtRaises(ValueEr
-00007fe0: 726f 722c 206d 7367 3d22 6661 696c 6564  ror, msg="failed
-00007ff0: 2027 696e 6465 7827 2074 6573 7420 286e   'index' test (n
-00008000: 6f74 2065 7869 7374 7329 2229 3a0a 2020  ot exists)"):.  
-00008010: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00008020: 312e 696e 6465 7828 6e6f 5f73 7563 685f  1.index(no_such_
-00008030: 7265 6329 0a0a 2020 2020 6465 6620 7465  rec)..    def te
-00008040: 7374 5f72 656d 6f76 6528 7365 6c66 293a  st_remove(self):
-00008050: 0a20 2020 2020 2020 2073 656c 662e 5f74  .        self._t
-00008060: 6573 745f 696e 6974 2829 0a20 2020 2020  est_init().     
-00008070: 2020 2072 6563 203d 2073 656c 662e 6d61     rec = self.ma
-00008080: 6b65 5f64 6174 615f 6f62 6a65 6374 2831  ke_data_object(1
-00008090: 2c20 312c 2031 290a 2020 2020 2020 2020  , 1, 1).        
-000080a0: 7072 6576 5f6c 656e 203d 206c 656e 2873  prev_len = len(s
-000080b0: 656c 662e 7431 290a 2020 2020 2020 2020  elf.t1).        
-000080c0: 7365 6c66 2e74 312e 7265 6d6f 7665 2872  self.t1.remove(r
-000080d0: 6563 290a 2020 2020 2020 2020 7365 6c66  ec).        self
-000080e0: 2e61 7373 6572 7446 616c 7365 2872 6563  .assertFalse(rec
-000080f0: 2069 6e20 7365 6c66 2e74 312c 2022 6661   in self.t1, "fa
-00008100: 696c 6564 2074 6f20 7265 6d6f 7665 2072  iled to remove r
-00008110: 6563 6f72 6420 6672 6f6d 2074 6162 6c65  ecord from table
-00008120: 2028 636f 6e74 6169 6e73 2922 290a 2020   (contains)").  
-00008130: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00008140: 7445 7175 616c 2870 7265 765f 6c65 6e2d  tEqual(prev_len-
-00008150: 312c 206c 656e 2873 656c 662e 7431 292c  1, len(self.t1),
-00008160: 2022 6661 696c 6564 2074 6f20 7265 6d6f   "failed to remo
-00008170: 7665 2072 6563 6f72 6420 6672 6f6d 2074  ve record from t
-00008180: 6162 6c65 2028 6c65 6e29 2229 0a0a 2020  able (len)")..  
-00008190: 2020 2020 2020 6e6f 5f73 7563 685f 7265        no_such_re
-000081a0: 6320 3d20 7365 6c66 2e6d 616b 655f 6461  c = self.make_da
-000081b0: 7461 5f6f 626a 6563 7428 7365 6c66 2e74  ta_object(self.t
-000081c0: 6573 745f 7369 7a65 2b31 2c20 7365 6c66  est_size+1, self
-000081d0: 2e74 6573 745f 7369 7a65 2b31 2c20 7365  .test_size+1, se
-000081e0: 6c66 2e74 6573 745f 7369 7a65 2b31 290a  lf.test_size+1).
-000081f0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00008200: 6572 7446 616c 7365 286e 6f5f 7375 6368  ertFalse(no_such
-00008210: 5f72 6563 2069 6e20 7365 6c66 2e74 312c  _rec in self.t1,
-00008220: 2022 6661 696c 6564 2074 6f20 6372 6561   "failed to crea
-00008230: 7465 206e 6f6e 2d65 7869 7374 656e 7420  te non-existent 
-00008240: 7265 636f 7264 2066 726f 6d20 7461 626c  record from tabl
-00008250: 6522 290a 2020 2020 2020 2020 7365 6c66  e").        self
-00008260: 2e74 312e 7265 6d6f 7665 286e 6f5f 7375  .t1.remove(no_su
-00008270: 6368 5f72 6563 290a 2020 2020 2020 2020  ch_rec).        
-00008280: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00008290: 2870 7265 765f 6c65 6e2d 312c 206c 656e  (prev_len-1, len
-000082a0: 2873 656c 662e 7431 292c 2022 6661 696c  (self.t1), "fail
-000082b0: 6564 2072 656d 6f76 696e 6720 6e6f 6e2d  ed removing non-
-000082c0: 6578 6973 7465 6e74 2072 6563 6f72 6420  existent record 
-000082d0: 6672 6f6d 2074 6162 6c65 2028 6c65 6e29  from table (len)
-000082e0: 2229 0a0a 2020 2020 2020 2020 6966 2069  ")..        if i
-000082f0: 7369 6e73 7461 6e63 6528 7365 6c66 2e74  sinstance(self.t
-00008300: 6573 745f 7265 632c 2053 696d 706c 654e  est_rec, SimpleN
-00008310: 616d 6573 7061 6365 293a 0a20 2020 2020  amespace):.     
-00008320: 2020 2020 2020 2073 656c 662e 7431 2e72         self.t1.r
-00008330: 656d 6f76 6528 7661 7273 2873 656c 662e  emove(vars(self.
-00008340: 7465 7374 5f72 6563 2929 0a20 2020 2020  test_rec)).     
-00008350: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00008360: 7274 4571 7561 6c28 7072 6576 5f6c 656e  rtEqual(prev_len
-00008370: 2d31 2c20 6c65 6e28 7365 6c66 2e74 3129  -1, len(self.t1)
-00008380: 2c20 2266 6169 6c65 6420 746f 2072 656d  , "failed to rem
-00008390: 6f76 6520 7265 636f 7264 2061 7320 6469  ove record as di
-000083a0: 6374 2066 726f 6d20 7461 626c 6520 286c  ct from table (l
-000083b0: 656e 2922 290a 0a20 2020 2064 6566 2074  en)")..    def t
-000083c0: 6573 745f 696e 6465 785f 6163 6365 7373  est_index_access
-000083d0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000083e0: 7365 6c66 2e5f 7465 7374 5f69 6e69 7428  self._test_init(
-000083f0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00008400: 7373 6572 7445 7175 616c 2873 656c 662e  ssertEqual(self.
-00008410: 7465 7374 5f72 6563 2c20 7365 6c66 2e74  test_rec, self.t
-00008420: 315b 3133 5d2c 2022 6661 696c 6564 2069  1[13], "failed i
-00008430: 6e64 6578 2061 6363 6573 7320 7465 7374  ndex access test
-00008440: 2229 0a0a 2020 2020 6465 6620 7465 7374  ")..    def test
-00008450: 5f63 6f75 6e74 2873 656c 6629 3a0a 2020  _count(self):.  
-00008460: 2020 2020 2020 7365 6c66 2e5f 7465 7374        self._test
-00008470: 5f69 6e69 7428 290a 2020 2020 2020 2020  _init().        
-00008480: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-00008490: 7365 6c66 2e74 312e 636f 756e 7428 7365  self.t1.count(se
-000084a0: 6c66 2e74 6573 745f 7265 6329 203d 3d20  lf.test_rec) == 
-000084b0: 312c 2022 6661 696c 6564 2063 6f75 6e74  1, "failed count
-000084c0: 2074 6573 7422 290a 2020 2020 2020 2020   test").        
-000084d0: 6966 2069 7369 6e73 7461 6e63 6528 7365  if isinstance(se
-000084e0: 6c66 2e74 6573 745f 7265 632c 2053 696d  lf.test_rec, Sim
-000084f0: 706c 654e 616d 6573 7061 6365 293a 0a20  pleNamespace):. 
-00008500: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008510: 6173 7365 7274 5472 7565 2873 656c 662e  assertTrue(self.
-00008520: 7431 2e63 6f75 6e74 2876 6172 7328 7365  t1.count(vars(se
-00008530: 6c66 2e74 6573 745f 7265 6329 2920 3d3d  lf.test_rec)) ==
-00008540: 2031 2c20 2266 6169 6c65 6420 636f 756e   1, "failed coun
-00008550: 7420 7465 7374 2229 0a0a 2020 2020 6465  t test")..    de
-00008560: 6620 7465 7374 5f64 656c 2873 656c 6629  f test_del(self)
-00008570: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-00008580: 7465 7374 5f69 6e69 7428 290a 2020 2020  test_init().    
-00008590: 2020 2020 6265 666f 7265 5f64 656c 5f6c      before_del_l
-000085a0: 656e 203d 206c 656e 2873 656c 662e 7431  en = len(self.t1
-000085b0: 290a 2020 2020 2020 2020 6465 6c20 7365  ).        del se
-000085c0: 6c66 2e74 315b 3133 5d0a 2020 2020 2020  lf.t1[13].      
-000085d0: 2020 7365 6c66 2e61 7373 6572 7446 616c    self.assertFal
-000085e0: 7365 2873 656c 662e 7465 7374 5f72 6563  se(self.test_rec
-000085f0: 2069 6e20 7365 6c66 2e74 312c 2022 6661   in self.t1, "fa
-00008600: 696c 6564 2064 656c 2074 6573 7422 290a  iled del test").
-00008610: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00008620: 6572 7445 7175 616c 2862 6566 6f72 655f  ertEqual(before_
-00008630: 6465 6c5f 6c65 6e20 2d20 312c 206c 656e  del_len - 1, len
-00008640: 2873 656c 662e 7431 2929 0a0a 2020 2020  (self.t1))..    
-00008650: 6465 6620 7465 7374 5f70 6f70 2873 656c  def test_pop(sel
-00008660: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00008670: 2e5f 7465 7374 5f69 6e69 7428 290a 2020  ._test_init().  
-00008680: 2020 2020 2020 6265 666f 7265 5f70 6f70        before_pop
-00008690: 5f6c 656e 203d 206c 656e 2873 656c 662e  _len = len(self.
-000086a0: 7431 290a 2020 2020 2020 2020 6f62 6a20  t1).        obj 
-000086b0: 3d20 7365 6c66 2e74 312e 706f 7028 3133  = self.t1.pop(13
-000086c0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-000086d0: 7373 6572 7446 616c 7365 286f 626a 2069  ssertFalse(obj i
-000086e0: 6e20 7365 6c66 2e74 3129 0a20 2020 2020  n self.t1).     
-000086f0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00008700: 7561 6c28 7365 6c66 2e74 6573 745f 7265  ual(self.test_re
-00008710: 632c 206f 626a 290a 2020 2020 2020 2020  c, obj).        
-00008720: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00008730: 2862 6566 6f72 655f 706f 705f 6c65 6e20  (before_pop_len 
-00008740: 2d20 312c 206c 656e 2873 656c 662e 7431  - 1, len(self.t1
-00008750: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
-00008760: 5f70 6f70 5f6c 6173 7428 7365 6c66 293a  _pop_last(self):
-00008770: 0a20 2020 2020 2020 2073 656c 662e 5f74  .        self._t
-00008780: 6573 745f 696e 6974 2829 0a20 2020 2020  est_init().     
-00008790: 2020 2062 6566 6f72 655f 706f 705f 6c65     before_pop_le
-000087a0: 6e20 3d20 6c65 6e28 7365 6c66 2e74 3129  n = len(self.t1)
-000087b0: 0a20 2020 2020 2020 2065 7870 6563 7465  .        expecte
-000087c0: 645f 706f 7020 3d20 636f 7079 2e63 6f70  d_pop = copy.cop
-000087d0: 7928 7365 6c66 2e74 315b 2d31 5d29 0a20  y(self.t1[-1]). 
-000087e0: 2020 2020 2020 206f 626a 203d 2073 656c         obj = sel
-000087f0: 662e 7431 2e70 6f70 2829 0a20 2020 2020  f.t1.pop().     
-00008800: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00008810: 7561 6c28 6578 7065 6374 6564 5f70 6f70  ual(expected_pop
-00008820: 2c20 6f62 6a29 0a20 2020 2020 2020 2073  , obj).        s
-00008830: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00008840: 6265 666f 7265 5f70 6f70 5f6c 656e 202d  before_pop_len -
-00008850: 2031 2c20 6c65 6e28 7365 6c66 2e74 3129   1, len(self.t1)
-00008860: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00008870: 7265 7665 7273 6564 2873 656c 6629 3a0a  reversed(self):.
-00008880: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
-00008890: 7374 5f69 6e69 7428 290a 2020 2020 2020  st_init().      
-000088a0: 2020 6c61 7374 5f72 6563 203d 206e 6578    last_rec = nex
-000088b0: 7428 7265 7665 7273 6564 2873 656c 662e  t(reversed(self.
-000088c0: 7431 2929 0a20 2020 2020 2020 2073 656c  t1)).        sel
-000088d0: 662e 6173 7365 7274 4571 7561 6c28 7365  f.assertEqual(se
-000088e0: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
-000088f0: 6563 7428 322c 2032 2c20 3229 2c20 6c61  ect(2, 2, 2), la
-00008900: 7374 5f72 6563 2c20 2266 6169 6c65 6420  st_rec, "failed 
-00008910: 7265 7665 7273 6564 2074 6573 7422 290a  reversed test").
-00008920: 0a20 2020 2064 6566 2074 6573 745f 6974  .    def test_it
-00008930: 6572 2873 656c 6629 3a0a 2020 2020 2020  er(self):.      
-00008940: 2020 7365 6c66 2e5f 7465 7374 5f69 6e69    self._test_ini
-00008950: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
-00008960: 2e61 7373 6572 7454 7275 6528 7365 6c66  .assertTrue(self
-00008970: 2e74 6573 745f 7265 6320 696e 2073 656c  .test_rec in sel
-00008980: 662e 7431 2c20 2266 6169 6c65 6420 2769  f.t1, "failed 'i
-00008990: 6e27 2028 636f 6e74 6169 6e73 2920 7465  n' (contains) te
-000089a0: 7374 2229 0a0a 2020 2020 6465 6620 7465  st")..    def te
-000089b0: 7374 5f68 6561 645f 616e 645f 7461 696c  st_head_and_tail
-000089c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000089d0: 7365 6c66 2e5f 7465 7374 5f69 6e69 7428  self._test_init(
-000089e0: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
-000089f0: 312e 6372 6561 7465 5f69 6e64 6578 2822  1.create_index("
-00008a00: 6122 290a 2020 2020 2020 2020 7365 6c66  a").        self
-00008a10: 2e74 312e 6372 6561 7465 5f69 6e64 6578  .t1.create_index
-00008a20: 2822 6322 290a 2020 2020 2020 2020 7365  ("c").        se
-00008a30: 6c66 2e61 7373 6572 7445 7175 616c 287b  lf.assertEqual({
-00008a40: 2261 222c 2022 6322 7d2c 2073 6574 2873  "a", "c"}, set(s
-00008a50: 656c 662e 7431 2e5f 696e 6465 7865 732e  elf.t1._indexes.
-00008a60: 6b65 7973 2829 292c 2022 6661 696c 6564  keys()), "failed
-00008a70: 2074 6f20 6372 6561 7465 2069 6e64 6578   to create index
-00008a80: 6573 2229 0a0a 2020 2020 2020 2020 7365  es")..        se
-00008a90: 6c66 2e61 7373 6572 7445 7175 616c 2873  lf.assertEqual(s
-00008aa0: 6574 2873 656c 662e 7431 2e5f 696e 6465  et(self.t1._inde
-00008ab0: 7865 732e 6b65 7973 2829 292c 0a20 2020  xes.keys()),.   
-00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ad0: 2020 2020 2020 7365 7428 7365 6c66 2e74        set(self.t
-00008ae0: 312e 6865 6164 2829 2e5f 696e 6465 7865  1.head()._indexe
-00008af0: 732e 6b65 7973 2829 292c 0a20 2020 2020  s.keys()),.     
-00008b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b10: 2020 2020 2266 6169 6c65 6420 746f 2063      "failed to c
-00008b20: 6f70 7920 696e 6465 7865 7320 746f 2068  opy indexes to h
-00008b30: 6561 6428 2922 290a 2020 2020 2020 2020  ead()").        
-00008b40: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00008b50: 2873 6574 2873 656c 662e 7431 2e5f 696e  (set(self.t1._in
-00008b60: 6465 7865 732e 6b65 7973 2829 292c 0a20  dexes.keys()),. 
-00008b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b80: 2020 2020 2020 2020 7365 7428 7365 6c66          set(self
-00008b90: 2e74 312e 7461 696c 2829 2e5f 696e 6465  .t1.tail()._inde
-00008ba0: 7865 732e 6b65 7973 2829 292c 0a20 2020  xes.keys()),.   
-00008bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bc0: 2020 2020 2020 2266 6169 6c65 6420 746f        "failed to
-00008bd0: 2063 6f70 7920 696e 6465 7865 7320 746f   copy indexes to
-00008be0: 2074 6169 6c28 2922 290a 0a20 2020 2064   tail()")..    d
-00008bf0: 6566 2074 6573 745f 756e 6971 7565 2873  ef test_unique(s
-00008c00: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-00008c10: 6c66 2e5f 7465 7374 5f69 6e69 7428 290a  lf._test_init().
-00008c20: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00008c30: 6572 7445 7175 616c 285b 302c 2031 2c20  ertEqual([0, 1, 
-00008c40: 325d 2c20 736f 7274 6564 285b 726f 772e  2], sorted([row.
-00008c50: 6120 666f 7220 726f 7720 696e 2073 656c  a for row in sel
-00008c60: 662e 7431 2e75 6e69 7175 6528 2761 2729  f.t1.unique('a')
-00008c70: 5d29 2c20 2266 6169 6c65 6420 6361 6c6c  ]), "failed call
-00008c80: 2074 6f20 756e 6971 7565 2229 0a0a 2020   to unique")..  
-00008c90: 2020 6465 6620 7465 7374 5f61 6c6c 5f61    def test_all_a
-00008ca0: 6363 6573 736f 7228 7365 6c66 293a 0a20  ccessor(self):. 
-00008cb0: 2020 2020 2020 2073 656c 662e 5f74 6573         self._tes
-00008cc0: 745f 696e 6974 2829 0a20 2020 2020 2020  t_init().       
-00008cd0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00008ce0: 6c28 7375 6d28 285b 695d 2a73 656c 662e  l(sum(([i]*self.
-00008cf0: 7465 7374 5f73 697a 652a 2a32 2066 6f72  test_size**2 for
-00008d00: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
-00008d10: 2e74 6573 745f 7369 7a65 2929 2c20 5b5d  .test_size)), []
-00008d20: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00008d30: 2020 2020 2020 2020 2020 2020 6c69 7374              list
-00008d40: 2873 656c 662e 7431 2e61 6c6c 2e61 292c  (self.t1.all.a),
-00008d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008d60: 2020 2020 2020 2020 2020 2266 6169 6c65            "faile
-00008d70: 6420 746f 2073 7563 6365 7373 6675 6c6c  d to successfull
-00008d80: 7920 6765 7420 616c 6c20 7661 6c75 6573  y get all values
-00008d90: 2069 6e20 2761 2722 290a 0a20 2020 2020   in 'a'")..     
-00008da0: 2020 2061 6c6c 5f61 7320 3d20 7365 6c66     all_as = self
-00008db0: 2e74 312e 616c 6c2e 610a 2020 2020 2020  .t1.all.a.      
-00008dc0: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
-00008dd0: 6528 616c 6c5f 6173 2069 7320 6974 6572  e(all_as is iter
-00008de0: 2861 6c6c 5f61 7329 2c20 2261 6c6c 2069  (all_as), "all i
-00008df0: 7465 7261 746f 7220 6661 696c 7320 746f  terator fails to
-00008e00: 2069 6465 6e74 6966 7920 6173 2069 7465   identify as ite
-00008e10: 7228 7365 6c66 2922 290a 0a20 2020 2064  r(self)")..    d
-00008e20: 6566 2074 6573 745f 666f 726d 6174 2873  ef test_format(s
-00008e30: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-00008e40: 6c66 2e5f 7465 7374 5f69 6e69 7428 290a  lf._test_init().
-00008e50: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00008e60: 6572 7445 7175 616c 285b 2730 3020 3020  ertEqual(['00 0 
-00008e70: 3027 2c20 2730 3020 3020 3127 2c20 2730  0', '00 0 1', '0
-00008e80: 3020 3020 3227 5d2c 0a20 2020 2020 2020  0 0 2'],.       
-00008e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ea0: 2020 6c69 7374 2873 656c 662e 7431 2e66    list(self.t1.f
-00008eb0: 6f72 6d61 7428 227b 613a 3032 647d 207b  ormat("{a:02d} {
-00008ec0: 627d 207b 637d 2229 295b 3a33 5d2c 0a20  b} {c}"))[:3],. 
-00008ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ee0: 2020 2020 2020 2020 2266 6169 6c65 6420          "failed 
-00008ef0: 746f 2063 7265 6174 6520 666f 726d 6174  to create format
-00008f00: 7465 6420 726f 7773 2229 0a0a 2020 2020  ted rows")..    
-00008f10: 6465 6620 7465 7374 5f61 735f 6874 6d6c  def test_as_html
-00008f20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00008f30: 7365 6c66 2e5f 7465 7374 5f69 6e69 7428  self._test_init(
-00008f40: 290a 2020 2020 2020 2020 6874 6d6c 5f6f  ).        html_o
-00008f50: 7574 7075 7420 3d20 7365 6c66 2e74 315b  utput = self.t1[
-00008f60: 3a31 305d 2e61 735f 6874 6d6c 2866 6965  :10].as_html(fie
-00008f70: 6c64 733d 2261 2062 2063 2229 0a20 2020  lds="a b c").   
-00008f80: 2020 2020 2070 7269 6e74 2868 746d 6c5f       print(html_
-00008f90: 6f75 7470 7574 290a 2020 2020 2020 2020  output).        
-00008fa0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-00008fb0: 223c 7468 6561 643e 2220 696e 2068 746d  "<thead>" in htm
-00008fc0: 6c5f 6f75 7470 7574 2061 6e64 2022 3c74  l_output and "<t
-00008fd0: 626f 6479 3e22 2069 6e20 6874 6d6c 5f6f  body>" in html_o
-00008fe0: 7574 7075 742c 0a20 2020 2020 2020 2020  utput,.         
-00008ff0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00009000: 6173 5f68 746d 6c20 646f 6573 206e 6f74  as_html does not
-00009010: 2069 6e63 6c75 6465 2074 6865 6164 2061   include thead a
-00009020: 6e64 2074 626f 6479 2074 6167 7322 290a  nd tbody tags").
-00009030: 0a20 2020 2020 2020 2068 746d 6c5f 6c69  .        html_li
-00009040: 6e65 7320 3d20 6874 6d6c 5f6f 7574 7075  nes = html_outpu
-00009050: 742e 7370 6c69 746c 696e 6573 2829 0a20  t.splitlines(). 
-00009060: 2020 2020 2020 2068 6472 5f6c 696e 6520         hdr_line 
-00009070: 3d20 6e65 7874 2868 2066 6f72 2068 2069  = next(h for h i
-00009080: 6e20 6874 6d6c 5f6c 696e 6573 2069 6620  n html_lines if 
-00009090: 2263 656e 7465 7222 2069 6e20 6829 0a20  "center" in h). 
-000090a0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000090b0: 7274 4571 7561 6c28 273c 7472 3e3c 7468  rtEqual('<tr><th
-000090c0: 3e3c 6469 7620 616c 6967 6e3d 2263 656e  ><div align="cen
-000090d0: 7465 7222 3e61 3c2f 6469 763e 3c2f 7468  ter">a</div></th
-000090e0: 3e27 0a20 2020 2020 2020 2020 2020 2020  >'.             
-000090f0: 2020 2020 2020 2020 2020 2020 273c 7468              '<th
-00009100: 3e3c 6469 7620 616c 6967 6e3d 2263 656e  ><div align="cen
-00009110: 7465 7222 3e62 3c2f 6469 763e 3c2f 7468  ter">b</div></th
-00009120: 3e27 0a20 2020 2020 2020 2020 2020 2020  >'.             
-00009130: 2020 2020 2020 2020 2020 2020 273c 7468              '<th
-00009140: 3e3c 6469 7620 616c 6967 6e3d 2263 656e  ><div align="cen
-00009150: 7465 7222 3e63 3c2f 6469 763e 3c2f 7468  ter">c</div></th
-00009160: 3e3c 2f74 723e 272c 0a20 2020 2020 2020  ></tr>',.       
-00009170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009180: 2020 6864 725f 6c69 6e65 2c0a 2020 2020    hdr_line,.    
-00009190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091a0: 2020 2020 2022 6661 696c 6564 2061 735f       "failed as_
-000091b0: 6874 6d6c 2077 6974 6820 616c 6c20 6669  html with all fi
-000091c0: 656c 6473 2229 0a0a 2020 2020 2020 2020  elds")..        
-000091d0: 6874 6d6c 5f6f 7574 7075 7420 3d20 7365  html_output = se
-000091e0: 6c66 2e74 315b 3a31 305d 2e61 735f 6874  lf.t1[:10].as_ht
-000091f0: 6d6c 2866 6965 6c64 733d 2261 202d 6220  ml(fields="a -b 
-00009200: 6322 290a 2020 2020 2020 2020 7072 696e  c").        prin
-00009210: 7428 6874 6d6c 5f6f 7574 7075 7429 0a20  t(html_output). 
-00009220: 2020 2020 2020 2068 746d 6c5f 6c69 6e65         html_line
-00009230: 7320 3d20 6874 6d6c 5f6f 7574 7075 742e  s = html_output.
-00009240: 7370 6c69 746c 696e 6573 2829 0a20 2020  splitlines().   
-00009250: 2020 2020 2068 6472 5f6c 696e 6520 3d20       hdr_line = 
-00009260: 6e65 7874 2868 2066 6f72 2068 2069 6e20  next(h for h in 
-00009270: 6874 6d6c 5f6c 696e 6573 2069 6620 2263  html_lines if "c
-00009280: 656e 7465 7222 2069 6e20 6829 0a20 2020  enter" in h).   
-00009290: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000092a0: 4571 7561 6c28 273c 7472 3e3c 7468 3e3c  Equal('<tr><th><
-000092b0: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
-000092c0: 7222 3e61 3c2f 6469 763e 3c2f 7468 3e27  r">a</div></th>'
-000092d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000092e0: 2020 2020 2020 2020 2020 273c 7468 3e3c            '<th><
-000092f0: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
-00009300: 7222 3e63 3c2f 6469 763e 3c2f 7468 3e3c  r">c</div></th><
-00009310: 2f74 723e 272c 0a20 2020 2020 2020 2020  /tr>',.         
-00009320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009330: 6864 725f 6c69 6e65 2c0a 2020 2020 2020  hdr_line,.      
-00009340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009350: 2020 2022 6661 696c 6564 2061 735f 6874     "failed as_ht
-00009360: 6d6c 2077 6974 6820 6e65 6761 7465 6420  ml with negated 
-00009370: 6669 656c 6422 290a 0a20 2020 2020 2020  field")..       
-00009380: 2068 746d 6c5f 6f75 7470 7574 203d 2073   html_output = s
-00009390: 656c 662e 7431 5b3a 3130 5d2e 6173 5f68  elf.t1[:10].as_h
-000093a0: 746d 6c28 6669 656c 6473 3d22 6120 6220  tml(fields="a b 
-000093b0: 6322 2c20 666f 726d 6174 733d 7b22 6222  c", formats={"b"
-000093c0: 3a20 227b 3a30 3364 7d22 7d29 0a20 2020  : "{:03d}"}).   
-000093d0: 2020 2020 2070 7269 6e74 2868 746d 6c5f       print(html_
-000093e0: 6f75 7470 7574 290a 2020 2020 2020 2020  output).        
-000093f0: 6874 6d6c 5f6c 696e 6573 203d 2068 746d  html_lines = htm
-00009400: 6c5f 6f75 7470 7574 2e73 706c 6974 6c69  l_output.splitli
-00009410: 6e65 7328 290a 2020 2020 2020 2020 6461  nes().        da
-00009420: 7461 5f6c 696e 6520 3d20 6e65 7874 2868  ta_line = next(h
-00009430: 2066 6f72 2068 2069 6e20 6874 6d6c 5f6c   for h in html_l
-00009440: 696e 6573 2069 6620 223c 7464 3e22 2069  ines if "<td>" i
-00009450: 6e20 6829 0a20 2020 2020 2020 2073 656c  n h).        sel
-00009460: 662e 6173 7365 7274 4571 7561 6c28 273c  f.assertEqual('<
-00009470: 7462 6f64 793e 3c74 723e 3c74 643e 3c64  tbody><tr><td><d
-00009480: 6976 2061 6c69 676e 3d22 7269 6768 7422  iv align="right"
-00009490: 3e30 3c2f 6469 763e 3c2f 7464 3e27 0a20  >0</div></td>'. 
-000094a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094b0: 2020 2020 2020 2020 273c 7464 3e3c 6469          '<td><di
-000094c0: 7620 616c 6967 6e3d 2272 6967 6874 223e  v align="right">
-000094d0: 3030 303c 2f64 6976 3e3c 2f74 643e 270a  000</div></td>'.
-000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094f0: 2020 2020 2020 2020 2027 3c74 643e 3c64           '<td><d
-00009500: 6976 2061 6c69 676e 3d22 7269 6768 7422  iv align="right"
-00009510: 3e30 3c2f 6469 763e 3c2f 7464 3e3c 2f74  >0</div></td></t
-00009520: 723e 272c 0a20 2020 2020 2020 2020 2020  r>',.           
-00009530: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00009540: 7461 5f6c 696e 652c 0a20 2020 2020 2020  ta_line,.       
-00009550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009560: 2020 2266 6169 6c65 6420 6173 5f68 746d    "failed as_htm
-00009570: 6c20 7769 7468 206e 616d 6564 2066 6965  l with named fie
-00009580: 6c64 2066 6f72 6d61 7420 666f 7220 7370  ld format for sp
-00009590: 6563 6966 6963 2066 6965 6c64 2229 0a0a  ecific field")..
-000095a0: 2020 2020 2020 2020 6874 6d6c 5f6f 7574          html_out
-000095b0: 7075 7420 3d20 7365 6c66 2e74 315b 3a31  put = self.t1[:1
-000095c0: 305d 2e61 735f 6874 6d6c 2866 6965 6c64  0].as_html(field
-000095d0: 733d 2261 2062 2063 222c 2066 6f72 6d61  s="a b c", forma
-000095e0: 7473 3d7b 696e 743a 2022 7b3a 3033 647d  ts={int: "{:03d}
-000095f0: 227d 290a 2020 2020 2020 2020 7072 696e  "}).        prin
-00009600: 7428 6874 6d6c 5f6f 7574 7075 7429 0a20  t(html_output). 
-00009610: 2020 2020 2020 2068 746d 6c5f 6c69 6e65         html_line
-00009620: 7320 3d20 6874 6d6c 5f6f 7574 7075 742e  s = html_output.
-00009630: 7370 6c69 746c 696e 6573 2829 0a20 2020  splitlines().   
-00009640: 2020 2020 2064 6174 615f 6c69 6e65 203d       data_line =
-00009650: 206e 6578 7428 6820 666f 7220 6820 696e   next(h for h in
-00009660: 2068 746d 6c5f 6c69 6e65 7320 6966 2022   html_lines if "
-00009670: 3c74 643e 2220 696e 2068 290a 2020 2020  <td>" in h).    
-00009680: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00009690: 7175 616c 2827 3c74 626f 6479 3e3c 7472  qual('<tbody><tr
-000096a0: 3e3c 7464 3e3c 6469 7620 616c 6967 6e3d  ><td><div align=
-000096b0: 2272 6967 6874 223e 3030 303c 2f64 6976  "right">000</div
-000096c0: 3e3c 2f74 643e 270a 2020 2020 2020 2020  ></td>'.        
-000096d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096e0: 2027 3c74 643e 3c64 6976 2061 6c69 676e   '<td><div align
-000096f0: 3d22 7269 6768 7422 3e30 3030 3c2f 6469  ="right">000</di
-00009700: 763e 3c2f 7464 3e27 0a20 2020 2020 2020  v></td>'.       
-00009710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009720: 2020 273c 7464 3e3c 6469 7620 616c 6967    '<td><div alig
-00009730: 6e3d 2272 6967 6874 223e 3030 303c 2f64  n="right">000</d
-00009740: 6976 3e3c 2f74 643e 3c2f 7472 3e27 2c0a  iv></td></tr>',.
-00009750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009760: 2020 2020 2020 2020 2064 6174 615f 6c69           data_li
-00009770: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00009780: 2020 2020 2020 2020 2020 2020 2022 6661               "fa
-00009790: 696c 6564 2061 735f 6874 6d6c 2077 6974  iled as_html wit
-000097a0: 6820 6461 7461 2074 7970 6520 666f 726d  h data type form
-000097b0: 6174 2066 6f72 2061 6c6c 2066 6965 6c64  at for all field
-000097c0: 7322 290a 0a20 2020 2020 2020 2068 746d  s")..        htm
-000097d0: 6c5f 6f75 7470 7574 203d 2073 656c 662e  l_output = self.
-000097e0: 7431 5b3a 3130 5d2e 6173 5f68 746d 6c28  t1[:10].as_html(
-000097f0: 6669 656c 6473 3d22 6120 6220 6322 2c20  fields="a b c", 
-00009800: 666f 726d 6174 733d 7b69 6e74 3a20 227b  formats={int: "{
-00009810: 3a30 3364 7d22 7d2c 2067 726f 7570 6279  :03d}"}, groupby
-00009820: 3d22 6122 290a 2020 2020 2020 2020 7072  ="a").        pr
-00009830: 696e 7428 6874 6d6c 5f6f 7574 7075 7429  int(html_output)
-00009840: 0a20 2020 2020 2020 2068 746d 6c5f 6c69  .        html_li
-00009850: 6e65 7320 3d20 6874 6d6c 5f6f 7574 7075  nes = html_outpu
-00009860: 742e 7370 6c69 746c 696e 6573 2829 0a20  t.splitlines(). 
-00009870: 2020 2020 2020 2064 6174 615f 6c69 6e65         data_line
-00009880: 203d 206e 6578 7428 6820 666f 7220 6820   = next(h for h 
-00009890: 696e 2068 746d 6c5f 6c69 6e65 7320 6966  in html_lines if
-000098a0: 2022 3c74 643e 2220 696e 2068 290a 2020   "<td>" in h).  
-000098b0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-000098c0: 7445 7175 616c 2827 3c74 626f 6479 3e3c  tEqual('<tbody><
-000098d0: 7472 3e3c 7464 3e3c 6469 7620 616c 6967  tr><td><div alig
-000098e0: 6e3d 2272 6967 6874 223e 3030 303c 2f64  n="right">000</d
-000098f0: 6976 3e3c 2f74 643e 270a 2020 2020 2020  iv></td>'.      
+000070a0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
+000070b0: 6173 7365 7274 4571 7561 6c28 3331 2c20  assertEqual(31, 
+000070c0: 7375 6d28 6669 7273 745f 7174 725f 7361  sum(first_qtr_sa
+000070d0: 6c65 732e 616c 6c2e 7174 7929 290a 0a20  les.all.qty)).. 
+000070e0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+000070f0: 7274 4571 7561 6c28 3331 2c20 7375 6d28  rtEqual(31, sum(
+00007100: 7361 6c65 732e 6279 2e64 6174 655b 3a22  sales.by.date[:"
+00007110: 3230 3030 2f30 342f 3031 225d 2e61 6c6c  2000/04/01"].all
+00007120: 2e71 7479 2929 0a20 2020 2020 2020 2073  .qty)).        s
+00007130: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00007140: 3936 2c20 7375 6d28 7361 6c65 732e 6279  96, sum(sales.by
+00007150: 2e64 6174 655b 2232 3030 302f 3034 2f30  .date["2000/04/0
+00007160: 3122 3a5d 2e61 6c6c 2e71 7479 2929 0a0a  1":].all.qty))..
+00007170: 2020 2020 6465 6620 7465 7374 5f69 6e64      def test_ind
+00007180: 6578 5f64 6972 2873 656c 6629 3a0a 2020  ex_dir(self):.  
+00007190: 2020 2020 2020 6368 6172 7320 3d20 2241        chars = "A
+000071a0: 4243 4445 4647 4849 4a4b 4c4d 4e4f 5051  BCDEFGHIJKLMNOPQ
+000071b0: 5253 5455 5657 5859 5a22 0a20 2020 2020  RSTUVWXYZ".     
+000071c0: 2020 206d 616b 655f 7265 6320 3d20 6c61     make_rec = la
+000071d0: 6d62 6461 2061 612c 2062 622c 2063 633a  mbda aa, bb, cc:
+000071e0: 2073 656c 662e 6d61 6b65 5f64 6174 615f   self.make_data_
+000071f0: 6f62 6a65 6374 2863 6861 7273 5b61 6120  object(chars[aa 
+00007200: 2520 6c65 6e28 6368 6172 7329 5d2c 0a20  % len(chars)],. 
+00007210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007240: 2020 2020 2020 2020 2020 2063 6861 7273             chars
+00007250: 5b62 6220 2520 6c65 6e28 6368 6172 7329  [bb % len(chars)
+00007260: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00007270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007290: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000072a0: 6861 7273 5b63 6320 2520 6c65 6e28 6368  hars[cc % len(ch
+000072b0: 6172 7329 5d29 0a20 2020 2020 2020 2074  ars)]).        t
+000072c0: 6573 745f 7369 7a65 203d 2031 300a 2020  est_size = 10.  
+000072d0: 2020 2020 2020 7461 626c 6520 3d20 6d61        table = ma
+000072e0: 6b65 5f74 6573 745f 7461 626c 6528 6d61  ke_test_table(ma
+000072f0: 6b65 5f72 6563 2c20 7465 7374 5f73 697a  ke_rec, test_siz
+00007300: 6529 0a20 2020 2020 2020 2074 6162 6c65  e).        table
+00007310: 2e63 7265 6174 655f 696e 6465 7828 2761  .create_index('a
+00007320: 2729 0a20 2020 2020 2020 2074 6162 6c65  ').        table
+00007330: 2e63 7265 6174 655f 696e 6465 7828 2762  .create_index('b
+00007340: 2729 0a0a 2020 2020 2020 2020 6469 725f  ')..        dir_
+00007350: 6c69 7374 203d 2064 6972 2874 6162 6c65  list = dir(table
+00007360: 2e62 7929 0a20 2020 2020 2020 2070 7269  .by).        pri
+00007370: 6e74 285b 6174 7472 2066 6f72 2061 7474  nt([attr for att
+00007380: 7220 696e 2064 6972 5f6c 6973 7420 6966  r in dir_list if
+00007390: 206e 6f74 2061 7474 722e 7374 6172 7473   not attr.starts
+000073a0: 7769 7468 2822 5f22 295d 290a 0a20 2020  with("_")])..   
+000073b0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000073c0: 5472 7565 2828 2761 2720 696e 2064 6972  True(('a' in dir
+000073d0: 5f6c 6973 7429 2061 6e64 2028 2762 2720  _list) and ('b' 
+000073e0: 696e 2064 6972 5f6c 6973 7429 2061 6e64  in dir_list) and
+000073f0: 2028 2763 2720 6e6f 7420 696e 2064 6972   ('c' not in dir
+00007400: 5f6c 6973 7429 290a 0a20 2020 2064 6566  _list))..    def
+00007410: 2074 6573 745f 6465 6c65 7465 5f62 795f   test_delete_by_
+00007420: 6669 6c74 6572 2873 656c 6629 3a0a 2020  filter(self):.  
+00007430: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
+00007440: 3d20 3130 0a20 2020 2020 2020 2074 6162  = 10.        tab
+00007450: 6c65 203d 206d 616b 655f 7465 7374 5f74  le = make_test_t
+00007460: 6162 6c65 2873 656c 662e 6d61 6b65 5f64  able(self.make_d
+00007470: 6174 615f 6f62 6a65 6374 2c20 7465 7374  ata_object, test
+00007480: 5f73 697a 6529 0a0a 2020 2020 2020 2020  _size)..        
+00007490: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000074a0: 2874 6573 745f 7369 7a65 2a74 6573 745f  (test_size*test_
+000074b0: 7369 7a65 2c20 7461 626c 652e 6465 6c65  size, table.dele
+000074c0: 7465 2862 3d35 2929 0a20 2020 2020 2020  te(b=5)).       
+000074d0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000074e0: 6c28 7465 7374 5f73 697a 652a 7465 7374  l(test_size*test
+000074f0: 5f73 697a 652a 2874 6573 745f 7369 7a65  _size*(test_size
+00007500: 2d31 292c 206c 656e 2874 6162 6c65 2929  -1), len(table))
+00007510: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00007520: 7365 7274 4571 7561 6c28 302c 2074 6162  sertEqual(0, tab
+00007530: 6c65 2e64 656c 6574 6528 623d 2d31 2929  le.delete(b=-1))
+00007540: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00007550: 7365 7274 4571 7561 6c28 302c 2074 6162  sertEqual(0, tab
+00007560: 6c65 2e64 656c 6574 6528 2929 0a0a 2020  le.delete())..  
+00007570: 2020 6465 6620 7465 7374 5f72 656d 6f76    def test_remov
+00007580: 655f 6d61 6e79 2873 656c 6629 3a0a 2020  e_many(self):.  
+00007590: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
+000075a0: 3d20 3130 0a20 2020 2020 2020 2074 6162  = 10.        tab
+000075b0: 6c65 203d 206d 616b 655f 7465 7374 5f74  le = make_test_t
+000075c0: 6162 6c65 2873 656c 662e 6d61 6b65 5f64  able(self.make_d
+000075d0: 6174 615f 6f62 6a65 6374 2c20 7465 7374  ata_object, test
+000075e0: 5f73 697a 6529 0a0a 2020 2020 2020 2020  _size)..        
+000075f0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00007600: 2874 6573 745f 7369 7a65 2a74 6573 745f  (test_size*test_
+00007610: 7369 7a65 2a74 6573 745f 7369 7a65 2f32  size*test_size/2
+00007620: 2c20 6c65 6e28 7461 626c 652e 7768 6572  , len(table.wher
+00007630: 6528 6c61 6d62 6461 2074 3a20 742e 6120  e(lambda t: t.a 
+00007640: 2520 3229 2929 0a20 2020 2020 2020 2074  % 2))).        t
+00007650: 6162 6c65 2e72 656d 6f76 655f 6d61 6e79  able.remove_many
+00007660: 2874 6162 6c65 2e77 6865 7265 286c 616d  (table.where(lam
+00007670: 6264 6120 743a 2074 2e61 2025 2032 2929  bda t: t.a % 2))
+00007680: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00007690: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
+000076a0: 697a 652a 7465 7374 5f73 697a 652a 7465  ize*test_size*te
+000076b0: 7374 5f73 697a 652f 322c 206c 656e 2874  st_size/2, len(t
+000076c0: 6162 6c65 2929 0a20 2020 2020 2020 2074  able)).        t
+000076d0: 6162 6c65 5f6c 656e 203d 206c 656e 2874  able_len = len(t
+000076e0: 6162 6c65 290a 2020 2020 2020 2020 7461  able).        ta
+000076f0: 626c 652e 7265 6d6f 7665 2874 6162 6c65  ble.remove(table
+00007700: 5b31 5d29 0a20 2020 2020 2020 2073 656c  [1]).        sel
+00007710: 662e 6173 7365 7274 4571 7561 6c28 7461  f.assertEqual(ta
+00007720: 626c 655f 6c65 6e2d 312c 206c 656e 2874  ble_len-1, len(t
+00007730: 6162 6c65 2929 0a0a 2020 2020 6465 6620  able))..    def 
+00007740: 7465 7374 5f61 6464 5f6e 6577 5f66 6965  test_add_new_fie
+00007750: 6c64 2873 656c 6629 3a0a 2020 2020 2020  ld(self):.      
+00007760: 2020 7465 7374 5f73 697a 6520 3d20 3130    test_size = 10
+00007770: 0a20 2020 2020 2020 2074 6162 6c65 203d  .        table =
+00007780: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
+00007790: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
+000077a0: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
+000077b0: 6529 0a0a 2020 2020 2020 2020 2320 6e6f  e)..        # no
+000077c0: 7420 616c 6c20 7374 6f72 6167 6520 636c  t all storage cl
+000077d0: 6173 7365 7320 7375 7070 6f72 7420 6164  asses support ad
+000077e0: 6469 6e67 206e 6577 2066 6965 6c64 730a  ding new fields.
+000077f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00007800: 7374 6f72 6167 655f 7375 7070 6f72 7473  storage_supports
+00007810: 5f61 6464 5f66 6965 6c64 3a0a 2020 2020  _add_field:.    
+00007820: 2020 2020 2020 2020 7461 626c 652e 6164          table.ad
+00007830: 645f 6669 656c 6428 2764 272c 206c 616d  d_field('d', lam
+00007840: 6264 6120 7265 633a 2072 6563 2e61 2b72  bda rec: rec.a+r
+00007850: 6563 2e62 2b72 6563 2e63 290a 0a20 2020  ec.b+rec.c)..   
+00007860: 2020 2020 2020 2020 2074 6162 6c65 2e63           table.c
+00007870: 7265 6174 655f 696e 6465 7828 2764 2729  reate_index('d')
+00007880: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00007890: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+000078a0: 6e28 7261 6e67 6528 302c 2032 372b 3129  n(range(0, 27+1)
+000078b0: 292c 206c 656e 2874 6162 6c65 2e62 792e  ), len(table.by.
+000078c0: 642e 6b65 7973 2829 2929 0a0a 2020 2020  d.keys()))..    
+000078d0: 6465 6620 7465 7374 5f61 6464 5f66 6965  def test_add_fie
+000078e0: 6c64 5f6f 7665 725f 6578 6973 7469 6e67  ld_over_existing
+000078f0: 5f69 6e64 6578 6564 5f66 6965 6c64 2873  _indexed_field(s
+00007900: 656c 6629 3a0a 2020 2020 2020 2020 7465  elf):.        te
+00007910: 7374 5f73 697a 6520 3d20 320a 2020 2020  st_size = 2.    
+00007920: 2020 2020 7461 626c 6520 3d20 6d61 6b65      table = make
+00007930: 5f74 6573 745f 7461 626c 6528 7365 6c66  _test_table(self
+00007940: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
+00007950: 742c 2074 6573 745f 7369 7a65 290a 2020  t, test_size).  
+00007960: 2020 2020 2020 7461 626c 652e 6372 6561        table.crea
+00007970: 7465 5f69 6e64 6578 2827 6327 290a 0a20  te_index('c').. 
+00007980: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00007990: 6c66 2e73 746f 7261 6765 5f69 735f 6d75  lf.storage_is_mu
+000079a0: 7461 626c 653a 0a20 2020 2020 2020 2020  table:.         
+000079b0: 2020 2072 6574 7572 6e0a 0a20 2020 2020     return..     
+000079c0: 2020 2074 6162 6c65 2e61 6464 5f66 6965     table.add_fie
+000079d0: 6c64 2827 6327 2c20 6c61 6d62 6461 2072  ld('c', lambda r
+000079e0: 6563 3a20 2d31 290a 2020 2020 2020 2020  ec: -1).        
+000079f0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00007a00: 280a 2020 2020 2020 2020 2020 2020 5b72  (.            [r
+00007a10: 6563 2e63 2066 6f72 2072 6563 2069 6e20  ec.c for rec in 
+00007a20: 7461 626c 655d 2c0a 2020 2020 2020 2020  table],.        
+00007a30: 2020 2020 6c69 7374 2874 6162 6c65 2e61      list(table.a
+00007a40: 6c6c 2e63 292c 0a20 2020 2020 2020 2020  ll.c),.         
+00007a50: 2020 2022 616c 6c20 6c69 7374 2072 6561     "all list rea
+00007a60: 6473 2069 6e64 6578 2c20 7768 6963 6820  ds index, which 
+00007a70: 6973 206e 6f74 2072 6562 7569 6c74 2062  is not rebuilt b
+00007a80: 7920 6164 645f 6669 656c 6422 2c0a 2020  y add_field",.  
+00007a90: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00007aa0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00007ab0: 6c28 0a20 2020 2020 2020 2020 2020 207b  l(.            {
+00007ac0: 2d31 7d2c 0a20 2020 2020 2020 2020 2020  -1},.           
+00007ad0: 2073 6574 2874 6162 6c65 2e62 792e 632e   set(table.by.c.
+00007ae0: 6b65 7973 2829 292c 0a20 2020 2020 2020  keys()),.       
+00007af0: 2020 2020 2022 696e 6465 7820 6b65 7973       "index keys
+00007b00: 2061 7265 206e 6f74 2072 6562 7569 6c74   are not rebuilt
+00007b10: 2062 7920 6164 645f 6669 656c 6422 2c0a   by add_field",.
+00007b20: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+00007b30: 6566 2074 6573 745f 6164 645f 7477 6f5f  ef test_add_two_
+00007b40: 7461 626c 6573 2873 656c 6629 3a0a 2020  tables(self):.  
+00007b50: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
+00007b60: 3d20 3130 0a20 2020 2020 2020 2074 3120  = 10.        t1 
+00007b70: 3d20 6d61 6b65 5f74 6573 745f 7461 626c  = make_test_tabl
+00007b80: 6528 7365 6c66 2e6d 616b 655f 6461 7461  e(self.make_data
+00007b90: 5f6f 626a 6563 742c 2074 6573 745f 7369  _object, test_si
+00007ba0: 7a65 290a 2020 2020 2020 2020 6d61 6b65  ze).        make
+00007bb0: 5f72 6563 203d 206c 616d 6264 6120 612c  _rec = lambda a,
+00007bc0: 622c 633a 2073 656c 662e 6d61 6b65 5f64  b,c: self.make_d
+00007bd0: 6174 615f 6f62 6a65 6374 2861 2b74 6573  ata_object(a+tes
+00007be0: 745f 7369 7a65 2c20 622c 2063 290a 2020  t_size, b, c).  
+00007bf0: 2020 2020 2020 7432 203d 206d 616b 655f        t2 = make_
+00007c00: 7465 7374 5f74 6162 6c65 286d 616b 655f  test_table(make_
+00007c10: 7265 632c 2074 6573 745f 7369 7a65 290a  rec, test_size).
+00007c20: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00007c30: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
+00007c40: 697a 652a 7465 7374 5f73 697a 652a 7465  ize*test_size*te
+00007c50: 7374 5f73 697a 652a 322c 206c 656e 2874  st_size*2, len(t
+00007c60: 312b 7432 2929 0a20 2020 2020 2020 2073  1+t2)).        s
+00007c70: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00007c80: 7465 7374 5f73 697a 6520 2a20 7465 7374  test_size * test
+00007c90: 5f73 697a 6520 2a20 7465 7374 5f73 697a  _size * test_siz
+00007ca0: 652c 206c 656e 2874 3129 290a 0a20 2020  e, len(t1))..   
+00007cb0: 2020 2020 2074 3120 2b3d 2074 320a 2020       t1 += t2.  
+00007cc0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00007cd0: 7445 7175 616c 2874 6573 745f 7369 7a65  tEqual(test_size
+00007ce0: 202a 2074 6573 745f 7369 7a65 202a 2074   * test_size * t
+00007cf0: 6573 745f 7369 7a65 202a 2032 2c20 6c65  est_size * 2, le
+00007d00: 6e28 7431 2929 0a0a 2020 2020 2020 2020  n(t1))..        
+00007d10: 6f66 6673 6574 203d 2074 6573 745f 7369  offset = test_si
+00007d20: 7a65 202a 2074 6573 745f 7369 7a65 0a20  ze * test_size. 
+00007d30: 2020 2020 2020 2074 3320 3d20 7431 202b         t3 = t1 +
+00007d40: 2028 7365 6c66 2e6d 616b 655f 6461 7461   (self.make_data
+00007d50: 5f6f 626a 6563 7428 7265 632e 612b 6f66  _object(rec.a+of
+00007d60: 6673 6574 2c20 7265 632e 622c 2072 6563  fset, rec.b, rec
+00007d70: 2e63 2920 666f 7220 7265 6320 696e 2074  .c) for rec in t
+00007d80: 3229 0a20 2020 2020 2020 2073 656c 662e  2).        self.
+00007d90: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
+00007da0: 5f73 697a 6520 2a20 7465 7374 5f73 697a  _size * test_siz
+00007db0: 6520 2a20 7465 7374 5f73 697a 6520 2a20  e * test_size * 
+00007dc0: 332c 206c 656e 2874 3329 290a 0a20 2020  3, len(t3))..   
+00007dd0: 2064 6566 2074 6573 745f 7461 626c 655f   def test_table_
+00007de0: 696e 666f 2873 656c 6629 3a0a 2020 2020  info(self):.    
+00007df0: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
+00007e00: 3130 0a20 2020 2020 2020 2077 6974 6820  10.        with 
+00007e10: 7469 6d65 7374 616d 705f 7374 6172 745f  timestamp_start_
+00007e20: 656e 6428 2920 6173 2074 696d 696e 673a  end() as timing:
+00007e30: 0a20 2020 2020 2020 2020 2020 2074 3120  .            t1 
+00007e40: 3d20 6d61 6b65 5f74 6573 745f 7461 626c  = make_test_tabl
+00007e50: 6528 7365 6c66 2e6d 616b 655f 6461 7461  e(self.make_data
+00007e60: 5f6f 626a 6563 742c 2074 6573 745f 7369  _object, test_si
+00007e70: 7a65 2928 2769 6e66 6f5f 7465 7374 2729  ze)('info_test')
+00007e80: 0a0a 2020 2020 2020 2020 7431 2e63 7265  ..        t1.cre
+00007e90: 6174 655f 696e 6465 7828 2762 2729 0a20  ate_index('b'). 
+00007ea0: 2020 2020 2020 2074 315f 696e 666f 203d         t1_info =
+00007eb0: 2074 312e 696e 666f 2829 0a20 2020 2020   t1.info().     
+00007ec0: 2020 2023 206d 7573 7420 736f 7274 2066     # must sort f
+00007ed0: 6965 6c64 7320 616e 6420 696e 6465 7865  ields and indexe
+00007ee0: 7320 7661 6c75 6573 2c20 666f 7220 7465  s values, for te
+00007ef0: 7374 2063 6f6d 7061 7269 736f 6e73 0a20  st comparisons. 
+00007f00: 2020 2020 2020 2074 315f 696e 666f 5b27         t1_info['
+00007f10: 6669 656c 6473 275d 2e73 6f72 7428 290a  fields'].sort().
+00007f20: 2020 2020 2020 2020 7431 5f69 6e66 6f5b          t1_info[
+00007f30: 2769 6e64 6578 6573 275d 2e73 6f72 7428  'indexes'].sort(
+00007f40: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00007f50: 7373 6572 7445 7175 616c 284e 6f6e 652c  ssertEqual(None,
+00007f60: 2074 315f 696e 666f 2e70 6f70 2822 6c61   t1_info.pop("la
+00007f70: 7374 5f69 6d70 6f72 7422 2929 0a20 2020  st_import")).   
+00007f80: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00007f90: 5472 7565 2874 696d 696e 672e 7374 6172  True(timing.star
+00007fa0: 7420 3c3d 2074 315f 696e 666f 2e70 6f70  t <= t1_info.pop
+00007fb0: 2822 6372 6561 7465 6422 2920 3c3d 2074  ("created") <= t
+00007fc0: 696d 696e 672e 656e 6429 0a20 2020 2020  iming.end).     
+00007fd0: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+00007fe0: 7565 2874 696d 696e 672e 7374 6172 7420  ue(timing.start 
+00007ff0: 3c3d 2074 315f 696e 666f 2e70 6f70 2822  <= t1_info.pop("
+00008000: 6d6f 6469 6669 6564 2229 203c 3d20 7469  modified") <= ti
+00008010: 6d69 6e67 2e65 6e64 290a 2020 2020 2020  ming.end).      
+00008020: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00008030: 616c 287b 2766 6965 6c64 7327 3a20 5b27  al({'fields': ['
+00008040: 6127 2c20 2762 272c 2027 6327 5d2c 0a20  a', 'b', 'c'],. 
+00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008060: 2020 2020 2020 2020 2027 696e 6465 7865           'indexe
+00008070: 7327 3a20 5b28 2762 272c 2046 616c 7365  s': [('b', False
+00008080: 295d 2c0a 2020 2020 2020 2020 2020 2020  )],.            
+00008090: 2020 2020 2020 2020 2020 2020 2020 276c                'l
+000080a0: 656e 273a 2031 3030 302c 0a20 2020 2020  en': 1000,.     
+000080b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080c0: 2020 2020 2027 6e61 6d65 273a 2027 696e       'name': 'in
+000080d0: 666f 5f74 6573 7427 7d2c 0a20 2020 2020  fo_test'},.     
+000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080f0: 2020 2020 7431 5f69 6e66 6f2c 2022 696e      t1_info, "in
+00008100: 7661 6c69 6420 696e 666f 2072 6573 756c  valid info resul
+00008110: 7473 2229 0a0a 0a40 6d61 6b65 5f74 6573  ts")...@make_tes
+00008120: 745f 636c 6173 7365 730a 636c 6173 7320  t_classes.class 
+00008130: 5461 626c 654c 6973 7454 6573 7473 3a0a  TableListTests:.
+00008140: 2020 2020 6465 6620 5f74 6573 745f 696e      def _test_in
+00008150: 6974 2873 656c 6629 3a0a 2020 2020 2020  it(self):.      
+00008160: 2020 7365 6c66 2e74 6573 745f 7369 7a65    self.test_size
+00008170: 203d 2033 0a20 2020 2020 2020 2073 656c   = 3.        sel
+00008180: 662e 7431 203d 206d 616b 655f 7465 7374  f.t1 = make_test
+00008190: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
+000081a0: 5f64 6174 615f 6f62 6a65 6374 2c20 7365  _data_object, se
+000081b0: 6c66 2e74 6573 745f 7369 7a65 290a 2020  lf.test_size).  
+000081c0: 2020 2020 2020 7365 6c66 2e74 6573 745f        self.test_
+000081d0: 7265 6320 3d20 7365 6c66 2e6d 616b 655f  rec = self.make_
+000081e0: 6461 7461 5f6f 626a 6563 7428 312c 2031  data_object(1, 1
+000081f0: 2c20 3129 0a0a 2020 2020 6465 6620 7465  , 1)..    def te
+00008200: 7374 5f63 6f6e 7461 696e 7328 7365 6c66  st_contains(self
+00008210: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00008220: 5f74 6573 745f 696e 6974 2829 0a20 2020  _test_init().   
+00008230: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00008240: 5472 7565 2873 656c 662e 7465 7374 5f72  True(self.test_r
+00008250: 6563 2069 6e20 7365 6c66 2e74 312c 2022  ec in self.t1, "
+00008260: 6661 696c 6564 2027 696e 2720 2863 6f6e  failed 'in' (con
+00008270: 7461 696e 7329 2074 6573 7422 290a 0a20  tains) test").. 
+00008280: 2020 2064 6566 2074 6573 745f 696e 6465     def test_inde
+00008290: 785f 6669 6e64 2873 656c 6629 3a0a 2020  x_find(self):.  
+000082a0: 2020 2020 2020 7365 6c66 2e5f 7465 7374        self._test
+000082b0: 5f69 6e69 7428 290a 2020 2020 2020 2020  _init().        
+000082c0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000082d0: 2831 332c 2073 656c 662e 7431 2e69 6e64  (13, self.t1.ind
+000082e0: 6578 2873 656c 662e 7465 7374 5f72 6563  ex(self.test_rec
+000082f0: 292c 2022 6661 696c 6564 2027 696e 6465  ), "failed 'inde
+00008300: 783b 2074 6573 7420 2865 7869 7374 7329  x; test (exists)
+00008310: 2229 0a20 2020 2020 2020 2069 6620 6973  ").        if is
+00008320: 696e 7374 616e 6365 2873 656c 662e 7465  instance(self.te
+00008330: 7374 5f72 6563 2c20 5369 6d70 6c65 4e61  st_rec, SimpleNa
+00008340: 6d65 7370 6163 6529 3a0a 2020 2020 2020  mespace):.      
+00008350: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00008360: 7445 7175 616c 2831 332c 2073 656c 662e  tEqual(13, self.
+00008370: 7431 2e69 6e64 6578 2876 6172 7328 7365  t1.index(vars(se
+00008380: 6c66 2e74 6573 745f 7265 6329 292c 2022  lf.test_rec)), "
+00008390: 6661 696c 6564 2027 696e 6465 783b 2074  failed 'index; t
+000083a0: 6573 7420 2865 7869 7374 7329 2229 0a0a  est (exists)")..
+000083b0: 2020 2020 2020 2020 6e6f 5f73 7563 685f          no_such_
+000083c0: 7265 6320 3d20 7365 6c66 2e6d 616b 655f  rec = self.make_
+000083d0: 6461 7461 5f6f 626a 6563 7428 7365 6c66  data_object(self
+000083e0: 2e74 6573 745f 7369 7a65 2b31 2c20 7365  .test_size+1, se
+000083f0: 6c66 2e74 6573 745f 7369 7a65 2b31 2c20  lf.test_size+1, 
+00008400: 7365 6c66 2e74 6573 745f 7369 7a65 2b31  self.test_size+1
+00008410: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+00008420: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
+00008430: 2856 616c 7565 4572 726f 722c 206d 7367  (ValueError, msg
+00008440: 3d22 6661 696c 6564 2027 696e 6465 7827  ="failed 'index'
+00008450: 2074 6573 7420 286e 6f74 2065 7869 7374   test (not exist
+00008460: 7329 2229 3a0a 2020 2020 2020 2020 2020  s)"):.          
+00008470: 2020 7365 6c66 2e74 312e 696e 6465 7828    self.t1.index(
+00008480: 6e6f 5f73 7563 685f 7265 6329 0a0a 2020  no_such_rec)..  
+00008490: 2020 6465 6620 7465 7374 5f72 656d 6f76    def test_remov
+000084a0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000084b0: 2073 656c 662e 5f74 6573 745f 696e 6974   self._test_init
+000084c0: 2829 0a20 2020 2020 2020 2072 6563 203d  ().        rec =
+000084d0: 2073 656c 662e 6d61 6b65 5f64 6174 615f   self.make_data_
+000084e0: 6f62 6a65 6374 2831 2c20 312c 2031 290a  object(1, 1, 1).
+000084f0: 2020 2020 2020 2020 7072 6576 5f6c 656e          prev_len
+00008500: 203d 206c 656e 2873 656c 662e 7431 290a   = len(self.t1).
+00008510: 2020 2020 2020 2020 7365 6c66 2e74 312e          self.t1.
+00008520: 7265 6d6f 7665 2872 6563 290a 2020 2020  remove(rec).    
+00008530: 2020 2020 7365 6c66 2e61 7373 6572 7446      self.assertF
+00008540: 616c 7365 2872 6563 2069 6e20 7365 6c66  alse(rec in self
+00008550: 2e74 312c 2022 6661 696c 6564 2074 6f20  .t1, "failed to 
+00008560: 7265 6d6f 7665 2072 6563 6f72 6420 6672  remove record fr
+00008570: 6f6d 2074 6162 6c65 2028 636f 6e74 6169  om table (contai
+00008580: 6e73 2922 290a 2020 2020 2020 2020 7365  ns)").        se
+00008590: 6c66 2e61 7373 6572 7445 7175 616c 2870  lf.assertEqual(p
+000085a0: 7265 765f 6c65 6e2d 312c 206c 656e 2873  rev_len-1, len(s
+000085b0: 656c 662e 7431 292c 2022 6661 696c 6564  elf.t1), "failed
+000085c0: 2074 6f20 7265 6d6f 7665 2072 6563 6f72   to remove recor
+000085d0: 6420 6672 6f6d 2074 6162 6c65 2028 6c65  d from table (le
+000085e0: 6e29 2229 0a0a 2020 2020 2020 2020 6e6f  n)")..        no
+000085f0: 5f73 7563 685f 7265 6320 3d20 7365 6c66  _such_rec = self
+00008600: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
+00008610: 7428 7365 6c66 2e74 6573 745f 7369 7a65  t(self.test_size
+00008620: 2b31 2c20 7365 6c66 2e74 6573 745f 7369  +1, self.test_si
+00008630: 7a65 2b31 2c20 7365 6c66 2e74 6573 745f  ze+1, self.test_
+00008640: 7369 7a65 2b31 290a 2020 2020 2020 2020  size+1).        
+00008650: 7365 6c66 2e61 7373 6572 7446 616c 7365  self.assertFalse
+00008660: 286e 6f5f 7375 6368 5f72 6563 2069 6e20  (no_such_rec in 
+00008670: 7365 6c66 2e74 312c 2022 6661 696c 6564  self.t1, "failed
+00008680: 2074 6f20 6372 6561 7465 206e 6f6e 2d65   to create non-e
+00008690: 7869 7374 656e 7420 7265 636f 7264 2066  xistent record f
+000086a0: 726f 6d20 7461 626c 6522 290a 2020 2020  rom table").    
+000086b0: 2020 2020 7365 6c66 2e74 312e 7265 6d6f      self.t1.remo
+000086c0: 7665 286e 6f5f 7375 6368 5f72 6563 290a  ve(no_such_rec).
+000086d0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000086e0: 6572 7445 7175 616c 2870 7265 765f 6c65  ertEqual(prev_le
+000086f0: 6e2d 312c 206c 656e 2873 656c 662e 7431  n-1, len(self.t1
+00008700: 292c 2022 6661 696c 6564 2072 656d 6f76  ), "failed remov
+00008710: 696e 6720 6e6f 6e2d 6578 6973 7465 6e74  ing non-existent
+00008720: 2072 6563 6f72 6420 6672 6f6d 2074 6162   record from tab
+00008730: 6c65 2028 6c65 6e29 2229 0a0a 2020 2020  le (len)")..    
+00008740: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00008750: 6528 7365 6c66 2e74 6573 745f 7265 632c  e(self.test_rec,
+00008760: 2053 696d 706c 654e 616d 6573 7061 6365   SimpleNamespace
+00008770: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00008780: 656c 662e 7431 2e72 656d 6f76 6528 7661  elf.t1.remove(va
+00008790: 7273 2873 656c 662e 7465 7374 5f72 6563  rs(self.test_rec
+000087a0: 2929 0a20 2020 2020 2020 2020 2020 2073  )).            s
+000087b0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000087c0: 7072 6576 5f6c 656e 2d31 2c20 6c65 6e28  prev_len-1, len(
+000087d0: 7365 6c66 2e74 3129 2c20 2266 6169 6c65  self.t1), "faile
+000087e0: 6420 746f 2072 656d 6f76 6520 7265 636f  d to remove reco
+000087f0: 7264 2061 7320 6469 6374 2066 726f 6d20  rd as dict from 
+00008800: 7461 626c 6520 286c 656e 2922 290a 0a20  table (len)").. 
+00008810: 2020 2064 6566 2074 6573 745f 696e 6465     def test_inde
+00008820: 785f 6163 6365 7373 2873 656c 6629 3a0a  x_access(self):.
+00008830: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
+00008840: 7374 5f69 6e69 7428 290a 2020 2020 2020  st_init().      
+00008850: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00008860: 616c 2873 656c 662e 7465 7374 5f72 6563  al(self.test_rec
+00008870: 2c20 7365 6c66 2e74 315b 3133 5d2c 2022  , self.t1[13], "
+00008880: 6661 696c 6564 2069 6e64 6578 2061 6363  failed index acc
+00008890: 6573 7320 7465 7374 2229 0a0a 2020 2020  ess test")..    
+000088a0: 6465 6620 7465 7374 5f63 6f75 6e74 2873  def test_count(s
+000088b0: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+000088c0: 6c66 2e5f 7465 7374 5f69 6e69 7428 290a  lf._test_init().
+000088d0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000088e0: 6572 7454 7275 6528 7365 6c66 2e74 312e  ertTrue(self.t1.
+000088f0: 636f 756e 7428 7365 6c66 2e74 6573 745f  count(self.test_
+00008900: 7265 6329 203d 3d20 312c 2022 6661 696c  rec) == 1, "fail
+00008910: 6564 2063 6f75 6e74 2074 6573 7422 290a  ed count test").
+00008920: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00008930: 7461 6e63 6528 7365 6c66 2e74 6573 745f  tance(self.test_
+00008940: 7265 632c 2053 696d 706c 654e 616d 6573  rec, SimpleNames
+00008950: 7061 6365 293a 0a20 2020 2020 2020 2020  pace):.         
+00008960: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+00008970: 7565 2873 656c 662e 7431 2e63 6f75 6e74  ue(self.t1.count
+00008980: 2876 6172 7328 7365 6c66 2e74 6573 745f  (vars(self.test_
+00008990: 7265 6329 2920 3d3d 2031 2c20 2266 6169  rec)) == 1, "fai
+000089a0: 6c65 6420 636f 756e 7420 7465 7374 2229  led count test")
+000089b0: 0a0a 2020 2020 6465 6620 7465 7374 5f64  ..    def test_d
+000089c0: 656c 2873 656c 6629 3a0a 2020 2020 2020  el(self):.      
+000089d0: 2020 7365 6c66 2e5f 7465 7374 5f69 6e69    self._test_ini
+000089e0: 7428 290a 2020 2020 2020 2020 6265 666f  t().        befo
+000089f0: 7265 5f64 656c 5f6c 656e 203d 206c 656e  re_del_len = len
+00008a00: 2873 656c 662e 7431 290a 2020 2020 2020  (self.t1).      
+00008a10: 2020 6465 6c20 7365 6c66 2e74 315b 3133    del self.t1[13
+00008a20: 5d0a 2020 2020 2020 2020 7365 6c66 2e61  ].        self.a
+00008a30: 7373 6572 7446 616c 7365 2873 656c 662e  ssertFalse(self.
+00008a40: 7465 7374 5f72 6563 2069 6e20 7365 6c66  test_rec in self
+00008a50: 2e74 312c 2022 6661 696c 6564 2064 656c  .t1, "failed del
+00008a60: 2074 6573 7422 290a 2020 2020 2020 2020   test").        
+00008a70: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00008a80: 2862 6566 6f72 655f 6465 6c5f 6c65 6e20  (before_del_len 
+00008a90: 2d20 312c 206c 656e 2873 656c 662e 7431  - 1, len(self.t1
+00008aa0: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
+00008ab0: 5f70 6f70 2873 656c 6629 3a0a 2020 2020  _pop(self):.    
+00008ac0: 2020 2020 7365 6c66 2e5f 7465 7374 5f69      self._test_i
+00008ad0: 6e69 7428 290a 2020 2020 2020 2020 6265  nit().        be
+00008ae0: 666f 7265 5f70 6f70 5f6c 656e 203d 206c  fore_pop_len = l
+00008af0: 656e 2873 656c 662e 7431 290a 2020 2020  en(self.t1).    
+00008b00: 2020 2020 6f62 6a20 3d20 7365 6c66 2e74      obj = self.t
+00008b10: 312e 706f 7028 3133 290a 2020 2020 2020  1.pop(13).      
+00008b20: 2020 7365 6c66 2e61 7373 6572 7446 616c    self.assertFal
+00008b30: 7365 286f 626a 2069 6e20 7365 6c66 2e74  se(obj in self.t
+00008b40: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+00008b50: 6173 7365 7274 4571 7561 6c28 7365 6c66  assertEqual(self
+00008b60: 2e74 6573 745f 7265 632c 206f 626a 290a  .test_rec, obj).
+00008b70: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00008b80: 6572 7445 7175 616c 2862 6566 6f72 655f  ertEqual(before_
+00008b90: 706f 705f 6c65 6e20 2d20 312c 206c 656e  pop_len - 1, len
+00008ba0: 2873 656c 662e 7431 2929 0a0a 2020 2020  (self.t1))..    
+00008bb0: 6465 6620 7465 7374 5f70 6f70 5f6c 6173  def test_pop_las
+00008bc0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+00008bd0: 2073 656c 662e 5f74 6573 745f 696e 6974   self._test_init
+00008be0: 2829 0a20 2020 2020 2020 2062 6566 6f72  ().        befor
+00008bf0: 655f 706f 705f 6c65 6e20 3d20 6c65 6e28  e_pop_len = len(
+00008c00: 7365 6c66 2e74 3129 0a20 2020 2020 2020  self.t1).       
+00008c10: 2065 7870 6563 7465 645f 706f 7020 3d20   expected_pop = 
+00008c20: 636f 7079 2e63 6f70 7928 7365 6c66 2e74  copy.copy(self.t
+00008c30: 315b 2d31 5d29 0a20 2020 2020 2020 206f  1[-1]).        o
+00008c40: 626a 203d 2073 656c 662e 7431 2e70 6f70  bj = self.t1.pop
+00008c50: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00008c60: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
+00008c70: 6374 6564 5f70 6f70 2c20 6f62 6a29 0a20  cted_pop, obj). 
+00008c80: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00008c90: 7274 4571 7561 6c28 6265 666f 7265 5f70  rtEqual(before_p
+00008ca0: 6f70 5f6c 656e 202d 2031 2c20 6c65 6e28  op_len - 1, len(
+00008cb0: 7365 6c66 2e74 3129 290a 0a20 2020 2064  self.t1))..    d
+00008cc0: 6566 2074 6573 745f 7265 7665 7273 6564  ef test_reversed
+00008cd0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00008ce0: 7365 6c66 2e5f 7465 7374 5f69 6e69 7428  self._test_init(
+00008cf0: 290a 2020 2020 2020 2020 6c61 7374 5f72  ).        last_r
+00008d00: 6563 203d 206e 6578 7428 7265 7665 7273  ec = next(revers
+00008d10: 6564 2873 656c 662e 7431 2929 0a20 2020  ed(self.t1)).   
+00008d20: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00008d30: 4571 7561 6c28 7365 6c66 2e6d 616b 655f  Equal(self.make_
+00008d40: 6461 7461 5f6f 626a 6563 7428 322c 2032  data_object(2, 2
+00008d50: 2c20 3229 2c20 6c61 7374 5f72 6563 2c20  , 2), last_rec, 
+00008d60: 2266 6169 6c65 6420 7265 7665 7273 6564  "failed reversed
+00008d70: 2074 6573 7422 290a 0a20 2020 2064 6566   test")..    def
+00008d80: 2074 6573 745f 6974 6572 2873 656c 6629   test_iter(self)
+00008d90: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00008da0: 7465 7374 5f69 6e69 7428 290a 2020 2020  test_init().    
+00008db0: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+00008dc0: 7275 6528 7365 6c66 2e74 6573 745f 7265  rue(self.test_re
+00008dd0: 6320 696e 2073 656c 662e 7431 2c20 2266  c in self.t1, "f
+00008de0: 6169 6c65 6420 2769 6e27 2028 636f 6e74  ailed 'in' (cont
+00008df0: 6169 6e73 2920 7465 7374 2229 0a0a 2020  ains) test")..  
+00008e00: 2020 6465 6620 7465 7374 5f68 6561 645f    def test_head_
+00008e10: 616e 645f 7461 696c 2873 656c 6629 3a0a  and_tail(self):.
+00008e20: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
+00008e30: 7374 5f69 6e69 7428 290a 2020 2020 2020  st_init().      
+00008e40: 2020 7365 6c66 2e74 312e 6372 6561 7465    self.t1.create
+00008e50: 5f69 6e64 6578 2822 6122 290a 2020 2020  _index("a").    
+00008e60: 2020 2020 7365 6c66 2e74 312e 6372 6561      self.t1.crea
+00008e70: 7465 5f69 6e64 6578 2822 6322 290a 2020  te_index("c").  
+00008e80: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00008e90: 7445 7175 616c 287b 2261 222c 2022 6322  tEqual({"a", "c"
+00008ea0: 7d2c 2073 6574 2873 656c 662e 7431 2e5f  }, set(self.t1._
+00008eb0: 696e 6465 7865 732e 6b65 7973 2829 292c  indexes.keys()),
+00008ec0: 2022 6661 696c 6564 2074 6f20 6372 6561   "failed to crea
+00008ed0: 7465 2069 6e64 6578 6573 2229 0a0a 2020  te indexes")..  
+00008ee0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00008ef0: 7445 7175 616c 2873 6574 2873 656c 662e  tEqual(set(self.
+00008f00: 7431 2e5f 696e 6465 7865 732e 6b65 7973  t1._indexes.keys
+00008f10: 2829 292c 0a20 2020 2020 2020 2020 2020  ()),.           
+00008f20: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00008f30: 7428 7365 6c66 2e74 312e 6865 6164 2829  t(self.t1.head()
+00008f40: 2e5f 696e 6465 7865 732e 6b65 7973 2829  ._indexes.keys()
+00008f50: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00008f60: 2020 2020 2020 2020 2020 2020 2266 6169              "fai
+00008f70: 6c65 6420 746f 2063 6f70 7920 696e 6465  led to copy inde
+00008f80: 7865 7320 746f 2068 6561 6428 2922 290a  xes to head()").
+00008f90: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00008fa0: 6572 7445 7175 616c 2873 6574 2873 656c  ertEqual(set(sel
+00008fb0: 662e 7431 2e5f 696e 6465 7865 732e 6b65  f.t1._indexes.ke
+00008fc0: 7973 2829 292c 0a20 2020 2020 2020 2020  ys()),.         
+00008fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fe0: 7365 7428 7365 6c66 2e74 312e 7461 696c  set(self.t1.tail
+00008ff0: 2829 2e5f 696e 6465 7865 732e 6b65 7973  ()._indexes.keys
+00009000: 2829 292c 0a20 2020 2020 2020 2020 2020  ()),.           
+00009010: 2020 2020 2020 2020 2020 2020 2020 2266                "f
+00009020: 6169 6c65 6420 746f 2063 6f70 7920 696e  ailed to copy in
+00009030: 6465 7865 7320 746f 2074 6169 6c28 2922  dexes to tail()"
+00009040: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+00009050: 756e 6971 7565 2873 656c 6629 3a0a 2020  unique(self):.  
+00009060: 2020 2020 2020 7365 6c66 2e5f 7465 7374        self._test
+00009070: 5f69 6e69 7428 290a 2020 2020 2020 2020  _init().        
+00009080: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00009090: 285b 302c 2031 2c20 325d 2c20 736f 7274  ([0, 1, 2], sort
+000090a0: 6564 285b 726f 772e 6120 666f 7220 726f  ed([row.a for ro
+000090b0: 7720 696e 2073 656c 662e 7431 2e75 6e69  w in self.t1.uni
+000090c0: 7175 6528 2761 2729 5d29 2c20 2266 6169  que('a')]), "fai
+000090d0: 6c65 6420 6361 6c6c 2074 6f20 756e 6971  led call to uniq
+000090e0: 7565 2229 0a0a 2020 2020 6465 6620 7465  ue")..    def te
+000090f0: 7374 5f61 6c6c 5f61 6363 6573 736f 7228  st_all_accessor(
+00009100: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+00009110: 656c 662e 5f74 6573 745f 696e 6974 2829  elf._test_init()
+00009120: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00009130: 7365 7274 4571 7561 6c28 7375 6d28 285b  sertEqual(sum(([
+00009140: 695d 2a73 656c 662e 7465 7374 5f73 697a  i]*self.test_siz
+00009150: 652a 2a32 2066 6f72 2069 2069 6e20 7261  e**2 for i in ra
+00009160: 6e67 6528 7365 6c66 2e74 6573 745f 7369  nge(self.test_si
+00009170: 7a65 2929 2c20 5b5d 292c 0a20 2020 2020  ze)), []),.     
+00009180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009190: 2020 2020 6c69 7374 2873 656c 662e 7431      list(self.t1
+000091a0: 2e61 6c6c 2e61 292c 0a20 2020 2020 2020  .all.a),.       
+000091b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091c0: 2020 2266 6169 6c65 6420 746f 2073 7563    "failed to suc
+000091d0: 6365 7373 6675 6c6c 7920 6765 7420 616c  cessfully get al
+000091e0: 6c20 7661 6c75 6573 2069 6e20 2761 2722  l values in 'a'"
+000091f0: 290a 0a20 2020 2020 2020 2061 6c6c 5f61  )..        all_a
+00009200: 7320 3d20 7365 6c66 2e74 312e 616c 6c2e  s = self.t1.all.
+00009210: 610a 2020 2020 2020 2020 7365 6c66 2e61  a.        self.a
+00009220: 7373 6572 7454 7275 6528 616c 6c5f 6173  ssertTrue(all_as
+00009230: 2069 7320 6974 6572 2861 6c6c 5f61 7329   is iter(all_as)
+00009240: 2c20 2261 6c6c 2069 7465 7261 746f 7220  , "all iterator 
+00009250: 6661 696c 7320 746f 2069 6465 6e74 6966  fails to identif
+00009260: 7920 6173 2069 7465 7228 7365 6c66 2922  y as iter(self)"
+00009270: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+00009280: 666f 726d 6174 2873 656c 6629 3a0a 2020  format(self):.  
+00009290: 2020 2020 2020 7365 6c66 2e5f 7465 7374        self._test
+000092a0: 5f69 6e69 7428 290a 2020 2020 2020 2020  _init().        
+000092b0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000092c0: 285b 2730 3020 3020 3027 2c20 2730 3020  (['00 0 0', '00 
+000092d0: 3020 3127 2c20 2730 3020 3020 3227 5d2c  0 1', '00 0 2'],
+000092e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000092f0: 2020 2020 2020 2020 2020 6c69 7374 2873            list(s
+00009300: 656c 662e 7431 2e66 6f72 6d61 7428 227b  elf.t1.format("{
+00009310: 613a 3032 647d 207b 627d 207b 637d 2229  a:02d} {b} {c}")
+00009320: 295b 3a33 5d2c 0a20 2020 2020 2020 2020  )[:3],.         
+00009330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009340: 2266 6169 6c65 6420 746f 2063 7265 6174  "failed to creat
+00009350: 6520 666f 726d 6174 7465 6420 726f 7773  e formatted rows
+00009360: 2229 0a0a 2020 2020 6465 6620 7465 7374  ")..    def test
+00009370: 5f61 735f 6874 6d6c 2873 656c 6629 3a0a  _as_html(self):.
+00009380: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
+00009390: 7374 5f69 6e69 7428 290a 2020 2020 2020  st_init().      
+000093a0: 2020 6874 6d6c 5f6f 7574 7075 7420 3d20    html_output = 
+000093b0: 7365 6c66 2e74 315b 3a31 305d 2e61 735f  self.t1[:10].as_
+000093c0: 6874 6d6c 2866 6965 6c64 733d 2261 2062  html(fields="a b
+000093d0: 2063 2229 0a20 2020 2020 2020 2070 7269   c").        pri
+000093e0: 6e74 2868 746d 6c5f 6f75 7470 7574 290a  nt(html_output).
+000093f0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00009400: 6572 7454 7275 6528 223c 7468 6561 643e  ertTrue("<thead>
+00009410: 2220 696e 2068 746d 6c5f 6f75 7470 7574  " in html_output
+00009420: 2061 6e64 2022 3c74 626f 6479 3e22 2069   and "<tbody>" i
+00009430: 6e20 6874 6d6c 5f6f 7574 7075 742c 0a20  n html_output,. 
+00009440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009450: 2020 2020 2020 2022 6173 5f68 746d 6c20         "as_html 
+00009460: 646f 6573 206e 6f74 2069 6e63 6c75 6465  does not include
+00009470: 2074 6865 6164 2061 6e64 2074 626f 6479   thead and tbody
+00009480: 2074 6167 7322 290a 0a20 2020 2020 2020   tags")..       
+00009490: 2068 746d 6c5f 6c69 6e65 7320 3d20 6874   html_lines = ht
+000094a0: 6d6c 5f6f 7574 7075 742e 7370 6c69 746c  ml_output.splitl
+000094b0: 696e 6573 2829 0a20 2020 2020 2020 2068  ines().        h
+000094c0: 6472 5f6c 696e 6520 3d20 6e65 7874 2868  dr_line = next(h
+000094d0: 2066 6f72 2068 2069 6e20 6874 6d6c 5f6c   for h in html_l
+000094e0: 696e 6573 2069 6620 2263 656e 7465 7222  ines if "center"
+000094f0: 2069 6e20 6829 0a20 2020 2020 2020 2073   in h).        s
+00009500: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00009510: 273c 7472 3e3c 7468 3e3c 6469 7620 616c  '<tr><th><div al
+00009520: 6967 6e3d 2263 656e 7465 7222 3e61 3c2f  ign="center">a</
+00009530: 6469 763e 3c2f 7468 3e27 0a20 2020 2020  div></th>'.     
+00009540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009550: 2020 2020 273c 7468 3e3c 6469 7620 616c      '<th><div al
+00009560: 6967 6e3d 2263 656e 7465 7222 3e62 3c2f  ign="center">b</
+00009570: 6469 763e 3c2f 7468 3e27 0a20 2020 2020  div></th>'.     
+00009580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009590: 2020 2020 273c 7468 3e3c 6469 7620 616c      '<th><div al
+000095a0: 6967 6e3d 2263 656e 7465 7222 3e63 3c2f  ign="center">c</
+000095b0: 6469 763e 3c2f 7468 3e3c 2f74 723e 272c  div></th></tr>',
+000095c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000095d0: 2020 2020 2020 2020 2020 6864 725f 6c69            hdr_li
+000095e0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+000095f0: 2020 2020 2020 2020 2020 2020 2022 6661               "fa
+00009600: 696c 6564 2061 735f 6874 6d6c 2077 6974  iled as_html wit
+00009610: 6820 616c 6c20 6669 656c 6473 2229 0a0a  h all fields")..
+00009620: 2020 2020 2020 2020 6874 6d6c 5f6f 7574          html_out
+00009630: 7075 7420 3d20 7365 6c66 2e74 315b 3a31  put = self.t1[:1
+00009640: 305d 2e61 735f 6874 6d6c 2866 6965 6c64  0].as_html(field
+00009650: 733d 2261 202d 6220 6322 290a 2020 2020  s="a -b c").    
+00009660: 2020 2020 7072 696e 7428 6874 6d6c 5f6f      print(html_o
+00009670: 7574 7075 7429 0a20 2020 2020 2020 2068  utput).        h
+00009680: 746d 6c5f 6c69 6e65 7320 3d20 6874 6d6c  tml_lines = html
+00009690: 5f6f 7574 7075 742e 7370 6c69 746c 696e  _output.splitlin
+000096a0: 6573 2829 0a20 2020 2020 2020 2068 6472  es().        hdr
+000096b0: 5f6c 696e 6520 3d20 6e65 7874 2868 2066  _line = next(h f
+000096c0: 6f72 2068 2069 6e20 6874 6d6c 5f6c 696e  or h in html_lin
+000096d0: 6573 2069 6620 2263 656e 7465 7222 2069  es if "center" i
+000096e0: 6e20 6829 0a20 2020 2020 2020 2073 656c  n h).        sel
+000096f0: 662e 6173 7365 7274 4571 7561 6c28 273c  f.assertEqual('<
+00009700: 7472 3e3c 7468 3e3c 6469 7620 616c 6967  tr><th><div alig
+00009710: 6e3d 2263 656e 7465 7222 3e61 3c2f 6469  n="center">a</di
+00009720: 763e 3c2f 7468 3e27 0a20 2020 2020 2020  v></th>'.       
+00009730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009740: 2020 273c 7468 3e3c 6469 7620 616c 6967    '<th><div alig
+00009750: 6e3d 2263 656e 7465 7222 3e63 3c2f 6469  n="center">c</di
+00009760: 763e 3c2f 7468 3e3c 2f74 723e 272c 0a20  v></th></tr>',. 
+00009770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009780: 2020 2020 2020 2020 6864 725f 6c69 6e65          hdr_line
+00009790: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000097a0: 2020 2020 2020 2020 2020 2022 6661 696c             "fail
+000097b0: 6564 2061 735f 6874 6d6c 2077 6974 6820  ed as_html with 
+000097c0: 6e65 6761 7465 6420 6669 656c 6422 290a  negated field").
+000097d0: 0a20 2020 2020 2020 2068 746d 6c5f 6f75  .        html_ou
+000097e0: 7470 7574 203d 2073 656c 662e 7431 5b3a  tput = self.t1[:
+000097f0: 3130 5d2e 6173 5f68 746d 6c28 6669 656c  10].as_html(fiel
+00009800: 6473 3d22 6120 6220 6322 2c20 666f 726d  ds="a b c", form
+00009810: 6174 733d 7b22 6222 3a20 227b 3a30 3364  ats={"b": "{:03d
+00009820: 7d22 7d29 0a20 2020 2020 2020 2070 7269  }"}).        pri
+00009830: 6e74 2868 746d 6c5f 6f75 7470 7574 290a  nt(html_output).
+00009840: 2020 2020 2020 2020 6874 6d6c 5f6c 696e          html_lin
+00009850: 6573 203d 2068 746d 6c5f 6f75 7470 7574  es = html_output
+00009860: 2e73 706c 6974 6c69 6e65 7328 290a 2020  .splitlines().  
+00009870: 2020 2020 2020 6461 7461 5f6c 696e 6520        data_line 
+00009880: 3d20 6e65 7874 2868 2066 6f72 2068 2069  = next(h for h i
+00009890: 6e20 6874 6d6c 5f6c 696e 6573 2069 6620  n html_lines if 
+000098a0: 223c 7464 3e22 2069 6e20 6829 0a20 2020  "<td>" in h).   
+000098b0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000098c0: 4571 7561 6c28 273c 7462 6f64 793e 3c74  Equal('<tbody><t
+000098d0: 723e 3c74 643e 3c64 6976 2061 6c69 676e  r><td><div align
+000098e0: 3d22 7269 6768 7422 3e30 3c2f 6469 763e  ="right">0</div>
+000098f0: 3c2f 7464 3e27 0a20 2020 2020 2020 2020  </td>'.         
 00009900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009910: 2020 2027 3c74 643e 3c64 6976 2061 6c69     '<td><div ali
-00009920: 676e 3d22 7269 6768 7422 3e30 3030 3c2f  gn="right">000</
-00009930: 6469 763e 3c2f 7464 3e27 0a20 2020 2020  div></td>'.     
+00009910: 273c 7464 3e3c 6469 7620 616c 6967 6e3d  '<td><div align=
+00009920: 2272 6967 6874 223e 3030 303c 2f64 6976  "right">000</div
+00009930: 3e3c 2f74 643e 270a 2020 2020 2020 2020  ></td>'.        
 00009940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009950: 2020 2020 273c 7464 3e3c 6469 7620 616c      '<td><div al
-00009960: 6967 6e3d 2272 6967 6874 223e 3030 303c  ign="right">000<
-00009970: 2f64 6976 3e3c 2f74 643e 3c2f 7472 3e27  /div></td></tr>'
-00009980: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00009990: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-000099a0: 6c69 6e65 2c0a 2020 2020 2020 2020 2020  line,.          
-000099b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000099c0: 6661 696c 6564 2061 735f 6874 6d6c 2077  failed as_html w
-000099d0: 6974 6820 6772 6f75 7062 7922 290a 0a20  ith groupby").. 
-000099e0: 2020 2020 2020 2068 746d 6c5f 6f75 7470         html_outp
-000099f0: 7574 203d 2073 656c 662e 7431 5b3a 3130  ut = self.t1[:10
-00009a00: 5d2e 6173 5f68 746d 6c28 6669 656c 6473  ].as_html(fields
-00009a10: 3d22 6120 6220 6322 2c20 7461 626c 655f  ="a b c", table_
-00009a20: 7072 6f70 6572 7469 6573 3d7b 2262 6f72  properties={"bor
-00009a30: 6465 7222 3a20 2232 227d 290a 2020 2020  der": "2"}).    
-00009a40: 2020 2020 7072 696e 7428 6874 6d6c 5f6f      print(html_o
-00009a50: 7574 7075 7429 0a20 2020 2020 2020 2073  utput).        s
-00009a60: 656c 662e 6173 7365 7274 5472 7565 2822  elf.assertTrue("
-00009a70: 3c74 6865 6164 3e22 2069 6e20 6874 6d6c  <thead>" in html
-00009a80: 5f6f 7574 7075 7420 616e 6420 223c 7462  _output and "<tb
-00009a90: 6f64 793e 2220 696e 2068 746d 6c5f 6f75  ody>" in html_ou
-00009aa0: 7470 7574 2c0a 2020 2020 2020 2020 2020  tput,.          
-00009ab0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-00009ac0: 735f 6874 6d6c 2064 6f65 7320 6e6f 7420  s_html does not 
-00009ad0: 696e 636c 7564 6520 7468 6561 6420 616e  include thead an
-00009ae0: 6420 7462 6f64 7920 7461 6773 2229 0a0a  d tbody tags")..
-00009af0: 0a20 2020 2064 6566 2074 6573 745f 6465  .    def test_de
-00009b00: 6c65 7465 5f73 6c69 6365 7328 7365 6c66  lete_slices(self
-00009b10: 293a 0a20 2020 2020 2020 2063 6f6d 7061  ):.        compa
-00009b20: 7265 5f6c 6973 7420 3d20 6c69 7374 2822  re_list = list("
-00009b30: 4142 4344 4546 4748 494a 4b4c 4d4e 4f50  ABCDEFGHIJKLMNOP
-00009b40: 5152 5354 5556 5758 595a 3031 3233 3435  QRSTUVWXYZ012345
-00009b50: 3637 3839 6162 6364 6566 6768 696a 6b6c  6789abcdefghijkl
-00009b60: 6d6e 6f70 7172 7374 7576 7778 797a 2229  mnopqrstuvwxyz")
-00009b70: 0a20 2020 2020 2020 2074 3120 3d20 6c74  .        t1 = lt
-00009b80: 2e54 6162 6c65 2829 2e69 6e73 6572 745f  .Table().insert_
-00009b90: 6d61 6e79 286c 742e 4461 7461 4f62 6a65  many(lt.DataObje
-00009ba0: 6374 2841 3d63 2920 666f 7220 6320 696e  ct(A=c) for c in
-00009bb0: 2063 6f6d 7061 7265 5f6c 6973 7429 0a0a   compare_list)..
-00009bc0: 2020 2020 2020 2020 6465 6620 6d69 6e69          def mini
-00009bd0: 5f74 6573 7428 736c 635f 7475 706c 6529  _test(slc_tuple)
-00009be0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00009bf0: 2069 7369 6e73 7461 6e63 6528 736c 635f   isinstance(slc_
-00009c00: 7475 706c 652c 2074 7570 6c65 293a 0a20  tuple, tuple):. 
-00009c10: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00009c20: 6162 656c 203d 2022 5b7b 7d3a 7b7d 3a7b  abel = "[{}:{}:{
-00009c30: 7d5d 222e 666f 726d 6174 282a 2869 2069  }]".format(*(i i
-00009c40: 6620 6920 6973 206e 6f74 204e 6f6e 6520  f i is not None 
-00009c50: 656c 7365 2027 2720 666f 7220 6920 696e  else '' for i in
-00009c60: 2073 6c63 5f74 7570 6c65 2929 0a20 2020   slc_tuple)).   
-00009c70: 2020 2020 2020 2020 2020 2020 2073 6c63               slc
-00009c80: 203d 2073 6c69 6365 282a 736c 635f 7475   = slice(*slc_tu
-00009c90: 706c 6529 0a20 2020 2020 2020 2020 2020  ple).           
-00009ca0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00009cb0: 2020 2020 2020 206c 6162 656c 203d 2073         label = s
-00009cc0: 7472 2873 6c63 5f74 7570 6c65 290a 2020  tr(slc_tuple).  
-00009cd0: 2020 2020 2020 2020 2020 2020 2020 736c                sl
-00009ce0: 6320 3d20 736c 635f 7475 706c 650a 0a20  c = slc_tuple.. 
-00009cf0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00009d00: 7365 6c66 2e73 7562 5465 7374 286c 6162  self.subTest(lab
-00009d10: 656c 2c20 736c 635f 7475 706c 653d 736c  el, slc_tuple=sl
-00009d20: 635f 7475 706c 6529 3a0a 2020 2020 2020  c_tuple):.      
-00009d30: 2020 2020 2020 2020 2020 6465 6c20 636f            del co
-00009d40: 6d70 6172 655f 6c69 7374 5b73 6c63 5d0a  mpare_list[slc].
-00009d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d60: 7072 696e 7428 6c61 6265 6c29 0a20 2020  print(label).   
-00009d70: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00009d80: 6e74 2827 4578 7065 6374 6564 272c 2063  nt('Expected', c
-00009d90: 6f6d 7061 7265 5f6c 6973 7429 0a20 2020  ompare_list).   
-00009da0: 2020 2020 2020 2020 2020 2020 2064 656c               del
-00009db0: 2074 315b 736c 635d 0a20 2020 2020 2020   t1[slc].       
-00009dc0: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00009dd0: 4f62 7365 7276 6564 272c 206c 6973 7428  Observed', list(
-00009de0: 7431 2e61 6c6c 2e41 2929 0a20 2020 2020  t1.all.A)).     
-00009df0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00009e00: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00009e10: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00009e20: 7561 6c28 2727 2e6a 6f69 6e28 636f 6d70  ual(''.join(comp
-00009e30: 6172 655f 6c69 7374 292c 2027 272e 6a6f  are_list), ''.jo
-00009e40: 696e 2874 312e 616c 6c2e 4129 2c20 2266  in(t1.all.A), "f
-00009e50: 6169 6c65 6420 2220 2b20 6c61 6265 6c29  ailed " + label)
-00009e60: 0a0a 2020 2020 2020 2020 6d69 6e69 5f74  ..        mini_t
-00009e70: 6573 7428 3529 0a20 2020 2020 2020 206d  est(5).        m
-00009e80: 696e 695f 7465 7374 282d 3529 0a20 2020  ini_test(-5).   
-00009e90: 2020 2020 206d 696e 695f 7465 7374 2828       mini_test((
-00009ea0: 2d35 2c20 4e6f 6e65 2c20 4e6f 6e65 2929  -5, None, None))
-00009eb0: 0a20 2020 2020 2020 206d 696e 695f 7465  .        mini_te
-00009ec0: 7374 2828 4e6f 6e65 2c20 332c 204e 6f6e  st((None, 3, Non
-00009ed0: 6529 290a 2020 2020 2020 2020 6d69 6e69  e)).        mini
-00009ee0: 5f74 6573 7428 284e 6f6e 652c 202d 6c65  _test((None, -le
-00009ef0: 6e28 636f 6d70 6172 655f 6c69 7374 292b  n(compare_list)+
-00009f00: 332c 204e 6f6e 6529 290a 2020 2020 2020  3, None)).      
-00009f10: 2020 6d69 6e69 5f74 6573 7428 284e 6f6e    mini_test((Non
-00009f20: 652c 204e 6f6e 652c 2035 2929 0a20 2020  e, None, 5)).   
-00009f30: 2020 2020 206d 696e 695f 7465 7374 2828       mini_test((
-00009f40: 4e6f 6e65 2c20 4e6f 6e65 2c20 2d35 2929  None, None, -5))
-00009f50: 0a20 2020 2020 2020 206d 696e 695f 7465  .        mini_te
-00009f60: 7374 2828 2d35 2c20 2d32 2c20 4e6f 6e65  st((-5, -2, None
-00009f70: 2929 0a20 2020 2020 2020 206d 696e 695f  )).        mini_
-00009f80: 7465 7374 2828 2d32 2c20 2d35 2c20 2d31  test((-2, -5, -1
-00009f90: 2929 0a20 2020 2020 2020 206d 696e 695f  )).        mini_
-00009fa0: 7465 7374 2828 352c 2032 302c 2032 2929  test((5, 20, 2))
-00009fb0: 0a20 2020 2020 2020 206d 696e 695f 7465  .        mini_te
-00009fc0: 7374 2828 6c65 6e28 636f 6d70 6172 655f  st((len(compare_
-00009fd0: 6c69 7374 292c 2035 2c20 2d33 2929 0a20  list), 5, -3)). 
-00009fe0: 2020 2020 2020 206d 696e 695f 7465 7374         mini_test
-00009ff0: 2828 3230 2c20 3131 2c20 2d37 2929 0a20  ((20, 11, -7)). 
-0000a000: 2020 2020 2020 206d 696e 695f 7465 7374         mini_test
-0000a010: 2828 352c 2035 2c20 4e6f 6e65 2929 0a20  ((5, 5, None)). 
-0000a020: 2020 2020 2020 206d 696e 695f 7465 7374         mini_test
-0000a030: 2828 4e6f 6e65 2c20 2d31 302c 2035 2929  ((None, -10, 5))
-0000a040: 0a20 2020 2020 2020 206d 696e 695f 7465  .        mini_te
-0000a050: 7374 2828 4e6f 6e65 2c20 2d31 302c 202d  st((None, -10, -
-0000a060: 3130 2929 0a20 2020 2020 2020 206d 696e  10)).        min
-0000a070: 695f 7465 7374 2828 3130 3030 2c20 3230  i_test((1000, 20
-0000a080: 3030 2c20 4e6f 6e65 2929 0a20 2020 2020  00, None)).     
-0000a090: 2020 206d 696e 695f 7465 7374 2828 4e6f     mini_test((No
-0000a0a0: 6e65 2c20 4e6f 6e65 2c20 2d31 2929 0a0a  ne, None, -1))..
-0000a0b0: 2020 2020 6465 6620 7465 7374 5f63 6c65      def test_cle
-0000a0c0: 6172 2873 656c 6629 3a0a 2020 2020 2020  ar(self):.      
-0000a0d0: 2020 7365 6c66 2e5f 7465 7374 5f69 6e69    self._test_ini
-0000a0e0: 7428 290a 2020 2020 2020 2020 6e75 6d5f  t().        num_
-0000a0f0: 6669 656c 6473 203d 206c 656e 2873 656c  fields = len(sel
-0000a100: 662e 7431 2e69 6e66 6f28 295b 2266 6965  f.t1.info()["fie
-0000a110: 6c64 7322 5d29 0a20 2020 2020 2020 2077  lds"]).        w
-0000a120: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000a130: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000a140: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000a150: 2873 656c 662e 7465 7374 5f73 697a 6520  (self.test_size 
-0000a160: 2a2a 206e 756d 5f66 6965 6c64 732c 206c  ** num_fields, l
-0000a170: 656e 2873 656c 662e 7431 292c 2022 696e  en(self.t1), "in
-0000a180: 7661 6c69 6420 6c65 6e22 290a 2020 2020  valid len").    
-0000a190: 2020 2020 7365 6c66 2e74 312e 6372 6561      self.t1.crea
-0000a1a0: 7465 5f69 6e64 6578 2822 6122 290a 0a20  te_index("a").. 
-0000a1b0: 2020 2020 2020 2073 656c 662e 7431 2e63         self.t1.c
-0000a1c0: 6c65 6172 2829 0a20 2020 2020 2020 2077  lear().        w
-0000a1d0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000a1e0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000a1f0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000a200: 2830 2c20 6c65 6e28 7365 6c66 2e74 3129  (0, len(self.t1)
-0000a210: 2c20 2269 6e76 616c 6964 206c 656e 2061  , "invalid len a
-0000a220: 6674 6572 2063 6c65 6172 2229 0a20 2020  fter clear").   
-0000a230: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-0000a240: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
-0000a250: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000a260: 7445 7175 616c 2831 2c20 6c65 6e28 7365  tEqual(1, len(se
-0000a270: 6c66 2e74 312e 696e 666f 2829 5b22 696e  lf.t1.info()["in
-0000a280: 6465 7865 7322 5d29 2c20 2269 6e76 616c  dexes"]), "inval
-0000a290: 6964 2069 6e64 6578 6573 2061 6674 6572  id indexes after
-0000a2a0: 2063 6c65 6172 2229 0a0a 2020 2020 6465   clear")..    de
-0000a2b0: 6620 7465 7374 5f73 7461 7473 2873 656c  f test_stats(sel
-0000a2c0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-0000a2d0: 2e5f 7465 7374 5f69 6e69 7428 290a 2020  ._test_init().  
-0000a2e0: 2020 2020 2020 6669 656c 645f 6e61 6d65        field_name
-0000a2f0: 7320 3d20 7365 6c66 2e74 312e 696e 666f  s = self.t1.info
-0000a300: 2829 5b22 6669 656c 6473 225d 0a20 2020  ()["fields"].   
-0000a310: 2020 2020 206e 756d 5f66 6965 6c64 7320       num_fields 
-0000a320: 3d20 6c65 6e28 6669 656c 645f 6e61 6d65  = len(field_name
-0000a330: 7329 0a20 2020 2020 2020 2074 315f 7374  s).        t1_st
-0000a340: 6174 7320 3d20 7365 6c66 2e74 312e 7374  ats = self.t1.st
-0000a350: 6174 7328 292e 7365 6c65 6374 2822 6e61  ats().select("na
-0000a360: 6d65 2063 6f75 6e74 206d 696e 206d 6178  me count min max
-0000a370: 206d 6561 6e22 290a 2020 2020 2020 2020   mean").        
-0000a380: 666f 7220 6669 656c 646e 616d 6520 696e  for fieldname in
-0000a390: 2066 6965 6c64 5f6e 616d 6573 3a0a 2020   field_names:.  
-0000a3a0: 2020 2020 2020 2020 2020 7374 6174 5f72            stat_r
-0000a3b0: 6563 203d 2074 315f 7374 6174 732e 6279  ec = t1_stats.by
-0000a3c0: 2e6e 616d 655b 6669 656c 646e 616d 655d  .name[fieldname]
-0000a3d0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-0000a3e0: 6820 7365 6c66 2e73 7562 5465 7374 2822  h self.subTest("
-0000a3f0: 6368 6563 6b20 636f 6d70 7574 6564 2073  check computed s
-0000a400: 7461 7422 2c20 6669 656c 646e 616d 653d  tat", fieldname=
-0000a410: 6669 656c 646e 616d 6529 3a0a 2020 2020  fieldname):.    
-0000a420: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a430: 2e61 7373 6572 7445 7175 616c 286c 742e  .assertEqual(lt.
-0000a440: 4461 7461 4f62 6a65 6374 286e 616d 653d  DataObject(name=
-0000a450: 6669 656c 646e 616d 652c 0a20 2020 2020  fieldname,.     
-0000a460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a480: 2020 2020 2020 2020 2020 636f 756e 743d            count=
-0000a490: 7365 6c66 2e74 6573 745f 7369 7a65 202a  self.test_size *
-0000a4a0: 2a20 6e75 6d5f 6669 656c 6473 2c0a 2020  * num_fields,.  
-0000a4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4d0: 2020 2020 2020 2020 2020 2020 206d 696e               min
-0000a4e0: 3d30 2c0a 2020 2020 2020 2020 2020 2020  =0,.            
-0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a510: 2020 206d 6178 3d73 656c 662e 7465 7374     max=self.test
-0000a520: 5f73 697a 6520 2d20 312c 0a20 2020 2020  _size - 1,.     
-0000a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a550: 2020 2020 2020 2020 2020 6d65 616e 3d28            mean=(
-0000a560: 7365 6c66 2e74 6573 745f 7369 7a65 202d  self.test_size -
-0000a570: 2031 2920 2f20 3229 2c0a 2020 2020 2020   1) / 2),.      
-0000a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a590: 2020 2020 2020 2020 2020 2073 7461 745f             stat_
-0000a5a0: 7265 632c 0a20 2020 2020 2020 2020 2020  rec,.           
-0000a5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5c0: 2020 2020 2020 6622 696e 7661 6c69 6420        f"invalid 
-0000a5d0: 7374 6174 2066 6f72 207b 6669 656c 646e  stat for {fieldn
-0000a5e0: 616d 657d 2229 0a0a 2020 2020 6465 6620  ame}")..    def 
-0000a5f0: 7465 7374 5f73 7461 7473 3228 7365 6c66  test_stats2(self
-0000a600: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0000a610: 5f74 6573 745f 696e 6974 2829 0a20 2020  _test_init().   
-0000a620: 2020 2020 2066 6965 6c64 5f6e 616d 6573       field_names
-0000a630: 203d 2073 656c 662e 7431 2e69 6e66 6f28   = self.t1.info(
-0000a640: 295b 2266 6965 6c64 7322 5d0a 2020 2020  )["fields"].    
-0000a650: 2020 2020 6e75 6d5f 6669 656c 6473 203d      num_fields =
-0000a660: 206c 656e 2866 6965 6c64 5f6e 616d 6573   len(field_names
-0000a670: 290a 2020 2020 2020 2020 7431 5f73 7461  ).        t1_sta
-0000a680: 7473 203d 2073 656c 662e 7431 2e73 7461  ts = self.t1.sta
-0000a690: 7473 2862 795f 6669 656c 643d 4661 6c73  ts(by_field=Fals
-0000a6a0: 6529 0a20 2020 2020 2020 2066 6f72 2073  e).        for s
-0000a6b0: 7461 742c 2076 616c 7565 2069 6e20 2828  tat, value in ((
-0000a6c0: 276d 696e 272c 2030 292c 2028 276d 6178  'min', 0), ('max
-0000a6d0: 272c 2073 656c 662e 7465 7374 5f73 697a  ', self.test_siz
-0000a6e0: 6520 2d20 3129 2c20 2827 636f 756e 7427  e - 1), ('count'
-0000a6f0: 2c20 7365 6c66 2e74 6573 745f 7369 7a65  , self.test_size
-0000a700: 202a 2a20 6e75 6d5f 6669 656c 6473 292c   ** num_fields),
-0000a710: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
-0000a720: 6f72 2066 6965 6c64 6e61 6d65 2069 6e20  or fieldname in 
-0000a730: 6669 656c 645f 6e61 6d65 733a 0a20 2020  field_names:.   
-0000a740: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-0000a750: 6820 7365 6c66 2e73 7562 5465 7374 2822  h self.subTest("
-0000a760: 6368 6563 6b20 636f 6d70 7574 6564 2073  check computed s
-0000a770: 7461 7422 2c20 7374 6174 3d73 7461 742c  tat", stat=stat,
-0000a780: 2066 6965 6c64 6e61 6d65 3d66 6965 6c64   fieldname=field
-0000a790: 6e61 6d65 293a 0a20 2020 2020 2020 2020  name):.         
-0000a7a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a7b0: 6173 7365 7274 4571 7561 6c28 7661 6c75  assertEqual(valu
-0000a7c0: 652c 2067 6574 6174 7472 2874 315f 7374  e, getattr(t1_st
-0000a7d0: 6174 732e 6279 2e73 7461 745b 7374 6174  ats.by.stat[stat
-0000a7e0: 5d2c 2066 6965 6c64 6e61 6d65 292c 0a20  ], fieldname),. 
-0000a7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a810: 6622 696e 7661 6c69 6420 7b73 7461 747d  f"invalid {stat}
-0000a820: 2073 7461 7420 666f 7220 7b66 6965 6c64   stat for {field
-0000a830: 6e61 6d65 7d22 290a 0a20 2020 2064 6566  name}")..    def
-0000a840: 2074 6573 745f 7374 6174 7333 2873 656c   test_stats3(sel
-0000a850: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-0000a860: 2e5f 7465 7374 5f69 6e69 7428 290a 2020  ._test_init().  
-0000a870: 2020 2020 2020 6669 656c 645f 6e61 6d65        field_name
-0000a880: 7320 3d20 7365 6c66 2e74 312e 696e 666f  s = self.t1.info
-0000a890: 2829 5b22 6669 656c 6473 225d 0a20 2020  ()["fields"].   
-0000a8a0: 2020 2020 206e 756d 5f66 6965 6c64 7320       num_fields 
-0000a8b0: 3d20 6c65 6e28 6669 656c 645f 6e61 6d65  = len(field_name
-0000a8c0: 7329 0a0a 2020 2020 2020 2020 2320 7665  s)..        # ve
-0000a8d0: 7269 6679 2074 6861 7420 7374 6174 7320  rify that stats 
-0000a8e0: 6361 6e20 2273 7465 7020 6f76 6572 2220  can "step over" 
-0000a8f0: 6e6f 6e2d 6e75 6d65 7269 6320 6461 7461  non-numeric data
-0000a900: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-0000a910: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-0000a920: 315b 305d 2e61 203d 2022 6e6f 7420 6120  1[0].a = "not a 
-0000a930: 6e75 6d62 6572 220a 2020 2020 2020 2020  number".        
-0000a940: 6578 6365 7074 2028 4174 7472 6962 7574  except (Attribut
-0000a950: 6545 7272 6f72 2c20 5479 7065 4572 726f  eError, TypeErro
-0000a960: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-0000a970: 2320 736f 6d65 2074 6573 7420 7479 7065  # some test type
-0000a980: 7320 6172 656e 2774 206d 7574 6162 6c65  s aren't mutable
-0000a990: 2c20 6d75 7374 2072 6570 6c61 6365 2072  , must replace r
-0000a9a0: 6563 2077 6974 6820 6120 6d6f 6469 6669  ec with a modifi
-0000a9b0: 6564 206f 6e65 0a20 2020 2020 2020 2020  ed one.         
-0000a9c0: 2020 206d 6f64 5f72 6563 203d 2073 656c     mod_rec = sel
-0000a9d0: 662e 7431 2e70 6f70 2830 290a 2020 2020  f.t1.pop(0).    
-0000a9e0: 2020 2020 2020 2020 7265 635f 7479 7065          rec_type
-0000a9f0: 203d 2074 7970 6528 6d6f 645f 7265 6329   = type(mod_rec)
-0000aa00: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
-0000aa10: 5f72 6563 5f64 6963 7420 3d20 6c74 2e5f  _rec_dict = lt._
-0000aa20: 746f 5f64 6963 7428 6d6f 645f 7265 6329  to_dict(mod_rec)
-0000aa30: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
-0000aa40: 5f72 6563 5f64 6963 745b 2761 275d 203d  _rec_dict['a'] =
-0000aa50: 2022 6e6f 7420 6120 6e75 6d62 6572 220a   "not a number".
-0000aa60: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0000aa70: 7265 6320 3d20 7265 635f 7479 7065 282a  rec = rec_type(*
-0000aa80: 2a6e 6577 5f72 6563 5f64 6963 7429 0a20  *new_rec_dict). 
-0000aa90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000aaa0: 7431 2e69 6e73 6572 7428 6e65 775f 7265  t1.insert(new_re
-0000aab0: 6329 0a0a 2020 2020 2020 2020 7431 5f73  c)..        t1_s
-0000aac0: 7461 7473 203d 2073 656c 662e 7431 2e73  tats = self.t1.s
-0000aad0: 7461 7473 2829 0a20 2020 2020 2020 2074  tats().        t
-0000aae0: 315f 7374 6174 7328 2274 315f 7374 6174  1_stats("t1_stat
-0000aaf0: 7322 290a 2020 2020 2020 2020 7431 5f73  s").        t1_s
-0000ab00: 7461 7473 2e63 7376 5f65 7870 6f72 7428  tats.csv_export(
-0000ab10: 7379 732e 7374 646f 7574 290a 2020 2020  sys.stdout).    
-0000ab20: 2020 2020 7431 5f73 7461 7473 2e70 7265      t1_stats.pre
-0000ab30: 7365 6e74 2829 0a20 2020 2020 2020 2073  sent().        s
-0000ab40: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000ab50: 7365 6c66 2e74 6573 745f 7369 7a65 202a  self.test_size *
-0000ab60: 2a20 6e75 6d5f 6669 656c 6473 202d 2031  * num_fields - 1
-0000ab70: 2c20 7431 5f73 7461 7473 2e62 792e 6e61  , t1_stats.by.na
-0000ab80: 6d65 5b22 6122 5d2e 636f 756e 7429 0a0a  me["a"].count)..
-0000ab90: 2020 2020 6465 6620 7465 7374 5f73 7461      def test_sta
-0000aba0: 7473 3428 7365 6c66 293a 0a20 2020 2020  ts4(self):.     
-0000abb0: 2020 2074 3120 3d20 6c74 2e54 6162 6c65     t1 = lt.Table
-0000abc0: 2829 2e63 7376 5f69 6d70 6f72 7428 7465  ().csv_import(te
-0000abd0: 7874 7772 6170 2e64 6564 656e 7428 2222  xtwrap.dedent(""
-0000abe0: 225c 0a20 2020 2020 2020 2061 2c62 0a20  "\.        a,b. 
-0000abf0: 2020 2020 2020 2031 2c32 0a20 2020 2020         1,2.     
-0000ac00: 2020 2033 2c0a 2020 2020 2020 2020 352c     3,.        5,
-0000ac10: 340a 2020 2020 2020 2020 2222 2229 2c20  4.        """), 
-0000ac20: 7472 616e 7366 6f72 6d73 3d7b 7d2e 6672  transforms={}.fr
-0000ac30: 6f6d 6b65 7973 285b 2261 222c 2022 6222  omkeys(["a", "b"
-0000ac40: 5d2c 2069 6e74 2929 0a20 2020 2020 2020  ], int)).       
-0000ac50: 2074 315f 7374 6174 7320 3d20 7431 2e73   t1_stats = t1.s
-0000ac60: 7461 7473 2829 0a20 2020 2020 2020 2074  tats().        t
-0000ac70: 315f 7374 6174 732e 7072 6573 656e 7428  1_stats.present(
-0000ac80: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-0000ac90: 7431 5f73 7461 7473 2e69 6e66 6f28 2929  t1_stats.info())
-0000aca0: 0a0a 2020 2020 2020 2020 6578 7065 6374  ..        expect
-0000acb0: 6564 203d 206c 742e 5461 626c 6528 292e  ed = lt.Table().
-0000acc0: 6373 765f 696d 706f 7274 2874 6578 7477  csv_import(textw
-0000acd0: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
-0000ace0: 2020 2020 2020 2020 6e61 6d65 2c6d 6561          name,mea
-0000acf0: 6e2c 6d69 6e2c 6d61 782c 7661 7269 616e  n,min,max,varian
-0000ad00: 6365 2c73 7464 5f64 6576 2c63 6f75 6e74  ce,std_dev,count
-0000ad10: 2c6d 6973 7369 6e67 0a20 2020 2020 2020  ,missing.       
-0000ad20: 2061 2c33 2e30 2c31 2c35 2c34 2c32 2e30   a,3.0,1,5,4,2.0
-0000ad30: 2c33 2c30 0a20 2020 2020 2020 2062 2c33  ,3,0.        b,3
-0000ad40: 2e30 2c32 2c34 2c32 2c31 2e34 3134 2c32  .0,2,4,2,1.414,2
-0000ad50: 2c31 0a20 2020 2020 2020 2022 2222 292c  ,1.        """),
-0000ad60: 2074 7261 6e73 666f 726d 733d 7b7d 2e66   transforms={}.f
-0000ad70: 726f 6d6b 6579 7328 226d 6561 6e20 6d69  romkeys("mean mi
-0000ad80: 6e20 6d61 7820 7661 7269 616e 6365 2073  n max variance s
-0000ad90: 7464 5f64 6576 2063 6f75 6e74 206d 6973  td_dev count mis
-0000ada0: 7369 6e67 222e 7370 6c69 7428 292c 2061  sing".split(), a
-0000adb0: 7374 2e6c 6974 6572 616c 5f65 7661 6c29  st.literal_eval)
-0000adc0: 290a 2020 2020 2020 2020 6578 7065 6374  ).        expect
-0000add0: 6564 2e70 7265 7365 6e74 2829 0a20 2020  ed.present().   
-0000ade0: 2020 2020 2070 7269 6e74 2865 7870 6563       print(expec
-0000adf0: 7465 642e 696e 666f 2829 290a 0a20 2020  ted.info())..   
-0000ae00: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-0000ae10: 7562 5465 7374 2822 6368 6563 6b20 636f  ubTest("check co
-0000ae20: 6d70 7574 6564 2073 7461 7420 6669 656c  mputed stat fiel
-0000ae30: 6473 2229 3a0a 2020 2020 2020 2020 2020  ds"):.          
-0000ae40: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0000ae50: 616c 2865 7870 6563 7465 642e 696e 666f  al(expected.info
-0000ae60: 2829 5b22 6669 656c 6473 225d 2c20 7431  ()["fields"], t1
-0000ae70: 5f73 7461 7473 2e69 6e66 6f28 295b 2266  _stats.info()["f
-0000ae80: 6965 6c64 7322 5d29 0a0a 2020 2020 2020  ields"])..      
-0000ae90: 2020 666f 7220 6578 7065 6374 6564 5f72    for expected_r
-0000aea0: 6f77 2c20 726f 7720 696e 207a 6970 2865  ow, row in zip(e
-0000aeb0: 7870 6563 7465 642c 2074 315f 7374 6174  xpected, t1_stat
-0000aec0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0000aed0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-0000aee0: 7428 2263 6865 636b 2063 6f6d 7075 7465  t("check compute
-0000aef0: 6420 7374 6174 2061 7474 7269 6275 7465  d stat attribute
-0000af00: 2028 6e61 6d65 2922 2c20 726f 773d 726f   (name)", row=ro
-0000af10: 7729 3a0a 2020 2020 2020 2020 2020 2020  w):.            
-0000af20: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000af30: 7175 616c 2865 7870 6563 7465 645f 726f  qual(expected_ro
-0000af40: 772e 6e61 6d65 2c20 726f 772e 6e61 6d65  w.name, row.name
-0000af50: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
-0000af60: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-0000af70: 2263 6865 636b 2063 6f6d 7075 7465 6420  "check computed 
-0000af80: 7374 6174 2061 7474 7269 6275 7465 2028  stat attribute (
-0000af90: 6d65 616e 2922 2c20 726f 773d 726f 7729  mean)", row=row)
-0000afa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000afb0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0000afc0: 616c 2865 7870 6563 7465 645f 726f 772e  al(expected_row.
-0000afd0: 6d65 616e 2c20 726f 772e 6d65 616e 290a  mean, row.mean).
-0000afe0: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000aff0: 2073 656c 662e 7375 6254 6573 7428 2263   self.subTest("c
-0000b000: 6865 636b 2063 6f6d 7075 7465 6420 7374  heck computed st
-0000b010: 6174 2061 7474 7269 6275 7465 2028 6d69  at attribute (mi
-0000b020: 6e29 222c 2072 6f77 3d72 6f77 293a 0a20  n)", row=row):. 
-0000b030: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000b040: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000b050: 6578 7065 6374 6564 5f72 6f77 2e6d 696e  expected_row.min
-0000b060: 2c20 726f 772e 6d69 6e29 0a20 2020 2020  , row.min).     
-0000b070: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0000b080: 2e73 7562 5465 7374 2822 6368 6563 6b20  .subTest("check 
-0000b090: 636f 6d70 7574 6564 2073 7461 7420 6174  computed stat at
-0000b0a0: 7472 6962 7574 6520 286d 6178 2922 2c20  tribute (max)", 
-0000b0b0: 726f 773d 726f 7729 3a0a 2020 2020 2020  row=row):.      
-0000b0c0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000b0d0: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
-0000b0e0: 7465 645f 726f 772e 6d61 782c 2072 6f77  ted_row.max, row
-0000b0f0: 2e6d 6178 290a 2020 2020 2020 2020 2020  .max).          
-0000b100: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-0000b110: 6573 7428 2263 6865 636b 2063 6f6d 7075  est("check compu
-0000b120: 7465 6420 7374 6174 2061 7474 7269 6275  ted stat attribu
-0000b130: 7465 2028 7661 7269 616e 6365 2922 2c20  te (variance)", 
-0000b140: 726f 773d 726f 7729 3a0a 2020 2020 2020  row=row):.      
-0000b150: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000b160: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
-0000b170: 7465 645f 726f 772e 7661 7269 616e 6365  ted_row.variance
-0000b180: 2c20 726f 772e 7661 7269 616e 6365 290a  , row.variance).
-0000b190: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000b1a0: 2073 656c 662e 7375 6254 6573 7428 2263   self.subTest("c
-0000b1b0: 6865 636b 2063 6f6d 7075 7465 6420 7374  heck computed st
-0000b1c0: 6174 2061 7474 7269 6275 7465 2028 7374  at attribute (st
-0000b1d0: 645f 6465 7629 222c 2072 6f77 3d72 6f77  d_dev)", row=row
-0000b1e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000b1f0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000b200: 7561 6c28 6578 7065 6374 6564 5f72 6f77  ual(expected_row
-0000b210: 2e73 7464 5f64 6576 2c20 726f 772e 7374  .std_dev, row.st
-0000b220: 645f 6465 7629 0a20 2020 2020 2020 2020  d_dev).         
-0000b230: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-0000b240: 5465 7374 2822 6368 6563 6b20 636f 6d70  Test("check comp
-0000b250: 7574 6564 2073 7461 7420 6174 7472 6962  uted stat attrib
-0000b260: 7574 6520 2863 6f75 6e74 2922 2c20 726f  ute (count)", ro
-0000b270: 773d 726f 7729 3a0a 2020 2020 2020 2020  w=row):.        
-0000b280: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0000b290: 6572 7445 7175 616c 2865 7870 6563 7465  ertEqual(expecte
-0000b2a0: 645f 726f 772e 636f 756e 742c 2072 6f77  d_row.count, row
-0000b2b0: 2e63 6f75 6e74 290a 2020 2020 2020 2020  .count).        
-0000b2c0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-0000b2d0: 6254 6573 7428 2263 6865 636b 2063 6f6d  bTest("check com
-0000b2e0: 7075 7465 6420 7374 6174 2061 7474 7269  puted stat attri
-0000b2f0: 6275 7465 2028 6d69 7373 696e 6729 222c  bute (missing)",
-0000b300: 2072 6f77 3d72 6f77 293a 0a20 2020 2020   row=row):.     
-0000b310: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b320: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
-0000b330: 6374 6564 5f72 6f77 2e6d 6973 7369 6e67  cted_row.missing
-0000b340: 2c20 726f 772e 6d69 7373 696e 6729 0a0a  , row.missing)..
-0000b350: 2020 2020 6465 6620 7465 7374 5f73 706c      def test_spl
-0000b360: 6974 6279 2873 656c 6629 3a0a 2020 2020  itby(self):.    
-0000b370: 2020 2020 7365 6c66 2e5f 7465 7374 5f69      self._test_i
-0000b380: 6e69 7428 290a 2020 2020 2020 2020 6973  nit().        is
-0000b390: 5f6f 6464 203d 206c 616d 6264 6120 7265  _odd = lambda re
-0000b3a0: 633a 2072 6563 2e61 2025 2032 0a20 2020  c: rec.a % 2.   
-0000b3b0: 2020 2020 2065 7665 6e73 2c20 6f64 6473       evens, odds
-0000b3c0: 203d 2073 656c 662e 7431 2e73 706c 6974   = self.t1.split
-0000b3d0: 6279 2869 735f 6f64 6429 0a20 2020 2020  by(is_odd).     
-0000b3e0: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-0000b3f0: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-0000b400: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000b410: 7175 616c 286c 656e 286f 6464 7329 202b  qual(len(odds) +
-0000b420: 206c 656e 2865 7665 6e73 292c 206c 656e   len(evens), len
-0000b430: 2873 656c 662e 7431 2929 0a20 2020 2020  (self.t1)).     
-0000b440: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-0000b450: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-0000b460: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000b470: 7175 616c 286c 656e 286f 6464 7329 2c20  qual(len(odds), 
-0000b480: 6c65 6e28 7365 6c66 2e74 312e 7768 6572  len(self.t1.wher
-0000b490: 6528 6973 5f6f 6464 2929 290a 0a20 2020  e(is_odd)))..   
-0000b4a0: 2020 2020 2065 7665 6e5f 6576 656e 732c       even_evens,
-0000b4b0: 206f 6464 5f65 7665 6e73 203d 2065 7665   odd_evens = eve
-0000b4c0: 6e73 2e73 706c 6974 6279 2869 735f 6f64  ns.splitby(is_od
-0000b4d0: 6429 0a20 2020 2020 2020 2077 6974 6820  d).        with 
-0000b4e0: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
-0000b4f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b500: 2e61 7373 6572 7445 7175 616c 2830 2c20  .assertEqual(0, 
-0000b510: 6c65 6e28 6f64 645f 6576 656e 7329 290a  len(odd_evens)).
-0000b520: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0000b530: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-0000b540: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0000b550: 7365 7274 4571 7561 6c28 6c65 6e28 6576  sertEqual(len(ev
-0000b560: 656e 5f65 7665 6e73 292c 206c 656e 2865  en_evens), len(e
-0000b570: 7665 6e73 2929 0a0a 2020 2020 2020 2020  vens))..        
-0000b580: 2320 6d61 6b65 2073 7572 6520 696e 6465  # make sure inde
-0000b590: 7865 7320 6172 6520 7072 6573 6572 7665  xes are preserve
-0000b5a0: 640a 2020 2020 2020 2020 7365 6c66 2e74  d.        self.t
-0000b5b0: 312e 6372 6561 7465 5f69 6e64 6578 2822  1.create_index("
-0000b5c0: 6122 290a 2020 2020 2020 2020 6576 656e  a").        even
-0000b5d0: 732c 206f 6464 7320 3d20 7365 6c66 2e74  s, odds = self.t
-0000b5e0: 312e 7370 6c69 7462 7928 6973 5f6f 6464  1.splitby(is_odd
-0000b5f0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
-0000b600: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-0000b610: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b620: 6173 7365 7274 4571 7561 6c28 7365 6c66  assertEqual(self
-0000b630: 2e74 312e 696e 666f 2829 5b22 696e 6465  .t1.info()["inde
-0000b640: 7865 7322 5d2c 2065 7665 6e73 2e69 6e66  xes"], evens.inf
-0000b650: 6f28 295b 2269 6e64 6578 6573 225d 290a  o()["indexes"]).
-0000b660: 0a20 2020 2020 2020 2023 2074 6573 7420  .        # test 
-0000b670: 7061 7373 696e 6720 616e 2061 7474 7269  passing an attri
-0000b680: 6275 7465 2061 7320 6120 6b65 790a 2020  bute as a key.  
-0000b690: 2020 2020 2020 7a65 726f 732c 206e 6f6e        zeros, non
-0000b6a0: 5f7a 6572 6f73 203d 2073 656c 662e 7431  _zeros = self.t1
-0000b6b0: 2e73 706c 6974 6279 2822 6122 290a 2020  .splitby("a").  
-0000b6c0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0000b6d0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-0000b6e0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000b6f0: 7274 5472 7565 2861 6c6c 2872 6563 2e61  rtTrue(all(rec.a
-0000b700: 203d 3d20 3020 666f 7220 7265 6320 696e   == 0 for rec in
-0000b710: 207a 6572 6f73 2929 0a20 2020 2020 2020   zeros)).       
-0000b720: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-0000b730: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-0000b740: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
-0000b750: 6528 616c 6c28 7265 632e 6120 213d 2030  e(all(rec.a != 0
-0000b760: 2066 6f72 2072 6563 2069 6e20 6e6f 6e5f   for rec in non_
-0000b770: 7a65 726f 7329 290a 0a20 2020 2020 2020  zeros))..       
-0000b780: 2023 2074 6573 7420 7573 696e 6720 7072   # test using pr
-0000b790: 6564 6963 6174 6520 7468 6174 2064 6f65  edicate that doe
-0000b7a0: 7320 6e6f 7420 616c 7761 7973 2072 6574  s not always ret
-0000b7b0: 7572 6e20 3020 6f72 2031 0a20 2020 2020  urn 0 or 1.     
-0000b7c0: 2020 2069 735f 6e6f 745f 6d75 6c74 6970     is_not_multip
-0000b7d0: 6c65 5f6f 665f 3320 3d20 6c61 6d62 6461  le_of_3 = lambda
-0000b7e0: 2072 6563 3a20 7265 632e 6120 2520 330a   rec: rec.a % 3.
-0000b7f0: 2020 2020 2020 2020 6d75 6c74 735f 6f66          mults_of
-0000b800: 5f33 2c20 6e6f 6e5f 6d75 6c74 735f 6f66  _3, non_mults_of
-0000b810: 5f33 203d 2073 656c 662e 7431 2e73 706c  _3 = self.t1.spl
-0000b820: 6974 6279 2869 735f 6e6f 745f 6d75 6c74  itby(is_not_mult
-0000b830: 6970 6c65 5f6f 665f 3329 0a20 2020 2020  iple_of_3).     
-0000b840: 2020 2070 7269 6e74 286c 6973 7428 6e6f     print(list(no
-0000b850: 6e5f 6d75 6c74 735f 6f66 5f33 2e61 6c6c  n_mults_of_3.all
-0000b860: 2e61 2929 0a20 2020 2020 2020 2070 7269  .a)).        pri
-0000b870: 6e74 286c 6973 7428 6d75 6c74 735f 6f66  nt(list(mults_of
-0000b880: 5f33 2e61 6c6c 2e61 2929 0a20 2020 2020  _3.all.a)).     
-0000b890: 2020 2023 2054 4f44 4f20 2d20 6164 6420     # TODO - add 
-0000b8a0: 6173 7365 7274 7320 6865 7265 0a0a 0a40  asserts here...@
-0000b8b0: 6d61 6b65 5f74 6573 745f 636c 6173 7365  make_test_classe
-0000b8c0: 730a 636c 6173 7320 5461 626c 654a 6f69  s.class TableJoi
-0000b8d0: 6e54 6573 7473 3a0a 2020 2020 6465 6620  nTests:.    def 
-0000b8e0: 7465 7374 5f73 696d 706c 655f 6a6f 696e  test_simple_join
-0000b8f0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000b900: 7465 7374 5f73 697a 6520 3d20 3130 0a20  test_size = 10. 
-0000b910: 2020 2020 2020 2074 3120 3d20 6d61 6b65         t1 = make
-0000b920: 5f74 6573 745f 7461 626c 6528 7365 6c66  _test_table(self
-0000b930: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
-0000b940: 742c 2074 6573 745f 7369 7a65 290a 2020  t, test_size).  
-0000b950: 2020 2020 2020 7431 2e63 7265 6174 655f        t1.create_
-0000b960: 696e 6465 7828 2761 2729 0a0a 2020 2020  index('a')..    
-0000b970: 2020 2020 7432 203d 206c 742e 5461 626c      t2 = lt.Tabl
-0000b980: 6528 290a 2020 2020 2020 2020 7432 2e63  e().        t2.c
-0000b990: 7265 6174 655f 696e 6465 7828 2761 2729  reate_index('a')
-0000b9a0: 0a20 2020 2020 2020 2074 322e 696e 7365  .        t2.inse
-0000b9b0: 7274 286c 742e 4461 7461 4f62 6a65 6374  rt(lt.DataObject
-0000b9c0: 2861 3d31 2c20 643d 3130 3029 290a 0a20  (a=1, d=100)).. 
-0000b9d0: 2020 2020 2020 206a 6f69 6e65 6420 3d20         joined = 
-0000b9e0: 2874 312e 6a6f 696e 5f6f 6e28 2761 2729  (t1.join_on('a')
-0000b9f0: 202b 2074 322e 6a6f 696e 5f6f 6e28 2761   + t2.join_on('a
-0000ba00: 2729 2928 290a 2020 2020 2020 2020 7769  '))().        wi
-0000ba10: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-0000ba20: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000ba30: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000ba40: 7465 7374 5f73 697a 6520 2a20 7465 7374  test_size * test
-0000ba50: 5f73 697a 652c 206c 656e 286a 6f69 6e65  _size, len(joine
-0000ba60: 6429 290a 0a20 2020 2020 2020 206a 6f69  d))..        joi
-0000ba70: 6e65 6420 3d20 2874 312e 6a6f 696e 5f6f  ned = (t1.join_o
-0000ba80: 6e28 2761 2729 202b 2074 3229 2829 0a20  n('a') + t2)(). 
-0000ba90: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0000baa0: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-0000bab0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0000bac0: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
-0000bad0: 7a65 202a 2074 6573 745f 7369 7a65 2c20  ze * test_size, 
-0000bae0: 6c65 6e28 6a6f 696e 6564 2929 0a0a 2020  len(joined))..  
-0000baf0: 2020 2020 2020 6a6f 696e 6564 203d 2028        joined = (
-0000bb00: 7431 202b 2074 322e 6a6f 696e 5f6f 6e28  t1 + t2.join_on(
-0000bb10: 2761 2729 2928 290a 2020 2020 2020 2020  'a'))().        
-0000bb20: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-0000bb30: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-0000bb40: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0000bb50: 6c28 7465 7374 5f73 697a 6520 2a20 7465  l(test_size * te
-0000bb60: 7374 5f73 697a 652c 206c 656e 286a 6f69  st_size, len(joi
-0000bb70: 6e65 6429 290a 0a20 2020 2020 2020 2074  ned))..        t
-0000bb80: 312e 6465 6c65 7465 5f69 6e64 6578 2827  1.delete_index('
-0000bb90: 6127 290a 2020 2020 2020 2020 7769 7468  a').        with
-0000bba0: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-0000bbb0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-0000bbc0: 6820 7365 6c66 2e61 7373 6572 7452 6169  h self.assertRai
-0000bbd0: 7365 7328 5661 6c75 6545 7272 6f72 293a  ses(ValueError):
-0000bbe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bbf0: 206a 6f69 6e65 6420 3d20 2874 3120 2b20   joined = (t1 + 
-0000bc00: 7432 2e6a 6f69 6e5f 6f6e 2827 6127 2929  t2.join_on('a'))
-0000bc10: 2829 0a0a 2020 2020 2020 2020 7769 7468  ()..        with
-0000bc20: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-0000bc30: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-0000bc40: 6820 7365 6c66 2e61 7373 6572 7452 6169  h self.assertRai
-0000bc50: 7365 7328 5479 7065 4572 726f 7229 3a0a  ses(TypeError):.
-0000bc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc70: 2320 696e 7661 6c69 6420 6a6f 696e 2c20  # invalid join, 
-0000bc80: 6e6f 206b 7761 7267 7320 6c69 7374 696e  no kwargs listin
-0000bc90: 6720 6174 7472 6962 7574 6573 2074 6f20  g attributes to 
-0000bca0: 6a6f 696e 206f 6e0a 2020 2020 2020 2020  join on.        
-0000bcb0: 2020 2020 2020 2020 7433 203d 2074 312e          t3 = t1.
-0000bcc0: 6a6f 696e 2874 322c 2027 612c 6427 290a  join(t2, 'a,d').
-0000bcd0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000bce0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-0000bcf0: 2020 2020 2020 2020 2020 7769 7468 2073            with s
-0000bd00: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
-0000bd10: 2856 616c 7565 4572 726f 7229 3a0a 2020  (ValueError):.  
-0000bd20: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000bd30: 696e 7661 6c69 6420 6a6f 696e 2c20 6e6f  invalid join, no
-0000bd40: 2073 7563 6820 6174 7472 6962 7574 6520   such attribute 
-0000bd50: 277a 270a 2020 2020 2020 2020 2020 2020  'z'.            
-0000bd60: 2020 2020 7433 203d 2074 312e 6a6f 696e      t3 = t1.join
-0000bd70: 2874 322c 2027 612c 642c 7a27 2c20 613d  (t2, 'a,d,z', a=
-0000bd80: 2761 2729 0a0a 2020 2020 2020 2020 7433  'a')..        t3
-0000bd90: 203d 2074 312e 6a6f 696e 2874 322c 2027   = t1.join(t2, '
-0000bda0: 612c 6427 2c20 613d 2761 2729 0a20 2020  a,d', a='a').   
-0000bdb0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-0000bdc0: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
-0000bdd0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000bde0: 7445 7175 616c 2874 6573 745f 7369 7a65  tEqual(test_size
-0000bdf0: 202a 2074 6573 745f 7369 7a65 2c20 6c65   * test_size, le
-0000be00: 6e28 7433 2929 0a0a 2020 2020 2020 2020  n(t3))..        
-0000be10: 7434 203d 2074 312e 6a6f 696e 2874 322c  t4 = t1.join(t2,
-0000be20: 2061 3d27 6127 292e 7365 6c65 6374 2827   a='a').select('
-0000be30: 6120 6320 6427 2c20 653d 6c61 6d62 6461  a c d', e=lambda
-0000be40: 2072 6563 3a20 7265 632e 6120 2b20 7265   rec: rec.a + re
-0000be50: 632e 6320 2b20 7265 632e 6429 0a20 2020  c.c + rec.d).   
-0000be60: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-0000be70: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
-0000be80: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000be90: 7454 7275 6528 616c 6c28 7265 632e 6520  tTrue(all(rec.e 
-0000bea0: 3d3d 2072 6563 2e61 2b72 6563 2e63 2b72  == rec.a+rec.c+r
-0000beb0: 6563 2e64 2066 6f72 2072 6563 2069 6e20  ec.d for rec in 
-0000bec0: 7434 2929 0a0a 2020 2020 2020 2020 2320  t4))..        # 
-0000bed0: 6a6f 696e 2074 6f20 656d 7074 7920 6c69  join to empty li
-0000bee0: 7374 2c20 7368 6f75 6c64 2072 6574 7572  st, should retur
-0000bef0: 6e20 656d 7074 7920 7461 626c 650a 2020  n empty table.  
-0000bf00: 2020 2020 2020 656d 7074 795f 7461 626c        empty_tabl
-0000bf10: 6520 3d20 6c74 2e54 6162 6c65 2829 0a20  e = lt.Table(). 
-0000bf20: 2020 2020 2020 2065 6d70 7479 5f74 6162         empty_tab
-0000bf30: 6c65 2e63 7265 6174 655f 696e 6465 7828  le.create_index(
-0000bf40: 2761 2729 0a20 2020 2020 2020 2074 3520  'a').        t5 
-0000bf50: 3d20 2874 312e 6a6f 696e 5f6f 6e28 2761  = (t1.join_on('a
-0000bf60: 2729 202b 2065 6d70 7479 5f74 6162 6c65  ') + empty_table
-0000bf70: 2928 290a 2020 2020 2020 2020 7769 7468  )().        with
-0000bf80: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-0000bf90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000bfa0: 662e 6173 7365 7274 4571 7561 6c28 302c  f.assertEqual(0,
-0000bfb0: 206c 656e 2874 3529 290a 0a20 2020 2064   len(t5))..    d
-0000bfc0: 6566 2074 6573 745f 6f75 7465 725f 6a6f  ef test_outer_jo
-0000bfd0: 696e 7328 7365 6c66 293a 0a20 2020 2020  ins(self):.     
-0000bfe0: 2020 2074 3120 3d20 6c74 2e54 6162 6c65     t1 = lt.Table
-0000bff0: 2822 6361 7461 6c6f 6722 290a 2020 2020  ("catalog").    
-0000c000: 2020 2020 7431 2e63 7376 5f69 6d70 6f72      t1.csv_impor
-0000c010: 7428 7465 7874 7772 6170 2e64 6564 656e  t(textwrap.deden
-0000c020: 7428 2222 225c 0a20 2020 2020 2020 2020  t("""\.         
-0000c030: 2020 2073 6b75 2c63 6f6c 6f72 2c73 697a     sku,color,siz
-0000c040: 652c 6d61 7465 7269 616c 0a20 2020 2020  e,material.     
-0000c050: 2020 2020 2020 2030 3031 2c72 6564 2c58         001,red,X
-0000c060: 4c2c 636f 7474 6f6e 0a20 2020 2020 2020  L,cotton.       
-0000c070: 2020 2020 2030 3032 2c62 6c75 652c 584c       002,blue,XL
-0000c080: 2c63 6f74 746f 6e2f 706f 6c79 0a20 2020  ,cotton/poly.   
-0000c090: 2020 2020 2020 2020 2030 3033 2c62 6c75           003,blu
-0000c0a0: 652c 4c2c 6c69 6e65 6e0a 2020 2020 2020  e,L,linen.      
-0000c0b0: 2020 2020 2020 3030 342c 7265 642c 4d2c        004,red,M,
-0000c0c0: 636f 7474 6f6e 0a20 2020 2020 2020 2020  cotton.         
-0000c0d0: 2020 2022 2222 2929 0a0a 2020 2020 2020     """))..      
-0000c0e0: 2020 7432 203d 206c 742e 5461 626c 6528    t2 = lt.Table(
-0000c0f0: 2270 7269 6365 7322 290a 2020 2020 2020  "prices").      
-0000c100: 2020 7432 2e63 7376 5f69 6d70 6f72 7428    t2.csv_import(
-0000c110: 7465 7874 7772 6170 2e64 6564 656e 7428  textwrap.dedent(
-0000c120: 2222 225c 0a20 2020 2020 2020 2020 2020  """\.           
-0000c130: 2073 6b75 2c75 6e69 745f 7072 6963 652c   sku,unit_price,
-0000c140: 7369 7a65 0a20 2020 2020 2020 2020 2020  size.           
-0000c150: 2030 3031 2c31 302c 4c0a 2020 2020 2020   001,10,L.      
-0000c160: 2020 2020 2020 3030 312c 3132 2c58 4c0a        001,12,XL.
-0000c170: 2020 2020 2020 2020 2020 2020 3030 322c              002,
-0000c180: 3131 2c0a 2020 2020 2020 2020 2020 2020  11,.            
-0000c190: 3030 342c 392c 0a20 2020 2020 2020 2020  004,9,.         
-0000c1a0: 2020 2022 2222 292c 2074 7261 6e73 666f     """), transfo
-0000c1b0: 726d 733d 7b27 7369 7a65 273a 206c 616d  rms={'size': lam
-0000c1c0: 6264 6120 783a 2078 206f 7220 4e6f 6e65  bda x: x or None
-0000c1d0: 7d29 0a20 2020 2020 2020 2070 7269 6e74  }).        print
-0000c1e0: 2874 312e 696e 666f 2829 290a 0a20 2020  (t1.info())..   
-0000c1f0: 2020 2020 2074 312e 7072 6573 656e 7428       t1.present(
-0000c200: 290a 2020 2020 2020 2020 7432 2e70 7265  ).        t2.pre
-0000c210: 7365 6e74 2829 0a0a 2020 2020 2020 2020  sent()..        
-0000c220: 7433 203d 2074 312e 6a6f 696e 2874 322c  t3 = t1.join(t2,
-0000c230: 2061 7574 6f5f 6372 6561 7465 5f69 6e64   auto_create_ind
-0000c240: 6578 6573 3d54 7275 652c 2073 6b75 3d22  exes=True, sku="
-0000c250: 736b 7522 290a 2020 2020 2020 2020 7072  sku").        pr
-0000c260: 696e 7428 7433 2e69 6e66 6f28 2929 0a20  int(t3.info()). 
-0000c270: 2020 2020 2020 2074 332e 7072 6573 656e         t3.presen
-0000c280: 7428 290a 2020 2020 2020 2020 7769 7468  t().        with
-0000c290: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-0000c2a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000c2b0: 662e 6173 7365 7274 4571 7561 6c28 342c  f.assertEqual(4,
-0000c2c0: 206c 656e 2874 3329 290a 0a20 2020 2020   len(t3))..     
-0000c2d0: 2020 2074 3320 3d20 7431 2e6a 6f69 6e28     t3 = t1.join(
-0000c2e0: 7432 2c20 6175 746f 5f63 7265 6174 655f  t2, auto_create_
-0000c2f0: 696e 6465 7865 733d 5472 7565 2c20 736b  indexes=True, sk
-0000c300: 753d 2273 6b75 222c 2073 697a 653d 2273  u="sku", size="s
-0000c310: 697a 6522 290a 2020 2020 2020 2020 7433  ize").        t3
-0000c320: 2822 696e 6e65 7220 6a6f 696e 202d 2022  ("inner join - "
-0000c330: 202b 2074 332e 7461 626c 655f 6e61 6d65   + t3.table_name
-0000c340: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-0000c350: 7433 2e69 6e66 6f28 2929 0a20 2020 2020  t3.info()).     
-0000c360: 2020 2074 332e 7072 6573 656e 7428 290a     t3.present().
-0000c370: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0000c380: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-0000c390: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0000c3a0: 7365 7274 4571 7561 6c28 312c 206c 656e  sertEqual(1, len
-0000c3b0: 2874 3329 290a 0a20 2020 2020 2020 2074  (t3))..        t
-0000c3c0: 3320 3d20 7431 2e6f 7574 6572 5f6a 6f69  3 = t1.outer_joi
-0000c3d0: 6e28 6c74 2e54 6162 6c65 2e52 4947 4854  n(lt.Table.RIGHT
-0000c3e0: 5f4f 5554 4552 5f4a 4f49 4e2c 2074 322c  _OUTER_JOIN, t2,
-0000c3f0: 2073 6b75 3d22 736b 7522 2c20 7369 7a65   sku="sku", size
-0000c400: 3d22 7369 7a65 2229 0a20 2020 2020 2020  ="size").       
-0000c410: 2074 3328 2272 6967 6874 206f 7574 6572   t3("right outer
-0000c420: 206a 6f69 6e20 2d20 2220 2b20 7433 2e74   join - " + t3.t
-0000c430: 6162 6c65 5f6e 616d 6529 0a20 2020 2020  able_name).     
-0000c440: 2020 2070 7269 6e74 2874 332e 696e 666f     print(t3.info
-0000c450: 2829 290a 2020 2020 2020 2020 7433 2e70  ()).        t3.p
-0000c460: 7265 7365 6e74 2829 0a20 2020 2020 2020  resent().       
-0000c470: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-0000c480: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-0000c490: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0000c4a0: 616c 2834 2c20 6c65 6e28 7433 2929 0a0a  al(4, len(t3))..
-0000c4b0: 2020 2020 2020 2020 7433 203d 2074 312e          t3 = t1.
-0000c4c0: 6f75 7465 725f 6a6f 696e 286c 742e 5461  outer_join(lt.Ta
-0000c4d0: 626c 652e 4c45 4654 5f4f 5554 4552 5f4a  ble.LEFT_OUTER_J
-0000c4e0: 4f49 4e2c 2074 322c 2073 6b75 3d22 736b  OIN, t2, sku="sk
-0000c4f0: 7522 2c20 7369 7a65 3d22 7369 7a65 2229  u", size="size")
-0000c500: 0a20 2020 2020 2020 2074 3328 226c 6566  .        t3("lef
-0000c510: 7420 6f75 7465 7220 6a6f 696e 202d 2022  t outer join - "
-0000c520: 202b 2074 332e 7461 626c 655f 6e61 6d65   + t3.table_name
-0000c530: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-0000c540: 7433 2e69 6e66 6f28 2929 0a20 2020 2020  t3.info()).     
-0000c550: 2020 2074 332e 7072 6573 656e 7428 290a     t3.present().
-0000c560: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0000c570: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-0000c580: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0000c590: 7365 7274 4571 7561 6c28 322c 206c 656e  sertEqual(2, len
-0000c5a0: 2874 3329 290a 0a20 2020 2020 2020 2074  (t3))..        t
-0000c5b0: 3320 3d20 7431 2e6f 7574 6572 5f6a 6f69  3 = t1.outer_joi
-0000c5c0: 6e28 6c74 2e54 6162 6c65 2e46 554c 4c5f  n(lt.Table.FULL_
-0000c5d0: 4f55 5445 525f 4a4f 494e 2c20 7432 2c20  OUTER_JOIN, t2, 
-0000c5e0: 736b 753d 2273 6b75 222c 2073 697a 653d  sku="sku", size=
-0000c5f0: 2273 697a 6522 290a 2020 2020 2020 2020  "size").        
-0000c600: 7433 2822 6675 6c6c 206f 7574 6572 206a  t3("full outer j
-0000c610: 6f69 6e20 2d20 2220 2b20 7433 2e74 6162  oin - " + t3.tab
-0000c620: 6c65 5f6e 616d 6529 0a20 2020 2020 2020  le_name).       
-0000c630: 2070 7269 6e74 2874 332e 696e 666f 2829   print(t3.info()
-0000c640: 290a 2020 2020 2020 2020 7433 2e70 7265  ).        t3.pre
-0000c650: 7365 6e74 2829 0a20 2020 2020 2020 2077  sent().        w
-0000c660: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000c670: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000c680: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000c690: 2831 322c 206c 656e 2874 3329 290a 0a20  (12, len(t3)).. 
-0000c6a0: 2020 2064 6566 2074 6573 745f 6f75 7465     def test_oute
-0000c6b0: 725f 6a6f 696e 5f65 7861 6d70 6c65 2873  r_join_example(s
-0000c6c0: 656c 6629 3a0a 2020 2020 2020 2020 2320  elf):.        # 
-0000c6d0: 6465 6669 6e65 2073 7475 6465 6e74 2061  define student a
-0000c6e0: 6e64 2072 6567 6973 7472 6174 696f 6e20  nd registration 
-0000c6f0: 6461 7461 0a20 2020 2020 2020 2073 7475  data.        stu
-0000c700: 6465 6e74 7320 3d20 6c74 2e54 6162 6c65  dents = lt.Table
-0000c710: 2822 7374 7564 656e 7473 2229 2e63 7376  ("students").csv
-0000c720: 5f69 6d70 6f72 7428 7465 7874 7772 6170  _import(textwrap
-0000c730: 2e64 6564 656e 7428 2222 225c 0a20 2020  .dedent("""\.   
-0000c740: 2020 2020 2020 2020 2073 7475 6465 6e74           student
-0000c750: 5f69 642c 6e61 6d65 0a20 2020 2020 2020  _id,name.       
-0000c760: 2020 2020 2030 3030 312c 416c 6963 650a       0001,Alice.
-0000c770: 2020 2020 2020 2020 2020 2020 3030 3032              0002
-0000c780: 2c42 6f62 0a20 2020 2020 2020 2020 2020  ,Bob.           
-0000c790: 2030 3030 332c 4368 6172 6c69 650a 2020   0003,Charlie.  
-0000c7a0: 2020 2020 2020 2020 2020 3030 3034 2c44            0004,D
-0000c7b0: 6176 650a 2020 2020 2020 2020 2020 2020  ave.            
-0000c7c0: 3030 3035 2c45 6e69 640a 2020 2020 2020  0005,Enid.      
-0000c7d0: 2020 2020 2020 2222 2229 290a 0a20 2020        """))..   
-0000c7e0: 2020 2020 2072 6567 6973 7472 6174 696f       registratio
-0000c7f0: 6e73 203d 206c 742e 5461 626c 6528 2272  ns = lt.Table("r
-0000c800: 6567 6973 7472 6174 696f 6e73 2229 2e63  egistrations").c
-0000c810: 7376 5f69 6d70 6f72 7428 7465 7874 7772  sv_import(textwr
-0000c820: 6170 2e64 6564 656e 7428 2222 225c 0a20  ap.dedent("""\. 
-0000c830: 2020 2020 2020 2020 2020 2073 7475 6465             stude
-0000c840: 6e74 5f69 642c 636f 7572 7365 0a20 2020  nt_id,course.   
-0000c850: 2020 2020 2020 2020 2030 3030 312c 5053           0001,PS
-0000c860: 5943 4831 3031 0a20 2020 2020 2020 2020  YCH101.         
-0000c870: 2020 2030 3030 312c 4341 4c43 310a 2020     0001,CALC1.  
-0000c880: 2020 2020 2020 2020 2020 3030 3033 2c42            0003,B
-0000c890: 494f 3230 300a 2020 2020 2020 2020 2020  IO200.          
-0000c8a0: 2020 3030 3035 2c43 4845 4d31 3031 0a20    0005,CHEM101. 
-0000c8b0: 2020 2020 2020 2020 2020 2030 3030 362c             0006,
-0000c8c0: 5048 5931 3031 0a20 2020 2020 2020 2020  PHY101.         
-0000c8d0: 2020 2022 2222 2929 0a0a 2020 2020 2020     """))..      
-0000c8e0: 2020 636f 7572 7365 7320 3d20 6c74 2e54    courses = lt.T
-0000c8f0: 6162 6c65 2822 636f 7572 7365 7322 292e  able("courses").
-0000c900: 6373 765f 696d 706f 7274 2874 6578 7477  csv_import(textw
-0000c910: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
-0000c920: 2020 2020 2020 2020 2020 2020 636f 7572              cour
-0000c930: 7365 0a20 2020 2020 2020 2020 2020 2042  se.            B
-0000c940: 494f 3230 300a 2020 2020 2020 2020 2020  IO200.          
-0000c950: 2020 4341 4c43 310a 2020 2020 2020 2020    CALC1.        
-0000c960: 2020 2020 4348 454d 3130 310a 2020 2020      CHEM101.    
-0000c970: 2020 2020 2020 2020 5053 5943 4831 3031          PSYCH101
-0000c980: 0a20 2020 2020 2020 2020 2020 2050 4531  .            PE1
-0000c990: 3031 0a20 2020 2020 2020 2020 2020 2022  01.            "
-0000c9a0: 2222 2929 0a0a 2020 2020 2020 2020 2320  ""))..        # 
-0000c9b0: 7065 7266 6f72 6d20 6f75 7465 7220 6a6f  perform outer jo
-0000c9c0: 696e 2061 6e64 2073 686f 7720 7265 7375  in and show resu
-0000c9d0: 6c74 733a 0a20 2020 2020 2020 206e 6f6e  lts:.        non
-0000c9e0: 5f72 6567 203d 2073 7475 6465 6e74 732e  _reg = students.
-0000c9f0: 6f75 7465 725f 6a6f 696e 286c 742e 5461  outer_join(lt.Ta
-0000ca00: 626c 652e 5249 4748 545f 4f55 5445 525f  ble.RIGHT_OUTER_
-0000ca10: 4a4f 494e 2c0a 2020 2020 2020 2020 2020  JOIN,.          
-0000ca20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca30: 2020 2020 2020 2020 2020 2020 7265 6769              regi
-0000ca40: 7374 7261 7469 6f6e 732c 0a20 2020 2020  strations,.     
-0000ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca70: 2073 7475 6465 6e74 5f69 643d 2273 7475   student_id="stu
-0000ca80: 6465 6e74 5f69 6422 292e 7768 6572 6528  dent_id").where(
-0000ca90: 636f 7572 7365 3d4e 6f6e 6529 0a20 2020  course=None).   
-0000caa0: 2020 2020 206e 6f6e 5f72 6567 2e70 7265       non_reg.pre
-0000cab0: 7365 6e74 2829 0a20 2020 2020 2020 2070  sent().        p
-0000cac0: 7269 6e74 286c 6973 7428 6e6f 6e5f 7265  rint(list(non_re
-0000cad0: 672e 616c 6c2e 6e61 6d65 2929 0a20 2020  g.all.name)).   
-0000cae0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-0000caf0: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
-0000cb00: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000cb10: 7445 7175 616c 285b 2742 6f62 272c 2027  tEqual(['Bob', '
-0000cb20: 4461 7665 275d 2c20 736f 7274 6564 286e  Dave'], sorted(n
-0000cb30: 6f6e 5f72 6567 2e61 6c6c 2e6e 616d 6529  on_reg.all.name)
-0000cb40: 290a 0a20 2020 2020 2020 2023 2063 6f75  )..        # cou
-0000cb50: 7273 6573 2077 6974 6820 6e6f 2073 7475  rses with no stu
-0000cb60: 6465 6e74 730a 2020 2020 2020 2020 6e6f  dents.        no
-0000cb70: 5f73 7475 6465 6e74 7320 3d20 7265 6769  _students = regi
-0000cb80: 7374 7261 7469 6f6e 732e 6f75 7465 725f  strations.outer_
-0000cb90: 6a6f 696e 286c 742e 5461 626c 652e 4c45  join(lt.Table.LE
-0000cba0: 4654 5f4f 5554 4552 5f4a 4f49 4e2c 0a20  FT_OUTER_JOIN,. 
-0000cbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbd0: 2020 2020 2020 2020 636f 7572 7365 732c          courses,
-0000cbe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc00: 2020 2020 2020 2020 2020 636f 7572 7365            course
-0000cc10: 3d22 636f 7572 7365 2229 2e77 6865 7265  ="course").where
-0000cc20: 2873 7475 6465 6e74 5f69 643d 4e6f 6e65  (student_id=None
-0000cc30: 290a 2020 2020 2020 2020 6e6f 5f73 7475  ).        no_stu
-0000cc40: 6465 6e74 732e 7072 6573 656e 7428 290a  dents.present().
-0000cc50: 2020 2020 2020 2020 7072 696e 7428 6c69          print(li
-0000cc60: 7374 286e 6f5f 7374 7564 656e 7473 2e61  st(no_students.a
-0000cc70: 6c6c 2e63 6f75 7273 6529 290a 2020 2020  ll.course)).    
-0000cc80: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-0000cc90: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-0000cca0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000ccb0: 4571 7561 6c28 5b27 5045 3130 3127 5d2c  Equal(['PE101'],
-0000ccc0: 2073 6f72 7465 6428 6e6f 5f73 7475 6465   sorted(no_stude
-0000ccd0: 6e74 732e 616c 6c2e 636f 7572 7365 2929  nts.all.course))
-0000cce0: 0a0a 0a20 2020 2020 2020 2066 756c 6c20  ...        full 
-0000ccf0: 3d20 2073 7475 6465 6e74 732e 6f75 7465  =  students.oute
-0000cd00: 725f 6a6f 696e 286c 742e 5461 626c 652e  r_join(lt.Table.
-0000cd10: 4655 4c4c 5f4f 5554 4552 5f4a 4f49 4e2c  FULL_OUTER_JOIN,
-0000cd20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd40: 2020 2020 2020 2072 6567 6973 7472 6174         registrat
-0000cd50: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd70: 2020 2020 2020 2020 2020 2020 7374 7564              stud
-0000cd80: 656e 745f 6964 3d22 7374 7564 656e 745f  ent_id="student_
-0000cd90: 6964 2229 2e77 6865 7265 286c 616d 6264  id").where(lambd
-0000cda0: 6120 7265 633a 2072 6563 2e63 6f75 7273  a rec: rec.cours
-0000cdb0: 6520 6973 204e 6f6e 650a 2020 2020 2020  e is None.      
-0000cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce00: 2020 2020 2020 2020 2020 206f 7220 7265             or re
-0000ce10: 632e 6e61 6d65 2069 7320 4e6f 6e65 290a  c.name is None).
-0000ce20: 2020 2020 2020 2020 6675 6c6c 2e70 7265          full.pre
-0000ce30: 7365 6e74 2829 0a20 2020 2020 2020 2070  sent().        p
-0000ce40: 7269 6e74 2873 6f72 7465 6428 6675 6c6c  rint(sorted(full
-0000ce50: 2e61 6c6c 2e73 7475 6465 6e74 5f69 6429  .all.student_id)
-0000ce60: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
-0000ce70: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-0000ce80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ce90: 6173 7365 7274 4571 7561 6c28 5b27 3030  assertEqual(['00
-0000cea0: 3032 272c 2027 3030 3034 272c 2027 3030  02', '0004', '00
-0000ceb0: 3036 275d 2c20 736f 7274 6564 2866 756c  06'], sorted(ful
-0000cec0: 6c2e 616c 6c2e 7374 7564 656e 745f 6964  l.all.student_id
-0000ced0: 2929 0a0a 0a40 6d61 6b65 5f74 6573 745f  ))...@make_test_
-0000cee0: 636c 6173 7365 730a 636c 6173 7320 5461  classes.class Ta
-0000cef0: 626c 6554 7261 6e73 666f 726d 5465 7374  bleTransformTest
-0000cf00: 733a 0a20 2020 2064 6566 2074 6573 745f  s:.    def test_
-0000cf10: 736f 7274 2873 656c 6629 3a0a 2020 2020  sort(self):.    
-0000cf20: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
-0000cf30: 3130 0a20 2020 2020 2020 2074 3120 3d20  10.        t1 = 
-0000cf40: 6d61 6b65 5f74 6573 745f 7461 626c 6528  make_test_table(
-0000cf50: 7365 6c66 2e6d 616b 655f 6461 7461 5f6f  self.make_data_o
-0000cf60: 626a 6563 742c 2074 6573 745f 7369 7a65  bject, test_size
-0000cf70: 290a 0a20 2020 2020 2020 2063 5f67 726f  )..        c_gro
-0000cf80: 7570 7320 3d20 300a 2020 2020 2020 2020  ups = 0.        
-0000cf90: 666f 7220 635f 7661 6c75 652c 2072 6563  for c_value, rec
-0000cfa0: 7320 696e 2069 7465 7274 6f6f 6c73 2e67  s in itertools.g
-0000cfb0: 726f 7570 6279 2874 312c 206b 6579 3d6c  roupby(t1, key=l
-0000cfc0: 616d 6264 6120 7265 633a 2072 6563 2e63  ambda rec: rec.c
-0000cfd0: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
-0000cfe0: 5f67 726f 7570 7320 2b3d 2031 0a20 2020  _groups += 1.   
-0000cff0: 2020 2020 2020 2020 206c 6973 7428 7265           list(re
-0000d000: 6373 290a 2020 2020 2020 2020 7769 7468  cs).        with
-0000d010: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-0000d020: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d030: 662e 6173 7365 7274 4571 7561 6c28 7465  f.assertEqual(te
-0000d040: 7374 5f73 697a 6520 2a20 7465 7374 5f73  st_size * test_s
-0000d050: 697a 6520 2a20 7465 7374 5f73 697a 652c  ize * test_size,
-0000d060: 2063 5f67 726f 7570 7329 0a0a 2020 2020   c_groups)..    
-0000d070: 2020 2020 7431 2e73 6f72 7428 2763 2729      t1.sort('c')
-0000d080: 0a20 2020 2020 2020 2063 5f67 726f 7570  .        c_group
-0000d090: 7320 3d20 300a 2020 2020 2020 2020 666f  s = 0.        fo
-0000d0a0: 7220 635f 7661 6c75 652c 2072 6563 7320  r c_value, recs 
-0000d0b0: 696e 2069 7465 7274 6f6f 6c73 2e67 726f  in itertools.gro
-0000d0c0: 7570 6279 2874 312c 206b 6579 3d6c 616d  upby(t1, key=lam
-0000d0d0: 6264 6120 7265 633a 2072 6563 2e63 293a  bda rec: rec.c):
-0000d0e0: 0a20 2020 2020 2020 2020 2020 2063 5f67  .            c_g
-0000d0f0: 726f 7570 7320 2b3d 2031 0a20 2020 2020  roups += 1.     
-0000d100: 2020 2020 2020 206c 6973 7428 7265 6373         list(recs
-0000d110: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
-0000d120: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-0000d130: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d140: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
-0000d150: 5f73 697a 652c 2063 5f67 726f 7570 7329  _size, c_groups)
-0000d160: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000d170: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-0000d180: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000d190: 7373 6572 7445 7175 616c 2830 2c20 7431  ssertEqual(0, t1
-0000d1a0: 5b30 5d2e 6329 0a0a 2020 2020 2020 2020  [0].c)..        
-0000d1b0: 7431 2e73 6f72 7428 2763 2064 6573 6327  t1.sort('c desc'
-0000d1c0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
-0000d1d0: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-0000d1e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d1f0: 6173 7365 7274 4571 7561 6c28 7465 7374  assertEqual(test
-0000d200: 5f73 697a 652d 312c 2074 315b 305d 2e63  _size-1, t1[0].c
-0000d210: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-0000d220: 736f 7274 3228 7365 6c66 293a 0a0a 2020  sort2(self):..  
-0000d230: 2020 2020 2020 726f 775f 7479 7065 203d        row_type =
-0000d240: 2074 7970 6528 7365 6c66 2e6d 616b 655f   type(self.make_
-0000d250: 6461 7461 5f6f 626a 6563 7428 302c 302c  data_object(0,0,
-0000d260: 3029 290a 2020 2020 2020 2020 7474 203d  0)).        tt =
-0000d270: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
-0000d280: 696d 706f 7274 2874 6578 7477 7261 702e  import(textwrap.
-0000d290: 6465 6465 6e74 2822 2222 5c0a 2020 2020  dedent("""\.    
-0000d2a0: 2020 2020 612c 632c 620a 2020 2020 2020      a,c,b.      
-0000d2b0: 2020 312c 322c 310a 2020 2020 2020 2020    1,2,1.        
-0000d2c0: 322c 332c 300a 2020 2020 2020 2020 352c  2,3,0.        5,
-0000d2d0: 352c 2d31 0a20 2020 2020 2020 2033 2c34  5,-1.        3,4
-0000d2e0: 2c2d 310a 2020 2020 2020 2020 322c 342c  ,-1.        2,4,
-0000d2f0: 2d33 2222 2229 2c20 726f 775f 636c 6173  -3"""), row_clas
-0000d300: 733d 726f 775f 7479 7065 2c20 7472 616e  s=row_type, tran
-0000d310: 7366 6f72 6d73 3d64 6963 742e 6672 6f6d  sforms=dict.from
-0000d320: 6b65 7973 2822 6120 6220 6322 2e73 706c  keys("a b c".spl
-0000d330: 6974 2829 2c20 696e 7429 290a 0a20 2020  it(), int))..   
-0000d340: 2020 2020 2064 6566 2074 6f5f 7475 706c       def to_tupl
-0000d350: 6573 2874 293a 0a20 2020 2020 2020 2020  es(t):.         
-0000d360: 2020 2072 6574 7572 6e20 6c69 7374 286d     return list(m
-0000d370: 6170 2861 7474 7267 6574 7465 7228 2a74  ap(attrgetter(*t
-0000d380: 2e69 6e66 6f28 295b 2766 6965 6c64 7327  .info()['fields'
-0000d390: 5d29 2c20 7429 290a 0a20 2020 2020 2020  ]), t))..       
-0000d3a0: 2070 7269 6e74 2874 742e 696e 666f 2829   print(tt.info()
-0000d3b0: 5b27 6669 656c 6473 275d 290a 0a20 2020  ['fields'])..   
-0000d3c0: 2020 2020 2073 6f72 745f 6172 6720 3d20       sort_arg = 
-0000d3d0: 2263 2062 222e 7370 6c69 7428 290a 2020  "c b".split().  
-0000d3e0: 2020 2020 2020 7072 696e 7428 6622 536f        print(f"So
-0000d3f0: 7274 696e 6720 6279 207b 736f 7274 5f61  rting by {sort_a
-0000d400: 7267 2172 7d22 290a 2020 2020 2020 2020  rg!r}").        
-0000d410: 7474 2e73 6875 6666 6c65 2829 0a20 2020  tt.shuffle().   
-0000d420: 2020 2020 2074 742e 736f 7274 2873 6f72       tt.sort(sor
-0000d430: 745f 6172 6729 0a20 2020 2020 2020 2074  t_arg).        t
-0000d440: 315f 7475 706c 6573 203d 2074 6f5f 7475  1_tuples = to_tu
-0000d450: 706c 6573 2874 7429 0a20 2020 2020 2020  ples(tt).       
-0000d460: 2066 6f72 2074 2069 6e20 7431 5f74 7570   for t in t1_tup
-0000d470: 6c65 733a 0a20 2020 2020 2020 2020 2020  les:.           
-0000d480: 2070 7269 6e74 2874 290a 2020 2020 2020   print(t).      
-0000d490: 2020 7072 696e 7428 290a 0a20 2020 2020    print()..     
-0000d4a0: 2020 2074 742e 7368 7566 666c 6528 290a     tt.shuffle().
-0000d4b0: 2020 2020 2020 2020 7474 2e73 6f72 7428          tt.sort(
-0000d4c0: 2262 2229 0a20 2020 2020 2020 2074 742e  "b").        tt.
-0000d4d0: 736f 7274 2822 6322 290a 2020 2020 2020  sort("c").      
-0000d4e0: 2020 7432 5f74 7570 6c65 7320 3d20 746f    t2_tuples = to
-0000d4f0: 5f74 7570 6c65 7328 7474 290a 2020 2020  _tuples(tt).    
-0000d500: 2020 2020 666f 7220 7420 696e 2074 325f      for t in t2_
-0000d510: 7475 706c 6573 3a0a 2020 2020 2020 2020  tuples:.        
-0000d520: 2020 2020 7072 696e 7428 7429 0a20 2020      print(t).   
-0000d530: 2020 2020 2070 7269 6e74 2829 0a0a 2020       print()..  
-0000d540: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0000d550: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-0000d560: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000d570: 7274 4571 7561 6c28 7431 5f74 7570 6c65  rtEqual(t1_tuple
-0000d580: 732c 2074 325f 7475 706c 6573 2c20 2266  s, t2_tuples, "f
-0000d590: 6169 6c65 6420 6d75 6c74 692d 6174 7472  ailed multi-attr
-0000d5a0: 6962 7574 6520 736f 7274 2c20 6769 7665  ibute sort, give
-0000d5b0: 6e20 6c69 7374 206f 6620 6174 7472 6962  n list of attrib
-0000d5c0: 7574 6573 2229 0a0a 2020 2020 2020 2020  utes")..        
-0000d5d0: 736f 7274 5f61 7267 203d 2022 632c 6222  sort_arg = "c,b"
-0000d5e0: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
-0000d5f0: 2253 6f72 7469 6e67 2062 7920 7b73 6f72  "Sorting by {sor
-0000d600: 745f 6172 6721 727d 2229 0a20 2020 2020  t_arg!r}").     
-0000d610: 2020 2074 742e 7368 7566 666c 6528 290a     tt.shuffle().
-0000d620: 2020 2020 2020 2020 7474 2e73 6f72 7428          tt.sort(
-0000d630: 736f 7274 5f61 7267 290a 2020 2020 2020  sort_arg).      
-0000d640: 2020 7431 5f74 7570 6c65 7320 3d20 746f    t1_tuples = to
-0000d650: 5f74 7570 6c65 7328 7474 290a 2020 2020  _tuples(tt).    
-0000d660: 2020 2020 666f 7220 7420 696e 2074 315f      for t in t1_
-0000d670: 7475 706c 6573 3a0a 2020 2020 2020 2020  tuples:.        
-0000d680: 2020 2020 7072 696e 7428 7429 0a20 2020      print(t).   
-0000d690: 2020 2020 2070 7269 6e74 2829 0a0a 2020       print()..  
-0000d6a0: 2020 2020 2020 7474 2e73 6875 6666 6c65        tt.shuffle
-0000d6b0: 2829 0a20 2020 2020 2020 2074 742e 736f  ().        tt.so
-0000d6c0: 7274 2822 6222 290a 2020 2020 2020 2020  rt("b").        
-0000d6d0: 7474 2e73 6f72 7428 2263 2229 0a20 2020  tt.sort("c").   
-0000d6e0: 2020 2020 2074 325f 7475 706c 6573 203d       t2_tuples =
-0000d6f0: 2074 6f5f 7475 706c 6573 2874 7429 0a20   to_tuples(tt). 
-0000d700: 2020 2020 2020 2066 6f72 2074 2069 6e20         for t in 
-0000d710: 7432 5f74 7570 6c65 733a 0a20 2020 2020  t2_tuples:.     
-0000d720: 2020 2020 2020 2070 7269 6e74 2874 290a         print(t).
-0000d730: 2020 2020 2020 2020 7072 696e 7428 290a          print().
-0000d740: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000d750: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-0000d760: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000d770: 7373 6572 7445 7175 616c 2874 315f 7475  ssertEqual(t1_tu
-0000d780: 706c 6573 2c20 7432 5f74 7570 6c65 732c  ples, t2_tuples,
-0000d790: 2022 6661 696c 6564 206d 756c 7469 2d61   "failed multi-a
-0000d7a0: 7474 7269 6275 7465 2073 6f72 742c 2067  ttribute sort, g
-0000d7b0: 6976 656e 2063 6f6d 6d61 2d73 6570 6172  iven comma-separ
-0000d7c0: 6174 6564 2061 7474 7269 6275 7465 7320  ated attributes 
-0000d7d0: 7374 7269 6e67 2229 0a0a 2020 2020 2020  string")..      
-0000d7e0: 2020 736f 7274 5f61 7267 203d 2022 632c    sort_arg = "c,
-0000d7f0: 6220 6465 7363 220a 2020 2020 2020 2020  b desc".        
-0000d800: 7072 696e 7428 6622 536f 7274 696e 6720  print(f"Sorting 
-0000d810: 6279 207b 736f 7274 5f61 7267 2172 7d22  by {sort_arg!r}"
-0000d820: 290a 2020 2020 2020 2020 7474 2e73 6875  ).        tt.shu
-0000d830: 6666 6c65 2829 0a20 2020 2020 2020 2074  ffle().        t
-0000d840: 742e 736f 7274 2873 6f72 745f 6172 6729  t.sort(sort_arg)
-0000d850: 0a20 2020 2020 2020 2074 315f 7475 706c  .        t1_tupl
-0000d860: 6573 203d 2074 6f5f 7475 706c 6573 2874  es = to_tuples(t
-0000d870: 7429 0a20 2020 2020 2020 2066 6f72 2074  t).        for t
-0000d880: 2069 6e20 7431 5f74 7570 6c65 733a 0a20   in t1_tuples:. 
-0000d890: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000d8a0: 2874 290a 2020 2020 2020 2020 7072 696e  (t).        prin
-0000d8b0: 7428 290a 0a20 2020 2020 2020 2074 742e  t()..        tt.
-0000d8c0: 7368 7566 666c 6528 290a 2020 2020 2020  shuffle().      
-0000d8d0: 2020 7474 2e73 6f72 7428 2262 2064 6573    tt.sort("b des
-0000d8e0: 6322 290a 2020 2020 2020 2020 7474 2e73  c").        tt.s
-0000d8f0: 6f72 7428 2263 2229 0a20 2020 2020 2020  ort("c").       
-0000d900: 2074 325f 7475 706c 6573 203d 2074 6f5f   t2_tuples = to_
-0000d910: 7475 706c 6573 2874 7429 0a20 2020 2020  tuples(tt).     
-0000d920: 2020 2066 6f72 2074 2069 6e20 7432 5f74     for t in t2_t
-0000d930: 7570 6c65 733a 0a20 2020 2020 2020 2020  uples:.         
-0000d940: 2020 2070 7269 6e74 2874 290a 2020 2020     print(t).    
-0000d950: 2020 2020 7072 696e 7428 290a 0a20 2020      print()..   
-0000d960: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-0000d970: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
-0000d980: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000d990: 7445 7175 616c 2874 315f 7475 706c 6573  tEqual(t1_tuples
-0000d9a0: 2c20 7432 5f74 7570 6c65 732c 2022 6661  , t2_tuples, "fa
-0000d9b0: 696c 6564 206d 6978 6564 2061 7363 656e  iled mixed ascen
-0000d9c0: 6469 6e67 2f64 6573 6365 6e64 696e 6720  ding/descending 
-0000d9d0: 6d75 6c74 692d 6174 7472 6962 7574 6520  multi-attribute 
-0000d9e0: 736f 7274 2229 0a0a 2020 2020 6465 6620  sort")..    def 
-0000d9f0: 7465 7374 5f73 6f72 7433 2873 656c 6629  test_sort3(self)
-0000da00: 3a0a 2020 2020 2020 2020 656d 706c 6f79  :.        employ
-0000da10: 6565 7320 3d20 6c74 2e54 6162 6c65 2829  ees = lt.Table()
-0000da20: 2e63 7376 5f69 6d70 6f72 7428 7465 7874  .csv_import(text
-0000da30: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
-0000da40: 0a20 2020 2020 2020 2020 2020 2065 6d70  .            emp
-0000da50: 5f69 642c 6e61 6d65 2c64 6570 742c 7361  _id,name,dept,sa
-0000da60: 6c61 7279 2c63 6f6d 6d69 7373 696f 6e0a  lary,commission.
-0000da70: 2020 2020 2020 2020 2020 2020 3030 3031              0001
-0000da80: 2c41 6c69 6365 2c53 616c 6573 2c35 3030  ,Alice,Sales,500
-0000da90: 3030 2c30 2e35 0a20 2020 2020 2020 2020  00,0.5.         
-0000daa0: 2020 2030 3030 322c 426f 622c 456e 6769     0002,Bob,Engi
-0000dab0: 6e65 6572 696e 672c 3130 3030 3030 2c0a  neering,100000,.
-0000dac0: 2020 2020 2020 2020 2020 2020 3030 3033              0003
-0000dad0: 2c43 6861 726c 6573 2c53 616c 6573 2c34  ,Charles,Sales,4
-0000dae0: 3530 3030 2c30 2e37 0a20 2020 2020 2020  5000,0.7.       
-0000daf0: 2020 2020 2030 3030 342c 4461 7665 2c53       0004,Dave,S
-0000db00: 616c 6573 2c34 3530 3030 2c30 2e36 0a20  ales,45000,0.6. 
-0000db10: 2020 2020 2020 2020 2020 2030 3030 352c             0005,
-0000db20: 456d 696c 792c 5361 6c65 732c 3530 3030  Emily,Sales,5000
-0000db30: 302c 302e 340a 2020 2020 2020 2020 2020  0,0.4.          
-0000db40: 2020 2222 2229 2c20 7472 616e 7366 6f72    """), transfor
-0000db50: 6d73 3d7b 2273 616c 6172 7922 3a20 696e  ms={"salary": in
-0000db60: 742c 2022 636f 6d6d 6973 7369 6f6e 223a  t, "commission":
-0000db70: 2066 6c6f 6174 7d29 0a0a 2020 2020 2020   float})..      
-0000db80: 2020 7361 6c65 735f 656d 706c 6f79 6565    sales_employee
-0000db90: 7320 3d20 656d 706c 6f79 6565 732e 7768  s = employees.wh
-0000dba0: 6572 6528 6465 7074 3d22 5361 6c65 7322  ere(dept="Sales"
-0000dbb0: 292e 736f 7274 2822 7361 6c61 7279 2064  ).sort("salary d
-0000dbc0: 6573 632c 636f 6d6d 6973 7369 6f6e 2229  esc,commission")
-0000dbd0: 0a0a 2020 2020 2020 2020 7361 6c65 735f  ..        sales_
-0000dbe0: 656d 706c 6f79 6565 732e 7072 6573 656e  employees.presen
-0000dbf0: 7428 290a 2020 2020 2020 2020 7072 696e  t().        prin
-0000dc00: 7428 6c69 7374 2873 616c 6573 5f65 6d70  t(list(sales_emp
-0000dc10: 6c6f 7965 6573 2e61 6c6c 2e65 6d70 5f69  loyees.all.emp_i
-0000dc20: 6429 290a 0a20 2020 2020 2020 2077 6974  d))..        wit
-0000dc30: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-0000dc40: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000dc50: 6c66 2e61 7373 6572 7445 7175 616c 285b  lf.assertEqual([
-0000dc60: 2730 3030 3527 2c20 2730 3030 3127 2c20  '0005', '0001', 
-0000dc70: 2730 3030 3427 2c20 2730 3030 3327 5d2c  '0004', '0003'],
-0000dc80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dc90: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-0000dca0: 7374 2873 616c 6573 5f65 6d70 6c6f 7965  st(sales_employe
-0000dcb0: 6573 2e61 6c6c 2e65 6d70 5f69 6429 290a  es.all.emp_id)).
-0000dcc0: 0a20 2020 2064 6566 2074 6573 745f 756e  .    def test_un
-0000dcd0: 6971 7565 2873 656c 6629 3a0a 2020 2020  ique(self):.    
-0000dce0: 2020 2020 7465 7374 5f73 697a 6520 3d20      test_size = 
-0000dcf0: 3130 0a20 2020 2020 2020 2074 3120 3d20  10.        t1 = 
-0000dd00: 6d61 6b65 5f74 6573 745f 7461 626c 6528  make_test_table(
-0000dd10: 7365 6c66 2e6d 616b 655f 6461 7461 5f6f  self.make_data_o
-0000dd20: 626a 6563 742c 2074 6573 745f 7369 7a65  bject, test_size
-0000dd30: 290a 0a20 2020 2020 2020 2074 3220 3d20  )..        t2 = 
-0000dd40: 7431 2e75 6e69 7175 6528 290a 2020 2020  t1.unique().    
-0000dd50: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-0000dd60: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-0000dd70: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000dd80: 4571 7561 6c28 6c65 6e28 7431 292c 206c  Equal(len(t1), l
-0000dd90: 656e 2874 3229 290a 0a20 2020 2020 2020  en(t2))..       
-0000dda0: 2074 3320 3d20 7431 2e75 6e69 7175 6528   t3 = t1.unique(
-0000ddb0: 6b65 793d 6c61 6d62 6461 2072 6563 3a20  key=lambda rec: 
-0000ddc0: 7265 632e 6329 0a20 2020 2020 2020 2077  rec.c).        w
-0000ddd0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000dde0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000ddf0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000de00: 2874 6573 745f 7369 7a65 2c20 6c65 6e28  (test_size, len(
-0000de10: 7433 2929 0a0a 0a40 6d61 6b65 5f74 6573  t3))...@make_tes
-0000de20: 745f 636c 6173 7365 730a 636c 6173 7320  t_classes.class 
-0000de30: 5461 626c 654f 7574 7075 7454 6573 7473  TableOutputTests
-0000de40: 3a0a 2020 2020 6465 6620 7465 7374 5f62  :.    def test_b
-0000de50: 6173 6963 5f70 7265 7365 6e74 2873 656c  asic_present(sel
-0000de60: 6629 3a0a 2020 2020 2020 2020 6966 2072  f):.        if r
-0000de70: 6963 6820 6973 204e 6f6e 653a 0a20 2020  ich is None:.   
-0000de80: 2020 2020 2020 2020 2069 6d70 6f72 7420           import 
-0000de90: 7761 726e 696e 6773 0a20 2020 2020 2020  warnings.       
-0000dea0: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
-0000deb0: 726e 2822 7269 6368 206e 6f74 2069 6e73  rn("rich not ins
-0000dec0: 7461 6c6c 6564 2c20 6361 6e6e 6f74 2072  talled, cannot r
-0000ded0: 756e 2074 6573 7422 290a 2020 2020 2020  un test").      
-0000dee0: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
-0000def0: 2020 2020 2020 6672 6f6d 2072 6963 6820        from rich 
-0000df00: 696d 706f 7274 2062 6f78 0a20 2020 2020  import box.     
-0000df10: 2020 2066 726f 6d20 696f 2069 6d70 6f72     from io impor
-0000df20: 7420 5374 7269 6e67 494f 0a20 2020 2020  t StringIO.     
-0000df30: 2020 2074 6162 6c65 203d 206c 742e 5461     table = lt.Ta
-0000df40: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
-0000df50: 2874 6578 7477 7261 702e 6465 6465 6e74  (textwrap.dedent
-0000df60: 2822 2222 5c0a 2020 2020 2020 2020 2020  ("""\.          
-0000df70: 2020 612c 620a 2020 2020 2020 2020 2020    a,b.          
-0000df80: 2020 3130 2c31 3030 0a20 2020 2020 2020    10,100.       
-0000df90: 2020 2020 2032 302c 3230 300a 2020 2020       20,200.    
-0000dfa0: 2020 2020 2020 2020 2222 2229 290a 2020          """)).  
-0000dfb0: 2020 2020 2020 7461 626c 652e 7072 6573        table.pres
-0000dfc0: 656e 7428 290a 2020 2020 2020 2020 6f75  ent().        ou
-0000dfd0: 7420 3d20 5374 7269 6e67 494f 2829 0a20  t = StringIO(). 
-0000dfe0: 2020 2020 2020 2074 6162 6c65 2e70 7265         table.pre
-0000dff0: 7365 6e74 2866 696c 653d 6f75 742c 2062  sent(file=out, b
-0000e000: 6f78 3d62 6f78 2e41 5343 4949 290a 2020  ox=box.ASCII).  
-0000e010: 2020 2020 2020 6578 7065 6374 6564 203d        expected =
-0000e020: 2074 6578 7477 7261 702e 6465 6465 6e74   textwrap.dedent
-0000e030: 2822 2222 5c0a 2020 2020 2020 2020 2020  ("""\.          
-0000e040: 2020 2b2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a20    +----------+. 
-0000e050: 2020 2020 2020 2020 2020 207c 2041 2020             | A  
-0000e060: 7c20 4220 2020 7c0a 2020 2020 2020 2020  | B   |.        
-0000e070: 2020 2020 7c2d 2d2d 2d2b 2d2d 2d2d 2d7c      |----+-----|
-0000e080: 0a20 2020 2020 2020 2020 2020 207c 2031  .            | 1
-0000e090: 3020 7c20 3130 3020 7c0a 2020 2020 2020  0 | 100 |.      
-0000e0a0: 2020 2020 2020 7c20 3230 207c 2032 3030        | 20 | 200
-0000e0b0: 207c 0a20 2020 2020 2020 2020 2020 202b   |.            +
-0000e0c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  ----------+.    
-0000e0d0: 2020 2020 2020 2020 2222 2229 0a20 2020          """).   
-0000e0e0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-0000e0f0: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
-0000e100: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000e110: 7445 7175 616c 2865 7870 6563 7465 642c  tEqual(expected,
-0000e120: 206f 7574 2e67 6574 7661 6c75 6528 2929   out.getvalue())
-0000e130: 0a0a 2020 2020 2020 2020 2320 7465 7374  ..        # test
-0000e140: 2062 7567 6669 7820 7768 656e 2074 6162   bugfix when tab
-0000e150: 6c65 2068 6173 2061 7474 7269 6275 7465  le has attribute
-0000e160: 2022 6465 6661 756c 7422 0a20 2020 2020   "default".     
-0000e170: 2020 2074 6162 6c65 203d 206c 742e 5461     table = lt.Ta
-0000e180: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
-0000e190: 2874 6578 7477 7261 702e 6465 6465 6e74  (textwrap.dedent
-0000e1a0: 2822 2222 5c0a 2020 2020 2020 2020 2020  ("""\.          
-0000e1b0: 2020 612c 622c 6465 6661 756c 740a 2020    a,b,default.  
-0000e1c0: 2020 2020 2020 2020 2020 3130 2c31 3030            10,100
-0000e1d0: 2c70 7572 706c 650a 2020 2020 2020 2020  ,purple.        
-0000e1e0: 2020 2020 3135 2c31 3530 2c0a 2020 2020      15,150,.    
-0000e1f0: 2020 2020 2020 2020 3230 2c32 3030 2c6f          20,200,o
-0000e200: 7261 6e67 650a 2020 2020 2020 2020 2020  range.          
-0000e210: 2020 2222 2229 290a 2020 2020 2020 2020    """)).        
-0000e220: 7461 626c 652e 7072 6573 656e 7428 290a  table.present().
-0000e230: 2020 2020 2020 2020 6f75 7420 3d20 5374          out = St
-0000e240: 7269 6e67 494f 2829 0a20 2020 2020 2020  ringIO().       
-0000e250: 2074 6162 6c65 2e70 7265 7365 6e74 2866   table.present(f
-0000e260: 696c 653d 6f75 742c 2062 6f78 3d62 6f78  ile=out, box=box
-0000e270: 2e41 5343 4949 290a 2020 2020 2020 2020  .ASCII).        
-0000e280: 6578 7065 6374 6564 203d 2074 6578 7477  expected = textw
-0000e290: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
-0000e2a0: 2020 2020 2020 2020 2020 2020 2b2d 2d2d              +---
-0000e2b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000e2c0: 2d2b 0a20 2020 2020 2020 2020 2020 207c  -+.            |
-0000e2d0: 2041 2020 7c20 4220 2020 7c20 4465 6661   A  | B   | Defa
-0000e2e0: 756c 7420 7c0a 2020 2020 2020 2020 2020  ult |.          
-0000e2f0: 2020 7c2d 2d2d 2d2b 2d2d 2d2d 2d2b 2d2d    |----+-----+--
-0000e300: 2d2d 2d2d 2d2d 2d7c 0a20 2020 2020 2020  -------|.       
-0000e310: 2020 2020 207c 2031 3020 7c20 3130 3020       | 10 | 100 
-0000e320: 7c20 7075 7270 6c65 2020 7c0a 2020 2020  | purple  |.    
-0000e330: 2020 2020 2020 2020 7c20 3135 207c 2031          | 15 | 1
-0000e340: 3530 207c 2020 2020 2020 2020 207c 0a20  50 |         |. 
-0000e350: 2020 2020 2020 2020 2020 207c 2032 3020             | 20 
-0000e360: 7c20 3230 3020 7c20 6f72 616e 6765 2020  | 200 | orange  
-0000e370: 7c0a 2020 2020 2020 2020 2020 2020 2b2d  |.            +-
-0000e380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000e390: 2d2d 2d2b 0a20 2020 2020 2020 2020 2020  ---+.           
-0000e3a0: 2022 2222 290a 2020 2020 2020 2020 7769   """).        wi
-0000e3b0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-0000e3c0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000e3d0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000e3e0: 6578 7065 6374 6564 2c20 6f75 742e 6765  expected, out.ge
-0000e3f0: 7476 616c 7565 2829 290a 0a20 2020 2020  tvalue())..     
-0000e400: 2020 2023 2074 6573 7420 6772 6f75 7062     # test groupb
-0000e410: 790a 2020 2020 2020 2020 7461 626c 6520  y.        table 
-0000e420: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
-0000e430: 5f69 6d70 6f72 7428 7465 7874 7772 6170  _import(textwrap
-0000e440: 2e64 6564 656e 7428 2222 225c 0a20 2020  .dedent("""\.   
-0000e450: 2020 2020 2020 2020 2061 2c62 2c64 6566           a,b,def
-0000e460: 6175 6c74 0a20 2020 2020 2020 2020 2020  ault.           
-0000e470: 2031 302c 3130 302c 7075 7270 6c65 0a20   10,100,purple. 
-0000e480: 2020 2020 2020 2020 2020 2031 352c 3135             15,15
-0000e490: 302c 7075 7270 6c65 0a20 2020 2020 2020  0,purple.       
-0000e4a0: 2020 2020 2032 302c 3230 302c 6f72 616e       20,200,oran
-0000e4b0: 6765 0a20 2020 2020 2020 2020 2020 2022  ge.            "
-0000e4c0: 2222 2929 0a20 2020 2020 2020 2074 6162  "")).        tab
-0000e4d0: 6c65 2e70 7265 7365 6e74 2829 0a20 2020  le.present().   
-0000e4e0: 2020 2020 2074 6162 6c65 2e70 7265 7365       table.prese
-0000e4f0: 6e74 2862 6f78 3d62 6f78 2e41 5343 4949  nt(box=box.ASCII
-0000e500: 2c20 6772 6f75 7062 793d 2264 6566 6175  , groupby="defau
-0000e510: 6c74 2229 0a20 2020 2020 2020 206f 7574  lt").        out
-0000e520: 203d 2053 7472 696e 6749 4f28 290a 2020   = StringIO().  
-0000e530: 2020 2020 2020 7461 626c 652e 7072 6573        table.pres
-0000e540: 656e 7428 6669 6c65 3d6f 7574 2c20 626f  ent(file=out, bo
-0000e550: 783d 626f 782e 4153 4349 492c 2067 726f  x=box.ASCII, gro
-0000e560: 7570 6279 3d22 6465 6661 756c 7422 290a  upby="default").
-0000e570: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-0000e580: 203d 2074 6578 7477 7261 702e 6465 6465   = textwrap.dede
-0000e590: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
-0000e5a0: 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d      +-----------
-0000e5b0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a20 2020 2020  ---------+.     
-0000e5c0: 2020 2020 2020 207c 2041 2020 7c20 4220         | A  | B 
-0000e5d0: 2020 7c20 4465 6661 756c 7420 7c0a 2020    | Default |.  
-0000e5e0: 2020 2020 2020 2020 2020 7c2d 2d2d 2d2b            |----+
-0000e5f0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d7c  -----+---------|
-0000e600: 0a20 2020 2020 2020 2020 2020 207c 2031  .            | 1
-0000e610: 3020 7c20 3130 3020 7c20 7075 7270 6c65  0 | 100 | purple
-0000e620: 2020 7c0a 2020 2020 2020 2020 2020 2020    |.            
-0000e630: 7c20 3135 207c 2031 3530 207c 2020 2020  | 15 | 150 |    
-0000e640: 2020 2020 207c 0a20 2020 2020 2020 2020       |.         
-0000e650: 2020 207c 2032 3020 7c20 3230 3020 7c20     | 20 | 200 | 
-0000e660: 6f72 616e 6765 2020 7c0a 2020 2020 2020  orange  |.      
-0000e670: 2020 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2d        +---------
-0000e680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a20 2020  -----------+.   
-0000e690: 2020 2020 2020 2020 2022 2222 290a 2020           """).  
-0000e6a0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0000e6b0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-0000e6c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000e6d0: 7274 4571 7561 6c28 6578 7065 6374 6564  rtEqual(expected
-0000e6e0: 2c20 6f75 742e 6765 7476 616c 7565 2829  , out.getvalue()
-0000e6f0: 290a 0a20 2020 2020 2020 2074 6162 6c65  )..        table
-0000e700: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
-0000e710: 765f 696d 706f 7274 2874 6578 7477 7261  v_import(textwra
-0000e720: 702e 6465 6465 6e74 2822 2222 5c0a 2020  p.dedent("""\.  
-0000e730: 2020 2020 2020 2020 2020 612c 622c 6465            a,b,de
-0000e740: 6661 756c 740a 2020 2020 2020 2020 2020  fault.          
-0000e750: 2020 3130 2c31 3030 2c70 7572 706c 650a    10,100,purple.
-0000e760: 2020 2020 2020 2020 2020 2020 3135 2c31              15,1
-0000e770: 3530 2c70 7572 706c 650a 2020 2020 2020  50,purple.      
-0000e780: 2020 2020 2020 3135 2c32 3030 2c6f 7261        15,200,ora
-0000e790: 6e67 650a 2020 2020 2020 2020 2020 2020  nge.            
-0000e7a0: 3135 2c32 3530 2c6f 7261 6e67 650a 2020  15,250,orange.  
-0000e7b0: 2020 2020 2020 2020 2020 3230 2c32 3530            20,250
-0000e7c0: 2c6f 7261 6e67 650a 2020 2020 2020 2020  ,orange.        
-0000e7d0: 2020 2020 2222 2229 290a 2020 2020 2020      """)).      
-0000e7e0: 2020 7461 626c 652e 7072 6573 656e 7428    table.present(
-0000e7f0: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
-0000e800: 7072 6573 656e 7428 626f 783d 626f 782e  present(box=box.
-0000e810: 4153 4349 492c 2067 726f 7570 6279 3d22  ASCII, groupby="
-0000e820: 6465 6661 756c 7420 6122 290a 2020 2020  default a").    
-0000e830: 2020 2020 6f75 7420 3d20 5374 7269 6e67      out = String
-0000e840: 494f 2829 0a20 2020 2020 2020 2074 6162  IO().        tab
-0000e850: 6c65 2e70 7265 7365 6e74 2866 696c 653d  le.present(file=
-0000e860: 6f75 742c 2062 6f78 3d62 6f78 2e41 5343  out, box=box.ASC
-0000e870: 4949 2c20 6772 6f75 7062 793d 2264 6566  II, groupby="def
-0000e880: 6175 6c74 2061 2229 0a20 2020 2020 2020  ault a").       
-0000e890: 2065 7870 6563 7465 6420 3d20 7465 7874   expected = text
-0000e8a0: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
-0000e8b0: 0a20 2020 2020 2020 2020 2020 202b 2d2d  .            +--
-0000e8c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000e8d0: 2d2d 2b0a 2020 2020 2020 2020 2020 2020  --+.            
-0000e8e0: 7c20 4120 207c 2042 2020 207c 2044 6566  | A  | B   | Def
-0000e8f0: 6175 6c74 207c 0a20 2020 2020 2020 2020  ault |.         
-0000e900: 2020 207c 2d2d 2d2d 2b2d 2d2d 2d2d 2b2d     |----+-----+-
-0000e910: 2d2d 2d2d 2d2d 2d2d 7c0a 2020 2020 2020  --------|.      
-0000e920: 2020 2020 2020 7c20 3130 207c 2031 3030        | 10 | 100
-0000e930: 207c 2070 7572 706c 6520 207c 0a20 2020   | purple  |.   
-0000e940: 2020 2020 2020 2020 207c 2031 3520 7c20           | 15 | 
-0000e950: 3135 3020 7c20 2020 2020 2020 2020 7c0a  150 |         |.
-0000e960: 2020 2020 2020 2020 2020 2020 7c20 3135              | 15
-0000e970: 207c 2032 3030 207c 206f 7261 6e67 6520   | 200 | orange 
-0000e980: 207c 0a20 2020 2020 2020 2020 2020 207c   |.            |
-0000e990: 2020 2020 7c20 3235 3020 7c20 2020 2020      | 250 |     
-0000e9a0: 2020 2020 7c0a 2020 2020 2020 2020 2020      |.          
-0000e9b0: 2020 7c20 3230 207c 2032 3530 207c 2020    | 20 | 250 |  
-0000e9c0: 2020 2020 2020 207c 0a20 2020 2020 2020         |.       
-0000e9d0: 2020 2020 202b 2d2d 2d2d 2d2d 2d2d 2d2d       +----------
-0000e9e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  ----------+.    
-0000e9f0: 2020 2020 2020 2020 2222 2229 0a20 2020          """).   
-0000ea00: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-0000ea10: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
-0000ea20: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000ea30: 7445 7175 616c 2865 7870 6563 7465 642c  tEqual(expected,
-0000ea40: 206f 7574 2e67 6574 7661 6c75 6528 2929   out.getvalue())
-0000ea50: 0a0a 2020 2020 2020 2020 7461 626c 6520  ..        table 
-0000ea60: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
-0000ea70: 5f69 6d70 6f72 7428 7465 7874 7772 6170  _import(textwrap
-0000ea80: 2e64 6564 656e 7428 2222 225c 0a20 2020  .dedent("""\.   
-0000ea90: 2020 2020 2020 2020 2061 2c62 2c64 6566           a,b,def
-0000eaa0: 6175 6c74 0a20 2020 2020 2020 2020 2020  ault.           
-0000eab0: 2031 302c 3130 302c 7075 7270 6c65 0a20   10,100,purple. 
-0000eac0: 2020 2020 2020 2020 2020 2031 352c 3230             15,20
-0000ead0: 302c 6f72 616e 6765 0a20 2020 2020 2020  0,orange.       
-0000eae0: 2020 2020 2031 352c 3135 302c 7075 7270       15,150,purp
-0000eaf0: 6c65 0a20 2020 2020 2020 2020 2020 2032  le.            2
-0000eb00: 302c 3235 302c 6f72 616e 6765 0a20 2020  0,250,orange.   
-0000eb10: 2020 2020 2020 2020 2031 352c 3235 302c           15,250,
-0000eb20: 6f72 616e 6765 0a20 2020 2020 2020 2020  orange.         
-0000eb30: 2020 2022 2222 2929 0a20 2020 2020 2020     """)).       
-0000eb40: 2074 6162 6c65 2e73 6f72 7428 2264 6566   table.sort("def
-0000eb50: 6175 6c74 2064 6573 632c 6122 290a 2020  ault desc,a").  
-0000eb60: 2020 2020 2020 7461 626c 652e 7072 6573        table.pres
-0000eb70: 656e 7428 290a 2020 2020 2020 2020 7461  ent().        ta
-0000eb80: 626c 652e 7072 6573 656e 7428 626f 783d  ble.present(box=
-0000eb90: 626f 782e 4153 4349 492c 2067 726f 7570  box.ASCII, group
-0000eba0: 6279 3d22 6465 6661 756c 7420 6122 290a  by="default a").
-0000ebb0: 2020 2020 2020 2020 6f75 7420 3d20 5374          out = St
-0000ebc0: 7269 6e67 494f 2829 0a20 2020 2020 2020  ringIO().       
-0000ebd0: 2074 6162 6c65 2e70 7265 7365 6e74 2866   table.present(f
-0000ebe0: 696c 653d 6f75 742c 2062 6f78 3d62 6f78  ile=out, box=box
-0000ebf0: 2e41 5343 4949 2c20 6772 6f75 7062 793d  .ASCII, groupby=
-0000ec00: 2264 6566 6175 6c74 2061 2229 0a20 2020  "default a").   
-0000ec10: 2020 2020 2065 7870 6563 7465 6420 3d20       expected = 
-0000ec20: 7465 7874 7772 6170 2e64 6564 656e 7428  textwrap.dedent(
-0000ec30: 2222 225c 0a20 2020 2020 2020 2020 2020  """\.           
-0000ec40: 202b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   +--------------
-0000ec50: 2d2d 2d2d 2d2d 2b0a 2020 2020 2020 2020  ------+.        
-0000ec60: 2020 2020 7c20 4120 207c 2042 2020 207c      | A  | B   |
-0000ec70: 2044 6566 6175 6c74 207c 0a20 2020 2020   Default |.     
-0000ec80: 2020 2020 2020 207c 2d2d 2d2d 2b2d 2d2d         |----+---
-0000ec90: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020  --+---------|.  
-0000eca0: 2020 2020 2020 2020 2020 7c20 3130 207c            | 10 |
-0000ecb0: 2031 3030 207c 2070 7572 706c 6520 207c   100 | purple  |
-0000ecc0: 0a20 2020 2020 2020 2020 2020 207c 2031  .            | 1
-0000ecd0: 3520 7c20 3135 3020 7c20 2020 2020 2020  5 | 150 |       
-0000ece0: 2020 7c0a 2020 2020 2020 2020 2020 2020    |.            
-0000ecf0: 7c20 3135 207c 2032 3030 207c 206f 7261  | 15 | 200 | ora
-0000ed00: 6e67 6520 207c 0a20 2020 2020 2020 2020  nge  |.         
-0000ed10: 2020 207c 2020 2020 7c20 3235 3020 7c20     |    | 250 | 
-0000ed20: 2020 2020 2020 2020 7c0a 2020 2020 2020          |.      
-0000ed30: 2020 2020 2020 7c20 3230 207c 2032 3530        | 20 | 250
-0000ed40: 207c 2020 2020 2020 2020 207c 0a20 2020   |         |.   
-0000ed50: 2020 2020 2020 2020 202b 2d2d 2d2d 2d2d           +------
-0000ed60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a  --------------+.
-0000ed70: 2020 2020 2020 2020 2020 2020 2222 2229              """)
-0000ed80: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000ed90: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-0000eda0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000edb0: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
-0000edc0: 7465 642c 206f 7574 2e67 6574 7661 6c75  ted, out.getvalu
-0000edd0: 6528 2929 0a0a 2020 2020 6465 6620 7465  e())..    def te
-0000ede0: 7374 5f6d 6172 6b64 6f77 6e28 7365 6c66  st_markdown(self
-0000edf0: 293a 0a20 2020 2020 2020 2074 6162 6c65  ):.        table
-0000ee00: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
-0000ee10: 765f 696d 706f 7274 2874 6578 7477 7261  v_import(textwra
-0000ee20: 702e 6465 6465 6e74 2822 2222 5c0a 2020  p.dedent("""\.  
-0000ee30: 2020 2020 2020 2020 2020 612c 620a 2020            a,b.  
-0000ee40: 2020 2020 2020 2020 2020 3130 2c31 3030            10,100
-0000ee50: 0a20 2020 2020 2020 2020 2020 2032 302c  .            20,
-0000ee60: 3230 300a 2020 2020 2020 2020 2020 2020  200.            
-0000ee70: 2222 2229 290a 2020 2020 2020 2020 6f75  """)).        ou
-0000ee80: 745f 6d61 726b 646f 776e 203d 2074 6162  t_markdown = tab
-0000ee90: 6c65 2e61 735f 6d61 726b 646f 776e 2829  le.as_markdown()
-0000eea0: 0a20 2020 2020 2020 2070 7269 6e74 286f  .        print(o
-0000eeb0: 7574 5f6d 6172 6b64 6f77 6e29 0a20 2020  ut_markdown).   
-0000eec0: 2020 2020 2065 7870 6563 7465 6420 3d20       expected = 
+00009950: 2027 3c74 643e 3c64 6976 2061 6c69 676e   '<td><div align
+00009960: 3d22 7269 6768 7422 3e30 3c2f 6469 763e  ="right">0</div>
+00009970: 3c2f 7464 3e3c 2f74 723e 272c 0a20 2020  </td></tr>',.   
+00009980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009990: 2020 2020 2020 6461 7461 5f6c 696e 652c        data_line,
+000099a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000099b0: 2020 2020 2020 2020 2020 2266 6169 6c65            "faile
+000099c0: 6420 6173 5f68 746d 6c20 7769 7468 206e  d as_html with n
+000099d0: 616d 6564 2066 6965 6c64 2066 6f72 6d61  amed field forma
+000099e0: 7420 666f 7220 7370 6563 6966 6963 2066  t for specific f
+000099f0: 6965 6c64 2229 0a0a 2020 2020 2020 2020  ield")..        
+00009a00: 6874 6d6c 5f6f 7574 7075 7420 3d20 7365  html_output = se
+00009a10: 6c66 2e74 315b 3a31 305d 2e61 735f 6874  lf.t1[:10].as_ht
+00009a20: 6d6c 2866 6965 6c64 733d 2261 2062 2063  ml(fields="a b c
+00009a30: 222c 2066 6f72 6d61 7473 3d7b 696e 743a  ", formats={int:
+00009a40: 2022 7b3a 3033 647d 227d 290a 2020 2020   "{:03d}"}).    
+00009a50: 2020 2020 7072 696e 7428 6874 6d6c 5f6f      print(html_o
+00009a60: 7574 7075 7429 0a20 2020 2020 2020 2068  utput).        h
+00009a70: 746d 6c5f 6c69 6e65 7320 3d20 6874 6d6c  tml_lines = html
+00009a80: 5f6f 7574 7075 742e 7370 6c69 746c 696e  _output.splitlin
+00009a90: 6573 2829 0a20 2020 2020 2020 2064 6174  es().        dat
+00009aa0: 615f 6c69 6e65 203d 206e 6578 7428 6820  a_line = next(h 
+00009ab0: 666f 7220 6820 696e 2068 746d 6c5f 6c69  for h in html_li
+00009ac0: 6e65 7320 6966 2022 3c74 643e 2220 696e  nes if "<td>" in
+00009ad0: 2068 290a 2020 2020 2020 2020 7365 6c66   h).        self
+00009ae0: 2e61 7373 6572 7445 7175 616c 2827 3c74  .assertEqual('<t
+00009af0: 626f 6479 3e3c 7472 3e3c 7464 3e3c 6469  body><tr><td><di
+00009b00: 7620 616c 6967 6e3d 2272 6967 6874 223e  v align="right">
+00009b10: 3030 303c 2f64 6976 3e3c 2f74 643e 270a  000</div></td>'.
+00009b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b30: 2020 2020 2020 2020 2027 3c74 643e 3c64           '<td><d
+00009b40: 6976 2061 6c69 676e 3d22 7269 6768 7422  iv align="right"
+00009b50: 3e30 3030 3c2f 6469 763e 3c2f 7464 3e27  >000</div></td>'
+00009b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009b70: 2020 2020 2020 2020 2020 273c 7464 3e3c            '<td><
+00009b80: 6469 7620 616c 6967 6e3d 2272 6967 6874  div align="right
+00009b90: 223e 3030 303c 2f64 6976 3e3c 2f74 643e  ">000</div></td>
+00009ba0: 3c2f 7472 3e27 2c0a 2020 2020 2020 2020  </tr>',.        
+00009bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bc0: 2064 6174 615f 6c69 6e65 2c0a 2020 2020   data_line,.    
+00009bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009be0: 2020 2020 2022 6661 696c 6564 2061 735f       "failed as_
+00009bf0: 6874 6d6c 2077 6974 6820 6461 7461 2074  html with data t
+00009c00: 7970 6520 666f 726d 6174 2066 6f72 2061  ype format for a
+00009c10: 6c6c 2066 6965 6c64 7322 290a 0a20 2020  ll fields")..   
+00009c20: 2020 2020 2068 746d 6c5f 6f75 7470 7574       html_output
+00009c30: 203d 2073 656c 662e 7431 5b3a 3130 5d2e   = self.t1[:10].
+00009c40: 6173 5f68 746d 6c28 6669 656c 6473 3d22  as_html(fields="
+00009c50: 6120 6220 6322 2c20 666f 726d 6174 733d  a b c", formats=
+00009c60: 7b69 6e74 3a20 227b 3a30 3364 7d22 7d2c  {int: "{:03d}"},
+00009c70: 2067 726f 7570 6279 3d22 6122 290a 2020   groupby="a").  
+00009c80: 2020 2020 2020 7072 696e 7428 6874 6d6c        print(html
+00009c90: 5f6f 7574 7075 7429 0a20 2020 2020 2020  _output).       
+00009ca0: 2068 746d 6c5f 6c69 6e65 7320 3d20 6874   html_lines = ht
+00009cb0: 6d6c 5f6f 7574 7075 742e 7370 6c69 746c  ml_output.splitl
+00009cc0: 696e 6573 2829 0a20 2020 2020 2020 2064  ines().        d
+00009cd0: 6174 615f 6c69 6e65 203d 206e 6578 7428  ata_line = next(
+00009ce0: 6820 666f 7220 6820 696e 2068 746d 6c5f  h for h in html_
+00009cf0: 6c69 6e65 7320 6966 2022 3c74 643e 2220  lines if "<td>" 
+00009d00: 696e 2068 290a 2020 2020 2020 2020 7365  in h).        se
+00009d10: 6c66 2e61 7373 6572 7445 7175 616c 2827  lf.assertEqual('
+00009d20: 3c74 626f 6479 3e3c 7472 3e3c 7464 3e3c  <tbody><tr><td><
+00009d30: 6469 7620 616c 6967 6e3d 2272 6967 6874  div align="right
+00009d40: 223e 3030 303c 2f64 6976 3e3c 2f74 643e  ">000</div></td>
+00009d50: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00009d60: 2020 2020 2020 2020 2020 2027 3c74 643e             '<td>
+00009d70: 3c64 6976 2061 6c69 676e 3d22 7269 6768  <div align="righ
+00009d80: 7422 3e30 3030 3c2f 6469 763e 3c2f 7464  t">000</div></td
+00009d90: 3e27 0a20 2020 2020 2020 2020 2020 2020  >'.             
+00009da0: 2020 2020 2020 2020 2020 2020 273c 7464              '<td
+00009db0: 3e3c 6469 7620 616c 6967 6e3d 2272 6967  ><div align="rig
+00009dc0: 6874 223e 3030 303c 2f64 6976 3e3c 2f74  ht">000</div></t
+00009dd0: 643e 3c2f 7472 3e27 2c0a 2020 2020 2020  d></tr>',.      
+00009de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009df0: 2020 2064 6174 615f 6c69 6e65 2c0a 2020     data_line,.  
+00009e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e10: 2020 2020 2020 2022 6661 696c 6564 2061         "failed a
+00009e20: 735f 6874 6d6c 2077 6974 6820 6772 6f75  s_html with grou
+00009e30: 7062 7922 290a 0a20 2020 2020 2020 2068  pby")..        h
+00009e40: 746d 6c5f 6f75 7470 7574 203d 2073 656c  tml_output = sel
+00009e50: 662e 7431 5b3a 3130 5d2e 6173 5f68 746d  f.t1[:10].as_htm
+00009e60: 6c28 6669 656c 6473 3d22 6120 6220 6322  l(fields="a b c"
+00009e70: 2c20 7461 626c 655f 7072 6f70 6572 7469  , table_properti
+00009e80: 6573 3d7b 2262 6f72 6465 7222 3a20 2232  es={"border": "2
+00009e90: 227d 290a 2020 2020 2020 2020 7072 696e  "}).        prin
+00009ea0: 7428 6874 6d6c 5f6f 7574 7075 7429 0a20  t(html_output). 
+00009eb0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00009ec0: 7274 5472 7565 2822 3c74 6865 6164 3e22  rtTrue("<thead>"
+00009ed0: 2069 6e20 6874 6d6c 5f6f 7574 7075 7420   in html_output 
+00009ee0: 616e 6420 223c 7462 6f64 793e 2220 696e  and "<tbody>" in
+00009ef0: 2068 746d 6c5f 6f75 7470 7574 2c0a 2020   html_output,.  
+00009f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f10: 2020 2020 2020 2261 735f 6874 6d6c 2064        "as_html d
+00009f20: 6f65 7320 6e6f 7420 696e 636c 7564 6520  oes not include 
+00009f30: 7468 6561 6420 616e 6420 7462 6f64 7920  thead and tbody 
+00009f40: 7461 6773 2229 0a0a 0a20 2020 2064 6566  tags")...    def
+00009f50: 2074 6573 745f 6465 6c65 7465 5f73 6c69   test_delete_sli
+00009f60: 6365 7328 7365 6c66 293a 0a20 2020 2020  ces(self):.     
+00009f70: 2020 2063 6f6d 7061 7265 5f6c 6973 7420     compare_list 
+00009f80: 3d20 6c69 7374 2822 4142 4344 4546 4748  = list("ABCDEFGH
+00009f90: 494a 4b4c 4d4e 4f50 5152 5354 5556 5758  IJKLMNOPQRSTUVWX
+00009fa0: 595a 3031 3233 3435 3637 3839 6162 6364  YZ0123456789abcd
+00009fb0: 6566 6768 696a 6b6c 6d6e 6f70 7172 7374  efghijklmnopqrst
+00009fc0: 7576 7778 797a 2229 0a20 2020 2020 2020  uvwxyz").       
+00009fd0: 2074 3120 3d20 6c74 2e54 6162 6c65 2829   t1 = lt.Table()
+00009fe0: 2e69 6e73 6572 745f 6d61 6e79 286c 742e  .insert_many(lt.
+00009ff0: 4461 7461 4f62 6a65 6374 2841 3d63 2920  DataObject(A=c) 
+0000a000: 666f 7220 6320 696e 2063 6f6d 7061 7265  for c in compare
+0000a010: 5f6c 6973 7429 0a0a 2020 2020 2020 2020  _list)..        
+0000a020: 6465 6620 6d69 6e69 5f74 6573 7428 736c  def mini_test(sl
+0000a030: 635f 7475 706c 6529 3a0a 2020 2020 2020  c_tuple):.      
+0000a040: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0000a050: 6e63 6528 736c 635f 7475 706c 652c 2074  nce(slc_tuple, t
+0000a060: 7570 6c65 293a 0a20 2020 2020 2020 2020  uple):.         
+0000a070: 2020 2020 2020 206c 6162 656c 203d 2022         label = "
+0000a080: 5b7b 7d3a 7b7d 3a7b 7d5d 222e 666f 726d  [{}:{}:{}]".form
+0000a090: 6174 282a 2869 2069 6620 6920 6973 206e  at(*(i if i is n
+0000a0a0: 6f74 204e 6f6e 6520 656c 7365 2027 2720  ot None else '' 
+0000a0b0: 666f 7220 6920 696e 2073 6c63 5f74 7570  for i in slc_tup
+0000a0c0: 6c65 2929 0a20 2020 2020 2020 2020 2020  le)).           
+0000a0d0: 2020 2020 2073 6c63 203d 2073 6c69 6365       slc = slice
+0000a0e0: 282a 736c 635f 7475 706c 6529 0a20 2020  (*slc_tuple).   
+0000a0f0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000a100: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000a110: 6162 656c 203d 2073 7472 2873 6c63 5f74  abel = str(slc_t
+0000a120: 7570 6c65 290a 2020 2020 2020 2020 2020  uple).          
+0000a130: 2020 2020 2020 736c 6320 3d20 736c 635f        slc = slc_
+0000a140: 7475 706c 650a 0a20 2020 2020 2020 2020  tuple..         
+0000a150: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+0000a160: 5465 7374 286c 6162 656c 2c20 736c 635f  Test(label, slc_
+0000a170: 7475 706c 653d 736c 635f 7475 706c 6529  tuple=slc_tuple)
+0000a180: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000a190: 2020 6465 6c20 636f 6d70 6172 655f 6c69    del compare_li
+0000a1a0: 7374 5b73 6c63 5d0a 2020 2020 2020 2020  st[slc].        
+0000a1b0: 2020 2020 2020 2020 7072 696e 7428 6c61          print(la
+0000a1c0: 6265 6c29 0a20 2020 2020 2020 2020 2020  bel).           
+0000a1d0: 2020 2020 2070 7269 6e74 2827 4578 7065       print('Expe
+0000a1e0: 6374 6564 272c 2063 6f6d 7061 7265 5f6c  cted', compare_l
+0000a1f0: 6973 7429 0a20 2020 2020 2020 2020 2020  ist).           
+0000a200: 2020 2020 2064 656c 2074 315b 736c 635d       del t1[slc]
+0000a210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a220: 2070 7269 6e74 2827 4f62 7365 7276 6564   print('Observed
+0000a230: 272c 206c 6973 7428 7431 2e61 6c6c 2e41  ', list(t1.all.A
+0000a240: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+0000a250: 2020 2070 7269 6e74 2829 0a20 2020 2020     print().     
+0000a260: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a270: 6173 7365 7274 4571 7561 6c28 2727 2e6a  assertEqual(''.j
+0000a280: 6f69 6e28 636f 6d70 6172 655f 6c69 7374  oin(compare_list
+0000a290: 292c 2027 272e 6a6f 696e 2874 312e 616c  ), ''.join(t1.al
+0000a2a0: 6c2e 4129 2c20 2266 6169 6c65 6420 2220  l.A), "failed " 
+0000a2b0: 2b20 6c61 6265 6c29 0a0a 2020 2020 2020  + label)..      
+0000a2c0: 2020 6d69 6e69 5f74 6573 7428 3529 0a20    mini_test(5). 
+0000a2d0: 2020 2020 2020 206d 696e 695f 7465 7374         mini_test
+0000a2e0: 282d 3529 0a20 2020 2020 2020 206d 696e  (-5).        min
+0000a2f0: 695f 7465 7374 2828 2d35 2c20 4e6f 6e65  i_test((-5, None
+0000a300: 2c20 4e6f 6e65 2929 0a20 2020 2020 2020  , None)).       
+0000a310: 206d 696e 695f 7465 7374 2828 4e6f 6e65   mini_test((None
+0000a320: 2c20 332c 204e 6f6e 6529 290a 2020 2020  , 3, None)).    
+0000a330: 2020 2020 6d69 6e69 5f74 6573 7428 284e      mini_test((N
+0000a340: 6f6e 652c 202d 6c65 6e28 636f 6d70 6172  one, -len(compar
+0000a350: 655f 6c69 7374 292b 332c 204e 6f6e 6529  e_list)+3, None)
+0000a360: 290a 2020 2020 2020 2020 6d69 6e69 5f74  ).        mini_t
+0000a370: 6573 7428 284e 6f6e 652c 204e 6f6e 652c  est((None, None,
+0000a380: 2035 2929 0a20 2020 2020 2020 206d 696e   5)).        min
+0000a390: 695f 7465 7374 2828 4e6f 6e65 2c20 4e6f  i_test((None, No
+0000a3a0: 6e65 2c20 2d35 2929 0a20 2020 2020 2020  ne, -5)).       
+0000a3b0: 206d 696e 695f 7465 7374 2828 2d35 2c20   mini_test((-5, 
+0000a3c0: 2d32 2c20 4e6f 6e65 2929 0a20 2020 2020  -2, None)).     
+0000a3d0: 2020 206d 696e 695f 7465 7374 2828 2d32     mini_test((-2
+0000a3e0: 2c20 2d35 2c20 2d31 2929 0a20 2020 2020  , -5, -1)).     
+0000a3f0: 2020 206d 696e 695f 7465 7374 2828 352c     mini_test((5,
+0000a400: 2032 302c 2032 2929 0a20 2020 2020 2020   20, 2)).       
+0000a410: 206d 696e 695f 7465 7374 2828 6c65 6e28   mini_test((len(
+0000a420: 636f 6d70 6172 655f 6c69 7374 292c 2035  compare_list), 5
+0000a430: 2c20 2d33 2929 0a20 2020 2020 2020 206d  , -3)).        m
+0000a440: 696e 695f 7465 7374 2828 3230 2c20 3131  ini_test((20, 11
+0000a450: 2c20 2d37 2929 0a20 2020 2020 2020 206d  , -7)).        m
+0000a460: 696e 695f 7465 7374 2828 352c 2035 2c20  ini_test((5, 5, 
+0000a470: 4e6f 6e65 2929 0a20 2020 2020 2020 206d  None)).        m
+0000a480: 696e 695f 7465 7374 2828 4e6f 6e65 2c20  ini_test((None, 
+0000a490: 2d31 302c 2035 2929 0a20 2020 2020 2020  -10, 5)).       
+0000a4a0: 206d 696e 695f 7465 7374 2828 4e6f 6e65   mini_test((None
+0000a4b0: 2c20 2d31 302c 202d 3130 2929 0a20 2020  , -10, -10)).   
+0000a4c0: 2020 2020 206d 696e 695f 7465 7374 2828       mini_test((
+0000a4d0: 3130 3030 2c20 3230 3030 2c20 4e6f 6e65  1000, 2000, None
+0000a4e0: 2929 0a20 2020 2020 2020 206d 696e 695f  )).        mini_
+0000a4f0: 7465 7374 2828 4e6f 6e65 2c20 4e6f 6e65  test((None, None
+0000a500: 2c20 2d31 2929 0a0a 2020 2020 6465 6620  , -1))..    def 
+0000a510: 7465 7374 5f63 6c65 6172 2873 656c 6629  test_clear(self)
+0000a520: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+0000a530: 7465 7374 5f69 6e69 7428 290a 2020 2020  test_init().    
+0000a540: 2020 2020 6e75 6d5f 6669 656c 6473 203d      num_fields =
+0000a550: 206c 656e 2873 656c 662e 7431 2e69 6e66   len(self.t1.inf
+0000a560: 6f28 295b 2266 6965 6c64 7322 5d29 0a20  o()["fields"]). 
+0000a570: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+0000a580: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+0000a590: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000a5a0: 6572 7445 7175 616c 2873 656c 662e 7465  ertEqual(self.te
+0000a5b0: 7374 5f73 697a 6520 2a2a 206e 756d 5f66  st_size ** num_f
+0000a5c0: 6965 6c64 732c 206c 656e 2873 656c 662e  ields, len(self.
+0000a5d0: 7431 292c 2022 696e 7661 6c69 6420 6c65  t1), "invalid le
+0000a5e0: 6e22 290a 2020 2020 2020 2020 7365 6c66  n").        self
+0000a5f0: 2e74 312e 6372 6561 7465 5f69 6e64 6578  .t1.create_index
+0000a600: 2822 6122 290a 0a20 2020 2020 2020 2073  ("a")..        s
+0000a610: 656c 662e 7431 2e63 6c65 6172 2829 0a20  elf.t1.clear(). 
+0000a620: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+0000a630: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+0000a640: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000a650: 6572 7445 7175 616c 2830 2c20 6c65 6e28  ertEqual(0, len(
+0000a660: 7365 6c66 2e74 3129 2c20 2269 6e76 616c  self.t1), "inval
+0000a670: 6964 206c 656e 2061 6674 6572 2063 6c65  id len after cle
+0000a680: 6172 2229 0a20 2020 2020 2020 2077 6974  ar").        wit
+0000a690: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+0000a6a0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000a6b0: 6c66 2e61 7373 6572 7445 7175 616c 2831  lf.assertEqual(1
+0000a6c0: 2c20 6c65 6e28 7365 6c66 2e74 312e 696e  , len(self.t1.in
+0000a6d0: 666f 2829 5b22 696e 6465 7865 7322 5d29  fo()["indexes"])
+0000a6e0: 2c20 2269 6e76 616c 6964 2069 6e64 6578  , "invalid index
+0000a6f0: 6573 2061 6674 6572 2063 6c65 6172 2229  es after clear")
+0000a700: 0a0a 2020 2020 6465 6620 7465 7374 5f73  ..    def test_s
+0000a710: 7461 7473 2873 656c 6629 3a0a 2020 2020  tats(self):.    
+0000a720: 2020 2020 7365 6c66 2e5f 7465 7374 5f69      self._test_i
+0000a730: 6e69 7428 290a 2020 2020 2020 2020 6669  nit().        fi
+0000a740: 656c 645f 6e61 6d65 7320 3d20 7365 6c66  eld_names = self
+0000a750: 2e74 312e 696e 666f 2829 5b22 6669 656c  .t1.info()["fiel
+0000a760: 6473 225d 0a20 2020 2020 2020 206e 756d  ds"].        num
+0000a770: 5f66 6965 6c64 7320 3d20 6c65 6e28 6669  _fields = len(fi
+0000a780: 656c 645f 6e61 6d65 7329 0a20 2020 2020  eld_names).     
+0000a790: 2020 2074 315f 7374 6174 7320 3d20 7365     t1_stats = se
+0000a7a0: 6c66 2e74 312e 7374 6174 7328 292e 7365  lf.t1.stats().se
+0000a7b0: 6c65 6374 2822 6e61 6d65 2063 6f75 6e74  lect("name count
+0000a7c0: 206d 696e 206d 6178 206d 6561 6e22 290a   min max mean").
+0000a7d0: 2020 2020 2020 2020 666f 7220 6669 656c          for fiel
+0000a7e0: 646e 616d 6520 696e 2066 6965 6c64 5f6e  dname in field_n
+0000a7f0: 616d 6573 3a0a 2020 2020 2020 2020 2020  ames:.          
+0000a800: 2020 7374 6174 5f72 6563 203d 2074 315f    stat_rec = t1_
+0000a810: 7374 6174 732e 6279 2e6e 616d 655b 6669  stats.by.name[fi
+0000a820: 656c 646e 616d 655d 0a20 2020 2020 2020  eldname].       
+0000a830: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000a840: 7562 5465 7374 2822 6368 6563 6b20 636f  ubTest("check co
+0000a850: 6d70 7574 6564 2073 7461 7422 2c20 6669  mputed stat", fi
+0000a860: 656c 646e 616d 653d 6669 656c 646e 616d  eldname=fieldnam
+0000a870: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+0000a880: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0000a890: 7175 616c 286c 742e 4461 7461 4f62 6a65  qual(lt.DataObje
+0000a8a0: 6374 286e 616d 653d 6669 656c 646e 616d  ct(name=fieldnam
+0000a8b0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000a8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8e0: 2020 636f 756e 743d 7365 6c66 2e74 6573    count=self.tes
+0000a8f0: 745f 7369 7a65 202a 2a20 6e75 6d5f 6669  t_size ** num_fi
+0000a900: 656c 6473 2c0a 2020 2020 2020 2020 2020  elds,.          
+0000a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a930: 2020 2020 206d 696e 3d30 2c0a 2020 2020       min=0,.    
+0000a940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a960: 2020 2020 2020 2020 2020 206d 6178 3d73             max=s
+0000a970: 656c 662e 7465 7374 5f73 697a 6520 2d20  elf.test_size - 
+0000a980: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
+0000a990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9b0: 2020 6d65 616e 3d28 7365 6c66 2e74 6573    mean=(self.tes
+0000a9c0: 745f 7369 7a65 202d 2031 2920 2f20 3229  t_size - 1) / 2)
+0000a9d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9f0: 2020 2073 7461 745f 7265 632c 0a20 2020     stat_rec,.   
+0000aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa10: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0000aa20: 696e 7661 6c69 6420 7374 6174 2066 6f72  invalid stat for
+0000aa30: 207b 6669 656c 646e 616d 657d 2229 0a0a   {fieldname}")..
+0000aa40: 2020 2020 6465 6620 7465 7374 5f73 7461      def test_sta
+0000aa50: 7473 3228 7365 6c66 293a 0a20 2020 2020  ts2(self):.     
+0000aa60: 2020 2073 656c 662e 5f74 6573 745f 696e     self._test_in
+0000aa70: 6974 2829 0a20 2020 2020 2020 2066 6965  it().        fie
+0000aa80: 6c64 5f6e 616d 6573 203d 2073 656c 662e  ld_names = self.
+0000aa90: 7431 2e69 6e66 6f28 295b 2266 6965 6c64  t1.info()["field
+0000aaa0: 7322 5d0a 2020 2020 2020 2020 6e75 6d5f  s"].        num_
+0000aab0: 6669 656c 6473 203d 206c 656e 2866 6965  fields = len(fie
+0000aac0: 6c64 5f6e 616d 6573 290a 2020 2020 2020  ld_names).      
+0000aad0: 2020 7431 5f73 7461 7473 203d 2073 656c    t1_stats = sel
+0000aae0: 662e 7431 2e73 7461 7473 2862 795f 6669  f.t1.stats(by_fi
+0000aaf0: 656c 643d 4661 6c73 6529 0a20 2020 2020  eld=False).     
+0000ab00: 2020 2066 6f72 2073 7461 742c 2076 616c     for stat, val
+0000ab10: 7565 2069 6e20 2828 276d 696e 272c 2030  ue in (('min', 0
+0000ab20: 292c 2028 276d 6178 272c 2073 656c 662e  ), ('max', self.
+0000ab30: 7465 7374 5f73 697a 6520 2d20 3129 2c20  test_size - 1), 
+0000ab40: 2827 636f 756e 7427 2c20 7365 6c66 2e74  ('count', self.t
+0000ab50: 6573 745f 7369 7a65 202a 2a20 6e75 6d5f  est_size ** num_
+0000ab60: 6669 656c 6473 292c 293a 0a20 2020 2020  fields),):.     
+0000ab70: 2020 2020 2020 2066 6f72 2066 6965 6c64         for field
+0000ab80: 6e61 6d65 2069 6e20 6669 656c 645f 6e61  name in field_na
+0000ab90: 6d65 733a 0a20 2020 2020 2020 2020 2020  mes:.           
+0000aba0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000abb0: 7562 5465 7374 2822 6368 6563 6b20 636f  ubTest("check co
+0000abc0: 6d70 7574 6564 2073 7461 7422 2c20 7374  mputed stat", st
+0000abd0: 6174 3d73 7461 742c 2066 6965 6c64 6e61  at=stat, fieldna
+0000abe0: 6d65 3d66 6965 6c64 6e61 6d65 293a 0a20  me=fieldname):. 
+0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac00: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000ac10: 7561 6c28 7661 6c75 652c 2067 6574 6174  ual(value, getat
+0000ac20: 7472 2874 315f 7374 6174 732e 6279 2e73  tr(t1_stats.by.s
+0000ac30: 7461 745b 7374 6174 5d2c 2066 6965 6c64  tat[stat], field
+0000ac40: 6e61 6d65 292c 0a20 2020 2020 2020 2020  name),.         
+0000ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac60: 2020 2020 2020 2020 6622 696e 7661 6c69          f"invali
+0000ac70: 6420 7b73 7461 747d 2073 7461 7420 666f  d {stat} stat fo
+0000ac80: 7220 7b66 6965 6c64 6e61 6d65 7d22 290a  r {fieldname}").
+0000ac90: 0a20 2020 2064 6566 2074 6573 745f 7374  .    def test_st
+0000aca0: 6174 7333 2873 656c 6629 3a0a 2020 2020  ats3(self):.    
+0000acb0: 2020 2020 7365 6c66 2e5f 7465 7374 5f69      self._test_i
+0000acc0: 6e69 7428 290a 2020 2020 2020 2020 6669  nit().        fi
+0000acd0: 656c 645f 6e61 6d65 7320 3d20 7365 6c66  eld_names = self
+0000ace0: 2e74 312e 696e 666f 2829 5b22 6669 656c  .t1.info()["fiel
+0000acf0: 6473 225d 0a20 2020 2020 2020 206e 756d  ds"].        num
+0000ad00: 5f66 6965 6c64 7320 3d20 6c65 6e28 6669  _fields = len(fi
+0000ad10: 656c 645f 6e61 6d65 7329 0a0a 2020 2020  eld_names)..    
+0000ad20: 2020 2020 2320 7665 7269 6679 2074 6861      # verify tha
+0000ad30: 7420 7374 6174 7320 6361 6e20 2273 7465  t stats can "ste
+0000ad40: 7020 6f76 6572 2220 6e6f 6e2d 6e75 6d65  p over" non-nume
+0000ad50: 7269 6320 6461 7461 0a20 2020 2020 2020  ric data.       
+0000ad60: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0000ad70: 2020 7365 6c66 2e74 315b 305d 2e61 203d    self.t1[0].a =
+0000ad80: 2022 6e6f 7420 6120 6e75 6d62 6572 220a   "not a number".
+0000ad90: 2020 2020 2020 2020 6578 6365 7074 2028          except (
+0000ada0: 4174 7472 6962 7574 6545 7272 6f72 2c20  AttributeError, 
+0000adb0: 5479 7065 4572 726f 7229 3a0a 2020 2020  TypeError):.    
+0000adc0: 2020 2020 2020 2020 2320 736f 6d65 2074          # some t
+0000add0: 6573 7420 7479 7065 7320 6172 656e 2774  est types aren't
+0000ade0: 206d 7574 6162 6c65 2c20 6d75 7374 2072   mutable, must r
+0000adf0: 6570 6c61 6365 2072 6563 2077 6974 6820  eplace rec with 
+0000ae00: 6120 6d6f 6469 6669 6564 206f 6e65 0a20  a modified one. 
+0000ae10: 2020 2020 2020 2020 2020 206d 6f64 5f72             mod_r
+0000ae20: 6563 203d 2073 656c 662e 7431 2e70 6f70  ec = self.t1.pop
+0000ae30: 2830 290a 2020 2020 2020 2020 2020 2020  (0).            
+0000ae40: 7265 635f 7479 7065 203d 2074 7970 6528  rec_type = type(
+0000ae50: 6d6f 645f 7265 6329 0a20 2020 2020 2020  mod_rec).       
+0000ae60: 2020 2020 206e 6577 5f72 6563 5f64 6963       new_rec_dic
+0000ae70: 7420 3d20 6c74 2e5f 746f 5f64 6963 7428  t = lt._to_dict(
+0000ae80: 6d6f 645f 7265 6329 0a20 2020 2020 2020  mod_rec).       
+0000ae90: 2020 2020 206e 6577 5f72 6563 5f64 6963       new_rec_dic
+0000aea0: 745b 2761 275d 203d 2022 6e6f 7420 6120  t['a'] = "not a 
+0000aeb0: 6e75 6d62 6572 220a 2020 2020 2020 2020  number".        
+0000aec0: 2020 2020 6e65 775f 7265 6320 3d20 7265      new_rec = re
+0000aed0: 635f 7479 7065 282a 2a6e 6577 5f72 6563  c_type(**new_rec
+0000aee0: 5f64 6963 7429 0a20 2020 2020 2020 2020  _dict).         
+0000aef0: 2020 2073 656c 662e 7431 2e69 6e73 6572     self.t1.inser
+0000af00: 7428 6e65 775f 7265 6329 0a0a 2020 2020  t(new_rec)..    
+0000af10: 2020 2020 7431 5f73 7461 7473 203d 2073      t1_stats = s
+0000af20: 656c 662e 7431 2e73 7461 7473 2829 0a20  elf.t1.stats(). 
+0000af30: 2020 2020 2020 2074 315f 7374 6174 7328         t1_stats(
+0000af40: 2274 315f 7374 6174 7322 290a 2020 2020  "t1_stats").    
+0000af50: 2020 2020 7431 5f73 7461 7473 2e63 7376      t1_stats.csv
+0000af60: 5f65 7870 6f72 7428 7379 732e 7374 646f  _export(sys.stdo
+0000af70: 7574 290a 2020 2020 2020 2020 7431 5f73  ut).        t1_s
+0000af80: 7461 7473 2e70 7265 7365 6e74 2829 0a20  tats.present(). 
+0000af90: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0000afa0: 7274 4571 7561 6c28 7365 6c66 2e74 6573  rtEqual(self.tes
+0000afb0: 745f 7369 7a65 202a 2a20 6e75 6d5f 6669  t_size ** num_fi
+0000afc0: 656c 6473 202d 2031 2c20 7431 5f73 7461  elds - 1, t1_sta
+0000afd0: 7473 2e62 792e 6e61 6d65 5b22 6122 5d2e  ts.by.name["a"].
+0000afe0: 636f 756e 7429 0a0a 2020 2020 6465 6620  count)..    def 
+0000aff0: 7465 7374 5f73 7461 7473 3428 7365 6c66  test_stats4(self
+0000b000: 293a 0a20 2020 2020 2020 2074 3120 3d20  ):.        t1 = 
+0000b010: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
+0000b020: 6d70 6f72 7428 7465 7874 7772 6170 2e64  mport(textwrap.d
+0000b030: 6564 656e 7428 2222 225c 0a20 2020 2020  edent("""\.     
+0000b040: 2020 2061 2c62 0a20 2020 2020 2020 2031     a,b.        1
+0000b050: 2c32 0a20 2020 2020 2020 2033 2c0a 2020  ,2.        3,.  
+0000b060: 2020 2020 2020 352c 340a 2020 2020 2020        5,4.      
+0000b070: 2020 2222 2229 2c20 7472 616e 7366 6f72    """), transfor
+0000b080: 6d73 3d7b 7d2e 6672 6f6d 6b65 7973 285b  ms={}.fromkeys([
+0000b090: 2261 222c 2022 6222 5d2c 2069 6e74 2929  "a", "b"], int))
+0000b0a0: 0a20 2020 2020 2020 2074 315f 7374 6174  .        t1_stat
+0000b0b0: 7320 3d20 7431 2e73 7461 7473 2829 0a20  s = t1.stats(). 
+0000b0c0: 2020 2020 2020 2074 315f 7374 6174 732e         t1_stats.
+0000b0d0: 7072 6573 656e 7428 290a 2020 2020 2020  present().      
+0000b0e0: 2020 7072 696e 7428 7431 5f73 7461 7473    print(t1_stats
+0000b0f0: 2e69 6e66 6f28 2929 0a0a 2020 2020 2020  .info())..      
+0000b100: 2020 6578 7065 6374 6564 203d 206c 742e    expected = lt.
+0000b110: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
+0000b120: 7274 2874 6578 7477 7261 702e 6465 6465  rt(textwrap.dede
+0000b130: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
+0000b140: 6e61 6d65 2c6d 6561 6e2c 6d69 6e2c 6d61  name,mean,min,ma
+0000b150: 782c 7661 7269 616e 6365 2c73 7464 5f64  x,variance,std_d
+0000b160: 6576 2c63 6f75 6e74 2c6d 6973 7369 6e67  ev,count,missing
+0000b170: 0a20 2020 2020 2020 2061 2c33 2e30 2c31  .        a,3.0,1
+0000b180: 2c35 2c34 2c32 2e30 2c33 2c30 0a20 2020  ,5,4,2.0,3,0.   
+0000b190: 2020 2020 2062 2c33 2e30 2c32 2c34 2c32       b,3.0,2,4,2
+0000b1a0: 2c31 2e34 3134 2c32 2c31 0a20 2020 2020  ,1.414,2,1.     
+0000b1b0: 2020 2022 2222 292c 2074 7261 6e73 666f     """), transfo
+0000b1c0: 726d 733d 7b7d 2e66 726f 6d6b 6579 7328  rms={}.fromkeys(
+0000b1d0: 226d 6561 6e20 6d69 6e20 6d61 7820 7661  "mean min max va
+0000b1e0: 7269 616e 6365 2073 7464 5f64 6576 2063  riance std_dev c
+0000b1f0: 6f75 6e74 206d 6973 7369 6e67 222e 7370  ount missing".sp
+0000b200: 6c69 7428 292c 2061 7374 2e6c 6974 6572  lit(), ast.liter
+0000b210: 616c 5f65 7661 6c29 290a 2020 2020 2020  al_eval)).      
+0000b220: 2020 6578 7065 6374 6564 2e70 7265 7365    expected.prese
+0000b230: 6e74 2829 0a20 2020 2020 2020 2070 7269  nt().        pri
+0000b240: 6e74 2865 7870 6563 7465 642e 696e 666f  nt(expected.info
+0000b250: 2829 290a 0a20 2020 2020 2020 2077 6974  ())..        wit
+0000b260: 6820 7365 6c66 2e73 7562 5465 7374 2822  h self.subTest("
+0000b270: 6368 6563 6b20 636f 6d70 7574 6564 2073  check computed s
+0000b280: 7461 7420 6669 656c 6473 2229 3a0a 2020  tat fields"):.  
+0000b290: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000b2a0: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
+0000b2b0: 7465 642e 696e 666f 2829 5b22 6669 656c  ted.info()["fiel
+0000b2c0: 6473 225d 2c20 7431 5f73 7461 7473 2e69  ds"], t1_stats.i
+0000b2d0: 6e66 6f28 295b 2266 6965 6c64 7322 5d29  nfo()["fields"])
+0000b2e0: 0a0a 2020 2020 2020 2020 666f 7220 6578  ..        for ex
+0000b2f0: 7065 6374 6564 5f72 6f77 2c20 726f 7720  pected_row, row 
+0000b300: 696e 207a 6970 2865 7870 6563 7465 642c  in zip(expected,
+0000b310: 2074 315f 7374 6174 7329 3a0a 2020 2020   t1_stats):.    
+0000b320: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0000b330: 662e 7375 6254 6573 7428 2263 6865 636b  f.subTest("check
+0000b340: 2063 6f6d 7075 7465 6420 7374 6174 2061   computed stat a
+0000b350: 7474 7269 6275 7465 2028 6e61 6d65 2922  ttribute (name)"
+0000b360: 2c20 726f 773d 726f 7729 3a0a 2020 2020  , row=row):.    
+0000b370: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b380: 2e61 7373 6572 7445 7175 616c 2865 7870  .assertEqual(exp
+0000b390: 6563 7465 645f 726f 772e 6e61 6d65 2c20  ected_row.name, 
+0000b3a0: 726f 772e 6e61 6d65 290a 2020 2020 2020  row.name).      
+0000b3b0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+0000b3c0: 7375 6254 6573 7428 2263 6865 636b 2063  subTest("check c
+0000b3d0: 6f6d 7075 7465 6420 7374 6174 2061 7474  omputed stat att
+0000b3e0: 7269 6275 7465 2028 6d65 616e 2922 2c20  ribute (mean)", 
+0000b3f0: 726f 773d 726f 7729 3a0a 2020 2020 2020  row=row):.      
+0000b400: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000b410: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
+0000b420: 7465 645f 726f 772e 6d65 616e 2c20 726f  ted_row.mean, ro
+0000b430: 772e 6d65 616e 290a 2020 2020 2020 2020  w.mean).        
+0000b440: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+0000b450: 6254 6573 7428 2263 6865 636b 2063 6f6d  bTest("check com
+0000b460: 7075 7465 6420 7374 6174 2061 7474 7269  puted stat attri
+0000b470: 6275 7465 2028 6d69 6e29 222c 2072 6f77  bute (min)", row
+0000b480: 3d72 6f77 293a 0a20 2020 2020 2020 2020  =row):.         
+0000b490: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0000b4a0: 7274 4571 7561 6c28 6578 7065 6374 6564  rtEqual(expected
+0000b4b0: 5f72 6f77 2e6d 696e 2c20 726f 772e 6d69  _row.min, row.mi
+0000b4c0: 6e29 0a20 2020 2020 2020 2020 2020 2077  n).            w
+0000b4d0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+0000b4e0: 2822 6368 6563 6b20 636f 6d70 7574 6564  ("check computed
+0000b4f0: 2073 7461 7420 6174 7472 6962 7574 6520   stat attribute 
+0000b500: 286d 6178 2922 2c20 726f 773d 726f 7729  (max)", row=row)
+0000b510: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b520: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000b530: 616c 2865 7870 6563 7465 645f 726f 772e  al(expected_row.
+0000b540: 6d61 782c 2072 6f77 2e6d 6178 290a 2020  max, row.max).  
+0000b550: 2020 2020 2020 2020 2020 7769 7468 2073            with s
+0000b560: 656c 662e 7375 6254 6573 7428 2263 6865  elf.subTest("che
+0000b570: 636b 2063 6f6d 7075 7465 6420 7374 6174  ck computed stat
+0000b580: 2061 7474 7269 6275 7465 2028 7661 7269   attribute (vari
+0000b590: 616e 6365 2922 2c20 726f 773d 726f 7729  ance)", row=row)
+0000b5a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b5b0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000b5c0: 616c 2865 7870 6563 7465 645f 726f 772e  al(expected_row.
+0000b5d0: 7661 7269 616e 6365 2c20 726f 772e 7661  variance, row.va
+0000b5e0: 7269 616e 6365 290a 2020 2020 2020 2020  riance).        
+0000b5f0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+0000b600: 6254 6573 7428 2263 6865 636b 2063 6f6d  bTest("check com
+0000b610: 7075 7465 6420 7374 6174 2061 7474 7269  puted stat attri
+0000b620: 6275 7465 2028 7374 645f 6465 7629 222c  bute (std_dev)",
+0000b630: 2072 6f77 3d72 6f77 293a 0a20 2020 2020   row=row):.     
+0000b640: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b650: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
+0000b660: 6374 6564 5f72 6f77 2e73 7464 5f64 6576  cted_row.std_dev
+0000b670: 2c20 726f 772e 7374 645f 6465 7629 0a20  , row.std_dev). 
+0000b680: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+0000b690: 7365 6c66 2e73 7562 5465 7374 2822 6368  self.subTest("ch
+0000b6a0: 6563 6b20 636f 6d70 7574 6564 2073 7461  eck computed sta
+0000b6b0: 7420 6174 7472 6962 7574 6520 2863 6f75  t attribute (cou
+0000b6c0: 6e74 2922 2c20 726f 773d 726f 7729 3a0a  nt)", row=row):.
+0000b6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6e0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000b6f0: 2865 7870 6563 7465 645f 726f 772e 636f  (expected_row.co
+0000b700: 756e 742c 2072 6f77 2e63 6f75 6e74 290a  unt, row.count).
+0000b710: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0000b720: 2073 656c 662e 7375 6254 6573 7428 2263   self.subTest("c
+0000b730: 6865 636b 2063 6f6d 7075 7465 6420 7374  heck computed st
+0000b740: 6174 2061 7474 7269 6275 7465 2028 6d69  at attribute (mi
+0000b750: 7373 696e 6729 222c 2072 6f77 3d72 6f77  ssing)", row=row
+0000b760: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000b770: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000b780: 7561 6c28 6578 7065 6374 6564 5f72 6f77  ual(expected_row
+0000b790: 2e6d 6973 7369 6e67 2c20 726f 772e 6d69  .missing, row.mi
+0000b7a0: 7373 696e 6729 0a0a 2020 2020 6465 6620  ssing)..    def 
+0000b7b0: 7465 7374 5f73 706c 6974 6279 2873 656c  test_splitby(sel
+0000b7c0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+0000b7d0: 2e5f 7465 7374 5f69 6e69 7428 290a 2020  ._test_init().  
+0000b7e0: 2020 2020 2020 6973 5f6f 6464 203d 206c        is_odd = l
+0000b7f0: 616d 6264 6120 7265 633a 2072 6563 2e61  ambda rec: rec.a
+0000b800: 2025 2032 0a20 2020 2020 2020 2065 7665   % 2.        eve
+0000b810: 6e73 2c20 6f64 6473 203d 2073 656c 662e  ns, odds = self.
+0000b820: 7431 2e73 706c 6974 6279 2869 735f 6f64  t1.splitby(is_od
+0000b830: 6429 0a20 2020 2020 2020 2077 6974 6820  d).        with 
+0000b840: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
+0000b850: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b860: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
+0000b870: 286f 6464 7329 202b 206c 656e 2865 7665  (odds) + len(eve
+0000b880: 6e73 292c 206c 656e 2873 656c 662e 7431  ns), len(self.t1
+0000b890: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
+0000b8a0: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
+0000b8b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b8c0: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
+0000b8d0: 286f 6464 7329 2c20 6c65 6e28 7365 6c66  (odds), len(self
+0000b8e0: 2e74 312e 7768 6572 6528 6973 5f6f 6464  .t1.where(is_odd
+0000b8f0: 2929 290a 0a20 2020 2020 2020 2065 7665  )))..        eve
+0000b900: 6e5f 6576 656e 732c 206f 6464 5f65 7665  n_evens, odd_eve
+0000b910: 6e73 203d 2065 7665 6e73 2e73 706c 6974  ns = evens.split
+0000b920: 6279 2869 735f 6f64 6429 0a20 2020 2020  by(is_odd).     
+0000b930: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+0000b940: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+0000b950: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0000b960: 7175 616c 2830 2c20 6c65 6e28 6f64 645f  qual(0, len(odd_
+0000b970: 6576 656e 7329 290a 2020 2020 2020 2020  evens)).        
+0000b980: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+0000b990: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+0000b9a0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000b9b0: 6c28 6c65 6e28 6576 656e 5f65 7665 6e73  l(len(even_evens
+0000b9c0: 292c 206c 656e 2865 7665 6e73 2929 0a0a  ), len(evens))..
+0000b9d0: 2020 2020 2020 2020 2320 6d61 6b65 2073          # make s
+0000b9e0: 7572 6520 696e 6465 7865 7320 6172 6520  ure indexes are 
+0000b9f0: 7072 6573 6572 7665 640a 2020 2020 2020  preserved.      
+0000ba00: 2020 7365 6c66 2e74 312e 6372 6561 7465    self.t1.create
+0000ba10: 5f69 6e64 6578 2822 6122 290a 2020 2020  _index("a").    
+0000ba20: 2020 2020 6576 656e 732c 206f 6464 7320      evens, odds 
+0000ba30: 3d20 7365 6c66 2e74 312e 7370 6c69 7462  = self.t1.splitb
+0000ba40: 7928 6973 5f6f 6464 290a 2020 2020 2020  y(is_odd).      
+0000ba50: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+0000ba60: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+0000ba70: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000ba80: 7561 6c28 7365 6c66 2e74 312e 696e 666f  ual(self.t1.info
+0000ba90: 2829 5b22 696e 6465 7865 7322 5d2c 2065  ()["indexes"], e
+0000baa0: 7665 6e73 2e69 6e66 6f28 295b 2269 6e64  vens.info()["ind
+0000bab0: 6578 6573 225d 290a 0a20 2020 2020 2020  exes"])..       
+0000bac0: 2023 2074 6573 7420 7061 7373 696e 6720   # test passing 
+0000bad0: 616e 2061 7474 7269 6275 7465 2061 7320  an attribute as 
+0000bae0: 6120 6b65 790a 2020 2020 2020 2020 7a65  a key.        ze
+0000baf0: 726f 732c 206e 6f6e 5f7a 6572 6f73 203d  ros, non_zeros =
+0000bb00: 2073 656c 662e 7431 2e73 706c 6974 6279   self.t1.splitby
+0000bb10: 2822 6122 290a 2020 2020 2020 2020 7769  ("a").        wi
+0000bb20: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+0000bb30: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000bb40: 656c 662e 6173 7365 7274 5472 7565 2861  elf.assertTrue(a
+0000bb50: 6c6c 2872 6563 2e61 203d 3d20 3020 666f  ll(rec.a == 0 fo
+0000bb60: 7220 7265 6320 696e 207a 6572 6f73 2929  r rec in zeros))
+0000bb70: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+0000bb80: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+0000bb90: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000bba0: 7373 6572 7454 7275 6528 616c 6c28 7265  ssertTrue(all(re
+0000bbb0: 632e 6120 213d 2030 2066 6f72 2072 6563  c.a != 0 for rec
+0000bbc0: 2069 6e20 6e6f 6e5f 7a65 726f 7329 290a   in non_zeros)).
+0000bbd0: 0a20 2020 2020 2020 2023 2074 6573 7420  .        # test 
+0000bbe0: 7573 696e 6720 7072 6564 6963 6174 6520  using predicate 
+0000bbf0: 7468 6174 2064 6f65 7320 6e6f 7420 616c  that does not al
+0000bc00: 7761 7973 2072 6574 7572 6e20 3020 6f72  ways return 0 or
+0000bc10: 2031 0a20 2020 2020 2020 2069 735f 6e6f   1.        is_no
+0000bc20: 745f 6d75 6c74 6970 6c65 5f6f 665f 3320  t_multiple_of_3 
+0000bc30: 3d20 6c61 6d62 6461 2072 6563 3a20 7265  = lambda rec: re
+0000bc40: 632e 6120 2520 330a 2020 2020 2020 2020  c.a % 3.        
+0000bc50: 6d75 6c74 735f 6f66 5f33 2c20 6e6f 6e5f  mults_of_3, non_
+0000bc60: 6d75 6c74 735f 6f66 5f33 203d 2073 656c  mults_of_3 = sel
+0000bc70: 662e 7431 2e73 706c 6974 6279 2869 735f  f.t1.splitby(is_
+0000bc80: 6e6f 745f 6d75 6c74 6970 6c65 5f6f 665f  not_multiple_of_
+0000bc90: 3329 0a20 2020 2020 2020 2070 7269 6e74  3).        print
+0000bca0: 286c 6973 7428 6e6f 6e5f 6d75 6c74 735f  (list(non_mults_
+0000bcb0: 6f66 5f33 2e61 6c6c 2e61 2929 0a20 2020  of_3.all.a)).   
+0000bcc0: 2020 2020 2070 7269 6e74 286c 6973 7428       print(list(
+0000bcd0: 6d75 6c74 735f 6f66 5f33 2e61 6c6c 2e61  mults_of_3.all.a
+0000bce0: 2929 0a20 2020 2020 2020 2023 2054 4f44  )).        # TOD
+0000bcf0: 4f20 2d20 6164 6420 6173 7365 7274 7320  O - add asserts 
+0000bd00: 6865 7265 0a0a 0a40 6d61 6b65 5f74 6573  here...@make_tes
+0000bd10: 745f 636c 6173 7365 730a 636c 6173 7320  t_classes.class 
+0000bd20: 5461 626c 654a 6f69 6e54 6573 7473 3a0a  TableJoinTests:.
+0000bd30: 2020 2020 6465 6620 7465 7374 5f73 696d      def test_sim
+0000bd40: 706c 655f 6a6f 696e 2873 656c 6629 3a0a  ple_join(self):.
+0000bd50: 2020 2020 2020 2020 7465 7374 5f73 697a          test_siz
+0000bd60: 6520 3d20 3130 0a20 2020 2020 2020 2074  e = 10.        t
+0000bd70: 3120 3d20 6d61 6b65 5f74 6573 745f 7461  1 = make_test_ta
+0000bd80: 626c 6528 7365 6c66 2e6d 616b 655f 6461  ble(self.make_da
+0000bd90: 7461 5f6f 626a 6563 742c 2074 6573 745f  ta_object, test_
+0000bda0: 7369 7a65 290a 2020 2020 2020 2020 7431  size).        t1
+0000bdb0: 2e63 7265 6174 655f 696e 6465 7828 2761  .create_index('a
+0000bdc0: 2729 0a0a 2020 2020 2020 2020 7432 203d  ')..        t2 =
+0000bdd0: 206c 742e 5461 626c 6528 290a 2020 2020   lt.Table().    
+0000bde0: 2020 2020 7432 2e63 7265 6174 655f 696e      t2.create_in
+0000bdf0: 6465 7828 2761 2729 0a20 2020 2020 2020  dex('a').       
+0000be00: 2074 322e 696e 7365 7274 286c 742e 4461   t2.insert(lt.Da
+0000be10: 7461 4f62 6a65 6374 2861 3d31 2c20 643d  taObject(a=1, d=
+0000be20: 3130 3029 290a 0a20 2020 2020 2020 206a  100))..        j
+0000be30: 6f69 6e65 6420 3d20 2874 312e 6a6f 696e  oined = (t1.join
+0000be40: 5f6f 6e28 2761 2729 202b 2074 322e 6a6f  _on('a') + t2.jo
+0000be50: 696e 5f6f 6e28 2761 2729 2928 290a 2020  in_on('a'))().  
+0000be60: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+0000be70: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+0000be80: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0000be90: 7274 4571 7561 6c28 7465 7374 5f73 697a  rtEqual(test_siz
+0000bea0: 6520 2a20 7465 7374 5f73 697a 652c 206c  e * test_size, l
+0000beb0: 656e 286a 6f69 6e65 6429 290a 0a20 2020  en(joined))..   
+0000bec0: 2020 2020 206a 6f69 6e65 6420 3d20 2874       joined = (t
+0000bed0: 312e 6a6f 696e 5f6f 6e28 2761 2729 202b  1.join_on('a') +
+0000bee0: 2074 3229 2829 0a20 2020 2020 2020 2077   t2)().        w
+0000bef0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+0000bf00: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000bf10: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000bf20: 2874 6573 745f 7369 7a65 202a 2074 6573  (test_size * tes
+0000bf30: 745f 7369 7a65 2c20 6c65 6e28 6a6f 696e  t_size, len(join
+0000bf40: 6564 2929 0a0a 2020 2020 2020 2020 6a6f  ed))..        jo
+0000bf50: 696e 6564 203d 2028 7431 202b 2074 322e  ined = (t1 + t2.
+0000bf60: 6a6f 696e 5f6f 6e28 2761 2729 2928 290a  join_on('a'))().
+0000bf70: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0000bf80: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+0000bf90: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+0000bfa0: 7365 7274 4571 7561 6c28 7465 7374 5f73  sertEqual(test_s
+0000bfb0: 697a 6520 2a20 7465 7374 5f73 697a 652c  ize * test_size,
+0000bfc0: 206c 656e 286a 6f69 6e65 6429 290a 0a20   len(joined)).. 
+0000bfd0: 2020 2020 2020 2074 312e 6465 6c65 7465         t1.delete
+0000bfe0: 5f69 6e64 6578 2827 6127 290a 2020 2020  _index('a').    
+0000bff0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+0000c000: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+0000c010: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
+0000c020: 7373 6572 7452 6169 7365 7328 5661 6c75  ssertRaises(Valu
+0000c030: 6545 7272 6f72 293a 0a20 2020 2020 2020  eError):.       
+0000c040: 2020 2020 2020 2020 206a 6f69 6e65 6420           joined 
+0000c050: 3d20 2874 3120 2b20 7432 2e6a 6f69 6e5f  = (t1 + t2.join_
+0000c060: 6f6e 2827 6127 2929 2829 0a0a 2020 2020  on('a'))()..    
+0000c070: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+0000c080: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+0000c090: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
+0000c0a0: 7373 6572 7452 6169 7365 7328 5479 7065  ssertRaises(Type
+0000c0b0: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
+0000c0c0: 2020 2020 2020 2020 2320 696e 7661 6c69          # invali
+0000c0d0: 6420 6a6f 696e 2c20 6e6f 206b 7761 7267  d join, no kwarg
+0000c0e0: 7320 6c69 7374 696e 6720 6174 7472 6962  s listing attrib
+0000c0f0: 7574 6573 2074 6f20 6a6f 696e 206f 6e0a  utes to join on.
+0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c110: 7433 203d 2074 312e 6a6f 696e 2874 322c  t3 = t1.join(t2,
+0000c120: 2027 612c 6427 290a 0a20 2020 2020 2020   'a,d')..       
+0000c130: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+0000c140: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+0000c150: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
+0000c160: 7274 5261 6973 6573 2856 616c 7565 4572  rtRaises(ValueEr
+0000c170: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
+0000c180: 2020 2020 2020 2320 696e 7661 6c69 6420        # invalid 
+0000c190: 6a6f 696e 2c20 6e6f 2073 7563 6820 6174  join, no such at
+0000c1a0: 7472 6962 7574 6520 277a 270a 2020 2020  tribute 'z'.    
+0000c1b0: 2020 2020 2020 2020 2020 2020 7433 203d              t3 =
+0000c1c0: 2074 312e 6a6f 696e 2874 322c 2027 612c   t1.join(t2, 'a,
+0000c1d0: 642c 7a27 2c20 613d 2761 2729 0a0a 2020  d,z', a='a')..  
+0000c1e0: 2020 2020 2020 7433 203d 2074 312e 6a6f        t3 = t1.jo
+0000c1f0: 696e 2874 322c 2027 612c 6427 2c20 613d  in(t2, 'a,d', a=
+0000c200: 2761 2729 0a20 2020 2020 2020 2077 6974  'a').        wit
+0000c210: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+0000c220: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000c230: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
+0000c240: 6573 745f 7369 7a65 202a 2074 6573 745f  est_size * test_
+0000c250: 7369 7a65 2c20 6c65 6e28 7433 2929 0a0a  size, len(t3))..
+0000c260: 2020 2020 2020 2020 7434 203d 2074 312e          t4 = t1.
+0000c270: 6a6f 696e 2874 322c 2061 3d27 6127 292e  join(t2, a='a').
+0000c280: 7365 6c65 6374 2827 6120 6320 6427 2c20  select('a c d', 
+0000c290: 653d 6c61 6d62 6461 2072 6563 3a20 7265  e=lambda rec: re
+0000c2a0: 632e 6120 2b20 7265 632e 6320 2b20 7265  c.a + rec.c + re
+0000c2b0: 632e 6429 0a20 2020 2020 2020 2077 6974  c.d).        wit
+0000c2c0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+0000c2d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000c2e0: 6c66 2e61 7373 6572 7454 7275 6528 616c  lf.assertTrue(al
+0000c2f0: 6c28 7265 632e 6520 3d3d 2072 6563 2e61  l(rec.e == rec.a
+0000c300: 2b72 6563 2e63 2b72 6563 2e64 2066 6f72  +rec.c+rec.d for
+0000c310: 2072 6563 2069 6e20 7434 2929 0a0a 2020   rec in t4))..  
+0000c320: 2020 2020 2020 2320 6a6f 696e 2074 6f20        # join to 
+0000c330: 656d 7074 7920 6c69 7374 2c20 7368 6f75  empty list, shou
+0000c340: 6c64 2072 6574 7572 6e20 656d 7074 7920  ld return empty 
+0000c350: 7461 626c 650a 2020 2020 2020 2020 656d  table.        em
+0000c360: 7074 795f 7461 626c 6520 3d20 6c74 2e54  pty_table = lt.T
+0000c370: 6162 6c65 2829 0a20 2020 2020 2020 2065  able().        e
+0000c380: 6d70 7479 5f74 6162 6c65 2e63 7265 6174  mpty_table.creat
+0000c390: 655f 696e 6465 7828 2761 2729 0a20 2020  e_index('a').   
+0000c3a0: 2020 2020 2074 3520 3d20 2874 312e 6a6f       t5 = (t1.jo
+0000c3b0: 696e 5f6f 6e28 2761 2729 202b 2065 6d70  in_on('a') + emp
+0000c3c0: 7479 5f74 6162 6c65 2928 290a 2020 2020  ty_table)().    
+0000c3d0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+0000c3e0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+0000c3f0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000c400: 4571 7561 6c28 302c 206c 656e 2874 3529  Equal(0, len(t5)
+0000c410: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+0000c420: 6f75 7465 725f 6a6f 696e 7328 7365 6c66  outer_joins(self
+0000c430: 293a 0a20 2020 2020 2020 2074 3120 3d20  ):.        t1 = 
+0000c440: 6c74 2e54 6162 6c65 2822 6361 7461 6c6f  lt.Table("catalo
+0000c450: 6722 290a 2020 2020 2020 2020 7431 2e63  g").        t1.c
+0000c460: 7376 5f69 6d70 6f72 7428 7465 7874 7772  sv_import(textwr
+0000c470: 6170 2e64 6564 656e 7428 2222 225c 0a20  ap.dedent("""\. 
+0000c480: 2020 2020 2020 2020 2020 2073 6b75 2c63             sku,c
+0000c490: 6f6c 6f72 2c73 697a 652c 6d61 7465 7269  olor,size,materi
+0000c4a0: 616c 0a20 2020 2020 2020 2020 2020 2030  al.            0
+0000c4b0: 3031 2c72 6564 2c58 4c2c 636f 7474 6f6e  01,red,XL,cotton
+0000c4c0: 0a20 2020 2020 2020 2020 2020 2030 3032  .            002
+0000c4d0: 2c62 6c75 652c 584c 2c63 6f74 746f 6e2f  ,blue,XL,cotton/
+0000c4e0: 706f 6c79 0a20 2020 2020 2020 2020 2020  poly.           
+0000c4f0: 2030 3033 2c62 6c75 652c 4c2c 6c69 6e65   003,blue,L,line
+0000c500: 6e0a 2020 2020 2020 2020 2020 2020 3030  n.            00
+0000c510: 342c 7265 642c 4d2c 636f 7474 6f6e 0a20  4,red,M,cotton. 
+0000c520: 2020 2020 2020 2020 2020 2022 2222 2929             """))
+0000c530: 0a0a 2020 2020 2020 2020 7432 203d 206c  ..        t2 = l
+0000c540: 742e 5461 626c 6528 2270 7269 6365 7322  t.Table("prices"
+0000c550: 290a 2020 2020 2020 2020 7432 2e63 7376  ).        t2.csv
+0000c560: 5f69 6d70 6f72 7428 7465 7874 7772 6170  _import(textwrap
+0000c570: 2e64 6564 656e 7428 2222 225c 0a20 2020  .dedent("""\.   
+0000c580: 2020 2020 2020 2020 2073 6b75 2c75 6e69           sku,uni
+0000c590: 745f 7072 6963 652c 7369 7a65 0a20 2020  t_price,size.   
+0000c5a0: 2020 2020 2020 2020 2030 3031 2c31 302c           001,10,
+0000c5b0: 4c0a 2020 2020 2020 2020 2020 2020 3030  L.            00
+0000c5c0: 312c 3132 2c58 4c0a 2020 2020 2020 2020  1,12,XL.        
+0000c5d0: 2020 2020 3030 322c 3131 2c0a 2020 2020      002,11,.    
+0000c5e0: 2020 2020 2020 2020 3030 342c 392c 0a20          004,9,. 
+0000c5f0: 2020 2020 2020 2020 2020 2022 2222 292c             """),
+0000c600: 2074 7261 6e73 666f 726d 733d 7b27 7369   transforms={'si
+0000c610: 7a65 273a 206c 616d 6264 6120 783a 2078  ze': lambda x: x
+0000c620: 206f 7220 4e6f 6e65 7d29 0a20 2020 2020   or None}).     
+0000c630: 2020 2070 7269 6e74 2874 312e 696e 666f     print(t1.info
+0000c640: 2829 290a 0a20 2020 2020 2020 2074 312e  ())..        t1.
+0000c650: 7072 6573 656e 7428 290a 2020 2020 2020  present().      
+0000c660: 2020 7432 2e70 7265 7365 6e74 2829 0a0a    t2.present()..
+0000c670: 2020 2020 2020 2020 7433 203d 2074 312e          t3 = t1.
+0000c680: 6a6f 696e 2874 322c 2061 7574 6f5f 6372  join(t2, auto_cr
+0000c690: 6561 7465 5f69 6e64 6578 6573 3d54 7275  eate_indexes=Tru
+0000c6a0: 652c 2073 6b75 3d22 736b 7522 290a 2020  e, sku="sku").  
+0000c6b0: 2020 2020 2020 7072 696e 7428 7433 2e69        print(t3.i
+0000c6c0: 6e66 6f28 2929 0a20 2020 2020 2020 2074  nfo()).        t
+0000c6d0: 332e 7072 6573 656e 7428 290a 2020 2020  3.present().    
+0000c6e0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+0000c6f0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+0000c700: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000c710: 4571 7561 6c28 342c 206c 656e 2874 3329  Equal(4, len(t3)
+0000c720: 290a 0a20 2020 2020 2020 2074 3320 3d20  )..        t3 = 
+0000c730: 7431 2e6a 6f69 6e28 7432 2c20 6175 746f  t1.join(t2, auto
+0000c740: 5f63 7265 6174 655f 696e 6465 7865 733d  _create_indexes=
+0000c750: 5472 7565 2c20 736b 753d 2273 6b75 222c  True, sku="sku",
+0000c760: 2073 697a 653d 2273 697a 6522 290a 2020   size="size").  
+0000c770: 2020 2020 2020 7433 2822 696e 6e65 7220        t3("inner 
+0000c780: 6a6f 696e 202d 2022 202b 2074 332e 7461  join - " + t3.ta
+0000c790: 626c 655f 6e61 6d65 290a 2020 2020 2020  ble_name).      
+0000c7a0: 2020 7072 696e 7428 7433 2e69 6e66 6f28    print(t3.info(
+0000c7b0: 2929 0a20 2020 2020 2020 2074 332e 7072  )).        t3.pr
+0000c7c0: 6573 656e 7428 290a 2020 2020 2020 2020  esent().        
+0000c7d0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+0000c7e0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+0000c7f0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000c800: 6c28 312c 206c 656e 2874 3329 290a 0a20  l(1, len(t3)).. 
+0000c810: 2020 2020 2020 2074 3320 3d20 7431 2e6f         t3 = t1.o
+0000c820: 7574 6572 5f6a 6f69 6e28 6c74 2e54 6162  uter_join(lt.Tab
+0000c830: 6c65 2e52 4947 4854 5f4f 5554 4552 5f4a  le.RIGHT_OUTER_J
+0000c840: 4f49 4e2c 2074 322c 2073 6b75 3d22 736b  OIN, t2, sku="sk
+0000c850: 7522 2c20 7369 7a65 3d22 7369 7a65 2229  u", size="size")
+0000c860: 0a20 2020 2020 2020 2074 3328 2272 6967  .        t3("rig
+0000c870: 6874 206f 7574 6572 206a 6f69 6e20 2d20  ht outer join - 
+0000c880: 2220 2b20 7433 2e74 6162 6c65 5f6e 616d  " + t3.table_nam
+0000c890: 6529 0a20 2020 2020 2020 2070 7269 6e74  e).        print
+0000c8a0: 2874 332e 696e 666f 2829 290a 2020 2020  (t3.info()).    
+0000c8b0: 2020 2020 7433 2e70 7265 7365 6e74 2829      t3.present()
+0000c8c0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+0000c8d0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+0000c8e0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000c8f0: 7373 6572 7445 7175 616c 2834 2c20 6c65  ssertEqual(4, le
+0000c900: 6e28 7433 2929 0a0a 2020 2020 2020 2020  n(t3))..        
+0000c910: 7433 203d 2074 312e 6f75 7465 725f 6a6f  t3 = t1.outer_jo
+0000c920: 696e 286c 742e 5461 626c 652e 4c45 4654  in(lt.Table.LEFT
+0000c930: 5f4f 5554 4552 5f4a 4f49 4e2c 2074 322c  _OUTER_JOIN, t2,
+0000c940: 2073 6b75 3d22 736b 7522 2c20 7369 7a65   sku="sku", size
+0000c950: 3d22 7369 7a65 2229 0a20 2020 2020 2020  ="size").       
+0000c960: 2074 3328 226c 6566 7420 6f75 7465 7220   t3("left outer 
+0000c970: 6a6f 696e 202d 2022 202b 2074 332e 7461  join - " + t3.ta
+0000c980: 626c 655f 6e61 6d65 290a 2020 2020 2020  ble_name).      
+0000c990: 2020 7072 696e 7428 7433 2e69 6e66 6f28    print(t3.info(
+0000c9a0: 2929 0a20 2020 2020 2020 2074 332e 7072  )).        t3.pr
+0000c9b0: 6573 656e 7428 290a 2020 2020 2020 2020  esent().        
+0000c9c0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+0000c9d0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+0000c9e0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000c9f0: 6c28 322c 206c 656e 2874 3329 290a 0a20  l(2, len(t3)).. 
+0000ca00: 2020 2020 2020 2074 3320 3d20 7431 2e6f         t3 = t1.o
+0000ca10: 7574 6572 5f6a 6f69 6e28 6c74 2e54 6162  uter_join(lt.Tab
+0000ca20: 6c65 2e46 554c 4c5f 4f55 5445 525f 4a4f  le.FULL_OUTER_JO
+0000ca30: 494e 2c20 7432 2c20 736b 753d 2273 6b75  IN, t2, sku="sku
+0000ca40: 222c 2073 697a 653d 2273 697a 6522 290a  ", size="size").
+0000ca50: 2020 2020 2020 2020 7433 2822 6675 6c6c          t3("full
+0000ca60: 206f 7574 6572 206a 6f69 6e20 2d20 2220   outer join - " 
+0000ca70: 2b20 7433 2e74 6162 6c65 5f6e 616d 6529  + t3.table_name)
+0000ca80: 0a20 2020 2020 2020 2070 7269 6e74 2874  .        print(t
+0000ca90: 332e 696e 666f 2829 290a 2020 2020 2020  3.info()).      
+0000caa0: 2020 7433 2e70 7265 7365 6e74 2829 0a20    t3.present(). 
+0000cab0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+0000cac0: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+0000cad0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000cae0: 6572 7445 7175 616c 2831 322c 206c 656e  ertEqual(12, len
+0000caf0: 2874 3329 290a 0a20 2020 2064 6566 2074  (t3))..    def t
+0000cb00: 6573 745f 6f75 7465 725f 6a6f 696e 5f65  est_outer_join_e
+0000cb10: 7861 6d70 6c65 2873 656c 6629 3a0a 2020  xample(self):.  
+0000cb20: 2020 2020 2020 2320 6465 6669 6e65 2073        # define s
+0000cb30: 7475 6465 6e74 2061 6e64 2072 6567 6973  tudent and regis
+0000cb40: 7472 6174 696f 6e20 6461 7461 0a20 2020  tration data.   
+0000cb50: 2020 2020 2073 7475 6465 6e74 7320 3d20       students = 
+0000cb60: 6c74 2e54 6162 6c65 2822 7374 7564 656e  lt.Table("studen
+0000cb70: 7473 2229 2e63 7376 5f69 6d70 6f72 7428  ts").csv_import(
+0000cb80: 7465 7874 7772 6170 2e64 6564 656e 7428  textwrap.dedent(
+0000cb90: 2222 225c 0a20 2020 2020 2020 2020 2020  """\.           
+0000cba0: 2073 7475 6465 6e74 5f69 642c 6e61 6d65   student_id,name
+0000cbb0: 0a20 2020 2020 2020 2020 2020 2030 3030  .            000
+0000cbc0: 312c 416c 6963 650a 2020 2020 2020 2020  1,Alice.        
+0000cbd0: 2020 2020 3030 3032 2c42 6f62 0a20 2020      0002,Bob.   
+0000cbe0: 2020 2020 2020 2020 2030 3030 332c 4368           0003,Ch
+0000cbf0: 6172 6c69 650a 2020 2020 2020 2020 2020  arlie.          
+0000cc00: 2020 3030 3034 2c44 6176 650a 2020 2020    0004,Dave.    
+0000cc10: 2020 2020 2020 2020 3030 3035 2c45 6e69          0005,Eni
+0000cc20: 640a 2020 2020 2020 2020 2020 2020 2222  d.            ""
+0000cc30: 2229 290a 0a20 2020 2020 2020 2072 6567  "))..        reg
+0000cc40: 6973 7472 6174 696f 6e73 203d 206c 742e  istrations = lt.
+0000cc50: 5461 626c 6528 2272 6567 6973 7472 6174  Table("registrat
+0000cc60: 696f 6e73 2229 2e63 7376 5f69 6d70 6f72  ions").csv_impor
+0000cc70: 7428 7465 7874 7772 6170 2e64 6564 656e  t(textwrap.deden
+0000cc80: 7428 2222 225c 0a20 2020 2020 2020 2020  t("""\.         
+0000cc90: 2020 2073 7475 6465 6e74 5f69 642c 636f     student_id,co
+0000cca0: 7572 7365 0a20 2020 2020 2020 2020 2020  urse.           
+0000ccb0: 2030 3030 312c 5053 5943 4831 3031 0a20   0001,PSYCH101. 
+0000ccc0: 2020 2020 2020 2020 2020 2030 3030 312c             0001,
+0000ccd0: 4341 4c43 310a 2020 2020 2020 2020 2020  CALC1.          
+0000cce0: 2020 3030 3033 2c42 494f 3230 300a 2020    0003,BIO200.  
+0000ccf0: 2020 2020 2020 2020 2020 3030 3035 2c43            0005,C
+0000cd00: 4845 4d31 3031 0a20 2020 2020 2020 2020  HEM101.         
+0000cd10: 2020 2030 3030 362c 5048 5931 3031 0a20     0006,PHY101. 
+0000cd20: 2020 2020 2020 2020 2020 2022 2222 2929             """))
+0000cd30: 0a0a 2020 2020 2020 2020 636f 7572 7365  ..        course
+0000cd40: 7320 3d20 6c74 2e54 6162 6c65 2822 636f  s = lt.Table("co
+0000cd50: 7572 7365 7322 292e 6373 765f 696d 706f  urses").csv_impo
+0000cd60: 7274 2874 6578 7477 7261 702e 6465 6465  rt(textwrap.dede
+0000cd70: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
+0000cd80: 2020 2020 636f 7572 7365 0a20 2020 2020      course.     
+0000cd90: 2020 2020 2020 2042 494f 3230 300a 2020         BIO200.  
+0000cda0: 2020 2020 2020 2020 2020 4341 4c43 310a            CALC1.
+0000cdb0: 2020 2020 2020 2020 2020 2020 4348 454d              CHEM
+0000cdc0: 3130 310a 2020 2020 2020 2020 2020 2020  101.            
+0000cdd0: 5053 5943 4831 3031 0a20 2020 2020 2020  PSYCH101.       
+0000cde0: 2020 2020 2050 4531 3031 0a20 2020 2020       PE101.     
+0000cdf0: 2020 2020 2020 2022 2222 2929 0a0a 2020         """))..  
+0000ce00: 2020 2020 2020 2320 7065 7266 6f72 6d20        # perform 
+0000ce10: 6f75 7465 7220 6a6f 696e 2061 6e64 2073  outer join and s
+0000ce20: 686f 7720 7265 7375 6c74 733a 0a20 2020  how results:.   
+0000ce30: 2020 2020 206e 6f6e 5f72 6567 203d 2073       non_reg = s
+0000ce40: 7475 6465 6e74 732e 6f75 7465 725f 6a6f  tudents.outer_jo
+0000ce50: 696e 286c 742e 5461 626c 652e 5249 4748  in(lt.Table.RIGH
+0000ce60: 545f 4f55 5445 525f 4a4f 494e 2c0a 2020  T_OUTER_JOIN,.  
+0000ce70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce90: 2020 2020 7265 6769 7374 7261 7469 6f6e      registration
+0000cea0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+0000ceb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cec0: 2020 2020 2020 2020 2073 7475 6465 6e74           student
+0000ced0: 5f69 643d 2273 7475 6465 6e74 5f69 6422  _id="student_id"
+0000cee0: 292e 7768 6572 6528 636f 7572 7365 3d4e  ).where(course=N
+0000cef0: 6f6e 6529 0a20 2020 2020 2020 206e 6f6e  one).        non
+0000cf00: 5f72 6567 2e70 7265 7365 6e74 2829 0a20  _reg.present(). 
+0000cf10: 2020 2020 2020 2070 7269 6e74 286c 6973         print(lis
+0000cf20: 7428 6e6f 6e5f 7265 672e 616c 6c2e 6e61  t(non_reg.all.na
+0000cf30: 6d65 2929 0a20 2020 2020 2020 2077 6974  me)).        wit
+0000cf40: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+0000cf50: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000cf60: 6c66 2e61 7373 6572 7445 7175 616c 285b  lf.assertEqual([
+0000cf70: 2742 6f62 272c 2027 4461 7665 275d 2c20  'Bob', 'Dave'], 
+0000cf80: 736f 7274 6564 286e 6f6e 5f72 6567 2e61  sorted(non_reg.a
+0000cf90: 6c6c 2e6e 616d 6529 290a 0a20 2020 2020  ll.name))..     
+0000cfa0: 2020 2023 2063 6f75 7273 6573 2077 6974     # courses wit
+0000cfb0: 6820 6e6f 2073 7475 6465 6e74 730a 2020  h no students.  
+0000cfc0: 2020 2020 2020 6e6f 5f73 7475 6465 6e74        no_student
+0000cfd0: 7320 3d20 7265 6769 7374 7261 7469 6f6e  s = registration
+0000cfe0: 732e 6f75 7465 725f 6a6f 696e 286c 742e  s.outer_join(lt.
+0000cff0: 5461 626c 652e 4c45 4654 5f4f 5554 4552  Table.LEFT_OUTER
+0000d000: 5f4a 4f49 4e2c 0a20 2020 2020 2020 2020  _JOIN,.         
+0000d010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d030: 636f 7572 7365 732c 0a20 2020 2020 2020  courses,.       
+0000d040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d060: 2020 636f 7572 7365 3d22 636f 7572 7365    course="course
+0000d070: 2229 2e77 6865 7265 2873 7475 6465 6e74  ").where(student
+0000d080: 5f69 643d 4e6f 6e65 290a 2020 2020 2020  _id=None).      
+0000d090: 2020 6e6f 5f73 7475 6465 6e74 732e 7072    no_students.pr
+0000d0a0: 6573 656e 7428 290a 2020 2020 2020 2020  esent().        
+0000d0b0: 7072 696e 7428 6c69 7374 286e 6f5f 7374  print(list(no_st
+0000d0c0: 7564 656e 7473 2e61 6c6c 2e63 6f75 7273  udents.all.cours
+0000d0d0: 6529 290a 2020 2020 2020 2020 7769 7468  e)).        with
+0000d0e0: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+0000d0f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d100: 662e 6173 7365 7274 4571 7561 6c28 5b27  f.assertEqual(['
+0000d110: 5045 3130 3127 5d2c 2073 6f72 7465 6428  PE101'], sorted(
+0000d120: 6e6f 5f73 7475 6465 6e74 732e 616c 6c2e  no_students.all.
+0000d130: 636f 7572 7365 2929 0a0a 0a20 2020 2020  course))...     
+0000d140: 2020 2066 756c 6c20 3d20 2073 7475 6465     full =  stude
+0000d150: 6e74 732e 6f75 7465 725f 6a6f 696e 286c  nts.outer_join(l
+0000d160: 742e 5461 626c 652e 4655 4c4c 5f4f 5554  t.Table.FULL_OUT
+0000d170: 4552 5f4a 4f49 4e2c 0a20 2020 2020 2020  ER_JOIN,.       
+0000d180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d190: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000d1a0: 6567 6973 7472 6174 696f 6e73 2c0a 2020  egistrations,.  
+0000d1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1d0: 2020 2020 7374 7564 656e 745f 6964 3d22      student_id="
+0000d1e0: 7374 7564 656e 745f 6964 2229 2e77 6865  student_id").whe
+0000d1f0: 7265 286c 616d 6264 6120 7265 633a 2072  re(lambda rec: r
+0000d200: 6563 2e63 6f75 7273 6520 6973 204e 6f6e  ec.course is Non
+0000d210: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d260: 2020 206f 7220 7265 632e 6e61 6d65 2069     or rec.name i
+0000d270: 7320 4e6f 6e65 290a 2020 2020 2020 2020  s None).        
+0000d280: 6675 6c6c 2e70 7265 7365 6e74 2829 0a20  full.present(). 
+0000d290: 2020 2020 2020 2070 7269 6e74 2873 6f72         print(sor
+0000d2a0: 7465 6428 6675 6c6c 2e61 6c6c 2e73 7475  ted(full.all.stu
+0000d2b0: 6465 6e74 5f69 6429 290a 2020 2020 2020  dent_id)).      
+0000d2c0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+0000d2d0: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+0000d2e0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000d2f0: 7561 6c28 5b27 3030 3032 272c 2027 3030  ual(['0002', '00
+0000d300: 3034 272c 2027 3030 3036 275d 2c20 736f  04', '0006'], so
+0000d310: 7274 6564 2866 756c 6c2e 616c 6c2e 7374  rted(full.all.st
+0000d320: 7564 656e 745f 6964 2929 0a0a 0a40 6d61  udent_id))...@ma
+0000d330: 6b65 5f74 6573 745f 636c 6173 7365 730a  ke_test_classes.
+0000d340: 636c 6173 7320 5461 626c 6554 7261 6e73  class TableTrans
+0000d350: 666f 726d 5465 7374 733a 0a20 2020 2064  formTests:.    d
+0000d360: 6566 2074 6573 745f 736f 7274 2873 656c  ef test_sort(sel
+0000d370: 6629 3a0a 2020 2020 2020 2020 7465 7374  f):.        test
+0000d380: 5f73 697a 6520 3d20 3130 0a20 2020 2020  _size = 10.     
+0000d390: 2020 2074 3120 3d20 6d61 6b65 5f74 6573     t1 = make_tes
+0000d3a0: 745f 7461 626c 6528 7365 6c66 2e6d 616b  t_table(self.mak
+0000d3b0: 655f 6461 7461 5f6f 626a 6563 742c 2074  e_data_object, t
+0000d3c0: 6573 745f 7369 7a65 290a 0a20 2020 2020  est_size)..     
+0000d3d0: 2020 2063 5f67 726f 7570 7320 3d20 300a     c_groups = 0.
+0000d3e0: 2020 2020 2020 2020 666f 7220 635f 7661          for c_va
+0000d3f0: 6c75 652c 2072 6563 7320 696e 2069 7465  lue, recs in ite
+0000d400: 7274 6f6f 6c73 2e67 726f 7570 6279 2874  rtools.groupby(t
+0000d410: 312c 206b 6579 3d6c 616d 6264 6120 7265  1, key=lambda re
+0000d420: 633a 2072 6563 2e63 293a 0a20 2020 2020  c: rec.c):.     
+0000d430: 2020 2020 2020 2063 5f67 726f 7570 7320         c_groups 
+0000d440: 2b3d 2031 0a20 2020 2020 2020 2020 2020  += 1.           
+0000d450: 206c 6973 7428 7265 6373 290a 2020 2020   list(recs).    
+0000d460: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+0000d470: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+0000d480: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000d490: 4571 7561 6c28 7465 7374 5f73 697a 6520  Equal(test_size 
+0000d4a0: 2a20 7465 7374 5f73 697a 6520 2a20 7465  * test_size * te
+0000d4b0: 7374 5f73 697a 652c 2063 5f67 726f 7570  st_size, c_group
+0000d4c0: 7329 0a0a 2020 2020 2020 2020 7431 2e73  s)..        t1.s
+0000d4d0: 6f72 7428 2763 2729 0a20 2020 2020 2020  ort('c').       
+0000d4e0: 2063 5f67 726f 7570 7320 3d20 300a 2020   c_groups = 0.  
+0000d4f0: 2020 2020 2020 666f 7220 635f 7661 6c75        for c_valu
+0000d500: 652c 2072 6563 7320 696e 2069 7465 7274  e, recs in itert
+0000d510: 6f6f 6c73 2e67 726f 7570 6279 2874 312c  ools.groupby(t1,
+0000d520: 206b 6579 3d6c 616d 6264 6120 7265 633a   key=lambda rec:
+0000d530: 2072 6563 2e63 293a 0a20 2020 2020 2020   rec.c):.       
+0000d540: 2020 2020 2063 5f67 726f 7570 7320 2b3d       c_groups +=
+0000d550: 2031 0a20 2020 2020 2020 2020 2020 206c   1.            l
+0000d560: 6973 7428 7265 6373 290a 2020 2020 2020  ist(recs).      
+0000d570: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+0000d580: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+0000d590: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000d5a0: 7561 6c28 7465 7374 5f73 697a 652c 2063  ual(test_size, c
+0000d5b0: 5f67 726f 7570 7329 0a20 2020 2020 2020  _groups).       
+0000d5c0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+0000d5d0: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+0000d5e0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000d5f0: 616c 2830 2c20 7431 5b30 5d2e 6329 0a0a  al(0, t1[0].c)..
+0000d600: 2020 2020 2020 2020 7431 2e73 6f72 7428          t1.sort(
+0000d610: 2763 2064 6573 6327 290a 2020 2020 2020  'c desc').      
+0000d620: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+0000d630: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+0000d640: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000d650: 7561 6c28 7465 7374 5f73 697a 652d 312c  ual(test_size-1,
+0000d660: 2074 315b 305d 2e63 290a 0a20 2020 2064   t1[0].c)..    d
+0000d670: 6566 2074 6573 745f 736f 7274 3228 7365  ef test_sort2(se
+0000d680: 6c66 293a 0a0a 2020 2020 2020 2020 726f  lf):..        ro
+0000d690: 775f 7479 7065 203d 2074 7970 6528 7365  w_type = type(se
+0000d6a0: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
+0000d6b0: 6563 7428 302c 302c 3029 290a 2020 2020  ect(0,0,0)).    
+0000d6c0: 2020 2020 7474 203d 206c 742e 5461 626c      tt = lt.Tabl
+0000d6d0: 6528 292e 6373 765f 696d 706f 7274 2874  e().csv_import(t
+0000d6e0: 6578 7477 7261 702e 6465 6465 6e74 2822  extwrap.dedent("
+0000d6f0: 2222 5c0a 2020 2020 2020 2020 612c 632c  ""\.        a,c,
+0000d700: 620a 2020 2020 2020 2020 312c 322c 310a  b.        1,2,1.
+0000d710: 2020 2020 2020 2020 322c 332c 300a 2020          2,3,0.  
+0000d720: 2020 2020 2020 352c 352c 2d31 0a20 2020        5,5,-1.   
+0000d730: 2020 2020 2033 2c34 2c2d 310a 2020 2020       3,4,-1.    
+0000d740: 2020 2020 322c 342c 2d33 2222 2229 2c20      2,4,-3"""), 
+0000d750: 726f 775f 636c 6173 733d 726f 775f 7479  row_class=row_ty
+0000d760: 7065 2c20 7472 616e 7366 6f72 6d73 3d64  pe, transforms=d
+0000d770: 6963 742e 6672 6f6d 6b65 7973 2822 6120  ict.fromkeys("a 
+0000d780: 6220 6322 2e73 706c 6974 2829 2c20 696e  b c".split(), in
+0000d790: 7429 290a 0a20 2020 2020 2020 2064 6566  t))..        def
+0000d7a0: 2074 6f5f 7475 706c 6573 2874 293a 0a20   to_tuples(t):. 
+0000d7b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000d7c0: 6e20 6c69 7374 286d 6170 2861 7474 7267  n list(map(attrg
+0000d7d0: 6574 7465 7228 2a74 2e69 6e66 6f28 295b  etter(*t.info()[
+0000d7e0: 2766 6965 6c64 7327 5d29 2c20 7429 290a  'fields']), t)).
+0000d7f0: 0a20 2020 2020 2020 2070 7269 6e74 2874  .        print(t
+0000d800: 742e 696e 666f 2829 5b27 6669 656c 6473  t.info()['fields
+0000d810: 275d 290a 0a20 2020 2020 2020 2073 6f72  '])..        sor
+0000d820: 745f 6172 6720 3d20 2263 2062 222e 7370  t_arg = "c b".sp
+0000d830: 6c69 7428 290a 2020 2020 2020 2020 7072  lit().        pr
+0000d840: 696e 7428 6622 536f 7274 696e 6720 6279  int(f"Sorting by
+0000d850: 207b 736f 7274 5f61 7267 2172 7d22 290a   {sort_arg!r}").
+0000d860: 2020 2020 2020 2020 7474 2e73 6875 6666          tt.shuff
+0000d870: 6c65 2829 0a20 2020 2020 2020 2074 742e  le().        tt.
+0000d880: 736f 7274 2873 6f72 745f 6172 6729 0a20  sort(sort_arg). 
+0000d890: 2020 2020 2020 2074 315f 7475 706c 6573         t1_tuples
+0000d8a0: 203d 2074 6f5f 7475 706c 6573 2874 7429   = to_tuples(tt)
+0000d8b0: 0a20 2020 2020 2020 2066 6f72 2074 2069  .        for t i
+0000d8c0: 6e20 7431 5f74 7570 6c65 733a 0a20 2020  n t1_tuples:.   
+0000d8d0: 2020 2020 2020 2020 2070 7269 6e74 2874           print(t
+0000d8e0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+0000d8f0: 290a 0a20 2020 2020 2020 2074 742e 7368  )..        tt.sh
+0000d900: 7566 666c 6528 290a 2020 2020 2020 2020  uffle().        
+0000d910: 7474 2e73 6f72 7428 2262 2229 0a20 2020  tt.sort("b").   
+0000d920: 2020 2020 2074 742e 736f 7274 2822 6322       tt.sort("c"
+0000d930: 290a 2020 2020 2020 2020 7432 5f74 7570  ).        t2_tup
+0000d940: 6c65 7320 3d20 746f 5f74 7570 6c65 7328  les = to_tuples(
+0000d950: 7474 290a 2020 2020 2020 2020 666f 7220  tt).        for 
+0000d960: 7420 696e 2074 325f 7475 706c 6573 3a0a  t in t2_tuples:.
+0000d970: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000d980: 7428 7429 0a20 2020 2020 2020 2070 7269  t(t).        pri
+0000d990: 6e74 2829 0a0a 2020 2020 2020 2020 7769  nt()..        wi
+0000d9a0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+0000d9b0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000d9c0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000d9d0: 7431 5f74 7570 6c65 732c 2074 325f 7475  t1_tuples, t2_tu
+0000d9e0: 706c 6573 2c20 2266 6169 6c65 6420 6d75  ples, "failed mu
+0000d9f0: 6c74 692d 6174 7472 6962 7574 6520 736f  lti-attribute so
+0000da00: 7274 2c20 6769 7665 6e20 6c69 7374 206f  rt, given list o
+0000da10: 6620 6174 7472 6962 7574 6573 2229 0a0a  f attributes")..
+0000da20: 2020 2020 2020 2020 736f 7274 5f61 7267          sort_arg
+0000da30: 203d 2022 632c 6222 0a20 2020 2020 2020   = "c,b".       
+0000da40: 2070 7269 6e74 2866 2253 6f72 7469 6e67   print(f"Sorting
+0000da50: 2062 7920 7b73 6f72 745f 6172 6721 727d   by {sort_arg!r}
+0000da60: 2229 0a20 2020 2020 2020 2074 742e 7368  ").        tt.sh
+0000da70: 7566 666c 6528 290a 2020 2020 2020 2020  uffle().        
+0000da80: 7474 2e73 6f72 7428 736f 7274 5f61 7267  tt.sort(sort_arg
+0000da90: 290a 2020 2020 2020 2020 7431 5f74 7570  ).        t1_tup
+0000daa0: 6c65 7320 3d20 746f 5f74 7570 6c65 7328  les = to_tuples(
+0000dab0: 7474 290a 2020 2020 2020 2020 666f 7220  tt).        for 
+0000dac0: 7420 696e 2074 315f 7475 706c 6573 3a0a  t in t1_tuples:.
+0000dad0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000dae0: 7428 7429 0a20 2020 2020 2020 2070 7269  t(t).        pri
+0000daf0: 6e74 2829 0a0a 2020 2020 2020 2020 7474  nt()..        tt
+0000db00: 2e73 6875 6666 6c65 2829 0a20 2020 2020  .shuffle().     
+0000db10: 2020 2074 742e 736f 7274 2822 6222 290a     tt.sort("b").
+0000db20: 2020 2020 2020 2020 7474 2e73 6f72 7428          tt.sort(
+0000db30: 2263 2229 0a20 2020 2020 2020 2074 325f  "c").        t2_
+0000db40: 7475 706c 6573 203d 2074 6f5f 7475 706c  tuples = to_tupl
+0000db50: 6573 2874 7429 0a20 2020 2020 2020 2066  es(tt).        f
+0000db60: 6f72 2074 2069 6e20 7432 5f74 7570 6c65  or t in t2_tuple
+0000db70: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
+0000db80: 7269 6e74 2874 290a 2020 2020 2020 2020  rint(t).        
+0000db90: 7072 696e 7428 290a 0a20 2020 2020 2020  print()..       
+0000dba0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+0000dbb0: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+0000dbc0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000dbd0: 616c 2874 315f 7475 706c 6573 2c20 7432  al(t1_tuples, t2
+0000dbe0: 5f74 7570 6c65 732c 2022 6661 696c 6564  _tuples, "failed
+0000dbf0: 206d 756c 7469 2d61 7474 7269 6275 7465   multi-attribute
+0000dc00: 2073 6f72 742c 2067 6976 656e 2063 6f6d   sort, given com
+0000dc10: 6d61 2d73 6570 6172 6174 6564 2061 7474  ma-separated att
+0000dc20: 7269 6275 7465 7320 7374 7269 6e67 2229  ributes string")
+0000dc30: 0a0a 2020 2020 2020 2020 736f 7274 5f61  ..        sort_a
+0000dc40: 7267 203d 2022 632c 6220 6465 7363 220a  rg = "c,b desc".
+0000dc50: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
+0000dc60: 536f 7274 696e 6720 6279 207b 736f 7274  Sorting by {sort
+0000dc70: 5f61 7267 2172 7d22 290a 2020 2020 2020  _arg!r}").      
+0000dc80: 2020 7474 2e73 6875 6666 6c65 2829 0a20    tt.shuffle(). 
+0000dc90: 2020 2020 2020 2074 742e 736f 7274 2873         tt.sort(s
+0000dca0: 6f72 745f 6172 6729 0a20 2020 2020 2020  ort_arg).       
+0000dcb0: 2074 315f 7475 706c 6573 203d 2074 6f5f   t1_tuples = to_
+0000dcc0: 7475 706c 6573 2874 7429 0a20 2020 2020  tuples(tt).     
+0000dcd0: 2020 2066 6f72 2074 2069 6e20 7431 5f74     for t in t1_t
+0000dce0: 7570 6c65 733a 0a20 2020 2020 2020 2020  uples:.         
+0000dcf0: 2020 2070 7269 6e74 2874 290a 2020 2020     print(t).    
+0000dd00: 2020 2020 7072 696e 7428 290a 0a20 2020      print()..   
+0000dd10: 2020 2020 2074 742e 7368 7566 666c 6528       tt.shuffle(
+0000dd20: 290a 2020 2020 2020 2020 7474 2e73 6f72  ).        tt.sor
+0000dd30: 7428 2262 2064 6573 6322 290a 2020 2020  t("b desc").    
+0000dd40: 2020 2020 7474 2e73 6f72 7428 2263 2229      tt.sort("c")
+0000dd50: 0a20 2020 2020 2020 2074 325f 7475 706c  .        t2_tupl
+0000dd60: 6573 203d 2074 6f5f 7475 706c 6573 2874  es = to_tuples(t
+0000dd70: 7429 0a20 2020 2020 2020 2066 6f72 2074  t).        for t
+0000dd80: 2069 6e20 7432 5f74 7570 6c65 733a 0a20   in t2_tuples:. 
+0000dd90: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000dda0: 2874 290a 2020 2020 2020 2020 7072 696e  (t).        prin
+0000ddb0: 7428 290a 0a20 2020 2020 2020 2077 6974  t()..        wit
+0000ddc0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+0000ddd0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000dde0: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
+0000ddf0: 315f 7475 706c 6573 2c20 7432 5f74 7570  1_tuples, t2_tup
+0000de00: 6c65 732c 2022 6661 696c 6564 206d 6978  les, "failed mix
+0000de10: 6564 2061 7363 656e 6469 6e67 2f64 6573  ed ascending/des
+0000de20: 6365 6e64 696e 6720 6d75 6c74 692d 6174  cending multi-at
+0000de30: 7472 6962 7574 6520 736f 7274 2229 0a0a  tribute sort")..
+0000de40: 2020 2020 6465 6620 7465 7374 5f73 6f72      def test_sor
+0000de50: 7433 2873 656c 6629 3a0a 2020 2020 2020  t3(self):.      
+0000de60: 2020 656d 706c 6f79 6565 7320 3d20 6c74    employees = lt
+0000de70: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
+0000de80: 6f72 7428 7465 7874 7772 6170 2e64 6564  ort(textwrap.ded
+0000de90: 656e 7428 2222 225c 0a20 2020 2020 2020  ent("""\.       
+0000dea0: 2020 2020 2065 6d70 5f69 642c 6e61 6d65       emp_id,name
+0000deb0: 2c64 6570 742c 7361 6c61 7279 2c63 6f6d  ,dept,salary,com
+0000dec0: 6d69 7373 696f 6e0a 2020 2020 2020 2020  mission.        
+0000ded0: 2020 2020 3030 3031 2c41 6c69 6365 2c53      0001,Alice,S
+0000dee0: 616c 6573 2c35 3030 3030 2c30 2e35 0a20  ales,50000,0.5. 
+0000def0: 2020 2020 2020 2020 2020 2030 3030 322c             0002,
+0000df00: 426f 622c 456e 6769 6e65 6572 696e 672c  Bob,Engineering,
+0000df10: 3130 3030 3030 2c0a 2020 2020 2020 2020  100000,.        
+0000df20: 2020 2020 3030 3033 2c43 6861 726c 6573      0003,Charles
+0000df30: 2c53 616c 6573 2c34 3530 3030 2c30 2e37  ,Sales,45000,0.7
+0000df40: 0a20 2020 2020 2020 2020 2020 2030 3030  .            000
+0000df50: 342c 4461 7665 2c53 616c 6573 2c34 3530  4,Dave,Sales,450
+0000df60: 3030 2c30 2e36 0a20 2020 2020 2020 2020  00,0.6.         
+0000df70: 2020 2030 3030 352c 456d 696c 792c 5361     0005,Emily,Sa
+0000df80: 6c65 732c 3530 3030 302c 302e 340a 2020  les,50000,0.4.  
+0000df90: 2020 2020 2020 2020 2020 2222 2229 2c20            """), 
+0000dfa0: 7472 616e 7366 6f72 6d73 3d7b 2273 616c  transforms={"sal
+0000dfb0: 6172 7922 3a20 696e 742c 2022 636f 6d6d  ary": int, "comm
+0000dfc0: 6973 7369 6f6e 223a 2066 6c6f 6174 7d29  ission": float})
+0000dfd0: 0a0a 2020 2020 2020 2020 7361 6c65 735f  ..        sales_
+0000dfe0: 656d 706c 6f79 6565 7320 3d20 656d 706c  employees = empl
+0000dff0: 6f79 6565 732e 7768 6572 6528 6465 7074  oyees.where(dept
+0000e000: 3d22 5361 6c65 7322 292e 736f 7274 2822  ="Sales").sort("
+0000e010: 7361 6c61 7279 2064 6573 632c 636f 6d6d  salary desc,comm
+0000e020: 6973 7369 6f6e 2229 0a0a 2020 2020 2020  ission")..      
+0000e030: 2020 7361 6c65 735f 656d 706c 6f79 6565    sales_employee
+0000e040: 732e 7072 6573 656e 7428 290a 2020 2020  s.present().    
+0000e050: 2020 2020 7072 696e 7428 6c69 7374 2873      print(list(s
+0000e060: 616c 6573 5f65 6d70 6c6f 7965 6573 2e61  ales_employees.a
+0000e070: 6c6c 2e65 6d70 5f69 6429 290a 0a20 2020  ll.emp_id))..   
+0000e080: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+0000e090: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+0000e0a0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000e0b0: 7445 7175 616c 285b 2730 3030 3527 2c20  tEqual(['0005', 
+0000e0c0: 2730 3030 3127 2c20 2730 3030 3427 2c20  '0001', '0004', 
+0000e0d0: 2730 3030 3327 5d2c 0a20 2020 2020 2020  '0003'],.       
+0000e0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0f0: 2020 2020 2020 6c69 7374 2873 616c 6573        list(sales
+0000e100: 5f65 6d70 6c6f 7965 6573 2e61 6c6c 2e65  _employees.all.e
+0000e110: 6d70 5f69 6429 290a 0a20 2020 2064 6566  mp_id))..    def
+0000e120: 2074 6573 745f 756e 6971 7565 2873 656c   test_unique(sel
+0000e130: 6629 3a0a 2020 2020 2020 2020 7465 7374  f):.        test
+0000e140: 5f73 697a 6520 3d20 3130 0a20 2020 2020  _size = 10.     
+0000e150: 2020 2074 3120 3d20 6d61 6b65 5f74 6573     t1 = make_tes
+0000e160: 745f 7461 626c 6528 7365 6c66 2e6d 616b  t_table(self.mak
+0000e170: 655f 6461 7461 5f6f 626a 6563 742c 2074  e_data_object, t
+0000e180: 6573 745f 7369 7a65 290a 0a20 2020 2020  est_size)..     
+0000e190: 2020 2074 3220 3d20 7431 2e75 6e69 7175     t2 = t1.uniqu
+0000e1a0: 6528 290a 2020 2020 2020 2020 7769 7468  e().        with
+0000e1b0: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+0000e1c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000e1d0: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+0000e1e0: 6e28 7431 292c 206c 656e 2874 3229 290a  n(t1), len(t2)).
+0000e1f0: 0a20 2020 2020 2020 2074 3320 3d20 7431  .        t3 = t1
+0000e200: 2e75 6e69 7175 6528 6b65 793d 6c61 6d62  .unique(key=lamb
+0000e210: 6461 2072 6563 3a20 7265 632e 6329 0a20  da rec: rec.c). 
+0000e220: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+0000e230: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+0000e240: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000e250: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
+0000e260: 7a65 2c20 6c65 6e28 7433 2929 0a0a 0a40  ze, len(t3))...@
+0000e270: 6d61 6b65 5f74 6573 745f 636c 6173 7365  make_test_classe
+0000e280: 730a 636c 6173 7320 5461 626c 654f 7574  s.class TableOut
+0000e290: 7075 7454 6573 7473 3a0a 2020 2020 6465  putTests:.    de
+0000e2a0: 6620 7465 7374 5f62 6173 6963 5f70 7265  f test_basic_pre
+0000e2b0: 7365 6e74 2873 656c 6629 3a0a 2020 2020  sent(self):.    
+0000e2c0: 2020 2020 6966 2072 6963 6820 6973 204e      if rich is N
+0000e2d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000e2e0: 2069 6d70 6f72 7420 7761 726e 696e 6773   import warnings
+0000e2f0: 0a20 2020 2020 2020 2020 2020 2077 6172  .            war
+0000e300: 6e69 6e67 732e 7761 726e 2822 7269 6368  nings.warn("rich
+0000e310: 206e 6f74 2069 6e73 7461 6c6c 6564 2c20   not installed, 
+0000e320: 6361 6e6e 6f74 2072 756e 2074 6573 7422  cannot run test"
+0000e330: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+0000e340: 7475 726e 0a0a 2020 2020 2020 2020 6672  turn..        fr
+0000e350: 6f6d 2072 6963 6820 696d 706f 7274 2062  om rich import b
+0000e360: 6f78 0a20 2020 2020 2020 2066 726f 6d20  ox.        from 
+0000e370: 696f 2069 6d70 6f72 7420 5374 7269 6e67  io import String
+0000e380: 494f 0a20 2020 2020 2020 2074 6162 6c65  IO.        table
+0000e390: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
+0000e3a0: 765f 696d 706f 7274 2874 6578 7477 7261  v_import(textwra
+0000e3b0: 702e 6465 6465 6e74 2822 2222 5c0a 2020  p.dedent("""\.  
+0000e3c0: 2020 2020 2020 2020 2020 612c 620a 2020            a,b.  
+0000e3d0: 2020 2020 2020 2020 2020 3130 2c31 3030            10,100
+0000e3e0: 0a20 2020 2020 2020 2020 2020 2032 302c  .            20,
+0000e3f0: 3230 300a 2020 2020 2020 2020 2020 2020  200.            
+0000e400: 2222 2229 290a 2020 2020 2020 2020 7461  """)).        ta
+0000e410: 626c 652e 7072 6573 656e 7428 290a 2020  ble.present().  
+0000e420: 2020 2020 2020 6f75 7420 3d20 5374 7269        out = Stri
+0000e430: 6e67 494f 2829 0a20 2020 2020 2020 2074  ngIO().        t
+0000e440: 6162 6c65 2e70 7265 7365 6e74 2866 696c  able.present(fil
+0000e450: 653d 6f75 742c 2062 6f78 3d62 6f78 2e41  e=out, box=box.A
+0000e460: 5343 4949 290a 2020 2020 2020 2020 6578  SCII).        ex
+0000e470: 7065 6374 6564 203d 2074 6578 7477 7261  pected = textwra
+0000e480: 702e 6465 6465 6e74 2822 2222 5c0a 2020  p.dedent("""\.  
+0000e490: 2020 2020 2020 2020 2020 2b2d 2d2d 2d2d            +-----
+0000e4a0: 2d2d 2d2d 2d2b 0a20 2020 2020 2020 2020  -----+.         
+0000e4b0: 2020 207c 2041 2020 7c20 4220 2020 7c0a     | A  | B   |.
+0000e4c0: 2020 2020 2020 2020 2020 2020 7c2d 2d2d              |---
+0000e4d0: 2d2b 2d2d 2d2d 2d7c 0a20 2020 2020 2020  -+-----|.       
+0000e4e0: 2020 2020 207c 2031 3020 7c20 3130 3020       | 10 | 100 
+0000e4f0: 7c0a 2020 2020 2020 2020 2020 2020 7c20  |.            | 
+0000e500: 3230 207c 2032 3030 207c 0a20 2020 2020  20 | 200 |.     
+0000e510: 2020 2020 2020 202b 2d2d 2d2d 2d2d 2d2d         +--------
+0000e520: 2d2d 2b0a 2020 2020 2020 2020 2020 2020  --+.            
+0000e530: 2222 2229 0a20 2020 2020 2020 2077 6974  """).        wit
+0000e540: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+0000e550: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000e560: 6c66 2e61 7373 6572 7445 7175 616c 2865  lf.assertEqual(e
+0000e570: 7870 6563 7465 642c 206f 7574 2e67 6574  xpected, out.get
+0000e580: 7661 6c75 6528 2929 0a0a 2020 2020 2020  value())..      
+0000e590: 2020 2320 7465 7374 2062 7567 6669 7820    # test bugfix 
+0000e5a0: 7768 656e 2074 6162 6c65 2068 6173 2061  when table has a
+0000e5b0: 7474 7269 6275 7465 2022 6465 6661 756c  ttribute "defaul
+0000e5c0: 7422 0a20 2020 2020 2020 2074 6162 6c65  t".        table
+0000e5d0: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
+0000e5e0: 765f 696d 706f 7274 2874 6578 7477 7261  v_import(textwra
+0000e5f0: 702e 6465 6465 6e74 2822 2222 5c0a 2020  p.dedent("""\.  
+0000e600: 2020 2020 2020 2020 2020 612c 622c 6465            a,b,de
+0000e610: 6661 756c 740a 2020 2020 2020 2020 2020  fault.          
+0000e620: 2020 3130 2c31 3030 2c70 7572 706c 650a    10,100,purple.
+0000e630: 2020 2020 2020 2020 2020 2020 3135 2c31              15,1
+0000e640: 3530 2c0a 2020 2020 2020 2020 2020 2020  50,.            
+0000e650: 3230 2c32 3030 2c6f 7261 6e67 650a 2020  20,200,orange.  
+0000e660: 2020 2020 2020 2020 2020 2222 2229 290a            """)).
+0000e670: 2020 2020 2020 2020 7461 626c 652e 7072          table.pr
+0000e680: 6573 656e 7428 290a 2020 2020 2020 2020  esent().        
+0000e690: 6f75 7420 3d20 5374 7269 6e67 494f 2829  out = StringIO()
+0000e6a0: 0a20 2020 2020 2020 2074 6162 6c65 2e70  .        table.p
+0000e6b0: 7265 7365 6e74 2866 696c 653d 6f75 742c  resent(file=out,
+0000e6c0: 2062 6f78 3d62 6f78 2e41 5343 4949 290a   box=box.ASCII).
+0000e6d0: 2020 2020 2020 2020 6578 7065 6374 6564          expected
+0000e6e0: 203d 2074 6578 7477 7261 702e 6465 6465   = textwrap.dede
+0000e6f0: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
+0000e700: 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d      +-----------
+0000e710: 2d2d 2d2d 2d2d 2d2d 2d2b 0a20 2020 2020  ---------+.     
+0000e720: 2020 2020 2020 207c 2041 2020 7c20 4220         | A  | B 
+0000e730: 2020 7c20 4465 6661 756c 7420 7c0a 2020    | Default |.  
+0000e740: 2020 2020 2020 2020 2020 7c2d 2d2d 2d2b            |----+
+0000e750: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d7c  -----+---------|
+0000e760: 0a20 2020 2020 2020 2020 2020 207c 2031  .            | 1
+0000e770: 3020 7c20 3130 3020 7c20 7075 7270 6c65  0 | 100 | purple
+0000e780: 2020 7c0a 2020 2020 2020 2020 2020 2020    |.            
+0000e790: 7c20 3135 207c 2031 3530 207c 2020 2020  | 15 | 150 |    
+0000e7a0: 2020 2020 207c 0a20 2020 2020 2020 2020       |.         
+0000e7b0: 2020 207c 2032 3020 7c20 3230 3020 7c20     | 20 | 200 | 
+0000e7c0: 6f72 616e 6765 2020 7c0a 2020 2020 2020  orange  |.      
+0000e7d0: 2020 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2d        +---------
+0000e7e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a20 2020  -----------+.   
+0000e7f0: 2020 2020 2020 2020 2022 2222 290a 2020           """).  
+0000e800: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+0000e810: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+0000e820: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0000e830: 7274 4571 7561 6c28 6578 7065 6374 6564  rtEqual(expected
+0000e840: 2c20 6f75 742e 6765 7476 616c 7565 2829  , out.getvalue()
+0000e850: 290a 0a20 2020 2020 2020 2023 2074 6573  )..        # tes
+0000e860: 7420 6772 6f75 7062 790a 2020 2020 2020  t groupby.      
+0000e870: 2020 7461 626c 6520 3d20 6c74 2e54 6162    table = lt.Tab
+0000e880: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
+0000e890: 7465 7874 7772 6170 2e64 6564 656e 7428  textwrap.dedent(
+0000e8a0: 2222 225c 0a20 2020 2020 2020 2020 2020  """\.           
+0000e8b0: 2061 2c62 2c64 6566 6175 6c74 0a20 2020   a,b,default.   
+0000e8c0: 2020 2020 2020 2020 2031 302c 3130 302c           10,100,
+0000e8d0: 7075 7270 6c65 0a20 2020 2020 2020 2020  purple.         
+0000e8e0: 2020 2031 352c 3135 302c 7075 7270 6c65     15,150,purple
+0000e8f0: 0a20 2020 2020 2020 2020 2020 2032 302c  .            20,
+0000e900: 3230 302c 6f72 616e 6765 0a20 2020 2020  200,orange.     
+0000e910: 2020 2020 2020 2022 2222 2929 0a20 2020         """)).   
+0000e920: 2020 2020 2074 6162 6c65 2e70 7265 7365       table.prese
+0000e930: 6e74 2829 0a20 2020 2020 2020 2074 6162  nt().        tab
+0000e940: 6c65 2e70 7265 7365 6e74 2862 6f78 3d62  le.present(box=b
+0000e950: 6f78 2e41 5343 4949 2c20 6772 6f75 7062  ox.ASCII, groupb
+0000e960: 793d 2264 6566 6175 6c74 2229 0a20 2020  y="default").   
+0000e970: 2020 2020 206f 7574 203d 2053 7472 696e       out = Strin
+0000e980: 6749 4f28 290a 2020 2020 2020 2020 7461  gIO().        ta
+0000e990: 626c 652e 7072 6573 656e 7428 6669 6c65  ble.present(file
+0000e9a0: 3d6f 7574 2c20 626f 783d 626f 782e 4153  =out, box=box.AS
+0000e9b0: 4349 492c 2067 726f 7570 6279 3d22 6465  CII, groupby="de
+0000e9c0: 6661 756c 7422 290a 2020 2020 2020 2020  fault").        
+0000e9d0: 6578 7065 6374 6564 203d 2074 6578 7477  expected = textw
+0000e9e0: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
+0000e9f0: 2020 2020 2020 2020 2020 2020 2b2d 2d2d              +---
+0000ea00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ea10: 2d2b 0a20 2020 2020 2020 2020 2020 207c  -+.            |
+0000ea20: 2041 2020 7c20 4220 2020 7c20 4465 6661   A  | B   | Defa
+0000ea30: 756c 7420 7c0a 2020 2020 2020 2020 2020  ult |.          
+0000ea40: 2020 7c2d 2d2d 2d2b 2d2d 2d2d 2d2b 2d2d    |----+-----+--
+0000ea50: 2d2d 2d2d 2d2d 2d7c 0a20 2020 2020 2020  -------|.       
+0000ea60: 2020 2020 207c 2031 3020 7c20 3130 3020       | 10 | 100 
+0000ea70: 7c20 7075 7270 6c65 2020 7c0a 2020 2020  | purple  |.    
+0000ea80: 2020 2020 2020 2020 7c20 3135 207c 2031          | 15 | 1
+0000ea90: 3530 207c 2020 2020 2020 2020 207c 0a20  50 |         |. 
+0000eaa0: 2020 2020 2020 2020 2020 207c 2032 3020             | 20 
+0000eab0: 7c20 3230 3020 7c20 6f72 616e 6765 2020  | 200 | orange  
+0000eac0: 7c0a 2020 2020 2020 2020 2020 2020 2b2d  |.            +-
+0000ead0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000eae0: 2d2d 2d2b 0a20 2020 2020 2020 2020 2020  ---+.           
+0000eaf0: 2022 2222 290a 2020 2020 2020 2020 7769   """).        wi
+0000eb00: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+0000eb10: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000eb20: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000eb30: 6578 7065 6374 6564 2c20 6f75 742e 6765  expected, out.ge
+0000eb40: 7476 616c 7565 2829 290a 0a20 2020 2020  tvalue())..     
+0000eb50: 2020 2074 6162 6c65 203d 206c 742e 5461     table = lt.Ta
+0000eb60: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
+0000eb70: 2874 6578 7477 7261 702e 6465 6465 6e74  (textwrap.dedent
+0000eb80: 2822 2222 5c0a 2020 2020 2020 2020 2020  ("""\.          
+0000eb90: 2020 612c 622c 6465 6661 756c 740a 2020    a,b,default.  
+0000eba0: 2020 2020 2020 2020 2020 3130 2c31 3030            10,100
+0000ebb0: 2c70 7572 706c 650a 2020 2020 2020 2020  ,purple.        
+0000ebc0: 2020 2020 3135 2c31 3530 2c70 7572 706c      15,150,purpl
+0000ebd0: 650a 2020 2020 2020 2020 2020 2020 3135  e.            15
+0000ebe0: 2c32 3030 2c6f 7261 6e67 650a 2020 2020  ,200,orange.    
+0000ebf0: 2020 2020 2020 2020 3135 2c32 3530 2c6f          15,250,o
+0000ec00: 7261 6e67 650a 2020 2020 2020 2020 2020  range.          
+0000ec10: 2020 3230 2c32 3530 2c6f 7261 6e67 650a    20,250,orange.
+0000ec20: 2020 2020 2020 2020 2020 2020 2222 2229              """)
+0000ec30: 290a 2020 2020 2020 2020 7461 626c 652e  ).        table.
+0000ec40: 7072 6573 656e 7428 290a 2020 2020 2020  present().      
+0000ec50: 2020 7461 626c 652e 7072 6573 656e 7428    table.present(
+0000ec60: 626f 783d 626f 782e 4153 4349 492c 2067  box=box.ASCII, g
+0000ec70: 726f 7570 6279 3d22 6465 6661 756c 7420  roupby="default 
+0000ec80: 6122 290a 2020 2020 2020 2020 6f75 7420  a").        out 
+0000ec90: 3d20 5374 7269 6e67 494f 2829 0a20 2020  = StringIO().   
+0000eca0: 2020 2020 2074 6162 6c65 2e70 7265 7365       table.prese
+0000ecb0: 6e74 2866 696c 653d 6f75 742c 2062 6f78  nt(file=out, box
+0000ecc0: 3d62 6f78 2e41 5343 4949 2c20 6772 6f75  =box.ASCII, grou
+0000ecd0: 7062 793d 2264 6566 6175 6c74 2061 2229  pby="default a")
+0000ece0: 0a20 2020 2020 2020 2065 7870 6563 7465  .        expecte
+0000ecf0: 6420 3d20 7465 7874 7772 6170 2e64 6564  d = textwrap.ded
+0000ed00: 656e 7428 2222 225c 0a20 2020 2020 2020  ent("""\.       
+0000ed10: 2020 2020 202b 2d2d 2d2d 2d2d 2d2d 2d2d       +----------
+0000ed20: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  ----------+.    
+0000ed30: 2020 2020 2020 2020 7c20 4120 207c 2042          | A  | B
+0000ed40: 2020 207c 2044 6566 6175 6c74 207c 0a20     | Default |. 
+0000ed50: 2020 2020 2020 2020 2020 207c 2d2d 2d2d             |----
+0000ed60: 2b2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  +-----+---------
+0000ed70: 7c0a 2020 2020 2020 2020 2020 2020 7c20  |.            | 
+0000ed80: 3130 207c 2031 3030 207c 2070 7572 706c  10 | 100 | purpl
+0000ed90: 6520 207c 0a20 2020 2020 2020 2020 2020  e  |.           
+0000eda0: 207c 2031 3520 7c20 3135 3020 7c20 2020   | 15 | 150 |   
+0000edb0: 2020 2020 2020 7c0a 2020 2020 2020 2020        |.        
+0000edc0: 2020 2020 7c20 3135 207c 2032 3030 207c      | 15 | 200 |
+0000edd0: 206f 7261 6e67 6520 207c 0a20 2020 2020   orange  |.     
+0000ede0: 2020 2020 2020 207c 2020 2020 7c20 3235         |    | 25
+0000edf0: 3020 7c20 2020 2020 2020 2020 7c0a 2020  0 |         |.  
+0000ee00: 2020 2020 2020 2020 2020 7c20 3230 207c            | 20 |
+0000ee10: 2032 3530 207c 2020 2020 2020 2020 207c   250 |         |
+0000ee20: 0a20 2020 2020 2020 2020 2020 202b 2d2d  .            +--
+0000ee30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ee40: 2d2d 2b0a 2020 2020 2020 2020 2020 2020  --+.            
+0000ee50: 2222 2229 0a20 2020 2020 2020 2077 6974  """).        wit
+0000ee60: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+0000ee70: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000ee80: 6c66 2e61 7373 6572 7445 7175 616c 2865  lf.assertEqual(e
+0000ee90: 7870 6563 7465 642c 206f 7574 2e67 6574  xpected, out.get
+0000eea0: 7661 6c75 6528 2929 0a0a 2020 2020 2020  value())..      
+0000eeb0: 2020 7461 626c 6520 3d20 6c74 2e54 6162    table = lt.Tab
+0000eec0: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
 0000eed0: 7465 7874 7772 6170 2e64 6564 656e 7428  textwrap.dedent(
 0000eee0: 2222 225c 0a20 2020 2020 2020 2020 2020  """\.           
-0000eef0: 207c 2061 207c 2062 207c 0a20 2020 2020   | a | b |.     
-0000ef00: 2020 2020 2020 207c 2d2d 2d7c 2d2d 2d7c         |---|---|
-0000ef10: 0a20 2020 2020 2020 2020 2020 207c 2031  .            | 1
-0000ef20: 3020 7c20 3130 3020 7c0a 2020 2020 2020  0 | 100 |.      
-0000ef30: 2020 2020 2020 7c20 3230 207c 2032 3030        | 20 | 200
-0000ef40: 207c 0a20 2020 2020 2020 2020 2020 2022   |.            "
-0000ef50: 2222 290a 2020 2020 2020 2020 7769 7468  "").        with
-0000ef60: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-0000ef70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000ef80: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
-0000ef90: 7065 6374 6564 2c20 6f75 745f 6d61 726b  pected, out_mark
-0000efa0: 646f 776e 290a 0a20 2020 2020 2020 2023  down)..        #
-0000efb0: 2074 6573 7420 6275 6766 6978 2077 6865   test bugfix whe
-0000efc0: 6e20 7461 626c 6520 6861 7320 6174 7472  n table has attr
-0000efd0: 6962 7574 6520 2264 6566 6175 6c74 220a  ibute "default".
-0000efe0: 2020 2020 2020 2020 7461 626c 6520 3d20          table = 
-0000eff0: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
-0000f000: 6d70 6f72 7428 7465 7874 7772 6170 2e64  mport(textwrap.d
-0000f010: 6564 656e 7428 2222 225c 0a20 2020 2020  edent("""\.     
-0000f020: 2020 2020 2020 2061 2c62 2c64 6566 6175         a,b,defau
-0000f030: 6c74 0a20 2020 2020 2020 2020 2020 2031  lt.            1
-0000f040: 302c 3130 302c 7075 7270 6c65 0a20 2020  0,100,purple.   
-0000f050: 2020 2020 2020 2020 2031 352c 3135 302c           15,150,
-0000f060: 0a20 2020 2020 2020 2020 2020 2032 302c  .            20,
-0000f070: 3230 302c 6f72 616e 6765 0a20 2020 2020  200,orange.     
-0000f080: 2020 2020 2020 2022 2222 2929 0a20 2020         """)).   
-0000f090: 2020 2020 206f 7574 5f6d 6172 6b64 6f77       out_markdow
-0000f0a0: 6e20 3d20 7461 626c 652e 6173 5f6d 6172  n = table.as_mar
-0000f0b0: 6b64 6f77 6e28 290a 2020 2020 2020 2020  kdown().        
-0000f0c0: 7072 696e 7428 6f75 745f 6d61 726b 646f  print(out_markdo
-0000f0d0: 776e 290a 2020 2020 2020 2020 6578 7065  wn).        expe
-0000f0e0: 6374 6564 203d 2074 6578 7477 7261 702e  cted = textwrap.
-0000f0f0: 6465 6465 6e74 2822 2222 5c0a 2020 2020  dedent("""\.    
-0000f100: 2020 2020 2020 2020 7c20 6120 7c20 6220          | a | b 
-0000f110: 7c20 6465 6661 756c 7420 7c0a 2020 2020  | default |.    
-0000f120: 2020 2020 2020 2020 7c2d 2d2d 7c2d 2d2d          |---|---
-0000f130: 7c2d 2d2d 7c0a 2020 2020 2020 2020 2020  |---|.          
-0000f140: 2020 7c20 3130 207c 2031 3030 207c 2070    | 10 | 100 | p
-0000f150: 7572 706c 6520 7c0a 2020 2020 2020 2020  urple |.        
-0000f160: 2020 2020 7c20 3135 207c 2031 3530 207c      | 15 | 150 |
-0000f170: 2020 7c0a 2020 2020 2020 2020 2020 2020    |.            
-0000f180: 7c20 3230 207c 2032 3030 207c 206f 7261  | 20 | 200 | ora
-0000f190: 6e67 6520 7c0a 2020 2020 2020 2020 2020  nge |.          
-0000f1a0: 2020 2222 2229 0a20 2020 2020 2020 2077    """).        w
-0000f1b0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-0000f1c0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000f1d0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000f1e0: 2865 7870 6563 7465 642c 206f 7574 5f6d  (expected, out_m
-0000f1f0: 6172 6b64 6f77 6e29 0a0a 2020 2020 2020  arkdown)..      
-0000f200: 2020 2320 7465 7374 2067 726f 7570 696e    # test groupin
-0000f210: 6720 696e 2061 735f 6d61 726b 646f 776e  g in as_markdown
-0000f220: 0a20 2020 2020 2020 2074 6162 6c65 203d  .        table =
-0000f230: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
-0000f240: 696d 706f 7274 2874 6578 7477 7261 702e  import(textwrap.
-0000f250: 6465 6465 6e74 2822 2222 5c0a 2020 2020  dedent("""\.    
-0000f260: 2020 2020 2020 2020 612c 622c 6465 6661          a,b,defa
-0000f270: 756c 740a 2020 2020 2020 2020 2020 2020  ult.            
-0000f280: 3130 2c31 3030 2c70 7572 706c 650a 2020  10,100,purple.  
-0000f290: 2020 2020 2020 2020 2020 3135 2c31 3530            15,150
-0000f2a0: 2c70 7572 706c 650a 2020 2020 2020 2020  ,purple.        
-0000f2b0: 2020 2020 3230 2c32 3030 2c6f 7261 6e67      20,200,orang
-0000f2c0: 650a 2020 2020 2020 2020 2020 2020 2222  e.            ""
-0000f2d0: 2229 290a 2020 2020 2020 2020 6f75 745f  ")).        out_
-0000f2e0: 6d61 726b 646f 776e 203d 2074 6162 6c65  markdown = table
-0000f2f0: 2e61 735f 6d61 726b 646f 776e 2867 726f  .as_markdown(gro
-0000f300: 7570 6279 3d22 6465 6661 756c 7422 290a  upby="default").
-0000f310: 2020 2020 2020 2020 7072 696e 7428 6f75          print(ou
-0000f320: 745f 6d61 726b 646f 776e 290a 2020 2020  t_markdown).    
-0000f330: 2020 2020 6578 7065 6374 6564 203d 2074      expected = t
-0000f340: 6578 7477 7261 702e 6465 6465 6e74 2822  extwrap.dedent("
-0000f350: 2222 5c0a 2020 2020 2020 2020 2020 2020  ""\.            
-0000f360: 7c20 6120 7c20 6220 7c20 6465 6661 756c  | a | b | defaul
-0000f370: 7420 7c0a 2020 2020 2020 2020 2020 2020  t |.            
-0000f380: 7c2d 2d2d 7c2d 2d2d 7c2d 2d2d 7c0a 2020  |---|---|---|.  
-0000f390: 2020 2020 2020 2020 2020 7c20 3130 207c            | 10 |
-0000f3a0: 2031 3030 207c 2070 7572 706c 6520 7c0a   100 | purple |.
-0000f3b0: 2020 2020 2020 2020 2020 2020 7c20 3135              | 15
-0000f3c0: 207c 2031 3530 207c 2020 7c0a 2020 2020   | 150 |  |.    
-0000f3d0: 2020 2020 2020 2020 7c20 3230 207c 2032          | 20 | 2
-0000f3e0: 3030 207c 206f 7261 6e67 6520 7c0a 2020  00 | orange |.  
-0000f3f0: 2020 2020 2020 2020 2020 2222 2229 0a20            """). 
-0000f400: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-0000f410: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-0000f420: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0000f430: 6572 7445 7175 616c 2865 7870 6563 7465  ertEqual(expecte
-0000f440: 642c 206f 7574 5f6d 6172 6b64 6f77 6e29  d, out_markdown)
-0000f450: 0a0a 2020 2020 2020 2020 7461 626c 6520  ..        table 
-0000f460: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
-0000f470: 5f69 6d70 6f72 7428 7465 7874 7772 6170  _import(textwrap
-0000f480: 2e64 6564 656e 7428 2222 225c 0a20 2020  .dedent("""\.   
-0000f490: 2020 2020 2020 2020 2061 2c62 2c64 6566           a,b,def
-0000f4a0: 6175 6c74 0a20 2020 2020 2020 2020 2020  ault.           
-0000f4b0: 2031 302c 3130 302c 7075 7270 6c65 0a20   10,100,purple. 
-0000f4c0: 2020 2020 2020 2020 2020 2031 352c 3230             15,20
-0000f4d0: 302c 6f72 616e 6765 0a20 2020 2020 2020  0,orange.       
-0000f4e0: 2020 2020 2031 352c 3135 302c 7075 7270       15,150,purp
-0000f4f0: 6c65 0a20 2020 2020 2020 2020 2020 2032  le.            2
-0000f500: 302c 3235 302c 6f72 616e 6765 0a20 2020  0,250,orange.   
-0000f510: 2020 2020 2020 2020 2031 352c 3235 302c           15,250,
-0000f520: 6f72 616e 6765 0a20 2020 2020 2020 2020  orange.         
-0000f530: 2020 2022 2222 2929 0a20 2020 2020 2020     """)).       
-0000f540: 2074 6162 6c65 2e73 6f72 7428 2264 6566   table.sort("def
-0000f550: 6175 6c74 2064 6573 632c 6122 290a 2020  ault desc,a").  
-0000f560: 2020 2020 2020 6f75 745f 6d61 726b 646f        out_markdo
-0000f570: 776e 203d 2074 6162 6c65 2e61 735f 6d61  wn = table.as_ma
-0000f580: 726b 646f 776e 2867 726f 7570 6279 3d22  rkdown(groupby="
-0000f590: 6465 6661 756c 7420 6122 290a 2020 2020  default a").    
-0000f5a0: 2020 2020 7072 696e 7428 6f75 745f 6d61      print(out_ma
-0000f5b0: 726b 646f 776e 290a 2020 2020 2020 2020  rkdown).        
-0000f5c0: 6578 7065 6374 6564 203d 2074 6578 7477  expected = textw
-0000f5d0: 7261 702e 6465 6465 6e74 2822 2222 5c0a  rap.dedent("""\.
-0000f5e0: 2020 2020 2020 2020 2020 2020 7c20 6120              | a 
-0000f5f0: 7c20 6220 7c20 6465 6661 756c 7420 7c0a  | b | default |.
-0000f600: 2020 2020 2020 2020 2020 2020 7c2d 2d2d              |---
-0000f610: 7c2d 2d2d 7c2d 2d2d 7c0a 2020 2020 2020  |---|---|.      
-0000f620: 2020 2020 2020 7c20 3130 207c 2031 3030        | 10 | 100
-0000f630: 207c 2070 7572 706c 6520 7c0a 2020 2020   | purple |.    
-0000f640: 2020 2020 2020 2020 7c20 3135 207c 2031          | 15 | 1
-0000f650: 3530 207c 2020 7c0a 2020 2020 2020 2020  50 |  |.        
-0000f660: 2020 2020 7c20 3135 207c 2032 3030 207c      | 15 | 200 |
-0000f670: 206f 7261 6e67 6520 7c0a 2020 2020 2020   orange |.      
-0000f680: 2020 2020 2020 7c20 207c 2032 3530 207c        |  | 250 |
-0000f690: 2020 7c0a 2020 2020 2020 2020 2020 2020    |.            
-0000f6a0: 7c20 3230 207c 2032 3530 207c 2020 7c0a  | 20 | 250 |  |.
-0000f6b0: 2020 2020 2020 2020 2020 2020 2222 2229              """)
-0000f6c0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0000f6d0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-0000f6e0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000f6f0: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
-0000f700: 7465 642c 206f 7574 5f6d 6172 6b64 6f77  ted, out_markdow
-0000f710: 6e29 0a0a 2320 7361 6d70 6c65 2069 6d70  n)..# sample imp
-0000f720: 6f72 7420 6461 7461 2073 6574 730a 6373  ort data sets.cs
-0000f730: 765f 6461 7461 203d 2022 2222 5c0a 612c  v_data = """\.a,
-0000f740: 622c 630a 302c 302c 300a 302c 302c 310a  b,c.0,0,0.0,0,1.
-0000f750: 302c 302c 320a 302c 312c 300a 302c 312c  0,0,2.0,1,0.0,1,
-0000f760: 310a 302c 312c 320a 302c 322c 300a 302c  1.0,1,2.0,2,0.0,
-0000f770: 322c 310a 302c 322c 320a 312c 302c 300a  2,1.0,2,2.1,0,0.
-0000f780: 312c 302c 310a 312c 302c 320a 312c 312c  1,0,1.1,0,2.1,1,
-0000f790: 300a 312c 312c 310a 312c 312c 320a 312c  0.1,1,1.1,1,2.1,
-0000f7a0: 322c 300a 312c 322c 310a 312c 322c 320a  2,0.1,2,1.1,2,2.
-0000f7b0: 322c 302c 300a 322c 302c 310a 322c 302c  2,0,0.2,0,1.2,0,
-0000f7c0: 320a 322c 312c 300a 322c 312c 310a 322c  2.2,1,0.2,1,1.2,
-0000f7d0: 312c 320a 322c 322c 300a 322c 322c 310a  1,2.2,2,0.2,2,1.
-0000f7e0: 322c 322c 320a 0a22 2222 0a0a 6a73 6f6e  2,2,2.."""..json
-0000f7f0: 5f64 6174 6120 3d20 2222 225c 0a20 2020  _data = """\.   
-0000f800: 207b 2261 223a 2030 2c20 2262 223a 2030   {"a": 0, "b": 0
-0000f810: 2c20 2263 223a 2030 7d0a 2020 2020 7b22  , "c": 0}.    {"
-0000f820: 6122 3a20 302c 2022 6222 3a20 302c 2022  a": 0, "b": 0, "
-0000f830: 6322 3a20 317d 0a20 2020 207b 2261 223a  c": 1}.    {"a":
-0000f840: 2030 2c20 2262 223a 2030 2c20 2263 223a   0, "b": 0, "c":
-0000f850: 2032 7d0a 2020 2020 7b22 6122 3a20 302c   2}.    {"a": 0,
-0000f860: 2022 6222 3a20 312c 2022 6322 3a20 307d   "b": 1, "c": 0}
-0000f870: 0a20 2020 207b 2261 223a 2030 2c20 2262  .    {"a": 0, "b
-0000f880: 223a 2031 2c20 2263 223a 2031 7d0a 2020  ": 1, "c": 1}.  
-0000f890: 2020 7b22 6122 3a20 302c 2022 6222 3a20    {"a": 0, "b": 
-0000f8a0: 312c 2022 6322 3a20 327d 0a20 2020 207b  1, "c": 2}.    {
-0000f8b0: 2261 223a 2030 2c20 2262 223a 2032 2c20  "a": 0, "b": 2, 
-0000f8c0: 2263 223a 2030 7d0a 2020 2020 7b22 6122  "c": 0}.    {"a"
-0000f8d0: 3a20 302c 2022 6222 3a20 322c 2022 6322  : 0, "b": 2, "c"
-0000f8e0: 3a20 317d 0a20 2020 207b 2261 223a 2030  : 1}.    {"a": 0
-0000f8f0: 2c20 2262 223a 2032 2c20 2263 223a 2032  , "b": 2, "c": 2
-0000f900: 7d0a 2020 2020 7b22 6122 3a20 312c 2022  }.    {"a": 1, "
-0000f910: 6222 3a20 302c 2022 6322 3a20 307d 0a20  b": 0, "c": 0}. 
-0000f920: 2020 207b 2261 223a 2031 2c20 2262 223a     {"a": 1, "b":
-0000f930: 2030 2c20 2263 223a 2031 7d0a 2020 2020   0, "c": 1}.    
-0000f940: 7b22 6122 3a20 312c 2022 6222 3a20 302c  {"a": 1, "b": 0,
-0000f950: 2022 6322 3a20 327d 0a20 2020 207b 2261   "c": 2}.    {"a
-0000f960: 223a 2031 2c20 2262 223a 2031 2c20 2263  ": 1, "b": 1, "c
-0000f970: 223a 2030 7d0a 2020 2020 7b22 6122 3a20  ": 0}.    {"a": 
-0000f980: 312c 2022 6222 3a20 312c 2022 6322 3a20  1, "b": 1, "c": 
-0000f990: 317d 0a20 2020 207b 2261 223a 2031 2c20  1}.    {"a": 1, 
-0000f9a0: 2262 223a 2031 2c20 2263 223a 2032 7d0a  "b": 1, "c": 2}.
-0000f9b0: 2020 2020 7b22 6122 3a20 312c 2022 6222      {"a": 1, "b"
-0000f9c0: 3a20 322c 2022 6322 3a20 307d 0a20 2020  : 2, "c": 0}.   
-0000f9d0: 207b 2261 223a 2031 2c20 2262 223a 2032   {"a": 1, "b": 2
-0000f9e0: 2c20 2263 223a 2031 7d0a 2020 2020 7b22  , "c": 1}.    {"
-0000f9f0: 6122 3a20 312c 2022 6222 3a20 322c 2022  a": 1, "b": 2, "
-0000fa00: 6322 3a20 327d 0a20 2020 207b 2261 223a  c": 2}.    {"a":
-0000fa10: 2032 2c20 2262 223a 2030 2c20 2263 223a   2, "b": 0, "c":
-0000fa20: 2030 7d0a 2020 2020 7b22 6122 3a20 322c   0}.    {"a": 2,
-0000fa30: 2022 6222 3a20 302c 2022 6322 3a20 317d   "b": 0, "c": 1}
-0000fa40: 0a20 2020 207b 2261 223a 2032 2c20 2262  .    {"a": 2, "b
-0000fa50: 223a 2030 2c20 2263 223a 2032 7d0a 2020  ": 0, "c": 2}.  
-0000fa60: 2020 7b22 6122 3a20 322c 2022 6222 3a20    {"a": 2, "b": 
-0000fa70: 312c 2022 6322 3a20 307d 0a20 2020 207b  1, "c": 0}.    {
-0000fa80: 2261 223a 2032 2c20 2262 223a 2031 2c20  "a": 2, "b": 1, 
-0000fa90: 2263 223a 2031 7d0a 2020 2020 7b22 6122  "c": 1}.    {"a"
-0000faa0: 3a20 322c 2022 6222 3a20 312c 2022 6322  : 2, "b": 1, "c"
-0000fab0: 3a20 327d 0a20 2020 207b 2261 223a 2032  : 2}.    {"a": 2
-0000fac0: 2c20 2262 223a 2032 2c20 2263 223a 2030  , "b": 2, "c": 0
-0000fad0: 7d0a 2020 2020 7b22 6122 3a20 322c 2022  }.    {"a": 2, "
-0000fae0: 6222 3a20 322c 2022 6322 3a20 317d 0a20  b": 2, "c": 1}. 
-0000faf0: 2020 207b 2261 223a 2032 2c20 2262 223a     {"a": 2, "b":
-0000fb00: 2032 2c20 2263 223a 2032 7d0a 0a22 2222   2, "c": 2}.."""
-0000fb10: 0a0a 6669 7865 645f 7769 6474 685f 6461  ..fixed_width_da
-0000fb20: 7461 203d 2022 2222 5c0a 3020 3020 300a  ta = """\.0 0 0.
-0000fb30: 3020 3020 310a 3020 3020 320a 3020 3120  0 0 1.0 0 2.0 1 
-0000fb40: 300a 3020 3120 310a 3020 3120 320a 3020  0.0 1 1.0 1 2.0 
-0000fb50: 3220 300a 3020 3220 310a 3020 3220 320a  2 0.0 2 1.0 2 2.
-0000fb60: 3120 3020 300a 3120 3020 310a 3120 3020  1 0 0.1 0 1.1 0 
-0000fb70: 320a 3120 3120 300a 3120 3120 310a 3120  2.1 1 0.1 1 1.1 
-0000fb80: 3120 320a 3120 3220 300a 3120 3220 310a  1 2.1 2 0.1 2 1.
-0000fb90: 3120 3220 320a 3220 3020 300a 3220 3020  1 2 2.2 0 0.2 0 
-0000fba0: 310a 3220 3020 320a 3220 3120 300a 3220  1.2 0 2.2 1 0.2 
-0000fbb0: 3120 310a 3220 3120 320a 3220 3220 300a  1 1.2 1 2.2 2 0.
-0000fbc0: 3220 3220 310a 3220 3220 320a 0a22 2222  2 2 1.2 2 2.."""
-0000fbd0: 0a0a 0a40 6d61 6b65 5f74 6573 745f 636c  ...@make_test_cl
-0000fbe0: 6173 7365 730a 636c 6173 7320 5461 626c  asses.class Tabl
-0000fbf0: 6549 6d70 6f72 7445 7870 6f72 7454 6573  eImportExportTes
-0000fc00: 7473 3a0a 2020 2020 6465 6620 7465 7374  ts:.    def test
-0000fc10: 5f63 7376 5f65 7870 6f72 7428 7365 6c66  _csv_export(self
-0000fc20: 293a 0a20 2020 2020 2020 2066 726f 6d20  ):.        from 
-0000fc30: 6974 6572 746f 6f6c 7320 696d 706f 7274  itertools import
-0000fc40: 2070 6572 6d75 7461 7469 6f6e 730a 2020   permutations.  
-0000fc50: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
-0000fc60: 3d20 330a 2020 2020 2020 2020 7431 203d  = 3.        t1 =
-0000fc70: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
-0000fc80: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
-0000fc90: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
-0000fca0: 6529 0a20 2020 2020 2020 2066 6f72 2066  e).        for f
-0000fcb0: 6965 6c64 6e61 6d65 7320 696e 2070 6572  ieldnames in per
-0000fcc0: 6d75 7461 7469 6f6e 7328 6c69 7374 2827  mutations(list('
-0000fcd0: 6162 6327 2929 3a0a 2020 2020 2020 2020  abc')):.        
-0000fce0: 2020 2020 6f75 7420 3d20 696f 2e53 7472      out = io.Str
-0000fcf0: 696e 6749 4f28 290a 2020 2020 2020 2020  ingIO().        
-0000fd00: 2020 2020 7431 2e63 7376 5f65 7870 6f72      t1.csv_expor
-0000fd10: 7428 6f75 742c 2066 6965 6c64 6e61 6d65  t(out, fieldname
-0000fd20: 7329 0a20 2020 2020 2020 2020 2020 206f  s).            o
-0000fd30: 7574 2e73 6565 6b28 3029 0a20 2020 2020  ut.seek(0).     
-0000fd40: 2020 2020 2020 206f 7574 6c69 6e65 7320         outlines 
-0000fd50: 3d20 6f75 742e 7265 6164 2829 2e73 706c  = out.read().spl
-0000fd60: 6974 6c69 6e65 7328 290a 2020 2020 2020  itlines().      
-0000fd70: 2020 2020 2020 6f75 742e 636c 6f73 6528        out.close(
-0000fd80: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
-0000fd90: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-0000fda0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000fdb0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0000fdc0: 7561 6c28 272c 272e 6a6f 696e 2866 6965  ual(','.join(fie
-0000fdd0: 6c64 6e61 6d65 7329 2c20 6f75 746c 696e  ldnames), outlin
-0000fde0: 6573 5b30 5d29 0a20 2020 2020 2020 2020  es[0]).         
-0000fdf0: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-0000fe00: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-0000fe10: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0000fe20: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
-0000fe30: 7a65 2a2a 332b 312c 206c 656e 286f 7574  ze**3+1, len(out
-0000fe40: 6c69 6e65 7329 290a 2020 2020 2020 2020  lines)).        
-0000fe50: 2020 2020 666f 7220 6f62 2c20 6c69 6e65      for ob, line
-0000fe60: 2069 6e20 7a69 7028 7431 2c20 6f75 746c   in zip(t1, outl
-0000fe70: 696e 6573 5b31 3a5d 293a 0a20 2020 2020  ines[1:]):.     
-0000fe80: 2020 2020 2020 2020 2020 2063 7376 5f76             csv_v
-0000fe90: 616c 7320 3d20 6c69 6e65 2e73 706c 6974  als = line.split
-0000fea0: 2827 2c27 290a 2020 2020 2020 2020 2020  (',').          
-0000feb0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0000fec0: 7375 6254 6573 7428 6f62 3d6f 622c 2063  subTest(ob=ob, c
-0000fed0: 7376 5f76 616c 733d 6373 765f 7661 6c73  sv_vals=csv_vals
-0000fee0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000fef0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000ff00: 7274 5472 7565 2861 6c6c 280a 2020 2020  rtTrue(all(.    
-0000ff10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff20: 2020 2020 696e 7428 6373 765f 7661 6c73      int(csv_vals
-0000ff30: 5b69 5d29 203d 3d20 6765 7461 7474 7228  [i]) == getattr(
-0000ff40: 6f62 2c20 666c 6429 2066 6f72 2069 2c20  ob, fld) for i, 
-0000ff50: 666c 6420 696e 2065 6e75 6d65 7261 7465  fld in enumerate
-0000ff60: 2866 6965 6c64 6e61 6d65 7329 0a20 2020  (fieldnames).   
-0000ff70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff80: 2029 290a 0a20 2020 2020 2020 2023 2072   ))..        # r
-0000ff90: 6572 756e 2075 7369 6e67 2061 6e20 656d  erun using an em
-0000ffa0: 7074 7920 7461 626c 650a 2020 2020 2020  pty table.      
-0000ffb0: 2020 7431 203d 206c 742e 5461 626c 6528    t1 = lt.Table(
-0000ffc0: 290a 2020 2020 2020 2020 666f 7220 6669  ).        for fi
-0000ffd0: 656c 646e 616d 6573 2069 6e20 7065 726d  eldnames in perm
-0000ffe0: 7574 6174 696f 6e73 286c 6973 7428 2761  utations(list('a
-0000fff0: 6263 2729 293a 0a20 2020 2020 2020 2020  bc')):.         
-00010000: 2020 206f 7574 203d 2069 6f2e 5374 7269     out = io.Stri
-00010010: 6e67 494f 2829 0a20 2020 2020 2020 2020  ngIO().         
-00010020: 2020 2074 312e 6373 765f 6578 706f 7274     t1.csv_export
-00010030: 286f 7574 2c20 6669 656c 646e 616d 6573  (out, fieldnames
-00010040: 290a 2020 2020 2020 2020 2020 2020 6f75  ).            ou
-00010050: 742e 7365 656b 2830 290a 2020 2020 2020  t.seek(0).      
-00010060: 2020 2020 2020 6f75 746c 696e 6573 203d        outlines =
-00010070: 206f 7574 2e72 6561 6428 292e 7370 6c69   out.read().spli
-00010080: 746c 696e 6573 2829 0a20 2020 2020 2020  tlines().       
-00010090: 2020 2020 206f 7574 2e63 6c6f 7365 2829       out.close()
-000100a0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-000100b0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-000100c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000100d0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000100e0: 616c 2827 2c27 2e6a 6f69 6e28 6669 656c  al(','.join(fiel
-000100f0: 646e 616d 6573 292c 206f 7574 6c69 6e65  dnames), outline
-00010100: 735b 305d 290a 2020 2020 2020 2020 2020  s[0]).          
-00010110: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-00010120: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-00010130: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00010140: 7274 4571 7561 6c28 312c 206c 656e 286f  rtEqual(1, len(o
-00010150: 7574 6c69 6e65 7329 290a 0a20 2020 2020  utlines))..     
-00010160: 2020 2023 2072 6572 756e 2075 7369 6e67     # rerun using
-00010170: 2061 6e20 656d 7074 7920 7461 626c 652c   an empty table,
-00010180: 2077 6974 6820 696e 6465 7865 7320 746f   with indexes to
-00010190: 2064 6963 7461 7465 2066 6965 6c64 6e61   dictate fieldna
-000101a0: 6d65 730a 2020 2020 2020 2020 666f 7220  mes.        for 
-000101b0: 6669 656c 646e 616d 6573 2069 6e20 7065  fieldnames in pe
-000101c0: 726d 7574 6174 696f 6e73 286c 6973 7428  rmutations(list(
-000101d0: 2761 6263 2729 293a 0a20 2020 2020 2020  'abc')):.       
-000101e0: 2020 2020 2074 3120 3d20 6c74 2e54 6162       t1 = lt.Tab
-000101f0: 6c65 2829 0a20 2020 2020 2020 2020 2020  le().           
-00010200: 2066 6f72 2066 6c64 2069 6e20 6669 656c   for fld in fiel
-00010210: 646e 616d 6573 3a0a 2020 2020 2020 2020  dnames:.        
-00010220: 2020 2020 2020 2020 7431 2e63 7265 6174          t1.creat
-00010230: 655f 696e 6465 7828 666c 6429 0a20 2020  e_index(fld).   
-00010240: 2020 2020 2020 2020 206f 7574 203d 2069           out = i
-00010250: 6f2e 5374 7269 6e67 494f 2829 0a20 2020  o.StringIO().   
-00010260: 2020 2020 2020 2020 2074 312e 6373 765f           t1.csv_
-00010270: 6578 706f 7274 286f 7574 290a 2020 2020  export(out).    
-00010280: 2020 2020 2020 2020 6f75 742e 7365 656b          out.seek
-00010290: 2830 290a 2020 2020 2020 2020 2020 2020  (0).            
-000102a0: 6f75 746c 696e 6573 203d 206f 7574 2e72  outlines = out.r
-000102b0: 6561 6428 292e 7370 6c69 746c 696e 6573  ead().splitlines
-000102c0: 2829 0a20 2020 2020 2020 2020 2020 206f  ().            o
-000102d0: 7574 2e63 6c6f 7365 2829 0a20 2020 2020  ut.close().     
-000102e0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-000102f0: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-00010300: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010310: 2e61 7373 6572 7445 7175 616c 2873 6574  .assertEqual(set
-00010320: 2866 6965 6c64 6e61 6d65 7329 2c20 7365  (fieldnames), se
-00010330: 7428 6f75 746c 696e 6573 5b30 5d2e 7370  t(outlines[0].sp
-00010340: 6c69 7428 272c 2729 2929 0a20 2020 2020  lit(','))).     
-00010350: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00010360: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-00010370: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010380: 2e61 7373 6572 7445 7175 616c 2831 2c20  .assertEqual(1, 
-00010390: 6c65 6e28 6f75 746c 696e 6573 2929 0a0a  len(outlines))..
-000103a0: 2020 2020 6465 6620 7465 7374 5f63 7376      def test_csv
-000103b0: 5f65 7870 6f72 745f 746f 5f73 7472 696e  _export_to_strin
-000103c0: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
-000103d0: 2066 726f 6d20 6974 6572 746f 6f6c 7320   from itertools 
-000103e0: 696d 706f 7274 2070 6572 6d75 7461 7469  import permutati
-000103f0: 6f6e 730a 2020 2020 2020 2020 7465 7374  ons.        test
-00010400: 5f73 697a 6520 3d20 330a 2020 2020 2020  _size = 3.      
-00010410: 2020 7431 203d 206d 616b 655f 7465 7374    t1 = make_test
-00010420: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
-00010430: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
-00010440: 7374 5f73 697a 6529 0a20 2020 2020 2020  st_size).       
-00010450: 2066 6f72 2066 6965 6c64 6e61 6d65 7320   for fieldnames 
-00010460: 696e 2070 6572 6d75 7461 7469 6f6e 7328  in permutations(
-00010470: 6c69 7374 2827 6162 6327 2929 3a0a 2020  list('abc')):.  
-00010480: 2020 2020 2020 2020 2020 6f75 745f 7374            out_st
-00010490: 7269 6e67 203d 2074 312e 6373 765f 6578  ring = t1.csv_ex
-000104a0: 706f 7274 284e 6f6e 652c 2066 6965 6c64  port(None, field
-000104b0: 6e61 6d65 7329 0a20 2020 2020 2020 2020  names).         
-000104c0: 2020 206f 7574 6c69 6e65 7320 3d20 6f75     outlines = ou
-000104d0: 745f 7374 7269 6e67 2e73 706c 6974 6c69  t_string.splitli
-000104e0: 6e65 7328 290a 2020 2020 2020 2020 2020  nes().          
-000104f0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-00010500: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-00010510: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00010520: 7274 4571 7561 6c28 272c 272e 6a6f 696e  rtEqual(','.join
-00010530: 2866 6965 6c64 6e61 6d65 7329 2c20 6f75  (fieldnames), ou
-00010540: 746c 696e 6573 5b30 5d29 0a20 2020 2020  tlines[0]).     
-00010550: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00010560: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-00010570: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010580: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
-00010590: 745f 7369 7a65 202a 2a20 3320 2b20 312c  t_size ** 3 + 1,
-000105a0: 206c 656e 286f 7574 6c69 6e65 7329 290a   len(outlines)).
-000105b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000105c0: 6f62 2c20 6c69 6e65 2069 6e20 7a69 7028  ob, line in zip(
-000105d0: 7431 2c20 6f75 746c 696e 6573 5b31 3a5d  t1, outlines[1:]
-000105e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000105f0: 2020 2063 7376 5f76 616c 7320 3d20 6c69     csv_vals = li
-00010600: 6e65 2e73 706c 6974 2827 2c27 290a 2020  ne.split(',').  
-00010610: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-00010620: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00010630: 6f62 3d6f 622c 2063 7376 5f76 616c 733d  ob=ob, csv_vals=
-00010640: 6373 765f 7661 6c73 293a 0a20 2020 2020  csv_vals):.     
-00010650: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010660: 656c 662e 6173 7365 7274 5472 7565 2861  elf.assertTrue(a
-00010670: 6c6c 280a 2020 2020 2020 2020 2020 2020  ll(.            
-00010680: 2020 2020 2020 2020 2020 2020 696e 7428              int(
-00010690: 6373 765f 7661 6c73 5b69 5d29 203d 3d20  csv_vals[i]) == 
-000106a0: 6765 7461 7474 7228 6f62 2c20 666c 6429  getattr(ob, fld)
-000106b0: 2066 6f72 2069 2c20 666c 6420 696e 2065   for i, fld in e
-000106c0: 6e75 6d65 7261 7465 2866 6965 6c64 6e61  numerate(fieldna
-000106d0: 6d65 7329 0a20 2020 2020 2020 2020 2020  mes).           
-000106e0: 2020 2020 2020 2020 2029 290a 0a20 2020           ))..   
-000106f0: 2064 6566 2074 6573 745f 6373 765f 696d   def test_csv_im
-00010700: 706f 7274 2873 656c 6629 3a0a 2020 2020  port(self):.    
-00010710: 2020 2020 6461 7461 203d 2063 7376 5f64      data = csv_d
-00010720: 6174 610a 2020 2020 2020 2020 696e 6373  ata.        incs
-00010730: 7620 3d20 696f 2e53 7472 696e 6749 4f28  v = io.StringIO(
-00010740: 6461 7461 290a 2020 2020 2020 2020 6373  data).        cs
-00010750: 7674 6162 6c65 203d 206c 742e 5461 626c  vtable = lt.Tabl
-00010760: 6528 292e 6373 765f 696d 706f 7274 2869  e().csv_import(i
-00010770: 6e63 7376 2c20 7472 616e 7366 6f72 6d73  ncsv, transforms
-00010780: 3d7b 2761 273a 2069 6e74 2c20 2762 273a  ={'a': int, 'b':
-00010790: 2069 6e74 2c20 2763 273a 2069 6e74 7d29   int, 'c': int})
-000107a0: 0a0a 2020 2020 2020 2020 7465 7374 5f73  ..        test_s
-000107b0: 697a 6520 3d20 330a 2020 2020 2020 2020  ize = 3.        
-000107c0: 7431 203d 206d 616b 655f 7465 7374 5f74  t1 = make_test_t
-000107d0: 6162 6c65 2873 656c 662e 6d61 6b65 5f64  able(self.make_d
-000107e0: 6174 615f 6f62 6a65 6374 2c20 7465 7374  ata_object, test
-000107f0: 5f73 697a 6529 0a0a 2020 2020 2020 2020  _size)..        
-00010800: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-00010810: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-00010820: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
-00010830: 2861 6c6c 286d 616b 655f 6461 7461 6f62  (all(make_dataob
-00010840: 6a65 6374 5f66 726f 6d5f 6f62 2872 6563  ject_from_ob(rec
-00010850: 3129 203d 3d20 7265 6332 2066 6f72 2072  1) == rec2 for r
-00010860: 6563 312c 2072 6563 3220 696e 207a 6970  ec1, rec2 in zip
-00010870: 2874 312c 2063 7376 7461 626c 6529 2929  (t1, csvtable)))
-00010880: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00010890: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-000108a0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000108b0: 7373 6572 7445 7175 616c 2873 756d 2831  ssertEqual(sum(1
-000108c0: 2066 6f72 206c 696e 6520 696e 2064 6174   for line in dat
-000108d0: 612e 7370 6c69 746c 696e 6573 2829 2069  a.splitlines() i
-000108e0: 6620 6c69 6e65 2e73 7472 6970 2829 292d  f line.strip())-
-000108f0: 312c 206c 656e 2863 7376 7461 626c 6529  1, len(csvtable)
-00010900: 290a 0a20 2020 2020 2020 2069 6e63 7376  )..        incsv
-00010910: 203d 2069 6f2e 5374 7269 6e67 494f 2864   = io.StringIO(d
-00010920: 6174 6129 0a20 2020 2020 2020 2072 6f77  ata).        row
-00010930: 5f70 726f 746f 7479 7065 203d 2073 656c  _prototype = sel
-00010940: 662e 6d61 6b65 5f64 6174 615f 6f62 6a65  f.make_data_obje
-00010950: 6374 2830 2c20 302c 2030 290a 2020 2020  ct(0, 0, 0).    
-00010960: 2020 2020 6373 7674 6162 6c65 3220 3d20      csvtable2 = 
-00010970: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
-00010980: 6d70 6f72 7428 696e 6373 762c 2074 7261  mport(incsv, tra
-00010990: 6e73 666f 726d 733d 7b27 6127 3a20 696e  nsforms={'a': in
-000109a0: 742c 2027 6227 3a20 696e 742c 2027 6327  t, 'b': int, 'c'
-000109b0: 3a20 696e 747d 2c20 726f 775f 636c 6173  : int}, row_clas
-000109c0: 733d 7479 7065 2872 6f77 5f70 726f 746f  s=type(row_proto
-000109d0: 7479 7065 2929 5b3a 335d 0a0a 2020 2020  type))[:3]..    
-000109e0: 2020 2020 7072 696e 7428 7479 7065 2874      print(type(t
-000109f0: 315b 305d 292e 5f5f 6e61 6d65 5f5f 2c20  1[0]).__name__, 
-00010a00: 7431 5b30 5d29 0a20 2020 2020 2020 2070  t1[0]).        p
-00010a10: 7269 6e74 2874 7970 6528 6373 7674 6162  rint(type(csvtab
-00010a20: 6c65 325b 305d 292e 5f5f 6e61 6d65 5f5f  le2[0]).__name__
-00010a30: 2c20 6373 7674 6162 6c65 325b 305d 290a  , csvtable2[0]).
-00010a40: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00010a50: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-00010a60: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00010a70: 7365 7274 4571 7561 6c28 7479 7065 2874  sertEqual(type(t
-00010a80: 315b 305d 292c 2074 7970 6528 6373 7674  1[0]), type(csvt
-00010a90: 6162 6c65 325b 305d 2929 0a0a 2020 2020  able2[0]))..    
-00010aa0: 6465 6620 7465 7374 5f63 7376 5f63 6f6d  def test_csv_com
-00010ab0: 7072 6573 7365 645f 696d 706f 7274 2873  pressed_import(s
-00010ac0: 656c 6629 3a0a 0a20 2020 2020 2020 2064  elf):..        d
-00010ad0: 6566 2076 6572 6966 795f 7469 6d65 7374  ef verify_timest
-00010ae0: 616d 7073 2874 312c 2074 322c 2069 6e66  amps(t1, t2, inf
-00010af0: 6f5f 6469 6374 293a 0a20 2020 2020 2020  o_dict):.       
-00010b00: 2020 2020 2066 6f72 2074 696d 6573 7461       for timesta
-00010b10: 6d70 5f61 7474 725f 6e61 6d65 2069 6e20  mp_attr_name in 
-00010b20: 2263 7265 6174 6564 206d 6f64 6966 6965  "created modifie
-00010b30: 6420 6c61 7374 5f69 6d70 6f72 7422 2e73  d last_import".s
-00010b40: 706c 6974 2829 3a0a 2020 2020 2020 2020  plit():.        
-00010b50: 2020 2020 2020 2020 7469 6d65 7374 616d          timestam
-00010b60: 705f 7661 6c75 6520 3d20 696e 666f 5f64  p_value = info_d
-00010b70: 6963 742e 706f 7028 7469 6d65 7374 616d  ict.pop(timestam
-00010b80: 705f 6174 7472 5f6e 616d 6529 0a20 2020  p_attr_name).   
-00010b90: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-00010ba0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-00010bb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010bc0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00010bd0: 7454 7275 6528 0a20 2020 2020 2020 2020  tTrue(.         
-00010be0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00010bf0: 3120 3c3d 2074 696d 6573 7461 6d70 5f76  1 <= timestamp_v
-00010c00: 616c 7565 203c 3d20 7432 2c0a 2020 2020  alue <= t2,.    
-00010c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c20: 2020 2020 6622 696e 636f 7272 6563 7420      f"incorrect 
-00010c30: 7b74 696d 6573 7461 6d70 5f61 7474 725f  {timestamp_attr_
-00010c40: 6e61 6d65 7d20 7469 6d65 220a 2020 2020  name} time".    
-00010c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c60: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
-00010c70: 7469 6d65 7374 616d 705f 7374 6172 745f  timestamp_start_
-00010c80: 656e 6428 2920 6173 2074 696d 696e 673a  end() as timing:
-00010c90: 0a20 2020 2020 2020 2020 2020 2074 7420  .            tt 
-00010ca0: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
-00010cb0: 5f69 6d70 6f72 7428 2274 6573 742f 6162  _import("test/ab
-00010cc0: 632e 6373 7622 2c20 7472 616e 7366 6f72  c.csv", transfor
-00010cd0: 6d73 3d64 6963 742e 6672 6f6d 6b65 7973  ms=dict.fromkeys
-00010ce0: 2822 6162 6322 2c20 696e 7429 290a 0a20  ("abc", int)).. 
-00010cf0: 2020 2020 2020 2065 7870 6563 7465 645f         expected_
-00010d00: 696e 666f 5f62 6173 6520 3d20 7474 2e69  info_base = tt.i
-00010d10: 6e66 6f28 290a 2020 2020 2020 2020 7665  nfo().        ve
-00010d20: 7269 6679 5f74 696d 6573 7461 6d70 7328  rify_timestamps(
-00010d30: 7469 6d69 6e67 2e73 7461 7274 2c20 7469  timing.start, ti
-00010d40: 6d69 6e67 2e65 6e64 2c20 6578 7065 6374  ming.end, expect
-00010d50: 6564 5f69 6e66 6f5f 6261 7365 290a 0a20  ed_info_base).. 
-00010d60: 2020 2020 2020 2070 7269 6e74 2822 6162         print("ab
-00010d70: 632e 6373 7622 2c20 6578 7065 6374 6564  c.csv", expected
-00010d80: 5f69 6e66 6f5f 6261 7365 290a 0a20 2020  _info_base)..   
-00010d90: 2020 2020 2063 6f6d 7072 6573 7365 645f       compressed_
-00010da0: 6669 6c65 7320 3d20 5b0a 2020 2020 2020  files = [.      
-00010db0: 2020 2020 2020 2261 6263 2e63 7376 2e7a        "abc.csv.z
-00010dc0: 6970 222c 0a20 2020 2020 2020 2020 2020  ip",.           
-00010dd0: 2022 6162 632e 6373 762e 677a 222c 0a20   "abc.csv.gz",. 
-00010de0: 2020 2020 2020 2020 2020 2022 6162 632e             "abc.
-00010df0: 6373 762e 787a 222c 0a20 2020 2020 2020  csv.xz",.       
-00010e00: 205d 0a20 2020 2020 2020 2066 6f72 206e   ].        for n
-00010e10: 616d 6520 696e 2063 6f6d 7072 6573 7365  ame in compresse
-00010e20: 645f 6669 6c65 733a 0a20 2020 2020 2020  d_files:.       
-00010e30: 2020 2020 2069 6d70 6f72 745f 736f 7572       import_sour
-00010e40: 6365 5f6e 616d 6520 3d20 2274 6573 742f  ce_name = "test/
-00010e50: 2220 2b20 6e61 6d65 0a20 2020 2020 2020  " + name.       
-00010e60: 2020 2020 2077 6974 6820 7469 6d65 7374       with timest
-00010e70: 616d 705f 7374 6172 745f 656e 6428 2920  amp_start_end() 
-00010e80: 6173 2074 696d 696e 673a 0a20 2020 2020  as timing:.     
-00010e90: 2020 2020 2020 2020 2020 2074 7432 203d             tt2 =
-00010ea0: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
-00010eb0: 696d 706f 7274 2869 6d70 6f72 745f 736f  import(import_so
-00010ec0: 7572 6365 5f6e 616d 652c 2074 7261 6e73  urce_name, trans
-00010ed0: 666f 726d 733d 6469 6374 2e66 726f 6d6b  forms=dict.fromk
-00010ee0: 6579 7328 2261 6263 222c 2069 6e74 2929  eys("abc", int))
-00010ef0: 0a0a 2020 2020 2020 2020 2020 2020 7474  ..            tt
-00010f00: 325f 696e 666f 203d 2074 7432 2e69 6e66  2_info = tt2.inf
-00010f10: 6f28 290a 2020 2020 2020 2020 2020 2020  o().            
-00010f20: 7072 696e 7428 6e61 6d65 2c20 7474 325f  print(name, tt2_
-00010f30: 696e 666f 290a 0a20 2020 2020 2020 2020  info)..         
-00010f40: 2020 2076 6572 6966 795f 7469 6d65 7374     verify_timest
-00010f50: 616d 7073 2874 696d 696e 672e 7374 6172  amps(timing.star
-00010f60: 742c 2074 696d 696e 672e 656e 642c 2074  t, timing.end, t
-00010f70: 7432 5f69 6e66 6f29 0a0a 2020 2020 2020  t2_info)..      
-00010f80: 2020 2020 2020 6578 7065 6374 6564 5f69        expected_i
-00010f90: 6e66 6f20 3d20 7b2a 2a65 7870 6563 7465  nfo = {**expecte
-00010fa0: 645f 696e 666f 5f62 6173 652c 2022 6e61  d_info_base, "na
-00010fb0: 6d65 223a 2069 6d70 6f72 745f 736f 7572  me": import_sour
-00010fc0: 6365 5f6e 616d 657d 0a20 2020 2020 2020  ce_name}.       
-00010fd0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-00010fe0: 7562 5465 7374 286e 616d 653d 6e61 6d65  ubTest(name=name
-00010ff0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00011000: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00011010: 7561 6c28 6578 7065 6374 6564 5f69 6e66  ual(expected_inf
-00011020: 6f2c 2074 7432 5f69 6e66 6f29 0a20 2020  o, tt2_info).   
-00011030: 2020 2020 2020 2020 2077 6974 6820 7365           with se
-00011040: 6c66 2e73 7562 5465 7374 286e 616d 653d  lf.subTest(name=
-00011050: 6e61 6d65 293a 0a20 2020 2020 2020 2020  name):.         
-00011060: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00011070: 7274 4571 7561 6c28 7375 6d28 7474 2e61  rtEqual(sum(tt.a
-00011080: 6c6c 2e61 292c 2073 756d 2874 7432 2e61  ll.a), sum(tt2.a
-00011090: 6c6c 2e61 2929 0a20 2020 2020 2020 2020  ll.a)).         
-000110a0: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-000110b0: 5465 7374 286e 616d 653d 6e61 6d65 293a  Test(name=name):
-000110c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000110d0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-000110e0: 6c28 7375 6d28 7474 2e61 6c6c 2e62 292c  l(sum(tt.all.b),
-000110f0: 2073 756d 2874 7432 2e61 6c6c 2e62 2929   sum(tt2.all.b))
-00011100: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00011110: 6820 7365 6c66 2e73 7562 5465 7374 286e  h self.subTest(n
-00011120: 616d 653d 6e61 6d65 293a 0a20 2020 2020  ame=name):.     
-00011130: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011140: 6173 7365 7274 4571 7561 6c28 7375 6d28  assertEqual(sum(
-00011150: 7474 2e61 6c6c 2e63 292c 2073 756d 2874  tt.all.c), sum(t
-00011160: 7432 2e61 6c6c 2e63 2929 0a0a 2020 2020  t2.all.c))..    
-00011170: 2020 2020 2320 7465 7374 2073 6570 6172      # test separ
-00011180: 6174 656c 792c 206e 6f20 7472 616e 7366  ately, no transf
-00011190: 6f72 6d73 2066 6f72 204a 534f 4e20 696d  orms for JSON im
-000111a0: 706f 7274 730a 2020 2020 2020 2020 696d  ports.        im
-000111b0: 706f 7274 5f73 6f75 7263 655f 6e61 6d65  port_source_name
-000111c0: 203d 2022 7465 7374 2f61 6263 2e6a 736f   = "test/abc.jso
-000111d0: 6e2e 677a 220a 2020 2020 2020 2020 7769  n.gz".        wi
-000111e0: 7468 2074 696d 6573 7461 6d70 5f73 7461  th timestamp_sta
-000111f0: 7274 5f65 6e64 2829 2061 7320 7469 6d69  rt_end() as timi
-00011200: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
-00011210: 7474 3220 3d20 6c74 2e54 6162 6c65 2829  tt2 = lt.Table()
-00011220: 2e6a 736f 6e5f 696d 706f 7274 2822 7465  .json_import("te
-00011230: 7374 2f61 6263 2e6a 736f 6e2e 677a 222c  st/abc.json.gz",
-00011240: 2073 7472 6561 6d69 6e67 3d54 7275 6529   streaming=True)
-00011250: 0a0a 2020 2020 2020 2020 7474 325f 696e  ..        tt2_in
-00011260: 666f 203d 2074 7432 2e69 6e66 6f28 290a  fo = tt2.info().
-00011270: 2020 2020 2020 2020 7072 696e 7428 2261          print("a
-00011280: 6263 2e6a 736f 6e2e 677a 222c 2074 7432  bc.json.gz", tt2
-00011290: 5f69 6e66 6f29 0a0a 2020 2020 2020 2020  _info)..        
-000112a0: 7665 7269 6679 5f74 696d 6573 7461 6d70  verify_timestamp
-000112b0: 7328 7469 6d69 6e67 2e73 7461 7274 2c20  s(timing.start, 
-000112c0: 7469 6d69 6e67 2e65 6e64 2c20 7474 325f  timing.end, tt2_
-000112d0: 696e 666f 290a 0a20 2020 2020 2020 2065  info)..        e
-000112e0: 7870 6563 7465 645f 696e 666f 203d 207b  xpected_info = {
-000112f0: 2a2a 6578 7065 6374 6564 5f69 6e66 6f5f  **expected_info_
-00011300: 6261 7365 2c20 226e 616d 6522 3a20 696d  base, "name": im
-00011310: 706f 7274 5f73 6f75 7263 655f 6e61 6d65  port_source_name
-00011320: 7d0a 2020 2020 2020 2020 7769 7468 2073  }.        with s
-00011330: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-00011340: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011350: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
-00011360: 6374 6564 5f69 6e66 6f2c 2074 7432 5f69  cted_info, tt2_i
-00011370: 6e66 6f29 0a20 2020 2020 2020 2077 6974  nfo).        wit
-00011380: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-00011390: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000113a0: 6c66 2e61 7373 6572 7445 7175 616c 2873  lf.assertEqual(s
-000113b0: 756d 2874 742e 616c 6c2e 6129 2c20 7375  um(tt.all.a), su
-000113c0: 6d28 7474 322e 616c 6c2e 6129 290a 2020  m(tt2.all.a)).  
-000113d0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-000113e0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-000113f0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00011400: 7274 4571 7561 6c28 7375 6d28 7474 2e61  rtEqual(sum(tt.a
-00011410: 6c6c 2e62 292c 2073 756d 2874 7432 2e61  ll.b), sum(tt2.a
-00011420: 6c6c 2e62 2929 0a20 2020 2020 2020 2077  ll.b)).        w
-00011430: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00011440: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00011450: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00011460: 2873 756d 2874 742e 616c 6c2e 6329 2c20  (sum(tt.all.c), 
-00011470: 7375 6d28 7474 322e 616c 6c2e 6329 290a  sum(tt2.all.c)).
-00011480: 0a20 2020 2064 6566 2074 6573 745f 6373  .    def test_cs
-00011490: 765f 696d 706f 7274 5f73 6f75 7263 655f  v_import_source_
-000114a0: 696e 666f 2873 656c 6629 3a0a 2020 2020  info(self):.    
-000114b0: 2020 2020 696d 706f 7274 7320 3d20 5b0a      imports = [.
-000114c0: 2020 2020 2020 2020 2020 2020 2822 6162              ("ab
-000114d0: 632e 6373 7622 2c20 6c74 2e49 6d70 6f72  c.csv", lt.Impor
-000114e0: 7453 6f75 7263 6554 7970 652e 6669 6c65  tSourceType.file
-000114f0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-00011500: 2261 6263 2e74 7376 222c 206c 742e 496d  "abc.tsv", lt.Im
-00011510: 706f 7274 536f 7572 6365 5479 7065 2e66  portSourceType.f
-00011520: 696c 6529 2c0a 2020 2020 2020 2020 2020  ile),.          
-00011530: 2020 2822 6162 632e 786c 7378 222c 206c    ("abc.xlsx", l
-00011540: 742e 496d 706f 7274 536f 7572 6365 5479  t.ImportSourceTy
-00011550: 7065 2e66 696c 6529 2c0a 2020 2020 2020  pe.file),.      
-00011560: 2020 2020 2020 2822 6162 632e 6373 762e        ("abc.csv.
-00011570: 7a69 7022 2c20 6c74 2e49 6d70 6f72 7453  zip", lt.ImportS
-00011580: 6f75 7263 6554 7970 652e 7a69 7029 2c0a  ourceType.zip),.
-00011590: 2020 2020 2020 2020 2020 2020 2822 6162              ("ab
-000115a0: 632e 6373 762e 677a 222c 206c 742e 496d  c.csv.gz", lt.Im
-000115b0: 706f 7274 536f 7572 6365 5479 7065 2e67  portSourceType.g
-000115c0: 7a69 7029 2c0a 2020 2020 2020 2020 2020  zip),.          
-000115d0: 2020 2822 6162 632e 6373 762e 787a 222c    ("abc.csv.xz",
-000115e0: 206c 742e 496d 706f 7274 536f 7572 6365   lt.ImportSource
-000115f0: 5479 7065 2e6c 7a6d 6129 2c0a 2020 2020  Type.lzma),.    
-00011600: 2020 2020 2020 2020 2822 612c 622c 635c          ("a,b,c\
-00011610: 6e31 2c32 2c33 222c 206c 742e 496d 706f  n1,2,3", lt.Impo
-00011620: 7274 536f 7572 6365 5479 7065 2e73 7472  rtSourceType.str
-00011630: 696e 6729 2c0a 2020 2020 2020 2020 5d0a  ing),.        ].
-00011640: 2020 2020 2020 2020 666f 7220 666e 616d          for fnam
-00011650: 652c 2065 7870 6563 7465 645f 7479 7065  e, expected_type
-00011660: 2069 6e20 696d 706f 7274 733a 0a20 2020   in imports:.   
-00011670: 2020 2020 2020 2020 2069 6620 225c 6e22           if "\n"
-00011680: 206e 6f74 2069 6e20 666e 616d 653a 0a20   not in fname:. 
-00011690: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000116a0: 6d70 6f72 745f 6e61 6d65 203d 2022 7465  mport_name = "te
-000116b0: 7374 2f22 202b 2066 6e61 6d65 0a20 2020  st/" + fname.   
-000116c0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000116d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000116e0: 6d70 6f72 745f 6e61 6d65 203d 2066 6e61  mport_name = fna
-000116f0: 6d65 0a20 2020 2020 2020 2020 2020 2069  me.            i
-00011700: 6620 696d 706f 7274 5f6e 616d 652e 656e  f import_name.en
-00011710: 6473 7769 7468 2822 2e63 7376 2229 3a0a  dswith(".csv"):.
-00011720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011730: 7462 6c20 3d20 6c74 2e54 6162 6c65 2829  tbl = lt.Table()
-00011740: 2e63 7376 5f69 6d70 6f72 7428 696d 706f  .csv_import(impo
-00011750: 7274 5f6e 616d 6529 0a20 2020 2020 2020  rt_name).       
-00011760: 2020 2020 2065 6c69 6620 696d 706f 7274       elif import
-00011770: 5f6e 616d 652e 656e 6473 7769 7468 2822  _name.endswith("
-00011780: 2e78 6c73 7822 293a 0a20 2020 2020 2020  .xlsx"):.       
-00011790: 2020 2020 2020 2020 2074 626c 203d 206c           tbl = l
-000117a0: 742e 5461 626c 6528 292e 6578 6365 6c5f  t.Table().excel_
-000117b0: 696d 706f 7274 2869 6d70 6f72 745f 6e61  import(import_na
-000117c0: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
-000117d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000117e0: 2020 2020 2020 7462 6c20 3d20 6c74 2e54        tbl = lt.T
-000117f0: 6162 6c65 2829 2e74 7376 5f69 6d70 6f72  able().tsv_impor
-00011800: 7428 696d 706f 7274 5f6e 616d 6529 0a0a  t(import_name)..
-00011810: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00011820: 7428 7265 7072 2869 6d70 6f72 745f 6e61  t(repr(import_na
-00011830: 6d65 292c 2074 626c 2e69 6d70 6f72 745f  me), tbl.import_
-00011840: 736f 7572 6365 2c20 7462 6c2e 696d 706f  source, tbl.impo
-00011850: 7274 5f73 6f75 7263 655f 7479 7065 290a  rt_source_type).
-00011860: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00011870: 225c 6e22 206e 6f74 2069 6e20 666e 616d  "\n" not in fnam
-00011880: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00011890: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-000118a0: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-000118b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000118c0: 2e61 7373 6572 7445 7175 616c 2869 6d70  .assertEqual(imp
-000118d0: 6f72 745f 6e61 6d65 2c20 7462 6c2e 696d  ort_name, tbl.im
-000118e0: 706f 7274 5f73 6f75 7263 6529 0a20 2020  port_source).   
-000118f0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00011900: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00011910: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00011920: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00011930: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00011940: 6572 7445 7175 616c 284e 6f6e 652c 2074  ertEqual(None, t
-00011950: 626c 2e69 6d70 6f72 745f 736f 7572 6365  bl.import_source
-00011960: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
-00011970: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00011980: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00011990: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000119a0: 7561 6c28 6578 7065 6374 6564 5f74 7970  ual(expected_typ
-000119b0: 652c 2074 626c 2e69 6d70 6f72 745f 736f  e, tbl.import_so
-000119c0: 7572 6365 5f74 7970 6529 0a0a 2020 2020  urce_type)..    
-000119d0: 6465 6620 7465 7374 5f63 7376 5f69 6d70  def test_csv_imp
-000119e0: 6f72 745f 6672 6f6d 5f75 726c 2873 656c  ort_from_url(sel
-000119f0: 6629 3a0a 2020 2020 2020 2020 6672 6f6d  f):.        from
-00011a00: 2068 7474 702e 7365 7276 6572 2069 6d70   http.server imp
-00011a10: 6f72 7420 4854 5450 5365 7276 6572 2c20  ort HTTPServer, 
-00011a20: 4261 7365 4854 5450 5265 7175 6573 7448  BaseHTTPRequestH
-00011a30: 616e 646c 6572 0a20 2020 2020 2020 2066  andler.        f
-00011a40: 726f 6d20 6874 7470 2069 6d70 6f72 7420  rom http import 
-00011a50: 4854 5450 5374 6174 7573 0a20 2020 2020  HTTPStatus.     
-00011a60: 2020 2069 6d70 6f72 7420 7468 7265 6164     import thread
-00011a70: 696e 670a 2020 2020 2020 2020 696d 706f  ing.        impo
-00011a80: 7274 2074 696d 650a 2020 2020 2020 2020  rt time.        
-00011a90: 696d 706f 7274 2075 726c 6c69 622e 6572  import urllib.er
-00011aa0: 726f 720a 2020 2020 2020 2020 696d 706f  ror.        impo
-00011ab0: 7274 2075 726c 6c69 622e 7265 7175 6573  rt urllib.reques
-00011ac0: 740a 0a20 2020 2020 2020 2069 6620 534b  t..        if SK
-00011ad0: 4950 5f43 5356 5f49 4d50 4f52 545f 5553  IP_CSV_IMPORT_US
-00011ae0: 494e 475f 5552 4c5f 5445 5354 533a 0a20  ING_URL_TESTS:. 
-00011af0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011b00: 736b 6970 5465 7374 2822 4353 5620 696d  skipTest("CSV im
-00011b10: 706f 7274 2074 6573 7473 2073 6b69 7070  port tests skipp
-00011b20: 6564 2229 0a0a 2020 2020 2020 2020 636c  ed")..        cl
-00011b30: 6173 7320 4353 5654 6573 7452 6571 7565  ass CSVTestReque
-00011b40: 7374 4861 6e64 6c65 7228 4261 7365 4854  stHandler(BaseHT
-00011b50: 5450 5265 7175 6573 7448 616e 646c 6572  TPRequestHandler
-00011b60: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
-00011b70: 6566 2064 6f5f 4745 5428 7365 6c66 293a  ef do_GET(self):
-00011b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011b90: 2073 656c 662e 6c6f 675f 6d65 7373 6167   self.log_messag
-00011ba0: 6528 2272 6563 6569 7665 6420 2573 2025  e("received %s %
-00011bb0: 7322 2c20 7365 6c66 2e63 6f6d 6d61 6e64  s", self.command
-00011bc0: 2c20 7365 6c66 2e70 6174 6829 0a20 2020  , self.path).   
-00011bd0: 2020 2020 2020 2020 2020 2020 2070 6174               pat
-00011be0: 6820 3d20 7365 6c66 2e70 6174 680a 2020  h = self.path.  
-00011bf0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00011c00: 2070 6174 6820 3d3d 2022 2f45 5849 5422   path == "/EXIT"
-00011c10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011c20: 2020 2020 2020 7365 6c66 2e73 656e 645f        self.send_
-00011c30: 7265 7370 6f6e 7365 2848 5454 5053 7461  response(HTTPSta
-00011c40: 7475 732e 4f4b 290a 2020 2020 2020 2020  tus.OK).        
-00011c50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011c60: 2e65 6e64 5f68 6561 6465 7273 2829 0a20  .end_headers(). 
-00011c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c80: 2020 2074 6872 6561 6469 6e67 2e54 6872     threading.Thr
-00011c90: 6561 6428 7461 7267 6574 3d6c 616d 6264  ead(target=lambd
-00011ca0: 613a 2073 656c 662e 7365 7276 6572 2e73  a: self.server.s
-00011cb0: 6875 7464 6f77 6e28 2929 2e73 7461 7274  hutdown()).start
-00011cc0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
-00011cd0: 2020 2020 656c 6966 2070 6174 6820 3d3d      elif path ==
-00011ce0: 2022 2f22 3a0a 2020 2020 2020 2020 2020   "/":.          
-00011cf0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00011d00: 656e 645f 7265 7370 6f6e 7365 2848 5454  end_response(HTT
-00011d10: 5053 7461 7475 732e 4f4b 290a 2020 2020  PStatus.OK).    
-00011d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d30: 7365 6c66 2e65 6e64 5f68 6561 6465 7273  self.end_headers
-00011d40: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
-00011d50: 2020 2020 656c 6966 2070 6174 682e 7374      elif path.st
-00011d60: 6172 7473 7769 7468 2822 2f61 6263 2e63  artswith("/abc.c
-00011d70: 7376 2229 3a0a 2020 2020 2020 2020 2020  sv"):.          
-00011d80: 2020 2020 2020 2020 2020 7365 6e64 5f62            send_b
-00011d90: 7974 6573 203d 2062 2261 2c62 2c63 5c6e  ytes = b"a,b,c\n
-00011da0: 312c 322c 335c 6e22 0a20 2020 2020 2020  1,2,3\n".       
-00011db0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00011dc0: 662e 7365 6e64 5f72 6573 706f 6e73 6528  f.send_response(
-00011dd0: 4854 5450 5374 6174 7573 2e4f 4b29 0a20  HTTPStatus.OK). 
-00011de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011df0: 2020 2073 656c 662e 656e 645f 6865 6164     self.end_head
-00011e00: 6572 7328 290a 2020 2020 2020 2020 2020  ers().          
-00011e10: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-00011e20: 6669 6c65 2e77 7269 7465 2873 656e 645f  file.write(send_
-00011e30: 6279 7465 7329 0a0a 2020 2020 2020 2020  bytes)..        
-00011e40: 6465 6620 7275 6e28 7365 7276 6572 5f63  def run(server_c
-00011e50: 6c61 7373 3d48 5454 5053 6572 7665 722c  lass=HTTPServer,
-00011e60: 2068 616e 646c 6572 5f63 6c61 7373 3d43   handler_class=C
-00011e70: 5356 5465 7374 5265 7175 6573 7448 616e  SVTestRequestHan
-00011e80: 646c 6572 293a 0a20 2020 2020 2020 2020  dler):.         
-00011e90: 2020 2073 6572 7665 725f 6164 6472 6573     server_addres
-00011ea0: 7320 3d20 2827 272c 2038 3838 3829 0a20  s = ('', 8888). 
-00011eb0: 2020 2020 2020 2020 2020 2068 7474 7064             httpd
-00011ec0: 203d 2073 6572 7665 725f 636c 6173 7328   = server_class(
-00011ed0: 7365 7276 6572 5f61 6464 7265 7373 2c20  server_address, 
-00011ee0: 6861 6e64 6c65 725f 636c 6173 7329 0a20  handler_class). 
-00011ef0: 2020 2020 2020 2020 2020 2068 7474 7064             httpd
-00011f00: 2e73 6572 7665 5f66 6f72 6576 6572 2829  .serve_forever()
-00011f10: 0a0a 2020 2020 2020 2020 6465 6620 7275  ..        def ru
-00011f20: 6e5f 6261 636b 6772 6f75 6e64 5f74 6573  n_background_tes
-00011f30: 745f 7365 7276 6572 2829 3a0a 2020 2020  t_server():.    
-00011f40: 2020 2020 2020 2020 7020 3d20 7468 7265          p = thre
-00011f50: 6164 696e 672e 5468 7265 6164 2874 6172  ading.Thread(tar
-00011f60: 6765 743d 7275 6e29 0a20 2020 2020 2020  get=run).       
-00011f70: 2020 2020 2070 2e73 7461 7274 2829 0a0a       p.start()..
-00011f80: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00011f90: 7472 6965 735f 7265 6d61 696e 696e 6720  tries_remaining 
-00011fa0: 696e 2072 6576 6572 7365 6428 7261 6e67  in reversed(rang
-00011fb0: 6528 3230 2929 3a0a 2020 2020 2020 2020  e(20)):.        
-00011fc0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00011fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fe0: 2077 6974 6820 7572 6c6c 6962 2e72 6571   with urllib.req
-00011ff0: 7565 7374 2e75 726c 6f70 656e 2822 6874  uest.urlopen("ht
-00012000: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a38  tp://localhost:8
-00012010: 3838 382f 2229 3a0a 2020 2020 2020 2020  888/"):.        
-00012020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012030: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
-00012040: 2020 2020 2020 6578 6365 7074 2075 726c        except url
-00012050: 6c69 622e 6572 726f 722e 5552 4c45 7272  lib.error.URLErr
-00012060: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-00012070: 2020 2020 2020 2020 6966 2074 7269 6573          if tries
-00012080: 5f72 656d 6169 6e69 6e67 3a0a 2020 2020  _remaining:.    
-00012090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120a0: 2020 2020 7469 6d65 2e73 6c65 6570 2830      time.sleep(0
-000120b0: 2e32 3529 0a0a 2020 2020 2020 2020 2020  .25)..          
-000120c0: 2020 7265 7475 726e 2070 0a0a 2020 2020    return p..    
-000120d0: 2020 2020 7765 625f 6164 6472 6573 7320      web_address 
-000120e0: 3d20 2268 7474 703a 2f2f 6c6f 6361 6c68  = "http://localh
-000120f0: 6f73 743a 3838 3838 220a 2020 2020 2020  ost:8888".      
-00012100: 2020 7020 3d20 7275 6e5f 6261 636b 6772    p = run_backgr
-00012110: 6f75 6e64 5f74 6573 745f 7365 7276 6572  ound_test_server
-00012120: 2829 0a0a 2020 2020 2020 2020 7572 6c20  ()..        url 
-00012130: 3d20 7765 625f 6164 6472 6573 7320 2b20  = web_address + 
-00012140: 222f 6162 632e 6373 7622 0a20 2020 2020  "/abc.csv".     
-00012150: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00012160: 2020 2020 7462 6c20 3d20 6c74 2e54 6162      tbl = lt.Tab
-00012170: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
-00012180: 7572 6c29 0a20 2020 2020 2020 2066 696e  url).        fin
-00012190: 616c 6c79 3a0a 2020 2020 2020 2020 2020  ally:.          
-000121a0: 2020 7769 7468 2075 726c 6c69 622e 7265    with urllib.re
-000121b0: 7175 6573 742e 7572 6c6f 7065 6e28 7765  quest.urlopen(we
-000121c0: 625f 6164 6472 6573 7320 2b20 222f 4558  b_address + "/EX
-000121d0: 4954 2229 3a0a 2020 2020 2020 2020 2020  IT"):.          
-000121e0: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
-000121f0: 2020 2020 2020 2070 2e6a 6f69 6e28 290a         p.join().
-00012200: 0a20 2020 2020 2020 2074 626c 2e70 7265  .        tbl.pre
-00012210: 7365 6e74 2829 0a20 2020 2020 2020 2077  sent().        w
-00012220: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00012230: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00012240: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00012250: 2875 726c 2c20 7462 6c2e 696d 706f 7274  (url, tbl.import
-00012260: 5f73 6f75 7263 6529 0a20 2020 2020 2020  _source).       
-00012270: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00012280: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00012290: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000122a0: 616c 286c 742e 496d 706f 7274 536f 7572  al(lt.ImportSour
-000122b0: 6365 5479 7065 2e75 726c 2c20 7462 6c2e  ceType.url, tbl.
-000122c0: 696d 706f 7274 5f73 6f75 7263 655f 7479  import_source_ty
-000122d0: 7065 290a 0a20 2020 2064 6566 2074 6573  pe)..    def tes
-000122e0: 745f 6373 765f 6669 6c74 6572 6564 5f69  t_csv_filtered_i
-000122f0: 6d70 6f72 7428 7365 6c66 293a 0a20 2020  mport(self):.   
-00012300: 2020 2020 2074 6573 745f 7369 7a65 203d       test_size =
-00012310: 2033 0a20 2020 2020 2020 2074 7420 3d20   3.        tt = 
-00012320: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
-00012330: 6d70 6f72 7428 2274 6573 742f 6162 632e  mport("test/abc.
-00012340: 6373 7622 2c20 7472 616e 7366 6f72 6d73  csv", transforms
-00012350: 3d64 6963 742e 6672 6f6d 6b65 7973 2822  =dict.fromkeys("
-00012360: 6162 6322 2c20 696e 7429 290a 2020 2020  abc", int)).    
-00012370: 2020 2020 7072 696e 7428 2261 6263 2e63      print("abc.c
-00012380: 7376 222c 2074 742e 696e 666f 2829 290a  sv", tt.info()).
-00012390: 0a20 2020 2020 2020 2074 7420 3d20 6c74  .        tt = lt
-000123a0: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
-000123b0: 6f72 7428 2274 6573 742f 6162 632e 6373  ort("test/abc.cs
-000123c0: 7622 2c20 7472 616e 7366 6f72 6d73 3d64  v", transforms=d
-000123d0: 6963 742e 6672 6f6d 6b65 7973 2822 6162  ict.fromkeys("ab
-000123e0: 6322 2c20 696e 7429 2c0a 2020 2020 2020  c", int),.      
-000123f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012400: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-00012410: 7465 7273 3d7b 2263 223a 206c 742e 5461  ters={"c": lt.Ta
-00012420: 626c 652e 6571 2831 297d 290a 2020 2020  ble.eq(1)}).    
-00012430: 2020 2020 7072 696e 7428 7474 2e69 6e66      print(tt.inf
-00012440: 6f28 2929 0a20 2020 2020 2020 2077 6974  o()).        wit
-00012450: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-00012460: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00012470: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
-00012480: 6573 745f 7369 7a65 202a 2074 6573 745f  est_size * test_
-00012490: 7369 7a65 2c20 6c65 6e28 7474 2929 0a0a  size, len(tt))..
-000124a0: 2020 2020 2020 2020 7474 203d 206c 742e          tt = lt.
-000124b0: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
-000124c0: 7274 2822 7465 7374 2f61 6263 2e63 7376  rt("test/abc.csv
-000124d0: 222c 2074 7261 6e73 666f 726d 733d 6469  ", transforms=di
-000124e0: 6374 2e66 726f 6d6b 6579 7328 2261 6263  ct.fromkeys("abc
-000124f0: 222c 2069 6e74 292c 0a20 2020 2020 2020  ", int),.       
-00012500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012510: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
-00012520: 6572 733d 7b22 6322 3a20 317d 290a 2020  ers={"c": 1}).  
-00012530: 2020 2020 2020 7072 696e 7428 7474 2e69        print(tt.i
-00012540: 6e66 6f28 2929 0a20 2020 2020 2020 2077  nfo()).        w
-00012550: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00012560: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00012570: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00012580: 2874 6573 745f 7369 7a65 202a 2074 6573  (test_size * tes
-00012590: 745f 7369 7a65 2c20 6c65 6e28 7474 2929  t_size, len(tt))
-000125a0: 0a0a 2020 2020 2020 2020 7474 203d 206c  ..        tt = l
-000125b0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
-000125c0: 706f 7274 2822 7465 7374 2f61 6263 2e63  port("test/abc.c
-000125d0: 7376 222c 2074 7261 6e73 666f 726d 733d  sv", transforms=
-000125e0: 6469 6374 2e66 726f 6d6b 6579 7328 2261  dict.fromkeys("a
-000125f0: 6263 222c 2069 6e74 292c 0a20 2020 2020  bc", int),.     
-00012600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012610: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00012620: 6c74 6572 733d 7b22 6322 3a20 6c61 6d62  lters={"c": lamb
-00012630: 6461 2078 3a20 3020 3c20 7820 3c20 327d  da x: 0 < x < 2}
-00012640: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-00012650: 7474 2e69 6e66 6f28 2929 0a20 2020 2020  tt.info()).     
-00012660: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-00012670: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-00012680: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00012690: 7175 616c 2874 6573 745f 7369 7a65 202a  qual(test_size *
-000126a0: 2074 6573 745f 7369 7a65 2c20 6c65 6e28   test_size, len(
-000126b0: 7474 2929 0a0a 2020 2020 2020 2020 2320  tt))..        # 
-000126c0: 7465 7374 2061 6c6c 2073 7065 6369 616c  test all special
-000126d0: 2063 6f6d 7061 7261 746f 7273 2077 6865   comparators whe
-000126e0: 6e20 7573 6564 2061 7320 6669 6c74 6572  n used as filter
-000126f0: 730a 2020 2020 2020 2020 2320 2020 2020  s.        #     
-00012700: 6973 5f6e 6f6e 6520 2d20 6174 7472 6962  is_none - attrib
-00012710: 7574 6520 7661 6c75 6520 6973 204e 6f6e  ute value is Non
-00012720: 650a 2020 2020 2020 2020 2320 2020 2020  e.        #     
-00012730: 6973 5f6e 6f74 5f6e 6f6e 6520 2d20 6174  is_not_none - at
-00012740: 7472 6962 7574 6520 7661 6c75 6520 6973  tribute value is
-00012750: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
-00012760: 2020 2320 2020 2020 6973 5f6e 756c 6c20    #     is_null 
-00012770: 2d20 6174 7472 6962 7574 6520 7661 6c75  - attribute valu
-00012780: 6520 6973 204e 6f6e 652c 2022 222c 206f  e is None, "", o
-00012790: 7220 6e6f 7420 6465 6669 6e65 640a 2020  r not defined.  
-000127a0: 2020 2020 2020 2320 2020 2020 6973 5f6e        #     is_n
-000127b0: 6f74 5f6e 756c 6c20 2d20 6174 7472 6962  ot_null - attrib
-000127c0: 7574 6520 7661 6c75 6520 6973 2064 6566  ute value is def
-000127d0: 696e 6564 2c20 616e 6420 6973 206e 6f74  ined, and is not
-000127e0: 204e 6f6e 6520 6f72 2022 220a 2020 2020   None or "".    
-000127f0: 2020 2020 2320 2020 2020 7374 6172 7473      #     starts
-00012800: 7769 7468 202d 2061 7474 7269 6275 7465  with - attribute
-00012810: 2076 616c 7565 2073 7461 7274 7320 7769   value starts wi
-00012820: 7468 2061 2067 6976 656e 2073 7472 696e  th a given strin
-00012830: 670a 2020 2020 2020 2020 2320 2020 2020  g.        #     
-00012840: 656e 6473 7769 7468 202d 2061 7474 7269  endswith - attri
-00012850: 6275 7465 2076 616c 7565 2065 6e64 7320  bute value ends 
-00012860: 7769 7468 2061 2067 6976 656e 2073 7472  with a given str
-00012870: 696e 670a 2020 2020 2020 2020 2320 2020  ing.        #   
-00012880: 2020 7265 5f6d 6174 6368 202d 2061 7474    re_match - att
-00012890: 7269 6275 7465 2076 616c 7565 206d 6174  ribute value mat
-000128a0: 6368 6573 2061 2072 6567 756c 6172 2065  ches a regular e
-000128b0: 7870 7265 7373 696f 6e0a 0a20 2020 2020  xpression..     
-000128c0: 2020 2070 7269 6e74 2829 0a20 2020 2020     print().     
-000128d0: 2020 2069 6e70 7574 5f64 6174 6120 3d20     input_data = 
-000128e0: 7465 7874 7772 6170 2e64 6564 656e 7428  textwrap.dedent(
-000128f0: 2222 225c 0a20 2020 2020 2020 206e 616d  """\.        nam
-00012900: 652c 612c 622c 630a 2020 2020 2020 2020  e,a,b,c.        
-00012910: 2241 222c 3130 302c 3130 302c 3130 300a  "A",100,100,100.
-00012920: 2020 2020 2020 2020 2242 222c 3230 302c          "B",200,
-00012930: 2c32 3030 0a20 2020 2020 2020 2022 4131  ,200.        "A1
-00012940: 222c 3130 312c 3130 312c 3130 310a 2020  ",101,101,101.  
-00012950: 2020 2020 2020 2242 3122 2c32 3031 2c2c        "B1",201,,
-00012960: 3230 310a 2020 2020 2020 2020 2243 3122  201.        "C1"
-00012970: 2c33 3031 2c2c 3330 310a 2020 2020 2020  ,301,,301.      
-00012980: 2020 2c39 392c 3939 2c39 390a 2020 2020    ,99,99,99.    
-00012990: 2020 2020 2222 2229 0a20 2020 2020 2020      """).       
-000129a0: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
-000129b0: 696d 706f 7274 2869 6e70 7574 5f64 6174  import(input_dat
-000129c0: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
-000129d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129e0: 2074 7261 6e73 666f 726d 733d 6469 6374   transforms=dict
-000129f0: 2e66 726f 6d6b 6579 7328 2261 6263 222c  .fromkeys("abc",
-00012a00: 2069 6e74 292c 0a20 2020 2020 2020 2020   int),.         
-00012a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a20: 2020 2020 2029 2e70 7265 7365 6e74 2829       ).present()
-00012a30: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00012a40: 2020 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2d        +---------
-00012a50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012a60: 2b0a 2020 2020 2020 2020 7c20 4e61 6d65  +.        | Name
-00012a70: 207c 2020 2041 207c 2020 2020 4220 7c20   |   A |    B | 
-00012a80: 2020 4320 7c0a 2020 2020 2020 2020 7c2d    C |.        |-
-00012a90: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2b 2d2d 2d2d  -----+-----+----
-00012aa0: 2d2d 2b2d 2d2d 2d2d 7c0a 2020 2020 2020  --+-----|.      
-00012ab0: 2020 7c20 4120 2020 207c 2031 3030 207c    | A    | 100 |
-00012ac0: 2020 3130 3020 7c20 3130 3020 7c0a 2020    100 | 100 |.  
-00012ad0: 2020 2020 2020 7c20 4220 2020 207c 2032        | B    | 2
-00012ae0: 3030 207c 204e 6f6e 6520 7c20 3230 3020  00 | None | 200 
-00012af0: 7c0a 2020 2020 2020 2020 7c20 4131 2020  |.        | A1  
-00012b00: 207c 2031 3031 207c 2020 3130 3120 7c20   | 101 |  101 | 
-00012b10: 3130 3120 7c0a 2020 2020 2020 2020 7c20  101 |.        | 
-00012b20: 4231 2020 207c 2032 3031 207c 204e 6f6e  B1   | 201 | Non
-00012b30: 6520 7c20 3230 3120 7c0a 2020 2020 2020  e | 201 |.      
-00012b40: 2020 7c20 4331 2020 207c 2033 3031 207c    | C1   | 301 |
-00012b50: 204e 6f6e 6520 7c20 3330 3120 7c0a 2020   None | 301 |.  
-00012b60: 2020 2020 2020 7c20 2020 2020 207c 2020        |      |  
-00012b70: 3939 207c 2020 2039 3920 7c20 2039 3920  99 |   99 |  99 
-00012b80: 7c0a 2020 2020 2020 2020 2b2d 2d2d 2d2d  |.        +-----
-00012b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012ba0: 2d2d 2d2d 2b0a 2020 2020 2020 2020 2222  ----+.        ""
-00012bb0: 220a 0a20 2020 2020 2020 2070 7269 6e74  "..        print
-00012bc0: 2822 6973 5f6e 6f6e 6528 2922 290a 2020  ("is_none()").  
-00012bd0: 2020 2020 2020 7820 3d20 6c74 2e54 6162        x = lt.Tab
-00012be0: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
-00012bf0: 696e 7075 745f 6461 7461 2c0a 2020 2020  input_data,.    
-00012c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c20: 2020 2020 2074 7261 6e73 666f 726d 733d       transforms=
-00012c30: 6469 6374 2e66 726f 6d6b 6579 7328 2261  dict.fromkeys("a
-00012c40: 6263 222c 2069 6e74 292c 0a20 2020 2020  bc", int),.     
-00012c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c70: 2020 2020 6669 6c74 6572 733d 7b22 6222      filters={"b"
-00012c80: 3a20 6c74 2e54 6162 6c65 2e69 735f 6e6f  : lt.Table.is_no
-00012c90: 6e65 2829 7d29 0a20 2020 2020 2020 2077  ne()}).        w
-00012ca0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00012cb0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00012cc0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00012cd0: 2833 2c20 6c65 6e28 7829 290a 2020 2020  (3, len(x)).    
-00012ce0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-00012cf0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-00012d00: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00012d10: 5472 7565 2861 6c6c 2862 2069 7320 4e6f  True(all(b is No
-00012d20: 6e65 2066 6f72 2062 2069 6e20 782e 616c  ne for b in x.al
-00012d30: 6c2e 6229 290a 0a20 2020 2020 2020 2070  l.b))..        p
-00012d40: 7269 6e74 2822 6973 5f6e 6f74 5f6e 6f6e  rint("is_not_non
-00012d50: 6528 2922 290a 2020 2020 2020 2020 7820  e()").        x 
-00012d60: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
-00012d70: 5f69 6d70 6f72 7428 696e 7075 745f 6461  _import(input_da
-00012d80: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
-00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012da0: 2020 2020 2020 7472 616e 7366 6f72 6d73        transforms
-00012db0: 3d64 6963 742e 6672 6f6d 6b65 7973 2822  =dict.fromkeys("
-00012dc0: 6162 6322 2c20 696e 7429 2c0a 2020 2020  abc", int),.    
-00012dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012de0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00012df0: 6c74 6572 733d 7b22 6222 3a20 6c74 2e54  lters={"b": lt.T
-00012e00: 6162 6c65 2e69 735f 6e6f 745f 6e6f 6e65  able.is_not_none
-00012e10: 2829 7d29 0a20 2020 2020 2020 2077 6974  ()}).        wit
-00012e20: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-00012e30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00012e40: 6c66 2e61 7373 6572 7445 7175 616c 2833  lf.assertEqual(3
-00012e50: 2c20 6c65 6e28 7829 290a 2020 2020 2020  , len(x)).      
-00012e60: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-00012e70: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-00012e80: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00012e90: 7561 6c28 3330 302c 2073 756d 2878 2e61  ual(300, sum(x.a
-00012ea0: 6c6c 2e62 2929 0a0a 2020 2020 2020 2020  ll.b))..        
-00012eb0: 7072 696e 7428 2262 2069 735f 6e75 6c6c  print("b is_null
-00012ec0: 2829 2229 0a20 2020 2020 2020 2078 203d  ()").        x =
-00012ed0: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
-00012ee0: 696d 706f 7274 2869 6e70 7574 5f64 6174  import(input_dat
-00012ef0: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
-00012f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f10: 2020 2020 2074 7261 6e73 666f 726d 733d       transforms=
-00012f20: 6469 6374 2e66 726f 6d6b 6579 7328 2261  dict.fromkeys("a
-00012f30: 6263 222c 2069 6e74 292c 0a20 2020 2020  bc", int),.     
-00012f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f50: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-00012f60: 7465 7273 3d7b 2262 223a 206c 742e 5461  ters={"b": lt.Ta
-00012f70: 626c 652e 6973 5f6e 756c 6c28 297d 290a  ble.is_null()}).
-00012f80: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00012f90: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-00012fa0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00012fb0: 7365 7274 4571 7561 6c28 332c 206c 656e  sertEqual(3, len
-00012fc0: 2878 2929 0a20 2020 2020 2020 2077 6974  (x)).        wit
-00012fd0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-00012fe0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00012ff0: 6c66 2e61 7373 6572 7454 7275 6528 616c  lf.assertTrue(al
-00013000: 6c28 6220 6973 204e 6f6e 6520 666f 7220  l(b is None for 
-00013010: 6220 696e 2078 2e61 6c6c 2e62 2929 0a0a  b in x.all.b))..
-00013020: 2020 2020 2020 2020 7072 696e 7428 2262          print("b
-00013030: 2069 735f 6e6f 745f 6e75 6c6c 2829 2229   is_not_null()")
-00013040: 0a20 2020 2020 2020 2078 203d 206c 742e  .        x = lt.
-00013050: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
-00013060: 7274 2869 6e70 7574 5f64 6174 612c 0a20  rt(input_data,. 
-00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013090: 2074 7261 6e73 666f 726d 733d 6469 6374   transforms=dict
-000130a0: 2e66 726f 6d6b 6579 7328 2261 6263 222c  .fromkeys("abc",
-000130b0: 2069 6e74 292c 0a20 2020 2020 2020 2020   int),.         
-000130c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130d0: 2020 2020 2020 2020 2066 696c 7465 7273           filters
-000130e0: 3d7b 2262 223a 206c 742e 5461 626c 652e  ={"b": lt.Table.
-000130f0: 6973 5f6e 6f74 5f6e 756c 6c28 297d 290a  is_not_null()}).
-00013100: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00013110: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-00013120: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00013130: 7365 7274 4571 7561 6c28 332c 206c 656e  sertEqual(3, len
-00013140: 2878 2929 0a20 2020 2020 2020 2077 6974  (x)).        wit
-00013150: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-00013160: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00013170: 6c66 2e61 7373 6572 7445 7175 616c 2833  lf.assertEqual(3
-00013180: 3030 2c20 7375 6d28 782e 616c 6c2e 6229  00, sum(x.all.b)
-00013190: 290a 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-000131a0: 2822 6e61 6d65 2069 735f 6e75 6c6c 2829  ("name is_null()
-000131b0: 2229 0a20 2020 2020 2020 2078 203d 206c  ").        x = l
-000131c0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
-000131d0: 706f 7274 2869 6e70 7574 5f64 6174 612c  port(input_data,
-000131e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eef0: 2061 2c62 2c64 6566 6175 6c74 0a20 2020   a,b,default.   
+0000ef00: 2020 2020 2020 2020 2031 302c 3130 302c           10,100,
+0000ef10: 7075 7270 6c65 0a20 2020 2020 2020 2020  purple.         
+0000ef20: 2020 2031 352c 3230 302c 6f72 616e 6765     15,200,orange
+0000ef30: 0a20 2020 2020 2020 2020 2020 2031 352c  .            15,
+0000ef40: 3135 302c 7075 7270 6c65 0a20 2020 2020  150,purple.     
+0000ef50: 2020 2020 2020 2032 302c 3235 302c 6f72         20,250,or
+0000ef60: 616e 6765 0a20 2020 2020 2020 2020 2020  ange.           
+0000ef70: 2031 352c 3235 302c 6f72 616e 6765 0a20   15,250,orange. 
+0000ef80: 2020 2020 2020 2020 2020 2022 2222 2929             """))
+0000ef90: 0a20 2020 2020 2020 2074 6162 6c65 2e73  .        table.s
+0000efa0: 6f72 7428 2264 6566 6175 6c74 2064 6573  ort("default des
+0000efb0: 632c 6122 290a 2020 2020 2020 2020 7461  c,a").        ta
+0000efc0: 626c 652e 7072 6573 656e 7428 290a 2020  ble.present().  
+0000efd0: 2020 2020 2020 7461 626c 652e 7072 6573        table.pres
+0000efe0: 656e 7428 626f 783d 626f 782e 4153 4349  ent(box=box.ASCI
+0000eff0: 492c 2067 726f 7570 6279 3d22 6465 6661  I, groupby="defa
+0000f000: 756c 7420 6122 290a 2020 2020 2020 2020  ult a").        
+0000f010: 6f75 7420 3d20 5374 7269 6e67 494f 2829  out = StringIO()
+0000f020: 0a20 2020 2020 2020 2074 6162 6c65 2e70  .        table.p
+0000f030: 7265 7365 6e74 2866 696c 653d 6f75 742c  resent(file=out,
+0000f040: 2062 6f78 3d62 6f78 2e41 5343 4949 2c20   box=box.ASCII, 
+0000f050: 6772 6f75 7062 793d 2264 6566 6175 6c74  groupby="default
+0000f060: 2061 2229 0a20 2020 2020 2020 2065 7870   a").        exp
+0000f070: 6563 7465 6420 3d20 7465 7874 7772 6170  ected = textwrap
+0000f080: 2e64 6564 656e 7428 2222 225c 0a20 2020  .dedent("""\.   
+0000f090: 2020 2020 2020 2020 202b 2d2d 2d2d 2d2d           +------
+0000f0a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a  --------------+.
+0000f0b0: 2020 2020 2020 2020 2020 2020 7c20 4120              | A 
+0000f0c0: 207c 2042 2020 207c 2044 6566 6175 6c74   | B   | Default
+0000f0d0: 207c 0a20 2020 2020 2020 2020 2020 207c   |.            |
+0000f0e0: 2d2d 2d2d 2b2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----+-----+-----
+0000f0f0: 2d2d 2d2d 7c0a 2020 2020 2020 2020 2020  ----|.          
+0000f100: 2020 7c20 3130 207c 2031 3030 207c 2070    | 10 | 100 | p
+0000f110: 7572 706c 6520 207c 0a20 2020 2020 2020  urple  |.       
+0000f120: 2020 2020 207c 2031 3520 7c20 3135 3020       | 15 | 150 
+0000f130: 7c20 2020 2020 2020 2020 7c0a 2020 2020  |         |.    
+0000f140: 2020 2020 2020 2020 7c20 3135 207c 2032          | 15 | 2
+0000f150: 3030 207c 206f 7261 6e67 6520 207c 0a20  00 | orange  |. 
+0000f160: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+0000f170: 7c20 3235 3020 7c20 2020 2020 2020 2020  | 250 |         
+0000f180: 7c0a 2020 2020 2020 2020 2020 2020 7c20  |.            | 
+0000f190: 3230 207c 2032 3530 207c 2020 2020 2020  20 | 250 |      
+0000f1a0: 2020 207c 0a20 2020 2020 2020 2020 2020     |.           
+0000f1b0: 202b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   +--------------
+0000f1c0: 2d2d 2d2d 2d2d 2b0a 2020 2020 2020 2020  ------+.        
+0000f1d0: 2020 2020 2222 2229 0a20 2020 2020 2020      """).       
+0000f1e0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+0000f1f0: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+0000f200: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000f210: 616c 2865 7870 6563 7465 642c 206f 7574  al(expected, out
+0000f220: 2e67 6574 7661 6c75 6528 2929 0a0a 2020  .getvalue())..  
+0000f230: 2020 6465 6620 7465 7374 5f6d 6172 6b64    def test_markd
+0000f240: 6f77 6e28 7365 6c66 293a 0a20 2020 2020  own(self):.     
+0000f250: 2020 2074 6162 6c65 203d 206c 742e 5461     table = lt.Ta
+0000f260: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
+0000f270: 2874 6578 7477 7261 702e 6465 6465 6e74  (textwrap.dedent
+0000f280: 2822 2222 5c0a 2020 2020 2020 2020 2020  ("""\.          
+0000f290: 2020 612c 620a 2020 2020 2020 2020 2020    a,b.          
+0000f2a0: 2020 3130 2c31 3030 0a20 2020 2020 2020    10,100.       
+0000f2b0: 2020 2020 2032 302c 3230 300a 2020 2020       20,200.    
+0000f2c0: 2020 2020 2020 2020 2222 2229 290a 2020          """)).  
+0000f2d0: 2020 2020 2020 6f75 745f 6d61 726b 646f        out_markdo
+0000f2e0: 776e 203d 2074 6162 6c65 2e61 735f 6d61  wn = table.as_ma
+0000f2f0: 726b 646f 776e 2829 0a20 2020 2020 2020  rkdown().       
+0000f300: 2070 7269 6e74 286f 7574 5f6d 6172 6b64   print(out_markd
+0000f310: 6f77 6e29 0a20 2020 2020 2020 2065 7870  own).        exp
+0000f320: 6563 7465 6420 3d20 7465 7874 7772 6170  ected = textwrap
+0000f330: 2e64 6564 656e 7428 2222 225c 0a20 2020  .dedent("""\.   
+0000f340: 2020 2020 2020 2020 207c 2061 207c 2062           | a | b
+0000f350: 207c 0a20 2020 2020 2020 2020 2020 207c   |.            |
+0000f360: 2d2d 2d7c 2d2d 2d7c 0a20 2020 2020 2020  ---|---|.       
+0000f370: 2020 2020 207c 2031 3020 7c20 3130 3020       | 10 | 100 
+0000f380: 7c0a 2020 2020 2020 2020 2020 2020 7c20  |.            | 
+0000f390: 3230 207c 2032 3030 207c 0a20 2020 2020  20 | 200 |.     
+0000f3a0: 2020 2020 2020 2022 2222 290a 2020 2020         """).    
+0000f3b0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+0000f3c0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+0000f3d0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000f3e0: 4571 7561 6c28 6578 7065 6374 6564 2c20  Equal(expected, 
+0000f3f0: 6f75 745f 6d61 726b 646f 776e 290a 0a20  out_markdown).. 
+0000f400: 2020 2020 2020 2023 2074 6573 7420 6275         # test bu
+0000f410: 6766 6978 2077 6865 6e20 7461 626c 6520  gfix when table 
+0000f420: 6861 7320 6174 7472 6962 7574 6520 2264  has attribute "d
+0000f430: 6566 6175 6c74 220a 2020 2020 2020 2020  efault".        
+0000f440: 7461 626c 6520 3d20 6c74 2e54 6162 6c65  table = lt.Table
+0000f450: 2829 2e63 7376 5f69 6d70 6f72 7428 7465  ().csv_import(te
+0000f460: 7874 7772 6170 2e64 6564 656e 7428 2222  xtwrap.dedent(""
+0000f470: 225c 0a20 2020 2020 2020 2020 2020 2061  "\.            a
+0000f480: 2c62 2c64 6566 6175 6c74 0a20 2020 2020  ,b,default.     
+0000f490: 2020 2020 2020 2031 302c 3130 302c 7075         10,100,pu
+0000f4a0: 7270 6c65 0a20 2020 2020 2020 2020 2020  rple.           
+0000f4b0: 2031 352c 3135 302c 0a20 2020 2020 2020   15,150,.       
+0000f4c0: 2020 2020 2032 302c 3230 302c 6f72 616e       20,200,oran
+0000f4d0: 6765 0a20 2020 2020 2020 2020 2020 2022  ge.            "
+0000f4e0: 2222 2929 0a20 2020 2020 2020 206f 7574  "")).        out
+0000f4f0: 5f6d 6172 6b64 6f77 6e20 3d20 7461 626c  _markdown = tabl
+0000f500: 652e 6173 5f6d 6172 6b64 6f77 6e28 290a  e.as_markdown().
+0000f510: 2020 2020 2020 2020 7072 696e 7428 6f75          print(ou
+0000f520: 745f 6d61 726b 646f 776e 290a 2020 2020  t_markdown).    
+0000f530: 2020 2020 6578 7065 6374 6564 203d 2074      expected = t
+0000f540: 6578 7477 7261 702e 6465 6465 6e74 2822  extwrap.dedent("
+0000f550: 2222 5c0a 2020 2020 2020 2020 2020 2020  ""\.            
+0000f560: 7c20 6120 7c20 6220 7c20 6465 6661 756c  | a | b | defaul
+0000f570: 7420 7c0a 2020 2020 2020 2020 2020 2020  t |.            
+0000f580: 7c2d 2d2d 7c2d 2d2d 7c2d 2d2d 7c0a 2020  |---|---|---|.  
+0000f590: 2020 2020 2020 2020 2020 7c20 3130 207c            | 10 |
+0000f5a0: 2031 3030 207c 2070 7572 706c 6520 7c0a   100 | purple |.
+0000f5b0: 2020 2020 2020 2020 2020 2020 7c20 3135              | 15
+0000f5c0: 207c 2031 3530 207c 2020 7c0a 2020 2020   | 150 |  |.    
+0000f5d0: 2020 2020 2020 2020 7c20 3230 207c 2032          | 20 | 2
+0000f5e0: 3030 207c 206f 7261 6e67 6520 7c0a 2020  00 | orange |.  
+0000f5f0: 2020 2020 2020 2020 2020 2222 2229 0a20            """). 
+0000f600: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+0000f610: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+0000f620: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000f630: 6572 7445 7175 616c 2865 7870 6563 7465  ertEqual(expecte
+0000f640: 642c 206f 7574 5f6d 6172 6b64 6f77 6e29  d, out_markdown)
+0000f650: 0a0a 2020 2020 2020 2020 2320 7465 7374  ..        # test
+0000f660: 2067 726f 7570 696e 6720 696e 2061 735f   grouping in as_
+0000f670: 6d61 726b 646f 776e 0a20 2020 2020 2020  markdown.       
+0000f680: 2074 6162 6c65 203d 206c 742e 5461 626c   table = lt.Tabl
+0000f690: 6528 292e 6373 765f 696d 706f 7274 2874  e().csv_import(t
+0000f6a0: 6578 7477 7261 702e 6465 6465 6e74 2822  extwrap.dedent("
+0000f6b0: 2222 5c0a 2020 2020 2020 2020 2020 2020  ""\.            
+0000f6c0: 612c 622c 6465 6661 756c 740a 2020 2020  a,b,default.    
+0000f6d0: 2020 2020 2020 2020 3130 2c31 3030 2c70          10,100,p
+0000f6e0: 7572 706c 650a 2020 2020 2020 2020 2020  urple.          
+0000f6f0: 2020 3135 2c31 3530 2c70 7572 706c 650a    15,150,purple.
+0000f700: 2020 2020 2020 2020 2020 2020 3230 2c32              20,2
+0000f710: 3030 2c6f 7261 6e67 650a 2020 2020 2020  00,orange.      
+0000f720: 2020 2020 2020 2222 2229 290a 2020 2020        """)).    
+0000f730: 2020 2020 6f75 745f 6d61 726b 646f 776e      out_markdown
+0000f740: 203d 2074 6162 6c65 2e61 735f 6d61 726b   = table.as_mark
+0000f750: 646f 776e 2867 726f 7570 6279 3d22 6465  down(groupby="de
+0000f760: 6661 756c 7422 290a 2020 2020 2020 2020  fault").        
+0000f770: 7072 696e 7428 6f75 745f 6d61 726b 646f  print(out_markdo
+0000f780: 776e 290a 2020 2020 2020 2020 6578 7065  wn).        expe
+0000f790: 6374 6564 203d 2074 6578 7477 7261 702e  cted = textwrap.
+0000f7a0: 6465 6465 6e74 2822 2222 5c0a 2020 2020  dedent("""\.    
+0000f7b0: 2020 2020 2020 2020 7c20 6120 7c20 6220          | a | b 
+0000f7c0: 7c20 6465 6661 756c 7420 7c0a 2020 2020  | default |.    
+0000f7d0: 2020 2020 2020 2020 7c2d 2d2d 7c2d 2d2d          |---|---
+0000f7e0: 7c2d 2d2d 7c0a 2020 2020 2020 2020 2020  |---|.          
+0000f7f0: 2020 7c20 3130 207c 2031 3030 207c 2070    | 10 | 100 | p
+0000f800: 7572 706c 6520 7c0a 2020 2020 2020 2020  urple |.        
+0000f810: 2020 2020 7c20 3135 207c 2031 3530 207c      | 15 | 150 |
+0000f820: 2020 7c0a 2020 2020 2020 2020 2020 2020    |.            
+0000f830: 7c20 3230 207c 2032 3030 207c 206f 7261  | 20 | 200 | ora
+0000f840: 6e67 6520 7c0a 2020 2020 2020 2020 2020  nge |.          
+0000f850: 2020 2222 2229 0a20 2020 2020 2020 2077    """).        w
+0000f860: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+0000f870: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000f880: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000f890: 2865 7870 6563 7465 642c 206f 7574 5f6d  (expected, out_m
+0000f8a0: 6172 6b64 6f77 6e29 0a0a 2020 2020 2020  arkdown)..      
+0000f8b0: 2020 7461 626c 6520 3d20 6c74 2e54 6162    table = lt.Tab
+0000f8c0: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
+0000f8d0: 7465 7874 7772 6170 2e64 6564 656e 7428  textwrap.dedent(
+0000f8e0: 2222 225c 0a20 2020 2020 2020 2020 2020  """\.           
+0000f8f0: 2061 2c62 2c64 6566 6175 6c74 0a20 2020   a,b,default.   
+0000f900: 2020 2020 2020 2020 2031 302c 3130 302c           10,100,
+0000f910: 7075 7270 6c65 0a20 2020 2020 2020 2020  purple.         
+0000f920: 2020 2031 352c 3230 302c 6f72 616e 6765     15,200,orange
+0000f930: 0a20 2020 2020 2020 2020 2020 2031 352c  .            15,
+0000f940: 3135 302c 7075 7270 6c65 0a20 2020 2020  150,purple.     
+0000f950: 2020 2020 2020 2032 302c 3235 302c 6f72         20,250,or
+0000f960: 616e 6765 0a20 2020 2020 2020 2020 2020  ange.           
+0000f970: 2031 352c 3235 302c 6f72 616e 6765 0a20   15,250,orange. 
+0000f980: 2020 2020 2020 2020 2020 2022 2222 2929             """))
+0000f990: 0a20 2020 2020 2020 2074 6162 6c65 2e73  .        table.s
+0000f9a0: 6f72 7428 2264 6566 6175 6c74 2064 6573  ort("default des
+0000f9b0: 632c 6122 290a 2020 2020 2020 2020 6f75  c,a").        ou
+0000f9c0: 745f 6d61 726b 646f 776e 203d 2074 6162  t_markdown = tab
+0000f9d0: 6c65 2e61 735f 6d61 726b 646f 776e 2867  le.as_markdown(g
+0000f9e0: 726f 7570 6279 3d22 6465 6661 756c 7420  roupby="default 
+0000f9f0: 6122 290a 2020 2020 2020 2020 7072 696e  a").        prin
+0000fa00: 7428 6f75 745f 6d61 726b 646f 776e 290a  t(out_markdown).
+0000fa10: 2020 2020 2020 2020 6578 7065 6374 6564          expected
+0000fa20: 203d 2074 6578 7477 7261 702e 6465 6465   = textwrap.dede
+0000fa30: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
+0000fa40: 2020 2020 7c20 6120 7c20 6220 7c20 6465      | a | b | de
+0000fa50: 6661 756c 7420 7c0a 2020 2020 2020 2020  fault |.        
+0000fa60: 2020 2020 7c2d 2d2d 7c2d 2d2d 7c2d 2d2d      |---|---|---
+0000fa70: 7c0a 2020 2020 2020 2020 2020 2020 7c20  |.            | 
+0000fa80: 3130 207c 2031 3030 207c 2070 7572 706c  10 | 100 | purpl
+0000fa90: 6520 7c0a 2020 2020 2020 2020 2020 2020  e |.            
+0000faa0: 7c20 3135 207c 2031 3530 207c 2020 7c0a  | 15 | 150 |  |.
+0000fab0: 2020 2020 2020 2020 2020 2020 7c20 3135              | 15
+0000fac0: 207c 2032 3030 207c 206f 7261 6e67 6520   | 200 | orange 
+0000fad0: 7c0a 2020 2020 2020 2020 2020 2020 7c20  |.            | 
+0000fae0: 207c 2032 3530 207c 2020 7c0a 2020 2020   | 250 |  |.    
+0000faf0: 2020 2020 2020 2020 7c20 3230 207c 2032          | 20 | 2
+0000fb00: 3530 207c 2020 7c0a 2020 2020 2020 2020  50 |  |.        
+0000fb10: 2020 2020 2222 2229 0a20 2020 2020 2020      """).       
+0000fb20: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+0000fb30: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+0000fb40: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000fb50: 616c 2865 7870 6563 7465 642c 206f 7574  al(expected, out
+0000fb60: 5f6d 6172 6b64 6f77 6e29 0a0a 2320 7361  _markdown)..# sa
+0000fb70: 6d70 6c65 2069 6d70 6f72 7420 6461 7461  mple import data
+0000fb80: 2073 6574 730a 6373 765f 6461 7461 203d   sets.csv_data =
+0000fb90: 2022 2222 5c0a 612c 622c 630a 302c 302c   """\.a,b,c.0,0,
+0000fba0: 300a 302c 302c 310a 302c 302c 320a 302c  0.0,0,1.0,0,2.0,
+0000fbb0: 312c 300a 302c 312c 310a 302c 312c 320a  1,0.0,1,1.0,1,2.
+0000fbc0: 302c 322c 300a 302c 322c 310a 302c 322c  0,2,0.0,2,1.0,2,
+0000fbd0: 320a 312c 302c 300a 312c 302c 310a 312c  2.1,0,0.1,0,1.1,
+0000fbe0: 302c 320a 312c 312c 300a 312c 312c 310a  0,2.1,1,0.1,1,1.
+0000fbf0: 312c 312c 320a 312c 322c 300a 312c 322c  1,1,2.1,2,0.1,2,
+0000fc00: 310a 312c 322c 320a 322c 302c 300a 322c  1.1,2,2.2,0,0.2,
+0000fc10: 302c 310a 322c 302c 320a 322c 312c 300a  0,1.2,0,2.2,1,0.
+0000fc20: 322c 312c 310a 322c 312c 320a 322c 322c  2,1,1.2,1,2.2,2,
+0000fc30: 300a 322c 322c 310a 322c 322c 320a 0a22  0.2,2,1.2,2,2.."
+0000fc40: 2222 0a0a 6a73 6f6e 5f64 6174 6120 3d20  ""..json_data = 
+0000fc50: 2222 225c 0a20 2020 207b 2261 223a 2030  """\.    {"a": 0
+0000fc60: 2c20 2262 223a 2030 2c20 2263 223a 2030  , "b": 0, "c": 0
+0000fc70: 7d0a 2020 2020 7b22 6122 3a20 302c 2022  }.    {"a": 0, "
+0000fc80: 6222 3a20 302c 2022 6322 3a20 317d 0a20  b": 0, "c": 1}. 
+0000fc90: 2020 207b 2261 223a 2030 2c20 2262 223a     {"a": 0, "b":
+0000fca0: 2030 2c20 2263 223a 2032 7d0a 2020 2020   0, "c": 2}.    
+0000fcb0: 7b22 6122 3a20 302c 2022 6222 3a20 312c  {"a": 0, "b": 1,
+0000fcc0: 2022 6322 3a20 307d 0a20 2020 207b 2261   "c": 0}.    {"a
+0000fcd0: 223a 2030 2c20 2262 223a 2031 2c20 2263  ": 0, "b": 1, "c
+0000fce0: 223a 2031 7d0a 2020 2020 7b22 6122 3a20  ": 1}.    {"a": 
+0000fcf0: 302c 2022 6222 3a20 312c 2022 6322 3a20  0, "b": 1, "c": 
+0000fd00: 327d 0a20 2020 207b 2261 223a 2030 2c20  2}.    {"a": 0, 
+0000fd10: 2262 223a 2032 2c20 2263 223a 2030 7d0a  "b": 2, "c": 0}.
+0000fd20: 2020 2020 7b22 6122 3a20 302c 2022 6222      {"a": 0, "b"
+0000fd30: 3a20 322c 2022 6322 3a20 317d 0a20 2020  : 2, "c": 1}.   
+0000fd40: 207b 2261 223a 2030 2c20 2262 223a 2032   {"a": 0, "b": 2
+0000fd50: 2c20 2263 223a 2032 7d0a 2020 2020 7b22  , "c": 2}.    {"
+0000fd60: 6122 3a20 312c 2022 6222 3a20 302c 2022  a": 1, "b": 0, "
+0000fd70: 6322 3a20 307d 0a20 2020 207b 2261 223a  c": 0}.    {"a":
+0000fd80: 2031 2c20 2262 223a 2030 2c20 2263 223a   1, "b": 0, "c":
+0000fd90: 2031 7d0a 2020 2020 7b22 6122 3a20 312c   1}.    {"a": 1,
+0000fda0: 2022 6222 3a20 302c 2022 6322 3a20 327d   "b": 0, "c": 2}
+0000fdb0: 0a20 2020 207b 2261 223a 2031 2c20 2262  .    {"a": 1, "b
+0000fdc0: 223a 2031 2c20 2263 223a 2030 7d0a 2020  ": 1, "c": 0}.  
+0000fdd0: 2020 7b22 6122 3a20 312c 2022 6222 3a20    {"a": 1, "b": 
+0000fde0: 312c 2022 6322 3a20 317d 0a20 2020 207b  1, "c": 1}.    {
+0000fdf0: 2261 223a 2031 2c20 2262 223a 2031 2c20  "a": 1, "b": 1, 
+0000fe00: 2263 223a 2032 7d0a 2020 2020 7b22 6122  "c": 2}.    {"a"
+0000fe10: 3a20 312c 2022 6222 3a20 322c 2022 6322  : 1, "b": 2, "c"
+0000fe20: 3a20 307d 0a20 2020 207b 2261 223a 2031  : 0}.    {"a": 1
+0000fe30: 2c20 2262 223a 2032 2c20 2263 223a 2031  , "b": 2, "c": 1
+0000fe40: 7d0a 2020 2020 7b22 6122 3a20 312c 2022  }.    {"a": 1, "
+0000fe50: 6222 3a20 322c 2022 6322 3a20 327d 0a20  b": 2, "c": 2}. 
+0000fe60: 2020 207b 2261 223a 2032 2c20 2262 223a     {"a": 2, "b":
+0000fe70: 2030 2c20 2263 223a 2030 7d0a 2020 2020   0, "c": 0}.    
+0000fe80: 7b22 6122 3a20 322c 2022 6222 3a20 302c  {"a": 2, "b": 0,
+0000fe90: 2022 6322 3a20 317d 0a20 2020 207b 2261   "c": 1}.    {"a
+0000fea0: 223a 2032 2c20 2262 223a 2030 2c20 2263  ": 2, "b": 0, "c
+0000feb0: 223a 2032 7d0a 2020 2020 7b22 6122 3a20  ": 2}.    {"a": 
+0000fec0: 322c 2022 6222 3a20 312c 2022 6322 3a20  2, "b": 1, "c": 
+0000fed0: 307d 0a20 2020 207b 2261 223a 2032 2c20  0}.    {"a": 2, 
+0000fee0: 2262 223a 2031 2c20 2263 223a 2031 7d0a  "b": 1, "c": 1}.
+0000fef0: 2020 2020 7b22 6122 3a20 322c 2022 6222      {"a": 2, "b"
+0000ff00: 3a20 312c 2022 6322 3a20 327d 0a20 2020  : 1, "c": 2}.   
+0000ff10: 207b 2261 223a 2032 2c20 2262 223a 2032   {"a": 2, "b": 2
+0000ff20: 2c20 2263 223a 2030 7d0a 2020 2020 7b22  , "c": 0}.    {"
+0000ff30: 6122 3a20 322c 2022 6222 3a20 322c 2022  a": 2, "b": 2, "
+0000ff40: 6322 3a20 317d 0a20 2020 207b 2261 223a  c": 1}.    {"a":
+0000ff50: 2032 2c20 2262 223a 2032 2c20 2263 223a   2, "b": 2, "c":
+0000ff60: 2032 7d0a 0a22 2222 0a0a 6669 7865 645f   2}.."""..fixed_
+0000ff70: 7769 6474 685f 6461 7461 203d 2022 2222  width_data = """
+0000ff80: 5c0a 3020 3020 300a 3020 3020 310a 3020  \.0 0 0.0 0 1.0 
+0000ff90: 3020 320a 3020 3120 300a 3020 3120 310a  0 2.0 1 0.0 1 1.
+0000ffa0: 3020 3120 320a 3020 3220 300a 3020 3220  0 1 2.0 2 0.0 2 
+0000ffb0: 310a 3020 3220 320a 3120 3020 300a 3120  1.0 2 2.1 0 0.1 
+0000ffc0: 3020 310a 3120 3020 320a 3120 3120 300a  0 1.1 0 2.1 1 0.
+0000ffd0: 3120 3120 310a 3120 3120 320a 3120 3220  1 1 1.1 1 2.1 2 
+0000ffe0: 300a 3120 3220 310a 3120 3220 320a 3220  0.1 2 1.1 2 2.2 
+0000fff0: 3020 300a 3220 3020 310a 3220 3020 320a  0 0.2 0 1.2 0 2.
+00010000: 3220 3120 300a 3220 3120 310a 3220 3120  2 1 0.2 1 1.2 1 
+00010010: 320a 3220 3220 300a 3220 3220 310a 3220  2.2 2 0.2 2 1.2 
+00010020: 3220 320a 0a22 2222 0a0a 0a40 6d61 6b65  2 2.."""...@make
+00010030: 5f74 6573 745f 636c 6173 7365 730a 636c  _test_classes.cl
+00010040: 6173 7320 5461 626c 6549 6d70 6f72 7445  ass TableImportE
+00010050: 7870 6f72 7454 6573 7473 3a0a 2020 2020  xportTests:.    
+00010060: 6465 6620 7465 7374 5f61 735f 6461 7461  def test_as_data
+00010070: 6672 616d 6528 7365 6c66 293a 0a20 2020  frame(self):.   
+00010080: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00010090: 2020 2020 2020 696d 706f 7274 2070 616e        import pan
+000100a0: 6461 7320 6173 2070 640a 2020 2020 2020  das as pd.      
+000100b0: 2020 6578 6365 7074 2049 6d70 6f72 7445    except ImportE
+000100c0: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
+000100d0: 2020 7072 696e 7428 2270 616e 6461 7320    print("pandas 
+000100e0: 6e6f 7420 696e 7374 616c 6c65 642c 2073  not installed, s
+000100f0: 6b69 7070 696e 6720 7465 7374 2229 0a20  kipping test"). 
+00010100: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00010110: 6e0a 0a20 2020 2020 2020 2069 6d70 6f72  n..        impor
+00010120: 7420 6a73 6f6e 0a0a 2020 2020 2020 2020  t json..        
+00010130: 7465 7374 5f73 697a 6520 3d20 330a 2020  test_size = 3.  
+00010140: 2020 2020 2020 7431 203d 206d 616b 655f        t1 = make_
+00010150: 7465 7374 5f74 6162 6c65 2873 656c 662e  test_table(self.
+00010160: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
+00010170: 2c20 7465 7374 5f73 697a 6529 0a0a 2020  , test_size)..  
+00010180: 2020 2020 2020 6466 3a20 7064 2e44 6174        df: pd.Dat
+00010190: 6146 7261 6d65 203d 2074 312e 6173 5f64  aFrame = t1.as_d
+000101a0: 6174 6166 7261 6d65 2822 2d62 2229 0a0a  ataframe("-b")..
+000101b0: 2020 2020 2020 2020 2320 6368 6563 6b20          # check 
+000101c0: 636f 6c75 6d6e 206e 616d 6573 0a20 2020  column names.   
+000101d0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000101e0: 4571 7561 6c28 5b22 6122 2c20 2263 225d  Equal(["a", "c"]
+000101f0: 2c20 6c69 7374 2864 662e 636f 6c75 6d6e  , list(df.column
+00010200: 7329 290a 0a20 2020 2020 2020 2023 2063  s))..        # c
+00010210: 6865 636b 2069 6d70 6f72 7465 6420 7661  heck imported va
+00010220: 6c75 6573 0a20 2020 2020 2020 2066 726f  lues.        fro
+00010230: 6d5f 6466 203d 2064 662e 746f 5f6a 736f  m_df = df.to_jso
+00010240: 6e28 6f72 6965 6e74 3d22 7661 6c75 6573  n(orient="values
+00010250: 2229 0a20 2020 2020 2020 2065 7870 6563  ").        expec
+00010260: 7465 6420 3d20 5b0a 2020 2020 2020 2020  ted = [.        
+00010270: 2020 2020 5b72 6563 2e61 2c20 7265 632e      [rec.a, rec.
+00010280: 635d 2066 6f72 2072 6563 2069 6e20 7431  c] for rec in t1
+00010290: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
+000102a0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000102b0: 7561 6c28 6578 7065 6374 6564 2c20 6a73  ual(expected, js
+000102c0: 6f6e 2e6c 6f61 6473 2866 726f 6d5f 6466  on.loads(from_df
+000102d0: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
+000102e0: 5f63 7376 5f65 7870 6f72 7428 7365 6c66  _csv_export(self
+000102f0: 293a 0a20 2020 2020 2020 2066 726f 6d20  ):.        from 
+00010300: 6974 6572 746f 6f6c 7320 696d 706f 7274  itertools import
+00010310: 2070 6572 6d75 7461 7469 6f6e 730a 2020   permutations.  
+00010320: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
+00010330: 3d20 330a 2020 2020 2020 2020 7431 203d  = 3.        t1 =
+00010340: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
+00010350: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
+00010360: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
+00010370: 6529 0a20 2020 2020 2020 2066 6f72 2066  e).        for f
+00010380: 6965 6c64 6e61 6d65 7320 696e 2070 6572  ieldnames in per
+00010390: 6d75 7461 7469 6f6e 7328 6c69 7374 2827  mutations(list('
+000103a0: 6162 6327 2929 3a0a 2020 2020 2020 2020  abc')):.        
+000103b0: 2020 2020 6f75 7420 3d20 696f 2e53 7472      out = io.Str
+000103c0: 696e 6749 4f28 290a 2020 2020 2020 2020  ingIO().        
+000103d0: 2020 2020 7431 2e63 7376 5f65 7870 6f72      t1.csv_expor
+000103e0: 7428 6f75 742c 2066 6965 6c64 6e61 6d65  t(out, fieldname
+000103f0: 7329 0a20 2020 2020 2020 2020 2020 206f  s).            o
+00010400: 7574 2e73 6565 6b28 3029 0a20 2020 2020  ut.seek(0).     
+00010410: 2020 2020 2020 206f 7574 6c69 6e65 7320         outlines 
+00010420: 3d20 6f75 742e 7265 6164 2829 2e73 706c  = out.read().spl
+00010430: 6974 6c69 6e65 7328 290a 2020 2020 2020  itlines().      
+00010440: 2020 2020 2020 6f75 742e 636c 6f73 6528        out.close(
+00010450: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
+00010460: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+00010470: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00010480: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00010490: 7561 6c28 272c 272e 6a6f 696e 2866 6965  ual(','.join(fie
+000104a0: 6c64 6e61 6d65 7329 2c20 6f75 746c 696e  ldnames), outlin
+000104b0: 6573 5b30 5d29 0a20 2020 2020 2020 2020  es[0]).         
+000104c0: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+000104d0: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+000104e0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000104f0: 6572 7445 7175 616c 2874 6573 745f 7369  ertEqual(test_si
+00010500: 7a65 2a2a 332b 312c 206c 656e 286f 7574  ze**3+1, len(out
+00010510: 6c69 6e65 7329 290a 2020 2020 2020 2020  lines)).        
+00010520: 2020 2020 666f 7220 6f62 2c20 6c69 6e65      for ob, line
+00010530: 2069 6e20 7a69 7028 7431 2c20 6f75 746c   in zip(t1, outl
+00010540: 696e 6573 5b31 3a5d 293a 0a20 2020 2020  ines[1:]):.     
+00010550: 2020 2020 2020 2020 2020 2063 7376 5f76             csv_v
+00010560: 616c 7320 3d20 6c69 6e65 2e73 706c 6974  als = line.split
+00010570: 2827 2c27 290a 2020 2020 2020 2020 2020  (',').          
+00010580: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00010590: 7375 6254 6573 7428 6f62 3d6f 622c 2063  subTest(ob=ob, c
+000105a0: 7376 5f76 616c 733d 6373 765f 7661 6c73  sv_vals=csv_vals
+000105b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000105c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+000105d0: 7274 5472 7565 2861 6c6c 280a 2020 2020  rtTrue(all(.    
+000105e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105f0: 2020 2020 696e 7428 6373 765f 7661 6c73      int(csv_vals
+00010600: 5b69 5d29 203d 3d20 6765 7461 7474 7228  [i]) == getattr(
+00010610: 6f62 2c20 666c 6429 2066 6f72 2069 2c20  ob, fld) for i, 
+00010620: 666c 6420 696e 2065 6e75 6d65 7261 7465  fld in enumerate
+00010630: 2866 6965 6c64 6e61 6d65 7329 0a20 2020  (fieldnames).   
+00010640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010650: 2029 290a 0a20 2020 2020 2020 2023 2072   ))..        # r
+00010660: 6572 756e 2075 7369 6e67 2061 6e20 656d  erun using an em
+00010670: 7074 7920 7461 626c 650a 2020 2020 2020  pty table.      
+00010680: 2020 7431 203d 206c 742e 5461 626c 6528    t1 = lt.Table(
+00010690: 290a 2020 2020 2020 2020 666f 7220 6669  ).        for fi
+000106a0: 656c 646e 616d 6573 2069 6e20 7065 726d  eldnames in perm
+000106b0: 7574 6174 696f 6e73 286c 6973 7428 2761  utations(list('a
+000106c0: 6263 2729 293a 0a20 2020 2020 2020 2020  bc')):.         
+000106d0: 2020 206f 7574 203d 2069 6f2e 5374 7269     out = io.Stri
+000106e0: 6e67 494f 2829 0a20 2020 2020 2020 2020  ngIO().         
+000106f0: 2020 2074 312e 6373 765f 6578 706f 7274     t1.csv_export
+00010700: 286f 7574 2c20 6669 656c 646e 616d 6573  (out, fieldnames
+00010710: 290a 2020 2020 2020 2020 2020 2020 6f75  ).            ou
+00010720: 742e 7365 656b 2830 290a 2020 2020 2020  t.seek(0).      
+00010730: 2020 2020 2020 6f75 746c 696e 6573 203d        outlines =
+00010740: 206f 7574 2e72 6561 6428 292e 7370 6c69   out.read().spli
+00010750: 746c 696e 6573 2829 0a20 2020 2020 2020  tlines().       
+00010760: 2020 2020 206f 7574 2e63 6c6f 7365 2829       out.close()
+00010770: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00010780: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00010790: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000107a0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000107b0: 616c 2827 2c27 2e6a 6f69 6e28 6669 656c  al(','.join(fiel
+000107c0: 646e 616d 6573 292c 206f 7574 6c69 6e65  dnames), outline
+000107d0: 735b 305d 290a 2020 2020 2020 2020 2020  s[0]).          
+000107e0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+000107f0: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00010800: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00010810: 7274 4571 7561 6c28 312c 206c 656e 286f  rtEqual(1, len(o
+00010820: 7574 6c69 6e65 7329 290a 0a20 2020 2020  utlines))..     
+00010830: 2020 2023 2072 6572 756e 2075 7369 6e67     # rerun using
+00010840: 2061 6e20 656d 7074 7920 7461 626c 652c   an empty table,
+00010850: 2077 6974 6820 696e 6465 7865 7320 746f   with indexes to
+00010860: 2064 6963 7461 7465 2066 6965 6c64 6e61   dictate fieldna
+00010870: 6d65 730a 2020 2020 2020 2020 666f 7220  mes.        for 
+00010880: 6669 656c 646e 616d 6573 2069 6e20 7065  fieldnames in pe
+00010890: 726d 7574 6174 696f 6e73 286c 6973 7428  rmutations(list(
+000108a0: 2761 6263 2729 293a 0a20 2020 2020 2020  'abc')):.       
+000108b0: 2020 2020 2074 3120 3d20 6c74 2e54 6162       t1 = lt.Tab
+000108c0: 6c65 2829 0a20 2020 2020 2020 2020 2020  le().           
+000108d0: 2066 6f72 2066 6c64 2069 6e20 6669 656c   for fld in fiel
+000108e0: 646e 616d 6573 3a0a 2020 2020 2020 2020  dnames:.        
+000108f0: 2020 2020 2020 2020 7431 2e63 7265 6174          t1.creat
+00010900: 655f 696e 6465 7828 666c 6429 0a20 2020  e_index(fld).   
+00010910: 2020 2020 2020 2020 206f 7574 203d 2069           out = i
+00010920: 6f2e 5374 7269 6e67 494f 2829 0a20 2020  o.StringIO().   
+00010930: 2020 2020 2020 2020 2074 312e 6373 765f           t1.csv_
+00010940: 6578 706f 7274 286f 7574 290a 2020 2020  export(out).    
+00010950: 2020 2020 2020 2020 6f75 742e 7365 656b          out.seek
+00010960: 2830 290a 2020 2020 2020 2020 2020 2020  (0).            
+00010970: 6f75 746c 696e 6573 203d 206f 7574 2e72  outlines = out.r
+00010980: 6561 6428 292e 7370 6c69 746c 696e 6573  ead().splitlines
+00010990: 2829 0a20 2020 2020 2020 2020 2020 206f  ().            o
+000109a0: 7574 2e63 6c6f 7365 2829 0a20 2020 2020  ut.close().     
+000109b0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+000109c0: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+000109d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000109e0: 2e61 7373 6572 7445 7175 616c 2873 6574  .assertEqual(set
+000109f0: 2866 6965 6c64 6e61 6d65 7329 2c20 7365  (fieldnames), se
+00010a00: 7428 6f75 746c 696e 6573 5b30 5d2e 7370  t(outlines[0].sp
+00010a10: 6c69 7428 272c 2729 2929 0a20 2020 2020  lit(','))).     
+00010a20: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00010a30: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+00010a40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010a50: 2e61 7373 6572 7445 7175 616c 2831 2c20  .assertEqual(1, 
+00010a60: 6c65 6e28 6f75 746c 696e 6573 2929 0a0a  len(outlines))..
+00010a70: 2020 2020 6465 6620 7465 7374 5f63 7376      def test_csv
+00010a80: 5f65 7870 6f72 745f 746f 5f73 7472 696e  _export_to_strin
+00010a90: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
+00010aa0: 2066 726f 6d20 6974 6572 746f 6f6c 7320   from itertools 
+00010ab0: 696d 706f 7274 2070 6572 6d75 7461 7469  import permutati
+00010ac0: 6f6e 730a 2020 2020 2020 2020 7465 7374  ons.        test
+00010ad0: 5f73 697a 6520 3d20 330a 2020 2020 2020  _size = 3.      
+00010ae0: 2020 7431 203d 206d 616b 655f 7465 7374    t1 = make_test
+00010af0: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
+00010b00: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
+00010b10: 7374 5f73 697a 6529 0a20 2020 2020 2020  st_size).       
+00010b20: 2066 6f72 2066 6965 6c64 6e61 6d65 7320   for fieldnames 
+00010b30: 696e 2070 6572 6d75 7461 7469 6f6e 7328  in permutations(
+00010b40: 6c69 7374 2827 6162 6327 2929 3a0a 2020  list('abc')):.  
+00010b50: 2020 2020 2020 2020 2020 6f75 745f 7374            out_st
+00010b60: 7269 6e67 203d 2074 312e 6373 765f 6578  ring = t1.csv_ex
+00010b70: 706f 7274 284e 6f6e 652c 2066 6965 6c64  port(None, field
+00010b80: 6e61 6d65 7329 0a20 2020 2020 2020 2020  names).         
+00010b90: 2020 206f 7574 6c69 6e65 7320 3d20 6f75     outlines = ou
+00010ba0: 745f 7374 7269 6e67 2e73 706c 6974 6c69  t_string.splitli
+00010bb0: 6e65 7328 290a 2020 2020 2020 2020 2020  nes().          
+00010bc0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00010bd0: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00010be0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00010bf0: 7274 4571 7561 6c28 272c 272e 6a6f 696e  rtEqual(','.join
+00010c00: 2866 6965 6c64 6e61 6d65 7329 2c20 6f75  (fieldnames), ou
+00010c10: 746c 696e 6573 5b30 5d29 0a20 2020 2020  tlines[0]).     
+00010c20: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00010c30: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+00010c40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010c50: 2e61 7373 6572 7445 7175 616c 2874 6573  .assertEqual(tes
+00010c60: 745f 7369 7a65 202a 2a20 3320 2b20 312c  t_size ** 3 + 1,
+00010c70: 206c 656e 286f 7574 6c69 6e65 7329 290a   len(outlines)).
+00010c80: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00010c90: 6f62 2c20 6c69 6e65 2069 6e20 7a69 7028  ob, line in zip(
+00010ca0: 7431 2c20 6f75 746c 696e 6573 5b31 3a5d  t1, outlines[1:]
+00010cb0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00010cc0: 2020 2063 7376 5f76 616c 7320 3d20 6c69     csv_vals = li
+00010cd0: 6e65 2e73 706c 6974 2827 2c27 290a 2020  ne.split(',').  
+00010ce0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+00010cf0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+00010d00: 6f62 3d6f 622c 2063 7376 5f76 616c 733d  ob=ob, csv_vals=
+00010d10: 6373 765f 7661 6c73 293a 0a20 2020 2020  csv_vals):.     
+00010d20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010d30: 656c 662e 6173 7365 7274 5472 7565 2861  elf.assertTrue(a
+00010d40: 6c6c 280a 2020 2020 2020 2020 2020 2020  ll(.            
+00010d50: 2020 2020 2020 2020 2020 2020 696e 7428              int(
+00010d60: 6373 765f 7661 6c73 5b69 5d29 203d 3d20  csv_vals[i]) == 
+00010d70: 6765 7461 7474 7228 6f62 2c20 666c 6429  getattr(ob, fld)
+00010d80: 2066 6f72 2069 2c20 666c 6420 696e 2065   for i, fld in e
+00010d90: 6e75 6d65 7261 7465 2866 6965 6c64 6e61  numerate(fieldna
+00010da0: 6d65 7329 0a20 2020 2020 2020 2020 2020  mes).           
+00010db0: 2020 2020 2020 2020 2029 290a 0a20 2020           ))..   
+00010dc0: 2064 6566 2074 6573 745f 6373 765f 696d   def test_csv_im
+00010dd0: 706f 7274 2873 656c 6629 3a0a 2020 2020  port(self):.    
+00010de0: 2020 2020 6461 7461 203d 2063 7376 5f64      data = csv_d
+00010df0: 6174 610a 2020 2020 2020 2020 696e 6373  ata.        incs
+00010e00: 7620 3d20 696f 2e53 7472 696e 6749 4f28  v = io.StringIO(
+00010e10: 6461 7461 290a 2020 2020 2020 2020 6373  data).        cs
+00010e20: 7674 6162 6c65 203d 206c 742e 5461 626c  vtable = lt.Tabl
+00010e30: 6528 292e 6373 765f 696d 706f 7274 2869  e().csv_import(i
+00010e40: 6e63 7376 2c20 7472 616e 7366 6f72 6d73  ncsv, transforms
+00010e50: 3d7b 2761 273a 2069 6e74 2c20 2762 273a  ={'a': int, 'b':
+00010e60: 2069 6e74 2c20 2763 273a 2069 6e74 7d29   int, 'c': int})
+00010e70: 0a0a 2020 2020 2020 2020 7465 7374 5f73  ..        test_s
+00010e80: 697a 6520 3d20 330a 2020 2020 2020 2020  ize = 3.        
+00010e90: 7431 203d 206d 616b 655f 7465 7374 5f74  t1 = make_test_t
+00010ea0: 6162 6c65 2873 656c 662e 6d61 6b65 5f64  able(self.make_d
+00010eb0: 6174 615f 6f62 6a65 6374 2c20 7465 7374  ata_object, test
+00010ec0: 5f73 697a 6529 0a0a 2020 2020 2020 2020  _size)..        
+00010ed0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00010ee0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+00010ef0: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+00010f00: 2861 6c6c 286d 616b 655f 6461 7461 6f62  (all(make_dataob
+00010f10: 6a65 6374 5f66 726f 6d5f 6f62 2872 6563  ject_from_ob(rec
+00010f20: 3129 203d 3d20 7265 6332 2066 6f72 2072  1) == rec2 for r
+00010f30: 6563 312c 2072 6563 3220 696e 207a 6970  ec1, rec2 in zip
+00010f40: 2874 312c 2063 7376 7461 626c 6529 2929  (t1, csvtable)))
+00010f50: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+00010f60: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+00010f70: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00010f80: 7373 6572 7445 7175 616c 2873 756d 2831  ssertEqual(sum(1
+00010f90: 2066 6f72 206c 696e 6520 696e 2064 6174   for line in dat
+00010fa0: 612e 7370 6c69 746c 696e 6573 2829 2069  a.splitlines() i
+00010fb0: 6620 6c69 6e65 2e73 7472 6970 2829 292d  f line.strip())-
+00010fc0: 312c 206c 656e 2863 7376 7461 626c 6529  1, len(csvtable)
+00010fd0: 290a 0a20 2020 2020 2020 2069 6e63 7376  )..        incsv
+00010fe0: 203d 2069 6f2e 5374 7269 6e67 494f 2864   = io.StringIO(d
+00010ff0: 6174 6129 0a20 2020 2020 2020 2072 6f77  ata).        row
+00011000: 5f70 726f 746f 7479 7065 203d 2073 656c  _prototype = sel
+00011010: 662e 6d61 6b65 5f64 6174 615f 6f62 6a65  f.make_data_obje
+00011020: 6374 2830 2c20 302c 2030 290a 2020 2020  ct(0, 0, 0).    
+00011030: 2020 2020 6373 7674 6162 6c65 3220 3d20      csvtable2 = 
+00011040: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
+00011050: 6d70 6f72 7428 696e 6373 762c 2074 7261  mport(incsv, tra
+00011060: 6e73 666f 726d 733d 7b27 6127 3a20 696e  nsforms={'a': in
+00011070: 742c 2027 6227 3a20 696e 742c 2027 6327  t, 'b': int, 'c'
+00011080: 3a20 696e 747d 2c20 726f 775f 636c 6173  : int}, row_clas
+00011090: 733d 7479 7065 2872 6f77 5f70 726f 746f  s=type(row_proto
+000110a0: 7479 7065 2929 5b3a 335d 0a0a 2020 2020  type))[:3]..    
+000110b0: 2020 2020 7072 696e 7428 7479 7065 2874      print(type(t
+000110c0: 315b 305d 292e 5f5f 6e61 6d65 5f5f 2c20  1[0]).__name__, 
+000110d0: 7431 5b30 5d29 0a20 2020 2020 2020 2070  t1[0]).        p
+000110e0: 7269 6e74 2874 7970 6528 6373 7674 6162  rint(type(csvtab
+000110f0: 6c65 325b 305d 292e 5f5f 6e61 6d65 5f5f  le2[0]).__name__
+00011100: 2c20 6373 7674 6162 6c65 325b 305d 290a  , csvtable2[0]).
+00011110: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00011120: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+00011130: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00011140: 7365 7274 4571 7561 6c28 7479 7065 2874  sertEqual(type(t
+00011150: 315b 305d 292c 2074 7970 6528 6373 7674  1[0]), type(csvt
+00011160: 6162 6c65 325b 305d 2929 0a0a 2020 2020  able2[0]))..    
+00011170: 6465 6620 7465 7374 5f63 7376 5f63 6f6d  def test_csv_com
+00011180: 7072 6573 7365 645f 696d 706f 7274 2873  pressed_import(s
+00011190: 656c 6629 3a0a 0a20 2020 2020 2020 2064  elf):..        d
+000111a0: 6566 2076 6572 6966 795f 7469 6d65 7374  ef verify_timest
+000111b0: 616d 7073 2874 312c 2074 322c 2069 6e66  amps(t1, t2, inf
+000111c0: 6f5f 6469 6374 293a 0a20 2020 2020 2020  o_dict):.       
+000111d0: 2020 2020 2066 6f72 2074 696d 6573 7461       for timesta
+000111e0: 6d70 5f61 7474 725f 6e61 6d65 2069 6e20  mp_attr_name in 
+000111f0: 2263 7265 6174 6564 206d 6f64 6966 6965  "created modifie
+00011200: 6420 6c61 7374 5f69 6d70 6f72 7422 2e73  d last_import".s
+00011210: 706c 6974 2829 3a0a 2020 2020 2020 2020  plit():.        
+00011220: 2020 2020 2020 2020 7469 6d65 7374 616d          timestam
+00011230: 705f 7661 6c75 6520 3d20 696e 666f 5f64  p_value = info_d
+00011240: 6963 742e 706f 7028 7469 6d65 7374 616d  ict.pop(timestam
+00011250: 705f 6174 7472 5f6e 616d 6529 0a20 2020  p_attr_name).   
+00011260: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+00011270: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00011280: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011290: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000112a0: 7454 7275 6528 0a20 2020 2020 2020 2020  tTrue(.         
+000112b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000112c0: 3120 3c3d 2074 696d 6573 7461 6d70 5f76  1 <= timestamp_v
+000112d0: 616c 7565 203c 3d20 7432 2c0a 2020 2020  alue <= t2,.    
+000112e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112f0: 2020 2020 6622 696e 636f 7272 6563 7420      f"incorrect 
+00011300: 7b74 696d 6573 7461 6d70 5f61 7474 725f  {timestamp_attr_
+00011310: 6e61 6d65 7d20 7469 6d65 220a 2020 2020  name} time".    
+00011320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011330: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+00011340: 7469 6d65 7374 616d 705f 7374 6172 745f  timestamp_start_
+00011350: 656e 6428 2920 6173 2074 696d 696e 673a  end() as timing:
+00011360: 0a20 2020 2020 2020 2020 2020 2074 7420  .            tt 
+00011370: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
+00011380: 5f69 6d70 6f72 7428 2274 6573 742f 6162  _import("test/ab
+00011390: 632e 6373 7622 2c20 7472 616e 7366 6f72  c.csv", transfor
+000113a0: 6d73 3d64 6963 742e 6672 6f6d 6b65 7973  ms=dict.fromkeys
+000113b0: 2822 6162 6322 2c20 696e 7429 290a 0a20  ("abc", int)).. 
+000113c0: 2020 2020 2020 2065 7870 6563 7465 645f         expected_
+000113d0: 696e 666f 5f62 6173 6520 3d20 7474 2e69  info_base = tt.i
+000113e0: 6e66 6f28 290a 2020 2020 2020 2020 7665  nfo().        ve
+000113f0: 7269 6679 5f74 696d 6573 7461 6d70 7328  rify_timestamps(
+00011400: 7469 6d69 6e67 2e73 7461 7274 2c20 7469  timing.start, ti
+00011410: 6d69 6e67 2e65 6e64 2c20 6578 7065 6374  ming.end, expect
+00011420: 6564 5f69 6e66 6f5f 6261 7365 290a 0a20  ed_info_base).. 
+00011430: 2020 2020 2020 2070 7269 6e74 2822 6162         print("ab
+00011440: 632e 6373 7622 2c20 6578 7065 6374 6564  c.csv", expected
+00011450: 5f69 6e66 6f5f 6261 7365 290a 0a20 2020  _info_base)..   
+00011460: 2020 2020 2063 6f6d 7072 6573 7365 645f       compressed_
+00011470: 6669 6c65 7320 3d20 5b0a 2020 2020 2020  files = [.      
+00011480: 2020 2020 2020 2261 6263 2e63 7376 2e7a        "abc.csv.z
+00011490: 6970 222c 0a20 2020 2020 2020 2020 2020  ip",.           
+000114a0: 2022 6162 632e 6373 762e 677a 222c 0a20   "abc.csv.gz",. 
+000114b0: 2020 2020 2020 2020 2020 2022 6162 632e             "abc.
+000114c0: 6373 762e 787a 222c 0a20 2020 2020 2020  csv.xz",.       
+000114d0: 205d 0a20 2020 2020 2020 2066 6f72 206e   ].        for n
+000114e0: 616d 6520 696e 2063 6f6d 7072 6573 7365  ame in compresse
+000114f0: 645f 6669 6c65 733a 0a20 2020 2020 2020  d_files:.       
+00011500: 2020 2020 2069 6d70 6f72 745f 736f 7572       import_sour
+00011510: 6365 5f6e 616d 6520 3d20 2274 6573 742f  ce_name = "test/
+00011520: 2220 2b20 6e61 6d65 0a20 2020 2020 2020  " + name.       
+00011530: 2020 2020 2077 6974 6820 7469 6d65 7374       with timest
+00011540: 616d 705f 7374 6172 745f 656e 6428 2920  amp_start_end() 
+00011550: 6173 2074 696d 696e 673a 0a20 2020 2020  as timing:.     
+00011560: 2020 2020 2020 2020 2020 2074 7432 203d             tt2 =
+00011570: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
+00011580: 696d 706f 7274 2869 6d70 6f72 745f 736f  import(import_so
+00011590: 7572 6365 5f6e 616d 652c 2074 7261 6e73  urce_name, trans
+000115a0: 666f 726d 733d 6469 6374 2e66 726f 6d6b  forms=dict.fromk
+000115b0: 6579 7328 2261 6263 222c 2069 6e74 2929  eys("abc", int))
+000115c0: 0a0a 2020 2020 2020 2020 2020 2020 7474  ..            tt
+000115d0: 325f 696e 666f 203d 2074 7432 2e69 6e66  2_info = tt2.inf
+000115e0: 6f28 290a 2020 2020 2020 2020 2020 2020  o().            
+000115f0: 7072 696e 7428 6e61 6d65 2c20 7474 325f  print(name, tt2_
+00011600: 696e 666f 290a 0a20 2020 2020 2020 2020  info)..         
+00011610: 2020 2076 6572 6966 795f 7469 6d65 7374     verify_timest
+00011620: 616d 7073 2874 696d 696e 672e 7374 6172  amps(timing.star
+00011630: 742c 2074 696d 696e 672e 656e 642c 2074  t, timing.end, t
+00011640: 7432 5f69 6e66 6f29 0a0a 2020 2020 2020  t2_info)..      
+00011650: 2020 2020 2020 6578 7065 6374 6564 5f69        expected_i
+00011660: 6e66 6f20 3d20 7b2a 2a65 7870 6563 7465  nfo = {**expecte
+00011670: 645f 696e 666f 5f62 6173 652c 2022 6e61  d_info_base, "na
+00011680: 6d65 223a 2069 6d70 6f72 745f 736f 7572  me": import_sour
+00011690: 6365 5f6e 616d 657d 0a20 2020 2020 2020  ce_name}.       
+000116a0: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+000116b0: 7562 5465 7374 286e 616d 653d 6e61 6d65  ubTest(name=name
+000116c0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000116d0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000116e0: 7561 6c28 6578 7065 6374 6564 5f69 6e66  ual(expected_inf
+000116f0: 6f2c 2074 7432 5f69 6e66 6f29 0a20 2020  o, tt2_info).   
+00011700: 2020 2020 2020 2020 2077 6974 6820 7365           with se
+00011710: 6c66 2e73 7562 5465 7374 286e 616d 653d  lf.subTest(name=
+00011720: 6e61 6d65 293a 0a20 2020 2020 2020 2020  name):.         
+00011730: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00011740: 7274 4571 7561 6c28 7375 6d28 7474 2e61  rtEqual(sum(tt.a
+00011750: 6c6c 2e61 292c 2073 756d 2874 7432 2e61  ll.a), sum(tt2.a
+00011760: 6c6c 2e61 2929 0a20 2020 2020 2020 2020  ll.a)).         
+00011770: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+00011780: 5465 7374 286e 616d 653d 6e61 6d65 293a  Test(name=name):
+00011790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000117a0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000117b0: 6c28 7375 6d28 7474 2e61 6c6c 2e62 292c  l(sum(tt.all.b),
+000117c0: 2073 756d 2874 7432 2e61 6c6c 2e62 2929   sum(tt2.all.b))
+000117d0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+000117e0: 6820 7365 6c66 2e73 7562 5465 7374 286e  h self.subTest(n
+000117f0: 616d 653d 6e61 6d65 293a 0a20 2020 2020  ame=name):.     
+00011800: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011810: 6173 7365 7274 4571 7561 6c28 7375 6d28  assertEqual(sum(
+00011820: 7474 2e61 6c6c 2e63 292c 2073 756d 2874  tt.all.c), sum(t
+00011830: 7432 2e61 6c6c 2e63 2929 0a0a 2020 2020  t2.all.c))..    
+00011840: 2020 2020 2320 7465 7374 2073 6570 6172      # test separ
+00011850: 6174 656c 792c 206e 6f20 7472 616e 7366  ately, no transf
+00011860: 6f72 6d73 2066 6f72 204a 534f 4e20 696d  orms for JSON im
+00011870: 706f 7274 730a 2020 2020 2020 2020 696d  ports.        im
+00011880: 706f 7274 5f73 6f75 7263 655f 6e61 6d65  port_source_name
+00011890: 203d 2022 7465 7374 2f61 6263 2e6a 736f   = "test/abc.jso
+000118a0: 6e2e 677a 220a 2020 2020 2020 2020 7769  n.gz".        wi
+000118b0: 7468 2074 696d 6573 7461 6d70 5f73 7461  th timestamp_sta
+000118c0: 7274 5f65 6e64 2829 2061 7320 7469 6d69  rt_end() as timi
+000118d0: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
+000118e0: 7474 3220 3d20 6c74 2e54 6162 6c65 2829  tt2 = lt.Table()
+000118f0: 2e6a 736f 6e5f 696d 706f 7274 2822 7465  .json_import("te
+00011900: 7374 2f61 6263 2e6a 736f 6e2e 677a 222c  st/abc.json.gz",
+00011910: 2073 7472 6561 6d69 6e67 3d54 7275 6529   streaming=True)
+00011920: 0a0a 2020 2020 2020 2020 7474 325f 696e  ..        tt2_in
+00011930: 666f 203d 2074 7432 2e69 6e66 6f28 290a  fo = tt2.info().
+00011940: 2020 2020 2020 2020 7072 696e 7428 2261          print("a
+00011950: 6263 2e6a 736f 6e2e 677a 222c 2074 7432  bc.json.gz", tt2
+00011960: 5f69 6e66 6f29 0a0a 2020 2020 2020 2020  _info)..        
+00011970: 7665 7269 6679 5f74 696d 6573 7461 6d70  verify_timestamp
+00011980: 7328 7469 6d69 6e67 2e73 7461 7274 2c20  s(timing.start, 
+00011990: 7469 6d69 6e67 2e65 6e64 2c20 7474 325f  timing.end, tt2_
+000119a0: 696e 666f 290a 0a20 2020 2020 2020 2065  info)..        e
+000119b0: 7870 6563 7465 645f 696e 666f 203d 207b  xpected_info = {
+000119c0: 2a2a 6578 7065 6374 6564 5f69 6e66 6f5f  **expected_info_
+000119d0: 6261 7365 2c20 226e 616d 6522 3a20 696d  base, "name": im
+000119e0: 706f 7274 5f73 6f75 7263 655f 6e61 6d65  port_source_name
+000119f0: 7d0a 2020 2020 2020 2020 7769 7468 2073  }.        with s
+00011a00: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+00011a10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011a20: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
+00011a30: 6374 6564 5f69 6e66 6f2c 2074 7432 5f69  cted_info, tt2_i
+00011a40: 6e66 6f29 0a20 2020 2020 2020 2077 6974  nfo).        wit
+00011a50: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00011a60: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00011a70: 6c66 2e61 7373 6572 7445 7175 616c 2873  lf.assertEqual(s
+00011a80: 756d 2874 742e 616c 6c2e 6129 2c20 7375  um(tt.all.a), su
+00011a90: 6d28 7474 322e 616c 6c2e 6129 290a 2020  m(tt2.all.a)).  
+00011aa0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00011ab0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+00011ac0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00011ad0: 7274 4571 7561 6c28 7375 6d28 7474 2e61  rtEqual(sum(tt.a
+00011ae0: 6c6c 2e62 292c 2073 756d 2874 7432 2e61  ll.b), sum(tt2.a
+00011af0: 6c6c 2e62 2929 0a20 2020 2020 2020 2077  ll.b)).        w
+00011b00: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00011b10: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00011b20: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00011b30: 2873 756d 2874 742e 616c 6c2e 6329 2c20  (sum(tt.all.c), 
+00011b40: 7375 6d28 7474 322e 616c 6c2e 6329 290a  sum(tt2.all.c)).
+00011b50: 0a20 2020 2064 6566 2074 6573 745f 6373  .    def test_cs
+00011b60: 765f 696d 706f 7274 5f73 6f75 7263 655f  v_import_source_
+00011b70: 696e 666f 2873 656c 6629 3a0a 2020 2020  info(self):.    
+00011b80: 2020 2020 696d 706f 7274 7320 3d20 5b0a      imports = [.
+00011b90: 2020 2020 2020 2020 2020 2020 2822 6162              ("ab
+00011ba0: 632e 6373 7622 2c20 6c74 2e49 6d70 6f72  c.csv", lt.Impor
+00011bb0: 7453 6f75 7263 6554 7970 652e 6669 6c65  tSourceType.file
+00011bc0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00011bd0: 2261 6263 2e74 7376 222c 206c 742e 496d  "abc.tsv", lt.Im
+00011be0: 706f 7274 536f 7572 6365 5479 7065 2e66  portSourceType.f
+00011bf0: 696c 6529 2c0a 2020 2020 2020 2020 2020  ile),.          
+00011c00: 2020 2822 6162 632e 786c 7378 222c 206c    ("abc.xlsx", l
+00011c10: 742e 496d 706f 7274 536f 7572 6365 5479  t.ImportSourceTy
+00011c20: 7065 2e66 696c 6529 2c0a 2020 2020 2020  pe.file),.      
+00011c30: 2020 2020 2020 2822 6162 632e 6373 762e        ("abc.csv.
+00011c40: 7a69 7022 2c20 6c74 2e49 6d70 6f72 7453  zip", lt.ImportS
+00011c50: 6f75 7263 6554 7970 652e 7a69 7029 2c0a  ourceType.zip),.
+00011c60: 2020 2020 2020 2020 2020 2020 2822 6162              ("ab
+00011c70: 632e 6373 762e 677a 222c 206c 742e 496d  c.csv.gz", lt.Im
+00011c80: 706f 7274 536f 7572 6365 5479 7065 2e67  portSourceType.g
+00011c90: 7a69 7029 2c0a 2020 2020 2020 2020 2020  zip),.          
+00011ca0: 2020 2822 6162 632e 6373 762e 787a 222c    ("abc.csv.xz",
+00011cb0: 206c 742e 496d 706f 7274 536f 7572 6365   lt.ImportSource
+00011cc0: 5479 7065 2e6c 7a6d 6129 2c0a 2020 2020  Type.lzma),.    
+00011cd0: 2020 2020 2020 2020 2822 612c 622c 635c          ("a,b,c\
+00011ce0: 6e31 2c32 2c33 222c 206c 742e 496d 706f  n1,2,3", lt.Impo
+00011cf0: 7274 536f 7572 6365 5479 7065 2e73 7472  rtSourceType.str
+00011d00: 696e 6729 2c0a 2020 2020 2020 2020 5d0a  ing),.        ].
+00011d10: 2020 2020 2020 2020 666f 7220 666e 616d          for fnam
+00011d20: 652c 2065 7870 6563 7465 645f 7479 7065  e, expected_type
+00011d30: 2069 6e20 696d 706f 7274 733a 0a20 2020   in imports:.   
+00011d40: 2020 2020 2020 2020 2069 6620 225c 6e22           if "\n"
+00011d50: 206e 6f74 2069 6e20 666e 616d 653a 0a20   not in fname:. 
+00011d60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00011d70: 6d70 6f72 745f 6e61 6d65 203d 2022 7465  mport_name = "te
+00011d80: 7374 2f22 202b 2066 6e61 6d65 0a20 2020  st/" + fname.   
+00011d90: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00011da0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00011db0: 6d70 6f72 745f 6e61 6d65 203d 2066 6e61  mport_name = fna
+00011dc0: 6d65 0a20 2020 2020 2020 2020 2020 2069  me.            i
+00011dd0: 6620 696d 706f 7274 5f6e 616d 652e 656e  f import_name.en
+00011de0: 6473 7769 7468 2822 2e63 7376 2229 3a0a  dswith(".csv"):.
+00011df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e00: 7462 6c20 3d20 6c74 2e54 6162 6c65 2829  tbl = lt.Table()
+00011e10: 2e63 7376 5f69 6d70 6f72 7428 696d 706f  .csv_import(impo
+00011e20: 7274 5f6e 616d 6529 0a20 2020 2020 2020  rt_name).       
+00011e30: 2020 2020 2065 6c69 6620 696d 706f 7274       elif import
+00011e40: 5f6e 616d 652e 656e 6473 7769 7468 2822  _name.endswith("
+00011e50: 2e78 6c73 7822 293a 0a20 2020 2020 2020  .xlsx"):.       
+00011e60: 2020 2020 2020 2020 2074 626c 203d 206c           tbl = l
+00011e70: 742e 5461 626c 6528 292e 6578 6365 6c5f  t.Table().excel_
+00011e80: 696d 706f 7274 2869 6d70 6f72 745f 6e61  import(import_na
+00011e90: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
+00011ea0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00011eb0: 2020 2020 2020 7462 6c20 3d20 6c74 2e54        tbl = lt.T
+00011ec0: 6162 6c65 2829 2e74 7376 5f69 6d70 6f72  able().tsv_impor
+00011ed0: 7428 696d 706f 7274 5f6e 616d 6529 0a0a  t(import_name)..
+00011ee0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00011ef0: 7428 7265 7072 2869 6d70 6f72 745f 6e61  t(repr(import_na
+00011f00: 6d65 292c 2074 626c 2e69 6d70 6f72 745f  me), tbl.import_
+00011f10: 736f 7572 6365 2c20 7462 6c2e 696d 706f  source, tbl.impo
+00011f20: 7274 5f73 6f75 7263 655f 7479 7065 290a  rt_source_type).
+00011f30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00011f40: 225c 6e22 206e 6f74 2069 6e20 666e 616d  "\n" not in fnam
+00011f50: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00011f60: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+00011f70: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+00011f80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00011f90: 2e61 7373 6572 7445 7175 616c 2869 6d70  .assertEqual(imp
+00011fa0: 6f72 745f 6e61 6d65 2c20 7462 6c2e 696d  ort_name, tbl.im
+00011fb0: 706f 7274 5f73 6f75 7263 6529 0a20 2020  port_source).   
+00011fc0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00011fd0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00011fe0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00011ff0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00012000: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00012010: 6572 7445 7175 616c 284e 6f6e 652c 2074  ertEqual(None, t
+00012020: 626c 2e69 6d70 6f72 745f 736f 7572 6365  bl.import_source
+00012030: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
+00012040: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+00012050: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00012060: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00012070: 7561 6c28 6578 7065 6374 6564 5f74 7970  ual(expected_typ
+00012080: 652c 2074 626c 2e69 6d70 6f72 745f 736f  e, tbl.import_so
+00012090: 7572 6365 5f74 7970 6529 0a0a 2020 2020  urce_type)..    
+000120a0: 6465 6620 7465 7374 5f63 7376 5f69 6d70  def test_csv_imp
+000120b0: 6f72 745f 6672 6f6d 5f75 726c 2873 656c  ort_from_url(sel
+000120c0: 6629 3a0a 2020 2020 2020 2020 6672 6f6d  f):.        from
+000120d0: 2068 7474 702e 7365 7276 6572 2069 6d70   http.server imp
+000120e0: 6f72 7420 4854 5450 5365 7276 6572 2c20  ort HTTPServer, 
+000120f0: 4261 7365 4854 5450 5265 7175 6573 7448  BaseHTTPRequestH
+00012100: 616e 646c 6572 0a20 2020 2020 2020 2066  andler.        f
+00012110: 726f 6d20 6874 7470 2069 6d70 6f72 7420  rom http import 
+00012120: 4854 5450 5374 6174 7573 0a20 2020 2020  HTTPStatus.     
+00012130: 2020 2069 6d70 6f72 7420 7468 7265 6164     import thread
+00012140: 696e 670a 2020 2020 2020 2020 696d 706f  ing.        impo
+00012150: 7274 2074 696d 650a 2020 2020 2020 2020  rt time.        
+00012160: 696d 706f 7274 2075 726c 6c69 622e 6572  import urllib.er
+00012170: 726f 720a 2020 2020 2020 2020 696d 706f  ror.        impo
+00012180: 7274 2075 726c 6c69 622e 7265 7175 6573  rt urllib.reques
+00012190: 740a 0a20 2020 2020 2020 2069 6620 534b  t..        if SK
+000121a0: 4950 5f43 5356 5f49 4d50 4f52 545f 5553  IP_CSV_IMPORT_US
+000121b0: 494e 475f 5552 4c5f 5445 5354 533a 0a20  ING_URL_TESTS:. 
+000121c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000121d0: 736b 6970 5465 7374 2822 4353 5620 696d  skipTest("CSV im
+000121e0: 706f 7274 2074 6573 7473 2073 6b69 7070  port tests skipp
+000121f0: 6564 2229 0a0a 2020 2020 2020 2020 636c  ed")..        cl
+00012200: 6173 7320 4353 5654 6573 7452 6571 7565  ass CSVTestReque
+00012210: 7374 4861 6e64 6c65 7228 4261 7365 4854  stHandler(BaseHT
+00012220: 5450 5265 7175 6573 7448 616e 646c 6572  TPRequestHandler
+00012230: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
+00012240: 6566 2064 6f5f 4745 5428 7365 6c66 293a  ef do_GET(self):
+00012250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012260: 2073 656c 662e 6c6f 675f 6d65 7373 6167   self.log_messag
+00012270: 6528 6622 7265 6365 6976 6564 207b 7365  e(f"received {se
+00012280: 6c66 2e63 6f6d 6d61 6e64 7d20 7b73 656c  lf.command} {sel
+00012290: 662e 7061 7468 7d22 290a 2020 2020 2020  f.path}").      
+000122a0: 2020 2020 2020 2020 2020 7061 7468 203d            path =
+000122b0: 2073 656c 662e 7061 7468 0a20 2020 2020   self.path.     
+000122c0: 2020 2020 2020 2020 2020 2073 656e 645f             send_
+000122d0: 6279 7465 7320 3d20 6222 220a 2020 2020  bytes = b"".    
+000122e0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+000122f0: 6174 6820 3d3d 2022 2f45 5849 5422 3a0a  ath == "/EXIT":.
+00012300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012310: 2020 2020 7365 6c66 2e73 656e 645f 7265      self.send_re
+00012320: 7370 6f6e 7365 2848 5454 5053 7461 7475  sponse(HTTPStatu
+00012330: 732e 4f4b 290a 2020 2020 2020 2020 2020  s.OK).          
+00012340: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
+00012350: 6e64 5f68 6561 6465 7273 2829 0a20 2020  nd_headers().   
+00012360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012370: 2073 656c 662e 7766 696c 652e 7772 6974   self.wfile.writ
+00012380: 6528 7365 6e64 5f62 7974 6573 290a 2020  e(send_bytes).  
+00012390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123a0: 2020 7468 7265 6164 696e 672e 5468 7265    threading.Thre
+000123b0: 6164 2874 6172 6765 743d 6c61 6d62 6461  ad(target=lambda
+000123c0: 3a20 7469 6d65 2e73 6c65 6570 2831 2920  : time.sleep(1) 
+000123d0: 6f72 2073 656c 662e 7365 7276 6572 2e73  or self.server.s
+000123e0: 6875 7464 6f77 6e28 2929 2e73 7461 7274  hutdown()).start
+000123f0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+00012400: 2020 2020 656c 6966 2070 6174 6820 3d3d      elif path ==
+00012410: 2022 2f22 3a0a 2020 2020 2020 2020 2020   "/":.          
+00012420: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00012430: 656e 645f 7265 7370 6f6e 7365 2848 5454  end_response(HTT
+00012440: 5053 7461 7475 732e 4f4b 290a 2020 2020  PStatus.OK).    
+00012450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012460: 7365 6c66 2e65 6e64 5f68 6561 6465 7273  self.end_headers
+00012470: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00012480: 2020 2020 2020 2073 656c 662e 7766 696c         self.wfil
+00012490: 652e 7772 6974 6528 7365 6e64 5f62 7974  e.write(send_byt
+000124a0: 6573 290a 0a20 2020 2020 2020 2020 2020  es)..           
+000124b0: 2020 2020 2065 6c69 6620 7061 7468 2e73       elif path.s
+000124c0: 7461 7274 7377 6974 6828 222f 6162 632e  tartswith("/abc.
+000124d0: 6373 7622 293a 0a20 2020 2020 2020 2020  csv"):.         
+000124e0: 2020 2020 2020 2020 2020 2073 656e 645f             send_
+000124f0: 6279 7465 7320 2b3d 2062 2261 2c62 2c63  bytes += b"a,b,c
+00012500: 5c6e 312c 322c 335c 6e22 0a20 2020 2020  \n1,2,3\n".     
+00012510: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012520: 656c 662e 7365 6e64 5f72 6573 706f 6e73  elf.send_respons
+00012530: 6528 4854 5450 5374 6174 7573 2e4f 4b29  e(HTTPStatus.OK)
+00012540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012550: 2020 2020 2073 656c 662e 7365 6e64 5f68       self.send_h
+00012560: 6561 6465 7228 2243 6f6e 7465 6e74 2d4c  eader("Content-L
+00012570: 656e 6774 6822 2c20 7374 7228 6c65 6e28  ength", str(len(
+00012580: 7365 6e64 5f62 7974 6573 2929 290a 2020  send_bytes))).  
+00012590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125a0: 2020 7365 6c66 2e65 6e64 5f68 6561 6465    self.end_heade
+000125b0: 7273 2829 0a20 2020 2020 2020 2020 2020  rs().           
+000125c0: 2020 2020 2020 2020 2073 656c 662e 7766           self.wf
+000125d0: 696c 652e 7772 6974 6528 7365 6e64 5f62  ile.write(send_b
+000125e0: 7974 6573 290a 0a20 2020 2020 2020 2020  ytes)..         
+000125f0: 2020 2064 6566 2064 6f5f 504f 5354 2873     def do_POST(s
+00012600: 656c 6629 3a0a 2020 2020 2020 2020 2020  elf):.          
+00012610: 2020 2020 2020 7365 6c66 2e6c 6f67 5f6d        self.log_m
+00012620: 6573 7361 6765 2866 2272 6563 6569 7665  essage(f"receive
+00012630: 6420 7b73 656c 662e 636f 6d6d 616e 647d  d {self.command}
+00012640: 207b 7365 6c66 2e70 6174 687d 2229 0a20   {self.path}"). 
+00012650: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00012660: 6174 6820 3d20 7365 6c66 2e70 6174 680a  ath = self.path.
+00012670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012680: 6164 6465 645f 7661 6c75 6520 3d20 7365  added_value = se
+00012690: 6c66 2e68 6561 6465 7273 5b22 5661 6c75  lf.headers["Valu
+000126a0: 6522 5d0a 2020 2020 2020 2020 2020 2020  e"].            
+000126b0: 2020 2020 7365 6c66 2e6c 6f67 5f6d 6573      self.log_mes
+000126c0: 7361 6765 2866 2272 6563 6569 7665 6420  sage(f"received 
+000126d0: 6865 6164 6572 2027 5661 6c75 6527 207b  header 'Value' {
+000126e0: 6164 6465 645f 7661 6c75 6521 727d 2229  added_value!r}")
+000126f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012700: 2073 656c 662e 6c6f 675f 6d65 7373 6167   self.log_messag
+00012710: 6528 2261 626f 7574 2074 6f20 7265 6164  e("about to read
+00012720: 2066 726f 6d20 7266 696c 6522 290a 2020   from rfile").  
+00012730: 2020 2020 2020 2020 2020 2020 2020 6164                ad
+00012740: 6465 645f 636f 6c75 6d6e 203d 2073 656c  ded_column = sel
+00012750: 662e 7266 696c 652e 7265 6164 2869 6e74  f.rfile.read(int
+00012760: 2873 656c 662e 6865 6164 6572 732e 6765  (self.headers.ge
+00012770: 7428 2743 6f6e 7465 6e74 2d4c 656e 6774  t('Content-Lengt
+00012780: 6827 2c20 2731 2729 2929 0a20 2020 2020  h', '1'))).     
+00012790: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+000127a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127b0: 2020 2020 6164 6465 645f 636f 6c75 6d6e      added_column
+000127c0: 5f73 7472 203d 2061 6464 6564 5f63 6f6c  _str = added_col
+000127d0: 756d 6e2e 6465 636f 6465 2829 0a20 2020  umn.decode().   
+000127e0: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+000127f0: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00012800: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
+00012810: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
+00012820: 5f6d 6573 7361 6765 2866 2245 7272 6f72  _message(f"Error
+00012830: 2064 6563 6f64 696e 6720 6164 6465 6420   decoding added 
+00012840: 636f 6c75 6d6e 3a20 7b74 7970 6528 6529  column: {type(e)
+00012850: 2e5f 5f6e 616d 655f 5f7d 3a20 7b65 7d22  .__name__}: {e}"
+00012860: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012870: 2020 2020 2020 6164 6465 645f 636f 6c75        added_colu
+00012880: 6d6e 5f73 7472 203d 2022 6572 726f 7222  mn_str = "error"
+00012890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000128a0: 2073 656c 662e 6c6f 675f 6d65 7373 6167   self.log_messag
+000128b0: 6528 2272 6561 6420 6672 6f6d 2072 6669  e("read from rfi
+000128c0: 6c65 2063 6f6d 706c 6574 6522 290a 2020  le complete").  
+000128d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000128e0: 6c66 2e6c 6f67 5f6d 6573 7361 6765 2866  lf.log_message(f
+000128f0: 2272 6563 6569 7665 6420 626f 6479 207b  "received body {
+00012900: 6164 6465 645f 636f 6c75 6d6e 2172 7d22  added_column!r}"
+00012910: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+00012920: 2020 2073 656e 645f 6279 7465 7320 3d20     send_bytes = 
+00012930: 6222 220a 2020 2020 2020 2020 2020 2020  b"".            
+00012940: 2020 2020 6966 2070 6174 682e 7374 6172      if path.star
+00012950: 7473 7769 7468 2822 2f61 6263 2e63 7376  tswith("/abc.csv
+00012960: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00012970: 2020 2020 2020 2020 7365 6e64 5f62 7974          send_byt
+00012980: 6573 202b 3d20 6622 612c 622c 632c 7b61  es += f"a,b,c,{a
+00012990: 6464 6564 5f63 6f6c 756d 6e5f 7374 727d  dded_column_str}
+000129a0: 5c6e 312c 322c 332c 7b61 6464 6564 5f76  \n1,2,3,{added_v
+000129b0: 616c 7565 7d5c 6e22 2e65 6e63 6f64 6528  alue}\n".encode(
+000129c0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+000129d0: 2020 2073 656c 662e 7365 6e64 5f72 6573     self.send_res
+000129e0: 706f 6e73 6528 4854 5450 5374 6174 7573  ponse(HTTPStatus
+000129f0: 2e4f 4b29 0a20 2020 2020 2020 2020 2020  .OK).           
+00012a00: 2020 2020 2073 656c 662e 7365 6e64 5f68       self.send_h
+00012a10: 6561 6465 7228 2243 6f6e 7465 6e74 2d4c  eader("Content-L
+00012a20: 656e 6774 6822 2c20 7374 7228 6c65 6e28  ength", str(len(
+00012a30: 7365 6e64 5f62 7974 6573 2929 290a 2020  send_bytes))).  
+00012a40: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012a50: 6c66 2e65 6e64 5f68 6561 6465 7273 2829  lf.end_headers()
+00012a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012a70: 2073 656c 662e 7766 696c 652e 7772 6974   self.wfile.writ
+00012a80: 6528 7365 6e64 5f62 7974 6573 290a 0a20  e(send_bytes).. 
+00012a90: 2020 2020 2020 2064 6566 2072 756e 2873         def run(s
+00012aa0: 6572 7665 725f 636c 6173 733d 4854 5450  erver_class=HTTP
+00012ab0: 5365 7276 6572 2c20 6861 6e64 6c65 725f  Server, handler_
+00012ac0: 636c 6173 733d 4353 5654 6573 7452 6571  class=CSVTestReq
+00012ad0: 7565 7374 4861 6e64 6c65 7229 3a0a 2020  uestHandler):.  
+00012ae0: 2020 2020 2020 2020 2020 7365 7276 6572            server
+00012af0: 5f61 6464 7265 7373 203d 2028 2727 2c20  _address = ('', 
+00012b00: 3838 3838 290a 2020 2020 2020 2020 2020  8888).          
+00012b10: 2020 6874 7470 6420 3d20 7365 7276 6572    httpd = server
+00012b20: 5f63 6c61 7373 2873 6572 7665 725f 6164  _class(server_ad
+00012b30: 6472 6573 732c 2068 616e 646c 6572 5f63  dress, handler_c
+00012b40: 6c61 7373 290a 2020 2020 2020 2020 2020  lass).          
+00012b50: 2020 6874 7470 642e 7365 7276 655f 666f    httpd.serve_fo
+00012b60: 7265 7665 7228 290a 0a20 2020 2020 2020  rever()..       
+00012b70: 2064 6566 2072 756e 5f62 6163 6b67 726f   def run_backgro
+00012b80: 756e 645f 7465 7374 5f73 6572 7665 7228  und_test_server(
+00012b90: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
+00012ba0: 203d 2074 6872 6561 6469 6e67 2e54 6872   = threading.Thr
+00012bb0: 6561 6428 7461 7267 6574 3d72 756e 290a  ead(target=run).
+00012bc0: 2020 2020 2020 2020 2020 2020 702e 7374              p.st
+00012bd0: 6172 7428 290a 0a20 2020 2020 2020 2020  art()..         
+00012be0: 2020 2066 6f72 2074 7269 6573 5f72 656d     for tries_rem
+00012bf0: 6169 6e69 6e67 2069 6e20 7265 7665 7273  aining in revers
+00012c00: 6564 2872 616e 6765 2832 3029 293a 0a20  ed(range(20)):. 
+00012c10: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00012c20: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00012c30: 2020 2020 2020 2020 7769 7468 2075 726c          with url
+00012c40: 6c69 622e 7265 7175 6573 742e 7572 6c6f  lib.request.urlo
+00012c50: 7065 6e28 2268 7474 703a 2f2f 6c6f 6361  pen("http://loca
+00012c60: 6c68 6f73 743a 3838 3838 2f22 293a 0a20  lhost:8888/"):. 
+00012c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c80: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+00012c90: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+00012ca0: 6570 7420 7572 6c6c 6962 2e65 7272 6f72  ept urllib.error
+00012cb0: 2e55 524c 4572 726f 723a 0a20 2020 2020  .URLError:.     
+00012cc0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00012cd0: 6620 7472 6965 735f 7265 6d61 696e 696e  f tries_remainin
+00012ce0: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
+00012cf0: 2020 2020 2020 2020 2020 2074 696d 652e             time.
+00012d00: 736c 6565 7028 302e 3235 290a 0a20 2020  sleep(0.25)..   
+00012d10: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00012d20: 700a 0a20 2020 2020 2020 2077 6562 5f61  p..        web_a
+00012d30: 6464 7265 7373 203d 2022 6874 7470 3a2f  ddress = "http:/
+00012d40: 2f6c 6f63 616c 686f 7374 3a38 3838 3822  /localhost:8888"
+00012d50: 0a20 2020 2020 2020 2070 203d 2072 756e  .        p = run
+00012d60: 5f62 6163 6b67 726f 756e 645f 7465 7374  _background_test
+00012d70: 5f73 6572 7665 7228 290a 0a20 2020 2020  _server()..     
+00012d80: 2020 2075 726c 203d 2077 6562 5f61 6464     url = web_add
+00012d90: 7265 7373 202b 2022 2f61 6263 2e63 7376  ress + "/abc.csv
+00012da0: 220a 2020 2020 2020 2020 7472 793a 0a20  ".        try:. 
+00012db0: 2020 2020 2020 2020 2020 2074 626c 203d             tbl =
+00012dc0: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
+00012dd0: 696d 706f 7274 2875 726c 290a 2020 2020  import(url).    
+00012de0: 2020 2020 2020 2020 7462 6c32 203d 206c          tbl2 = l
+00012df0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
+00012e00: 706f 7274 280a 2020 2020 2020 2020 2020  port(.          
+00012e10: 2020 2020 2020 7572 6c2c 0a20 2020 2020        url,.     
+00012e20: 2020 2020 2020 2020 2020 2064 6174 613d             data=
+00012e30: 6222 6578 7472 6122 2c0a 2020 2020 2020  b"extra",.      
+00012e40: 2020 2020 2020 2020 2020 6865 6164 6572            header
+00012e50: 733d 7b22 5641 4c55 4522 3a20 2231 3030  s={"VALUE": "100
+00012e60: 227d 2c0a 2020 2020 2020 2020 2020 2020  "},.            
+00012e70: 2020 2020 7472 616e 7366 6f72 6d73 3d7b      transforms={
+00012e80: 7d2e 6672 6f6d 6b65 7973 2822 6120 6220  }.fromkeys("a b 
+00012e90: 6320 6578 7472 6122 2e73 706c 6974 2829  c extra".split()
+00012ea0: 2c20 696e 7429 2c0a 2020 2020 2020 2020  , int),.        
+00012eb0: 2020 2020 290a 2020 2020 2020 2020 6669      ).        fi
+00012ec0: 6e61 6c6c 793a 0a20 2020 2020 2020 2020  nally:.         
+00012ed0: 2020 2077 6974 6820 7572 6c6c 6962 2e72     with urllib.r
+00012ee0: 6571 7565 7374 2e75 726c 6f70 656e 2877  equest.urlopen(w
+00012ef0: 6562 5f61 6464 7265 7373 202b 2022 2f45  eb_address + "/E
+00012f00: 5849 5422 293a 0a20 2020 2020 2020 2020  XIT"):.         
+00012f10: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
+00012f20: 2020 2020 2020 2020 702e 6a6f 696e 2829          p.join()
+00012f30: 0a0a 2020 2020 2020 2020 7462 6c2e 7072  ..        tbl.pr
+00012f40: 6573 656e 7428 290a 2020 2020 2020 2020  esent().        
+00012f50: 7462 6c32 2e70 7265 7365 6e74 2829 0a0a  tbl2.present()..
+00012f60: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00012f70: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+00012f80: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00012f90: 7365 7274 4571 7561 6c28 7572 6c2c 2074  sertEqual(url, t
+00012fa0: 626c 2e69 6d70 6f72 745f 736f 7572 6365  bl.import_source
+00012fb0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+00012fc0: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+00012fd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012fe0: 6173 7365 7274 4571 7561 6c28 6c74 2e49  assertEqual(lt.I
+00012ff0: 6d70 6f72 7453 6f75 7263 6554 7970 652e  mportSourceType.
+00013000: 7572 6c2c 2074 626c 2e69 6d70 6f72 745f  url, tbl.import_
+00013010: 736f 7572 6365 5f74 7970 6529 0a0a 2020  source_type)..  
+00013020: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00013030: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+00013040: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00013050: 7274 4571 7561 6c28 2261 2062 2063 2065  rtEqual("a b c e
+00013060: 7874 7261 222e 7370 6c69 7428 292c 2074  xtra".split(), t
+00013070: 626c 322e 696e 666f 2829 5b22 6669 656c  bl2.info()["fiel
+00013080: 6473 225d 290a 2020 2020 2020 2020 7769  ds"]).        wi
+00013090: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+000130a0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+000130b0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000130c0: 3130 302c 2074 626c 325b 305d 2e65 7874  100, tbl2[0].ext
+000130d0: 7261 290a 0a20 2020 2064 6566 2074 6573  ra)..    def tes
+000130e0: 745f 6373 765f 6669 6c74 6572 6564 5f69  t_csv_filtered_i
+000130f0: 6d70 6f72 7428 7365 6c66 293a 0a20 2020  mport(self):.   
+00013100: 2020 2020 2074 6573 745f 7369 7a65 203d       test_size =
+00013110: 2033 0a20 2020 2020 2020 2074 7420 3d20   3.        tt = 
+00013120: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
+00013130: 6d70 6f72 7428 2274 6573 742f 6162 632e  mport("test/abc.
+00013140: 6373 7622 2c20 7472 616e 7366 6f72 6d73  csv", transforms
+00013150: 3d64 6963 742e 6672 6f6d 6b65 7973 2822  =dict.fromkeys("
+00013160: 6162 6322 2c20 696e 7429 290a 2020 2020  abc", int)).    
+00013170: 2020 2020 7072 696e 7428 2261 6263 2e63      print("abc.c
+00013180: 7376 222c 2074 742e 696e 666f 2829 290a  sv", tt.info()).
+00013190: 0a20 2020 2020 2020 2074 7420 3d20 6c74  .        tt = lt
+000131a0: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
+000131b0: 6f72 7428 2274 6573 742f 6162 632e 6373  ort("test/abc.cs
+000131c0: 7622 2c20 7472 616e 7366 6f72 6d73 3d64  v", transforms=d
+000131d0: 6963 742e 6672 6f6d 6b65 7973 2822 6162  ict.fromkeys("ab
+000131e0: 6322 2c20 696e 7429 2c0a 2020 2020 2020  c", int),.      
 000131f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013200: 2020 2074 7261 6e73 666f 726d 733d 6469     transforms=di
-00013210: 6374 2e66 726f 6d6b 6579 7328 2261 6263  ct.fromkeys("abc
-00013220: 222c 2069 6e74 292c 0a20 2020 2020 2020  ", int),.       
-00013230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013240: 2020 2020 2020 2020 2020 2066 696c 7465             filte
-00013250: 7273 3d7b 226e 616d 6522 3a20 6c74 2e54  rs={"name": lt.T
-00013260: 6162 6c65 2e69 735f 6e75 6c6c 2829 7d29  able.is_null()})
-00013270: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00013280: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-00013290: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000132a0: 7373 6572 7445 7175 616c 2831 2c20 6c65  ssertEqual(1, le
-000132b0: 6e28 7829 290a 2020 2020 2020 2020 7769  n(x)).        wi
-000132c0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-000132d0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-000132e0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000132f0: 332a 3939 2c20 785b 305d 2e61 202b 2078  3*99, x[0].a + x
-00013300: 5b30 5d2e 6220 2b20 785b 305d 2e63 290a  [0].b + x[0].c).
-00013310: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-00013320: 6e61 6d65 2069 735f 6e6f 745f 6e75 6c6c  name is_not_null
-00013330: 2829 2229 0a20 2020 2020 2020 2078 203d  ()").        x =
-00013340: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
-00013350: 696d 706f 7274 2869 6e70 7574 5f64 6174  import(input_dat
-00013360: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
-00013370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013380: 2020 2020 2074 7261 6e73 666f 726d 733d       transforms=
-00013390: 6469 6374 2e66 726f 6d6b 6579 7328 2261  dict.fromkeys("a
-000133a0: 6263 222c 2069 6e74 292c 0a20 2020 2020  bc", int),.     
-000133b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133c0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-000133d0: 7465 7273 3d7b 226e 616d 6522 3a20 6c74  ters={"name": lt
-000133e0: 2e54 6162 6c65 2e69 735f 6e6f 745f 6e75  .Table.is_not_nu
-000133f0: 6c6c 2829 7d29 0a20 2020 2020 2020 2077  ll()}).        w
-00013400: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00013410: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00013420: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00013430: 2835 2c20 6c65 6e28 7829 290a 2020 2020  (5, len(x)).    
-00013440: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-00013450: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-00013460: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00013470: 4571 7561 6c28 2241 2042 2041 3120 4231  Equal("A B A1 B1
-00013480: 2043 3122 2e73 706c 6974 2829 2c20 6c69   C1".split(), li
-00013490: 7374 2878 2e61 6c6c 2e6e 616d 6529 290a  st(x.all.name)).
-000134a0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-000134b0: 6e61 6d65 2073 7461 7274 7377 6974 6828  name startswith(
-000134c0: 2742 2729 2229 0a20 2020 2020 2020 2078  'B')").        x
-000134d0: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
-000134e0: 765f 696d 706f 7274 2869 6e70 7574 5f64  v_import(input_d
-000134f0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-00013500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013510: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
-00013520: 733d 6469 6374 2e66 726f 6d6b 6579 7328  s=dict.fromkeys(
-00013530: 2261 6263 222c 2069 6e74 292c 0a20 2020  "abc", int),.   
-00013540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013550: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00013560: 696c 7465 7273 3d7b 226e 616d 6522 3a20  ilters={"name": 
-00013570: 6c74 2e54 6162 6c65 2e73 7461 7274 7377  lt.Table.startsw
-00013580: 6974 6828 2242 2229 7d29 0a20 2020 2020  ith("B")}).     
-00013590: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-000135a0: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-000135b0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-000135c0: 7175 616c 2832 2c20 6c65 6e28 7829 290a  qual(2, len(x)).
-000135d0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-000135e0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-000135f0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00013600: 7365 7274 4571 7561 6c28 2242 2042 3122  sertEqual("B B1"
-00013610: 2e73 706c 6974 2829 2c20 6c69 7374 2878  .split(), list(x
-00013620: 2e61 6c6c 2e6e 616d 6529 290a 0a20 2020  .all.name))..   
-00013630: 2020 2020 2070 7269 6e74 2822 6e61 6d65       print("name
-00013640: 2065 6e64 7377 6974 6828 2731 2729 2229   endswith('1')")
-00013650: 0a20 2020 2020 2020 2078 203d 206c 742e  .        x = lt.
-00013660: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
-00013670: 7274 2869 6e70 7574 5f64 6174 612c 0a20  rt(input_data,. 
-00013680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136a0: 2074 7261 6e73 666f 726d 733d 6469 6374   transforms=dict
-000136b0: 2e66 726f 6d6b 6579 7328 2261 6263 222c  .fromkeys("abc",
-000136c0: 2069 6e74 292c 0a20 2020 2020 2020 2020   int),.         
-000136d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136e0: 2020 2020 2020 2020 2066 696c 7465 7273           filters
-000136f0: 3d7b 226e 616d 6522 3a20 6c74 2e54 6162  ={"name": lt.Tab
-00013700: 6c65 2e65 6e64 7377 6974 6828 2231 2229  le.endswith("1")
-00013710: 7d29 0a20 2020 2020 2020 2077 6974 6820  }).        with 
-00013720: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
-00013730: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013740: 2e61 7373 6572 7445 7175 616c 2833 2c20  .assertEqual(3, 
-00013750: 6c65 6e28 7829 290a 2020 2020 2020 2020  len(x)).        
-00013760: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-00013770: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-00013780: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00013790: 6c28 2241 3120 4231 2043 3122 2e73 706c  l("A1 B1 C1".spl
-000137a0: 6974 2829 2c20 6c69 7374 2878 2e61 6c6c  it(), list(x.all
-000137b0: 2e6e 616d 6529 290a 0a20 2020 2020 2020  .name))..       
-000137c0: 2070 7269 6e74 2872 226e 616d 6520 7265   print(r"name re
-000137d0: 5f6d 6174 6368 2872 275b 4142 5d5c 6427  _match(r'[AB]\d'
-000137e0: 2922 290a 2020 2020 2020 2020 7820 3d20  )").        x = 
-000137f0: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
-00013800: 6d70 6f72 7428 696e 7075 745f 6461 7461  mport(input_data
-00013810: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00013820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013830: 2020 2020 7472 616e 7366 6f72 6d73 3d64      transforms=d
-00013840: 6963 742e 6672 6f6d 6b65 7973 2822 6162  ict.fromkeys("ab
-00013850: 6322 2c20 696e 7429 2c0a 2020 2020 2020  c", int),.      
-00013860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013870: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
-00013880: 6572 733d 7b22 6e61 6d65 223a 206c 742e  ers={"name": lt.
-00013890: 5461 626c 652e 7265 5f6d 6174 6368 2872  Table.re_match(r
-000138a0: 225b 4142 5d5c 6422 297d 290a 2020 2020  "[AB]\d")}).    
-000138b0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
-000138c0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
-000138d0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000138e0: 4571 7561 6c28 322c 206c 656e 2878 2929  Equal(2, len(x))
-000138f0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00013900: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-00013910: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00013920: 7373 6572 7445 7175 616c 2822 4131 2042  ssertEqual("A1 B
-00013930: 3122 2e73 706c 6974 2829 2c20 6c69 7374  1".split(), list
-00013940: 2878 2e61 6c6c 2e6e 616d 6529 290a 0a20  (x.all.name)).. 
-00013950: 2020 2064 6566 2074 6573 745f 6373 765f     def test_csv_
-00013960: 7374 7269 6e67 5f69 6d70 6f72 7428 7365  string_import(se
-00013970: 6c66 293a 0a20 2020 2020 2020 2064 6174  lf):.        dat
-00013980: 6120 3d20 6373 765f 6461 7461 0a20 2020  a = csv_data.   
-00013990: 2020 2020 2063 7376 7461 626c 6520 3d20       csvtable = 
-000139a0: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
-000139b0: 6d70 6f72 7428 6373 765f 736f 7572 6365  mport(csv_source
-000139c0: 3d64 6174 612c 2074 7261 6e73 666f 726d  =data, transform
-000139d0: 733d 7b27 6127 3a20 696e 742c 2027 6227  s={'a': int, 'b'
-000139e0: 3a20 696e 742c 2027 6327 3a20 696e 747d  : int, 'c': int}
-000139f0: 290a 0a20 2020 2020 2020 2074 6573 745f  )..        test_
-00013a00: 7369 7a65 203d 2033 0a20 2020 2020 2020  size = 3.       
-00013a10: 2074 3120 3d20 6d61 6b65 5f74 6573 745f   t1 = make_test_
-00013a20: 7461 626c 6528 7365 6c66 2e6d 616b 655f  table(self.make_
-00013a30: 6461 7461 5f6f 626a 6563 742c 2074 6573  data_object, tes
-00013a40: 745f 7369 7a65 290a 0a20 2020 2020 2020  t_size)..       
-00013a50: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-00013a60: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
-00013a70: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
-00013a80: 6528 616c 6c28 6d61 6b65 5f64 6174 616f  e(all(make_datao
-00013a90: 626a 6563 745f 6672 6f6d 5f6f 6228 7265  bject_from_ob(re
-00013aa0: 6331 2920 3d3d 2072 6563 3220 666f 7220  c1) == rec2 for 
-00013ab0: 7265 6331 2c20 7265 6332 2069 6e20 7a69  rec1, rec2 in zi
-00013ac0: 7028 7431 2c20 6373 7674 6162 6c65 2929  p(t1, csvtable))
-00013ad0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
-00013ae0: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-00013af0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013b00: 6173 7365 7274 4571 7561 6c28 7375 6d28  assertEqual(sum(
-00013b10: 3120 666f 7220 6c69 6e65 2069 6e20 6461  1 for line in da
-00013b20: 7461 2e73 706c 6974 6c69 6e65 7328 2920  ta.splitlines() 
-00013b30: 6966 206c 696e 652e 7374 7269 7028 2929  if line.strip())
-00013b40: 2d31 2c20 6c65 6e28 6373 7674 6162 6c65  -1, len(csvtable
-00013b50: 2929 0a0a 2020 2020 2020 2020 726f 775f  ))..        row_
-00013b60: 7072 6f74 6f74 7970 6520 3d20 7365 6c66  prototype = self
-00013b70: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
-00013b80: 7428 302c 2030 2c20 3029 0a20 2020 2020  t(0, 0, 0).     
-00013b90: 2020 2063 7376 7461 626c 6532 203d 206c     csvtable2 = l
-00013ba0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
-00013bb0: 706f 7274 2864 6174 612c 2074 7261 6e73  port(data, trans
-00013bc0: 666f 726d 733d 7b27 6127 3a20 696e 742c  forms={'a': int,
-00013bd0: 2027 6227 3a20 696e 742c 2027 6327 3a20   'b': int, 'c': 
-00013be0: 696e 747d 2c0a 2020 2020 2020 2020 2020  int},.          
-00013bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c10: 726f 775f 636c 6173 733d 7479 7065 2872  row_class=type(r
-00013c20: 6f77 5f70 726f 746f 7479 7065 2929 5b3a  ow_prototype))[:
-00013c30: 335d 0a0a 2020 2020 2020 2020 7072 696e  3]..        prin
-00013c40: 7428 7479 7065 2874 315b 305d 292e 5f5f  t(type(t1[0]).__
-00013c50: 6e61 6d65 5f5f 2c20 7431 5b30 5d29 0a20  name__, t1[0]). 
-00013c60: 2020 2020 2020 2070 7269 6e74 2874 7970         print(typ
-00013c70: 6528 6373 7674 6162 6c65 325b 305d 292e  e(csvtable2[0]).
-00013c80: 5f5f 6e61 6d65 5f5f 2c20 6373 7674 6162  __name__, csvtab
-00013c90: 6c65 325b 305d 290a 2020 2020 2020 2020  le2[0]).        
-00013ca0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-00013cb0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-00013cc0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00013cd0: 6c28 7479 7065 2874 315b 305d 292c 2074  l(type(t1[0]), t
-00013ce0: 7970 6528 6373 7674 6162 6c65 325b 305d  ype(csvtable2[0]
-00013cf0: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
-00013d00: 5f63 7376 5f6c 696d 6974 5f69 6d70 6f72  _csv_limit_impor
-00013d10: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
-00013d20: 2064 6174 6120 3d20 6373 765f 6461 7461   data = csv_data
-00013d30: 0a20 2020 2020 2020 2069 6d70 6f72 745f  .        import_
-00013d40: 6c69 6d69 7420 3d20 3130 0a20 2020 2020  limit = 10.     
-00013d50: 2020 2063 7376 7461 626c 6520 3d20 6c74     csvtable = lt
-00013d60: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
-00013d70: 6f72 7428 6373 765f 736f 7572 6365 3d64  ort(csv_source=d
-00013d80: 6174 612c 2074 7261 6e73 666f 726d 733d  ata, transforms=
-00013d90: 7b27 6127 3a20 696e 742c 2027 6227 3a20  {'a': int, 'b': 
-00013da0: 696e 742c 2027 6327 3a20 696e 747d 2c0a  int, 'c': int},.
-00013db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013dd0: 2020 2020 2020 2020 206c 696d 6974 3d69           limit=i
-00013de0: 6d70 6f72 745f 6c69 6d69 7429 0a0a 2020  mport_limit)..  
-00013df0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00013e00: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-00013e10: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00013e20: 7274 4571 7561 6c28 696d 706f 7274 5f6c  rtEqual(import_l
-00013e30: 696d 6974 2c20 6c65 6e28 6373 7674 6162  imit, len(csvtab
-00013e40: 6c65 2929 0a0a 2020 2020 2020 2020 6373  le))..        cs
-00013e50: 7674 6162 6c65 203d 206c 742e 5461 626c  vtable = lt.Tabl
-00013e60: 6528 292e 6373 765f 696d 706f 7274 2863  e().csv_import(c
-00013e70: 7376 5f73 6f75 7263 653d 6461 7461 2c20  sv_source=data, 
-00013e80: 7472 616e 7366 6f72 6d73 3d7b 2761 273a  transforms={'a':
-00013e90: 2069 6e74 2c20 2762 273a 2069 6e74 2c20   int, 'b': int, 
-00013ea0: 2763 273a 2069 6e74 7d2c 0a20 2020 2020  'c': int},.     
-00013eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013200: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00013210: 7465 7273 3d7b 2263 223a 206c 742e 5461  ters={"c": lt.Ta
+00013220: 626c 652e 6571 2831 297d 290a 2020 2020  ble.eq(1)}).    
+00013230: 2020 2020 7072 696e 7428 7474 2e69 6e66      print(tt.inf
+00013240: 6f28 2929 0a20 2020 2020 2020 2077 6974  o()).        wit
+00013250: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00013260: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00013270: 6c66 2e61 7373 6572 7445 7175 616c 2874  lf.assertEqual(t
+00013280: 6573 745f 7369 7a65 202a 2074 6573 745f  est_size * test_
+00013290: 7369 7a65 2c20 6c65 6e28 7474 2929 0a0a  size, len(tt))..
+000132a0: 2020 2020 2020 2020 7474 203d 206c 742e          tt = lt.
+000132b0: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
+000132c0: 7274 2822 7465 7374 2f61 6263 2e63 7376  rt("test/abc.csv
+000132d0: 222c 2074 7261 6e73 666f 726d 733d 6469  ", transforms=di
+000132e0: 6374 2e66 726f 6d6b 6579 7328 2261 6263  ct.fromkeys("abc
+000132f0: 222c 2069 6e74 292c 0a20 2020 2020 2020  ", int),.       
+00013300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013310: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
+00013320: 6572 733d 7b22 6322 3a20 317d 290a 2020  ers={"c": 1}).  
+00013330: 2020 2020 2020 7072 696e 7428 7474 2e69        print(tt.i
+00013340: 6e66 6f28 2929 0a20 2020 2020 2020 2077  nfo()).        w
+00013350: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00013360: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00013370: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00013380: 2874 6573 745f 7369 7a65 202a 2074 6573  (test_size * tes
+00013390: 745f 7369 7a65 2c20 6c65 6e28 7474 2929  t_size, len(tt))
+000133a0: 0a0a 2020 2020 2020 2020 7474 203d 206c  ..        tt = l
+000133b0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
+000133c0: 706f 7274 2822 7465 7374 2f61 6263 2e63  port("test/abc.c
+000133d0: 7376 222c 2074 7261 6e73 666f 726d 733d  sv", transforms=
+000133e0: 6469 6374 2e66 726f 6d6b 6579 7328 2261  dict.fromkeys("a
+000133f0: 6263 222c 2069 6e74 292c 0a20 2020 2020  bc", int),.     
+00013400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013410: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00013420: 6c74 6572 733d 7b22 6322 3a20 6c61 6d62  lters={"c": lamb
+00013430: 6461 2078 3a20 3020 3c20 7820 3c20 327d  da x: 0 < x < 2}
+00013440: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+00013450: 7474 2e69 6e66 6f28 2929 0a20 2020 2020  tt.info()).     
+00013460: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+00013470: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+00013480: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00013490: 7175 616c 2874 6573 745f 7369 7a65 202a  qual(test_size *
+000134a0: 2074 6573 745f 7369 7a65 2c20 6c65 6e28   test_size, len(
+000134b0: 7474 2929 0a0a 2020 2020 2020 2020 2320  tt))..        # 
+000134c0: 7465 7374 2061 6c6c 2073 7065 6369 616c  test all special
+000134d0: 2063 6f6d 7061 7261 746f 7273 2077 6865   comparators whe
+000134e0: 6e20 7573 6564 2061 7320 6669 6c74 6572  n used as filter
+000134f0: 730a 2020 2020 2020 2020 2320 2020 2020  s.        #     
+00013500: 6973 5f6e 6f6e 6520 2d20 6174 7472 6962  is_none - attrib
+00013510: 7574 6520 7661 6c75 6520 6973 204e 6f6e  ute value is Non
+00013520: 650a 2020 2020 2020 2020 2320 2020 2020  e.        #     
+00013530: 6973 5f6e 6f74 5f6e 6f6e 6520 2d20 6174  is_not_none - at
+00013540: 7472 6962 7574 6520 7661 6c75 6520 6973  tribute value is
+00013550: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
+00013560: 2020 2320 2020 2020 6973 5f6e 756c 6c20    #     is_null 
+00013570: 2d20 6174 7472 6962 7574 6520 7661 6c75  - attribute valu
+00013580: 6520 6973 204e 6f6e 652c 2022 222c 206f  e is None, "", o
+00013590: 7220 6e6f 7420 6465 6669 6e65 640a 2020  r not defined.  
+000135a0: 2020 2020 2020 2320 2020 2020 6973 5f6e        #     is_n
+000135b0: 6f74 5f6e 756c 6c20 2d20 6174 7472 6962  ot_null - attrib
+000135c0: 7574 6520 7661 6c75 6520 6973 2064 6566  ute value is def
+000135d0: 696e 6564 2c20 616e 6420 6973 206e 6f74  ined, and is not
+000135e0: 204e 6f6e 6520 6f72 2022 220a 2020 2020   None or "".    
+000135f0: 2020 2020 2320 2020 2020 7374 6172 7473      #     starts
+00013600: 7769 7468 202d 2061 7474 7269 6275 7465  with - attribute
+00013610: 2076 616c 7565 2073 7461 7274 7320 7769   value starts wi
+00013620: 7468 2061 2067 6976 656e 2073 7472 696e  th a given strin
+00013630: 670a 2020 2020 2020 2020 2320 2020 2020  g.        #     
+00013640: 656e 6473 7769 7468 202d 2061 7474 7269  endswith - attri
+00013650: 6275 7465 2076 616c 7565 2065 6e64 7320  bute value ends 
+00013660: 7769 7468 2061 2067 6976 656e 2073 7472  with a given str
+00013670: 696e 670a 2020 2020 2020 2020 2320 2020  ing.        #   
+00013680: 2020 7265 5f6d 6174 6368 202d 2061 7474    re_match - att
+00013690: 7269 6275 7465 2076 616c 7565 206d 6174  ribute value mat
+000136a0: 6368 6573 2061 2072 6567 756c 6172 2065  ches a regular e
+000136b0: 7870 7265 7373 696f 6e0a 0a20 2020 2020  xpression..     
+000136c0: 2020 2070 7269 6e74 2829 0a20 2020 2020     print().     
+000136d0: 2020 2069 6e70 7574 5f64 6174 6120 3d20     input_data = 
+000136e0: 7465 7874 7772 6170 2e64 6564 656e 7428  textwrap.dedent(
+000136f0: 2222 225c 0a20 2020 2020 2020 206e 616d  """\.        nam
+00013700: 652c 612c 622c 630a 2020 2020 2020 2020  e,a,b,c.        
+00013710: 2241 222c 3130 302c 3130 302c 3130 300a  "A",100,100,100.
+00013720: 2020 2020 2020 2020 2242 222c 3230 302c          "B",200,
+00013730: 2c32 3030 0a20 2020 2020 2020 2022 4131  ,200.        "A1
+00013740: 222c 3130 312c 3130 312c 3130 310a 2020  ",101,101,101.  
+00013750: 2020 2020 2020 2242 3122 2c32 3031 2c2c        "B1",201,,
+00013760: 3230 310a 2020 2020 2020 2020 2243 3122  201.        "C1"
+00013770: 2c33 3031 2c2c 3330 310a 2020 2020 2020  ,301,,301.      
+00013780: 2020 2c39 392c 3939 2c39 390a 2020 2020    ,99,99,99.    
+00013790: 2020 2020 2222 2229 0a20 2020 2020 2020      """).       
+000137a0: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
+000137b0: 696d 706f 7274 2869 6e70 7574 5f64 6174  import(input_dat
+000137c0: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+000137d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137e0: 2074 7261 6e73 666f 726d 733d 6469 6374   transforms=dict
+000137f0: 2e66 726f 6d6b 6579 7328 2261 6263 222c  .fromkeys("abc",
+00013800: 2069 6e74 292c 0a20 2020 2020 2020 2020   int),.         
+00013810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013820: 2020 2020 2029 2e70 7265 7365 6e74 2829       ).present()
+00013830: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00013840: 2020 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2d        +---------
+00013850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013860: 2b0a 2020 2020 2020 2020 7c20 4e61 6d65  +.        | Name
+00013870: 207c 2020 2041 207c 2020 2020 4220 7c20   |   A |    B | 
+00013880: 2020 4320 7c0a 2020 2020 2020 2020 7c2d    C |.        |-
+00013890: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2b 2d2d 2d2d  -----+-----+----
+000138a0: 2d2d 2b2d 2d2d 2d2d 7c0a 2020 2020 2020  --+-----|.      
+000138b0: 2020 7c20 4120 2020 207c 2031 3030 207c    | A    | 100 |
+000138c0: 2020 3130 3020 7c20 3130 3020 7c0a 2020    100 | 100 |.  
+000138d0: 2020 2020 2020 7c20 4220 2020 207c 2032        | B    | 2
+000138e0: 3030 207c 204e 6f6e 6520 7c20 3230 3020  00 | None | 200 
+000138f0: 7c0a 2020 2020 2020 2020 7c20 4131 2020  |.        | A1  
+00013900: 207c 2031 3031 207c 2020 3130 3120 7c20   | 101 |  101 | 
+00013910: 3130 3120 7c0a 2020 2020 2020 2020 7c20  101 |.        | 
+00013920: 4231 2020 207c 2032 3031 207c 204e 6f6e  B1   | 201 | Non
+00013930: 6520 7c20 3230 3120 7c0a 2020 2020 2020  e | 201 |.      
+00013940: 2020 7c20 4331 2020 207c 2033 3031 207c    | C1   | 301 |
+00013950: 204e 6f6e 6520 7c20 3330 3120 7c0a 2020   None | 301 |.  
+00013960: 2020 2020 2020 7c20 2020 2020 207c 2020        |      |  
+00013970: 3939 207c 2020 2039 3920 7c20 2039 3920  99 |   99 |  99 
+00013980: 7c0a 2020 2020 2020 2020 2b2d 2d2d 2d2d  |.        +-----
+00013990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000139a0: 2d2d 2d2d 2b0a 2020 2020 2020 2020 2222  ----+.        ""
+000139b0: 220a 0a20 2020 2020 2020 2070 7269 6e74  "..        print
+000139c0: 2822 6973 5f6e 6f6e 6528 2922 290a 2020  ("is_none()").  
+000139d0: 2020 2020 2020 7820 3d20 6c74 2e54 6162        x = lt.Tab
+000139e0: 6c65 2829 2e63 7376 5f69 6d70 6f72 7428  le().csv_import(
+000139f0: 696e 7075 745f 6461 7461 2c0a 2020 2020  input_data,.    
+00013a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a20: 2020 2020 2074 7261 6e73 666f 726d 733d       transforms=
+00013a30: 6469 6374 2e66 726f 6d6b 6579 7328 2261  dict.fromkeys("a
+00013a40: 6263 222c 2069 6e74 292c 0a20 2020 2020  bc", int),.     
+00013a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a70: 2020 2020 6669 6c74 6572 733d 7b22 6222      filters={"b"
+00013a80: 3a20 6c74 2e54 6162 6c65 2e69 735f 6e6f  : lt.Table.is_no
+00013a90: 6e65 2829 7d29 0a20 2020 2020 2020 2077  ne()}).        w
+00013aa0: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00013ab0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00013ac0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00013ad0: 2833 2c20 6c65 6e28 7829 290a 2020 2020  (3, len(x)).    
+00013ae0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+00013af0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+00013b00: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00013b10: 5472 7565 2861 6c6c 2862 2069 7320 4e6f  True(all(b is No
+00013b20: 6e65 2066 6f72 2062 2069 6e20 782e 616c  ne for b in x.al
+00013b30: 6c2e 6229 290a 0a20 2020 2020 2020 2070  l.b))..        p
+00013b40: 7269 6e74 2822 6973 5f6e 6f74 5f6e 6f6e  rint("is_not_non
+00013b50: 6528 2922 290a 2020 2020 2020 2020 7820  e()").        x 
+00013b60: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
+00013b70: 5f69 6d70 6f72 7428 696e 7075 745f 6461  _import(input_da
+00013b80: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+00013b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ba0: 2020 2020 2020 7472 616e 7366 6f72 6d73        transforms
+00013bb0: 3d64 6963 742e 6672 6f6d 6b65 7973 2822  =dict.fromkeys("
+00013bc0: 6162 6322 2c20 696e 7429 2c0a 2020 2020  abc", int),.    
+00013bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013be0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00013bf0: 6c74 6572 733d 7b22 6222 3a20 6c74 2e54  lters={"b": lt.T
+00013c00: 6162 6c65 2e69 735f 6e6f 745f 6e6f 6e65  able.is_not_none
+00013c10: 2829 7d29 0a20 2020 2020 2020 2077 6974  ()}).        wit
+00013c20: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00013c30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00013c40: 6c66 2e61 7373 6572 7445 7175 616c 2833  lf.assertEqual(3
+00013c50: 2c20 6c65 6e28 7829 290a 2020 2020 2020  , len(x)).      
+00013c60: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00013c70: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00013c80: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00013c90: 7561 6c28 3330 302c 2073 756d 2878 2e61  ual(300, sum(x.a
+00013ca0: 6c6c 2e62 2929 0a0a 2020 2020 2020 2020  ll.b))..        
+00013cb0: 7072 696e 7428 2262 2069 735f 6e75 6c6c  print("b is_null
+00013cc0: 2829 2229 0a20 2020 2020 2020 2078 203d  ()").        x =
+00013cd0: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
+00013ce0: 696d 706f 7274 2869 6e70 7574 5f64 6174  import(input_dat
+00013cf0: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+00013d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d10: 2020 2020 2074 7261 6e73 666f 726d 733d       transforms=
+00013d20: 6469 6374 2e66 726f 6d6b 6579 7328 2261  dict.fromkeys("a
+00013d30: 6263 222c 2069 6e74 292c 0a20 2020 2020  bc", int),.     
+00013d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d50: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00013d60: 7465 7273 3d7b 2262 223a 206c 742e 5461  ters={"b": lt.Ta
+00013d70: 626c 652e 6973 5f6e 756c 6c28 297d 290a  ble.is_null()}).
+00013d80: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00013d90: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+00013da0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00013db0: 7365 7274 4571 7561 6c28 332c 206c 656e  sertEqual(3, len
+00013dc0: 2878 2929 0a20 2020 2020 2020 2077 6974  (x)).        wit
+00013dd0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00013de0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00013df0: 6c66 2e61 7373 6572 7454 7275 6528 616c  lf.assertTrue(al
+00013e00: 6c28 6220 6973 204e 6f6e 6520 666f 7220  l(b is None for 
+00013e10: 6220 696e 2078 2e61 6c6c 2e62 2929 0a0a  b in x.all.b))..
+00013e20: 2020 2020 2020 2020 7072 696e 7428 2262          print("b
+00013e30: 2069 735f 6e6f 745f 6e75 6c6c 2829 2229   is_not_null()")
+00013e40: 0a20 2020 2020 2020 2078 203d 206c 742e  .        x = lt.
+00013e50: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
+00013e60: 7274 2869 6e70 7574 5f64 6174 612c 0a20  rt(input_data,. 
+00013e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e90: 2074 7261 6e73 666f 726d 733d 6469 6374   transforms=dict
+00013ea0: 2e66 726f 6d6b 6579 7328 2261 6263 222c  .fromkeys("abc",
+00013eb0: 2069 6e74 292c 0a20 2020 2020 2020 2020   int),.         
 00013ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ed0: 2020 2020 6c69 6d69 743d 3029 0a0a 2020      limit=0)..  
-00013ee0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00013ef0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-00013f00: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00013f10: 7274 4571 7561 6c28 302c 206c 656e 2863  rtEqual(0, len(c
-00013f20: 7376 7461 626c 6529 290a 0a20 2020 2064  svtable))..    d
-00013f30: 6566 2074 6573 745f 6373 765f 7374 7269  ef test_csv_stri
-00013f40: 6e67 5f6c 6973 745f 696d 706f 7274 2873  ng_list_import(s
-00013f50: 656c 6629 3a0a 2020 2020 2020 2020 6461  elf):.        da
-00013f60: 7461 203d 2063 7376 5f64 6174 610a 2020  ta = csv_data.  
-00013f70: 2020 2020 2020 6373 7674 6162 6c65 203d        csvtable =
-00013f80: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
-00013f90: 696d 706f 7274 2863 7376 5f73 6f75 7263  import(csv_sourc
-00013fa0: 653d 6461 7461 2e73 706c 6974 6c69 6e65  e=data.splitline
-00013fb0: 7328 292c 2074 7261 6e73 666f 726d 733d  s(), transforms=
-00013fc0: 7b27 6127 3a20 696e 742c 2027 6227 3a20  {'a': int, 'b': 
-00013fd0: 696e 742c 2027 6327 3a20 696e 747d 290a  int, 'c': int}).
-00013fe0: 0a20 2020 2020 2020 2074 6573 745f 7369  .        test_si
-00013ff0: 7a65 203d 2033 0a20 2020 2020 2020 2074  ze = 3.        t
-00014000: 3120 3d20 6d61 6b65 5f74 6573 745f 7461  1 = make_test_ta
-00014010: 626c 6528 7365 6c66 2e6d 616b 655f 6461  ble(self.make_da
-00014020: 7461 5f6f 626a 6563 742c 2074 6573 745f  ta_object, test_
-00014030: 7369 7a65 290a 0a20 2020 2020 2020 2077  size)..        w
-00014040: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00014050: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00014060: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-00014070: 616c 6c28 6d61 6b65 5f64 6174 616f 626a  all(make_dataobj
-00014080: 6563 745f 6672 6f6d 5f6f 6228 7265 6331  ect_from_ob(rec1
-00014090: 2920 3d3d 2072 6563 3220 666f 7220 7265  ) == rec2 for re
-000140a0: 6331 2c20 7265 6332 2069 6e20 7a69 7028  c1, rec2 in zip(
-000140b0: 7431 2c20 6373 7674 6162 6c65 2929 290a  t1, csvtable))).
-000140c0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-000140d0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-000140e0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-000140f0: 7365 7274 4571 7561 6c28 7375 6d28 3120  sertEqual(sum(1 
-00014100: 666f 7220 6c69 6e65 2069 6e20 6461 7461  for line in data
-00014110: 2e73 706c 6974 6c69 6e65 7328 2920 6966  .splitlines() if
-00014120: 206c 696e 652e 7374 7269 7028 2929 2d31   line.strip())-1
-00014130: 2c20 6c65 6e28 6373 7674 6162 6c65 2929  , len(csvtable))
-00014140: 0a0a 2020 2020 2020 2020 726f 775f 7072  ..        row_pr
-00014150: 6f74 6f74 7970 6520 3d20 7365 6c66 2e6d  ototype = self.m
-00014160: 616b 655f 6461 7461 5f6f 626a 6563 7428  ake_data_object(
-00014170: 302c 2030 2c20 3029 0a20 2020 2020 2020  0, 0, 0).       
-00014180: 2063 7376 7461 626c 6532 203d 206c 742e   csvtable2 = lt.
-00014190: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
-000141a0: 7274 2864 6174 612c 2074 7261 6e73 666f  rt(data, transfo
-000141b0: 726d 733d 7b27 6127 3a20 696e 742c 2027  rms={'a': int, '
-000141c0: 6227 3a20 696e 742c 2027 6327 3a20 696e  b': int, 'c': in
-000141d0: 747d 2c0a 2020 2020 2020 2020 2020 2020  t},.            
-000141e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141f0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-00014200: 775f 636c 6173 733d 7479 7065 2872 6f77  w_class=type(row
-00014210: 5f70 726f 746f 7479 7065 2929 5b3a 335d  _prototype))[:3]
-00014220: 0a0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00014230: 7479 7065 2874 315b 305d 292e 5f5f 6e61  type(t1[0]).__na
-00014240: 6d65 5f5f 2c20 7431 5b30 5d29 0a20 2020  me__, t1[0]).   
-00014250: 2020 2020 2070 7269 6e74 2874 7970 6528       print(type(
-00014260: 6373 7674 6162 6c65 325b 305d 292e 5f5f  csvtable2[0]).__
-00014270: 6e61 6d65 5f5f 2c20 6373 7674 6162 6c65  name__, csvtable
-00014280: 325b 305d 290a 2020 2020 2020 2020 7769  2[0]).        wi
-00014290: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-000142a0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-000142b0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-000142c0: 7479 7065 2874 315b 305d 292c 2074 7970  type(t1[0]), typ
-000142d0: 6528 6373 7674 6162 6c65 325b 305d 2929  e(csvtable2[0]))
-000142e0: 0a0a 2020 2020 6465 6620 7465 7374 5f63  ..    def test_c
-000142f0: 7376 5f6e 756d 6572 6963 5f74 7261 6e73  sv_numeric_trans
-00014300: 666f 726d 7328 7365 6c66 293a 0a20 2020  forms(self):.   
-00014310: 2020 2020 2064 6174 6120 3d20 7465 7874       data = text
-00014320: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
-00014330: 0a20 2020 2020 2020 2020 2020 2074 7970  .            typ
-00014340: 652c 7661 6c75 650a 2020 2020 2020 2020  e,value.        
-00014350: 2020 2020 696e 742c 3130 3030 0a20 2020      int,1000.   
-00014360: 2020 2020 2020 2020 2066 6c6f 6174 2c33           float,3
-00014370: 2e31 340a 2020 2020 2020 2020 2020 2020  .14.            
-00014380: 656d 7074 792c 0a20 2020 2020 2020 2020  empty,.         
-00014390: 2020 2073 7472 2ce2 93a0 2a62 6572 740a     str,...*bert.
-000143a0: 2020 2020 2020 2020 2020 2020 2222 2229              """)
-000143b0: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
-000143c0: 656c 662e 7375 6254 6573 7428 2263 6f6e  elf.subTest("con
-000143d0: 7665 7274 5f6e 756d 6572 6963 2229 3a0a  vert_numeric"):.
-000143e0: 2020 2020 2020 2020 2020 2020 7462 6c20              tbl 
-000143f0: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
-00014400: 5f69 6d70 6f72 7428 6461 7461 2c20 7472  _import(data, tr
-00014410: 616e 7366 6f72 6d73 3d7b 2776 616c 7565  ansforms={'value
-00014420: 273a 206c 742e 5461 626c 652e 636f 6e76  ': lt.Table.conv
-00014430: 6572 745f 6e75 6d65 7269 637d 290a 2020  ert_numeric}).  
-00014440: 2020 2020 2020 2020 2020 7462 6c2e 7072            tbl.pr
-00014450: 6573 656e 7428 290a 2020 2020 2020 2020  esent().        
-00014460: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00014470: 7175 616c 285b 3130 3030 2c20 332e 3134  qual([1000, 3.14
-00014480: 2c20 2727 2c20 27e2 93a0 2a62 6572 7427  , '', '...*bert'
-00014490: 5d2c 206c 6973 7428 7462 6c2e 616c 6c2e  ], list(tbl.all.
-000144a0: 7661 6c75 6529 290a 0a20 2020 2020 2020  value))..       
-000144b0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-000144c0: 7374 2822 636f 6e76 6572 745f 6e75 6d65  st("convert_nume
-000144d0: 7269 6328 2922 293a 0a20 2020 2020 2020  ric()"):.       
-000144e0: 2020 2020 2074 626c 203d 206c 742e 5461       tbl = lt.Ta
-000144f0: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
-00014500: 2864 6174 612c 2074 7261 6e73 666f 726d  (data, transform
-00014510: 733d 7b27 7661 6c75 6527 3a20 6c74 2e54  s={'value': lt.T
-00014520: 6162 6c65 2e63 6f6e 7665 7274 5f6e 756d  able.convert_num
-00014530: 6572 6963 2829 7d29 0a20 2020 2020 2020  eric()}).       
-00014540: 2020 2020 2074 626c 2e70 7265 7365 6e74       tbl.present
-00014550: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-00014560: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00014570: 5b31 3030 302c 2033 2e31 342c 2027 272c  [1000, 3.14, '',
-00014580: 2027 e293 a02a 6265 7274 275d 2c20 6c69   '...*bert'], li
-00014590: 7374 2874 626c 2e61 6c6c 2e76 616c 7565  st(tbl.all.value
-000145a0: 2929 0a0a 2020 2020 2020 2020 7769 7468  ))..        with
-000145b0: 2073 656c 662e 7375 6254 6573 7428 2263   self.subTest("c
-000145c0: 6f6e 7665 7274 5f6e 756d 6572 6963 286e  onvert_numeric(n
-000145d0: 6f6e 5f6e 756d 6572 6963 3d4e 6f6e 6529  on_numeric=None)
-000145e0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-000145f0: 7462 6c20 3d20 6c74 2e54 6162 6c65 2829  tbl = lt.Table()
-00014600: 2e63 7376 5f69 6d70 6f72 7428 6461 7461  .csv_import(data
-00014610: 2c20 7472 616e 7366 6f72 6d73 3d7b 2776  , transforms={'v
-00014620: 616c 7565 273a 206c 742e 5461 626c 652e  alue': lt.Table.
-00014630: 636f 6e76 6572 745f 6e75 6d65 7269 6328  convert_numeric(
-00014640: 6e6f 6e5f 6e75 6d65 7269 633d 4e6f 6e65  non_numeric=None
-00014650: 297d 290a 2020 2020 2020 2020 2020 2020  )}).            
-00014660: 7462 6c2e 7072 6573 656e 7428 290a 2020  tbl.present().  
-00014670: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00014680: 7373 6572 7445 7175 616c 285b 3130 3030  ssertEqual([1000
-00014690: 2c20 332e 3134 2c20 2727 2c20 4e6f 6e65  , 3.14, '', None
-000146a0: 5d2c 206c 6973 7428 7462 6c2e 616c 6c2e  ], list(tbl.all.
-000146b0: 7661 6c75 6529 290a 0a20 2020 2020 2020  value))..       
-000146c0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
-000146d0: 7374 2822 636f 6e76 6572 745f 6e75 6d65  st("convert_nume
-000146e0: 7269 6328 6e6f 6e5f 6e75 6d65 7269 633d  ric(non_numeric=
-000146f0: 3029 2229 3a0a 2020 2020 2020 2020 2020  0)"):.          
-00014700: 2020 7462 6c20 3d20 6c74 2e54 6162 6c65    tbl = lt.Table
-00014710: 2829 2e63 7376 5f69 6d70 6f72 7428 6461  ().csv_import(da
-00014720: 7461 2c20 7472 616e 7366 6f72 6d73 3d7b  ta, transforms={
-00014730: 2776 616c 7565 273a 206c 742e 5461 626c  'value': lt.Tabl
-00014740: 652e 636f 6e76 6572 745f 6e75 6d65 7269  e.convert_numeri
-00014750: 6328 6e6f 6e5f 6e75 6d65 7269 633d 3029  c(non_numeric=0)
-00014760: 7d29 0a20 2020 2020 2020 2020 2020 2074  }).            t
-00014770: 626c 2e70 7265 7365 6e74 2829 0a20 2020  bl.present().   
-00014780: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00014790: 7365 7274 4571 7561 6c28 5b31 3030 302c  sertEqual([1000,
-000147a0: 2033 2e31 342c 2027 272c 2030 5d2c 206c   3.14, '', 0], l
-000147b0: 6973 7428 7462 6c2e 616c 6c2e 7661 6c75  ist(tbl.all.valu
-000147c0: 6529 290a 0a20 2020 2020 2020 2077 6974  e))..        wit
-000147d0: 6820 7365 6c66 2e73 7562 5465 7374 2822  h self.subTest("
-000147e0: 636f 6e76 6572 745f 6e75 6d65 7269 6328  convert_numeric(
-000147f0: 696e 745f 746f 5f66 6c6f 6174 3d54 7275  int_to_float=Tru
-00014800: 6529 2229 3a0a 2020 2020 2020 2020 2020  e)"):.          
-00014810: 2020 7462 6c20 3d20 6c74 2e54 6162 6c65    tbl = lt.Table
-00014820: 2829 2e63 7376 5f69 6d70 6f72 7428 6461  ().csv_import(da
-00014830: 7461 2c20 7472 616e 7366 6f72 6d73 3d7b  ta, transforms={
-00014840: 2776 616c 7565 273a 206c 742e 5461 626c  'value': lt.Tabl
-00014850: 652e 636f 6e76 6572 745f 6e75 6d65 7269  e.convert_numeri
-00014860: 6328 666f 7263 655f 666c 6f61 743d 5472  c(force_float=Tr
-00014870: 7565 297d 290a 2020 2020 2020 2020 2020  ue)}).          
-00014880: 2020 7462 6c2e 7072 6573 656e 7428 290a    tbl.present().
-00014890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000148a0: 2e61 7373 6572 7445 7175 616c 285b 3130  .assertEqual([10
-000148b0: 3030 2e30 2c20 332e 3134 2c20 2727 2c20  00.0, 3.14, '', 
-000148c0: 27e2 93a0 2a62 6572 7427 5d2c 206c 6973  '...*bert'], lis
-000148d0: 7428 7462 6c2e 616c 6c2e 7661 6c75 6529  t(tbl.all.value)
-000148e0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000148f0: 6c66 2e61 7373 6572 7445 7175 616c 285b  lf.assertEqual([
-00014900: 666c 6f61 742c 2066 6c6f 6174 2c20 7374  float, float, st
-00014910: 722c 2073 7472 5d2c 206c 6973 7428 7479  r, str], list(ty
-00014920: 7065 2876 2920 666f 7220 7620 696e 2074  pe(v) for v in t
-00014930: 626c 2e61 6c6c 2e76 616c 7565 2929 0a0a  bl.all.value))..
-00014940: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00014950: 662e 7375 6254 6573 7428 2263 6f6e 7665  f.subTest("conve
-00014960: 7274 5f6e 756d 6572 6963 286e 6f6e 5f6e  rt_numeric(non_n
-00014970: 756d 6572 6963 3d4e 6f6e 652c 2065 6d70  umeric=None, emp
-00014980: 7479 3d4e 6f6e 6529 2229 3a0a 2020 2020  ty=None)"):.    
-00014990: 2020 2020 2020 2020 7462 6c20 3d20 6c74          tbl = lt
-000149a0: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
-000149b0: 6f72 7428 6461 7461 2c20 7472 616e 7366  ort(data, transf
-000149c0: 6f72 6d73 3d7b 2776 616c 7565 273a 206c  orms={'value': l
-000149d0: 742e 5461 626c 652e 636f 6e76 6572 745f  t.Table.convert_
-000149e0: 6e75 6d65 7269 6328 6e6f 6e5f 6e75 6d65  numeric(non_nume
-000149f0: 7269 633d 4e6f 6e65 2c20 656d 7074 793d  ric=None, empty=
-00014a00: 4e6f 6e65 297d 290a 2020 2020 2020 2020  None)}).        
-00014a10: 2020 2020 7462 6c2e 7072 6573 656e 7428      tbl.present(
-00014a20: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00014a30: 6c66 2e61 7373 6572 7445 7175 616c 285b  lf.assertEqual([
-00014a40: 3130 3030 2c20 332e 3134 2c20 4e6f 6e65  1000, 3.14, None
-00014a50: 2c20 4e6f 6e65 5d2c 206c 6973 7428 7462  , None], list(tb
-00014a60: 6c2e 616c 6c2e 7661 6c75 6529 290a 0a20  l.all.value)).. 
-00014a70: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00014a80: 2e73 7562 5465 7374 2822 636f 6e76 6572  .subTest("conver
-00014a90: 745f 6e75 6d65 7269 6328 656d 7074 793d  t_numeric(empty=
-00014aa0: 4e6f 6e65 2922 293a 0a20 2020 2020 2020  None)"):.       
-00014ab0: 2020 2020 2074 626c 203d 206c 742e 5461       tbl = lt.Ta
-00014ac0: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
-00014ad0: 2864 6174 612c 2074 7261 6e73 666f 726d  (data, transform
-00014ae0: 733d 7b27 7661 6c75 6527 3a20 6c74 2e54  s={'value': lt.T
-00014af0: 6162 6c65 2e63 6f6e 7665 7274 5f6e 756d  able.convert_num
-00014b00: 6572 6963 2865 6d70 7479 3d4e 6f6e 6529  eric(empty=None)
-00014b10: 7d29 0a20 2020 2020 2020 2020 2020 2074  }).            t
-00014b20: 626c 2e70 7265 7365 6e74 2829 0a20 2020  bl.present().   
-00014b30: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00014b40: 7365 7274 4571 7561 6c28 5b31 3030 302c  sertEqual([1000,
-00014b50: 2033 2e31 342c 204e 6f6e 652c 2027 e293   3.14, None, '..
-00014b60: a02a 6265 7274 275d 2c20 6c69 7374 2874  .*bert'], list(t
-00014b70: 626c 2e61 6c6c 2e76 616c 7565 2929 0a0a  bl.all.value))..
-00014b80: 2020 2020 6465 6620 7465 7374 5f6a 736f      def test_jso
-00014b90: 6e5f 6578 706f 7274 5f73 7472 6561 6d69  n_export_streami
-00014ba0: 6e67 2873 656c 6629 3a0a 2020 2020 2020  ng(self):.      
-00014bb0: 2020 6672 6f6d 2069 7465 7274 6f6f 6c73    from itertools
-00014bc0: 2069 6d70 6f72 7420 7065 726d 7574 6174   import permutat
-00014bd0: 696f 6e73 0a20 2020 2020 2020 2074 6573  ions.        tes
-00014be0: 745f 7369 7a65 203d 2033 0a20 2020 2020  t_size = 3.     
-00014bf0: 2020 2074 3120 3d20 6d61 6b65 5f74 6573     t1 = make_tes
-00014c00: 745f 7461 626c 6528 7365 6c66 2e6d 616b  t_table(self.mak
-00014c10: 655f 6461 7461 5f6f 626a 6563 742c 2074  e_data_object, t
-00014c20: 6573 745f 7369 7a65 290a 2020 2020 2020  est_size).      
-00014c30: 2020 666f 7220 6669 656c 646e 616d 6573    for fieldnames
-00014c40: 2069 6e20 7065 726d 7574 6174 696f 6e73   in permutations
-00014c50: 286c 6973 7428 2761 6263 2729 293a 0a20  (list('abc')):. 
-00014c60: 2020 2020 2020 2020 2020 206f 7574 5f73             out_s
-00014c70: 7472 696e 6720 3d20 7431 2e6a 736f 6e5f  tring = t1.json_
-00014c80: 6578 706f 7274 284e 6f6e 652c 2066 6965  export(None, fie
-00014c90: 6c64 6e61 6d65 733d 6669 656c 646e 616d  ldnames=fieldnam
-00014ca0: 6573 2c20 7374 7265 616d 696e 673d 5472  es, streaming=Tr
-00014cb0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-00014cc0: 6f75 746c 696e 6573 203d 206f 7574 5f73  outlines = out_s
-00014cd0: 7472 696e 672e 7370 6c69 746c 696e 6573  tring.splitlines
-00014ce0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
-00014cf0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-00014d00: 7428 6669 656c 646e 616d 6573 3d66 6965  t(fieldnames=fie
-00014d10: 6c64 6e61 6d65 7329 3a0a 2020 2020 2020  ldnames):.      
-00014d20: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00014d30: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
-00014d40: 7369 7a65 2a2a 332c 206c 656e 286f 7574  size**3, len(out
-00014d50: 6c69 6e65 7329 290a 0a20 2020 2020 2020  lines))..       
-00014d60: 2020 2020 2066 6f72 206f 622c 206c 696e       for ob, lin
-00014d70: 6520 696e 207a 6970 2874 312c 206f 7574  e in zip(t1, out
-00014d80: 6c69 6e65 7329 3a0a 2020 2020 2020 2020  lines):.        
-00014d90: 2020 2020 2020 2020 6a73 6f6e 5f64 6963          json_dic
-00014da0: 7420 3d20 6a73 6f6e 2e6c 6f61 6473 286c  t = json.loads(l
-00014db0: 696e 6529 0a20 2020 2020 2020 2020 2020  ine).           
-00014dc0: 2020 2020 2074 315f 6461 7461 6f62 6a20       t1_dataobj 
-00014dd0: 3d20 6d61 6b65 5f64 6174 616f 626a 6563  = make_dataobjec
-00014de0: 745f 6672 6f6d 5f6f 6228 6f62 290a 2020  t_from_ob(ob).  
-00014df0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-00014e00: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
-00014e10: 6f62 3d6f 622c 206c 696e 653d 6c69 6e65  ob=ob, line=line
-00014e20: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00014e30: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00014e40: 7274 4571 7561 6c28 7431 5f64 6174 616f  rtEqual(t1_datao
-00014e50: 626a 2c20 6c74 2e44 6174 614f 626a 6563  bj, lt.DataObjec
-00014e60: 7428 2a2a 6a73 6f6e 5f64 6963 7429 290a  t(**json_dict)).
-00014e70: 0a20 2020 2064 6566 2074 6573 745f 6a73  .    def test_js
-00014e80: 6f6e 5f65 7870 6f72 745f 6e6f 6e73 7472  on_export_nonstr
-00014e90: 6561 6d69 6e67 2873 656c 6629 3a0a 2020  eaming(self):.  
-00014ea0: 2020 2020 2020 6672 6f6d 2069 7465 7274        from itert
-00014eb0: 6f6f 6c73 2069 6d70 6f72 7420 7065 726d  ools import perm
-00014ec0: 7574 6174 696f 6e73 0a20 2020 2020 2020  utations.       
-00014ed0: 2069 6d70 6f72 7420 6a73 6f6e 0a20 2020   import json.   
-00014ee0: 2020 2020 2074 6573 745f 7369 7a65 203d       test_size =
-00014ef0: 2033 0a20 2020 2020 2020 2074 3120 3d20   3.        t1 = 
-00014f00: 6d61 6b65 5f74 6573 745f 7461 626c 6528  make_test_table(
-00014f10: 7365 6c66 2e6d 616b 655f 6461 7461 5f6f  self.make_data_o
-00014f20: 626a 6563 742c 2074 6573 745f 7369 7a65  bject, test_size
-00014f30: 290a 2020 2020 2020 2020 666f 7220 6669  ).        for fi
-00014f40: 656c 646e 616d 6573 2069 6e20 7065 726d  eldnames in perm
-00014f50: 7574 6174 696f 6e73 286c 6973 7428 2761  utations(list('a
-00014f60: 6263 2729 293a 0a20 2020 2020 2020 2020  bc')):.         
-00014f70: 2020 206f 7574 5f73 7472 696e 6720 3d20     out_string = 
-00014f80: 7431 2e6a 736f 6e5f 6578 706f 7274 284e  t1.json_export(N
-00014f90: 6f6e 652c 2066 6965 6c64 6e61 6d65 733d  one, fieldnames=
-00014fa0: 6669 656c 646e 616d 6573 2c20 7374 7265  fieldnames, stre
-00014fb0: 616d 696e 673d 4661 6c73 6529 0a20 2020  aming=False).   
-00014fc0: 2020 2020 2020 2020 206f 6273 6572 7665           observe
-00014fd0: 645f 6a73 6f6e 203d 206a 736f 6e2e 6c6f  d_json = json.lo
-00014fe0: 6164 7328 6f75 745f 7374 7269 6e67 290a  ads(out_string).
-00014ff0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00015000: 6820 7365 6c66 2e73 7562 5465 7374 2866  h self.subTest(f
-00015010: 6965 6c64 6e61 6d65 733d 6669 656c 646e  ieldnames=fieldn
-00015020: 616d 6573 293a 0a20 2020 2020 2020 2020  ames):.         
-00015030: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00015040: 7274 4571 7561 6c28 7465 7374 5f73 697a  rtEqual(test_siz
-00015050: 652a 2a33 2c20 6c65 6e28 6f62 7365 7276  e**3, len(observ
-00015060: 6564 5f6a 736f 6e29 290a 0a20 2020 2020  ed_json))..     
-00015070: 2020 2020 2020 2066 6f72 206f 622c 206a         for ob, j
-00015080: 736f 6e5f 6469 6374 2069 6e20 7a69 7028  son_dict in zip(
-00015090: 7431 2c20 6f62 7365 7276 6564 5f6a 736f  t1, observed_jso
-000150a0: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
-000150b0: 2020 2020 7431 5f64 6174 616f 626a 203d      t1_dataobj =
-000150c0: 206d 616b 655f 6461 7461 6f62 6a65 6374   make_dataobject
-000150d0: 5f66 726f 6d5f 6f62 286f 6229 0a20 2020  _from_ob(ob).   
-000150e0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-000150f0: 6820 7365 6c66 2e73 7562 5465 7374 286f  h self.subTest(o
-00015100: 623d 6f62 2c20 6a73 6f6e 5f64 6963 743d  b=ob, json_dict=
-00015110: 6a73 6f6e 5f64 6963 7429 3a0a 2020 2020  json_dict):.    
-00015120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015130: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00015140: 2874 315f 6461 7461 6f62 6a2c 206c 742e  (t1_dataobj, lt.
-00015150: 4461 7461 4f62 6a65 6374 282a 2a6a 736f  DataObject(**jso
-00015160: 6e5f 6469 6374 2929 0a0a 2020 2020 6465  n_dict))..    de
-00015170: 6620 7465 7374 5f6a 736f 6e5f 696d 706f  f test_json_impo
-00015180: 7274 2873 656c 6629 3a0a 2020 2020 2020  rt(self):.      
-00015190: 2020 6461 7461 203d 206a 736f 6e5f 6461    data = json_da
-000151a0: 7461 0a20 2020 2020 2020 2069 6e6a 736f  ta.        injso
-000151b0: 6e20 3d20 696f 2e53 7472 696e 6749 4f28  n = io.StringIO(
-000151c0: 6461 7461 290a 2020 2020 2020 2020 6a73  data).        js
-000151d0: 6f6e 7461 626c 6520 3d20 6c74 2e54 6162  ontable = lt.Tab
-000151e0: 6c65 2829 2e6a 736f 6e5f 696d 706f 7274  le().json_import
-000151f0: 2869 6e6a 736f 6e2c 2073 7472 6561 6d69  (injson, streami
-00015200: 6e67 3d54 7275 652c 2074 7261 6e73 666f  ng=True, transfo
-00015210: 726d 733d 7b27 6127 3a20 696e 742c 2027  rms={'a': int, '
-00015220: 6227 3a20 696e 742c 2027 6327 3a20 696e  b': int, 'c': in
-00015230: 747d 290a 0a20 2020 2020 2020 2074 6573  t})..        tes
-00015240: 745f 7369 7a65 203d 2033 0a20 2020 2020  t_size = 3.     
-00015250: 2020 2074 3120 3d20 6d61 6b65 5f74 6573     t1 = make_tes
-00015260: 745f 7461 626c 6528 7365 6c66 2e6d 616b  t_table(self.mak
-00015270: 655f 6461 7461 5f6f 626a 6563 742c 2074  e_data_object, t
-00015280: 6573 745f 7369 7a65 290a 0a20 2020 2020  est_size)..     
-00015290: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-000152a0: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-000152b0: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
-000152c0: 7275 6528 616c 6c28 6d61 6b65 5f64 6174  rue(all(make_dat
-000152d0: 616f 626a 6563 745f 6672 6f6d 5f6f 6228  aobject_from_ob(
-000152e0: 7265 6331 2920 3d3d 2072 6563 3220 666f  rec1) == rec2 fo
-000152f0: 7220 7265 6331 2c20 7265 6332 2069 6e20  r rec1, rec2 in 
-00015300: 7a69 7028 7431 2c20 6a73 6f6e 7461 626c  zip(t1, jsontabl
-00015310: 6529 2929 0a20 2020 2020 2020 2077 6974  e))).        wit
-00015320: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-00015330: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00015340: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
-00015350: 656e 285b 6420 666f 7220 6420 696e 2064  en([d for d in d
-00015360: 6174 612e 7370 6c69 746c 696e 6573 2829  ata.splitlines()
-00015370: 2069 6620 642e 7374 7269 7028 295d 292c   if d.strip()]),
-00015380: 206c 656e 286a 736f 6e74 6162 6c65 2929   len(jsontable))
-00015390: 0a0a 2020 2020 6465 6620 7465 7374 5f6a  ..    def test_j
-000153a0: 736f 6e5f 7374 7269 6e67 5f69 6d70 6f72  son_string_impor
-000153b0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
-000153c0: 2064 6174 6120 3d20 6a73 6f6e 5f64 6174   data = json_dat
-000153d0: 610a 2020 2020 2020 2020 6a73 6f6e 7461  a.        jsonta
-000153e0: 626c 6520 3d20 6c74 2e54 6162 6c65 2829  ble = lt.Table()
-000153f0: 2e6a 736f 6e5f 696d 706f 7274 2864 6174  .json_import(dat
-00015400: 612c 2073 7472 6561 6d69 6e67 3d54 7275  a, streaming=Tru
-00015410: 652c 2074 7261 6e73 666f 726d 733d 7b27  e, transforms={'
-00015420: 6127 3a20 696e 742c 2027 6227 3a20 696e  a': int, 'b': in
-00015430: 742c 2027 6327 3a20 696e 747d 290a 0a20  t, 'c': int}).. 
-00015440: 2020 2020 2020 2074 6573 745f 7369 7a65         test_size
-00015450: 203d 2033 0a20 2020 2020 2020 2074 3120   = 3.        t1 
-00015460: 3d20 6d61 6b65 5f74 6573 745f 7461 626c  = make_test_tabl
-00015470: 6528 7365 6c66 2e6d 616b 655f 6461 7461  e(self.make_data
-00015480: 5f6f 626a 6563 742c 2074 6573 745f 7369  _object, test_si
-00015490: 7a65 290a 0a20 2020 2020 2020 2077 6974  ze)..        wit
-000154a0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-000154b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000154c0: 6c66 2e61 7373 6572 7454 7275 6528 616c  lf.assertTrue(al
-000154d0: 6c28 6d61 6b65 5f64 6174 616f 626a 6563  l(make_dataobjec
-000154e0: 745f 6672 6f6d 5f6f 6228 7265 6331 2920  t_from_ob(rec1) 
-000154f0: 3d3d 2072 6563 3220 666f 7220 7265 6331  == rec2 for rec1
-00015500: 2c20 7265 6332 2069 6e20 7a69 7028 7431  , rec2 in zip(t1
-00015510: 2c20 6a73 6f6e 7461 626c 6529 2929 0a20  , jsontable))). 
-00015520: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00015530: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-00015540: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00015550: 6572 7445 7175 616c 286c 656e 285b 6420  ertEqual(len([d 
-00015560: 666f 7220 6420 696e 2064 6174 612e 7370  for d in data.sp
-00015570: 6c69 746c 696e 6573 2829 2069 6620 642e  litlines() if d.
-00015580: 7374 7269 7028 295d 292c 206c 656e 286a  strip()]), len(j
-00015590: 736f 6e74 6162 6c65 2929 0a0a 2020 2020  sontable))..    
-000155a0: 6465 6620 7465 7374 5f6a 736f 6e5f 7374  def test_json_st
-000155b0: 7269 6e67 5f6c 6973 745f 696d 706f 7274  ring_list_import
-000155c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000155d0: 6461 7461 203d 206a 736f 6e5f 6461 7461  data = json_data
-000155e0: 0a20 2020 2020 2020 206a 736f 6e74 6162  .        jsontab
-000155f0: 6c65 203d 206c 742e 5461 626c 6528 292e  le = lt.Table().
-00015600: 6a73 6f6e 5f69 6d70 6f72 7428 6461 7461  json_import(data
-00015610: 2e73 706c 6974 6c69 6e65 7328 292c 2073  .splitlines(), s
-00015620: 7472 6561 6d69 6e67 3d54 7275 652c 2074  treaming=True, t
-00015630: 7261 6e73 666f 726d 733d 7b27 6127 3a20  ransforms={'a': 
-00015640: 696e 742c 2027 6227 3a20 696e 742c 2027  int, 'b': int, '
-00015650: 6327 3a20 696e 747d 290a 0a20 2020 2020  c': int})..     
-00015660: 2020 2074 6573 745f 7369 7a65 203d 2033     test_size = 3
-00015670: 0a20 2020 2020 2020 2074 3120 3d20 6d61  .        t1 = ma
-00015680: 6b65 5f74 6573 745f 7461 626c 6528 7365  ke_test_table(se
-00015690: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
-000156a0: 6563 742c 2074 6573 745f 7369 7a65 290a  ect, test_size).
-000156b0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-000156c0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
-000156d0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000156e0: 7373 6572 7454 7275 6528 616c 6c28 6d61  ssertTrue(all(ma
-000156f0: 6b65 5f64 6174 616f 626a 6563 745f 6672  ke_dataobject_fr
-00015700: 6f6d 5f6f 6228 7265 6331 2920 3d3d 2072  om_ob(rec1) == r
-00015710: 6563 3220 666f 7220 7265 6331 2c20 7265  ec2 for rec1, re
-00015720: 6332 2069 6e20 7a69 7028 7431 2c20 6a73  c2 in zip(t1, js
-00015730: 6f6e 7461 626c 6529 2929 0a20 2020 2020  ontable))).     
-00015740: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-00015750: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
-00015760: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00015770: 7175 616c 286c 656e 285b 6420 666f 7220  qual(len([d for 
-00015780: 6420 696e 2064 6174 612e 7370 6c69 746c  d in data.splitl
-00015790: 696e 6573 2829 2069 6620 642e 7374 7269  ines() if d.stri
-000157a0: 7028 295d 292c 206c 656e 286a 736f 6e74  p()]), len(jsont
-000157b0: 6162 6c65 2929 0a0a 2020 2020 6465 6620  able))..    def 
-000157c0: 7465 7374 5f6a 736f 6e5f 6e6f 6e73 7472  test_json_nonstr
-000157d0: 6561 6d69 6e67 5f77 6974 685f 7061 7468  eaming_with_path
-000157e0: 5f69 6d70 6f72 7428 7365 6c66 293a 0a20  _import(self):. 
-000157f0: 2020 2020 2020 2064 6174 6120 3d20 6a73         data = js
-00015800: 6f6e 5f64 6174 610a 2020 2020 2020 2020  on_data.        
-00015810: 6461 7461 203d 2027 2c5c 6e27 2e6a 6f69  data = ',\n'.joi
-00015820: 6e28 6461 7461 2e72 7374 7269 7028 292e  n(data.rstrip().
-00015830: 7370 6c69 746c 696e 6573 2829 290a 2020  splitlines()).  
-00015840: 2020 2020 2020 6a73 6f6e 5f69 6e70 7574        json_input
-00015850: 3020 3d20 275b 2720 2b20 6461 7461 202b  0 = '[' + data +
-00015860: 2027 5d27 0a20 2020 2020 2020 206a 736f   ']'.        jso
-00015870: 6e5f 696e 7075 7431 203d 2027 7b20 2264  n_input1 = '{ "d
-00015880: 6174 6122 3a20 5b27 202b 2064 6174 6120  ata": [' + data 
-00015890: 2b20 275d 7d27 0a20 2020 2020 2020 206a  + ']}'.        j
-000158a0: 736f 6e5f 696e 7075 7432 203d 2027 7b20  son_input2 = '{ 
-000158b0: 2264 6174 6122 3a20 7b20 2269 7465 6d73  "data": { "items
-000158c0: 223a 205b 2720 2b20 6461 7461 202b 2027  ": [' + data + '
-000158d0: 5d7d 7d27 0a0a 2020 2020 2020 2020 666f  ]}}'..        fo
-000158e0: 7220 6a73 6f6e 5f69 6e70 7574 2c20 7061  r json_input, pa
-000158f0: 7468 2069 6e20 5b0a 2020 2020 2020 2020  th in [.        
-00015900: 2020 2020 286a 736f 6e5f 696e 7075 7430      (json_input0
-00015910: 2c20 2222 292c 0a20 2020 2020 2020 2020  , ""),.         
-00015920: 2020 2028 6a73 6f6e 5f69 6e70 7574 312c     (json_input1,
-00015930: 2022 6461 7461 2229 2c0a 2020 2020 2020   "data"),.      
-00015940: 2020 2020 2020 286a 736f 6e5f 696e 7075        (json_inpu
-00015950: 7432 2c20 2264 6174 612e 6974 656d 7322  t2, "data.items"
-00015960: 292c 0a20 2020 2020 2020 205d 3a0a 2020  ),.        ]:.  
-00015970: 2020 2020 2020 2020 2020 6a73 6f6e 7461            jsonta
-00015980: 626c 6520 3d20 6c74 2e54 6162 6c65 2829  ble = lt.Table()
-00015990: 2e6a 736f 6e5f 696d 706f 7274 286a 736f  .json_import(jso
-000159a0: 6e5f 696e 7075 742c 0a20 2020 2020 2020  n_input,.       
-000159b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000159c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000159d0: 2020 2020 2020 2020 7061 7468 3d70 6174          path=pat
-000159e0: 682c 0a20 2020 2020 2020 2020 2020 2020  h,.             
-000159f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a10: 2020 7472 616e 7366 6f72 6d73 3d7b 2761    transforms={'a
-00015a20: 273a 2069 6e74 2c20 2762 273a 2069 6e74  ': int, 'b': int
-00015a30: 2c20 2763 273a 2069 6e74 7d29 0a0a 2020  , 'c': int})..  
-00015a40: 2020 2020 2020 2020 2020 7465 7374 5f73            test_s
-00015a50: 697a 6520 3d20 330a 2020 2020 2020 2020  ize = 3.        
-00015a60: 2020 2020 7431 203d 206d 616b 655f 7465      t1 = make_te
-00015a70: 7374 5f74 6162 6c65 2873 656c 662e 6d61  st_table(self.ma
-00015a80: 6b65 5f64 6174 615f 6f62 6a65 6374 2c20  ke_data_object, 
-00015a90: 7465 7374 5f73 697a 6529 0a0a 2020 2020  test_size)..    
-00015aa0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00015ab0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-00015ac0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015ad0: 662e 6173 7365 7274 5472 7565 2861 6c6c  f.assertTrue(all
-00015ae0: 286d 616b 655f 6461 7461 6f62 6a65 6374  (make_dataobject
-00015af0: 5f66 726f 6d5f 6f62 2872 6563 3129 203d  _from_ob(rec1) =
-00015b00: 3d20 7265 6332 2066 6f72 2072 6563 312c  = rec2 for rec1,
-00015b10: 2072 6563 3220 696e 207a 6970 2874 312c   rec2 in zip(t1,
-00015b20: 206a 736f 6e74 6162 6c65 2929 290a 2020   jsontable))).  
-00015b30: 2020 2020 2020 2020 2020 7769 7468 2073            with s
-00015b40: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-00015b50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015b60: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00015b70: 6c65 6e28 5b64 2066 6f72 2064 2069 6e20  len([d for d in 
-00015b80: 6461 7461 2e73 706c 6974 6c69 6e65 7328  data.splitlines(
-00015b90: 2920 6966 2064 2e73 7472 6970 2829 5d29  ) if d.strip()])
-00015ba0: 2c20 6c65 6e28 6a73 6f6e 7461 626c 6529  , len(jsontable)
-00015bb0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00015bc0: 6a73 6f6e 5f69 6d70 6f72 745f 7769 7468  json_import_with
-00015bd0: 5f63 7573 746f 6d5f 656e 636f 6465 7228  _custom_encoder(
-00015be0: 7365 6c66 293a 0a20 2020 2020 2020 2066  self):.        f
-00015bf0: 726f 6d20 6461 7465 7469 6d65 2069 6d70  rom datetime imp
-00015c00: 6f72 7420 6461 7465 0a20 2020 2020 2020  ort date.       
-00015c10: 2064 6174 6120 3d20 5b0a 2020 2020 2020   data = [.      
-00015c20: 2020 2020 2020 7b27 6127 3a20 3130 302c        {'a': 100,
-00015c30: 2027 6227 3a20 6461 7465 2832 3030 302c   'b': date(2000,
-00015c40: 2031 2c20 3129 2c20 2763 273a 2032 3030   1, 1), 'c': 200
-00015c50: 7d2c 0a20 2020 2020 2020 2020 2020 207b  },.            {
-00015c60: 2761 273a 2031 3031 2c20 2762 273a 2064  'a': 101, 'b': d
-00015c70: 6174 6528 3230 3031 2c20 312c 2031 292c  ate(2001, 1, 1),
-00015c80: 2027 6327 3a20 3230 317d 2c0a 2020 2020   'c': 201},.    
-00015c90: 2020 2020 5d0a 2020 2020 2020 2020 7462      ].        tb
-00015ca0: 6c20 3d20 6c74 2e54 6162 6c65 2829 2e69  l = lt.Table().i
-00015cb0: 6e73 6572 745f 6d61 6e79 2864 6174 6129  nsert_many(data)
-00015cc0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00015cd0: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
-00015ce0: 5479 7065 4572 726f 7229 3a0a 2020 2020  TypeError):.    
-00015cf0: 2020 2020 2020 2020 7820 3d20 7462 6c2e          x = tbl.
-00015d00: 6a73 6f6e 5f65 7870 6f72 7428 290a 0a20  json_export().. 
-00015d10: 2020 2020 2020 2063 6c61 7373 204a 736f         class Jso
-00015d20: 6e44 6174 6545 6e63 6f64 6572 286a 736f  nDateEncoder(jso
-00015d30: 6e2e 4a53 4f4e 456e 636f 6465 7229 3a0a  n.JSONEncoder):.
-00015d40: 2020 2020 2020 2020 2020 2020 6465 6620              def 
-00015d50: 6465 6661 756c 7428 7365 6c66 2c20 6f29  default(self, o)
-00015d60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00015d70: 2020 696d 706f 7274 2064 6174 6574 696d    import datetim
-00015d80: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00015d90: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00015da0: 6f2c 2064 6174 6574 696d 652e 6461 7465  o, datetime.date
-00015db0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00015dc0: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
-00015dd0: 7228 6f29 0a20 2020 2020 2020 2020 2020  r(o).           
-00015de0: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-00015df0: 7228 292e 6465 6661 756c 7428 6f29 0a0a  r().default(o)..
-00015e00: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-00015e10: 203d 2074 6578 7477 7261 702e 6465 6465   = textwrap.dede
-00015e20: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
-00015e30: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
-00015e40: 2020 7b22 6122 3a20 3130 302c 2022 6222    {"a": 100, "b"
-00015e50: 3a20 2232 3030 302d 3031 2d30 3122 2c20  : "2000-01-01", 
-00015e60: 2263 223a 2032 3030 7d2c 0a20 2020 2020  "c": 200},.     
-00015e70: 2020 2020 2020 207b 2261 223a 2031 3031         {"a": 101
-00015e80: 2c20 2262 223a 2022 3230 3031 2d30 312d  , "b": "2001-01-
-00015e90: 3031 222c 2022 6322 3a20 3230 317d 0a20  01", "c": 201}. 
-00015ea0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-00015eb0: 2020 2020 2020 2020 2022 2222 290a 2020           """).  
-00015ec0: 2020 2020 2020 6a73 6f6e 5f72 6573 756c        json_resul
-00015ed0: 7420 3d20 7462 6c2e 6a73 6f6e 5f65 7870  t = tbl.json_exp
-00015ee0: 6f72 7428 6a73 6f6e 5f65 6e63 6f64 6572  ort(json_encoder
-00015ef0: 3d4a 736f 6e44 6174 6545 6e63 6f64 6572  =JsonDateEncoder
-00015f00: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00015f10: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
-00015f20: 7465 642c 206a 736f 6e5f 7265 7375 6c74  ted, json_result
-00015f30: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00015f40: 6a73 6f6e 5f69 6d70 6f72 745f 7769 7468  json_import_with
-00015f50: 5f6d 756c 7469 706c 655f 6375 7374 6f6d  _multiple_custom
-00015f60: 5f65 6e63 6f64 6572 7328 7365 6c66 293a  _encoders(self):
-00015f70: 0a20 2020 2020 2020 2066 726f 6d20 6461  .        from da
-00015f80: 7465 7469 6d65 2069 6d70 6f72 7420 6461  tetime import da
-00015f90: 7465 0a0a 2020 2020 2020 2020 636c 6173  te..        clas
-00015fa0: 7320 4141 413a 0a20 2020 2020 2020 2020  s AAA:.         
-00015fb0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00015fc0: 7365 6c66 2c20 6e61 6d65 293a 0a20 2020  self, name):.   
-00015fd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015fe0: 662e 6e61 6d65 203d 206e 616d 650a 0a20  f.name = name.. 
-00015ff0: 2020 2020 2020 2064 6174 6120 3d20 5b0a         data = [.
-00016000: 2020 2020 2020 2020 2020 2020 7b27 6127              {'a'
-00016010: 3a20 3130 302c 2027 6227 3a20 6461 7465  : 100, 'b': date
-00016020: 2832 3030 302c 2031 2c20 3129 2c20 2763  (2000, 1, 1), 'c
-00016030: 273a 2032 3030 2c20 2764 273a 2041 4141  ': 200, 'd': AAA
-00016040: 2822 416c 6963 6522 297d 2c0a 2020 2020  ("Alice")},.    
-00016050: 2020 2020 2020 2020 7b27 6127 3a20 3130          {'a': 10
-00016060: 312c 2027 6227 3a20 6461 7465 2832 3030  1, 'b': date(200
-00016070: 312c 2031 2c20 3129 2c20 2763 273a 2032  1, 1, 1), 'c': 2
-00016080: 3031 2c20 2764 273a 2041 4141 2822 426f  01, 'd': AAA("Bo
-00016090: 6222 297d 2c0a 2020 2020 2020 2020 5d0a  b")},.        ].
-000160a0: 2020 2020 2020 2020 7462 6c20 3d20 6c74          tbl = lt
-000160b0: 2e54 6162 6c65 2829 2e69 6e73 6572 745f  .Table().insert_
-000160c0: 6d61 6e79 2864 6174 6129 0a20 2020 2020  many(data).     
-000160d0: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
-000160e0: 6572 7452 6169 7365 7328 5479 7065 4572  ertRaises(TypeEr
-000160f0: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
-00016100: 2020 7820 3d20 7462 6c2e 6a73 6f6e 5f65    x = tbl.json_e
-00016110: 7870 6f72 7428 290a 0a20 2020 2020 2020  xport()..       
-00016120: 2063 6c61 7373 204a 736f 6e44 6174 6545   class JsonDateE
-00016130: 6e63 6f64 6572 286a 736f 6e2e 4a53 4f4e  ncoder(json.JSON
-00016140: 456e 636f 6465 7229 3a0a 2020 2020 2020  Encoder):.      
-00016150: 2020 2020 2020 6465 6620 6465 6661 756c        def defaul
-00016160: 7428 7365 6c66 2c20 6f29 3a0a 2020 2020  t(self, o):.    
-00016170: 2020 2020 2020 2020 2020 2020 696d 706f              impo
-00016180: 7274 2064 6174 6574 696d 650a 2020 2020  rt datetime.    
-00016190: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-000161a0: 7369 6e73 7461 6e63 6528 6f2c 2064 6174  sinstance(o, dat
-000161b0: 6574 696d 652e 6461 7465 293a 0a20 2020  etime.date):.   
-000161c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161d0: 2072 6574 7572 6e20 7374 7228 6f29 0a20   return str(o). 
-000161e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000161f0: 6574 7572 6e20 7375 7065 7228 292e 6465  eturn super().de
-00016200: 6661 756c 7428 6f29 0a0a 2020 2020 2020  fault(o)..      
-00016210: 2020 636c 6173 7320 4a73 6f6e 4141 4145    class JsonAAAE
-00016220: 6e63 6f64 6572 286a 736f 6e2e 4a53 4f4e  ncoder(json.JSON
-00016230: 456e 636f 6465 7229 3a0a 2020 2020 2020  Encoder):.      
-00016240: 2020 2020 2020 6465 6620 6465 6661 756c        def defaul
-00016250: 7428 7365 6c66 2c20 6f29 3a0a 2020 2020  t(self, o):.    
-00016260: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00016270: 7369 6e73 7461 6e63 6528 6f2c 2041 4141  sinstance(o, AAA
-00016280: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00016290: 2020 2020 2020 2072 6574 7572 6e20 6622         return f"
-000162a0: 4141 4128 6e61 6d65 3d7b 6f2e 6e61 6d65  AAA(name={o.name
-000162b0: 2172 7d29 220a 0a20 2020 2020 2020 2065  !r})"..        e
-000162c0: 7870 6563 7465 6420 3d20 7465 7874 7772  xpected = textwr
-000162d0: 6170 2e64 6564 656e 7428 2222 225c 0a20  ap.dedent("""\. 
-000162e0: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
-000162f0: 2020 2020 2020 2020 207b 2261 223a 2031           {"a": 1
-00016300: 3030 2c20 2262 223a 2022 3230 3030 2d30  00, "b": "2000-0
-00016310: 312d 3031 222c 2022 6322 3a20 3230 302c  1-01", "c": 200,
-00016320: 2022 6422 3a20 2241 4141 286e 616d 653d   "d": "AAA(name=
-00016330: 2741 6c69 6365 2729 227d 2c0a 2020 2020  'Alice')"},.    
-00016340: 2020 2020 2020 2020 7b22 6122 3a20 3130          {"a": 10
-00016350: 312c 2022 6222 3a20 2232 3030 312d 3031  1, "b": "2001-01
-00016360: 2d30 3122 2c20 2263 223a 2032 3031 2c20  -01", "c": 201, 
-00016370: 2264 223a 2022 4141 4128 6e61 6d65 3d27  "d": "AAA(name='
-00016380: 426f 6227 2922 7d0a 2020 2020 2020 2020  Bob')"}.        
-00016390: 2020 2020 5d0a 2020 2020 2020 2020 2222      ].        ""
-000163a0: 2229 0a0a 2020 2020 2020 2020 6a73 6f6e  ")..        json
-000163b0: 5f72 6573 756c 7420 3d20 7462 6c2e 6a73  _result = tbl.js
-000163c0: 6f6e 5f65 7870 6f72 7428 6a73 6f6e 5f65  on_export(json_e
-000163d0: 6e63 6f64 6572 3d28 4a73 6f6e 4461 7465  ncoder=(JsonDate
-000163e0: 456e 636f 6465 722c 204a 736f 6e41 4141  Encoder, JsonAAA
-000163f0: 456e 636f 6465 7229 290a 2020 2020 2020  Encoder)).      
-00016400: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00016410: 616c 2865 7870 6563 7465 642c 206a 736f  al(expected, jso
-00016420: 6e5f 7265 7375 6c74 290a 0a20 2020 2064  n_result)..    d
-00016430: 6566 2074 6573 745f 6669 7865 645f 7769  ef test_fixed_wi
-00016440: 6474 685f 696d 706f 7274 2873 656c 6629  dth_import(self)
-00016450: 3a0a 2020 2020 2020 2020 6461 7461 203d  :.        data =
-00016460: 2066 6978 6564 5f77 6964 7468 5f64 6174   fixed_width_dat
-00016470: 610a 2020 2020 2020 2020 6461 7461 5f66  a.        data_f
-00016480: 696c 6520 3d20 696f 2e53 7472 696e 6749  ile = io.StringI
-00016490: 4f28 6461 7461 290a 2020 2020 2020 2020  O(data).        
-000164a0: 6677 5f73 7065 6320 3d20 5b28 2761 272c  fw_spec = [('a',
-000164b0: 2030 2c20 4e6f 6e65 2c20 696e 7429 2c20   0, None, int), 
-000164c0: 2827 6227 2c20 322c 204e 6f6e 652c 2069  ('b', 2, None, i
-000164d0: 6e74 292c 2028 2763 272c 2034 2c20 4e6f  nt), ('c', 4, No
-000164e0: 6e65 2c20 696e 7429 2c20 5d0a 2020 2020  ne, int), ].    
-000164f0: 2020 2020 7474 203d 206c 742e 5461 626c      tt = lt.Tabl
-00016500: 6528 292e 696e 7365 7274 5f6d 616e 7928  e().insert_many(
-00016510: 6c74 2e44 6174 614f 626a 6563 7428 2a2a  lt.DataObject(**
-00016520: 7265 6329 2066 6f72 2072 6563 2069 6e20  rec) for rec in 
-00016530: 6c74 2e46 6978 6564 5769 6474 6852 6561  lt.FixedWidthRea
-00016540: 6465 7228 6677 5f73 7065 632c 2064 6174  der(fw_spec, dat
-00016550: 615f 6669 6c65 2929 0a0a 2020 2020 2020  a_file))..      
-00016560: 2020 7465 7374 5f73 697a 6520 3d20 330a    test_size = 3.
-00016570: 2020 2020 2020 2020 7431 203d 206d 616b          t1 = mak
-00016580: 655f 7465 7374 5f74 6162 6c65 2873 656c  e_test_table(sel
-00016590: 662e 6d61 6b65 5f64 6174 615f 6f62 6a65  f.make_data_obje
-000165a0: 6374 2c20 7465 7374 5f73 697a 6529 0a0a  ct, test_size)..
-000165b0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-000165c0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-000165d0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-000165e0: 7365 7274 5472 7565 2861 6c6c 286d 616b  sertTrue(all(mak
-000165f0: 655f 6461 7461 6f62 6a65 6374 5f66 726f  e_dataobject_fro
-00016600: 6d5f 6f62 2872 6563 3129 203d 3d20 7265  m_ob(rec1) == re
-00016610: 6332 2066 6f72 2072 6563 312c 2072 6563  c2 for rec1, rec
-00016620: 3220 696e 207a 6970 2874 312c 2074 7429  2 in zip(t1, tt)
-00016630: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
-00016640: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
-00016650: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016660: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
-00016670: 285b 6420 666f 7220 6420 696e 2064 6174  ([d for d in dat
-00016680: 612e 7370 6c69 746c 696e 6573 2829 2069  a.splitlines() i
-00016690: 6620 642e 7374 7269 7028 295d 292c 206c  f d.strip()]), l
-000166a0: 656e 2874 7429 290a 0a20 2020 2064 6566  en(tt))..    def
-000166b0: 2074 6573 745f 6669 7865 645f 7769 6474   test_fixed_widt
-000166c0: 685f 7374 7269 6e67 5f69 6d70 6f72 7428  h_string_import(
-000166d0: 7365 6c66 293a 0a20 2020 2020 2020 2064  self):.        d
-000166e0: 6174 6120 3d20 6669 7865 645f 7769 6474  ata = fixed_widt
-000166f0: 685f 6461 7461 0a20 2020 2020 2020 2066  h_data.        f
-00016700: 775f 7370 6563 203d 205b 2827 6127 2c20  w_spec = [('a', 
-00016710: 302c 204e 6f6e 652c 2069 6e74 292c 2028  0, None, int), (
-00016720: 2762 272c 2032 2c20 4e6f 6e65 2c20 696e  'b', 2, None, in
-00016730: 7429 2c20 2827 6327 2c20 342c 204e 6f6e  t), ('c', 4, Non
-00016740: 652c 2069 6e74 292c 205d 0a20 2020 2020  e, int), ].     
-00016750: 2020 2074 7420 3d20 6c74 2e54 6162 6c65     tt = lt.Table
-00016760: 2829 2e69 6e73 6572 745f 6d61 6e79 286c  ().insert_many(l
-00016770: 742e 4461 7461 4f62 6a65 6374 282a 2a72  t.DataObject(**r
-00016780: 6563 2920 666f 7220 7265 6320 696e 206c  ec) for rec in l
-00016790: 742e 4669 7865 6457 6964 7468 5265 6164  t.FixedWidthRead
-000167a0: 6572 2866 775f 7370 6563 2c20 6461 7461  er(fw_spec, data
-000167b0: 2929 0a0a 2020 2020 2020 2020 7465 7374  ))..        test
-000167c0: 5f73 697a 6520 3d20 330a 2020 2020 2020  _size = 3.      
-000167d0: 2020 7431 203d 206d 616b 655f 7465 7374    t1 = make_test
-000167e0: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
-000167f0: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
-00016800: 7374 5f73 697a 6529 0a0a 2020 2020 2020  st_size)..      
-00016810: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-00016820: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-00016830: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-00016840: 7565 2861 6c6c 286d 616b 655f 6461 7461  ue(all(make_data
-00016850: 6f62 6a65 6374 5f66 726f 6d5f 6f62 2872  object_from_ob(r
-00016860: 6563 3129 203d 3d20 7265 6332 2066 6f72  ec1) == rec2 for
-00016870: 2072 6563 312c 2072 6563 3220 696e 207a   rec1, rec2 in z
-00016880: 6970 2874 312c 2074 7429 2929 0a20 2020  ip(t1, tt))).   
-00016890: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
-000168a0: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
-000168b0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-000168c0: 7445 7175 616c 286c 656e 285b 6420 666f  tEqual(len([d fo
-000168d0: 7220 6420 696e 2064 6174 612e 7370 6c69  r d in data.spli
-000168e0: 746c 696e 6573 2829 2069 6620 642e 7374  tlines() if d.st
-000168f0: 7269 7028 295d 292c 206c 656e 2874 7429  rip()]), len(tt)
-00016900: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00016910: 6669 7865 645f 7769 6474 685f 7374 7269  fixed_width_stri
-00016920: 6e67 5f6c 6973 745f 696d 706f 7274 2873  ng_list_import(s
-00016930: 656c 6629 3a0a 2020 2020 2020 2020 6461  elf):.        da
-00016940: 7461 203d 2066 6978 6564 5f77 6964 7468  ta = fixed_width
-00016950: 5f64 6174 610a 2020 2020 2020 2020 6677  _data.        fw
-00016960: 5f73 7065 6320 3d20 5b28 2761 272c 2030  _spec = [('a', 0
-00016970: 2c20 4e6f 6e65 2c20 696e 7429 2c20 2827  , None, int), ('
-00016980: 6227 2c20 322c 204e 6f6e 652c 2069 6e74  b', 2, None, int
-00016990: 292c 2028 2763 272c 2034 2c20 4e6f 6e65  ), ('c', 4, None
-000169a0: 2c20 696e 7429 2c5d 0a20 2020 2020 2020  , int),].       
-000169b0: 2074 7420 3d20 6c74 2e54 6162 6c65 2829   tt = lt.Table()
-000169c0: 2e69 6e73 6572 745f 6d61 6e79 286c 742e  .insert_many(lt.
-000169d0: 4461 7461 4f62 6a65 6374 282a 2a72 6563  DataObject(**rec
-000169e0: 2920 666f 7220 7265 6320 696e 206c 742e  ) for rec in lt.
-000169f0: 4669 7865 6457 6964 7468 5265 6164 6572  FixedWidthReader
-00016a00: 2866 775f 7370 6563 2c20 6461 7461 2e73  (fw_spec, data.s
-00016a10: 706c 6974 6c69 6e65 7328 2929 290a 0a20  plitlines())).. 
-00016a20: 2020 2020 2020 2074 6573 745f 7369 7a65         test_size
-00016a30: 203d 2033 0a20 2020 2020 2020 2074 3120   = 3.        t1 
-00016a40: 3d20 6d61 6b65 5f74 6573 745f 7461 626c  = make_test_tabl
-00016a50: 6528 7365 6c66 2e6d 616b 655f 6461 7461  e(self.make_data
-00016a60: 5f6f 626a 6563 742c 2074 6573 745f 7369  _object, test_si
-00016a70: 7a65 290a 0a20 2020 2020 2020 2077 6974  ze)..        wit
-00016a80: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
-00016a90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00016aa0: 6c66 2e61 7373 6572 7454 7275 6528 616c  lf.assertTrue(al
-00016ab0: 6c28 6d61 6b65 5f64 6174 616f 626a 6563  l(make_dataobjec
-00016ac0: 745f 6672 6f6d 5f6f 6228 7265 6331 2920  t_from_ob(rec1) 
-00016ad0: 3d3d 2072 6563 3220 666f 7220 7265 6331  == rec2 for rec1
-00016ae0: 2c20 7265 6332 2069 6e20 7a69 7028 7431  , rec2 in zip(t1
-00016af0: 2c20 7474 2929 290a 2020 2020 2020 2020  , tt))).        
-00016b00: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-00016b10: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-00016b20: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00016b30: 6c28 6c65 6e28 5b64 2066 6f72 2064 2069  l(len([d for d i
-00016b40: 6e20 6461 7461 2e73 706c 6974 6c69 6e65  n data.splitline
-00016b50: 7328 2920 6966 2064 2e73 7472 6970 2829  s() if d.strip()
-00016b60: 5d29 2c20 6c65 6e28 7474 2929 0a0a 2020  ]), len(tt))..  
-00016b70: 2020 6465 6620 7465 7374 5f65 7863 656c    def test_excel
-00016b80: 5f69 6d70 6f72 7428 7365 6c66 293a 0a20  _import(self):. 
-00016b90: 2020 2020 2020 2066 696c 655f 6e61 6d65         file_name
-00016ba0: 203d 2022 7465 7374 2f61 6263 2e78 6c73   = "test/abc.xls
-00016bb0: 7822 0a20 2020 2020 2020 2065 7863 656c  x".        excel
-00016bc0: 5f74 6162 6c65 203d 206c 742e 5461 626c  _table = lt.Tabl
-00016bd0: 6528 292e 6578 6365 6c5f 696d 706f 7274  e().excel_import
-00016be0: 2866 696c 655f 6e61 6d65 2c20 7472 616e  (file_name, tran
-00016bf0: 7366 6f72 6d73 3d7b 2761 273a 2069 6e74  sforms={'a': int
-00016c00: 2c20 2762 273a 2069 6e74 2c20 2763 273a  , 'b': int, 'c':
-00016c10: 2069 6e74 7d29 0a0a 2020 2020 2020 2020   int})..        
-00016c20: 7465 7374 5f73 697a 6520 3d20 330a 2020  test_size = 3.  
-00016c30: 2020 2020 2020 7431 203d 206d 616b 655f        t1 = make_
-00016c40: 7465 7374 5f74 6162 6c65 2873 656c 662e  test_table(self.
-00016c50: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
-00016c60: 2c20 7465 7374 5f73 697a 6529 0a0a 2020  , test_size)..  
-00016c70: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00016c80: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-00016c90: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00016ca0: 7274 5472 7565 2861 6c6c 286d 616b 655f  rtTrue(all(make_
-00016cb0: 6461 7461 6f62 6a65 6374 5f66 726f 6d5f  dataobject_from_
-00016cc0: 6f62 2872 6563 3129 203d 3d20 7265 6332  ob(rec1) == rec2
-00016cd0: 2066 6f72 2072 6563 312c 2072 6563 3220   for rec1, rec2 
-00016ce0: 696e 207a 6970 2874 312c 2065 7863 656c  in zip(t1, excel
-00016cf0: 5f74 6162 6c65 2929 290a 2020 2020 2020  _table))).      
-00016d00: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-00016d10: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-00016d20: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00016d30: 7561 6c28 7375 6d28 3120 666f 7220 6c69  ual(sum(1 for li
-00016d40: 6e65 2069 6e20 6373 765f 6461 7461 2e73  ne in csv_data.s
-00016d50: 706c 6974 6c69 6e65 7328 2920 6966 206c  plitlines() if l
-00016d60: 696e 652e 7374 7269 7028 2929 2d31 2c20  ine.strip())-1, 
-00016d70: 6c65 6e28 6578 6365 6c5f 7461 626c 6529  len(excel_table)
-00016d80: 290a 0a20 2020 2020 2020 2072 6f77 5f70  )..        row_p
-00016d90: 726f 746f 7479 7065 203d 2073 656c 662e  rototype = self.
-00016da0: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
-00016db0: 2830 2c20 302c 2030 290a 2020 2020 2020  (0, 0, 0).      
-00016dc0: 2020 6373 7674 6162 6c65 3220 3d20 6c74    csvtable2 = lt
-00016dd0: 2e54 6162 6c65 2829 2e65 7863 656c 5f69  .Table().excel_i
-00016de0: 6d70 6f72 7428 0a20 2020 2020 2020 2020  mport(.         
-00016df0: 2020 2066 696c 655f 6e61 6d65 2c20 7472     file_name, tr
-00016e00: 616e 7366 6f72 6d73 3d7b 2761 273a 2069  ansforms={'a': i
-00016e10: 6e74 2c20 2762 273a 2069 6e74 2c20 2763  nt, 'b': int, 'c
-00016e20: 273a 2069 6e74 7d2c 2072 6f77 5f63 6c61  ': int}, row_cla
-00016e30: 7373 3d74 7970 6528 726f 775f 7072 6f74  ss=type(row_prot
-00016e40: 6f74 7970 6529 0a20 2020 2020 2020 2029  otype).        )
-00016e50: 5b3a 335d 0a0a 2020 2020 2020 2020 7072  [:3]..        pr
-00016e60: 696e 7428 7479 7065 2874 315b 305d 292e  int(type(t1[0]).
-00016e70: 5f5f 6e61 6d65 5f5f 2c20 7431 5b30 5d29  __name__, t1[0])
-00016e80: 0a20 2020 2020 2020 2070 7269 6e74 2874  .        print(t
-00016e90: 7970 6528 6373 7674 6162 6c65 325b 305d  ype(csvtable2[0]
-00016ea0: 292e 5f5f 6e61 6d65 5f5f 2c20 6373 7674  ).__name__, csvt
-00016eb0: 6162 6c65 325b 305d 290a 2020 2020 2020  able2[0]).      
-00016ec0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-00016ed0: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-00016ee0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00016ef0: 7561 6c28 7479 7065 2874 315b 305d 292c  ual(type(t1[0]),
-00016f00: 2074 7970 6528 6373 7674 6162 6c65 325b   type(csvtable2[
-00016f10: 305d 2929 0a0a 2020 2020 6465 6620 7465  0]))..    def te
-00016f20: 7374 5f65 7863 656c 5f65 7870 6f72 7428  st_excel_export(
-00016f30: 7365 6c66 293a 0a20 2020 2020 2020 2066  self):.        f
-00016f40: 696c 655f 6e61 6d65 203d 2022 7465 7374  ile_name = "test
-00016f50: 2f61 6263 2e78 6c73 7822 0a20 2020 2020  /abc.xlsx".     
-00016f60: 2020 2065 7863 656c 5f74 6162 6c65 203d     excel_table =
-00016f70: 206c 742e 5461 626c 6528 292e 6578 6365   lt.Table().exce
-00016f80: 6c5f 696d 706f 7274 2866 696c 655f 6e61  l_import(file_na
-00016f90: 6d65 2c20 7472 616e 7366 6f72 6d73 3d7b  me, transforms={
-00016fa0: 2761 273a 2069 6e74 2c20 2762 273a 2069  'a': int, 'b': i
-00016fb0: 6e74 2c20 2763 273a 2069 6e74 7d2c 206c  nt, 'c': int}, l
-00016fc0: 696d 6974 3d31 290a 2020 2020 2020 2020  imit=1).        
-00016fd0: 6f75 7466 696c 6520 3d20 696f 2e42 7974  outfile = io.Byt
-00016fe0: 6573 494f 2829 0a20 2020 2020 2020 2065  esIO().        e
-00016ff0: 7863 656c 5f74 6162 6c65 2e65 7863 656c  xcel_table.excel
-00017000: 5f65 7870 6f72 7428 6f75 7466 696c 6529  _export(outfile)
-00017010: 0a20 2020 2020 2020 2065 7870 6f72 7465  .        exporte
-00017020: 645f 7461 626c 6520 3d20 6c74 2e54 6162  d_table = lt.Tab
-00017030: 6c65 2829 2e65 7863 656c 5f69 6d70 6f72  le().excel_impor
-00017040: 7428 6f75 7466 696c 652c 2074 7261 6e73  t(outfile, trans
-00017050: 666f 726d 733d 7b27 6127 3a20 696e 742c  forms={'a': int,
-00017060: 2027 6227 3a20 696e 742c 2027 6327 3a20   'b': int, 'c': 
-00017070: 696e 747d 290a 0a20 2020 2020 2020 2077  int})..        w
-00017080: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
-00017090: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000170a0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-000170b0: 616c 6c28 6d61 6b65 5f64 6174 616f 626a  all(make_dataobj
-000170c0: 6563 745f 6672 6f6d 5f6f 6228 7265 6331  ect_from_ob(rec1
-000170d0: 2920 3d3d 2072 6563 3220 666f 7220 7265  ) == rec2 for re
-000170e0: 6331 2c20 7265 6332 2069 6e20 7a69 7028  c1, rec2 in zip(
-000170f0: 6578 706f 7274 6564 5f74 6162 6c65 2c20  exported_table, 
-00017100: 6578 6365 6c5f 7461 626c 6529 2929 0a0a  excel_table)))..
-00017110: 2020 2020 6465 6620 7465 7374 5f6d 6f64      def test_mod
-00017120: 756c 655f 6c65 7665 6c5f 6373 765f 696d  ule_level_csv_im
-00017130: 706f 7274 6572 2873 656c 6629 3a0a 2020  porter(self):.  
-00017140: 2020 2020 2020 6461 7461 203d 2063 7376        data = csv
-00017150: 5f64 6174 610a 2020 2020 2020 2020 6373  _data.        cs
-00017160: 7674 6162 6c65 203d 206c 742e 6373 765f  vtable = lt.csv_
-00017170: 696d 706f 7274 2863 7376 5f73 6f75 7263  import(csv_sourc
-00017180: 653d 6461 7461 2c20 7472 616e 7366 6f72  e=data, transfor
-00017190: 6d73 3d7b 2761 273a 2069 6e74 2c20 2762  ms={'a': int, 'b
-000171a0: 273a 2069 6e74 2c20 2763 273a 2069 6e74  ': int, 'c': int
-000171b0: 7d29 0a0a 2020 2020 2020 2020 7465 7374  })..        test
-000171c0: 5f73 697a 6520 3d20 330a 2020 2020 2020  _size = 3.      
-000171d0: 2020 7431 203d 206d 616b 655f 7465 7374    t1 = make_test
-000171e0: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
-000171f0: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
-00017200: 7374 5f73 697a 6529 0a0a 2020 2020 2020  st_size)..      
-00017210: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
-00017220: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
-00017230: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-00017240: 7565 2861 6c6c 286d 616b 655f 6461 7461  ue(all(make_data
-00017250: 6f62 6a65 6374 5f66 726f 6d5f 6f62 2872  object_from_ob(r
-00017260: 6563 3129 203d 3d20 7265 6332 2066 6f72  ec1) == rec2 for
-00017270: 2072 6563 312c 2072 6563 3220 696e 207a   rec1, rec2 in z
-00017280: 6970 2874 312c 2063 7376 7461 626c 6529  ip(t1, csvtable)
-00017290: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
-000172a0: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
-000172b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000172c0: 2e61 7373 6572 7445 7175 616c 2873 756d  .assertEqual(sum
-000172d0: 2831 2066 6f72 206c 696e 6520 696e 2064  (1 for line in d
-000172e0: 6174 612e 7370 6c69 746c 696e 6573 2829  ata.splitlines()
-000172f0: 2069 6620 6c69 6e65 2e73 7472 6970 2829   if line.strip()
-00017300: 292d 312c 206c 656e 2863 7376 7461 626c  )-1, len(csvtabl
-00017310: 6529 290a 0a20 2020 2064 6566 2074 6573  e))..    def tes
-00017320: 745f 6d6f 6475 6c65 5f6c 6576 656c 5f6a  t_module_level_j
-00017330: 736f 6e5f 696d 706f 7274 6572 2873 656c  son_importer(sel
-00017340: 6629 3a0a 2020 2020 2020 2020 6461 7461  f):.        data
-00017350: 203d 206a 736f 6e5f 6461 7461 0a20 2020   = json_data.   
-00017360: 2020 2020 206a 736f 6e74 6162 6c65 203d       jsontable =
-00017370: 206c 742e 6a73 6f6e 5f69 6d70 6f72 7428   lt.json_import(
-00017380: 6461 7461 2c20 7374 7265 616d 696e 673d  data, streaming=
-00017390: 5472 7565 2c20 7472 616e 7366 6f72 6d73  True, transforms
-000173a0: 3d7b 2761 273a 2069 6e74 2c20 2762 273a  ={'a': int, 'b':
-000173b0: 2069 6e74 2c20 2763 273a 2069 6e74 7d29   int, 'c': int})
-000173c0: 0a0a 2020 2020 2020 2020 7465 7374 5f73  ..        test_s
-000173d0: 697a 6520 3d20 330a 2020 2020 2020 2020  ize = 3.        
-000173e0: 7431 203d 206d 616b 655f 7465 7374 5f74  t1 = make_test_t
-000173f0: 6162 6c65 2873 656c 662e 6d61 6b65 5f64  able(self.make_d
-00017400: 6174 615f 6f62 6a65 6374 2c20 7465 7374  ata_object, test
-00017410: 5f73 697a 6529 0a0a 2020 2020 2020 2020  _size)..        
-00017420: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
-00017430: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-00017440: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
-00017450: 2861 6c6c 286d 616b 655f 6461 7461 6f62  (all(make_dataob
-00017460: 6a65 6374 5f66 726f 6d5f 6f62 2872 6563  ject_from_ob(rec
-00017470: 3129 203d 3d20 7265 6332 2066 6f72 2072  1) == rec2 for r
-00017480: 6563 312c 2072 6563 3220 696e 207a 6970  ec1, rec2 in zip
-00017490: 2874 312c 206a 736f 6e74 6162 6c65 2929  (t1, jsontable))
-000174a0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
-000174b0: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
-000174c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000174d0: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
-000174e0: 5b64 2066 6f72 2064 2069 6e20 6461 7461  [d for d in data
-000174f0: 2e73 706c 6974 6c69 6e65 7328 2920 6966  .splitlines() if
-00017500: 2064 2e73 7472 6970 2829 5d29 2c20 6c65   d.strip()]), le
-00017510: 6e28 6a73 6f6e 7461 626c 6529 290a 0a20  n(jsontable)).. 
-00017520: 2020 2064 6566 2074 6573 745f 6d6f 6475     def test_modu
-00017530: 6c65 5f6c 6576 656c 5f65 7863 656c 5f69  le_level_excel_i
-00017540: 6d70 6f72 7428 7365 6c66 293a 0a20 2020  mport(self):.   
-00017550: 2020 2020 2066 696c 655f 6e61 6d65 203d       file_name =
-00017560: 2022 7465 7374 2f61 6263 2e78 6c73 7822   "test/abc.xlsx"
-00017570: 0a20 2020 2020 2020 2065 7863 656c 5f74  .        excel_t
-00017580: 6162 6c65 203d 206c 742e 6578 6365 6c5f  able = lt.excel_
-00017590: 696d 706f 7274 2866 696c 655f 6e61 6d65  import(file_name
-000175a0: 2c20 7472 616e 7366 6f72 6d73 3d7b 2761  , transforms={'a
-000175b0: 273a 2069 6e74 2c20 2762 273a 2069 6e74  ': int, 'b': int
-000175c0: 2c20 2763 273a 2069 6e74 7d29 0a0a 2020  , 'c': int})..  
-000175d0: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
-000175e0: 3d20 330a 2020 2020 2020 2020 7431 203d  = 3.        t1 =
-000175f0: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
-00017600: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
-00017610: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
-00017620: 6529 0a0a 2020 2020 2020 2020 7769 7468  e)..        with
-00017630: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
-00017640: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00017650: 662e 6173 7365 7274 5472 7565 2861 6c6c  f.assertTrue(all
-00017660: 286d 616b 655f 6461 7461 6f62 6a65 6374  (make_dataobject
-00017670: 5f66 726f 6d5f 6f62 2872 6563 3129 203d  _from_ob(rec1) =
-00017680: 3d20 7265 6332 2066 6f72 2072 6563 312c  = rec2 for rec1,
-00017690: 2072 6563 3220 696e 207a 6970 2874 312c   rec2 in zip(t1,
-000176a0: 2065 7863 656c 5f74 6162 6c65 2929 290a   excel_table))).
-000176b0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-000176c0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
-000176d0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-000176e0: 7365 7274 4571 7561 6c28 7375 6d28 3120  sertEqual(sum(1 
-000176f0: 666f 7220 6c69 6e65 2069 6e20 6373 765f  for line in csv_
-00017700: 6461 7461 2e73 706c 6974 6c69 6e65 7328  data.splitlines(
-00017710: 2920 6966 206c 696e 652e 7374 7269 7028  ) if line.strip(
-00017720: 2929 2d31 2c20 6c65 6e28 6578 6365 6c5f  ))-1, len(excel_
-00017730: 7461 626c 6529 290a 0a0a 406d 616b 655f  table))...@make_
-00017740: 7465 7374 5f63 6c61 7373 6573 0a63 6c61  test_classes.cla
-00017750: 7373 2054 6162 6c65 5069 766f 7454 6573  ss TablePivotTes
-00017760: 7473 3a0a 2020 2020 6465 6620 7465 7374  ts:.    def test
-00017770: 5f70 6976 6f74 2873 656c 6629 3a0a 2020  _pivot(self):.  
-00017780: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
-00017790: 3d20 350a 2020 2020 2020 2020 7431 203d  = 5.        t1 =
-000177a0: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
-000177b0: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
-000177c0: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
-000177d0: 6529 0a20 2020 2020 2020 2074 312e 6372  e).        t1.cr
-000177e0: 6561 7465 5f69 6e64 6578 2827 6127 290a  eate_index('a').
-000177f0: 2020 2020 2020 2020 7431 2e63 7265 6174          t1.creat
-00017800: 655f 696e 6465 7828 2762 2729 0a20 2020  e_index('b').   
-00017810: 2020 2020 2074 3170 6976 6f74 203d 2074       t1pivot = t
-00017820: 312e 7069 766f 7428 2761 2729 0a20 2020  1.pivot('a').   
-00017830: 2020 2020 2074 3170 6976 6f74 2e64 756d       t1pivot.dum
-00017840: 7028 290a 2020 2020 2020 2020 7431 7069  p().        t1pi
-00017850: 766f 742e 6475 6d70 5f63 6f75 6e74 7328  vot.dump_counts(
-00017860: 290a 2020 2020 2020 2020 7431 7069 766f  ).        t1pivo
-00017870: 742e 7375 6d6d 6172 795f 636f 756e 7473  t.summary_counts
-00017880: 2829 0a0a 2020 2020 2020 2020 7432 7069  ()..        t2pi
-00017890: 766f 7420 3d20 7431 2e70 6976 6f74 2827  vot = t1.pivot('
-000178a0: 6120 6227 290a 2020 2020 2020 2020 7432  a b').        t2
-000178b0: 7069 766f 742e 6475 6d70 2829 0a20 2020  pivot.dump().   
-000178c0: 2020 2020 2074 3270 6976 6f74 2e64 756d       t2pivot.dum
-000178d0: 705f 636f 756e 7473 2829 0a20 2020 2020  p_counts().     
-000178e0: 2020 2074 3270 6976 6f74 2e73 756d 6d61     t2pivot.summa
-000178f0: 7279 5f63 6f75 6e74 7328 290a 0a20 2020  ry_counts()..   
-00017900: 2020 2020 2023 2054 4f44 4f20 2d20 6164       # TODO - ad
-00017910: 6420 6173 7365 7274 730a 0a0a 636c 6173  d asserts...clas
-00017920: 7320 5461 626c 6553 6561 7263 6854 6573  s TableSearchTes
-00017930: 7473 2875 6e69 7474 6573 742e 5465 7374  ts(unittest.Test
-00017940: 4361 7365 293a 0a20 2020 2072 6563 6970  Case):.    recip
-00017950: 655f 6461 7461 203d 2074 6578 7477 7261  e_data = textwra
-00017960: 702e 6465 6465 6e74 2822 2222 5c0a 2020  p.dedent("""\.  
-00017970: 2020 2020 2020 6964 2c74 6974 6c65 2c69        id,title,i
-00017980: 6e67 7265 6469 656e 7473 0a20 2020 2020  ngredients.     
-00017990: 2020 2031 2c54 756e 6120 6361 7373 6572     1,Tuna casser
-000179a0: 6f6c 652c 2274 756e 612c 206e 6f6f 646c  ole,"tuna, noodl
-000179b0: 6573 2c20 4372 6561 6d20 6f66 204d 7573  es, Cream of Mus
-000179c0: 6872 6f6f 6d20 536f 7570 220a 2020 2020  hroom Soup".    
-000179d0: 2020 2020 322c 4861 7761 6969 616e 2070      2,Hawaiian p
-000179e0: 697a 7a61 2c70 697a 7a61 2064 6f75 6768  izza,pizza dough
-000179f0: 2070 696e 6561 7070 6c65 2068 616d 2074   pineapple ham t
-00017a00: 6f6d 6174 6f20 7361 7563 650a 2020 2020  omato sauce.    
-00017a10: 2020 2020 332c 4d61 7267 6865 7269 7461      3,Margherita
-00017a20: 2070 697a 7a61 2c70 697a 7a61 2064 6f75   pizza,pizza dou
-00017a30: 6768 2063 6865 6573 6520 7065 7374 6f20  gh cheese pesto 
-00017a40: 6172 7469 6368 6f6b 6520 6865 6172 7473  artichoke hearts
-00017a50: 0a20 2020 2020 2020 2034 2c50 6570 7065  .        4,Peppe
-00017a60: 726f 6e69 2070 697a 7a61 2c70 697a 7a61  roni pizza,pizza
-00017a70: 2064 6f75 6768 2063 6865 6573 6520 746f   dough cheese to
-00017a80: 6d61 746f 2073 6175 6365 2070 6570 7065  mato sauce peppe
-00017a90: 726f 6e69 0a20 2020 2020 2020 2035 2c47  roni.        5,G
-00017aa0: 7269 6c6c 6564 2063 6865 6573 6520 7361  rilled cheese sa
-00017ab0: 6e64 7769 6368 2c62 7265 6164 2063 6865  ndwich,bread che
-00017ac0: 6573 6520 6275 7474 6572 0a20 2020 2020  ese butter.     
-00017ad0: 2020 2036 2c54 756e 6120 6d65 6c74 2c74     6,Tuna melt,t
-00017ae0: 756e 6120 6d61 796f 6e6e 6169 7365 2074  una mayonnaise t
-00017af0: 6f6d 6174 6f20 6272 6561 6420 6368 6565  omato bread chee
-00017b00: 7365 0a20 2020 2020 2020 2037 2c43 6869  se.        7,Chi
-00017b10: 6c69 2064 6f67 2c68 6f74 2064 6f67 2063  li dog,hot dog c
-00017b20: 6869 6c69 206f 6e69 6f6e 2062 756e 0a20  hili onion bun. 
-00017b30: 2020 2020 2020 2038 2c46 7265 6e63 6820         8,French 
-00017b40: 746f 6173 742c 6567 6720 6d69 6c6b 2076  toast,egg milk v
-00017b50: 616e 696c 6c61 2062 7265 6164 206d 6170  anilla bread map
-00017b60: 6c65 2073 7972 7570 0a20 2020 2020 2020  le syrup.       
-00017b70: 2039 2c42 4c54 2c62 7265 6164 2062 6163   9,BLT,bread bac
-00017b80: 6f6e 206c 6574 7475 6365 2074 6f6d 6174  on lettuce tomat
-00017b90: 6f20 6d61 796f 6e6e 6169 7365 0a20 2020  o mayonnaise.   
-00017ba0: 2020 2020 2031 302c 5265 7562 656e 2073       10,Reuben s
-00017bb0: 616e 6477 6963 682c 7279 6520 6272 6561  andwich,rye brea
-00017bc0: 6420 7361 7565 726b 7261 7574 2063 6f72  d sauerkraut cor
-00017bd0: 6e65 6420 6265 6566 2073 7769 7373 2063  ned beef swiss c
-00017be0: 6865 6573 6520 7275 7373 6961 6e20 6472  heese russian dr
-00017bf0: 6573 7369 6e67 2074 686f 7573 616e 6420  essing thousand 
-00017c00: 6973 6c61 6e64 0a20 2020 2020 2020 2031  island.        1
-00017c10: 312c 4861 6d62 7572 6765 722c 6772 6f75  1,Hamburger,grou
-00017c20: 6e64 2062 6565 6620 6275 6e20 6c65 7474  nd beef bun lett
-00017c30: 7563 6520 6b65 7463 6875 7020 6d75 7374  uce ketchup must
-00017c40: 6172 6420 7069 636b 6c65 0a20 2020 2020  ard pickle.     
-00017c50: 2020 2031 322c 4368 6565 7365 6275 7267     12,Cheeseburg
-00017c60: 6572 2c67 726f 756e 6420 6265 6566 2062  er,ground beef b
-00017c70: 756e 206c 6574 7475 6365 206b 6574 6368  un lettuce ketch
-00017c80: 7570 206d 7573 7461 7264 2070 6963 6b6c  up mustard pickl
-00017c90: 6520 6368 6565 7365 0a20 2020 2020 2020  e cheese.       
-00017ca0: 2031 332c 4261 636f 6e20 6368 6565 7365   13,Bacon cheese
-00017cb0: 6275 7267 6572 2c67 726f 756e 6420 6265  burger,ground be
-00017cc0: 6566 2062 756e 206c 6574 7475 6365 206b  ef bun lettuce k
-00017cd0: 6574 6368 7570 206d 7573 7461 7264 2070  etchup mustard p
-00017ce0: 6963 6b6c 6520 6368 6565 7365 2062 6163  ickle cheese bac
-00017cf0: 6f6e 0a20 2020 2020 2020 2022 2222 290a  on.        """).
-00017d00: 0a20 2020 2064 6566 2073 6574 5570 2873  .    def setUp(s
-00017d10: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-00017d20: 6c66 2e72 6563 6970 6573 203d 206c 742e  lf.recipes = lt.
-00017d30: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
-00017d40: 7274 2873 656c 662e 7265 6369 7065 5f64  rt(self.recipe_d
-00017d50: 6174 612c 2074 7261 6e73 666f 726d 733d  ata, transforms=
-00017d60: 6469 6374 2869 643d 696e 7429 290a 2020  dict(id=int)).  
-00017d70: 2020 2020 2020 7365 6c66 2e72 6563 6970        self.recip
-00017d80: 6573 2e63 7265 6174 655f 696e 6465 7828  es.create_index(
-00017d90: 2269 6422 2c20 756e 6971 7565 3d54 7275  "id", unique=Tru
-00017da0: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-00017db0: 7265 6369 7065 732e 6372 6561 7465 5f73  recipes.create_s
-00017dc0: 6561 7263 685f 696e 6465 7828 2269 6e67  earch_index("ing
-00017dd0: 7265 6469 656e 7473 2229 0a0a 2020 2020  redients")..    
-00017de0: 4061 6e6e 6f75 6e63 655f 7465 7374 0a20  @announce_test. 
-00017df0: 2020 2064 6566 2074 6573 745f 6163 6365     def test_acce
-00017e00: 7373 5f6e 6f6e 5f65 7869 7374 656e 745f  ss_non_existent_
-00017e10: 7365 6172 6368 5f61 7474 7269 6275 7465  search_attribute
-00017e20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00017e30: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
-00017e40: 5261 6973 6573 2856 616c 7565 4572 726f  Raises(ValueErro
-00017e50: 722c 206d 7367 3d22 6661 696c 6564 2074  r, msg="failed t
-00017e60: 6f20 7261 6973 6520 5661 6c75 6545 7272  o raise ValueErr
-00017e70: 6f72 2077 6865 6e20 6163 6365 7373 696e  or when accessin
-00017e80: 6720 6e6f 6e2d 6578 6973 7465 6e74 2073  g non-existent s
-00017e90: 6561 7263 6820 696e 6465 7822 293a 0a20  earch index"):. 
-00017ea0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017eb0: 7265 6369 7065 732e 7365 6172 6368 2e74  recipes.search.t
-00017ec0: 6974 6c65 2822 7879 7a22 290a 0a20 2020  itle("xyz")..   
-00017ed0: 2040 616e 6e6f 756e 6365 5f74 6573 740a   @announce_test.
-00017ee0: 2020 2020 6465 6620 7465 7374 5f73 6561      def test_sea
-00017ef0: 7263 685f 6469 7228 7365 6c66 293a 0a20  rch_dir(self):. 
-00017f00: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00017f10: 7274 4571 7561 6c28 5b27 696e 6772 6564  rtEqual(['ingred
-00017f20: 6965 6e74 7327 5d2c 2064 6972 2873 656c  ients'], dir(sel
-00017f30: 662e 7265 6369 7065 732e 7365 6172 6368  f.recipes.search
-00017f40: 292c 2022 6661 696c 6564 2074 6f20 6765  ), "failed to ge
-00017f50: 6e65 7261 7465 2063 6f72 7265 6374 2064  nerate correct d
-00017f60: 6972 2829 2072 6573 706f 6e73 6522 290a  ir() response").
-00017f70: 0a20 2020 2040 616e 6e6f 756e 6365 5f74  .    @announce_t
-00017f80: 6573 740a 2020 2020 6465 6620 7465 7374  est.    def test
-00017f90: 5f74 6578 745f 7365 6172 6368 2873 656c  _text_search(sel
-00017fa0: 6629 3a0a 2020 2020 2020 2020 666f 7220  f):.        for 
-00017fb0: 7175 6572 792c 2065 7870 6563 7465 6420  query, expected 
-00017fc0: 696e 205b 0a20 2020 2020 2020 2020 2020  in [.           
-00017fd0: 2028 2222 2c20 5b5d 292c 0a20 2020 2020   ("", []),.     
-00017fe0: 2020 2020 2020 2028 2274 756e 6122 2c20         ("tuna", 
-00017ff0: 5b31 2c20 365d 292c 0a20 2020 2020 2020  [1, 6]),.       
-00018000: 2020 2020 2028 2274 756e 6120 2b63 6865       ("tuna +che
-00018010: 6573 6522 2c20 5b36 2c20 332c 2034 2c20  ese", [6, 3, 4, 
-00018020: 352c 2031 302c 2031 322c 2031 332c 2031  5, 10, 12, 13, 1
-00018030: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00018040: 2822 7069 6e65 6170 706c 6520 2b62 6163  ("pineapple +bac
-00018050: 6f6e 206c 6574 7475 6365 2062 6565 6620  on lettuce beef 
-00018060: 2d73 6175 6572 6b72 6175 7420 746f 6d61  -sauerkraut toma
-00018070: 746f 222c 205b 392c 2031 332c 2032 2c20  to", [9, 13, 2, 
-00018080: 3131 2c20 3132 2c20 342c 2036 2c20 3130  11, 12, 4, 6, 10
-00018090: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-000180a0: 2822 7069 7a7a 6120 646f 7567 6820 2d70  ("pizza dough -p
-000180b0: 696e 6561 7070 6c65 222c 205b 332c 2034  ineapple", [3, 4
-000180c0: 2c20 325d 292c 0a20 2020 2020 2020 2020  , 2]),.         
-000180d0: 2020 2028 2270 697a 7a61 2064 6f75 6768     ("pizza dough
-000180e0: 202d 2d70 696e 6561 7070 6c65 222c 205b   --pineapple", [
-000180f0: 332c 2034 5d29 2c0a 2020 2020 2020 2020  3, 4]),.        
-00018100: 2020 2020 2822 6272 6561 6420 6261 636f      ("bread baco
-00018110: 6e22 2c20 5b39 2c20 352c 2036 2c20 382c  n", [9, 5, 6, 8,
-00018120: 2031 302c 2031 335d 292c 0a20 2020 2020   10, 13]),.     
-00018130: 2020 2020 2020 2028 2262 7265 6164 202b         ("bread +
-00018140: 2b62 6163 6f6e 222c 205b 392c 2031 335d  +bacon", [9, 13]
-00018150: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-00018160: 2262 7265 6164 202b 2b61 6e63 686f 7669  "bread ++anchovi
-00018170: 6573 222c 205b 5d29 2c0a 2020 2020 2020  es", []),.      
-00018180: 2020 2020 2020 2822 6272 6561 6420 2b2b        ("bread ++
-00018190: 6261 636f 6e20 2b2b 616e 6368 6f76 6965  bacon ++anchovie
-000181a0: 7322 2c20 5b5d 292c 0a20 2020 2020 2020  s", []),.       
-000181b0: 2020 2020 2028 2262 7265 6164 2062 6163       ("bread bac
-000181c0: 6f6e 202d 2d61 6e63 686f 7669 6573 222c  on --anchovies",
-000181d0: 205b 392c 2035 2c20 362c 2038 2c20 3130   [9, 5, 6, 8, 10
-000181e0: 2c20 3133 5d29 2c0a 2020 2020 2020 2020  , 13]),.        
-000181f0: 5d3a 0a20 2020 2020 2020 2020 2020 206d  ]:.            m
-00018200: 6174 6368 6573 203d 2073 656c 662e 7265  atches = self.re
-00018210: 6369 7065 732e 7365 6172 6368 2e69 6e67  cipes.search.ing
-00018220: 7265 6469 656e 7473 2871 7565 7279 2c20  redients(query, 
-00018230: 6173 5f74 6162 6c65 3d46 616c 7365 2c20  as_table=False, 
-00018240: 6d69 6e5f 7363 6f72 653d 2d31 3030 3030  min_score=-10000
-00018250: 290a 2020 2020 2020 2020 2020 2020 6d61  ).            ma
-00018260: 7463 685f 6964 7320 3d20 5b72 6563 6970  tch_ids = [recip
-00018270: 652e 6964 2066 6f72 2072 6563 6970 652c  e.id for recipe,
-00018280: 205f 2069 6e20 6d61 7463 6865 735d 0a20   _ in matches]. 
-00018290: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-000182a0: 2872 6570 7228 7175 6572 7929 2c20 272d  (repr(query), '-
-000182b0: 3e27 2c20 5b28 7265 6369 7065 2e69 642c  >', [(recipe.id,
-000182c0: 2073 636f 7265 2920 666f 7220 7265 6369   score) for reci
-000182d0: 7065 2c20 7363 6f72 6520 696e 206d 6174  pe, score in mat
-000182e0: 6368 6573 5d29 0a20 2020 2020 2020 2020  ches]).         
-000182f0: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-00018300: 5465 7374 2871 7565 7279 3d71 7565 7279  Test(query=query
-00018310: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00018320: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00018330: 7561 6c28 6578 7065 6374 6564 2c20 6d61  ual(expected, ma
-00018340: 7463 685f 6964 732c 0a20 2020 2020 2020  tch_ids,.       
-00018350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018360: 2020 2020 2020 2020 2020 6622 696e 7661            f"inva
-00018370: 6c69 6420 7265 7375 6c74 7320 666f 7220  lid results for 
-00018380: 7175 6572 7920 7b71 7565 7279 2172 7d2c  query {query!r},
-00018390: 2065 7870 6563 7465 6420 7b65 7870 6563   expected {expec
-000183a0: 7465 647d 2c20 676f 7420 7b6d 6174 6368  ted}, got {match
-000183b0: 5f69 6473 7d22 290a 0a20 2020 2040 616e  _ids}")..    @an
-000183c0: 6e6f 756e 6365 5f74 6573 740a 2020 2020  nounce_test.    
-000183d0: 6465 6620 7465 7374 5f69 6e76 616c 6964  def test_invalid
-000183e0: 6174 655f 696e 6465 7828 7365 6c66 293a  ate_index(self):
-000183f0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00018400: 6369 7065 732e 706f 7028 3029 0a20 2020  cipes.pop(0).   
-00018410: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
-00018420: 7373 6572 7452 6169 7365 7328 6c74 2e53  ssertRaises(lt.S
-00018430: 6561 7263 6849 6e64 6578 496e 636f 6e73  earchIndexIncons
-00018440: 6973 7465 6e74 4572 726f 722c 0a20 2020  istentError,.   
-00018450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018460: 2020 2020 2020 2020 2020 2020 6d73 673d              msg=
-00018470: 2266 6169 6c65 6420 746f 2072 6169 7365  "failed to raise
-00018480: 2065 7863 6570 7469 6f6e 2077 6865 6e20   exception when 
-00018490: 7365 6172 6368 696e 6720 6d6f 6469 6669  searching modifi
-000184a0: 6564 2074 6162 6c65 2229 3a0a 2020 2020  ed table"):.    
-000184b0: 2020 2020 2020 2020 7365 6c66 2e72 6563          self.rec
-000184c0: 6970 6573 2e73 6561 7263 682e 696e 6772  ipes.search.ingr
-000184d0: 6564 6965 6e74 7328 2262 6163 6f6e 2229  edients("bacon")
-000184e0: 0a0a 2020 2020 4061 6e6e 6f75 6e63 655f  ..    @announce_
-000184f0: 7465 7374 0a20 2020 2064 6566 2074 6573  test.    def tes
-00018500: 745f 7365 6172 6368 5f77 6974 685f 6b65  t_search_with_ke
-00018510: 7977 6f72 6473 2873 656c 6629 3a0a 2020  ywords(self):.  
-00018520: 2020 2020 2020 666f 7220 7175 6572 792c        for query,
-00018530: 2065 7870 6563 7465 642c 2065 7870 6563   expected, expec
-00018540: 7465 645f 776f 7264 7320 696e 205b 0a20  ted_words in [. 
-00018550: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00018560: 2274 756e 6122 2c20 5b31 2c20 365d 2c20  "tuna", [1, 6], 
-00018570: 5b7b 276e 6f6f 646c 6573 272c 2027 6e6f  [{'noodles', 'no
-00018580: 6f64 6c65 272c 2027 7475 6e61 272c 2027  odle', 'tuna', '
-00018590: 736f 7570 272c 2027 6372 6561 6d27 2c20  soup', 'cream', 
-000185a0: 276d 7573 6872 6f6f 6d27 7d2c 0a20 2020  'mushroom'},.   
-000185b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185c0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000185d0: 2774 6f6d 6174 6f27 2c20 2774 756e 6127  'tomato', 'tuna'
-000185e0: 2c20 276d 6179 6f6e 6e61 6973 6527 2c20  , 'mayonnaise', 
-000185f0: 2762 7265 6164 272c 2027 6368 6565 7365  'bread', 'cheese
-00018600: 277d 5d29 2c0a 2020 2020 2020 2020 2020  '}]),.          
-00018610: 2020 2020 2020 5d3a 0a20 2020 2020 2020        ]:.       
-00018620: 2020 2020 206d 6174 6368 6573 203d 2073       matches = s
-00018630: 656c 662e 7265 6369 7065 732e 7365 6172  elf.recipes.sear
-00018640: 6368 2e69 6e67 7265 6469 656e 7473 2871  ch.ingredients(q
-00018650: 7565 7279 2c20 6d69 6e5f 7363 6f72 653d  uery, min_score=
-00018660: 2d31 3030 3030 2c20 6173 5f74 6162 6c65  -10000, as_table
-00018670: 3d46 616c 7365 2c20 696e 636c 7564 655f  =False, include_
-00018680: 776f 7264 733d 5472 7565 290a 2020 2020  words=True).    
-00018690: 2020 2020 2020 2020 6d61 7463 685f 6964          match_id
-000186a0: 7320 3d20 5b72 6563 6970 652e 6964 2066  s = [recipe.id f
-000186b0: 6f72 2072 6563 6970 652c 2073 636f 7265  or recipe, score
-000186c0: 2c20 776f 7264 7320 696e 206d 6174 6368  , words in match
-000186d0: 6573 5d0a 2020 2020 2020 2020 2020 2020  es].            
-000186e0: 7072 696e 7428 7265 7072 2871 7565 7279  print(repr(query
-000186f0: 292c 2027 2d3e 272c 205b 2872 6563 6970  ), '->', [(recip
-00018700: 652e 6964 2c20 7363 6f72 652c 2077 6f72  e.id, score, wor
-00018710: 6473 2920 666f 7220 7265 6369 7065 2c20  ds) for recipe, 
-00018720: 7363 6f72 652c 2077 6f72 6473 2069 6e20  score, words in 
-00018730: 6d61 7463 6865 735d 290a 2020 2020 2020  matches]).      
-00018740: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00018750: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
-00018760: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018770: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
-00018780: 6374 6564 2c20 6d61 7463 685f 6964 732c  cted, match_ids,
-00018790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000187a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187b0: 2020 6622 696e 7661 6c69 6420 7265 7375    f"invalid resu
-000187c0: 6c74 7320 666f 7220 7175 6572 7920 7b71  lts for query {q
-000187d0: 7565 7279 2172 7d2c 2065 7870 6563 7465  uery!r}, expecte
-000187e0: 6420 7b65 7870 6563 7465 647d 2c20 676f  d {expected}, go
-000187f0: 7420 7b6d 6174 6368 5f69 6473 7d22 290a  t {match_ids}").
-00018800: 2020 2020 2020 2020 2020 2020 6d61 7463              matc
-00018810: 685f 776f 7264 7320 3d20 5b73 6574 2877  h_words = [set(w
-00018820: 6f72 6473 2920 666f 7220 7265 6369 7065  ords) for recipe
-00018830: 2c20 7363 6f72 652c 2077 6f72 6473 2069  , score, words i
-00018840: 6e20 6d61 7463 6865 735d 0a20 2020 2020  n matches].     
-00018850: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00018860: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
-00018870: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018880: 2e61 7373 6572 7445 7175 616c 2865 7870  .assertEqual(exp
-00018890: 6563 7465 645f 776f 7264 732c 206d 6174  ected_words, mat
-000188a0: 6368 5f77 6f72 6473 2c0a 2020 2020 2020  ch_words,.      
-000188b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188c0: 2020 2020 2020 2020 2020 2022 696e 7661             "inva
-000188d0: 6c69 6420 6d61 7463 6820 776f 7264 7320  lid match words 
-000188e0: 666f 7220 7175 6572 7920 7b21 727d 2c20  for query {!r}, 
-000188f0: 6578 7065 6374 6564 207b 7d2c 2067 6f74  expected {}, got
-00018900: 207b 7d22 2e66 6f72 6d61 7428 7175 6572   {}".format(quer
-00018910: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
-00018920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018970: 2020 2020 2065 7870 6563 7465 645f 776f       expected_wo
-00018980: 7264 732c 0a20 2020 2020 2020 2020 2020  rds,.           
-00018990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189e0: 2020 2020 2020 206d 6174 6368 5f77 6f72         match_wor
-000189f0: 6473 2929 0a0a 2020 2020 4061 6e6e 6f75  ds))..    @annou
-00018a00: 6e63 655f 7465 7374 0a20 2020 2064 6566  nce_test.    def
-00018a10: 2074 6573 745f 7365 6172 6368 5f77 6974   test_search_wit
-00018a20: 685f 6c69 6d69 7428 7365 6c66 293a 0a20  h_limit(self):. 
-00018a30: 2020 2020 2020 2066 6f72 2071 7565 7279         for query
-00018a40: 2c20 6578 7065 6374 6564 2069 6e20 5b0a  , expected in [.
-00018a50: 2020 2020 2020 2020 2020 2020 2822 222c              ("",
-00018a60: 205b 5d29 2c0a 2020 2020 2020 2020 2020   []),.          
-00018a70: 2020 2822 7475 6e61 222c 205b 312c 2036    ("tuna", [1, 6
-00018a80: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00018a90: 2822 7475 6e61 202b 6368 6565 7365 222c  ("tuna +cheese",
-00018aa0: 205b 362c 2033 2c20 345d 292c 0a20 2020   [6, 3, 4]),.   
-00018ab0: 2020 2020 2020 2020 2028 2270 696e 6561           ("pinea
-00018ac0: 7070 6c65 202b 6261 636f 6e20 6c65 7474  pple +bacon lett
-00018ad0: 7563 6520 6265 6566 202d 7361 7565 726b  uce beef -sauerk
-00018ae0: 7261 7574 2074 6f6d 6174 6f22 2c20 5b39  raut tomato", [9
-00018af0: 2c20 3133 2c20 325d 292c 0a20 2020 2020  , 13, 2]),.     
-00018b00: 2020 2020 2020 2028 2270 697a 7a61 2064         ("pizza d
-00018b10: 6f75 6768 202d 7069 6e65 6170 706c 6522  ough -pineapple"
-00018b20: 2c20 5b33 2c20 342c 2032 5d29 2c0a 2020  , [3, 4, 2]),.  
-00018b30: 2020 2020 2020 2020 2020 2822 7069 7a7a            ("pizz
-00018b40: 6120 646f 7567 6820 2d2d 7069 6e65 6170  a dough --pineap
-00018b50: 706c 6522 2c20 5b33 2c20 345d 292c 0a20  ple", [3, 4]),. 
-00018b60: 2020 2020 2020 2020 2020 2028 2262 7265             ("bre
-00018b70: 6164 2062 6163 6f6e 222c 205b 392c 2035  ad bacon", [9, 5
-00018b80: 2c20 365d 292c 0a20 2020 2020 2020 2020  , 6]),.         
-00018b90: 2020 2028 2262 7265 6164 202b 2b62 6163     ("bread ++bac
-00018ba0: 6f6e 222c 205b 392c 2031 335d 292c 0a20  on", [9, 13]),. 
-00018bb0: 2020 2020 2020 2020 2020 2028 2262 7265             ("bre
-00018bc0: 6164 202b 2b61 6e63 686f 7669 6573 222c  ad ++anchovies",
-00018bd0: 205b 5d29 2c0a 2020 2020 2020 2020 2020   []),.          
-00018be0: 2020 2822 6272 6561 6420 2b2b 6261 636f    ("bread ++baco
-00018bf0: 6e20 2b2b 616e 6368 6f76 6965 7322 2c20  n ++anchovies", 
-00018c00: 5b5d 292c 0a20 2020 2020 2020 2020 2020  []),.           
-00018c10: 2028 2262 7265 6164 2062 6163 6f6e 202d   ("bread bacon -
-00018c20: 2d61 6e63 686f 7669 6573 222c 205b 392c  -anchovies", [9,
-00018c30: 2035 2c20 365d 292c 0a20 2020 2020 2020   5, 6]),.       
-00018c40: 205d 3a0a 2020 2020 2020 2020 2020 2020   ]:.            
-00018c50: 6d61 7463 6865 7320 3d20 7365 6c66 2e72  matches = self.r
-00018c60: 6563 6970 6573 2e73 6561 7263 682e 696e  ecipes.search.in
-00018c70: 6772 6564 6965 6e74 7328 7175 6572 792c  gredients(query,
-00018c80: 2061 735f 7461 626c 653d 4661 6c73 652c   as_table=False,
-00018c90: 206d 696e 5f73 636f 7265 3d2d 3130 3030   min_score=-1000
-00018ca0: 302c 206c 696d 6974 3d33 290a 2020 2020  0, limit=3).    
-00018cb0: 2020 2020 2020 2020 6d61 7463 685f 6964          match_id
-00018cc0: 7320 3d20 5b72 6563 6970 652e 6964 2066  s = [recipe.id f
-00018cd0: 6f72 2072 6563 6970 652c 205f 2069 6e20  or recipe, _ in 
-00018ce0: 6d61 7463 6865 735d 0a20 2020 2020 2020  matches].       
-00018cf0: 2020 2020 2070 7269 6e74 2872 6570 7228       print(repr(
-00018d00: 7175 6572 7929 2c20 272d 3e27 2c20 5b28  query), '->', [(
-00018d10: 7265 6369 7065 2e69 642c 2073 636f 7265  recipe.id, score
-00018d20: 2920 666f 7220 7265 6369 7065 2c20 7363  ) for recipe, sc
-00018d30: 6f72 6520 696e 206d 6174 6368 6573 5d29  ore in matches])
-00018d40: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00018d50: 6820 7365 6c66 2e73 7562 5465 7374 2871  h self.subTest(q
-00018d60: 7565 7279 3d71 7565 7279 293a 0a20 2020  uery=query):.   
-00018d70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018d80: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
-00018d90: 7065 6374 6564 2c20 6d61 7463 685f 6964  pected, match_id
-00018da0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00018db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018dc0: 2020 2020 6622 696e 7661 6c69 6420 7265      f"invalid re
-00018dd0: 7375 6c74 7320 666f 7220 7175 6572 7920  sults for query 
-00018de0: 7b71 7565 7279 2172 7d2c 2065 7870 6563  {query!r}, expec
-00018df0: 7465 6420 7b65 7870 6563 7465 647d 2c20  ted {expected}, 
-00018e00: 676f 7420 7b6d 6174 6368 5f69 6473 7d22  got {match_ids}"
-00018e10: 290a 0a20 2020 2040 616e 6e6f 756e 6365  )..    @announce
-00018e20: 5f74 6573 740a 2020 2020 6465 6620 7465  _test.    def te
-00018e30: 7374 5f73 6561 7263 685f 7769 7468 5f6d  st_search_with_m
-00018e40: 696e 5f73 636f 7265 2873 656c 6629 3a0a  in_score(self):.
-00018e50: 2020 2020 2020 2020 666f 7220 7175 6572          for quer
-00018e60: 792c 2065 7870 6563 7465 6420 696e 205b  y, expected in [
-00018e70: 0a20 2020 2020 2020 2020 2020 2028 2222  .            (""
-00018e80: 2c20 5b5d 292c 0a20 2020 2020 2020 2020  , []),.         
-00018e90: 2020 2028 2274 756e 6122 2c20 5b5d 292c     ("tuna", []),
-00018ea0: 0a20 2020 2020 2020 2020 2020 2028 2274  .            ("t
-00018eb0: 756e 6120 2b63 6865 6573 6522 2c20 5b36  una +cheese", [6
-00018ec0: 2c5d 292c 0a20 2020 2020 2020 2020 2020  ,]),.           
-00018ed0: 2028 2270 696e 6561 7070 6c65 202b 6261   ("pineapple +ba
-00018ee0: 636f 6e20 6c65 7474 7563 6520 6265 6566  con lettuce beef
-00018ef0: 202d 7361 7565 726b 7261 7574 2074 6f6d   -sauerkraut tom
-00018f00: 6174 6f22 2c20 5b39 2c20 3133 5d29 2c0a  ato", [9, 13]),.
-00018f10: 2020 2020 2020 2020 2020 2020 2822 7069              ("pi
-00018f20: 7a7a 6120 646f 7567 6820 2d70 696e 6561  zza dough -pinea
-00018f30: 7070 6c65 222c 205b 5d29 2c0a 2020 2020  pple", []),.    
-00018f40: 2020 2020 2020 2020 2822 7069 7a7a 6120          ("pizza 
-00018f50: 646f 7567 6820 2d2d 7069 6e65 6170 706c  dough --pineappl
-00018f60: 6522 2c20 5b5d 292c 0a20 2020 2020 2020  e", []),.       
-00018f70: 2020 2020 2028 2262 7265 6164 2062 6163       ("bread bac
-00018f80: 6f6e 222c 205b 5d29 2c0a 2020 2020 2020  on", []),.      
-00018f90: 2020 2020 2020 2822 6272 6561 6420 2b2b        ("bread ++
-00018fa0: 6261 636f 6e22 2c20 5b39 2c5d 292c 0a20  bacon", [9,]),. 
-00018fb0: 2020 2020 2020 2020 2020 2028 2262 7265             ("bre
-00018fc0: 6164 202b 2b61 6e63 686f 7669 6573 222c  ad ++anchovies",
-00018fd0: 205b 5d29 2c0a 2020 2020 2020 2020 2020   []),.          
-00018fe0: 2020 2822 6272 6561 6420 2b2b 6261 636f    ("bread ++baco
-00018ff0: 6e20 2b2b 616e 6368 6f76 6965 7322 2c20  n ++anchovies", 
-00019000: 5b5d 292c 0a20 2020 2020 2020 2020 2020  []),.           
-00019010: 2028 2262 7265 6164 2062 6163 6f6e 202d   ("bread bacon -
-00019020: 2d61 6e63 686f 7669 6573 222c 205b 5d29  -anchovies", [])
-00019030: 2c0a 2020 2020 2020 2020 5d3a 0a20 2020  ,.        ]:.   
-00019040: 2020 2020 2020 2020 206d 6174 6368 6573           matches
-00019050: 203d 2073 656c 662e 7265 6369 7065 732e   = self.recipes.
-00019060: 7365 6172 6368 2e69 6e67 7265 6469 656e  search.ingredien
-00019070: 7473 2871 7565 7279 2c20 6173 5f74 6162  ts(query, as_tab
-00019080: 6c65 3d46 616c 7365 2c20 6d69 6e5f 7363  le=False, min_sc
-00019090: 6f72 653d 3130 3030 290a 2020 2020 2020  ore=1000).      
-000190a0: 2020 2020 2020 6d61 7463 685f 6964 7320        match_ids 
-000190b0: 3d20 5b72 6563 6970 652e 6964 2066 6f72  = [recipe.id for
-000190c0: 2072 6563 6970 652c 205f 2069 6e20 6d61   recipe, _ in ma
-000190d0: 7463 6865 735d 0a20 2020 2020 2020 2020  tches].         
-000190e0: 2020 2070 7269 6e74 2872 6570 7228 7175     print(repr(qu
-000190f0: 6572 7929 2c20 272d 3e27 2c20 5b28 7265  ery), '->', [(re
-00019100: 6369 7065 2e69 642c 2073 636f 7265 2920  cipe.id, score) 
-00019110: 666f 7220 7265 6369 7065 2c20 7363 6f72  for recipe, scor
-00019120: 6520 696e 206d 6174 6368 6573 5d29 0a20  e in matches]). 
-00019130: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00019140: 7365 6c66 2e73 7562 5465 7374 2871 7565  self.subTest(que
-00019150: 7279 3d71 7565 7279 293a 0a20 2020 2020  ry=query):.     
-00019160: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019170: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
-00019180: 6374 6564 2c20 6d61 7463 685f 6964 732c  cted, match_ids,
-00019190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000191a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191b0: 2020 6622 696e 7661 6c69 6420 7265 7375    f"invalid resu
-000191c0: 6c74 7320 666f 7220 7175 6572 7920 7b71  lts for query {q
-000191d0: 7565 7279 2172 7d2c 2065 7870 6563 7465  uery!r}, expecte
-000191e0: 6420 7b65 7870 6563 7465 647d 2c20 676f  d {expected}, go
-000191f0: 7420 7b6d 6174 6368 5f69 6473 7d22 290a  t {match_ids}").
-00019200: 0a20 2020 2040 616e 6e6f 756e 6365 5f74  .    @announce_t
-00019210: 6573 740a 2020 2020 6465 6620 7465 7374  est.    def test
-00019220: 5f73 6561 7263 685f 7769 7468 5f61 735f  _search_with_as_
-00019230: 7461 626c 6528 7365 6c66 293a 0a20 2020  table(self):.   
-00019240: 2020 2020 2066 6f72 2071 7565 7279 2c20       for query, 
-00019250: 6578 7065 6374 6564 2069 6e20 5b0a 2020  expected in [.  
-00019260: 2020 2020 2020 2020 2020 2822 222c 205b            ("", [
-00019270: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00019280: 2822 7475 6e61 222c 205b 5d29 2c0a 2020  ("tuna", []),.  
-00019290: 2020 2020 2020 2020 2020 2822 7475 6e61            ("tuna
-000192a0: 202b 6368 6565 7365 222c 205b 362c 5d29   +cheese", [6,])
-000192b0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
-000192c0: 7069 6e65 6170 706c 6520 2b62 6163 6f6e  pineapple +bacon
-000192d0: 206c 6574 7475 6365 2062 6565 6620 2d73   lettuce beef -s
-000192e0: 6175 6572 6b72 6175 7420 746f 6d61 746f  auerkraut tomato
-000192f0: 222c 205b 392c 2031 335d 292c 0a20 2020  ", [9, 13]),.   
-00019300: 2020 2020 2020 2020 2028 2270 697a 7a61           ("pizza
-00019310: 2064 6f75 6768 202d 7069 6e65 6170 706c   dough -pineappl
-00019320: 6522 2c20 5b5d 292c 0a20 2020 2020 2020  e", []),.       
-00019330: 2020 2020 2028 2270 697a 7a61 2064 6f75       ("pizza dou
-00019340: 6768 202d 2d70 696e 6561 7070 6c65 222c  gh --pineapple",
-00019350: 205b 5d29 2c0a 2020 2020 2020 2020 2020   []),.          
-00019360: 2020 2822 6272 6561 6420 6261 636f 6e22    ("bread bacon"
-00019370: 2c20 5b5d 292c 0a20 2020 2020 2020 2020  , []),.         
-00019380: 2020 2028 2262 7265 6164 202b 2b62 6163     ("bread ++bac
-00019390: 6f6e 222c 205b 392c 5d29 2c0a 2020 2020  on", [9,]),.    
-000193a0: 2020 2020 2020 2020 2822 6272 6561 6420          ("bread 
-000193b0: 2b2b 616e 6368 6f76 6965 7322 2c20 5b5d  ++anchovies", []
-000193c0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-000193d0: 2262 7265 6164 202b 2b62 6163 6f6e 202b  "bread ++bacon +
-000193e0: 2b61 6e63 686f 7669 6573 222c 205b 5d29  +anchovies", [])
-000193f0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
-00019400: 6272 6561 6420 6261 636f 6e20 2d2d 616e  bread bacon --an
-00019410: 6368 6f76 6965 7322 2c20 5b5d 292c 0a20  chovies", []),. 
-00019420: 2020 2020 2020 205d 3a0a 2020 2020 2020         ]:.      
-00019430: 2020 2020 2020 6d61 7463 6865 7320 3d20        matches = 
-00019440: 7365 6c66 2e72 6563 6970 6573 2e73 6561  self.recipes.sea
-00019450: 7263 682e 696e 6772 6564 6965 6e74 7328  rch.ingredients(
-00019460: 7175 6572 792c 206d 696e 5f73 636f 7265  query, min_score
-00019470: 3d31 3030 302c 2061 735f 7461 626c 653d  =1000, as_table=
-00019480: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-00019490: 2020 6d61 7463 685f 6964 7320 3d20 5b72    match_ids = [r
-000194a0: 6563 6970 652e 6964 2066 6f72 2072 6563  ecipe.id for rec
-000194b0: 6970 6520 696e 206d 6174 6368 6573 5d0a  ipe in matches].
-000194c0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000194d0: 7428 7265 7072 2871 7565 7279 292c 2027  t(repr(query), '
-000194e0: 2d3e 272c 205b 2872 6563 6970 652e 6964  ->', [(recipe.id
-000194f0: 2c20 7265 6369 7065 2e69 6e67 7265 6469  , recipe.ingredi
-00019500: 656e 7473 5f73 6561 7263 685f 7363 6f72  ents_search_scor
-00019510: 6529 2066 6f72 2072 6563 6970 6520 696e  e) for recipe in
-00019520: 206d 6174 6368 6573 5d29 0a20 2020 2020   matches]).     
-00019530: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00019540: 2e73 7562 5465 7374 2871 7565 7279 3d71  .subTest(query=q
-00019550: 7565 7279 293a 0a20 2020 2020 2020 2020  uery):.         
-00019560: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00019570: 7274 4571 7561 6c28 6578 7065 6374 6564  rtEqual(expected
-00019580: 2c20 6d61 7463 685f 6964 732c 0a20 2020  , match_ids,.   
-00019590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195a0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-000195b0: 696e 7661 6c69 6420 7265 7375 6c74 7320  invalid results 
-000195c0: 666f 7220 7175 6572 7920 7b71 7565 7279  for query {query
-000195d0: 2172 7d2c 2065 7870 6563 7465 6420 7b65  !r}, expected {e
-000195e0: 7870 6563 7465 647d 2c20 676f 7420 7b6d  xpected}, got {m
-000195f0: 6174 6368 5f69 6473 7d22 290a 0a20 2020  atch_ids}")..   
-00019600: 2020 2020 2020 2020 2073 636f 7265 5f61           score_a
-00019610: 7474 7220 3d20 2269 6e67 7265 6469 656e  ttr = "ingredien
-00019620: 7473 5f73 6561 7263 685f 7363 6f72 6522  ts_search_score"
-00019630: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00019640: 662e 6173 7365 7274 5472 7565 280a 2020  f.assertTrue(.  
-00019650: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00019660: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
-00019670: 2020 2020 2020 2068 6173 6174 7472 286d         hasattr(m
-00019680: 6174 6368 6573 2e62 792e 6964 5b6d 6964  atches.by.id[mid
-00019690: 5d2c 2073 636f 7265 5f61 7474 7229 0a20  ], score_attr). 
-000196a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196b0: 2020 2066 6f72 206d 6964 2069 6e20 6d61     for mid in ma
-000196c0: 7463 685f 6964 730a 2020 2020 2020 2020  tch_ids.        
-000196d0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-000196e0: 2020 2020 2020 2020 2020 2066 2261 735f             f"as_
-000196f0: 7461 626c 6520 6469 6420 6e6f 7420 706f  table did not po
-00019700: 7075 6c61 7465 2073 6f6d 6520 7365 6172  pulate some sear
-00019710: 6368 2072 6563 6f72 6473 2077 6974 6820  ch records with 
-00019720: 7b73 636f 7265 5f61 7474 7221 727d 220a  {score_attr!r}".
-00019730: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00019740: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019750: 6173 7365 7274 4661 6c73 6528 0a20 2020  assertFalse(.   
-00019760: 2020 2020 2020 2020 2020 2020 2061 6e79               any
-00019770: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00019780: 2020 2020 2020 6861 7361 7474 7228 7365        hasattr(se
-00019790: 6c66 2e72 6563 6970 6573 2e62 792e 6964  lf.recipes.by.id
-000197a0: 5b6d 6964 5d2c 2073 636f 7265 5f61 7474  [mid], score_att
-000197b0: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
-000197c0: 2020 2020 2020 2066 6f72 206d 6964 2069         for mid i
-000197d0: 6e20 6d61 7463 685f 6964 730a 2020 2020  n match_ids.    
-000197e0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-000197f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00019800: 2261 735f 7461 626c 6520 706f 7075 6c61  "as_table popula
-00019810: 7465 6420 736f 6d65 206f 7269 6769 6e61  ted some origina
-00019820: 6c20 7265 636f 7264 7320 7769 7468 207b  l records with {
-00019830: 7363 6f72 655f 6174 7472 2172 7d22 0a20  score_attr!r}". 
-00019840: 2020 2020 2020 2020 2020 2029 0a0a 636c             )..cl
-00019850: 6173 7320 5461 626c 6553 6561 7263 6854  ass TableSearchT
-00019860: 6573 7473 5f44 6174 614f 626a 6563 7473  ests_DataObjects
-00019870: 2854 6162 6c65 5365 6172 6368 5465 7374  (TableSearchTest
-00019880: 732c 2055 7369 6e67 4461 7461 4f62 6a65  s, UsingDataObje
-00019890: 6374 7329 3a0a 2020 2020 7061 7373 0a0a  cts):.    pass..
-000198a0: 636c 6173 7320 5461 626c 6553 6561 7263  class TableSearc
-000198b0: 6854 6573 7473 5f4e 616d 6564 7475 706c  hTests_Namedtupl
-000198c0: 6573 2854 6162 6c65 5365 6172 6368 5465  es(TableSearchTe
-000198d0: 7374 732c 2055 7369 6e67 4e61 6d65 6474  sts, UsingNamedt
-000198e0: 7570 6c65 7329 3a0a 2020 2020 7061 7373  uples):.    pass
-000198f0: 0a0a 636c 6173 7320 5461 626c 6553 6561  ..class TableSea
-00019900: 7263 6854 6573 7473 5f54 7970 696e 674e  rchTests_TypingN
-00019910: 616d 6564 7475 706c 6573 2854 6162 6c65  amedtuples(Table
-00019920: 5365 6172 6368 5465 7374 732c 2055 7369  SearchTests, Usi
-00019930: 6e67 5479 7069 6e67 4e61 6d65 6454 7570  ngTypingNamedTup
-00019940: 6c65 293a 0a20 2020 2070 6173 730a 0a63  le):.    pass..c
-00019950: 6c61 7373 2054 6162 6c65 5365 6172 6368  lass TableSearch
-00019960: 5465 7374 735f 5479 7069 6e67 5479 7065  Tests_TypingType
-00019970: 6444 6963 7428 5461 626c 6553 6561 7263  dDict(TableSearc
-00019980: 6854 6573 7473 2c20 5573 696e 6754 7970  hTests, UsingTyp
-00019990: 696e 6754 7970 6564 4469 6374 293a 0a20  ingTypedDict):. 
-000199a0: 2020 2070 6173 730a 0a63 6c61 7373 2054     pass..class T
-000199b0: 6162 6c65 5365 6172 6368 5465 7374 735f  ableSearchTests_
-000199c0: 536c 6f74 7465 6428 5461 626c 6553 6561  Slotted(TableSea
-000199d0: 7263 6854 6573 7473 2c20 5573 696e 6753  rchTests, UsingS
-000199e0: 6c6f 7474 6564 4f62 6a65 6374 7329 3a0a  lottedObjects):.
-000199f0: 2020 2020 7061 7373 0a0a 636c 6173 7320      pass..class 
-00019a00: 5461 626c 6553 6561 7263 6854 6573 7473  TableSearchTests
-00019a10: 5f53 696d 706c 654e 616d 6573 7061 6365  _SimpleNamespace
-00019a20: 2854 6162 6c65 5365 6172 6368 5465 7374  (TableSearchTest
-00019a30: 732c 2055 7369 6e67 5369 6d70 6c65 4e61  s, UsingSimpleNa
-00019a40: 6d65 7370 6163 6529 3a0a 2020 2020 7061  mespace):.    pa
-00019a50: 7373 0a0a 6966 2064 6174 6163 6c61 7373  ss..if dataclass
-00019a60: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
-00019a70: 2020 2020 636c 6173 7320 5461 626c 6553      class TableS
-00019a80: 6561 7263 6854 6573 7473 5f44 6174 6163  earchTests_Datac
-00019a90: 6c61 7373 6573 2854 6162 6c65 5365 6172  lasses(TableSear
-00019aa0: 6368 5465 7374 732c 2055 7369 6e67 4461  chTests, UsingDa
-00019ab0: 7461 636c 6173 7365 7329 3a0a 2020 2020  taclasses):.    
-00019ac0: 2020 2020 7061 7373 0a0a 6966 2070 7964      pass..if pyd
-00019ad0: 616e 7469 6320 6973 206e 6f74 204e 6f6e  antic is not Non
-00019ae0: 653a 0a20 2020 2063 6c61 7373 2054 6162  e:.    class Tab
-00019af0: 6c65 5365 6172 6368 5465 7374 735f 5079  leSearchTests_Py
-00019b00: 6461 6e74 6963 4d6f 6465 6c73 2854 6162  danticModels(Tab
-00019b10: 6c65 5365 6172 6368 5465 7374 732c 2055  leSearchTests, U
-00019b20: 7369 6e67 5079 6461 6e74 6963 4d6f 6465  singPydanticMode
-00019b30: 6c29 3a0a 2020 2020 2020 2020 7061 7373  l):.        pass
-00019b40: 0a0a 2020 2020 636c 6173 7320 5461 626c  ..    class Tabl
-00019b50: 6553 6561 7263 6854 6573 7473 5f50 7964  eSearchTests_Pyd
-00019b60: 616e 7469 6349 6d6d 7574 6162 6c65 4d6f  anticImmutableMo
-00019b70: 6465 6c73 2854 6162 6c65 5365 6172 6368  dels(TableSearch
-00019b80: 5465 7374 732c 2055 7369 6e67 5079 6461  Tests, UsingPyda
-00019b90: 6e74 6963 496d 6d75 7461 626c 654d 6f64  nticImmutableMod
-00019ba0: 656c 293a 0a20 2020 2020 2020 2070 6173  el):.        pas
-00019bb0: 730a 0a20 2020 2063 6c61 7373 2054 6162  s..    class Tab
-00019bc0: 6c65 5365 6172 6368 5465 7374 735f 5079  leSearchTests_Py
-00019bd0: 6461 6e74 6963 4f52 4d4d 6f64 656c 7328  danticORMModels(
-00019be0: 5461 626c 6553 6561 7263 6854 6573 7473  TableSearchTests
-00019bf0: 2c20 5573 696e 6750 7964 616e 7469 634f  , UsingPydanticO
-00019c00: 524d 4d6f 6465 6c29 3a0a 2020 2020 2020  RMModel):.      
-00019c10: 2020 7061 7373 0a0a 6966 2061 7474 7220    pass..if attr 
-00019c20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00019c30: 2063 6c61 7373 2054 6162 6c65 5365 6172   class TableSear
-00019c40: 6368 5465 7374 735f 4174 7472 436c 6173  chTests_AttrClas
-00019c50: 7365 7328 5461 626c 6553 6561 7263 6854  ses(TableSearchT
-00019c60: 6573 7473 2c20 5573 696e 6741 7474 7243  ests, UsingAttrC
-00019c70: 6c61 7373 293a 0a20 2020 2020 2020 2070  lass):.        p
-00019c80: 6173 730a 0a69 6620 7472 6169 746c 6574  ass..if traitlet
-00019c90: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-00019ca0: 2020 2063 6c61 7373 2054 6162 6c65 5365     class TableSe
-00019cb0: 6172 6368 5465 7374 735f 5472 6169 746c  archTests_Traitl
-00019cc0: 6574 7343 6c61 7373 6573 2854 6162 6c65  etsClasses(Table
-00019cd0: 5365 6172 6368 5465 7374 732c 2055 7369  SearchTests, Usi
-00019ce0: 6e67 5472 6169 746c 6574 7343 6c61 7373  ngTraitletsClass
-00019cf0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-00019d00: 0a69 6620 536c 6f74 7465 6457 6974 6844  .if SlottedWithD
-00019d10: 6963 7420 6973 206e 6f74 204e 6f6e 653a  ict is not None:
-00019d20: 0a20 2020 2063 6c61 7373 2054 6162 6c65  .    class Table
-00019d30: 5365 6172 6368 5465 7374 735f 536c 6f74  SearchTests_Slot
-00019d40: 7465 6457 6974 6844 6963 7428 5461 626c  tedWithDict(Tabl
-00019d50: 6553 6561 7263 6854 6573 7473 2c20 5573  eSearchTests, Us
-00019d60: 696e 6753 6c6f 7474 6564 5769 7468 4469  ingSlottedWithDi
-00019d70: 6374 4f62 6a65 6374 7329 3a0a 2020 2020  ctObjects):.    
-00019d80: 2020 2020 7061 7373 0a0a 0a63 6c61 7373      pass...class
-00019d90: 2049 6e69 7469 616c 5465 7374 2875 6e69   InitialTest(uni
-00019da0: 7474 6573 742e 5465 7374 4361 7365 293a  ttest.TestCase):
-00019db0: 0a20 2020 2066 726f 6d20 6c69 7474 6c65  .    from little
-00019dc0: 7461 626c 6520 696d 706f 7274 2028 0a20  table import (. 
-00019dd0: 2020 2020 2020 205f 5f76 6572 7369 6f6e         __version
-00019de0: 5f5f 2061 7320 6c69 7474 6c65 7461 626c  __ as littletabl
-00019df0: 655f 7665 7273 696f 6e2c 0a20 2020 2020  e_version,.     
-00019e00: 2020 205f 5f76 6572 7369 6f6e 5f74 696d     __version_tim
-00019e10: 655f 5f20 6173 206c 6974 746c 6574 6162  e__ as littletab
-00019e20: 6c65 5f76 6572 7369 6f6e 5f74 696d 652c  le_version_time,
-00019e30: 0a20 2020 2020 2020 205f 5f76 6572 7369  .        __versi
-00019e40: 6f6e 5f69 6e66 6f5f 5f20 6173 206c 6974  on_info__ as lit
-00019e50: 746c 6574 6162 6c65 5f76 6572 7369 6f6e  tletable_version
-00019e60: 5f69 6e66 6f2c 0a20 2020 2029 0a0a 2020  _info,.    )..  
-00019e70: 2020 7072 696e 7428 0a20 2020 2020 2020    print(.       
-00019e80: 2066 2242 6567 696e 6e69 6e67 2074 6573   f"Beginning tes
-00019e90: 7420 6f66 206c 6974 746c 6574 6162 6c65  t of littletable
-00019ea0: 2c20 7665 7273 696f 6e20 7b6c 6974 746c  , version {littl
-00019eb0: 6574 6162 6c65 5f76 6572 7369 6f6e 7d2c  etable_version},
-00019ec0: 207b 6c69 7474 6c65 7461 626c 655f 7665   {littletable_ve
-00019ed0: 7273 696f 6e5f 7469 6d65 7d22 2c0a 2020  rsion_time}",.  
-00019ee0: 2020 290a 2020 2020 7072 696e 7428 6c69    ).    print(li
-00019ef0: 7474 6c65 7461 626c 655f 7665 7273 696f  ttletable_versio
-00019f00: 6e5f 696e 666f 290a 2020 2020 7072 696e  n_info).    prin
-00019f10: 7428 2250 7974 686f 6e20 7665 7273 696f  t("Python versio
-00019f20: 6e22 2c20 7379 732e 7665 7273 696f 6e29  n", sys.version)
-00019f30: 0a20 2020 2070 7269 6e74 2829 0a0a 0a63  .    print()...c
-00019f40: 6c61 7373 2053 746f 7261 6765 496e 6465  lass StorageInde
-00019f50: 7065 6e64 656e 7454 6573 7473 2875 6e69  pendentTests(uni
-00019f60: 7474 6573 742e 5465 7374 4361 7365 293a  ttest.TestCase):
-00019f70: 0a20 2020 2040 616e 6e6f 756e 6365 5f74  .    @announce_t
-00019f80: 6573 740a 2020 2020 6465 6620 7465 7374  est.    def test
-00019f90: 5f6e 6f72 6d61 6c69 7a65 5f73 7472 2873  _normalize_str(s
-00019fa0: 656c 6629 3a0a 2020 2020 2020 2020 666f  elf):.        fo
-00019fb0: 7220 696e 5f77 6f72 642c 2065 7870 6563  r in_word, expec
-00019fc0: 7465 645f 776f 7264 2069 6e20 5b0a 2020  ted_word in [.  
-00019fd0: 2020 2020 2020 2020 2020 2822 6e6f 6368            ("noch
-00019fe0: 616e 6765 222c 2022 6e6f 6368 616e 6765  ange", "nochange
-00019ff0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-0001a000: 2822 546f 4c6f 7765 7222 2c20 2274 6f6c  ("ToLower", "tol
-0001a010: 6f77 6572 2229 2c0a 2020 2020 2020 2020  ower"),.        
-0001a020: 2020 2020 2822 492e 422e 4d2e 222c 2022      ("I.B.M.", "
-0001a030: 6962 6d22 292c 0a20 2020 2020 2020 2020  ibm"),.         
-0001a040: 2020 2028 2247 2e45 2e22 2c20 2267 6522     ("G.E.", "ge"
-0001a050: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-0001a060: 224d 2e22 2c20 226d 2229 2c0a 2020 2020  "M.", "m"),.    
-0001a070: 2020 2020 2020 2020 2822 4d2e 7879 7a22          ("M.xyz"
-0001a080: 2c20 226d 2229 2c0a 2020 2020 2020 2020  , "m"),.        
-0001a090: 2020 2020 2822 2a78 7878 2d68 6868 222c      ("*xxx-hhh",
-0001a0a0: 2022 7878 782d 6868 6822 292c 0a20 2020   "xxx-hhh"),.   
-0001a0b0: 2020 2020 2020 2020 2028 222b 626c 6168           ("+blah
-0001a0c0: 466f 6f22 2c20 2262 6c61 6866 6f6f 2229  Foo", "blahfoo")
-0001a0d0: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
-0001a0e0: 2822 666f 7865 7322 2c20 2266 6f78 2229  ("foxes", "fox")
-0001a0f0: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
-0001a100: 2822 6368 7572 6368 6573 222c 2022 6368  ("churches", "ch
-0001a110: 7572 6368 2229 2c0a 2020 2020 2020 2020  urch"),.        
-0001a120: 2020 2020 2320 2822 6472 6573 7365 7322      # ("dresses"
-0001a130: 2c20 2264 7265 7373 2229 2c0a 2020 2020  , "dress"),.    
-0001a140: 2020 2020 5d3a 0a20 2020 2020 2020 2020      ]:.         
-0001a150: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
-0001a160: 5465 7374 2869 6e5f 776f 7264 293a 0a20  Test(in_word):. 
-0001a170: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001a180: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0001a190: 6578 7065 6374 6564 5f77 6f72 642c 206c  expected_word, l
-0001a1a0: 742e 5461 626c 652e 5f6e 6f72 6d61 6c69  t.Table._normali
-0001a1b0: 7a65 5f77 6f72 6428 696e 5f77 6f72 6429  ze_word(in_word)
-0001a1c0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-0001a1d0: 6e6f 726d 616c 697a 655f 7374 725f 6765  normalize_str_ge
-0001a1e0: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
-0001a1f0: 2066 6f72 2069 6e5f 776f 7264 2c20 6578   for in_word, ex
-0001a200: 7065 6374 6564 5f77 6f72 6473 2069 6e20  pected_words in 
-0001a210: 5b0a 2020 2020 2020 2020 2020 2020 2822  [.            ("
-0001a220: 6e6f 6368 616e 6765 222c 205b 226e 6f63  nochange", ["noc
-0001a230: 6861 6e67 6522 5d29 2c0a 2020 2020 2020  hange"]),.      
-0001a240: 2020 2020 2020 2822 546f 4c6f 7765 7222        ("ToLower"
-0001a250: 2c20 5b22 746f 6c6f 7765 7222 5d29 2c0a  , ["tolower"]),.
-0001a260: 2020 2020 2020 2020 2020 2020 2822 492e              ("I.
-0001a270: 422e 4d2e 222c 205b 2269 2e62 2e6d 2e22  B.M.", ["i.b.m."
-0001a280: 2c20 2269 626d 225d 292c 0a20 2020 2020  , "ibm"]),.     
-0001a290: 2020 2020 2020 2028 2247 2e45 2e22 2c20         ("G.E.", 
-0001a2a0: 5b22 672e 652e 222c 2022 6765 225d 292c  ["g.e.", "ge"]),
-0001a2b0: 0a20 2020 2020 2020 2020 2020 2028 2241  .            ("A
-0001a2c0: 2e49 2e22 2c20 5b22 612e 692e 222c 2022  .I.", ["a.i.", "
-0001a2d0: 6169 225d 292c 0a20 2020 2020 2020 2020  ai"]),.         
-0001a2e0: 2020 2028 2241 4922 2c20 5b22 6169 225d     ("AI", ["ai"]
-0001a2f0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-0001a300: 224d 2e22 2c20 5b22 6d22 5d29 2c0a 2020  "M.", ["m"]),.  
-0001a310: 2020 2020 2020 2020 2020 2822 6d6d 2e78            ("mm.x
-0001a320: 797a 222c 205b 226d 6d22 2c20 226d 6d2e  yz", ["mm", "mm.
-0001a330: 7879 7a22 2c20 2278 797a 225d 292c 0a20  xyz", "xyz"]),. 
-0001a340: 2020 2020 2020 2020 2020 2028 224d 4d2e             ("MM.
-0001a350: 7879 7a22 2c20 5b22 6d6d 222c 2022 6d6d  xyz", ["mm", "mm
-0001a360: 2e78 797a 222c 2022 7879 7a22 5d29 2c0a  .xyz", "xyz"]),.
-0001a370: 2020 2020 2020 2020 2020 2020 2822 5468              ("Th
-0001a380: 7265 6164 696e 672e 6973 416c 6976 6528  reading.isAlive(
-0001a390: 2922 2c20 5b27 6973 616c 6976 6527 2c20  )", ['isalive', 
-0001a3a0: 2774 6872 6561 6469 6e67 272c 2027 7468  'threading', 'th
-0001a3b0: 7265 6164 696e 672e 6973 616c 6976 6527  reading.isalive'
-0001a3c0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-0001a3d0: 2822 2a78 7878 2d68 6868 222c 205b 2768  ("*xxx-hhh", ['h
-0001a3e0: 6868 272c 2027 7878 7827 2c20 2778 7878  hh', 'xxx', 'xxx
-0001a3f0: 2d68 6868 275d 292c 0a20 2020 2020 2020  -hhh']),.       
-0001a400: 2020 2020 2028 222b 626c 6168 466f 6f22       ("+blahFoo"
-0001a410: 2c20 5b22 626c 6168 666f 6f22 5d29 2c0a  , ["blahfoo"]),.
-0001a420: 2020 2020 2020 2020 2020 2020 2822 7374              ("st
-0001a430: 722e 6c73 7472 6970 222c 205b 226c 7374  r.lstrip", ["lst
-0001a440: 7269 7022 2c20 2273 7472 222c 2022 7374  rip", "str", "st
-0001a450: 722e 6c73 7472 6970 225d 292c 0a20 2020  r.lstrip"]),.   
-0001a460: 2020 2020 2020 2020 2028 2273 7472 2e6c           ("str.l
-0001a470: 7374 7269 7028 2922 2c20 5b22 6c73 7472  strip()", ["lstr
-0001a480: 6970 222c 2022 7374 7222 2c20 2273 7472  ip", "str", "str
-0001a490: 2e6c 7374 7269 7022 5d29 2c0a 2020 2020  .lstrip"]),.    
-0001a4a0: 2020 2020 2020 2020 2822 7365 6c66 2e61          ("self.a
-0001a4b0: 7373 6572 7445 7175 616c 7322 2c20 5b22  ssertEquals", ["
-0001a4c0: 6173 7365 7274 6571 7561 6c73 222c 2022  assertequals", "
-0001a4d0: 7365 6c66 222c 2022 7365 6c66 2e61 7373  self", "self.ass
-0001a4e0: 6572 7465 7175 616c 7322 5d29 2c0a 2020  ertequals"]),.  
-0001a4f0: 2020 2020 2020 2020 2020 2822 5465 7374            ("Test
-0001a500: 4361 7365 2e61 7373 6572 7445 7175 616c  Case.assertEqual
-0001a510: 7322 2c20 5b22 6173 7365 7274 6571 7561  s", ["assertequa
-0001a520: 6c73 222c 2022 7465 7374 6361 7365 222c  ls", "testcase",
-0001a530: 2022 7465 7374 6361 7365 2e61 7373 6572   "testcase.asser
-0001a540: 7465 7175 616c 7322 5d29 2c0a 2020 2020  tequals"]),.    
-0001a550: 2020 2020 2020 2020 2822 756e 6974 7465          ("unitte
-0001a560: 7374 2e54 6573 7443 6173 652e 6173 7365  st.TestCase.asse
-0001a570: 7274 4571 7561 6c73 222c 0a20 2020 2020  rtEquals",.     
-0001a580: 2020 2020 2020 2020 5b22 6173 7365 7274          ["assert
-0001a590: 6571 7561 6c73 222c 2022 7465 7374 6361  equals", "testca
-0001a5a0: 7365 222c 2022 756e 6974 7465 7374 222c  se", "unittest",
-0001a5b0: 2022 756e 6974 7465 7374 2e74 6573 7463   "unittest.testc
-0001a5c0: 6173 652e 6173 7365 7274 6571 7561 6c73  ase.assertequals
-0001a5d0: 225d 292c 0a20 2020 2020 2020 2020 2020  "]),.           
-0001a5e0: 2028 2266 6f78 6573 222c 205b 2266 6f78   ("foxes", ["fox
-0001a5f0: 222c 2022 666f 7865 7322 5d29 2c0a 2020  ", "foxes"]),.  
-0001a600: 2020 2020 2020 2020 2020 2822 6368 7572            ("chur
-0001a610: 6368 6573 222c 205b 2263 6875 7263 6822  ches", ["church"
-0001a620: 2c20 2263 6875 7263 6865 7322 5d29 2c0a  , "churches"]),.
-0001a630: 2020 2020 2020 2020 2020 2020 2822 6472              ("dr
-0001a640: 6573 7365 7322 2c20 5b22 6472 6573 7322  esses", ["dress"
-0001a650: 2c20 2264 7265 7373 6573 225d 292c 0a20  , "dresses"]),. 
-0001a660: 2020 2020 2020 2020 2020 2028 2264 7265             ("dre
-0001a670: 7373 222c 205b 2264 7265 7373 222c 205d  ss", ["dress", ]
-0001a680: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
-0001a690: 2262 6961 7322 2c20 5b22 6269 6173 222c  "bias", ["bias",
-0001a6a0: 205d 292c 0a20 2020 2020 2020 2020 2020   ]),.           
-0001a6b0: 2028 2274 6f79 7322 2c20 5b22 746f 7922   ("toys", ["toy"
-0001a6c0: 2c20 2274 6f79 7322 5d29 2c0a 2020 2020  , "toys"]),.    
-0001a6d0: 2020 2020 2020 2020 2822 6261 6269 6573          ("babies
-0001a6e0: 222c 205b 2262 6162 6965 7322 2c20 2262  ", ["babies", "b
-0001a6f0: 6162 7922 5d29 2c0a 2020 2020 2020 2020  aby"]),.        
-0001a700: 2020 2020 2822 6164 6465 6e64 6122 2c20      ("addenda", 
-0001a710: 5b22 6164 6465 6e64 6122 2c20 2261 6464  ["addenda", "add
-0001a720: 656e 6475 6d22 5d29 2c0a 2020 2020 2020  endum"]),.      
-0001a730: 2020 2020 2020 2822 7261 6269 6573 222c        ("rabies",
-0001a740: 205b 2272 6162 6965 7322 5d29 2c0a 2020   ["rabies"]),.  
-0001a750: 2020 2020 2020 2020 2020 2822 6c61 7a69            ("lazi
-0001a760: 6e65 7373 222c 205b 226c 617a 696e 6573  ness", ["lazines
-0001a770: 7322 5d29 2c0a 2020 2020 2020 2020 2020  s"]),.          
-0001a780: 2020 2822 7068 7973 6963 7322 2c20 5b22    ("physics", ["
-0001a790: 7068 7973 6963 7322 5d29 2c0a 2020 2020  physics"]),.    
-0001a7a0: 2020 2020 2020 2020 2822 5079 7468 6f6e          ("Python
-0001a7b0: 2773 222c 205b 2270 7974 686f 6e22 5d29  's", ["python"])
-0001a7c0: 2c0a 2020 2020 2020 2020 2020 2020 2827  ,.            ('
-0001a7d0: 5661 6c75 6545 7272 6f72 272c 205b 2765  ValueError', ['e
-0001a7e0: 7272 6f72 272c 2027 7661 6c75 6565 7272  rror', 'valueerr
-0001a7f0: 6f72 275d 292c 0a20 2020 2020 2020 2020  or']),.         
-0001a800: 2020 2028 2744 6570 7265 6361 7469 6f6e     ('Deprecation
-0001a810: 5761 726e 696e 6727 2c20 5b27 6465 7072  Warning', ['depr
-0001a820: 6563 6174 696f 6e77 6172 6e69 6e67 272c  ecationwarning',
-0001a830: 2027 7761 726e 696e 6727 5d29 2c0a 2020   'warning']),.  
-0001a840: 2020 2020 2020 2020 2020 2827 4375 7374            ('Cust
-0001a850: 6f6d 4578 6365 7074 696f 6e27 2c20 5b27  omException', ['
-0001a860: 6375 7374 6f6d 6578 6365 7074 696f 6e27  customexception'
-0001a870: 2c20 2765 7863 6570 7469 6f6e 275d 292c  , 'exception']),
-0001a880: 0a20 2020 2020 2020 205d 3a0a 2020 2020  .        ]:.    
-0001a890: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0001a8a0: 662e 7375 6254 6573 7428 696e 5f77 6f72  f.subTest(in_wor
-0001a8b0: 6429 3a0a 2020 2020 2020 2020 2020 2020  d):.            
-0001a8c0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0001a8d0: 7175 616c 2865 7870 6563 7465 645f 776f  qual(expected_wo
-0001a8e0: 7264 732c 0a20 2020 2020 2020 2020 2020  rds,.           
-0001a8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a900: 2020 2020 2020 736f 7274 6564 286c 6973        sorted(lis
-0001a910: 7428 6c74 2e54 6162 6c65 2e5f 6e6f 726d  t(lt.Table._norm
-0001a920: 616c 697a 655f 776f 7264 5f67 656e 2869  alize_word_gen(i
-0001a930: 6e5f 776f 7264 2c20 6672 6f7a 656e 7365  n_word, frozense
-0001a940: 7428 2929 2929 290a 0a20 2020 2040 616e  t()))))..    @an
-0001a950: 6e6f 756e 6365 5f74 6573 740a 2020 2020  nounce_test.    
-0001a960: 6465 6620 7465 7374 5f6e 6f72 6d61 6c69  def test_normali
-0001a970: 7a65 5f73 706c 6974 2873 656c 6629 3a0a  ze_split(self):.
-0001a980: 2020 2020 2020 2020 666f 7220 696e 5f73          for in_s
-0001a990: 7472 2c20 6578 7065 6374 6564 5f73 7472  tr, expected_str
-0001a9a0: 5f73 6574 2069 6e20 5b0a 2020 2020 2020  _set in [.      
-0001a9b0: 2020 2020 2020 2822 7374 722e 6c73 7472        ("str.lstr
-0001a9c0: 6970 2829 222c 205b 226c 7374 7269 7022  ip()", ["lstrip"
-0001a9d0: 2c20 2273 7472 222c 2022 7374 722e 6c73  , "str", "str.ls
-0001a9e0: 7472 6970 225d 292c 0a20 2020 2020 2020  trip"]),.       
-0001a9f0: 2020 2020 2028 2273 7472 2e6c 7374 7269       ("str.lstri
-0001aa00: 7028 2920 7374 722e 7273 7472 6970 2829  p() str.rstrip()
-0001aa10: 222c 205b 226c 7374 7269 7022 2c20 2272  ", ["lstrip", "r
-0001aa20: 7374 7269 7022 2c20 2273 7472 222c 2022  strip", "str", "
-0001aa30: 7374 722e 6c73 7472 6970 222c 2022 7374  str.lstrip", "st
-0001aa40: 722e 7273 7472 6970 225d 292c 0a20 2020  r.rstrip"]),.   
-0001aa50: 2020 2020 2020 2020 2023 2028 2222 2c20           # ("", 
-0001aa60: 5b5d 292c 0a20 2020 2020 2020 2020 2020  []),.           
-0001aa70: 2023 2028 2222 2c20 5b5d 292c 0a20 2020   # ("", []),.   
-0001aa80: 2020 2020 2020 2020 2023 2028 2222 2c20           # ("", 
-0001aa90: 5b5d 292c 0a20 2020 2020 2020 205d 3a0a  []),.        ]:.
-0001aaa0: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0001aab0: 2073 656c 662e 7375 6254 6573 7428 696e   self.subTest(in
-0001aac0: 5f73 7472 293a 0a20 2020 2020 2020 2020  _str):.         
-0001aad0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0001aae0: 7274 4571 7561 6c28 6578 7065 6374 6564  rtEqual(expected
-0001aaf0: 5f73 7472 5f73 6574 2c0a 2020 2020 2020  _str_set,.      
-0001ab00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab10: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
-0001ab20: 6428 7365 7428 6c74 2e54 6162 6c65 2e5f  d(set(lt.Table._
-0001ab30: 6e6f 726d 616c 697a 655f 7370 6c69 7428  normalize_split(
-0001ab40: 696e 5f73 7472 2929 2929 0a0a 2020 2020  in_str))))..    
-0001ab50: 4061 6e6e 6f75 6e63 655f 7465 7374 0a20  @announce_test. 
-0001ab60: 2020 2064 6566 2074 6573 745f 706c 7572     def test_plur
-0001ab70: 616c 735f 7769 7468 5f74 7261 696c 696e  als_with_trailin
-0001ab80: 675f 7075 6e63 7475 6174 696f 6e28 7365  g_punctuation(se
-0001ab90: 6c66 293a 0a20 2020 2020 2020 2066 6f72  lf):.        for
-0001aba0: 2028 6c69 6e65 2c20 6578 7065 6374 6564   (line, expected
-0001abb0: 2920 696e 205b 0a20 2020 2020 2020 2020  ) in [.         
-0001abc0: 2020 2028 2749 2063 6f75 6c64 2068 6561     ('I could hea
-0001abd0: 7220 7468 6520 6261 6269 6573 2063 7269  r the babies cri
-0001abe0: 6573 2e27 2c20 5b27 6261 6269 6573 272c  es.', ['babies',
-0001abf0: 2027 6261 6279 272c 2027 636f 756c 6427   'baby', 'could'
-0001ac00: 2c20 2763 7269 6573 272c 2027 6372 7927  , 'cries', 'cry'
-0001ac10: 2c20 2768 6561 7227 2c20 2769 272c 2027  , 'hear', 'i', '
-0001ac20: 7468 6527 5d29 2c0a 2020 2020 2020 2020  the']),.        
-0001ac30: 2020 2020 2827 5768 6f20 6172 6520 7468      ('Who are th
-0001ac40: 6f73 6520 6261 6269 6573 3f27 2c20 5b27  ose babies?', ['
-0001ac50: 6172 6527 2c20 2762 6162 6965 7327 2c20  are', 'babies', 
-0001ac60: 2762 6162 7927 2c20 2774 686f 7365 272c  'baby', 'those',
-0001ac70: 2027 7768 6f27 5d29 2c0a 2020 2020 2020   'who']),.      
-0001ac80: 2020 2020 2020 2822 5768 6f20 746f 6f6b        ("Who took
-0001ac90: 2074 6865 2062 6162 6965 7327 2072 6174   the babies' rat
-0001aca0: 746c 6573 2074 6869 7320 7469 6d65 3f22  tles this time?"
-0001acb0: 2c0a 2020 2020 2020 2020 2020 2020 205b  ,.             [
-0001acc0: 2762 6162 6965 7327 2c20 2762 6162 7927  'babies', 'baby'
-0001acd0: 2c20 2772 6174 746c 6527 2c20 2772 6174  , 'rattle', 'rat
-0001ace0: 746c 6573 272c 2027 7468 6527 2c20 2774  tles', 'the', 't
-0001acf0: 6869 7327 2c20 2774 696d 6527 2c20 2774  his', 'time', 't
-0001ad00: 6f6f 6b27 2c20 2777 686f 275d 292c 0a20  ook', 'who']),. 
-0001ad10: 2020 2020 2020 2020 2020 2028 2749 206c             ('I l
-0001ad20: 6f76 6520 7468 6573 6520 6361 6b65 7321  ove these cakes!
-0001ad30: 272c 205b 2763 616b 6527 2c20 2763 616b  ', ['cake', 'cak
-0001ad40: 6573 272c 2027 6927 2c20 276c 6f76 6527  es', 'i', 'love'
-0001ad50: 2c20 2774 6865 7365 275d 292c 0a20 2020  , 'these']),.   
-0001ad60: 2020 2020 2020 2020 2028 2757 6865 6e20           ('When 
-0001ad70: 6d79 2077 6966 6520 636f 6f6b 732c 2073  my wife cooks, s
-0001ad80: 6865 2062 616b 6573 2e27 2c20 5b27 6261  he bakes.', ['ba
-0001ad90: 6b65 272c 2027 6261 6b65 7327 2c20 2763  ke', 'bakes', 'c
-0001ada0: 6f6f 6b27 2c20 2763 6f6f 6b73 272c 2027  ook', 'cooks', '
-0001adb0: 6d79 272c 2027 7368 6527 2c20 2777 6865  my', 'she', 'whe
-0001adc0: 6e27 2c20 2777 6966 6527 5d29 2c0a 2020  n', 'wife']),.  
-0001add0: 2020 2020 2020 2020 2020 2822 4c65 7427            ("Let'
-0001ade0: 7320 676f 2073 686f 7070 696e 6720 666f  s go shopping fo
-0001adf0: 7220 616e 7469 7175 6573 2122 2c20 5b27  r antiques!", ['
-0001ae00: 616e 7469 7175 6527 2c20 2761 6e74 6971  antique', 'antiq
-0001ae10: 7565 7327 2c20 2766 6f72 272c 2027 676f  ues', 'for', 'go
-0001ae20: 272c 2027 6c65 7427 2c20 2773 686f 7070  ', 'let', 'shopp
-0001ae30: 696e 6727 5d29 2c0a 2020 2020 2020 2020  ing']),.        
-0001ae40: 2020 2020 2827 5468 6973 2069 7320 616e      ('This is an
-0001ae50: 2061 6e74 6971 7565 2076 6173 652c 2077   antique vase, w
-0001ae60: 6f72 7468 2074 686f 7573 616e 6473 2127  orth thousands!'
-0001ae70: 2c0a 2020 2020 2020 2020 2020 2020 205b  ,.             [
-0001ae80: 2761 6e27 2c20 2761 6e74 6971 7565 272c  'an', 'antique',
-0001ae90: 2027 6973 272c 2027 7468 6973 272c 2027   'is', 'this', '
-0001aea0: 7468 6f75 7361 6e64 272c 2027 7468 6f75  thousand', 'thou
-0001aeb0: 7361 6e64 7327 2c20 2776 6173 6527 2c20  sands', 'vase', 
-0001aec0: 2777 6f72 7468 275d 292c 0a20 2020 2020  'worth']),.     
-0001aed0: 2020 2020 2020 2028 2757 6865 6e20 7765         ('When we
-0001aee0: 206d 6565 742c 2079 6f75 2061 7265 2061   meet, you are a
-0001aef0: 2067 6961 6e74 2061 6d6f 6e67 206d 656e   giant among men
-0001af00: 2e27 2c0a 2020 2020 2020 2020 2020 2020  .',.            
-0001af10: 205b 2761 272c 2027 616d 6f6e 6727 2c20   ['a', 'among', 
-0001af20: 2761 7265 272c 2027 6769 616e 7427 2c20  'are', 'giant', 
-0001af30: 276d 616e 272c 2027 6d65 6574 272c 2027  'man', 'meet', '
-0001af40: 6d65 6e27 2c20 2777 6527 2c20 2777 6865  men', 'we', 'whe
-0001af50: 6e27 2c20 2779 6f75 275d 292c 0a20 2020  n', 'you']),.   
-0001af60: 2020 2020 2020 2020 2028 2757 6865 6e20           ('When 
-0001af70: 7765 2061 7265 2061 6d6f 6e67 206d 656e  we are among men
-0001af80: 2c20 796f 7520 6172 6520 6120 6769 616e  , you are a gian
-0001af90: 7420 6d65 6174 6261 6c6c 2e27 2c0a 2020  t meatball.',.  
-0001afa0: 2020 2020 2020 2020 2020 205b 2761 272c             ['a',
-0001afb0: 2027 616d 6f6e 6727 2c20 2761 7265 272c   'among', 'are',
-0001afc0: 2027 6172 6527 2c20 2767 6961 6e74 272c   'are', 'giant',
-0001afd0: 2027 6d61 6e27 2c20 276d 6561 7462 616c   'man', 'meatbal
-0001afe0: 6c27 2c20 276d 656e 272c 2027 7765 272c  l', 'men', 'we',
-0001aff0: 2027 7768 656e 272c 2027 796f 7527 5d29   'when', 'you'])
-0001b000: 2c0a 2020 2020 2020 2020 5d3a 0a20 2020  ,.        ]:.   
-0001b010: 2020 2020 2020 2020 2077 6974 6820 7365           with se
-0001b020: 6c66 2e73 7562 5465 7374 286c 696e 6529  lf.subTest(line)
-0001b030: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001b040: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0001b050: 616c 2865 7870 6563 7465 642c 2073 6f72  al(expected, sor
-0001b060: 7465 6428 6c74 2e54 6162 6c65 2e5f 6e6f  ted(lt.Table._no
-0001b070: 726d 616c 697a 655f 7370 6c69 7428 6c69  rmalize_split(li
-0001b080: 6e65 2929 290a 0a0a 6966 205f 5f6e 616d  ne)))...if __nam
-0001b090: 655f 5f20 3d3d 2027 5f5f 6d61 696e 5f5f  e__ == '__main__
-0001b0a0: 273a 0a20 2020 2075 6e69 7474 6573 742e  ':.    unittest.
-0001b0b0: 6d61 696e 2829 0a                        main().
+00013ed0: 2020 2020 2020 2020 2066 696c 7465 7273           filters
+00013ee0: 3d7b 2262 223a 206c 742e 5461 626c 652e  ={"b": lt.Table.
+00013ef0: 6973 5f6e 6f74 5f6e 756c 6c28 297d 290a  is_not_null()}).
+00013f00: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00013f10: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+00013f20: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00013f30: 7365 7274 4571 7561 6c28 332c 206c 656e  sertEqual(3, len
+00013f40: 2878 2929 0a20 2020 2020 2020 2077 6974  (x)).        wit
+00013f50: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00013f60: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00013f70: 6c66 2e61 7373 6572 7445 7175 616c 2833  lf.assertEqual(3
+00013f80: 3030 2c20 7375 6d28 782e 616c 6c2e 6229  00, sum(x.all.b)
+00013f90: 290a 0a20 2020 2020 2020 2070 7269 6e74  )..        print
+00013fa0: 2822 6e61 6d65 2069 735f 6e75 6c6c 2829  ("name is_null()
+00013fb0: 2229 0a20 2020 2020 2020 2078 203d 206c  ").        x = l
+00013fc0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
+00013fd0: 706f 7274 2869 6e70 7574 5f64 6174 612c  port(input_data,
+00013fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014000: 2020 2074 7261 6e73 666f 726d 733d 6469     transforms=di
+00014010: 6374 2e66 726f 6d6b 6579 7328 2261 6263  ct.fromkeys("abc
+00014020: 222c 2069 6e74 292c 0a20 2020 2020 2020  ", int),.       
+00014030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014040: 2020 2020 2020 2020 2020 2066 696c 7465             filte
+00014050: 7273 3d7b 226e 616d 6522 3a20 6c74 2e54  rs={"name": lt.T
+00014060: 6162 6c65 2e69 735f 6e75 6c6c 2829 7d29  able.is_null()})
+00014070: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+00014080: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+00014090: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000140a0: 7373 6572 7445 7175 616c 2831 2c20 6c65  ssertEqual(1, le
+000140b0: 6e28 7829 290a 2020 2020 2020 2020 7769  n(x)).        wi
+000140c0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+000140d0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+000140e0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000140f0: 332a 3939 2c20 785b 305d 2e61 202b 2078  3*99, x[0].a + x
+00014100: 5b30 5d2e 6220 2b20 785b 305d 2e63 290a  [0].b + x[0].c).
+00014110: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+00014120: 6e61 6d65 2069 735f 6e6f 745f 6e75 6c6c  name is_not_null
+00014130: 2829 2229 0a20 2020 2020 2020 2078 203d  ()").        x =
+00014140: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
+00014150: 696d 706f 7274 2869 6e70 7574 5f64 6174  import(input_dat
+00014160: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+00014170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014180: 2020 2020 2074 7261 6e73 666f 726d 733d       transforms=
+00014190: 6469 6374 2e66 726f 6d6b 6579 7328 2261  dict.fromkeys("a
+000141a0: 6263 222c 2069 6e74 292c 0a20 2020 2020  bc", int),.     
+000141b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141c0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+000141d0: 7465 7273 3d7b 226e 616d 6522 3a20 6c74  ters={"name": lt
+000141e0: 2e54 6162 6c65 2e69 735f 6e6f 745f 6e75  .Table.is_not_nu
+000141f0: 6c6c 2829 7d29 0a20 2020 2020 2020 2077  ll()}).        w
+00014200: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00014210: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00014220: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00014230: 2835 2c20 6c65 6e28 7829 290a 2020 2020  (5, len(x)).    
+00014240: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+00014250: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+00014260: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00014270: 4571 7561 6c28 2241 2042 2041 3120 4231  Equal("A B A1 B1
+00014280: 2043 3122 2e73 706c 6974 2829 2c20 6c69   C1".split(), li
+00014290: 7374 2878 2e61 6c6c 2e6e 616d 6529 290a  st(x.all.name)).
+000142a0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+000142b0: 6e61 6d65 2073 7461 7274 7377 6974 6828  name startswith(
+000142c0: 2742 2729 2229 0a20 2020 2020 2020 2078  'B')").        x
+000142d0: 203d 206c 742e 5461 626c 6528 292e 6373   = lt.Table().cs
+000142e0: 765f 696d 706f 7274 2869 6e70 7574 5f64  v_import(input_d
+000142f0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+00014300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014310: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
+00014320: 733d 6469 6374 2e66 726f 6d6b 6579 7328  s=dict.fromkeys(
+00014330: 2261 6263 222c 2069 6e74 292c 0a20 2020  "abc", int),.   
+00014340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014350: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00014360: 696c 7465 7273 3d7b 226e 616d 6522 3a20  ilters={"name": 
+00014370: 6c74 2e54 6162 6c65 2e73 7461 7274 7377  lt.Table.startsw
+00014380: 6974 6828 2242 2229 7d29 0a20 2020 2020  ith("B")}).     
+00014390: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+000143a0: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+000143b0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+000143c0: 7175 616c 2832 2c20 6c65 6e28 7829 290a  qual(2, len(x)).
+000143d0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+000143e0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+000143f0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00014400: 7365 7274 4571 7561 6c28 2242 2042 3122  sertEqual("B B1"
+00014410: 2e73 706c 6974 2829 2c20 6c69 7374 2878  .split(), list(x
+00014420: 2e61 6c6c 2e6e 616d 6529 290a 0a20 2020  .all.name))..   
+00014430: 2020 2020 2070 7269 6e74 2822 6e61 6d65       print("name
+00014440: 2065 6e64 7377 6974 6828 2731 2729 2229   endswith('1')")
+00014450: 0a20 2020 2020 2020 2078 203d 206c 742e  .        x = lt.
+00014460: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
+00014470: 7274 2869 6e70 7574 5f64 6174 612c 0a20  rt(input_data,. 
+00014480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144a0: 2074 7261 6e73 666f 726d 733d 6469 6374   transforms=dict
+000144b0: 2e66 726f 6d6b 6579 7328 2261 6263 222c  .fromkeys("abc",
+000144c0: 2069 6e74 292c 0a20 2020 2020 2020 2020   int),.         
+000144d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144e0: 2020 2020 2020 2020 2066 696c 7465 7273           filters
+000144f0: 3d7b 226e 616d 6522 3a20 6c74 2e54 6162  ={"name": lt.Tab
+00014500: 6c65 2e65 6e64 7377 6974 6828 2231 2229  le.endswith("1")
+00014510: 7d29 0a20 2020 2020 2020 2077 6974 6820  }).        with 
+00014520: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
+00014530: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014540: 2e61 7373 6572 7445 7175 616c 2833 2c20  .assertEqual(3, 
+00014550: 6c65 6e28 7829 290a 2020 2020 2020 2020  len(x)).        
+00014560: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00014570: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+00014580: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00014590: 6c28 2241 3120 4231 2043 3122 2e73 706c  l("A1 B1 C1".spl
+000145a0: 6974 2829 2c20 6c69 7374 2878 2e61 6c6c  it(), list(x.all
+000145b0: 2e6e 616d 6529 290a 0a20 2020 2020 2020  .name))..       
+000145c0: 2070 7269 6e74 2872 226e 616d 6520 7265   print(r"name re
+000145d0: 5f6d 6174 6368 2872 275b 4142 5d5c 6427  _match(r'[AB]\d'
+000145e0: 2922 290a 2020 2020 2020 2020 7820 3d20  )").        x = 
+000145f0: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
+00014600: 6d70 6f72 7428 696e 7075 745f 6461 7461  mport(input_data
+00014610: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014630: 2020 2020 7472 616e 7366 6f72 6d73 3d64      transforms=d
+00014640: 6963 742e 6672 6f6d 6b65 7973 2822 6162  ict.fromkeys("ab
+00014650: 6322 2c20 696e 7429 2c0a 2020 2020 2020  c", int),.      
+00014660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014670: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
+00014680: 6572 733d 7b22 6e61 6d65 223a 206c 742e  ers={"name": lt.
+00014690: 5461 626c 652e 7265 5f6d 6174 6368 2872  Table.re_match(r
+000146a0: 225b 4142 5d5c 6422 297d 290a 2020 2020  "[AB]\d")}).    
+000146b0: 2020 2020 7769 7468 2073 656c 662e 7375      with self.su
+000146c0: 6254 6573 7428 293a 0a20 2020 2020 2020  bTest():.       
+000146d0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000146e0: 4571 7561 6c28 322c 206c 656e 2878 2929  Equal(2, len(x))
+000146f0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+00014700: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+00014710: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00014720: 7373 6572 7445 7175 616c 2822 4131 2042  ssertEqual("A1 B
+00014730: 3122 2e73 706c 6974 2829 2c20 6c69 7374  1".split(), list
+00014740: 2878 2e61 6c6c 2e6e 616d 6529 290a 0a20  (x.all.name)).. 
+00014750: 2020 2064 6566 2074 6573 745f 6373 765f     def test_csv_
+00014760: 7374 7269 6e67 5f69 6d70 6f72 7428 7365  string_import(se
+00014770: 6c66 293a 0a20 2020 2020 2020 2064 6174  lf):.        dat
+00014780: 6120 3d20 6373 765f 6461 7461 0a20 2020  a = csv_data.   
+00014790: 2020 2020 2063 7376 7461 626c 6520 3d20       csvtable = 
+000147a0: 6c74 2e54 6162 6c65 2829 2e63 7376 5f69  lt.Table().csv_i
+000147b0: 6d70 6f72 7428 6373 765f 736f 7572 6365  mport(csv_source
+000147c0: 3d64 6174 612c 2074 7261 6e73 666f 726d  =data, transform
+000147d0: 733d 7b27 6127 3a20 696e 742c 2027 6227  s={'a': int, 'b'
+000147e0: 3a20 696e 742c 2027 6327 3a20 696e 747d  : int, 'c': int}
+000147f0: 290a 0a20 2020 2020 2020 2074 6573 745f  )..        test_
+00014800: 7369 7a65 203d 2033 0a20 2020 2020 2020  size = 3.       
+00014810: 2074 3120 3d20 6d61 6b65 5f74 6573 745f   t1 = make_test_
+00014820: 7461 626c 6528 7365 6c66 2e6d 616b 655f  table(self.make_
+00014830: 6461 7461 5f6f 626a 6563 742c 2074 6573  data_object, tes
+00014840: 745f 7369 7a65 290a 0a20 2020 2020 2020  t_size)..       
+00014850: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+00014860: 7374 2829 3a0a 2020 2020 2020 2020 2020  st():.          
+00014870: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+00014880: 6528 616c 6c28 6d61 6b65 5f64 6174 616f  e(all(make_datao
+00014890: 626a 6563 745f 6672 6f6d 5f6f 6228 7265  bject_from_ob(re
+000148a0: 6331 2920 3d3d 2072 6563 3220 666f 7220  c1) == rec2 for 
+000148b0: 7265 6331 2c20 7265 6332 2069 6e20 7a69  rec1, rec2 in zi
+000148c0: 7028 7431 2c20 6373 7674 6162 6c65 2929  p(t1, csvtable))
+000148d0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+000148e0: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+000148f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014900: 6173 7365 7274 4571 7561 6c28 7375 6d28  assertEqual(sum(
+00014910: 3120 666f 7220 6c69 6e65 2069 6e20 6461  1 for line in da
+00014920: 7461 2e73 706c 6974 6c69 6e65 7328 2920  ta.splitlines() 
+00014930: 6966 206c 696e 652e 7374 7269 7028 2929  if line.strip())
+00014940: 2d31 2c20 6c65 6e28 6373 7674 6162 6c65  -1, len(csvtable
+00014950: 2929 0a0a 2020 2020 2020 2020 726f 775f  ))..        row_
+00014960: 7072 6f74 6f74 7970 6520 3d20 7365 6c66  prototype = self
+00014970: 2e6d 616b 655f 6461 7461 5f6f 626a 6563  .make_data_objec
+00014980: 7428 302c 2030 2c20 3029 0a20 2020 2020  t(0, 0, 0).     
+00014990: 2020 2063 7376 7461 626c 6532 203d 206c     csvtable2 = l
+000149a0: 742e 5461 626c 6528 292e 6373 765f 696d  t.Table().csv_im
+000149b0: 706f 7274 2864 6174 612c 2074 7261 6e73  port(data, trans
+000149c0: 666f 726d 733d 7b27 6127 3a20 696e 742c  forms={'a': int,
+000149d0: 2027 6227 3a20 696e 742c 2027 6327 3a20   'b': int, 'c': 
+000149e0: 696e 747d 2c0a 2020 2020 2020 2020 2020  int},.          
+000149f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a10: 726f 775f 636c 6173 733d 7479 7065 2872  row_class=type(r
+00014a20: 6f77 5f70 726f 746f 7479 7065 2929 5b3a  ow_prototype))[:
+00014a30: 335d 0a0a 2020 2020 2020 2020 7072 696e  3]..        prin
+00014a40: 7428 7479 7065 2874 315b 305d 292e 5f5f  t(type(t1[0]).__
+00014a50: 6e61 6d65 5f5f 2c20 7431 5b30 5d29 0a20  name__, t1[0]). 
+00014a60: 2020 2020 2020 2070 7269 6e74 2874 7970         print(typ
+00014a70: 6528 6373 7674 6162 6c65 325b 305d 292e  e(csvtable2[0]).
+00014a80: 5f5f 6e61 6d65 5f5f 2c20 6373 7674 6162  __name__, csvtab
+00014a90: 6c65 325b 305d 290a 2020 2020 2020 2020  le2[0]).        
+00014aa0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00014ab0: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+00014ac0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00014ad0: 6c28 7479 7065 2874 315b 305d 292c 2074  l(type(t1[0]), t
+00014ae0: 7970 6528 6373 7674 6162 6c65 325b 305d  ype(csvtable2[0]
+00014af0: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
+00014b00: 5f63 7376 5f6c 696d 6974 5f69 6d70 6f72  _csv_limit_impor
+00014b10: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+00014b20: 2064 6174 6120 3d20 6373 765f 6461 7461   data = csv_data
+00014b30: 0a20 2020 2020 2020 2069 6d70 6f72 745f  .        import_
+00014b40: 6c69 6d69 7420 3d20 3130 0a20 2020 2020  limit = 10.     
+00014b50: 2020 2063 7376 7461 626c 6520 3d20 6c74     csvtable = lt
+00014b60: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
+00014b70: 6f72 7428 6373 765f 736f 7572 6365 3d64  ort(csv_source=d
+00014b80: 6174 612c 2074 7261 6e73 666f 726d 733d  ata, transforms=
+00014b90: 7b27 6127 3a20 696e 742c 2027 6227 3a20  {'a': int, 'b': 
+00014ba0: 696e 742c 2027 6327 3a20 696e 747d 2c0a  int, 'c': int},.
+00014bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014bd0: 2020 2020 2020 2020 206c 696d 6974 3d69           limit=i
+00014be0: 6d70 6f72 745f 6c69 6d69 7429 0a0a 2020  mport_limit)..  
+00014bf0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00014c00: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+00014c10: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00014c20: 7274 4571 7561 6c28 696d 706f 7274 5f6c  rtEqual(import_l
+00014c30: 696d 6974 2c20 6c65 6e28 6373 7674 6162  imit, len(csvtab
+00014c40: 6c65 2929 0a0a 2020 2020 2020 2020 6373  le))..        cs
+00014c50: 7674 6162 6c65 203d 206c 742e 5461 626c  vtable = lt.Tabl
+00014c60: 6528 292e 6373 765f 696d 706f 7274 2863  e().csv_import(c
+00014c70: 7376 5f73 6f75 7263 653d 6461 7461 2c20  sv_source=data, 
+00014c80: 7472 616e 7366 6f72 6d73 3d7b 2761 273a  transforms={'a':
+00014c90: 2069 6e74 2c20 2762 273a 2069 6e74 2c20   int, 'b': int, 
+00014ca0: 2763 273a 2069 6e74 7d2c 0a20 2020 2020  'c': int},.     
+00014cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014cd0: 2020 2020 6c69 6d69 743d 3029 0a0a 2020      limit=0)..  
+00014ce0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00014cf0: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+00014d00: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00014d10: 7274 4571 7561 6c28 302c 206c 656e 2863  rtEqual(0, len(c
+00014d20: 7376 7461 626c 6529 290a 0a20 2020 2064  svtable))..    d
+00014d30: 6566 2074 6573 745f 6373 765f 7374 7269  ef test_csv_stri
+00014d40: 6e67 5f6c 6973 745f 696d 706f 7274 2873  ng_list_import(s
+00014d50: 656c 6629 3a0a 2020 2020 2020 2020 6461  elf):.        da
+00014d60: 7461 203d 2063 7376 5f64 6174 610a 2020  ta = csv_data.  
+00014d70: 2020 2020 2020 6373 7674 6162 6c65 203d        csvtable =
+00014d80: 206c 742e 5461 626c 6528 292e 6373 765f   lt.Table().csv_
+00014d90: 696d 706f 7274 2863 7376 5f73 6f75 7263  import(csv_sourc
+00014da0: 653d 6461 7461 2e73 706c 6974 6c69 6e65  e=data.splitline
+00014db0: 7328 292c 2074 7261 6e73 666f 726d 733d  s(), transforms=
+00014dc0: 7b27 6127 3a20 696e 742c 2027 6227 3a20  {'a': int, 'b': 
+00014dd0: 696e 742c 2027 6327 3a20 696e 747d 290a  int, 'c': int}).
+00014de0: 0a20 2020 2020 2020 2074 6573 745f 7369  .        test_si
+00014df0: 7a65 203d 2033 0a20 2020 2020 2020 2074  ze = 3.        t
+00014e00: 3120 3d20 6d61 6b65 5f74 6573 745f 7461  1 = make_test_ta
+00014e10: 626c 6528 7365 6c66 2e6d 616b 655f 6461  ble(self.make_da
+00014e20: 7461 5f6f 626a 6563 742c 2074 6573 745f  ta_object, test_
+00014e30: 7369 7a65 290a 0a20 2020 2020 2020 2077  size)..        w
+00014e40: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00014e50: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00014e60: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
+00014e70: 616c 6c28 6d61 6b65 5f64 6174 616f 626a  all(make_dataobj
+00014e80: 6563 745f 6672 6f6d 5f6f 6228 7265 6331  ect_from_ob(rec1
+00014e90: 2920 3d3d 2072 6563 3220 666f 7220 7265  ) == rec2 for re
+00014ea0: 6331 2c20 7265 6332 2069 6e20 7a69 7028  c1, rec2 in zip(
+00014eb0: 7431 2c20 6373 7674 6162 6c65 2929 290a  t1, csvtable))).
+00014ec0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00014ed0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+00014ee0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00014ef0: 7365 7274 4571 7561 6c28 7375 6d28 3120  sertEqual(sum(1 
+00014f00: 666f 7220 6c69 6e65 2069 6e20 6461 7461  for line in data
+00014f10: 2e73 706c 6974 6c69 6e65 7328 2920 6966  .splitlines() if
+00014f20: 206c 696e 652e 7374 7269 7028 2929 2d31   line.strip())-1
+00014f30: 2c20 6c65 6e28 6373 7674 6162 6c65 2929  , len(csvtable))
+00014f40: 0a0a 2020 2020 2020 2020 726f 775f 7072  ..        row_pr
+00014f50: 6f74 6f74 7970 6520 3d20 7365 6c66 2e6d  ototype = self.m
+00014f60: 616b 655f 6461 7461 5f6f 626a 6563 7428  ake_data_object(
+00014f70: 302c 2030 2c20 3029 0a20 2020 2020 2020  0, 0, 0).       
+00014f80: 2063 7376 7461 626c 6532 203d 206c 742e   csvtable2 = lt.
+00014f90: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
+00014fa0: 7274 2864 6174 612c 2074 7261 6e73 666f  rt(data, transfo
+00014fb0: 726d 733d 7b27 6127 3a20 696e 742c 2027  rms={'a': int, '
+00014fc0: 6227 3a20 696e 742c 2027 6327 3a20 696e  b': int, 'c': in
+00014fd0: 747d 2c0a 2020 2020 2020 2020 2020 2020  t},.            
+00014fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ff0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
+00015000: 775f 636c 6173 733d 7479 7065 2872 6f77  w_class=type(row
+00015010: 5f70 726f 746f 7479 7065 2929 5b3a 335d  _prototype))[:3]
+00015020: 0a0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00015030: 7479 7065 2874 315b 305d 292e 5f5f 6e61  type(t1[0]).__na
+00015040: 6d65 5f5f 2c20 7431 5b30 5d29 0a20 2020  me__, t1[0]).   
+00015050: 2020 2020 2070 7269 6e74 2874 7970 6528       print(type(
+00015060: 6373 7674 6162 6c65 325b 305d 292e 5f5f  csvtable2[0]).__
+00015070: 6e61 6d65 5f5f 2c20 6373 7674 6162 6c65  name__, csvtable
+00015080: 325b 305d 290a 2020 2020 2020 2020 7769  2[0]).        wi
+00015090: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+000150a0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+000150b0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000150c0: 7479 7065 2874 315b 305d 292c 2074 7970  type(t1[0]), typ
+000150d0: 6528 6373 7674 6162 6c65 325b 305d 2929  e(csvtable2[0]))
+000150e0: 0a0a 2020 2020 6465 6620 7465 7374 5f63  ..    def test_c
+000150f0: 7376 5f6e 756d 6572 6963 5f74 7261 6e73  sv_numeric_trans
+00015100: 666f 726d 7328 7365 6c66 293a 0a20 2020  forms(self):.   
+00015110: 2020 2020 2064 6174 6120 3d20 7465 7874       data = text
+00015120: 7772 6170 2e64 6564 656e 7428 2222 225c  wrap.dedent("""\
+00015130: 0a20 2020 2020 2020 2020 2020 2074 7970  .            typ
+00015140: 652c 7661 6c75 650a 2020 2020 2020 2020  e,value.        
+00015150: 2020 2020 696e 742c 3130 3030 0a20 2020      int,1000.   
+00015160: 2020 2020 2020 2020 2066 6c6f 6174 2c33           float,3
+00015170: 2e31 340a 2020 2020 2020 2020 2020 2020  .14.            
+00015180: 656d 7074 792c 0a20 2020 2020 2020 2020  empty,.         
+00015190: 2020 2073 7472 2ce2 93a0 2a62 6572 740a     str,...*bert.
+000151a0: 2020 2020 2020 2020 2020 2020 2222 2229              """)
+000151b0: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
+000151c0: 656c 662e 7375 6254 6573 7428 2263 6f6e  elf.subTest("con
+000151d0: 7665 7274 5f6e 756d 6572 6963 2229 3a0a  vert_numeric"):.
+000151e0: 2020 2020 2020 2020 2020 2020 7462 6c20              tbl 
+000151f0: 3d20 6c74 2e54 6162 6c65 2829 2e63 7376  = lt.Table().csv
+00015200: 5f69 6d70 6f72 7428 6461 7461 2c20 7472  _import(data, tr
+00015210: 616e 7366 6f72 6d73 3d7b 2776 616c 7565  ansforms={'value
+00015220: 273a 206c 742e 5461 626c 652e 636f 6e76  ': lt.Table.conv
+00015230: 6572 745f 6e75 6d65 7269 637d 290a 2020  ert_numeric}).  
+00015240: 2020 2020 2020 2020 2020 7462 6c2e 7072            tbl.pr
+00015250: 6573 656e 7428 290a 2020 2020 2020 2020  esent().        
+00015260: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00015270: 7175 616c 285b 3130 3030 2c20 332e 3134  qual([1000, 3.14
+00015280: 2c20 2727 2c20 27e2 93a0 2a62 6572 7427  , '', '...*bert'
+00015290: 5d2c 206c 6973 7428 7462 6c2e 616c 6c2e  ], list(tbl.all.
+000152a0: 7661 6c75 6529 290a 0a20 2020 2020 2020  value))..       
+000152b0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+000152c0: 7374 2822 636f 6e76 6572 745f 6e75 6d65  st("convert_nume
+000152d0: 7269 6328 2922 293a 0a20 2020 2020 2020  ric()"):.       
+000152e0: 2020 2020 2074 626c 203d 206c 742e 5461       tbl = lt.Ta
+000152f0: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
+00015300: 2864 6174 612c 2074 7261 6e73 666f 726d  (data, transform
+00015310: 733d 7b27 7661 6c75 6527 3a20 6c74 2e54  s={'value': lt.T
+00015320: 6162 6c65 2e63 6f6e 7665 7274 5f6e 756d  able.convert_num
+00015330: 6572 6963 2829 7d29 0a20 2020 2020 2020  eric()}).       
+00015340: 2020 2020 2074 626c 2e70 7265 7365 6e74       tbl.present
+00015350: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00015360: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00015370: 5b31 3030 302c 2033 2e31 342c 2027 272c  [1000, 3.14, '',
+00015380: 2027 e293 a02a 6265 7274 275d 2c20 6c69   '...*bert'], li
+00015390: 7374 2874 626c 2e61 6c6c 2e76 616c 7565  st(tbl.all.value
+000153a0: 2929 0a0a 2020 2020 2020 2020 7769 7468  ))..        with
+000153b0: 2073 656c 662e 7375 6254 6573 7428 2263   self.subTest("c
+000153c0: 6f6e 7665 7274 5f6e 756d 6572 6963 286e  onvert_numeric(n
+000153d0: 6f6e 5f6e 756d 6572 6963 3d4e 6f6e 6529  on_numeric=None)
+000153e0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+000153f0: 7462 6c20 3d20 6c74 2e54 6162 6c65 2829  tbl = lt.Table()
+00015400: 2e63 7376 5f69 6d70 6f72 7428 6461 7461  .csv_import(data
+00015410: 2c20 7472 616e 7366 6f72 6d73 3d7b 2776  , transforms={'v
+00015420: 616c 7565 273a 206c 742e 5461 626c 652e  alue': lt.Table.
+00015430: 636f 6e76 6572 745f 6e75 6d65 7269 6328  convert_numeric(
+00015440: 6e6f 6e5f 6e75 6d65 7269 633d 4e6f 6e65  non_numeric=None
+00015450: 297d 290a 2020 2020 2020 2020 2020 2020  )}).            
+00015460: 7462 6c2e 7072 6573 656e 7428 290a 2020  tbl.present().  
+00015470: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00015480: 7373 6572 7445 7175 616c 285b 3130 3030  ssertEqual([1000
+00015490: 2c20 332e 3134 2c20 2727 2c20 4e6f 6e65  , 3.14, '', None
+000154a0: 5d2c 206c 6973 7428 7462 6c2e 616c 6c2e  ], list(tbl.all.
+000154b0: 7661 6c75 6529 290a 0a20 2020 2020 2020  value))..       
+000154c0: 2077 6974 6820 7365 6c66 2e73 7562 5465   with self.subTe
+000154d0: 7374 2822 636f 6e76 6572 745f 6e75 6d65  st("convert_nume
+000154e0: 7269 6328 6e6f 6e5f 6e75 6d65 7269 633d  ric(non_numeric=
+000154f0: 3029 2229 3a0a 2020 2020 2020 2020 2020  0)"):.          
+00015500: 2020 7462 6c20 3d20 6c74 2e54 6162 6c65    tbl = lt.Table
+00015510: 2829 2e63 7376 5f69 6d70 6f72 7428 6461  ().csv_import(da
+00015520: 7461 2c20 7472 616e 7366 6f72 6d73 3d7b  ta, transforms={
+00015530: 2776 616c 7565 273a 206c 742e 5461 626c  'value': lt.Tabl
+00015540: 652e 636f 6e76 6572 745f 6e75 6d65 7269  e.convert_numeri
+00015550: 6328 6e6f 6e5f 6e75 6d65 7269 633d 3029  c(non_numeric=0)
+00015560: 7d29 0a20 2020 2020 2020 2020 2020 2074  }).            t
+00015570: 626c 2e70 7265 7365 6e74 2829 0a20 2020  bl.present().   
+00015580: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00015590: 7365 7274 4571 7561 6c28 5b31 3030 302c  sertEqual([1000,
+000155a0: 2033 2e31 342c 2027 272c 2030 5d2c 206c   3.14, '', 0], l
+000155b0: 6973 7428 7462 6c2e 616c 6c2e 7661 6c75  ist(tbl.all.valu
+000155c0: 6529 290a 0a20 2020 2020 2020 2077 6974  e))..        wit
+000155d0: 6820 7365 6c66 2e73 7562 5465 7374 2822  h self.subTest("
+000155e0: 636f 6e76 6572 745f 6e75 6d65 7269 6328  convert_numeric(
+000155f0: 696e 745f 746f 5f66 6c6f 6174 3d54 7275  int_to_float=Tru
+00015600: 6529 2229 3a0a 2020 2020 2020 2020 2020  e)"):.          
+00015610: 2020 7462 6c20 3d20 6c74 2e54 6162 6c65    tbl = lt.Table
+00015620: 2829 2e63 7376 5f69 6d70 6f72 7428 6461  ().csv_import(da
+00015630: 7461 2c20 7472 616e 7366 6f72 6d73 3d7b  ta, transforms={
+00015640: 2776 616c 7565 273a 206c 742e 5461 626c  'value': lt.Tabl
+00015650: 652e 636f 6e76 6572 745f 6e75 6d65 7269  e.convert_numeri
+00015660: 6328 666f 7263 655f 666c 6f61 743d 5472  c(force_float=Tr
+00015670: 7565 297d 290a 2020 2020 2020 2020 2020  ue)}).          
+00015680: 2020 7462 6c2e 7072 6573 656e 7428 290a    tbl.present().
+00015690: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000156a0: 2e61 7373 6572 7445 7175 616c 285b 3130  .assertEqual([10
+000156b0: 3030 2e30 2c20 332e 3134 2c20 2727 2c20  00.0, 3.14, '', 
+000156c0: 27e2 93a0 2a62 6572 7427 5d2c 206c 6973  '...*bert'], lis
+000156d0: 7428 7462 6c2e 616c 6c2e 7661 6c75 6529  t(tbl.all.value)
+000156e0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000156f0: 6c66 2e61 7373 6572 7445 7175 616c 285b  lf.assertEqual([
+00015700: 666c 6f61 742c 2066 6c6f 6174 2c20 7374  float, float, st
+00015710: 722c 2073 7472 5d2c 206c 6973 7428 7479  r, str], list(ty
+00015720: 7065 2876 2920 666f 7220 7620 696e 2074  pe(v) for v in t
+00015730: 626c 2e61 6c6c 2e76 616c 7565 2929 0a0a  bl.all.value))..
+00015740: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+00015750: 662e 7375 6254 6573 7428 2263 6f6e 7665  f.subTest("conve
+00015760: 7274 5f6e 756d 6572 6963 286e 6f6e 5f6e  rt_numeric(non_n
+00015770: 756d 6572 6963 3d4e 6f6e 652c 2065 6d70  umeric=None, emp
+00015780: 7479 3d4e 6f6e 6529 2229 3a0a 2020 2020  ty=None)"):.    
+00015790: 2020 2020 2020 2020 7462 6c20 3d20 6c74          tbl = lt
+000157a0: 2e54 6162 6c65 2829 2e63 7376 5f69 6d70  .Table().csv_imp
+000157b0: 6f72 7428 6461 7461 2c20 7472 616e 7366  ort(data, transf
+000157c0: 6f72 6d73 3d7b 2776 616c 7565 273a 206c  orms={'value': l
+000157d0: 742e 5461 626c 652e 636f 6e76 6572 745f  t.Table.convert_
+000157e0: 6e75 6d65 7269 6328 6e6f 6e5f 6e75 6d65  numeric(non_nume
+000157f0: 7269 633d 4e6f 6e65 2c20 656d 7074 793d  ric=None, empty=
+00015800: 4e6f 6e65 297d 290a 2020 2020 2020 2020  None)}).        
+00015810: 2020 2020 7462 6c2e 7072 6573 656e 7428      tbl.present(
+00015820: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00015830: 6c66 2e61 7373 6572 7445 7175 616c 285b  lf.assertEqual([
+00015840: 3130 3030 2c20 332e 3134 2c20 4e6f 6e65  1000, 3.14, None
+00015850: 2c20 4e6f 6e65 5d2c 206c 6973 7428 7462  , None], list(tb
+00015860: 6c2e 616c 6c2e 7661 6c75 6529 290a 0a20  l.all.value)).. 
+00015870: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00015880: 2e73 7562 5465 7374 2822 636f 6e76 6572  .subTest("conver
+00015890: 745f 6e75 6d65 7269 6328 656d 7074 793d  t_numeric(empty=
+000158a0: 4e6f 6e65 2922 293a 0a20 2020 2020 2020  None)"):.       
+000158b0: 2020 2020 2074 626c 203d 206c 742e 5461       tbl = lt.Ta
+000158c0: 626c 6528 292e 6373 765f 696d 706f 7274  ble().csv_import
+000158d0: 2864 6174 612c 2074 7261 6e73 666f 726d  (data, transform
+000158e0: 733d 7b27 7661 6c75 6527 3a20 6c74 2e54  s={'value': lt.T
+000158f0: 6162 6c65 2e63 6f6e 7665 7274 5f6e 756d  able.convert_num
+00015900: 6572 6963 2865 6d70 7479 3d4e 6f6e 6529  eric(empty=None)
+00015910: 7d29 0a20 2020 2020 2020 2020 2020 2074  }).            t
+00015920: 626c 2e70 7265 7365 6e74 2829 0a20 2020  bl.present().   
+00015930: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00015940: 7365 7274 4571 7561 6c28 5b31 3030 302c  sertEqual([1000,
+00015950: 2033 2e31 342c 204e 6f6e 652c 2027 e293   3.14, None, '..
+00015960: a02a 6265 7274 275d 2c20 6c69 7374 2874  .*bert'], list(t
+00015970: 626c 2e61 6c6c 2e76 616c 7565 2929 0a0a  bl.all.value))..
+00015980: 2020 2020 6465 6620 7465 7374 5f6a 736f      def test_jso
+00015990: 6e5f 6578 706f 7274 5f73 7472 6561 6d69  n_export_streami
+000159a0: 6e67 2873 656c 6629 3a0a 2020 2020 2020  ng(self):.      
+000159b0: 2020 6672 6f6d 2069 7465 7274 6f6f 6c73    from itertools
+000159c0: 2069 6d70 6f72 7420 7065 726d 7574 6174   import permutat
+000159d0: 696f 6e73 0a20 2020 2020 2020 2074 6573  ions.        tes
+000159e0: 745f 7369 7a65 203d 2033 0a20 2020 2020  t_size = 3.     
+000159f0: 2020 2074 3120 3d20 6d61 6b65 5f74 6573     t1 = make_tes
+00015a00: 745f 7461 626c 6528 7365 6c66 2e6d 616b  t_table(self.mak
+00015a10: 655f 6461 7461 5f6f 626a 6563 742c 2074  e_data_object, t
+00015a20: 6573 745f 7369 7a65 290a 2020 2020 2020  est_size).      
+00015a30: 2020 666f 7220 6669 656c 646e 616d 6573    for fieldnames
+00015a40: 2069 6e20 7065 726d 7574 6174 696f 6e73   in permutations
+00015a50: 286c 6973 7428 2761 6263 2729 293a 0a20  (list('abc')):. 
+00015a60: 2020 2020 2020 2020 2020 206f 7574 5f73             out_s
+00015a70: 7472 696e 6720 3d20 7431 2e6a 736f 6e5f  tring = t1.json_
+00015a80: 6578 706f 7274 284e 6f6e 652c 2066 6965  export(None, fie
+00015a90: 6c64 6e61 6d65 733d 6669 656c 646e 616d  ldnames=fieldnam
+00015aa0: 6573 2c20 7374 7265 616d 696e 673d 5472  es, streaming=Tr
+00015ab0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+00015ac0: 6f75 746c 696e 6573 203d 206f 7574 5f73  outlines = out_s
+00015ad0: 7472 696e 672e 7370 6c69 746c 696e 6573  tring.splitlines
+00015ae0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+00015af0: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00015b00: 7428 6669 656c 646e 616d 6573 3d66 6965  t(fieldnames=fie
+00015b10: 6c64 6e61 6d65 7329 3a0a 2020 2020 2020  ldnames):.      
+00015b20: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00015b30: 7373 6572 7445 7175 616c 2874 6573 745f  ssertEqual(test_
+00015b40: 7369 7a65 2a2a 332c 206c 656e 286f 7574  size**3, len(out
+00015b50: 6c69 6e65 7329 290a 0a20 2020 2020 2020  lines))..       
+00015b60: 2020 2020 2066 6f72 206f 622c 206c 696e       for ob, lin
+00015b70: 6520 696e 207a 6970 2874 312c 206f 7574  e in zip(t1, out
+00015b80: 6c69 6e65 7329 3a0a 2020 2020 2020 2020  lines):.        
+00015b90: 2020 2020 2020 2020 6a73 6f6e 5f64 6963          json_dic
+00015ba0: 7420 3d20 6a73 6f6e 2e6c 6f61 6473 286c  t = json.loads(l
+00015bb0: 696e 6529 0a20 2020 2020 2020 2020 2020  ine).           
+00015bc0: 2020 2020 2074 315f 6461 7461 6f62 6a20       t1_dataobj 
+00015bd0: 3d20 6d61 6b65 5f64 6174 616f 626a 6563  = make_dataobjec
+00015be0: 745f 6672 6f6d 5f6f 6228 6f62 290a 2020  t_from_ob(ob).  
+00015bf0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+00015c00: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+00015c10: 6f62 3d6f 622c 206c 696e 653d 6c69 6e65  ob=ob, line=line
+00015c20: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00015c30: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00015c40: 7274 4571 7561 6c28 7431 5f64 6174 616f  rtEqual(t1_datao
+00015c50: 626a 2c20 6c74 2e44 6174 614f 626a 6563  bj, lt.DataObjec
+00015c60: 7428 2a2a 6a73 6f6e 5f64 6963 7429 290a  t(**json_dict)).
+00015c70: 0a20 2020 2064 6566 2074 6573 745f 6a73  .    def test_js
+00015c80: 6f6e 5f65 7870 6f72 745f 6e6f 6e73 7472  on_export_nonstr
+00015c90: 6561 6d69 6e67 2873 656c 6629 3a0a 2020  eaming(self):.  
+00015ca0: 2020 2020 2020 6672 6f6d 2069 7465 7274        from itert
+00015cb0: 6f6f 6c73 2069 6d70 6f72 7420 7065 726d  ools import perm
+00015cc0: 7574 6174 696f 6e73 0a20 2020 2020 2020  utations.       
+00015cd0: 2069 6d70 6f72 7420 6a73 6f6e 0a20 2020   import json.   
+00015ce0: 2020 2020 2074 6573 745f 7369 7a65 203d       test_size =
+00015cf0: 2033 0a20 2020 2020 2020 2074 3120 3d20   3.        t1 = 
+00015d00: 6d61 6b65 5f74 6573 745f 7461 626c 6528  make_test_table(
+00015d10: 7365 6c66 2e6d 616b 655f 6461 7461 5f6f  self.make_data_o
+00015d20: 626a 6563 742c 2074 6573 745f 7369 7a65  bject, test_size
+00015d30: 290a 2020 2020 2020 2020 666f 7220 6669  ).        for fi
+00015d40: 656c 646e 616d 6573 2069 6e20 7065 726d  eldnames in perm
+00015d50: 7574 6174 696f 6e73 286c 6973 7428 2761  utations(list('a
+00015d60: 6263 2729 293a 0a20 2020 2020 2020 2020  bc')):.         
+00015d70: 2020 206f 7574 5f73 7472 696e 6720 3d20     out_string = 
+00015d80: 7431 2e6a 736f 6e5f 6578 706f 7274 284e  t1.json_export(N
+00015d90: 6f6e 652c 2066 6965 6c64 6e61 6d65 733d  one, fieldnames=
+00015da0: 6669 656c 646e 616d 6573 2c20 7374 7265  fieldnames, stre
+00015db0: 616d 696e 673d 4661 6c73 6529 0a20 2020  aming=False).   
+00015dc0: 2020 2020 2020 2020 206f 6273 6572 7665           observe
+00015dd0: 645f 6a73 6f6e 203d 206a 736f 6e2e 6c6f  d_json = json.lo
+00015de0: 6164 7328 6f75 745f 7374 7269 6e67 290a  ads(out_string).
+00015df0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00015e00: 6820 7365 6c66 2e73 7562 5465 7374 2866  h self.subTest(f
+00015e10: 6965 6c64 6e61 6d65 733d 6669 656c 646e  ieldnames=fieldn
+00015e20: 616d 6573 293a 0a20 2020 2020 2020 2020  ames):.         
+00015e30: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00015e40: 7274 4571 7561 6c28 7465 7374 5f73 697a  rtEqual(test_siz
+00015e50: 652a 2a33 2c20 6c65 6e28 6f62 7365 7276  e**3, len(observ
+00015e60: 6564 5f6a 736f 6e29 290a 0a20 2020 2020  ed_json))..     
+00015e70: 2020 2020 2020 2066 6f72 206f 622c 206a         for ob, j
+00015e80: 736f 6e5f 6469 6374 2069 6e20 7a69 7028  son_dict in zip(
+00015e90: 7431 2c20 6f62 7365 7276 6564 5f6a 736f  t1, observed_jso
+00015ea0: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
+00015eb0: 2020 2020 7431 5f64 6174 616f 626a 203d      t1_dataobj =
+00015ec0: 206d 616b 655f 6461 7461 6f62 6a65 6374   make_dataobject
+00015ed0: 5f66 726f 6d5f 6f62 286f 6229 0a20 2020  _from_ob(ob).   
+00015ee0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+00015ef0: 6820 7365 6c66 2e73 7562 5465 7374 286f  h self.subTest(o
+00015f00: 623d 6f62 2c20 6a73 6f6e 5f64 6963 743d  b=ob, json_dict=
+00015f10: 6a73 6f6e 5f64 6963 7429 3a0a 2020 2020  json_dict):.    
+00015f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f30: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00015f40: 2874 315f 6461 7461 6f62 6a2c 206c 742e  (t1_dataobj, lt.
+00015f50: 4461 7461 4f62 6a65 6374 282a 2a6a 736f  DataObject(**jso
+00015f60: 6e5f 6469 6374 2929 0a0a 2020 2020 6465  n_dict))..    de
+00015f70: 6620 7465 7374 5f6a 736f 6e5f 696d 706f  f test_json_impo
+00015f80: 7274 2873 656c 6629 3a0a 2020 2020 2020  rt(self):.      
+00015f90: 2020 6461 7461 203d 206a 736f 6e5f 6461    data = json_da
+00015fa0: 7461 0a20 2020 2020 2020 2069 6e6a 736f  ta.        injso
+00015fb0: 6e20 3d20 696f 2e53 7472 696e 6749 4f28  n = io.StringIO(
+00015fc0: 6461 7461 290a 2020 2020 2020 2020 6a73  data).        js
+00015fd0: 6f6e 7461 626c 6520 3d20 6c74 2e54 6162  ontable = lt.Tab
+00015fe0: 6c65 2829 2e6a 736f 6e5f 696d 706f 7274  le().json_import
+00015ff0: 2869 6e6a 736f 6e2c 2073 7472 6561 6d69  (injson, streami
+00016000: 6e67 3d54 7275 652c 2074 7261 6e73 666f  ng=True, transfo
+00016010: 726d 733d 7b27 6127 3a20 696e 742c 2027  rms={'a': int, '
+00016020: 6227 3a20 696e 742c 2027 6327 3a20 696e  b': int, 'c': in
+00016030: 747d 290a 0a20 2020 2020 2020 2074 6573  t})..        tes
+00016040: 745f 7369 7a65 203d 2033 0a20 2020 2020  t_size = 3.     
+00016050: 2020 2074 3120 3d20 6d61 6b65 5f74 6573     t1 = make_tes
+00016060: 745f 7461 626c 6528 7365 6c66 2e6d 616b  t_table(self.mak
+00016070: 655f 6461 7461 5f6f 626a 6563 742c 2074  e_data_object, t
+00016080: 6573 745f 7369 7a65 290a 0a20 2020 2020  est_size)..     
+00016090: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+000160a0: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+000160b0: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+000160c0: 7275 6528 616c 6c28 6d61 6b65 5f64 6174  rue(all(make_dat
+000160d0: 616f 626a 6563 745f 6672 6f6d 5f6f 6228  aobject_from_ob(
+000160e0: 7265 6331 2920 3d3d 2072 6563 3220 666f  rec1) == rec2 fo
+000160f0: 7220 7265 6331 2c20 7265 6332 2069 6e20  r rec1, rec2 in 
+00016100: 7a69 7028 7431 2c20 6a73 6f6e 7461 626c  zip(t1, jsontabl
+00016110: 6529 2929 0a20 2020 2020 2020 2077 6974  e))).        wit
+00016120: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00016130: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00016140: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
+00016150: 656e 285b 6420 666f 7220 6420 696e 2064  en([d for d in d
+00016160: 6174 612e 7370 6c69 746c 696e 6573 2829  ata.splitlines()
+00016170: 2069 6620 642e 7374 7269 7028 295d 292c   if d.strip()]),
+00016180: 206c 656e 286a 736f 6e74 6162 6c65 2929   len(jsontable))
+00016190: 0a0a 2020 2020 6465 6620 7465 7374 5f6a  ..    def test_j
+000161a0: 736f 6e5f 7374 7269 6e67 5f69 6d70 6f72  son_string_impor
+000161b0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+000161c0: 2064 6174 6120 3d20 6a73 6f6e 5f64 6174   data = json_dat
+000161d0: 610a 2020 2020 2020 2020 6a73 6f6e 7461  a.        jsonta
+000161e0: 626c 6520 3d20 6c74 2e54 6162 6c65 2829  ble = lt.Table()
+000161f0: 2e6a 736f 6e5f 696d 706f 7274 2864 6174  .json_import(dat
+00016200: 612c 2073 7472 6561 6d69 6e67 3d54 7275  a, streaming=Tru
+00016210: 652c 2074 7261 6e73 666f 726d 733d 7b27  e, transforms={'
+00016220: 6127 3a20 696e 742c 2027 6227 3a20 696e  a': int, 'b': in
+00016230: 742c 2027 6327 3a20 696e 747d 290a 0a20  t, 'c': int}).. 
+00016240: 2020 2020 2020 2074 6573 745f 7369 7a65         test_size
+00016250: 203d 2033 0a20 2020 2020 2020 2074 3120   = 3.        t1 
+00016260: 3d20 6d61 6b65 5f74 6573 745f 7461 626c  = make_test_tabl
+00016270: 6528 7365 6c66 2e6d 616b 655f 6461 7461  e(self.make_data
+00016280: 5f6f 626a 6563 742c 2074 6573 745f 7369  _object, test_si
+00016290: 7a65 290a 0a20 2020 2020 2020 2077 6974  ze)..        wit
+000162a0: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+000162b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000162c0: 6c66 2e61 7373 6572 7454 7275 6528 616c  lf.assertTrue(al
+000162d0: 6c28 6d61 6b65 5f64 6174 616f 626a 6563  l(make_dataobjec
+000162e0: 745f 6672 6f6d 5f6f 6228 7265 6331 2920  t_from_ob(rec1) 
+000162f0: 3d3d 2072 6563 3220 666f 7220 7265 6331  == rec2 for rec1
+00016300: 2c20 7265 6332 2069 6e20 7a69 7028 7431  , rec2 in zip(t1
+00016310: 2c20 6a73 6f6e 7461 626c 6529 2929 0a20  , jsontable))). 
+00016320: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00016330: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+00016340: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00016350: 6572 7445 7175 616c 286c 656e 285b 6420  ertEqual(len([d 
+00016360: 666f 7220 6420 696e 2064 6174 612e 7370  for d in data.sp
+00016370: 6c69 746c 696e 6573 2829 2069 6620 642e  litlines() if d.
+00016380: 7374 7269 7028 295d 292c 206c 656e 286a  strip()]), len(j
+00016390: 736f 6e74 6162 6c65 2929 0a0a 2020 2020  sontable))..    
+000163a0: 6465 6620 7465 7374 5f6a 736f 6e5f 7374  def test_json_st
+000163b0: 7269 6e67 5f6c 6973 745f 696d 706f 7274  ring_list_import
+000163c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000163d0: 6461 7461 203d 206a 736f 6e5f 6461 7461  data = json_data
+000163e0: 0a20 2020 2020 2020 206a 736f 6e74 6162  .        jsontab
+000163f0: 6c65 203d 206c 742e 5461 626c 6528 292e  le = lt.Table().
+00016400: 6a73 6f6e 5f69 6d70 6f72 7428 6461 7461  json_import(data
+00016410: 2e73 706c 6974 6c69 6e65 7328 292c 2073  .splitlines(), s
+00016420: 7472 6561 6d69 6e67 3d54 7275 652c 2074  treaming=True, t
+00016430: 7261 6e73 666f 726d 733d 7b27 6127 3a20  ransforms={'a': 
+00016440: 696e 742c 2027 6227 3a20 696e 742c 2027  int, 'b': int, '
+00016450: 6327 3a20 696e 747d 290a 0a20 2020 2020  c': int})..     
+00016460: 2020 2074 6573 745f 7369 7a65 203d 2033     test_size = 3
+00016470: 0a20 2020 2020 2020 2074 3120 3d20 6d61  .        t1 = ma
+00016480: 6b65 5f74 6573 745f 7461 626c 6528 7365  ke_test_table(se
+00016490: 6c66 2e6d 616b 655f 6461 7461 5f6f 626a  lf.make_data_obj
+000164a0: 6563 742c 2074 6573 745f 7369 7a65 290a  ect, test_size).
+000164b0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+000164c0: 6c66 2e73 7562 5465 7374 2829 3a0a 2020  lf.subTest():.  
+000164d0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000164e0: 7373 6572 7454 7275 6528 616c 6c28 6d61  ssertTrue(all(ma
+000164f0: 6b65 5f64 6174 616f 626a 6563 745f 6672  ke_dataobject_fr
+00016500: 6f6d 5f6f 6228 7265 6331 2920 3d3d 2072  om_ob(rec1) == r
+00016510: 6563 3220 666f 7220 7265 6331 2c20 7265  ec2 for rec1, re
+00016520: 6332 2069 6e20 7a69 7028 7431 2c20 6a73  c2 in zip(t1, js
+00016530: 6f6e 7461 626c 6529 2929 0a20 2020 2020  ontable))).     
+00016540: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+00016550: 5465 7374 2829 3a0a 2020 2020 2020 2020  Test():.        
+00016560: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00016570: 7175 616c 286c 656e 285b 6420 666f 7220  qual(len([d for 
+00016580: 6420 696e 2064 6174 612e 7370 6c69 746c  d in data.splitl
+00016590: 696e 6573 2829 2069 6620 642e 7374 7269  ines() if d.stri
+000165a0: 7028 295d 292c 206c 656e 286a 736f 6e74  p()]), len(jsont
+000165b0: 6162 6c65 2929 0a0a 2020 2020 6465 6620  able))..    def 
+000165c0: 7465 7374 5f6a 736f 6e5f 6e6f 6e73 7472  test_json_nonstr
+000165d0: 6561 6d69 6e67 5f77 6974 685f 7061 7468  eaming_with_path
+000165e0: 5f69 6d70 6f72 7428 7365 6c66 293a 0a20  _import(self):. 
+000165f0: 2020 2020 2020 2064 6174 6120 3d20 6a73         data = js
+00016600: 6f6e 5f64 6174 610a 2020 2020 2020 2020  on_data.        
+00016610: 6461 7461 203d 2027 2c5c 6e27 2e6a 6f69  data = ',\n'.joi
+00016620: 6e28 6461 7461 2e72 7374 7269 7028 292e  n(data.rstrip().
+00016630: 7370 6c69 746c 696e 6573 2829 290a 2020  splitlines()).  
+00016640: 2020 2020 2020 6a73 6f6e 5f69 6e70 7574        json_input
+00016650: 3020 3d20 275b 2720 2b20 6461 7461 202b  0 = '[' + data +
+00016660: 2027 5d27 0a20 2020 2020 2020 206a 736f   ']'.        jso
+00016670: 6e5f 696e 7075 7431 203d 2027 7b20 2264  n_input1 = '{ "d
+00016680: 6174 6122 3a20 5b27 202b 2064 6174 6120  ata": [' + data 
+00016690: 2b20 275d 7d27 0a20 2020 2020 2020 206a  + ']}'.        j
+000166a0: 736f 6e5f 696e 7075 7432 203d 2027 7b20  son_input2 = '{ 
+000166b0: 2264 6174 6122 3a20 7b20 2269 7465 6d73  "data": { "items
+000166c0: 223a 205b 2720 2b20 6461 7461 202b 2027  ": [' + data + '
+000166d0: 5d7d 7d27 0a0a 2020 2020 2020 2020 666f  ]}}'..        fo
+000166e0: 7220 6a73 6f6e 5f69 6e70 7574 2c20 7061  r json_input, pa
+000166f0: 7468 2069 6e20 5b0a 2020 2020 2020 2020  th in [.        
+00016700: 2020 2020 286a 736f 6e5f 696e 7075 7430      (json_input0
+00016710: 2c20 2222 292c 0a20 2020 2020 2020 2020  , ""),.         
+00016720: 2020 2028 6a73 6f6e 5f69 6e70 7574 312c     (json_input1,
+00016730: 2022 6461 7461 2229 2c0a 2020 2020 2020   "data"),.      
+00016740: 2020 2020 2020 286a 736f 6e5f 696e 7075        (json_inpu
+00016750: 7432 2c20 2264 6174 612e 6974 656d 7322  t2, "data.items"
+00016760: 292c 0a20 2020 2020 2020 205d 3a0a 2020  ),.        ]:.  
+00016770: 2020 2020 2020 2020 2020 6a73 6f6e 7461            jsonta
+00016780: 626c 6520 3d20 6c74 2e54 6162 6c65 2829  ble = lt.Table()
+00016790: 2e6a 736f 6e5f 696d 706f 7274 286a 736f  .json_import(jso
+000167a0: 6e5f 696e 7075 742c 0a20 2020 2020 2020  n_input,.       
+000167b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000167c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000167d0: 2020 2020 2020 2020 7061 7468 3d70 6174          path=pat
+000167e0: 682c 0a20 2020 2020 2020 2020 2020 2020  h,.             
+000167f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016810: 2020 7472 616e 7366 6f72 6d73 3d7b 2761    transforms={'a
+00016820: 273a 2069 6e74 2c20 2762 273a 2069 6e74  ': int, 'b': int
+00016830: 2c20 2763 273a 2069 6e74 7d29 0a0a 2020  , 'c': int})..  
+00016840: 2020 2020 2020 2020 2020 7465 7374 5f73            test_s
+00016850: 697a 6520 3d20 330a 2020 2020 2020 2020  ize = 3.        
+00016860: 2020 2020 7431 203d 206d 616b 655f 7465      t1 = make_te
+00016870: 7374 5f74 6162 6c65 2873 656c 662e 6d61  st_table(self.ma
+00016880: 6b65 5f64 6174 615f 6f62 6a65 6374 2c20  ke_data_object, 
+00016890: 7465 7374 5f73 697a 6529 0a0a 2020 2020  test_size)..    
+000168a0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+000168b0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+000168c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000168d0: 662e 6173 7365 7274 5472 7565 2861 6c6c  f.assertTrue(all
+000168e0: 286d 616b 655f 6461 7461 6f62 6a65 6374  (make_dataobject
+000168f0: 5f66 726f 6d5f 6f62 2872 6563 3129 203d  _from_ob(rec1) =
+00016900: 3d20 7265 6332 2066 6f72 2072 6563 312c  = rec2 for rec1,
+00016910: 2072 6563 3220 696e 207a 6970 2874 312c   rec2 in zip(t1,
+00016920: 206a 736f 6e74 6162 6c65 2929 290a 2020   jsontable))).  
+00016930: 2020 2020 2020 2020 2020 7769 7468 2073            with s
+00016940: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+00016950: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016960: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00016970: 6c65 6e28 5b64 2066 6f72 2064 2069 6e20  len([d for d in 
+00016980: 6461 7461 2e73 706c 6974 6c69 6e65 7328  data.splitlines(
+00016990: 2920 6966 2064 2e73 7472 6970 2829 5d29  ) if d.strip()])
+000169a0: 2c20 6c65 6e28 6a73 6f6e 7461 626c 6529  , len(jsontable)
+000169b0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+000169c0: 6a73 6f6e 5f69 6d70 6f72 745f 7769 7468  json_import_with
+000169d0: 5f63 7573 746f 6d5f 656e 636f 6465 7228  _custom_encoder(
+000169e0: 7365 6c66 293a 0a20 2020 2020 2020 2066  self):.        f
+000169f0: 726f 6d20 6461 7465 7469 6d65 2069 6d70  rom datetime imp
+00016a00: 6f72 7420 6461 7465 0a20 2020 2020 2020  ort date.       
+00016a10: 2064 6174 6120 3d20 5b0a 2020 2020 2020   data = [.      
+00016a20: 2020 2020 2020 7b27 6127 3a20 3130 302c        {'a': 100,
+00016a30: 2027 6227 3a20 6461 7465 2832 3030 302c   'b': date(2000,
+00016a40: 2031 2c20 3129 2c20 2763 273a 2032 3030   1, 1), 'c': 200
+00016a50: 7d2c 0a20 2020 2020 2020 2020 2020 207b  },.            {
+00016a60: 2761 273a 2031 3031 2c20 2762 273a 2064  'a': 101, 'b': d
+00016a70: 6174 6528 3230 3031 2c20 312c 2031 292c  ate(2001, 1, 1),
+00016a80: 2027 6327 3a20 3230 317d 2c0a 2020 2020   'c': 201},.    
+00016a90: 2020 2020 5d0a 2020 2020 2020 2020 7462      ].        tb
+00016aa0: 6c20 3d20 6c74 2e54 6162 6c65 2829 2e69  l = lt.Table().i
+00016ab0: 6e73 6572 745f 6d61 6e79 2864 6174 6129  nsert_many(data)
+00016ac0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+00016ad0: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
+00016ae0: 5479 7065 4572 726f 7229 3a0a 2020 2020  TypeError):.    
+00016af0: 2020 2020 2020 2020 7820 3d20 7462 6c2e          x = tbl.
+00016b00: 6a73 6f6e 5f65 7870 6f72 7428 290a 0a20  json_export().. 
+00016b10: 2020 2020 2020 2063 6c61 7373 204a 736f         class Jso
+00016b20: 6e44 6174 6545 6e63 6f64 6572 286a 736f  nDateEncoder(jso
+00016b30: 6e2e 4a53 4f4e 456e 636f 6465 7229 3a0a  n.JSONEncoder):.
+00016b40: 2020 2020 2020 2020 2020 2020 6465 6620              def 
+00016b50: 6465 6661 756c 7428 7365 6c66 2c20 6f29  default(self, o)
+00016b60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016b70: 2020 696d 706f 7274 2064 6174 6574 696d    import datetim
+00016b80: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00016b90: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00016ba0: 6f2c 2064 6174 6574 696d 652e 6461 7465  o, datetime.date
+00016bb0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00016bc0: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
+00016bd0: 7228 6f29 0a20 2020 2020 2020 2020 2020  r(o).           
+00016be0: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+00016bf0: 7228 292e 6465 6661 756c 7428 6f29 0a0a  r().default(o)..
+00016c00: 2020 2020 2020 2020 6578 7065 6374 6564          expected
+00016c10: 203d 2074 6578 7477 7261 702e 6465 6465   = textwrap.dede
+00016c20: 6e74 2822 2222 5c0a 2020 2020 2020 2020  nt("""\.        
+00016c30: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+00016c40: 2020 7b22 6122 3a20 3130 302c 2022 6222    {"a": 100, "b"
+00016c50: 3a20 2232 3030 302d 3031 2d30 3122 2c20  : "2000-01-01", 
+00016c60: 2263 223a 2032 3030 7d2c 0a20 2020 2020  "c": 200},.     
+00016c70: 2020 2020 2020 207b 2261 223a 2031 3031         {"a": 101
+00016c80: 2c20 2262 223a 2022 3230 3031 2d30 312d  , "b": "2001-01-
+00016c90: 3031 222c 2022 6322 3a20 3230 317d 0a20  01", "c": 201}. 
+00016ca0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+00016cb0: 2020 2020 2020 2020 2022 2222 290a 2020           """).  
+00016cc0: 2020 2020 2020 6a73 6f6e 5f72 6573 756c        json_resul
+00016cd0: 7420 3d20 7462 6c2e 6a73 6f6e 5f65 7870  t = tbl.json_exp
+00016ce0: 6f72 7428 6a73 6f6e 5f65 6e63 6f64 6572  ort(json_encoder
+00016cf0: 3d4a 736f 6e44 6174 6545 6e63 6f64 6572  =JsonDateEncoder
+00016d00: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00016d10: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
+00016d20: 7465 642c 206a 736f 6e5f 7265 7375 6c74  ted, json_result
+00016d30: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+00016d40: 6a73 6f6e 5f69 6d70 6f72 745f 7769 7468  json_import_with
+00016d50: 5f6d 756c 7469 706c 655f 6375 7374 6f6d  _multiple_custom
+00016d60: 5f65 6e63 6f64 6572 7328 7365 6c66 293a  _encoders(self):
+00016d70: 0a20 2020 2020 2020 2066 726f 6d20 6461  .        from da
+00016d80: 7465 7469 6d65 2069 6d70 6f72 7420 6461  tetime import da
+00016d90: 7465 0a0a 2020 2020 2020 2020 636c 6173  te..        clas
+00016da0: 7320 4141 413a 0a20 2020 2020 2020 2020  s AAA:.         
+00016db0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00016dc0: 7365 6c66 2c20 6e61 6d65 293a 0a20 2020  self, name):.   
+00016dd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016de0: 662e 6e61 6d65 203d 206e 616d 650a 0a20  f.name = name.. 
+00016df0: 2020 2020 2020 2064 6174 6120 3d20 5b0a         data = [.
+00016e00: 2020 2020 2020 2020 2020 2020 7b27 6127              {'a'
+00016e10: 3a20 3130 302c 2027 6227 3a20 6461 7465  : 100, 'b': date
+00016e20: 2832 3030 302c 2031 2c20 3129 2c20 2763  (2000, 1, 1), 'c
+00016e30: 273a 2032 3030 2c20 2764 273a 2041 4141  ': 200, 'd': AAA
+00016e40: 2822 416c 6963 6522 297d 2c0a 2020 2020  ("Alice")},.    
+00016e50: 2020 2020 2020 2020 7b27 6127 3a20 3130          {'a': 10
+00016e60: 312c 2027 6227 3a20 6461 7465 2832 3030  1, 'b': date(200
+00016e70: 312c 2031 2c20 3129 2c20 2763 273a 2032  1, 1, 1), 'c': 2
+00016e80: 3031 2c20 2764 273a 2041 4141 2822 426f  01, 'd': AAA("Bo
+00016e90: 6222 297d 2c0a 2020 2020 2020 2020 5d0a  b")},.        ].
+00016ea0: 2020 2020 2020 2020 7462 6c20 3d20 6c74          tbl = lt
+00016eb0: 2e54 6162 6c65 2829 2e69 6e73 6572 745f  .Table().insert_
+00016ec0: 6d61 6e79 2864 6174 6129 0a20 2020 2020  many(data).     
+00016ed0: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
+00016ee0: 6572 7452 6169 7365 7328 5479 7065 4572  ertRaises(TypeEr
+00016ef0: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
+00016f00: 2020 7820 3d20 7462 6c2e 6a73 6f6e 5f65    x = tbl.json_e
+00016f10: 7870 6f72 7428 290a 0a20 2020 2020 2020  xport()..       
+00016f20: 2063 6c61 7373 204a 736f 6e44 6174 6545   class JsonDateE
+00016f30: 6e63 6f64 6572 286a 736f 6e2e 4a53 4f4e  ncoder(json.JSON
+00016f40: 456e 636f 6465 7229 3a0a 2020 2020 2020  Encoder):.      
+00016f50: 2020 2020 2020 6465 6620 6465 6661 756c        def defaul
+00016f60: 7428 7365 6c66 2c20 6f29 3a0a 2020 2020  t(self, o):.    
+00016f70: 2020 2020 2020 2020 2020 2020 696d 706f              impo
+00016f80: 7274 2064 6174 6574 696d 650a 2020 2020  rt datetime.    
+00016f90: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00016fa0: 7369 6e73 7461 6e63 6528 6f2c 2064 6174  sinstance(o, dat
+00016fb0: 6574 696d 652e 6461 7465 293a 0a20 2020  etime.date):.   
+00016fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fd0: 2072 6574 7572 6e20 7374 7228 6f29 0a20   return str(o). 
+00016fe0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00016ff0: 6574 7572 6e20 7375 7065 7228 292e 6465  eturn super().de
+00017000: 6661 756c 7428 6f29 0a0a 2020 2020 2020  fault(o)..      
+00017010: 2020 636c 6173 7320 4a73 6f6e 4141 4145    class JsonAAAE
+00017020: 6e63 6f64 6572 286a 736f 6e2e 4a53 4f4e  ncoder(json.JSON
+00017030: 456e 636f 6465 7229 3a0a 2020 2020 2020  Encoder):.      
+00017040: 2020 2020 2020 6465 6620 6465 6661 756c        def defaul
+00017050: 7428 7365 6c66 2c20 6f29 3a0a 2020 2020  t(self, o):.    
+00017060: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00017070: 7369 6e73 7461 6e63 6528 6f2c 2041 4141  sinstance(o, AAA
+00017080: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00017090: 2020 2020 2020 2072 6574 7572 6e20 6622         return f"
+000170a0: 4141 4128 6e61 6d65 3d7b 6f2e 6e61 6d65  AAA(name={o.name
+000170b0: 2172 7d29 220a 0a20 2020 2020 2020 2065  !r})"..        e
+000170c0: 7870 6563 7465 6420 3d20 7465 7874 7772  xpected = textwr
+000170d0: 6170 2e64 6564 656e 7428 2222 225c 0a20  ap.dedent("""\. 
+000170e0: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
+000170f0: 2020 2020 2020 2020 207b 2261 223a 2031           {"a": 1
+00017100: 3030 2c20 2262 223a 2022 3230 3030 2d30  00, "b": "2000-0
+00017110: 312d 3031 222c 2022 6322 3a20 3230 302c  1-01", "c": 200,
+00017120: 2022 6422 3a20 2241 4141 286e 616d 653d   "d": "AAA(name=
+00017130: 2741 6c69 6365 2729 227d 2c0a 2020 2020  'Alice')"},.    
+00017140: 2020 2020 2020 2020 7b22 6122 3a20 3130          {"a": 10
+00017150: 312c 2022 6222 3a20 2232 3030 312d 3031  1, "b": "2001-01
+00017160: 2d30 3122 2c20 2263 223a 2032 3031 2c20  -01", "c": 201, 
+00017170: 2264 223a 2022 4141 4128 6e61 6d65 3d27  "d": "AAA(name='
+00017180: 426f 6227 2922 7d0a 2020 2020 2020 2020  Bob')"}.        
+00017190: 2020 2020 5d0a 2020 2020 2020 2020 2222      ].        ""
+000171a0: 2229 0a0a 2020 2020 2020 2020 6a73 6f6e  ")..        json
+000171b0: 5f72 6573 756c 7420 3d20 7462 6c2e 6a73  _result = tbl.js
+000171c0: 6f6e 5f65 7870 6f72 7428 6a73 6f6e 5f65  on_export(json_e
+000171d0: 6e63 6f64 6572 3d28 4a73 6f6e 4461 7465  ncoder=(JsonDate
+000171e0: 456e 636f 6465 722c 204a 736f 6e41 4141  Encoder, JsonAAA
+000171f0: 456e 636f 6465 7229 290a 2020 2020 2020  Encoder)).      
+00017200: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00017210: 616c 2865 7870 6563 7465 642c 206a 736f  al(expected, jso
+00017220: 6e5f 7265 7375 6c74 290a 0a20 2020 2064  n_result)..    d
+00017230: 6566 2074 6573 745f 6669 7865 645f 7769  ef test_fixed_wi
+00017240: 6474 685f 696d 706f 7274 2873 656c 6629  dth_import(self)
+00017250: 3a0a 2020 2020 2020 2020 6461 7461 203d  :.        data =
+00017260: 2066 6978 6564 5f77 6964 7468 5f64 6174   fixed_width_dat
+00017270: 610a 2020 2020 2020 2020 6461 7461 5f66  a.        data_f
+00017280: 696c 6520 3d20 696f 2e53 7472 696e 6749  ile = io.StringI
+00017290: 4f28 6461 7461 290a 2020 2020 2020 2020  O(data).        
+000172a0: 6677 5f73 7065 6320 3d20 5b28 2761 272c  fw_spec = [('a',
+000172b0: 2030 2c20 4e6f 6e65 2c20 696e 7429 2c20   0, None, int), 
+000172c0: 2827 6227 2c20 322c 204e 6f6e 652c 2069  ('b', 2, None, i
+000172d0: 6e74 292c 2028 2763 272c 2034 2c20 4e6f  nt), ('c', 4, No
+000172e0: 6e65 2c20 696e 7429 2c20 5d0a 2020 2020  ne, int), ].    
+000172f0: 2020 2020 7474 203d 206c 742e 5461 626c      tt = lt.Tabl
+00017300: 6528 292e 696e 7365 7274 5f6d 616e 7928  e().insert_many(
+00017310: 6c74 2e44 6174 614f 626a 6563 7428 2a2a  lt.DataObject(**
+00017320: 7265 6329 2066 6f72 2072 6563 2069 6e20  rec) for rec in 
+00017330: 6c74 2e46 6978 6564 5769 6474 6852 6561  lt.FixedWidthRea
+00017340: 6465 7228 6677 5f73 7065 632c 2064 6174  der(fw_spec, dat
+00017350: 615f 6669 6c65 2929 0a0a 2020 2020 2020  a_file))..      
+00017360: 2020 7465 7374 5f73 697a 6520 3d20 330a    test_size = 3.
+00017370: 2020 2020 2020 2020 7431 203d 206d 616b          t1 = mak
+00017380: 655f 7465 7374 5f74 6162 6c65 2873 656c  e_test_table(sel
+00017390: 662e 6d61 6b65 5f64 6174 615f 6f62 6a65  f.make_data_obje
+000173a0: 6374 2c20 7465 7374 5f73 697a 6529 0a0a  ct, test_size)..
+000173b0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+000173c0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+000173d0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+000173e0: 7365 7274 5472 7565 2861 6c6c 286d 616b  sertTrue(all(mak
+000173f0: 655f 6461 7461 6f62 6a65 6374 5f66 726f  e_dataobject_fro
+00017400: 6d5f 6f62 2872 6563 3129 203d 3d20 7265  m_ob(rec1) == re
+00017410: 6332 2066 6f72 2072 6563 312c 2072 6563  c2 for rec1, rec
+00017420: 3220 696e 207a 6970 2874 312c 2074 7429  2 in zip(t1, tt)
+00017430: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
+00017440: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
+00017450: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017460: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
+00017470: 285b 6420 666f 7220 6420 696e 2064 6174  ([d for d in dat
+00017480: 612e 7370 6c69 746c 696e 6573 2829 2069  a.splitlines() i
+00017490: 6620 642e 7374 7269 7028 295d 292c 206c  f d.strip()]), l
+000174a0: 656e 2874 7429 290a 0a20 2020 2064 6566  en(tt))..    def
+000174b0: 2074 6573 745f 6669 7865 645f 7769 6474   test_fixed_widt
+000174c0: 685f 7374 7269 6e67 5f69 6d70 6f72 7428  h_string_import(
+000174d0: 7365 6c66 293a 0a20 2020 2020 2020 2064  self):.        d
+000174e0: 6174 6120 3d20 6669 7865 645f 7769 6474  ata = fixed_widt
+000174f0: 685f 6461 7461 0a20 2020 2020 2020 2066  h_data.        f
+00017500: 775f 7370 6563 203d 205b 2827 6127 2c20  w_spec = [('a', 
+00017510: 302c 204e 6f6e 652c 2069 6e74 292c 2028  0, None, int), (
+00017520: 2762 272c 2032 2c20 4e6f 6e65 2c20 696e  'b', 2, None, in
+00017530: 7429 2c20 2827 6327 2c20 342c 204e 6f6e  t), ('c', 4, Non
+00017540: 652c 2069 6e74 292c 205d 0a20 2020 2020  e, int), ].     
+00017550: 2020 2074 7420 3d20 6c74 2e54 6162 6c65     tt = lt.Table
+00017560: 2829 2e69 6e73 6572 745f 6d61 6e79 286c  ().insert_many(l
+00017570: 742e 4461 7461 4f62 6a65 6374 282a 2a72  t.DataObject(**r
+00017580: 6563 2920 666f 7220 7265 6320 696e 206c  ec) for rec in l
+00017590: 742e 4669 7865 6457 6964 7468 5265 6164  t.FixedWidthRead
+000175a0: 6572 2866 775f 7370 6563 2c20 6461 7461  er(fw_spec, data
+000175b0: 2929 0a0a 2020 2020 2020 2020 7465 7374  ))..        test
+000175c0: 5f73 697a 6520 3d20 330a 2020 2020 2020  _size = 3.      
+000175d0: 2020 7431 203d 206d 616b 655f 7465 7374    t1 = make_test
+000175e0: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
+000175f0: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
+00017600: 7374 5f73 697a 6529 0a0a 2020 2020 2020  st_size)..      
+00017610: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00017620: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00017630: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+00017640: 7565 2861 6c6c 286d 616b 655f 6461 7461  ue(all(make_data
+00017650: 6f62 6a65 6374 5f66 726f 6d5f 6f62 2872  object_from_ob(r
+00017660: 6563 3129 203d 3d20 7265 6332 2066 6f72  ec1) == rec2 for
+00017670: 2072 6563 312c 2072 6563 3220 696e 207a   rec1, rec2 in z
+00017680: 6970 2874 312c 2074 7429 2929 0a20 2020  ip(t1, tt))).   
+00017690: 2020 2020 2077 6974 6820 7365 6c66 2e73       with self.s
+000176a0: 7562 5465 7374 2829 3a0a 2020 2020 2020  ubTest():.      
+000176b0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000176c0: 7445 7175 616c 286c 656e 285b 6420 666f  tEqual(len([d fo
+000176d0: 7220 6420 696e 2064 6174 612e 7370 6c69  r d in data.spli
+000176e0: 746c 696e 6573 2829 2069 6620 642e 7374  tlines() if d.st
+000176f0: 7269 7028 295d 292c 206c 656e 2874 7429  rip()]), len(tt)
+00017700: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+00017710: 6669 7865 645f 7769 6474 685f 7374 7269  fixed_width_stri
+00017720: 6e67 5f6c 6973 745f 696d 706f 7274 2873  ng_list_import(s
+00017730: 656c 6629 3a0a 2020 2020 2020 2020 6461  elf):.        da
+00017740: 7461 203d 2066 6978 6564 5f77 6964 7468  ta = fixed_width
+00017750: 5f64 6174 610a 2020 2020 2020 2020 6677  _data.        fw
+00017760: 5f73 7065 6320 3d20 5b28 2761 272c 2030  _spec = [('a', 0
+00017770: 2c20 4e6f 6e65 2c20 696e 7429 2c20 2827  , None, int), ('
+00017780: 6227 2c20 322c 204e 6f6e 652c 2069 6e74  b', 2, None, int
+00017790: 292c 2028 2763 272c 2034 2c20 4e6f 6e65  ), ('c', 4, None
+000177a0: 2c20 696e 7429 2c5d 0a20 2020 2020 2020  , int),].       
+000177b0: 2074 7420 3d20 6c74 2e54 6162 6c65 2829   tt = lt.Table()
+000177c0: 2e69 6e73 6572 745f 6d61 6e79 286c 742e  .insert_many(lt.
+000177d0: 4461 7461 4f62 6a65 6374 282a 2a72 6563  DataObject(**rec
+000177e0: 2920 666f 7220 7265 6320 696e 206c 742e  ) for rec in lt.
+000177f0: 4669 7865 6457 6964 7468 5265 6164 6572  FixedWidthReader
+00017800: 2866 775f 7370 6563 2c20 6461 7461 2e73  (fw_spec, data.s
+00017810: 706c 6974 6c69 6e65 7328 2929 290a 0a20  plitlines())).. 
+00017820: 2020 2020 2020 2074 6573 745f 7369 7a65         test_size
+00017830: 203d 2033 0a20 2020 2020 2020 2074 3120   = 3.        t1 
+00017840: 3d20 6d61 6b65 5f74 6573 745f 7461 626c  = make_test_tabl
+00017850: 6528 7365 6c66 2e6d 616b 655f 6461 7461  e(self.make_data
+00017860: 5f6f 626a 6563 742c 2074 6573 745f 7369  _object, test_si
+00017870: 7a65 290a 0a20 2020 2020 2020 2077 6974  ze)..        wit
+00017880: 6820 7365 6c66 2e73 7562 5465 7374 2829  h self.subTest()
+00017890: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000178a0: 6c66 2e61 7373 6572 7454 7275 6528 616c  lf.assertTrue(al
+000178b0: 6c28 6d61 6b65 5f64 6174 616f 626a 6563  l(make_dataobjec
+000178c0: 745f 6672 6f6d 5f6f 6228 7265 6331 2920  t_from_ob(rec1) 
+000178d0: 3d3d 2072 6563 3220 666f 7220 7265 6331  == rec2 for rec1
+000178e0: 2c20 7265 6332 2069 6e20 7a69 7028 7431  , rec2 in zip(t1
+000178f0: 2c20 7474 2929 290a 2020 2020 2020 2020  , tt))).        
+00017900: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00017910: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+00017920: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00017930: 6c28 6c65 6e28 5b64 2066 6f72 2064 2069  l(len([d for d i
+00017940: 6e20 6461 7461 2e73 706c 6974 6c69 6e65  n data.splitline
+00017950: 7328 2920 6966 2064 2e73 7472 6970 2829  s() if d.strip()
+00017960: 5d29 2c20 6c65 6e28 7474 2929 0a0a 2020  ]), len(tt))..  
+00017970: 2020 6465 6620 7465 7374 5f65 7863 656c    def test_excel
+00017980: 5f69 6d70 6f72 7428 7365 6c66 293a 0a20  _import(self):. 
+00017990: 2020 2020 2020 2066 696c 655f 6e61 6d65         file_name
+000179a0: 203d 2022 7465 7374 2f61 6263 2e78 6c73   = "test/abc.xls
+000179b0: 7822 0a20 2020 2020 2020 2065 7863 656c  x".        excel
+000179c0: 5f74 6162 6c65 203d 206c 742e 5461 626c  _table = lt.Tabl
+000179d0: 6528 292e 6578 6365 6c5f 696d 706f 7274  e().excel_import
+000179e0: 2866 696c 655f 6e61 6d65 2c20 7472 616e  (file_name, tran
+000179f0: 7366 6f72 6d73 3d7b 2761 273a 2069 6e74  sforms={'a': int
+00017a00: 2c20 2762 273a 2069 6e74 2c20 2763 273a  , 'b': int, 'c':
+00017a10: 2069 6e74 7d29 0a0a 2020 2020 2020 2020   int})..        
+00017a20: 7465 7374 5f73 697a 6520 3d20 330a 2020  test_size = 3.  
+00017a30: 2020 2020 2020 7431 203d 206d 616b 655f        t1 = make_
+00017a40: 7465 7374 5f74 6162 6c65 2873 656c 662e  test_table(self.
+00017a50: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
+00017a60: 2c20 7465 7374 5f73 697a 6529 0a0a 2020  , test_size)..  
+00017a70: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00017a80: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+00017a90: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00017aa0: 7274 5472 7565 2861 6c6c 286d 616b 655f  rtTrue(all(make_
+00017ab0: 6461 7461 6f62 6a65 6374 5f66 726f 6d5f  dataobject_from_
+00017ac0: 6f62 2872 6563 3129 203d 3d20 7265 6332  ob(rec1) == rec2
+00017ad0: 2066 6f72 2072 6563 312c 2072 6563 3220   for rec1, rec2 
+00017ae0: 696e 207a 6970 2874 312c 2065 7863 656c  in zip(t1, excel
+00017af0: 5f74 6162 6c65 2929 290a 2020 2020 2020  _table))).      
+00017b00: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00017b10: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00017b20: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00017b30: 7561 6c28 7375 6d28 3120 666f 7220 6c69  ual(sum(1 for li
+00017b40: 6e65 2069 6e20 6373 765f 6461 7461 2e73  ne in csv_data.s
+00017b50: 706c 6974 6c69 6e65 7328 2920 6966 206c  plitlines() if l
+00017b60: 696e 652e 7374 7269 7028 2929 2d31 2c20  ine.strip())-1, 
+00017b70: 6c65 6e28 6578 6365 6c5f 7461 626c 6529  len(excel_table)
+00017b80: 290a 0a20 2020 2020 2020 2072 6f77 5f70  )..        row_p
+00017b90: 726f 746f 7479 7065 203d 2073 656c 662e  rototype = self.
+00017ba0: 6d61 6b65 5f64 6174 615f 6f62 6a65 6374  make_data_object
+00017bb0: 2830 2c20 302c 2030 290a 2020 2020 2020  (0, 0, 0).      
+00017bc0: 2020 6373 7674 6162 6c65 3220 3d20 6c74    csvtable2 = lt
+00017bd0: 2e54 6162 6c65 2829 2e65 7863 656c 5f69  .Table().excel_i
+00017be0: 6d70 6f72 7428 0a20 2020 2020 2020 2020  mport(.         
+00017bf0: 2020 2066 696c 655f 6e61 6d65 2c20 7472     file_name, tr
+00017c00: 616e 7366 6f72 6d73 3d7b 2761 273a 2069  ansforms={'a': i
+00017c10: 6e74 2c20 2762 273a 2069 6e74 2c20 2763  nt, 'b': int, 'c
+00017c20: 273a 2069 6e74 7d2c 2072 6f77 5f63 6c61  ': int}, row_cla
+00017c30: 7373 3d74 7970 6528 726f 775f 7072 6f74  ss=type(row_prot
+00017c40: 6f74 7970 6529 0a20 2020 2020 2020 2029  otype).        )
+00017c50: 5b3a 335d 0a0a 2020 2020 2020 2020 7072  [:3]..        pr
+00017c60: 696e 7428 7479 7065 2874 315b 305d 292e  int(type(t1[0]).
+00017c70: 5f5f 6e61 6d65 5f5f 2c20 7431 5b30 5d29  __name__, t1[0])
+00017c80: 0a20 2020 2020 2020 2070 7269 6e74 2874  .        print(t
+00017c90: 7970 6528 6373 7674 6162 6c65 325b 305d  ype(csvtable2[0]
+00017ca0: 292e 5f5f 6e61 6d65 5f5f 2c20 6373 7674  ).__name__, csvt
+00017cb0: 6162 6c65 325b 305d 290a 2020 2020 2020  able2[0]).      
+00017cc0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00017cd0: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00017ce0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00017cf0: 7561 6c28 7479 7065 2874 315b 305d 292c  ual(type(t1[0]),
+00017d00: 2074 7970 6528 6373 7674 6162 6c65 325b   type(csvtable2[
+00017d10: 305d 2929 0a0a 2020 2020 6465 6620 7465  0]))..    def te
+00017d20: 7374 5f65 7863 656c 5f65 7870 6f72 7428  st_excel_export(
+00017d30: 7365 6c66 293a 0a20 2020 2020 2020 2066  self):.        f
+00017d40: 696c 655f 6e61 6d65 203d 2022 7465 7374  ile_name = "test
+00017d50: 2f61 6263 2e78 6c73 7822 0a20 2020 2020  /abc.xlsx".     
+00017d60: 2020 2065 7863 656c 5f74 6162 6c65 203d     excel_table =
+00017d70: 206c 742e 5461 626c 6528 292e 6578 6365   lt.Table().exce
+00017d80: 6c5f 696d 706f 7274 2866 696c 655f 6e61  l_import(file_na
+00017d90: 6d65 2c20 7472 616e 7366 6f72 6d73 3d7b  me, transforms={
+00017da0: 2761 273a 2069 6e74 2c20 2762 273a 2069  'a': int, 'b': i
+00017db0: 6e74 2c20 2763 273a 2069 6e74 7d2c 206c  nt, 'c': int}, l
+00017dc0: 696d 6974 3d31 290a 2020 2020 2020 2020  imit=1).        
+00017dd0: 6f75 7466 696c 6520 3d20 696f 2e42 7974  outfile = io.Byt
+00017de0: 6573 494f 2829 0a20 2020 2020 2020 2065  esIO().        e
+00017df0: 7863 656c 5f74 6162 6c65 2e65 7863 656c  xcel_table.excel
+00017e00: 5f65 7870 6f72 7428 6f75 7466 696c 6529  _export(outfile)
+00017e10: 0a20 2020 2020 2020 2065 7870 6f72 7465  .        exporte
+00017e20: 645f 7461 626c 6520 3d20 6c74 2e54 6162  d_table = lt.Tab
+00017e30: 6c65 2829 2e65 7863 656c 5f69 6d70 6f72  le().excel_impor
+00017e40: 7428 6f75 7466 696c 652c 2074 7261 6e73  t(outfile, trans
+00017e50: 666f 726d 733d 7b27 6127 3a20 696e 742c  forms={'a': int,
+00017e60: 2027 6227 3a20 696e 742c 2027 6327 3a20   'b': int, 'c': 
+00017e70: 696e 747d 290a 0a20 2020 2020 2020 2077  int})..        w
+00017e80: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+00017e90: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00017ea0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
+00017eb0: 616c 6c28 6d61 6b65 5f64 6174 616f 626a  all(make_dataobj
+00017ec0: 6563 745f 6672 6f6d 5f6f 6228 7265 6331  ect_from_ob(rec1
+00017ed0: 2920 3d3d 2072 6563 3220 666f 7220 7265  ) == rec2 for re
+00017ee0: 6331 2c20 7265 6332 2069 6e20 7a69 7028  c1, rec2 in zip(
+00017ef0: 6578 706f 7274 6564 5f74 6162 6c65 2c20  exported_table, 
+00017f00: 6578 6365 6c5f 7461 626c 6529 2929 0a0a  excel_table)))..
+00017f10: 2020 2020 6465 6620 7465 7374 5f6d 6f64      def test_mod
+00017f20: 756c 655f 6c65 7665 6c5f 6373 765f 696d  ule_level_csv_im
+00017f30: 706f 7274 6572 2873 656c 6629 3a0a 2020  porter(self):.  
+00017f40: 2020 2020 2020 6461 7461 203d 2063 7376        data = csv
+00017f50: 5f64 6174 610a 2020 2020 2020 2020 6373  _data.        cs
+00017f60: 7674 6162 6c65 203d 206c 742e 6373 765f  vtable = lt.csv_
+00017f70: 696d 706f 7274 2863 7376 5f73 6f75 7263  import(csv_sourc
+00017f80: 653d 6461 7461 2c20 7472 616e 7366 6f72  e=data, transfor
+00017f90: 6d73 3d7b 2761 273a 2069 6e74 2c20 2762  ms={'a': int, 'b
+00017fa0: 273a 2069 6e74 2c20 2763 273a 2069 6e74  ': int, 'c': int
+00017fb0: 7d29 0a0a 2020 2020 2020 2020 7465 7374  })..        test
+00017fc0: 5f73 697a 6520 3d20 330a 2020 2020 2020  _size = 3.      
+00017fd0: 2020 7431 203d 206d 616b 655f 7465 7374    t1 = make_test
+00017fe0: 5f74 6162 6c65 2873 656c 662e 6d61 6b65  _table(self.make
+00017ff0: 5f64 6174 615f 6f62 6a65 6374 2c20 7465  _data_object, te
+00018000: 7374 5f73 697a 6529 0a0a 2020 2020 2020  st_size)..      
+00018010: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+00018020: 6573 7428 293a 0a20 2020 2020 2020 2020  est():.         
+00018030: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+00018040: 7565 2861 6c6c 286d 616b 655f 6461 7461  ue(all(make_data
+00018050: 6f62 6a65 6374 5f66 726f 6d5f 6f62 2872  object_from_ob(r
+00018060: 6563 3129 203d 3d20 7265 6332 2066 6f72  ec1) == rec2 for
+00018070: 2072 6563 312c 2072 6563 3220 696e 207a   rec1, rec2 in z
+00018080: 6970 2874 312c 2063 7376 7461 626c 6529  ip(t1, csvtable)
+00018090: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
+000180a0: 7365 6c66 2e73 7562 5465 7374 2829 3a0a  self.subTest():.
+000180b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000180c0: 2e61 7373 6572 7445 7175 616c 2873 756d  .assertEqual(sum
+000180d0: 2831 2066 6f72 206c 696e 6520 696e 2064  (1 for line in d
+000180e0: 6174 612e 7370 6c69 746c 696e 6573 2829  ata.splitlines()
+000180f0: 2069 6620 6c69 6e65 2e73 7472 6970 2829   if line.strip()
+00018100: 292d 312c 206c 656e 2863 7376 7461 626c  )-1, len(csvtabl
+00018110: 6529 290a 0a20 2020 2064 6566 2074 6573  e))..    def tes
+00018120: 745f 6d6f 6475 6c65 5f6c 6576 656c 5f6a  t_module_level_j
+00018130: 736f 6e5f 696d 706f 7274 6572 2873 656c  son_importer(sel
+00018140: 6629 3a0a 2020 2020 2020 2020 6461 7461  f):.        data
+00018150: 203d 206a 736f 6e5f 6461 7461 0a20 2020   = json_data.   
+00018160: 2020 2020 206a 736f 6e74 6162 6c65 203d       jsontable =
+00018170: 206c 742e 6a73 6f6e 5f69 6d70 6f72 7428   lt.json_import(
+00018180: 6461 7461 2c20 7374 7265 616d 696e 673d  data, streaming=
+00018190: 5472 7565 2c20 7472 616e 7366 6f72 6d73  True, transforms
+000181a0: 3d7b 2761 273a 2069 6e74 2c20 2762 273a  ={'a': int, 'b':
+000181b0: 2069 6e74 2c20 2763 273a 2069 6e74 7d29   int, 'c': int})
+000181c0: 0a0a 2020 2020 2020 2020 7465 7374 5f73  ..        test_s
+000181d0: 697a 6520 3d20 330a 2020 2020 2020 2020  ize = 3.        
+000181e0: 7431 203d 206d 616b 655f 7465 7374 5f74  t1 = make_test_t
+000181f0: 6162 6c65 2873 656c 662e 6d61 6b65 5f64  able(self.make_d
+00018200: 6174 615f 6f62 6a65 6374 2c20 7465 7374  ata_object, test
+00018210: 5f73 697a 6529 0a0a 2020 2020 2020 2020  _size)..        
+00018220: 7769 7468 2073 656c 662e 7375 6254 6573  with self.subTes
+00018230: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
+00018240: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+00018250: 2861 6c6c 286d 616b 655f 6461 7461 6f62  (all(make_dataob
+00018260: 6a65 6374 5f66 726f 6d5f 6f62 2872 6563  ject_from_ob(rec
+00018270: 3129 203d 3d20 7265 6332 2066 6f72 2072  1) == rec2 for r
+00018280: 6563 312c 2072 6563 3220 696e 207a 6970  ec1, rec2 in zip
+00018290: 2874 312c 206a 736f 6e74 6162 6c65 2929  (t1, jsontable))
+000182a0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+000182b0: 656c 662e 7375 6254 6573 7428 293a 0a20  elf.subTest():. 
+000182c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000182d0: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
+000182e0: 5b64 2066 6f72 2064 2069 6e20 6461 7461  [d for d in data
+000182f0: 2e73 706c 6974 6c69 6e65 7328 2920 6966  .splitlines() if
+00018300: 2064 2e73 7472 6970 2829 5d29 2c20 6c65   d.strip()]), le
+00018310: 6e28 6a73 6f6e 7461 626c 6529 290a 0a20  n(jsontable)).. 
+00018320: 2020 2064 6566 2074 6573 745f 6d6f 6475     def test_modu
+00018330: 6c65 5f6c 6576 656c 5f65 7863 656c 5f69  le_level_excel_i
+00018340: 6d70 6f72 7428 7365 6c66 293a 0a20 2020  mport(self):.   
+00018350: 2020 2020 2066 696c 655f 6e61 6d65 203d       file_name =
+00018360: 2022 7465 7374 2f61 6263 2e78 6c73 7822   "test/abc.xlsx"
+00018370: 0a20 2020 2020 2020 2065 7863 656c 5f74  .        excel_t
+00018380: 6162 6c65 203d 206c 742e 6578 6365 6c5f  able = lt.excel_
+00018390: 696d 706f 7274 2866 696c 655f 6e61 6d65  import(file_name
+000183a0: 2c20 7472 616e 7366 6f72 6d73 3d7b 2761  , transforms={'a
+000183b0: 273a 2069 6e74 2c20 2762 273a 2069 6e74  ': int, 'b': int
+000183c0: 2c20 2763 273a 2069 6e74 7d29 0a0a 2020  , 'c': int})..  
+000183d0: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
+000183e0: 3d20 330a 2020 2020 2020 2020 7431 203d  = 3.        t1 =
+000183f0: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
+00018400: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
+00018410: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
+00018420: 6529 0a0a 2020 2020 2020 2020 7769 7468  e)..        with
+00018430: 2073 656c 662e 7375 6254 6573 7428 293a   self.subTest():
+00018440: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00018450: 662e 6173 7365 7274 5472 7565 2861 6c6c  f.assertTrue(all
+00018460: 286d 616b 655f 6461 7461 6f62 6a65 6374  (make_dataobject
+00018470: 5f66 726f 6d5f 6f62 2872 6563 3129 203d  _from_ob(rec1) =
+00018480: 3d20 7265 6332 2066 6f72 2072 6563 312c  = rec2 for rec1,
+00018490: 2072 6563 3220 696e 207a 6970 2874 312c   rec2 in zip(t1,
+000184a0: 2065 7863 656c 5f74 6162 6c65 2929 290a   excel_table))).
+000184b0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+000184c0: 662e 7375 6254 6573 7428 293a 0a20 2020  f.subTest():.   
+000184d0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+000184e0: 7365 7274 4571 7561 6c28 7375 6d28 3120  sertEqual(sum(1 
+000184f0: 666f 7220 6c69 6e65 2069 6e20 6373 765f  for line in csv_
+00018500: 6461 7461 2e73 706c 6974 6c69 6e65 7328  data.splitlines(
+00018510: 2920 6966 206c 696e 652e 7374 7269 7028  ) if line.strip(
+00018520: 2929 2d31 2c20 6c65 6e28 6578 6365 6c5f  ))-1, len(excel_
+00018530: 7461 626c 6529 290a 0a0a 406d 616b 655f  table))...@make_
+00018540: 7465 7374 5f63 6c61 7373 6573 0a63 6c61  test_classes.cla
+00018550: 7373 2054 6162 6c65 5069 766f 7454 6573  ss TablePivotTes
+00018560: 7473 3a0a 2020 2020 6465 6620 7465 7374  ts:.    def test
+00018570: 5f70 6976 6f74 2873 656c 6629 3a0a 2020  _pivot(self):.  
+00018580: 2020 2020 2020 7465 7374 5f73 697a 6520        test_size 
+00018590: 3d20 350a 2020 2020 2020 2020 7431 203d  = 5.        t1 =
+000185a0: 206d 616b 655f 7465 7374 5f74 6162 6c65   make_test_table
+000185b0: 2873 656c 662e 6d61 6b65 5f64 6174 615f  (self.make_data_
+000185c0: 6f62 6a65 6374 2c20 7465 7374 5f73 697a  object, test_siz
+000185d0: 6529 0a20 2020 2020 2020 2074 312e 6372  e).        t1.cr
+000185e0: 6561 7465 5f69 6e64 6578 2827 6127 290a  eate_index('a').
+000185f0: 2020 2020 2020 2020 7431 2e63 7265 6174          t1.creat
+00018600: 655f 696e 6465 7828 2762 2729 0a20 2020  e_index('b').   
+00018610: 2020 2020 2074 3170 6976 6f74 203d 2074       t1pivot = t
+00018620: 312e 7069 766f 7428 2761 2729 0a20 2020  1.pivot('a').   
+00018630: 2020 2020 2074 3170 6976 6f74 2e64 756d       t1pivot.dum
+00018640: 7028 290a 2020 2020 2020 2020 7431 7069  p().        t1pi
+00018650: 766f 742e 6475 6d70 5f63 6f75 6e74 7328  vot.dump_counts(
+00018660: 290a 2020 2020 2020 2020 7431 7069 766f  ).        t1pivo
+00018670: 742e 7375 6d6d 6172 795f 636f 756e 7473  t.summary_counts
+00018680: 2829 0a0a 2020 2020 2020 2020 7432 7069  ()..        t2pi
+00018690: 766f 7420 3d20 7431 2e70 6976 6f74 2827  vot = t1.pivot('
+000186a0: 6120 6227 290a 2020 2020 2020 2020 7432  a b').        t2
+000186b0: 7069 766f 742e 6475 6d70 2829 0a20 2020  pivot.dump().   
+000186c0: 2020 2020 2074 3270 6976 6f74 2e64 756d       t2pivot.dum
+000186d0: 705f 636f 756e 7473 2829 0a20 2020 2020  p_counts().     
+000186e0: 2020 2074 3270 6976 6f74 2e73 756d 6d61     t2pivot.summa
+000186f0: 7279 5f63 6f75 6e74 7328 290a 0a20 2020  ry_counts()..   
+00018700: 2020 2020 2023 2054 4f44 4f20 2d20 6164       # TODO - ad
+00018710: 6420 6173 7365 7274 730a 0a0a 636c 6173  d asserts...clas
+00018720: 7320 5461 626c 6553 6561 7263 6854 6573  s TableSearchTes
+00018730: 7473 2875 6e69 7474 6573 742e 5465 7374  ts(unittest.Test
+00018740: 4361 7365 293a 0a20 2020 2072 6563 6970  Case):.    recip
+00018750: 655f 6461 7461 203d 2074 6578 7477 7261  e_data = textwra
+00018760: 702e 6465 6465 6e74 2822 2222 5c0a 2020  p.dedent("""\.  
+00018770: 2020 2020 2020 6964 2c74 6974 6c65 2c69        id,title,i
+00018780: 6e67 7265 6469 656e 7473 0a20 2020 2020  ngredients.     
+00018790: 2020 2031 2c54 756e 6120 6361 7373 6572     1,Tuna casser
+000187a0: 6f6c 652c 2274 756e 612c 206e 6f6f 646c  ole,"tuna, noodl
+000187b0: 6573 2c20 4372 6561 6d20 6f66 204d 7573  es, Cream of Mus
+000187c0: 6872 6f6f 6d20 536f 7570 220a 2020 2020  hroom Soup".    
+000187d0: 2020 2020 322c 4861 7761 6969 616e 2070      2,Hawaiian p
+000187e0: 697a 7a61 2c70 697a 7a61 2064 6f75 6768  izza,pizza dough
+000187f0: 2070 696e 6561 7070 6c65 2068 616d 2074   pineapple ham t
+00018800: 6f6d 6174 6f20 7361 7563 650a 2020 2020  omato sauce.    
+00018810: 2020 2020 332c 4d61 7267 6865 7269 7461      3,Margherita
+00018820: 2070 697a 7a61 2c70 697a 7a61 2064 6f75   pizza,pizza dou
+00018830: 6768 2063 6865 6573 6520 7065 7374 6f20  gh cheese pesto 
+00018840: 6172 7469 6368 6f6b 6520 6865 6172 7473  artichoke hearts
+00018850: 0a20 2020 2020 2020 2034 2c50 6570 7065  .        4,Peppe
+00018860: 726f 6e69 2070 697a 7a61 2c70 697a 7a61  roni pizza,pizza
+00018870: 2064 6f75 6768 2063 6865 6573 6520 746f   dough cheese to
+00018880: 6d61 746f 2073 6175 6365 2070 6570 7065  mato sauce peppe
+00018890: 726f 6e69 0a20 2020 2020 2020 2035 2c47  roni.        5,G
+000188a0: 7269 6c6c 6564 2063 6865 6573 6520 7361  rilled cheese sa
+000188b0: 6e64 7769 6368 2c62 7265 6164 2063 6865  ndwich,bread che
+000188c0: 6573 6520 6275 7474 6572 0a20 2020 2020  ese butter.     
+000188d0: 2020 2036 2c54 756e 6120 6d65 6c74 2c74     6,Tuna melt,t
+000188e0: 756e 6120 6d61 796f 6e6e 6169 7365 2074  una mayonnaise t
+000188f0: 6f6d 6174 6f20 6272 6561 6420 6368 6565  omato bread chee
+00018900: 7365 0a20 2020 2020 2020 2037 2c43 6869  se.        7,Chi
+00018910: 6c69 2064 6f67 2c68 6f74 2064 6f67 2063  li dog,hot dog c
+00018920: 6869 6c69 206f 6e69 6f6e 2062 756e 0a20  hili onion bun. 
+00018930: 2020 2020 2020 2038 2c46 7265 6e63 6820         8,French 
+00018940: 746f 6173 742c 6567 6720 6d69 6c6b 2076  toast,egg milk v
+00018950: 616e 696c 6c61 2062 7265 6164 206d 6170  anilla bread map
+00018960: 6c65 2073 7972 7570 0a20 2020 2020 2020  le syrup.       
+00018970: 2039 2c42 4c54 2c62 7265 6164 2062 6163   9,BLT,bread bac
+00018980: 6f6e 206c 6574 7475 6365 2074 6f6d 6174  on lettuce tomat
+00018990: 6f20 6d61 796f 6e6e 6169 7365 0a20 2020  o mayonnaise.   
+000189a0: 2020 2020 2031 302c 5265 7562 656e 2073       10,Reuben s
+000189b0: 616e 6477 6963 682c 7279 6520 6272 6561  andwich,rye brea
+000189c0: 6420 7361 7565 726b 7261 7574 2063 6f72  d sauerkraut cor
+000189d0: 6e65 6420 6265 6566 2073 7769 7373 2063  ned beef swiss c
+000189e0: 6865 6573 6520 7275 7373 6961 6e20 6472  heese russian dr
+000189f0: 6573 7369 6e67 2074 686f 7573 616e 6420  essing thousand 
+00018a00: 6973 6c61 6e64 0a20 2020 2020 2020 2031  island.        1
+00018a10: 312c 4861 6d62 7572 6765 722c 6772 6f75  1,Hamburger,grou
+00018a20: 6e64 2062 6565 6620 6275 6e20 6c65 7474  nd beef bun lett
+00018a30: 7563 6520 6b65 7463 6875 7020 6d75 7374  uce ketchup must
+00018a40: 6172 6420 7069 636b 6c65 0a20 2020 2020  ard pickle.     
+00018a50: 2020 2031 322c 4368 6565 7365 6275 7267     12,Cheeseburg
+00018a60: 6572 2c67 726f 756e 6420 6265 6566 2062  er,ground beef b
+00018a70: 756e 206c 6574 7475 6365 206b 6574 6368  un lettuce ketch
+00018a80: 7570 206d 7573 7461 7264 2070 6963 6b6c  up mustard pickl
+00018a90: 6520 6368 6565 7365 0a20 2020 2020 2020  e cheese.       
+00018aa0: 2031 332c 4261 636f 6e20 6368 6565 7365   13,Bacon cheese
+00018ab0: 6275 7267 6572 2c67 726f 756e 6420 6265  burger,ground be
+00018ac0: 6566 2062 756e 206c 6574 7475 6365 206b  ef bun lettuce k
+00018ad0: 6574 6368 7570 206d 7573 7461 7264 2070  etchup mustard p
+00018ae0: 6963 6b6c 6520 6368 6565 7365 2062 6163  ickle cheese bac
+00018af0: 6f6e 0a20 2020 2020 2020 2022 2222 290a  on.        """).
+00018b00: 0a20 2020 2064 6566 2073 6574 5570 2873  .    def setUp(s
+00018b10: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+00018b20: 6c66 2e72 6563 6970 6573 203d 206c 742e  lf.recipes = lt.
+00018b30: 5461 626c 6528 292e 6373 765f 696d 706f  Table().csv_impo
+00018b40: 7274 2873 656c 662e 7265 6369 7065 5f64  rt(self.recipe_d
+00018b50: 6174 612c 2074 7261 6e73 666f 726d 733d  ata, transforms=
+00018b60: 6469 6374 2869 643d 696e 7429 290a 2020  dict(id=int)).  
+00018b70: 2020 2020 2020 7365 6c66 2e72 6563 6970        self.recip
+00018b80: 6573 2e63 7265 6174 655f 696e 6465 7828  es.create_index(
+00018b90: 2269 6422 2c20 756e 6971 7565 3d54 7275  "id", unique=Tru
+00018ba0: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+00018bb0: 7265 6369 7065 732e 6372 6561 7465 5f73  recipes.create_s
+00018bc0: 6561 7263 685f 696e 6465 7828 2269 6e67  earch_index("ing
+00018bd0: 7265 6469 656e 7473 2229 0a0a 2020 2020  redients")..    
+00018be0: 4061 6e6e 6f75 6e63 655f 7465 7374 0a20  @announce_test. 
+00018bf0: 2020 2064 6566 2074 6573 745f 6163 6365     def test_acce
+00018c00: 7373 5f6e 6f6e 5f65 7869 7374 656e 745f  ss_non_existent_
+00018c10: 7365 6172 6368 5f61 7474 7269 6275 7465  search_attribute
+00018c20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00018c30: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
+00018c40: 5261 6973 6573 2856 616c 7565 4572 726f  Raises(ValueErro
+00018c50: 722c 206d 7367 3d22 6661 696c 6564 2074  r, msg="failed t
+00018c60: 6f20 7261 6973 6520 5661 6c75 6545 7272  o raise ValueErr
+00018c70: 6f72 2077 6865 6e20 6163 6365 7373 696e  or when accessin
+00018c80: 6720 6e6f 6e2d 6578 6973 7465 6e74 2073  g non-existent s
+00018c90: 6561 7263 6820 696e 6465 7822 293a 0a20  earch index"):. 
+00018ca0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018cb0: 7265 6369 7065 732e 7365 6172 6368 2e74  recipes.search.t
+00018cc0: 6974 6c65 2822 7879 7a22 290a 0a20 2020  itle("xyz")..   
+00018cd0: 2040 616e 6e6f 756e 6365 5f74 6573 740a   @announce_test.
+00018ce0: 2020 2020 6465 6620 7465 7374 5f73 6561      def test_sea
+00018cf0: 7263 685f 6469 7228 7365 6c66 293a 0a20  rch_dir(self):. 
+00018d00: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00018d10: 7274 4571 7561 6c28 5b27 696e 6772 6564  rtEqual(['ingred
+00018d20: 6965 6e74 7327 5d2c 2064 6972 2873 656c  ients'], dir(sel
+00018d30: 662e 7265 6369 7065 732e 7365 6172 6368  f.recipes.search
+00018d40: 292c 2022 6661 696c 6564 2074 6f20 6765  ), "failed to ge
+00018d50: 6e65 7261 7465 2063 6f72 7265 6374 2064  nerate correct d
+00018d60: 6972 2829 2072 6573 706f 6e73 6522 290a  ir() response").
+00018d70: 0a20 2020 2040 616e 6e6f 756e 6365 5f74  .    @announce_t
+00018d80: 6573 740a 2020 2020 6465 6620 7465 7374  est.    def test
+00018d90: 5f74 6578 745f 7365 6172 6368 2873 656c  _text_search(sel
+00018da0: 6629 3a0a 2020 2020 2020 2020 666f 7220  f):.        for 
+00018db0: 7175 6572 792c 2065 7870 6563 7465 6420  query, expected 
+00018dc0: 696e 205b 0a20 2020 2020 2020 2020 2020  in [.           
+00018dd0: 2028 2222 2c20 5b5d 292c 0a20 2020 2020   ("", []),.     
+00018de0: 2020 2020 2020 2028 2274 756e 6122 2c20         ("tuna", 
+00018df0: 5b31 2c20 365d 292c 0a20 2020 2020 2020  [1, 6]),.       
+00018e00: 2020 2020 2028 2274 756e 6120 2b63 6865       ("tuna +che
+00018e10: 6573 6522 2c20 5b36 2c20 332c 2034 2c20  ese", [6, 3, 4, 
+00018e20: 352c 2031 302c 2031 322c 2031 332c 2031  5, 10, 12, 13, 1
+00018e30: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+00018e40: 2822 7069 6e65 6170 706c 6520 2b62 6163  ("pineapple +bac
+00018e50: 6f6e 206c 6574 7475 6365 2062 6565 6620  on lettuce beef 
+00018e60: 2d73 6175 6572 6b72 6175 7420 746f 6d61  -sauerkraut toma
+00018e70: 746f 222c 205b 392c 2031 332c 2032 2c20  to", [9, 13, 2, 
+00018e80: 3131 2c20 3132 2c20 342c 2036 2c20 3130  11, 12, 4, 6, 10
+00018e90: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+00018ea0: 2822 7069 7a7a 6120 646f 7567 6820 2d70  ("pizza dough -p
+00018eb0: 696e 6561 7070 6c65 222c 205b 332c 2034  ineapple", [3, 4
+00018ec0: 2c20 325d 292c 0a20 2020 2020 2020 2020  , 2]),.         
+00018ed0: 2020 2028 2270 697a 7a61 2064 6f75 6768     ("pizza dough
+00018ee0: 202d 2d70 696e 6561 7070 6c65 222c 205b   --pineapple", [
+00018ef0: 332c 2034 5d29 2c0a 2020 2020 2020 2020  3, 4]),.        
+00018f00: 2020 2020 2822 6272 6561 6420 6261 636f      ("bread baco
+00018f10: 6e22 2c20 5b39 2c20 352c 2036 2c20 382c  n", [9, 5, 6, 8,
+00018f20: 2031 302c 2031 335d 292c 0a20 2020 2020   10, 13]),.     
+00018f30: 2020 2020 2020 2028 2262 7265 6164 202b         ("bread +
+00018f40: 2b62 6163 6f6e 222c 205b 392c 2031 335d  +bacon", [9, 13]
+00018f50: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+00018f60: 2262 7265 6164 202b 2b61 6e63 686f 7669  "bread ++anchovi
+00018f70: 6573 222c 205b 5d29 2c0a 2020 2020 2020  es", []),.      
+00018f80: 2020 2020 2020 2822 6272 6561 6420 2b2b        ("bread ++
+00018f90: 6261 636f 6e20 2b2b 616e 6368 6f76 6965  bacon ++anchovie
+00018fa0: 7322 2c20 5b5d 292c 0a20 2020 2020 2020  s", []),.       
+00018fb0: 2020 2020 2028 2262 7265 6164 2062 6163       ("bread bac
+00018fc0: 6f6e 202d 2d61 6e63 686f 7669 6573 222c  on --anchovies",
+00018fd0: 205b 392c 2035 2c20 362c 2038 2c20 3130   [9, 5, 6, 8, 10
+00018fe0: 2c20 3133 5d29 2c0a 2020 2020 2020 2020  , 13]),.        
+00018ff0: 5d3a 0a20 2020 2020 2020 2020 2020 206d  ]:.            m
+00019000: 6174 6368 6573 203d 2073 656c 662e 7265  atches = self.re
+00019010: 6369 7065 732e 7365 6172 6368 2e69 6e67  cipes.search.ing
+00019020: 7265 6469 656e 7473 2871 7565 7279 2c20  redients(query, 
+00019030: 6173 5f74 6162 6c65 3d46 616c 7365 2c20  as_table=False, 
+00019040: 6d69 6e5f 7363 6f72 653d 2d31 3030 3030  min_score=-10000
+00019050: 290a 2020 2020 2020 2020 2020 2020 6d61  ).            ma
+00019060: 7463 685f 6964 7320 3d20 5b72 6563 6970  tch_ids = [recip
+00019070: 652e 6964 2066 6f72 2072 6563 6970 652c  e.id for recipe,
+00019080: 205f 2069 6e20 6d61 7463 6865 735d 0a20   _ in matches]. 
+00019090: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000190a0: 2872 6570 7228 7175 6572 7929 2c20 272d  (repr(query), '-
+000190b0: 3e27 2c20 5b28 7265 6369 7065 2e69 642c  >', [(recipe.id,
+000190c0: 2073 636f 7265 2920 666f 7220 7265 6369   score) for reci
+000190d0: 7065 2c20 7363 6f72 6520 696e 206d 6174  pe, score in mat
+000190e0: 6368 6573 5d29 0a20 2020 2020 2020 2020  ches]).         
+000190f0: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+00019100: 5465 7374 2871 7565 7279 3d71 7565 7279  Test(query=query
+00019110: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00019120: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00019130: 7561 6c28 6578 7065 6374 6564 2c20 6d61  ual(expected, ma
+00019140: 7463 685f 6964 732c 0a20 2020 2020 2020  tch_ids,.       
+00019150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019160: 2020 2020 2020 2020 2020 6622 696e 7661            f"inva
+00019170: 6c69 6420 7265 7375 6c74 7320 666f 7220  lid results for 
+00019180: 7175 6572 7920 7b71 7565 7279 2172 7d2c  query {query!r},
+00019190: 2065 7870 6563 7465 6420 7b65 7870 6563   expected {expec
+000191a0: 7465 647d 2c20 676f 7420 7b6d 6174 6368  ted}, got {match
+000191b0: 5f69 6473 7d22 290a 0a20 2020 2040 616e  _ids}")..    @an
+000191c0: 6e6f 756e 6365 5f74 6573 740a 2020 2020  nounce_test.    
+000191d0: 6465 6620 7465 7374 5f69 6e76 616c 6964  def test_invalid
+000191e0: 6174 655f 696e 6465 7828 7365 6c66 293a  ate_index(self):
+000191f0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00019200: 6369 7065 732e 706f 7028 3029 0a20 2020  cipes.pop(0).   
+00019210: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
+00019220: 7373 6572 7452 6169 7365 7328 6c74 2e53  ssertRaises(lt.S
+00019230: 6561 7263 6849 6e64 6578 496e 636f 6e73  earchIndexIncons
+00019240: 6973 7465 6e74 4572 726f 722c 0a20 2020  istentError,.   
+00019250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019260: 2020 2020 2020 2020 2020 2020 6d73 673d              msg=
+00019270: 2266 6169 6c65 6420 746f 2072 6169 7365  "failed to raise
+00019280: 2065 7863 6570 7469 6f6e 2077 6865 6e20   exception when 
+00019290: 7365 6172 6368 696e 6720 6d6f 6469 6669  searching modifi
+000192a0: 6564 2074 6162 6c65 2229 3a0a 2020 2020  ed table"):.    
+000192b0: 2020 2020 2020 2020 7365 6c66 2e72 6563          self.rec
+000192c0: 6970 6573 2e73 6561 7263 682e 696e 6772  ipes.search.ingr
+000192d0: 6564 6965 6e74 7328 2262 6163 6f6e 2229  edients("bacon")
+000192e0: 0a0a 2020 2020 4061 6e6e 6f75 6e63 655f  ..    @announce_
+000192f0: 7465 7374 0a20 2020 2064 6566 2074 6573  test.    def tes
+00019300: 745f 7365 6172 6368 5f77 6974 685f 6b65  t_search_with_ke
+00019310: 7977 6f72 6473 2873 656c 6629 3a0a 2020  ywords(self):.  
+00019320: 2020 2020 2020 666f 7220 7175 6572 792c        for query,
+00019330: 2065 7870 6563 7465 642c 2065 7870 6563   expected, expec
+00019340: 7465 645f 776f 7264 7320 696e 205b 0a20  ted_words in [. 
+00019350: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00019360: 2274 756e 6122 2c20 5b31 2c20 365d 2c20  "tuna", [1, 6], 
+00019370: 5b7b 276e 6f6f 646c 6573 272c 2027 6e6f  [{'noodles', 'no
+00019380: 6f64 6c65 272c 2027 7475 6e61 272c 2027  odle', 'tuna', '
+00019390: 736f 7570 272c 2027 6372 6561 6d27 2c20  soup', 'cream', 
+000193a0: 276d 7573 6872 6f6f 6d27 7d2c 0a20 2020  'mushroom'},.   
+000193b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193c0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+000193d0: 2774 6f6d 6174 6f27 2c20 2774 756e 6127  'tomato', 'tuna'
+000193e0: 2c20 276d 6179 6f6e 6e61 6973 6527 2c20  , 'mayonnaise', 
+000193f0: 2762 7265 6164 272c 2027 6368 6565 7365  'bread', 'cheese
+00019400: 277d 5d29 2c0a 2020 2020 2020 2020 2020  '}]),.          
+00019410: 2020 2020 2020 5d3a 0a20 2020 2020 2020        ]:.       
+00019420: 2020 2020 206d 6174 6368 6573 203d 2073       matches = s
+00019430: 656c 662e 7265 6369 7065 732e 7365 6172  elf.recipes.sear
+00019440: 6368 2e69 6e67 7265 6469 656e 7473 2871  ch.ingredients(q
+00019450: 7565 7279 2c20 6d69 6e5f 7363 6f72 653d  uery, min_score=
+00019460: 2d31 3030 3030 2c20 6173 5f74 6162 6c65  -10000, as_table
+00019470: 3d46 616c 7365 2c20 696e 636c 7564 655f  =False, include_
+00019480: 776f 7264 733d 5472 7565 290a 2020 2020  words=True).    
+00019490: 2020 2020 2020 2020 6d61 7463 685f 6964          match_id
+000194a0: 7320 3d20 5b72 6563 6970 652e 6964 2066  s = [recipe.id f
+000194b0: 6f72 2072 6563 6970 652c 2073 636f 7265  or recipe, score
+000194c0: 2c20 776f 7264 7320 696e 206d 6174 6368  , words in match
+000194d0: 6573 5d0a 2020 2020 2020 2020 2020 2020  es].            
+000194e0: 7072 696e 7428 7265 7072 2871 7565 7279  print(repr(query
+000194f0: 292c 2027 2d3e 272c 205b 2872 6563 6970  ), '->', [(recip
+00019500: 652e 6964 2c20 7363 6f72 652c 2077 6f72  e.id, score, wor
+00019510: 6473 2920 666f 7220 7265 6369 7065 2c20  ds) for recipe, 
+00019520: 7363 6f72 652c 2077 6f72 6473 2069 6e20  score, words in 
+00019530: 6d61 7463 6865 735d 290a 2020 2020 2020  matches]).      
+00019540: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00019550: 7375 6254 6573 7428 293a 0a20 2020 2020  subTest():.     
+00019560: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019570: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
+00019580: 6374 6564 2c20 6d61 7463 685f 6964 732c  cted, match_ids,
+00019590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000195a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195b0: 2020 6622 696e 7661 6c69 6420 7265 7375    f"invalid resu
+000195c0: 6c74 7320 666f 7220 7175 6572 7920 7b71  lts for query {q
+000195d0: 7565 7279 2172 7d2c 2065 7870 6563 7465  uery!r}, expecte
+000195e0: 6420 7b65 7870 6563 7465 647d 2c20 676f  d {expected}, go
+000195f0: 7420 7b6d 6174 6368 5f69 6473 7d22 290a  t {match_ids}").
+00019600: 2020 2020 2020 2020 2020 2020 6d61 7463              matc
+00019610: 685f 776f 7264 7320 3d20 5b73 6574 2877  h_words = [set(w
+00019620: 6f72 6473 2920 666f 7220 7265 6369 7065  ords) for recipe
+00019630: 2c20 7363 6f72 652c 2077 6f72 6473 2069  , score, words i
+00019640: 6e20 6d61 7463 6865 735d 0a20 2020 2020  n matches].     
+00019650: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00019660: 2e73 7562 5465 7374 2829 3a0a 2020 2020  .subTest():.    
+00019670: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019680: 2e61 7373 6572 7445 7175 616c 2865 7870  .assertEqual(exp
+00019690: 6563 7465 645f 776f 7264 732c 206d 6174  ected_words, mat
+000196a0: 6368 5f77 6f72 6473 2c0a 2020 2020 2020  ch_words,.      
+000196b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196c0: 2020 2020 2020 2020 2020 2022 696e 7661             "inva
+000196d0: 6c69 6420 6d61 7463 6820 776f 7264 7320  lid match words 
+000196e0: 666f 7220 7175 6572 7920 7b21 727d 2c20  for query {!r}, 
+000196f0: 6578 7065 6374 6564 207b 7d2c 2067 6f74  expected {}, got
+00019700: 207b 7d22 2e66 6f72 6d61 7428 7175 6572   {}".format(quer
+00019710: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
+00019720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019770: 2020 2020 2065 7870 6563 7465 645f 776f       expected_wo
+00019780: 7264 732c 0a20 2020 2020 2020 2020 2020  rds,.           
+00019790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197e0: 2020 2020 2020 206d 6174 6368 5f77 6f72         match_wor
+000197f0: 6473 2929 0a0a 2020 2020 4061 6e6e 6f75  ds))..    @annou
+00019800: 6e63 655f 7465 7374 0a20 2020 2064 6566  nce_test.    def
+00019810: 2074 6573 745f 7365 6172 6368 5f77 6974   test_search_wit
+00019820: 685f 6c69 6d69 7428 7365 6c66 293a 0a20  h_limit(self):. 
+00019830: 2020 2020 2020 2066 6f72 2071 7565 7279         for query
+00019840: 2c20 6578 7065 6374 6564 2069 6e20 5b0a  , expected in [.
+00019850: 2020 2020 2020 2020 2020 2020 2822 222c              ("",
+00019860: 205b 5d29 2c0a 2020 2020 2020 2020 2020   []),.          
+00019870: 2020 2822 7475 6e61 222c 205b 312c 2036    ("tuna", [1, 6
+00019880: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+00019890: 2822 7475 6e61 202b 6368 6565 7365 222c  ("tuna +cheese",
+000198a0: 205b 362c 2033 2c20 345d 292c 0a20 2020   [6, 3, 4]),.   
+000198b0: 2020 2020 2020 2020 2028 2270 696e 6561           ("pinea
+000198c0: 7070 6c65 202b 6261 636f 6e20 6c65 7474  pple +bacon lett
+000198d0: 7563 6520 6265 6566 202d 7361 7565 726b  uce beef -sauerk
+000198e0: 7261 7574 2074 6f6d 6174 6f22 2c20 5b39  raut tomato", [9
+000198f0: 2c20 3133 2c20 325d 292c 0a20 2020 2020  , 13, 2]),.     
+00019900: 2020 2020 2020 2028 2270 697a 7a61 2064         ("pizza d
+00019910: 6f75 6768 202d 7069 6e65 6170 706c 6522  ough -pineapple"
+00019920: 2c20 5b33 2c20 342c 2032 5d29 2c0a 2020  , [3, 4, 2]),.  
+00019930: 2020 2020 2020 2020 2020 2822 7069 7a7a            ("pizz
+00019940: 6120 646f 7567 6820 2d2d 7069 6e65 6170  a dough --pineap
+00019950: 706c 6522 2c20 5b33 2c20 345d 292c 0a20  ple", [3, 4]),. 
+00019960: 2020 2020 2020 2020 2020 2028 2262 7265             ("bre
+00019970: 6164 2062 6163 6f6e 222c 205b 392c 2035  ad bacon", [9, 5
+00019980: 2c20 365d 292c 0a20 2020 2020 2020 2020  , 6]),.         
+00019990: 2020 2028 2262 7265 6164 202b 2b62 6163     ("bread ++bac
+000199a0: 6f6e 222c 205b 392c 2031 335d 292c 0a20  on", [9, 13]),. 
+000199b0: 2020 2020 2020 2020 2020 2028 2262 7265             ("bre
+000199c0: 6164 202b 2b61 6e63 686f 7669 6573 222c  ad ++anchovies",
+000199d0: 205b 5d29 2c0a 2020 2020 2020 2020 2020   []),.          
+000199e0: 2020 2822 6272 6561 6420 2b2b 6261 636f    ("bread ++baco
+000199f0: 6e20 2b2b 616e 6368 6f76 6965 7322 2c20  n ++anchovies", 
+00019a00: 5b5d 292c 0a20 2020 2020 2020 2020 2020  []),.           
+00019a10: 2028 2262 7265 6164 2062 6163 6f6e 202d   ("bread bacon -
+00019a20: 2d61 6e63 686f 7669 6573 222c 205b 392c  -anchovies", [9,
+00019a30: 2035 2c20 365d 292c 0a20 2020 2020 2020   5, 6]),.       
+00019a40: 205d 3a0a 2020 2020 2020 2020 2020 2020   ]:.            
+00019a50: 6d61 7463 6865 7320 3d20 7365 6c66 2e72  matches = self.r
+00019a60: 6563 6970 6573 2e73 6561 7263 682e 696e  ecipes.search.in
+00019a70: 6772 6564 6965 6e74 7328 7175 6572 792c  gredients(query,
+00019a80: 2061 735f 7461 626c 653d 4661 6c73 652c   as_table=False,
+00019a90: 206d 696e 5f73 636f 7265 3d2d 3130 3030   min_score=-1000
+00019aa0: 302c 206c 696d 6974 3d33 290a 2020 2020  0, limit=3).    
+00019ab0: 2020 2020 2020 2020 6d61 7463 685f 6964          match_id
+00019ac0: 7320 3d20 5b72 6563 6970 652e 6964 2066  s = [recipe.id f
+00019ad0: 6f72 2072 6563 6970 652c 205f 2069 6e20  or recipe, _ in 
+00019ae0: 6d61 7463 6865 735d 0a20 2020 2020 2020  matches].       
+00019af0: 2020 2020 2070 7269 6e74 2872 6570 7228       print(repr(
+00019b00: 7175 6572 7929 2c20 272d 3e27 2c20 5b28  query), '->', [(
+00019b10: 7265 6369 7065 2e69 642c 2073 636f 7265  recipe.id, score
+00019b20: 2920 666f 7220 7265 6369 7065 2c20 7363  ) for recipe, sc
+00019b30: 6f72 6520 696e 206d 6174 6368 6573 5d29  ore in matches])
+00019b40: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00019b50: 6820 7365 6c66 2e73 7562 5465 7374 2871  h self.subTest(q
+00019b60: 7565 7279 3d71 7565 7279 293a 0a20 2020  uery=query):.   
+00019b70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019b80: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
+00019b90: 7065 6374 6564 2c20 6d61 7463 685f 6964  pected, match_id
+00019ba0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00019bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019bc0: 2020 2020 6622 696e 7661 6c69 6420 7265      f"invalid re
+00019bd0: 7375 6c74 7320 666f 7220 7175 6572 7920  sults for query 
+00019be0: 7b71 7565 7279 2172 7d2c 2065 7870 6563  {query!r}, expec
+00019bf0: 7465 6420 7b65 7870 6563 7465 647d 2c20  ted {expected}, 
+00019c00: 676f 7420 7b6d 6174 6368 5f69 6473 7d22  got {match_ids}"
+00019c10: 290a 0a20 2020 2040 616e 6e6f 756e 6365  )..    @announce
+00019c20: 5f74 6573 740a 2020 2020 6465 6620 7465  _test.    def te
+00019c30: 7374 5f73 6561 7263 685f 7769 7468 5f6d  st_search_with_m
+00019c40: 696e 5f73 636f 7265 2873 656c 6629 3a0a  in_score(self):.
+00019c50: 2020 2020 2020 2020 666f 7220 7175 6572          for quer
+00019c60: 792c 2065 7870 6563 7465 6420 696e 205b  y, expected in [
+00019c70: 0a20 2020 2020 2020 2020 2020 2028 2222  .            (""
+00019c80: 2c20 5b5d 292c 0a20 2020 2020 2020 2020  , []),.         
+00019c90: 2020 2028 2274 756e 6122 2c20 5b5d 292c     ("tuna", []),
+00019ca0: 0a20 2020 2020 2020 2020 2020 2028 2274  .            ("t
+00019cb0: 756e 6120 2b63 6865 6573 6522 2c20 5b36  una +cheese", [6
+00019cc0: 2c5d 292c 0a20 2020 2020 2020 2020 2020  ,]),.           
+00019cd0: 2028 2270 696e 6561 7070 6c65 202b 6261   ("pineapple +ba
+00019ce0: 636f 6e20 6c65 7474 7563 6520 6265 6566  con lettuce beef
+00019cf0: 202d 7361 7565 726b 7261 7574 2074 6f6d   -sauerkraut tom
+00019d00: 6174 6f22 2c20 5b39 2c20 3133 5d29 2c0a  ato", [9, 13]),.
+00019d10: 2020 2020 2020 2020 2020 2020 2822 7069              ("pi
+00019d20: 7a7a 6120 646f 7567 6820 2d70 696e 6561  zza dough -pinea
+00019d30: 7070 6c65 222c 205b 5d29 2c0a 2020 2020  pple", []),.    
+00019d40: 2020 2020 2020 2020 2822 7069 7a7a 6120          ("pizza 
+00019d50: 646f 7567 6820 2d2d 7069 6e65 6170 706c  dough --pineappl
+00019d60: 6522 2c20 5b5d 292c 0a20 2020 2020 2020  e", []),.       
+00019d70: 2020 2020 2028 2262 7265 6164 2062 6163       ("bread bac
+00019d80: 6f6e 222c 205b 5d29 2c0a 2020 2020 2020  on", []),.      
+00019d90: 2020 2020 2020 2822 6272 6561 6420 2b2b        ("bread ++
+00019da0: 6261 636f 6e22 2c20 5b39 2c5d 292c 0a20  bacon", [9,]),. 
+00019db0: 2020 2020 2020 2020 2020 2028 2262 7265             ("bre
+00019dc0: 6164 202b 2b61 6e63 686f 7669 6573 222c  ad ++anchovies",
+00019dd0: 205b 5d29 2c0a 2020 2020 2020 2020 2020   []),.          
+00019de0: 2020 2822 6272 6561 6420 2b2b 6261 636f    ("bread ++baco
+00019df0: 6e20 2b2b 616e 6368 6f76 6965 7322 2c20  n ++anchovies", 
+00019e00: 5b5d 292c 0a20 2020 2020 2020 2020 2020  []),.           
+00019e10: 2028 2262 7265 6164 2062 6163 6f6e 202d   ("bread bacon -
+00019e20: 2d61 6e63 686f 7669 6573 222c 205b 5d29  -anchovies", [])
+00019e30: 2c0a 2020 2020 2020 2020 5d3a 0a20 2020  ,.        ]:.   
+00019e40: 2020 2020 2020 2020 206d 6174 6368 6573           matches
+00019e50: 203d 2073 656c 662e 7265 6369 7065 732e   = self.recipes.
+00019e60: 7365 6172 6368 2e69 6e67 7265 6469 656e  search.ingredien
+00019e70: 7473 2871 7565 7279 2c20 6173 5f74 6162  ts(query, as_tab
+00019e80: 6c65 3d46 616c 7365 2c20 6d69 6e5f 7363  le=False, min_sc
+00019e90: 6f72 653d 3130 3030 290a 2020 2020 2020  ore=1000).      
+00019ea0: 2020 2020 2020 6d61 7463 685f 6964 7320        match_ids 
+00019eb0: 3d20 5b72 6563 6970 652e 6964 2066 6f72  = [recipe.id for
+00019ec0: 2072 6563 6970 652c 205f 2069 6e20 6d61   recipe, _ in ma
+00019ed0: 7463 6865 735d 0a20 2020 2020 2020 2020  tches].         
+00019ee0: 2020 2070 7269 6e74 2872 6570 7228 7175     print(repr(qu
+00019ef0: 6572 7929 2c20 272d 3e27 2c20 5b28 7265  ery), '->', [(re
+00019f00: 6369 7065 2e69 642c 2073 636f 7265 2920  cipe.id, score) 
+00019f10: 666f 7220 7265 6369 7065 2c20 7363 6f72  for recipe, scor
+00019f20: 6520 696e 206d 6174 6368 6573 5d29 0a20  e in matches]). 
+00019f30: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00019f40: 7365 6c66 2e73 7562 5465 7374 2871 7565  self.subTest(que
+00019f50: 7279 3d71 7565 7279 293a 0a20 2020 2020  ry=query):.     
+00019f60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019f70: 6173 7365 7274 4571 7561 6c28 6578 7065  assertEqual(expe
+00019f80: 6374 6564 2c20 6d61 7463 685f 6964 732c  cted, match_ids,
+00019f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019fb0: 2020 6622 696e 7661 6c69 6420 7265 7375    f"invalid resu
+00019fc0: 6c74 7320 666f 7220 7175 6572 7920 7b71  lts for query {q
+00019fd0: 7565 7279 2172 7d2c 2065 7870 6563 7465  uery!r}, expecte
+00019fe0: 6420 7b65 7870 6563 7465 647d 2c20 676f  d {expected}, go
+00019ff0: 7420 7b6d 6174 6368 5f69 6473 7d22 290a  t {match_ids}").
+0001a000: 0a20 2020 2040 616e 6e6f 756e 6365 5f74  .    @announce_t
+0001a010: 6573 740a 2020 2020 6465 6620 7465 7374  est.    def test
+0001a020: 5f73 6561 7263 685f 7769 7468 5f61 735f  _search_with_as_
+0001a030: 7461 626c 6528 7365 6c66 293a 0a20 2020  table(self):.   
+0001a040: 2020 2020 2066 6f72 2071 7565 7279 2c20       for query, 
+0001a050: 6578 7065 6374 6564 2069 6e20 5b0a 2020  expected in [.  
+0001a060: 2020 2020 2020 2020 2020 2822 222c 205b            ("", [
+0001a070: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+0001a080: 2822 7475 6e61 222c 205b 5d29 2c0a 2020  ("tuna", []),.  
+0001a090: 2020 2020 2020 2020 2020 2822 7475 6e61            ("tuna
+0001a0a0: 202b 6368 6565 7365 222c 205b 362c 5d29   +cheese", [6,])
+0001a0b0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
+0001a0c0: 7069 6e65 6170 706c 6520 2b62 6163 6f6e  pineapple +bacon
+0001a0d0: 206c 6574 7475 6365 2062 6565 6620 2d73   lettuce beef -s
+0001a0e0: 6175 6572 6b72 6175 7420 746f 6d61 746f  auerkraut tomato
+0001a0f0: 222c 205b 392c 2031 335d 292c 0a20 2020  ", [9, 13]),.   
+0001a100: 2020 2020 2020 2020 2028 2270 697a 7a61           ("pizza
+0001a110: 2064 6f75 6768 202d 7069 6e65 6170 706c   dough -pineappl
+0001a120: 6522 2c20 5b5d 292c 0a20 2020 2020 2020  e", []),.       
+0001a130: 2020 2020 2028 2270 697a 7a61 2064 6f75       ("pizza dou
+0001a140: 6768 202d 2d70 696e 6561 7070 6c65 222c  gh --pineapple",
+0001a150: 205b 5d29 2c0a 2020 2020 2020 2020 2020   []),.          
+0001a160: 2020 2822 6272 6561 6420 6261 636f 6e22    ("bread bacon"
+0001a170: 2c20 5b5d 292c 0a20 2020 2020 2020 2020  , []),.         
+0001a180: 2020 2028 2262 7265 6164 202b 2b62 6163     ("bread ++bac
+0001a190: 6f6e 222c 205b 392c 5d29 2c0a 2020 2020  on", [9,]),.    
+0001a1a0: 2020 2020 2020 2020 2822 6272 6561 6420          ("bread 
+0001a1b0: 2b2b 616e 6368 6f76 6965 7322 2c20 5b5d  ++anchovies", []
+0001a1c0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0001a1d0: 2262 7265 6164 202b 2b62 6163 6f6e 202b  "bread ++bacon +
+0001a1e0: 2b61 6e63 686f 7669 6573 222c 205b 5d29  +anchovies", [])
+0001a1f0: 2c0a 2020 2020 2020 2020 2020 2020 2822  ,.            ("
+0001a200: 6272 6561 6420 6261 636f 6e20 2d2d 616e  bread bacon --an
+0001a210: 6368 6f76 6965 7322 2c20 5b5d 292c 0a20  chovies", []),. 
+0001a220: 2020 2020 2020 205d 3a0a 2020 2020 2020         ]:.      
+0001a230: 2020 2020 2020 6d61 7463 6865 7320 3d20        matches = 
+0001a240: 7365 6c66 2e72 6563 6970 6573 2e73 6561  self.recipes.sea
+0001a250: 7263 682e 696e 6772 6564 6965 6e74 7328  rch.ingredients(
+0001a260: 7175 6572 792c 206d 696e 5f73 636f 7265  query, min_score
+0001a270: 3d31 3030 302c 2061 735f 7461 626c 653d  =1000, as_table=
+0001a280: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+0001a290: 2020 6d61 7463 685f 6964 7320 3d20 5b72    match_ids = [r
+0001a2a0: 6563 6970 652e 6964 2066 6f72 2072 6563  ecipe.id for rec
+0001a2b0: 6970 6520 696e 206d 6174 6368 6573 5d0a  ipe in matches].
+0001a2c0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0001a2d0: 7428 7265 7072 2871 7565 7279 292c 2027  t(repr(query), '
+0001a2e0: 2d3e 272c 205b 2872 6563 6970 652e 6964  ->', [(recipe.id
+0001a2f0: 2c20 7265 6369 7065 2e69 6e67 7265 6469  , recipe.ingredi
+0001a300: 656e 7473 5f73 6561 7263 685f 7363 6f72  ents_search_scor
+0001a310: 6529 2066 6f72 2072 6563 6970 6520 696e  e) for recipe in
+0001a320: 206d 6174 6368 6573 5d29 0a20 2020 2020   matches]).     
+0001a330: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+0001a340: 2e73 7562 5465 7374 2871 7565 7279 3d71  .subTest(query=q
+0001a350: 7565 7279 293a 0a20 2020 2020 2020 2020  uery):.         
+0001a360: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001a370: 7274 4571 7561 6c28 6578 7065 6374 6564  rtEqual(expected
+0001a380: 2c20 6d61 7463 685f 6964 732c 0a20 2020  , match_ids,.   
+0001a390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a3a0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0001a3b0: 696e 7661 6c69 6420 7265 7375 6c74 7320  invalid results 
+0001a3c0: 666f 7220 7175 6572 7920 7b71 7565 7279  for query {query
+0001a3d0: 2172 7d2c 2065 7870 6563 7465 6420 7b65  !r}, expected {e
+0001a3e0: 7870 6563 7465 647d 2c20 676f 7420 7b6d  xpected}, got {m
+0001a3f0: 6174 6368 5f69 6473 7d22 290a 0a20 2020  atch_ids}")..   
+0001a400: 2020 2020 2020 2020 2073 636f 7265 5f61           score_a
+0001a410: 7474 7220 3d20 2269 6e67 7265 6469 656e  ttr = "ingredien
+0001a420: 7473 5f73 6561 7263 685f 7363 6f72 6522  ts_search_score"
+0001a430: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001a440: 662e 6173 7365 7274 5472 7565 280a 2020  f.assertTrue(.  
+0001a450: 2020 2020 2020 2020 2020 2020 2020 616c                al
+0001a460: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+0001a470: 2020 2020 2020 2068 6173 6174 7472 286d         hasattr(m
+0001a480: 6174 6368 6573 2e62 792e 6964 5b6d 6964  atches.by.id[mid
+0001a490: 5d2c 2073 636f 7265 5f61 7474 7229 0a20  ], score_attr). 
+0001a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4b0: 2020 2066 6f72 206d 6964 2069 6e20 6d61     for mid in ma
+0001a4c0: 7463 685f 6964 730a 2020 2020 2020 2020  tch_ids.        
+0001a4d0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+0001a4e0: 2020 2020 2020 2020 2020 2066 2261 735f             f"as_
+0001a4f0: 7461 626c 6520 6469 6420 6e6f 7420 706f  table did not po
+0001a500: 7075 6c61 7465 2073 6f6d 6520 7365 6172  pulate some sear
+0001a510: 6368 2072 6563 6f72 6473 2077 6974 6820  ch records with 
+0001a520: 7b73 636f 7265 5f61 7474 7221 727d 220a  {score_attr!r}".
+0001a530: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+0001a540: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001a550: 6173 7365 7274 4661 6c73 6528 0a20 2020  assertFalse(.   
+0001a560: 2020 2020 2020 2020 2020 2020 2061 6e79               any
+0001a570: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0001a580: 2020 2020 2020 6861 7361 7474 7228 7365        hasattr(se
+0001a590: 6c66 2e72 6563 6970 6573 2e62 792e 6964  lf.recipes.by.id
+0001a5a0: 5b6d 6964 5d2c 2073 636f 7265 5f61 7474  [mid], score_att
+0001a5b0: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
+0001a5c0: 2020 2020 2020 2066 6f72 206d 6964 2069         for mid i
+0001a5d0: 6e20 6d61 7463 685f 6964 730a 2020 2020  n match_ids.    
+0001a5e0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+0001a5f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001a600: 2261 735f 7461 626c 6520 706f 7075 6c61  "as_table popula
+0001a610: 7465 6420 736f 6d65 206f 7269 6769 6e61  ted some origina
+0001a620: 6c20 7265 636f 7264 7320 7769 7468 207b  l records with {
+0001a630: 7363 6f72 655f 6174 7472 2172 7d22 0a20  score_attr!r}". 
+0001a640: 2020 2020 2020 2020 2020 2029 0a0a 636c             )..cl
+0001a650: 6173 7320 5461 626c 6553 6561 7263 6854  ass TableSearchT
+0001a660: 6573 7473 5f44 6174 614f 626a 6563 7473  ests_DataObjects
+0001a670: 2854 6162 6c65 5365 6172 6368 5465 7374  (TableSearchTest
+0001a680: 732c 2055 7369 6e67 4461 7461 4f62 6a65  s, UsingDataObje
+0001a690: 6374 7329 3a0a 2020 2020 7061 7373 0a0a  cts):.    pass..
+0001a6a0: 636c 6173 7320 5461 626c 6553 6561 7263  class TableSearc
+0001a6b0: 6854 6573 7473 5f4e 616d 6564 7475 706c  hTests_Namedtupl
+0001a6c0: 6573 2854 6162 6c65 5365 6172 6368 5465  es(TableSearchTe
+0001a6d0: 7374 732c 2055 7369 6e67 4e61 6d65 6474  sts, UsingNamedt
+0001a6e0: 7570 6c65 7329 3a0a 2020 2020 7061 7373  uples):.    pass
+0001a6f0: 0a0a 636c 6173 7320 5461 626c 6553 6561  ..class TableSea
+0001a700: 7263 6854 6573 7473 5f54 7970 696e 674e  rchTests_TypingN
+0001a710: 616d 6564 7475 706c 6573 2854 6162 6c65  amedtuples(Table
+0001a720: 5365 6172 6368 5465 7374 732c 2055 7369  SearchTests, Usi
+0001a730: 6e67 5479 7069 6e67 4e61 6d65 6454 7570  ngTypingNamedTup
+0001a740: 6c65 293a 0a20 2020 2070 6173 730a 0a63  le):.    pass..c
+0001a750: 6c61 7373 2054 6162 6c65 5365 6172 6368  lass TableSearch
+0001a760: 5465 7374 735f 5479 7069 6e67 5479 7065  Tests_TypingType
+0001a770: 6444 6963 7428 5461 626c 6553 6561 7263  dDict(TableSearc
+0001a780: 6854 6573 7473 2c20 5573 696e 6754 7970  hTests, UsingTyp
+0001a790: 696e 6754 7970 6564 4469 6374 293a 0a20  ingTypedDict):. 
+0001a7a0: 2020 2070 6173 730a 0a63 6c61 7373 2054     pass..class T
+0001a7b0: 6162 6c65 5365 6172 6368 5465 7374 735f  ableSearchTests_
+0001a7c0: 536c 6f74 7465 6428 5461 626c 6553 6561  Slotted(TableSea
+0001a7d0: 7263 6854 6573 7473 2c20 5573 696e 6753  rchTests, UsingS
+0001a7e0: 6c6f 7474 6564 4f62 6a65 6374 7329 3a0a  lottedObjects):.
+0001a7f0: 2020 2020 7061 7373 0a0a 636c 6173 7320      pass..class 
+0001a800: 5461 626c 6553 6561 7263 6854 6573 7473  TableSearchTests
+0001a810: 5f53 696d 706c 654e 616d 6573 7061 6365  _SimpleNamespace
+0001a820: 2854 6162 6c65 5365 6172 6368 5465 7374  (TableSearchTest
+0001a830: 732c 2055 7369 6e67 5369 6d70 6c65 4e61  s, UsingSimpleNa
+0001a840: 6d65 7370 6163 6529 3a0a 2020 2020 7061  mespace):.    pa
+0001a850: 7373 0a0a 6966 2064 6174 6163 6c61 7373  ss..if dataclass
+0001a860: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
+0001a870: 2020 2020 636c 6173 7320 5461 626c 6553      class TableS
+0001a880: 6561 7263 6854 6573 7473 5f44 6174 6163  earchTests_Datac
+0001a890: 6c61 7373 6573 2854 6162 6c65 5365 6172  lasses(TableSear
+0001a8a0: 6368 5465 7374 732c 2055 7369 6e67 4461  chTests, UsingDa
+0001a8b0: 7461 636c 6173 7365 7329 3a0a 2020 2020  taclasses):.    
+0001a8c0: 2020 2020 7061 7373 0a0a 6966 2070 7964      pass..if pyd
+0001a8d0: 616e 7469 6320 6973 206e 6f74 204e 6f6e  antic is not Non
+0001a8e0: 653a 0a20 2020 2063 6c61 7373 2054 6162  e:.    class Tab
+0001a8f0: 6c65 5365 6172 6368 5465 7374 735f 5079  leSearchTests_Py
+0001a900: 6461 6e74 6963 4d6f 6465 6c73 2854 6162  danticModels(Tab
+0001a910: 6c65 5365 6172 6368 5465 7374 732c 2055  leSearchTests, U
+0001a920: 7369 6e67 5079 6461 6e74 6963 4d6f 6465  singPydanticMode
+0001a930: 6c29 3a0a 2020 2020 2020 2020 7061 7373  l):.        pass
+0001a940: 0a0a 2020 2020 636c 6173 7320 5461 626c  ..    class Tabl
+0001a950: 6553 6561 7263 6854 6573 7473 5f50 7964  eSearchTests_Pyd
+0001a960: 616e 7469 6349 6d6d 7574 6162 6c65 4d6f  anticImmutableMo
+0001a970: 6465 6c73 2854 6162 6c65 5365 6172 6368  dels(TableSearch
+0001a980: 5465 7374 732c 2055 7369 6e67 5079 6461  Tests, UsingPyda
+0001a990: 6e74 6963 496d 6d75 7461 626c 654d 6f64  nticImmutableMod
+0001a9a0: 656c 293a 0a20 2020 2020 2020 2070 6173  el):.        pas
+0001a9b0: 730a 0a20 2020 2063 6c61 7373 2054 6162  s..    class Tab
+0001a9c0: 6c65 5365 6172 6368 5465 7374 735f 5079  leSearchTests_Py
+0001a9d0: 6461 6e74 6963 4f52 4d4d 6f64 656c 7328  danticORMModels(
+0001a9e0: 5461 626c 6553 6561 7263 6854 6573 7473  TableSearchTests
+0001a9f0: 2c20 5573 696e 6750 7964 616e 7469 634f  , UsingPydanticO
+0001aa00: 524d 4d6f 6465 6c29 3a0a 2020 2020 2020  RMModel):.      
+0001aa10: 2020 7061 7373 0a0a 6966 2061 7474 7220    pass..if attr 
+0001aa20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0001aa30: 2063 6c61 7373 2054 6162 6c65 5365 6172   class TableSear
+0001aa40: 6368 5465 7374 735f 4174 7472 436c 6173  chTests_AttrClas
+0001aa50: 7365 7328 5461 626c 6553 6561 7263 6854  ses(TableSearchT
+0001aa60: 6573 7473 2c20 5573 696e 6741 7474 7243  ests, UsingAttrC
+0001aa70: 6c61 7373 293a 0a20 2020 2020 2020 2070  lass):.        p
+0001aa80: 6173 730a 0a69 6620 7472 6169 746c 6574  ass..if traitlet
+0001aa90: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+0001aaa0: 2020 2063 6c61 7373 2054 6162 6c65 5365     class TableSe
+0001aab0: 6172 6368 5465 7374 735f 5472 6169 746c  archTests_Traitl
+0001aac0: 6574 7343 6c61 7373 6573 2854 6162 6c65  etsClasses(Table
+0001aad0: 5365 6172 6368 5465 7374 732c 2055 7369  SearchTests, Usi
+0001aae0: 6e67 5472 6169 746c 6574 7343 6c61 7373  ngTraitletsClass
+0001aaf0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+0001ab00: 0a69 6620 536c 6f74 7465 6457 6974 6844  .if SlottedWithD
+0001ab10: 6963 7420 6973 206e 6f74 204e 6f6e 653a  ict is not None:
+0001ab20: 0a20 2020 2063 6c61 7373 2054 6162 6c65  .    class Table
+0001ab30: 5365 6172 6368 5465 7374 735f 536c 6f74  SearchTests_Slot
+0001ab40: 7465 6457 6974 6844 6963 7428 5461 626c  tedWithDict(Tabl
+0001ab50: 6553 6561 7263 6854 6573 7473 2c20 5573  eSearchTests, Us
+0001ab60: 696e 6753 6c6f 7474 6564 5769 7468 4469  ingSlottedWithDi
+0001ab70: 6374 4f62 6a65 6374 7329 3a0a 2020 2020  ctObjects):.    
+0001ab80: 2020 2020 7061 7373 0a0a 0a63 6c61 7373      pass...class
+0001ab90: 2049 6e69 7469 616c 5465 7374 2875 6e69   InitialTest(uni
+0001aba0: 7474 6573 742e 5465 7374 4361 7365 293a  ttest.TestCase):
+0001abb0: 0a20 2020 2066 726f 6d20 6c69 7474 6c65  .    from little
+0001abc0: 7461 626c 6520 696d 706f 7274 2028 0a20  table import (. 
+0001abd0: 2020 2020 2020 205f 5f76 6572 7369 6f6e         __version
+0001abe0: 5f5f 2061 7320 6c69 7474 6c65 7461 626c  __ as littletabl
+0001abf0: 655f 7665 7273 696f 6e2c 0a20 2020 2020  e_version,.     
+0001ac00: 2020 205f 5f76 6572 7369 6f6e 5f74 696d     __version_tim
+0001ac10: 655f 5f20 6173 206c 6974 746c 6574 6162  e__ as littletab
+0001ac20: 6c65 5f76 6572 7369 6f6e 5f74 696d 652c  le_version_time,
+0001ac30: 0a20 2020 2020 2020 205f 5f76 6572 7369  .        __versi
+0001ac40: 6f6e 5f69 6e66 6f5f 5f20 6173 206c 6974  on_info__ as lit
+0001ac50: 746c 6574 6162 6c65 5f76 6572 7369 6f6e  tletable_version
+0001ac60: 5f69 6e66 6f2c 0a20 2020 2029 0a0a 2020  _info,.    )..  
+0001ac70: 2020 7072 696e 7428 0a20 2020 2020 2020    print(.       
+0001ac80: 2066 2242 6567 696e 6e69 6e67 2074 6573   f"Beginning tes
+0001ac90: 7420 6f66 206c 6974 746c 6574 6162 6c65  t of littletable
+0001aca0: 2c20 7665 7273 696f 6e20 7b6c 6974 746c  , version {littl
+0001acb0: 6574 6162 6c65 5f76 6572 7369 6f6e 7d2c  etable_version},
+0001acc0: 207b 6c69 7474 6c65 7461 626c 655f 7665   {littletable_ve
+0001acd0: 7273 696f 6e5f 7469 6d65 7d22 2c0a 2020  rsion_time}",.  
+0001ace0: 2020 290a 2020 2020 7072 696e 7428 6c69    ).    print(li
+0001acf0: 7474 6c65 7461 626c 655f 7665 7273 696f  ttletable_versio
+0001ad00: 6e5f 696e 666f 290a 2020 2020 7072 696e  n_info).    prin
+0001ad10: 7428 2250 7974 686f 6e20 7665 7273 696f  t("Python versio
+0001ad20: 6e22 2c20 7379 732e 7665 7273 696f 6e29  n", sys.version)
+0001ad30: 0a20 2020 2070 7269 6e74 2829 0a0a 0a63  .    print()...c
+0001ad40: 6c61 7373 2053 746f 7261 6765 496e 6465  lass StorageInde
+0001ad50: 7065 6e64 656e 7454 6573 7473 2875 6e69  pendentTests(uni
+0001ad60: 7474 6573 742e 5465 7374 4361 7365 293a  ttest.TestCase):
+0001ad70: 0a20 2020 2040 616e 6e6f 756e 6365 5f74  .    @announce_t
+0001ad80: 6573 740a 2020 2020 6465 6620 7465 7374  est.    def test
+0001ad90: 5f6e 6f72 6d61 6c69 7a65 5f73 7472 2873  _normalize_str(s
+0001ada0: 656c 6629 3a0a 2020 2020 2020 2020 666f  elf):.        fo
+0001adb0: 7220 696e 5f77 6f72 642c 2065 7870 6563  r in_word, expec
+0001adc0: 7465 645f 776f 7264 2069 6e20 5b0a 2020  ted_word in [.  
+0001add0: 2020 2020 2020 2020 2020 2822 6e6f 6368            ("noch
+0001ade0: 616e 6765 222c 2022 6e6f 6368 616e 6765  ange", "nochange
+0001adf0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+0001ae00: 2822 546f 4c6f 7765 7222 2c20 2274 6f6c  ("ToLower", "tol
+0001ae10: 6f77 6572 2229 2c0a 2020 2020 2020 2020  ower"),.        
+0001ae20: 2020 2020 2822 492e 422e 4d2e 222c 2022      ("I.B.M.", "
+0001ae30: 6962 6d22 292c 0a20 2020 2020 2020 2020  ibm"),.         
+0001ae40: 2020 2028 2247 2e45 2e22 2c20 2267 6522     ("G.E.", "ge"
+0001ae50: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0001ae60: 224d 2e22 2c20 226d 2229 2c0a 2020 2020  "M.", "m"),.    
+0001ae70: 2020 2020 2020 2020 2822 4d2e 7879 7a22          ("M.xyz"
+0001ae80: 2c20 226d 2229 2c0a 2020 2020 2020 2020  , "m"),.        
+0001ae90: 2020 2020 2822 2a78 7878 2d68 6868 222c      ("*xxx-hhh",
+0001aea0: 2022 7878 782d 6868 6822 292c 0a20 2020   "xxx-hhh"),.   
+0001aeb0: 2020 2020 2020 2020 2028 222b 626c 6168           ("+blah
+0001aec0: 466f 6f22 2c20 2262 6c61 6866 6f6f 2229  Foo", "blahfoo")
+0001aed0: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+0001aee0: 2822 666f 7865 7322 2c20 2266 6f78 2229  ("foxes", "fox")
+0001aef0: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+0001af00: 2822 6368 7572 6368 6573 222c 2022 6368  ("churches", "ch
+0001af10: 7572 6368 2229 2c0a 2020 2020 2020 2020  urch"),.        
+0001af20: 2020 2020 2320 2822 6472 6573 7365 7322      # ("dresses"
+0001af30: 2c20 2264 7265 7373 2229 2c0a 2020 2020  , "dress"),.    
+0001af40: 2020 2020 5d3a 0a20 2020 2020 2020 2020      ]:.         
+0001af50: 2020 2077 6974 6820 7365 6c66 2e73 7562     with self.sub
+0001af60: 5465 7374 2869 6e5f 776f 7264 293a 0a20  Test(in_word):. 
+0001af70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001af80: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001af90: 6578 7065 6374 6564 5f77 6f72 642c 206c  expected_word, l
+0001afa0: 742e 5461 626c 652e 5f6e 6f72 6d61 6c69  t.Table._normali
+0001afb0: 7a65 5f77 6f72 6428 696e 5f77 6f72 6429  ze_word(in_word)
+0001afc0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+0001afd0: 6e6f 726d 616c 697a 655f 7374 725f 6765  normalize_str_ge
+0001afe0: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
+0001aff0: 2066 6f72 2069 6e5f 776f 7264 2c20 6578   for in_word, ex
+0001b000: 7065 6374 6564 5f77 6f72 6473 2069 6e20  pected_words in 
+0001b010: 5b0a 2020 2020 2020 2020 2020 2020 2822  [.            ("
+0001b020: 6e6f 6368 616e 6765 222c 205b 226e 6f63  nochange", ["noc
+0001b030: 6861 6e67 6522 5d29 2c0a 2020 2020 2020  hange"]),.      
+0001b040: 2020 2020 2020 2822 546f 4c6f 7765 7222        ("ToLower"
+0001b050: 2c20 5b22 746f 6c6f 7765 7222 5d29 2c0a  , ["tolower"]),.
+0001b060: 2020 2020 2020 2020 2020 2020 2822 492e              ("I.
+0001b070: 422e 4d2e 222c 205b 2269 2e62 2e6d 2e22  B.M.", ["i.b.m."
+0001b080: 2c20 2269 626d 225d 292c 0a20 2020 2020  , "ibm"]),.     
+0001b090: 2020 2020 2020 2028 2247 2e45 2e22 2c20         ("G.E.", 
+0001b0a0: 5b22 672e 652e 222c 2022 6765 225d 292c  ["g.e.", "ge"]),
+0001b0b0: 0a20 2020 2020 2020 2020 2020 2028 2241  .            ("A
+0001b0c0: 2e49 2e22 2c20 5b22 612e 692e 222c 2022  .I.", ["a.i.", "
+0001b0d0: 6169 225d 292c 0a20 2020 2020 2020 2020  ai"]),.         
+0001b0e0: 2020 2028 2241 4922 2c20 5b22 6169 225d     ("AI", ["ai"]
+0001b0f0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0001b100: 224d 2e22 2c20 5b22 6d22 5d29 2c0a 2020  "M.", ["m"]),.  
+0001b110: 2020 2020 2020 2020 2020 2822 6d6d 2e78            ("mm.x
+0001b120: 797a 222c 205b 226d 6d22 2c20 226d 6d2e  yz", ["mm", "mm.
+0001b130: 7879 7a22 2c20 2278 797a 225d 292c 0a20  xyz", "xyz"]),. 
+0001b140: 2020 2020 2020 2020 2020 2028 224d 4d2e             ("MM.
+0001b150: 7879 7a22 2c20 5b22 6d6d 222c 2022 6d6d  xyz", ["mm", "mm
+0001b160: 2e78 797a 222c 2022 7879 7a22 5d29 2c0a  .xyz", "xyz"]),.
+0001b170: 2020 2020 2020 2020 2020 2020 2822 5468              ("Th
+0001b180: 7265 6164 696e 672e 6973 416c 6976 6528  reading.isAlive(
+0001b190: 2922 2c20 5b27 6973 616c 6976 6527 2c20  )", ['isalive', 
+0001b1a0: 2774 6872 6561 6469 6e67 272c 2027 7468  'threading', 'th
+0001b1b0: 7265 6164 696e 672e 6973 616c 6976 6527  reading.isalive'
+0001b1c0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+0001b1d0: 2822 2a78 7878 2d68 6868 222c 205b 2768  ("*xxx-hhh", ['h
+0001b1e0: 6868 272c 2027 7878 7827 2c20 2778 7878  hh', 'xxx', 'xxx
+0001b1f0: 2d68 6868 275d 292c 0a20 2020 2020 2020  -hhh']),.       
+0001b200: 2020 2020 2028 222b 626c 6168 466f 6f22       ("+blahFoo"
+0001b210: 2c20 5b22 626c 6168 666f 6f22 5d29 2c0a  , ["blahfoo"]),.
+0001b220: 2020 2020 2020 2020 2020 2020 2822 7374              ("st
+0001b230: 722e 6c73 7472 6970 222c 205b 226c 7374  r.lstrip", ["lst
+0001b240: 7269 7022 2c20 2273 7472 222c 2022 7374  rip", "str", "st
+0001b250: 722e 6c73 7472 6970 225d 292c 0a20 2020  r.lstrip"]),.   
+0001b260: 2020 2020 2020 2020 2028 2273 7472 2e6c           ("str.l
+0001b270: 7374 7269 7028 2922 2c20 5b22 6c73 7472  strip()", ["lstr
+0001b280: 6970 222c 2022 7374 7222 2c20 2273 7472  ip", "str", "str
+0001b290: 2e6c 7374 7269 7022 5d29 2c0a 2020 2020  .lstrip"]),.    
+0001b2a0: 2020 2020 2020 2020 2822 7365 6c66 2e61          ("self.a
+0001b2b0: 7373 6572 7445 7175 616c 7322 2c20 5b22  ssertEquals", ["
+0001b2c0: 6173 7365 7274 6571 7561 6c73 222c 2022  assertequals", "
+0001b2d0: 7365 6c66 222c 2022 7365 6c66 2e61 7373  self", "self.ass
+0001b2e0: 6572 7465 7175 616c 7322 5d29 2c0a 2020  ertequals"]),.  
+0001b2f0: 2020 2020 2020 2020 2020 2822 5465 7374            ("Test
+0001b300: 4361 7365 2e61 7373 6572 7445 7175 616c  Case.assertEqual
+0001b310: 7322 2c20 5b22 6173 7365 7274 6571 7561  s", ["assertequa
+0001b320: 6c73 222c 2022 7465 7374 6361 7365 222c  ls", "testcase",
+0001b330: 2022 7465 7374 6361 7365 2e61 7373 6572   "testcase.asser
+0001b340: 7465 7175 616c 7322 5d29 2c0a 2020 2020  tequals"]),.    
+0001b350: 2020 2020 2020 2020 2822 756e 6974 7465          ("unitte
+0001b360: 7374 2e54 6573 7443 6173 652e 6173 7365  st.TestCase.asse
+0001b370: 7274 4571 7561 6c73 222c 0a20 2020 2020  rtEquals",.     
+0001b380: 2020 2020 2020 2020 5b22 6173 7365 7274          ["assert
+0001b390: 6571 7561 6c73 222c 2022 7465 7374 6361  equals", "testca
+0001b3a0: 7365 222c 2022 756e 6974 7465 7374 222c  se", "unittest",
+0001b3b0: 2022 756e 6974 7465 7374 2e74 6573 7463   "unittest.testc
+0001b3c0: 6173 652e 6173 7365 7274 6571 7561 6c73  ase.assertequals
+0001b3d0: 225d 292c 0a20 2020 2020 2020 2020 2020  "]),.           
+0001b3e0: 2028 2266 6f78 6573 222c 205b 2266 6f78   ("foxes", ["fox
+0001b3f0: 222c 2022 666f 7865 7322 5d29 2c0a 2020  ", "foxes"]),.  
+0001b400: 2020 2020 2020 2020 2020 2822 6368 7572            ("chur
+0001b410: 6368 6573 222c 205b 2263 6875 7263 6822  ches", ["church"
+0001b420: 2c20 2263 6875 7263 6865 7322 5d29 2c0a  , "churches"]),.
+0001b430: 2020 2020 2020 2020 2020 2020 2822 6472              ("dr
+0001b440: 6573 7365 7322 2c20 5b22 6472 6573 7322  esses", ["dress"
+0001b450: 2c20 2264 7265 7373 6573 225d 292c 0a20  , "dresses"]),. 
+0001b460: 2020 2020 2020 2020 2020 2028 2264 7265             ("dre
+0001b470: 7373 222c 205b 2264 7265 7373 222c 205d  ss", ["dress", ]
+0001b480: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0001b490: 2262 6961 7322 2c20 5b22 6269 6173 222c  "bias", ["bias",
+0001b4a0: 205d 292c 0a20 2020 2020 2020 2020 2020   ]),.           
+0001b4b0: 2028 2274 6f79 7322 2c20 5b22 746f 7922   ("toys", ["toy"
+0001b4c0: 2c20 2274 6f79 7322 5d29 2c0a 2020 2020  , "toys"]),.    
+0001b4d0: 2020 2020 2020 2020 2822 6261 6269 6573          ("babies
+0001b4e0: 222c 205b 2262 6162 6965 7322 2c20 2262  ", ["babies", "b
+0001b4f0: 6162 7922 5d29 2c0a 2020 2020 2020 2020  aby"]),.        
+0001b500: 2020 2020 2822 6164 6465 6e64 6122 2c20      ("addenda", 
+0001b510: 5b22 6164 6465 6e64 6122 2c20 2261 6464  ["addenda", "add
+0001b520: 656e 6475 6d22 5d29 2c0a 2020 2020 2020  endum"]),.      
+0001b530: 2020 2020 2020 2822 7261 6269 6573 222c        ("rabies",
+0001b540: 205b 2272 6162 6965 7322 5d29 2c0a 2020   ["rabies"]),.  
+0001b550: 2020 2020 2020 2020 2020 2822 6c61 7a69            ("lazi
+0001b560: 6e65 7373 222c 205b 226c 617a 696e 6573  ness", ["lazines
+0001b570: 7322 5d29 2c0a 2020 2020 2020 2020 2020  s"]),.          
+0001b580: 2020 2822 7068 7973 6963 7322 2c20 5b22    ("physics", ["
+0001b590: 7068 7973 6963 7322 5d29 2c0a 2020 2020  physics"]),.    
+0001b5a0: 2020 2020 2020 2020 2822 5079 7468 6f6e          ("Python
+0001b5b0: 2773 222c 205b 2270 7974 686f 6e22 5d29  's", ["python"])
+0001b5c0: 2c0a 2020 2020 2020 2020 2020 2020 2827  ,.            ('
+0001b5d0: 5661 6c75 6545 7272 6f72 272c 205b 2765  ValueError', ['e
+0001b5e0: 7272 6f72 272c 2027 7661 6c75 6565 7272  rror', 'valueerr
+0001b5f0: 6f72 275d 292c 0a20 2020 2020 2020 2020  or']),.         
+0001b600: 2020 2028 2744 6570 7265 6361 7469 6f6e     ('Deprecation
+0001b610: 5761 726e 696e 6727 2c20 5b27 6465 7072  Warning', ['depr
+0001b620: 6563 6174 696f 6e77 6172 6e69 6e67 272c  ecationwarning',
+0001b630: 2027 7761 726e 696e 6727 5d29 2c0a 2020   'warning']),.  
+0001b640: 2020 2020 2020 2020 2020 2827 4375 7374            ('Cust
+0001b650: 6f6d 4578 6365 7074 696f 6e27 2c20 5b27  omException', ['
+0001b660: 6375 7374 6f6d 6578 6365 7074 696f 6e27  customexception'
+0001b670: 2c20 2765 7863 6570 7469 6f6e 275d 292c  , 'exception']),
+0001b680: 0a20 2020 2020 2020 2020 2020 2028 2774  .            ('t
+0001b690: 6572 726f 7227 2c20 5b27 7465 7272 6f72  error', ['terror
+0001b6a0: 275d 292c 0a20 2020 2020 2020 2020 2020  ']),.           
+0001b6b0: 2028 2765 7272 6f72 272c 205b 2765 7272   ('error', ['err
+0001b6c0: 6f72 275d 292c 0a20 2020 2020 2020 205d  or']),.        ]
+0001b6d0: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
+0001b6e0: 7468 2073 656c 662e 7375 6254 6573 7428  th self.subTest(
+0001b6f0: 696e 5f77 6f72 6429 3a0a 2020 2020 2020  in_word):.      
+0001b700: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0001b710: 7373 6572 7445 7175 616c 2865 7870 6563  ssertEqual(expec
+0001b720: 7465 645f 776f 7264 732c 0a20 2020 2020  ted_words,.     
+0001b730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b740: 2020 2020 2020 2020 2020 2020 736f 7274              sort
+0001b750: 6564 286c 6973 7428 6c74 2e54 6162 6c65  ed(list(lt.Table
+0001b760: 2e5f 6e6f 726d 616c 697a 655f 776f 7264  ._normalize_word
+0001b770: 5f67 656e 2869 6e5f 776f 7264 2c20 6672  _gen(in_word, fr
+0001b780: 6f7a 656e 7365 7428 2929 2929 290a 0a20  ozenset())))).. 
+0001b790: 2020 2040 616e 6e6f 756e 6365 5f74 6573     @announce_tes
+0001b7a0: 740a 2020 2020 6465 6620 7465 7374 5f6e  t.    def test_n
+0001b7b0: 6f72 6d61 6c69 7a65 5f73 706c 6974 2873  ormalize_split(s
+0001b7c0: 656c 6629 3a0a 2020 2020 2020 2020 666f  elf):.        fo
+0001b7d0: 7220 696e 5f73 7472 2c20 6578 7065 6374  r in_str, expect
+0001b7e0: 6564 5f73 7472 5f73 6574 2069 6e20 5b0a  ed_str_set in [.
+0001b7f0: 2020 2020 2020 2020 2020 2020 2822 7374              ("st
+0001b800: 722e 6c73 7472 6970 2829 222c 205b 226c  r.lstrip()", ["l
+0001b810: 7374 7269 7022 2c20 2273 7472 222c 2022  strip", "str", "
+0001b820: 7374 722e 6c73 7472 6970 225d 292c 0a20  str.lstrip"]),. 
+0001b830: 2020 2020 2020 2020 2020 2028 2273 7472             ("str
+0001b840: 2e6c 7374 7269 7028 2920 7374 722e 7273  .lstrip() str.rs
+0001b850: 7472 6970 2829 222c 205b 226c 7374 7269  trip()", ["lstri
+0001b860: 7022 2c20 2272 7374 7269 7022 2c20 2273  p", "rstrip", "s
+0001b870: 7472 222c 2022 7374 722e 6c73 7472 6970  tr", "str.lstrip
+0001b880: 222c 2022 7374 722e 7273 7472 6970 225d  ", "str.rstrip"]
+0001b890: 292c 0a20 2020 2020 2020 2020 2020 2023  ),.            #
+0001b8a0: 2028 2222 2c20 5b5d 292c 0a20 2020 2020   ("", []),.     
+0001b8b0: 2020 2020 2020 2023 2028 2222 2c20 5b5d         # ("", []
+0001b8c0: 292c 0a20 2020 2020 2020 2020 2020 2023  ),.            #
+0001b8d0: 2028 2222 2c20 5b5d 292c 0a20 2020 2020   ("", []),.     
+0001b8e0: 2020 205d 3a0a 2020 2020 2020 2020 2020     ]:.          
+0001b8f0: 2020 7769 7468 2073 656c 662e 7375 6254    with self.subT
+0001b900: 6573 7428 696e 5f73 7472 293a 0a20 2020  est(in_str):.   
+0001b910: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001b920: 662e 6173 7365 7274 4571 7561 6c28 6578  f.assertEqual(ex
+0001b930: 7065 6374 6564 5f73 7472 5f73 6574 2c0a  pected_str_set,.
+0001b940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b960: 2073 6f72 7465 6428 7365 7428 6c74 2e54   sorted(set(lt.T
+0001b970: 6162 6c65 2e5f 6e6f 726d 616c 697a 655f  able._normalize_
+0001b980: 7370 6c69 7428 696e 5f73 7472 2929 2929  split(in_str))))
+0001b990: 0a0a 2020 2020 4061 6e6e 6f75 6e63 655f  ..    @announce_
+0001b9a0: 7465 7374 0a20 2020 2064 6566 2074 6573  test.    def tes
+0001b9b0: 745f 706c 7572 616c 735f 7769 7468 5f74  t_plurals_with_t
+0001b9c0: 7261 696c 696e 675f 7075 6e63 7475 6174  railing_punctuat
+0001b9d0: 696f 6e28 7365 6c66 293a 0a20 2020 2020  ion(self):.     
+0001b9e0: 2020 2066 6f72 2028 6c69 6e65 2c20 6578     for (line, ex
+0001b9f0: 7065 6374 6564 2920 696e 205b 0a20 2020  pected) in [.   
+0001ba00: 2020 2020 2020 2020 2028 2749 2063 6f75           ('I cou
+0001ba10: 6c64 2068 6561 7220 7468 6520 6261 6269  ld hear the babi
+0001ba20: 6573 2063 7269 6573 2e27 2c20 5b27 6261  es cries.', ['ba
+0001ba30: 6269 6573 272c 2027 6261 6279 272c 2027  bies', 'baby', '
+0001ba40: 636f 756c 6427 2c20 2763 7269 6573 272c  could', 'cries',
+0001ba50: 2027 6372 7927 2c20 2768 6561 7227 2c20   'cry', 'hear', 
+0001ba60: 2769 272c 2027 7468 6527 5d29 2c0a 2020  'i', 'the']),.  
+0001ba70: 2020 2020 2020 2020 2020 2827 5768 6f20            ('Who 
+0001ba80: 6172 6520 7468 6f73 6520 6261 6269 6573  are those babies
+0001ba90: 3f27 2c20 5b27 6172 6527 2c20 2762 6162  ?', ['are', 'bab
+0001baa0: 6965 7327 2c20 2762 6162 7927 2c20 2774  ies', 'baby', 't
+0001bab0: 686f 7365 272c 2027 7768 6f27 5d29 2c0a  hose', 'who']),.
+0001bac0: 2020 2020 2020 2020 2020 2020 2822 5768              ("Wh
+0001bad0: 6f20 746f 6f6b 2074 6865 2062 6162 6965  o took the babie
+0001bae0: 7327 2072 6174 746c 6573 2074 6869 7320  s' rattles this 
+0001baf0: 7469 6d65 3f22 2c0a 2020 2020 2020 2020  time?",.        
+0001bb00: 2020 2020 205b 2762 6162 6965 7327 2c20       ['babies', 
+0001bb10: 2762 6162 7927 2c20 2772 6174 746c 6527  'baby', 'rattle'
+0001bb20: 2c20 2772 6174 746c 6573 272c 2027 7468  , 'rattles', 'th
+0001bb30: 6527 2c20 2774 6869 7327 2c20 2774 696d  e', 'this', 'tim
+0001bb40: 6527 2c20 2774 6f6f 6b27 2c20 2777 686f  e', 'took', 'who
+0001bb50: 275d 292c 0a20 2020 2020 2020 2020 2020  ']),.           
+0001bb60: 2028 2749 206c 6f76 6520 7468 6573 6520   ('I love these 
+0001bb70: 6361 6b65 7321 272c 205b 2763 616b 6527  cakes!', ['cake'
+0001bb80: 2c20 2763 616b 6573 272c 2027 6927 2c20  , 'cakes', 'i', 
+0001bb90: 276c 6f76 6527 2c20 2774 6865 7365 275d  'love', 'these']
+0001bba0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0001bbb0: 2757 6865 6e20 6d79 2077 6966 6520 636f  'When my wife co
+0001bbc0: 6f6b 732c 2073 6865 2062 616b 6573 2e27  oks, she bakes.'
+0001bbd0: 2c20 5b27 6261 6b65 272c 2027 6261 6b65  , ['bake', 'bake
+0001bbe0: 7327 2c20 2763 6f6f 6b27 2c20 2763 6f6f  s', 'cook', 'coo
+0001bbf0: 6b73 272c 2027 6d79 272c 2027 7368 6527  ks', 'my', 'she'
+0001bc00: 2c20 2777 6865 6e27 2c20 2777 6966 6527  , 'when', 'wife'
+0001bc10: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+0001bc20: 2822 4c65 7427 7320 676f 2073 686f 7070  ("Let's go shopp
+0001bc30: 696e 6720 666f 7220 616e 7469 7175 6573  ing for antiques
+0001bc40: 2122 2c20 5b27 616e 7469 7175 6527 2c20  !", ['antique', 
+0001bc50: 2761 6e74 6971 7565 7327 2c20 2766 6f72  'antiques', 'for
+0001bc60: 272c 2027 676f 272c 2027 6c65 7427 2c20  ', 'go', 'let', 
+0001bc70: 2773 686f 7070 696e 6727 5d29 2c0a 2020  'shopping']),.  
+0001bc80: 2020 2020 2020 2020 2020 2827 5468 6973            ('This
+0001bc90: 2069 7320 616e 2061 6e74 6971 7565 2076   is an antique v
+0001bca0: 6173 652c 2077 6f72 7468 2074 686f 7573  ase, worth thous
+0001bcb0: 616e 6473 2127 2c0a 2020 2020 2020 2020  ands!',.        
+0001bcc0: 2020 2020 205b 2761 6e27 2c20 2761 6e74       ['an', 'ant
+0001bcd0: 6971 7565 272c 2027 6973 272c 2027 7468  ique', 'is', 'th
+0001bce0: 6973 272c 2027 7468 6f75 7361 6e64 272c  is', 'thousand',
+0001bcf0: 2027 7468 6f75 7361 6e64 7327 2c20 2776   'thousands', 'v
+0001bd00: 6173 6527 2c20 2777 6f72 7468 275d 292c  ase', 'worth']),
+0001bd10: 0a20 2020 2020 2020 2020 2020 2028 2757  .            ('W
+0001bd20: 6865 6e20 7765 206d 6565 742c 2079 6f75  hen we meet, you
+0001bd30: 2061 7265 2061 2067 6961 6e74 2061 6d6f   are a giant amo
+0001bd40: 6e67 206d 656e 2e27 2c0a 2020 2020 2020  ng men.',.      
+0001bd50: 2020 2020 2020 205b 2761 272c 2027 616d         ['a', 'am
+0001bd60: 6f6e 6727 2c20 2761 7265 272c 2027 6769  ong', 'are', 'gi
+0001bd70: 616e 7427 2c20 276d 616e 272c 2027 6d65  ant', 'man', 'me
+0001bd80: 6574 272c 2027 6d65 6e27 2c20 2777 6527  et', 'men', 'we'
+0001bd90: 2c20 2777 6865 6e27 2c20 2779 6f75 275d  , 'when', 'you']
+0001bda0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+0001bdb0: 2757 6865 6e20 7765 2061 7265 2061 6d6f  'When we are amo
+0001bdc0: 6e67 206d 656e 2c20 796f 7520 6172 6520  ng men, you are 
+0001bdd0: 6120 6769 616e 7420 6d65 6174 6261 6c6c  a giant meatball
+0001bde0: 2e27 2c0a 2020 2020 2020 2020 2020 2020  .',.            
+0001bdf0: 205b 2761 272c 2027 616d 6f6e 6727 2c20   ['a', 'among', 
+0001be00: 2761 7265 272c 2027 6172 6527 2c20 2767  'are', 'are', 'g
+0001be10: 6961 6e74 272c 2027 6d61 6e27 2c20 276d  iant', 'man', 'm
+0001be20: 6561 7462 616c 6c27 2c20 276d 656e 272c  eatball', 'men',
+0001be30: 2027 7765 272c 2027 7768 656e 272c 2027   'we', 'when', '
+0001be40: 796f 7527 5d29 2c0a 2020 2020 2020 2020  you']),.        
+0001be50: 5d3a 0a20 2020 2020 2020 2020 2020 2077  ]:.            w
+0001be60: 6974 6820 7365 6c66 2e73 7562 5465 7374  ith self.subTest
+0001be70: 286c 696e 6529 3a0a 2020 2020 2020 2020  (line):.        
+0001be80: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0001be90: 6572 7445 7175 616c 2865 7870 6563 7465  ertEqual(expecte
+0001bea0: 642c 2073 6f72 7465 6428 6c74 2e54 6162  d, sorted(lt.Tab
+0001beb0: 6c65 2e5f 6e6f 726d 616c 697a 655f 7370  le._normalize_sp
+0001bec0: 6c69 7428 6c69 6e65 2929 290a 0a0a 6966  lit(line)))...if
+0001bed0: 205f 5f6e 616d 655f 5f20 3d3d 2027 5f5f   __name__ == '__
+0001bee0: 6d61 696e 5f5f 273a 0a20 2020 2075 6e69  main__':.    uni
+0001bef0: 7474 6573 742e 6d61 696e 2829 0a         ttest.main().
```

