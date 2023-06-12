# Comparing `tmp/ansys-math-core-0.1.1.tar.gz` & `tmp/ansys_math_core-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-math-core-0.1.1.tar", last modified: Wed Apr 12 13:16:23 2023, max compression
+gzip compressed data, was "ansys_math_core-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys-math-core-0.1.1.tar` & `ansys_math_core-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1089 2023-04-12 13:16:03.397489 ansys-math-core-0.1.1/LICENSE
--rw-r--r--   0        0        0     3266 2023-04-12 13:16:03.397489 ansys-math-core-0.1.1/README.rst
--rw-r--r--   0        0        0     2809 2023-04-12 13:16:03.397489 ansys-math-core-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      868 2023-04-12 13:16:03.397489 ansys-math-core-0.1.1/src/ansys/math/core/__init__.py
--rw-r--r--   0        0        0    62314 2023-04-12 13:16:03.397489 ansys-math-core-0.1.1/src/ansys/math/core/math.py
--rw-r--r--   0        0        0     5745 1970-01-01 00:00:00.000000 ansys-math-core-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-12 15:51:50.086311 ansys_math_core-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3370 2023-06-12 15:51:50.086311 ansys_math_core-0.1.2/README.rst
+-rw-r--r--   0        0        0     2823 2023-06-12 15:51:50.090312 ansys_math_core-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      868 2023-06-12 15:51:50.090312 ansys_math_core-0.1.2/src/ansys/math/core/__init__.py
+-rw-r--r--   0        0        0    65264 2023-06-12 15:51:50.090312 ansys_math_core-0.1.2/src/ansys/math/core/math.py
+-rw-r--r--   0        0        0     5862 1970-01-01 00:00:00.000000 ansys_math_core-0.1.2/PKG-INFO
```

### Comparing `ansys-math-core-0.1.1/LICENSE` & `ansys_math_core-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-math-core-0.1.1/README.rst` & `ansys_math_core-0.1.2/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -6,72 +6,71 @@
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
 .. |pypi| image:: https://img.shields.io/pypi/v/ansys-math-core.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/ansys-math-core/
 
-.. |codecov| image:: https://codecov.io/gh/pyansys/pyansys-math/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/pyansys/pyansys-math
+.. |codecov| image:: https://codecov.io/gh/ansys/pyansys-math/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/ansys/pyansys-math
 
-.. |GH-CI| image:: https://github.com/pyansys/pyansys-math/actions/workflows/ci_cd.yml/badge.svg
-   :target: https://github.com/pyansys/pyansys-math/actions/workflows/ci_cd.yml
+.. |GH-CI| image:: https://github.com/ansys/pyansys-math/actions/workflows/ci_cd.yml/badge.svg
+   :target: https://github.com/ansys/pyansys-math/actions/workflows/ci_cd.yml
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
   :target: https://github.com/psf/black
   :alt: black
 
+.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/ansys/pyansys-math/main.svg
+   :target: https://results.pre-commit.ci/latest/github/ansys/pyansys-math/main
+   :alt: pre-commit.ci status
+
 
 PyAnsys Math is a Python repository holding Ansys mathematical libraries.
 To use them, you must have a local installation of Ansys Mechanical APDL.
 
 For information on getting a licensed copy of Ansys Mechanical APDL, visit
 the `Ansys web site <https://www.ansys.com/>`_.
 
 
 
 Installation
 ------------
 
 For users
 ~~~~~~~~~
-The ``ansys.math.core`` package currently supports Python 3.7 through
-Python 3.10 on Windows, Mac OS, and Linux.
-
-.. warning:: 
-
-   ``ansys.math.core`` will no longer support Python 3.7 by June 2023.
-
+The ``ansys.math.core`` package currently supports Python 3.8 through
+Python 3.11 on Windows, Mac OS, and Linux.
 
 Install the latest package for use with this command:
 
 .. code::
 
    pip install ansys-math-core
 
 Alternatively, install the latest
-`PyAnsys Math GitHub <https://github.com/pyansys/pyansys-math.git>`_ package
+`PyAnsys Math GitHub <https://github.com/ansys/pyansys-math.git>`_ package
 with this command:
 
 .. code::
 
-   pip install git+https://github.com/pyansys/pyansys-math.git
+   pip install git+https://github.com/ansys/pyansys-math.git
 
 
 
 For developers
 ~~~~~~~~~~~~~~
 For a local *development* version, install the latest package with:
 
 .. code::
 
-   git clone https://github.com/pyansys/pyansys-math.git
+   git clone https://github.com/ansys/pyansys-math.git
    cd pyansys-math
    pip install -e .
 
 
 Installing the development version allows you to edit the ``ansys-math-core``
 package locally. The changes that you make are reflected in your setup
 after restarting the Python kernel.
```

### Comparing `ansys-math-core-0.1.1/pyproject.toml` & `ansys_math_core-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,95 +1,96 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-math-core"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Python wrapper for PyAnsys Math libraries."
 readme = "README.rst"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
 maintainers = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
 classifiers=[
     "Development Status :: 4 - Beta",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "ansys-mapdl-core>=0.64.0",
+    "ansys-tools-path>=0.2.4",
     "pyansys-tools-versioning>=0.3.3",
     "numpy>=1.14.0",
     "importlib-metadata>=4.0,<5; python_version<='3.8'",
+    "scipy>=1.3.0",  # for sparse (consider optional?)
 ]
 
 [project.optional-dependencies]
 tests = [
-    "ansys-mapdl-core==0.64.0",
+    "ansys-mapdl-core==0.65.0",
     "scipy==1.10.1",
     "pyansys-tools-report==0.5.0",
-    "pytest==7.2.2",
-    "pytest-cov==4.0.0",
+    "pytest==7.3.2",
+    "pytest-cov==4.1.0",
     "pytest-rerunfailures==11.1.2",
-    "pyvista==0.38.5",
+    "pyvista==0.39.1",
     "vtk==9.2.6",
 ]
 doc = [
-    "Sphinx==5.3.0",
-    "ansys-mapdl-core==0.64.0",
-    "ansys-mapdl-reader==0.52.11",
-    "ansys-sphinx-theme==0.9.7",
+    "Sphinx==6.2.1",
+    "ansys-mapdl-core==0.65.0",
+    "ansys-mapdl-reader==0.52.15",
+    "ansys-sphinx-theme==0.9.9",
     "jupyter_sphinx==0.4.0",
-    "jupyterlab==3.6.3",
+    "jupyterlab==4.0.2",
     "numpydoc==1.5.0",
-    "pandas==2.0.0",
+    "pandas==2.0.2",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
-    "pyvista==0.38.5",
+    "pyvista==0.39.1",
     "sphinx-autobuild==2021.3.14",
-    "sphinx-autodoc-typehints==1.22",
-    "sphinx-copybutton==0.5.1",
+    "sphinx-autodoc-typehints==1.23.0",
+    "sphinx-copybutton==0.5.2",
     "sphinx-notfound-page==0.8.3",
-    "sphinx-gallery==0.12.2",
+    "sphinx-gallery==0.13.0",
     "vtk==9.2.6",
 ]
 
 [tool.flit.module]
 name = "ansys.math.core"
 
 [project.urls]
-Homepage = "https://github.com/pyansys/ansys-math/"
+Homepage = "https://github.com/ansys/ansys-math/"
 Documentation = "https://math.docs.pyansys.com"
-Source = "https://github.com/pyansys/ansys-math"
-Tracker = "https://github.com/pyansys/ansys-math/issues"
+Source = "https://github.com/ansys/ansys-math"
+Tracker = "https://github.com/ansys/ansys-math/issues"
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
 profile = "black"
 force_sort_within_sections = true
 line_length = 100
 default_section = "THIRDPARTY"
 src_paths = ["doc", "src", "tests"]
 
 [tool.coverage.run]
-source = ["src"]
+source = ["ansys/pyansys-math"]
 
 [tool.coverage.report]
 show_missing = true
 
 [tool.codespell]
-skip = '*.pyc,*.txt,*.gif,*.png,*.jpg,*.js,*.html,*.doctree,*.ttf,*.woff,*.woff2,*.eot,*.mp4,*.inv,*.pickle,*.ipynb,flycheck*,./.git/*,./.hypothesis/*,*.yml,./doc/build/*,./doc/images/*,./dist/*,*~,.hypothesis*,./doc/source/examples/*,*cover,*.dat,*.mac,build,./docker/mapdl/v*,./factory/*,./ansys/mapdl/core/mapdl_functions.py,PKG-INFO,*.mypy_cache/*,./docker/mapdl/*,./_unused/*'
+skip = '*.pyc,*.txt,*.gif,*.png,*.jpg,*.js,*.html,*.doctree,*.ttf,*.woff,*.woff2,*.eot,*.mp4,*.inv,*.pickle,*.ipynb,flycheck*,./.git/*,./.hypothesis/*,*.yml,./doc/build/*,./doc/images/*,./dist/*,*~,.hypothesis*,./doc/source/examples/*,*cover,*.dat,*.mac,build,./docker/mapdl/v*,./factory/*,PKG-INFO,*.mypy_cache/*,./docker/mapdl/*,./_unused/*'
 ignore-words = "doc/styles/Vocab/ANSYS/accept.txt"
 quiet-level = 3
```

### Comparing `ansys-math-core-0.1.1/src/ansys/math/core/__init__.py` & `ansys_math_core-0.1.2/src/ansys/math/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-math-core-0.1.1/src/ansys/math/core/math.py` & `ansys_math_core-0.1.2/src/ansys/math/core/math.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,29 @@
 import os
 import random
 import string
 from warnings import warn
 
 from ansys.api.mapdl.v0 import ansys_kernel_pb2 as anskernel
 from ansys.api.mapdl.v0 import mapdl_pb2 as pb_types
+from ansys.mapdl.core import VERSION_MAP, launch_mapdl
 from ansys.mapdl.core.common_grpc import (
     ANSYS_VALUE_TYPE,
     DEFAULT_CHUNKSIZE,
     DEFAULT_FILE_CHUNK_SIZE,
 )
-from ansys.mapdl.core.errors import ANSYSDataTypeError, protect_grpc
-from ansys.mapdl.core.launcher import launch_mapdl
+from ansys.mapdl.core.errors import (
+    ANSYSDataTypeError,
+    MapdlRuntimeError,
+    VersionError,
+    protect_grpc,
+)
 from ansys.mapdl.core.misc import load_file
 from ansys.mapdl.core.parameters import interp_star_status
 from ansys.tools.versioning import requires_version
-from ansys.tools.versioning.exceptions import VersionError
 from ansys.tools.versioning.utils import server_meets_version
 import numpy as np
 
 MYCTYPE = {
     np.int32: "I",
     np.int64: "L",
     np.single: "F",
@@ -161,15 +165,15 @@
         RMAXLQ       SMAT   0.011           [126:126]               1
         WWYLBR       SMAT   0.011           [126:126]               1
         FIOMZR       VEC    0.001           126                     1
 
         """
         print(self._status)
 
-    def vec(self, size=0, dtype=np.double, init="zeros", name=None, asarray=False):
+    def vec(self, size=0, dtype=np.double, init=None, name=None, asarray=False):
         """Create a vector.
 
         Parameters
         ----------
         size : int
             Size of the vector.
         dtype : np.dtype, optional
@@ -205,15 +209,15 @@
         if asarray:
             vec = self._mapdl._vec_data(ans_vec.id)
         else:
             vec = ans_vec
 
         return vec
 
-    def mat(self, nrow=1, ncol=1, dtype=np.double, init="zeros", name=None, asarray=False):
+    def mat(self, nrow=1, ncol=1, dtype=np.double, init=None, name=None, asarray=False):
         """Create a matrix.
 
         Parameters
         ----------
         nrow : int, optional
             Number of rows. The default is ``1``.
         ncol : int, optional
@@ -248,15 +252,17 @@
             self._mapdl.run(f"*DMAT,{name},{MYCTYPE[dtype]},ALLOC,{nrow},{ncol}", mute=True)
             mat = AnsDenseMat(name, self._mapdl)
 
             if init == "rand":
                 mat.rand()
             elif init == "ones":
                 mat.ones()
-            elif init != "zeros":
+            elif init == "zeros" or init is None:
+                mat.zeros()
+            elif init is not None:
                 raise ValueError(f"Invalid initialization method '{init}'.")
         else:
             info = self._mapdl._data_info(name)
             if info.objtype == pb_types.DataType.DMAT:
                 mat = AnsDenseMat(name, self._mapdl)
             elif info.objtype == pb_types.DataType.SMAT:
                 mat = AnsSparseMat(name, self._mapdl)
@@ -626,15 +632,17 @@
         -------
         AnsMat or scipy.sparse.csr.csr_matrix
             AnsMath matrix or SciPy sparse matrix, depending on the value for
             the ``asarray`` parameter.
 
         Examples
         --------
-        >>> mass = mapdl.math.mass()
+        >>> import ansys.math.core.math as pymath
+        >>> mm = pymath.AnsMath()
+        >>> mass = mm.mass()
         >>> mass
         AnsMath matrix 60 x 60
 
         Convert to a SciPy array.
 
         >>> mat = mass.asarray()
         >>> mat
@@ -668,15 +676,17 @@
         -------
         AnsMat or `scipy.sparse.csr.csr_matrix`
             AnsMath matrix or SciPy sparse matrix, depending on the value for
             the ``asarray`` parameter.
 
         Examples
         --------
-        >>> ans_mat = mapdl.math.damp()
+        >>> import ansys.math.core.math as pymath
+        >>> mm = pymath.AnsMath()
+        >>> ans_mat = mm.damp()
         >>> ans_mat
         AnsMath Matrix 60 x 60
 
         Convert to a SciPy array.
 
         >>> mat = ans_mat.asarray()
         >>> mat
@@ -896,15 +906,26 @@
         thresh : float, optional
             Numerical threshold value for sparsifying. The default
             value is ``1E-16``.
         """
         kwargs.setdefault("mute", True)
         self._mapdl.run(f"*COMP,{mat.id},SPARSE,{thresh}", **kwargs)
 
-    def eigs(self, nev, k, m=None, c=None, phi=None, algo=None, fmin=None, fmax=None):
+    def eigs(
+        self,
+        nev,
+        k,
+        m=None,
+        c=None,
+        phi=None,
+        algo=None,
+        fmin=None,
+        fmax=None,
+        cpxmod=None,
+    ):
         """Solve an eigenproblem.
 
         Parameters
         ----------
         nev : int
             Number of eigenvalues to compute.
         k : AnsMat
@@ -927,29 +948,31 @@
         >>> a = mm.mat(k.nrow, nev)
         >>> ev = mm.eigs(nev, k, m, phi=a)
         """
         if not fmin:
             fmin = ""
         if not fmax:
             fmax = ""
+        if not cpxmod:
+            cpxmod = ""
 
         cid = ""
         if not c:
             if k.sym() and m.sym():
                 if not algo:
                     algo = "LANB"
             else:
                 algo = "UNSYM"
         else:
             cid = c.id
             algo = "DAMP"
 
         self._mapdl.run("/SOLU", mute=True)
         self._mapdl.run("antype,modal", mute=True)
-        self._mapdl.run(f"modopt,{algo},{nev},{fmin},{fmax}", mute=True)
+        self._mapdl.run(f"modopt,{algo},{nev},{fmin},{fmax},{cpxmod}", mute=True)
         ev = self.vec()
 
         phistr = "" if not phi else phi.id
         self._mapdl.run(f"*EIG,{k.id},{m.id},{cid},{ev.id},{phistr}", mute=True)
         return ev
 
     def dot(self, vec_a, vec_b):
@@ -1167,15 +1190,15 @@
                 raise ValueError("Arrays must be 2-dimensional.")
 
         if sparse.issparse(arr):
             self._send_sparse(mname, arr, sym, dtype, chunk_size)
         else:  # must be dense matrix
             self._send_dense(mname, arr, dtype, chunk_size)
 
-    @requires_version((0, 4, 0))
+    @requires_version((0, 4, 0), VERSION_MAP)
     def _send_dense(self, mname, arr, dtype, chunk_size):
         """Send a dense NumPy array/matrix to MAPDL."""
         if dtype is not None:
             if arr.dtype != dtype:
                 arr = arr.astype(dtype)
 
         if arr.dtype not in list(NP_VALUE_TYPE.keys()):
@@ -1345,14 +1368,61 @@
         """
         if not hasattr(obj, "id"):
             raise TypeError("The object to be added must be an AnsMath object.")
         self._mapdl._log.info("Call MAPDL to perform an AXPY operation.")
         self._mapdl.run(f"*AXPY,{val1},0,{obj.id},{val2},0,{self.id}", mute=True)
         return self
 
+    def kron(self, obj):
+        """Calculates the Kronecker product of two matrices/vectors
+
+        Parameters
+        ----------
+        obj : ``AnsVec`` or ``AnsMat``
+            AnsMath object.
+
+        Returns
+        -------
+        ``AnsMat`` or ``AnsVec``
+            Kronecker product between the two matrices/vectors.
+
+        .. note::
+            Requires at least MAPDL version 2023R2.
+
+        Examples
+        --------
+        >>> import ansys.math.core.math as pymath
+        >>> mm = pymath.AnsMath()
+        >>> m1 = mm.rand(3, 3)
+        >>> m2 = mm.rand(4,2)
+        >>> res = m1.kron(m2)
+        """
+
+        mapdl_version = self._mapdl.version
+        if mapdl_version < 23.2:  # pragma: no cover
+            raise VersionError("``kron`` requires MAPDL version 2023R2")
+
+        if not isinstance(obj, AnsMath):
+            raise TypeError("Must be an AnsMath object.")
+
+        if not isinstance(self, (AnsMat, AnsVec)):
+            raise TypeError(f"Kron product aborted: Unknown obj type ({self.type})")
+        if not isinstance(obj, (AnsMat, AnsVec)):
+            raise TypeError(f"Kron product aborted: Unknown obj type ({obj.type})")
+
+        name = id_generator()  # internal name of the new vector/matrix
+        # perform the Kronecker product
+        self._mapdl.run(f"*KRON,{self.id},{obj.id},{name}")
+
+        if isinstance(self, AnsVec) and isinstance(obj, AnsVec):
+            objout = AnsVec(name, self._mapdl)
+        else:
+            objout = AnsMat(name, self._mapdl)
+        return objout
+
     def __add__(self, op2):
         if not hasattr(op2, "id"):
             raise TypeError("The object to be added must be an AnsMath object.")
 
         opout = self.copy()
         self._mapdl._log.info("Call MAPDL to perform an AXPY operation.")
         self._mapdl.run(f"*AXPY,1,0,{op2.id},1,0,{opout.id}", mute=True)
@@ -1373,16 +1443,28 @@
     def __iadd__(self, op):
         return self.axpy(op, 1, 1)
 
     def __isub__(self, op):
         return self.axpy(op, -1, 1)
 
     def __imul__(self, val):
-        self._mapdl._log.info("Call MAPDL to scale the object.")
-        self._mapdl.run(f"*SCAL,{self.id},{val}", mute=True)
+        mapdl_version = self._mapdl.version
+        self._mapdl._log.info("Call MAPDL to scale the object")
+
+        if isinstance(val, AnsVec):
+            if mapdl_version < 23.2:  # pragma: no cover
+                raise VersionError("Scaling by a vector requires MAPDL version 2023R2 or superior.")
+            else:
+                self._mapdl._log.info(f"Scaling ({self.type}) by a vector")
+                self._mapdl.run(f"*SCAL,{self.id},{val.id}", mute=False)
+        elif isinstance(val, (int, float)):
+            self._mapdl.run(f"*SCAL,{self.id},{val}", mute=True)
+        else:
+            raise TypeError(f"The provided type {type(val)} is not supported.")
+
         return self
 
     def __itruediv__(self, val):
         if val == 0:
             raise ZeroDivisionError("division by zero")
         self._mapdl._log.info("Call MAPDL to 1/scale the object.")
         self._mapdl.run(f"*SCAL,{self.id},{1/val}", mute=True)
@@ -1413,28 +1495,42 @@
         elif init == "ones":
             self.ones()
         elif init == "zeros":
             self.zeros()
 
     @property
     def size(self):
-        """Number of items in the vector."""
+        """Number of items in this vector."""
         sz = self._mapdl.scalar_param(f"{self.id}_DIM")
         if sz is None:
-            raise RuntimeError("This vector has been deleted within MAPDL.")
+            raise MapdlRuntimeError("This vector has been deleted within MAPDL.")
         return int(sz)
 
     def __repr__(self):
         return f"AnsMath vector size {self.size}"
 
     def __getitem__(self, num):
+        info = self._mapdl._data_info(self.id)
+        dtype = ANSYS_VALUE_TYPE[info.stype]
         if num < 0:
-            raise ValueError("Negative indices are not permitted.")
-        self._mapdl.run(f"pyval={self.id}({num+1})", mute=True)
-        return self._mapdl.scalar_param("pyval")
+            raise ValueError("Negative indices not permitted")
+
+        self._mapdl.run(f"pyval_={self.id}({num+1})", mute=True)
+        item_val = self._mapdl.scalar_param("pyval_")
+
+        if MYCTYPE[dtype].upper() in ["C", "Z"]:
+            self._mapdl.run(f"pyval_img_={self.id}({num+1},2)", mute=True)
+            img_val = self._mapdl.scalar_param("pyval_img_")
+            item_val = item_val + img_val * 1j
+
+            # Clean parameters
+            self._mapdl.run("item_val =")
+            self._mapdl.run("pyval_img_=")
+
+        return item_val
 
     def __mul__(self, vec):
         """Return the element-wise product with another AnsMath vector.
 
         This value is known as a Hadamard product.
 
         .. note::
@@ -1497,16 +1593,16 @@
     def asarray(self, dtype=None) -> np.ndarray:
         """Return the vector as a NumPy array.
 
         Parameters
         ----------
         dtype : numpy.dtype, optional
             NumPy data type to upload the array as. The options are `np.double <numpy.double>`_,
-            `np.int32 <numpy.int32>`_, and `np.int64 <numpy.int64>`_. The default is the current array
-            type.
+            `np.int32 <numpy.int32>`_, and `np.int64 <numpy.int64>`_. The default is the current
+            array type.
 
         Returns
         -------
         np.ndarray
             NumPy array with the defined data type.
 
         Examples
```

### Comparing `ansys-math-core-0.1.1/PKG-INFO` & `ansys_math_core-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 Metadata-Version: 2.1
 Name: ansys-math-core
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python wrapper for PyAnsys Math libraries.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: ansys-mapdl-core>=0.64.0
+Requires-Dist: ansys-tools-path>=0.2.4
 Requires-Dist: pyansys-tools-versioning>=0.3.3
 Requires-Dist: numpy>=1.14.0
 Requires-Dist: importlib-metadata>=4.0,<5; python_version<='3.8'
-Requires-Dist: Sphinx==5.3.0 ; extra == "doc"
-Requires-Dist: ansys-mapdl-core==0.64.0 ; extra == "doc"
-Requires-Dist: ansys-mapdl-reader==0.52.11 ; extra == "doc"
-Requires-Dist: ansys-sphinx-theme==0.9.7 ; extra == "doc"
+Requires-Dist: scipy>=1.3.0
+Requires-Dist: Sphinx==6.2.1 ; extra == "doc"
+Requires-Dist: ansys-mapdl-core==0.65.0 ; extra == "doc"
+Requires-Dist: ansys-mapdl-reader==0.52.15 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.4.0 ; extra == "doc"
-Requires-Dist: jupyterlab==3.6.3 ; extra == "doc"
+Requires-Dist: jupyterlab==4.0.2 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
-Requires-Dist: pandas==2.0.0 ; extra == "doc"
+Requires-Dist: pandas==2.0.2 ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
-Requires-Dist: pyvista==0.38.5 ; extra == "doc"
+Requires-Dist: pyvista==0.39.1 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints==1.22 ; extra == "doc"
-Requires-Dist: sphinx-copybutton==0.5.1 ; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints==1.23.0 ; extra == "doc"
+Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
-Requires-Dist: sphinx-gallery==0.12.2 ; extra == "doc"
+Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: vtk==9.2.6 ; extra == "doc"
-Requires-Dist: ansys-mapdl-core==0.64.0 ; extra == "tests"
+Requires-Dist: ansys-mapdl-core==0.65.0 ; extra == "tests"
 Requires-Dist: scipy==1.10.1 ; extra == "tests"
 Requires-Dist: pyansys-tools-report==0.5.0 ; extra == "tests"
-Requires-Dist: pytest==7.2.2 ; extra == "tests"
-Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
+Requires-Dist: pytest==7.3.2 ; extra == "tests"
+Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
 Requires-Dist: pytest-rerunfailures==11.1.2 ; extra == "tests"
-Requires-Dist: pyvista==0.38.5 ; extra == "tests"
+Requires-Dist: pyvista==0.39.1 ; extra == "tests"
 Requires-Dist: vtk==9.2.6 ; extra == "tests"
 Project-URL: Documentation, https://math.docs.pyansys.com
-Project-URL: Homepage, https://github.com/pyansys/ansys-math/
-Project-URL: Source, https://github.com/pyansys/ansys-math
-Project-URL: Tracker, https://github.com/pyansys/ansys-math/issues
+Project-URL: Homepage, https://github.com/ansys/ansys-math/
+Project-URL: Source, https://github.com/ansys/ansys-math
+Project-URL: Tracker, https://github.com/ansys/ansys-math/issues
 Provides-Extra: doc
 Provides-Extra: tests
 
 PyAnsys Math
 ============
 
 |pyansys| |pypi| |GH-CI| |codecov| |MIT| |black|
@@ -58,72 +59,71 @@
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
 .. |pypi| image:: https://img.shields.io/pypi/v/ansys-math-core.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/ansys-math-core/
 
-.. |codecov| image:: https://codecov.io/gh/pyansys/pyansys-math/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/pyansys/pyansys-math
+.. |codecov| image:: https://codecov.io/gh/ansys/pyansys-math/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/ansys/pyansys-math
 
-.. |GH-CI| image:: https://github.com/pyansys/pyansys-math/actions/workflows/ci_cd.yml/badge.svg
-   :target: https://github.com/pyansys/pyansys-math/actions/workflows/ci_cd.yml
+.. |GH-CI| image:: https://github.com/ansys/pyansys-math/actions/workflows/ci_cd.yml/badge.svg
+   :target: https://github.com/ansys/pyansys-math/actions/workflows/ci_cd.yml
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
   :target: https://github.com/psf/black
   :alt: black
 
+.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/ansys/pyansys-math/main.svg
+   :target: https://results.pre-commit.ci/latest/github/ansys/pyansys-math/main
+   :alt: pre-commit.ci status
+
 
 PyAnsys Math is a Python repository holding Ansys mathematical libraries.
 To use them, you must have a local installation of Ansys Mechanical APDL.
 
 For information on getting a licensed copy of Ansys Mechanical APDL, visit
 the `Ansys web site <https://www.ansys.com/>`_.
 
 
 
 Installation
 ------------
 
 For users
 ~~~~~~~~~
-The ``ansys.math.core`` package currently supports Python 3.7 through
-Python 3.10 on Windows, Mac OS, and Linux.
-
-.. warning:: 
-
-   ``ansys.math.core`` will no longer support Python 3.7 by June 2023.
-
+The ``ansys.math.core`` package currently supports Python 3.8 through
+Python 3.11 on Windows, Mac OS, and Linux.
 
 Install the latest package for use with this command:
 
 .. code::
 
    pip install ansys-math-core
 
 Alternatively, install the latest
-`PyAnsys Math GitHub <https://github.com/pyansys/pyansys-math.git>`_ package
+`PyAnsys Math GitHub <https://github.com/ansys/pyansys-math.git>`_ package
 with this command:
 
 .. code::
 
-   pip install git+https://github.com/pyansys/pyansys-math.git
+   pip install git+https://github.com/ansys/pyansys-math.git
 
 
 
 For developers
 ~~~~~~~~~~~~~~
 For a local *development* version, install the latest package with:
 
 .. code::
 
-   git clone https://github.com/pyansys/pyansys-math.git
+   git clone https://github.com/ansys/pyansys-math.git
    cd pyansys-math
    pip install -e .
 
 
 Installing the development version allows you to edit the ``ansys-math-core``
 package locally. The changes that you make are reflected in your setup
 after restarting the Python kernel.
```

