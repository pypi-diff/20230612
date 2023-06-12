# Comparing `tmp/workforce-1.0.6.tar.gz` & `tmp/workforce-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workforce-1.0.6.tar", last modified: Sun Jun 11 23:21:31 2023, max compression
+gzip compressed data, was "workforce-1.0.7.tar", last modified: Mon Jun 12 01:18:21 2023, max compression
```

## Comparing `workforce-1.0.6.tar` & `workforce-1.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:21:31.791297 workforce-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-11 23:21:19.000000 workforce-1.0.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-11 23:21:19.000000 workforce-1.0.6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-11 23:21:19.000000 workforce-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-11 23:21:19.000000 workforce-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-11 23:21:31.791297 workforce-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-11 23:21:19.000000 workforce-1.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:21:31.787297 workforce-1.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4807 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 23:21:31.791297 workforce-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-11 23:21:19.000000 workforce-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:21:31.791297 workforce-1.0.6/workforce/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-11 23:21:19.000000 workforce-1.0.6/workforce/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-06-11 23:21:19.000000 workforce-1.0.6/workforce/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4958 2023-06-11 23:21:19.000000 workforce-1.0.6/workforce/gui.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-11 23:21:19.000000 workforce-1.0.6/workforce/workforce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:21:31.791297 workforce-1.0.6/workforce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-11 23:21:31.000000 workforce-1.0.6/workforce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-11 23:21:31.000000 workforce-1.0.6/workforce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:21:31.000000 workforce-1.0.6/workforce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-11 23:21:31.000000 workforce-1.0.6/workforce.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-11 23:21:31.000000 workforce-1.0.6/workforce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 23:21:31.000000 workforce-1.0.6/workforce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:18:21.110607 workforce-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-12 01:18:10.000000 workforce-1.0.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-12 01:18:10.000000 workforce-1.0.7/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-12 01:18:10.000000 workforce-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-12 01:18:10.000000 workforce-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-12 01:18:21.110607 workforce-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-12 01:18:10.000000 workforce-1.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:18:21.110607 workforce-1.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-12 01:18:10.000000 workforce-1.0.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 01:18:10.000000 workforce-1.0.7/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4807 2023-06-12 01:18:10.000000 workforce-1.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 01:18:10.000000 workforce-1.0.7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 01:18:10.000000 workforce-1.0.7/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-12 01:18:10.000000 workforce-1.0.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-12 01:18:10.000000 workforce-1.0.7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-12 01:18:10.000000 workforce-1.0.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 01:18:10.000000 workforce-1.0.7/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-12 01:18:10.000000 workforce-1.0.7/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 01:18:21.110607 workforce-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-12 01:18:10.000000 workforce-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:18:21.110607 workforce-1.0.7/workforce/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-12 01:18:10.000000 workforce-1.0.7/workforce/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-06-12 01:18:10.000000 workforce-1.0.7/workforce/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4933 2023-06-12 01:18:10.000000 workforce-1.0.7/workforce/gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-12 01:18:10.000000 workforce-1.0.7/workforce/workforce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:18:21.110607 workforce-1.0.7/workforce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-12 01:18:21.000000 workforce-1.0.7/workforce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-12 01:18:21.000000 workforce-1.0.7/workforce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 01:18:21.000000 workforce-1.0.7/workforce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 01:18:21.000000 workforce-1.0.7/workforce.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-12 01:18:21.000000 workforce-1.0.7/workforce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 01:18:21.000000 workforce-1.0.7/workforce.egg-info/top_level.txt
```

### Comparing `workforce-1.0.6/LICENSE` & `workforce-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `workforce-1.0.6/PKG-INFO` & `workforce-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workforce
-Version: 1.0.6
+Version: 1.0.7
 Summary: Run bash commands with python multiprocessing according to a csv file edgelist.
 Home-page: https://github.com/theoportlock/workforce
 Author: Theo Portlock
 Author-email: zn.tportlock@gmail.com
 License: MIT license
 Keywords: workforce
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `workforce-1.0.6/README.rst` & `workforce-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `workforce-1.0.6/docs/Makefile` & `workforce-1.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `workforce-1.0.6/docs/conf.py` & `workforce-1.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `workforce-1.0.6/docs/installation.rst` & `workforce-1.0.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `workforce-1.0.6/docs/make.bat` & `workforce-1.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `workforce-1.0.6/setup.py` & `workforce-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,9 +36,9 @@
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     keywords='workforce',
     name='workforce',
     packages = ["workforce"],
     url='https://github.com/theoportlock/workforce',
-    version='1.0.6',
+    version='1.0.7',
 )
```

### Comparing `workforce-1.0.6/workforce/gui.py` & `workforce-1.0.7/workforce/gui.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,55 +55,53 @@
                   Input('txt_to', 'value'),
                   State('upload-data', 'filename'),
                   State('upload-data', 'last_modified'),
                   State('cytoscape-elements', 'elements'),
                   prevent_initial_call=True)
     def load_data(contents, n_clicks, txt_from, txt_to, filename, last_modified, elements):
         # For data load
-        print(contents, n_clicks, txt_from, txt_to, filename, last_modified)
         if ctx.triggered_id == 'upload-data':
+            elements, edges, nodes =[], [], []
             edges = parse_contents(contents, filename)
             nodes = np.concatenate([edges.source.unique(), edges.target.unique()])
             nodes = [{'data': {'id': name, 'label': name}} for name in nodes]
             edges = [
                 {'data': {'source': source, 'target': target}}
                 for source, target in edges[['source','target']].values
             ]
             elements = edges+nodes
         # For adding data
         elif ctx.triggered_id == 'btn-add':
             edges = elements_to_edges(elements) if elements else pd.DataFrame()
             edges = pd.concat([edges, pd.DataFrame([txt_from,txt_to], index=['source','target']).T], axis=0, ignore_index=True).drop_duplicates()
             elements = edges_to_elements(edges)
-            print(elements)
         return elements
 
     # Save data
     @app.callback(Output('download-data', 'data'),
                   Input('btn-download', 'n_clicks'),
                   State('cytoscape-elements', 'elements'),
                   prevent_initial_call=True)
     def save_data(n_clicks, elements):
         ele = pd.concat([pd.DataFrame.from_dict(i) for i in elements], axis=1).T.set_index('id')
         edges = ele.drop('label', axis=1).dropna().set_index('source')
-        return dcc.send_data_frame(edges.to_csv, 'mydf.csv')
+        return dcc.send_data_frame(edges.to_csv, 'mydf.csv', header=False)
 
     # Other functions
     def parse_contents(contents, filename):
         import base64
         import io
         content_type, content_string = contents.split(',')
         decoded = base64.b64decode(content_string)
         try:
             if 'csv' in filename:
-                df = pd.read_csv(io.StringIO(decoded.decode('utf-8')))
+                df = pd.read_csv(io.StringIO(decoded.decode('utf-8')), header=None, names=['source','target'])
             elif 'xls' in filename:
                 df = pd.read_excel(io.BytesIO(decoded))
         except Exception as e:
-            print(e)
             return html.Div([
                 'There was an error processing this file.'
             ])
         return df
 
     def elements_to_edges(elements):
         ele = pd.concat([pd.DataFrame.from_dict(i) for i in elements], axis=1).T.set_index('id')
```

### Comparing `workforce-1.0.6/workforce/workforce.py` & `workforce-1.0.7/workforce/workforce.py`

 * *Files identical despite different names*

### Comparing `workforce-1.0.6/workforce.egg-info/PKG-INFO` & `workforce-1.0.7/workforce.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workforce
-Version: 1.0.6
+Version: 1.0.7
 Summary: Run bash commands with python multiprocessing according to a csv file edgelist.
 Home-page: https://github.com/theoportlock/workforce
 Author: Theo Portlock
 Author-email: zn.tportlock@gmail.com
 License: MIT license
 Keywords: workforce
 Classifier: Development Status :: 2 - Pre-Alpha
```

