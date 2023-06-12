# Comparing `tmp/pocketsearch-0.7.0.tar.gz` & `tmp/pocketsearch-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketsearch-0.7.0.tar", last modified: Sat Jun 10 19:33:07 2023, max compression
+gzip compressed data, was "pocketsearch-0.7.1.tar", last modified: Mon Jun 12 14:26:23 2023, max compression
```

## Comparing `pocketsearch-0.7.0.tar` & `pocketsearch-0.7.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:33:07.813548 pocketsearch-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-10 19:32:57.000000 pocketsearch-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-10 19:33:07.809548 pocketsearch-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12019 2023-06-10 19:32:57.000000 pocketsearch-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 19:33:07.813548 pocketsearch-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-10 19:32:57.000000 pocketsearch-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:33:07.805548 pocketsearch-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:33:07.809548 pocketsearch-0.7.0/src/pocketsearch/
--rw-r--r--   0 runner    (1001) docker     (123)    41876 2023-06-10 19:32:57.000000 pocketsearch-0.7.0/src/pocketsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20355 2023-06-10 19:32:57.000000 pocketsearch-0.7.0/src/pocketsearch/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:33:07.809548 pocketsearch-0.7.0/src/pocketsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-10 19:33:07.000000 pocketsearch-0.7.0/src/pocketsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-10 19:33:07.000000 pocketsearch-0.7.0/src/pocketsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 19:33:07.000000 pocketsearch-0.7.0/src/pocketsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-10 19:33:07.000000 pocketsearch-0.7.0/src/pocketsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:26:23.198541 pocketsearch-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-12 14:26:14.000000 pocketsearch-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-06-12 14:26:23.194541 pocketsearch-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-06-12 14:26:14.000000 pocketsearch-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:26:23.198541 pocketsearch-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-12 14:26:14.000000 pocketsearch-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:26:23.194541 pocketsearch-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:26:23.194541 pocketsearch-0.7.1/src/pocketsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)    42408 2023-06-12 14:26:14.000000 pocketsearch-0.7.1/src/pocketsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21934 2023-06-12 14:26:14.000000 pocketsearch-0.7.1/src/pocketsearch/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:26:23.194541 pocketsearch-0.7.1/src/pocketsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-06-12 14:26:23.000000 pocketsearch-0.7.1/src/pocketsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-12 14:26:23.000000 pocketsearch-0.7.1/src/pocketsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:26:23.000000 pocketsearch-0.7.1/src/pocketsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 14:26:23.000000 pocketsearch-0.7.1/src/pocketsearch.egg-info/top_level.txt
```

### Comparing `pocketsearch-0.7.0/LICENSE` & `pocketsearch-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pocketsearch-0.7.0/PKG-INFO` & `pocketsearch-0.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.7.0
+Version: 0.7.1
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Project-URL: Change log, https://github.com/kaykay-dv/pocketsearch/blob/main/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
@@ -65,26 +65,32 @@
 print(pocket_search.search(text="hello")[0].text)
 Hello World !
 ```
 
 From a database perspective, the new document will be immediately available 
 to the search index, as each insert is followed by a database commit.
 
-Be ware that the search methods limits results to 10 by default. Results 
+Be aware that the search methods limits results to 10 by default. Results 
 are ordered by the rank of the search result which is calculated by the 
-FTS extension in sqlite and showing how relevant a document is to a 
-given query. 
+FTS extension in sqlite (see https://www.sqlite.org/fts5.html#the_bm25_function for more details) 
+showing how relevant a document is to a given query. 
 
 The API also supports iteration:
 
 ```Python
 for document in pocket_search.search(text="hello"):
     print(document.text)
 ```
 
+There is also supported for slicing:
+
+```Python
+pocket_search.search(text="hello")[1:3]
+```
+
 ## AND/OR queries
 
 The FTS5 engines supports AND/OR queries. By 
 default they are disabled in the API, if you want to make boolean 
 queries, you have to use a lookup parameter in your query: 
 
 ```Python
@@ -305,14 +311,22 @@
 pocket_search.search(price__lte=3)
 # Matches products with price greater than equal 3
 pocket_search.search(price__gte=3)
 # Matches products with price greater than equal 3 AND where the description contains "apple".
 pocket_search.search(price__gte=3,description="apple")
 ```
 
+You can also provide an index for numeric data by setting ...
+
+```Python
+price = Int(index=True)
+```
+
+... to speed up queries.
+
 ## Searching date fields
 
 pocketsearch also provides some (experimental) support for searching dates:
 
 ```Python
 class AllFields(Schema):
 
@@ -341,15 +355,15 @@
 pocket_search = PocketSearch(db_name="my_db.db",writeable=True)
 # now, all operations will be done on the my_db database that is stored in the 
 # current working directory.
 ```
 
 When working with search indices that are stored on disk, *it is important to 
 provide the writeable argument*, as any PocketSearch instance that works 
-with file sqlite databases, is in read-only mode be default (unlike their 
+with file sqlite databases, is in read-only mode by default (unlike their 
 in-memory counterpart.). 
 
 # Behind the scenes: how searching works
 
 pocketsearch uses the FTS5 extension of sqlite. More information can be found here:
 https://www.sqlite.org/fts5.html
```

### Comparing `pocketsearch-0.7.0/README.md` & `pocketsearch-0.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,26 +41,32 @@
 print(pocket_search.search(text="hello")[0].text)
 Hello World !
 ```
 
 From a database perspective, the new document will be immediately available 
 to the search index, as each insert is followed by a database commit.
 
-Be ware that the search methods limits results to 10 by default. Results 
+Be aware that the search methods limits results to 10 by default. Results 
 are ordered by the rank of the search result which is calculated by the 
-FTS extension in sqlite and showing how relevant a document is to a 
-given query. 
+FTS extension in sqlite (see https://www.sqlite.org/fts5.html#the_bm25_function for more details) 
+showing how relevant a document is to a given query. 
 
 The API also supports iteration:
 
 ```Python
 for document in pocket_search.search(text="hello"):
     print(document.text)
 ```
 
+There is also supported for slicing:
+
+```Python
+pocket_search.search(text="hello")[1:3]
+```
+
 ## AND/OR queries
 
 The FTS5 engines supports AND/OR queries. By 
 default they are disabled in the API, if you want to make boolean 
 queries, you have to use a lookup parameter in your query: 
 
 ```Python
@@ -281,14 +287,22 @@
 pocket_search.search(price__lte=3)
 # Matches products with price greater than equal 3
 pocket_search.search(price__gte=3)
 # Matches products with price greater than equal 3 AND where the description contains "apple".
 pocket_search.search(price__gte=3,description="apple")
 ```
 
+You can also provide an index for numeric data by setting ...
+
+```Python
+price = Int(index=True)
+```
+
+... to speed up queries.
+
 ## Searching date fields
 
 pocketsearch also provides some (experimental) support for searching dates:
 
 ```Python
 class AllFields(Schema):
 
@@ -317,15 +331,15 @@
 pocket_search = PocketSearch(db_name="my_db.db",writeable=True)
 # now, all operations will be done on the my_db database that is stored in the 
 # current working directory.
 ```
 
 When working with search indices that are stored on disk, *it is important to 
 provide the writeable argument*, as any PocketSearch instance that works 
-with file sqlite databases, is in read-only mode be default (unlike their 
+with file sqlite databases, is in read-only mode by default (unlike their 
 in-memory counterpart.). 
 
 # Behind the scenes: how searching works
 
 pocketsearch uses the FTS5 extension of sqlite. More information can be found here:
 https://www.sqlite.org/fts5.html
```

### Comparing `pocketsearch-0.7.0/setup.py` & `pocketsearch-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "pocketsearch",
-    version = "0.7.0",
+    version = "0.7.1",
     author = "kaykay-dv",
     author_email = "kaykay2306@gmail.com",
     description = "A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/kaykay-dv/pocketsearch/",
     project_urls = {
```

### Comparing `pocketsearch-0.7.0/src/pocketsearch/__init__.py` & `pocketsearch-0.7.1/src/pocketsearch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE FOR ANY DAMAGES OR OTHER LIABILITY,
 WHETHER IN CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR
 THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 '''
 
-import pdb;
-import logging
 import sqlite3
 import os
 import time
 import abc
+import copy
 
 
 class Timer:
     '''
     A helper class that displays
     a progress bar in console.
     '''
@@ -105,26 +104,24 @@
         '''
         Return the full qualified name including its table for the given field.
         '''
         if self.index:
             if self.fts_enabled():
                 return "%s_fts.%s" % (self.schema.name, self.name)
             else:
-                return "%s_.%s" % (self.schema.name, self.name)
+                return "%s.%s" % (self.schema.name, self.name)
         else:
             return "%s.%s" % (self.schema.name, self.name)
 
     def to_sql(self, index_table=False):
         '''
         Returns sql representation of field for SQL table generation.
         '''
-        try:
-            self.data_type
-        except AttributeError as exc:
-            raise AttributeError("class %s (field=%s) has not attribute data_type" % (self.__class__.__name__, self.name)) from exc
+        if self.data_type is None:
+            raise self.schema.SchemaError("class %s (field=%s) has no data_type set" % (self.__class__.__name__, self.name))
         name = self.schema.reverse_lookup[self]
         if index_table:
             _data_type = ""
         else:
             _data_type = self.data_type
         return "%s %s %s" % (name, _data_type, self.constraints())
 
@@ -680,14 +677,15 @@
         Adds an order_by clause to the current statement. sort_dir can either be "+" (ascending)
         or "-" (descending)
         '''
         if clear:
             self.v_order_by.clear()
         self.v_order_by.append(OrderBy(field=field, sort_dir=sort_dir, sql_query=self))
 
+
     def limit_and_offset(self, limit, offset):
         '''
         Set limit and offset of query
         '''
         self.v_limit_and_offset = LimitAndOffset(limit=limit, offset=offset, sql_query=self)
 
     def add_value(self, value):
@@ -744,17 +742,24 @@
                 self.sql_query.where(field=argument.field, lookup=lookup)
         self.sql_query.select("rank")
         self.sql_query.table(table_name=self.search_instance.schema.name)
         self.sql_query.table(table_name="%s_fts" % self.search_instance.schema.name)
         self.sql_query.join(self.sql_query.v_from_tables[0], self.sql_query.v_from_tables[1], "id", "rowid")
         self.sql_query.order_by("+rank")
         self.sql_query.limit_and_offset(limit=10, offset=0)
-        self._defaults_set = True
+        #self._defaults_set = True
+        self._default_order_by_set = True
+        self._default_values_set = True
         self.is_aggregate_query = False
 
+    def _defaults_set(self):
+        # Returns true if any default parameters set for .values and .order_by
+        # clauses have been changed
+        return self._default_order_by_set & self._default_values_set
+
     def count(self):
         '''
         Sets the query object into count mode.
         '''
         self.is_aggregate_query = True
         self.sql_query.count()
         for query in self.unions:
@@ -762,31 +767,33 @@
         return self._query()
 
     def order_by(self, *args):
         '''
         Add order by clauses. To indicate ascending or descending order,
         arguments should start with either "+" or ".".
         '''
-        self._defaults_set = False
         for a in args:
             if a.startswith("+") or a.startswith("-"):
                 field = self.search_instance.schema.get_field(a[1:], raise_exception=True)
                 sort_dir = a[0]
             else:
                 field = self.search_instance.schema.get_field(a, raise_exception=True)
                 sort_dir = "+"
-            self.sql_query.order_by(field, sort_dir, clear=True)
+            # If the _defaults_set parameter is True, only the default sort order 
+            # in the constructor has been yet. In that case we clear the order by 
+            # list and set the new order by clause.
+            self.sql_query.order_by(field, sort_dir, clear=self._default_order_by_set)
+            self._default_order_by_set = False
         return self
 
     def _adapt_union_queries(self):
         '''
         Re-organizes the structure of the order by
         and limit clauses.
         '''
-        import copy
         if len(self.unions) > 0:
             # Copy order by clause and limit / offsets to the last query in the union
             last_query = self.unions[len(self.unions)-1]
             if not(self.is_aggregate_query):
                 last_query.sql_query.v_order_by = copy.copy(self.sql_query.v_order_by)
                 last_query.sql_query.v_limit_and_offset = copy.copy(self.sql_query.v_limit_and_offset)
             else:
@@ -797,27 +804,28 @@
             obj.sql_query.v_limit_and_offset = None
         self.sql_query.v_order_by.clear()
         self.sql_query.v_limit_and_offset = None
 
     def __or__(self, obj):
         if not(isinstance(obj, Query)):
             raise self.QueryError("Only instances of class Query can be used with the OR operator.")
-        if not(obj._defaults_set) or not(self._defaults_set):
+        if not(obj._defaults_set()) or not(self._defaults_set()):
             raise self.QueryError("You cannot use .values and .order_by methods in the context of a union.")
         self.unions.append(obj)
         return self
 
     def values(self, *args):
         '''
         Set the values you want to have in the search result list.
         '''
-        self._defaults_set = False
+        self._default_values_set = False
         for a in args:
             field = self.search_instance.schema.get_field(a, raise_exception=True)
-            self.sql_query.select(field)
+            self.sql_query.select(field,clear=self._default_values_set)
+            self._default_values_set = False
         return self
 
     def _build_results(self, results):
         documents = SearchResult()
         for result in results:
             document = Document(result.keys())
             for field in result.keys():
@@ -829,15 +837,14 @@
         if len(self.unions) > 0:
             self._adapt_union_queries()
         stmt, query_args = self.sql_query.to_sql()
         for query in self.unions:
             u_stmt, u_ar = query.sql_query.to_sql()
             stmt += " UNION ALL " + u_stmt
             query_args = query_args + u_ar
-        logging.debug(stmt)
         if self.is_aggregate_query:
             count = 0
             for sub_count in self.search_instance.execute_sql(stmt, *query_args):
                 count = count+sub_count["COUNT(*)"]
             return count
         return self._build_results(self.search_instance.execute_sql(stmt, *query_args))
 
@@ -1012,15 +1019,15 @@
         self.cursor.execute(sql_table)
         self.cursor.execute(sql_virtual_table)
         self.cursor.execute(self._format_sql(index_name, fields, sql_trigger_insert))
         self.cursor.execute(self._format_sql(index_name, fields, sql_trigger_delete))
         self.cursor.execute(self._format_sql(index_name, fields, sql_trigger_update))
         # create standard indices
         for field in default_index_fields:
-            self.cursor.execute("CREATE INDEX idx_std_{index_name}_%s ON {index_name} ({field});".format(index_name=index_name, field=field))
+            self.cursor.execute("CREATE INDEX idx_std_{index_name}_{field} ON {index_name} ({field});".format(index_name=index_name, field=field.name))
 
     def get_arguments(self, kwargs, for_search=True):
         '''
         Extracts field names and lookups from the keywords arguments and returns
         a dictionary of argument objects.
         '''
         referenced_fields = {}
```

### Comparing `pocketsearch-0.7.0/src/pocketsearch/tests.py` & `pocketsearch-0.7.1/src/pocketsearch/tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,19 @@
     '''
     A simple movie schema we use for tests.
     '''
 
     title = Text(index=True)
     text = Text(index=True)
 
+class CustomField(Field): 
+    '''
+    Field with no data type provided
+    '''
+    pass
 
 class Page(Schema):
     '''
     Page schema to use multi-field searches
     '''
 
     title = Text(index=True)
@@ -36,33 +41,55 @@
 class BrokenSchemaUnderscores(Schema):
     '''
     Broken schema definition - Underscores are not allowed
     '''
 
     test__123 = Field()
 
+class SchemaCustomField(Schema):
+    '''
+    Schema using a custom field with no data type
+    '''
+
+    custom_field = CustomField()
 
 class SchemaTest(unittest.TestCase):
     '''
     Tests for schema generation
     '''
 
     def test_create_schema(self):
+        '''
+        Schema creation test
+        '''
         schema = Movie(name="movie")
         for field in ["title", "text"]:
             self.assertEqual(field in schema.fields, True)
 
     def test_use_underscores_in_fields(self):
+        '''
+        Schema creation test with field containing underscores
+        '''
         with self.assertRaises(Schema.SchemaError):
-            BrokenSchemaUnderscores(name="broken")
+            schema = BrokenSchemaUnderscores(name="broken")
 
     def test_use_reserved_keywords(self):
+        '''
+        Schema creation test with field containing keywords
+        '''                
         with self.assertRaises(Schema.SchemaError):
             BrokenSchema(name="broken")
 
+    def test_field_no_data_type(self):
+        '''
+        Schema creation test with field having no data type
+        '''                        
+        schema = SchemaCustomField(name="broken")
+        with self.assertRaises(Schema.SchemaError):
+            schema.custom_field.to_sql()
 
 class BaseTest(unittest.TestCase):
     '''
     Base test class that creates some test data
     '''
 
     def setUp(self):
@@ -77,14 +104,18 @@
 
 
 class OperatorSearch(BaseTest):
     '''
     Tests covering the usage of boolean operators and prefix search
     '''
 
+    def test_search_len_func(self):
+        # test application of len function to search result
+        self.assertEqual(len(self.pocket_search.search(text="france")[0:1]), 1)
+
     def test_search_prefix(self):
         # by default, prefix search is not supported:
         self.assertEqual(self.pocket_search.search(text="fran*").count(), 0)
 
     def test_search_prefix_explicit(self):
         # by default, prefix search is not supported:
         self.assertEqual(self.pocket_search.search(text__allow_prefix="fran*").count(), 1)
@@ -198,33 +229,48 @@
         results = self.pocket_search.search(text="is")[0:2]
         results[0]
 
     def test_iteration(self):
         for idx, item in enumerate(self.pocket_search.search(text="is")):
             item.text  # just check, if it possible to call the attribute
 
-    def test_combine_search_results_illegal_calls(self):
+    def test_combine_search_results_1(self):
         '''
         These are all invalid queries. When we perform
         a union order by or value arguments cannot be
-        provided.
+        provided. UC: order_by in second query
         '''
         with self.assertRaises(Query.QueryError):
-            q1 = self.pocket_search.search(text="paris") | self.pocket_search.search(text="england").order_by("rank")
+            q = self.pocket_search.search(text="paris") | self.pocket_search.search(text="england").order_by("rank")
+
+    def test_combine_search_results_2(self):
+        '''
+        These are all invalid queries. When we perform
+        a union order by or value arguments cannot be
+        provided. UC: order_by in first query
+        '''
         with self.assertRaises(Query.QueryError):
-            q1 = self.pocket_search.search(text="paris").order_by("rank") | self.pocket_search.search(text="england")
+            q = self.pocket_search.search(text="paris").order_by("rank") | self.pocket_search.search(text="england")
+
+    def test_combine_search_results_3(self):
+        '''
+        These are all invalid queries. When we perform
+        a union order by or value arguments cannot be
+        provided.  UC: values in both queries
+        '''        
         with self.assertRaises(Query.QueryError):
-            self.pocket_search.search(text="paris").values("id") | self.pocket_search.search(text="paris").values("id")
+            q = self.pocket_search.search(text="paris").values("id") | self.pocket_search.search(text="paris").values("id")
 
     def test_combine_search_results(self):
         # This is a correct query:
         q1 = self.pocket_search.search(text="paris") | self.pocket_search.search(text="england")
         self.assertEqual(q1.count(), 2)
 
-    def test_order_by(self):
+    def test_order_by_override_default_order_by(self):
+        # This should override the default rank sorting by the text sorting
         r = self.pocket_search.search(text="is").values("id", "rank", "text").order_by("-text")
         self.assertEqual(r[0].text, self.data[0])
         self.assertEqual(r[1].text, self.data[2])
         self.assertEqual(r[2].text, self.data[1])
 
 
 class IDFieldTest(unittest.TestCase):
@@ -409,15 +455,15 @@
         self.assertEqual(self.pocket_search.search(text="Blade", title="runner").count(), 1)
 
 
 class FieldTypeTests(unittest.TestCase):
 
     class AllFields(Schema):
 
-        f1 = Int()
+        f1 = Int(index=True) # implicitly tests if non-fts index generation work
         f2 = Text(index=True)
         f3 = Blob()
         f4 = Real()
         f5 = Datetime()
         f6 = Date()
 
     def setUp(self):
```

### Comparing `pocketsearch-0.7.0/src/pocketsearch.egg-info/PKG-INFO` & `pocketsearch-0.7.1/src/pocketsearch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketsearch
-Version: 0.7.0
+Version: 0.7.1
 Summary: A pure-Python full text indexing search engine based on sqlite and the FTS5 extension.
 Home-page: https://github.com/kaykay-dv/pocketsearch/
 Author: kaykay-dv
 Author-email: kaykay2306@gmail.com
 Project-URL: Bug Tracker, https://github.com/kaykay-dv/pocketsearch/issues
 Project-URL: Change log, https://github.com/kaykay-dv/pocketsearch/blob/main/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
@@ -65,26 +65,32 @@
 print(pocket_search.search(text="hello")[0].text)
 Hello World !
 ```
 
 From a database perspective, the new document will be immediately available 
 to the search index, as each insert is followed by a database commit.
 
-Be ware that the search methods limits results to 10 by default. Results 
+Be aware that the search methods limits results to 10 by default. Results 
 are ordered by the rank of the search result which is calculated by the 
-FTS extension in sqlite and showing how relevant a document is to a 
-given query. 
+FTS extension in sqlite (see https://www.sqlite.org/fts5.html#the_bm25_function for more details) 
+showing how relevant a document is to a given query. 
 
 The API also supports iteration:
 
 ```Python
 for document in pocket_search.search(text="hello"):
     print(document.text)
 ```
 
+There is also supported for slicing:
+
+```Python
+pocket_search.search(text="hello")[1:3]
+```
+
 ## AND/OR queries
 
 The FTS5 engines supports AND/OR queries. By 
 default they are disabled in the API, if you want to make boolean 
 queries, you have to use a lookup parameter in your query: 
 
 ```Python
@@ -305,14 +311,22 @@
 pocket_search.search(price__lte=3)
 # Matches products with price greater than equal 3
 pocket_search.search(price__gte=3)
 # Matches products with price greater than equal 3 AND where the description contains "apple".
 pocket_search.search(price__gte=3,description="apple")
 ```
 
+You can also provide an index for numeric data by setting ...
+
+```Python
+price = Int(index=True)
+```
+
+... to speed up queries.
+
 ## Searching date fields
 
 pocketsearch also provides some (experimental) support for searching dates:
 
 ```Python
 class AllFields(Schema):
 
@@ -341,15 +355,15 @@
 pocket_search = PocketSearch(db_name="my_db.db",writeable=True)
 # now, all operations will be done on the my_db database that is stored in the 
 # current working directory.
 ```
 
 When working with search indices that are stored on disk, *it is important to 
 provide the writeable argument*, as any PocketSearch instance that works 
-with file sqlite databases, is in read-only mode be default (unlike their 
+with file sqlite databases, is in read-only mode by default (unlike their 
 in-memory counterpart.). 
 
 # Behind the scenes: how searching works
 
 pocketsearch uses the FTS5 extension of sqlite. More information can be found here:
 https://www.sqlite.org/fts5.html
```

