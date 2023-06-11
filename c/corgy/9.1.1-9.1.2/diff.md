# Comparing `tmp/corgy-9.1.1.tar.gz` & `tmp/corgy-9.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corgy-9.1.1.tar", max compression
+gzip compressed data, was "corgy-9.1.2.tar", max compression
```

## Comparing `corgy-9.1.1.tar` & `corgy-9.1.2.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0    32171 2023-06-01 13:42:06.222186 corgy-9.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     1072 2023-06-01 13:42:06.222186 corgy-9.1.1/LICENSE
--rw-r--r--   0        0        0     4196 2023-06-01 13:42:06.222186 corgy-9.1.1/README.md
--rw-r--r--   0        0        0      468 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/__init__.py
--rw-r--r--   0        0        0     2329 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/_actions.py
--rw-r--r--   0        0        0      505 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/_annotations.py
--rw-r--r--   0        0        0    53646 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/_corgy.py
--rw-r--r--   0        0        0     3202 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/_corgychecker.py
--rw-r--r--   0        0        0     6237 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/_corgyparser.py
--rw-r--r--   0        0        0    37670 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/_helpfmt.py
--rw-r--r--   0        0        0    19746 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/_meta.py
--rw-r--r--   0        0        0       64 2023-06-01 13:42:46.770316 corgy-9.1.1/corgy/_version.py
--rw-r--r--   0        0        0        0 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/py.typed
--rw-r--r--   0        0        0     1598 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/types/__init__.py
--rw-r--r--   0        0        0     2382 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/types/_expand.py
--rw-r--r--   0        0        0     3750 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/types/_initargs.py
--rw-r--r--   0        0        0     2777 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/types/_inputfile.py
--rw-r--r--   0        0        0     5464 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/types/_keyvaluepairs.py
--rw-r--r--   0        0        0     5271 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/types/_outputfile.py
--rw-r--r--   0        0        0     9846 2023-06-01 13:42:06.226186 corgy-9.1.1/corgy/types/_subclass.py
--rw-r--r--   0        0        0    36201 2023-06-01 13:42:06.226186 corgy-9.1.1/docs/corgy.md
--rw-r--r--   0        0        0    11884 2023-06-01 13:42:06.226186 corgy-9.1.1/docs/corgy.types.md
--rw-r--r--   0        0        0      132 2023-06-01 13:42:06.226186 corgy-9.1.1/docs/index.md
--rw-r--r--   0        0        0     2697 2023-06-01 13:42:46.770316 corgy-9.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/__init__.py
--rw-r--r--   0        0        0    94529 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/test_corgy.py
--rw-r--r--   0        0        0     4753 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/test_corgychecker.py
--rw-r--r--   0        0        0    20305 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/test_corgyparser.py
--rw-r--r--   0        0        0      800 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/test_doctests.py
--rw-r--r--   0        0        0    49021 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/test_helpfmt.py
--rw-r--r--   0        0        0        0 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/__init__.py
--rw-r--r--   0        0        0      328 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/_pklclasses.py
--rw-r--r--   0        0        0     2002 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/_specialtmps.py
--rw-r--r--   0        0        0     3356 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/_test_file.py
--rw-r--r--   0        0        0     2678 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/test_initargs.py
--rw-r--r--   0        0        0     2496 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/test_inputfiles.py
--rw-r--r--   0        0        0     5443 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/test_keyvaluepairs.py
--rw-r--r--   0        0        0     5122 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/test_outputfiles.py
--rw-r--r--   0        0        0     7082 2023-06-01 13:42:06.226186 corgy-9.1.1/tests/types/test_subclass.py
--rw-r--r--   0        0        0     5497 1970-01-01 00:00:00.000000 corgy-9.1.1/PKG-INFO
+-rw-r--r--   0        0        0    32262 2023-06-11 23:23:51.214913 corgy-9.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1077 2023-06-11 23:23:51.214913 corgy-9.1.2/LICENSE
+-rw-r--r--   0        0        0     4020 2023-06-11 23:23:51.214913 corgy-9.1.2/README.md
+-rw-r--r--   0        0        0      468 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/__init__.py
+-rw-r--r--   0        0        0     2329 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/_actions.py
+-rw-r--r--   0        0        0      505 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/_annotations.py
+-rw-r--r--   0        0        0    53646 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/_corgy.py
+-rw-r--r--   0        0        0     3202 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/_corgychecker.py
+-rw-r--r--   0        0        0     6237 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/_corgyparser.py
+-rw-r--r--   0        0        0    37670 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/_helpfmt.py
+-rw-r--r--   0        0        0    19746 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/_meta.py
+-rw-r--r--   0        0        0       64 2023-06-11 23:24:33.410706 corgy-9.1.2/corgy/_version.py
+-rw-r--r--   0        0        0        0 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/py.typed
+-rw-r--r--   0        0        0     1598 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/types/__init__.py
+-rw-r--r--   0        0        0     2382 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/types/_expand.py
+-rw-r--r--   0        0        0     3750 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/types/_initargs.py
+-rw-r--r--   0        0        0     2777 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/types/_inputfile.py
+-rw-r--r--   0        0        0     5464 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/types/_keyvaluepairs.py
+-rw-r--r--   0        0        0     5271 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/types/_outputfile.py
+-rw-r--r--   0        0        0     9846 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/types/_subclass.py
+-rw-r--r--   0        0        0    36201 2023-06-11 23:23:51.214913 corgy-9.1.2/docs/corgy.md
+-rw-r--r--   0        0        0    11884 2023-06-11 23:23:51.214913 corgy-9.1.2/docs/corgy.types.md
+-rw-r--r--   0        0        0      132 2023-06-11 23:23:51.214913 corgy-9.1.2/docs/index.md
+-rw-r--r--   0        0        0       82 2023-06-11 23:23:51.214913 corgy-9.1.2/docs/www/usage/corgy.md
+-rw-r--r--   0        0        0      389 2023-06-11 23:23:51.214913 corgy-9.1.2/docs/www/usage/corgy.types.md
+-rw-r--r--   0        0        0     2801 2023-06-11 23:24:33.410706 corgy-9.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-11 23:23:51.214913 corgy-9.1.2/tests/__init__.py
+-rw-r--r--   0        0        0    94529 2023-06-11 23:23:51.214913 corgy-9.1.2/tests/test_corgy.py
+-rw-r--r--   0        0        0     4753 2023-06-11 23:23:51.214913 corgy-9.1.2/tests/test_corgychecker.py
+-rw-r--r--   0        0        0    20305 2023-06-11 23:23:51.214913 corgy-9.1.2/tests/test_corgyparser.py
+-rw-r--r--   0        0        0      800 2023-06-11 23:23:51.214913 corgy-9.1.2/tests/test_doctests.py
+-rw-r--r--   0        0        0    49021 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/test_helpfmt.py
+-rw-r--r--   0        0        0        0 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/__init__.py
+-rw-r--r--   0        0        0      328 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/_pklclasses.py
+-rw-r--r--   0        0        0     2002 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/_specialtmps.py
+-rw-r--r--   0        0        0     3356 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/_test_file.py
+-rw-r--r--   0        0        0     2678 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/test_initargs.py
+-rw-r--r--   0        0        0     2496 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/test_inputfiles.py
+-rw-r--r--   0        0        0     5443 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/test_keyvaluepairs.py
+-rw-r--r--   0        0        0     5122 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/test_outputfiles.py
+-rw-r--r--   0        0        0     7082 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/test_subclass.py
+-rw-r--r--   0        0        0     5321 1970-01-01 00:00:00.000000 corgy-9.1.2/PKG-INFO
```

### Comparing `corgy-9.1.1/CHANGELOG.md` & `corgy-9.1.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+### [9.1.2](https://github.com/jayanthkoushik/corgy/compare/v9.1.1...v9.1.2) (2023-06-11)
+
 ### [9.1.1](https://github.com/jayanthkoushik/corgy/compare/v9.1.0...v9.1.1) (2023-06-01)
 
 
 ### Bug Fixes
 
 * fallback to base formatting for subparsers in `CorgyHelpFormatter` ([87dede1](https://github.com/jayanthkoushik/corgy/commit/87dede132403735a584e2ed83de85b739877f86a))
```

### Comparing `corgy-9.1.1/LICENSE` & `corgy-9.1.2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Jayanth Koushik
+Copyright (c) 2021-2023 Jayanth Koushik
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `corgy-9.1.1/README.md` & `corgy-9.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+---
+title: Home
+---
 # corgy
 
 Corgy is a Python library that allows you to create feature rich data
 classes using intuitive type annotations.
 
 ```pycon
 >>> from typing import List
@@ -21,125 +24,125 @@
 ```
 
 ## Features
 
 * **Type checking**: `Corgy` instances are type-checked, and support a
   number of type modifiers.
 
-  ```pycon
-  >>> from typing import Tuple
+```pycon
+>>> from typing import Tuple
+
+>>> class C(Corgy):
+...     x: int
+...     y: Tuple[int, int]
 
-  >>> class C(Corgy):
-  ...     x: int
-  ...     y: Tuple[int, int]
-
-  >>> C(x="1")
-  Traceback (most recent call last):
-      ...
-  ValueError: error setting `x`: invalid value for type '<class 'int'>': '1'
-
-  >>> C(y=(1, 2, 3))
-  Traceback (most recent call last):
-      ...
-  ValueError: error setting `y`: invalid value for type 'typing.Tuple[int, int]': (1, 2, 3): expected exactly '2' elements
+>>> C(x="1")
+Traceback (most recent call last):
+    ...
+ValueError: error setting `x`: invalid value for type '<class 'int'>': '1'
+
+>>> C(y=(1, 2, 3))
+Traceback (most recent call last):
+    ...
+ValueError: error setting `y`: invalid value for type 'typing.Tuple[int, int]': (1, 2, 3): expected exactly '2' elements
 
-  ```
+```
 
 * **Dictionary interface**: `Corgy` instances can be converted to/from
   dictionaries.
 
-  ```pycon
-  >>> class G(Corgy):
-  ...     x: int
-
-  >>> class C(Corgy):
-  ...     x: int
-  ...     g: G
-
-  >>> g = G.from_dict({"x": 1})
-  >>> g
-  G(x=1)
-
-  >>> c = C(x=2, g=g)
-  >>> c.as_dict()
-  {'x': 2, 'g': {'x': 1}}
+```pycon
+>>> class G(Corgy):
+...     x: int
 
-  ```
+>>> class C(Corgy):
+...     x: int
+...     g: G
+
+>>> g = G.from_dict({"x": 1})
+>>> g
+G(x=1)
+
+>>> c = C(x=2, g=g)
+>>> c.as_dict()
+{'x': 2, 'g': {'x': 1}}
+
+```
 
 * **Command-line parsing**: `Corgy` class attributes can be added to an
   `ArgumentParser` instance, and parsed from the command-line. Help
   messages can be added to attributes with `Annotated`, and will be
   passed to the command line parser.
 
-  ```pycon
-  >>> from argparse import ArgumentParser
-  >>> from typing import Optional
-  >>> from typing_extensions import Annotated
-
-  >>> class ArgGroup(Corgy):
-  ...     arg1: Annotated[Optional[int], "optional number"]
-  ...     arg2: Annotated[bool, "a boolean"]
-
-  >>> class MyArgs(Corgy):
-  ...     arg1: Annotated[int, "a number"] = 1
-  ...     arg2: Annotated[Tuple[float, ...], "at least one float"]
-  ...     grp1: Annotated[ArgGroup, "group 1"]
-
-  >>> parser = ArgumentParser(usage="")
-  >>> MyArgs.add_args_to_parser(parser)
-  >>> parser.print_help()  # doctest: +SKIP
-  usage:
-
-  optional arguments:
-    -h, --help            show this help message and exit
-    --arg1 ARG1           a number
-    --arg2 ARG2 [ARG2 ...]
-                          at least one float
-
-  grp1:
-    group 1
-
-    --grp1:arg1 [GRP1:ARG1]
-                          optional number
-    --grp1:arg2, --no-grp1:arg2
-                          a boolean
+```pycon
+>>> from argparse import ArgumentParser
+>>> from typing import Optional
+>>> from typing_extensions import Annotated
+
+>>> class ArgGroup(Corgy):
+...     arg1: Annotated[Optional[int], "optional number"]
+...     arg2: Annotated[bool, "a boolean"]
+
+>>> class MyArgs(Corgy):
+...     arg1: Annotated[int, "a number"] = 1
+...     arg2: Annotated[Tuple[float, ...], "at least one float"]
+...     grp1: Annotated[ArgGroup, "group 1"]
+
+>>> parser = ArgumentParser(usage="")
+>>> MyArgs.add_args_to_parser(parser)
+>>> parser.print_help()  # doctest: +SKIP
+usage:
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --arg1 ARG1           a number
+  --arg2 ARG2 [ARG2 ...]
+                        at least one float
+
+grp1:
+  group 1
+
+  --grp1:arg1 [GRP1:ARG1]
+                        optional number
+  --grp1:arg2, --no-grp1:arg2
+                        a boolean
 
-  ```
+```
 
 * **Enhanced argparse formatting**: The `corgy` package provides
   `CorgyHelpFormatter`, a formatter class for `argparse`, with support
   for colorized output. It can also be used independent of `Corgy`
   classes.
 
-  ```pycon
-  >>> from corgy import CorgyHelpFormatter
+```pycon
+>>> from corgy import CorgyHelpFormatter
 
-  >>> # `ArgGroup` and `MyArgs` as defined above
-  >>> parser = ArgumentParser(usage="", formatter_class=CorgyHelpFormatter)
-  >>> MyArgs.add_args_to_parser(parser)
-  >>> parser.print_help()  # doctest: +SKIP
-  ```
+>>> # `ArgGroup` and `MyArgs` as defined above
+>>> parser = ArgumentParser(usage="", formatter_class=CorgyHelpFormatter)
+>>> MyArgs.add_args_to_parser(parser)
+>>> parser.print_help()  # doctest: +SKIP
+```
 
-    ![Sample argparse output with `CorgyHelpFormatter`](https://raw.githubusercontent.com/jayanthkoushik/corgy/44d0d2bdc225456e1d1d0ac78cfde26065f9b86f/example.svg)
+  ![Sample argparse output with `CorgyHelpFormatter`](https://raw.githubusercontent.com/jayanthkoushik/corgy/44d0d2bdc225456e1d1d0ac78cfde26065f9b86f/example.svg)
 
 * **Convenience types**: `corgy.types` provides a number of types for
   converting strings into objects like paths, dictionaries, classes,
   etc. These can be used standalone, but are especially useful for
   parsing from command line arguments. Refer to the docs for details on
   all available types. A small example is shown below.
 
-  ```pycon
-  >>> T = KeyValuePairs[str, int]
-  >>> m = T("x=1,y=2")
-  >>> print(m)
-  {'x': 1, 'y': 2}
+```pycon
+>>> T = KeyValuePairs[str, int]
+>>> m = T("x=1,y=2")
+>>> print(m)
+{'x': 1, 'y': 2}
 
-  ```
+```
 
-# Install
+## Install
 `corgy` is available on PyPI, and can be installed with pip:
 
 ```bash
 pip install corgy
 ```
 
 Support for colorized output requires the `crayons` package, also
@@ -153,10 +156,7 @@
 Parsing `Corgy` objects from `toml` files requires the `tomli` package
 on Python versions below 3.11. This can be installed automatically with
 the `toml` extra:
 
 ```bash
 pip install corgy[toml]
 ```
-
-# Usage
-For documentation on usage, refer to docs/index.md.
```

### Comparing `corgy-9.1.1/corgy/_actions.py` & `corgy-9.1.2/corgy/_actions.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/corgy/_corgy.py` & `corgy-9.1.2/corgy/_corgy.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/corgy/_corgychecker.py` & `corgy-9.1.2/corgy/_corgychecker.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/corgy/_corgyparser.py` & `corgy-9.1.2/corgy/_corgyparser.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/corgy/_helpfmt.py` & `corgy-9.1.2/corgy/_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/corgy/_meta.py` & `corgy-9.1.2/corgy/_meta.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/corgy/types/__init__.py` & `corgy-9.1.2/corgy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/corgy/types/_expand.py` & `corgy-9.1.2/corgy/types/_expand.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/corgy/types/_initargs.py` & `corgy-9.1.2/corgy/types/_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/corgy/types/_inputfile.py` & `corgy-9.1.2/corgy/types/_inputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/corgy/types/_keyvaluepairs.py` & `corgy-9.1.2/corgy/types/_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/corgy/types/_outputfile.py` & `corgy-9.1.2/corgy/types/_outputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/corgy/types/_subclass.py` & `corgy-9.1.2/corgy/types/_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/docs/corgy.md` & `corgy-9.1.2/docs/corgy.md`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/docs/corgy.types.md` & `corgy-9.1.2/docs/corgy.types.md`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/pyproject.toml` & `corgy-9.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "corgy"
-version = "9.1.1"  # managed by `poetry-dynamic-versioning`
+version = "9.1.2"  # managed by `poetry-dynamic-versioning`
 description = "Elegant data classes"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jayanthkoushik/corgy"
 packages = [
   { include = "corgy" },
@@ -47,14 +47,17 @@
 pylint = "~2.13.0"
 pre-commit = "^2.0"
 isort = "^5.1"
 mypy = "~1.1.0"
 pydocstyle = "^6.1"
 sphinx = "^4.2"
 sphinx-markdown-builder = { git = "https://github.com/clayrisser/sphinx-markdown-builder" }
+mkdocstrings = { extras = ["python"], version = "^0.22.0" }
+mkdocs-material = "^9.1.15"
+mike = "^1.1.2"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poetry-dynamic-versioning.substitution]
```

### Comparing `corgy-9.1.1/tests/test_corgy.py` & `corgy-9.1.2/tests/test_corgy.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/tests/test_corgychecker.py` & `corgy-9.1.2/tests/test_corgychecker.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/tests/test_corgyparser.py` & `corgy-9.1.2/tests/test_corgyparser.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/tests/test_doctests.py` & `corgy-9.1.2/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/tests/test_helpfmt.py` & `corgy-9.1.2/tests/test_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/tests/types/_specialtmps.py` & `corgy-9.1.2/tests/types/_specialtmps.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/tests/types/_test_file.py` & `corgy-9.1.2/tests/types/_test_file.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/tests/types/test_initargs.py` & `corgy-9.1.2/tests/types/test_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/tests/types/test_inputfiles.py` & `corgy-9.1.2/tests/types/test_inputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/tests/types/test_keyvaluepairs.py` & `corgy-9.1.2/tests/types/test_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/tests/types/test_outputfiles.py` & `corgy-9.1.2/tests/types/test_outputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/tests/types/test_subclass.py` & `corgy-9.1.2/tests/types/test_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.1/PKG-INFO` & `corgy-9.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corgy
-Version: 9.1.1
+Version: 9.1.2
 Summary: Elegant data classes
 Home-page: https://github.com/jayanthkoushik/corgy
 License: MIT
 Keywords: data classes,argparse,argument parsing,command line parsing,cli
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.7,<4.0
@@ -25,14 +25,17 @@
 Provides-Extra: toml
 Requires-Dist: crayons (>=0.4.0,<0.5.0) ; extra == "colors"
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; (python_version < "3.11") and (extra == "toml")
 Requires-Dist: typing_extensions (>=4.0,<5.0) ; python_version < "3.11"
 Project-URL: Repository, https://github.com/jayanthkoushik/corgy
 Description-Content-Type: text/markdown
 
+---
+title: Home
+---
 # corgy
 
 Corgy is a Python library that allows you to create feature rich data
 classes using intuitive type annotations.
 
 ```pycon
 >>> from typing import List
@@ -52,125 +55,125 @@
 ```
 
 ## Features
 
 * **Type checking**: `Corgy` instances are type-checked, and support a
   number of type modifiers.
 
-  ```pycon
-  >>> from typing import Tuple
+```pycon
+>>> from typing import Tuple
+
+>>> class C(Corgy):
+...     x: int
+...     y: Tuple[int, int]
 
-  >>> class C(Corgy):
-  ...     x: int
-  ...     y: Tuple[int, int]
-
-  >>> C(x="1")
-  Traceback (most recent call last):
-      ...
-  ValueError: error setting `x`: invalid value for type '<class 'int'>': '1'
-
-  >>> C(y=(1, 2, 3))
-  Traceback (most recent call last):
-      ...
-  ValueError: error setting `y`: invalid value for type 'typing.Tuple[int, int]': (1, 2, 3): expected exactly '2' elements
+>>> C(x="1")
+Traceback (most recent call last):
+    ...
+ValueError: error setting `x`: invalid value for type '<class 'int'>': '1'
+
+>>> C(y=(1, 2, 3))
+Traceback (most recent call last):
+    ...
+ValueError: error setting `y`: invalid value for type 'typing.Tuple[int, int]': (1, 2, 3): expected exactly '2' elements
 
-  ```
+```
 
 * **Dictionary interface**: `Corgy` instances can be converted to/from
   dictionaries.
 
-  ```pycon
-  >>> class G(Corgy):
-  ...     x: int
-
-  >>> class C(Corgy):
-  ...     x: int
-  ...     g: G
-
-  >>> g = G.from_dict({"x": 1})
-  >>> g
-  G(x=1)
-
-  >>> c = C(x=2, g=g)
-  >>> c.as_dict()
-  {'x': 2, 'g': {'x': 1}}
+```pycon
+>>> class G(Corgy):
+...     x: int
 
-  ```
+>>> class C(Corgy):
+...     x: int
+...     g: G
+
+>>> g = G.from_dict({"x": 1})
+>>> g
+G(x=1)
+
+>>> c = C(x=2, g=g)
+>>> c.as_dict()
+{'x': 2, 'g': {'x': 1}}
+
+```
 
 * **Command-line parsing**: `Corgy` class attributes can be added to an
   `ArgumentParser` instance, and parsed from the command-line. Help
   messages can be added to attributes with `Annotated`, and will be
   passed to the command line parser.
 
-  ```pycon
-  >>> from argparse import ArgumentParser
-  >>> from typing import Optional
-  >>> from typing_extensions import Annotated
-
-  >>> class ArgGroup(Corgy):
-  ...     arg1: Annotated[Optional[int], "optional number"]
-  ...     arg2: Annotated[bool, "a boolean"]
-
-  >>> class MyArgs(Corgy):
-  ...     arg1: Annotated[int, "a number"] = 1
-  ...     arg2: Annotated[Tuple[float, ...], "at least one float"]
-  ...     grp1: Annotated[ArgGroup, "group 1"]
-
-  >>> parser = ArgumentParser(usage="")
-  >>> MyArgs.add_args_to_parser(parser)
-  >>> parser.print_help()  # doctest: +SKIP
-  usage:
-
-  optional arguments:
-    -h, --help            show this help message and exit
-    --arg1 ARG1           a number
-    --arg2 ARG2 [ARG2 ...]
-                          at least one float
-
-  grp1:
-    group 1
-
-    --grp1:arg1 [GRP1:ARG1]
-                          optional number
-    --grp1:arg2, --no-grp1:arg2
-                          a boolean
+```pycon
+>>> from argparse import ArgumentParser
+>>> from typing import Optional
+>>> from typing_extensions import Annotated
+
+>>> class ArgGroup(Corgy):
+...     arg1: Annotated[Optional[int], "optional number"]
+...     arg2: Annotated[bool, "a boolean"]
+
+>>> class MyArgs(Corgy):
+...     arg1: Annotated[int, "a number"] = 1
+...     arg2: Annotated[Tuple[float, ...], "at least one float"]
+...     grp1: Annotated[ArgGroup, "group 1"]
+
+>>> parser = ArgumentParser(usage="")
+>>> MyArgs.add_args_to_parser(parser)
+>>> parser.print_help()  # doctest: +SKIP
+usage:
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --arg1 ARG1           a number
+  --arg2 ARG2 [ARG2 ...]
+                        at least one float
+
+grp1:
+  group 1
+
+  --grp1:arg1 [GRP1:ARG1]
+                        optional number
+  --grp1:arg2, --no-grp1:arg2
+                        a boolean
 
-  ```
+```
 
 * **Enhanced argparse formatting**: The `corgy` package provides
   `CorgyHelpFormatter`, a formatter class for `argparse`, with support
   for colorized output. It can also be used independent of `Corgy`
   classes.
 
-  ```pycon
-  >>> from corgy import CorgyHelpFormatter
+```pycon
+>>> from corgy import CorgyHelpFormatter
 
-  >>> # `ArgGroup` and `MyArgs` as defined above
-  >>> parser = ArgumentParser(usage="", formatter_class=CorgyHelpFormatter)
-  >>> MyArgs.add_args_to_parser(parser)
-  >>> parser.print_help()  # doctest: +SKIP
-  ```
+>>> # `ArgGroup` and `MyArgs` as defined above
+>>> parser = ArgumentParser(usage="", formatter_class=CorgyHelpFormatter)
+>>> MyArgs.add_args_to_parser(parser)
+>>> parser.print_help()  # doctest: +SKIP
+```
 
-    ![Sample argparse output with `CorgyHelpFormatter`](https://raw.githubusercontent.com/jayanthkoushik/corgy/44d0d2bdc225456e1d1d0ac78cfde26065f9b86f/example.svg)
+  ![Sample argparse output with `CorgyHelpFormatter`](https://raw.githubusercontent.com/jayanthkoushik/corgy/44d0d2bdc225456e1d1d0ac78cfde26065f9b86f/example.svg)
 
 * **Convenience types**: `corgy.types` provides a number of types for
   converting strings into objects like paths, dictionaries, classes,
   etc. These can be used standalone, but are especially useful for
   parsing from command line arguments. Refer to the docs for details on
   all available types. A small example is shown below.
 
-  ```pycon
-  >>> T = KeyValuePairs[str, int]
-  >>> m = T("x=1,y=2")
-  >>> print(m)
-  {'x': 1, 'y': 2}
+```pycon
+>>> T = KeyValuePairs[str, int]
+>>> m = T("x=1,y=2")
+>>> print(m)
+{'x': 1, 'y': 2}
 
-  ```
+```
 
-# Install
+## Install
 `corgy` is available on PyPI, and can be installed with pip:
 
 ```bash
 pip install corgy
 ```
 
 Support for colorized output requires the `crayons` package, also
@@ -185,10 +188,7 @@
 on Python versions below 3.11. This can be installed automatically with
 the `toml` extra:
 
 ```bash
 pip install corgy[toml]
 ```
 
-# Usage
-For documentation on usage, refer to docs/index.md.
-
```

