# Comparing `tmp/screens_py-0.5.0.post1.tar.gz` & `tmp/screens_py-0.5.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screens_py-0.5.0.post1.tar", max compression
+gzip compressed data, was "screens_py-0.5.0.post2.tar", max compression
```

## Comparing `screens_py-0.5.0.post1.tar` & `screens_py-0.5.0.post2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35134 2023-06-12 19:09:16.833566 screens_py-0.5.0.post1/LICENSE
--rw-r--r--   0        0        0      766 2023-06-12 19:09:16.833566 screens_py-0.5.0.post1/README.md
--rw-r--r--   0        0        0      447 2023-06-12 20:34:01.098575 screens_py-0.5.0.post1/pyproject.toml
--rw-r--r--   0        0        0      134 2023-06-12 19:09:16.833566 screens_py-0.5.0.post1/screens/__init__.py
--rw-r--r--   0        0        0      714 2023-06-12 19:09:16.833566 screens_py-0.5.0.post1/screens/exceptions.py
--rw-r--r--   0        0        0      457 2023-06-12 20:33:12.464308 screens_py-0.5.0.post1/screens/req.py
--rw-r--r--   0        0        0     1906 2023-06-12 19:09:16.833566 screens_py-0.5.0.post1/screens/screens.py
--rw-r--r--   0        0        0       99 2023-06-12 19:09:16.833566 screens_py-0.5.0.post1/screens/units.py
--rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 screens_py-0.5.0.post1/PKG-INFO
+-rw-r--r--   0        0        0    35134 2023-06-12 19:09:16.833566 screens_py-0.5.0.post2/LICENSE
+-rw-r--r--   0        0        0      766 2023-06-12 19:09:16.833566 screens_py-0.5.0.post2/README.md
+-rw-r--r--   0        0        0      447 2023-06-12 20:55:55.274686 screens_py-0.5.0.post2/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-06-12 19:09:16.833566 screens_py-0.5.0.post2/screens/__init__.py
+-rw-r--r--   0        0        0      608 2023-06-12 21:20:26.748179 screens_py-0.5.0.post2/screens/exceptions.py
+-rw-r--r--   0        0        0      467 2023-06-12 21:44:16.639778 screens_py-0.5.0.post2/screens/req.py
+-rw-r--r--   0        0        0     1946 2023-06-12 21:42:19.488677 screens_py-0.5.0.post2/screens/screens.py
+-rw-r--r--   0        0        0       81 2023-06-12 21:26:54.865241 screens_py-0.5.0.post2/screens/units.py
+-rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 screens_py-0.5.0.post2/PKG-INFO
```

### Comparing `screens_py-0.5.0.post1/LICENSE` & `screens_py-0.5.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `screens_py-0.5.0.post1/README.md` & `screens_py-0.5.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `screens_py-0.5.0.post1/screens/exceptions.py` & `screens_py-0.5.0.post2/screens/exceptions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 class CreateScreenError(Exception):
     """Called if screen session creation has failed."""
     def __init__(self, *args: str) -> None:
         """Called if the screen command does not exist."""
-        self.msg = "Failed to create a screen-session" if len(args) == 0 else " ".join([str(i) for i in args])
-    
-    def __str__(self) -> str: return self.msg
+        if len(args) > 0: self.args = args
+        else: self.args = ("Failed to create a screen-session.",)
 
 class ScreenExistsError(Exception):
     """Called if the screen command does not exist"""
     def __init__(self, *args: str) -> None:
         """Called if the screen command does not exist"""
-        self.msg = "Install the 'screen' on your device!" if len(args) == 0 else " ".join([str(i) for i in args])
-    
-    def __str__(self) -> str: return self.msg
+        if len(args) > 0: self.args = args
+        else: self.args = ("Install the 'screen' on your device!",)
```

### Comparing `screens_py-0.5.0.post1/screens/screens.py` & `screens_py-0.5.0.post2/screens/screens.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,41 +3,44 @@
 from typing import List, Optional, Dict, Any
 # > Local Import's
 from .units import SCREEN_LS
 from .req import screen, check_pattern
 from .exceptions import CreateScreenError
 
 class Screen:
-    def __init__(self, name: str, **kwargs) -> None:
+    def __init__(self, name: str, *args, **kwargs) -> None:
         self.name = name
-        self.id = kwargs.get("id", None)
+        self.id: Optional[int] = kwargs.get("id", None)
         
         if self.id is None:
             if (s:=get_session_by_name(self.name)) is not None:
                 self.id: int = s.id
             else:
                 try:
-                    screen("-d", "-m", "-S", f"{name}")
+                    screen("-dmS", f"\"{name}\"")
                     s: Screen = get_session_by_name(self.name)
                     self.id: int = s.id
                 except:
                     raise CreateScreenError()
     
-    def __str__(self) -> str: return f'ScreenSession(name={self.name.__repr__()}, id={self.id.__repr__()})'
-    def __repr__(self) -> str: return self.__str__()
+    def __str__(self) -> str:
+        return f'ScreenSession(name={repr(self.name)}, id={repr(self.id)})'
+    
+    def __repr__(self) -> str:
+        return self.__str__()
     
     def kill(self) -> None:
         if self.id is not None:
             Process(self.id).kill()
             self.id = None
             wipe()
     
     def send_command(self, c: str) -> None:
         if self.id is not None:
-            screen("-r", self.name, "-X", "stuff", f"{c} \r")
+            screen("-r", f"\"{self.name}\"", "-X", "stuff", f"\"{c}\r\"")
 
 # ! Other
 def wipe() -> None: screen("-wipe")
 
 # ! Get Sessions
 def get_sessions_dict() -> List[Dict[str, Any]]:
     patcher, sessions = Patcher(), []
@@ -54,8 +57,8 @@
     for i in get_sessions():
         if name == i.name:
             return i
 
 def get_session_by_id(_id: int) -> Optional[Screen]:
     for i in get_sessions():
         if _id == i.id:
-            return i
+            return i
```

### Comparing `screens_py-0.5.0.post1/PKG-INFO` & `screens_py-0.5.0.post2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screens-py
-Version: 0.5.0.post1
+Version: 0.5.0.post2
 Summary: A light-weight library for easy interaction between Python and GNU screen.
 License: GNU GENERAL PUBLIC
 Author: Romani
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

