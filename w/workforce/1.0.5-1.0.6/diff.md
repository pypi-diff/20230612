# Comparing `tmp/workforce-1.0.5.tar.gz` & `tmp/workforce-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workforce-1.0.5.tar", last modified: Sun Jun 11 22:41:56 2023, max compression
+gzip compressed data, was "workforce-1.0.6.tar", last modified: Sun Jun 11 23:21:31 2023, max compression
```

## Comparing `workforce-1.0.5.tar` & `workforce-1.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:41:56.091722 workforce-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-11 22:41:44.000000 workforce-1.0.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-11 22:41:44.000000 workforce-1.0.5/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-11 22:41:44.000000 workforce-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-11 22:41:44.000000 workforce-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-11 22:41:56.091722 workforce-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-11 22:41:44.000000 workforce-1.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:41:56.091722 workforce-1.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4807 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 22:41:56.091722 workforce-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-11 22:41:44.000000 workforce-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:41:56.091722 workforce-1.0.5/workforce/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-11 22:41:44.000000 workforce-1.0.5/workforce/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-06-11 22:41:44.000000 workforce-1.0.5/workforce/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4316 2023-06-11 22:41:44.000000 workforce-1.0.5/workforce/gui.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-11 22:41:44.000000 workforce-1.0.5/workforce/workforce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:41:56.091722 workforce-1.0.5/workforce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-11 22:41:56.000000 workforce-1.0.5/workforce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-11 22:41:56.000000 workforce-1.0.5/workforce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 22:41:56.000000 workforce-1.0.5/workforce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-11 22:41:56.000000 workforce-1.0.5/workforce.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-11 22:41:56.000000 workforce-1.0.5/workforce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 22:41:56.000000 workforce-1.0.5/workforce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:21:31.791297 workforce-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-11 23:21:19.000000 workforce-1.0.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-11 23:21:19.000000 workforce-1.0.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-11 23:21:19.000000 workforce-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-11 23:21:19.000000 workforce-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-11 23:21:31.791297 workforce-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-11 23:21:19.000000 workforce-1.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:21:31.787297 workforce-1.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4807 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-11 23:21:19.000000 workforce-1.0.6/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 23:21:31.791297 workforce-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-11 23:21:19.000000 workforce-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:21:31.791297 workforce-1.0.6/workforce/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-11 23:21:19.000000 workforce-1.0.6/workforce/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-06-11 23:21:19.000000 workforce-1.0.6/workforce/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4958 2023-06-11 23:21:19.000000 workforce-1.0.6/workforce/gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-11 23:21:19.000000 workforce-1.0.6/workforce/workforce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:21:31.791297 workforce-1.0.6/workforce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-11 23:21:31.000000 workforce-1.0.6/workforce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-11 23:21:31.000000 workforce-1.0.6/workforce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:21:31.000000 workforce-1.0.6/workforce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-11 23:21:31.000000 workforce-1.0.6/workforce.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-11 23:21:31.000000 workforce-1.0.6/workforce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 23:21:31.000000 workforce-1.0.6/workforce.egg-info/top_level.txt
```

### Comparing `workforce-1.0.5/LICENSE` & `workforce-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `workforce-1.0.5/PKG-INFO` & `workforce-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workforce
-Version: 1.0.5
+Version: 1.0.6
 Summary: Run bash commands with python multiprocessing according to a csv file edgelist.
 Home-page: https://github.com/theoportlock/workforce
 Author: Theo Portlock
 Author-email: zn.tportlock@gmail.com
 License: MIT license
 Keywords: workforce
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -46,51 +46,45 @@
 ------------
 Installation can be done with 
 
 .. code-block:: bash
 
    pip install workforce
 
-Running workforce
------------------
-To try a sample plan, run with:
+Building a workforce workflow
+-----------------------------
+To build a workflow, simply run:
 
 .. code-block:: bash
 
-   workforce example_plan.csv
+   workforce
 
-To view the program graph, networkx and matplotlib are required. The -g flag is required to produce a dot file of the network:
+Then, paste the IP address into into your browsers address bar and build your program.
+
+Running workforce
+-----------------
+To run a sample plan from workforce github project:
 
 .. code-block:: bash
 
-   workforce -g example_plan.csv
+   workforce example_plan.csv
 
 To import and use in a python shell, use the following command:
 
 .. code-block:: python
 
    from workforce.workforce import worker
    steve = worker("<PLAN.CSV>")
    steve.run()
 
-Graph print
------------
-Converting the graph to a dot can be done using an online dot viewer or using Graphviz software with the example command:
-
-.. code-block:: bash
-
-   dot -Tpng -Kdot -o <DOT_FILENAME>.png <DOT_FILENAME>
-
-.. image:: example_plan.png
-
 The schema should be in the format of a csv with two columns. On the left and right column is the source and target command respectively (see example). Produces a logfile for each run.
 
 Testing
 -------
-Testing can be done within this directory by running:
+Testing can be done within the github directory by running:
 
 .. code-block:: bash
 
    python -m unittest -v
 
 
 =======
```

### Comparing `workforce-1.0.5/README.rst` & `workforce-1.0.6/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -24,48 +24,42 @@
 ------------
 Installation can be done with 
 
 .. code-block:: bash
 
    pip install workforce
 
-Running workforce
------------------
-To try a sample plan, run with:
+Building a workforce workflow
+-----------------------------
+To build a workflow, simply run:
 
 .. code-block:: bash
 
-   workforce example_plan.csv
+   workforce
 
-To view the program graph, networkx and matplotlib are required. The -g flag is required to produce a dot file of the network:
+Then, paste the IP address into into your browsers address bar and build your program.
+
+Running workforce
+-----------------
+To run a sample plan from workforce github project:
 
 .. code-block:: bash
 
-   workforce -g example_plan.csv
+   workforce example_plan.csv
 
 To import and use in a python shell, use the following command:
 
 .. code-block:: python
 
    from workforce.workforce import worker
    steve = worker("<PLAN.CSV>")
    steve.run()
 
-Graph print
------------
-Converting the graph to a dot can be done using an online dot viewer or using Graphviz software with the example command:
-
-.. code-block:: bash
-
-   dot -Tpng -Kdot -o <DOT_FILENAME>.png <DOT_FILENAME>
-
-.. image:: example_plan.png
-
 The schema should be in the format of a csv with two columns. On the left and right column is the source and target command respectively (see example). Produces a logfile for each run.
 
 Testing
 -------
-Testing can be done within this directory by running:
+Testing can be done within the github directory by running:
 
 .. code-block:: bash
 
    python -m unittest -v
```

### Comparing `workforce-1.0.5/docs/Makefile` & `workforce-1.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `workforce-1.0.5/docs/conf.py` & `workforce-1.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `workforce-1.0.5/docs/installation.rst` & `workforce-1.0.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `workforce-1.0.5/docs/make.bat` & `workforce-1.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `workforce-1.0.5/setup.py` & `workforce-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,9 +36,9 @@
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     keywords='workforce',
     name='workforce',
     packages = ["workforce"],
     url='https://github.com/theoportlock/workforce',
-    version='1.0.5',
+    version='1.0.6',
 )
```

### Comparing `workforce-1.0.5/workforce/gui.py` & `workforce-1.0.6/workforce/gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,35 @@
                   ]),
         html.Div([
             html.Button('Add Node', id='btn-add', n_clicks=0),
             html.Button('Remove Node', id='btn-remove', n_clicks=0),
         ]),
         cyto.Cytoscape(
             id='cytoscape-elements',
-            layout={'name': 'breadthfirst'},
-            style={'width': '100%', 'height': '450px'},
+            layout={'name': 'breadthfirst',
+                    'directed':True},
+            style={'width': '100%', 'height': '650px'},
+            stylesheet=[
+                {
+                    'selector': 'node',
+                    'style': {
+                        'background-color': 'steelblue',
+                        'label': 'data(id)',
+                        'font-size': '14px',
+                        'width': '30px',
+                        'height': '30px',
+                    }
+                },
+                {
+                    'selector': 'edge',
+                    'style': {
+                        'curve-style': 'taxi',
+                        'target-arrow-shape': 'triangle',
+                        #'events': 'yes'
+                    }}],
             elements=[]
         )
     ])
 
     # Update Graph through load or add
     @app.callback(Output('cytoscape-elements', 'elements'),
                   Input('upload-data', 'contents'),
@@ -36,28 +55,30 @@
                   Input('txt_to', 'value'),
                   State('upload-data', 'filename'),
                   State('upload-data', 'last_modified'),
                   State('cytoscape-elements', 'elements'),
                   prevent_initial_call=True)
     def load_data(contents, n_clicks, txt_from, txt_to, filename, last_modified, elements):
         # For data load
+        print(contents, n_clicks, txt_from, txt_to, filename, last_modified)
         if ctx.triggered_id == 'upload-data':
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
-            edges = elements_to_edges(elements)
+            edges = elements_to_edges(elements) if elements else pd.DataFrame()
             edges = pd.concat([edges, pd.DataFrame([txt_from,txt_to], index=['source','target']).T], axis=0, ignore_index=True).drop_duplicates()
             elements = edges_to_elements(edges)
+            print(elements)
         return elements
 
     # Save data
     @app.callback(Output('download-data', 'data'),
                   Input('btn-download', 'n_clicks'),
                   State('cytoscape-elements', 'elements'),
                   prevent_initial_call=True)
@@ -70,22 +91,21 @@
     def parse_contents(contents, filename):
         import base64
         import io
         content_type, content_string = contents.split(',')
         decoded = base64.b64decode(content_string)
         try:
             if 'csv' in filename:
-                df = pd.read_csv(io.StringIO(decoded.decode('utf-8')), names=['source','target'])
-            if 'tsv' in filename:
-                df = pd.read_csv(io.StringIO(decoded.decode('utf-8')), sep='\t', names=['source','target'])
+                df = pd.read_csv(io.StringIO(decoded.decode('utf-8')))
             elif 'xls' in filename:
-                df = pd.read_excel(io.BytesIO(decoded), names=['source','target'])
+                df = pd.read_excel(io.BytesIO(decoded))
         except Exception as e:
+            print(e)
             return html.Div([
-                'There was an error processing the edgelist'
+                'There was an error processing this file.'
             ])
         return df
 
     def elements_to_edges(elements):
         ele = pd.concat([pd.DataFrame.from_dict(i) for i in elements], axis=1).T.set_index('id')
         edges = ele.drop('label', axis=1).dropna().reset_index(drop=True)
         return edges
```

### Comparing `workforce-1.0.5/workforce/workforce.py` & `workforce-1.0.6/workforce/workforce.py`

 * *Files identical despite different names*

### Comparing `workforce-1.0.5/workforce.egg-info/PKG-INFO` & `workforce-1.0.6/workforce.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workforce
-Version: 1.0.5
+Version: 1.0.6
 Summary: Run bash commands with python multiprocessing according to a csv file edgelist.
 Home-page: https://github.com/theoportlock/workforce
 Author: Theo Portlock
 Author-email: zn.tportlock@gmail.com
 License: MIT license
 Keywords: workforce
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -46,51 +46,45 @@
 ------------
 Installation can be done with 
 
 .. code-block:: bash
 
    pip install workforce
 
-Running workforce
------------------
-To try a sample plan, run with:
+Building a workforce workflow
+-----------------------------
+To build a workflow, simply run:
 
 .. code-block:: bash
 
-   workforce example_plan.csv
+   workforce
 
-To view the program graph, networkx and matplotlib are required. The -g flag is required to produce a dot file of the network:
+Then, paste the IP address into into your browsers address bar and build your program.
+
+Running workforce
+-----------------
+To run a sample plan from workforce github project:
 
 .. code-block:: bash
 
-   workforce -g example_plan.csv
+   workforce example_plan.csv
 
 To import and use in a python shell, use the following command:
 
 .. code-block:: python
 
    from workforce.workforce import worker
    steve = worker("<PLAN.CSV>")
    steve.run()
 
-Graph print
------------
-Converting the graph to a dot can be done using an online dot viewer or using Graphviz software with the example command:
-
-.. code-block:: bash
-
-   dot -Tpng -Kdot -o <DOT_FILENAME>.png <DOT_FILENAME>
-
-.. image:: example_plan.png
-
 The schema should be in the format of a csv with two columns. On the left and right column is the source and target command respectively (see example). Produces a logfile for each run.
 
 Testing
 -------
-Testing can be done within this directory by running:
+Testing can be done within the github directory by running:
 
 .. code-block:: bash
 
    python -m unittest -v
 
 
 =======
```

