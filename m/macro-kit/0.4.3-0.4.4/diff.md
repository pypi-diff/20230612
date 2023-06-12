# Comparing `tmp/macro-kit-0.4.3.tar.gz` & `tmp/macro_kit-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macro-kit-0.4.3.tar", last modified: Thu Jun  8 14:35:57 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `macro-kit-0.4.3.tar` & `macro_kit-0.4.4.tar`

### file list

```diff
@@ -1,38 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 14:35:57.778597 macro-kit-0.4.3/
--rw-rw-rw-   0        0        0     1546 2021-10-22 07:44:24.000000 macro-kit-0.4.3/LICENSE
--rw-rw-rw-   0        0        0     3907 2023-06-08 14:35:57.777600 macro-kit-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     3310 2021-12-15 12:07:35.000000 macro-kit-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 14:35:57.711391 macro-kit-0.4.3/macro_kit.egg-info/
--rw-rw-rw-   0        0        0     3907 2023-06-08 14:35:57.000000 macro-kit-0.4.3/macro_kit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      651 2023-06-08 14:35:57.000000 macro-kit-0.4.3/macro_kit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 14:35:57.000000 macro-kit-0.4.3/macro_kit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-08 14:35:57.000000 macro-kit-0.4.3/macro_kit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-08 14:35:57.000000 macro-kit-0.4.3/macro_kit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-08 14:35:57.757247 macro-kit-0.4.3/macrokit/
--rw-rw-rw-   0        0        0     1954 2023-06-02 12:49:04.000000 macro-kit-0.4.3/macrokit/__init__.py
--rw-rw-rw-   0        0        0   399422 2023-06-08 14:35:07.000000 macro-kit-0.4.3/macrokit/_symbol.c
--rw-rw-rw-   0        0        0     4829 2023-01-23 07:23:00.000000 macro-kit-0.4.3/macrokit/_symbol.py
--rw-rw-rw-   0        0        0   364851 2023-06-08 14:35:07.000000 macro-kit-0.4.3/macrokit/_validator.c
--rw-rw-rw-   0        0        0     3421 2023-06-08 14:08:03.000000 macro-kit-0.4.3/macrokit/_validator.py
--rw-rw-rw-   0        0        0  1205196 2023-06-08 14:35:07.000000 macro-kit-0.4.3/macrokit/ast.c
--rw-rw-rw-   0        0        0    16235 2023-06-08 14:16:54.000000 macro-kit-0.4.3/macrokit/ast.py
--rw-rw-rw-   0        0        0  1719807 2023-06-08 14:35:08.000000 macro-kit-0.4.3/macrokit/expression.c
--rw-rw-rw-   0        0        0    27744 2023-06-08 14:33:18.000000 macro-kit-0.4.3/macrokit/expression.py
--rw-rw-rw-   0        0        0   153095 2023-06-08 14:35:08.000000 macro-kit-0.4.3/macrokit/head.c
--rw-rw-rw-   0        0        0     1168 2023-06-08 14:02:23.000000 macro-kit-0.4.3/macrokit/head.py
-drwxrwxrwx   0        0        0        0 2023-06-08 14:35:57.762258 macro-kit-0.4.3/macrokit/ipython/
--rw-rw-rw-   0        0        0       65 2021-12-05 08:15:33.000000 macro-kit-0.4.3/macrokit/ipython/__init__.py
--rw-rw-rw-   0        0        0     1470 2022-01-12 15:01:21.000000 macro-kit-0.4.3/macrokit/ipython/magic.py
-drwxrwxrwx   0        0        0        0 2023-06-08 14:35:57.766278 macro-kit-0.4.3/macrokit/julia/
--rw-rw-rw-   0        0        0        0 2021-10-25 23:55:49.000000 macro-kit-0.4.3/macrokit/julia/__init__.py
--rw-rw-rw-   0        0        0     2457 2021-12-05 07:46:04.000000 macro-kit-0.4.3/macrokit/julia/translate.py
--rw-rw-rw-   0        0        0    33105 2023-01-23 07:23:00.000000 macro-kit-0.4.3/macrokit/macro.py
--rw-rw-rw-   0        0        0    10628 2023-05-09 02:09:18.000000 macro-kit-0.4.3/macrokit/mock.py
--rw-rw-rw-   0        0        0        0 2022-01-22 14:27:53.000000 macro-kit-0.4.3/macrokit/py.typed
--rw-rw-rw-   0        0        0     2825 2023-01-23 07:23:00.000000 macro-kit-0.4.3/macrokit/type_map.py
--rw-rw-rw-   0        0        0       42 2023-06-08 14:35:57.778597 macro-kit-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     3514 2023-06-08 11:44:06.000000 macro-kit-0.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 14:35:57.774600 macro-kit-0.4.3/tests/
--rw-rw-rw-   0        0        0    12073 2023-06-08 14:07:22.000000 macro-kit-0.4.3/tests/test_macrokit.py
--rw-rw-rw-   0        0        0     1234 2023-05-09 02:02:37.000000 macro-kit-0.4.3/tests/test_mock.py
--rw-rw-rw-   0        0        0     1501 2023-01-23 07:23:00.000000 macro-kit-0.4.3/tests/test_symbol.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/__init__.py
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/_symbol.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/_validator.py
+-rw-r--r--   0        0        0    17970 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/ast.py
+-rw-r--r--   0        0        0    32474 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/expression.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/head.py
+-rw-r--r--   0        0        0    33105 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/macro.py
+-rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/mock.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/py.typed
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/type_map.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/utils.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/ipython/__init__.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/ipython/magic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/julia/__init__.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 macro_kit-0.4.4/macrokit/julia/translate.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 macro_kit-0.4.4/.gitignore
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 macro_kit-0.4.4/LICENSE
+-rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 macro_kit-0.4.4/README.md
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 macro_kit-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 macro_kit-0.4.4/PKG-INFO
```

### Comparing `macro-kit-0.4.3/LICENSE` & `macro_kit-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `macro-kit-0.4.3/README.md` & `macro_kit-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 ## Installation
 
 - use pip
 
 ```
-pip install macro-kit
+pip install macro-kit -U
 ```
 
 - from source
 
 ```
 pip install git+https://github.com/hanjinliu/macro-kit
 ```
@@ -42,15 +42,15 @@
 ```
 
 Use `format` method to rename variable names.
 
 ```python
 # substitute identifiers of variables
 # var0x24fdc2d1530 -> x
-macro.format([(val0, "x")]) 
+macro.format([(val0, "x")])
 ```
 ```
 [Out]
 x = str_add(1, 2)
 var0x24fdc211df0 = str_add(x, 'xyz')
 ```
 
@@ -72,25 +72,25 @@
 ```python
 macro = Macro()
 
 @macro.record
 class C:
     def __init__(self, val: int):
         self.value = val
-    
+
     @property
     def value(self):
         return self._value
-    
+
     @value.setter
     def value(self, new_value: int):
         if not isinstance(new_value, int):
             raise TypeError("new_value must be an integer.")
         self._value = new_value
-    
+
     def show(self):
         print(self._value)
 
 c = C(1)
 c.value = 5
 c.value = -10
 c.show()
@@ -104,15 +104,15 @@
 
 ```python
 macro.format([(c, "ins")])
 ```
 ```
 [Out]
 ins = C(1)
-ins.value = -10     
+ins.value = -10
 var0x7ffed09d2cd8 = ins.show()
 ```
 
 `eval` can evaluate macro.
 
 ```python
 macro.eval({"C": C})
@@ -123,15 +123,15 @@
 ```
 
 3. Record module
 
 ```python
 import numpy as np
 macro = Macro()
-np = macro.record(np) # macro-recordable numpy
+np = macro.record(np)  # macro-recordable numpy
 
 arr = np.random.random(30)
 mean = np.mean(arr)
 
 macro
 ```
 ```
@@ -139,30 +139,30 @@
 var0x2a0a2864090 = numpy.random.random(30)
 var0x2a0a40daef0 = numpy.mean(var0x2a0a2864090)
 ```
 
 Recorded module is stored in `Symbol` so you can safely `eval` the macro without passing the module object as the global variables.
 
 ```python
-macro.eval() # this works
+macro.eval()  # this works
 ```
 
 4. String parsing
 
 `parse` calls `ast.parse` inside so that you can safely make `Expr` from string.
 
 ```python
 from macrokit import parse
 
 expr = parse("result = f(0, l[2:8])")
 expr
 ```
 ```
 [Out]
-:(result = f(0, l[slice(2, 8, None)])
+:(result = f(0, l[slice(2, 8, None)]))
 ```
 ```python
 print(expr.dump())
 ```
 ```
 [Out]
 head: assign
@@ -172,8 +172,8 @@
     args:
      0: f
      1: 0
      2: head: getitem
         args:
          0: l
          1: slice(2, 8, None)
-```
+```
```

### Comparing `macro-kit-0.4.3/macrokit/__init__.py` & `macro_kit-0.4.4/macrokit/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """macro-kit is a package for macro recording and metaprogramming in Python."""
 
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 __author__ = "Hanjin Liu"
 __email__ = "liuhanjin-sc@g.ecc.u-tokyo.ac.jp"
 
 from macrokit._symbol import Symbol
 from macrokit.expression import (
     Expr,
     Head,
@@ -16,16 +16,14 @@
 )
 from macrokit.macro import Macro, MacroFlags, BaseMacro
 from macrokit.mock import Mock
 from macrokit.ast import parse
 from macrokit.type_map import register_type, unregister_type, type_registered
 from functools import wraps
 
-from macrokit._symbol import COMPILED
-
 __all__ = [
     "Symbol",
     "Head",
     "Expr",
     "Macro",
     "BaseMacro",
     "Mock",
```

### Comparing `macro-kit-0.4.3/macrokit/_symbol.py` & `macro_kit-0.4.4/macrokit/_symbol.py`

 * *Files 16% similar despite different names*

```diff
@@ -135,18 +135,7 @@
 
     @classmethod
     def asvar(cls, obj: Any) -> "Symbol":
         """Convert input object as a variable."""
         out = Symbol(Symbol.make_symbol_str(obj), id(obj))
         out.constant = False
         return out
-
-
-try:
-    import cython
-except ImportError:  # pragma: no cover
-    COMPILED: bool = False
-else:  # pragma: no cover
-    try:
-        COMPILED = cython.compiled
-    except AttributeError:
-        COMPILED = False
```

### Comparing `macro-kit-0.4.3/macrokit/_validator.py` & `macro_kit-0.4.4/macrokit/_validator.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,16 @@
 @validator.register(Head.empty)
 def _no_arg(args):
     if len(args) != 0:
         raise ValidationError()
     return args
 
 
-@validator.register(Head.del_)
+@validator.register(Head.star)
+@validator.register(Head.starstar)
 def _single_arg(args):
     if len(args) != 1:
         raise ValidationError()
     return args
 
 
 @validator.register(Head.comment)
@@ -97,14 +98,15 @@
             raise ValidationError()
         k = Symbol.var(k.name)
     # here, annotated function call will be a list.
     return [k, v]
 
 
 @validator.register(Head.assign)
+@validator.register(Head.walrus)
 def _symbols_and_any(args):
     if len(args) != 2:
         raise ValidationError()
     k, v = args
     if isinstance(k, str):
         k = Symbol.var(k)
     elif isinstance(k, Symbol) and k.constant:
@@ -117,27 +119,27 @@
 def _three_args(args):
     if len(args) != 3:
         raise ValidationError()
     return args
 
 
 @validator.register(Head.function)
+@validator.register(Head.class_)
 @validator.register(Head.for_)
 @validator.register(Head.while_)
 def _an_arg_and_a_block(args):
     if len(args) != 2:
         raise ValidationError()
     b = args[1]
     if getattr(b, "head", None) != Head.block:
         raise ValidationError()
     return args
 
 
 @validator.register(Head.if_)
-@validator.register(Head.elif_)
 def _two_args_and_a_block(args):
     if len(args) != 3:
         raise ValidationError()
     b = args[2]
     if getattr(b, "head", None) != Head.block:
         raise ValidationError()
     return args
```

### Comparing `macro-kit-0.4.3/macrokit/ast.py` & `macro_kit-0.4.4/macrokit/ast.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import ast
 import inspect
-import sys
-from typing import Callable, Union, get_type_hints
+from typing import Any, Callable, Union, get_type_hints
 
-from macrokit.expression import Expr, Head, symbol, _STORED_VALUES
+from macrokit.expression import Expr, Head, symbol, _STORED_SYMBOLS
 from macrokit._symbol import Symbol
 
 
 NoneType = type(None)
 LAMBDA = Symbol._reserved("<lambda>")
 
 AST_BINOP_MAP = {
@@ -57,30 +56,33 @@
 
     out = from_ast(ast_object)
     if not squeeze and len(body) == 1:
         out = Expr(Head.block, [out])
     return out
 
 
+_ParseFunc = Callable[[Any], Union[Symbol, Expr]]
+
+
 class singledispatch:
     """Simplified version of functools.singledispatch."""
 
-    def __init__(self, func: Callable):
+    def __init__(self, func: _ParseFunc):
         self.func = func
-        self._registry: "dict[type, Callable]" = {}
+        self._registry: "dict[type, _ParseFunc]" = {}
 
     def __call__(self, *args, **kwargs):
         """Dispatch to the registered function for the type of the first argument."""
         try:
             f = self._registry[args[0].__class__]
         except KeyError:
             f = self.func
         return f(*args, **kwargs)
 
-    def register(self, func: Callable):
+    def register(self, func: _ParseFunc) -> _ParseFunc:
         """Register function as a handler for a specific type."""
         cls = next(iter(get_type_hints(func).values()))
         self._registry[cls] = func
         return func
 
 
 @singledispatch
@@ -95,50 +97,25 @@
 
 
 @from_ast.register
 def _expr(ast_object: ast.Expr):
     return from_ast(ast_object.value)
 
 
-if sys.version_info < (3, 8):
-
-    @from_ast.register
-    def _(ast_object: ast.Num):
-        return symbol(ast_object.n)
-
-    @from_ast.register
-    def _str(ast_object: ast.Str):
-        return symbol(ast_object.s)
-
-    @from_ast.register
-    def _name_constant(ast_object: ast.NameConstant):
-        return symbol(ast_object.n)
-
-    @from_ast.register
-    def _bytes(ast_object: ast.Bytes):
-        return symbol(ast_object.s)
-
-    @from_ast.register
-    def _ellipsis(ast_object: ast.Ellipsis):
-        return symbol(ast_object.s)
-
-else:
-
-    @from_ast.register
-    def _constant(ast_object: ast.Constant):
-        return symbol(ast_object.value)
+@from_ast.register
+def _constant(ast_object: ast.Constant):
+    return symbol(ast_object.value)
 
 
 @from_ast.register
 def _name(ast_object: ast.Name):
     name = ast_object.id
-    for sym, v in _STORED_VALUES.values():
-        if isinstance(sym, Symbol) and sym.name == name:
-            return symbol(v)
-    return Symbol(ast_object.id)
+    if name in _STORED_SYMBOLS:
+        return symbol(_STORED_SYMBOLS[name])
+    return Symbol(name)
 
 
 @from_ast.register
 def _unaryop(ast_object: ast.UnaryOp):
     return Expr(
         Head.unop, [AST_UNOP_MAP[type(ast_object.op)], from_ast(ast_object.operand)]
     )
@@ -274,15 +251,15 @@
     kwargs = [
         Expr(Head.kw, [from_ast(k), from_ast(v)])
         for k, v in zip(fargs.args[nargs:], fargs.defaults)
     ]
     return Expr(
         head,
         [
-            Expr(Head.call, [LAMBDA] + args + kwargs),  # type: ignore
+            Expr(Head.call, [LAMBDA] + args + kwargs),
             from_ast(ast_object.body),
         ],
     )
 
 
 @from_ast.register
 def _for(ast_object: ast.For):
@@ -294,14 +271,49 @@
     block = from_ast(ast_object.body)
     if ast_object.orelse:
         raise ValueError("'else' block is not supported yet")
     return Expr(head, [top, block])
 
 
 @from_ast.register
+def _try(ast_object: ast.Try):
+    head = Head.try_
+    args = [from_ast(ast_object.body)]
+    for k in ast_object.handlers:
+        args.extend(_except_to_list(k))
+    if ast_object.orelse:
+        args.append(from_ast(ast_object.orelse))
+    else:
+        args.append(Expr.empty())
+    if ast_object.finalbody:
+        args.append(from_ast(ast_object.finalbody))
+    else:
+        args.append(Expr.empty())
+
+    return Expr(head, args)
+
+
+def _except_to_list(ast_object: ast.ExceptHandler) -> "list[Symbol | Expr]":
+    if ast_object.type is not None:
+        if isinstance(ast_object.type, ast.Name):
+            type_: Symbol | Expr = Symbol(ast_object.type.id)
+        else:
+            type_ = symbol(ast_object.type)
+        if ast_object.name:
+            arg0: Symbol | Expr = Expr(Head.as_, [type_, Symbol(ast_object.name)])
+        else:
+            arg0 = type_
+    else:
+        arg0 = Expr.empty()
+
+    block = from_ast(ast_object.body)
+    return [arg0, block]
+
+
+@from_ast.register
 def _while(ast_object: ast.While):
     head = Head.while_
     test = from_ast(ast_object.test)
     block = from_ast(ast_object.body)
     if ast_object.orelse:
         raise ValueError("'else' block is not supported yet")
     return Expr(head, [test, block])
@@ -351,30 +363,52 @@
     head = Head.block
     args = [from_ast(k) for k in ast_object]
     return Expr(head, args)
 
 
 @from_ast.register
 def _function_def(ast_object: ast.FunctionDef):
-    # TODO: positional only etc. are not supported
     head = Head.function
+    _call_args: list[Symbol | Expr] = []
     fname = Symbol(ast_object.name)
+    _call_args.append(fname)
     fargs = ast_object.args
+    vararg = fargs.vararg
     nargs = len(fargs.args) - len(fargs.defaults)
-    args = [from_ast(k) for k in fargs.args[:nargs]]
-    kwargs = [
+    _call_args.extend(from_ast(k) for k in fargs.args[:nargs])  # args
+    if fargs.posonlyargs:
+        _call_args.insert(len(fargs.posonlyargs), Symbol._reserved("/"))
+    _call_args.extend(
         Expr(Head.kw, [from_ast(k), from_ast(v)])
         for k, v in zip(fargs.args[nargs:], fargs.defaults)
-    ]
+    )  # kwargs
+    if vararg is not None:  # *args
+        _input_expr = Expr(Head.star, [Symbol(vararg.arg)])
+        if vararg.annotation is not None:
+            _input_expr = Expr(
+                Head.annotate, [_input_expr, from_ast(vararg.annotation)]
+            )
+        _call_args.append(_input_expr)
+    if fargs.kwonlyargs:
+        _call_args.append(Symbol._reserved("*"))
+        _call_args.extend(
+            Expr(Head.kw, [from_ast(k), from_ast(v)])
+            for k, v in zip(fargs.kwonlyargs, fargs.kw_defaults)
+        )
+    if fargs.kwarg:  # **kwargs
+        _input_expr = Expr(Head.starstar, [Symbol(fargs.kwarg.arg)])
+        if fargs.kwarg.annotation is not None:
+            _input_expr = Expr(
+                Head.annotate, [_input_expr, from_ast(fargs.kwarg.annotation)]
+            )
+        _call_args.append(_input_expr)
+
     out = Expr(
         head,
-        [
-            Expr(Head.call, [fname] + args + kwargs),  # type: ignore
-            from_ast(ast_object.body),
-        ],
+        [Expr(Head.call, _call_args), from_ast(ast_object.body)],
     )
     for dec in ast_object.decorator_list:
         out = Expr(Head.decorator, [from_ast(dec), out])
 
     return out
 
 
@@ -424,15 +458,15 @@
     if ast_object.cause:
         args.append(Expr(Head.from_, [from_ast(ast_object.cause)]))
     return Expr(Head.raise_, args)
 
 
 @from_ast.register
 def _del(ast_object: ast.Delete):
-    return Expr(Head.del_, [from_ast(ast_object.targets)])
+    return Expr(Head.del_, [from_ast(t) for t in ast_object.targets])
 
 
 @from_ast.register
 def _return(ast_object: ast.Return):
     head = Head.return_
     args = [from_ast(ast_object.value)]
     return Expr(head, args)
@@ -506,26 +540,37 @@
     for dec in ast_object.decorator_list:
         out = Expr(Head.decorator, [from_ast(dec), out])
     return out
 
 
 @from_ast.register
 def _keyword(ast_object: ast.keyword):
-    return Expr(Head.kw, [from_ast(ast_object.arg), from_ast(ast_object.value)])
+    val = from_ast(ast_object.value)
+    if ast_object is not None:
+        return Expr(Head.kw, [from_ast(ast_object.arg), val])
+    return Expr(Head.starstar, [val])
 
 
 @from_ast.register
 def _assert(ast_object: ast.Assert):
     head = Head.assert_
     args = [from_ast(ast_object.test)]
     if ast_object.msg:
         args.append(from_ast(ast_object.msg))
     return Expr(head, args)
 
 
+@from_ast.register
+def _named_expr(ast_object: ast.NamedExpr):
+    head = Head.walrus
+    target = from_ast(ast_object.target)
+    args = [target, from_ast(ast_object.value)]
+    return Expr(head, args)
+
+
 def _nest_binop(op, values: "list[ast.expr]"):
     if len(values) == 2:
         return [op, from_ast(values[0]), from_ast(values[1])]
     else:
         return [op, from_ast(values[0]), Expr(Head.binop, _nest_binop(op, values[1:]))]
```

### Comparing `macro-kit-0.4.3/macrokit/expression.py` & `macro_kit-0.4.4/macrokit/expression.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import builtins
 from copy import deepcopy
 from numbers import Number
+from weakref import WeakValueDictionary
 from types import FunctionType, ModuleType
 from typing import (
     Any,
     Callable,
     Iterable,
     Iterator,
     Sequence,
     overload,
     Union,
 )
 import inspect
 
-from macrokit.head import EXEC, Head
+from macrokit.head import EXEC, Head, HAS_BLOCK
 from macrokit.type_map import _TYPE_MAP, register_type
 from macrokit._validator import validator
 from macrokit._symbol import Symbol
 
 
 def str_(expr: Any, indent: int = 0):
     """Convert expr into a proper string."""
@@ -92,14 +93,41 @@
 def _yield_str(x: "Expr", i: int):
     args = x.args
     if isinstance(args[0], Expr) and args[0].head is Head.from_:
         return f"{_s_(i)}yield from {str_(args[0].args[0])}"
     return f"{_s_(i)}yield {sjoin(', ', args)}"
 
 
+def _try_str(x: "Expr", i: int):
+    _try = x.args[0]
+    _else = x.args[-2]
+    _finally = x.args[-1]
+    _excepts = list(x.args[1:-2])
+    strs = [f"{_s_(i)}try:\n{str_(_try, indent=i + 4)}"]
+
+    while _excepts:
+        _exc_as = _excepts.pop(0)
+        _exc_block = _excepts.pop(0)
+        assert isinstance(_exc_block, Expr)
+        if isinstance(_exc_as, Expr) and _exc_as.head is Head.empty:
+            strs.append(f"{_s_(i)}except:\n{str_(_exc_block, indent=i + 4)}")
+        else:
+            strs.append(
+                f"{_s_(i)}except {str_(_exc_as)}:\n{str_(_exc_block, indent=i + 4)}"
+            )
+
+    assert isinstance(_else, Expr)
+    assert isinstance(_finally, Expr)
+    if _else.head is not Head.empty:
+        strs.append(f"{_s_(i)}else:\n{str_(_else, indent=i + 4)}")
+    if _finally.head is not Head.empty:
+        strs.append(f"{_s_(i)}finally:\n{str_(_finally, indent=i + 4)}")
+    return "\n".join(strs)
+
+
 def _import_str(x: "Expr", i: int):
     arg0 = x.args[-1]
     if isinstance(arg0, Expr) and arg0.head == Head.from_:
         args = x.args[:-1]
         prefix = f"from {arg0.args[0]} "
     else:
         args = x.args
@@ -107,15 +135,15 @@
 
     return f"{_s_(i)}{prefix}import {sjoin(', ', args, i)}"
 
 
 _STR_MAP: "dict[Head, Callable[[Expr, int], str]]" = {
     Head.empty: lambda e, i: "",
     Head.getattr: lambda e, i: f"{str_(e.args[0], i)}.{str_(e.args[1])}",
-    Head.getitem: lambda e, i: f"{str_(e.args[0], i)}[{str_(e.args[1])}]",
+    Head.getitem: lambda e, i: f"{str_(e.args[0], i)}[{rm_par(str_(e.args[1]))}]",
     Head.del_: lambda e, i: f"{_s_(i)}del {str_(e.args[0])}",
     Head.tuple: _tuple_str,
     Head.list: lambda e, i: f"{_s_(i)}[{', '.join(str_(arg) for arg in e.args)}]",
     Head.braces: lambda e, i: f"{_s_(i)}{{{', '.join(str_(arg) for arg in e.args)}}}",
     Head.call: lambda e, i: f"{str_(e.args[0], i)}({sjoin(', ', e.args[1:])})",
     Head.assign: lambda e, i: f"{str_(e.args[0], i)} = {e.args[1]}",
     Head.kw: lambda e, i: f"{str_(e.args[0])}={str_(e.args[1])}",
@@ -127,27 +155,29 @@
     Head.block: lambda e, i: sjoin("\n", e.args, i),
     Head.function: lambda e, i: f"{_s_(i)}def {str_(e.args[0])}:\n{str_(e.args[1], i+4)}",  # noqa
     Head.lambda_: lambda e, i: f"{str_lmd(e.args[0], i)}: {str_(e.args[1])}",  # noqa
     Head.return_: lambda e, i: f"{_s_(i)}return {sjoin(', ', e.args)}",
     Head.yield_: _yield_str,
     Head.raise_: lambda e, i: f"{_s_(i)}raise {str_(e.args[0])}",
     Head.if_: lambda e, i: f"{_s_(i)}if {rm_par(str_(e.args[0]))}:\n{str_(e.args[1], i+4)}\n{_s_(i)}else:\n{str_(e.args[2], i+4)}",  # noqa
-    Head.elif_: lambda e, i: f"{_s_(i)}if {rm_par(str_(e.args[0]))}:\n{str_(e.args[1], i+4)}\n{_s_(i)}else:\n{str_(e.args[2], i+4)}",  # noqa
+    Head.try_: _try_str,
     Head.for_: lambda e, i: f"{_s_(i)}for {rm_par(str_(e.args[0]))}:\n{str_(e.args[1], i+4)}",  # noqa
     Head.while_: lambda e, i: f"{_s_(i)}while {rm_par(str_(e.args[0]))}:\n{str_(e.args[1], i+4)}",  # noqa
     Head.generator: _generator_str,
     Head.filter: _filt_str,
     Head.annotate: lambda e, i: f"{str_(e.args[0], i)}: {str_(e.args[1])}",
     Head.class_: lambda e, i: f"{_s_(i)}class {str_(e.args[0])}:\n{str_(e.args[1], i+4)}",  # noqa
     Head.from_: lambda e, i: f"{_s_(i)}from {str_(e.args[0])}",  # noqa
     Head.with_: lambda e, i: f"{_s_(i)}with {str_(e.args[0])}:\n{str_(e.args[1], i+4)}",  # noqa
     Head.as_: lambda e, i: f"{str_(e.args[0])} as {e.args[1]}",
     Head.import_: _import_str,
     Head.star: lambda e, i: f"{_s_(i)}*{str_(e.args[0])}",
+    Head.starstar: lambda e, i: f"{_s_(i)}**{str_(e.args[0])}",
     Head.decorator: lambda e, i: f"{_s_(i)}@{str_(e.args[0])}\n{_s_(i)}{e.args[1]}",
+    Head.walrus: lambda e, i: f"({str_(e.args[0])} := {str_(e.args[1])})",
 }
 
 _Expr = Union[Symbol, "Expr"]
 
 
 class Expr:
     """An expression object for metaprogramming."""
@@ -269,54 +299,59 @@
             return eval(str(self), _glb, _locals)
 
     @classmethod
     def parse_method(
         cls,
         obj: Any,
         func: Callable,
-        args: "tuple[Any, ...]" = None,
-        kwargs: dict = None,
+        args: "tuple[Any, ...] | None" = None,
+        kwargs: "dict[str, Any] | None" = None,
     ) -> "Expr":
         """Parse ``obj.func(*args, **kwargs)``."""
         method = cls(head=Head.getattr, args=[symbol(obj), func])
         return cls.parse_call(method, args, kwargs)
 
     @classmethod
     def parse_init(
         cls,
         obj: Any,
-        init_cls: Union[type, "Expr"] = None,
-        args: "tuple[Any, ...]" = None,
-        kwargs: dict = None,
+        init_cls: "type | Expr | None" = None,
+        args: "tuple[Any, ...] | None" = None,
+        kwargs: "dict[str, Any] | None" = None,
     ) -> "Expr":
         """Parse ``obj = init_cls(*args, **kwargs)``."""
         if init_cls is None:
             init_cls = type(obj)
         sym = symbol(obj)
         return cls(Head.assign, [sym, cls.parse_call(init_cls, args, kwargs)])
 
     @classmethod
     def parse_call(
         cls,
         func: Union[Callable, _Expr],
-        args: "tuple[Any, ...]" = None,
-        kwargs: dict = None,
+        args: "tuple[Any, ...] | None" = None,
+        kwargs: "dict[str, Any] | None" = None,
     ) -> "Expr":
         """Parse ``func(*args, **kwargs)``."""
         if args is None:
             args = ()
         elif not isinstance(args, tuple):
             raise TypeError("args must be a tuple")
         if kwargs is None:
             kwargs = {}
         elif not isinstance(kwargs, dict):
             raise TypeError("kwargs must be a dict")
         inputs = [func] + cls._convert_args(args, kwargs)
         return cls(head=Head.call, args=inputs)
 
+    @classmethod
+    def empty(cls) -> "Expr":
+        """Create an empty expression."""
+        return cls(head=Head.empty, args=[])
+
     def split_call(self) -> "tuple[_Expr, tuple[_Expr, ...], dict[str, _Expr]]":
         """Split ``func(*args, **kwargs)`` to (func, args, kwargs)."""
         if self.head is not Head.call:
             raise ValueError(f"Expected {Head.call}, got {self.head}.")
         args = []
         kwargs = {}
         for arg in self.args[1:]:
@@ -593,14 +628,96 @@
                     new = mapping[arg]
                 except KeyError:
                     pass
                 else:
                     self.args[i] = new
         return self
 
+    def iter_lines(self, allow_one_line: bool = True) -> "Iterator[Symbol | Expr]":
+        """Iterate over all the lines in the expression."""
+        if self.head not in HAS_BLOCK:
+            if allow_one_line:
+                yield self
+                return
+            else:
+                raise ValueError(f"Expr of {self.head} does not have code block.")
+        yield from _iter_lines(self)
+
+    def iter_getattr(self) -> "Iterator[Expr]":
+        """Iterate over all the get-attribute expression."""
+        if self.head is Head.getattr:
+            yield self
+            return
+        for arg in self.args:
+            if isinstance(arg, Symbol):
+                continue
+            if arg.head is Head.getattr:
+                yield arg
+            else:
+                yield from arg.iter_getattr()
+
+    def iter_call(self) -> "Iterator[Expr]":
+        """Iterate over all the function call."""
+        if self.head is Head.call:
+            yield self
+        for arg in self.args:
+            if isinstance(arg, Symbol):
+                continue
+            if arg.head is Head.call:
+                yield arg
+            else:
+                yield from arg.iter_call()
+
+    def iter_call_args(
+        self,
+    ) -> "Iterator[tuple[_Expr, tuple[_Expr, ...], dict[str, _Expr]]]":
+        """Iterate over all the function call and its split."""
+        for expr in self.iter_call():
+            yield expr.split_call()
+
+
+def _iter_lines(expr: Expr) -> "Iterator[Symbol | Expr]":
+    for arg in expr.args:
+        if isinstance(arg, Symbol):
+            continue
+        if arg.head is Head.block:
+            yield from _iter_lines(arg)
+        elif arg.head is Head.if_:  # = cond, if, else
+            yield arg.args[0]
+            assert isinstance(arg.args[1], Expr)
+            yield from _iter_lines(arg.args[1])
+            assert isinstance(arg.args[2], Expr)
+            yield from _iter_lines(arg.args[2])
+        elif arg.head in (Head.for_, Head.while_):  # = binop, block
+            yield arg.args[0]
+            assert isinstance(arg.args[1], Expr)
+            yield from _iter_lines(arg.args[1])
+        elif arg.head in (Head.function, Head.class_, Head.with_):
+            assert isinstance(arg.args[1], Expr)
+            yield from _iter_lines(arg.args[1])
+        elif arg.head is Head.try_:
+            assert isinstance(arg.args[0], Expr)
+            yield from _iter_lines(arg.args[0])
+            for a in arg.args[1:-2:2]:
+                assert isinstance(a, Expr) and isinstance(a.args[0], Expr)
+                yield from _iter_lines(a.args[0])
+            _else, _finally = arg.args[-2:]
+            if isinstance(_else, Expr) and _else.head is Head.block:
+                assert isinstance(_else.args[0], Expr)
+                yield from _iter_lines(_else.args[0])
+            if isinstance(_finally, Expr) and _finally.head is Head.block:
+                assert isinstance(_finally.args[0], Expr)
+                yield from _iter_lines(_finally.args[0])
+        elif arg.head is Head.decorator:
+            assert isinstance(arg.args[1], Expr)
+            yield from _iter_lines(arg.args[1])
+        else:
+            if arg.head is not Head.empty:
+                yield arg
+
 
 def _check_format_mapping(mapping_list: Iterable) -> "dict[Symbol, _Expr]":
     _dict: "dict[Symbol, _Expr]" = {}
     for comp in mapping_list:
         if len(comp) != 2:
             raise ValueError("Wrong style of mapping list.")
         k, v = comp
@@ -624,15 +741,15 @@
 def _tuple(*args) -> tuple:
     return args
 
 
 # Stored symbols and the actual values. These will be used even after parse()
 # method, to make parse(str(macro)) executable.
 _STORED_VALUES: "dict[int, tuple[_Expr, Any]]" = {}
-
+_STORED_SYMBOLS: "WeakValueDictionary[str, Any]" = WeakValueDictionary()
 
 # Map to speed up type check
 _SUBCLASS_MAP: "dict[type, type]" = {}
 
 
 def symbol(obj: Any, constant: bool = True) -> _Expr:
     """
@@ -696,14 +813,15 @@
         # calling the eval() function.
         *main, seq = obj.__name__.split(".")
         sym = Symbol(seq, obj_id)
         sym.constant = True
         if len(main) == 0:
             # submodules should not be registered
             _STORED_VALUES[obj_id] = (sym, obj)
+            _STORED_SYMBOLS[sym.name] = obj
         return sym
 
     if isinstance(seq, (Symbol, Expr)):
         # The output of register_type can be a Symbol or Expr
         return seq
     else:
         sym = Symbol(seq, obj_id)
@@ -717,14 +835,15 @@
     if not isinstance(sym, Symbol):
         raise ValueError(f"Object {obj!r} was not converted into a Symbol.")
     obj_id = id(obj)
     name = sym.name
     if not name.isidentifier():
         raise ValueError(f"{name} is not an identifier.")
     _STORED_VALUES[obj_id] = (sym, obj)
+    _STORED_SYMBOLS[sym.name] = obj
     return sym
 
 
 def store_sequence(obj: Sequence[Any]) -> Symbol:
     """Store a sequence object and make its contents expressed as varXX[i]."""
     if not isinstance(obj, Sequence):
         raise TypeError(f"Expected tuple, got {type(obj)}.")
```

### Comparing `macro-kit-0.4.3/macrokit/head.py` & `macro_kit-0.4.4/macrokit/head.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
     empty = "empty"
     getattr = "getattr"
     getitem = "getitem"
     del_ = "del"
     call = "call"
     assign = "assign"
+    walrus = "walrus"
     kw = "kw"
     tuple = "tuple"
     list = "list"
     braces = "braces"
     comment = "comment"
     assert_ = "assert"
     unop = "unop"
@@ -22,42 +23,54 @@
     block = "block"
     function = "function"
     lambda_ = "lambda"
     return_ = "return"
     yield_ = "yield"
     raise_ = "raise"
     if_ = "if"
-    elif_ = "elif"
+    try_ = "try"
     for_ = "for"
     while_ = "while"
     generator = "generator"
     filter = "filter"
     annotate = "annotate"
     import_ = "import"
     from_ = "from"
     as_ = "as"
     with_ = "with"
     class_ = "class"
     star = "star"
+    starstar = "starstar"
     decorator = "decorator"
 
 
-EXEC = (
+EXEC = {
     Head.assign,
     Head.assert_,
     Head.comment,
     Head.del_,
     Head.block,
     Head.function,
     Head.return_,
     Head.raise_,
     Head.if_,
-    Head.elif_,
     Head.for_,
     Head.while_,
     Head.annotate,
     Head.import_,
     Head.from_,
     Head.as_,
     Head.with_,
     Head.class_,
-)
+    Head.try_,
+}
+
+HAS_BLOCK = {
+    Head.block,
+    Head.if_,
+    Head.for_,
+    Head.while_,
+    Head.function,
+    Head.class_,
+    Head.with_,
+    Head.try_,
+}
```

### Comparing `macro-kit-0.4.3/macrokit/ipython/magic.py` & `macro_kit-0.4.4/macrokit/ipython/magic.py`

 * *Files identical despite different names*

### Comparing `macro-kit-0.4.3/macrokit/julia/translate.py` & `macro_kit-0.4.4/macrokit/julia/translate.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,28 +24,25 @@
     Head.getitem  : lambda e, i: f"{as_str(e.args[0], i)}[{as_str(e.args[1])}]",
     Head.call     : lambda e, i: f"{as_str(e.args[0], i)}({sjoin(', ', e.args[1:])})",
     Head.assign   : lambda e, i: f"{as_str(e.args[0], i)} = {e.args[1]}",
     Head.kw       : lambda e, i: f"{as_str(e.args[0])}={as_str(e.args[1])}",
     Head.assert_  : lambda e, i: " "*i + f"@assert {as_str(e.args[0])}, {as_str(e.args[1])}".rstrip(", "),
     Head.comment  : lambda e, i: " "*i + f"# {e.args[0]}",
     Head.binop    : lambda e, i: " "*i + f"({as_str(e.args[1])} {as_str(e.args[0])} {as_str(e.args[2])})",
-    
+
     Head.block    : lambda e, i: sjoin("\n", e.args, i),
     Head.function : lambda e, i: " "*i + f"function {as_str(e.args[0])}\n{as_str(e.args[1], i+4)}\n" + \
                                  " "*i + "end",
     Head.return_  : lambda e, i: " "*i + f"return {sjoin(', ', e.args)}",
     Head.if_      : lambda e, i: " "*i + f"if {rm_par(as_str(e.args[0]))}\n{as_str(e.args[1], i+4)}\n" + \
                                  " "*i + f"else\n{as_str(e.args[2], i+4)}\n" + \
                                  " "*i + "end",
-    Head.elif_    : lambda e, i: " "*i + f"if {rm_par(as_str(e.args[0]))}\n{as_str(e.args[1], i+4)}\n" + \
-                                 " "*i + f"else\n{as_str(e.args[2], i+4)}\n" + \
-                                 " "*i + "end",
     Head.for_     : lambda e, i: " "*i + f"for {rm_par(as_str(e.args[0]))}\n{as_str(e.args[1], i+4)}\n" + \
                                  " "*i + "end",
     Head.annotate : lambda e, i: f"{as_str(e.args[0], i)}::{as_str(e.args[1])}"
 }
 
 def to_julia_expr(s: str|Expr):
     if isinstance(s, str):
         s = parse(s)
     julia_code = as_str(s)
-    return julia_code
+    return julia_code
```

### Comparing `macro-kit-0.4.3/macrokit/macro.py` & `macro_kit-0.4.4/macrokit/macro.py`

 * *Files identical despite different names*

### Comparing `macro-kit-0.4.3/macrokit/mock.py` & `macro_kit-0.4.4/macrokit/mock.py`

 * *Files identical despite different names*

### Comparing `macro-kit-0.4.3/macrokit/type_map.py` & `macro_kit-0.4.4/macrokit/type_map.py`

 * *Files identical despite different names*

