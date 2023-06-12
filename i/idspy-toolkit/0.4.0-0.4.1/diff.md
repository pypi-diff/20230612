# Comparing `tmp/idspy_toolkit-0.4.0.tar.gz` & `tmp/idspy_toolkit-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idspy_toolkit-0.4.0.tar", last modified: Thu Jun  8 16:07:18 2023, max compression
+gzip compressed data, was "idspy_toolkit-0.4.1.tar", last modified: Mon Jun 12 10:50:43 2023, max compression
```

## Comparing `idspy_toolkit-0.4.0.tar` & `idspy_toolkit-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-08 16:07:18.461959 idspy_toolkit-0.4.0/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1599 2023-06-08 14:59:54.000000 idspy_toolkit-0.4.0/LICENSE
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     5013 2023-06-08 16:07:18.450953 idspy_toolkit-0.4.0/PKG-INFO
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2410 2023-06-08 16:07:08.000000 idspy_toolkit-0.4.0/README.rst
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-08 16:07:17.310120 idspy_toolkit-0.4.0/idspy_toolkit/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      611 2023-06-08 14:59:30.000000 idspy_toolkit-0.4.0/idspy_toolkit/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    14508 2023-06-08 14:59:30.000000 idspy_toolkit-0.4.0/idspy_toolkit/accessor.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2182 2023-06-08 14:59:30.000000 idspy_toolkit-0.4.0/idspy_toolkit/constants.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8579 2023-06-08 14:59:30.000000 idspy_toolkit-0.4.0/idspy_toolkit/converter.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1757 2023-06-08 14:59:30.000000 idspy_toolkit-0.4.0/idspy_toolkit/snippets.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8257 2023-06-08 14:59:30.000000 idspy_toolkit-0.4.0/idspy_toolkit/toolkit.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     6738 2023-06-08 14:59:30.000000 idspy_toolkit-0.4.0/idspy_toolkit/utils.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-08 16:07:17.757774 idspy_toolkit-0.4.0/idspy_toolkit.egg-info/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     5013 2023-06-08 16:07:15.000000 idspy_toolkit-0.4.0/idspy_toolkit.egg-info/PKG-INFO
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      548 2023-06-08 16:07:16.000000 idspy_toolkit-0.4.0/idspy_toolkit.egg-info/SOURCES.txt
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        1 2023-06-08 16:07:15.000000 idspy_toolkit-0.4.0/idspy_toolkit.egg-info/dependency_links.txt
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       94 2023-06-08 16:07:15.000000 idspy_toolkit-0.4.0/idspy_toolkit.egg-info/requires.txt
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       14 2023-06-08 16:07:15.000000 idspy_toolkit-0.4.0/idspy_toolkit.egg-info/top_level.txt
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     7894 2023-06-08 15:26:44.000000 idspy_toolkit-0.4.0/pyproject.toml
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       38 2023-06-08 16:07:18.464938 idspy_toolkit-0.4.0/setup.cfg
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       39 2023-06-08 15:03:37.000000 idspy_toolkit-0.4.0/setup.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-08 16:07:18.347628 idspy_toolkit-0.4.0/tests/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     5401 2023-06-08 14:51:40.000000 idspy_toolkit-0.4.0/tests/test_accessor.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     5184 2023-06-08 14:51:40.000000 idspy_toolkit-0.4.0/tests/test_converter_hdf5.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1493 2023-06-08 14:51:39.000000 idspy_toolkit-0.4.0/tests/test_hdf5_io.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2515 2023-06-08 14:51:40.000000 idspy_toolkit-0.4.0/tests/test_ids_browse.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1397 2023-06-08 14:51:40.000000 idspy_toolkit-0.4.0/tests/test_snippets.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1692 2023-06-08 14:51:39.000000 idspy_toolkit-0.4.0/tests/test_utils.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-12 10:50:43.095178 idspy_toolkit-0.4.1/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1599 2023-06-08 14:59:54.000000 idspy_toolkit-0.4.1/LICENSE
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     5436 2023-06-12 10:50:43.082233 idspy_toolkit-0.4.1/PKG-INFO
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2841 2023-06-12 10:46:26.000000 idspy_toolkit-0.4.1/README.rst
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-12 10:50:42.042017 idspy_toolkit-0.4.1/idspy_toolkit/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      611 2023-06-12 09:28:55.000000 idspy_toolkit-0.4.1/idspy_toolkit/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    14707 2023-06-12 09:28:01.000000 idspy_toolkit-0.4.1/idspy_toolkit/accessor.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2182 2023-06-08 14:59:30.000000 idspy_toolkit-0.4.1/idspy_toolkit/constants.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    10769 2023-06-12 09:28:19.000000 idspy_toolkit-0.4.1/idspy_toolkit/converter.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2245 2023-06-12 09:29:10.000000 idspy_toolkit-0.4.1/idspy_toolkit/snippets.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8365 2023-06-12 09:29:21.000000 idspy_toolkit-0.4.1/idspy_toolkit/toolkit.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     7094 2023-06-12 09:29:32.000000 idspy_toolkit-0.4.1/idspy_toolkit/utils.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-12 10:50:42.428149 idspy_toolkit-0.4.1/idspy_toolkit.egg-info/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     5436 2023-06-12 10:50:40.000000 idspy_toolkit-0.4.1/idspy_toolkit.egg-info/PKG-INFO
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      548 2023-06-12 10:50:41.000000 idspy_toolkit-0.4.1/idspy_toolkit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        1 2023-06-12 10:50:40.000000 idspy_toolkit-0.4.1/idspy_toolkit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       65 2023-06-12 10:50:40.000000 idspy_toolkit-0.4.1/idspy_toolkit.egg-info/requires.txt
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       14 2023-06-12 10:50:40.000000 idspy_toolkit-0.4.1/idspy_toolkit.egg-info/top_level.txt
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     7857 2023-06-12 09:25:37.000000 idspy_toolkit-0.4.1/pyproject.toml
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       38 2023-06-12 10:50:43.099905 idspy_toolkit-0.4.1/setup.cfg
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       39 2023-06-08 15:03:37.000000 idspy_toolkit-0.4.1/setup.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-12 10:50:42.971318 idspy_toolkit-0.4.1/tests/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     6344 2023-06-12 10:04:40.000000 idspy_toolkit-0.4.1/tests/test_accessor.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     6459 2023-06-12 10:05:13.000000 idspy_toolkit-0.4.1/tests/test_converter_hdf5.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1493 2023-06-08 14:51:39.000000 idspy_toolkit-0.4.1/tests/test_hdf5_io.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2542 2023-06-12 10:05:30.000000 idspy_toolkit-0.4.1/tests/test_ids_browse.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1397 2023-06-08 14:51:40.000000 idspy_toolkit-0.4.1/tests/test_snippets.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2217 2023-06-12 10:05:47.000000 idspy_toolkit-0.4.1/tests/test_utils.py
```

### Comparing `idspy_toolkit-0.4.0/LICENSE` & `idspy_toolkit-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.0/PKG-INFO` & `idspy_toolkit-0.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idspy_toolkit
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tools to manipulate the IDSPy Dictionaries
 Author-email: Guillaume Fuhr <guillaume.fuhr@univ-amu.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CNRS, contributor: Y. Camenen
         Copyright (c) 2023, Aix-Marseille Univ., contributor: G. Fuhr
         All rights reserved.
@@ -50,14 +50,21 @@
 Provides-Extra: test
 License-File: LICENSE
 
 IDSPy Toolkit
 =============
 
 Changelog :
+  * v 0.4.1
+
+   - correction of a bug with numpy.array having ndim=0 `#7 <https://gitlab.com/gkdb/imas-gk/-/issues/7>`_
+   - improved error message when trying to reach the root of an IDS using a path as string `#8 <https://gitlab.com/gkdb/imas-gk/-/issues/8>`_
+   - list_ids_members returns only all the ids members and not anymore ids root path also
+   - add possibility to overwrite HDF5 file written
+
   * v 0.4.0
 
    - pypi packaging
    - tests using tox
    - increase code coverage
 
   * v 0.3.0
@@ -87,20 +94,21 @@
  * hdf5_to_ids
  * get_ids_value_from_string
  * set_ids_value_from_string
  * list_ids_members
  * copy_ids
 
 
-**Please note that this work is stull under progress/heavy development and as experimental status.
+**Please note that this work is still under progress/heavy development and as experimental status.
 This means that functions arguments/signatures as long as HDF5 structure might be totally redesigned in the next updates.**
 
 ## Quick example
 #################################################################################################
 .. code-block:: python
+   :number-lines:
 
     import pprint
     import dataclasses
 
     import idspy_toolkit
     from idspy_dictionaries import ids_gyrokinetics
```

### Comparing `idspy_toolkit-0.4.0/README.rst` & `idspy_toolkit-0.4.1/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 IDSPy Toolkit
 =============
 
 Changelog :
+  * v 0.4.1
+
+   - correction of a bug with numpy.array having ndim=0 `#7 <https://gitlab.com/gkdb/imas-gk/-/issues/7>`_
+   - improved error message when trying to reach the root of an IDS using a path as string `#8 <https://gitlab.com/gkdb/imas-gk/-/issues/8>`_
+   - list_ids_members returns only all the ids members and not anymore ids root path also
+   - add possibility to overwrite HDF5 file written
+
   * v 0.4.0
 
    - pypi packaging
    - tests using tox
    - increase code coverage
 
   * v 0.3.0
@@ -35,20 +42,21 @@
  * hdf5_to_ids
  * get_ids_value_from_string
  * set_ids_value_from_string
  * list_ids_members
  * copy_ids
 
 
-**Please note that this work is stull under progress/heavy development and as experimental status.
+**Please note that this work is still under progress/heavy development and as experimental status.
 This means that functions arguments/signatures as long as HDF5 structure might be totally redesigned in the next updates.**
 
 ## Quick example
 #################################################################################################
 .. code-block:: python
+   :number-lines:
 
     import pprint
     import dataclasses
 
     import idspy_toolkit
     from idspy_dictionaries import ids_gyrokinetics
```

### Comparing `idspy_toolkit-0.4.0/idspy_toolkit/__init__.py` & `idspy_toolkit-0.4.1/idspy_toolkit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from idspy_toolkit.toolkit import fill_default_values_ids, list_ids_members,\
     get_ids_classes_as_dict
 from idspy_toolkit.converter import ids_to_hdf5, hdf5_to_ids
 from idspy_toolkit.accessor import get_ids_value_from_string, \
     set_ids_value_from_string, copy_ids
 from idspy_toolkit.utils import get_field_with_type
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 __all__ = [
     "__version__",
     "fill_default_values_ids",
     "ids_to_hdf5",
     "hdf5_to_ids",
     "get_ids_value_from_string",
```

### Comparing `idspy_toolkit-0.4.0/idspy_toolkit/accessor.py` & `idspy_toolkit-0.4.1/idspy_toolkit/accessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import dataclasses
 from dataclasses import Field
 from typing import get_type_hints, Any, get_origin, TypeVar, Type, Union
 from typing_extensions import Protocol
-from idspy_toolkit.utils import camel2snake, get_field_with_type, extract_ndarray_info
+from idspy_toolkit.utils import camel2snake,  extract_ndarray_info
 import inspect
 from numpy import ndarray
 
 
 class DataClass(Protocol):
     __dataclass_fields__: dict[str, Any]
 
@@ -52,15 +52,15 @@
 def get_type_arg(clazz: Type[DC], field_clazz: Union[str, Field[Any]]) -> Any:
     """
     Get the type argument of a dataclass field.
 
     :param clazz: The dataclass to get the field from.
     :param field_clazz: The name of the field to get the type argument from.
     :return: A tuple containing the type argument of the field and a boolean value indicating if the field is a list.
-    :raises AttributeError: If the specified field is not found in the dataclass.
+    :raises KeyError: If the specified field is not found in the dataclass.
 
     Examples:
         >>> @dataclass
         ... class Foo:
         ...     bar: list[int]
         ...
         >>> get_type_arg(Foo, 'bar')
@@ -98,14 +98,15 @@
 
     :param ids: The dataclass object to get the field_clazz value from.
     :param path: The path to the field_clazz within the dataclass object.
     :return: The value of the specified field_clazz.
     :raises AttributeError: If the specified path does not correspond to the type of the given dataclass object.
     :raises ValueError: If the specified path contains a non-existent field_clazz or if a list field_clazz is accessed with an out-of-range index.
     :raises TypeError: If the specified path contains a list field_clazz but the next part of the path is not an index.
+    :raises KeyError: If the specified path corresponds to an IDS root and not an IDS member.
 
     Examples:
         >>> @dataclass
         ... class Foo:
         ...     bar: int = 0
         ...
         >>> foo = Foo()
@@ -118,17 +119,19 @@
         ...     bar: List[str] = []
         ...
         >>> foo = Foo()
         >>> foo.bar = ['hello', 'world']
         >>> get_ids_value_from_string(foo, 'bar#0')
         'hello'
     """
-
-    path_members = __split_path(path, str(type(ids)))
-    current_attr = ids
+    try:
+        path_members = __split_path(path, str(type(ids)))
+        current_attr = ids
+    except IndexError:
+        raise KeyError("get_ids_value_from_string does not allow to get a full IDS, just IDS members")
 
     for idx, subpath in enumerate(path_members):
         if "#" in subpath:
             name, offset = subpath.strip().split("#")
             offset = int(offset)
             name = camel2snake(name)
             # TODO: check that return value of getattr is a list as expected
@@ -218,15 +221,15 @@
         # '#' indicates current item is a list element
         if "#" in subpath:
             name, offset = subpath.strip().split("#")
             offset = int(offset)
             name = camel2snake(name)
             list_attr = getattr(current_attr, name, None)
             len_list_attr = len(list_attr)
-            type_arg_list, is_list = get_type_arg(old_attr, name)
+            type_arg_list, _ = get_type_arg(old_attr, name)
             # TODO: exact role of create missing
             if name is None:
                 if create_missing is False:
                     raise AttributeError(f"missing element {subpath}")
             if not isinstance(list_attr, (list, tuple)):
                 raise AttributeError(f"element {name} is not a list")
             if len_list_attr < offset and offset > 0:
@@ -248,15 +251,15 @@
             if current_attr is None:
                 if create_missing is False:
                     raise AttributeError(f"missing element {subpath}")
                 else:
                     if isinstance(old_attr, (list, tuple)):
                         raise AttributeError(
                             f" item {path_members[idx - 1]} is represented by a list in the dataclass and should be "
-                            f"reached with the syntex item#XXXX")
+                            f"reached with the syntax item#XXXX")
                     if not dataclasses.is_dataclass(old_attr):
                         raise AttributeError(f" item {path_members[idx - 1]} is not of dataclass type {old_attr}")
 
     if isinstance(current_attr, (list, tuple)):
         raise AttributeError(f"attribute [{path_members[-2]}] is a list so it must be used as {path_members[-2]}#XXXX")
     if current_attr is None:
         raise AttributeError(f"attribute [{path_members[-2]}] is missing in the IDS {type(ids)}")
@@ -267,15 +270,15 @@
         offset = int(offset)
         attr_value = getattr(current_attr, name)
         if isinstance(attr_value, (list, tuple)):
             return setattr(current_attr, name[offset], value)
         else:
             raise AttributeError(f"attribute {name} is of type {type(attr_value)} and not list")
 
-    attr_type, attr_list = get_type_arg(current_attr, path_members[-1])
+    attr_type, _ = get_type_arg(current_attr, path_members[-1])
     if isinstance(value, bytes):
         value = value.decode("utf8")
     if isinstance(value, str) and (attr_type is not str):
         raise ValueError(
             f"value for attr {path_members[-1]} is of type {type(value)} and should be of type {attr_type}")
 
     setattr(current_attr, path_members[-1], value)
```

### Comparing `idspy_toolkit-0.4.0/idspy_toolkit/constants.py` & `idspy_toolkit-0.4.1/idspy_toolkit/constants.py`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.0/idspy_toolkit/converter.py` & `idspy_toolkit-0.4.1/idspy_toolkit/converter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 """
 
 """
 import dataclasses
 from typing import Any, Union, Tuple, TypeVar, Type
 from typing_extensions import Protocol
+from os import rename as os_rename
 import os
 import h5py
 import numpy as np
 import simplejson as js
 
-from idspy_toolkit.snippets import is_dataclass_instance, is_dataclass_field, sort_h5_keys
+from idspy_toolkit.snippets import is_dataclass_instance, is_dataclass_field, sort_h5_keys, _format_ids_substring
 from idspy_toolkit.constants import IMAS_DEFAULT_INT, IMAS_DEFAULT_FLOAT, IMAS_DEFAULT_CPLX, IMAS_DEFAULT_STR
 from idspy_toolkit.accessor import set_ids_value_from_string
 
+
 class DataClass(Protocol):
     __dataclass_fields__: dict[str, Any]
 
+
 DC = TypeVar("DC", bound=DataClass)
 
+
 def _create_hdf5_dataset(value_name: str, value, parent_group) -> int:
     """
         create the dataset and write the associated value
         dict as serialized as strings
     :param value_name:
     :param value:
     :param parent_group:
     :return: number of created dataset or ValueError in case where value is a list with more than one type of elements
     """
     if value is None:
         raise ValueError("cannot write None value in hdf5 file")
 
+    if isinstance(value, np.ndarray):
+        if value.ndim == 0:
+            value = float(value)
+
     str_type = h5py.special_dtype(vlen=str)
     parent_group.attrs["len"] = 1
     parent_group.attrs["type"] = "item"
     created_dataset = 1
     if isinstance(value, str):
         parent_group.create_dataset(value_name,
                                     data=value.encode("utf8"),
@@ -65,15 +73,19 @@
                                             dtype=str_type)
         elif isinstance(value_ref, (list, tuple)):
             inner_val = np.asarray(value)
             created_dataset = 1
             parent_group.create_dataset(value_name, data=inner_val, )
         else:
             created_dataset = 1
-            parent_group.create_dataset(value_name, data=value, )
+            try:
+                parent_group.create_dataset(value_name, data=value, )
+            except TypeError:
+                print(f"error raised for {value_name}:{value}/{type(value)}")
+                raise
     else:
         parent_group.create_dataset(value_name, data=value, )
 
     return created_dataset
 
 
 def get_inner_type_list(item: Union[list, tuple]) -> Union[Any, None]:
@@ -83,24 +95,66 @@
         try:
             test_var = test_var[0]
         except IndexError:
             return None
 
     return test_var
 
+def _is_list_empty(item: Any) -> bool:
+    """
+    Check if the given item is an empty list, tuple, or numpy array.
+
+    :param item: The item to be checked.
+    :type item: Any
+
+    :return: True if the item is an empty list, tuple, or numpy array, False otherwise.
+    :rtype: bool
+    """
+    if isinstance(item, (list, tuple)):
+        if len(item) == 0:
+            return True
+    elif isinstance(item, np.ndarray):
+        if item.ndim == 0:
+            return False
+        else:
+            if len(item) == 0:
+                return True
+    return False
+
+
+def _is_item_list(item: Any) -> bool:
+    """
+    Check if the given item is a list, tuple, or numpy array.
+
+    :param item: The item to be checked.
+    :type item: Any
+
+    :return: True if the item is a list, tuple, or numpy array, False otherwise.
+    :rtype: bool
+    """
+    if isinstance(item, (list, tuple)):
+        return True
+    elif isinstance(item, np.ndarray):
+        if item.ndim == 0:
+            return False
+        else:
+            return True
+    return False
+
 
-def ids_to_hdf5(ids: Type[DC], filename: str)->Tuple[int, int]:
+def ids_to_hdf5(ids: Type[DC], filename: str, overwrite:bool = False) -> Tuple[int, int]:
     """
     store an IDS class to a HDF5 file
     dict are stored as serialized json
     List of dict are serialized as a sequence of dataset
     List of values (int/float) as multidimensional dataset
     :param ids: IDS to store
     :param filename: name of the HDF5 file
-    :return: IOError if HDF5 file already exist, number of written groups and keys otherwise
+    :param overwrite: what to do if file already exists?
+    :return: IOError if HDF5 file already exist and overwrite is False, number of written groups and keys otherwise
     :TODO: manage empty files and empty group/dataclass
     :TODO: store strings as bytes
     """
     total_group: int = 0
     total_dataset: int = 0
 
     def _hdf5_header_metadata(parent_group):
@@ -114,50 +168,59 @@
         pass
 
     def __check_all_fields_none(current_ids, default_vals_list):
         number_fields = len(list(dataclasses.fields(current_ids)))
         list_default = []
         for field in dataclasses.fields(current_ids):
             field_value = getattr(current_ids, field.name)
-            if isinstance(field_value, (list, tuple, np.ndarray)):
+            if isinstance(field_value, (list, tuple)):
                 if len(field_value) == 0:
                     list_default.append(None)
+            elif isinstance(field_value, np.ndarray):
+                if field_value.ndim == 0:
+                    if field_value[()] in default_vals_list:
+                        list_default.append(None)
+                else:
+                    if len(field_value) == 0:
+                        list_default.append(None)
             elif field_value in default_vals_list:
                 list_default.append(None)
         return len(list_default) == number_fields
 
     def _browse_ids(current_ids, parent_group, ids_group: int, ids_dataset: int,
                     named_group: Union[str, None] = None,
                     flat_idx: Union[int, None] = None) -> tuple[int, int]:
         if named_group is None:
             root_grp = str(type(current_ids)).split(".")[-1][:-2]
         else:
             root_grp = named_group
         list_default_values = (IMAS_DEFAULT_INT, IMAS_DEFAULT_FLOAT,
                                IMAS_DEFAULT_CPLX, IMAS_DEFAULT_STR, None)
         if flat_idx is not None:
-            root_grp = "{0}#{1:04d}".format(root_grp, flat_idx)
+            root_grp = "{0}{1}".format(root_grp, _format_ids_substring(flat_idx))
 
         all_none = __check_all_fields_none(current_ids, list_default_values)
 
         if all_none is True:
             return ids_group, ids_dataset
 
         current_grp = parent_group.create_group(root_grp)
         ids_group += 1
 
         for field in dataclasses.fields(current_ids):
             field_name = field.name
             field_value = getattr(current_ids, field_name)
             # check if field contains one of the 'default' value
-            if isinstance(field_value, (list, tuple, np.ndarray)):
-                if len(field_value) == 0:
+            is_item_list = _is_item_list(field_value)
+            if is_item_list is True:
+                if _is_list_empty(field_value):
+                    continue
+            else:
+                if field_value in list_default_values:
                     continue
-            elif field_value in list_default_values:
-                continue
 
             if isinstance(field_value, (list, tuple)):
                 if len(field_value) == 0:
                     continue
                 if is_dataclass_instance(field_value[0]):
                     for i, sub_ids in enumerate(field_value):
                         ids_group, ids_dataset = _browse_ids(sub_ids, current_grp,
@@ -173,21 +236,27 @@
                                                      ids_group, ids_dataset,
                                                      named_group=field_name)
             else:
                 ids_dataset += _create_hdf5_dataset(field_name, field_value,
                                                     current_grp)
         return ids_group, ids_dataset
 
-    if os.path.exists(filename):
-        raise IOError(f"HDF5 file {filename} already exist")
-
+    if overwrite is False :
+        tmp_file = filename
+        if os.path.exists(filename):
+            raise IOError(f"HDF5 file {filename} already exist")
+    if overwrite is True :
+        tmp_file = filename+".tmp"
     # open the hdf5 file
-    with h5py.File(filename, "w") as h5f:
+    with h5py.File(tmp_file, "w") as h5f:
         total_group, total_dataset = _browse_ids(ids, h5f, total_group, total_dataset)
-
+    if overwrite is True:
+        os.remove(filename)
+        os_rename(tmp_file, filename)
+    print(f"IDS written to file : {filename}")
     return total_group, total_dataset
 
 
 def _iterate_hdf5_dataset(name: str, hdf5obj: Any, h5struct: list) -> None:
     if isinstance(hdf5obj, h5py.Dataset):
         h5struct.append(r"/" + name)
     return None
@@ -199,15 +268,15 @@
     :param filename: hdf5 filename
     :param ids: ids dataclass, has to be a fully develop IDS
     :return: IDS dataclass
     """
     if not os.path.exists(filename):
         raise IOError(f"HDF5 file {filename} not found")
 
-    h5struct_ds = []
+    h5struct_ds:list = []
     # open the hdf5 file and read it recursively
     with h5py.File(filename, "r") as h5f:
         h5f.visititems(lambda x, y: _iterate_hdf5_dataset(x, y, h5struct_ds))
         if len(h5struct_ds) == 0:
             raise ValueError(f"file [{filename}] seems to not contain any data")
         h5struct_ds = sort_h5_keys(h5struct_ds)
```

### Comparing `idspy_toolkit-0.4.0/idspy_toolkit/snippets.py` & `idspy_toolkit-0.4.1/idspy_toolkit/snippets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,32 @@
 from typing import Any
 from dataclasses import is_dataclass
 from dataclasses import Field, fields
 from typing import Union, Any
 import inspect
 
+_IDS_LIST_DELIMITER = "#"
+
+def _format_ids_substring(number: int, delimiter: str = "#") -> str:
+    """
+        return format for IDS list index.
+
+        Args:
+            number (int): index to consider.
+
+        Returns:
+            str:: A string representation of the list index.
+
+        Example:
+            >>> import idspy_toolkit
+            >>> format_ids_substring(123,"#")
+            #000123
+        """
+    return "{0}{1:06d}".format(delimiter, number)
+
 
 def is_dataclass_field(ids: object, item: Union["str", Field[Any]]) -> bool:
     """
     Check if an item is a dataclass field.
 
     :param ids: The object to check for the field.
     :param item: The item to check, which can be a string representing the field name or a Field instance.
```

### Comparing `idspy_toolkit-0.4.0/idspy_toolkit/toolkit.py` & `idspy_toolkit-0.4.1/idspy_toolkit/toolkit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import inspect
 import dataclasses
 from typing import Union, Type, TypeVar, Any, get_args
 from typing_extensions import Protocol
 import numpy as np
 
-from idspy_toolkit.snippets import is_dataclass_field, is_dataclass_instance
+from idspy_toolkit.snippets import is_dataclass_field, is_dataclass_instance, _format_ids_substring
 from idspy_toolkit.utils import snake2camel, extract_ndarray_info, _imas_default_values
 from idspy_toolkit.accessor import get_type_arg
 
 
 class DataClass(Protocol):
     __dataclass_fields__: dict[str, Any]
 
+
 DC = TypeVar("DC", bound=DataClass)
 
-def get_ids_classes_as_dict(module_alias) -> dict[str,Type]:
+
+
+def get_ids_classes_as_dict(module_alias) -> dict[str, Type]:
     """
     Extracts the names of all dataclasses in the specified module.
 
     Args:
         module_alias (module): A module object or an alias to a module.
 
     Returns:
@@ -31,15 +34,16 @@
     Example:
         >>> import my_module
         >>> get_ids_classes_as_dict(my_module)
         {'Person':Person, 'Address':Address}
     """
     if not inspect.ismodule(module_alias):
         raise TypeError(f"module_alias should be a module object or alias, not {type(module_alias)}")
-    return {x[0]:x[1] for x in inspect.getmembers(module_alias) if inspect.isclass(x[1]) and hasattr(x[1], '__dataclass_fields__')}
+    return {x[0]: x[1] for x in inspect.getmembers(module_alias) if
+            inspect.isclass(x[1]) and hasattr(x[1], '__dataclass_fields__')}
 
 
 def list_ids_members(ids: Type[DC], ) -> list:
     """
     List all attributes' IDs of a dataclass instance and its nested dataclass instances.
 
 
@@ -101,17 +105,18 @@
         """
         if named_group is None:
             root_grp = delimiter + str(type(current_ids)).split(".")[-1][:-2]
         else:
             root_grp = named_group
 
         if flat_idx is not None:
-            root_grp = "{0}#{1:04d}".format(root_grp, flat_idx)
+            root_grp = "{0}{1}".format(root_grp, _format_ids_substring(flat_idx))
 
-        list_attrs.append(root_grp)
+        # do not print sub ids "root path"
+        # list_attrs.append(root_grp)
         for field in dataclasses.fields(current_ids):
             field_name = field.name
             field_value = getattr(current_ids, field_name)
             named_group = root_grp + delimiter + field_name
             if isinstance(field_value, (list, tuple)):
                 if len(field_value) == 0:
                     continue
```

### Comparing `idspy_toolkit-0.4.0/idspy_toolkit/utils.py` & `idspy_toolkit-0.4.1/idspy_toolkit/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from inspect import getmembers, isclass
 from typing_extensions import Protocol
 import numpy as np
 import re
 from idspy_toolkit.snippets import is_dataclass_field
 from inspect import isdatadescriptor
 
+
 class DataClass(Protocol):
     __dataclass_fields__: dict[str, Any]
 
 
 DC = TypeVar("DC", bound=DataClass)
 
 
@@ -113,15 +114,14 @@
     elif hasattr(ids, "__dataclass_fields__"):
         if ids.__dataclass_fields__.get(ids_field, None) is not None:
             extracted_field: dict[str, Any] = ids.__dataclass_fields__.get(ids_field)
             field_value = getattr(ids, extracted_field.name)
     else:
         raise ValueError(f"argument {str(ids_field)} does not represent a fieldname of the class {str(ids)}")
 
-
     expected_field_type = __get_field_type(extracted_field)
     if field_value is None:
         return None, expected_field_type
 
     if isinstance(field_value, (tuple, list)):
         if len(field_value) == 0:
             return field_value, expected_field_type
@@ -174,9 +174,15 @@
 
     match = re.match(pattern, expr)
     if match:
         contents = match.group(1)
         data_type = match.group(2)
     else:
         raise ValueError(f"expression {expr} does not match with an numpy.ndarray")
+
+    dim_set = tuple(set([x.strip() for x in contents.split(',') if x != '']))
+    if len(dim_set) > 1:
+        raise ValueError(f"expression {expr} does not match with an numpy.ndarray, dimension error")
+    if dim_set[0] != "<class 'int'>":
+        raise ValueError(f"expression {expr} does not match with an numpy.ndarray, dimension has to be integer")
     shape = (0,) * len([x for x in contents.split(',') if x != ''])
     return shape, data_type_equiv.get(data_type, str)
```

### Comparing `idspy_toolkit-0.4.0/idspy_toolkit.egg-info/PKG-INFO` & `idspy_toolkit-0.4.1/idspy_toolkit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idspy-toolkit
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tools to manipulate the IDSPy Dictionaries
 Author-email: Guillaume Fuhr <guillaume.fuhr@univ-amu.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CNRS, contributor: Y. Camenen
         Copyright (c) 2023, Aix-Marseille Univ., contributor: G. Fuhr
         All rights reserved.
@@ -50,14 +50,21 @@
 Provides-Extra: test
 License-File: LICENSE
 
 IDSPy Toolkit
 =============
 
 Changelog :
+  * v 0.4.1
+
+   - correction of a bug with numpy.array having ndim=0 `#7 <https://gitlab.com/gkdb/imas-gk/-/issues/7>`_
+   - improved error message when trying to reach the root of an IDS using a path as string `#8 <https://gitlab.com/gkdb/imas-gk/-/issues/8>`_
+   - list_ids_members returns only all the ids members and not anymore ids root path also
+   - add possibility to overwrite HDF5 file written
+
   * v 0.4.0
 
    - pypi packaging
    - tests using tox
    - increase code coverage
 
   * v 0.3.0
@@ -87,20 +94,21 @@
  * hdf5_to_ids
  * get_ids_value_from_string
  * set_ids_value_from_string
  * list_ids_members
  * copy_ids
 
 
-**Please note that this work is stull under progress/heavy development and as experimental status.
+**Please note that this work is still under progress/heavy development and as experimental status.
 This means that functions arguments/signatures as long as HDF5 structure might be totally redesigned in the next updates.**
 
 ## Quick example
 #################################################################################################
 .. code-block:: python
+   :number-lines:
 
     import pprint
     import dataclasses
 
     import idspy_toolkit
     from idspy_dictionaries import ids_gyrokinetics
```

### Comparing `idspy_toolkit-0.4.0/idspy_toolkit.egg-info/SOURCES.txt` & `idspy_toolkit-0.4.1/idspy_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.0/pyproject.toml` & `idspy_toolkit-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,28 +6,26 @@
     "setuptools>=61.0.0",
     "wheel",
 ]
 # build-backend = "setuptools.build_meta"
 
 [project]
 name = 'idspy_toolkit'
-version = '0.4.0'
+version = '0.4.1'
 description = 'Tools to manipulate the IDSPy Dictionaries'
 readme = 'README.rst'
 authors = [
   { name = 'Guillaume Fuhr', email='guillaume.fuhr@univ-amu.fr' },
 ]
 license = {file = 'LICENSE'}
 requires-python = '>=3.10'
 dependencies = [
   "idspy_dictionaries>=0.3.1",
 "numpy>=1.22",
-"h5py",
-"simplejson",
-"typing_extensions"
+"h5py"
 ]
 
 classifiers = [
     'Development Status :: 4 - Beta',
     'Environment :: Console',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: MIT License',
```

### Comparing `idspy_toolkit-0.4.0/tests/test_accessor.py` & `idspy_toolkit-0.4.1/tests/test_accessor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 import dataclasses
 from typing import Optional
 from numpy import ndarray
 
 from tests.classes_skels import *
 from idspy_toolkit.accessor import get_ids_value_from_string, \
-    set_ids_value_from_string, is_list_member, copy_ids
-
+    set_ids_value_from_string, is_list_member, copy_ids, get_type_arg
+from idspy_toolkit.toolkit import list_ids_members
 
 @dataclasses.dataclass
 class SubSubClass:
     member_subsubclass_aa: Optional[str] = dataclasses.field(default=""
                                                              )
     member_subsubclass_bb: Optional[int] = dataclasses.field(default=999999999
                                                              )
@@ -68,19 +68,31 @@
 class MainDataClass:
     field1: str
     field2: int
     subfield: SubDataClass
     subfield_list: list[SubDataClass]
 
 
+@dataclasses.dataclass
+class MyClass:
+    my_list: list[int]
+    my_string: str
+
+def test_get_type_arg():
+    assert get_type_arg(MyClass, "my_list") == (int, True)
+    assert get_type_arg(MyClass, "my_string") == (str, False)
+    with pytest.raises(KeyError):
+        get_type_arg(MyClass, "nonexistent_field")
+
+
 def test_is_list_member():
     assert is_list_member(BaseClass, "list_member") is True
     assert is_list_member(BaseClass, "list_member_foreign") is True
     assert is_list_member(BaseClass, "nda_member") is False
-
+    assert is_list_member(MainDataClass, "subfield_list") is True
 
 def test_get_ids_value_from_string():
     # create source dataclass with nested dataclass containing list
     source_subfield_list = [
         SubDataClass("subfield1_1", 1),
         SubDataClass("subfield1_2", 2),
         SubDataClass("subfield1_3", 3),
@@ -97,21 +109,27 @@
         SubDataClass("dest_subfield1_4", 40),
         SubDataClass("dest_subfield1_5", 50)
     ]
     dest_dataclass = MainDataClass("dest_field1", 456, SubDataClass("dest_subfield1", 100), dest_subfield_list)
 
     # copy source to destination
     copy_ids(dest_dataclass, source_dataclass)
+    with pytest.raises(KeyError):
+        get_ids_value_from_string(source_dataclass, "/MainDataClass/subfield_list#000000/")
+    with pytest.raises(KeyError):
+        get_ids_value_from_string(source_dataclass, "/MainDataClass/subfield_list#000001/")
+    with pytest.raises(KeyError):
+        get_ids_value_from_string(source_dataclass, "/MainDataClass/subfield_list#000001")
 
     # check that destination dataclass now has same values as source dataclass
     assert get_ids_value_from_string(dest_dataclass, "field1") == "field1"
     assert get_ids_value_from_string(dest_dataclass, "field2") == 123
     assert get_ids_value_from_string(dest_dataclass, "subfield/subfield1") == "subfield1"
     assert get_ids_value_from_string(dest_dataclass, "subfield/subfield2") == 1
-
+    assert get_ids_value_from_string(source_dataclass, "subfield_list#000001/subfield1") == "subfield1_2"
 
 def test_set_ids_value_from_string():
     # Create a test instance of MainDataClass
     test_mc = DbgMainDataClass(
         field1="value1",
         field2=123,
         subfield_list=[
```

### Comparing `idspy_toolkit-0.4.0/tests/test_hdf5_io.py` & `idspy_toolkit-0.4.1/tests/test_hdf5_io.py`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.0/tests/test_ids_browse.py` & `idspy_toolkit-0.4.1/tests/test_ids_browse.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,53 +32,53 @@
 
 
 
 def test_list_ids_members():
     # Test case 1: list all attribute IDs of a simple dataclass instance
     person = Person(name="John", age=30, address=Address(street="123 Main St.", city="New York", zip_code=10001))
     expected_ids = [
-        "/Person",
+    #    "/Person",
         "/Person/name",
         "/Person/age",
-        "/Person/address",
+    #    "/Person/address",
         "/Person/address/street",
         "/Person/address/city",
         "/Person/address/zip_code"
     ]
     assert sorted(list_ids_members(person)) == sorted(expected_ids)
 
     # Test case 2: list all attribute IDs of a nested dataclass instance
     employee = Employee(id=1, person=person)
     expected_ids = [
-        "/Employee",
+     #   "/Employee",
         "/Employee/id",
-        "/Employee/person",
+     #   "/Employee/person",
         "/Employee/person/name",
         "/Employee/person/age",
-        "/Employee/person/address",
+     #   "/Employee/person/address",
         "/Employee/person/address/street",
         "/Employee/person/address/city",
         "/Employee/person/address/zip_code"
     ]
     assert sorted(list_ids_members(employee)) == sorted(expected_ids)
 
     # Test case 3: list all attribute IDs of a dataclass instance with a list of nested dataclass instances
     department = Department(id=1, name="Sales", employees=[employee])
     expected_ids = [
-        "/Department",
+    #    "/Department",
         "/Department/id",
         "/Department/name",
-        "/Department/employees#0000",
-        "/Department/employees#0000/id",
-        "/Department/employees#0000/person",
-        "/Department/employees#0000/person/name",
-        "/Department/employees#0000/person/age",
-        "/Department/employees#0000/person/address",
-        "/Department/employees#0000/person/address/street",
-        "/Department/employees#0000/person/address/city",
-        "/Department/employees#0000/person/address/zip_code"
+  #      "/Department/employees#000000",
+        "/Department/employees#000000/id",
+   #     "/Department/employees#000000/person",
+        "/Department/employees#000000/person/name",
+        "/Department/employees#000000/person/age",
+    #    "/Department/employees#000000/person/address",
+        "/Department/employees#000000/person/address/street",
+        "/Department/employees#000000/person/address/city",
+        "/Department/employees#000000/person/address/zip_code"
     ]
     assert sorted(list_ids_members(department)) == sorted(expected_ids)
 
     # Test case 4: raise TypeError if the input parameter is not a dataclass instance
     with pytest.raises(TypeError):
         list_ids_members("not a dataclass instance")
```

### Comparing `idspy_toolkit-0.4.0/tests/test_snippets.py` & `idspy_toolkit-0.4.1/tests/test_snippets.py`

 * *Files identical despite different names*

