# Comparing `tmp/autosar-e2e-0.3.0.tar.gz` & `tmp/autosar-e2e-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosar-e2e-0.3.0.tar", last modified: Mon Jun  5 15:27:53 2023, max compression
+gzip compressed data, was "autosar-e2e-0.4.0.tar", last modified: Mon Jun 12 14:50:17 2023, max compression
```

## Comparing `autosar-e2e-0.3.0.tar` & `autosar-e2e-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:27:53.560941 autosar-e2e-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-05 15:27:53.556940 autosar-e2e-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:27:53.560941 autosar-e2e-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:27:53.552940 autosar-e2e-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:27:53.556940 autosar-e2e-0.3.0/src/autosar_e2e.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-05 15:27:53.000000 autosar-e2e-0.3.0/src/autosar_e2e.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-05 15:27:53.000000 autosar-e2e-0.3.0/src/autosar_e2e.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:27:53.000000 autosar-e2e-0.3.0/src/autosar_e2e.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-05 15:27:53.000000 autosar-e2e-0.3.0/src/autosar_e2e.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:27:53.556940 autosar-e2e-0.3.0/src/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19179 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/crc.c
--rw-r--r--   0 runner    (1001) docker     (123)    25095 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/crc.h
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/crc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/p01.c
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/p01.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/p02.c
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/p02.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/src/e2e/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:27:53.556940 autosar-e2e-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/test/test_crc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/test/test_p01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-05 15:27:41.000000 autosar-e2e-0.3.0/test/test_p02.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:50:17.588371 autosar-e2e-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-12 14:50:17.588371 autosar-e2e-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:50:17.588371 autosar-e2e-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:50:17.584371 autosar-e2e-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:50:17.584371 autosar-e2e-0.4.0/src/autosar_e2e.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-12 14:50:17.000000 autosar-e2e-0.4.0/src/autosar_e2e.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-12 14:50:17.000000 autosar-e2e-0.4.0/src/autosar_e2e.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:50:17.000000 autosar-e2e-0.4.0/src/autosar_e2e.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-12 14:50:17.000000 autosar-e2e-0.4.0/src/autosar_e2e.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:50:17.588371 autosar-e2e-0.4.0/src/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/src/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19179 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/src/e2e/crc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25095 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/src/e2e/crc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/src/e2e/crc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/src/e2e/p01.c
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/src/e2e/p01.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/src/e2e/p02.c
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/src/e2e/p02.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/src/e2e/p05.c
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/src/e2e/p05.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/src/e2e/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:50:17.588371 autosar-e2e-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/test/test_crc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/test/test_p01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/test/test_p02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-12 14:50:04.000000 autosar-e2e-0.4.0/test/test_p05.py
```

### Comparing `autosar-e2e-0.3.0/LICENSE.txt` & `autosar-e2e-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autosar-e2e-0.3.0/PKG-INFO` & `autosar-e2e-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosar-e2e
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python implementation of the AUTOSAR E2E Protocol
 Author-email: Artur Drogunow <artur.drogunow@zf.com>
 License: MIT
 Project-URL: Documentation, https://autosar-e2e.readthedocs.io/en/latest
 Project-URL: Issues, https://github.com/zariiii9003/autosar-e2e/issues
 Project-URL: Source, https://github.com/zariiii9003/autosar-e2e
 Project-URL: Homepage, https://github.com/zariiii9003/autosar-e2e
@@ -41,15 +41,15 @@
 - [License](#license)
 
 ## Description
 
 This library provides fast C implementations of the E2E CRC algorithms and E2E profiles. 
 
 Currently, all relevant CRC algorithms are available in module `e2e.crc`
-but only E2E profiles 1 and 2 are available. 
+but only E2E profiles 1, 2 and 5 are available. 
 If you provide example data for the other profiles I would try to implement them, too.
 
 ## Installation
 
 ```console
 pip install autosar-e2e
 ```
```

### Comparing `autosar-e2e-0.3.0/README.md` & `autosar-e2e-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 - [License](#license)
 
 ## Description
 
 This library provides fast C implementations of the E2E CRC algorithms and E2E profiles. 
 
 Currently, all relevant CRC algorithms are available in module `e2e.crc`
-but only E2E profiles 1 and 2 are available. 
+but only E2E profiles 1, 2 and 5 are available. 
 If you provide example data for the other profiles I would try to implement them, too.
 
 ## Installation
 
 ```console
 pip install autosar-e2e
 ```
```

### Comparing `autosar-e2e-0.3.0/pyproject.toml` & `autosar-e2e-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autosar-e2e-0.3.0/setup.py` & `autosar-e2e-0.4.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,15 +25,24 @@
     f"{import_pkg_name}.p02",
     sources=[
         str(pkg_dir / "p02.c"),
         str(pkg_dir / "crc.c"),
     ],
     include_dirs=[pkg_dir.as_posix()],
 )
+p05_module = Extension(
+    f"{import_pkg_name}.p05",
+    sources=[
+        str(pkg_dir / "p05.c"),
+        str(pkg_dir / "crc.c"),
+    ],
+    include_dirs=[pkg_dir.as_posix()],
+)
 
 setup(
     ext_modules=[
         crc_module,
         p01_module,
         p02_module,
+        p05_module,
     ],
 )
```

### Comparing `autosar-e2e-0.3.0/src/autosar_e2e.egg-info/PKG-INFO` & `autosar-e2e-0.4.0/src/autosar_e2e.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosar-e2e
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python implementation of the AUTOSAR E2E Protocol
 Author-email: Artur Drogunow <artur.drogunow@zf.com>
 License: MIT
 Project-URL: Documentation, https://autosar-e2e.readthedocs.io/en/latest
 Project-URL: Issues, https://github.com/zariiii9003/autosar-e2e/issues
 Project-URL: Source, https://github.com/zariiii9003/autosar-e2e
 Project-URL: Homepage, https://github.com/zariiii9003/autosar-e2e
@@ -41,15 +41,15 @@
 - [License](#license)
 
 ## Description
 
 This library provides fast C implementations of the E2E CRC algorithms and E2E profiles. 
 
 Currently, all relevant CRC algorithms are available in module `e2e.crc`
-but only E2E profiles 1 and 2 are available. 
+but only E2E profiles 1, 2 and 5 are available. 
 If you provide example data for the other profiles I would try to implement them, too.
 
 ## Installation
 
 ```console
 pip install autosar-e2e
 ```
```

### Comparing `autosar-e2e-0.3.0/src/e2e/crc.c` & `autosar-e2e-0.4.0/src/e2e/crc.c`

 * *Files identical despite different names*

### Comparing `autosar-e2e-0.3.0/src/e2e/crc.h` & `autosar-e2e-0.4.0/src/e2e/crc.h`

 * *Files identical despite different names*

### Comparing `autosar-e2e-0.3.0/src/e2e/crc.pyi` & `autosar-e2e-0.4.0/src/e2e/crc.pyi`

 * *Files identical despite different names*

### Comparing `autosar-e2e-0.3.0/src/e2e/p01.c` & `autosar-e2e-0.4.0/src/e2e/p01.c`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
              "Calculate CRC inplace according to AUTOSAR E2E Profile 1. \n"
              "\n"
              ":param bytearray data: \n"
              "    Mutable `bytes-like object <https://docs.python.org/3/glossary.html#term-bytes-like-object>`_\n"
              "    starting with the CRC byte. This CRC byte will be updated inplace. \n"
              ":param int length: \n"
              "    Number of data bytes which are considered for CRC calculation. `length` must fulfill \n"
-             "    the following condition: ``1 <= length < len(data)`` \n"
+             "    the following condition: ``1 <= length <= len(data) - 1`` \n"
              ":param int data_id: \n"
              "    A unique identifier which is used to protect against masquerading. The `data_id` is a 16bit unsigned integer. \n"
              ":param int data_id_mode: \n"
              "    This attribute describes the inclusion mode that is used to include the `data_id`. The possible inclusion modes are\n"
              "    :attr:`~e2e.p01.E2E_P01_DATAID_BOTH`, :attr:`~e2e.p01.E2E_P01_DATAID_ALT`, :attr:`~e2e.p01.E2E_P01_DATAID_LOW` \n"
              "    and :attr:`~e2e.p01.E2E_P01_DATAID_NIBBLE`.\n"
              ":param bool increment_counter: \n"
@@ -122,22 +122,22 @@
     }
 
     if (data.readonly)
     {
         PyErr_SetString(PyExc_ValueError, "\"data\" must be mutable. Use a bytearray or any object that implements the buffer protocol.");
         goto error;
     }
-    if (data.len < 2)
+    if (data.len <= 2)
     {
-        PyErr_SetString(PyExc_ValueError, "The length of bytearray \"data\" must be greater than 1.");
+        PyErr_SetString(PyExc_ValueError, "The length of bytearray \"data\" must be greater than 2.");
         goto error;
     }
     if (length < 1 || length > data.len - 1)
     {
-        PyErr_SetString(PyExc_ValueError, "Parameter \"length\" must fulfill the following condition: 1 <= length < len(data).");
+        PyErr_SetString(PyExc_ValueError, "Parameter \"length\" must fulfill the following condition: 1 <= length <= len(data) - 1.");
         goto error;
     }
 
     uint8_t *data_ptr = (uint8_t *)data.buf;
 
     // The counter goes either into low nibble or high nibble of data
     uint8_t counter = 0;
```

### Comparing `autosar-e2e-0.3.0/src/e2e/p01.pyi` & `autosar-e2e-0.4.0/src/e2e/p01.pyi`

 * *Files identical despite different names*

### Comparing `autosar-e2e-0.3.0/src/e2e/p02.c` & `autosar-e2e-0.4.0/src/e2e/p02.c`

 * *Files 3% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 
 #include <stdbool.h>
 #include <stdint.h>
 
 #include "crc.h"
 
 PyDoc_STRVAR(e2e_p02_protect_doc,
-             "e2e_p02_protect(data: bytearray, length: int, data_id_list: bytes, increment_counter: bool = True) -> None \n"
+             "e2e_p02_protect(data: bytearray, length: int, data_id_list: bytes, *, increment_counter: bool = True) -> None \n"
              "Calculate CRC inplace according to AUTOSAR E2E Profile 2. \n"
              "\n"
              ":param bytearray data: \n"
              "    Mutable `bytes-like object <https://docs.python.org/3/glossary.html#term-bytes-like-object>`_\n"
              "    starting with the CRC byte. This CRC byte will be updated inplace. \n"
              ":param int length: \n"
              "    Number of data bytes which are considered for CRC calculation. `length` must fulfill \n"
-             "    the following condition: ``1 <= length < len(data)`` \n"
+             "    the following condition: ``1 <= length <= len(data) - 1`` \n"
              ":param bytes data_id_list: \n"
              "    A `bytes-like object <https://docs.python.org/3/glossary.html#term-bytes-like-object>`_\n"
              "    of length 16 which is used to protect against masquerading. \n"
              ":param bool increment_counter: \n"
              "    If `True` the counter in byte 1 will be incremented before calculating the CRC. \n");
 
 static PyObject *
@@ -39,32 +39,32 @@
     static char *kwlist[] = {
         "data",
         "length",
         "data_id_list",
         "increment_counter",
         NULL};
 
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*ky*|p:e2e_p02_protect",
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*ky*|$p:e2e_p02_protect",
                                      kwlist, &data, &length, &data_id_list, &increment))
     {
         return NULL;
     }
     if (data.readonly)
     {
         PyErr_SetString(PyExc_ValueError, "\"data\" must be mutable. Use a bytearray or any object that implements the buffer protocol.");
         goto error;
     }
-    if (data.len < 2)
+    if (data.len <= 2)
     {
-        PyErr_SetString(PyExc_ValueError, "The length of bytearray \"data\" must be greater than 1.");
+        PyErr_SetString(PyExc_ValueError, "The length of bytearray \"data\" must be greater than 2.");
         goto error;
     }
     if (length < 1 || length > data.len - 1)
     {
-        PyErr_SetString(PyExc_ValueError, "Parameter \"length\" must fulfill the following condition: 1 <= length < len(data).");
+        PyErr_SetString(PyExc_ValueError, "Parameter \"length\" must fulfill the following condition: 1 <= length <= len(data) - 1.");
         goto error;
     }
     if (data_id_list.len != 16)
     {
         PyErr_SetString(PyExc_ValueError, "Argument \"data_id_list\" must be a bytes object with length 16.");
         goto error;
     }
@@ -100,15 +100,15 @@
              "Return ``True`` if CRC is correct according to AUTOSAR E2E Profile 2. \n"
              "\n"
              ":param data: \n"
              "    `bytes-like object <https://docs.python.org/3/glossary.html#term-bytes-like-object>`_\n"
              "    starting with the CRC byte. \n"
              ":param length: \n"
              "    Data byte count over which the CRC must be calculated. `length` must fulfill \n"
-             "    the following condition: ``1 <= length < len(data)`` \n"
+             "    the following condition: ``1 <= length <= len(data) - 1`` \n"
              ":param data_id_list: \n"
              "    A `bytes-like object <https://docs.python.org/3/glossary.html#term-bytes-like-object>`_\n"
              "    of length 16 which is used to protect against masquerading. \n"
              ":return:\n"
              "    `True` if CRC is valid, otherwise return `False`");
 
 static PyObject *
```

### Comparing `autosar-e2e-0.3.0/test/test_crc.py` & `autosar-e2e-0.4.0/test/test_crc.py`

 * *Files identical despite different names*

### Comparing `autosar-e2e-0.3.0/test/test_p01.py` & `autosar-e2e-0.4.0/test/test_p01.py`

 * *Files identical despite different names*

### Comparing `autosar-e2e-0.3.0/test/test_p02.py` & `autosar-e2e-0.4.0/test/test_p02.py`

 * *Files identical despite different names*

