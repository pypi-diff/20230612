# Comparing `tmp/ofrak_patch_maker-4.0.0.tar.gz` & `tmp/ofrak_patch_maker-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofrak_patch_maker-4.0.0.tar", last modified: Wed Apr 26 18:59:52 2023, max compression
+gzip compressed data, was "ofrak_patch_maker-4.0.1.tar", last modified: Mon Jun 12 18:29:16 2023, max compression
```

## Comparing `ofrak_patch_maker-4.0.0.tar` & `ofrak_patch_maker-4.0.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-04-26 18:59:52.767519 ofrak_patch_maker-4.0.0/
--rw-r--r--   0 edward     (501) staff       (20)    14321 2022-08-24 21:38:35.000000 ofrak_patch_maker-4.0.0/LICENSE
--rw-r--r--   0 edward     (501) staff       (20)       67 2023-03-20 14:52:33.000000 ofrak_patch_maker-4.0.0/MANIFEST.in
--rw-r--r--   0 edward     (501) staff       (20)     4276 2023-04-26 18:59:52.766912 ofrak_patch_maker-4.0.0/PKG-INFO
--rw-r--r--   0 edward     (501) staff       (20)     3342 2023-02-02 23:02:32.000000 ofrak_patch_maker-4.0.0/README.md
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-04-26 18:59:52.748170 ofrak_patch_maker-4.0.0/ofrak_patch_maker/
--rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/__init__.py
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-04-26 18:59:52.752535 ofrak_patch_maker-4.0.0/ofrak_patch_maker/binary_parser/
--rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/binary_parser/__init__.py
--rw-r--r--   0 edward     (501) staff       (20)      770 2023-03-30 19:29:16.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/binary_parser/abstract.py
--rw-r--r--   0 edward     (501) staff       (20)     4610 2023-03-30 19:29:16.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/binary_parser/gnu.py
--rw-r--r--   0 edward     (501) staff       (20)     6099 2023-03-30 19:29:16.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/binary_parser/llvm.py
--rw-r--r--   0 edward     (501) staff       (20)     3623 2023-03-30 19:29:16.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/model.py
--rw-r--r--   0 edward     (501) staff       (20)    20807 2023-03-30 19:29:16.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/patch_maker.py
--rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/py.typed
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-04-26 18:59:52.765783 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/
--rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/__init__.py
--rw-r--r--   0 edward     (501) staff       (20)    18006 2023-03-30 19:29:24.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/abstract.py
--rw-r--r--   0 edward     (501) staff       (20)    13102 2023-03-30 19:29:24.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu.py
--rw-r--r--   0 edward     (501) staff       (20)     3018 2023-03-30 19:29:24.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_aarch64.py
--rw-r--r--   0 edward     (501) staff       (20)     1830 2023-01-11 21:57:41.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_arm.py
--rw-r--r--   0 edward     (501) staff       (20)     2492 2023-02-02 23:02:32.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_avr.py
--rw-r--r--   0 edward     (501) staff       (20)     2249 2023-01-11 21:57:41.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_m68k.py
--rw-r--r--   0 edward     (501) staff       (20)     2919 2023-03-21 23:02:49.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_ppc.py
--rw-r--r--   0 edward     (501) staff       (20)     5999 2023-03-17 18:25:04.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_vbcc_m68k.py
--rw-r--r--   0 edward     (501) staff       (20)     2796 2023-01-11 21:57:41.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_x64.py
--rw-r--r--   0 edward     (501) staff       (20)    12252 2023-03-30 19:29:16.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/llvm_12.py
--rw-r--r--   0 edward     (501) staff       (20)     4047 2023-03-30 19:29:16.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/model.py
--rw-r--r--   0 edward     (501) staff       (20)     5258 2023-01-11 21:57:41.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/utils.py
--rw-r--r--   0 edward     (501) staff       (20)     2327 2023-03-21 23:02:49.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain.conf
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-04-26 18:59:52.750628 ofrak_patch_maker-4.0.0/ofrak_patch_maker.egg-info/
--rw-r--r--   0 edward     (501) staff       (20)     4276 2023-04-26 18:59:52.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker.egg-info/PKG-INFO
--rw-r--r--   0 edward     (501) staff       (20)     1088 2023-04-26 18:59:52.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker.egg-info/SOURCES.txt
--rw-r--r--   0 edward     (501) staff       (20)        1 2023-04-26 18:59:52.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker.egg-info/dependency_links.txt
--rw-r--r--   0 edward     (501) staff       (20)      107 2023-04-26 18:59:52.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker.egg-info/requires.txt
--rw-r--r--   0 edward     (501) staff       (20)       18 2023-04-26 18:59:52.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker.egg-info/top_level.txt
--rw-r--r--   0 edward     (501) staff       (20)       34 2023-02-16 21:44:18.000000 ofrak_patch_maker-4.0.0/requirements.txt
--rw-r--r--   0 edward     (501) staff       (20)       38 2023-04-26 18:59:52.767694 ofrak_patch_maker-4.0.0/setup.cfg
--rw-r--r--   0 edward     (501) staff       (20)     2387 2023-04-26 17:26:19.000000 ofrak_patch_maker-4.0.0/setup.py
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-06-12 18:29:16.337569 ofrak_patch_maker-4.0.1/
+-rw-r--r--   0 edward     (501) staff       (20)    14321 2022-08-24 21:38:35.000000 ofrak_patch_maker-4.0.1/LICENSE
+-rw-r--r--   0 edward     (501) staff       (20)       67 2023-04-27 21:00:41.000000 ofrak_patch_maker-4.0.1/MANIFEST.in
+-rw-r--r--   0 edward     (501) staff       (20)     4276 2023-06-12 18:29:16.337238 ofrak_patch_maker-4.0.1/PKG-INFO
+-rw-r--r--   0 edward     (501) staff       (20)     3342 2023-02-02 23:02:32.000000 ofrak_patch_maker-4.0.1/README.md
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-06-12 18:29:16.320461 ofrak_patch_maker-4.0.1/ofrak_patch_maker/
+-rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/__init__.py
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-06-12 18:29:16.326156 ofrak_patch_maker-4.0.1/ofrak_patch_maker/binary_parser/
+-rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/binary_parser/__init__.py
+-rw-r--r--   0 edward     (501) staff       (20)      770 2023-04-27 21:00:41.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/binary_parser/abstract.py
+-rw-r--r--   0 edward     (501) staff       (20)     4610 2023-05-26 22:11:41.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/binary_parser/gnu.py
+-rw-r--r--   0 edward     (501) staff       (20)     6099 2023-05-26 22:11:41.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/binary_parser/llvm.py
+-rw-r--r--   0 edward     (501) staff       (20)     3623 2023-05-26 22:11:41.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/model.py
+-rw-r--r--   0 edward     (501) staff       (20)    20807 2023-06-05 18:52:20.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/patch_maker.py
+-rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/py.typed
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-06-12 18:29:16.336661 ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/
+-rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/__init__.py
+-rw-r--r--   0 edward     (501) staff       (20)    18171 2023-06-12 14:38:39.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/abstract.py
+-rw-r--r--   0 edward     (501) staff       (20)    13102 2023-05-26 22:11:41.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/gnu.py
+-rw-r--r--   0 edward     (501) staff       (20)     3018 2023-05-26 22:11:41.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/gnu_aarch64.py
+-rw-r--r--   0 edward     (501) staff       (20)     1830 2023-01-11 21:57:41.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/gnu_arm.py
+-rw-r--r--   0 edward     (501) staff       (20)     2492 2023-02-02 23:02:32.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/gnu_avr.py
+-rw-r--r--   0 edward     (501) staff       (20)     2249 2023-01-11 21:57:41.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/gnu_m68k.py
+-rw-r--r--   0 edward     (501) staff       (20)     2919 2023-03-21 23:02:49.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/gnu_ppc.py
+-rw-r--r--   0 edward     (501) staff       (20)     5999 2023-03-17 18:25:04.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/gnu_vbcc_m68k.py
+-rw-r--r--   0 edward     (501) staff       (20)     2796 2023-01-11 21:57:41.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/gnu_x64.py
+-rw-r--r--   0 edward     (501) staff       (20)    12252 2023-05-26 22:11:41.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/llvm_12.py
+-rw-r--r--   0 edward     (501) staff       (20)     4037 2023-06-12 14:38:39.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/model.py
+-rw-r--r--   0 edward     (501) staff       (20)     5418 2023-06-12 14:38:39.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/utils.py
+-rw-r--r--   0 edward     (501) staff       (20)     2327 2023-05-26 22:11:34.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain.conf
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-06-12 18:29:16.323815 ofrak_patch_maker-4.0.1/ofrak_patch_maker.egg-info/
+-rw-r--r--   0 edward     (501) staff       (20)    14321 2022-08-24 21:38:35.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker.egg-info/LICENSE
+-rw-r--r--   0 edward     (501) staff       (20)     4276 2023-06-12 18:29:16.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker.egg-info/PKG-INFO
+-rw-r--r--   0 edward     (501) staff       (20)     1123 2023-06-12 18:29:16.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker.egg-info/SOURCES.txt
+-rw-r--r--   0 edward     (501) staff       (20)        1 2023-06-12 18:29:16.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker.egg-info/dependency_links.txt
+-rw-r--r--   0 edward     (501) staff       (20)      107 2023-06-12 18:29:16.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker.egg-info/requires.txt
+-rw-r--r--   0 edward     (501) staff       (20)       18 2023-06-12 18:29:16.000000 ofrak_patch_maker-4.0.1/ofrak_patch_maker.egg-info/top_level.txt
+-rw-r--r--   0 edward     (501) staff       (20)       34 2023-02-16 21:44:18.000000 ofrak_patch_maker-4.0.1/requirements.txt
+-rw-r--r--   0 edward     (501) staff       (20)       38 2023-06-12 18:29:16.337663 ofrak_patch_maker-4.0.1/setup.cfg
+-rw-r--r--   0 edward     (501) staff       (20)     2387 2023-06-12 18:26:08.000000 ofrak_patch_maker-4.0.1/setup.py
```

### Comparing `ofrak_patch_maker-4.0.0/LICENSE` & `ofrak_patch_maker-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-4.0.0/PKG-INFO` & `ofrak_patch_maker-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofrak_patch_maker
-Version: 4.0.0
+Version: 4.0.1
 Summary: PatchMaker tool for applying source-code patches to binaries
 Home-page: https://ofrak.com/
 Download-URL: https://github.com/redballoonsecurity/ofrak
 Author: Red Balloon Security
 Author-email: ofrak@redballoonsecurity.com
 License: Proprietary
 Project-URL: Documentation, https://ofrak.com/docs/
```

### Comparing `ofrak_patch_maker-4.0.0/README.md` & `ofrak_patch_maker-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/binary_parser/abstract.py` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/binary_parser/abstract.py`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/binary_parser/gnu.py` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/binary_parser/gnu.py`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/binary_parser/llvm.py` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/binary_parser/llvm.py`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/model.py` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/model.py`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/patch_maker.py` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/patch_maker.py`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/abstract.py` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     for use with [PatchMaker][ofrak_patch_maker.patch_maker.PatchMaker].
 """
 import logging
 import os
 import subprocess
 from abc import ABC, abstractmethod
 from os.path import join, split
-from typing import Dict, Iterable, List, Optional, Tuple, Mapping
+from typing import Dict, Iterable, List, Optional, Tuple, Mapping, Type
 
 from ofrak_type import ArchInfo
 from ofrak_patch_maker.binary_parser.abstract import AbstractBinaryFileParser
 from ofrak_patch_maker.toolchain.model import Segment, ToolchainConfig
 from ofrak_patch_maker.toolchain.utils import get_repository_config
 from ofrak_type.architecture import InstructionSet
 from ofrak_type.bit_width import BitWidth
@@ -26,14 +26,15 @@
     "*\n"
     "*/\n\n"
 )
 
 
 class Toolchain(ABC):
     binary_file_parsers: List[AbstractBinaryFileParser] = []
+    toolchain_implementations: List[Type["Toolchain"]] = []
 
     def __init__(
         self,
         processor: ArchInfo,
         toolchain_config: ToolchainConfig,
         logger: logging.Logger = logging.getLogger(),
     ):
@@ -95,14 +96,17 @@
             ".eh_frame",
             ".altinstructions",
         ]
 
         self._assembler_target = self._get_assembler_target(processor)
         self._compiler_target = self._get_compiler_target(processor)
 
+    def __init_subclass__(cls, **kwargs):
+        Toolchain.toolchain_implementations.append(cls)
+
     @property
     @abstractmethod
     def name(self) -> str:
         """
         :return str: name property that matches the value used in `toolchain.conf` to access paths
         """
         raise NotImplementedError()
```

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu.py` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/gnu.py`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_aarch64.py` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/gnu_aarch64.py`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_arm.py` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/gnu_arm.py`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_avr.py` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/gnu_avr.py`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_m68k.py` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/gnu_m68k.py`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_ppc.py` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/gnu_ppc.py`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_vbcc_m68k.py` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/gnu_vbcc_m68k.py`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_x64.py` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/gnu_x64.py`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/llvm_12.py` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/llvm_12.py`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/model.py` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,8 +117,8 @@
     debug_info: bool = True
     check_overlap: bool = True
     userspace_dynamic_linker: Optional[str] = None
     isysroot: Optional[str] = None
     c_standard: Optional[CStandardVersion] = CStandardVersion.C99
     separate_data_sections: bool = False
     include_subsections: bool = False
-    hard_float: Optional[bool] = False
+    hard_float: bool = False
```

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/utils.py` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import configparser
 import math
 import os
 import platform
 from multiprocessing import Pool, cpu_count
 from typing import Optional, Dict, Mapping, Tuple
 
-import magic
-
 from ofrak_patch_maker.toolchain.model import BinFileType, Segment
 from ofrak_type.error import NotFoundError
 from ofrak_type.memory_permissions import MemoryPermissions
 
 
 def get_file_format(path):
+    try:
+        import magic
+    except ImportError:
+        # ImportError is likely raise because libmagic cannot be found on the system. See error message.
+        raise
+
     result = magic.from_file(path).split(" ")[0].lower()
     try:
         return BinFileType(result)
     except:
         ValueError("Invalid BinFileType!!!")
```

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain.conf` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker/toolchain.conf`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker.egg-info/PKG-INFO` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofrak-patch-maker
-Version: 4.0.0
+Version: 4.0.1
 Summary: PatchMaker tool for applying source-code patches to binaries
 Home-page: https://ofrak.com/
 Download-URL: https://github.com/redballoonsecurity/ofrak
 Author: Red Balloon Security
 Author-email: ofrak@redballoonsecurity.com
 License: Proprietary
 Project-URL: Documentation, https://ofrak.com/docs/
```

### Comparing `ofrak_patch_maker-4.0.0/ofrak_patch_maker.egg-info/SOURCES.txt` & `ofrak_patch_maker-4.0.1/ofrak_patch_maker.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 requirements.txt
 setup.py
 ofrak_patch_maker/__init__.py
 ofrak_patch_maker/model.py
 ofrak_patch_maker/patch_maker.py
 ofrak_patch_maker/py.typed
 ofrak_patch_maker/toolchain.conf
+ofrak_patch_maker.egg-info/LICENSE
 ofrak_patch_maker.egg-info/PKG-INFO
 ofrak_patch_maker.egg-info/SOURCES.txt
 ofrak_patch_maker.egg-info/dependency_links.txt
 ofrak_patch_maker.egg-info/requires.txt
 ofrak_patch_maker.egg-info/top_level.txt
 ofrak_patch_maker/binary_parser/__init__.py
 ofrak_patch_maker/binary_parser/abstract.py
```

### Comparing `ofrak_patch_maker-4.0.0/setup.py` & `ofrak_patch_maker-4.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             str(requirement)
             for requirement in pkg_resources.parse_requirements(requirements_handle)
         ]
 
 
 setuptools.setup(
     name="ofrak_patch_maker",
-    version="4.0.0",
+    version="4.0.1",
     description="PatchMaker tool for applying source-code patches to binaries",
     packages=setuptools.find_packages(exclude=("ofrak_patch_maker_test",)),
     package_data={"ofrak_patch_maker": ["py.typed"]},
     install_requires=[
         "ofrak_type>=2.2.0rc0,==2.*",
     ]
     + read_requirements("requirements.txt"),
```

