# Comparing `tmp/pytreeclass-0.3.7.tar.gz` & `tmp/pytreeclass-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytreeclass-0.3.7.tar", last modified: Tue May 30 07:07:32 2023, max compression
+gzip compressed data, was "pytreeclass-0.3.8.tar", last modified: Mon Jun 12 18:31:08 2023, max compression
```

## Comparing `pytreeclass-0.3.7.tar` & `pytreeclass-0.3.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:07:32.940313 pytreeclass-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-05-30 07:07:32.940313 pytreeclass-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:07:32.936313 pytreeclass-0.3.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:07:32.936313 pytreeclass-0.3.7/pytreeclass/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/pytreeclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:07:32.940313 pytreeclass-0.3.7/pytreeclass/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/pytreeclass/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/pytreeclass/_src/code_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    19808 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/pytreeclass/_src/tree_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    26343 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/pytreeclass/_src/tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    27290 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/pytreeclass/_src/tree_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:07:32.936313 pytreeclass-0.3.7/pytreeclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-05-30 07:07:32.000000 pytreeclass-0.3.7/pytreeclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-30 07:07:32.000000 pytreeclass-0.3.7/pytreeclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 07:07:32.000000 pytreeclass-0.3.7/pytreeclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 07:07:32.000000 pytreeclass-0.3.7/pytreeclass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 07:07:32.000000 pytreeclass-0.3.7/pytreeclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 07:07:32.000000 pytreeclass-0.3.7/pytreeclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 07:07:32.940313 pytreeclass-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:07:32.940313 pytreeclass-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17765 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/test_tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/test_tree_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/test_tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/test_tree_viz_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/test_treeclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-30 07:07:19.000000 pytreeclass-0.3.7/tests/test_under_jit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:31:08.022609 pytreeclass-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-12 18:31:08.022609 pytreeclass-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:31:08.018608 pytreeclass-0.3.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:31:08.018608 pytreeclass-0.3.8/pytreeclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/pytreeclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:31:08.018608 pytreeclass-0.3.8/pytreeclass/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/pytreeclass/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/pytreeclass/_src/code_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25307 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/pytreeclass/_src/tree_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26345 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/pytreeclass/_src/tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23013 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/pytreeclass/_src/tree_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:31:08.018608 pytreeclass-0.3.8/pytreeclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-12 18:31:07.000000 pytreeclass-0.3.8/pytreeclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-12 18:31:07.000000 pytreeclass-0.3.8/pytreeclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:31:07.000000 pytreeclass-0.3.8/pytreeclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:31:07.000000 pytreeclass-0.3.8/pytreeclass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 18:31:07.000000 pytreeclass-0.3.8/pytreeclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 18:31:07.000000 pytreeclass-0.3.8/pytreeclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 18:31:08.022609 pytreeclass-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:31:08.022609 pytreeclass-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/test_tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/test_tree_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17367 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/test_tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/test_tree_viz_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/test_treeclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-12 18:30:58.000000 pytreeclass-0.3.8/tests/test_under_jit.py
```

### Comparing `pytreeclass-0.3.7/LICENSE` & `pytreeclass-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.7/docs/conf.py` & `pytreeclass-0.3.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.7/pytreeclass/__init__.py` & `pytreeclass-0.3.8/pytreeclass/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from pytreeclass._src.code_build import field, fields
-from pytreeclass._src.tree_base import AtIndexer, TreeClass
+from pytreeclass._src.tree_base import (
+    AtIndexer,
+    TreeClass,
+    freeze,
+    is_frozen,
+    is_nondiff,
+    unfreeze,
+)
 from pytreeclass._src.tree_pprint import (
     tree_diagram,
     tree_indent,
     tree_mermaid,
     tree_repr,
     tree_repr_with_trace,
     tree_str,
     tree_summary,
 )
 from pytreeclass._src.tree_util import (
     Partial,
+    RegexKey,
     bcmap,
-    freeze,
-    is_frozen,
-    is_nondiff,
     is_tree_equal,
     tree_flatten_with_trace,
     tree_leaves_with_trace,
     tree_map_with_trace,
-    unfreeze,
 )
 
 __all__ = (
     # general utils
     "TreeClass",
     "is_tree_equal",
     "field",
@@ -44,14 +48,15 @@
     "bcmap",
     "AtIndexer",
     "tree_map_with_trace",
     "tree_leaves_with_trace",
     "tree_flatten_with_trace",
     "tree_repr_with_trace",
     "Partial",
+    "RegexKey",
 )
 
-__version__ = "0.3.7"
+__version__ = "0.3.8"
 
 AtIndexer.__module__ = "pytreeclass"
 TreeClass.__module__ = "pytreeclass"
 Partial.__module__ = "pytreeclass"
```

### Comparing `pytreeclass-0.3.7/pytreeclass/_src/__init__.py` & `pytreeclass-0.3.8/pytreeclass/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.7/pytreeclass/_src/code_build.py` & `pytreeclass-0.3.8/pytreeclass/_src/code_build.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 # limitations under the License.
 """Constructor code generation from type annotations."""
 
 from __future__ import annotations
 
 import functools as ft
 import sys
-from collections.abc import Callable, MutableMapping, MutableSequence
+from collections.abc import Callable, MutableMapping, MutableSequence, MutableSet
 from types import FunctionType, MappingProxyType
 from typing import Any, Literal, NamedTuple, Sequence, TypeVar, get_args
 
 T = TypeVar("T")
 PyTree = Any
 EllipsisType = type(Ellipsis)
 ArgKindType = Literal["POS_ONLY", "POS_OR_KW", "KW_ONLY"]
 ArgKind = get_args(ArgKindType)
 NULL = type("NULL", (), {"__repr__": lambda _: "NULL"})()
-MUTABLE_TYPES = (MutableSequence, MutableMapping, set)
+MUTABLE_TYPES = (MutableSequence, MutableMapping, MutableSet)
 # https://github.com/google/jax/issues/14295
 
 
 class Field(NamedTuple):
     name: str | None = None
     type: type | None = None
     default: Any = NULL
```

### Comparing `pytreeclass-0.3.7/pytreeclass/_src/tree_base.py` & `pytreeclass-0.3.8/pytreeclass/_src/tree_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """Define a class that convert a class to a JAX compatible tree structure"""
 
 from __future__ import annotations
 
 import abc
 from collections.abc import Callable
 from contextlib import contextmanager
-from typing import Any, NamedTuple, TypeVar
+from typing import Any, Generic, Hashable, NamedTuple, TypeVar
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy as np
 from typing_extensions import dataclass_transform
 
@@ -32,22 +32,24 @@
     _build_init_method,
     field,
 )
 from pytreeclass._src.tree_pprint import tree_repr, tree_str
 from pytreeclass._src.tree_util import (
     IsLeafType,
     NamedSequenceKey,
+    WhereAtomType,
+    WhereType,
     _leafwise_transform,
     _resolve_where,
     is_tree_equal,
     tree_copy,
     tree_hash,
 )
 
-T = TypeVar("T", bound="TreeClass")
+T = TypeVar("T", bound=Hashable)
 PyTree = Any
 EllipsisType = type(Ellipsis)
 _no_initializer = object()
 
 # allow methods in mutable context to be called without raising `AttributeError`
 # the instances are registered  during initialization and using `at`  property
 # with `__call__ this is done by registering the instance id in a set before
@@ -119,18 +121,18 @@
         ...        return f"{self.__class__.__name__}(a={self.a}, b={self.b})"
 
         >>> Tree(1, 2).at["a"].get()
         Tree(a=1, b=None)
     """
 
     tree: PyTree
-    where: tuple[str | int] | PyTree
+    where: tuple[str | int] | PyTree = ()
 
-    def __getitem__(self, where: str | int | PyTree | EllipsisType) -> AtIndexer:
-        if isinstance(where, (type(self.tree), str, int, EllipsisType)):
+    def __getitem__(self, where: WhereType) -> AtIndexer:
+        if isinstance(where, (type(self.tree), *WhereAtomType)):
             return AtIndexer(self.tree, (*self.where, where))
 
         raise NotImplementedError(
             f"Indexing with {type(where).__name__} is not implemented.\n"
             "Example of supported indexing:\n\n"
             ">>> import jax\n"
             ">>> import pytreeclass as pytc\n"
@@ -139,15 +141,17 @@
             f">>> tree = {type(self.tree).__name__}(...)\n"
             ">>> # indexing by boolean pytree\n"
             ">>> mask = jax.tree_map(lambda x: x > 0, tree)\n"
             ">>> tree.at[mask].get()\n\n"
             ">>> # indexing by attribute name\n"
             ">>> tree.at[`attribute_name`].get()\n\n"
             ">>> # indexing by leaf index\n"
-            ">>> tree.at[index].get()"
+            ">>> tree.at[index].get()\n"
+            ">>> # indexing by regex pattern\n"
+            ">>> tree.at[pytc.RegexKey(`pattern`)].get()\n"
         )
 
     def get(self, *, is_leaf: IsLeafType = None) -> PyTree:
         """Get the leaf values at the specified location.
 
         Args:
             is_leaf: a predicate function to determine if a value is a leaf.
@@ -511,15 +515,15 @@
             >>> tree.at["a"].apply(lambda x: 100)
             Tree(a=100, b=2.0)
             >>> # call `add` and return a tuple of
             >>> # (return value, new instance)
             >>> tree.at["add"](99)
             (100, Tree(a=100, b=2.0))
         """
-        return AtIndexer(self, where=())
+        return AtIndexer(self)
 
     def __repr__(self) -> str:
         return tree_repr(self)
 
     def __str__(self) -> str:
         return tree_str(self)
 
@@ -527,7 +531,154 @@
         return tree_copy(self)
 
     def __hash__(self) -> int:
         return tree_hash(self)
 
     def __eq__(self, other: Any) -> bool | jax.Array:
         return is_tree_equal(self, other)
+
+
+def _frozen_error(opname: str, tree):
+    raise NotImplementedError(
+        f"Cannot apply `{opname}` operation to a frozen object `{tree!r}`.\n"
+        "Unfreeze the object first to apply operations to it\n"
+        "Example:\n"
+        ">>> import jax\n"
+        ">>> import pytreeclass as pytc\n"
+        ">>> tree = jax.tree_map(pytc.unfreeze, tree, is_leaf=pytc.is_frozen)"
+    )
+
+
+class _Frozen(Generic[T]):
+    __slots__ = ("__wrapped__", "__weakref__")
+    __wrapped__: T
+
+    def __init__(self, x: T) -> None:
+        object.__setattr__(self, "__wrapped__", x)
+
+    def __setattr__(self, _, __) -> None:
+        raise AttributeError("Cannot assign to frozen instance.")
+
+    def __delattr__(self, _: str) -> None:
+        raise AttributeError("Cannot delete from frozen instance.")
+
+    def __repr__(self) -> str:
+        return "#" + tree_repr(self.__wrapped__)
+
+    def __str__(self) -> str:
+        return "#" + tree_str(self.__wrapped__)
+
+    def __copy__(self) -> _Frozen[T]:
+        return _Frozen(tree_copy(self.__wrapped__))
+
+    def __eq__(self, rhs: Any) -> bool | jax.Array:
+        if not isinstance(rhs, _Frozen):
+            return False
+        return is_tree_equal(self.__wrapped__, rhs.__wrapped__)
+
+    def __hash__(self) -> int:
+        return tree_hash(self.__wrapped__)
+
+    # raise helpful error message when trying to interact with frozen object
+    __add__ = __radd__ = __iadd__ = lambda x, _: _frozen_error("+", x)
+    __sub__ = __rsub__ = __isub__ = lambda x, _: _frozen_error("-", x)
+    __mul__ = __rmul__ = __imul__ = lambda x, _: _frozen_error("*", x)
+    __matmul__ = __rmatmul__ = __imatmul__ = lambda x, _: _frozen_error("@", x)
+    __truediv__ = __rtruediv__ = __itruediv__ = lambda x, _: _frozen_error("/", x)
+    __floordiv__ = __rfloordiv__ = __ifloordiv__ = lambda x, _: _frozen_error("//", x)
+    __mod__ = __rmod__ = __imod__ = lambda x, _: _frozen_error("%", x)
+    __pow__ = __rpow__ = __ipow__ = lambda x, _: _frozen_error("**", x)
+    __lshift__ = __rlshift__ = __ilshift__ = lambda x, _: _frozen_error("<<", x)
+    __rshift__ = __rrshift__ = __irshift__ = lambda x, _: _frozen_error(">>", x)
+    __and__ = __rand__ = __iand__ = lambda x, _: _frozen_error("and", x)
+    __xor__ = __rxor__ = __ixor__ = lambda x, _: _frozen_error("xor", x)
+    __or__ = __ror__ = __ior__ = lambda x, _: _frozen_error("or", x)
+    __neg__ = __pos__ = __abs__ = __invert__ = lambda x: _frozen_error("unary op", x)
+    __call__ = lambda x, *_, **__: _frozen_error("call", x)
+
+
+jtu.register_pytree_node(
+    nodetype=_Frozen,
+    flatten_func=lambda tree: ((), tree),
+    unflatten_func=lambda treedef, _: treedef,
+)
+
+
+def freeze(wrapped: _Frozen[T] | T) -> _Frozen[T]:
+    """Freeze a value to avoid updating it by `jax` transformations.
+
+    Example:
+        >>> import jax
+        >>> import pytreeclass as pytc
+        >>> import jax.tree_util as jtu
+        >>> # Usage with `jax.tree_util.tree_leaves`
+        >>> # no leaves for a wrapped value
+        >>> jtu.tree_leaves(pytc.freeze(2.))
+        []
+
+        >>> # retrieve the frozen wrapper value using `is_leaf=pytc.is_frozen`
+        >>> jtu.tree_leaves(pytc.freeze(2.), is_leaf=pytc.is_frozen)
+        [#2.0]
+
+        >>> # Usage with `jax.tree_util.tree_map`
+        >>> a= [1,2,3]
+        >>> a[1] = pytc.freeze(a[1])
+        >>> jtu.tree_map(lambda x:x+100, a)
+        [101, #2, 103]
+    """
+    return wrapped if is_frozen(wrapped) else _Frozen(wrapped)  # type: ignore
+
+
+def is_frozen(wrapped: Any) -> bool:
+    """Returns True if the value is a frozen wrapper."""
+    return isinstance(wrapped, _Frozen)
+
+
+def unfreeze(wrapped: _Frozen[T] | T) -> T:
+    """Unfreeze `frozen` value, otherwise return the value itself.
+
+    - use `is_leaf=pytc.is_frozen` with `jax.tree_map` to unfreeze a tree.**
+
+    Example:
+        >>> import pytreeclass as pytc
+        >>> import jax
+        >>> frozen_value = pytc.freeze(1)
+        >>> pytc.unfreeze(frozen_value)
+        1
+        >>> # usage with `jax.tree_map`
+        >>> frozen_tree = jax.tree_map(pytc.freeze, {"a": 1, "b": 2})
+        >>> unfrozen_tree = jax.tree_map(pytc.unfreeze, frozen_tree, is_leaf=pytc.is_frozen)
+        >>> unfrozen_tree
+        {'a': 1, 'b': 2}
+    """
+    return getattr(wrapped, "__wrapped__") if is_frozen(wrapped) else wrapped
+
+
+def is_nondiff(wrapped: Any) -> bool:
+    """
+    Returns True if the node is a non-differentiable node, and False for if the
+    node is of type float, complex number, or a numpy array of floats or
+    complex numbers.
+
+    Example:
+        >>> import pytreeclass as pytc
+        >>> import jax.numpy as jnp
+        >>> pytc.is_nondiff(jnp.array(1))  # int array is non-diff type
+        True
+        >>> pytc.is_nondiff(jnp.array(1.))  # float array is diff type
+        False
+        >>> pytc.is_nondiff(1)  # int is non-diff type
+        True
+        >>> pytc.is_nondiff(1.)  # float is diff type
+        False
+
+    Note:
+        This function is meant to be used with `jax.tree_map` to
+        create a mask for non-differentiable nodes in a tree, that can be used
+        to freeze the non-differentiable nodes before passing the tree to a
+        `jax` transformation.
+    """
+    if hasattr(wrapped, "dtype") and np.issubdtype(wrapped.dtype, np.inexact):
+        return False
+    if isinstance(wrapped, (float, complex)):
+        return False
+    return True
```

### Comparing `pytreeclass-0.3.7/pytreeclass/_src/tree_pprint.py` & `pytreeclass-0.3.8/pytreeclass/_src/tree_pprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,16 +115,15 @@
 
 def general_pp(node: Any, **spec: Unpack[PPSpec]) -> str:
     text = f"{node!r}" if spec["kind"] == "REPR" else f"{node!s}"
 
     if "\n" not in text:
         return text
 
-    indent = spec["indent"] + 1
-    return "\n" + "\t" * indent + ("\n" + "\t" * indent).join(text.split("\n"))
+    return ("\n" + "\t" * (spec["indent"])).join(text.split("\n"))
 
 
 def shape_dtype_pp(node: Any, **spec: Unpack[PPSpec]) -> str:
     """Pretty print a node with dtype and shape"""
     shape = f"{node.shape}".replace(",", "")
     shape = shape.replace("(", "[")
     shape = shape.replace(")", "]")
@@ -180,15 +179,15 @@
     return text
 
 
 def list_pp(node: list, **spec: Unpack[PPSpec]) -> str:
     return "[" + pps(node, pp=pp, **spec) + "]"
 
 
-def tuple_pp(node: tuple, **spec) -> str:
+def tuple_pp(node: tuple, **spec: Unpack[PPSpec]) -> str:
     return "(" + pps(node, pp=pp, **spec) + ")"
 
 
 def set_pp(node: set, **spec: Unpack[PPSpec]) -> str:
     return "{" + pps(node, pp=pp, **spec) + "}"
 
 
@@ -698,15 +697,15 @@
         is_leaf: function to determine if a node is a leaf. defaults to None
 
     Returns:
         String summary of the tree structure
         - First column: path to the node
         - Second column: type of the node
         - Third column: number of leaves in the node
-        - Last row: type of parent, number of leaves and size of parent
+        - Last row: type of parent, number of leaves of the parent
 
     Note:
         Array elements are considered as leaves, for example:
         `jnp.array([1,2,3])` has 3 leaves
 
     Example:
         >>> import pytreeclass as pytc
@@ -826,10 +825,10 @@
         names = "->".join(str(i) for i in trace[0])
         ROWS += [["Name path", names]]
 
         types = "->".join(i.__name__ for i in trace[1])
         ROWS += [["Type path", types]]
 
         # make a pretty table for each leaf
-        return _table(ROWS, transpose=transpose)
+        return "\n\t" + ("\n\t").join(_table(ROWS, transpose=transpose).split("\n"))
 
     return tree_map_with_trace(leaf_trace_summary, tree, is_leaf=is_leaf)
```

### Comparing `pytreeclass-0.3.7/pytreeclass/_src/tree_util.py` & `pytreeclass-0.3.8/pytreeclass/_src/tree_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,202 +7,132 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""Utility functions for pytrees."""
 
 from __future__ import annotations
 
 import dataclasses as dc
 import functools as ft
 import operator as op
+import re
 from collections import defaultdict
 from math import ceil, floor, trunc
 from typing import (
     Any,
     Callable,
-    Generic,
     Hashable,
     Iterator,
+    NamedTuple,
     Sequence,
     Tuple,
     TypeVar,
     Union,
 )
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
-import numpy as np
 from jax._src.tree_util import _registry, _registry_with_keypaths
 from jax.util import unzip2
 
 T = TypeVar("T")
 PyTree = Any
-EllipsisType = type(Ellipsis)
+# TODO: swich to type(Ellipsis) for python 3.10
+EllipsisType = TypeVar("EllipsisType")
 KeyEntry = TypeVar("KeyEntry", bound=Hashable)
 TypeEntry = TypeVar("TypeEntry", bound=type)
 TraceEntry = Tuple[KeyEntry, TypeEntry]
 KeyPath = Tuple[KeyEntry, ...]
 TypePath = Tuple[TypeEntry, ...]
 TraceType = Tuple[KeyPath, TypePath]
-IsLeafType = Union[type(None), Callable[[Any], bool]]
+IsLeafType = Union[None, Callable[[Any], bool]]
 
 
-def tree_hash(*trees: PyTree) -> int:
-    leaves, treedef = jtu.tree_flatten(trees)
-    return hash((*leaves, treedef))
+class RegexKey(NamedTuple):
+    """Match a leaf with a regex pattern inside 'at' property.
 
+    Args:
+        pattern: regex pattern to match.
 
-def _frozen_error(opname: str, tree):
-    raise NotImplementedError(
-        f"Cannot apply `{opname}` operation to a frozen object `{tree!r}`.\n"
-        "Unfreeze the object first to apply operations to it\n"
-        "Example:\n"
-        ">>> import jax\n"
-        ">>> import pytreeclass as pytc\n"
-        ">>> tree = jax.tree_map(pytc.unfreeze, tree, is_leaf=pytc.is_frozen)"
-    )
-
-
-class _FrozenWrapper(Generic[T]):
-    __slots__ = ("__wrapped__", "__weakref__")
-
-    def __init__(self, x: T) -> None:
-        object.__setattr__(self, "__wrapped__", x)
-
-    def __setattr__(self, _, __) -> None:
-        raise AttributeError("Cannot assign to frozen instance.")
 
-    def __delattr__(self, _: str) -> None:
-        raise AttributeError("Cannot delete from frozen instance.")
+    Example:
+        >>> import pytreeclass as pytc
+        >>> class Tree(pytc.TreeClass):
+        ...     weight_1: float = 1.0
+        ...     weight_2: float = 2.0
+        ...     weight_3: float = 3.0
+        ...     bias: float = 0.0
+        >>> tree = Tree()
+        >>> tree.at[pytc.RegexKey(r"weight_.*")].set(100.0)  # set all weights to 100.0
+        Tree(weight_1=100.0, weight_2=100.0, weight_3=100.0, bias=0.0)
+    """
 
-    def __repr__(self):
-        return f"#{self.__wrapped__!r}"
+    pattern: str
 
-    def __eq__(self, rhs: Any) -> bool | jax.Array:
-        if not isinstance(rhs, _FrozenWrapper):
+    def __eq__(self, other: Any) -> bool:
+        """Return True if other fully matches the regex pattern."""
+        if not isinstance(other, str):
             return False
-        return is_tree_equal(self.__wrapped__, rhs.__wrapped__)
-
-    def __hash__(self) -> int:
-        return tree_hash(self.__wrapped__)
-
-    # raise helpful error message when trying to interact with frozen object
-    __add__ = __radd__ = __iadd__ = lambda x, _: _frozen_error("+", x)
-    __sub__ = __rsub__ = __isub__ = lambda x, _: _frozen_error("-", x)
-    __mul__ = __rmul__ = __imul__ = lambda x, _: _frozen_error("*", x)
-    __matmul__ = __rmatmul__ = __imatmul__ = lambda x, _: _frozen_error("@", x)
-    __truediv__ = __rtruediv__ = __itruediv__ = lambda x, _: _frozen_error("/", x)
-    __floordiv__ = __rfloordiv__ = __ifloordiv__ = lambda x, _: _frozen_error("//", x)
-    __mod__ = __rmod__ = __imod__ = lambda x, _: _frozen_error("%", x)
-    __pow__ = __rpow__ = __ipow__ = lambda x, _: _frozen_error("**", x)
-    __lshift__ = __rlshift__ = __ilshift__ = lambda x, _: _frozen_error("<<", x)
-    __rshift__ = __rrshift__ = __irshift__ = lambda x, _: _frozen_error(">>", x)
-    __and__ = __rand__ = __iand__ = lambda x, _: _frozen_error("and", x)
-    __xor__ = __rxor__ = __ixor__ = lambda x, _: _frozen_error("xor", x)
-    __or__ = __ror__ = __ior__ = lambda x, _: _frozen_error("or", x)
-    __neg__ = __pos__ = __abs__ = __invert__ = lambda x: _frozen_error("unary op", x)
-    __call__ = lambda x, *_, **__: _frozen_error("call", x)
-
-
-jtu.register_pytree_node(
-    nodetype=_FrozenWrapper,
-    flatten_func=lambda tree: ((), tree),
-    unflatten_func=lambda treedef, _: treedef,
-)
-
+        return re.fullmatch(self.pattern, other) is not None
 
-def freeze(wrapped: Any) -> _FrozenWrapper:
-    """Freeze a value to avoid updating it by `jax` transformations.
 
-    Example:
-        >>> import jax
-        >>> import pytreeclass as pytc
-        >>> import jax.tree_util as jtu
-        >>> # Usage with `jax.tree_util.tree_leaves`
-        >>> # no leaves for a wrapped value
-        >>> jtu.tree_leaves(pytc.freeze(2.))
-        []
-
-        >>> # retrieve the frozen wrapper value using `is_leaf=pytc.is_frozen`
-        >>> jtu.tree_leaves(pytc.freeze(2.), is_leaf=pytc.is_frozen)
-        [#2.0]
-
-        >>> # Usage with `jax.tree_util.tree_map`
-        >>> a= [1,2,3]
-        >>> a[1] = pytc.freeze(a[1])
-        >>> jtu.tree_map(lambda x:x+100, a)
-        [101, #2, 103]
-    """
-    return wrapped if is_frozen(wrapped) else _FrozenWrapper(wrapped)
+WhereAtomType = (int, str, type(...), RegexKey)
+WhereType = Union[int, str, RegexKey, PyTree, EllipsisType]
 
 
-def is_frozen(wrapped: Any) -> bool:
-    """Returns True if the value is a frozen wrapper."""
-    return isinstance(wrapped, _FrozenWrapper)
+def tree_hash(*trees: PyTree) -> int:
+    leaves, treedef = jtu.tree_flatten(trees)
+    return hash((*leaves, treedef))
 
 
-def unfreeze(wrapped: Any) -> Any:
-    """Unfreeze `frozen` value, otherwise return the value itself.
+def tree_copy(tree: T) -> T:
+    """Return a copy of the tree."""
+    return jtu.tree_unflatten(*jtu.tree_flatten(tree)[::-1])
 
-    - use `is_leaf=pytc.is_frozen` with `jax.tree_map` to unfreeze a tree.**
 
-    Example:
-        >>> import pytreeclass as pytc
-        >>> import jax
-        >>> frozen_value = pytc.freeze(1)
-        >>> pytc.unfreeze(frozen_value)
-        1
-        >>> # usage with `jax.tree_map`
-        >>> frozen_tree = jax.tree_map(pytc.freeze, {"a": 1, "b": 2})
-        >>> unfrozen_tree = jax.tree_map(pytc.unfreeze, frozen_tree, is_leaf=pytc.is_frozen)
-        >>> unfrozen_tree
-        {'a': 1, 'b': 2}
-    """
-    return getattr(wrapped, "__wrapped__") if is_frozen(wrapped) else wrapped
+def _is_leaf_rhs_equal(leaf, rhs) -> bool | jax.Array:
+    if hasattr(leaf, "shape") and hasattr(leaf, "dtype"):
+        if hasattr(rhs, "shape") and hasattr(rhs, "dtype"):
+            if leaf.shape != rhs.shape:
+                return False
+            if leaf.dtype != rhs.dtype:
+                return False
+            try:
+                return bool(verdict := jnp.all(leaf == rhs))
+            except Exception:
+                return verdict  # fail under `jit`
+        return False
+    return leaf == rhs
 
 
-def is_nondiff(wrapped: Any) -> bool:
-    """
-    Returns True if the node is a non-differentiable node, and False for if the
-    node is of type float, complex number, or a numpy array of floats or
-    complex numbers.
+def is_tree_equal(*trees: Any) -> bool | jax.Array:
+    """Return `True` if all pytrees are equal.
 
-    Example:
-        >>> import pytreeclass as pytc
-        >>> import jax.numpy as jnp
-        >>> pytc.is_nondiff(jnp.array(1))  # int array is non-diff type
-        True
-        >>> pytc.is_nondiff(jnp.array(1.))  # float array is diff type
-        False
-        >>> pytc.is_nondiff(1)  # int is non-diff type
-        True
-        >>> pytc.is_nondiff(1.)  # float is diff type
-        False
+    Note:
+        trees are compared using their leaves and treedefs.
 
     Note:
-        This function is meant to be used with `jax.tree_map` to
-        create a mask for non-differentiable nodes in a tree, that can be used
-        to freeze the non-differentiable nodes before passing the tree to a
-        `jax` transformation.
+        Under `jit` the return type is boolean `jax.Array` instead of `bool`.
     """
-    if hasattr(wrapped, "dtype") and np.issubdtype(wrapped.dtype, np.inexact):
-        return False
-    if isinstance(wrapped, (float, complex)):
-        return False
-    return True
 
+    tree0, *rest = trees
+    leaves0, treedef0 = jtu.tree_flatten(tree0)
+    verdict = True
 
-def tree_copy(tree: T) -> T:
-    """Return a copy of the tree."""
-    leaves, treedef = jtu.tree_flatten(tree)
-    return jtu.tree_unflatten(treedef, leaves)
+    for tree in rest:
+        leaves, treedef = jtu.tree_flatten(tree)
+        if (treedef != treedef0) or verdict is False:
+            return False
+        verdict = ft.reduce(op.and_, map(_is_leaf_rhs_equal, leaves0, leaves), verdict)
+    return verdict
 
 
 class Partial:
     """
     jaxable Partial function with support for positional partial application.
 
     Example:
@@ -269,15 +199,15 @@
     nodetype=Partial,
     flatten_func=lambda x: ((x.func, x.args, x.kwargs), None),
     unflatten_func=lambda _, xs: Partial(*xs),
 )
 
 
 def bcmap(
-    func: Callable[..., Any],
+    func: Callable,
     *,
     is_leaf: IsLeafType = None,
 ) -> Callable:
     """
     (map)s a function over pytrees leaves with automatic (b)road(c)asting
     for scalar arguments
 
@@ -355,32 +285,31 @@
             if treedef0 == jtu.tree_structure(kwargs[key]):
                 masked_kwargs[key] = ...
                 leaves += [treedef0.flatten_up_to(kwargs[key])]
                 leaves_keys += [key]
             else:
                 masked_kwargs[key] = kwargs[key]
 
-        # avoid circular import by importing Partial here
-        from pytreeclass import Partial
-
         bfunc = Partial(func, *masked_args, **masked_kwargs)
 
         if len(leaves_keys) == 0:
             # no kwargs leaves are present, so we can immediately zip
             return jtu.tree_unflatten(treedef0, [bfunc(*xs) for xs in zip(*leaves)])
 
         # kwargs leaves are present, so we need to zip them
         kwargnum = len(leaves) - len(leaves_keys)
         all_leaves = []
         for xs in zip(*leaves):
             xs_args, xs_kwargs = xs[:kwargnum], xs[kwargnum:]
             all_leaves += [bfunc(*xs_args, **dict(zip(leaves_keys, xs_kwargs)))]
         return jtu.tree_unflatten(treedef0, all_leaves)
 
-    docs = f"Broadcasted version of {func.__name__}\n{func.__doc__}"
+    name = getattr(func, "__name__", func)
+
+    docs = f"Broadcasted version of {name}\n{func.__doc__}"
     wrapper.__doc__ = docs
     return wrapper
 
 
 def _unary_op(func):
     def wrapper(self):
         return jtu.tree_map(func, self)
@@ -453,93 +382,57 @@
         if key not in vars(klass):
             # do not override any user defined methods
             # this behavior similar is to `dataclasses.dataclass`
             setattr(klass, key, method)
     return klass
 
 
-def _is_leaf_rhs_equal(leaf, rhs) -> bool | jax.Array:
-    if hasattr(leaf, "shape") and hasattr(leaf, "dtype"):
-        if hasattr(rhs, "shape") and hasattr(rhs, "dtype"):
-            if leaf.shape != rhs.shape:
-                return False
-            if leaf.dtype != rhs.dtype:
-                return False
-            try:
-                return bool(verdict := jnp.all(leaf == rhs))
-            except Exception:
-                return verdict  # fail under `jit`
-        return False
-    return leaf == rhs
-
-
-def is_tree_equal(*trees: Any) -> bool | jax.Array:
-    """Return `True` if all pytrees are equal.
-
-    Note:
-        trees are compared using their leaves and treedefs.
-
-    Note:
-        Under `jit` the return type is boolean `jax.Array` instead of `bool`.
-    """
-
-    tree0, *rest = trees
-    leaves0, treedef0 = jtu.tree_flatten(tree0)
-    verdict = True
-
-    for tree in rest:
-        leaves, treedef = jtu.tree_flatten(tree)
-        if (treedef != treedef0) or verdict is False:
-            return False
-        verdict = ft.reduce(op.and_, map(_is_leaf_rhs_equal, leaves0, leaves), verdict)
-    return verdict
-
-
 @dc.dataclass(frozen=True)
 class NamedSequenceKey(jtu.GetAttrKey, jtu.SequenceKey):
     # inherit from both `jtu.GetAttrKey` and `jtu.SequenceKey`
     # in case the user perform isinstance check to unpack the name/index
     # `TreeClass` is modeled as a `NamedTuple`` with both `name` and `idx` identifiers
     def __str__(self):
         return f".{self.name}"
 
 
 # indexing matching registry
 # define rule for indexing matching through `at` property
 # for example, `jax` internals uses `jtu.GetAttrKey` to index an attribute,
 # however its not ergonomic to use `tree.at[jtu.GetAttrKey("attr")]`
 # to index an attribute instead `tree.at['attr']` is more ergonomic
-match_registry: dict[type, Callable] = defaultdict(lambda entry: (entry,))
+match_registry: dict[type, Callable] = defaultdict(lambda entry: (entry,))  # type: ignore
 match_registry[jtu.GetAttrKey] = lambda entry: (entry.name,)
 match_registry[jtu.SequenceKey] = lambda entry: (entry.idx,)
 match_registry[NamedSequenceKey] = lambda entry: (entry.idx, entry.name)
 match_registry[jtu.DictKey] = lambda entry: (entry.key,)
 match_registry[jtu.FlattenedIndexKey] = lambda entry: (entry.key,)
 
 
 def _generate_path_mask(
     tree: PyTree,
-    where: tuple[int | str, ...],
+    where: tuple[WhereType, ...],
     is_leaf: IsLeafType = None,
 ) -> PyTree:
     # generate a mask for `where` path in `tree`
     # where path is a tuple of indices or keys, for example
     # where=("a",) wil set all leaves of `tree` with key "a" to True and
     # all other leaves to False
     match = False
 
     def map_func(path, _: Any):
         if len(where) > len(path):
             # path is shorter than `where` path. for example
             # where=("a", "b") and the current path is ("a",) then
             # the current path is not a match
             return False
-
         for wi, ki in zip(where, path):
-            if wi not in (..., *match_registry[type(ki)](ki)):
+            if not any(wi == ei for ei in (..., *match_registry[type(ki)](ki))):
+                # use equality instead of `in` to trigger regex matching
+                # for the overloaded `RegexKey` __eq__ method.
                 return False
 
         nonlocal match
 
         return (match := True)
 
     mask = jtu.tree_map_with_path(map_func, tree, is_leaf=is_leaf)
@@ -570,24 +463,24 @@
         return verdict
 
     return jtu.tree_map(map_func, *masks)
 
 
 def _resolve_where(
     tree: PyTree,
-    where: tuple[int | str | PyTree | EllipsisType, ...],
+    where: tuple[WhereType, ...],  # type: ignore
     is_leaf: IsLeafType = None,
 ):
     mask = None
 
-    if path := [i for i in where if isinstance(i, (int, str, type(...)))]:
+    if path := tuple(i for i in where if isinstance(i, WhereAtomType)):
         mask = _generate_path_mask(tree, path, is_leaf=is_leaf)
 
-    if maybe_bool_masks := [i for i in where if isinstance(i, type(tree))]:
-        all_masks = [mask, *maybe_bool_masks] if mask else maybe_bool_masks
+    if maybe_bool_masks := tuple(i for i in where if isinstance(i, type(tree))):
+        all_masks = (mask, *maybe_bool_masks) if mask else maybe_bool_masks
         mask = _combine_maybe_bool_masks(*all_masks)
 
     return mask
 
 
 def flatten_one_trace_level(
     trace: TraceType,
@@ -725,14 +618,15 @@
     traces_leaves, treedef = tree_flatten_with_trace(tree, is_leaf=is_leaf)
     traces_leaves = list(zip(*traces_leaves))
     traces_leaves += [treedef.flatten_up_to(r) for r in rest]
     return treedef.unflatten(func(*xs) for xs in zip(*traces_leaves))
 
 
 class Node:
+    # mainly used for visualization
     __slots__ = ("data", "parent", "children", "__weakref__")
 
     def __init__(
         self,
         data: tuple[TraceEntry, Any],
         parent: Node | None = None,
     ):
@@ -758,23 +652,14 @@
     def __repr__(self) -> str:
         return f"Node(data={self.data})"
 
     def __contains__(self, key: TraceEntry) -> bool:
         return key in self.children
 
 
-# disallow traversal to avoid infinite recursion
-# in case of circular references
-jtu.register_pytree_node(
-    nodetype=Node,
-    flatten_func=lambda tree: ((), tree),
-    unflatten_func=lambda treedef, _: treedef[0],
-)
-
-
 def construct_tree(
     tree: PyTree,
     is_leaf: IsLeafType = None,
     is_trace_leaf: IsLeafType = None,
 ) -> Node:
     # construct a tree with `Node` objects using `tree_leaves_with_trace`
     # to establish parent-child relationship between nodes
```

### Comparing `pytreeclass-0.3.7/pytreeclass.egg-info/SOURCES.txt` & `pytreeclass-0.3.8/pytreeclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.7/setup.py` & `pytreeclass-0.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.7/tests/test_indexing.py` & `pytreeclass-0.3.8/tests/test_indexing.py`

 * *Files 1% similar despite different names*

```diff
@@ -687,7 +687,24 @@
 def test_construct_tree():
     tree = construct_tree([1, 2, [3, 4]])
 
     assert repr(tree) == "Node(data=((None, <class 'list'>), None))"
 
     with pytest.raises(TypeError):
         tree.add_child("a")
+
+
+def test_regexkey():
+    class Tree(pytc.TreeClass):
+        weight_1: float = 1.0
+        weight_2: float = 2.0
+        weight_3: float = 3.0
+        bias: float = 0.0
+
+    tree = Tree()
+
+    tree = tree.at[pytc.RegexKey(r"weight_.*")].set(100.0)
+    # Tree(weight_1=100.0, weight_2=100.0, weight_3=100.0, bias=0.0)
+    assert jtu.tree_leaves(tree) == [100.0, 100.0, 100.0, 0.0]
+
+    assert pytc.RegexKey(r"w.*") == "woof"
+    assert pytc.RegexKey(r"w.*") != "meow"
```

### Comparing `pytreeclass-0.3.7/tests/test_nn.py` & `pytreeclass-0.3.8/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.7/tests/test_tree_freeze.py` & `pytreeclass-0.3.8/tests/test_tree_freeze.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.7/tests/test_tree_operator.py` & `pytreeclass-0.3.8/tests/test_tree_operator.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.7/tests/test_tree_pprint.py` & `pytreeclass-0.3.8/tests/test_tree_pprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,21 +67,21 @@
     assert tree_repr(r1, depth=0) == "Repr1(...)"
 
 
 def test_str():
     assert (
         tree_str(r1)
         # trunk-ignore(flake8/E501)
-        == "Repr1(\n  a=1, \n  b=string, \n  c=1.0, \n  d=aaaaa, \n  e=[10, 10, 10, 10, 10], \n  f={1, 2, 3}, \n  g={\n    a:aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa, \n    b:bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb, \n    c:\n      [[1. 1. 1. 1. 1.]\n       [1. 1. 1. 1. 1.]\n       [1. 1. 1. 1. 1.]\n       [1. 1. 1. 1. 1.]\n       [1. 1. 1. 1. 1.]]\n  }, \n  h=[[1.] [1.] [1.] [1.] [1.]], \n  i=[[1. 1. 1. 1. 1. 1.]], \n  j=[[[[1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]]]], \n  l=a(b=1, c=2), \n  m=\n    [[1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]], \n  n=True, \n  o=[1.+0.j 2.+0.j]\n)"
+        == "Repr1(\n  a=1, \n  b=string, \n  c=1.0, \n  d=aaaaa, \n  e=[10, 10, 10, 10, 10], \n  f={1, 2, 3}, \n  g={\n    a:aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa, \n    b:bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb, \n    c:[[1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]]\n  }, \n  h=[[1.] [1.] [1.] [1.] [1.]], \n  i=[[1. 1. 1. 1. 1. 1.]], \n  j=[[[[1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]]]], \n  l=a(b=1, c=2), \n  m=[[1. 1. 1. 1. 1.]\n   [1. 1. 1. 1. 1.]\n   [1. 1. 1. 1. 1.]\n   [1. 1. 1. 1. 1.]\n   [1. 1. 1. 1. 1.]], \n  n=True, \n  o=[1.+0.j 2.+0.j]\n)"
     )
 
     assert (
         tree_str(r1, depth=1)
         # trunk-ignore(flake8/E501)
-        == "Repr1(\n  a=1, \n  b=string, \n  c=1.0, \n  d=aaaaa, \n  e=[...], \n  f={...}, \n  g={...}, \n  h=[[1.] [1.] [1.] [1.] [1.]], \n  i=[[1. 1. 1. 1. 1. 1.]], \n  j=[[[[1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]]]], \n  l=a(...), \n  m=\n    [[1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]\n     [1. 1. 1. 1. 1.]], \n  n=True, \n  o=[1.+0.j 2.+0.j]\n)"
+        == "Repr1(\n  a=1, \n  b=string, \n  c=1.0, \n  d=aaaaa, \n  e=[...], \n  f={...}, \n  g={...}, \n  h=[[1.] [1.] [1.] [1.] [1.]], \n  i=[[1. 1. 1. 1. 1. 1.]], \n  j=[[[[1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]   [1. 1. 1. 1. 1.]]]], \n  l=a(...), \n  m=[[1. 1. 1. 1. 1.]\n   [1. 1. 1. 1. 1.]\n   [1. 1. 1. 1. 1.]\n   [1. 1. 1. 1. 1.]\n   [1. 1. 1. 1. 1.]], \n  n=True, \n  o=[1.+0.j 2.+0.j]\n)"
     )
 
 
 def test_tree_summary():
     assert (
         tree_summary(r1, depth=0)
         == "┌────┬─────┬─────┐\n│Name│Type │Count│\n├────┼─────┼─────┤\n│Σ   │Repr1│1    │\n└────┴─────┴─────┘"
```

### Comparing `pytreeclass-0.3.7/tests/test_tree_viz_util.py` & `pytreeclass-0.3.8/tests/test_tree_viz_util.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.7/tests/test_treeclass.py` & `pytreeclass-0.3.8/tests/test_treeclass.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.7/tests/test_under_jit.py` & `pytreeclass-0.3.8/tests/test_under_jit.py`

 * *Files identical despite different names*

