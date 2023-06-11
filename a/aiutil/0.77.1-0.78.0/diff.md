# Comparing `tmp/aiutil-0.77.1.tar.gz` & `tmp/aiutil-0.78.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiutil-0.77.1.tar", max compression
+gzip compressed data, was "aiutil-0.78.0.tar", max compression
```

## Comparing `aiutil-0.77.1.tar` & `aiutil-0.78.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0     1081 2023-01-10 05:37:50.308727 aiutil-0.77.1/LICENSE
--rw-r--r--   0        0        0       96 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/__init__.py
--rw-r--r--   0        0        0     1968 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/collections.py
--rw-r--r--   0        0        0    10716 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/cv.py
--rw-r--r--   0        0        0     3248 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/dataframe.py
--rw-r--r--   0        0        0     3501 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/datetime.py
--rw-r--r--   0        0        0     2092 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/dockerhub.py
--rw-r--r--   0        0        0    22905 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/filesystem.py
--rw-r--r--   0        0        0       81 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/hadoop/__init__.py
--rw-r--r--   0        0        0     9194 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/hadoop/hdfs.py
--rw-r--r--   0        0        0     5910 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/hadoop/kerberos.py
--rw-r--r--   0        0        0    18754 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/hadoop/log.py
--rw-r--r--   0        0        0     7473 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/hadoop/logf.py
--rw-r--r--   0        0        0    16000 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/hadoop/pyspark_submit.py
--rw-r--r--   0        0        0     1245 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/hadoop/pyspark_submit.yaml
--rw-r--r--   0        0        0     1450 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/hash.py
--rw-r--r--   0        0        0     3950 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/memory.py
--rw-r--r--   0        0        0        0 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/notebook/__init__.py
--rwxr-xr-x   0        0        0     7613 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/notebook/search.py
--rw-r--r--   0        0        0     2389 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/notebook/util.py
--rw-r--r--   0        0        0     1612 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/pdf.py
--rw-r--r--   0        0        0    10570 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/poetry.py
--rw-r--r--   0        0        0     1102 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/pypi.py
--rw-r--r--   0        0        0     2111 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/shebang.py
--rw-r--r--   0        0        0     4504 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/shell.py
--rw-r--r--   0        0        0      660 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/sql.py
--rw-r--r--   0        0        0      651 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/url.py
--rw-r--r--   0        0        0     1159 2023-01-10 05:37:50.308727 aiutil-0.77.1/aiutil/utils.py
--rw-r--r--   0        0        0     2547 2023-01-10 05:37:50.312727 aiutil-0.77.1/pyproject.toml
--rw-r--r--   0        0        0     1780 2023-01-10 05:37:50.312727 aiutil-0.77.1/readme.md
--rw-r--r--   0        0        0     3868 1970-01-01 00:00:00.000000 aiutil-0.77.1/setup.py
--rw-r--r--   0        0        0     3729 1970-01-01 00:00:00.000000 aiutil-0.77.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-11 22:53:53.604088 aiutil-0.78.0/LICENSE
+-rw-r--r--   0        0        0     1825 2023-06-11 22:53:53.604088 aiutil-0.78.0/README.md
+-rw-r--r--   0        0        0       96 2023-06-11 22:53:53.604088 aiutil-0.78.0/aiutil/__init__.py
+-rw-r--r--   0        0        0     1968 2023-06-11 22:53:53.604088 aiutil-0.78.0/aiutil/collections.py
+-rw-r--r--   0        0        0    10716 2023-06-11 22:53:53.604088 aiutil-0.78.0/aiutil/cv.py
+-rw-r--r--   0        0        0     3246 2023-06-11 22:53:53.604088 aiutil-0.78.0/aiutil/dataframe.py
+-rw-r--r--   0        0        0     3501 2023-06-11 22:53:53.604088 aiutil-0.78.0/aiutil/datetime.py
+-rw-r--r--   0        0        0     2092 2023-06-11 22:53:53.604088 aiutil-0.78.0/aiutil/dockerhub.py
+-rw-r--r--   0        0        0    22905 2023-06-11 22:53:53.604088 aiutil-0.78.0/aiutil/filesystem.py
+-rw-r--r--   0        0        0       81 2023-06-11 22:53:53.604088 aiutil-0.78.0/aiutil/hadoop/__init__.py
+-rw-r--r--   0        0        0     9194 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/hadoop/hdfs.py
+-rw-r--r--   0        0        0     5910 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/hadoop/kerberos.py
+-rw-r--r--   0        0        0    18754 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/hadoop/log.py
+-rw-r--r--   0        0        0     7473 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/hadoop/logf.py
+-rw-r--r--   0        0        0    16000 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/hadoop/pyspark_submit.py
+-rw-r--r--   0        0        0     1245 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/hadoop/pyspark_submit.yaml
+-rw-r--r--   0        0        0     1450 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/hash.py
+-rw-r--r--   0        0        0     3950 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/memory.py
+-rw-r--r--   0        0        0        0 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/notebook/__init__.py
+-rwxr-xr-x   0        0        0     9614 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/notebook/search.py
+-rw-r--r--   0        0        0     2337 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/notebook/util.py
+-rw-r--r--   0        0        0     1612 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/pdf.py
+-rw-r--r--   0        0        0    10562 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/poetry.py
+-rw-r--r--   0        0        0     1102 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/pypi.py
+-rw-r--r--   0        0        0     2111 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/shebang.py
+-rw-r--r--   0        0        0     4504 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/shell.py
+-rw-r--r--   0        0        0      660 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/sql.py
+-rw-r--r--   0        0        0      651 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/url.py
+-rw-r--r--   0        0        0     1159 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/utils.py
+-rw-r--r--   0        0        0     2508 2023-06-11 22:53:53.608088 aiutil-0.78.0/pyproject.toml
+-rw-r--r--   0        0        0     3773 1970-01-01 00:00:00.000000 aiutil-0.78.0/PKG-INFO
```

### Comparing `aiutil-0.77.1/LICENSE` & `aiutil-0.78.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/collections.py` & `aiutil-0.78.0/aiutil/collections.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/cv.py` & `aiutil-0.78.0/aiutil/cv.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/dataframe.py` & `aiutil-0.78.0/aiutil/dataframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Pandas DataFrame related utils.
 """
 from __future__ import annotations
 from typing import Union
 from pathlib import Path
 from loguru import logger
 import pandas as pd
-from pandas_profiling import ProfileReport
+from ydata_profiling import ProfileReport
 
 
 def table_2w(
     frame: Union[pd.DataFrame, pd.Series],
     columns: Union[str, list[str], None],
     na_as=None,
 ) -> pd.DataFrame:
@@ -48,15 +48,15 @@
         return pd.read_csv(path, **kwargs)
     return pd.concat(pd.read_csv(csv, **kwargs) for csv in path.glob("*.csv"))
 
 
 def dump_profile(
     df: Union[pd.DataFrame, str, Path], title: str, output_dir: Union[str, Path]
 ):
-    """Run pandas profiling on a DataFrame and dump the report into files.
+    """Run ydata-profiling on a DataFrame and dump the report into files.
 
     :param df: A pandas DataFrame.
     :param title: The title of the generated report.
     :param output_dir: The output directory for reports.
     :raises ValueError: If an input file other than Parquet/Pickle/CSV is provided.
     """
     if isinstance(df, str):
```

### Comparing `aiutil-0.77.1/aiutil/datetime.py` & `aiutil-0.78.0/aiutil/datetime.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/dockerhub.py` & `aiutil-0.78.0/aiutil/dockerhub.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/filesystem.py` & `aiutil-0.78.0/aiutil/filesystem.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/hadoop/hdfs.py` & `aiutil-0.78.0/aiutil/hadoop/hdfs.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/hadoop/kerberos.py` & `aiutil-0.78.0/aiutil/hadoop/kerberos.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/hadoop/log.py` & `aiutil-0.78.0/aiutil/hadoop/log.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/hadoop/logf.py` & `aiutil-0.78.0/aiutil/hadoop/logf.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/hadoop/pyspark_submit.py` & `aiutil-0.78.0/aiutil/hadoop/pyspark_submit.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/hadoop/pyspark_submit.yaml` & `aiutil-0.78.0/aiutil/hadoop/pyspark_submit.yaml`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/hash.py` & `aiutil-0.78.0/aiutil/hash.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/memory.py` & `aiutil-0.78.0/aiutil/memory.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/notebook/search.py` & `aiutil-0.78.0/aiutil/notebook/search.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,129 +1,175 @@
 #!/usr/bin/env python3
+"""Search Jupyter/Lab notebooks.
+"""
 from typing import TypeAlias, Sequence
 import json
 from pathlib import Path
 from collections import Counter
 from argparse import ArgumentParser, Namespace
 from loguru import logger
 
 Criterion: TypeAlias = str | list[str] | dict[str, list[str]]
 
 
 def _reg_criterion(criterion: str | list[str] | dict[str, list[str]]):
+    """Convert different criterion specification into universal dict specification."""
     if isinstance(criterion, str):
         if criterion == "":
             criterion = []
         else:
             criterion = [criterion]
     if isinstance(criterion, list):
         criterion = {"include": criterion, "exclude": []}
     return criterion
 
 
 class Cell:
+    """Class representing a cell in a notebook."""
+
     def __init__(self, cell: dict):
+        """Initialize a cell.
+        :param cell: A cell in the dict representation.
+        """
         self._cell = cell
         self._source = self.source(0)
 
-    def source(self, indent: int = 0):
+    def source(self, indent: int = 0) -> str:
+        """Get the source code in the cell.
+        :param indent: The number of spaces to add before each line of code.
+        """
         return "".join(" " * indent + line for line in self._cell["source"])
 
-    def match_keyword(self, keyword: Criterion):
+    def match_keyword(self, keyword: Criterion) -> bool:
+        """Match source code of this cell against the specified keyword criterion.
+        :param keyword: A keyword criterion.
+        """
         kwd = _reg_criterion(keyword)
         return all(k in self._source for k in kwd["include"]) and not any(
             k in self._source for k in kwd["exclude"]
         )
 
     def match_type(self, type_: str) -> bool:
+        """Match this cell's type against the specified one.
+        :param type_: The type of cell to match.
+        If empty, it matches all types.
+        """
         if type_ == "":
             return True
         return self._cell["cell_type"] == type_
 
 
 class Notebook:
+    """A class representing a Jupyter/Lab notebook."""
+
     def __init__(self, path: str | Path):
+        """Initialize a notebook.
+        :param path: The path to a notebook.
+        """
         self.path = Path(path) if isinstance(path, str) else path
         self._notebook = self._read_notebook()
         self.lang = self._get_lang().lower()
         self._cells = [Cell(cell) for cell in self._notebook["cells"]]
 
     def _get_lang(self) -> str:
+        """Get the language of the notebook."""
         if "metadata" not in self._notebook:
             return "python"
         metadata = self._notebook["metadata"]
         if "kernelspec" in metadata:
             kernelspec = metadata["kernelspec"]
             if "language" in kernelspec:
                 return kernelspec["language"]
             if "name" in kernelspec:
                 return kernelspec["name"]
         elif "language_info" in metadata:
             return metadata["language_info"]["name"]
         return "python"
 
     def _read_notebook(self) -> dict:
-        with self.path.open() as fin:
+        """Read the content of the notebook as a dict."""
+        with self.path.open(encoding="utf-8") as fin:
             return json.load(fin)
 
     def match_language(self, language: Criterion) -> bool:
+        """Match the language of the notebook against the specified language criterion.
+        :param language: A language criterion.
+        """
         lang = _reg_criterion(language)
         return all(self.lang == l.lower() for l in lang["include"]) and not any(
             self.lang == l.lower() for l in lang["exclude"]
         )
 
     def cells(self, keyword: Criterion, type_: str = "") -> list[Cell]:
+        """Get a list of cells in this notebook."""
         return [
             cell
             for cell in self._cells
             if cell.match_type(type_) and cell.match_keyword(keyword)
         ]
 
     def __repr__(self) -> str:
         return f"Notebook({self.path})"
 
 
 def print_nb_cells(
     nb_cells: tuple[tuple[Notebook, Cell], ...], num_notebooks: int, num_cells: int
 ):
+    """Print cells of notebooks.
+    :param nb_cells: Notebook cells to print.
+    :param num_notebooks: The max number of notebooks to print.
+    :param num_cells: The max number of cells per notebook to print.
+    """
     n = len(nb_cells)
     print(f"Matched {n} notebooks")
     print(
         f"Display {min(n, num_notebooks)} notebooks each with up to {num_cells} cells\n"
     )
     for nb, cells in nb_cells[:num_notebooks]:
         print(f"{nb.path}: {nb.lang}")
         for idx, cell in enumerate(cells[:num_cells]):
             print(
                 f"    ------------------------------------ Cell {idx} ------------------------------------"
             )
             print(cell.source(4))
         print(
-            f"========================================================================================\n\n"
+            "========================================================================================\n\n"
         )
 
 
 def search_notebooks(
     notebooks: list[Notebook],
     keyword: Criterion = "",
     type_: str = "",
     language: Criterion = "",
 ):
+    """Search notebooks using the specified criterions.
+    :param notebooks: A list of notebooks among which to search.
+    :param keyword: A keyword criterion.
+    :param type_: A type criterion.
+    :param language: A language criterion.
+    """
     notebooks = [nb for nb in notebooks if nb.match_language(language)]
     return tuple((nb, cells) for nb in notebooks if (cells := nb.cells(keyword, type_)))
 
 
 def list_languages(notebooks: list[Notebook]) -> list[tuple[str, int]]:
+    """List languages used in notebooks.
+    :param notebooks: A list of notebooks.
+    """
     counter = Counter(nb.lang for nb in notebooks)
     counter = list(counter.items())
     counter.sort(key=lambda t: -t[1])
     return counter
 
 
 def find_notebooks(paths: Sequence[str]) -> list[Notebook]:
+    """Find all notebooks under the given paths.
+    :param paths: A list of paths.
+    """
     notebooks = set()
     for path in paths:
         path = Path(path)
         if path.is_file():
             if path.suffix == ".ipynb":
                 notebooks.add(path)
             else:
@@ -153,15 +199,19 @@
         "exclude": args.kwd_exclude,
     }
     nb_cells = search_notebooks(notebooks, keyword=kwd, language=lang)
     print_nb_cells(nb_cells, args.num_notebooks, args.num_cells)
 
 
 def parse_args(args=None, namespace=None) -> Namespace:
-    """Parse command-line arguments."""
+    """Parse command-line arguments.
+    :param args: The arguments to parse.
+        If None, the arguments from command-line are parsed.
+    :param namespace: An inital Namespace object.
+    """
     parser = ArgumentParser(description="Search for notebooks.")
     subparsers = parser.add_subparsers(dest="sub_cmd", help="Sub commands.")
     _subparse_search(subparsers)
     _subparse_list(subparsers)
     return parser.parse_args(args=args, namespace=namespace)
```

### Comparing `aiutil-0.77.1/aiutil/notebook/util.py` & `aiutil-0.78.0/aiutil/notebook/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 #!/usr/bin/env python3
 """Jupyter/Lab notebooks related utils.
 """
-import os
 from typing import Union
 from pathlib import Path
 import subprocess as sp
 import itertools as it
-import tempfile
 import nbformat
-from loguru import logger
 from nbconvert import HTMLExporter
 
 HOME = Path.home()
 
 
 def nbconvert_notebooks(root_dir: Union[str, Path], cache: bool = False) -> None:
     """Convert all notebooks under a directory and its subdirectories using nbconvert.
```

### Comparing `aiutil-0.77.1/aiutil/pdf.py` & `aiutil-0.78.0/aiutil/pdf.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/poetry.py` & `aiutil-0.78.0/aiutil/poetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """This module makes it easy to work with poetry to managing your Python project.
 """
 from __future__ import annotations
 from typing import Optional, Union, Iterable
 from pathlib import Path
-import sys
 import os
 import shutil
 import subprocess as sp
 import toml
 from loguru import logger
 import git
 import pathspec
 from .filesystem import replace_patterns
 
 DIST = "dist"
-README = "readme.md"
+README = "README.md"
 TOML = "pyproject.toml"
 
 
 def _project_dir() -> Path:
     """Get the root directory of the Poetry project.
 
     :return: The root directory of the Poetry project.
@@ -49,15 +48,15 @@
     :param proj_dir: The root directory of the Poetry project.
     :return: Version of the project.
     """
     return toml.load(proj_dir / TOML)["tool"]["poetry"]["version"]
 
 
 def _update_version_readme(ver: str, proj_dir: Path) -> None:
-    """Update the version information in readme.
+    """Update the version information in README.md.
 
     :param ver: The new version.
     :param proj_dir: The root directory of the Poetry project.
     """
     replace_patterns(proj_dir / README, pattern=r"\d+\.\d+\.\d+", repl=f"{ver}")
```

### Comparing `aiutil-0.77.1/aiutil/pypi.py` & `aiutil-0.78.0/aiutil/pypi.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/shebang.py` & `aiutil-0.78.0/aiutil/shebang.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/shell.py` & `aiutil-0.78.0/aiutil/shell.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/sql.py` & `aiutil-0.78.0/aiutil/sql.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/url.py` & `aiutil-0.78.0/aiutil/url.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/aiutil/utils.py` & `aiutil-0.78.0/aiutil/utils.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.77.1/pyproject.toml` & `aiutil-0.78.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "aiutil"
-version = "0.77.1"
+version = "0.78.0"
 description = "A utils Python package for data scientists."
 authors = ["Benjamin Du <longendu@yahoo.com>"]
 license = "MIT"
-readme = "readme.md"
+readme = "README.md"
 repository = "https://github.com/legendu-net/aiutil"
 keywords = ["AI", "Machine Learning", "tools", "utils"]
 
 [tool.poetry.scripts]
 logf = "aiutil.hadoop:logf.main"
 repart_hdfs = "aiutil.hadoop:repart_hdfs.main"
 pyspark_submit = "aiutil.hadoop:pyspark_submit.main"
@@ -19,15 +19,15 @@
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 sqlparse = ">=0.4.1"
 pathspec = ">=0.8.1"
 dateparser = ">=0.7.1"
 numba = ">=0.53.0rc1.post1"
 pandas = ">=1.2.0"
-pandas-profiling = ">=2.9.0"
+ydata-profiling = ">=4.2.0"
 loguru = ">=0.3.2"
 toml = ">=0.10.0"
 GitPython = ">=3.0.0"
 notifiers = ">=1.2.1"
 PyYAML = ">=5.3.1"
 python-magic = ">=0.4.0"
 tqdm = ">=4.59.0"
@@ -56,18 +56,16 @@
 pdf = ["PyPDF2"]
 jupyter = ["nbformat", "nbconvert", "black"]
 admin = ["psutil"]
 all = ["opencv-python", "pillow", "docker", "networkx", "requests", "PyPDF2", "nbformat", "nbconvert", "black", "psutil"]
 
 [tool.poetry.group.dev.dependencies]
 pylint = ">=2.7.0"
-flake8 = ">=3.8.4"
-pytype = {git = "https://github.com/google/pytype.git"}
+#pytype = {git = "https://github.com/google/pytype.git"}
 darglint = ">=1.5.8"
-pyspark = ">=3.0.1"
 
 [tool.pylint.master]
 ignore = ".venv,.ipynb_checkpoints"
 unsafe-load-any-extension = "no"
 extension-pkg-whitelist = "numpy,cv2,pyspark"
 generated-members = "sqlite3.*,cv2.*,pyspark.*"
 ignored-modules = "pyspark.sql.functions"
```

### Comparing `aiutil-0.77.1/readme.md` & `aiutil-0.78.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,16 @@
         - Pythonic wrappers to the `hdfs` command.
         - A auto authentication tool for Kerberos.
         - An improved version of `spark_submit`.
         - Other misc PySpark functions. 
     
 ## Supported Operating Systems and Python Versions
 
-Python >= 3.10 on Linux, macOS and Windows.
+Python 3.10.x on Linux and macOS.
+It might work on Windows but is not tested on Windows.
 
 ## Installation
 
 ```bash
 pip3 install --user -U aiutil
 ```
 Use the following commands if you want to install all components of aiutil.
```

### Comparing `aiutil-0.77.1/PKG-INFO` & `aiutil-0.78.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiutil
-Version: 0.77.1
+Version: 0.78.0
 Summary: A utils Python package for data scientists.
 Home-page: https://github.com/legendu-net/aiutil
 License: MIT
 Keywords: AI,Machine Learning,tools,utils
 Author: Benjamin Du
 Author-email: longendu@yahoo.com
 Requires-Python: >=3.10,<3.11
@@ -28,25 +28,25 @@
 Requires-Dist: nbconvert (>=5.6.1) ; extra == "jupyter" or extra == "all"
 Requires-Dist: nbformat (>=5.0.7) ; extra == "jupyter" or extra == "all"
 Requires-Dist: networkx (>=2.5) ; extra == "docker" or extra == "all"
 Requires-Dist: notifiers (>=1.2.1)
 Requires-Dist: numba (>=0.53.0rc1.post1)
 Requires-Dist: opencv-python (>=4.0.0.0) ; extra == "cv" or extra == "all"
 Requires-Dist: pandas (>=1.2.0)
-Requires-Dist: pandas-profiling (>=2.9.0)
 Requires-Dist: pathspec (>=0.8.1)
 Requires-Dist: pillow (>=7.0.0) ; extra == "cv" or extra == "all"
 Requires-Dist: psutil (>=5.7.3) ; extra == "admin" or extra == "all"
 Requires-Dist: pytest (>=3.0)
 Requires-Dist: python-magic (>=0.4.0)
 Requires-Dist: requests (>=2.20.0) ; extra == "docker" or extra == "all"
 Requires-Dist: scikit-image (>=0.18.3)
 Requires-Dist: sqlparse (>=0.4.1)
 Requires-Dist: toml (>=0.10.0)
 Requires-Dist: tqdm (>=4.59.0)
+Requires-Dist: ydata-profiling (>=4.2.0)
 Project-URL: Repository, https://github.com/legendu-net/aiutil
 Description-Content-Type: text/markdown
 
 # [aiutil](https://github.com/legendu-net/aiutil): Data Science Utils
 
 This is a Python pacakage that contains misc utils for Data Science.
 
@@ -72,15 +72,16 @@
         - Pythonic wrappers to the `hdfs` command.
         - A auto authentication tool for Kerberos.
         - An improved version of `spark_submit`.
         - Other misc PySpark functions. 
     
 ## Supported Operating Systems and Python Versions
 
-Python >= 3.10 on Linux, macOS and Windows.
+Python 3.10.x on Linux and macOS.
+It might work on Windows but is not tested on Windows.
 
 ## Installation
 
 ```bash
 pip3 install --user -U aiutil
 ```
 Use the following commands if you want to install all components of aiutil.
```

