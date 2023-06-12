# Comparing `tmp/ldfparser-0.9.0.tar.gz` & `tmp/ldfparser-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ldfparser-0.9.0.tar", last modified: Fri Jul 30 21:27:57 2021, max compression
+gzip compressed data, was "dist/ldfparser-0.9.1.tar", last modified: Sat Sep 11 07:37:34 2021, max compression
```

## Comparing `ldfparser-0.9.0.tar` & `ldfparser-0.9.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-30 21:27:57.000000 ldfparser-0.9.0/
--rw-r--r--   0 root         (0) root         (0)     1127 2021-07-30 21:27:43.000000 ldfparser-0.9.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     4744 2021-07-30 21:27:43.000000 ldfparser-0.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-30 21:27:57.000000 ldfparser-0.9.0/ldfparser.egg-info/
--rw-r--r--   0 root         (0) root         (0)       27 2021-07-30 21:27:57.000000 ldfparser-0.9.0/ldfparser.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       50 2021-07-30 21:27:57.000000 ldfparser-0.9.0/ldfparser.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       30 2021-07-30 21:27:57.000000 ldfparser-0.9.0/ldfparser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     5557 2021-07-30 21:27:57.000000 ldfparser-0.9.0/ldfparser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-30 21:27:57.000000 ldfparser-0.9.0/ldfparser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      647 2021-07-30 21:27:57.000000 ldfparser-0.9.0/ldfparser.egg-info/SOURCES.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-30 21:27:57.000000 ldfparser-0.9.0/ldfparser/
--rw-r--r--   0 root         (0) root         (0)      543 2021-07-30 21:27:43.000000 ldfparser-0.9.0/ldfparser/comment.py
--rw-r--r--   0 root         (0) root         (0)      139 2021-07-30 21:27:43.000000 ldfparser-0.9.0/ldfparser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4591 2021-07-30 21:27:43.000000 ldfparser-0.9.0/ldfparser/lin.py
--rw-r--r--   0 root         (0) root         (0)      343 2021-07-30 21:27:43.000000 ldfparser-0.9.0/ldfparser/comment.lark
--rw-r--r--   0 root         (0) root         (0)    15419 2021-07-30 21:27:43.000000 ldfparser-0.9.0/ldfparser/parser.py
--rw-r--r--   0 root         (0) root         (0)     1393 2021-07-30 21:27:43.000000 ldfparser-0.9.0/ldfparser/node.py
--rw-r--r--   0 root         (0) root         (0)     3800 2021-07-30 21:27:43.000000 ldfparser-0.9.0/ldfparser/encoding.py
--rw-r--r--   0 root         (0) root         (0)     7897 2021-07-30 21:27:43.000000 ldfparser-0.9.0/ldfparser/ldf.lark
--rw-r--r--   0 root         (0) root         (0)     5452 2021-07-30 21:27:43.000000 ldfparser-0.9.0/ldfparser/cli.py
--rw-r--r--   0 root         (0) root         (0)     1057 2021-07-30 21:27:43.000000 ldfparser-0.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5557 2021-07-30 21:27:57.000000 ldfparser-0.9.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-30 21:27:57.000000 ldfparser-0.9.0/tests/
--rw-r--r--   0 root         (0) root         (0)     6381 2021-07-30 21:27:43.000000 ldfparser-0.9.0/tests/test_encoding.py
--rw-r--r--   0 root         (0) root         (0)      448 2021-07-30 21:27:43.000000 ldfparser-0.9.0/tests/test_schema.py
--rw-r--r--   0 root         (0) root         (0)     5437 2021-07-30 21:27:43.000000 ldfparser-0.9.0/tests/test_frame.py
--rw-r--r--   0 root         (0) root         (0)      887 2021-07-30 21:27:43.000000 ldfparser-0.9.0/tests/test_signal.py
--rw-r--r--   0 root         (0) root         (0)      556 2021-07-30 21:27:43.000000 ldfparser-0.9.0/tests/snapshot_data.py
--rw-r--r--   0 root         (0) root         (0)     1818 2021-07-30 21:27:43.000000 ldfparser-0.9.0/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-30 21:27:43.000000 ldfparser-0.9.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      887 2021-07-30 21:27:43.000000 ldfparser-0.9.0/tests/test_json.py
--rw-r--r--   0 root         (0) root         (0)     1415 2021-07-30 21:27:43.000000 ldfparser-0.9.0/tests/test_performance.py
--rw-r--r--   0 root         (0) root         (0)     1230 2021-07-30 21:27:43.000000 ldfparser-0.9.0/tests/test_comment.py
--rw-r--r--   0 root         (0) root         (0)     4510 2021-07-30 21:27:43.000000 ldfparser-0.9.0/tests/test_parser.py
--rw-r--r--   0 root         (0) root         (0)       66 2021-07-30 21:27:57.000000 ldfparser-0.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-11 07:37:34.000000 ldfparser-0.9.1/
+-rw-r--r--   0 root         (0) root         (0)       66 2021-09-11 07:37:34.000000 ldfparser-0.9.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-11 07:37:34.000000 ldfparser-0.9.1/ldfparser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       50 2021-09-11 07:37:34.000000 ldfparser-0.9.1/ldfparser.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      647 2021-09-11 07:37:34.000000 ldfparser-0.9.1/ldfparser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2021-09-11 07:37:34.000000 ldfparser-0.9.1/ldfparser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     5557 2021-09-11 07:37:34.000000 ldfparser-0.9.1/ldfparser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       27 2021-09-11 07:37:34.000000 ldfparser-0.9.1/ldfparser.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-09-11 07:37:34.000000 ldfparser-0.9.1/ldfparser.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-11 07:37:34.000000 ldfparser-0.9.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     5437 2021-09-11 07:37:21.000000 ldfparser-0.9.1/tests/test_frame.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2021-09-11 07:37:21.000000 ldfparser-0.9.1/tests/test_comment.py
+-rw-r--r--   0 root         (0) root         (0)      887 2021-09-11 07:37:21.000000 ldfparser-0.9.1/tests/test_json.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2021-09-11 07:37:21.000000 ldfparser-0.9.1/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     5145 2021-09-11 07:37:21.000000 ldfparser-0.9.1/tests/test_parser.py
+-rw-r--r--   0 root         (0) root         (0)      887 2021-09-11 07:37:21.000000 ldfparser-0.9.1/tests/test_signal.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-09-11 07:37:21.000000 ldfparser-0.9.1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6381 2021-09-11 07:37:21.000000 ldfparser-0.9.1/tests/test_encoding.py
+-rw-r--r--   0 root         (0) root         (0)     1415 2021-09-11 07:37:21.000000 ldfparser-0.9.1/tests/test_performance.py
+-rw-r--r--   0 root         (0) root         (0)      448 2021-09-11 07:37:21.000000 ldfparser-0.9.1/tests/test_schema.py
+-rw-r--r--   0 root         (0) root         (0)      556 2021-09-11 07:37:21.000000 ldfparser-0.9.1/tests/snapshot_data.py
+-rw-r--r--   0 root         (0) root         (0)     5557 2021-09-11 07:37:34.000000 ldfparser-0.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1127 2021-09-11 07:37:21.000000 ldfparser-0.9.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1057 2021-09-11 07:37:21.000000 ldfparser-0.9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4744 2021-09-11 07:37:21.000000 ldfparser-0.9.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-11 07:37:34.000000 ldfparser-0.9.1/ldfparser/
+-rw-r--r--   0 root         (0) root         (0)    16160 2021-09-11 07:37:21.000000 ldfparser-0.9.1/ldfparser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     7897 2021-09-11 07:37:21.000000 ldfparser-0.9.1/ldfparser/ldf.lark
+-rw-r--r--   0 root         (0) root         (0)     5452 2021-09-11 07:37:21.000000 ldfparser-0.9.1/ldfparser/cli.py
+-rw-r--r--   0 root         (0) root         (0)      343 2021-09-11 07:37:21.000000 ldfparser-0.9.1/ldfparser/comment.lark
+-rw-r--r--   0 root         (0) root         (0)     1393 2021-09-11 07:37:21.000000 ldfparser-0.9.1/ldfparser/node.py
+-rw-r--r--   0 root         (0) root         (0)     4591 2021-09-11 07:37:21.000000 ldfparser-0.9.1/ldfparser/lin.py
+-rw-r--r--   0 root         (0) root         (0)     3800 2021-09-11 07:37:21.000000 ldfparser-0.9.1/ldfparser/encoding.py
+-rw-r--r--   0 root         (0) root         (0)      139 2021-09-11 07:37:21.000000 ldfparser-0.9.1/ldfparser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      543 2021-09-11 07:37:21.000000 ldfparser-0.9.1/ldfparser/comment.py
```

### Comparing `ldfparser-0.9.0/setup.py` & `ldfparser-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `ldfparser-0.9.0/README.md` & `ldfparser-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ldfparser-0.9.0/ldfparser.egg-info/PKG-INFO` & `ldfparser-0.9.1/ldfparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldfparser
-Version: 0.9.0
+Version: 0.9.1
 Summary: LDF Language support for Python
 Home-page: https://github.com/c4deszes/ldfparser
 Author: Balazs Eszes
 Author-email: c4deszes@gmail.com
 License: MIT
 Project-URL: Documentation, https://c4deszes.github.io/ldfparser/
 Project-URL: Source Code, https://github.com/c4deszes/ldfparser
```

### Comparing `ldfparser-0.9.0/ldfparser.egg-info/SOURCES.txt` & `ldfparser-0.9.1/ldfparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ldfparser-0.9.0/ldfparser/comment.py` & `ldfparser-0.9.1/ldfparser/comment.py`

 * *Files identical despite different names*

### Comparing `ldfparser-0.9.0/ldfparser/lin.py` & `ldfparser-0.9.1/ldfparser/lin.py`

 * *Files identical despite different names*

### Comparing `ldfparser-0.9.0/ldfparser/parser.py` & `ldfparser-0.9.1/ldfparser/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 		slave.n_as_timeout = node['N_As_timeout']
 	if node.get('N_Cr_timeout') is not None:
 		slave.n_cr_timeout = node['N_Cr_timeout']
 
 	return slave
 
 
-def _link_ldf_signals(json: dict, ldf: LDF):
+def _link_ldf_signals(json: dict, ldf: LDF):  # noqa: C901
 	for signal in _require_key(json, 'signals', 'LDF missing Signals section.'):
 		signal_obj = ldf.signal(signal['name'])
 		if signal['publisher'] == ldf.master.name:
 			ldf.master.publishes.append(signal_obj)
 			signal_obj.publisher = ldf.master
 		else:
 			slave = ldf.slave(signal['publisher'])
@@ -177,14 +177,30 @@
 		for subscriber in signal['subscribers']:
 			if subscriber != ldf.master.name:
 				slave = ldf.slave(subscriber)
 				if slave is None:
 					raise ValueError(f"Signal {signal_obj.name} references non existent node {subscriber}")
 				slave.subscribes_to.append(signal_obj)
 				signal_obj.subscribers.append(slave)
+	if ldf.protocol_version < 2.0:
+		return
+	for node in json['node_attributes']:
+		slave = ldf.slave(node['name'])
+		if node.get('response_error'):
+			slave.response_error = ldf.signal(node['response_error'])
+		if node.get('fault_state_signals'):
+			for signal in node['fault_state_signals']:
+				slave.fault_state_signals.append(ldf.signal(signal))
+		if node.get('configurable_frames'):
+			if isinstance(node['configurable_frames'], Dict):
+				for (frame, pid) in node['configurable_frames'].items():
+					slave.configurable_frames[pid] = ldf.frame(frame)
+			elif isinstance(node['configurable_frames'], List):
+				for (id, frame) in enumerate(node['configurable_frames']):
+					slave.configurable_frames[id] = ldf.frame(frame)
 
 
 def _link_ldf_frames(json: dict, ldf: LDF):
 	for frame in _require_key(json, 'frames', 'LDF missing Frames sections.'):
 		frame_obj = ldf.frame(frame['frame_id'])
 		if frame['publisher'] == ldf.master.name:
 			ldf.master.publishes_frames.append(frame_obj)
```

### Comparing `ldfparser-0.9.0/ldfparser/node.py` & `ldfparser-0.9.1/ldfparser/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 		self.product_id: LinProductId = None
 		self.response_error: LinSignal = None
 		self.fault_state_signals: List[LinSignal] = []
 		self.p2_min: float = 0.05
 		self.st_min: float = 0
 		self.n_as_timeout: float = 1
 		self.n_cr_timeout: float = 1
-		self.configurable_frames = []
+		self.configurable_frames = {}
 
 
 class LinNodeCompositionConfiguration:
 
 	def __init__(self, name: str) -> None:
 		self.name: str = name
 		self.compositions: List[LinNodeComposition] = []
```

### Comparing `ldfparser-0.9.0/ldfparser/encoding.py` & `ldfparser-0.9.1/ldfparser/encoding.py`

 * *Files identical despite different names*

### Comparing `ldfparser-0.9.0/ldfparser/ldf.lark` & `ldfparser-0.9.1/ldfparser/ldf.lark`

 * *Files identical despite different names*

### Comparing `ldfparser-0.9.0/ldfparser/cli.py` & `ldfparser-0.9.1/ldfparser/cli.py`

 * *Files identical despite different names*

### Comparing `ldfparser-0.9.0/LICENSE` & `ldfparser-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ldfparser-0.9.0/PKG-INFO` & `ldfparser-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldfparser
-Version: 0.9.0
+Version: 0.9.1
 Summary: LDF Language support for Python
 Home-page: https://github.com/c4deszes/ldfparser
 Author: Balazs Eszes
 Author-email: c4deszes@gmail.com
 License: MIT
 Project-URL: Documentation, https://c4deszes.github.io/ldfparser/
 Project-URL: Source Code, https://github.com/c4deszes/ldfparser
```

### Comparing `ldfparser-0.9.0/tests/test_encoding.py` & `ldfparser-0.9.1/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `ldfparser-0.9.0/tests/test_frame.py` & `ldfparser-0.9.1/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `ldfparser-0.9.0/tests/test_signal.py` & `ldfparser-0.9.1/tests/test_signal.py`

 * *Files identical despite different names*

### Comparing `ldfparser-0.9.0/tests/snapshot_data.py` & `ldfparser-0.9.1/tests/snapshot_data.py`

 * *Files identical despite different names*

### Comparing `ldfparser-0.9.0/tests/test_cli.py` & `ldfparser-0.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ldfparser-0.9.0/tests/test_json.py` & `ldfparser-0.9.1/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `ldfparser-0.9.0/tests/test_performance.py` & `ldfparser-0.9.1/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `ldfparser-0.9.0/tests/test_comment.py` & `ldfparser-0.9.1/tests/test_comment.py`

 * *Files identical despite different names*

### Comparing `ldfparser-0.9.0/tests/test_parser.py` & `ldfparser-0.9.1/tests/test_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -79,14 +79,26 @@
 	LSM = ldf.slave('LSM')
 	assert LSM is not None
 	assert isinstance(LSM.subscribes_to[0], LinSignal)
 	assert isinstance(LSM.publishes[0], LinSignal)
 	assert isinstance(LSM.publishes_frames[0], LinFrame)
 	assert LSM.product_id.supplier_id == 0x4A4F
 	assert LSM.product_id.function_id == 0x4841
+	assert LSM.fault_state_signals == [ldf.signal('IntTest')]
+	assert LSM.response_error == ldf.signal('LSMerror')
+	assert LSM.configurable_frames[0] == ldf.frame('Node_Status_Event')
+	assert LSM.configurable_frames[1] == ldf.frame('CEM_Frm1')
+	assert LSM.configurable_frames[2] == ldf.frame('LSM_Frm1')
+	assert LSM.configurable_frames[3] == ldf.frame('LSM_Frm2')
+
+	RSM = ldf.slave('RSM')
+	assert RSM.configurable_frames[0] == ldf.frame('Node_Status_Event')
+	assert RSM.configurable_frames[1] == ldf.frame('CEM_Frm1')
+	assert RSM.configurable_frames[2] == ldf.frame('RSM_Frm1')
+	assert RSM.configurable_frames[3] == ldf.frame('RSM_Frm2')
 
 	converter = ldf.converters['InternalLightsRequest']
 	assert converter.name == 'Dig2Bit'
 	assert isinstance(converter._converters[0], LogicalValue)
 
 
 @pytest.mark.unit
```

