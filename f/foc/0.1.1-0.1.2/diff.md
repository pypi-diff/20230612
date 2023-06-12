# Comparing `tmp/foc-0.1.1.tar.gz` & `tmp/foc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foc-0.1.1.tar", last modified: Wed Jun  7 00:38:12 2023, max compression
+gzip compressed data, was "foc-0.1.2.tar", last modified: Mon Jun 12 00:48:24 2023, max compression
```

## Comparing `foc-0.1.1.tar` & `foc-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-07 00:38:12.376820 foc-0.1.1/
--rw-r--r--   0 thyeem     (501) staff       (20)       31 2023-06-07 00:37:35.000000 foc-0.1.1/ChangeLog.md
--rw-r--r--   0 thyeem     (501) staff       (20)     1068 2023-05-15 21:22:31.000000 foc-0.1.1/LICENSE
--rw-r--r--   0 thyeem     (501) staff       (20)       55 2023-06-06 23:18:02.000000 foc-0.1.1/MANIFEST.in
--rw-r--r--   0 thyeem     (501) staff       (20)      420 2023-06-07 00:38:12.376919 foc-0.1.1/PKG-INFO
--rw-r--r--   0 thyeem     (501) staff       (20)    16005 2023-06-07 00:35:01.000000 foc-0.1.1/README.md
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-07 00:38:12.375446 foc-0.1.1/foc/
--rw-r--r--   0 thyeem     (501) staff       (20)    15894 2023-06-06 23:58:42.000000 foc-0.1.1/foc/__init__.py
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-07 00:38:12.376594 foc-0.1.1/foc.egg-info/
--rw-r--r--   0 thyeem     (501) staff       (20)      420 2023-06-07 00:38:12.000000 foc-0.1.1/foc.egg-info/PKG-INFO
--rw-r--r--   0 thyeem     (501) staff       (20)      185 2023-06-07 00:38:12.000000 foc-0.1.1/foc.egg-info/SOURCES.txt
--rw-r--r--   0 thyeem     (501) staff       (20)        1 2023-06-07 00:38:12.000000 foc-0.1.1/foc.egg-info/dependency_links.txt
--rw-r--r--   0 thyeem     (501) staff       (20)        4 2023-06-07 00:38:12.000000 foc-0.1.1/foc.egg-info/top_level.txt
--rw-r--r--   0 thyeem     (501) staff       (20)      102 2023-06-07 00:38:12.377327 foc-0.1.1/setup.cfg
--rw-r--r--   0 thyeem     (501) staff       (20)      696 2023-06-07 00:37:27.000000 foc-0.1.1/setup.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-12 00:48:24.984709 foc-0.1.2/
+-rw-r--r--   0 thyeem     (501) staff       (20)      164 2023-06-12 00:47:08.000000 foc-0.1.2/ChangeLog.md
+-rw-r--r--   0 thyeem     (501) staff       (20)     1068 2023-05-15 21:22:31.000000 foc-0.1.2/LICENSE
+-rw-r--r--   0 thyeem     (501) staff       (20)       55 2023-06-06 23:18:02.000000 foc-0.1.2/MANIFEST.in
+-rw-r--r--   0 thyeem     (501) staff       (20)      420 2023-06-12 00:48:24.984821 foc-0.1.2/PKG-INFO
+-rw-r--r--   0 thyeem     (501) staff       (20)    16522 2023-06-11 21:45:18.000000 foc-0.1.2/README.md
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-12 00:48:24.982955 foc-0.1.2/foc/
+-rw-r--r--   0 thyeem     (501) staff       (20)    16576 2023-06-11 21:33:00.000000 foc-0.1.2/foc/__init__.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-12 00:48:24.984035 foc-0.1.2/foc.egg-info/
+-rw-r--r--   0 thyeem     (501) staff       (20)      420 2023-06-12 00:48:24.000000 foc-0.1.2/foc.egg-info/PKG-INFO
+-rw-r--r--   0 thyeem     (501) staff       (20)      221 2023-06-12 00:48:24.000000 foc-0.1.2/foc.egg-info/SOURCES.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)        1 2023-06-12 00:48:24.000000 foc-0.1.2/foc.egg-info/dependency_links.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)       10 2023-06-12 00:48:24.000000 foc-0.1.2/foc.egg-info/top_level.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)      102 2023-06-12 00:48:24.985543 foc-0.1.2/setup.cfg
+-rw-r--r--   0 thyeem     (501) staff       (20)      696 2023-06-12 00:43:14.000000 foc-0.1.2/setup.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-06-12 00:48:24.984484 foc-0.1.2/tests/
+-rw-r--r--   0 thyeem     (501) staff       (20)        0 2023-06-11 20:28:50.000000 foc-0.1.2/tests/__init__.py
+-rw-r--r--   0 thyeem     (501) staff       (20)     7973 2023-06-11 21:43:33.000000 foc-0.1.2/tests/test_foc.py
```

### Comparing `foc-0.1.1/LICENSE` & `foc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `foc-0.1.1/README.md` & `foc-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,55 +15,55 @@
 - _Take a look at the examples below._
 
 ### Use
 ```bash
 # install
 $ pip install -U foc
 
-# import (python 3.6+ maybe)
+# import
 >>> from foc import *
 ```
 
+> To list all available functions, call `flist()`.
+
 ### Ground rules
 - Followed `Haskell`-like function names and arguments order
 - Considered using generators first if possible. (_lazy-evaluation_)
 > `map`, `filter`, `zip`, `range`, `flat` ...
 - Provide the functions that unpack generators in `list` as well. (annoying to unpack with `[*]` or `list` every time)
 - Function names that end in `l` indicate the result will be unpacked in a list.
 > `mapl`, `filterl`, `zipl`, `rangel`, `flatl`, ...
 - Function names that end in `_` indicate that the function is a **partial application** (_not-fully-evaluated function_) builder.
 > `f_`, `ff_`, `c_`, `cc_`, `m_`, `v_`, ...
 - Most function implementations _should be less than 5-lines_.
 - No dependencies except for the `Python` standard library
 - No unnessary wrapping objects.
 
 ### Examples
-> To see all available functions, use `flist()`.
-
 __Note__: `foc`'s functions are valid for any _iterable_ such as `list`, `tuple`, `deque`, `set`, `str`, ...
 ```python
 >>> id("francis")
 'francis'
 
 >>> fst(["sofia", "maria", "claire"])
 'sofia'
 
 >>> snd(("sofia", "maria", "claire"))
 'maria'
 
->>> nth(["sofia", "maria", "claire"], 3)    # not list index, but literally n-th
+>>> nth(3, ["sofia", "maria", "claire"])    # not list index, but literally n-th
 'claire'
 
 >>> take(3, range(5, 10))
 [5, 6, 7]
 
->>> list(drop(3, "github"))    # `drop` returns a generator
+>>> list(drop(3, "github"))   # `drop` returns a generator
 ['h', 'u', 'b']
 
->>> head(range(1,5))           # range(1, 5) = [1, 2, 3, 4]
+>>> head(range(1,5))          # range(1, 5) = [1, 2, 3, 4]
 1
 
 >>> last(range(1,5))
 4
 
 >>> list(init(range(1,5)))    # `init` returns a generator
 [1, 2, 3]
@@ -94,27 +94,27 @@
 
 >>> lines("fun\non\nfunctions")
 ['fun', 'on', 'functions']
 
 >>> unlines(['fun', 'on', 'functions'])
 ("fun\non\nfunctions")
 
->>> take(3, repeat(5))    # repeat(5) = [5, 5, ...]
+>>> take(3, repeat(5))        # repeat(5) = [5, 5, ...]
 [5, 5, 5]
 
->>> take(5, cycle("fun"))    # cycle("fun") = ['f', 'u', 'n', 'f', 'u', 'n', ...]
+>>> take(5, cycle("fun"))     # cycle("fun") = ['f', 'u', 'n', 'f', 'u', 'n', ...]
 ['f', 'u', 'n', 'f', 'u']
 
->>> replicate(3, 5)   # the same as 'take(3, repeat(5))'
+>>> replicate(3, 5)           # the same as 'take(3, repeat(5))'
 [5, 5, 5]
 
->>> take(3, count(2))    # count(2) = [2, 3, 4, 5, ...]
+>>> take(3, count(2))         # count(2) = [2, 3, 4, 5, ...]
 [2, 3, 4]
 
->>> take(3, count(2, 3))    # count(2, 3) = [2, 5, 8, 11, ...]
+>>> take(3, count(2, 3))      # count(2, 3) = [2, 5, 8, 11, ...]
 [2, 5, 8]
 ```
 
 #### Build partial application: `f_` and `ff_`
 `f_` takes arguments _from the left_ (left-associative) while `ff_` takes them _from the right_ (right-associative).
 
 > When using `ff_`, passing arguments in reverse order for a long-args function is painful.
@@ -296,50 +296,66 @@
 >>> bimap(f_(op.add, 3), f_(op.mul, 7), (5, 7))    # bimap (3+) (7*) (5, 7)
 (8, 49)                                            # (3+5, 7*7)
 
 >>> first(f_(op.add, 3), (5, 7))                   # first (3+) (5, 7)
 (8, 7)                                             # (3+5, 7)
 
 >>> second(f_(op.mul, 7), (5, 7))                  # second (7*) (5, 7)
-(5, 49)                                             # (5, 7*7)
+(5, 49)                                            # (5, 7*7)
 
 >>> take(5, iterate(lambda x: x**2, 2))            # [2, 2**2, (2**2)**2, ((2**2)**2)**2, ...]
 [2, 4, 16, 256, 65536]
 
 >>> [* takewhile(even, [2, 4, 6, 1, 3, 5]) ]       # `takewhile` returns a generator
 [2, 4, 6]
 
->>> takewhilel(even, [2, 4, 6, 1, 3, 5]) ]
+>>> takewhilel(even, [2, 4, 6, 1, 3, 5])
 [2, 4, 6]
 
 >>> [* dropwhile(even, [2, 4, 6, 1, 3, 5]) ]       # `dropwhile` returns a generator
 [1, 3, 5]
 
->>> dropwhilel(even, [2, 4, 6, 1, 3, 5]) ]
+>>> dropwhilel(even, [2, 4, 6, 1, 3, 5])
 [1, 3, 5]
 
-# fold with a given initial value
->>> fold(op.add, 3, range(1, 6))                   # foldl (+) 3 [1..5]
-18
-
-# fold without an initial (first item used)
->>> fold1(op.add, range(1, 6))                     # foldl1 (+) [1..5]
-15
-
-# scan with a given initial value (see also 'scan')
->>> scanl(op.add, 3, range(1, 6))                  # scanl (+) 3 [1..5]
-[3, 4, 6, 9, 13, 18]
-
-# scan without an initial (see also 'scan1')
->>> scan1l(op.add, range(1, 6))                    # scan1l (+) [1..5]
-[1, 3, 6, 10, 15]
+# fold with a given initial value from the left
+>>> foldl(op.sub, 10, range(1, 5))                 # foldl (-) 10 [1..4]
+0
+
+# fold with a given initial value from the right
+>>> foldr(op.sub, 10, range(1, 5))                 # foldr (-) 10 [1..4]
+8
+
+# `foldl` without an initial value (used first item instead)
+>>> foldl1(op.sub, range(1, 5))                    # foldl1 (-) [1..4]
+-8
+
+# `foldr` without an initial value (used first item instead)
+>>> foldr1(op.sub, range(1, 5))                    # foldr1 (-) [1..4]
+-2
+
+# accumulate reduced values from the left
+>>> scanl(op.sub, 10, range(1, 5))                 # scanl (-) 10 [1..4]
+[10, 9, 7, 4, 0]
+
+# accumulate reduced values from the right
+>>> scanr(op.sub, 10, range(1, 5))                 # scanr (-) 10 [1..4]
+[8, -7, 9, -6, 10]
+
+# `scanl` but no starting value
+>>> scanl1(op.sub, range(1, 5))                    # scanl1 (-) [1..4]
+[1, -1, -4, -8]
+
+# `scanr` but no starting value
+>>> scanr1(op.sub, range(1, 5))                    # scanr1 (-) [1..4]
+[-2, 3, -1, 4]
 
 # See also 'concat' that returns a generator
 >>> concatl(["sofia", "maria"])
-['s', 'o', 'f', 'i', 'a', 'm', 'a', 'r', 'i', 'a'
+['s', 'o', 'f', 'i', 'a', 'm', 'a', 'r', 'i', 'a']
 
 # See also 'concatmap' that returns a generator
 >>> concatmapl(str.upper, ["sofia", "maria"])      # concatmapl = cfd(list, concat)(map)
 ['S', 'O', 'F', 'I', 'A', 'M', 'A', 'R', 'I', 'A']
 ```
 
 #### Lazy Evaluation: `lazy` and `force`
@@ -356,22 +372,22 @@
 >>> r = lazy(pow, 2, 12345)
 >>> r()       # fully evaluate it!
 
 # or
 >>> force(r)  # like Haskell's "force", x `seq` x.
 
 >>> replicate(5, random_int(1, 10))    # wrong. not wanted.
-[7, 7, 7, 7, 7]        # evaluation is not delayed. duplication of the same elements.
+[7, 7, 7, 7, 7]         # evaluation is not delayed. duplication of the same elements.
 
 >>> randos = replicate(5, lazy(random_int, 1, 10))    # [ delayed_fn, delayed_fn .., ]
 
 >>> ml_(force)(randos)  # map 'force' over list of delayed functions
 [6, 2, 5, 1, 9]
 
->>> forcemap(randos)    # the same as ml_(force)(randos)
+>>> mforce(randos)      # the same as ml_(force)(randos)
 [7, 3, 9, 1, 3]         # expected result
 ```
 
 #### Normalize containers: `flat`
 `flat` flattens all kinds of iterables except for string-like object, _regardless of the number of arguments_.
 
 ```python
@@ -413,15 +429,15 @@
 ```
 
 #### Dot-accessible dictionary: `dmap`
 `dmap` is a _yet another_ `dict`. It's exactly the same as `dict` but it enables to access its nested structure with '_dot notations_'.
 
 ```python
 >>> d = dmap(name="yunchan lim", age=19, profession="pianist")
-{'name': 'yunchan lim', 'age': 19, 'profession': 'pianist'
+{'name': 'yunchan lim', 'age': 19, 'profession': 'pianist'}
 
 >>> d.cliburn.semifinal.mozart.concerto = "No.22"
 >>> d.cliburn.final.rachmaninoff = "crazy!"
 
 # pretty-printer
 >>> import json
 >>> pprint = cf_(print, ff_(json.dumps, indent=2)
```

### Comparing `foc-0.1.1/foc/__init__.py` & `foc-0.1.2/foc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import re
 import threading
 from collections import deque
 from datetime import datetime, timedelta
 from functools import cache, partial, reduce, wraps
 from inspect import signature
-from itertools import count, cycle, dropwhile, takewhile
+from itertools import count, cycle, dropwhile, takewhile, tee
 from shutil import rmtree
 from textwrap import fill
 
 __all__ = [
     "flist",
     "op",
     "deque",
@@ -32,19 +32,19 @@
     "odd",
     "even",
     "null",
     "words",
     "unwords",
     "lines",
     "unlines",
-    "iterate",
     "repeat",
     "replicate",
     "cycle",
     "count",
+    "tee",
     "product",
     "flip",
     "f_",
     "ff_",
     "curry",
     "c_",
     "cc_",
@@ -60,39 +60,42 @@
     "vvl_",
     "mapl",
     "filterl",
     "zipl",
     "rangel",
     "enumeratel",
     "reverse",
-    "reversel",
     "sort",
     "takewhile",
     "takewhilel",
     "dropwhile",
     "dropwhilel",
     "bimap",
     "first",
     "second",
-    "fold",
-    "fold1",
-    "scan",
+    "iterate",
+    "foldl",
+    "foldl1",
+    "foldr",
+    "foldr1",
     "scanl",
-    "scan1",
-    "scan1l",
+    "scanl1",
+    "scanr",
+    "scanr1",
     "permutation",
     "combination",
-    "cprod",
+    "cartprod",
+    "cartprodl",
     "concat",
     "concatl",
     "concatmap",
     "concatmapl",
     "lazy",
     "force",
-    "forcemap",
+    "mforce",
     "flat",
     "flatl",
     "flatt",
     "flatd",
     "flats",
     "fread",
     "fwrite",
@@ -221,31 +224,25 @@
     return x.split("\n")
 
 
 def unlines(x):
     return "\n".join(x)
 
 
-def iterate(f, x):
-    while True:
-        yield x
-        x = f(x)
-
-
 def repeat(x):
     return (x for _ in it.count())
 
 
 def replicate(n, x):
     return take(n, repeat(x))
 
 
 def product(x):
     """product of the elements of given iterable"""
-    return fold1(op.mul, x)
+    return foldl1(op.mul, x)
 
 
 def flip(f):
     """flip(f) takes its arguments in the reverse order of f"""
 
     @wraps(f)
     def wrapper(*args, **kwargs):
@@ -391,20 +388,17 @@
 rangel.__doc__ = "unpacks the result in list after `range`"
 
 
 enumeratel = cfd(list)(enumerate)
 enumeratel.__doc__ = "unpacks the result in list after `enumerate`"
 
 
-# for clarity of function names
-reverse = reversed
-
-
-reversel = cfd(list)(reverse)
-reversel.__doc__ = "unpacks the result in list after `reverse`"
+def reverse(x):
+    """returns reversed sequence"""
+    return list(x)[::-1]
 
 
 # "for clarity of function names"
 sort = sorted
 
 
 takewhilel = cfd(list)(takewhile)
@@ -428,52 +422,80 @@
 
 
 def second(g, x):
     """map covariantly over the 'second' argument"""
     return fst(x), g(snd(x))
 
 
-def fold(f, initial, xs):
-    """folding an foldable object from the left. The same as 'foldl' in Haskell"""
+def iterate(f, x):
+    while True:
+        yield x
+        x = f(x)
+
+
+def foldl(f, initial, xs):
+    """left-associative fold of an iterable. The same as 'foldl' in Haskell"""
     return reduce(f, xs, initial)
 
 
-def fold1(f, xs):
-    """equivalent to 'foldl1' in Haskell"""
+def foldl1(f, xs):
+    """`foldl` without initial value. The same as 'foldl1' in Haskell"""
     return reduce(f, xs)
 
 
-def scan(f, initial, xs):
-    """accumulation from the left. Equivalent to 'scanl' in Haskell"""
-    return it.accumulate(xs, f, initial=initial)
+def foldr(f, inital, xs):
+    """right-associative fold of an iterable. The same as 'foldr' in Haskell"""
+    return reduce(flip(f), xs[::-1], inital)
 
 
-def scan1(f, xs):
-    """equivalent to 'scanl1' in Haskell"""
-    return scan(f, None, xs)
+def foldr1(f, xs):
+    """`foldr` without initial value. The same as 'foldr1' in Haskell"""
+    return reduce(flip(f), xs[::-1])
 
 
-scanl = cfd(list)(scan)
-scanl.__doc__ = "unpacks the result in list after `scan`"
+@cfd(list)
+def scanl(f, initial, xs):
+    """returns a list of successive reduced values from the left
+    The same as `scanl` in Haskell"""
+    return it.accumulate(xs, f, initial=initial)
 
 
-scan1l = cfd(list)(scan1)
-scan1l.__doc__ = "unpacks the result in list after `scan1`"
+@cfd(list)
+def scanl1(f, xs):
+    """`scanl` without starting value. The same as 'scanl1' in Haskell"""
+    return it.accumulate(xs, f)
+
+
+@cfd(reverse)
+def scanr(f, initial, xs):
+    """returns a list of successive reduced values from the right
+    The same as `scanr` in Haskell"""
+    return it.accumulate(xs[::-1], flip(f), initial=initial)
+
+
+@cfd(reverse)
+def scanr1(f, xs):
+    """`scanr` without starting value. The same as 'scanr1' in Haskell"""
+    return it.accumulate(xs[::-1], flip(f))
 
 
 def permutation(x, r, rep=False):
     return it.product(x, repeat=r) if rep else it.permutations(x, r)
 
 
 def combination(x, r, rep=False):
     return it.combinations_with_replacement(x, r) if rep else it.combinations(x, r)
 
 
-cprod = ff_(it.product, repeat=1)
-cprod.__doc__ = "returns Cartesian product"
+cartprod = ff_(it.product, repeat=1)
+cartprod.__doc__ = "returns Cartesian product"
+
+
+cartprodl = cfd(list)(cartprod)
+cartprodl.__doc__ = "unpacks the result in list after `cartprod`"
 
 
 # concatenates all elements of iterables"
 concat = it.chain.from_iterable
 
 
 concatl = cfd(list)(concat)
@@ -498,16 +520,16 @@
 
 
 def force(x, *args, **kwargs):
     """forces the delayed-expression to be fully evaluated"""
     return x(*args, **kwargs) if callable(x) else x
 
 
-forcemap = ml_(force)
-forcemap.__doc__ = "map 'force' over iterables of delayed-evaluation"
+mforce = ml_(force)
+mforce.__doc__ = "map 'force' over iterables of delayed-evaluation"
 
 
 def _is_ns_iter(x):
     """check if the given is a non-string-like iterable"""
     return all(
         (
             hasattr(x, "__iter__"),
@@ -576,15 +598,15 @@
     """split interables into the given `n-length` pieces"""
     return it.zip_longest(*(iter(x),) * n, fillvalue=fill)
 
 
 def capture(p, string):
     x = captures(p, string)
     if x:
-        return x.pop()
+        return fst(x)
 
 
 def captures(p, string):
     return re.compile(p).findall(string)
 
 
 def error(str, e=Exception):
@@ -791,12 +813,12 @@
             return signature(o).__str__()
         except:
             return " is valid, but live-inspect not available"
 
     return dmap({x: x + sig(eval(x)) for x in __all__[3:]})
 
 
-def flist(o=False):
-    if o:
+def flist(to_dict=False):
+    if to_dict:
         return __sig__()
     else:
         nprint(__sig__(), _indent=14)
```

### Comparing `foc-0.1.1/setup.py` & `foc-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_decription = f.read()
 
 setuptools.setup(
     name="foc",
-    version="0.1.1",
+    version="0.1.2",
     author="Francis Lim",
     author_email="thyeem@gmail.com",
     description="A collection of python functions for somebody's sanity",
     long_decription=long_decription,
     long_decription_content_type="text/markdown",
     install_requires=[],
     url="https://github.com/thyeem/foc",
```

