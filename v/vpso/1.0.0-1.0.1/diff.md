# Comparing `tmp/vpso-1.0.0.tar.gz` & `tmp/vpso-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vpso-1.0.0.tar", last modified: Sun Jun 11 15:13:06 2023, max compression
+gzip compressed data, was "vpso-1.0.1.tar", last modified: Mon Jun 12 16:37:50 2023, max compression
```

## Comparing `vpso-1.0.0.tar` & `vpso-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 15:13:06.249745 vpso-1.0.0/
--rw-rw-rw-   0        0        0     1093 2023-06-06 07:34:41.000000 vpso-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3573 2023-06-11 15:13:06.247746 vpso-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2872 2023-06-11 14:02:36.000000 vpso-1.0.0/README.md
--rw-rw-rw-   0        0        0      975 2023-06-11 15:09:34.000000 vpso-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-11 15:13:06.249745 vpso-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-11 15:13:06.167644 vpso-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 15:13:06.209306 vpso-1.0.0/src/vpso/
--rw-rw-rw-   0        0        0       50 2023-06-06 08:52:06.000000 vpso-1.0.0/src/vpso/__init__.py
--rw-rw-rw-   0        0        0     5009 2023-06-10 18:52:17.000000 vpso-1.0.0/src/vpso/adaptation.py
--rw-rw-rw-   0        0        0     5107 2023-06-10 18:52:27.000000 vpso-1.0.0/src/vpso/ask_and_tell.py
--rw-rw-rw-   0        0        0     3916 2023-06-10 10:39:45.000000 vpso-1.0.0/src/vpso/initialization.py
--rw-rw-rw-   0        0        0     3070 2023-06-10 18:52:34.000000 vpso-1.0.0/src/vpso/jit.py
--rw-rw-rw-   0        0        0     4668 2023-06-10 18:49:31.000000 vpso-1.0.0/src/vpso/math.py
--rw-rw-rw-   0        0        0     3748 2023-06-10 18:52:54.000000 vpso-1.0.0/src/vpso/mutation.py
--rw-rw-rw-   0        0        0     3268 2023-06-10 18:52:44.000000 vpso-1.0.0/src/vpso/reparation.py
--rw-rw-rw-   0        0        0      225 2023-06-08 20:48:48.000000 vpso-1.0.0/src/vpso/typing.py
--rw-rw-rw-   0        0        0     6067 2023-06-11 14:42:53.000000 vpso-1.0.0/src/vpso/vpso.py
-drwxrwxrwx   0        0        0        0 2023-06-11 15:13:06.224367 vpso-1.0.0/src/vpso.egg-info/
--rw-rw-rw-   0        0        0     3573 2023-06-11 15:13:06.000000 vpso-1.0.0/src/vpso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      545 2023-06-11 15:13:06.000000 vpso-1.0.0/src/vpso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 15:13:06.000000 vpso-1.0.0/src/vpso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-11 15:13:06.000000 vpso-1.0.0/src/vpso.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-11 15:13:06.000000 vpso-1.0.0/src/vpso.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 15:13:06.245742 vpso-1.0.0/tests/
--rw-rw-rw-   0        0        0     4245 2023-06-10 16:34:01.000000 vpso-1.0.0/tests/test_adaptation.py
--rw-rw-rw-   0        0        0     1201 2023-06-10 15:53:49.000000 vpso-1.0.0/tests/test_initialization.py
--rw-rw-rw-   0        0        0     2893 2023-06-10 15:56:08.000000 vpso-1.0.0/tests/test_math.py
--rw-rw-rw-   0        0        0     3669 2023-06-10 15:56:14.000000 vpso-1.0.0/tests/test_mutation.py
--rw-rw-rw-   0        0        0     2075 2023-06-11 14:10:49.000000 vpso-1.0.0/tests/test_numerical.py
--rw-rw-rw-   0        0        0     3211 2023-06-10 15:56:23.000000 vpso-1.0.0/tests/test_reparation.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:37:50.423300 vpso-1.0.1/
+-rw-rw-rw-   0        0        0     1093 2023-06-06 07:34:41.000000 vpso-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3573 2023-06-12 16:37:50.421043 vpso-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2872 2023-06-11 14:02:36.000000 vpso-1.0.1/README.md
+-rw-rw-rw-   0        0        0      975 2023-06-12 16:09:23.000000 vpso-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 16:37:50.423800 vpso-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 16:37:50.334618 vpso-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 16:37:50.383369 vpso-1.0.1/src/vpso/
+-rw-rw-rw-   0        0        0       50 2023-06-06 08:52:06.000000 vpso-1.0.1/src/vpso/__init__.py
+-rw-rw-rw-   0        0        0     5630 2023-06-12 15:35:37.000000 vpso-1.0.1/src/vpso/adaptation.py
+-rw-rw-rw-   0        0        0     5419 2023-06-11 16:30:12.000000 vpso-1.0.1/src/vpso/ask_and_tell.py
+-rw-rw-rw-   0        0        0     5099 2023-06-11 17:50:23.000000 vpso-1.0.1/src/vpso/initialization.py
+-rw-rw-rw-   0        0        0     3470 2023-06-12 15:29:16.000000 vpso-1.0.1/src/vpso/jit.py
+-rw-rw-rw-   0        0        0     4668 2023-06-11 16:30:12.000000 vpso-1.0.1/src/vpso/math.py
+-rw-rw-rw-   0        0        0     3748 2023-06-11 16:30:12.000000 vpso-1.0.1/src/vpso/mutation.py
+-rw-rw-rw-   0        0        0     3268 2023-06-11 16:30:12.000000 vpso-1.0.1/src/vpso/reparation.py
+-rw-rw-rw-   0        0        0     5511 2023-06-12 15:47:43.000000 vpso-1.0.1/src/vpso/termination.py
+-rw-rw-rw-   0        0        0      295 2023-06-12 15:05:01.000000 vpso-1.0.1/src/vpso/typing.py
+-rw-rw-rw-   0        0        0     7929 2023-06-12 16:32:33.000000 vpso-1.0.1/src/vpso/vpso.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:37:50.399687 vpso-1.0.1/src/vpso.egg-info/
+-rw-rw-rw-   0        0        0     3573 2023-06-12 16:37:50.000000 vpso-1.0.1/src/vpso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2023-06-12 16:37:50.000000 vpso-1.0.1/src/vpso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 16:37:50.000000 vpso-1.0.1/src/vpso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-12 16:37:50.000000 vpso-1.0.1/src/vpso.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-12 16:37:50.000000 vpso-1.0.1/src/vpso.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 16:37:50.417580 vpso-1.0.1/tests/
+-rw-rw-rw-   0        0        0     4314 2023-06-12 15:49:15.000000 vpso-1.0.1/tests/test_adaptation.py
+-rw-rw-rw-   0        0        0     1201 2023-06-10 15:53:49.000000 vpso-1.0.1/tests/test_initialization.py
+-rw-rw-rw-   0        0        0     2893 2023-06-10 15:56:08.000000 vpso-1.0.1/tests/test_math.py
+-rw-rw-rw-   0        0        0     3669 2023-06-10 15:56:14.000000 vpso-1.0.1/tests/test_mutation.py
+-rw-rw-rw-   0        0        0     2119 2023-06-12 15:53:52.000000 vpso-1.0.1/tests/test_numerical.py
+-rw-rw-rw-   0        0        0     3211 2023-06-10 15:56:23.000000 vpso-1.0.1/tests/test_reparation.py
```

### Comparing `vpso-1.0.0/LICENSE` & `vpso-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vpso-1.0.0/PKG-INFO` & `vpso-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vpso
-Version: 1.0.0
+Version: 1.0.1
 Summary: Multiple Particle Swarm Optimization
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/vectorized-particle-swarm
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/vectorized-particle-swarm/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vpso-1.0.0/README.md` & `vpso-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `vpso-1.0.0/pyproject.toml` & `vpso-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vpso"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Filippo Airaldi", email="filippoairaldi@gmail.com" },
 ]
 description = "Multiple Particle Swarm Optimization"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "MIT" }
```

### Comparing `vpso-1.0.0/src/vpso/adaptation.py` & `vpso-1.0.1/src/vpso/adaptation.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 ----------
 [1] Z. H. Zhan, J. Zhang, Y. Li and H. S. H. Chung, "Adaptive Particle Swarm
     Optimization," in IEEE Transactions on Systems, Man, and Cybernetics, Part B
     (Cybernetics), vol. 39, no. 6, pp. 1362-1381, Dec. 2009,
     doi: 10.1109/TSMCB.2009.2015956.
 """
 
+import logging
+
 import numpy as np
 
-from vpso.jit import jit
+from vpso.jit import _int, jit
 from vpso.math import batch_cdist, batch_pdist, batch_squareform
 from vpso.typing import Array1d, Array2d, Array3d
 
 
 @jit
 def adaptation_strategy(f: Array1d) -> Array2d:
     """Picks the adaptation strategy for each problem based on the ratio of average
@@ -44,25 +46,28 @@
     deltas = np.where(f < 0.5, [(0.5, -0.5)], deltas)  # S2
     deltas = np.where(f < 7 / 30, [(0.5, 0.5)], deltas)  # S3
     return deltas
 
 
 @jit
 def perform_adaptation(
+    nvec: int,
     w: Array3d,
     c1: Array3d,
     c2: Array3d,
     stage: Array1d,
     np_random: np.random.Generator,
 ) -> tuple[Array3d, Array3d, Array3d]:
     """Performs the adaptation of the parameters `w`, `c1` and `c2` based on the
     stage of the algorithm.
 
     Parameters
     ----------
+    nvec : int
+        Number of vectorized problems.
     w : 3d array
         Inertia weight. An array of shape `(N, 1, 1)`, where each element is used for
         the corresponding problem.
     c1 : 3d array
         Cognitive weight. An array of shape `(N, 1, 1)`, where each element is used for
         the corresponding problem.
     c2 : 3d array
@@ -80,44 +85,48 @@
         The newly adapted parameters `w`, `c1` and `c2`.
     """
     # adapt w
     w = (1 / (1 + 1.5 * np.exp(-2.6 * stage)))[:, np.newaxis, np.newaxis]
 
     # adapt c1 and c2
     deltas = adaptation_strategy(stage) * np_random.uniform(
-        0.05, 0.1, size=(w.shape[0], 1)
+        0.05, 0.1, size=(nvec, _int(1))
     )
     c1 = (c1 + deltas[:, 0, np.newaxis, np.newaxis]).clip(1.5, 2.5)
     c2 = (c2 + deltas[:, 1, np.newaxis, np.newaxis]).clip(1.5, 2.5)
     sum_c = c1 + c2
     mask = sum_c > 4
     c1 = np.where(mask, 4 * c1 / sum_c, c1)
     c2 = np.where(mask, 4 * c2 / sum_c, c2)
     return w, c1, c2
 
 
 def adapt(
     px: Array3d,
     sx: Array3d,
+    nvec: int,
     swarmsize: int,
     lb: Array3d,
     ub: Array3d,
     w: Array3d,
     c1: Array3d,
     c2: Array3d,
     np_random: np.random.Generator,
+    logger: logging.Logger,
 ) -> tuple[Array3d, Array3d, Array3d]:
     """Adapts the parameters `w`, `c1` and `c2` on-line.
 
     Parameters
     ----------
     px : 3d array
         Best positions of the particles so far. An array of shape `(N, M, d)`.
     sx : 3d array
         Social best, i.e., the best particle so far. An array of shape `(N, 1, d)`.
+    nvec : int
+        Number of vectorized problems.
     swarmsize : int
         Number of particles in the swarm.
     lb : 3d array
         Lower bound of the search space. An array of shape `(N, 1, d)`.
     ub : 3d array
         Upper bound of the search space. An array of shape `(N, 1, d)`.
     w : 3d array
@@ -127,22 +136,37 @@
         Cognitive weight. An array of shape `(N, 1, 1)`, where each element is used for
         the corresponding problem.
     c2 : 3d array
         Social weight. An array of shape `(N, 1, 1)`, where each element is used for
         the corresponding problem.
     np_random : np.random.Generator
         Random number generator.
+    logger : logging.Logger
+        Logger object.
 
     Returns
     -------
     tuple of 3d arrays
         The newly adapted parameters `w`, `c1` and `c2`.
     """
     domain = ub - lb
     px_normalized = px / domain
     sx_normalized = sx / domain
     D = batch_squareform(batch_pdist(px_normalized)).sum(2) / (swarmsize - 1)
     Dmin = D.min(1)
     Dmax = D.max(1)
     G = batch_cdist(px_normalized, sx_normalized).mean((1, 2))
     stage = (G - Dmin) / (Dmax - Dmin + 1e-32)
-    return perform_adaptation(w, c1, c2, stage, np_random)
+    w_new, c1_new, c2_new = perform_adaptation(nvec, w, c1, c2, stage, np_random)
+
+    if logger.level <= logging.DEBUG:
+        logger.debug(
+            "adaptation: w ∈ [%e, %e], c1 ∈ [%e, %e], c2 ∈ [%e, %e]",
+            w_new.min(),
+            w_new.max(),
+            c1_new.min(),
+            c1_new.max(),
+            c2_new.min(),
+            c2_new.max(),
+        )
+
+    return w_new, c1_new, c2_new
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vpso-1.0.0/src/vpso/ask_and_tell.py` & `vpso-1.0.1/src/vpso/ask_and_tell.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 import numpy as np
 
 from vpso.jit import jit
 from vpso.math import pso_equation
 from vpso.mutation import mutate
 from vpso.reparation import repair_out_of_bounds
 from vpso.typing import Array1d, Array2d, Array3d
@@ -111,32 +113,41 @@
     """
     improvement_mask = f < pf
     px = np.where(improvement_mask[:, :, np.newaxis], x, px)
     pf = np.where(improvement_mask, f, pf)
     return px, pf
 
 
-def get_best(px: Array3d, pf: Array2d, nvec: int) -> tuple[Array3d, Array1d]:
+def get_best(
+    px: Array3d, pf: Array2d, nvec: int, logger: logging.Logger, iter: int
+) -> tuple[Array3d, Array1d]:
     """Returns the best particle and its value for each problem.
 
     Parameters
     ----------
     px : 3d array
         Best positions of the particles so far. An array of shape `(N, M, d)`, where `N`
         is the number of vectorized problems to solve simultaneously, `M` is the number
         of particles in the swarm, and `d` is the dimension of the search space.
     pf : 2d array
         Best values of the particles so far. An array of shape `(N, M)`.
     nvec : int
         Number of vectorized problems.
+    logger : logging.Logger
+        Logger object.
+    iter : int
+        Current iteration. Only used for logging.
 
     Returns
     -------
     tuple of 3d and 1d arrays
         The best particle and its value for each problem with shape `(N, 1, d)` and
         `(N,)`, respectively.
     """
     idx = np.arange(nvec)
     k = pf.argmin(1)
     sx = px[idx, np.newaxis, k]  # (social/global) best particle
     sf = pf[idx, k]  # (social/global) best value
+
+    if logger.level <= logging.INFO:
+        logger.info("best values at iteration %i ∈ [%e, %e]", iter, sf.min(), sf.max())
     return sx, sf
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vpso-1.0.0/src/vpso/initialization.py` & `vpso-1.0.1/src/vpso/initialization.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,46 @@
 from numbers import Number
-from typing import Union
+from typing import Literal, Union
 
 import numpy as np
 from scipy.stats.qmc import LatinHypercube
 
-from vpso.typing import Array1d, Array2d, Array3d
+from vpso.typing import Array1d, Array1i, Array2d, Array3d
+
+
+def _asarray(val, nvec, dtype, ndim: Literal[1, 3]):
+    if isinstance(val, Number):
+        val = np.full(nvec, val, dtype=dtype)
+    shape = (nvec, 1, 1) if ndim == 3 else (nvec,)
+    return np.reshape(val, shape).astype(dtype, copy=False)
 
 
 def adjust_dimensions(
     lb: Array2d,
     ub: Array2d,
     max_velocity_rate: Union[float, Array1d],
     w: Union[float, Array1d],
     c1: Union[float, Array1d],
     c2: Union[float, Array1d],
-) -> tuple[Array3d, Array3d, int, int, Array3d, Array3d, Array3d, Array3d]:
+    ftol: Union[float, Array1d],
+    xtol: Union[float, Array1d],
+    patience: Union[int, Array1i],
+) -> tuple[
+    Array3d,
+    Array3d,
+    int,
+    int,
+    Array3d,
+    Array3d,
+    Array3d,
+    Array3d,
+    Array1d,
+    Array1d,
+    Array1i,
+]:
     """Adjusts the dimensions of the input arrays to be compatible with the vectorized
     algorithm, i.e., adds dimensions when necessary or converts to array.
 
     lb : 2d array
         Lower bound of the search space. An array of shape `(N, d)`.
     ub : 2d array
         Upper bound of the search space. An array of shape `(N, d)`.
@@ -32,36 +54,49 @@
         of the `N` vectorized problems.
     c1 : float, optional
         Cognitive weight. By default, `2.0`. Can also be an 1d array_like of shape
         `(N,)` to specify a different value for each of the `N` vectorized problems.
     c2 : float, optional
         Social weight. By default, `2.0`. Can also be an 1d array_like of shape `(N,)`
         to specify a different value for each of the `N` vectorized problems.
+    ftol : float or 1d array_like of floats, optional
+        Tolerance for changes in the objective function value before terminating the
+        solver. Can also be an 1d array_like of shape `(N,)` to specify a different
+        value for each of the `N` vectorized problems. By default, `1e-8`.
+    xtol : float or 1d array_like of floats, optional
+        Tolerance for average changes in the objective minimizer before terminating the
+        solver. Can also be an 1d array_like of shape `(N,)` to specify a different
+        value for each of the `N` vectorized problems. By default, `1e-8`.
+    patience : int or 1d array_like of ints, optional
+        Number of iterations to wait before terminating the solver if no improvement is
+        witnessed. Can also be an 1d array_like of shape `(N,)` to specify a different
+        value for each of the `N` vectorized problems. By default, `1`.
 
     Returns
     -------
-    tuple of (3d array, 3d array, int, int, 3d array, 3d array, 3d array, 3d array)
-        Returns the `lb`, `ub`, `nvec`, `dim`, `max_velocity_rate`, `w`, `c1`, and `c2`.
+    tuple of 3d and 1d arrays
+        Returns the `lb`, `ub`, `nvec`, `dim`, `max_velocity_rate`, `w`, `c1`, `c2`,
+        `ftol`, `xtol`, and `patience`.
     """
     lb = np.expand_dims(lb, 1)  # add swarm dimension
     ub = np.expand_dims(ub, 1)  # add swarm dimension
     nvec, _, dim = lb.shape
-    if isinstance(max_velocity_rate, Number):
-        max_velocity_rate = np.full(nvec, max_velocity_rate)
-    max_velocity_rate = np.reshape(max_velocity_rate, (nvec, 1, 1))
-    if isinstance(w, Number):
-        w = np.full(nvec, w)
-    w = np.reshape(w, (nvec, 1, 1))
-    if isinstance(c1, Number):
-        c1 = np.full(nvec, c1)
-    c1 = np.reshape(c1, (nvec, 1, 1))
-    if isinstance(c2, Number):
-        c2 = np.full(nvec, c2)
-    c2 = np.reshape(c2, (nvec, 1, 1))
-    return lb, ub, nvec, dim, max_velocity_rate, w, c1, c2
+    return (
+        lb,
+        ub,
+        nvec,
+        dim,
+        _asarray(max_velocity_rate, nvec, float, 3),
+        _asarray(w, nvec, float, 3),
+        _asarray(c1, nvec, float, 3),
+        _asarray(c2, nvec, float, 3),
+        _asarray(ftol, nvec, float, 1),
+        _asarray(xtol, nvec, float, 1),
+        _asarray(patience, nvec, int, 1),
+    )
 
 
 def initialize_particles(
     nvec: int,
     swarmsize: int,
     dim: int,
     lb: Array3d,
```

### Comparing `vpso-1.0.0/src/vpso/jit.py` & `vpso-1.0.1/src/vpso/jit.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,19 +76,31 @@
         _int,  # iters
         nb.bool_,  # perturb_best
         _float,  # mutation_prob
         nb.types.NumPyRandomGeneratorType("NumPyRandomGeneratorType"),
     ),
     "adaptation_strategy": _float[:, :](_float[:]),
     "perform_adaptation": nb.types.UniTuple(_float[:, :, :], 3)(
+        _int,  # nvec
         _float[:, :, :],  # w
         _float[:, :, :],  # c1
         _float[:, :, :],  # c2
         _float[:],  # stage
         nb.types.NumPyRandomGeneratorType("NumPyRandomGeneratorType"),
     ),
+    "update_patience": nb.types.UniTuple(_float[:], 2)(
+        _float[:, :, :],  # sx
+        _float[:],  # sf
+        _float[:, :, :],  # sx_new
+        _float[:],  # sf_new
+        _float[:, :, :],  # lb
+        _float[:, :, :],  # ub
+        _float[:],  # xtol
+        _float[:],  # ftol
+        _int[:, :],  # current_patience_level
+    ),
 }
 
 
-def jit(func: Callable) -> Callable:
+def jit(func: Callable, cache: bool = True) -> Callable:
     """Assigns a jit decorator to the given function with the correct signature."""
-    return nb.njit(_signatures[func.__name__], cache=True)(func)
+    return nb.njit(_signatures[func.__name__], cache=cache)(func)
```

### Comparing `vpso-1.0.0/src/vpso/math.py` & `vpso-1.0.1/src/vpso/math.py`

 * *Files identical despite different names*

### Comparing `vpso-1.0.0/src/vpso/mutation.py` & `vpso-1.0.1/src/vpso/mutation.py`

 * *Files identical despite different names*

### Comparing `vpso-1.0.0/src/vpso/reparation.py` & `vpso-1.0.1/src/vpso/reparation.py`

 * *Files identical despite different names*

### Comparing `vpso-1.0.0/src/vpso/vpso.py` & `vpso-1.0.1/src/vpso/vpso.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 
 import numpy as np
 from numpy.typing import ArrayLike
 from scipy.stats.qmc import LatinHypercube
 
 from vpso.adaptation import adapt
 from vpso.ask_and_tell import advance_population, generate_offsprings, get_best
-from vpso.initialization import adjust_dimensions, initialize_particles
-from vpso.typing import Array1d, Array2d, Array3d
+from vpso.initialization import adjust_dimensions as adj_dim
+from vpso.initialization import initialize_particles
+from vpso.termination import termination
+from vpso.typing import Array1d, Array1i, Array2d, Array3d
 
 logger = logging.getLogger(__name__)
 
 
 def vpso(
     func: Callable[[Array3d], ArrayLike],
     lb: Array2d,
@@ -25,18 +27,18 @@
     c2: Union[float, Array1d] = 2.0,
     #
     repair_iters: int = 20,
     perturb_best: bool = True,
     mutation_prob: float = 0.9,
     adaptive: bool = True,
     #
-    maxiter: int = 300,
-    ftol: float = 1e-8,
-    xtol: float = 1e-8,
-    patience: int = 10,
+    maxiter: int = 300,  # could be an array, but only the max would be then used
+    ftol: Union[float, Array1d] = 1e-8,
+    xtol: Union[float, Array1d] = 1e-8,
+    patience: Union[int, Array1i] = 30,
     #
     seed: Optional[int] = None,
     verbosity: int = logging.WARNING,
 ) -> tuple[Array2d, Array1d, str]:
     """Vectorized Particle Swarm Optimization (VPSO). This implementation of PSO is able
     to solve multiple optimization problems simultaneously in a vectorized fashion.
 
@@ -50,41 +52,55 @@
     lb : 2d array
         Lower bound of the search space. An array of shape `(N, d)`. Can be different
         in each of the `N` vectorized problems.
     ub : 2d array
         Upper bound of the search space. An array of shape `(N, d)`.
     swarmsize : int, optional
         Number of particles in the swarm to solve each problem. By default, `25`.
-    max_velocity_rate : float or array, optional
+    max_velocity_rate : float or array_like, optional
         Maximum velocity rate used to initialize the particles. By default, `0.2`. Can
         also be an 1d array_like of shape `(N,)` to specify a different value for each
         of the `N` vectorized problems.
-    w : float or 1d array, optional
+    w : float or 1d array_like, optional
         Inertia weight. By default, `0.9`. Can
         also be an 1d array_like of shape `(N,)` to specify a different value for each
         of the `N` vectorized problems.
-    c1 : float or 1d array, optional
+    c1 : float or 1d array_like, optional
         Cognitive weight. By default, `2.0`. Can also be an 1d array_like of shape
         `(N,)` to specify a different value for each of the `N` vectorized problems.
-    c2 : float or 1d array, optional
+    c2 : float or 1d array_like, optional
         Social weight. By default, `2.0`. Can also be an 1d array_like of shape `(N,)`
         to specify a different value for each of the `N` vectorized problems.
     repair_iters : int, optional
         Number of iterations to repair particles that are outside bounds. If this
         reparation fails, the particle is randomly re-sampled. By default, `20`.
     perturb_best : bool, optional
         Whether to perturb the best particle in the swarm at each iteration.
         By default, `True`.
     mutation_prob : float, optional
         Probability of mutating the best particle in the swarm at each iteration. By
         default, `0.9`. Only used if `perturb_best=True`.
     adaptive : bool, optional
         Whether to adapt the weights at each iteration. By default, `True`.
-    maxiter : int, optional
+    maxiter : int , optional
         Maximum number of iterations to run the optimization for. By default, `300`.
+    ftol : float or 1d array_like of floats, optional
+        Tolerance for changes in the objective function value before terminating the
+        solver. Can also be an 1d array_like of shape `(N,)` to specify a different
+        value for each of the `N` vectorized problems. By default, `1e-8`. Pass a
+        negative value to disable this check.
+    xtol : float or 1d array_like of floats, optional
+        Tolerance for average changes in the objective minimizer before terminating the
+        solver. Can also be an 1d array_like of shape `(N,)` to specify a different
+        value for each of the `N` vectorized problems. By default, `1e-8`. Pass a
+        negative value to disable this check.
+    patience : int or 1d array_like of ints, optional
+        Number of iterations to wait before terminating the solver if no improvement is
+        witnessed. Can also be an 1d array_like of shape `(N,)` to specify a different
+        value for each of the `N` vectorized problems. By default, `1`.
     seed : int, optional
         Seed for the random number generator. By default, `None`.
     verbosity : int, optional
         Verbosity level of the solver. Levels higher than `INFO` log nothig. By default,
         `logging.WARNING` is used.
 
     Returns
@@ -94,31 +110,32 @@
          - the best minimizer of each problem
          - the best minimum of each problem
          - the termination reason as a string
     """
     logger.setLevel(verbosity)
 
     # first, adjust some dimensions
-    lb, ub, nvec, dim, max_velocity_rate, w, c1, c2 = adjust_dimensions(
-        lb, ub, max_velocity_rate, w, c1, c2
+    lb, ub, nvec, dim, max_velocity_rate, w, c1, c2, ftol, xtol, patience = adj_dim(
+        lb, ub, max_velocity_rate, w, c1, c2, ftol, xtol, patience
     )
 
     # initialize particle positions and velocities
     lhs_sampler = LatinHypercube(d=nvec * dim, seed=seed)
     np_random = np.random.Generator(np.random.PCG64(seed))
     x, v, v_max = initialize_particles(
         nvec, swarmsize, dim, lb, ub, max_velocity_rate, lhs_sampler, np_random
     )
 
     # initialize particle's best pos/value and global best
     px = x  # particle's best position
     pf = np.reshape(func(x), (nvec, swarmsize))  # particle's best value
-    sx, sf = get_best(px, pf, nvec)  # social/global best position/value
+    sx, sf = get_best(px, pf, nvec, logger, 0)  # social/global best position/value
 
     # main optimization loop
+    patience_level = np.zeros((nvec, 2), dtype=np.int32)  # 2 level for x and for f
     termination_reason = "maxiter"
     for i in range(1, maxiter + 1):
         x, v = generate_offsprings(
             x,
             px,
             pf,
             sx,
@@ -134,26 +151,44 @@
             repair_iters,
             perturb_best,
             mutation_prob,
             np_random,
         )
         f = np.reshape(func(x), (nvec, swarmsize))  # evaluate particles (non-jittable)
         px, pf = advance_population(x, f, px, pf)
+        sx_new, sf_new = get_best(px, pf, nvec, logger, i)
+
+        # DEBUG
+        # px.flags.writeable = (
+        #     pf.flags.writeable
+        # ) = sx.flags.writeable = sf.flags.writeable = False
+        # assert (sf_new <= sf).all()
+
         if adaptive:
             w, c1, c2 = adapt(
                 px,
-                sx,
+                sx_new,
+                nvec,
                 swarmsize,
                 lb,
                 ub,
                 w,
                 c1,
                 c2,
                 np_random,
+                logger,
             )
-        sx, sf = get_best(px, pf, nvec)
-        logger.debug("average best at iteration %d is %e", i, sf.mean())
 
-        # TODO: check termination conditions
+        # check termination conditions
+        should_terminate, reason = termination(
+            sx, sf, sx_new, sf_new, lb, ub, xtol, ftol, patience, patience_level, logger
+        )
+        if should_terminate:
+            termination_reason = reason
+            break
+
+        # save new best
+        sx = sx_new
+        sf = sf_new
 
     logger.info('termination due to "%s"', termination_reason)
     return sx[:, 0], sf, termination_reason
```

### Comparing `vpso-1.0.0/src/vpso.egg-info/PKG-INFO` & `vpso-1.0.1/src/vpso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vpso
-Version: 1.0.0
+Version: 1.0.1
 Summary: Multiple Particle Swarm Optimization
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/vectorized-particle-swarm
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/vectorized-particle-swarm/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vpso-1.0.0/src/vpso.egg-info/SOURCES.txt` & `vpso-1.0.1/src/vpso.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/vpso/adaptation.py
 src/vpso/ask_and_tell.py
 src/vpso/initialization.py
 src/vpso/jit.py
 src/vpso/math.py
 src/vpso/mutation.py
 src/vpso/reparation.py
+src/vpso/termination.py
 src/vpso/typing.py
 src/vpso/vpso.py
 src/vpso.egg-info/PKG-INFO
 src/vpso.egg-info/SOURCES.txt
 src/vpso.egg-info/dependency_links.txt
 src/vpso.egg-info/requires.txt
 src/vpso.egg-info/top_level.txt
```

### Comparing `vpso-1.0.0/tests/test_adaptation.py` & `vpso-1.0.1/tests/test_adaptation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import unittest
 
 import numpy as np
 from pymoo.problems.functional import FunctionalProblem
 from pymoo.util.misc import norm_eucl_dist
 
 from vpso.adaptation import adapt, adaptation_strategy
@@ -113,21 +114,23 @@
             c1_new.append(o[1])
             c2_new.append(o[2])
 
         np_random = np.random.Generator(np.random.PCG64(seed))
         w_new_, c1_new_, c2_new_ = adapt(
             px,
             sx[:, np.newaxis],
+            nvec,
             swarmsize,
             lb[:, np.newaxis],
             ub[:, np.newaxis],
             w[:, np.newaxis, np.newaxis],
             c1[:, np.newaxis, np.newaxis],
             c2[:, np.newaxis, np.newaxis],
             np_random,
+            logging.getLogger(),
         )
         np.testing.assert_allclose(w_new_.squeeze(), w_new, err_msg="w")
         np.testing.assert_allclose(c1_new_.squeeze(), c1_new, err_msg="c1")
         np.testing.assert_allclose(c2_new_.squeeze(), c2_new, err_msg="c2")
 
 
 if __name__ == "__main__":
```

### Comparing `vpso-1.0.0/tests/test_initialization.py` & `vpso-1.0.1/tests/test_initialization.py`

 * *Files identical despite different names*

### Comparing `vpso-1.0.0/tests/test_math.py` & `vpso-1.0.1/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `vpso-1.0.0/tests/test_mutation.py` & `vpso-1.0.1/tests/test_mutation.py`

 * *Files identical despite different names*

### Comparing `vpso-1.0.0/tests/test_numerical.py` & `vpso-1.0.1/tests/test_numerical.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,16 @@
             np.tile(problem.xl, (nvec, 1)),
             np.tile(problem.xu, (nvec, 1)),
             #
             swarmsize=swarmsize,
             #
             maxiter=maxiter,
             #
+            xtol=-1,
+            ftol=-1,
             seed=np.random.randint(0, 1000),
         )
 
         pf = problem.pareto_front().item()
         ps = problem.pareto_set().squeeze()
         np.testing.assert_allclose(
             actual_f, pf, atol=1e-3, rtol=1e-3, err_msg=f"f {cls.__name__}"
```

### Comparing `vpso-1.0.0/tests/test_reparation.py` & `vpso-1.0.1/tests/test_reparation.py`

 * *Files identical despite different names*

