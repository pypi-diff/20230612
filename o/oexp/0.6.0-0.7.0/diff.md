# Comparing `tmp/oexp-0.6.0.tar.gz` & `tmp/oexp-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oexp-0.6.0.tar", last modified: Tue May  9 02:37:50 2023, max compression
+gzip compressed data, was "oexp-0.7.0.tar", last modified: Mon Jun 12 02:48:56 2023, max compression
```

## Comparing `oexp-0.6.0.tar` & `oexp-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 02:37:50.245425 oexp-0.6.0/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 02:37:50.245232 oexp-0.6.0/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.6.0/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 02:37:50.244340 oexp-0.6.0/oexp/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.6.0/oexp/__init__.py
--r--r--r--   0 matthewgroth   (501) staff       (20)    79528 2023-05-09 02:37:35.000000 oexp-0.6.0/oexp/access.py
--r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-05-09 02:37:20.000000 oexp-0.6.0/oexp/gen.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     5375 2023-05-09 01:14:01.000000 oexp-0.6.0/oexp/jbridge.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 02:37:50.245068 oexp-0.6.0/oexp.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 02:37:50.000000 oexp-0.6.0/oexp.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      224 2023-05-09 02:37:50.000000 oexp-0.6.0/oexp.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-05-09 02:37:50.000000 oexp-0.6.0/oexp.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-05-09 02:37:50.000000 oexp-0.6.0/oexp.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-05-09 02:37:50.000000 oexp-0.6.0/oexp.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-05-09 02:37:45.000000 oexp-0.6.0/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-05-09 02:37:50.245472 oexp-0.6.0/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 02:48:56.572866 oexp-0.7.0/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-12 02:48:56.572651 oexp-0.7.0/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.7.0/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 02:48:56.570859 oexp-0.7.0/oexp/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.7.0/oexp/__init__.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)    80499 2023-06-12 02:47:58.000000 oexp-0.7.0/oexp/access.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-06-12 02:47:47.000000 oexp-0.7.0/oexp/gen.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2011 2023-06-12 01:50:22.000000 oexp-0.7.0/oexp/jbridge.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 02:48:56.572281 oexp-0.7.0/oexp/util/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        0 2023-06-10 17:43:13.000000 oexp-0.7.0/oexp/util/__init__.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2291 2023-06-10 17:46:38.000000 oexp-0.7.0/oexp/util/ops.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     1612 2023-06-10 17:47:40.000000 oexp-0.7.0/oexp/util/vals.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 02:48:56.571717 oexp-0.7.0/oexp.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-12 02:48:56.000000 oexp-0.7.0/oexp.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      281 2023-06-12 02:48:56.000000 oexp-0.7.0/oexp.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-06-12 02:48:56.000000 oexp-0.7.0/oexp.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-06-12 02:48:56.000000 oexp-0.7.0/oexp.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-06-12 02:48:56.000000 oexp-0.7.0/oexp.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-06-12 02:48:51.000000 oexp-0.7.0/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-06-12 02:48:56.572916 oexp-0.7.0/setup.cfg
```

### Comparing `oexp-0.6.0/oexp/access.py` & `oexp-0.7.0/oexp/access.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     global _SAFE_PROCESS, _SAFE_THREAD
     if current_process().pid != _SAFE_PROCESS or current_thread().ident != _SAFE_THREAD:
         raise Exception(
             f"Python-Kotlin communication is currently not safe to use across multiple threads or processes. If you need this feature, please let me know."
         )
 
 
-JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/367/oexp-front-0-all.jar"
+JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/525/oexp-front-0-all.jar"
 
 
 class OexpExitSocketHeaders(Enum):
     EXIT = b"\x00"
 
 
 EXIT = b"\x00"
@@ -189,17 +189,15 @@
 class _ObjectID:
     _object_ids = {}
 
     def __init__(self, _id):
         self._id = _id
 
     def __str__(self):
-        _sendall(STR)
-        _send_long(self._id._id)
-        return _recv_string()
+        return f"_ObjectID[{self._id}]"
 
     def __repr__(self):
         return str(self)
 
 
 def _object_id(_id):
     ref = _ObjectID._object_ids.get(_id)
@@ -208,18 +206,26 @@
     else:
         obj = _ObjectID(_id)
         wref = weakref.ref(obj, lambda ref: _gc_callback(_id))
         _ObjectID._object_ids[_id] = wref
         return obj
 
 
+_PROBABLY_DISCONNECTED = False
+
+
 def _gc_callback(the_id):
-    _sendall(GC)
-    _send_long(the_id)
-    del _ObjectID._object_ids[the_id]
+    global _PROBABLY_DISCONNECTED
+    if not _PROBABLY_DISCONNECTED:
+        try:
+            _sendall(GC)
+            _send_long(the_id)
+            del _ObjectID._object_ids[the_id]
+        except OSError:
+            _PROBABLY_DISCONNECTED = True
 
 
 def _exit_server():
     _sendall(EXIT)
 
 
 # [[matt.oexp.front.api.ApiKt#login]]
@@ -233,15 +239,15 @@
     _send_string(password)
     _recv_exception_check()
     return _recv_object(OnlineExperiments, nullable=False)
 
 
 class KBClass(abc.ABC):
     def __str__(self):
-        return f"_ObjectID with id {self._id}"
+        return f"{type(self)} with id {self._id}"
 
 
 class KBVClass(KBClass, abc.ABC):
     pass
 
 
 class KBDClass(KBClass, abc.ABC):
@@ -274,20 +280,21 @@
         if API._id is None:
             jbridge._init_java()
             _sendall(INIT_OBJECT)
             _send_string("matt.oexp.front.api.API")
             API._id = _object_id(_recv_long())
 
     # [[matt.oexp.front.api.API#enableLocalMode]]
-    def enable_local_mode(self):
+    def enable_local_mode(self, port):
         _ensure_synchronized()
         API._init()
         _sendall(CALL_FUN)
         _send_long(self._id._id)
         _send_int(0)
+        _send_int(port)
         _recv_exception_check()
         return _recv_confirmation()
 
     # [[matt.oexp.front.api.API#enableStageMode]]
     def enable_stage_mode(self, token):
         _ensure_synchronized()
         API._init()
@@ -612,20 +619,42 @@
         _sendall(CALL_FUN)
         _send_long(self._id._id)
         _send_int(1)
         _send_string(name)
         _recv_exception_check()
         return _recv_object(Experiment, nullable=False)
 
+    # [[matt.oexp.front.api.OnlineExperiments#experimentWithUid]]
+    def experiment_with_uid(self, uid) -> Experiment:
+        _ensure_synchronized()
+        _sendall(CALL_FUN)
+        _send_long(self._id._id)
+        _send_int(2)
+        _send_long(uid._id._id)
+        _recv_exception_check()
+        return _recv_object(Experiment, nullable=False)
+
+    # [[matt.oexp.front.api.OnlineExperiments#listExperimentData]]
+    def list_experiment_data(self) -> List[ExperimentConfig]:
+        _ensure_synchronized()
+        _sendall(CALL_FUN)
+        _send_long(self._id._id)
+        _send_int(3)
+        _recv_exception_check()
+        return _recv_list(
+            elementReceiveFun=lambda: _recv_object(ExperimentConfig, nullable=False),
+            nullable=False,
+        )
+
     # [[matt.oexp.front.api.OnlineExperiments#listExperiments]]
     def list_experiments(self) -> List[Experiment]:
         _ensure_synchronized()
         _sendall(CALL_FUN)
         _send_long(self._id._id)
-        _send_int(2)
+        _send_int(4)
         _recv_exception_check()
         return _recv_list(
             elementReceiveFun=lambda: _recv_object(Experiment, nullable=False),
             nullable=False,
         )
 
     # [[matt.oexp.front.api.OnlineExperiments]]
@@ -741,30 +770,30 @@
         _send_long(self._id._id)
         _send_int(3)
         temp = _recv_string(nullable=False)
         return temp
 
     # [[matt.oexp.olang.lab.model.ExperimentConfig#prolificStudyID]]
     @property
-    def prolific_study_id(self) -> Optional[ProlificStudyID]:
+    def prolific_study_id(self) -> Optional[ProlificStudyId]:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(4)
-        temp = _recv_object(ProlificStudyID, nullable=True)
+        temp = _recv_object(ProlificStudyId, nullable=True)
         return temp
 
     # [[matt.oexp.olang.lab.model.ExperimentConfig#uid]]
     @property
-    def uid(self) -> ExperimentUID:
+    def uid(self) -> ExperimentUid:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(5)
-        temp = _recv_object(ExperimentUID, nullable=False)
+        temp = _recv_object(ExperimentUid, nullable=False)
         return temp
 
     # [[matt.oexp.olang.lab.model.ExperimentConfig#willProvideAManifest]]
     @property
     def will_provide_a_manifest(self) -> bool:
         _ensure_synchronized()
         _sendall(GET_VAL)
@@ -1315,15 +1344,15 @@
 
 
 # [[matt.oexp.olang.model.ExperimentEvent]]
 class ExperimentEvent(KBClass, abc.ABC):
     # [[matt.oexp.olang.model.ExperimentEvent#expUID]]
     @property
     @abc.abstractmethod
-    def exp_uid(self) -> ExperimentUID:
+    def exp_uid(self) -> ExperimentUid:
         pass
 
     # [[matt.oexp.olang.model.ExperimentEvent#pid]]
     @property
     @abc.abstractmethod
     def pid(self) -> ProlificParticipantUid:
         pass
@@ -1393,20 +1422,20 @@
             _send_long(args[4]._id._id)
             self._id = _object_id(_recv_long())
         else:
             self._id = _object_id(_id)
 
     # [[matt.oexp.olang.model.ExperimentStart#expUID]]
     @property
-    def exp_uid(self) -> ExperimentUID:
+    def exp_uid(self) -> ExperimentUid:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
-        temp = _recv_object(ExperimentUID, nullable=False)
+        temp = _recv_object(ExperimentUid, nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.ExperimentStart#pid]]
     @property
     def pid(self) -> ProlificParticipantUid:
         _ensure_synchronized()
         _sendall(GET_VAL)
@@ -1937,15 +1966,15 @@
     @abc.abstractmethod
     def trial_index(self) -> int:
         pass
 
     # [[matt.oexp.olang.model.TrialData#expUID]]
     @property
     @abc.abstractmethod
-    def exp_uid(self) -> ExperimentUID:
+    def exp_uid(self) -> ExperimentUid:
         pass
 
 
 def completion_code(code=NO_DEFAULT, code_type=NO_DEFAULT, actions=NO_DEFAULT):
     if code == NO_DEFAULT:
         raise Exception(f"there is no default value for code, so it must be defined")
     if code_type == NO_DEFAULT:
@@ -2314,20 +2343,20 @@
             ),
             nullable=False,
         )
         return temp
 
     # [[matt.oexp.olang.model.EncryptedSubjectTrialData#expUID]]
     @property
-    def exp_uid(self) -> ExperimentUID:
+    def exp_uid(self) -> ExperimentUid:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(1)
-        temp = _recv_object(ExperimentUID, nullable=False)
+        temp = _recv_object(ExperimentUid, nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.EncryptedSubjectTrialData#log]]
     @property
     def log(self) -> List[SubjectTrialEvent]:
         _ensure_synchronized()
         _sendall(GET_VAL)
@@ -2486,20 +2515,20 @@
             _send_long(args[4]._id._id)
             self._id = _object_id(_recv_long())
         else:
             self._id = _object_id(_id)
 
     # [[matt.oexp.olang.model.ExitFullScreenEvent#expUID]]
     @property
-    def exp_uid(self) -> ExperimentUID:
+    def exp_uid(self) -> ExperimentUid:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
-        temp = _recv_object(ExperimentUID, nullable=False)
+        temp = _recv_object(ExperimentUid, nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.ExitFullScreenEvent#pid]]
     @property
     def pid(self) -> ProlificParticipantUid:
         _ensure_synchronized()
         _sendall(GET_VAL)
```

