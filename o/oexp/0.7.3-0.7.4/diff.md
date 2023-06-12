# Comparing `tmp/oexp-0.7.3.tar.gz` & `tmp/oexp-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oexp-0.7.3.tar", last modified: Mon Jun 12 14:11:30 2023, max compression
+gzip compressed data, was "oexp-0.7.4.tar", last modified: Mon Jun 12 15:29:40 2023, max compression
```

## Comparing `oexp-0.7.3.tar` & `oexp-0.7.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 14:11:30.203868 oexp-0.7.3/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-12 14:11:30.203629 oexp-0.7.3/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.7.3/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 14:11:30.202061 oexp-0.7.3/oexp/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.7.3/oexp/__init__.py
--r--r--r--   0 matthewgroth   (501) staff       (20)    80499 2023-06-12 13:23:43.000000 oexp-0.7.3/oexp/access.py
--r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-06-12 13:23:43.000000 oexp-0.7.3/oexp/gen.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     2011 2023-06-12 01:50:22.000000 oexp-0.7.3/oexp/jbridge.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 14:11:30.203232 oexp-0.7.3/oexp/util/
--rw-r--r--   0 matthewgroth   (501) staff       (20)        0 2023-06-10 17:43:13.000000 oexp-0.7.3/oexp/util/__init__.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     2650 2023-06-12 14:09:05.000000 oexp-0.7.3/oexp/util/ops.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     1612 2023-06-10 17:47:40.000000 oexp-0.7.3/oexp/util/vals.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 14:11:30.202816 oexp-0.7.3/oexp.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-12 14:11:30.000000 oexp-0.7.3/oexp.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      281 2023-06-12 14:11:30.000000 oexp-0.7.3/oexp.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-06-12 14:11:30.000000 oexp-0.7.3/oexp.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-06-12 14:11:30.000000 oexp-0.7.3/oexp.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-06-12 14:11:30.000000 oexp-0.7.3/oexp.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-06-12 14:11:25.000000 oexp-0.7.3/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-06-12 14:11:30.203933 oexp-0.7.3/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 15:29:40.267432 oexp-0.7.4/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-12 15:29:40.267268 oexp-0.7.4/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.7.4/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 15:29:40.266040 oexp-0.7.4/oexp/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.7.4/oexp/__init__.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)    82438 2023-06-12 15:02:08.000000 oexp-0.7.4/oexp/access.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-06-12 15:02:07.000000 oexp-0.7.4/oexp/gen.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2011 2023-06-12 01:50:22.000000 oexp-0.7.4/oexp/jbridge.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 15:29:40.267079 oexp-0.7.4/oexp/util/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        0 2023-06-10 17:43:13.000000 oexp-0.7.4/oexp/util/__init__.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2650 2023-06-12 14:09:05.000000 oexp-0.7.4/oexp/util/ops.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     1612 2023-06-10 17:47:40.000000 oexp-0.7.4/oexp/util/vals.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 15:29:40.266676 oexp-0.7.4/oexp.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-12 15:29:40.000000 oexp-0.7.4/oexp.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      281 2023-06-12 15:29:40.000000 oexp-0.7.4/oexp.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-06-12 15:29:40.000000 oexp-0.7.4/oexp.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-06-12 15:29:40.000000 oexp-0.7.4/oexp.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-06-12 15:29:40.000000 oexp-0.7.4/oexp.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-06-12 15:29:35.000000 oexp-0.7.4/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-06-12 15:29:40.267475 oexp-0.7.4/setup.cfg
```

### Comparing `oexp-0.7.3/oexp/access.py` & `oexp-0.7.4/oexp/access.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     global _SAFE_PROCESS, _SAFE_THREAD
     if current_process().pid != _SAFE_PROCESS or current_thread().ident != _SAFE_THREAD:
         raise Exception(
             f"Python-Kotlin communication is currently not safe to use across multiple threads or processes. If you need this feature, please let me know."
         )
 
 
-JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/526/oexp-front-0-all.jar"
+JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/527/oexp-front-0-all.jar"
 
 
 class OexpExitSocketHeaders(Enum):
     EXIT = b"\x00"
 
 
 EXIT = b"\x00"
@@ -483,19 +483,45 @@
         _sendall(CALL_FUN)
         _send_long(self._id._id)
         _send_int(5)
         _recv_exception_check()
         return _recv_confirmation()
 
     # [[matt.oexp.front.api.Experiment#sessionUrl]]
-    def session_url(self) -> str:
+    def session_url(self, disable_auto_fullscreen, allow_fullscreen_exit) -> str:
         _ensure_synchronized()
         _sendall(CALL_FUN)
         _send_long(self._id._id)
         _send_int(6)
+        if disable_auto_fullscreen == DEFAULT_VALUE:
+            _sendall(b"\x00")
+        else:
+            _sendall(b"\x01")
+            if disable_auto_fullscreen is None:
+                _sendall(b"\x00")
+            else:
+                _sendall(b"\x01")
+            if disable_auto_fullscreen is not None:
+                if disable_auto_fullscreen:
+                    _sendall(b"\x01")
+                else:
+                    _sendall(b"\x00")
+        if allow_fullscreen_exit == DEFAULT_VALUE:
+            _sendall(b"\x00")
+        else:
+            _sendall(b"\x01")
+            if allow_fullscreen_exit is None:
+                _sendall(b"\x00")
+            else:
+                _sendall(b"\x01")
+            if allow_fullscreen_exit is not None:
+                if allow_fullscreen_exit:
+                    _sendall(b"\x01")
+                else:
+                    _sendall(b"\x00")
         _recv_exception_check()
         return _recv_string(nullable=False)
 
     # [[matt.oexp.front.api.Experiment#subjectData]]
     def subject_data(self) -> SubjectData:
         _ensure_synchronized()
         _sendall(CALL_FUN)
@@ -1383,14 +1409,15 @@
 
 def experiment_start(
     pid=NO_DEFAULT,
     session_id=NO_DEFAULT,
     unix_time_millis=NO_DEFAULT,
     session_number=NO_DEFAULT,
     exp_uid=NO_DEFAULT,
+    query_params=DEFAULT_VALUE,
 ):
     if pid == NO_DEFAULT:
         raise Exception(f"there is no default value for pid, so it must be defined")
     if session_id == NO_DEFAULT:
         raise Exception(
             f"there is no default value for session_id, so it must be defined"
         )
@@ -1400,15 +1427,17 @@
         )
     if session_number == NO_DEFAULT:
         raise Exception(
             f"there is no default value for session_number, so it must be defined"
         )
     if exp_uid == NO_DEFAULT:
         raise Exception(f"there is no default value for exp_uid, so it must be defined")
-    return ExperimentStart(pid, session_id, unix_time_millis, session_number, exp_uid)
+    return ExperimentStart(
+        pid, session_id, unix_time_millis, session_number, exp_uid, query_params
+    )
 
 
 # [[matt.oexp.olang.model.ExperimentStart]]
 class ExperimentStart(ExperimentEvent, KBClass):
     def __init__(self, *args, _id=None):
         _ensure_synchronized()
         if _id is None:
@@ -1416,14 +1445,27 @@
             _sendall(CREATE_OBJECT)
             _send_string("matt.oexp.olang.model.ExperimentStart")
             _send_long(args[0]._id._id)
             _send_long(args[1]._id._id)
             _send_long(args[2])
             _send_long(args[3]._id._id)
             _send_long(args[4]._id._id)
+            if args[5] == DEFAULT_VALUE:
+                _sendall(b"\x00")
+            else:
+                _sendall(b"\x01")
+                if args[5] is None:
+                    _sendall(b"\x00")
+                else:
+                    _sendall(b"\x01")
+                if args[5] is not None:
+                    _send_int(len(args[5]))
+                    for k, v in args[5].items():
+                        _send_string(k)
+                        _send_string(v)
             self._id = _object_id(_recv_long())
         else:
             self._id = _object_id(_id)
 
     # [[matt.oexp.olang.model.ExperimentStart#expUID]]
     @property
     def exp_uid(self) -> ExperimentUid:
@@ -1440,41 +1482,55 @@
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(1)
         temp = _recv_object(ProlificParticipantUid, nullable=False)
         return temp
 
+    # [[matt.oexp.olang.model.ExperimentStart#queryParams]]
+    @property
+    def query_params(self) -> Optional[Dict[str, str]]:
+        _ensure_synchronized()
+        _sendall(GET_VAL)
+        _send_long(self._id._id)
+        _send_int(2)
+        temp = _recv_map(
+            keyReceiveFun=lambda: _recv_string(nullable=False),
+            valueReceiveFun=lambda: _recv_string(nullable=False),
+            nullable=True,
+        )
+        return temp
+
     # [[matt.oexp.olang.model.ExperimentStart#sessionID]]
     @property
     def session_id(self) -> ProlificSessionId:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
-        _send_int(2)
+        _send_int(3)
         temp = _recv_object(ProlificSessionId, nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.ExperimentStart#sessionNumber]]
     @property
     def session_number(self) -> SessionNumber:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
-        _send_int(3)
+        _send_int(4)
         temp = _recv_object(SessionNumber, nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.ExperimentStart#unixTimeMillis]]
     @property
     def unix_time_millis(self) -> int:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
-        _send_int(4)
+        _send_int(5)
         temp = _recv_long(nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.ExperimentStart]]
     def to_json(self):
         _ensure_synchronized()
         _sendall(GET_JSON)
```

### Comparing `oexp-0.7.3/oexp/jbridge.py` & `oexp-0.7.4/oexp/jbridge.py`

 * *Files identical despite different names*

### Comparing `oexp-0.7.3/oexp/util/ops.py` & `oexp-0.7.4/oexp/util/ops.py`

 * *Files identical despite different names*

### Comparing `oexp-0.7.3/oexp/util/vals.py` & `oexp-0.7.4/oexp/util/vals.py`

 * *Files identical despite different names*

