# Comparing `tmp/cr_pre_commit_hooks-0.1.0.tar.gz` & `tmp/cr_pre_commit_hooks-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cr_pre_commit_hooks-0.1.0.tar", max compression
+gzip compressed data, was "cr_pre_commit_hooks-0.1.1.tar", max compression
```

## Comparing `cr_pre_commit_hooks-0.1.0.tar` & `cr_pre_commit_hooks-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1465 2023-06-09 09:45:28.580454 cr_pre_commit_hooks-0.1.0/README.md
--rw-r--r--   0        0        0     3292 2023-06-09 09:45:28.576454 cr_pre_commit_hooks-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      268 2023-06-09 09:45:28.576454 cr_pre_commit_hooks-0.1.0/src/cr_pre_commit_hooks/__init__.py
--rw-r--r--   0        0        0     3123 2023-06-09 08:05:26.399044 cr_pre_commit_hooks-0.1.0/src/cr_pre_commit_hooks/docstrings.py
--rw-r--r--   0        0        0        0 2023-06-09 09:45:28.244453 cr_pre_commit_hooks-0.1.0/src/cr_pre_commit_hooks/py.typed
--rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 cr_pre_commit_hooks-0.1.0/setup.py
--rw-r--r--   0        0        0     2093 1970-01-01 00:00:00.000000 cr_pre_commit_hooks-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1541 2023-06-12 07:06:32.007091 cr_pre_commit_hooks-0.1.1/README.md
+-rw-r--r--   0        0        0     3292 2023-06-12 07:09:12.529479 cr_pre_commit_hooks-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      268 2023-06-12 07:06:32.007091 cr_pre_commit_hooks-0.1.1/src/cr_pre_commit_hooks/__init__.py
+-rw-r--r--   0        0        0     3282 2023-06-12 07:06:32.007091 cr_pre_commit_hooks-0.1.1/src/cr_pre_commit_hooks/docstrings.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:06:32.007091 cr_pre_commit_hooks-0.1.1/src/cr_pre_commit_hooks/py.typed
+-rw-r--r--   0        0        0     2169 1970-01-01 00:00:00.000000 cr_pre_commit_hooks-0.1.1/PKG-INFO
```

### Comparing `cr_pre_commit_hooks-0.1.0/pyproject.toml` & `cr_pre_commit_hooks-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.coverage.run]
 source = ["src"]
 branch = true
 
 [tool.poetry]
 name = "cr-pre-commit-hooks"
-version = "0.1.0"
+version = "0.1.1"
 description = "pre-commit hooks for ensuring consistency across our code base. Included are hooks which are not available elsewhere and also not super useful outside of a CR context."
 authors = ["Mika Pflüger <mika.pflueger@climate-resource.com>"]
 readme = "README.md"
 packages = [{include = "cr_pre_commit_hooks", from = "src"}]
 
 [tool.poetry.scripts]
 check-docstrings = 'cr_pre_commit_hooks.docstrings:main'
 
 [tool.commitizen]
-version = "0.1.0"
+version = "0.1.1"
 version_files = ["pyproject.toml:^version"]
 tag_format = "v$version"
 major_version_zero = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
 docstring-parser = "^0.15"
```

### Comparing `cr_pre_commit_hooks-0.1.0/src/cr_pre_commit_hooks/docstrings.py` & `cr_pre_commit_hooks-0.1.1/src/cr_pre_commit_hooks/docstrings.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,25 @@
 
 import docstring_parser
 
 
 def iter_docstrings(
     fname: typing.Union[str, pathlib.Path]
 ) -> collections.abc.Iterator[tuple[ast.FunctionDef, str]]:
-    """Yield all function docstrings in the given file."""
+    """Find all function's docstrings in the given file.
+
+    Parameters
+    ----------
+    fname
+        The file to parse.
+
+    Yields
+    ------
+        node, docstring. The function node and its docstring.
+    """
     with open(fname) as fd:
         code = ast.parse(fd.read())
     for node in ast.walk(code):
         if isinstance(node, ast.FunctionDef):
             docstring = ast.get_docstring(node)
             if docstring:
                 yield node, docstring
```

### Comparing `cr_pre_commit_hooks-0.1.0/setup.py` & `cr_pre_commit_hooks-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,62 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cr-pre-commit-hooks
+Version: 0.1.1
+Summary: pre-commit hooks for ensuring consistency across our code base. Included are hooks which are not available elsewhere and also not super useful outside of a CR context.
+Author: Mika Pflüger
+Author-email: mika.pflueger@climate-resource.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: docstring-parser (>=0.15,<0.16)
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# Climate Resource pre-commit hooks
 
-packages = \
-['cr_pre_commit_hooks']
+<!--- sec-begin-description -->
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['docstring-parser>=0.15,<0.16']
-
-entry_points = \
-{'console_scripts': ['check-docstrings = cr_pre_commit_hooks.docstrings:main']}
-
-setup_kwargs = {
-    'name': 'cr-pre-commit-hooks',
-    'version': '0.1.0',
-    'description': 'pre-commit hooks for ensuring consistency across our code base. Included are hooks which are not available elsewhere and also not super useful outside of a CR context.',
-    'long_description': '# Climate Resource pre-commit hooks\n\n<!--- sec-begin-description -->\n\n[pre-commit](https://pre-commit.com/) hooks for ensuring consistency across our code\nbase. Included are hooks which are not available elsewhere and also not super useful\noutside of a CR context.\n\n<!--- sec-end-description -->\n\n## Installation\n\n<!--- sec-begin-installation -->\n\nClimate Resource pre-commit hooks can be installed with pip:\n\n```bash\npip install cr-pre-commit-hooks\n```\n\n<!--- sec-end-installation -->\n\n### For developers\n\n<!--- sec-begin-installation-dev -->\n\nFor development, we rely on [poetry](https://python-poetry.org) for all our\ndependency management. To get started, you will need to make sure that poetry\nis installed\n([instructions here](https://python-poetry.org/docs/#installing-with-the-official-installer),\nwe found that pipx and pip worked better to install on a Mac).\n\nFor all of work, we use our `Makefile`.\nYou can read the instructions out and run the commands by hand if you wish,\nbut we generally discourage this because it can be error prone.\nIn order to create your environment, run `make virtual-environment`.\n\nIf there are any issues, the messages from the `Makefile` should guide you\nthrough. If not, please raise an issue in the [issue tracker][issue_tracker].\n\nFor the rest of our developer docs, please see [](development-reference).\n\n[issue_tracker]: https://gitlab.com/climate-resource/cr-pre-commit-hooks/issues\n\n<!--- sec-end-installation-dev -->\n',
-    'author': 'Mika Pflüger',
-    'author_email': 'mika.pflueger@climate-resource.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+[pre-commit](https://pre-commit.com/) hooks for ensuring consistency across our code
+base. Included are hooks which are not available elsewhere and also not super useful
+outside of a CR context.
 
+<!--- sec-end-description -->
+
+## Usage
+
+<!--- sec-begin-usage -->
+
+To use the hooks in a project, add to your `.pre-commit-config.yaml`:
+```yaml
+  - repo: https://gitlab.com/climate-resource/cr-pre-commit-hooks
+    rev: v0.1.0
+    hooks:
+      - id: check-docstrings
+```
+
+<!--- sec-end-usage -->
+
+## For developers
+
+<!--- sec-begin-installation-dev -->
+
+For development, we rely on [poetry](https://python-poetry.org) for all our
+dependency management. To get started, you will need to make sure that poetry
+is installed
+([instructions here](https://python-poetry.org/docs/#installing-with-the-official-installer),
+we found that pipx and pip worked better to install on a Mac).
+
+For all of work, we use our `Makefile`.
+You can read the instructions out and run the commands by hand if you wish,
+but we generally discourage this because it can be error prone.
+In order to create your environment, run `make virtual-environment`.
+
+If there are any issues, the messages from the `Makefile` should guide you
+through. If not, please raise an issue in the [issue tracker][issue_tracker].
+
+For the rest of our developer docs, please see [](development-reference).
+
+[issue_tracker]: https://gitlab.com/climate-resource/cr-pre-commit-hooks/issues
+
+<!--- sec-end-installation-dev -->
 
-setup(**setup_kwargs)
```

### Comparing `cr_pre_commit_hooks-0.1.0/PKG-INFO` & `cr_pre_commit_hooks-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,32 @@
-Metadata-Version: 2.1
-Name: cr-pre-commit-hooks
-Version: 0.1.0
-Summary: pre-commit hooks for ensuring consistency across our code base. Included are hooks which are not available elsewhere and also not super useful outside of a CR context.
-Author: Mika Pflüger
-Author-email: mika.pflueger@climate-resource.com
-Requires-Python: >=3.9,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: docstring-parser (>=0.15,<0.16)
-Description-Content-Type: text/markdown
-
 # Climate Resource pre-commit hooks
 
 <!--- sec-begin-description -->
 
 [pre-commit](https://pre-commit.com/) hooks for ensuring consistency across our code
 base. Included are hooks which are not available elsewhere and also not super useful
 outside of a CR context.
 
 <!--- sec-end-description -->
 
-## Installation
-
-<!--- sec-begin-installation -->
+## Usage
 
-Climate Resource pre-commit hooks can be installed with pip:
+<!--- sec-begin-usage -->
 
-```bash
-pip install cr-pre-commit-hooks
+To use the hooks in a project, add to your `.pre-commit-config.yaml`:
+```yaml
+  - repo: https://gitlab.com/climate-resource/cr-pre-commit-hooks
+    rev: v0.1.0
+    hooks:
+      - id: check-docstrings
 ```
 
-<!--- sec-end-installation -->
+<!--- sec-end-usage -->
 
-### For developers
+## For developers
 
 <!--- sec-begin-installation-dev -->
 
 For development, we rely on [poetry](https://python-poetry.org) for all our
 dependency management. To get started, you will need to make sure that poetry
 is installed
 ([instructions here](https://python-poetry.org/docs/#installing-with-the-official-installer),
@@ -53,8 +41,7 @@
 through. If not, please raise an issue in the [issue tracker][issue_tracker].
 
 For the rest of our developer docs, please see [](development-reference).
 
 [issue_tracker]: https://gitlab.com/climate-resource/cr-pre-commit-hooks/issues
 
 <!--- sec-end-installation-dev -->
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

