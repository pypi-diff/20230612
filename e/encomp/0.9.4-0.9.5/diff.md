# Comparing `tmp/encomp-0.9.4.tar.gz` & `tmp/encomp-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encomp-0.9.4.tar", max compression
+gzip compressed data, was "encomp-0.9.5.tar", max compression
```

## Comparing `encomp-0.9.4.tar` & `encomp-0.9.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1072 2023-04-25 07:41:03.603957 encomp-0.9.4/LICENSE
--rw-r--r--   0        0        0    10441 2023-04-25 07:41:03.603957 encomp-0.9.4/README.md
--rw-r--r--   0        0        0       78 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/__init__.py
--rw-r--r--   0        0        0      710 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/constants.py
--rw-r--r--   0        0        0     1895 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/context.py
--rw-r--r--   0        0        0     1976 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/conversion.py
--rw-r--r--   0        0        0     4453 2023-03-12 08:05:11.060958 encomp-0.9.4/encomp/defs/constants.txt
--rw-r--r--   0        0        0    31139 2023-03-12 08:05:11.060958 encomp-0.9.4/encomp/defs/units.txt
--rw-r--r--   0        0        0    44819 2023-05-11 17:03:16.518616 encomp-0.9.4/encomp/fluids.py
--rw-r--r--   0        0        0    12415 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/gases.py
--rw-r--r--   0        0        0     7133 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/math.py
--rw-r--r--   0        0        0     5269 2023-04-25 08:07:46.797762 encomp-0.9.4/encomp/misc.py
--rw-r--r--   0        0        0        0 2023-03-12 08:05:11.060958 encomp-0.9.4/encomp/py.typed
--rw-r--r--   0        0        0    14354 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/serialize.py
--rw-r--r--   0        0        0      416 2023-04-25 07:32:25.073969 encomp-0.9.4/encomp/session.py
--rw-r--r--   0        0        0     2645 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/settings.py
--rw-r--r--   0        0        0     2882 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/structures.py
--rw-r--r--   0        0        0    23410 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/sympy.py
--rw-r--r--   0        0        0        0 2023-03-12 08:05:11.060958 encomp-0.9.4/encomp/tests/__init__.py
--rw-r--r--   0        0        0      197 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/tests/test_constants.py
--rw-r--r--   0        0        0      904 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/tests/test_context.py
--rw-r--r--   0        0        0      934 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/tests/test_conversion.py
--rw-r--r--   0        0        0    10665 2023-05-11 17:03:39.366721 encomp-0.9.4/encomp/tests/test_fluids.py
--rw-r--r--   0        0        0     3065 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/tests/test_fluids_types.py
--rw-r--r--   0        0        0     2542 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/tests/test_function_signatures.py
--rw-r--r--   0        0        0     1103 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/tests/test_gases.py
--rw-r--r--   0        0        0      189 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/tests/test_math.py
--rw-r--r--   0        0        0     2066 2023-04-25 08:08:32.357986 encomp-0.9.4/encomp/tests/test_misc.py
--rw-r--r--   0        0        0     1544 2023-05-11 10:09:11.799816 encomp-0.9.4/encomp/tests/test_pandas.py
--rw-r--r--   0        0        0      777 2023-05-11 10:07:40.203132 encomp-0.9.4/encomp/tests/test_polars.py
--rw-r--r--   0        0        0     5478 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/tests/test_quantity_combined.py
--rw-r--r--   0        0        0     1243 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/tests/test_quantity_guard.py
--rw-r--r--   0        0        0     5200 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/tests/test_quantity_inferred.py
--rw-r--r--   0        0        0      649 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/tests/test_quantity_magnitude.py
--rw-r--r--   0        0        0    23222 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/tests/test_quantity_types.py
--rw-r--r--   0        0        0     3453 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/tests/test_serialize.py
--rw-r--r--   0        0        0      124 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/tests/test_settings.py
--rw-r--r--   0        0        0     1768 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/tests/test_structures.py
--rw-r--r--   0        0        0     1812 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/tests/test_sympy.py
--rw-r--r--   0        0        0      929 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/tests/test_thermo.py
--rw-r--r--   0        0        0    36826 2023-05-29 06:48:33.865940 encomp-0.9.4/encomp/tests/test_units.py
--rw-r--r--   0        0        0     6402 2023-04-25 07:41:03.603957 encomp-0.9.4/encomp/thermo.py
--rw-r--r--   0        0        0    43417 2023-05-29 07:19:21.577082 encomp-0.9.4/encomp/units.py
--rw-r--r--   0        0        0    79936 2023-05-29 07:00:53.820668 encomp-0.9.4/encomp/units.pyi
--rw-r--r--   0        0        0    21664 2023-05-11 10:41:15.866326 encomp-0.9.4/encomp/utypes.py
--rw-r--r--   0        0        0     2973 2023-05-29 07:19:27.117103 encomp-0.9.4/pyproject.toml
--rw-r--r--   0        0        0    11685 1970-01-01 00:00:00.000000 encomp-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-25 07:41:03.603957 encomp-0.9.5/LICENSE
+-rw-r--r--   0        0        0    10423 2023-06-12 08:10:46.714920 encomp-0.9.5/README.md
+-rw-r--r--   0        0        0       78 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/__init__.py
+-rw-r--r--   0        0        0      710 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/constants.py
+-rw-r--r--   0        0        0     1895 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/context.py
+-rw-r--r--   0        0        0     1976 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/conversion.py
+-rw-r--r--   0        0        0     4453 2023-03-12 08:05:11.060958 encomp-0.9.5/encomp/defs/constants.txt
+-rw-r--r--   0        0        0    31139 2023-03-12 08:05:11.060958 encomp-0.9.5/encomp/defs/units.txt
+-rw-r--r--   0        0        0    44819 2023-05-11 17:03:16.518616 encomp-0.9.5/encomp/fluids.py
+-rw-r--r--   0        0        0    12415 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/gases.py
+-rw-r--r--   0        0        0     7133 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/math.py
+-rw-r--r--   0        0        0     5269 2023-04-25 08:07:46.797762 encomp-0.9.5/encomp/misc.py
+-rw-r--r--   0        0        0        0 2023-03-12 08:05:11.060958 encomp-0.9.5/encomp/py.typed
+-rw-r--r--   0        0        0    14354 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/serialize.py
+-rw-r--r--   0        0        0      416 2023-04-25 07:32:25.073969 encomp-0.9.5/encomp/session.py
+-rw-r--r--   0        0        0     2645 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/settings.py
+-rw-r--r--   0        0        0     2882 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/structures.py
+-rw-r--r--   0        0        0    23410 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/sympy.py
+-rw-r--r--   0        0        0        0 2023-03-12 08:05:11.060958 encomp-0.9.5/encomp/tests/__init__.py
+-rw-r--r--   0        0        0      197 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/tests/test_constants.py
+-rw-r--r--   0        0        0      904 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/tests/test_context.py
+-rw-r--r--   0        0        0      934 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/tests/test_conversion.py
+-rw-r--r--   0        0        0    10665 2023-05-11 17:03:39.366721 encomp-0.9.5/encomp/tests/test_fluids.py
+-rw-r--r--   0        0        0     3065 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/tests/test_fluids_types.py
+-rw-r--r--   0        0        0     2542 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/tests/test_function_signatures.py
+-rw-r--r--   0        0        0     1103 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/tests/test_gases.py
+-rw-r--r--   0        0        0      189 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/tests/test_math.py
+-rw-r--r--   0        0        0     2066 2023-04-25 08:08:32.357986 encomp-0.9.5/encomp/tests/test_misc.py
+-rw-r--r--   0        0        0     1544 2023-05-11 10:09:11.799816 encomp-0.9.5/encomp/tests/test_pandas.py
+-rw-r--r--   0        0        0      777 2023-05-11 10:07:40.203132 encomp-0.9.5/encomp/tests/test_polars.py
+-rw-r--r--   0        0        0     5478 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/tests/test_quantity_combined.py
+-rw-r--r--   0        0        0     1243 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/tests/test_quantity_guard.py
+-rw-r--r--   0        0        0     5200 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/tests/test_quantity_inferred.py
+-rw-r--r--   0        0        0      649 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/tests/test_quantity_magnitude.py
+-rw-r--r--   0        0        0    23222 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/tests/test_quantity_types.py
+-rw-r--r--   0        0        0     3453 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/tests/test_serialize.py
+-rw-r--r--   0        0        0      124 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/tests/test_settings.py
+-rw-r--r--   0        0        0     1768 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/tests/test_structures.py
+-rw-r--r--   0        0        0     1812 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/tests/test_sympy.py
+-rw-r--r--   0        0        0      929 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/tests/test_thermo.py
+-rw-r--r--   0        0        0    36826 2023-06-12 08:14:20.991078 encomp-0.9.5/encomp/tests/test_units.py
+-rw-r--r--   0        0        0     6402 2023-04-25 07:41:03.603957 encomp-0.9.5/encomp/thermo.py
+-rw-r--r--   0        0        0    43273 2023-06-12 08:15:21.999121 encomp-0.9.5/encomp/units.py
+-rw-r--r--   0        0        0    79936 2023-05-29 07:00:53.820668 encomp-0.9.5/encomp/units.pyi
+-rw-r--r--   0        0        0    21664 2023-05-11 10:41:15.866326 encomp-0.9.5/encomp/utypes.py
+-rw-r--r--   0        0        0     2969 2023-06-12 08:12:06.774981 encomp-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0    11594 1970-01-01 00:00:00.000000 encomp-0.9.5/PKG-INFO
```

### Comparing `encomp-0.9.4/LICENSE` & `encomp-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/README.md` & `encomp-0.9.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # encomp
 
 > General-purpose library for *en*gineering *comp*utations, with focus on clean and consistent interfaces.
 
 Documentation at <https://encomp.readthedocs.io/en/latest/>
 
-`encomp` is tested on Windows and Linux, with Python versions 3.10 and 3.11.
+`encomp` is tested on Windows and Linux, with Python 3.11.
 
 ## Features
 
 Main functionality of the `encomp` library:
 
 - Handles physical quantities with magnitude(s), dimensionality and units
```

### Comparing `encomp-0.9.4/encomp/constants.py` & `encomp-0.9.5/encomp/constants.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/context.py` & `encomp-0.9.5/encomp/context.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/conversion.py` & `encomp-0.9.5/encomp/conversion.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/defs/constants.txt` & `encomp-0.9.5/encomp/defs/constants.txt`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/defs/units.txt` & `encomp-0.9.5/encomp/defs/units.txt`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/fluids.py` & `encomp-0.9.5/encomp/fluids.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/gases.py` & `encomp-0.9.5/encomp/gases.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/math.py` & `encomp-0.9.5/encomp/math.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/misc.py` & `encomp-0.9.5/encomp/misc.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/serialize.py` & `encomp-0.9.5/encomp/serialize.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/settings.py` & `encomp-0.9.5/encomp/settings.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/structures.py` & `encomp-0.9.5/encomp/structures.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/sympy.py` & `encomp-0.9.5/encomp/sympy.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_context.py` & `encomp-0.9.5/encomp/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_conversion.py` & `encomp-0.9.5/encomp/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_fluids.py` & `encomp-0.9.5/encomp/tests/test_fluids.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_fluids_types.py` & `encomp-0.9.5/encomp/tests/test_fluids_types.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_function_signatures.py` & `encomp-0.9.5/encomp/tests/test_function_signatures.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_gases.py` & `encomp-0.9.5/encomp/tests/test_gases.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_misc.py` & `encomp-0.9.5/encomp/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_pandas.py` & `encomp-0.9.5/encomp/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_polars.py` & `encomp-0.9.5/encomp/tests/test_polars.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_quantity_combined.py` & `encomp-0.9.5/encomp/tests/test_quantity_combined.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_quantity_guard.py` & `encomp-0.9.5/encomp/tests/test_quantity_guard.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_quantity_inferred.py` & `encomp-0.9.5/encomp/tests/test_quantity_inferred.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_quantity_magnitude.py` & `encomp-0.9.5/encomp/tests/test_quantity_magnitude.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_quantity_types.py` & `encomp-0.9.5/encomp/tests/test_quantity_types.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_serialize.py` & `encomp-0.9.5/encomp/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_structures.py` & `encomp-0.9.5/encomp/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_sympy.py` & `encomp-0.9.5/encomp/tests/test_sympy.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_thermo.py` & `encomp-0.9.5/encomp/tests/test_thermo.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/tests/test_units.py` & `encomp-0.9.5/encomp/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/thermo.py` & `encomp-0.9.5/encomp/thermo.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/units.py` & `encomp-0.9.5/encomp/units.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 """
 
 
 from __future__ import annotations
 
 import copy
 import numbers
-import logging
 import re
 import warnings
 from types import UnionType
 from typing import Any, ClassVar, Generic, Iterable, Literal, TypeVar
 
 import numpy as np
 import pandas as pd
@@ -25,16 +24,14 @@
 import sympy as sp
 from pint.errors import DimensionalityError
 from pint.facets.formatting.objects import FormattingQuantity, FormattingUnit
 from pint.facets.measurement.objects import MeasurementQuantity
 from pint.facets.nonmultiplicative.objects import NonMultiplicativeQuantity
 from pint.facets.numpy.quantity import NumpyQuantity
 from pint.facets.numpy.unit import NumpyUnit
-from pint.facets.plain.quantity import PlainQuantity
-from pint.facets.plain.unit import PlainUnit
 from pint.registry import LazyRegistry, UnitRegistry
 from pint.util import UnitsContainer
 
 from .misc import isinstance_types
 from .settings import SETTINGS
 from .utypes import (
     _BASE_SI_UNITS,
@@ -53,15 +50,14 @@
 if SETTINGS.ignore_ndarray_unit_stripped_warning:
     warnings.filterwarnings(
         "ignore",
         message="The unit of the quantity is stripped when downcasting to ndarray.",
     )
 
 
-
 # custom errors inherit from pint.errors.DimensionalityError
 # (which inherits from TypeError)
 # this makes it possible to use
 # try:
 #     ...
 # except DimensionalityError:
 #     ...
@@ -199,21 +195,20 @@
         # TODO: determine if this is called from the underlying pint
         # API or directly and validate the subclass and unit dimensionality
         # based on this
 
         return super().__call__(*args, **kwargs)
 
 
-class Unit(PlainUnit, NumpyUnit, FormattingUnit, Generic[DT]):
+class Unit(NumpyUnit, FormattingUnit, Generic[DT]):
     pass
 
 
 class Quantity(
     NonMultiplicativeQuantity,
-    PlainQuantity,
     MeasurementQuantity,
     NumpyQuantity,
     FormattingQuantity,
     Generic[DT, MT],
     metaclass=QuantityMeta,
 ):
     """
```

### Comparing `encomp-0.9.4/encomp/units.pyi` & `encomp-0.9.5/encomp/units.pyi`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/encomp/utypes.py` & `encomp-0.9.5/encomp/utypes.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.4/pyproject.toml` & `encomp-0.9.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [tool.poetry]
 name = "encomp"
-version = "0.9.4"
+version = "0.9.5"
 description = "General-purpose library for engineering calculations"
 authors = ["William Laurén <lauren.william.a@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{ include = "encomp" }]
 include = ["encomp/defs"]
 
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 urllib3 = "^1"             # https://github.com/urllib3/urllib3/issues/3010
 python-dateutil = "*"
 python-dotenv = "*"
 pydantic = "*"
-typeguard = "^3"
+typeguard = "*"
 typing-extensions = "*"
 asttokens = "*"
 numpy = "*"
 pandas = "*"
 pyarrow = "*"
 polars = "*"
 sympy = "*"
 symbolic-equation = "*"
-pint = "~0.21"
-coolprop = "^6.4"
+pint = "~0.22"
+coolprop = "*"
 uncertainties = "*"
 matplotlib = { version = "*", optional = true }
 seaborn = { version = "*", optional = true }
 scipy = { version = "*", optional = true }
 fire = { version = "*", optional = true }
 fluids = { version = "*", optional = true }
 thermo = { version = "*", optional = true }
```

### Comparing `encomp-0.9.4/PKG-INFO` & `encomp-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 Metadata-Version: 2.1
 Name: encomp
-Version: 0.9.4
+Version: 0.9.5
 Summary: General-purpose library for engineering calculations
 License: MIT
 Author: William Laurén
 Author-email: lauren.william.a@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: optional
 Requires-Dist: asttokens
-Requires-Dist: coolprop (>=6.4,<7.0)
+Requires-Dist: coolprop
 Requires-Dist: fire ; extra == "optional"
 Requires-Dist: fluids ; extra == "optional"
 Requires-Dist: ht ; extra == "optional"
 Requires-Dist: matplotlib ; extra == "optional"
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: pint (>=0.21,<0.22)
+Requires-Dist: pint (>=0.22,<0.23)
 Requires-Dist: polars
 Requires-Dist: pyarrow
 Requires-Dist: pydantic
 Requires-Dist: python-dateutil
 Requires-Dist: python-dotenv
 Requires-Dist: scipy ; extra == "optional"
 Requires-Dist: seaborn ; extra == "optional"
 Requires-Dist: symbolic-equation
 Requires-Dist: sympy
 Requires-Dist: thermo ; extra == "optional"
-Requires-Dist: typeguard (>=3,<4)
+Requires-Dist: typeguard
 Requires-Dist: typing-extensions
 Requires-Dist: uncertainties
 Requires-Dist: urllib3 (>=1,<2)
 Description-Content-Type: text/markdown
 
 # encomp
 
 > General-purpose library for *en*gineering *comp*utations, with focus on clean and consistent interfaces.
 
 Documentation at <https://encomp.readthedocs.io/en/latest/>
 
-`encomp` is tested on Windows and Linux, with Python versions 3.10 and 3.11.
+`encomp` is tested on Windows and Linux, with Python 3.11.
 
 ## Features
 
 Main functionality of the `encomp` library:
 
 - Handles physical quantities with magnitude(s), dimensionality and units
```

