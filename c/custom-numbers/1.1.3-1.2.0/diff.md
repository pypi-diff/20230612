# Comparing `tmp/custom_numbers-1.1.3.tar.gz` & `tmp/custom_numbers-1.2.0.tar.gz`

## Comparing `custom_numbers-1.1.3.tar` & `custom_numbers-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/.bumpversion.cfg
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/CHANGELOG.md
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/i2.sh
--rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/inst.sh
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/mm.sh
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/pytest.ini
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/requirements.txt
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/setup_environment.sh
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/t.sh
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/uninst.sh
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/conda/meta.yaml
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/src/custom_numbers/__init__.py
--rw-r--r--   0        0        0    16943 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/src/custom_numbers/custom_numbers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/src/custom_numbers/py.typed
--rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/tests/test_customnumber.py
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/tests/test_customnumeralsystem.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/tests/test_geariterator.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/LICENSE
--rw-r--r--   0        0        0     8675 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/README.md
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/pyproject.toml
--rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 custom_numbers-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/.bumpversion.cfg
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/CHANGELOG.md
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/i2.sh
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/inst.sh
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/mm.sh
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/pytest.ini
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/requirements.txt
+-rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/setup_environment.sh
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/t.sh
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/uninst.sh
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/conda/meta.yaml
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/src/custom_numbers/__init__.py
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/src/custom_numbers/custom_numbers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/src/custom_numbers/py.typed
+-rw-r--r--   0        0        0    10742 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/tests/test_customnumber.py
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/tests/test_customnumeralsystem.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/tests/test_geariterator.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/LICENSE
+-rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/README.md
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10681 2020-02-02 00:00:00.000000 custom_numbers-1.2.0/PKG-INFO
```

### Comparing `custom_numbers-1.1.3/.github/ISSUE_TEMPLATE/bug_report.md` & `custom_numbers-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.3/.github/ISSUE_TEMPLATE/feature_request.md` & `custom_numbers-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.3/conda/meta.yaml` & `custom_numbers-1.2.0/conda/meta.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% set name = 'custom-numbers' %}
 {% set filename = 'custom_numbers' %}
 {% set char1 = str(ord(name[0])) %}
-{% set version = '1.1.3' %}
+{% set version = '1.2.0' %}
 
 package:
     name: {{ name|lower }}
     version: {{ version }}
 
 about:
     summary: "A Swiss-army knife for numbers of custom numeral systems."
```

### Comparing `custom_numbers-1.1.3/src/custom_numbers/custom_numbers.py` & `custom_numbers-1.2.0/src/custom_numbers/custom_numbers.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 https://github.com/StrayFeral/custom_numbers
 """
 
 import re
 import math
 from typing import List
 
-__version__: str = "1.1.3"
+__version__: str = "1.2.0"
 __author__: str = r"Evgueni Antonov (Evgueni.Antonov@gmail.com)"
 
 
 
 class CustomNumeralSystem:
     r"""Definition of custom numeral systems with basic consistency validation.
 
@@ -157,18 +157,20 @@
     _POSITIVE: str = r"+"
     _NEGATIVE: str = r"-"
 
     
     def __init__(self, numeral_system: CustomNumeralSystem, number: str) -> None:
         self._numeral_system: CustomNumeralSystem = numeral_system
         self._init_value: str = number  # Just in case we will keep the original value
-        self._value: str = number
-
-        self.absolute()  # This will set the sign as well
-
+        self._value: str = self.__abs__(number)
+        self._sign: str = self._POSITIVE
+        
+        if number[0] == self._NEGATIVE:
+            self._sign = self._NEGATIVE
+        
         if not numeral_system.valid_number(self._value):
             raise ValueError("Invalid characters in number, which are not in the chosen numeral system.")
 
     
     def __repr__(self) -> str:
         if self._sign == self._NEGATIVE:
             return f"-{self._value}"
@@ -280,32 +282,25 @@
             raise ValueError("Numbers must be from the same numeral system.")
         result: int = self.to_decimal() % other.to_decimal()
         num: CustomNumber = CustomNumber(self.numeral_system, str(self.numeral_system)[0])  # Dummy init_value
         num.from_decimal(result)
         return num
 
     
-    def absolute(self, number: str = "") -> str:
+    def __abs__(self, number: str = "") -> str:
         """Returns the absolute value."""
 
         num: str = number
+        
         if len(number) == 0:
             num = self._value
 
-        sign: str = self._POSITIVE
-        if num[0] == self._NEGATIVE:
-            sign = self._NEGATIVE
-
         if num[0] == self._POSITIVE or num[0] == self._NEGATIVE:
             num = num[1:]  # Strip sign
 
-        if len(number) == 0:
-            self._value = num
-            self._sign = sign
-
         return num
 
     
     def digit_to_int(self, digit: str) -> int:
         r"""Fastest and simplest possible conversion. Left-most one is the zero."""
 
         if len(digit) != 1:
```

### Comparing `custom_numbers-1.1.3/tests/test_customnumber.py` & `custom_numbers-1.2.0/tests/test_customnumber.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,25 +232,29 @@
         numN2 = cn.CustomNumber(sysN1, "f")
         result = numN1 - numN2
         assert str(result) == expected
 
     
     def test_absolute_value_positive_signed(self):
         expected = "a"
+        original = "a"
         sysN = cn.CustomNumeralSystem("paf")  # 0 1 2
         num = cn.CustomNumber(sysN, "+a")
-        result = num.absolute()
+        result = abs(num)
+        assert str(num) == original
         assert str(result) == expected
 
     
     def test_absolute_value_negative_number(self):
         expected = "a"
+        original = "-a"
         sysN = cn.CustomNumeralSystem("paf")  # 0 1 2
-        num = cn.CustomNumber(sysN, "-a")
-        result = num.absolute()
+        num = cn.CustomNumber(sysN, original)
+        result = abs(num)
+        assert str(num) == original
         assert str(result) == expected
 
     
     def test_negative_number_subtraction1(self):
         expected = "p"  # 0
         sysN1 = cn.CustomNumeralSystem("paf")  # 0 1 2
         numN1 = cn.CustomNumber(sysN1, "-a")
@@ -325,8 +329,18 @@
     def test_modulo2(self):
         expected = "0"
         sysN1 = cn.CustomNumeralSystem("0123456789")  # Common decimal system
         numN1 = cn.CustomNumber(sysN1, "5")
         numN2 = cn.CustomNumber(sysN1, "5")
         result = numN1 % numN2
         assert str(result) == expected
+    
+    
+    def test_issue2(self):
+        expected = "bc"
+        original = "-bc"
+        sysN = cn.CustomNumeralSystem("abc")  # 0 1 2
+        num = cn.CustomNumber(sysN, original)
+        result = abs(num)
+        assert str(num) == original
+        assert str(result) == expected
```

### Comparing `custom_numbers-1.1.3/tests/test_customnumeralsystem.py` & `custom_numbers-1.2.0/tests/test_customnumeralsystem.py`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.3/tests/test_geariterator.py` & `custom_numbers-1.2.0/tests/test_geariterator.py`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.3/.gitignore` & `custom_numbers-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.3/LICENSE` & `custom_numbers-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_numbers-1.1.3/README.md` & `custom_numbers-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# custom_numbers 1.1.3
+# custom_numbers 1.2.0
 
 ## DESCRIPTION
 
 A Swiss-army knife for numbers of custom numeral systems.
 
 ## AUTHOR
 
@@ -201,14 +201,15 @@
 numN1 // numN2  # Floor division
 numN1 / numN2   # NOTE: This will perform floor division as well!
 # as floating point numbers are not supported by this class and will
 # never be.
 numN1 * numN2   # Multiplication
 numN1 ** numN2  # Power
 numN1 % numN2   # Modulo division
+abs(numN)       # Absolute value
 ```
 
 Using the iterator:
 
 ```
 sysN = cn.CustomNumeralSystem("paf")
 it = cn.GearIterator(sysN, 0, 2)
```

### Comparing `custom_numbers-1.1.3/pyproject.toml` & `custom_numbers-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "custom_numbers"
-version = "1.1.3"
+version = "1.2.0"
 authors = [
     { name = "Evgueni Antonov", email = "Evgueni.Antonov@gmail.com" },
 ]
 description = "Swiss-army knife for numbers of custom numeral systems."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `custom_numbers-1.1.3/PKG-INFO` & `custom_numbers-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom_numbers
-Version: 1.1.3
+Version: 1.2.0
 Summary: Swiss-army knife for numbers of custom numeral systems.
 Project-URL: Homepage, https://github.com/StrayFeral/custom_numbers
 Project-URL: Bug Tracker, https://github.com/StrayFeral/custom_numbers/issues
 Author-email: Evgueni Antonov <Evgueni.Antonov@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Evgueni Antonov
@@ -32,15 +32,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# custom_numbers 1.1.3
+# custom_numbers 1.2.0
 
 ## DESCRIPTION
 
 A Swiss-army knife for numbers of custom numeral systems.
 
 ## AUTHOR
 
@@ -239,14 +239,15 @@
 numN1 // numN2  # Floor division
 numN1 / numN2   # NOTE: This will perform floor division as well!
 # as floating point numbers are not supported by this class and will
 # never be.
 numN1 * numN2   # Multiplication
 numN1 ** numN2  # Power
 numN1 % numN2   # Modulo division
+abs(numN)       # Absolute value
 ```
 
 Using the iterator:
 
 ```
 sysN = cn.CustomNumeralSystem("paf")
 it = cn.GearIterator(sysN, 0, 2)
```

