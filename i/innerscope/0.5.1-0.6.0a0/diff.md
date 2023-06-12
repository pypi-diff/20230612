# Comparing `tmp/innerscope-0.5.1.tar.gz` & `tmp/innerscope-0.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerscope-0.5.1.tar", last modified: Fri Jan 28 04:32:29 2022, max compression
+gzip compressed data, was "innerscope-0.6.0a0.tar", last modified: Mon Jun 12 17:51:19 2023, max compression
```

## Comparing `innerscope-0.5.1.tar` & `innerscope-0.6.0a0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 04:32:29.627033 innerscope-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-01-28 04:32:14.000000 innerscope-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-01-28 04:32:14.000000 innerscope-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5940 2022-01-28 04:32:29.627033 innerscope-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5024 2022-01-28 04:32:14.000000 innerscope-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 04:32:29.627033 innerscope-0.5.1/innerscope/
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-01-28 04:32:14.000000 innerscope-0.5.1/innerscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-01-28 04:32:29.627033 innerscope-0.5.1/innerscope/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-01-28 04:32:14.000000 innerscope-0.5.1/innerscope/cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)    32395 2022-01-28 04:32:14.000000 innerscope-0.5.1/innerscope/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 04:32:29.627033 innerscope-0.5.1/innerscope/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-28 04:32:14.000000 innerscope-0.5.1/innerscope/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-01-28 04:32:14.000000 innerscope-0.5.1/innerscope/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    17417 2022-01-28 04:32:14.000000 innerscope-0.5.1/innerscope/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     8785 2022-01-28 04:32:14.000000 innerscope-0.5.1/innerscope/tests/test_repr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 04:32:29.627033 innerscope-0.5.1/innerscope.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5940 2022-01-28 04:32:29.000000 innerscope-0.5.1/innerscope.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-01-28 04:32:29.000000 innerscope-0.5.1/innerscope.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-28 04:32:29.000000 innerscope-0.5.1/innerscope.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-01-28 04:32:29.000000 innerscope-0.5.1/innerscope.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-01-28 04:32:29.000000 innerscope-0.5.1/innerscope.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-01-28 04:32:14.000000 innerscope-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-01-28 04:32:29.627033 innerscope-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-01-28 04:32:14.000000 innerscope-0.5.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68449 2022-01-28 04:32:14.000000 innerscope-0.5.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:51:19.518545 innerscope-0.6.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-06-12 17:51:19.518545 innerscope-0.6.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:51:19.514544 innerscope-0.6.0a0/innerscope/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/innerscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/innerscope/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33653 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/innerscope/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:51:19.518545 innerscope-0.6.0a0/innerscope/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/innerscope/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/innerscope/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/innerscope/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/innerscope/tests/test_repr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:51:19.514544 innerscope-0.6.0a0/innerscope.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-06-12 17:51:19.000000 innerscope-0.6.0a0/innerscope.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-12 17:51:19.000000 innerscope-0.6.0a0/innerscope.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:51:19.000000 innerscope-0.6.0a0/innerscope.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 17:51:19.000000 innerscope-0.6.0a0/innerscope.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 17:51:19.000000 innerscope-0.6.0a0/innerscope.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 17:51:19.518545 innerscope-0.6.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/setup.py
```

### Comparing `innerscope-0.5.1/LICENSE` & `innerscope-0.6.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `innerscope-0.5.1/PKG-INFO` & `innerscope-0.6.0a0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,23 @@
-Metadata-Version: 2.1
-Name: innerscope
-Version: 0.5.1
-Summary: Expose the inner scope of functions
-Home-page: https://github.com/eriknw/innerscope
-Author: Erik Welch
-License: BSD
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Innerscope
 
-[![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%20PyPy-blue)](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%20PyPy-blue)
-[![Version](https://img.shields.io/pypi/v/innerscope.svg)](https://pypi.org/project/innerscope/)
+[![conda-forge](https://img.shields.io/conda/vn/conda-forge/innerscope.svg)](https://anaconda.org/conda-forge/innerscope)
+[![pypi](https://img.shields.io/pypi/v/innerscope.svg)](https://pypi.python.org/pypi/innerscope/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/innerscope)](https://pypi.python.org/pypi/innerscope/)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/eriknw/innerscope/blob/master/LICENSE)
-[![Build Status](https://github.com/eriknw/innerscope/workflows/Test/badge.svg)](https://github.com/eriknw/innerscope/actions)
-[![Coverage Status](https://coveralls.io/repos/eriknw/innerscope/badge.svg?branch=master)](https://coveralls.io/r/eriknw/innerscope)
-[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Tests](https://github.com/eriknw/innerscope/workflows/Test/badge.svg?branch=main)](https://github.com/eriknw/innerscope/actions)
+[![Coverage](https://coveralls.io/repos/eriknw/innerscope/badge.svg?branch=main)](https://coveralls.io/r/eriknw/innerscope)
 
 `innerscope` exposes the inner scope of functions and offers primitives suitable for creating pipelines.  It explores a design space around functions, dictionaries, and classes.
 
 **To install with pip:**
-- `pip install innerscope`
+`pip install innerscope`
+
 **To install with conda:**
-- `conda install -c conda-forge innerscope`
+`conda install -c conda-forge innerscope`
 
 A function can be made to act like a dictionary:
 ```python
 @innerscope.call
 def info():
     first_name = 'Erik'
     last_name = 'Welch'
@@ -150,10 +127,7 @@
 
 ## Why?
 It's all [@mrocklin's](https://github.com/mrocklin) fault for [asking a question.](https://github.com/dask/distributed/issues/4003)
 `innerscope` is exploring a data model that could be convenient for running code remotely with [dask.](https://dask.org)
 I bet it would even be useful for building pipelines with dask.  I'm sure there are other creative uses for it just waiting to be discovered. **Update:** and [`afar`](https://github.com/eriknw/afar) has been born!
 
 #### *This library is totally awesome and you should use it and tell all your friends* 😉 *!*
-
-
-
```

### Comparing `innerscope-0.5.1/innerscope/core.py` & `innerscope-0.6.0a0/innerscope/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,59 +2,81 @@
 import dis
 import functools
 import html
 import inspect
 import sys
 import warnings
 from collections.abc import Mapping
-from types import CodeType, FunctionType, MethodType
+from types import CellType, CodeType, FunctionType, MethodType
 
 from tlz import concatv, merge
 
 from . import cfg
 
-try:
-    # Added in Python 3.8
-    from types import CellType
-
-    def code_replace(code, *, co_code, co_names, co_stacksize):
-        return code.replace(
-            co_code=co_code,
-            co_names=co_names,
-            co_stacksize=co_stacksize,
+if sys.version_info < (3, 11):
+    NEW_CODE = (
+        bytes([dis.opmap["LOAD_GLOBAL"]])
+        + b"%b"
+        + bytes([dis.opmap["CALL_FUNCTION"], 0, dis.opmap["LOAD_GLOBAL"]])
+        + b"%b"
+        + bytes([dis.opmap["BUILD_TUPLE"], 3, dis.opmap["RETURN_VALUE"], 0])
+    )
+else:
+    NEW_CODE = (
+        bytes([dis.opmap["LOAD_GLOBAL"]])
+        + b"%b"
+        + bytes(
+            [
+                dis.opmap["CACHE"],
+                0,
+                dis.opmap["CACHE"],
+                0,
+                dis.opmap["CACHE"],
+                0,
+                dis.opmap["CACHE"],
+                0,
+                dis.opmap["CACHE"],
+                0,
+                dis.opmap["PRECALL"],
+                0,
+                dis.opmap["CACHE"],
+                0,
+                dis.opmap["CALL"],
+                0,
+                dis.opmap["CACHE"],
+                0,
+                dis.opmap["CACHE"],
+                0,
+                dis.opmap["CACHE"],
+                0,
+                dis.opmap["CACHE"],
+                0,
+                dis.opmap["LOAD_GLOBAL"],
+            ]
         )
-
-except ImportError:
-
-    def CellType(x):
-        def inner():  # pragma: no cover
-            return x
-
-        return inner.__closure__[0]
-
-    def code_replace(code, *, co_code, co_names, co_stacksize):
-        return CodeType(
-            code.co_argcount,
-            code.co_kwonlyargcount,
-            code.co_nlocals,
-            co_stacksize,
-            code.co_flags,
-            co_code,
-            code.co_consts,
-            co_names,
-            code.co_varnames,
-            code.co_filename,
-            code.co_name,
-            code.co_firstlineno,
-            code.co_lnotab,
-            code.co_freevars,
-            code.co_cellvars,
+        + b"%b"
+        + bytes(
+            [
+                dis.opmap["CACHE"],
+                0,
+                dis.opmap["CACHE"],
+                0,
+                dis.opmap["CACHE"],
+                0,
+                dis.opmap["CACHE"],
+                0,
+                dis.opmap["CACHE"],
+                0,
+                dis.opmap["BUILD_TUPLE"],
+                3,
+                dis.opmap["RETURN_VALUE"],
+                0,
+            ]
         )
-
-
+    )
 BUILTINS = set(dir(builtins))
 
 
 def _get_globals_recursive(func, *, seen=None, isclass=False):
     """Get all global names used by func and all functions and classes defined within it."""
     if isclass:
         global_names = set()
@@ -73,15 +95,20 @@
         }
     if seen is None:
         seen = set()
     num_classes = 0
     for inst in dis.get_instructions(func):
         if inst.opname == "LOAD_CONST" and type(inst.argval) is CodeType:
             if num_classes > 0:
-                code_inst = next(dis.get_instructions(inst.argval))
+                it = dis.get_instructions(inst.argval)
+                code_inst = next(it)
+                if code_inst.opname == "COPY_FREE_VARS":
+                    code_inst = next(it)
+                if code_inst.opname == "RESUME":
+                    code_inst = next(it)
                 isclass = code_inst.opname == "LOAD_NAME" and code_inst.argval == "__name__"
                 num_classes -= isclass
             if inst.argval in seen:  # pragma: no cover
                 # I don't know how to get into a recursive cycle, but let's prevent it anyway.
                 continue
             seen.add(inst.argval)
             global_names.update(_get_globals_recursive(inst.argval, seen=seen, isclass=isclass))
@@ -462,54 +489,48 @@
                     target_index -= 1
                     jump_target = return_indices[target_index]
                     target = jump_target - i - 2
                 if target_index == 0 or target > 255 or target < 0:
                     break
                 co_code, chunk = co_code[:i], co_code[i + 2 :]
                 chunks.append(chunk)
-                if sys.version_info.minor >= 10:
+                if sys.version_info >= (3, 10):
                     target //= 2  # :crossed_fingers:
                 chunks.append(bytes([dis.opmap["JUMP_FORWARD"], target]))
             chunks.append(co_code)
             co_code = b"".join(reversed(chunks))
 
         # Modify to end with `return (rv, locals(), secret)`
-        co_names = code.co_names + ("_innerscope_locals_", "_innerscope_secret_")
-        co_code = co_code + bytes(
-            [
-                dis.opmap["LOAD_GLOBAL"],
-                len(code.co_names),
-                dis.opmap["CALL_FUNCTION"],
-                0,
-                dis.opmap["LOAD_GLOBAL"],
-                len(code.co_names) + 1,
-                dis.opmap["BUILD_TUPLE"],
-                3,
-                dis.opmap["RETURN_VALUE"],
-                0,
-            ]
-        )
+        co_names = (*code.co_names, "_innerscope_locals_", "_innerscope_secret_")
+        if sys.version_info < (3, 11):
+            new_code = NEW_CODE % (bytes([len(code.co_names)]), bytes([len(code.co_names) + 1]))
+        else:
+            new_code = NEW_CODE % (
+                bytes([2 * len(code.co_names) + 1]),
+                bytes([2 * len(code.co_names) + 2]),
+            )
+        co_code = co_code + new_code
 
         # stacksize must be at least 3, because we make a length three tuple
-        self._code = code_replace(
-            code,
+        self._code = code.replace(
             co_code=co_code,
             co_names=co_names,
             co_stacksize=max(code.co_stacksize, 3),
         )
 
     def __call__(self, *args, **kwargs):
         [scope] = self._call(args, kwargs)
         return scope
 
     def _call(self, args, kwargs):
         if self.missing:
             warnings.warn(
                 f"Undefined variables: {', '.join(repr(name) for name in self.missing)}.\n"
-                "Perhaps use `bind` method to assign values for these names before calling."
+                "Perhaps use `bind` method to assign values for these names before calling.",
+                stacklevel=2,
             )
         # Should we use builtins, builtins.__dict__, or self.func.__globals__['__builtins__']?
         outer_scope = self.outer_scope.copy()
         outer_scope["__builtins__"] = builtins
         outer_scope["_innerscope_locals_"] = locals
         outer_scope["_innerscope_secret_"] = secret = object()
         is_trace = self.method == "trace"
@@ -548,20 +569,28 @@
             if is_trace:
                 sys.settrace(trace_func)
             return_value = func(*args, **kwargs)
             if type(self) is ScopedGeneratorFunction:
                 return_value = yield from return_value
         except UnboundLocalError as exc:
             message = exc.args and exc.args[0] or ""
-            if (
-                isinstance(message, str)
-                and message.startswith("local variable ")
+            if isinstance(message, str) and (
+                message.startswith("local variable ")
                 and message.endswith(" referenced before assignment")
+                or message.startswith("cannot access local variable")
+                and message.endswith("where it is not associated with a value")
             ):
-                name = message[len("local variable ") : -len(" referenced before assignment")]
+                if message.startswith("local variable "):
+                    name = message[len("local variable ") : -len(" referenced before assignment")]
+                else:
+                    name = message[
+                        len("cannot access local variable ") : -len(
+                            "where it is not associated with a value"
+                        )
+                    ]
                 raise UnboundLocalError(
                     f"{message}.\n\n"
                     "This probably means you assigned to a local variable with the same name as a "
                     "variable in an outer scope that you meant to use.  This is, unfortunately, "
                     "a current limitation of `innerscope`.  Workarounds include:\n"
                     f"    - Pass {name} in as an argument to the function.\n"
                     f"    - Don't assign to {name}; use a different name for the local variable.\n"
```

### Comparing `innerscope-0.5.1/innerscope/tests/test_core.py` & `innerscope-0.6.0a0/innerscope/tests/test_core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-import builtins
 import pickle
 
 import pytest
-from pytest import raises, warns
 
 import innerscope
 from innerscope import cfg, scoped_function
 
 global_x = 1
 hex = 1  # shadow a builtin
 
 
+def test_version():
+    assert innerscope.__version__ >= "0.5"
+
+
 def test_no_args():
     @scoped_function
     def f1():
         a = 1
         b = a + 1
 
     assert not f1.missing
@@ -34,17 +36,16 @@
         assert scope2 == dict(b=2, c=3)
 
     check(innerscope.bindwith(b=2)(f2))
     check(innerscope.bindwith({"b": 2})(f2))
 
     sf2 = scoped_function(f2)
     assert sf2.missing == {"b"}
-    with warns(UserWarning, match="Undefined variables: 'b'"):
-        with raises(NameError):
-            sf2()
+    with pytest.warns(UserWarning, match="Undefined variables: 'b'"), pytest.raises(NameError):
+        sf2()
 
     check(sf2.bind(b=2))
     check(sf2.bind({"b": 2}))
     check(sf2.bind(scope1))
     check(scope1.bindto(sf2))
     check(scope1.bindto(sf2.func))
     check(scoped_function(sf2, scope1))
@@ -68,17 +69,17 @@
 
     def check(scope2):
         assert scope2 == dict(b=2, c=3)
 
     check(scope1.call(f2))
     check(scope1.callwith()(f2))
 
-    with raises(TypeError, match="missing 1 required positional"):
+    with pytest.raises(TypeError, match="missing 1 required positional"):
         scope1.call()
-    with raises(TypeError, match="missing 1 required positional"):
+    with pytest.raises(TypeError, match="missing 1 required positional"):
         innerscope.call()
 
 
 def test_with_args():
     def f1(a):
         b = a + 1
 
@@ -220,15 +221,15 @@
 
 
 def test_raises_error():
     @scoped_function
     def f():
         1 / 0
 
-    with raises(ZeroDivisionError):
+    with pytest.raises(ZeroDivisionError):
         f()
 
 
 def test_return_values():
     @innerscope.call
     def f1():
         pass
@@ -258,15 +259,15 @@
     def f(boolean):
         if boolean:
             return 42
         a = 1
         b = a + 1
 
     # But we can check the return type
-    # with raises(ValueError, match="must return at the very end of the function"):
+    # with pytest.raises(ValueError, match="must return at the very end of the function"):
     #     f(True)
     scope = f(True)
     assert scope == {"boolean": True}
     assert scope.return_value == 42
 
     scope = f(False)
     assert scope == dict(a=1, b=2, boolean=False)
@@ -274,15 +275,15 @@
     @scoped_function
     def g(boolean):
         if boolean:
             return (1, 2, 3)
         a = 1
         b = a + 1
 
-    # with raises(ValueError, match="must return at the very end of the function"):
+    # with pytest.raises(ValueError, match="must return at the very end of the function"):
     #     g(True)
     scope = g(True)
     assert scope == {"boolean": True}
     assert scope.return_value == (1, 2, 3)
 
     scope = g(False)
     assert scope == dict(a=1, b=2, boolean=False)
@@ -299,24 +300,24 @@
         x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ;
         x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ;
         x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ;
         x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ;
         y = x
         return 2
 
-    if cfg.default_method == 'bytecode':
-        with raises(ValueError, match="The first return statement is too far away"):
+    if cfg.default_method == "bytecode":
+        with pytest.raises(ValueError, match="The first return statement is too far away"):
             f1(True)
-    if cfg.default_method == 'trace':
+    if cfg.default_method == "trace":
         scope = f1(True)
-        assert scope == {'x': 1, 'arg': True}
+        assert scope == {"x": 1, "arg": True}
         assert scope.return_value == 1
 
     scope = f1(False)
-    assert scope == {'arg': False,  'y': 1, 'x': 1}
+    assert scope == {"arg": False,  "y": 1, "x": 1}
     assert scope.return_value == 2
 
     @scoped_function
     def f2(arg):
         if arg == 0:
             return 1
         x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ;
@@ -327,22 +328,22 @@
         x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ;
         x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ;
         x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ;
         y = x
         return 3
 
     scope = f2(0)
-    assert scope == {'arg': 0, 'x': 1}
+    assert scope == {"arg": 0, "x": 1}
     assert scope.return_value == 1
 
     scope = f2(1)
-    assert scope == {'arg': 1, 'x': 1}
+    assert scope == {"arg": 1, "x": 1}
     assert scope.return_value == 2
     scope = f2(2)
-    assert scope == {'arg': 2, 'x': 1, 'y': 1}
+    assert scope == {"arg": 2, "x": 1, "y": 1}
     assert scope.return_value == 3
 
     @scoped_function
     def f3(arg):
         if arg == 0:
             return 1
         x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ;
@@ -356,31 +357,31 @@
         x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ;
         x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ; x ;
         if arg == 2:
             return 3
         y = x
         return 4
 
-    if cfg.default_method == 'bytecode':
-        with raises(ValueError, match="The first 2 return statements are too far away"):
+    if cfg.default_method == "bytecode":
+        with pytest.raises(ValueError, match="The first 2 return statements are too far away"):
             f3(0)
-        with raises(ValueError, match="The first 2 return statements are too far away"):
+        with pytest.raises(ValueError, match="The first 2 return statements are too far away"):
             f3(1)
-    if cfg.default_method == 'trace':
+    if cfg.default_method == "trace":
         scope = f3(0)
-        assert scope == {'arg': 0, 'x': 1}
+        assert scope == {"arg": 0, "x": 1}
         assert scope.return_value == 1
         scope = f3(1)
-        assert scope == {'arg': 1, 'x': 1}
+        assert scope == {"arg": 1, "x": 1}
         assert scope.return_value == (1, 2, 3)
     scope = f3(2)
-    assert scope == {'arg': 2, 'x': 1}
+    assert scope == {"arg": 2, "x": 1}
     assert scope.return_value == 3
     scope = f3(3)
-    assert scope == {'arg': 3, 'x': 1, 'y': 1}
+    assert scope == {"arg": 3, "x": 1, "y": 1}
     assert scope.return_value == 4
     # fmt: on
 
 
 # @pytest.mark.xfail(reason="Local variable can't yet be the same name as an outer variable")
 # This limitation may actually be okay to live with
 def test_inner_and_outer_variable():
@@ -390,24 +391,27 @@
     scope1 = innerscope.call(f1)
     assert scope1 == {"x": 1}
 
     @scope1.bindto
     def f2():
         x = x + 1  # pragma: no cover
 
-    with raises(
-        UnboundLocalError, match="local variable 'x' referenced before assignment.\n\nThis probably"
+    with pytest.raises(
+        UnboundLocalError,
+        match="local variable 'x' referenced before assignment.\n\nThis probably"
+        "|cannot access local variable 'x' where it is not associated with a value."
+        "\n\nThis probably",
     ):
         f2()
 
     @scoped_function
     def f3():
         raise UnboundLocalError("hahaha")
 
-    with raises(UnboundLocalError, match="hahaha$"):
+    with pytest.raises(UnboundLocalError, match="hahaha$"):
         f3()
 
 
 def test_default_args():
     @innerscope.callwith(0, z=3)
     def f(w, x=1, *args, y=2, z, **kwargs):
         pass
@@ -491,23 +495,23 @@
     assert scope["A"].z == 120
 
 
 def test_bad_method():
     def f():
         x = 1
 
-    with raises(ValueError, match="method= argument to ScopedFunc"):
+    with pytest.raises(ValueError, match="method= argument to ScopedFunc"):
         scoped_function(f, method="bad_method")
     old_default = cfg.default_method
     try:
         cfg.default_method = "bad_method"
-        with raises(ValueError, match="method= argument to ScopedFunc"):
+        with pytest.raises(ValueError, match="method= argument to ScopedFunc"):
             scoped_function(f)
         cfg.default_method = "default"
-        with raises(ValueError, match="silly"):
+        with pytest.raises(ValueError, match="silly"):
             scoped_function(f)
     finally:
         cfg.default_method = old_default
     assert innerscope.call(f) == {"x": 1}
 
 
 def test_generator():
@@ -532,23 +536,23 @@
     assert scope.return_value == 10
 
 
 def test_coroutine():
     async def f():  # pragma: no cover
         await 5
 
-    with raises(ValueError, match="does not yet work on coroutine functions"):
+    with pytest.raises(ValueError, match="does not yet work on coroutine functions"):
         scoped_function(f)
 
 
 def test_asyncgen():
     async def f():  # pragma: no cover
         yield 5
 
-    with raises(ValueError, match="does not yet work on async generator functions"):
+    with pytest.raises(ValueError, match="does not yet work on async generator functions"):
         scoped_function(f)
 
 
 def test_classmethod():
     class A:
         @scoped_function
         def f(self):
@@ -658,15 +662,15 @@
 
 def test_bad_type():
     def f(x):
         y = x + 1
         return y + 1
 
     cf = classmethod(f)
-    with raises(TypeError, match="expects a Python function"):
+    with pytest.raises(TypeError, match="expects a Python function"):
         scoped_function(cf)
     assert innerscope.call(f, 1) == {"x": 1, "y": 2}
 
 
 # Define globally so pickle can find it easily
 def global_func():
     a = 1
```

### Comparing `innerscope-0.5.1/innerscope/tests/test_repr.py` & `innerscope-0.6.0a0/innerscope/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `innerscope-0.5.1/innerscope.egg-info/PKG-INFO` & `innerscope-0.6.0a0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,83 @@
 Metadata-Version: 2.1
 Name: innerscope
-Version: 0.5.1
+Version: 0.6.0a0
 Summary: Expose the inner scope of functions
-Home-page: https://github.com/eriknw/innerscope
-Author: Erik Welch
-License: BSD
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Author: Innerscope contributors
+Author-email: Erik Welch <erik.n.welch@gmail.com>
+Maintainer-email: Erik Welch <erik.n.welch@gmail.com>
+License: Copyright (c) 2020 Erik Welch
+        
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+          a. Redistributions of source code must retain the above copyright notice,
+             this list of conditions and the following disclaimer.
+          b. Redistributions in binary form must reproduce the above copyright
+             notice, this list of conditions and the following disclaimer in the
+             documentation and/or other materials provided with the distribution.
+          c. Neither the name of innerscope nor the names of its contributors
+             may be used to endorse or promote products derived from this software
+             without specific prior written permission.
+        
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+        ARE DISCLAIMED. IN NO EVENT SHALL THE REGENTS OR CONTRIBUTORS BE LIABLE FOR
+        ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
+        LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
+        OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH
+        DAMAGE.
+        
+Project-URL: homepage, https://github.com/eriknw/innerscope
+Project-URL: repository, https://github.com/eriknw/innerscope
+Project-URL: changelog, https://github.com/eriknw/innerscope/releases
+Keywords: introspection,dict,utility,bytecode
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Other Audience
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # Innerscope
 
-[![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%20PyPy-blue)](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%20PyPy-blue)
-[![Version](https://img.shields.io/pypi/v/innerscope.svg)](https://pypi.org/project/innerscope/)
+[![conda-forge](https://img.shields.io/conda/vn/conda-forge/innerscope.svg)](https://anaconda.org/conda-forge/innerscope)
+[![pypi](https://img.shields.io/pypi/v/innerscope.svg)](https://pypi.python.org/pypi/innerscope/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/innerscope)](https://pypi.python.org/pypi/innerscope/)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/eriknw/innerscope/blob/master/LICENSE)
-[![Build Status](https://github.com/eriknw/innerscope/workflows/Test/badge.svg)](https://github.com/eriknw/innerscope/actions)
-[![Coverage Status](https://coveralls.io/repos/eriknw/innerscope/badge.svg?branch=master)](https://coveralls.io/r/eriknw/innerscope)
-[![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Tests](https://github.com/eriknw/innerscope/workflows/Test/badge.svg?branch=main)](https://github.com/eriknw/innerscope/actions)
+[![Coverage](https://coveralls.io/repos/eriknw/innerscope/badge.svg?branch=main)](https://coveralls.io/r/eriknw/innerscope)
 
 `innerscope` exposes the inner scope of functions and offers primitives suitable for creating pipelines.  It explores a design space around functions, dictionaries, and classes.
 
 **To install with pip:**
-- `pip install innerscope`
+`pip install innerscope`
+
 **To install with conda:**
-- `conda install -c conda-forge innerscope`
+`conda install -c conda-forge innerscope`
 
 A function can be made to act like a dictionary:
 ```python
 @innerscope.call
 def info():
     first_name = 'Erik'
     last_name = 'Welch'
@@ -150,10 +187,7 @@
 
 ## Why?
 It's all [@mrocklin's](https://github.com/mrocklin) fault for [asking a question.](https://github.com/dask/distributed/issues/4003)
 `innerscope` is exploring a data model that could be convenient for running code remotely with [dask.](https://dask.org)
 I bet it would even be useful for building pipelines with dask.  I'm sure there are other creative uses for it just waiting to be discovered. **Update:** and [`afar`](https://github.com/eriknw/afar) has been born!
 
 #### *This library is totally awesome and you should use it and tell all your friends* 😉 *!*
-
-
-
```

