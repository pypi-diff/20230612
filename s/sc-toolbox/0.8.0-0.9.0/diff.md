# Comparing `tmp/sc-toolbox-0.8.0.tar.gz` & `tmp/sc-toolbox-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc-toolbox-0.8.0.tar", max compression
+gzip compressed data, was "sc-toolbox-0.9.0.tar", max compression
```

## Comparing `sc-toolbox-0.8.0.tar` & `sc-toolbox-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1070 2021-05-27 09:53:32.573976 sc-toolbox-0.8.0/LICENSE
--rw-r--r--   0        0        0     3946 2021-05-27 09:53:32.573976 sc-toolbox-0.8.0/README.rst
--rw-r--r--   0        0        0     1957 2021-05-27 09:53:32.677975 sc-toolbox-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      174 2021-05-27 09:53:32.677975 sc-toolbox-0.8.0/sc_toolbox/__init__.py
--rw-r--r--   0        0        0     4147 2021-05-27 09:53:32.677975 sc-toolbox-0.8.0/sc_toolbox/__main__.py
--rw-r--r--   0        0        0        0 2021-05-27 09:53:32.677975 sc-toolbox-0.8.0/sc_toolbox/api/__init__.py
--rw-r--r--   0        0        0    17460 2021-05-27 09:53:32.677975 sc-toolbox-0.8.0/sc_toolbox/api/calc/__init__.py
--rw-r--r--   0        0        0  1377008 2021-05-27 09:53:32.685975 sc-toolbox-0.8.0/sc_toolbox/api/calc/markers/lung_particle_markers.txt
--rw-r--r--   0        0        0    37900 2021-05-27 09:53:32.685975 sc-toolbox-0.8.0/sc_toolbox/api/plot/__init__.py
--rw-r--r--   0        0        0     1744 2021-05-27 09:53:32.685975 sc-toolbox-0.8.0/sc_toolbox/api/util/__init__.py
--rw-r--r--   0        0        0        0 2021-05-27 09:53:32.685975 sc-toolbox-0.8.0/sc_toolbox/cli/__init__.py
--rw-r--r--   0        0        0        0 2021-05-27 09:53:32.685975 sc-toolbox-0.8.0/sc_toolbox/cli/commands/__init__.py
--rw-r--r--   0        0        0     2617 2021-05-27 09:53:32.685975 sc-toolbox-0.8.0/sc_toolbox/cli/commands/create.py
--rw-r--r--   0        0        0       51 2021-05-27 09:53:32.685975 sc-toolbox-0.8.0/sc_toolbox/cli/commands/templates/simple_docker/cookiecutter.json
--rw-r--r--   0        0        0     1469 2021-05-27 09:53:32.685975 sc-toolbox-0.8.0/sc_toolbox/cli/commands/templates/simple_docker/{{ cookiecutter.project_slug }}/Dockerfile
--rw-r--r--   0        0        0      390 2021-05-27 09:53:32.685975 sc-toolbox-0.8.0/sc_toolbox/cli/commands/templates/simple_docker/{{ cookiecutter.project_slug }}/README.md
--rw-r--r--   0        0        0      541 2021-05-27 09:53:32.685975 sc-toolbox-0.8.0/sc_toolbox/cli/commands/templates/simple_docker/{{ cookiecutter.project_slug }}/environment.yml
--rwxr-xr-x   0        0        0       38 2021-05-27 09:53:32.685975 sc-toolbox-0.8.0/sc_toolbox/cli/commands/templates/simple_docker/{{ cookiecutter.project_slug }}/start.sh
--rw-r--r--   0        0        0     4166 2021-05-27 09:53:32.685975 sc-toolbox-0.8.0/sc_toolbox/cli/commands/upgrade.py
--rw-r--r--   0        0        0     3025 2021-05-27 09:53:32.685975 sc-toolbox-0.8.0/sc_toolbox/cli/questionary.py
--rw-r--r--   0        0        0        0 2021-05-27 09:53:32.685975 sc-toolbox-0.8.0/sc_toolbox/py.typed
--rw-r--r--   0        0        0     5593 2021-05-27 09:53:41.654463 sc-toolbox-0.8.0/setup.py
--rw-r--r--   0        0        0     5263 2021-05-27 09:53:41.654855 sc-toolbox-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2021-06-08 15:49:50.490482 sc-toolbox-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3946 2021-06-08 15:49:50.490482 sc-toolbox-0.9.0/README.rst
+-rw-r--r--   0        0        0     1957 2021-06-08 15:49:50.614482 sc-toolbox-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      174 2021-06-08 15:49:50.614482 sc-toolbox-0.9.0/sc_toolbox/__init__.py
+-rw-r--r--   0        0        0     4147 2021-06-08 15:49:50.614482 sc-toolbox-0.9.0/sc_toolbox/__main__.py
+-rw-r--r--   0        0        0        0 2021-06-08 15:49:50.614482 sc-toolbox-0.9.0/sc_toolbox/api/__init__.py
+-rw-r--r--   0        0        0    18526 2021-06-08 15:49:50.614482 sc-toolbox-0.9.0/sc_toolbox/api/calc/__init__.py
+-rw-r--r--   0        0        0  1377008 2021-06-08 15:49:50.626482 sc-toolbox-0.9.0/sc_toolbox/api/calc/markers/lung_particle_markers.txt
+-rw-r--r--   0        0        0    37900 2021-06-08 15:49:50.626482 sc-toolbox-0.9.0/sc_toolbox/api/plot/__init__.py
+-rw-r--r--   0        0        0     1744 2021-06-08 15:49:50.626482 sc-toolbox-0.9.0/sc_toolbox/api/util/__init__.py
+-rw-r--r--   0        0        0        0 2021-06-08 15:49:50.626482 sc-toolbox-0.9.0/sc_toolbox/cli/__init__.py
+-rw-r--r--   0        0        0        0 2021-06-08 15:49:50.626482 sc-toolbox-0.9.0/sc_toolbox/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2617 2021-06-08 15:49:50.626482 sc-toolbox-0.9.0/sc_toolbox/cli/commands/create.py
+-rw-r--r--   0        0        0       51 2021-06-08 15:49:50.626482 sc-toolbox-0.9.0/sc_toolbox/cli/commands/templates/simple_docker/cookiecutter.json
+-rw-r--r--   0        0        0     1469 2021-06-08 15:49:50.626482 sc-toolbox-0.9.0/sc_toolbox/cli/commands/templates/simple_docker/{{ cookiecutter.project_slug }}/Dockerfile
+-rw-r--r--   0        0        0      390 2021-06-08 15:49:50.626482 sc-toolbox-0.9.0/sc_toolbox/cli/commands/templates/simple_docker/{{ cookiecutter.project_slug }}/README.md
+-rw-r--r--   0        0        0      541 2021-06-08 15:49:50.626482 sc-toolbox-0.9.0/sc_toolbox/cli/commands/templates/simple_docker/{{ cookiecutter.project_slug }}/environment.yml
+-rwxr-xr-x   0        0        0       38 2021-06-08 15:49:50.626482 sc-toolbox-0.9.0/sc_toolbox/cli/commands/templates/simple_docker/{{ cookiecutter.project_slug }}/start.sh
+-rw-r--r--   0        0        0     4166 2021-06-08 15:49:50.626482 sc-toolbox-0.9.0/sc_toolbox/cli/commands/upgrade.py
+-rw-r--r--   0        0        0     3025 2021-06-08 15:49:50.626482 sc-toolbox-0.9.0/sc_toolbox/cli/questionary.py
+-rw-r--r--   0        0        0        0 2021-06-08 15:49:50.626482 sc-toolbox-0.9.0/sc_toolbox/py.typed
+-rw-r--r--   0        0        0     5593 2021-06-08 15:50:00.287063 sc-toolbox-0.9.0/setup.py
+-rw-r--r--   0        0        0     5263 2021-06-08 15:50:00.287555 sc-toolbox-0.9.0/PKG-INFO
```

### Comparing `sc-toolbox-0.8.0/LICENSE` & `sc-toolbox-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sc-toolbox-0.8.0/README.rst` & `sc-toolbox-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `sc-toolbox-0.8.0/pyproject.toml` & `sc-toolbox-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sc-toolbox"
-version = "0.8.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.9.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "A collection of project templates and useful code snippets for single-cell data analysis with Scanpy."
 authors = ["Lukas Heumos <lukas.heumos@posteo.net>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/schillerlab/sc-toolbox"
 repository = "https://github.com/schillerlab/sc-toolbox"
 documentation = "https://sc-toolbox.readthedocs.io"
@@ -34,30 +34,30 @@
 adjustText = "^0.7.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
 coverage = {extras = ["toml"], version = "^5.3"}
 safety = "^1.9.0"
 mypy = "^0.812"
-typeguard = "^2.12.0"
+typeguard = "^2.12.1"
 xdoctest = {extras = ["colors"], version = "^0.15.0"}
 sphinx = ">=3.5.4"
 sphinx-autobuild = ">=2021.3.14"
 pre-commit = "^2.13.0"
 flake8 = ">=3.9.2"
-black = "^21.5b1"
+black = "^21.5b2"
 flake8-bandit = ">=2.1.2"
 flake8-bugbear = ">=21.4.3"
 flake8-docstrings = ">=1.5.0"
 flake8-rst-docstrings = ">=0.2.3"
 pep8-naming = ">=0.11.1"
 darglint = ">=1.5.8"
 pre-commit-hooks = "^4.0.1"
 sphinx-rtd-theme = ">=0.5.0"
-sphinx-rtd-dark-mode = "^1.2.1"
+sphinx-rtd-dark-mode = "^1.2.2"
 sphinx-click = ">=2.5.0"
 Pygments = ">=2.9.0"
 
 [tool.poetry.scripts]
 sc-toolbox = "sc_toolbox.__main__:main"
 
 [tool.black]
```

### Comparing `sc-toolbox-0.8.0/sc_toolbox/__main__.py` & `sc-toolbox-0.9.0/sc_toolbox/__main__.py`

 * *Files identical despite different names*

### Comparing `sc-toolbox-0.8.0/sc_toolbox/api/calc/__init__.py` & `sc-toolbox-0.9.0/sc_toolbox/api/calc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -445,14 +445,43 @@
 
     all_markers_df = pd.concat(all_markers)
     all_markers_df = all_markers_df[all_markers_df.pval_adj < qval_thresh].copy()
 
     return all_markers_df
 
 
+def generate_pseudobulk(adata: AnnData, group_key: str = "identifier", sep="\t", save: str = None) -> pd.DataFrame:
+    """
+    Generates a pseudobulk for a given key of groups in the AnnData object.
+    Looks like:
+      Genes    group_member_1    group_member_2
+    1 gene_1   value_1           value_2
+    2 gene_2   value_3           value_4
+
+    Args:
+        adata: AnnData object
+        group_key: The key to group by. E.g. by mice, by condition, ... (default: 'identifier')
+        sep: Separator to use when saving the pseudobulk table (default: '\t')
+        save: Path to save the pseudobulk table to (default: None)
+
+    Returns:
+        A Pandas DataFrame containing the pseudobulk table
+    """
+    pseudobulk = pd.DataFrame(data=adata.var_names.values, columns=["Genes"])
+
+    for i in adata.obs.loc[:, group_key].cat.categories:
+        temp = adata.obs.loc[:, group_key] == i
+        pseudobulk[i] = adata[temp].X.sum(0, dtype=int)  # column sums (genes)
+
+    if save:
+        pseudobulk.to_csv(save, sep=sep, index=False)
+
+    return pseudobulk
+
+
 def automated_marker_annotation(
     adata: AnnData,
     organism: str,
     tissue: str,
     marker_file: str,
     key: str = "rank_genes_groups",
     normalize: Optional[Literal["reference", "data"]] = "reference",
```

### Comparing `sc-toolbox-0.8.0/sc_toolbox/api/calc/markers/lung_particle_markers.txt` & `sc-toolbox-0.9.0/sc_toolbox/api/calc/markers/lung_particle_markers.txt`

 * *Files identical despite different names*

### Comparing `sc-toolbox-0.8.0/sc_toolbox/api/plot/__init__.py` & `sc-toolbox-0.9.0/sc_toolbox/api/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `sc-toolbox-0.8.0/sc_toolbox/api/util/__init__.py` & `sc-toolbox-0.9.0/sc_toolbox/api/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sc-toolbox-0.8.0/sc_toolbox/cli/commands/create.py` & `sc-toolbox-0.9.0/sc_toolbox/cli/commands/create.py`

 * *Files identical despite different names*

### Comparing `sc-toolbox-0.8.0/sc_toolbox/cli/commands/templates/simple_docker/{{ cookiecutter.project_slug }}/Dockerfile` & `sc-toolbox-0.9.0/sc_toolbox/cli/commands/templates/simple_docker/{{ cookiecutter.project_slug }}/Dockerfile`

 * *Files identical despite different names*

### Comparing `sc-toolbox-0.8.0/sc_toolbox/cli/commands/templates/simple_docker/{{ cookiecutter.project_slug }}/environment.yml` & `sc-toolbox-0.9.0/sc_toolbox/cli/commands/templates/simple_docker/{{ cookiecutter.project_slug }}/environment.yml`

 * *Files identical despite different names*

### Comparing `sc-toolbox-0.8.0/sc_toolbox/cli/commands/upgrade.py` & `sc-toolbox-0.9.0/sc_toolbox/cli/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `sc-toolbox-0.8.0/sc_toolbox/cli/questionary.py` & `sc-toolbox-0.9.0/sc_toolbox/cli/questionary.py`

 * *Files identical despite different names*

### Comparing `sc-toolbox-0.8.0/setup.py` & `sc-toolbox-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
  'typing-extensions>=3.10.0,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['sc-toolbox = sc_toolbox.__main__:main']}
 
 setup_kwargs = {
     'name': 'sc-toolbox',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'A collection of project templates and useful code snippets for single-cell data analysis with Scanpy.',
     'long_description': ".. image:: https://user-images.githubusercontent.com/21954664/116578141-65a85180-a911-11eb-9c33-925a2ec600c6.png\n    :target: https://github.com/schillerlab/sc-toolbox\n    :alt: sc-toolbox logo\n    :align: center\n    :width: 200px\n\n\nsc-toolbox\n==========\n\n|PyPI| |Downloads| |Python Version| |License| |Read the Docs| |Build| |Tests| |Codecov| |pre-commit| |Black|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/sc-toolbox.svg\n   :target: https://pypi.org/project/sc-toolbox/\n   :alt: PyPI\n.. |Downloads| image:: https://pepy.tech/badge/sc-toolbox\n    :target: https://pepy.tech/badge/sc-toolbox\n    :alt: PyPI Downloads\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/sc-toolbox\n   :target: https://pypi.org/project/sc-toolbox\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/github/license/schillerlab/sc-toolbox\n   :target: https://opensource.org/licenses/MIT\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/sc-toolbox/latest.svg?label=Read%20the%20Docs\n   :target: https://sc-toolbox.readthedocs.io/\n   :alt: Read the documentation at https://sc-toolbox.readthedocs.io/\n.. |Build| image:: https://github.com/schillerlab/sc-toolbox/workflows/Build%20sc-toolbox%20Package/badge.svg\n   :target: https://github.com/schillerlab/sc-toolbox/actions?workflow=Package\n   :alt: Build Package Status\n.. |Tests| image:: https://github.com/schillerlab/sc-toolbox/workflows/Run%20sc-toolbox%20Tests/badge.svg\n   :target: https://github.com/schillerlab/sc-toolbox/actions?workflow=Tests\n   :alt: Run Tests Status\n.. |Codecov| image:: https://codecov.io/gh/schillerlab/sc-toolbox/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/schillerlab/sc-toolbox\n   :alt: Codecov\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\n.. warning::\n    This package is still under heavy development. It is primarily designed for in-house analyses at the `Theislab <https://github.com/theislab>`_\n    and `Schillerlab <https://github.com/schillerlab>`_. Don't yet expect it to be well tested or documented.\n    However, contributions are highly welcome and we will provide guidance if required.\n\n\nFeatures\n--------\n\n* Create minimal best-practice containers for single-cell data analysis with Scanpy\n* API for advanced Scanpy based plots and analyses\n\n.. figure:: https://user-images.githubusercontent.com/21954664/116225631-5fb84200-a752-11eb-9489-16571428918f.png\n   :alt: Preview plot\n\n.. figure:: https://user-images.githubusercontent.com/21954664/116225765-824a5b00-a752-11eb-8cbf-c14ebd9ac030.png\n   :alt: Preview plot 2\n\n.. figure:: https://user-images.githubusercontent.com/21954664/116226005-c5a4c980-a752-11eb-9846-8dc72315d373.png\n   :alt: Preview plot 3\n\nInstallation\n------------\n\nYou can install *sc-toolbox* via pip_ from PyPI_:\n\n.. code:: console\n\n   $ pip install sc-toolbox\n\nUsage\n-----\n\n.. code:: python\n\n   import sc_toolbox.api as sct\n\nPlease see the `Usage documentation <Usage_>`_.\n\nCredits\n-------\n\nThis package was created with cookietemple_ using cookiecutter_ based on Hypermodern_Python_Cookiecutter_.\nMost scripts were developed by `Meshal Ansari <https://github.com/mesh09/>`_ and the package was designed by `Lukas Heumos <https://github.com/zethson>`_.\n\n.. _cookietemple: https://cookietemple.com\n.. _cookiecutter: https://github.com/audreyr/cookiecutter\n.. _MIT: http://opensource.org/licenses/MIT\n.. _PyPI: https://pypi.org/\n.. _Hypermodern_Python_Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n.. _pip: https://pip.pypa.io/\n.. _Usage: https://sc-toolbox.readthedocs.io/en/latest/usage.html\n.. _API: https://sc-toolbox.readthedocs.io/en/latest/api.html\n",
     'author': 'Lukas Heumos',
     'author_email': 'lukas.heumos@posteo.net',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/schillerlab/sc-toolbox',
```

### Comparing `sc-toolbox-0.8.0/PKG-INFO` & `sc-toolbox-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-toolbox
-Version: 0.8.0
+Version: 0.9.0
 Summary: A collection of project templates and useful code snippets for single-cell data analysis with Scanpy.
 Home-page: https://github.com/schillerlab/sc-toolbox
 License: MIT
 Author: Lukas Heumos
 Author-email: lukas.heumos@posteo.net
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: MIT License
```

