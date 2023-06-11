# Comparing `tmp/workforce-0.0.5.tar.gz` & `tmp/workforce-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workforce-0.0.5.tar", last modified: Tue Jan 19 01:22:51 2021, max compression
+gzip compressed data, was "workforce-1.0.5.tar", last modified: Sun Jun 11 22:41:56 2023, max compression
```

## Comparing `workforce-0.0.5.tar` & `workforce-1.0.5.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 theo      (1000) users      (985)        0 2021-01-19 01:22:51.701971 workforce-0.0.5/
--rw-r--r--   0 theo      (1000) users      (985)      161 2021-01-16 23:54:45.000000 workforce-0.0.5/AUTHORS.rst
--rw-r--r--   0 theo      (1000) users      (985)       89 2021-01-16 23:56:28.000000 workforce-0.0.5/HISTORY.rst
--rw-r--r--   0 theo      (1000) users      (985)     1072 2021-01-16 13:09:03.000000 workforce-0.0.5/LICENSE
--rw-r--r--   0 theo      (1000) users      (985)      262 2021-01-18 15:56:56.000000 workforce-0.0.5/MANIFEST.in
--rw-r--r--   0 theo      (1000) users      (985)     3264 2021-01-19 01:22:51.701971 workforce-0.0.5/PKG-INFO
--rw-r--r--   0 theo      (1000) users      (985)     1824 2021-01-17 00:01:11.000000 workforce-0.0.5/README.rst
-drwxr-xr-x   0 theo      (1000) users      (985)        0 2021-01-19 01:22:51.701971 workforce-0.0.5/docs/
--rw-r--r--   0 theo      (1000) users      (985)      610 2021-01-17 00:22:48.000000 workforce-0.0.5/docs/Makefile
--rw-r--r--   0 theo      (1000) users      (985)       28 2021-01-17 00:22:48.000000 workforce-0.0.5/docs/authors.rst
--rwxr-xr-x   0 theo      (1000) users      (985)     4807 2021-01-17 00:22:48.000000 workforce-0.0.5/docs/conf.py
--rw-r--r--   0 theo      (1000) users      (985)       33 2021-01-17 00:22:48.000000 workforce-0.0.5/docs/contributing.rst
--rw-r--r--   0 theo      (1000) users      (985)       28 2021-01-17 00:22:48.000000 workforce-0.0.5/docs/history.rst
--rw-r--r--   0 theo      (1000) users      (985)      306 2021-01-17 00:22:48.000000 workforce-0.0.5/docs/index.rst
--rw-r--r--   0 theo      (1000) users      (985)     1146 2021-01-17 00:22:48.000000 workforce-0.0.5/docs/installation.rst
--rw-r--r--   0 theo      (1000) users      (985)      771 2021-01-17 00:22:48.000000 workforce-0.0.5/docs/make.bat
--rw-r--r--   0 theo      (1000) users      (985)       27 2021-01-17 00:22:48.000000 workforce-0.0.5/docs/readme.rst
--rw-r--r--   0 theo      (1000) users      (985)       73 2021-01-17 00:22:48.000000 workforce-0.0.5/docs/usage.rst
--rw-r--r--   0 theo      (1000) users      (985)       38 2021-01-19 01:22:51.701971 workforce-0.0.5/setup.cfg
--rw-r--r--   0 theo      (1000) users      (985)     1309 2021-01-19 01:09:09.000000 workforce-0.0.5/setup.py
-drwxr-xr-x   0 theo      (1000) users      (985)        0 2021-01-19 01:22:51.701971 workforce-0.0.5/workforce/
--rw-r--r--   0 theo      (1000) users      (985)      132 2021-01-17 13:22:24.000000 workforce-0.0.5/workforce/__init__.py
--rwxr-xr-x   0 theo      (1000) users      (985)      594 2021-01-19 01:22:43.000000 workforce-0.0.5/workforce/cli.py
--rwxr-xr-x   0 theo      (1000) users      (985)     1663 2021-01-19 01:16:00.000000 workforce-0.0.5/workforce/workforce.py
-drwxr-xr-x   0 theo      (1000) users      (985)        0 2021-01-19 01:22:51.701971 workforce-0.0.5/workforce.egg-info/
--rw-r--r--   0 theo      (1000) users      (985)     3264 2021-01-19 01:22:51.000000 workforce-0.0.5/workforce.egg-info/PKG-INFO
--rw-r--r--   0 theo      (1000) users      (985)      490 2021-01-19 01:22:51.000000 workforce-0.0.5/workforce.egg-info/SOURCES.txt
--rw-r--r--   0 theo      (1000) users      (985)        1 2021-01-19 01:22:51.000000 workforce-0.0.5/workforce.egg-info/dependency_links.txt
--rw-r--r--   0 theo      (1000) users      (985)       50 2021-01-19 01:22:51.000000 workforce-0.0.5/workforce.egg-info/entry_points.txt
--rw-r--r--   0 theo      (1000) users      (985)       15 2021-01-19 01:22:51.000000 workforce-0.0.5/workforce.egg-info/requires.txt
--rw-r--r--   0 theo      (1000) users      (985)       10 2021-01-19 01:22:51.000000 workforce-0.0.5/workforce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:41:56.091722 workforce-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-11 22:41:44.000000 workforce-1.0.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-11 22:41:44.000000 workforce-1.0.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-11 22:41:44.000000 workforce-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-11 22:41:44.000000 workforce-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-11 22:41:56.091722 workforce-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-11 22:41:44.000000 workforce-1.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:41:56.091722 workforce-1.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4807 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-11 22:41:44.000000 workforce-1.0.5/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 22:41:56.091722 workforce-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-11 22:41:44.000000 workforce-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:41:56.091722 workforce-1.0.5/workforce/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-11 22:41:44.000000 workforce-1.0.5/workforce/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-06-11 22:41:44.000000 workforce-1.0.5/workforce/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4316 2023-06-11 22:41:44.000000 workforce-1.0.5/workforce/gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-11 22:41:44.000000 workforce-1.0.5/workforce/workforce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:41:56.091722 workforce-1.0.5/workforce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-11 22:41:56.000000 workforce-1.0.5/workforce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-11 22:41:56.000000 workforce-1.0.5/workforce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 22:41:56.000000 workforce-1.0.5/workforce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-11 22:41:56.000000 workforce-1.0.5/workforce.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-11 22:41:56.000000 workforce-1.0.5/workforce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 22:41:56.000000 workforce-1.0.5/workforce.egg-info/top_level.txt
```

### Comparing `workforce-0.0.5/LICENSE` & `workforce-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `workforce-0.0.5/PKG-INFO` & `workforce-1.0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,103 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: workforce
-Version: 0.0.5
+Version: 1.0.5
 Summary: Run bash commands with python multiprocessing according to a csv file edgelist.
 Home-page: https://github.com/theoportlock/workforce
 Author: Theo Portlock
 Author-email: zn.tportlock@gmail.com
 License: MIT license
-Description: =========
-        workforce
-        =========
-        
-        
-        .. image:: https://img.shields.io/pypi/v/workforce.svg
-                :target: https://pypi.python.org/pypi/workforce
-        
-        .. image:: https://img.shields.io/travis/theoportlock/workforce.svg
-                :target: https://travis-ci.com/theoportlock/workforce
-        
-        .. image:: https://readthedocs.org/projects/workforce/badge/?version=latest
-                :target: https://workforce.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        
-        
-        
-        Run bash commands with python multiprocessing according to a csv file edgelist.
-        
-        
-        * Free software: MIT license
-        * Documentation: https://workforce.readthedocs.io.
-        
-        
-        Features
-        --------
-        Installation can be done with 
-        
-        `pip install workforce`
-        
-        To try a sample plan, run with:
-        
-        `python workforce.py example_plan.csv`
-        
-        To view the program graph, networkx and matplotlib are required. The -g flag is required to produce a dot file of the network:
-        
-        `python3 workforce.py -g example_plan.csv`
-        
-        Converting the graph to a dot can be done using an online dot viewer or using Graphviz software with the example command:
-        
-        `dot -Tpng -Kdot -o <DOT_FILENAME>.png <DOT_FILENAME>`
-        
-        .. image:: example_plan.png
-        
-        The schema should be in the format of a csv with two columns. On the left and right column is the source and target command respectively (see example). Produces a logfile for each run.
-        
-        The following bashrc alias is recommended if this repository is in your home directory:
-        
-        `alias wf="python ~/workforce/workforce.py"`
-        
-        Testing can be done within this directory by running:
-        `python -m unittest -v`
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.0 (2021-01-16)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: workforce
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=========
+workforce
+=========
+
+
+.. image:: https://img.shields.io/pypi/v/workforce.svg
+        :target: https://pypi.python.org/pypi/workforce
+
+.. image:: https://img.shields.io/travis/theoportlock/workforce.svg
+        :target: https://travis-ci.com/theoportlock/workforce
+
+.. image:: https://readthedocs.org/projects/workforce/badge/?version=latest
+        :target: https://workforce.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+
+Run bash commands with python multiprocessing according to a csv file edgelist.
+
+* Free software: MIT license
+* Documentation: https://workforce.readthedocs.io.
+
+
+Installation
+------------
+Installation can be done with 
+
+.. code-block:: bash
+
+   pip install workforce
+
+Running workforce
+-----------------
+To try a sample plan, run with:
+
+.. code-block:: bash
+
+   workforce example_plan.csv
+
+To view the program graph, networkx and matplotlib are required. The -g flag is required to produce a dot file of the network:
+
+.. code-block:: bash
+
+   workforce -g example_plan.csv
+
+To import and use in a python shell, use the following command:
+
+.. code-block:: python
+
+   from workforce.workforce import worker
+   steve = worker("<PLAN.CSV>")
+   steve.run()
+
+Graph print
+-----------
+Converting the graph to a dot can be done using an online dot viewer or using Graphviz software with the example command:
+
+.. code-block:: bash
+
+   dot -Tpng -Kdot -o <DOT_FILENAME>.png <DOT_FILENAME>
+
+.. image:: example_plan.png
+
+The schema should be in the format of a csv with two columns. On the left and right column is the source and target command respectively (see example). Produces a logfile for each run.
+
+Testing
+-------
+Testing can be done within this directory by running:
+
+.. code-block:: bash
+
+   python -m unittest -v
+
+
+=======
+History
+=======
+
+0.1.0 (2021-01-16)
+------------------
+
+* First release on PyPI.
```

### Comparing `workforce-0.0.5/docs/Makefile` & `workforce-1.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `workforce-0.0.5/docs/conf.py` & `workforce-1.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `workforce-0.0.5/docs/installation.rst` & `workforce-1.0.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `workforce-0.0.5/docs/make.bat` & `workforce-1.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `workforce-0.0.5/setup.py` & `workforce-1.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ["networkx", "pydot",]
+requirements = ["networkx", "pydot", "dash_cytoscape", "dash", "pandas", "matplotlib", "openpyxl", ]
 
 setup(
     author="Theo Portlock",
     author_email='zn.tportlock@gmail.com',
     python_requires='>=3.5',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
@@ -36,9 +36,9 @@
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     keywords='workforce',
     name='workforce',
     packages = ["workforce"],
     url='https://github.com/theoportlock/workforce',
-    version='0.0.5',
+    version='1.0.5',
 )
```

### Comparing `workforce-0.0.5/workforce/workforce.py` & `workforce-1.0.5/workforce/workforce.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,21 +11,14 @@
 class worker:
     def __init__(self, plan_file):
         # Load plan
         self.plan_file = plan_file
         with open(self.plan_file) as csvfile:
             self.plan = list(csv.reader(csvfile, skipinitialspace=True))
 
-    def graph(self):
-        # Create graph based on a dataframe
-        import networkx as nx
-        G = nx.MultiDiGraph()
-        G.add_edges_from((({'' : '#'}.get(i, i), {'' : '#'}.get(j, j)) for (i, j) in self.plan))
-        nx.drawing.nx_pydot.write_dot(G, self.plan_file + ".dot")
-
     def run(self):
         # Run loaded plan beginning from the first row
         self.init_time = str(time())
         logging.basicConfig(
                 filename=str(Path.home())+"/.wflog.csv",
                 filemode="a",
                 format="%(created).6f, "+self.init_time+", "+str(os.getpid())+", %(processName)s, %(message)s",
```

### Comparing `workforce-0.0.5/workforce.egg-info/PKG-INFO` & `workforce-1.0.5/workforce.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,103 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: workforce
-Version: 0.0.5
+Version: 1.0.5
 Summary: Run bash commands with python multiprocessing according to a csv file edgelist.
 Home-page: https://github.com/theoportlock/workforce
 Author: Theo Portlock
 Author-email: zn.tportlock@gmail.com
 License: MIT license
-Description: =========
-        workforce
-        =========
-        
-        
-        .. image:: https://img.shields.io/pypi/v/workforce.svg
-                :target: https://pypi.python.org/pypi/workforce
-        
-        .. image:: https://img.shields.io/travis/theoportlock/workforce.svg
-                :target: https://travis-ci.com/theoportlock/workforce
-        
-        .. image:: https://readthedocs.org/projects/workforce/badge/?version=latest
-                :target: https://workforce.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        
-        
-        
-        Run bash commands with python multiprocessing according to a csv file edgelist.
-        
-        
-        * Free software: MIT license
-        * Documentation: https://workforce.readthedocs.io.
-        
-        
-        Features
-        --------
-        Installation can be done with 
-        
-        `pip install workforce`
-        
-        To try a sample plan, run with:
-        
-        `python workforce.py example_plan.csv`
-        
-        To view the program graph, networkx and matplotlib are required. The -g flag is required to produce a dot file of the network:
-        
-        `python3 workforce.py -g example_plan.csv`
-        
-        Converting the graph to a dot can be done using an online dot viewer or using Graphviz software with the example command:
-        
-        `dot -Tpng -Kdot -o <DOT_FILENAME>.png <DOT_FILENAME>`
-        
-        .. image:: example_plan.png
-        
-        The schema should be in the format of a csv with two columns. On the left and right column is the source and target command respectively (see example). Produces a logfile for each run.
-        
-        The following bashrc alias is recommended if this repository is in your home directory:
-        
-        `alias wf="python ~/workforce/workforce.py"`
-        
-        Testing can be done within this directory by running:
-        `python -m unittest -v`
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.0 (2021-01-16)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: workforce
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=========
+workforce
+=========
+
+
+.. image:: https://img.shields.io/pypi/v/workforce.svg
+        :target: https://pypi.python.org/pypi/workforce
+
+.. image:: https://img.shields.io/travis/theoportlock/workforce.svg
+        :target: https://travis-ci.com/theoportlock/workforce
+
+.. image:: https://readthedocs.org/projects/workforce/badge/?version=latest
+        :target: https://workforce.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+
+Run bash commands with python multiprocessing according to a csv file edgelist.
+
+* Free software: MIT license
+* Documentation: https://workforce.readthedocs.io.
+
+
+Installation
+------------
+Installation can be done with 
+
+.. code-block:: bash
+
+   pip install workforce
+
+Running workforce
+-----------------
+To try a sample plan, run with:
+
+.. code-block:: bash
+
+   workforce example_plan.csv
+
+To view the program graph, networkx and matplotlib are required. The -g flag is required to produce a dot file of the network:
+
+.. code-block:: bash
+
+   workforce -g example_plan.csv
+
+To import and use in a python shell, use the following command:
+
+.. code-block:: python
+
+   from workforce.workforce import worker
+   steve = worker("<PLAN.CSV>")
+   steve.run()
+
+Graph print
+-----------
+Converting the graph to a dot can be done using an online dot viewer or using Graphviz software with the example command:
+
+.. code-block:: bash
+
+   dot -Tpng -Kdot -o <DOT_FILENAME>.png <DOT_FILENAME>
+
+.. image:: example_plan.png
+
+The schema should be in the format of a csv with two columns. On the left and right column is the source and target command respectively (see example). Produces a logfile for each run.
+
+Testing
+-------
+Testing can be done within this directory by running:
+
+.. code-block:: bash
+
+   python -m unittest -v
+
+
+=======
+History
+=======
+
+0.1.0 (2021-01-16)
+------------------
+
+* First release on PyPI.
```

