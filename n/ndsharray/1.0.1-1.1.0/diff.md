# Comparing `tmp/ndsharray-1.0.1-py3-none-any.whl.zip` & `tmp/ndsharray-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 8378 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      271 b- defN 22-Aug-24 13:14 ndsharray/__init__.py
--rw-rw-rw-  2.0 fat    17265 b- defN 22-Aug-24 09:48 ndsharray/ndsharray.py
--rw-rw-rw-  2.0 fat     1548 b- defN 22-Aug-24 13:16 ndsharray-1.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3755 b- defN 22-Aug-24 13:16 ndsharray-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Aug-24 13:16 ndsharray-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 22-Aug-24 13:16 ndsharray-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      553 b- defN 22-Aug-24 13:16 ndsharray-1.0.1.dist-info/RECORD
-7 files, 23494 bytes uncompressed, 7400 bytes compressed:  68.5%
+Zip file size: 8498 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      271 b- defN 23-Jun-12 06:51 ndsharray/__init__.py
+-rw-rw-rw-  2.0 fat    18159 b- defN 23-Jun-12 06:50 ndsharray/ndsharray.py
+-rw-rw-rw-  2.0 fat     1548 b- defN 23-Jun-12 07:00 ndsharray-1.1.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3688 b- defN 23-Jun-12 07:00 ndsharray-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 07:00 ndsharray-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-12 07:00 ndsharray-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      553 b- defN 23-Jun-12 07:00 ndsharray-1.1.0.dist-info/RECORD
+7 files, 24321 bytes uncompressed, 7520 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: ndsharray/__init__.py
 Comment: 
 
 Filename: ndsharray/ndsharray.py
 Comment: 
 
-Filename: ndsharray-1.0.1.dist-info/LICENSE
+Filename: ndsharray-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: ndsharray-1.0.1.dist-info/METADATA
+Filename: ndsharray-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: ndsharray-1.0.1.dist-info/WHEEL
+Filename: ndsharray-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: ndsharray-1.0.1.dist-info/top_level.txt
+Filename: ndsharray-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ndsharray-1.0.1.dist-info/RECORD
+Filename: ndsharray-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ndsharray/__init__.py

```diff
@@ -1,11 +1,11 @@
 """Top-level package"""
 
 from ndsharray.ndsharray import NdShArray
 from ndsharray.ndsharray import supported_types
 
 __author__ = 'Rune Monzel'
 __email__ = 'runemonzel@googlemail.com'
-__version__ = '1.0.1'
+__version__ = '1.1.0'
 __all__ = ["NdShArray",
            "supported_types"]
```

## ndsharray/ndsharray.py

```diff
@@ -112,23 +112,25 @@
         self._mmap: mmap.mmap
         self._fd: Union[None, int] = None
 
         # holds the numpy ndarray
         self._ndarray_mmap: Union[None, mmap.mmap] = None
         self._ndarray_fd: Union[None, int] = None
 
+        self._is_valid = False
+
         # buffer size of the _mmap_ndarray
         _bytes = self._array_to_bytes(self._array)
         self._buffer_size: int = len(_bytes)
 
         # create the mmap which holds the name of the ndarray mmap
         self._mmap, self._fd = self._create_mmap(self._name, len(self.ndarray_mmap_name), r_w=self._access)
 
         # create ndarray mmap
-        self._create_ndarray_mmap()
+        self._is_valid = self._create_ndarray_mmap()
 
         if self._access == "w":
             self.write(array)  # call write to force saving the array via mmap.flush!
 
     def __del__(self):
 
         # closing the mmap
@@ -144,14 +146,23 @@
         the name must be declared at class instantiation and is read only after instantiation
 
         :return name:
         """
         return self._name
 
     @property
+    def is_valid(self) -> bool:
+        """
+        checks if the header of the numpy array is valid or not
+
+        :return:
+        """
+        return self._is_valid
+
+    @property
     def ndarray_mmap_name(self) -> str:
         """
         returns the name of the mmap which holds the current ndarray
 
         ndarray_mmap_name consists of the name and an uuid which is generated for each new ndarray size (changes in
         dtype, shape or dimension does a change in size)
 
@@ -329,44 +340,45 @@
         # get the ndarray mmap name
         self._mmap.seek(0)
         _ndarray_mmap_name = bytes_to_str(self._mmap.read(len(self._name)+33))
         if _ndarray_mmap_name != self.ndarray_mmap_name:
             self._create_ndarray_mmap()
             _recreated_map = True
 
-        # first stage of checking if new data have been arrived
-        self._ndarray_mmap.seek(0)
-        _bytes = self._ndarray_mmap.read(8)
-        try:
-            _write_time = struct.unpack("d", _bytes)[0]
-        except ValueError:
-            _write_time = 0
-        if _write_time <= self._last_write_time and not _recreated_map:
-            return False, _numpy_array
-
-        # without checking, read the whole buffer
-        _bytes += self._ndarray_mmap.read()
-
-        if len(_bytes) != self._buffer_size:
-            self._create_ndarray_mmap()
-
-        _mmap_correct, _validity, _numpy_array = self._bytes_to_array(_bytes)
-        if not _mmap_correct:
-            warnings.warn("The mmap of the ndarray seems to be corrupt and the used protocol does not fit.",
-                          BytesWarning)
-
-        # for efficiency
-        self._array = _numpy_array
-        # for debug purpose
-        self._read_time_ms = (time.monotonic()-_write_time) * 1000.0
-        self._last_write_time = _write_time
+        if self._is_valid:
+            # first stage of checking if new data have been arrived
+            self._ndarray_mmap.seek(0)
+            _bytes = self._ndarray_mmap.read(8)
+            try:
+                _write_time = struct.unpack("d", _bytes)[0]
+            except ValueError:
+                _write_time = 0
+            if _write_time <= self._last_write_time and not _recreated_map:
+                return False, _numpy_array
+
+            # without checking, read the whole buffer
+            _bytes += self._ndarray_mmap.read()
+
+            if len(_bytes) != self._buffer_size:
+                self._create_ndarray_mmap()
+
+            _mmap_correct, _validity, _numpy_array = self._bytes_to_array(_bytes)
+            if not _mmap_correct:
+                warnings.warn("The mmap of the ndarray seems to be corrupt and the used protocol does not fit.",
+                              BytesWarning)
+
+            # for efficiency
+            self._array = _numpy_array
+            # for debug purpose
+            self._read_time_ms = (time.monotonic()-_write_time) * 1000.0
+            self._last_write_time = _write_time
 
         return _validity, _numpy_array
 
-    def _create_ndarray_mmap(self) -> None:
+    def _create_ndarray_mmap(self) -> bool:
         """
         creates two mmap:
             - the mmap with tag 'name' just holds the mmap-tag-name of ndarray
             - the mmap of the ndarray may change its name every time a new shape, dimension or dtype is detected
 
         :return:
         """
@@ -382,46 +394,56 @@
             self._ndarray_mmap, self._ndarray_fd = self._create_mmap(self.ndarray_mmap_name, self._buffer_size,
                                                                      r_w=self._access)
 
         elif self._access == "r":
             self._mmap.seek(0)
             _ndarray_mmap_name = bytes_to_str(self._mmap.read(len(self._name)+33))
             self._uuid = _ndarray_mmap_name[-32:]
-
-            # create temporary mmap to get the dtype and dimension of the array
-            _tmp_mmap, _tmp_fd = self._create_mmap(self.ndarray_mmap_name, 8+2*n_bytes_for_int, r_w="r")
-            _tmp_mmap.seek(0)
-            _bytes = _tmp_mmap.read(8+2*n_bytes_for_int)  # skip the time: +8
-            idx = 8
-            _np_dtype = supported_types[bytes_to_int(_bytes[idx:idx+n_bytes_for_int])]
-            idx += n_bytes_for_int
-            _np_dim = bytes_to_int(_bytes[idx:idx+n_bytes_for_int])
-            self._close_mmap(_tmp_mmap, _tmp_fd)
-
-            # create temporary mmap to get the shape of the array
-            _tmp_2_mmap, _tmp_2_fd = self._create_mmap(self.ndarray_mmap_name,
-                                                       8 + 2 * n_bytes_for_int + _np_dim * n_bytes_for_int,
-                                                       r_w="r")
-            _tmp_2_mmap.seek(8+2*n_bytes_for_int)  # skip the time, dtype and dimension
-            # read shape
-            _bytes += _tmp_2_mmap.read(_np_dim * n_bytes_for_int)
-            idx = 8 + 2 * n_bytes_for_int
-            _np_shape = []
-            for s in range(_np_dim):
-                _np_shape.append(bytes_to_int(_bytes[idx:idx + n_bytes_for_int]))
-                idx += n_bytes_for_int
-            _np_shape = tuple(_np_shape)
-            self._close_mmap(_tmp_2_mmap, _tmp_2_fd)
-
-            # rebuild _array and get the length of the byte array -> super lazy and inefficient...
-            self._array = np.ndarray(_np_shape, dtype=_np_dtype)
-            self._buffer_size = len(self._array_to_bytes(self._array))
-
-            self._ndarray_mmap, self._ndarray_fd = self._create_mmap(self.ndarray_mmap_name, self._buffer_size,
-                                                                     r_w=self._access)
+            try:
+                int(self._uuid, 16)
+                self._is_valid = True
+            except ValueError:
+                self._is_valid = False
+
+            try:
+                if self._is_valid:
+                    # create temporary mmap to get the dtype and dimension of the array
+                    _tmp_mmap, _tmp_fd = self._create_mmap(self.ndarray_mmap_name, 8+2*n_bytes_for_int, r_w="r")
+                    _tmp_mmap.seek(0)
+                    _bytes = _tmp_mmap.read(8+2*n_bytes_for_int)  # skip the time: +8
+                    idx = 8
+                    _np_dtype = supported_types[bytes_to_int(_bytes[idx:idx+n_bytes_for_int])]
+                    idx += n_bytes_for_int
+                    _np_dim = bytes_to_int(_bytes[idx:idx+n_bytes_for_int])
+                    self._close_mmap(_tmp_mmap, _tmp_fd)
+
+                    # create temporary mmap to get the shape of the array
+                    _tmp_2_mmap, _tmp_2_fd = self._create_mmap(self.ndarray_mmap_name,
+                                                               8 + 2 * n_bytes_for_int + _np_dim * n_bytes_for_int,
+                                                               r_w="r")
+                    _tmp_2_mmap.seek(8+2*n_bytes_for_int)  # skip the time, dtype and dimension
+                    # read shape
+                    _bytes += _tmp_2_mmap.read(_np_dim * n_bytes_for_int)
+                    idx = 8 + 2 * n_bytes_for_int
+                    _np_shape = []
+                    for s in range(_np_dim):
+                        _np_shape.append(bytes_to_int(_bytes[idx:idx + n_bytes_for_int]))
+                        idx += n_bytes_for_int
+                    _np_shape = tuple(_np_shape)
+                    self._close_mmap(_tmp_2_mmap, _tmp_2_fd)
+
+                    # rebuild _array and get the length of the byte array -> super lazy and inefficient...
+                    self._array = np.ndarray(_np_shape, dtype=_np_dtype)
+                    self._buffer_size = len(self._array_to_bytes(self._array))
+
+                    self._ndarray_mmap, self._ndarray_fd = self._create_mmap(self.ndarray_mmap_name, self._buffer_size,
+                                                                             r_w=self._access)
+            except:
+                self.is_valid = False
+        return self._is_valid
 
     @staticmethod
     def _create_mmap(name: str, buffer_size: int, r_w: str) -> Tuple[mmap.mmap, Union[None, int]]:
         """
         static helper function to create a mmap for a specific  operating system
 
         :param name:
```

## Comparing `ndsharray-1.0.1.dist-info/LICENSE` & `ndsharray-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ndsharray-1.0.1.dist-info/METADATA` & `ndsharray-1.1.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndsharray
-Version: 1.0.1
+Version: 1.1.0
 Summary: Sharing numpy ndarray with a simple API between different python processes with shared memory.
 Home-page: https://github.com/monzelr/ndsharray
 Author: Rune Monzel
 Author-email: runemonzel@googlemail.com
 License: BSD 3-Clause License
 Keywords: sharing numpy arrays,inter process communication,subprocess,multiple process reading a numpy ndarray
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,18 +32,18 @@
 ------------
 This python module let you share a numpy ndarray within different processes (either via python's multiprocessing or 
 sharing between different python instances). The library behind this package is the lib 
 [mmap](https://docs.python.org/3/library/mmap.html) from official python - no extra library, except numpy, is needed. 
 The mmap approach is using the shared memory, which can be accessed by different CPUs/python instances. Using shared 
 memory is much 
 faster than the pickle approach - you can even do a video streaming on a Raspberry Pi / Jetson Nano over multiple 
-python processes\
-This library is eas to use, just initialize the shared array with a unique tag and write/read! You can even change the 
-numpy array size/shape/dtype during runtime - the mmap will be silently rebuild if there is a change in the numpy array 
-size/shape/dtype.
+python processes.\
+This library is easy-to-use, just initialize the shared array with a unique tag and write/read! You can even change the 
+numpy array dimension/shape/dtype during runtime - the mmap will be silently rebuild if there is a change in the 
+numpy array  size/shape/dtype.
 
 Small Example Code:
 ```python
 import numpy as np
 from ndsharray import NdShArray
     
 shared_array = NdShArray("my_unique_tag", r_w='w')  # r_w must be specified
@@ -84,25 +84,26 @@
 Some technical notes
 --------------------
 This library shall be an easy-to-use library and also shall be faster than pickling numpy arrays to another process. 
 Please note that the python's provided 
 [shared_memory](https://docs.python.org/3/library/multiprocessing.shared_memory.html) does the same as ndsharray, but 
 is using byte array instead of numpy array! However, shared_memory is available since python 3.8 and not 
 supported for python 3.6.
-The performance of this library is good enough for video streaming (see also example)!
 
 
 Installation from Github
 ------------------------
 Make sure to have git, python and pip in your environment path or activate your python environment.\
 To install enter in cmd/shell:
+```console
+git clone https://github.com/monzelr/ndsharray.git
 
-    git clone https://github.com/monzelr/ndsharray.git
+cd ndsharray
 
-    cd ndsharray
-
-    pip install .
+pip install .
+```
 
 Alternative with python:
-
-    python setup.py install
+```console
+python setup.py install
+```
```

