# Comparing `tmp/pycse-2.2.0.tar.gz` & `tmp/pycse-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycse-2.2.0.tar", last modified: Wed Feb  1 16:38:13 2023, max compression
+gzip compressed data, was "pycse-2.2.3.tar", last modified: Mon Jun 12 12:42:28 2023, max compression
```

## Comparing `pycse-2.2.0.tar` & `pycse-2.2.3.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 jkitchin   (501) staff       (20)        0 2023-02-01 16:38:13.679810 pycse-2.2.0/
--rw-r--r--   0 jkitchin   (501) staff       (20)    18091 2021-06-26 14:31:14.000000 pycse-2.2.0/LICENSE
--rw-r--r--   0 jkitchin   (501) staff       (20)      528 2023-02-01 16:38:13.679876 pycse-2.2.0/PKG-INFO
-drwxr-xr-x   0 jkitchin   (501) staff       (20)        0 2023-02-01 16:38:13.678996 pycse-2.2.0/pycse/
--rw-r--r--   0 jkitchin   (501) staff       (20)    10410 2022-05-28 15:39:58.000000 pycse-2.2.0/pycse/PYCSE.py
--rw-r--r--   0 jkitchin   (501) staff       (20)     2567 2023-01-31 00:13:12.000000 pycse-2.2.0/pycse/__init__.py
--rw-r--r--   0 jkitchin   (501) staff       (20)     5356 2022-04-27 14:20:10.000000 pycse-2.2.0/pycse/beginner.py
--rw-r--r--   0 jkitchin   (501) staff       (20)    19347 2022-05-22 16:38:59.000000 pycse-2.2.0/pycse/colab.py
--rw-r--r--   0 jkitchin   (501) staff       (20)    34116 2022-04-25 17:32:11.000000 pycse-2.2.0/pycse/colors.py
--rw-r--r--   0 jkitchin   (501) staff       (20)     6126 2023-01-31 00:28:40.000000 pycse-2.2.0/pycse/hashcache.py
--rw-r--r--   0 jkitchin   (501) staff       (20)     6753 2022-05-22 16:38:58.000000 pycse-2.2.0/pycse/lisp.py
--rw-r--r--   0 jkitchin   (501) staff       (20)      726 2022-05-22 16:38:58.000000 pycse-2.2.0/pycse/obipython.py
--rw-r--r--   0 jkitchin   (501) staff       (20)     6424 2022-05-22 16:38:58.000000 pycse-2.2.0/pycse/orgmode.py
--rw-r--r--   0 jkitchin   (501) staff       (20)     6897 2022-05-22 16:38:58.000000 pycse-2.2.0/pycse/orgmode_v1.py
--rw-r--r--   0 jkitchin   (501) staff       (20)      857 2023-01-31 00:05:39.000000 pycse-2.2.0/pycse/plotly.py
--rw-r--r--   0 jkitchin   (501) staff       (20)      714 2022-04-25 23:28:56.000000 pycse-2.2.0/pycse/sandbox.py
--rw-r--r--   0 jkitchin   (501) staff       (20)     3333 2022-07-18 13:27:29.000000 pycse-2.2.0/pycse/search.py
--rw-r--r--   0 jkitchin   (501) staff       (20)     2136 2022-05-22 16:38:58.000000 pycse-2.2.0/pycse/utils.py
-drwxr-xr-x   0 jkitchin   (501) staff       (20)        0 2023-02-01 16:38:13.679698 pycse-2.2.0/pycse.egg-info/
--rw-r--r--   0 jkitchin   (501) staff       (20)      528 2023-02-01 16:38:13.000000 pycse-2.2.0/pycse.egg-info/PKG-INFO
--rw-r--r--   0 jkitchin   (501) staff       (20)      422 2023-02-01 16:38:13.000000 pycse-2.2.0/pycse.egg-info/SOURCES.txt
--rw-r--r--   0 jkitchin   (501) staff       (20)        1 2023-02-01 16:38:13.000000 pycse-2.2.0/pycse.egg-info/dependency_links.txt
--rw-r--r--   0 jkitchin   (501) staff       (20)       25 2023-02-01 16:38:13.000000 pycse-2.2.0/pycse.egg-info/requires.txt
--rw-r--r--   0 jkitchin   (501) staff       (20)        6 2023-02-01 16:38:13.000000 pycse-2.2.0/pycse.egg-info/top_level.txt
--rw-r--r--   0 jkitchin   (501) staff       (20)       13 2022-05-22 16:36:42.000000 pycse-2.2.0/requirements.txt
--rw-r--r--   0 jkitchin   (501) staff       (20)      251 2023-02-01 16:38:13.680155 pycse-2.2.0/setup.cfg
--rw-r--r--   0 jkitchin   (501) staff       (20)     1120 2023-01-31 00:12:06.000000 pycse-2.2.0/setup.py
+drwxr-xr-x   0 jkitchin   (501) staff       (20)        0 2023-06-12 12:42:28.422922 pycse-2.2.3/
+-rw-r--r--   0 jkitchin   (501) staff       (20)    18091 2021-06-26 14:31:14.000000 pycse-2.2.3/LICENSE
+-rw-r--r--   0 jkitchin   (501) staff       (20)      527 2023-06-12 12:42:28.423026 pycse-2.2.3/PKG-INFO
+drwxr-xr-x   0 jkitchin   (501) staff       (20)        0 2023-06-12 12:42:28.421047 pycse-2.2.3/pycse/
+-rw-r--r--   0 jkitchin   (501) staff       (20)    10413 2023-06-11 20:54:31.000000 pycse-2.2.3/pycse/PYCSE.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)     2567 2023-02-01 22:27:33.000000 pycse-2.2.3/pycse/__init__.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)     5165 2023-06-11 17:37:43.000000 pycse-2.2.3/pycse/beginner.py
+-rwxr-xr-x   0 jkitchin   (501) staff       (20)     3032 2023-06-12 12:37:32.000000 pycse-2.2.3/pycse/cli.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)    19347 2022-05-22 16:38:59.000000 pycse-2.2.3/pycse/colab.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)    34116 2022-04-25 17:32:11.000000 pycse-2.2.3/pycse/colors.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)     6387 2023-06-11 15:24:44.000000 pycse-2.2.3/pycse/hashcache.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)     6753 2022-05-22 16:38:58.000000 pycse-2.2.3/pycse/lisp.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)      726 2022-05-22 16:38:58.000000 pycse-2.2.3/pycse/obipython.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)     6424 2022-05-22 16:38:58.000000 pycse-2.2.3/pycse/orgmode.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)     6897 2022-05-22 16:38:58.000000 pycse-2.2.3/pycse/orgmode_v1.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)      857 2023-01-31 00:05:57.000000 pycse-2.2.3/pycse/plotly.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)      714 2022-04-25 23:28:56.000000 pycse-2.2.3/pycse/sandbox.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)     3333 2022-07-18 13:27:29.000000 pycse-2.2.3/pycse/search.py
+-rw-r--r--   0 jkitchin   (501) staff       (20)     2136 2022-05-22 16:38:58.000000 pycse-2.2.3/pycse/utils.py
+drwxr-xr-x   0 jkitchin   (501) staff       (20)        0 2023-06-12 12:42:28.422686 pycse-2.2.3/pycse.egg-info/
+-rw-r--r--   0 jkitchin   (501) staff       (20)      527 2023-06-12 12:42:28.000000 pycse-2.2.3/pycse.egg-info/PKG-INFO
+-rw-r--r--   0 jkitchin   (501) staff       (20)      467 2023-06-12 12:42:28.000000 pycse-2.2.3/pycse.egg-info/SOURCES.txt
+-rw-r--r--   0 jkitchin   (501) staff       (20)        1 2023-06-12 12:42:28.000000 pycse-2.2.3/pycse.egg-info/dependency_links.txt
+-rw-r--r--   0 jkitchin   (501) staff       (20)       42 2023-06-12 12:42:28.000000 pycse-2.2.3/pycse.egg-info/entry_points.txt
+-rw-r--r--   0 jkitchin   (501) staff       (20)       25 2023-06-12 12:42:28.000000 pycse-2.2.3/pycse.egg-info/requires.txt
+-rw-r--r--   0 jkitchin   (501) staff       (20)        6 2023-06-12 12:42:28.000000 pycse-2.2.3/pycse.egg-info/top_level.txt
+-rw-r--r--   0 jkitchin   (501) staff       (20)       27 2023-06-11 15:25:22.000000 pycse-2.2.3/requirements.txt
+-rw-r--r--   0 jkitchin   (501) staff       (20)      271 2023-06-12 12:42:28.423463 pycse-2.2.3/setup.cfg
+-rw-r--r--   0 jkitchin   (501) staff       (20)     1187 2023-06-12 12:40:06.000000 pycse-2.2.3/setup.py
```

### Comparing `pycse-2.2.0/LICENSE` & `pycse-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycse-2.2.0/PKG-INFO` & `pycse-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycse
-Version: 2.2.0
+Version: 2.2.3
 Summary: python computations in science and engineering
 Home-page: https://github.com/jkitchin/pycse
 Maintainer: John Kitchin
 Maintainer-email: jkitchin@andrew.cmu.edu
 License: GPL
 Platform: linux
 License-File: LICENSE
@@ -14,8 +14,7 @@
 
 This package provides functions that are useful in science and engineering
 computations.
 
 See https://kitchingroup.cheme.cmu.edu/pycse for documentation.
 
       
-
```

### Comparing `pycse-2.2.0/pycse/PYCSE.py` & `pycse-2.2.3/pycse/PYCSE.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,16 +235,16 @@
 
 
 def nlpredict(X, y, model, loss, popt, xnew, alpha=0.05, ub=1e-5, ef=1.05):
     """Prediction error for a nonlinear fit.
 
     Parameters
     ----------
-    model : model function with signature model(x, *p)
-    loss : loss function the model was fitted with loss(*p)
+    model : model function with signature model(x, ...)
+    loss : loss function the model was fitted with loss(...)
     popt : the optimized paramters
     xnew : x-values to predict at
     alpha : confidence level, 95% = 0.05
     ub : upper bound for smallest allowed Hessian eigenvalue
     ef : eigenvalue factor for scaling Hessian
 
     This function uses numdifftools for the Hessian and Jacobian.
@@ -298,15 +298,15 @@
 
 
 def bic(x, y, model, popt):
     """Compute the Bayesian information criterion (BIC).
 
     Parameters
     ----------
-    model : function(x, *p) returns prediction for y
+    model : function(x, ...) returns prediction for y
     popt : optimal parameters
     y : array, known y-values
 
     Returns
     -------
     BIC : float
```

### Comparing `pycse-2.2.0/pycse/__init__.py` & `pycse-2.2.3/pycse/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Python calculations in Science and Engineering.
 
 Pycse is compatible with Python 3.6+.
 
 """
 
-__version__ = "2.1.9"
+__version__ = "2.2.1"
 
 # * Setup inline images for IPython
 # Make inline figures the default
 
 from .PYCSE import (
     polyfit,
     regress,
```

### Comparing `pycse-2.2.0/pycse/beginner.py` & `pycse-2.2.3/pycse/beginner.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,113 +6,113 @@
 
 There are a series of functions to access parts of a list, e.g. the first-fifth
 and nth elements, the last element, all but the first, and all but the last
 elements. There is also a cut function to avoid list slicing syntax. The point
 of these is to delay introducing indexing syntax.
 
 """
-import collections
-import numpy as np
+import collections.abc
 from scipy.optimize import fsolve as _fsolve
 from scipy.integrate import quad
 
 
 def first(x):
     """Return the first element of x if it is iterable, else return x."""
-    if not isinstance(x, collections.Iterable):
+    if not isinstance(x, collections.abc.Iterable):
         raise Exception("{} is not iterable.".format(x))
 
     return x[0]
 
 
 def second(x):
     """Return the second element of x."""
-    if not isinstance(x, collections.Iterable):
+    if not isinstance(x, collections.abc.Iterable):
         raise Exception("{} is not iterable.".format(x))
 
     if not len(x) >= 2:
         raise Exception("{} does not have a second element.".format(x))
 
     return x[1]
 
 
 def third(x):
     """Return the third element of x."""
-    if not isinstance(x, collections.Iterable):
+    if not isinstance(x, collections.abc.Iterable):
         raise Exception("{} is not iterable.".format(x))
 
     if not len(x) >= 3:
         raise Exception("{} does not have a third element.".format(x))
 
     return x[2]
 
 
 def fourth(x):
     """Return the fourth element of x."""
-    if not isinstance(x, collections.Iterable):
+    if not isinstance(x, collections.abc.Iterable):
         raise Exception("{} is not iterable.".format(x))
 
     if not len(x) >= 4:
         raise Exception("{} does not have a fourth element.".format(x))
 
     return x[3]
 
 
 def fifth(x):
     """Return the fifth element of x."""
-    if not isinstance(x, collections.Iterable):
+    if not isinstance(x, collections.abc.Iterable):
         raise Exception("{} is not iterable.".format(x))
 
     if not len(x) >= 5:
         raise Exception("{} does not have a fifth element.".format(x))
 
     return x[4]
 
 
 def nth(x, n=0):
-    """Return the nth value of x."""
-    if not isinstance(x, collections.Iterable):
+    """Return the nth value of x.
+    Note that `n` starts at 0."""
+    if not isinstance(x, collections.abc.Iterable):
         raise Exception("{} is not iterable.".format(x))
 
     if not len(x) >= n:
         raise Exception("{} does not have an n={} element.".format(x, n))
 
     return x[n]
 
 
 def cut(x, start=0, stop=None, step=None):
     """Alias for x[start:stop:step].
 
     This is to avoid having to introduce the slicing syntax.
     """
-    if not isinstance(x, collections.Iterable):
+    if not isinstance(x, collections.abc.Iterable):
         raise Exception("{} is not iterable.".format(x))
 
     return x[slice(start, stop, step)]
 
 
 def last(x):
     """Return the last element of x if it is iterable."""
-    if not isinstance(x, collections.Iterable):
+    if not isinstance(x, collections.abc.Iterable):
         raise Exception("{} is not iterable.".format(x))
 
     return x[-1]
 
 
 def rest(x):
     """Return everything after the first element of x."""
-    if not isinstance(x, collections.Iterable):
+    if not isinstance(x, collections.abc.Iterable):
         raise Exception("{} is not iterable.".format(x))
 
     return x[1:]
 
 
 def butlast(x):
     """Return everything but the last element of x."""
-    if not isinstance(x, collections.Iterable):
+    if not isinstance(x, collections.abc.Iterable):
         raise Exception("{} is not iterable.".format(x))
 
     return x[0:-1]
 
 
 # * Wrapped functions
 
@@ -175,20 +175,7 @@
     if second(results) > tolerance:
         raise Exception(
             "Your integral error {} is too large. ".format(second(results))
             + "{} ".format(fourth(results))
             + "See your instructor for help"
         )
     return first(results)
-
-
-def heaviside(x):
-    """Return the heaviside function of x.
-
-    This is equal to zero for x < 0, 0.5 for x==0, and 1 for x > 0.
-    """
-    return 0.5 * (np.sign(x) + 1)
-
-
-def step(x):
-    """Alias for heaviside(x)."""
-    return heaviside(x)
```

### Comparing `pycse-2.2.0/pycse/colab.py` & `pycse-2.2.3/pycse/colab.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.0/pycse/colors.py` & `pycse-2.2.3/pycse/colors.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.0/pycse/hashcache.py` & `pycse-2.2.3/pycse/hashcache.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,18 +55,20 @@
 def get_hash(func, args, kwargs):
     g = dict(inspect.getmembers(func))["__globals__"]
 
     return joblib.hash(
         [
             func.__code__.co_name,  # This is the function name
             func.__code__.co_varnames,  # names of arguments,
-            func.__code__.co_names,  # these are other things than
-            # args, usually outside vars
-            # I don't know how to get their values though
-            [g[var] for var in func.__code__.co_names],
+            func.__code__.co_names,  # these are other things than args, usually
+            # outside vars This usually gets a value. But, it includes things
+            # like print, which are not variables. I don't know all the
+            # variations that might be included, so we just pass on things that
+            # aren't there with None. That is a weakness.
+            [g.get(var, None) for var in func.__code__.co_names],
             func.__code__.co_code,
             args,
             kwargs,
         ],
         hash_name="sha1",
     )
 
@@ -137,15 +139,17 @@
             os.makedirs(hshdir, exist_ok=True)
             g = dict(inspect.getmembers(func))["__globals__"]
             data = {
                 "output": value,
                 "args": args,
                 "arg-names": func.__code__.co_names,
                 "other-names": func.__code__.co_names,
-                "other-values": [g[var] for var in func.__code__.co_names],
+                "other-values": [
+                    g.get(var, None) for var in func.__code__.co_names
+                ],
                 "kwargs": kwargs,
                 "cwd": os.getcwd(),  # Is this a good idea? Could it leak
                 # sensitive information from the path?
                 # should we include other info like
                 # hostname?
                 "user": os.getlogin(),
                 "run-at": t0,
```

### Comparing `pycse-2.2.0/pycse/lisp.py` & `pycse-2.2.3/pycse/lisp.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.0/pycse/obipython.py` & `pycse-2.2.3/pycse/obipython.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.0/pycse/orgmode.py` & `pycse-2.2.3/pycse/orgmode.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.0/pycse/orgmode_v1.py` & `pycse-2.2.3/pycse/orgmode_v1.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.0/pycse/plotly.py` & `pycse-2.2.3/pycse/plotly.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.0/pycse/sandbox.py` & `pycse-2.2.3/pycse/sandbox.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.0/pycse/search.py` & `pycse-2.2.3/pycse/search.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.0/pycse/utils.py` & `pycse-2.2.3/pycse/utils.py`

 * *Files identical despite different names*

### Comparing `pycse-2.2.0/pycse.egg-info/PKG-INFO` & `pycse-2.2.3/pycse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycse
-Version: 2.2.0
+Version: 2.2.3
 Summary: python computations in science and engineering
 Home-page: https://github.com/jkitchin/pycse
 Maintainer: John Kitchin
 Maintainer-email: jkitchin@andrew.cmu.edu
 License: GPL
 Platform: linux
 License-File: LICENSE
@@ -14,8 +14,7 @@
 
 This package provides functions that are useful in science and engineering
 computations.
 
 See https://kitchingroup.cheme.cmu.edu/pycse for documentation.
 
       
-
```

### Comparing `pycse-2.2.0/setup.py` & `pycse-2.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # Copyright 2015-2021 John Kitchin
 # (see accompanying license files for details).
 from setuptools import setup
 
 setup(
     name="pycse",
-    version="2.2.0",
+    version="2.2.3",
     description="python computations in science and engineering",
     url="https://github.com/jkitchin/pycse",
     maintainer="John Kitchin",
     maintainer_email="jkitchin@andrew.cmu.edu",
     license="GPL",
     platforms=["linux"],
     packages=["pycse"],
     setup_requires=["nose>=1.0"],
     data_files=["requirements.txt", "LICENSE"],
     install_requires=["numpy", "scipy", "numdifftools"],
+    entry_points={"console_scripts": ["pycse = pycse.cli:pycse"]},
     long_description="""\
 python computations in science and engineering
 ===============================================
 
 This package provides functions that are useful in science and engineering
 computations.
```

