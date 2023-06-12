# Comparing `tmp/cfgpie-3.0.1.tar.gz` & `tmp/cfgpie-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfgpie-3.0.1.tar", last modified: Fri May 26 06:52:34 2023, max compression
+gzip compressed data, was "cfgpie-3.0.2.tar", last modified: Mon Jun 12 10:04:26 2023, max compression
```

## Comparing `cfgpie-3.0.1.tar` & `cfgpie-3.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 06:52:34.132279 cfgpie-3.0.1/
--rw-rw-rw-   0        0        0     1090 2022-09-04 11:44:11.000000 cfgpie-3.0.1/LICENSE
--rw-rw-rw-   0        0        0       14 2022-10-24 07:53:37.000000 cfgpie-3.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5732 2023-05-26 06:52:34.132279 cfgpie-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4929 2023-05-24 15:13:32.000000 cfgpie-3.0.1/README.md
--rw-rw-rw-   0        0        0       93 2022-08-10 18:07:14.000000 cfgpie-3.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      963 2023-05-26 06:52:34.132279 cfgpie-3.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 06:52:34.116667 cfgpie-3.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 06:52:34.132279 cfgpie-3.0.1/src/cfgpie/
--rw-rw-rw-   0        0        0      145 2023-05-24 14:22:23.000000 cfgpie-3.0.1/src/cfgpie/__init__.py
--rw-rw-rw-   0        0        0      719 2023-05-24 14:22:23.000000 cfgpie-3.0.1/src/cfgpie/constants.py
--rw-rw-rw-   0        0        0      275 2023-05-24 14:16:08.000000 cfgpie-3.0.1/src/cfgpie/exceptions.py
--rw-rw-rw-   0        0        0     7339 2023-05-26 06:47:54.000000 cfgpie-3.0.1/src/cfgpie/handlers.py
--rw-rw-rw-   0        0        0     1270 2023-05-24 14:08:16.000000 cfgpie-3.0.1/src/cfgpie/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:52:34.132279 cfgpie-3.0.1/src/cfgpie.egg-info/
--rw-rw-rw-   0        0        0     5732 2023-05-26 06:52:34.000000 cfgpie-3.0.1/src/cfgpie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-05-26 06:52:34.000000 cfgpie-3.0.1/src/cfgpie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 06:52:34.000000 cfgpie-3.0.1/src/cfgpie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-04 16:13:39.000000 cfgpie-3.0.1/src/cfgpie.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-05-26 06:52:34.000000 cfgpie-3.0.1/src/cfgpie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 10:04:26.047438 cfgpie-3.0.2/
+-rw-rw-rw-   0        0        0     1090 2022-09-04 11:44:11.000000 cfgpie-3.0.2/LICENSE
+-rw-rw-rw-   0        0        0       14 2022-10-24 07:53:37.000000 cfgpie-3.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5732 2023-06-12 10:04:26.047438 cfgpie-3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4929 2023-05-24 15:13:32.000000 cfgpie-3.0.2/README.md
+-rw-rw-rw-   0        0        0       93 2022-08-10 18:07:14.000000 cfgpie-3.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      963 2023-06-12 10:04:26.047438 cfgpie-3.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 10:04:26.028496 cfgpie-3.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 10:04:26.042425 cfgpie-3.0.2/src/cfgpie/
+-rw-rw-rw-   0        0        0      145 2023-05-24 14:22:23.000000 cfgpie-3.0.2/src/cfgpie/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-05-24 14:22:23.000000 cfgpie-3.0.2/src/cfgpie/constants.py
+-rw-rw-rw-   0        0        0      275 2023-05-24 14:16:08.000000 cfgpie-3.0.2/src/cfgpie/exceptions.py
+-rw-rw-rw-   0        0        0     7757 2023-06-12 09:58:53.000000 cfgpie-3.0.2/src/cfgpie/handlers.py
+-rw-rw-rw-   0        0        0     1270 2023-05-24 14:08:16.000000 cfgpie-3.0.2/src/cfgpie/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 10:04:26.047438 cfgpie-3.0.2/src/cfgpie.egg-info/
+-rw-rw-rw-   0        0        0     5732 2023-06-12 10:04:26.000000 cfgpie-3.0.2/src/cfgpie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-06-12 10:04:26.000000 cfgpie-3.0.2/src/cfgpie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 10:04:26.000000 cfgpie-3.0.2/src/cfgpie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-04 16:13:39.000000 cfgpie-3.0.2/src/cfgpie.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-12 10:04:26.000000 cfgpie-3.0.2/src/cfgpie.egg-info/top_level.txt
```

### Comparing `cfgpie-3.0.1/LICENSE` & `cfgpie-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cfgpie-3.0.1/PKG-INFO` & `cfgpie-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfgpie
-Version: 3.0.1
+Version: 3.0.2
 Summary: Simplified `ConfigParser` setup.
 Home-page: https://github.com/ClaudiuDrug/cfgpie
 Author: Claudiu DRUG
 Author-email: claudiu.drug@outlook.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ClaudiuDrug/cfgpie/issues
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `cfgpie-3.0.1/README.md` & `cfgpie-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cfgpie-3.0.1/setup.cfg` & `cfgpie-3.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6667 7069 650d 0a76 6572 7369   = cfgpie..versi
-00000020: 6f6e 203d 2033 2e30 2e31 0d0a 6175 7468  on = 3.0.1..auth
+00000020: 6f6e 203d 2033 2e30 2e32 0d0a 6175 7468  on = 3.0.2..auth
 00000030: 6f72 203d 2043 6c61 7564 6975 2044 5255  or = Claudiu DRU
 00000040: 470d 0a61 7574 686f 725f 656d 6169 6c20  G..author_email 
 00000050: 3d20 636c 6175 6469 752e 6472 7567 406f  = claudiu.drug@o
 00000060: 7574 6c6f 6f6b 2e63 6f6d 0d0a 6c69 6365  utlook.com..lice
 00000070: 6e73 6520 3d20 4d49 5420 4c69 6365 6e73  nse = MIT Licens
 00000080: 650d 0a64 6573 6372 6970 7469 6f6e 203d  e..description =
 00000090: 2053 696d 706c 6966 6965 6420 6043 6f6e   Simplified `Con
```

### Comparing `cfgpie-3.0.1/src/cfgpie/constants.py` & `cfgpie-3.0.2/src/cfgpie/constants.py`

 * *Files identical despite different names*

### Comparing `cfgpie-3.0.1/src/cfgpie/handlers.py` & `cfgpie-3.0.2/src/cfgpie/handlers.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from .constants import NAME, INSTANCES, RLOCKS, ROOT
 from .exceptions import ArgParseError
 from .utils import folder, file, ensure_folder, as_dict
 
 __all__ = [
     "BasicInterpolation",
     "ExtendedInterpolation",
+    "Singleton",
+    "ArgsParser",
     "CfgParser",
 ]
 
 
 DEFAULTS: dict = {
     "directory": ROOT,
 }
@@ -33,14 +35,66 @@
     "dict": literal_eval,
     "path": realpath,
     "folder": folder,
     "file": file,
 }
 
 
+class Singleton(object):
+
+    @staticmethod
+    def _check_name(value: str) -> str:
+        if not isinstance(value, str):
+            raise TypeError(
+                f"CfgParser 'name' attribute must be of "
+                f"type 'str' not '{type(value).__name__}'!"
+            )
+        if len(value) == 0:
+            raise ValueError(
+                f"CfgParser 'name' attribute must be a "
+                f"string object with a length greater than '0'!"
+            )
+        return value
+
+    @staticmethod
+    def _check_defaults(params: dict):
+        defaults: dict = DEFAULTS.copy()
+        if "defaults" in params:
+            defaults.update(params.pop("defaults"))
+        params.update(defaults=defaults)
+
+    @staticmethod
+    def _check_interpolation(params: dict):
+        if "interpolation" not in params:
+            params.update(interpolation=ExtendedInterpolation())
+
+    @staticmethod
+    def _check_converters(params: dict):
+        converters: dict = CONVERTERS.copy()
+        if "converters" in params:
+            converters.update(params.pop("converters"))
+        params.update(converters=converters)
+
+    def __init__(self, parser: Type[CfgParser]):
+        self._parser = parser
+
+    def __call__(self, name: str = NAME, **kwargs):
+        self._check_name(name)
+        if name not in INSTANCES:
+            self._check_params(kwargs)
+            instance = self._parser(name, **kwargs)
+            INSTANCES.update({name: instance})
+        return INSTANCES.get(name)
+
+    def _check_params(self, params: dict):
+        self._check_defaults(params)
+        self._check_interpolation(params)
+        self._check_converters(params)
+
+
 class ArgsParser(object):
 
     @staticmethod
     def _check_argv(args: Union[str, List[str], Tuple[str]]) -> Union[List[str], Tuple[str]]:
         if args is None:
             return argv[1:]
         elif isinstance(args, str):
@@ -79,27 +133,14 @@
                         else:
                             raise ArgParseError(f"Incorrect value '{value}' for parameter '{arg}'!")
             else:
                 raise ArgParseError(f"Inconsistency in cmd-line parameters '{arg}'!")
         return temp
 
 
-class Singleton(object):
-
-    def __init__(self, parser: Type[CfgParser]):
-        self._parser = parser
-
-    def __call__(self, name: str = NAME, **kwargs):
-        self._parser._check_name(name)
-        if name not in INSTANCES:
-            instance = self._parser(name, **kwargs)
-            INSTANCES.update({name: instance})
-        return INSTANCES.get(name)
-
-
 @Singleton
 class CfgParser(ConfigParser, ArgsParser):
     """
     ConfigParser that:
 
         - sets `DEFAULT` section with `directory` pointing at root folder of the project;
         - implements interpolation using :class:`ExtendedInterpolation()`;
@@ -109,45 +150,17 @@
     @staticmethod
     def _dispatch_rlock(name: str = NAME) -> RLock:
         if name not in RLOCKS:
             instance: RLock = RLock()
             RLOCKS.update({name: instance})
         return RLOCKS.get(name)
 
-    @staticmethod
-    def _check_name(value: str) -> str:
-        if not isinstance(value, str):
-            raise TypeError(
-                f"CfgParser 'name' attribute must be of "
-                f"type 'str' not '{type(value).__name__}'!"
-            )
-        if len(value) == 0:
-            raise ValueError(
-                f"CfgParser 'name' attribute must be a "
-                f"string object with a length greater than '0'!"
-            )
-        return value
-
     def __init__(self, name: str = NAME, **kwargs):
-        self._name = name
-
-        defaults: dict = DEFAULTS.copy()
-        if "defaults" in kwargs:
-            defaults.update(kwargs.pop("defaults"))
-        kwargs.update(defaults=defaults)
-
-        if "interpolation" not in kwargs:
-            kwargs.update(interpolation=ExtendedInterpolation())
-
-        converters: dict = CONVERTERS.copy()
-        if "converters" in kwargs:
-            converters.update(kwargs.pop("converters"))
-        kwargs.update(converters=converters)
-
         super(ConfigParser, self).__init__(**kwargs)
+        self._name = name
 
     @property
     def name(self) -> str:
         return self._name
 
     def open(self, file_path: str, encoding: str = "UTF-8", fallback: dict = None):
         """
```

### Comparing `cfgpie-3.0.1/src/cfgpie/utils.py` & `cfgpie-3.0.2/src/cfgpie/utils.py`

 * *Files identical despite different names*

### Comparing `cfgpie-3.0.1/src/cfgpie.egg-info/PKG-INFO` & `cfgpie-3.0.2/src/cfgpie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfgpie
-Version: 3.0.1
+Version: 3.0.2
 Summary: Simplified `ConfigParser` setup.
 Home-page: https://github.com/ClaudiuDrug/cfgpie
 Author: Claudiu DRUG
 Author-email: claudiu.drug@outlook.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ClaudiuDrug/cfgpie/issues
 Classifier: Programming Language :: Python :: 3.7
```

