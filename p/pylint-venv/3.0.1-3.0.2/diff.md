# Comparing `tmp/pylint_venv-3.0.1.tar.gz` & `tmp/pylint_venv-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint_venv-3.0.1.tar", max compression
+gzip compressed data, was "pylint_venv-3.0.2.tar", max compression
```

## Comparing `pylint_venv-3.0.1.tar` & `pylint_venv-3.0.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     2604 2023-02-23 20:52:16.566789 pylint_venv-3.0.1/CHANGES.md
--rw-r--r--   0        0        0     1116 2023-02-23 20:52:16.566789 pylint_venv-3.0.1/LICENSE.txt
--rw-r--r--   0        0        0     3668 2023-02-23 20:52:16.566789 pylint_venv-3.0.1/README.rst
--rw-r--r--   0        0        0     4165 2023-02-23 20:52:16.566789 pylint_venv-3.0.1/pylint_venv.py
--rw-r--r--   0        0        0     1416 2023-02-23 20:52:16.566789 pylint_venv-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     4411 1970-01-01 00:00:00.000000 pylint_venv-3.0.1/setup.py
--rw-r--r--   0        0        0     5156 1970-01-01 00:00:00.000000 pylint_venv-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2785 2023-06-12 15:48:26.929004 pylint_venv-3.0.2/CHANGES.md
+-rw-r--r--   0        0        0     1116 2023-06-12 15:48:26.929004 pylint_venv-3.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     3668 2023-06-12 15:48:26.929004 pylint_venv-3.0.2/README.rst
+-rw-r--r--   0        0        0     4316 2023-06-12 15:48:26.929004 pylint_venv-3.0.2/pylint_venv.py
+-rw-r--r--   0        0        0     1416 2023-06-12 15:48:26.929004 pylint_venv-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4906 1970-01-01 00:00:00.000000 pylint_venv-3.0.2/PKG-INFO
```

### Comparing `pylint_venv-3.0.1/CHANGES.md` & `pylint_venv-3.0.2/CHANGES.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [3.0.2] - 2023-06-12
+
+### Fixed
+
+- Handle symlinks pointing to the main `python3.x` directory in a venv.
+  In particular, this fixes an issue with Conda and Python 3.10 (#16).
+
+
 ## [3.0.1] - 2023-02-23
 
 ### Fixed
 
 - Add changelog (`CHANGES.md`) back into source distribution.
```

### Comparing `pylint_venv-3.0.1/LICENSE.txt` & `pylint_venv-3.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pylint_venv-3.0.1/README.rst` & `pylint_venv-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pylint_venv-3.0.1/pylint_venv.py` & `pylint_venv-3.0.2/pylint_venv.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,23 +82,27 @@
     if IS_PYPY:
         site_packages = os.path.join(venv, "site-packages")
     elif IS_WIN:
         site_packages = os.path.join(venv, "Lib", "site-packages")
     else:
         lib_dir = os.path.join(venv, "lib")
         python_dirs = [d for d in os.listdir(lib_dir) if re.match(r"python\d+.\d+", d)]
+
+        # Resolve symlinks and remove repeated directories
+        python_dirs = set([os.path.realpath(os.path.join(lib_dir, d)) for d in python_dirs])
+
         if len(python_dirs) == 0:
             raise IncompatibleVenvError(
                 f"The virtual environment {venv!r} is missing a lib/pythonX.Y directory."
             )
         if len(python_dirs) > 1:
             raise IncompatibleVenvError(
                 f"The virtual environment {venv!r} has multiple lib/pythonX.Y directories."
             )
-        site_packages = os.path.join(lib_dir, python_dirs[0], "site-packages")
+        site_packages = os.path.join(list(python_dirs)[0], "site-packages")
 
     prev = set(sys.path)
     site.addsitedir(site_packages)
     sys.real_prefix = sys.prefix
     sys.prefix = venv
 
     # Move the added items to the front of sys.path (in place!)
```

### Comparing `pylint_venv-3.0.1/pyproject.toml` & `pylint_venv-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 include = ["pylint_venv.py", {path = "CHANGES.md", format = "sdist"}]
 keywords = ["pylint", "virtualenv", "venv"]
 license = "MIT"
 maintainers = ["Jan Gosmann <jan@hyper-world.de>"]
 name = "pylint-venv"
 readme = "README.rst"
 repository = "https://github.com/jgosmann/pylint-venv/"
-version = "3.0.1"
+version = "3.0.2"
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
 
 [tool.poetry.dev-dependencies]
 pylint = '^2.14.0'
```

### Comparing `pylint_venv-3.0.1/setup.py` & `pylint_venv-3.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,157 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pylint-venv
+Version: 3.0.2
+Summary: pylint-venv provides a Pylint init-hook to use the same Pylint installation with different virtual environments.
+Home-page: https://github.com/jgosmann/pylint-venv/
+License: MIT
+Keywords: pylint,virtualenv,venv
+Author: Jan Gosmann
+Author-email: jan@hyper-world.de
+Maintainer: Jan Gosmann
+Maintainer-email: jan@hyper-world.de
+Requires-Python: >=3.7.2,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Plugins
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development
+Project-URL: Repository, https://github.com/jgosmann/pylint-venv/
+Description-Content-Type: text/x-rst
 
-modules = \
-['pylint_venv']
-setup_kwargs = {
-    'name': 'pylint-venv',
-    'version': '3.0.1',
-    'description': 'pylint-venv provides a Pylint init-hook to use the same Pylint installation with different virtual environments.',
-    'long_description': 'pylint-venv\n===========\n\nPylint_ does not respect the currently activated virtualenv_ if it is not\ninstalled in every virtual environment individually.  This module provides\na Pylint init-hook to use the same Pylint installation with different virtual\nenvironments.\n\nInstallation\n------------\n\n.. code:: bash\n\n    pip install pylint-venv\n\nAdd the following to your ``~/.pylintrc``:\n\n.. code:: ini\n\n    [MAIN]\n    init-hook=\n        try: import pylint_venv\n        except ImportError: pass\n        else: pylint_venv.inithook()\n\nThe hook will then be used automatically if\n\n- a virtualenv without pylint is active,\n\n- or a Conda environment without pylint is active,\n\n- or no environment is active but your CWD contains virtualenv directory.\n\nAnything listed in the ``PYLINT_VENV_PATH`` environment variable is considered\na virtualenv directory. The default, if the variable is unset, is `.venv`. Use\na colon (`:`) as path separator. Example for checking directories ``.venv`` and\n``.virtualenv``:\n\n.. code:: console\n\n    PYLINT_VENV_PATH=.venv:.virtualenv\n\nYou can also call the hook via a command line argument:\n\n.. code:: console\n\n    $ pylint --init-hook="import pylint_venv; pylint_venv.inithook()"\n\nThis way you can also explicitly set an environment to be used:\n\n.. code:: console\n\n    $ pylint --init-hook="import pylint_venv; pylint_venv.inithook(\'$(pwd)/env\')"\n\nIf ``pylint`` itself is installed in a virtualenv, then you can ignore it by passing\n``force_venv_activation=True`` to force the activation of a different virtualenv:\n\n.. code:: console\n\n    $ pylint --init-hook="import pylint_venv; pylint_venv.inithook(force_venv_activation=True)"\n\n\nThis will try to automatically detect virtualenv and activate it.\n\n\nTroubleshooting\n---------------\n\nGeneral\n^^^^^^^\n\npylint_venv fails to import\n"""""""""""""""""""""""""""\n\nMost likely pylint-venv is not installed in the same virtual environment as\npylint. Either make sure to ensure pylint-venv into the same virtual environment\nas pylint, or add the appropriate path in the init hook:\n\n.. code:: python\n\n    import sys\n    sys.path.append("/path/to/installation/folder/of/pylint_venv")\n\n\npylint_venv breaks parsing with tools\n"""""""""""""""""""""""""""""""""""""\n\nWhen tools call pylint with :code:`-f json`, an extra line may break the parser, as the \noutput is no longer valid json. To avoid printing "using venv ...", pass :code:`quiet=True`\nto :code:`inithook`\n\n.. code:: console\n\n   $ pylint -f json --init-hook="import pylint_venv; pylint_venv.inithook(quiet=True)"\n\n\nVirtual environment does not get used (installed modules are reported as \'unable to import\')\n""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""\n\nMost likely the virtual environment does not get activated because pylint itself\nruns in a virtual environment. You can force the activation of the virtual\nenvironment with the :code:`force_venv_activation=True` flag to the\n:code:`pylint_venv.inithook` function.\n\n\nHomebrew\n^^^^^^^^\n\nHomebrew installs pylint into a separate virtual environment, thus you will\nneed to set the `force_venv_activation=True` flag. This also means, that\npylint_venv will be in a different search path and you must add the proper\npath to `sys.path`. You can use the following configuration adjusted to your\nPython version:\n\n.. code:: ini\n\n    [MAIN]\n    init-hook=\n        import sys\n        sys.path.append("/usr/local/lib/python3.8/site-packages")\n        try: import pylint_venv\n        except ImportError: pass\n        else: pylint_venv.inithook(force_venv_activation=True)\n\n\n.. _Pylint: http://www.pylint.org/\n.. _virtualenv: https://virtualenv.pypa.io/en/latest/\n',
-    'author': 'Jan Gosmann',
-    'author_email': 'jan@hyper-world.de',
-    'maintainer': 'Jan Gosmann',
-    'maintainer_email': 'jan@hyper-world.de',
-    'url': 'https://github.com/jgosmann/pylint-venv/',
-    'py_modules': modules,
-    'python_requires': '>=3.7.2,<4.0.0',
-}
+pylint-venv
+===========
 
+Pylint_ does not respect the currently activated virtualenv_ if it is not
+installed in every virtual environment individually.  This module provides
+a Pylint init-hook to use the same Pylint installation with different virtual
+environments.
+
+Installation
+------------
+
+.. code:: bash
+
+    pip install pylint-venv
+
+Add the following to your ``~/.pylintrc``:
+
+.. code:: ini
+
+    [MAIN]
+    init-hook=
+        try: import pylint_venv
+        except ImportError: pass
+        else: pylint_venv.inithook()
+
+The hook will then be used automatically if
+
+- a virtualenv without pylint is active,
+
+- or a Conda environment without pylint is active,
+
+- or no environment is active but your CWD contains virtualenv directory.
+
+Anything listed in the ``PYLINT_VENV_PATH`` environment variable is considered
+a virtualenv directory. The default, if the variable is unset, is `.venv`. Use
+a colon (`:`) as path separator. Example for checking directories ``.venv`` and
+``.virtualenv``:
+
+.. code:: console
+
+    PYLINT_VENV_PATH=.venv:.virtualenv
+
+You can also call the hook via a command line argument:
+
+.. code:: console
+
+    $ pylint --init-hook="import pylint_venv; pylint_venv.inithook()"
+
+This way you can also explicitly set an environment to be used:
+
+.. code:: console
+
+    $ pylint --init-hook="import pylint_venv; pylint_venv.inithook('$(pwd)/env')"
+
+If ``pylint`` itself is installed in a virtualenv, then you can ignore it by passing
+``force_venv_activation=True`` to force the activation of a different virtualenv:
+
+.. code:: console
+
+    $ pylint --init-hook="import pylint_venv; pylint_venv.inithook(force_venv_activation=True)"
+
+
+This will try to automatically detect virtualenv and activate it.
+
+
+Troubleshooting
+---------------
+
+General
+^^^^^^^
+
+pylint_venv fails to import
+"""""""""""""""""""""""""""
+
+Most likely pylint-venv is not installed in the same virtual environment as
+pylint. Either make sure to ensure pylint-venv into the same virtual environment
+as pylint, or add the appropriate path in the init hook:
+
+.. code:: python
+
+    import sys
+    sys.path.append("/path/to/installation/folder/of/pylint_venv")
+
+
+pylint_venv breaks parsing with tools
+"""""""""""""""""""""""""""""""""""""
+
+When tools call pylint with :code:`-f json`, an extra line may break the parser, as the 
+output is no longer valid json. To avoid printing "using venv ...", pass :code:`quiet=True`
+to :code:`inithook`
+
+.. code:: console
+
+   $ pylint -f json --init-hook="import pylint_venv; pylint_venv.inithook(quiet=True)"
+
+
+Virtual environment does not get used (installed modules are reported as 'unable to import')
+""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
+
+Most likely the virtual environment does not get activated because pylint itself
+runs in a virtual environment. You can force the activation of the virtual
+environment with the :code:`force_venv_activation=True` flag to the
+:code:`pylint_venv.inithook` function.
+
+
+Homebrew
+^^^^^^^^
+
+Homebrew installs pylint into a separate virtual environment, thus you will
+need to set the `force_venv_activation=True` flag. This also means, that
+pylint_venv will be in a different search path and you must add the proper
+path to `sys.path`. You can use the following configuration adjusted to your
+Python version:
+
+.. code:: ini
+
+    [MAIN]
+    init-hook=
+        import sys
+        sys.path.append("/usr/local/lib/python3.8/site-packages")
+        try: import pylint_venv
+        except ImportError: pass
+        else: pylint_venv.inithook(force_venv_activation=True)
+
+
+.. _Pylint: http://www.pylint.org/
+.. _virtualenv: https://virtualenv.pypa.io/en/latest/
 
-setup(**setup_kwargs)
```

