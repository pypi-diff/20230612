# Comparing `tmp/sqlite_dataset-0.4.0.tar.gz` & `tmp/sqlite_dataset-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite_dataset-0.4.0.tar", max compression
+gzip compressed data, was "sqlite_dataset-0.5.0.tar", max compression
```

## Comparing `sqlite_dataset-0.4.0.tar` & `sqlite_dataset-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1089 2023-06-09 11:39:25.599908 sqlite_dataset-0.4.0/LICENSE
--rw-r--r--   0        0        0      528 2023-06-09 15:07:34.828133 sqlite_dataset-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5374 2023-06-09 15:11:27.339707 sqlite_dataset-0.4.0/README.md
--rw-r--r--   0        0        0       89 2023-06-09 13:45:27.347401 sqlite_dataset-0.4.0/sqlite_dataset/__init__.py
--rw-r--r--   0        0        0     5064 2023-06-09 14:52:12.604865 sqlite_dataset-0.4.0/sqlite_dataset/dataset.py
--rw-r--r--   0        0        0      440 2023-06-09 13:34:22.954170 sqlite_dataset-0.4.0/sqlite_dataset/fields.py
--rw-r--r--   0        0        0     1471 2023-06-09 13:45:56.787610 sqlite_dataset-0.4.0/sqlite_dataset/test.py
--rw-r--r--   0        0        0      308 2023-03-27 09:27:16.270611 sqlite_dataset-0.4.0/sqlite_dataset/utils.py
--rw-r--r--   0        0        0     6048 1970-01-01 00:00:00.000000 sqlite_dataset-0.4.0/setup.py
--rw-r--r--   0        0        0     5937 1970-01-01 00:00:00.000000 sqlite_dataset-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-09 11:39:25.599908 sqlite_dataset-0.5.0/LICENSE
+-rw-r--r--   0        0        0      528 2023-06-12 16:10:55.983467 sqlite_dataset-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5374 2023-06-09 15:11:27.339707 sqlite_dataset-0.5.0/README.md
+-rw-r--r--   0        0        0       89 2023-06-09 13:45:27.347401 sqlite_dataset-0.5.0/sqlite_dataset/__init__.py
+-rw-r--r--   0        0        0     5873 2023-06-12 13:08:36.472992 sqlite_dataset-0.5.0/sqlite_dataset/dataset.py
+-rw-r--r--   0        0        0      702 2023-06-12 12:56:44.150591 sqlite_dataset-0.5.0/sqlite_dataset/fields.py
+-rw-r--r--   0        0        0     1536 2023-06-12 13:15:21.856534 sqlite_dataset-0.5.0/sqlite_dataset/test.py
+-rw-r--r--   0        0        0      308 2023-03-27 09:27:16.270611 sqlite_dataset-0.5.0/sqlite_dataset/utils.py
+-rw-r--r--   0        0        0     6048 1970-01-01 00:00:00.000000 sqlite_dataset-0.5.0/setup.py
+-rw-r--r--   0        0        0     5937 1970-01-01 00:00:00.000000 sqlite_dataset-0.5.0/PKG-INFO
```

### Comparing `sqlite_dataset-0.4.0/LICENSE` & `sqlite_dataset-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite_dataset-0.4.0/pyproject.toml` & `sqlite_dataset-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlite-dataset"
-version = "0.4.0"
+version = "0.5.0"
 description = "Use SQLite database to store datasets."
 authors = ["Jinshuai Ma <mayazureee@gmail.com>"]
 readme = "README.md"
 packages = [{include = "sqlite_dataset"}]
 license = "MIT"
 repository = "https://github.com/Mayazure/sqlite-dataset"
```

### Comparing `sqlite_dataset-0.4.0/README.md` & `sqlite_dataset-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlite_dataset-0.4.0/sqlite_dataset/dataset.py` & `sqlite_dataset-0.5.0/sqlite_dataset/dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 import os
 import warnings
 from collections import OrderedDict
 
 from sqlalchemy import MetaData, Table, insert, Column, select, text
 
-from sqlite_dataset.fields import Field
+from sqlite_dataset.fields import Field, DataTable
 from sqlite_dataset.utils import create_sqlite_db_engine
 
 
 def _get_fields_by_mro(klass):
     mro = inspect.getmro(klass)
     return sum(
         (
@@ -18,40 +18,63 @@
             )
             for base in mro[:0:-1]
         ),
         [],
     )
 
 
-def is_field_class(val):
+def is_class(val, klass):
     try:
-        return issubclass(val, Field)
+        return issubclass(val, klass)
     except TypeError:
-        return isinstance(val, Field)
+        return isinstance(val, klass)
+
+
+def is_field_class(val):
+    return is_class(val, Field)
+
+
+def is_table_class(val):
+    return is_class(val, DataTable)
 
 
 def _get_fields(attrs):
     fields = [
         (field_name, field_value)
         for field_name, field_value in attrs.items()
         if is_field_class(field_value)
     ]
     return fields
 
 
+def _get_table_fields(attrs):
+    table_fields = []
+    for table_name, table_value in attrs.items():
+        if is_table_class(table_value):
+            use_tablename = table_value.tablename or table_name
+            for (field_name, field_value) in table_value.fields:
+                field_value.tablename = use_tablename
+                table_fields.append((field_name, field_value))
+    return table_fields
+
+
 class DatasetMeta(type):
 
     def __new__(mcs, name, bases, attrs):
+        __defaulttable__ = attrs.get('__defaulttable__', 'data')
         cls_fields = _get_fields(attrs)
-        for field_name, _ in cls_fields:
+        table_fields = _get_table_fields(attrs)
+        for field_name, field_col in cls_fields:
+            if field_col.tablename is None:
+                field_col.tablename = __defaulttable__
             del attrs[field_name]
         klass = super().__new__(mcs, name, bases, attrs)
         inherited_fields = _get_fields_by_mro(klass)
         klass._declared_fields = mcs.get_declared_fields(
-            cls_fields=cls_fields,
+            cls_fields=[*cls_fields, *table_fields],
             inherited_fields=inherited_fields,
         )
         return klass
 
     @classmethod
     def get_declared_fields(
             mcs,
```

### Comparing `sqlite_dataset-0.4.0/sqlite_dataset/test.py` & `sqlite_dataset-0.5.0/sqlite_dataset/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import pandas as pd
 
 from sqlite_dataset import SQLiteDataset, Field, String, Float
+from sqlite_dataset.fields import DataTable
 
 
 class MyBaseIrisDataset(SQLiteDataset):
-    text = Field(String, tablename='sentence')
-    sepal_length_cm = Field(String, tablename='iris')
+    __defaulttable__ = 'sentence'
+
+    text = Field(String)
+    iris = DataTable(
+        sepal_length_cm=Field(String, tablename='iris')
+    )
 
 
 class MyIrisDataset(MyBaseIrisDataset):
-    sepal_width_cm = Field(Float, tablename='iris')
-    petal_length_cm = Field(Float, tablename='iris')
-    petal_width_cm = Field(Float, tablename='iris')
-    class_field = Field(String, name='class', tablename='iris')
+    iris = DataTable(
+        sepal_width_cm=Field(Float),
+        petal_length_cm=Field(Float),
+        petal_width_cm=Field(Float),
+        class_field=Field(String, name='class')
+    )
+
 
 data = [
     {
         'sepal_length_cm': '5.1',
         'sepal_width_cm': '3.5',
         'petal_length_cm': '1.4',
         'petal_width_cm': '0.2',
@@ -39,15 +47,15 @@
 with MyIrisDataset('iris11.db') as ds:
     ds.insert_data('iris', data)
 
 with MyIrisDataset('iris.db') as ds:
     res = ds.read_data('iris')
     print(res)
 
-import seaborn as sns
+# import seaborn as sns
 
 # df = sns.load_dataset('iris')
 # with MyIrisDataset('iris11.db') as ds:
 #     df.to_sql('iris', ds.connection)
 #     ds.connection.commit()
 #     # res = pd.read_sql(
 #     #     ds.get_table('iris').select(),
```

### Comparing `sqlite_dataset-0.4.0/setup.py` & `sqlite_dataset-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['sqlalchemy>=1.3.0']
 
 setup_kwargs = {
     'name': 'sqlite-dataset',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': 'Use SQLite database to store datasets.',
     'long_description': "# SQLite Dataset\n\nUse [SQLite](https://sqlite.org/index.html) database to store datasets. Based on [SQLAlchemy core](https://docs.sqlalchemy.org/en/20/core/).\n\n## Structure\n\nThe core of sqlite-dataset is the Class **SQLiteDataset**, which wraps a SQLAlchemy connection to a SQLite database.\n\n## Usage\n\n### Declare a dataset\n\nTo declare a dataset, extend the base **SQLiteDataset** class and specify fields.\n\n```python\nfrom sqlite_dataset import SQLiteDataset, Field, String, Float\n\nclass MyIrisDataset(SQLiteDataset):\n    \n    sepal_length_cm = Field(String, tablename='iris')\n    sepal_width_cm = Field(Float, tablename='iris')\n    petal_length_cm = Field(Float, tablename='iris')\n    petal_width_cm = Field(Float, tablename='iris')\n    class_field = Field(String, tablename='iris', name='class')\n\nds = MyIrisDataset('my_iris_dataset.db')\n```\n\nThis will create a sqlite database file on the specified path. If a dataset already exists, it will then be loaded. \n\n#### The *Field* object\n\n`Field` can be seen as a factory that can create a SQLAlchemy's Column object.\n\nThe `Field` object's constructor takes same arguments as `sqlalchemy.schema.Column` with the difference that `Field` does not take positional name argument and has an extra keyword argument `tablename`.\n\nDeclare a Column using sqlalchemy.Column:\n\n```python\nfrom sqlalchemy import Column, String\n\nColumn('sepal_length_cm', String)\nColumn(name='sepal_length_cm', type_=String)\n```\n\nDeclare a sqlite_dataset.Field:\n\n```python\nfrom sqlite_dataset import Field, String\n\nsepal_length_cm = Field(String)\n```\n\nThe variable name will be automatically used as the column name.\n\nColumn name can also be specified using `name` argument, which is useful if the column name is a Python preserved keyword:\n\n```python\nfrom sqlite_dataset import SQLiteDataset, Field, String\n\nclass MyDataset(SQLiteDataset):\n    class_field = Field(String, name='class')\n    type_field = Field(String, name='type')\n```\n\nTable name can be specified using `tablename` keyword argument:\n\n```python\nfrom sqlite_dataset import SQLiteDataset, Field, String\n\nclass MyDataset(SQLiteDataset):\n    class_field = Field(String, name='class', tablename='table1')\n    type_field = Field(String, name='type', tablename='table2')\n```\n\nThis will create two tables: table1, table2.\n\nIf tablename is not specified, the column will be created in default table **data**. \n\n#### Field type and keyword arguments\n\nThe field type is the sqlalchemy column type. All sqlalchemy members were imported into sqlite_dataset.\n\n```python\nfrom sqlalchemy import String, Integer\n```\n\nis exactly the same as:\n\n```python\nfrom sqlite_dataset import String, Integer\n```\n\n### Inheritance\n\nDataset can be inherited.\n\n```python\nfrom sqlite_dataset import SQLiteDataset, Field, String, Float\n\nclass BaseDataset(SQLiteDataset):\n    class_field = Field(String, tablename='iris', name='class')\n    example_field = Field(String, tablename='example_table')\n\nclass ChildDataset(BaseDataset): \n    sepal_length_cm = Field(String, tablename='iris')\n    sepal_width_cm = Field(Float, tablename='iris')\n    petal_length_cm = Field(Float, tablename='iris')\n    petal_width_cm = Field(Float, tablename='iris')\n```\n\n### Connect to an existing dataset\n\nTo connect to a dataset, call the `connect()` method. Call `close()` to close it.\n\n```python\nds = SQLiteDataset('test.db')\nds.connect()\n# do something\nds.close()\n```\n\nOr the dataset can be used as a context manager\n\n```python\nwith SQLiteDataset('test.db') as ds:\n    # do something\n    pass\n```\n\n### Schema for existing dataset\n\n**SQLiteDataset** object uses SQLAlchemy connection under the hood, so a schema is required to make any database queries or operations.\n\nIf no schema provided by either of the above, a [SQLAlchemy **reflection**](https://docs.sqlalchemy.org/en/13/core/reflection.html) is performed to load and parse schema from the existing database.\n\nIt is recommended to explicitly define the schema as **reflection** may have performance issue in some cases if the schema is very large and complex.\n\n## Add and read data\n\n```python\ndata = [\n    {\n        'sepal_length_cm': '5.1',\n        'sepal_width_cm': '3.5',\n        'petal_length_cm': '1.4',\n        'petal_width_cm': '0.2',\n        'class': 'setosa'\n    },\n    {\n        'sepal_length_cm': '4.9',\n        'sepal_width_cm': '3.0',\n        'petal_length_cm': '1.4',\n        'petal_width_cm': '0.2',\n        'class': 'setosa'\n    }\n]\n\nwith MyIrisDataset('test.db') as ds:\n    ds.insert_data('iris', data)\n```\n\n```python\nwith MyIrisDataset('test.db') as ds:\n    res = ds.read_data('iris')\n```\n\n\n### Use with pandas\n\nA pandas DataFrame can be inserted into a dataset by utilizing the `to_sql()` function, and read from the dataset using `read_sql` function.\n\nBe aware that in this case, `SQLiteDataset()` should be used without specifying the schema.\n\n```python\nimport seaborn as sns\nimport pandas as pd\n\ndf = sns.load_dataset('iris')\nwith SQLiteDataset('iris11.db') as ds:\n    df.to_sql('iris', ds.connection)\n    ds.connection.commit()\n```\n\n```python\nwith SQLiteDataset('iris11.db') as ds:\n    res = pd.read_sql(\n        ds.get_table('iris').select(),\n        ds.connection\n    )\n```",
     'author': 'Jinshuai Ma',
     'author_email': 'mayazureee@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Mayazure/sqlite-dataset',
```

### Comparing `sqlite_dataset-0.4.0/PKG-INFO` & `sqlite_dataset-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-dataset
-Version: 0.4.0
+Version: 0.5.0
 Summary: Use SQLite database to store datasets.
 Home-page: https://github.com/Mayazure/sqlite-dataset
 License: MIT
 Author: Jinshuai Ma
 Author-email: mayazureee@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

