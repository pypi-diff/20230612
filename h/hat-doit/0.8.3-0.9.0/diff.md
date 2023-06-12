# Comparing `tmp/hat_doit-0.8.3-cp38.cp39.cp310-none-any.whl.zip` & `tmp/hat_doit-0.9.0-cp38.cp39.cp310-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13360 bytes, number of entries: 13
+Zip file size: 13783 bytes, number of entries: 13
 -rw-r--r--  2.0 unx        0 b- defN 21-Aug-04 17:49 hat/doit/__init__.py
--rw-r--r--  2.0 unx     6434 b- defN 21-Dec-29 18:31 hat/doit/c.py
--rw-r--r--  2.0 unx     4211 b- defN 21-Dec-29 18:44 hat/doit/common.py
+-rw-r--r--  2.0 unx     8896 b- defN 22-May-27 21:20 hat/doit/c.py
+-rw-r--r--  2.0 unx     4353 b- defN 22-May-27 20:47 hat/doit/common.py
 -rw-r--r--  2.0 unx     2016 b- defN 22-Mar-26 18:59 hat/doit/docs.py
 -rw-r--r--  2.0 unx     1941 b- defN 21-Nov-07 15:49 hat/doit/js.py
--rw-r--r--  2.0 unx     5484 b- defN 21-Dec-29 18:27 hat/doit/py.py
+-rw-r--r--  2.0 unx     5594 b- defN 22-May-27 21:19 hat/doit/py.py
 -rw-r--r--  2.0 unx        0 b- defN 22-May-16 16:08 hat/doit/sphinx/__init__.py
 -rw-r--r--  2.0 unx      359 b- defN 22-May-16 15:10 hat/doit/sphinx/static/hat.css
--rw-r--r--  2.0 unx    11358 b- defN 22-May-16 16:09 hat_doit-0.8.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1953 b- defN 22-May-16 16:09 hat_doit-0.8.3.dist-info/METADATA
--rw-r--r--  2.0 unx      132 b- defN 22-May-16 16:09 hat_doit-0.8.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 22-May-16 16:09 hat_doit-0.8.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      993 b- defN 22-May-16 16:09 hat_doit-0.8.3.dist-info/RECORD
-13 files, 34885 bytes uncompressed, 11718 bytes compressed:  66.4%
+-rw-r--r--  2.0 unx    11358 b- defN 22-May-27 21:48 hat_doit-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1953 b- defN 22-May-27 21:48 hat_doit-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      132 b- defN 22-May-27 21:48 hat_doit-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 22-May-27 21:48 hat_doit-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      993 b- defN 22-May-27 21:48 hat_doit-0.9.0.dist-info/RECORD
+13 files, 37599 bytes uncompressed, 12141 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: hat/doit/sphinx/__init__.py
 Comment: 
 
 Filename: hat/doit/sphinx/static/hat.css
 Comment: 
 
-Filename: hat_doit-0.8.3.dist-info/LICENSE
+Filename: hat_doit-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: hat_doit-0.8.3.dist-info/METADATA
+Filename: hat_doit-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: hat_doit-0.8.3.dist-info/WHEEL
+Filename: hat_doit-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: hat_doit-0.8.3.dist-info/top_level.txt
+Filename: hat_doit-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: hat_doit-0.8.3.dist-info/RECORD
+Filename: hat_doit-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hat/doit/c.py

```diff
@@ -1,53 +1,57 @@
 from pathlib import Path
 import os
+import sysconfig
 import typing
 
 from . import common
 
 
 def get_exe_suffix(platform: common.Platform) -> str:
-    if platform == common.Platform.WINDOWS:
+    if platform == common.Platform.WINDOWS_AMD64:
         return '.exe'
 
-    if platform == common.Platform.DARWIN:
-        return ''
-
-    if platform == common.Platform.LINUX:
+    if platform in (common.Platform.DARWIN_X86_64,
+                    common.Platform.LINUX_X86_64,
+                    common.Platform.LINUX_AARCH64):
         return ''
 
     raise ValueError('unsupported platform')
 
 
 def get_lib_suffix(platform: common.Platform) -> str:
-    if platform == common.Platform.WINDOWS:
+    if platform == common.Platform.WINDOWS_AMD64:
         return '.dll'
 
-    if platform == common.Platform.DARWIN:
+    if platform == common.Platform.DARWIN_X86_64:
         return '.dylib'
 
-    if platform == common.Platform.LINUX:
+    if platform in (common.Platform.LINUX_X86_64,
+                    common.Platform.LINUX_AARCH64):
         return '.so'
 
     raise ValueError('unsupported platform')
 
 
 def get_ext_suffix(platform: common.Platform,
                    py_version: common.PyVersion
                    ) -> str:
     _, major, minor = py_version.value
 
-    if platform == common.Platform.LINUX:
-        return f'.cpython-{major}{minor}-x86_64-linux-gnu.so'
+    if platform == common.Platform.WINDOWS_AMD64:
+        return f'.cp{major}{minor}-win_amd64.pyd'
 
-    elif platform == common.Platform.DARWIN:
+    elif platform == common.Platform.DARWIN_X86_64:
         return f'.cpython-{major}{minor}-darwin.so'
 
-    elif platform == common.Platform.WINDOWS:
-        return f'.cp{major}{minor}-win_amd64.pyd'
+    elif platform == common.Platform.LINUX_X86_64:
+        return f'.cpython-{major}{minor}-x86_64-linux-gnu.so'
+
+    elif platform == common.Platform.LINUX_AARCH64:
+        return f'.cpython-{major}{minor}-aarch64-linux-gnu.so'
 
     raise ValueError('unsupported platform')
 
 
 local_exe_suffix: str = get_exe_suffix(common.local_platform)
 target_exe_suffix: str = get_exe_suffix(common.target_platform)
 
@@ -60,36 +64,91 @@
                                         common.target_py_version)
 
 
 def get_cpp(platform: common.Platform) -> str:
     if platform == common.local_platform:
         return os.environ.get('CPP', 'cpp')
 
-    if (common.local_platform, platform) == (common.Platform.LINUX,
-                                             common.Platform.WINDOWS):
+    if (common.local_platform, platform) == (common.Platform.LINUX_X86_64,
+                                             common.Platform.WINDOWS_AMD64):
         return 'x86_64-w64-mingw32-cpp'
 
+    if (common.local_platform, platform) == (common.Platform.LINUX_X86_64,
+                                             common.Platform.LINUX_AARCH64):
+        return 'aarch64-linux-gnu-cpp'
+
     raise ValueError('unsupported platform')
 
 
 def get_cc(platform: common.Platform) -> str:
     if platform == common.local_platform:
         return os.environ.get('CC', 'cc')
 
-    if (common.local_platform, platform) == (common.Platform.LINUX,
-                                             common.Platform.WINDOWS):
+    if (common.local_platform, platform) == (common.Platform.LINUX_X86_64,
+                                             common.Platform.WINDOWS_AMD64):
         return 'x86_64-w64-mingw32-cc'
 
+    if (common.local_platform, platform) == (common.Platform.LINUX_X86_64,
+                                             common.Platform.LINUX_AARCH64):
+        return 'aarch64-linux-gnu-gcc'
+
     raise ValueError('unsupported platform')
 
 
 def get_ld(platform: common.Platform) -> str:
     return get_cc(platform)
 
 
+def get_py_cpp_flags() -> typing.Iterable[str]:
+    _, major, minor = common.target_py_version.value
+
+    if common.target_platform == common.local_platform:
+        if common.target_py_version == common.local_py_version:
+            include_path = sysconfig.get_path('include')
+            if include_path:
+                yield f'-I{include_path}'
+
+        elif common.local_platform == common.Platform.LINUX_X86_64:
+            yield f'-I/usr/include/python{major}.{minor}'
+
+        else:
+            raise ValueError('unsupported version')
+
+    elif (common.local_platform, common.target_platform) == (
+            common.Platform.LINUX_X86_64, common.Platform.WINDOWS_AMD64):
+        yield f'-I/usr/x86_64-w64-mingw32/include/python{major}{minor}'
+
+    elif (common.local_platform, common.target_platform) == (
+            common.Platform.LINUX_X86_64, common.Platform.LINUX_AARCH64):
+        yield f'-I/usr/include/python{major}.{minor}'
+
+    else:
+        raise ValueError('unsupported platform')
+
+
+def get_py_ld_flags() -> typing.Iterable[str]:
+    _, major, minor = common.target_py_version.value
+
+    if common.target_platform == common.local_platform:
+        if common.local_platform == common.Platform.DARWIN_X86_64:
+            stdlib_path = (Path(sysconfig.get_path('stdlib')) /
+                           f'config-{major}.{minor}-darwin')
+            yield f"-L{stdlib_path}"
+
+        elif common.local_platform == common.Platform.WINDOWS_AMD64:
+            data_path = sysconfig.get_path('data')
+            yield f"-L{data_path}"
+
+    if common.target_platform == common.Platform.WINDOWS_AMD64:
+        yield f"-lpython{major}{minor}"
+
+    elif common.target_platform == common.Platform.DARWIN_X86_64:
+        yield f"-lpython{major}.{minor}"
+
+
 class CBuild:
 
     def __init__(self,
                  src_paths: typing.List[Path],
                  build_dir: Path, *,
                  src_dir: Path = Path('.'),
                  platform: common.Platform = common.target_platform,
@@ -118,16 +177,17 @@
                'file_dep': obj_paths,
                'task_dep': self._task_dep,
                'targets': [exe_path]}
 
     def get_task_lib(self, lib_path: Path) -> typing.Dict:
         obj_paths = [self._get_obj_path(src_path)
                      for src_path in self._src_paths]
-        shared_flag = ('-mdll' if self._platform == common.Platform.WINDOWS
-                       else '-shared')
+        shared_flag = (
+            '-mdll' if self._platform == common.Platform.WINDOWS_AMD64
+            else '-shared')
         yield {'name': str(lib_path),
                'actions': [(common.mkdir_p, [lib_path.parent]),
                            [get_ld(self._platform),
                             *(str(obj_path) for obj_path in obj_paths),
                             '-o', str(lib_path), shared_flag,
                             *self._ld_flags]],
                'file_dep': obj_paths,
```

## hat/doit/common.py

```diff
@@ -1,28 +1,30 @@
 from pathlib import Path
 import datetime
 import enum
 import functools
 import itertools
 import multiprocessing
 import os
+import platform
 import shutil
 import subprocess
 import sys
 import typing
 
 import packaging.requirements
 import packaging.tags
 import packaging.version
 
 
 class Platform(enum.Enum):
-    WINDOWS = 'win32'
-    DARWIN = 'darwin'
-    LINUX = 'linux'
+    WINDOWS_AMD64 = ('win32', 'amd64')
+    DARWIN_X86_64 = ('darwin', 'x86_64')
+    LINUX_X86_64 = ('linux', 'x86_64')
+    LINUX_AARCH64 = ('linux', 'aarch64')
 
 
 class PyVersion(enum.Enum):
     CP38 = ('cp', 3, 8)
     CP39 = ('cp', 3, 9)
     CP310 = ('cp', 3, 10)
 
@@ -36,15 +38,15 @@
     APACHE2 = 'Apache-2.0'
     GPL3 = 'GPLv3'
     PROPRIETARY = 'PROPRIETARY'
 
 
 now: datetime.datetime = datetime.datetime.now()
 
-local_platform: Platform = Platform(sys.platform)
+local_platform: Platform = Platform((sys.platform, platform.machine().lower()))
 target_platform: Platform = (Platform[os.environ['TARGET_PLATFORM'].upper()]
                              if 'TARGET_PLATFORM' in os.environ
                              else local_platform)
 
 local_py_version: PyVersion = PyVersion((packaging.tags.interpreter_name(),
                                          sys.version_info.major,
                                          sys.version_info.minor))
```

## hat/doit/py.py

```diff
@@ -109,23 +109,26 @@
     raise ValueError('unsupported license')
 
 
 def _get_wheel_plat_name(platform):
     if not platform:
         return 'any'
 
-    if platform == common.Platform.WINDOWS:
+    if platform == common.Platform.WINDOWS_AMD64:
         return 'win_amd64'
 
-    if platform == common.Platform.DARWIN:
+    if platform == common.Platform.DARWIN_X86_64:
         return 'macosx_10_13_x86_64'
 
-    if platform == common.Platform.LINUX:
+    if platform == common.Platform.LINUX_X86_64:
         return 'manylinux1_x86_64'
 
+    if platform == common.Platform.LINUX_AARCH64:
+        return 'manylinux2014_aarch64'
+
     raise NotImplementedError()
 
 
 _wheel_setup_py = r"""
 from setuptools import setup
 
 name = {name}
```

## Comparing `hat_doit-0.8.3.dist-info/LICENSE` & `hat_doit-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hat_doit-0.8.3.dist-info/METADATA` & `hat_doit-0.9.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hat-doit
-Version: 0.8.3
+Version: 0.9.0
 Summary: Hat build utility functions
 Home-page: https://github.com/hat-open/hat-doit
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

## Comparing `hat_doit-0.8.3.dist-info/RECORD` & `hat_doit-0.9.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 hat/doit/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-hat/doit/c.py,sha256=7OfbAAtQRLtCl-ckU0z8eKXS51j3OnYYUap1puRCFa4,6434
-hat/doit/common.py,sha256=cqW_jkzZjcvlSc0cXsYhRjHvIM9ecBJunE1K7iHQx6k,4211
+hat/doit/c.py,sha256=ocCp9qvSTqgggA31f0vG-uRB0ZqbRFJd31bQ3VEKWyg,8896
+hat/doit/common.py,sha256=VeQQzEwnBoEJ4BQOzpqJmQdMgOddc-akJMvbHcPrvzg,4353
 hat/doit/docs.py,sha256=2jeb60EfB8iEFonRwT4tXaT2RAAq_bOzY0VlVN9Kp3Y,2016
 hat/doit/js.py,sha256=rpDkAEpYP6RRU4KVHz7Cz5XW1fIoAPufEXDxrKuYwzI,1941
-hat/doit/py.py,sha256=0T7Jv__cQ_cBMAZi-7vahSOo-fGDg2nTnqyPUaK3aIU,5484
+hat/doit/py.py,sha256=GKcwfZ8eMIUysXpHsn0dxN2-tF8lpOByITG6S-4oswo,5594
 hat/doit/sphinx/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hat/doit/sphinx/static/hat.css,sha256=IZm370sNnNsYVtoEAA20Tg3TVcEHK7bjqmvIKHO7mKM,359
-hat_doit-0.8.3.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-hat_doit-0.8.3.dist-info/METADATA,sha256=nZlFMB7rUn-1DjyLoH_x2BKs2TMtT3_g9Bj8BMMRwXY,1953
-hat_doit-0.8.3.dist-info/WHEEL,sha256=J6o_EVcUhZ99gpCSeF2DGIW9mETC6p0M-27vXCgDo6E,132
-hat_doit-0.8.3.dist-info/top_level.txt,sha256=3RuRoRsaXQZNKwr3T2RE9XepBRTk4YpnXUbMiH5nes8,4
-hat_doit-0.8.3.dist-info/RECORD,,
+hat_doit-0.9.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+hat_doit-0.9.0.dist-info/METADATA,sha256=7ee3CG4QwvzsMU2X-0dfJJ1h8Rq7ggzOAq1kPO-7-K4,1953
+hat_doit-0.9.0.dist-info/WHEEL,sha256=J6o_EVcUhZ99gpCSeF2DGIW9mETC6p0M-27vXCgDo6E,132
+hat_doit-0.9.0.dist-info/top_level.txt,sha256=3RuRoRsaXQZNKwr3T2RE9XepBRTk4YpnXUbMiH5nes8,4
+hat_doit-0.9.0.dist-info/RECORD,,
```

