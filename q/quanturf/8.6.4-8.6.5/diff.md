# Comparing `tmp/quanturf-8.6.4.tar.gz` & `tmp/quanturf-8.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quanturf-8.6.4.tar", last modified: Tue May 30 15:55:00 2023, max compression
+gzip compressed data, was "quanturf-8.6.5.tar", last modified: Mon Jun 12 14:18:53 2023, max compression
```

## Comparing `quanturf-8.6.4.tar` & `quanturf-8.6.5.tar`

### file list

```diff
@@ -1,29 +1,20 @@
-drwxr-xr-x   0 aayush    (1000) aayush    (1000)        0 2023-05-30 15:55:00.469720 quanturf-8.6.4/
--rw-r--r--   0 aayush    (1000) aayush    (1000)    35149 2023-05-29 13:06:01.000000 quanturf-8.6.4/LICENCE.txt
--rw-r--r--   0 aayush    (1000) aayush    (1000)      780 2023-05-30 15:55:00.469720 quanturf-8.6.4/PKG-INFO
--rw-r--r--   0 aayush    (1000) aayush    (1000)     6705 2023-05-29 13:06:01.000000 quanturf-8.6.4/README.md
-drwxr-xr-x   0 aayush    (1000) aayush    (1000)        0 2023-05-30 15:55:00.468720 quanturf-8.6.4/quanturf/
--rw-r--r--   0 aayush    (1000) aayush    (1000)   728602 2023-05-29 13:06:01.000000 quanturf-8.6.4/quanturf/BarraFactorModel_FactorBased.ipynb
--rw-r--r--   0 aayush    (1000) aayush    (1000)     4437 2023-05-29 13:06:01.000000 quanturf-8.6.4/quanturf/MACD.ipynb
--rw-r--r--   0 aayush    (1000) aayush    (1000)     3025 2023-05-29 13:06:01.000000 quanturf-8.6.4/quanturf/RSI.ipynb
--rw-r--r--   0 aayush    (1000) aayush    (1000)   715205 2023-05-29 13:06:01.000000 quanturf-8.6.4/quanturf/RelativeStrengthIndex(RSI)_Indicator.ipynb
--rw-r--r--   0 aayush    (1000) aayush    (1000)  1092269 2023-05-29 13:06:01.000000 quanturf-8.6.4/quanturf/StochasticOscillator_Indicators.ipynb
--rw-r--r--   0 aayush    (1000) aayush    (1000)        0 2023-05-29 13:06:01.000000 quanturf-8.6.4/quanturf/__init__.py
--rw-r--r--   0 aayush    (1000) aayush    (1000)     6969 2023-05-30 15:53:47.000000 quanturf-8.6.4/quanturf/__main__.py
--rw-r--r--   0 aayush    (1000) aayush    (1000)      127 2023-05-29 14:11:12.000000 quanturf-8.6.4/quanturf/config.yaml
--rw-r--r--   0 aayush    (1000) aayush    (1000)     1667 2023-05-29 13:06:01.000000 quanturf-8.6.4/quanturf/download_data.ipynb
--rw-r--r--   0 aayush    (1000) aayush    (1000)     3186 2023-05-29 13:06:01.000000 quanturf-8.6.4/quanturf/golden_cross.ipynb
--rw-r--r--   0 aayush    (1000) aayush    (1000)    29723 2023-05-29 13:06:01.000000 quanturf-8.6.4/quanturf/jupyter_notebook_config.py
--rw-r--r--   0 aayush    (1000) aayush    (1000)     4102 2023-05-29 13:06:01.000000 quanturf-8.6.4/quanturf/mlp_model.ipynb
--rw-r--r--   0 aayush    (1000) aayush    (1000)     3680 2023-05-30 15:53:47.000000 quanturf-8.6.4/quanturf/quanturf.ipynb
--rw-r--r--   0 aayush    (1000) aayush    (1000)    17341 2023-05-29 13:06:01.000000 quanturf-8.6.4/quanturf/quanturf_logo.py
-drwxr-xr-x   0 aayush    (1000) aayush    (1000)        0 2023-05-30 15:55:00.469720 quanturf-8.6.4/quanturf.egg-info/
--rw-r--r--   0 aayush    (1000) aayush    (1000)      780 2023-05-30 15:55:00.000000 quanturf-8.6.4/quanturf.egg-info/PKG-INFO
--rw-r--r--   0 aayush    (1000) aayush    (1000)      648 2023-05-30 15:55:00.000000 quanturf-8.6.4/quanturf.egg-info/SOURCES.txt
--rw-r--r--   0 aayush    (1000) aayush    (1000)        1 2023-05-30 15:55:00.000000 quanturf-8.6.4/quanturf.egg-info/dependency_links.txt
--rw-r--r--   0 aayush    (1000) aayush    (1000)       52 2023-05-30 15:55:00.000000 quanturf-8.6.4/quanturf.egg-info/entry_points.txt
--rw-r--r--   0 aayush    (1000) aayush    (1000)       68 2023-05-30 15:55:00.000000 quanturf-8.6.4/quanturf.egg-info/requires.txt
--rw-r--r--   0 aayush    (1000) aayush    (1000)        9 2023-05-30 15:55:00.000000 quanturf-8.6.4/quanturf.egg-info/top_level.txt
--rw-r--r--   0 aayush    (1000) aayush    (1000)       38 2023-05-30 15:55:00.469720 quanturf-8.6.4/setup.cfg
--rw-r--r--   0 aayush    (1000) aayush    (1000)     2542 2023-05-30 15:53:47.000000 quanturf-8.6.4/setup.py
--rw-r--r--   0 aayush    (1000) aayush    (1000)      329 2023-05-29 13:19:34.000000 quanturf-8.6.4/version.py
+drwxr-xr-x   0 aayush    (1000) aayush    (1000)        0 2023-06-12 14:18:53.780182 quanturf-8.6.5/
+-rw-r--r--   0 aayush    (1000) aayush    (1000)    35149 2023-05-29 13:06:01.000000 quanturf-8.6.5/LICENCE.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)      780 2023-06-12 14:18:53.780182 quanturf-8.6.5/PKG-INFO
+-rw-r--r--   0 aayush    (1000) aayush    (1000)     6705 2023-05-29 13:06:01.000000 quanturf-8.6.5/README.md
+drwxr-xr-x   0 aayush    (1000) aayush    (1000)        0 2023-06-12 14:18:53.780182 quanturf-8.6.5/quanturf/
+-rw-r--r--   0 aayush    (1000) aayush    (1000)        0 2023-05-29 13:06:01.000000 quanturf-8.6.5/quanturf/__init__.py
+-rw-r--r--   0 aayush    (1000) aayush    (1000)     2055 2023-06-12 14:15:03.000000 quanturf-8.6.5/quanturf/__main__.py
+-rw-r--r--   0 aayush    (1000) aayush    (1000)      157 2023-06-12 14:15:03.000000 quanturf-8.6.5/quanturf/config.yaml
+-rw-r--r--   0 aayush    (1000) aayush    (1000)    29725 2023-06-12 14:15:03.000000 quanturf-8.6.5/quanturf/jupyter_notebook_config.py
+-rw-r--r--   0 aayush    (1000) aayush    (1000)     3674 2023-06-12 14:15:03.000000 quanturf-8.6.5/quanturf/quanturf.ipynb
+drwxr-xr-x   0 aayush    (1000) aayush    (1000)        0 2023-06-12 14:18:53.780182 quanturf-8.6.5/quanturf.egg-info/
+-rw-r--r--   0 aayush    (1000) aayush    (1000)      780 2023-06-12 14:18:53.000000 quanturf-8.6.5/quanturf.egg-info/PKG-INFO
+-rw-r--r--   0 aayush    (1000) aayush    (1000)      358 2023-06-12 14:18:53.000000 quanturf-8.6.5/quanturf.egg-info/SOURCES.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)        1 2023-06-12 14:18:53.000000 quanturf-8.6.5/quanturf.egg-info/dependency_links.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)       52 2023-06-12 14:18:53.000000 quanturf-8.6.5/quanturf.egg-info/entry_points.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)       75 2023-06-12 14:18:53.000000 quanturf-8.6.5/quanturf.egg-info/requires.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)        9 2023-06-12 14:18:53.000000 quanturf-8.6.5/quanturf.egg-info/top_level.txt
+-rw-r--r--   0 aayush    (1000) aayush    (1000)       38 2023-06-12 14:18:53.780182 quanturf-8.6.5/setup.cfg
+-rw-r--r--   0 aayush    (1000) aayush    (1000)     2518 2023-06-12 14:17:25.000000 quanturf-8.6.5/setup.py
+-rw-r--r--   0 aayush    (1000) aayush    (1000)      329 2023-05-29 13:19:34.000000 quanturf-8.6.5/version.py
```

### Comparing `quanturf-8.6.4/LICENCE.txt` & `quanturf-8.6.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `quanturf-8.6.4/PKG-INFO` & `quanturf-8.6.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quanturf
-Version: 8.6.4
+Version: 8.6.5
 Summary: REMOTE_USER Authenticator: An Authenticator for Jupyterhub to read user information from HTTP request headers, as when running behind an authenticating proxy.
 Home-page: https://github.com/Quanturf/quanturf_pypi_package.git
 Author: Quanturf
 Author-email: quanturf.finance@gmail.com
 License: GPLv3
 Keywords: Interactive,Interpreter,Shell,Web
 Platform: Linux
```

### Comparing `quanturf-8.6.4/README.md` & `quanturf-8.6.5/README.md`

 * *Files identical despite different names*

### Comparing `quanturf-8.6.4/quanturf/jupyter_notebook_config.py` & `quanturf-8.6.5/quanturf/jupyter_notebook_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
 
 ## Dict of Python modules to load as notebook server extensions.Entry values can
 #  be used to enable and disable the loading ofthe extensions. The extensions
 #  will be loaded in alphabetical order.
 #c.NotebookApp.nbserver_extensions = {}
 
 ## The directory to use for notebooks and kernels.
-c.NotebookApp.notebook_dir = 'D:\\Python'
+# c.NotebookApp.notebook_dir = 'D:\\Python'
 
 ## Whether to open in a browser after starting. The specific browser used is
 #  platform dependent and determined by the python standard library `webbrowser`
 #  module, unless it is overridden using the --browser (NotebookApp.browser)
 #  configuration option.
 #c.NotebookApp.open_browser = True
```

### Comparing `quanturf-8.6.4/quanturf/quanturf.ipynb` & `quanturf-8.6.5/quanturf/quanturf.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978174603174603%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(2, "*

 * *            '\'Repo.clone_from("https://github.com/Quanturf/AlphaLab-Backtesting", '*

 * *            '"Backtesting")\')], delete: [2]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.11.3'}}"}*

```diff
@@ -63,15 +63,15 @@
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {},
             "outputs": [],
             "source": [
                 "!pip install gitpython\n",
                 "from git import Repo\n",
-                "Repo.clone_from(\"https://github.com/Quanturf/quanturf_alpha_backtesting\", \"Backtesting\")"
+                "Repo.clone_from(\"https://github.com/Quanturf/AlphaLab-Backtesting\", \"Backtesting\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<a id='3.1'></a>\n",
@@ -123,15 +123,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.11.3"
         },
         "vscode": {
             "interpreter": {
                 "hash": "6078e1eae653dd11849a714345a472fcdb72b5135b6ae53d82bc4917104af5e0"
             }
         }
     },
```

### Comparing `quanturf-8.6.4/quanturf.egg-info/PKG-INFO` & `quanturf-8.6.5/quanturf.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quanturf
-Version: 8.6.4
+Version: 8.6.5
 Summary: REMOTE_USER Authenticator: An Authenticator for Jupyterhub to read user information from HTTP request headers, as when running behind an authenticating proxy.
 Home-page: https://github.com/Quanturf/quanturf_pypi_package.git
 Author: Quanturf
 Author-email: quanturf.finance@gmail.com
 License: GPLv3
 Keywords: Interactive,Interpreter,Shell,Web
 Platform: Linux
```

### Comparing `quanturf-8.6.4/setup.py` & `quanturf-8.6.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 version_ns = {}
 with open(pjoin(here, 'version.py')) as f:
     exec(f.read(), {}, version_ns)
 
 setup_args = dict(
     name='quanturf',
     packages=['quanturf'],
-    version="8.6.4",
+    version="8.6.5",
     description="""REMOTE_USER Authenticator: An Authenticator for Jupyterhub to read user information from HTTP request headers, as when running behind an authenticating proxy.""",
     long_description="",
     author="Quanturf",
     author_email="quanturf.finance@gmail.com",
     url="https://github.com/Quanturf/quanturf_pypi_package.git",
     license="GPLv3",
     platforms="Linux, Mac OS X",
@@ -65,19 +65,18 @@
         ]
     }
 )
 
 # setuptools requirements
 if 'setuptools' in sys.modules:
     setup_args['install_requires'] = install_requires = []
-    install_requires.append('jupyterlab')
-    install_requires.append('jupyterlab_templates')
-    install_requires.append('jupyter-app-launcher')
-    install_requires.append('typer')
-    install_requires.append('maskpass')
+    install_requires.append('jupyterlab==3.6.3')
+    install_requires.append('jupyter-app-launcher==0.1.6')
+    install_requires.append('typer==0.9.0')
+    install_requires.append('maskpass==0.3.7')
 
 
 def main():
     setup(**setup_args)
 
 
 if __name__ == '__main__':
```

