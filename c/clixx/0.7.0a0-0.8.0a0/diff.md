# Comparing `tmp/clixx-0.7.0a0.tar.gz` & `tmp/clixx-0.8.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clixx-0.7.0a0.tar", last modified: Sun May 14 07:44:18 2023, max compression
+gzip compressed data, was "clixx-0.8.0a0.tar", last modified: Mon Jun 12 03:12:09 2023, max compression
```

## Comparing `clixx-0.7.0a0.tar` & `clixx-0.8.0a0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 07:44:18.908827 clixx-0.7.0a0/
--rw-rw-rw-   0        0        0      258 2022-08-20 12:06:12.000000 clixx-0.7.0a0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1087 2023-02-14 02:01:01.000000 clixx-0.7.0a0/LICENSE
--rw-rw-rw-   0        0        0      151 2023-05-01 02:49:08.000000 clixx-0.7.0a0/MANIFEST.in
--rw-rw-rw-   0        0        0     2202 2023-05-14 07:44:18.909827 clixx-0.7.0a0/PKG-INFO
--rw-rw-rw-   0        0        0      920 2023-05-14 07:39:38.000000 clixx-0.7.0a0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 07:44:18.876828 clixx-0.7.0a0/docs/
--rw-rw-rw-   0        0        0      638 2022-10-15 01:44:45.000000 clixx-0.7.0a0/docs/Makefile
--rwxrwxrwx   0        0        0      804 2022-10-15 01:44:45.000000 clixx-0.7.0a0/docs/make.bat
--rw-rw-rw-   0        0        0      997 2023-05-01 02:56:19.000000 clixx-0.7.0a0/docs/release.py
--rw-rw-rw-   0        0        0       78 2023-04-28 02:42:53.000000 clixx-0.7.0a0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 07:44:18.879829 clixx-0.7.0a0/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-14 07:44:18.887828 clixx-0.7.0a0/docs/source/api/
--rw-rw-rw-   0        0        0      638 2022-11-21 08:42:57.000000 clixx-0.7.0a0/docs/source/api/arguments.rst
--rw-rw-rw-   0        0        0     1189 2022-11-24 08:57:53.000000 clixx-0.7.0a0/docs/source/api/exceptions.rst
--rw-rw-rw-   0        0        0      657 2022-11-18 02:37:53.000000 clixx-0.7.0a0/docs/source/api/groups.rst
--rw-rw-rw-   0        0        0      134 2022-12-04 02:13:38.000000 clixx-0.7.0a0/docs/source/api/index.rst
--rw-rw-rw-   0        0        0      573 2022-12-04 02:30:04.000000 clixx-0.7.0a0/docs/source/api/printers.rst
--rw-rw-rw-   0        0        0     1058 2022-11-23 12:44:53.000000 clixx-0.7.0a0/docs/source/api/types.rst
--rw-rw-rw-   0        0        0     2903 2023-02-15 06:42:24.000000 clixx-0.7.0a0/docs/source/conf.py
--rw-rw-rw-   0        0        0      810 2022-10-30 07:36:12.000000 clixx-0.7.0a0/docs/source/index.rst
--rw-rw-rw-   0        0        0     1157 2023-05-01 02:54:06.000000 clixx-0.7.0a0/pyproject.toml
--rw-rw-rw-   0        0        0     1528 2023-05-14 07:44:18.910828 clixx-0.7.0a0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 07:44:18.862829 clixx-0.7.0a0/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 07:44:18.901829 clixx-0.7.0a0/src/clixx/
--rw-rw-rw-   0        0        0     1814 2023-05-14 07:42:54.000000 clixx-0.7.0a0/src/clixx/__init__.py
--rw-rw-rw-   0        0        0     6430 2023-01-07 09:23:51.000000 clixx-0.7.0a0/src/clixx/_rich.py
--rw-rw-rw-   0        0        0    19776 2023-03-14 14:34:27.000000 clixx-0.7.0a0/src/clixx/arguments.py
--rw-rw-rw-   0        0        0    12117 2023-03-15 03:02:39.000000 clixx-0.7.0a0/src/clixx/commands.py
--rw-rw-rw-   0        0        0      242 2023-03-14 14:01:46.000000 clixx-0.7.0a0/src/clixx/constants.py
--rw-rw-rw-   0        0        0    13810 2023-01-09 08:49:13.000000 clixx-0.7.0a0/src/clixx/decorators.py
--rw-rw-rw-   0        0        0     1620 2022-11-13 12:34:28.000000 clixx-0.7.0a0/src/clixx/exceptions.py
--rw-rw-rw-   0        0        0     5387 2023-03-17 08:08:59.000000 clixx-0.7.0a0/src/clixx/groups.py
--rw-rw-rw-   0        0        0    12440 2023-03-15 02:58:49.000000 clixx-0.7.0a0/src/clixx/parsers.py
--rw-rw-rw-   0        0        0     6902 2023-03-15 03:01:45.000000 clixx-0.7.0a0/src/clixx/printers.py
--rw-rw-rw-   0        0        0        0 2022-08-20 08:21:13.000000 clixx-0.7.0a0/src/clixx/py.typed
--rw-rw-rw-   0        0        0    19894 2023-03-14 15:41:00.000000 clixx-0.7.0a0/src/clixx/types.py
-drwxrwxrwx   0        0        0        0 2023-05-14 07:44:18.907827 clixx-0.7.0a0/src/clixx.egg-info/
--rw-rw-rw-   0        0        0     2202 2023-05-14 07:44:18.000000 clixx-0.7.0a0/src/clixx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      794 2023-05-14 07:44:18.000000 clixx-0.7.0a0/src/clixx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 07:44:18.000000 clixx-0.7.0a0/src/clixx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2023-05-14 07:44:18.000000 clixx-0.7.0a0/src/clixx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-14 07:44:18.000000 clixx-0.7.0a0/src/clixx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-10-09 02:10:23.000000 clixx-0.7.0a0/src/clixx.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-12 03:12:09.115541 clixx-0.8.0a0/
+-rw-rw-rw-   0        0        0      258 2022-08-20 12:06:12.000000 clixx-0.8.0a0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1087 2023-02-14 02:01:01.000000 clixx-0.8.0a0/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-06-01 05:13:09.000000 clixx-0.8.0a0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2202 2023-06-12 03:12:09.115541 clixx-0.8.0a0/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2023-05-14 07:39:38.000000 clixx-0.8.0a0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 03:12:09.078540 clixx-0.8.0a0/docs/
+-rw-rw-rw-   0        0        0      638 2022-10-15 01:44:45.000000 clixx-0.8.0a0/docs/Makefile
+-rwxrwxrwx   0        0        0      804 2022-10-15 01:44:45.000000 clixx-0.8.0a0/docs/make.bat
+-rw-rw-rw-   0        0        0     1476 2023-06-08 11:17:18.000000 clixx-0.8.0a0/docs/release.py
+-rw-rw-rw-   0        0        0       69 2023-06-01 07:15:09.000000 clixx-0.8.0a0/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 03:12:09.080542 clixx-0.8.0a0/docs/source/
+drwxrwxrwx   0        0        0        0 2023-06-12 03:12:09.089541 clixx-0.8.0a0/docs/source/api/
+-rw-rw-rw-   0        0        0      457 2023-06-01 09:14:52.000000 clixx-0.8.0a0/docs/source/api/arguments.rst
+-rw-rw-rw-   0        0        0      643 2023-06-02 10:51:04.000000 clixx-0.8.0a0/docs/source/api/exceptions.rst
+-rw-rw-rw-   0        0        0      462 2023-06-02 10:52:03.000000 clixx-0.8.0a0/docs/source/api/groups.rst
+-rw-rw-rw-   0        0        0      134 2023-06-01 07:18:28.000000 clixx-0.8.0a0/docs/source/api/index.rst
+-rw-rw-rw-   0        0        0      378 2023-06-02 10:52:28.000000 clixx-0.8.0a0/docs/source/api/printers.rst
+-rw-rw-rw-   0        0        0      512 2023-06-01 09:11:06.000000 clixx-0.8.0a0/docs/source/api/types.rst
+-rw-rw-rw-   0        0        0     2707 2023-06-03 12:58:19.000000 clixx-0.8.0a0/docs/source/conf.py
+-rw-rw-rw-   0        0        0     1274 2023-06-12 02:48:17.000000 clixx-0.8.0a0/pyproject.toml
+-rw-rw-rw-   0        0        0     1553 2023-06-12 03:12:09.116540 clixx-0.8.0a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 03:12:09.063539 clixx-0.8.0a0/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 03:12:09.106538 clixx-0.8.0a0/src/clixx/
+-rw-rw-rw-   0        0        0     2025 2023-06-12 03:07:22.000000 clixx-0.8.0a0/src/clixx/__init__.py
+-rw-rw-rw-   0        0        0     6430 2023-01-07 09:23:51.000000 clixx-0.8.0a0/src/clixx/_rich.py
+-rw-rw-rw-   0        0        0    20121 2023-06-12 02:57:15.000000 clixx-0.8.0a0/src/clixx/arguments.py
+-rw-rw-rw-   0        0        0    11305 2023-05-21 11:40:40.000000 clixx-0.8.0a0/src/clixx/commands.py
+-rw-rw-rw-   0        0        0      412 2023-05-15 03:19:16.000000 clixx-0.8.0a0/src/clixx/constants.py
+-rw-rw-rw-   0        0        0    13951 2023-05-17 12:15:48.000000 clixx-0.8.0a0/src/clixx/decorators.py
+-rw-rw-rw-   0        0        0     1620 2022-11-13 12:34:28.000000 clixx-0.8.0a0/src/clixx/exceptions.py
+-rw-rw-rw-   0        0        0     5325 2023-05-15 08:40:19.000000 clixx-0.8.0a0/src/clixx/groups.py
+-rw-rw-rw-   0        0        0    12505 2023-06-01 09:37:06.000000 clixx-0.8.0a0/src/clixx/parsers.py
+-rw-rw-rw-   0        0        0     6898 2023-05-14 13:16:46.000000 clixx-0.8.0a0/src/clixx/printers.py
+-rw-rw-rw-   0        0        0        0 2022-08-20 08:21:13.000000 clixx-0.8.0a0/src/clixx/py.typed
+-rw-rw-rw-   0        0        0    21064 2023-06-12 03:00:46.000000 clixx-0.8.0a0/src/clixx/types.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:12:09.114540 clixx-0.8.0a0/src/clixx.egg-info/
+-rw-rw-rw-   0        0        0     2202 2023-06-12 03:12:09.000000 clixx-0.8.0a0/src/clixx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      772 2023-06-12 03:12:09.000000 clixx-0.8.0a0/src/clixx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 03:12:09.000000 clixx-0.8.0a0/src/clixx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2023-06-12 03:12:09.000000 clixx-0.8.0a0/src/clixx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 03:12:09.000000 clixx-0.8.0a0/src/clixx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-10-09 02:10:23.000000 clixx-0.8.0a0/src/clixx.egg-info/zip-safe
```

### Comparing `clixx-0.7.0a0/LICENSE` & `clixx-0.8.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `clixx-0.7.0a0/PKG-INFO` & `clixx-0.8.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clixx
-Version: 0.7.0a0
+Version: 0.8.0a0
 Summary: Command-line interface parser & framework for Python
 Home-page: https://github.com/xymy/clixx
 Author: xymy
 Author-email: thyfan@163.com
 Maintainer: xymy
 Maintainer-email: thyfan@163.com
 License: MIT
```

### Comparing `clixx-0.7.0a0/README.md` & `clixx-0.8.0a0/README.md`

 * *Files identical despite different names*

### Comparing `clixx-0.7.0a0/docs/Makefile` & `clixx-0.8.0a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clixx-0.7.0a0/docs/make.bat` & `clixx-0.8.0a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clixx-0.7.0a0/pyproject.toml` & `clixx-0.8.0a0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -21,23 +21,27 @@
     "W",      # pycodestyle warning
     "D3",     # pydocstyle
     "YTT",    # flake8-2020
     "B",      # flake8-bugbear
     "C4",     # flake8-comprehensions
     "ISC",    # flake8-implicit-str-concat
     "SIM",    # flake8-simplify
+    "INT",    # flake8-gettext
     "RUF100",
 ]
 ignore = [
     # Module level import not at top of file
     "E402",
     # Line too long ({width} > {limit} characters)
     "E501",
 ]
 
+[tool.ruff.flake8-comprehensions]
+allow-dict-calls-with-keyword-arguments = true
+
 [tool.mypy]
 ignore_missing_imports = true
 disallow_untyped_defs = true
 check_untyped_defs = true
 no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
```

### Comparing `clixx-0.7.0a0/setup.cfg` & `clixx-0.8.0a0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -73,24 +73,26 @@
 00000480: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
 00000490: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
 000004a0: 655f 6461 7461 203d 2054 7275 650d 0a7a  e_data = True..z
 000004b0: 6970 5f73 6166 6520 3d20 5472 7565 0d0a  ip_safe = True..
 000004c0: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
 000004d0: 3d20 3e3d 332e 380d 0a69 6e73 7461 6c6c  = >=3.8..install
 000004e0: 5f72 6571 7569 7265 7320 3d20 0d0a 0972  _requires = ...r
-000004f0: 6963 683e 3d31 332e 300d 0a0d 0a5b 6f70  ich>=13.0....[op
-00000500: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
-00000510: 7569 7265 5d0d 0a6c 696e 7420 3d20 0d0a  uire]..lint = ..
-00000520: 0962 6c61 636b 3e3d 3233 2e33 0d0a 0969  .black>=23.3...i
-00000530: 736f 7274 3e3d 352e 3132 0d0a 0972 7566  sort>=5.12...ruf
-00000540: 663e 3d30 2e30 2e32 3630 0d0a 096d 7970  f>=0.0.260...myp
-00000550: 793e 3d31 2e32 0d0a 7465 7374 203d 200d  y>=1.2..test = .
-00000560: 0a09 636f 7665 7261 6765 3e3d 372e 320d  ..coverage>=7.2.
-00000570: 0a09 6879 706f 7468 6573 6973 3e3d 362e  ..hypothesis>=6.
-00000580: 3730 0d0a 0970 7974 6573 743e 3d37 2e32  70...pytest>=7.2
-00000590: 0d0a 0970 7974 6573 742d 636f 763e 3d34  ...pytest-cov>=4
-000005a0: 2e30 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .0....[options.p
-000005b0: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
-000005c0: 6865 7265 203d 2073 7263 0d0a 0d0a 5b65  here = src....[e
-000005d0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-000005e0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-000005f0: 203d 2030 0d0a 0d0a                       = 0....
+000004f0: 6963 683e 3d31 332e 300d 0a09 7479 7069  ich>=13.0...typi
+00000500: 6e67 2d65 7874 656e 7369 6f6e 733e 3d34  ng-extensions>=4
+00000510: 2e34 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .4....[options.p
+00000520: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
+00000530: 6865 7265 203d 2073 7263 0d0a 0d0a 5b6f  here = src....[o
+00000540: 7074 696f 6e73 2e65 7874 7261 735f 7265  ptions.extras_re
+00000550: 7175 6972 655d 0d0a 6c69 6e74 203d 200d  quire]..lint = .
+00000560: 0a09 626c 6163 6b3e 3d32 332e 330d 0a09  ..black>=23.3...
+00000570: 6973 6f72 743e 3d35 2e31 320d 0a09 7275  isort>=5.12...ru
+00000580: 6666 3e3d 302e 302e 3237 300d 0a09 6d79  ff>=0.0.270...my
+00000590: 7079 3e3d 312e 330d 0a74 6573 7420 3d20  py>=1.3..test = 
+000005a0: 0d0a 0963 6f76 6572 6167 653e 3d37 2e32  ...coverage>=7.2
+000005b0: 0d0a 0968 7970 6f74 6865 7369 733e 3d36  ...hypothesis>=6
+000005c0: 2e37 300d 0a09 7079 7465 7374 3e3d 372e  .70...pytest>=7.
+000005d0: 330d 0a09 7079 7465 7374 2d63 6f76 3e3d  3...pytest-cov>=
+000005e0: 342e 310d 0a0d 0a5b 6567 675f 696e 666f  4.1....[egg_info
+000005f0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000600: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000610: 0a                                       .
```

### Comparing `clixx-0.7.0a0/src/clixx/__init__.py` & `clixx-0.8.0a0/src/clixx/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,20 @@
-from .arguments import Argument, CountOption, FlagOption, HelpOption, Option, SignalOption, VersionOption
+from .arguments import (
+    AppendOption,
+    Argument,
+    CountOption,
+    FlagOption,
+    HelpOption,
+    Option,
+    SignalOption,
+    VersionOption,
+    is_long_option,
+    is_separator,
+    is_short_option,
+)
 from .commands import Command, SuperCommand
 from .decorators import (
     append_option,
     argument,
     argument_group,
     command,
     count_option,
@@ -34,18 +46,22 @@
 )
 
 __all__ = [
     # arguments
     "Argument",
     "Option",
     "FlagOption",
+    "AppendOption",
     "CountOption",
     "SignalOption",
     "HelpOption",
     "VersionOption",
+    "is_separator",
+    "is_long_option",
+    "is_short_option",
     # commands
     "Command",
     "SuperCommand",
     # decorators
     "argument",
     "option",
     "flag_option",
@@ -85,10 +101,10 @@
     "Path",
     "DirPath",
     "FilePath",
     "resolve_type",
 ]
 
 __title__ = "clixx"
-__version__ = "0.7.0a"
+__version__ = "0.8.0a"
 __author__ = "xymy"
 __email__ = "thyfan@163.com"
```

### Comparing `clixx-0.7.0a0/src/clixx/_rich.py` & `clixx-0.8.0a0/src/clixx/_rich.py`

 * *Files identical despite different names*

### Comparing `clixx-0.7.0a0/src/clixx/arguments.py` & `clixx-0.8.0a0/src/clixx/arguments.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from __future__ import annotations
 
 from keyword import iskeyword
-from typing import Any, Final, Sequence, cast
+from typing import Any, Sequence, cast
 
-from .constants import LONG_PREFIX, LONG_PREFIX_LEN, SHORT_PREFIX, SHORT_PREFIX_LEN
+from .constants import LONG_PREFIX, LONG_PREFIX_LEN, RESERVED_CHARACTERS, SEPARATOR, SHORT_PREFIX, SHORT_PREFIX_LEN
 from .exceptions import DefinitionError, HelpSignal, TypeConversionError, VersionSignal
 from .types import Int, Str, Type, resolve_type
 
-# The reserved characters for arguments and options.
-_RESERVED: Final = frozenset("\"'<>")
-
 
 def _check_dest(dest: str) -> str:
     dest = dest.replace("-", "_")
     if not dest.isidentifier():
         raise DefinitionError(f"{dest!r} is not a valid identifier.")
     if iskeyword(dest):
         raise DefinitionError(f"{dest!r} is a keyword.")
@@ -24,15 +21,15 @@
     return metavar.replace("-", "_").upper()
 
 
 def _parse_decl(decl: str) -> str:
     if not decl:
         raise DefinitionError("Argument must be non-empty.")
 
-    for rc in _RESERVED:
+    for rc in RESERVED_CHARACTERS:
         if rc in decl:
             raise DefinitionError(f"Argument {decl!r} contains reserved character {rc!r}.")
     return decl
 
 
 def _parse_decls(decls: Sequence[str]) -> tuple[list[str], list[str]]:
     if not decls:
@@ -56,36 +53,35 @@
                 raise DefinitionError(f"Short option {decl!r} is too long.")
             short_options.append(decl)
         elif not decl:
             raise DefinitionError("Option must be non-empty.")
         else:
             raise DefinitionError(f"Option must start with {LONG_PREFIX!r} or {SHORT_PREFIX!r}, got {decl!r}.")
 
-        if inter := _RESERVED.intersection(decl):
-            inter_str = ", ".join(map(repr, sorted(inter)))
-            raise DefinitionError(f"Option {decl!r} contains reserved character {inter_str}.")
+        if rcs := RESERVED_CHARACTERS.intersection(decl):
+            rcs_str = ", ".join(map(repr, sorted(rcs)))
+            raise DefinitionError(f"Option {decl!r} contains reserved character {rcs_str}.")
     return long_options, short_options
 
 
 class Argument:
     """The argument, aka positional argument.
 
     Parameters:
         decl (str):
             The declaration for this argument.
         dest (str | None, default=None):
-            The destination used to store/forward the argument value. If ``None``,
-            infer from declaration. If empty string, disable store/forward.
+            The destination used to store the argument value. If ``None``, infer
+            from declaration. If empty string, disable the store action.
         nargs (int, default=1):
-            The number of argument values. Valid values are ``nargs == 1`` or
-            ``nargs == -1``.
+            The number of argument values. Valid values are ``1`` or ``-1``.
         required (bool, default=False):
             Whether this argument is required or optional.
         type (Type | type | None, default=None):
-            The type converter. If ``None``, use ``Str()``.
+            The type converter. If ``None``, use :class:`clixx.types.Str()`.
         default (Any, default=None):
             The default value used if argument omitted.
         hidden (bool, default=False):
             If ``True``, hide this argument from help information.
         show_default (bool, default=False):
             If ``True``, show the default value in help information.
         metavar (str | None, default=None):
@@ -119,48 +115,46 @@
         self.metavar = metavar
         self.help = help
 
     @staticmethod
     def _parse(decl: str, *, dest: str | None) -> tuple[str, str]:
         argument = _parse_decl(decl)
 
-        # Infer destination from declaration if ``dest`` not given.
         if dest is not None:  # noqa
             dest = _check_dest(dest) if dest else ""
         else:
             dest = _check_dest(argument)
         return dest, argument
 
     def store(self, args: dict[str, Any], value: str) -> None:
         """Store value to destination."""
 
         if not self.dest:
             return
 
         result = self.type.convert_str(value)
         if self.nargs == 1:
+            if self.dest in args:  # noexcept
+                self.type.release(args[self.dest])
             args[self.dest] = result
         else:
             # Variadic arguments are stored as list.
             cast(list, args.setdefault(self.dest, [])).append(result)
 
     def store_default(self, args: dict[str, Any]) -> None:
         """Store default value to destination."""
 
-        if not self.dest:
+        if not self.dest or self.dest in args:
             return
 
-        if self.nargs == 1:
-            result = None if self.default is None else self.type(self.default)
+        if self.nargs == 1:  # noqa
+            result = self.type(self.default) if self.default is not None else None
         else:
-            # Variadic arguments are stored as list. Defaults to empty list.
-            if self.default is None:
-                result = []
-            else:
-                result = [self.type(value) for value in cast(list, self.default)]
+            # Variadic arguments default to empty list.
+            result = []
         args[self.dest] = result
 
     def format_decl(self) -> str:
         """Format declaration."""
 
         return repr(self.argument)
 
@@ -188,17 +182,15 @@
 
     @default.setter
     def default(self, value: Any) -> None:
         if value is not None:
             if self.nargs == 1:
                 value = self._verify(value)
             else:
-                if not isinstance(value, (list, tuple)):
-                    raise DefinitionError("For nargs == -1, the default value must be list, tuple or None.")
-                value = [self._verify(v) for v in value]
+                raise DefinitionError("For nargs == -1, the default value must be None.")
         self._default = value
 
     def _verify(self, value: Any) -> Any:
         try:
             return self.type.safe_convert(value)
         except TypeConversionError as e:
             raise DefinitionError(f"Invalid default value for argument {self.format_decl()}. {str(e)}") from e
@@ -207,20 +199,20 @@
 class Option:
     """The option, aka optional argument.
 
     Parameters:
         decls (tuple[str, ...]):
             The declarations for this option.
         dest (str | None, default=None):
-            The destination used to store/forward the option value. If ``None``,
-            infer from declarations. If empty string, disable store/forward.
+            The destination used to store the option value. If ``None``, infer
+            from declarations. If empty string, disable the store action.
         required (bool, default=False):
             Whether this option is required or optional.
         type (Type | type | None, default=None):
-            The type converter. If ``None``, use ``Str()``.
+            The type converter. If ``None``, use :class:`clixx.types.Str()`.
         default (Any, default=None):
             The default value used if option omitted.
         hidden (bool, default=False):
             If ``True``, hide this option from help information.
         show_default (bool, default=False):
             If ``True``, show the default value in help information.
         metavar (str | None, default=None):
@@ -251,15 +243,14 @@
         self.metavar = metavar
         self.help = help
 
     @staticmethod
     def _parse(decls: Sequence[str], *, dest: str | None = None) -> tuple[str, list[str], list[str]]:
         long_options, short_options = _parse_decls(decls)
 
-        # Infer destination from declarations if ``dest`` not given.
         if dest is not None:
             dest = _check_dest(dest) if dest else ""
         elif long_options:
             dest = _check_dest(long_options[0][LONG_PREFIX_LEN:])
         else:
             dest = _check_dest(short_options[0][SHORT_PREFIX_LEN:])
         return dest, long_options, short_options
@@ -270,31 +261,33 @@
         Availability: ``nargs == 1``.
         """
 
         if not self.dest:
             return
 
         result = self.type.convert_str(value)
+        if self.dest in args:  # noexcept
+            self.type.release(args[self.dest])
         args[self.dest] = result
 
     def store_const(self, args: dict[str, Any]) -> None:
         """Store constant value to destination.
 
         Availability: ``nargs == 0``.
         """
 
         raise NotImplementedError
 
     def store_default(self, args: dict[str, Any]) -> None:
         """Store default value to destination."""
 
-        if not self.dest:
+        if not self.dest or self.dest in args:
             return
 
-        result = None if self.default is None else self.type(self.default)
+        result = self.type(self.default) if self.default is not None else None
         args[self.dest] = result
 
     def format_decls(self) -> str:
         """Format declarations."""
 
         return " / ".join(map(repr, self.short_options + self.long_options))
 
@@ -337,16 +330,16 @@
 class FlagOption(Option):
     """The flag option.
 
     Parameters:
         decls (tuple[str, ...]):
             The declarations for this option.
         dest (str | None, default=None):
-            The destination used to store/forward the option value. If ``None``,
-            infer from declarations. If empty string, disable store/forward.
+            The destination used to store the option value. If ``None``, infer
+            from declarations. If empty string, disable the store action.
         const (Any, default=True):
             The constant value used if option occurred.
         default (Any, default=False):
             The default value used if option omitted.
         hidden (bool, default=False):
             If ``True``, hide this option from help information.
         help (str, default=''):
@@ -378,15 +371,17 @@
     def store(self, args: dict[str, Any], value: str) -> None:
         raise NotImplementedError
 
     def store_const(self, args: dict[str, Any]) -> None:
         if not self.dest:
             return
 
-        result = None if self.const is None else self.type(self.const)
+        result = self.type(self.const) if self.const is not None else None
+        if self.dest in args:  # noexcept
+            self.type.release(args[self.dest])
         args[self.dest] = result
 
     @property
     def nargs(self) -> int:
         """Return ``0``.
 
         Note:
@@ -412,18 +407,18 @@
 class AppendOption(Option):
     """The append option.
 
     Parameters:
         decls (tuple[str, ...]):
             The declarations for this option.
         dest (str | None, default=None):
-            The destination used to store/forward the option value. If ``None``,
-            infer from declarations. If empty string, disable store/forward.
+            The destination used to store the option value. If ``None``, infer
+            from declarations. If empty string, disable the store action.
         type (Type | type | None, default=None):
-            The type converter. If ``None``, use ``Str()``.
+            The type converter. If ``None``, use :class:`clixx.types.Str()`.
         hidden (bool, default=False):
             If ``True``, hide this option from help information.
         metavar (str | None, default=None):
             The option value name used in usage. If ``None``, infer from
             declarations. If empty string, disable metavar.
         help (str, default=''):
             The help information.
@@ -454,15 +449,15 @@
         if not self.dest:
             return
 
         result = self.type.convert_str(value)
         cast(list, args.setdefault(self.dest, [])).append(result)
 
     def store_default(self, args: dict[str, Any]) -> None:
-        if not self.dest:
+        if not self.dest or self.dest in args:
             return
 
         args[self.dest] = []
 
     @property
     def nargs(self) -> int:
         """Return ``1``.
@@ -478,26 +473,26 @@
 class CountOption(Option):
     """The count option.
 
     Parameters:
         decls (tuple[str, ...]):
             The declarations for this option.
         dest (str | None, default=None):
-            The destination used to store/forward the option value. If ``None``,
-            infer from declarations. If empty string, disable store/forward.
-        default (Any, default=0):
+            The destination used to store the option value. If ``None``, infer
+            from declarations. If empty string, disable the store action.
+        default (int, default=0):
             The default value used if option omitted.
         hidden (bool, default=False):
             If ``True``, hide this option from help information.
         help (str, default=''):
             The help information.
     """
 
     def __init__(
-        self, *decls: str, dest: str | None = None, default: Any = 0, hidden: bool = False, help: str = ""
+        self, *decls: str, dest: str | None = None, default: int = 0, hidden: bool = False, help: str = ""
     ) -> None:
         super().__init__(
             *decls,
             dest=dest,
             required=False,
             type=Int(),
             default=default,
@@ -601,7 +596,25 @@
     """
 
     def __init__(self, *decls: str, hidden: bool = False, help: str = "Show version information and exit.") -> None:
         super().__init__(*decls, hidden=hidden, help=help)
 
     def store_const(self, args: dict[str, Any]) -> None:
         raise VersionSignal
+
+
+def is_separator(arg: str) -> bool:
+    """Determine whether the ``arg`` is a separator."""
+
+    return arg == SEPARATOR
+
+
+def is_long_option(arg: str) -> bool:
+    """Determine whether the ``arg`` is a long option."""
+
+    return arg.startswith(LONG_PREFIX) and len(arg) > LONG_PREFIX_LEN
+
+
+def is_short_option(arg: str) -> bool:
+    """Determine whether the ``arg`` is a short option."""
+
+    return arg.startswith(SHORT_PREFIX) and len(arg) > SHORT_PREFIX_LEN
```

### Comparing `clixx-0.7.0a0/src/clixx/commands.py` & `clixx-0.8.0a0/src/clixx/parsers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,351 +1,360 @@
 from __future__ import annotations
 
-import sys
-from contextlib import suppress
-from typing import TYPE_CHECKING, Any, Callable, Iterator, Literal, NoReturn, Optional, TypeVar, Union, overload
-
-from .constants import DEST_COMMAND_NAME
-from .exceptions import CommandError
-from .groups import ArgumentGroup, CommandGroup, OptionGroup
-from .parsers import Context, Parser, SuperParser
-from .printers import PrinterFactory, PrinterHelper, SuperPrinterFactory, SuperPrinterHelper
-
-if TYPE_CHECKING:
-    from typing_extensions import Self
-
-ProcessFunction = Callable[..., Optional[int]]
-
-
-def _dummy_func(*args: Any, **kwargs: Any) -> None:
-    pass
-
-
-def _interpret_standalone(standalone: bool) -> dict[str, bool]:
-    return {"is_exit": standalone, "is_raise": not standalone}
-
-
-def _exit_command(exit_code: int | None, standalone: bool) -> int | NoReturn:
-    if standalone:
-        sys.exit(exit_code)
-    return 0 if exit_code is None else exit_code
-
-
-class _Command:
-    #: The parent command. Should be set by parent.
-    parent: SuperCommand | None
-    #: The program name. Should be set by parent.
-    prog: str | None
-    #: The parsed arguments. Should be set after parsing by ``__call__``.
-    args: dict[str, Any] | None
-
-    def __init__(
-        self, name: str | None = None, version: str | None = None, description: str = "", *, pass_cmd: bool = False
-    ) -> None:
-        self.name = name
-        self.version = version
-        self.description = description
-
-        self.pass_cmd = pass_cmd
-
-        self.parent = None
-        self.prog = None
-        self.args = None
-
-        self.process_function = _dummy_func
-
-    def get_name(self) -> str:
-        if self.name is not None:
-            return self.name
-        if self.parent is not None:
-            return self.parent.get_name()
-        return "Unknown Program"
-
-    def get_version(self) -> str:
-        if self.version is not None:
-            return self.version
-        if self.parent is not None:
-            return self.parent.get_version()
-        return "Unknown Version"
-
-    def get_prog(self) -> str:
-        prog = sys.argv[0] if self.prog is None else self.prog
-        if self.parent is None:
-            return prog
-        return f"{self.parent.get_prog()} {prog}"
+import weakref
+from contextlib import contextmanager
+from typing import Any, Callable, Generator, cast
+
+from .arguments import Argument, Option, is_long_option, is_separator, is_short_option
+from .constants import DEST_COMMAND_NAME, SHORT_PREFIX_LEN
+from .exceptions import (
+    InvalidArgumentValue,
+    InvalidOptionValue,
+    MissingOption,
+    ParserContextError,
+    TooFewArguments,
+    TooFewOptionValues,
+    TooManyArguments,
+    TooManyOptionValues,
+    TypeConversionError,
+    UnknownOption,
+)
+from .groups import ArgumentGroup, OptionGroup
+
+
+@contextmanager
+def _raise_invalid_argument_value(format_decl: Callable[[], str]) -> Generator[None, None, None]:
+    try:
+        yield
+    except TypeConversionError as e:
+        name = format_decl()
+        raise InvalidArgumentValue(f"Invalid value for argument {name}. {str(e)}") from e
+
+
+@contextmanager
+def _raise_invalid_option_value(format_decls: Callable[[], str]) -> Generator[None, None, None]:
+    try:
+        yield
+    except TypeConversionError as e:
+        name = format_decls()
+        raise InvalidOptionValue(f"Invalid value for option {name}. {str(e)}") from e
+
+
+class ArgumentNode:
+    """The stateful argument node."""
+
+    def __init__(self, argument: Argument, parent: ArgumentGroupNode) -> None:
+        self._argument = argument
+        self.parent = cast(ArgumentGroupNode, weakref.proxy(parent))
+        self.occurred = False
+
+    def _inc_occurred(self) -> None:
+        if not self.occurred:
+            self.occurred = True
+            self.parent.num_occurred += 1
+
+    def store(self, args: dict[str, Any], value: str) -> None:
+        with _raise_invalid_argument_value(self.format_decl):
+            self._argument.store(args, value)
+        self._inc_occurred()
+
+    def store_default(self, args: dict[str, Any]) -> None:
+        with _raise_invalid_argument_value(self.format_decl):
+            self._argument.store_default(args)
+
+    def format_decl(self) -> str:
+        return self._argument.format_decl()
+
+    @property
+    def nargs(self) -> int:
+        return self._argument.nargs
 
     @property
-    def process_function(self) -> ProcessFunction:
-        """The process function."""
+    def required(self) -> bool:
+        return self._argument.required
 
-        return self._process_function
 
-    @process_function.setter
-    def process_function(self, value: ProcessFunction) -> None:
-        self._process_function = value
-
-
-class Command(_Command):
-    """The command.
-
-    Parameters:
-        name (str | None, default=None):
-            The name used when showing version information.
-        version (str | None, default=None):
-            The version used when showing version information.
-        description (str, default=''):
-            The description.
-        pass_cmd (bool, default=False):
-            If ``True``, pass this command instance to the process function.
-        printer_factory (PrinterFactory | None, default=None):
-            The printer factory.
-        printer_config (dict[str, Any] | None, default=None):
-            The printer config.
-    """
-
-    def __init__(
-        self,
-        name: str | None = None,
-        version: str | None = None,
-        description: str = "",
-        *,
-        pass_cmd: bool = False,
-        printer_factory: PrinterFactory | None = None,
-        printer_config: dict[str, Any] | None = None,
-    ) -> None:
-        super().__init__(name, version, description, pass_cmd=pass_cmd)
-
-        self.printer_factory = printer_factory
-        self.printer_config = printer_config
-
-        self.argument_groups: list[ArgumentGroup] = []
-        self.option_groups: list[OptionGroup] = []
-
-    def add_argument_group(self, group: ArgumentGroup) -> Self:
-        self.argument_groups.append(group)
-        return self
-
-    def add_option_group(self, group: OptionGroup) -> Self:
-        self.option_groups.append(group)
-        return self
-
-    def __call__(
-        self,
-        argv: list[str] | None = None,
-        *,
-        parent: SuperCommand | None = None,
-        prog: str | None = None,
-        standalone: bool = True,
-    ) -> int | NoReturn:
-        with PrinterHelper(self, self.printer_factory, self.printer_config, **_interpret_standalone(standalone)):
-            self.parent = parent
-            self.prog = prog
+class ArgumentGroupNode:
+    """The stateful argument group node."""
 
-            args = self.parse_args(argv, **_interpret_standalone(standalone))
-            self.args = args
+    def __init__(self, group: ArgumentGroup, children: list[ArgumentNode]) -> None:
+        self._group = group
+        self.children = children
+        self.num_occurred = 0
+
+
+class OptionNode:
+    """The stateful option node."""
+
+    def __init__(self, option: Option, parent: OptionGroupNode) -> None:
+        self._option = option
+        self.parent = cast(OptionGroupNode, weakref.proxy(parent))
+        self.occurred = False
+
+    def _inc_occurred(self) -> None:
+        if not self.occurred:
+            self.occurred = True
+            self.parent.num_occurred += 1
+
+    def store(self, args: dict[str, Any], value: str, *, key: str) -> None:
+        with _raise_invalid_option_value(lambda: repr(key)):
+            self._option.store(args, value)
+        self._inc_occurred()
+
+    def store_const(self, args: dict[str, Any]) -> None:
+        with _raise_invalid_option_value(self.format_decls):
+            self._option.store_const(args)
+        self._inc_occurred()
+
+    def store_default(self, args: dict[str, Any]) -> None:
+        with _raise_invalid_option_value(self.format_decls):
+            self._option.store_default(args)
+
+    def format_decls(self) -> str:
+        return self._option.format_decls()
+
+    @property
+    def nargs(self) -> int:
+        return self._option.nargs
+
+    @property
+    def required(self) -> bool:
+        return self._option.required
 
-            if self.pass_cmd:  # noqa
-                exit_code = self.process_function(self, **args)
-            else:
-                exit_code = self.process_function(**args)
 
-        return _exit_command(exit_code, standalone)
+class OptionGroupNode:
+    """The stateful option group node."""
 
-    @overload
-    def parse_args(
-        self, argv: list[str] | None = None, *, is_exit: bool = True, is_raise: bool = False, return_ctx: Literal[True]
-    ) -> tuple[dict[str, Any], Context]:
-        ...
-
-    @overload
-    def parse_args(
-        self, argv: list[str] | None = None, *, is_exit: bool = True, is_raise: bool = False, return_ctx: Literal[False]
-    ) -> dict[str, Any]:
-        ...
-
-    @overload
-    def parse_args(
-        self, argv: list[str] | None = None, *, is_exit: bool = True, is_raise: bool = False
-    ) -> dict[str, Any]:
-        ...
-
-    @overload
-    def parse_args(
-        self, argv: list[str] | None = None, *, is_exit: bool = True, is_raise: bool = False, return_ctx: bool
-    ) -> dict[str, Any] | tuple[dict[str, Any], Context]:
-        ...
-
-    def parse_args(
-        self, argv: list[str] | None = None, *, is_exit: bool = True, is_raise: bool = False, return_ctx: bool = False
-    ) -> dict[str, Any] | tuple[dict[str, Any], Context]:
-        args: dict[str, Any] = {}
-        argv = sys.argv[1:] if argv is None else argv
-        with PrinterHelper(self, self.printer_factory, self.printer_config, is_exit=is_exit, is_raise=is_raise):
-            parser = Parser(self.argument_groups, self.option_groups)
-            ctx = parser.parse_args(args, argv)
-
-        if return_ctx:
-            return args, ctx
-        return args
-
-
-class SuperCommand(_Command):
-    """The super command.
-
-    Parameters:
-        name (str | None, default=None):
-            The name used when showing version information.
-        version (str | None, default=None):
-            The version used when showing version information.
-        description (str, default=''):
-            The description.
-        pass_cmd (bool, default=False):
-            If ``True``, pass this command instance to the process function.
-        printer_factory (SuperPrinterFactory | None, default=None):
-            The super printer factory.
-        printer_config (dict[str, Any] | None, default=None):
-            The super printer config.
-    """
-
-    def __init__(
-        self,
-        name: str | None = None,
-        version: str | None = None,
-        description: str = "",
-        *,
-        pass_cmd: bool = False,
-        printer_factory: SuperPrinterFactory | None = None,
-        printer_config: dict[str, Any] | None = None,
-    ) -> None:
-        super().__init__(name, version, description, pass_cmd=pass_cmd)
-
-        self.printer_factory = printer_factory
-        self.printer_config = printer_config
-
-        self.option_groups: list[OptionGroup] = []
-
-    def add_option_group(self, group: OptionGroup) -> Self:
-        self.option_groups.append(group)
-        return self
-
-    def iter_command_group(self) -> Iterator[CommandGroup]:
-        raise NotImplementedError
-
-    def load_command(self, name: str) -> Command | SuperCommand | None:
-        raise NotImplementedError
-
-    def __call__(
-        self,
-        argv: list[str] | None = None,
-        *,
-        parent: SuperCommand | None = None,
-        prog: str | None = None,
-        standalone: bool = True,
-    ) -> int | NoReturn:
-        with SuperPrinterHelper(self, self.printer_factory, self.printer_config, **_interpret_standalone(standalone)):
-            self.parent = parent
-            self.prog = prog
-
-            args, ctx = self.parse_args(argv, **_interpret_standalone(standalone), return_ctx=True)
-            self.args = args
+    def __init__(self, group: OptionGroup, children: list[OptionNode]) -> None:
+        self._group = group
+        self.children = children
+        self.num_occurred = 0
 
-            if (cmd_name := args.pop(DEST_COMMAND_NAME, None)) is None:
-                raise CommandError("Missing command.")
+    def check(self) -> None:
+        self._group.check(self.num_occurred)
 
-            if (cmd := self.load_command(cmd_name)) is None:
-                raise CommandError(f"Unknown command {cmd_name!r}.")
 
-            if self.pass_cmd:  # noqa
-                exit_code = self.process_function(self, **args)
+class Context:
+    """The context for a parsing."""
+
+    def __init__(self, args: dict[str, Any], argv: list[str]) -> None:
+        self.args = args
+        self.argv = argv
+        self._index = 0
+        self._curr_arg: str | None = None
+
+    @property
+    def curr_arg(self) -> str | None:
+        return self._curr_arg
+
+    @property
+    def next_arg(self) -> str | None:
+        if self._index < len(self.argv):
+            arg = self.argv[self._index]
+            self._index += 1
+        else:
+            arg = None
+        self._curr_arg = arg
+        return arg
+
+    @property
+    def argc_consumed(self) -> int:
+        return self._index
+
+    @property
+    def argv_remained(self) -> list[str]:
+        return self.argv[self._index :]
+
+
+class ArgumentParser:
+    """The parser for arguments."""
+
+    def __init__(self, argument_groups: list[ArgumentGroup]) -> None:
+        self.argument_tree, self.argument_seq = self._build(argument_groups)
+        self._pos = 0
+
+    @staticmethod
+    def _build(argument_groups: list[ArgumentGroup]) -> tuple[list[ArgumentGroupNode], list[ArgumentNode]]:
+        tree: list[ArgumentGroupNode] = []
+        seq: list[ArgumentNode] = []
+        for group in argument_groups:
+            group_node = ArgumentGroupNode(group, [])
+            tree.append(group_node)
+            for argument in group:
+                node = ArgumentNode(argument, group_node)
+                group_node.children.append(node)
+                seq.append(node)
+        return tree, seq
+
+    def finalize(self, ctx: Context, args: dict[str, Any]) -> None:
+        for group in self.argument_tree:
+            for argument in group.children:
+                if not argument.occurred:
+                    if argument.required:
+                        raise TooFewArguments(
+                            f"Got too few arguments. {argument.format_decl()} is required but not given."
+                        )
+                    argument.store_default(args)
+
+    def _get_argument(self, arg: str) -> ArgumentNode:
+        if self._pos >= len(self.argument_seq):
+            raise TooManyArguments(f"Got too many arguments. Found extra argument {arg!r}.")
+        argument = self.argument_seq[self._pos]
+        if argument.nargs == 1:
+            self._pos += 1
+        return argument
+
+    def parse_argument(self, ctx: Context, args: dict[str, Any], arg: str) -> None:
+        argument = self._get_argument(arg)
+        argument.store(args, arg)
+
+
+class OptionParser:
+    """The parser for options."""
+
+    def __init__(self, option_groups: list[OptionGroup]) -> None:
+        self.option_tree, self.option_map = self._build(option_groups)
+
+    @staticmethod
+    def _build(option_groups: list[OptionGroup]) -> tuple[list[OptionGroupNode], dict[str, OptionNode]]:
+        tree: list[OptionGroupNode] = []
+        map: dict[str, OptionNode] = {}
+        for group in option_groups:
+            group_node = OptionGroupNode(group, [])
+            tree.append(group_node)
+            for option in group:
+                node = OptionNode(option, group_node)
+                group_node.children.append(node)
+                for key in option.long_options:
+                    if key in map:
+                        raise ParserContextError(f"Option {key!r} conflicts.")
+                    map[key] = node
+                for key in option.short_options:
+                    if key in map:
+                        raise ParserContextError(f"Option {key!r} conflicts.")
+                    map[key] = node
+        return tree, map
+
+    def finalize(self, ctx: Context, args: dict[str, Any]) -> None:
+        for group in self.option_tree:
+            for option in group.children:
+                if not option.occurred:
+                    if option.required:
+                        raise MissingOption(f"Missing option {option.format_decls()}.")
+                    option.store_default(args)
+            group.check()
+
+    def _get_option(self, key: str) -> OptionNode:
+        option = self.option_map.get(key, None)
+        if option is None:
+            raise UnknownOption(f"Unknown option {key!r}.")
+        return option
+
+    def parse_long_option(self, ctx: Context, args: dict[str, Any], arg: str) -> None:
+        value: str | None
+
+        if "=" in arg:  # --option=value
+            key, value = arg.split("=", 1)
+            option = self._get_option(key)
+            if option.nargs == 0:
+                raise TooManyOptionValues(f"Option {key!r} does not take a value.")
+            option.store(args, value, key=key)
+
+        else:  # --option [value]
+            key = arg
+            option = self._get_option(key)
+            if option.nargs == 0:
+                option.store_const(args)
             else:
-                exit_code = self.process_function(**args)
+                if (value := ctx.next_arg) is None:
+                    raise TooFewOptionValues(f"Option {key!r} requires a value.")
+                option.store(args, value, key=key)
+
+    def parse_short_option(self, ctx: Context, args: dict[str, Any], arg: str) -> None:
+        index = SHORT_PREFIX_LEN
+        while index < len(arg):
+            key = "-" + arg[index]
+            index += 1
+            option = self._get_option(key)
 
-            exit_code = cmd(ctx.argv_remained, standalone=standalone)
+            if option.nargs == 0:
+                option.store_const(args)
+            else:
+                value: str | None
+
+                if index < len(arg):  # -ovalue
+                    value = arg[index:]
+                else:  # -o value
+                    if (value := ctx.next_arg) is None:
+                        raise TooFewOptionValues(f"Option {key!r} requires a value.")
+                option.store(args, value, key=key)
+                break  # end of parsing
+
+
+class Parser:
+    """The command-line interface parser."""
+
+    def __init__(self, argument_groups: list[ArgumentGroup], option_groups: list[OptionGroup]) -> None:
+        self.argument_groups = argument_groups
+        self.option_groups = option_groups
+
+    def parse_args(self, args: dict[str, Any], argv: list[str]) -> Context:
+        ctx = Context(args, argv)
+        argument_parser = ArgumentParser(self.argument_groups)
+        option_parser = OptionParser(self.option_groups)
+
+        switch_to_positional_only = False
+        while (arg := ctx.next_arg) is not None:
+            if is_separator(arg):
+                switch_to_positional_only = True
+                break
+            elif is_long_option(arg):
+                option_parser.parse_long_option(ctx, args, arg)
+            elif is_short_option(arg):
+                option_parser.parse_short_option(ctx, args, arg)
+            else:
+                argument_parser.parse_argument(ctx, args, arg)
 
-        return _exit_command(exit_code, standalone)
+        if switch_to_positional_only:
+            while (arg := ctx.next_arg) is not None:
+                argument_parser.parse_argument(ctx, args, arg)
+
+        option_parser.finalize(ctx, args)
+        argument_parser.finalize(ctx, args)
+        return ctx
+
+
+class SuperParser:
+    """The super command-line interface parser."""
+
+    def __init__(self, option_groups: list[OptionGroup]) -> None:
+        self.option_groups = option_groups
+
+    def parse_args(self, args: dict[str, Any], argv: list[str]) -> Context:
+        ctx = Context(args, argv)
+        option_parser = OptionParser(self.option_groups)
+
+        switch_to_positional_only = False
+        while (arg := ctx.next_arg) is not None:
+            if is_separator(arg):
+                switch_to_positional_only = True
+                break
+            elif is_long_option(arg):
+                option_parser.parse_long_option(ctx, args, arg)
+            elif is_short_option(arg):
+                option_parser.parse_short_option(ctx, args, arg)
+            else:
+                self._store_command(ctx, args, arg)
+                break
 
-    @overload
-    def parse_args(
-        self, argv: list[str] | None = None, *, is_exit: bool = True, is_raise: bool = False, return_ctx: Literal[True]
-    ) -> tuple[dict[str, Any], Context]:
-        ...
-
-    @overload
-    def parse_args(
-        self, argv: list[str] | None = None, *, is_exit: bool = True, is_raise: bool = False, return_ctx: Literal[False]
-    ) -> dict[str, Any]:
-        ...
-
-    @overload
-    def parse_args(
-        self, argv: list[str] | None = None, *, is_exit: bool = True, is_raise: bool = False
-    ) -> dict[str, Any]:
-        ...
-
-    @overload
-    def parse_args(
-        self, argv: list[str] | None = None, *, is_exit: bool = True, is_raise: bool = False, return_ctx: bool
-    ) -> dict[str, Any] | tuple[dict[str, Any], Context]:
-        ...
-
-    def parse_args(
-        self, argv: list[str] | None = None, *, is_exit: bool = True, is_raise: bool = False, return_ctx: bool = False
-    ) -> dict[str, Any] | tuple[dict[str, Any], Context]:
-        args: dict[str, Any] = {}
-        argv = sys.argv[1:] if argv is None else argv
-        with SuperPrinterHelper(self, self.printer_factory, self.printer_config, is_exit=is_exit, is_raise=is_raise):
-            parser = SuperParser(self.option_groups)
-            ctx = parser.parse_args(args, argv)
-
-        if return_ctx:
-            return args, ctx
-        return args
-
-
-AnyCommand = TypeVar("AnyCommand", bound=Union[Command, SuperCommand])
-
-
-class SimpleSuperCommand(SuperCommand):
-    def __init__(
-        self,
-        name: str | None = None,
-        version: str | None = None,
-        description: str = "",
-        *,
-        pass_cmd: bool = False,
-        printer_factory: SuperPrinterFactory | None = None,
-        printer_config: dict[str, Any] | None = None,
-    ) -> None:
-        super().__init__(
-            name,
-            version,
-            description,
-            pass_cmd=pass_cmd,
-            printer_factory=printer_factory,
-            printer_config=printer_config,
-        )
-        self.commands: dict[str, dict[str, Command | SuperCommand]] = {}
-
-    def add_command(self, group_name: str, cmd_name: str, cmd: Command | SuperCommand) -> Self:
-        group_dict = self.commands.setdefault(group_name, {})
-        group_dict[cmd_name] = cmd
-        return self
-
-    def register_command(self, group_name: str, cmd_name: str) -> Callable[[AnyCommand], AnyCommand]:
-        def decorator(cmd: AnyCommand) -> AnyCommand:
-            self.add_command(group_name, cmd_name, cmd)
-            return cmd
-
-        return decorator
-
-    def iter_command_group(self) -> Iterator[CommandGroup]:
-        for group_name, group_dict in self.commands.items():
-            group = CommandGroup(group_name)
-            for cmd_name in group_dict:
-                group.add(cmd_name)
-            yield group
-
-    def load_command(self, name: str) -> Command | SuperCommand | None:
-        for group_dict in self.commands.values():
-            with suppress(KeyError):
-                return group_dict[name]
-        return None
+        if switch_to_positional_only:
+            while (arg := ctx.next_arg) is not None:
+                self._store_command(ctx, args, arg)
+                break
+
+        option_parser.finalize(ctx, args)
+        return ctx
+
+    @staticmethod
+    def _store_command(ctx: Context, args: dict[str, Any], arg: str) -> None:
+        # Store command name to a special destination.
+        args[DEST_COMMAND_NAME] = arg
```

### Comparing `clixx-0.7.0a0/src/clixx/decorators.py` & `clixx-0.8.0a0/src/clixx/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 from __future__ import annotations
 
 from contextlib import suppress
-from typing import Any, Callable, TypeVar
+from typing import Any, Callable, TypeVar, Union
 
 from .arguments import AppendOption, Argument, CountOption, FlagOption, HelpOption, Option, VersionOption
-from .commands import Command, ProcessFunction, SimpleSuperCommand
+from .commands import Command, CommandFunction, SimpleSuperCommand, SuperCommandFunction
 from .exceptions import DefinitionError
 from .groups import ANY, ArgumentGroup, GroupType, OptionGroup
 from .printers import PrinterFactory, SuperPrinterFactory
 from .types import Type
 
-F = TypeVar("F", bound=ProcessFunction)
+CF = TypeVar("CF", bound=CommandFunction)
+SCF = TypeVar("SCF", bound=SuperCommandFunction)
+F = TypeVar("F", bound=Union[CommandFunction, SuperCommandFunction])
 
 
 def _prepare_definition(func: F, obj: Argument | Option | ArgumentGroup | OptionGroup) -> None:
     if not hasattr(func, "__clixx_definition__"):
-        func.__clixx_definition__ = []  # type: ignore [attr-defined]
-    func.__clixx_definition__.append(obj)  # type: ignore [attr-defined]
+        func.__clixx_definition__ = []  # type: ignore [union-attr]
+    func.__clixx_definition__.append(obj)  # type: ignore [union-attr]
 
 
 def argument(
     decl: str,
     *,
     dest: str | None = None,
     nargs: int = 1,
     required: bool = False,
     type: Type | type | None = None,
     default: Any = None,
     hidden: bool = False,
     show_default: bool = False,
     metavar: str | None = None,
     help: str = "",
-) -> Callable[[F], F]:
+) -> Callable[[CF], CF]:
     """The argument, aka positional argument.
 
     Parameters:
         decl (str):
             The declaration for this argument.
         dest (str | None, default=None):
             The destination used to store/forward the argument value. If ``None``,
@@ -56,15 +58,15 @@
         metavar (str | None, default=None):
             The argument value name used in usage. If ``None``, infer from
             declaration. If empty string, disable metavar.
         help (str, default=''):
             The help information.
     """
 
-    def decorator(func: F) -> F:
+    def decorator(func: CF) -> CF:
         obj = Argument(
             decl,
             dest=dest,
             nargs=nargs,
             required=required,
             type=type,
             default=default,
@@ -313,16 +315,16 @@
     name: str | None = None,
     version: str | None = None,
     description: str = "",
     *,
     pass_cmd: bool = False,
     printer_factory: PrinterFactory | None = None,
     printer_config: dict[str, Any] | None = None,
-) -> Callable[[F], Command]:
-    def decorator(func: F) -> Command:
+) -> Callable[[CF], Command]:
+    def decorator(func: CF) -> Command:
         cmd = Command(
             name,
             version,
             description,
             pass_cmd=pass_cmd,
             printer_factory=printer_factory,
             printer_config=printer_config,
@@ -345,30 +347,30 @@
                         if isinstance(group, Argument):
                             raise DefinitionError(f"Found non-grouped argument {group!r}.")
                         if isinstance(group, Option):
                             raise DefinitionError(f"Found non-grouped option {group!r}.")
                         raise DefinitionError(f"Found unexpected object {group!r}.")
                     group = member
 
-        cmd.process_function = func
+        cmd.function = func
         return cmd
 
     return decorator
 
 
 def simple_super_command(
     name: str | None = None,
     version: str | None = None,
     description: str = "",
     *,
     pass_cmd: bool = False,
     printer_factory: SuperPrinterFactory | None = None,
     printer_config: dict[str, Any] | None = None,
-) -> Callable[[F], SimpleSuperCommand]:
-    def decorator(func: F) -> SimpleSuperCommand:
+) -> Callable[[SCF], SimpleSuperCommand]:
+    def decorator(func: SCF) -> SimpleSuperCommand:
         cmd = SimpleSuperCommand(
             name,
             version,
             description,
             pass_cmd=pass_cmd,
             printer_factory=printer_factory,
             printer_config=printer_config,
@@ -389,11 +391,11 @@
                         if isinstance(group, Argument):
                             raise DefinitionError("Super command does not support argument.")
                         if isinstance(group, Option):
                             raise DefinitionError(f"Found non-grouped option {group!r}.")
                         raise DefinitionError(f"Found unexpected object {group!r}.")
                     group = member
 
-        cmd.process_function = func
+        cmd.function = func
         return cmd
 
     return decorator
```

### Comparing `clixx-0.7.0a0/src/clixx/exceptions.py` & `clixx-0.8.0a0/src/clixx/exceptions.py`

 * *Files identical despite different names*

### Comparing `clixx-0.7.0a0/src/clixx/groups.py` & `clixx-0.8.0a0/src/clixx/groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 
 import enum
-from typing import TYPE_CHECKING, Final, Generic, Iterator, TypeVar
+from typing import Final, Generic, Iterator, TypeVar
+
+from typing_extensions import Self
 
 from .arguments import Argument, Option
 from .exceptions import GroupError
 
-if TYPE_CHECKING:  # pragma: no cover
-    from typing_extensions import Self
-
 
 class GroupType(enum.Enum):
     """The group constraint type."""
 
     ANY = enum.auto()  #: Require any.
     ALL = enum.auto()  #: Require all.
     NONE = enum.auto()  #: Require none.
@@ -108,25 +107,26 @@
         """Check the group constraint.
 
         Parameters:
             num_occurred (int):
                 The number of occurred options.
         """
 
-        if self.type == ANY:
+        type = self.type
+        if type == ANY:
             return self._check_any(num_occurred)
-        elif self.type == ALL:
+        elif type == ALL:
             return self._check_all(num_occurred)
-        elif self.type == NONE:
+        elif type == NONE:
             return self._check_none(num_occurred)
-        elif self.type == AT_LEAST_ONE:
+        elif type == AT_LEAST_ONE:
             return self._check_at_least_one(num_occurred)
-        elif self.type == AT_MOST_ONE:
+        elif type == AT_MOST_ONE:
             return self._check_at_most_one(num_occurred)
-        elif self.type == EXACTLY_ONE:
+        elif type == EXACTLY_ONE:
             return self._check_exactly_one(num_occurred)
         else:
             raise AssertionError
 
     def _check_any(self, num_occurred: int) -> None:
         pass
```

### Comparing `clixx-0.7.0a0/src/clixx/printers.py` & `clixx-0.8.0a0/src/clixx/printers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import sys
 from typing import TYPE_CHECKING, Any, Callable, Dict, Protocol
 
+from typing_extensions import Self
+
 from .exceptions import CLIXXException, HelpSignal, VersionSignal
 
 if TYPE_CHECKING:  # pragma: no cover
-    from typing_extensions import Self
-
     from .commands import Command, SuperCommand
 
 
 class Printer(Protocol):
     """The protocol class for printer."""
 
     def print_error(self, cmd: Command, exc: CLIXXException) -> None:
```

### Comparing `clixx-0.7.0a0/src/clixx/types.py` & `clixx-0.8.0a0/src/clixx/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 import datetime
 import enum
 import os
 import pathlib
 import stat
 import sys
 from contextlib import suppress
-from typing import IO, Any, Callable, Sequence, cast
+from typing import IO, Any, Callable, Sequence, Union, cast
 
 from .exceptions import DefinitionError, TypeConversionError
 
 
 def _force_decode(filename: Any) -> str:
-    fn = os.fspath(filename)
-    if isinstance(fn, str):
-        return fn
-    return fn.decode(sys.getfilesystemencoding(), "backslashreplace")
+    fname = cast(Union[str, bytes], os.fspath(filename))
+    if isinstance(fname, str):
+        return fname
+    return fname.decode(sys.getfilesystemencoding(), "backslashreplace")
 
 
 def _resolve_norm(case_sensitive: bool) -> Callable[[str], str]:
     if case_sensitive:
         return str
     return str.casefold
 
 
 class Type:
     """The base class for all CLIXX type converters.
 
-    This class also represents any type which does not apply type conversion.
+    This class also represents *any* type which does not apply type conversion.
     """
 
     def __call__(self, value: Any) -> Any:
         """Convert to expected value."""
 
         if isinstance(value, str):
             return self.convert_str(value)
@@ -45,23 +45,33 @@
 
     def convert_str(self, value: str) -> Any:
         """Convert string to expected value."""
 
         return value
 
     def safe_convert(self, value: Any) -> Any:
-        """Safe convert to compatible value."""
+        """Safe convert to compatible value without side effect.
+
+        This is used to verify and preprocess the *constant*/*default* values.
+        """
 
         return self(value)
 
+    def release(self, value: Any) -> None:
+        """Release the resource.
+
+        This is used to release the resource for the previous parsed values
+        which are overrided by the current value.
+        """
+
     def format(self, value: Any) -> str:
         """Format value.
 
         The ``value`` must be compatible with this type, usually the return
-        value of :meth:`~Type.safe_convert`.
+        value of :meth:`~clixx.types.Type.safe_convert`.
         """
 
         return str(value)
 
     def suggest_metavar(self) -> str | None:
         """Suggest metavar for help information."""
 
@@ -393,14 +403,18 @@
         errors (str | None, default=None):
             The same as :func:`open`.
         newline (str | None, default=None):
             The same as :func:`open`.
         dash (bool, default=True):
             If ``True``, recognize dash (-) as stdin/stdout.
 
+    Important:
+        CLIXX will not close the file automatically when the command is
+        finished. It's user's responsibility to close the file.
+
     Warning:
         The dash will be recognized only if ``value`` is a string. That means
         ``pathlib.Path("-")`` will never be recognized as stdin/stdout.
 
     See Also:
         - https://docs.python.org/3/library/functions.html#open
     """
@@ -421,62 +435,65 @@
         self.errors = errors
         self.newline = newline
         self.dash = dash
 
     def convert(self, value: Any) -> Any:
         if hasattr(value, "read") or hasattr(value, "write"):
             return value
-        if isinstance(value, pathlib.Path):
+        if isinstance(value, (bytes, pathlib.Path)):
             return self._open(value)
         raise TypeConversionError(f"{value!r} is not a valid file.")
 
     def convert_str(self, value: str) -> Any:
         if self.dash and value == "-":
             if "r" in self.mode:
                 return sys.stdin.buffer if "b" in self.mode else sys.stdin
             else:
                 return sys.stdout.buffer if "b" in self.mode else sys.stdout
         return self._open(value)
 
-    def _open(self, path: str | pathlib.Path) -> IO:
+    def _open(self, path: str | bytes | pathlib.Path) -> IO:
         try:
             return open(  # noqa
                 path, self.mode, self.buffering, encoding=self.encoding, errors=self.errors, newline=self.newline
             )
         except OSError as e:
             raise TypeConversionError(f"Can not open {str(path)!r}. {e.strerror}.") from e
 
     def safe_convert(self, value: Any) -> Any:
-        if isinstance(value, (str, pathlib.Path)) or hasattr(value, "read") or hasattr(value, "write"):
+        if isinstance(value, (str, bytes, pathlib.Path)) or hasattr(value, "read") or hasattr(value, "write"):
             return value
         raise TypeConversionError(f"{value!r} is not a valid file.")
 
+    def release(self, value: Any) -> None:
+        cast(IO, value).close()
+
     def format(self, value: Any) -> str:
-        assert isinstance(value, (str, pathlib.Path)) or hasattr(value, "read") or hasattr(value, "write")
-        if isinstance(value, (str, pathlib.Path)):
-            return str(value)
-        if hasattr(value, "name"):
+        # These types can be decoded anyway.
+        if isinstance(value, (str, bytes, pathlib.Path)):
+            return _force_decode(value)
+        # The file object may know its filename.
+        if (name := getattr(value, "name", None)) is not None:
             with suppress(TypeError):
-                return _force_decode(value.name)
+                return _force_decode(name)
         # This file does not have a pretty string representation. Just return a rough string.
         return str(value)
 
     def suggest_metavar(self) -> str | None:
         return "FILE"
 
 
 class Path(Type):
     """The class used to convert command-line arguments to path.
 
     Target type: :class:`pathlib.Path`.
 
     Parameters:
         resolve (bool, default=False):
-            If ``True``, make the path absolute, resolve all symlinks, and
-            normalize it.
+            If ``True``, make the path absolute, resolve all symlinks, and normalize it.
         exists (bool, default=False):
             If ``True``, check whether the path exists.
         readable (bool, default=False):
             If ``True``, check whether the path is readable.
         writable (bool, default=False):
             If ``True``, check whether the path is writable.
         executable (bool, default=False):
@@ -497,14 +514,19 @@
         self.readable = readable
         self.writable = writable
         self.executable = executable
 
     def convert(self, value: Any) -> Any:
         if isinstance(value, pathlib.Path):
             return self._check_path(value)
+        if isinstance(value, bytes):
+            try:
+                return self.convert_str(os.fsdecode(value))
+            except Exception as e:
+                raise TypeConversionError(f"{value!r} is not a valid path.") from e
         raise TypeConversionError(f"{value!r} is not a valid path.")
 
     def convert_str(self, value: str) -> Any:
         return self._check_path(pathlib.Path(value))
 
     def _check_path(self, path: pathlib.Path) -> pathlib.Path:
         if self.resolve:
@@ -527,61 +549,66 @@
         return path
 
     @staticmethod
     def _check_path_stat(path: pathlib.Path, st: os.stat_result) -> None:
         pass
 
     def safe_convert(self, value: Any) -> Any:
-        if isinstance(value, (str, pathlib.Path)):
+        if isinstance(value, (str, bytes, pathlib.Path)):
             return value
         raise TypeConversionError(f"{value!r} is not a valid path.")
 
+    def format(self, value: Any) -> str:
+        return _force_decode(value)
+
     def suggest_metavar(self) -> str | None:
         return "PATH"
 
 
 class DirPath(Path):
-    """Similar to :class:`Path`, but check whether the path is a directory if it exists."""
+    """Similar to :class:`clixx.types.Path`, but check whether the path is a
+    directory if it exists."""
 
     @staticmethod
     def _check_path_stat(path: pathlib.Path, st: os.stat_result) -> None:
         if not stat.S_ISDIR(st.st_mode):
             raise TypeConversionError(f"{str(path)!r} is not a directory.")
 
     def suggest_metavar(self) -> str | None:
         return "DIRECTORY"
 
 
 class FilePath(Path):
-    """Similar to :class:`Path`, but check whether the path is a file if it exists."""
+    """Similar to :class:`clixx.types.Path`, but check whether the path is a
+    file if it exists."""
 
     @staticmethod
     def _check_path_stat(path: pathlib.Path, st: os.stat_result) -> None:
         if not stat.S_ISREG(st.st_mode):
             raise TypeConversionError(f"{str(path)!r} is not a file.")
 
     def suggest_metavar(self) -> str | None:
         return "FILE"
 
 
 def resolve_type(type: Type | type) -> Type:
     """Convert Python's builtin type to CLIXX's type. Return as is if ``type``
-    is already an instance of :class:`Type`.
+    is already an instance of :class:`clixx.types.Type`.
 
-    +----------------+------------------+
-    | Source         | Target           |
-    +================+==================+
-    | :class:`str`   | :class:`Str()`   |
-    +----------------+------------------+
-    | :class:`bool`  | :class:`Bool()`  |
-    +----------------+------------------+
-    | :class:`int`   | :class:`Int()`   |
-    +----------------+------------------+
-    | :class:`float` | :class:`Float()` |
-    +----------------+------------------+
+    +----------------+------------------------------+
+    | Source         | Target                       |
+    +================+==============================+
+    | :class:`str`   | :class:`clixx.types.Str()`   |
+    +----------------+------------------------------+
+    | :class:`bool`  | :class:`clixx.types.Bool()`  |
+    +----------------+------------------------------+
+    | :class:`int`   | :class:`clixx.types.Int()`   |
+    +----------------+------------------------------+
+    | :class:`float` | :class:`clixx.types.Float()` |
+    +----------------+------------------------------+
     """
 
     if isinstance(type, Type):
         return type
     if type is str:
         return Str()
     if type is bool:
```

### Comparing `clixx-0.7.0a0/src/clixx.egg-info/PKG-INFO` & `clixx-0.8.0a0/src/clixx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clixx
-Version: 0.7.0a0
+Version: 0.8.0a0
 Summary: Command-line interface parser & framework for Python
 Home-page: https://github.com/xymy/clixx
 Author: xymy
 Author-email: thyfan@163.com
 Maintainer: xymy
 Maintainer-email: thyfan@163.com
 License: MIT
```

### Comparing `clixx-0.7.0a0/src/clixx.egg-info/SOURCES.txt` & `clixx-0.8.0a0/src/clixx.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 pyproject.toml
 setup.cfg
 docs/Makefile
 docs/make.bat
 docs/release.py
 docs/requirements.txt
 docs/source/conf.py
-docs/source/index.rst
 docs/source/api/arguments.rst
 docs/source/api/exceptions.rst
 docs/source/api/groups.rst
 docs/source/api/index.rst
 docs/source/api/printers.rst
 docs/source/api/types.rst
 src/clixx/__init__.py
```

