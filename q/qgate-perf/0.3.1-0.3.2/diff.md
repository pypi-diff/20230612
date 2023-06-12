# Comparing `tmp/qgate_perf-0.3.1-py3-none-any.whl.zip` & `tmp/qgate_perf-0.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 17528 bytes, number of entries: 17
+Zip file size: 17650 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-29 09:53 qgate_perf/__init__.py
 -rw-rw-rw-  2.0 fat      428 b- defN 23-May-06 06:01 qgate_perf/bundle_helper.py
 -rw-rw-rw-  2.0 fat     5714 b- defN 23-May-06 17:21 qgate_perf/executor_helper.py
--rw-rw-rw-  2.0 fat     1053 b- defN 23-May-04 18:36 qgate_perf/file_format.py
--rw-rw-rw-  2.0 fat    14335 b- defN 23-Jun-06 14:21 qgate_perf/parallel_executor.py
+-rw-rw-rw-  2.0 fat     1078 b- defN 23-Jun-12 11:44 qgate_perf/file_format.py
+-rw-rw-rw-  2.0 fat    14690 b- defN 23-Jun-12 13:27 qgate_perf/parallel_executor.py
 -rw-rw-rw-  2.0 fat     5431 b- defN 23-Jun-05 18:34 qgate_perf/parallel_probe.py
 -rw-rw-rw-  2.0 fat      384 b- defN 23-May-06 12:01 qgate_perf/run_return.py
 -rw-rw-rw-  2.0 fat     1824 b- defN 23-May-30 17:30 qgate_perf/run_setup.py
--rw-rw-rw-  2.0 fat      215 b- defN 23-Jun-06 14:39 qgate_perf/version.py
+-rw-rw-rw-  2.0 fat      215 b- defN 23-Jun-12 13:27 qgate_perf/version.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-05 17:45 tests/__init__.py
 -rw-rw-rw-  2.0 fat      731 b- defN 23-May-26 14:21 tests/test_dir.py
 -rw-rw-rw-  2.0 fat     5367 b- defN 23-Jun-06 11:35 tests/test_run.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-06 14:39 qgate_perf-0.3.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6964 b- defN 23-Jun-06 14:39 qgate_perf-0.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 14:39 qgate_perf-0.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-06 14:39 qgate_perf-0.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1359 b- defN 23-Jun-06 14:39 qgate_perf-0.3.1.dist-info/RECORD
-17 files, 55512 bytes uncompressed, 15304 bytes compressed:  72.4%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-12 13:27 qgate_perf-0.3.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6964 b- defN 23-Jun-12 13:27 qgate_perf-0.3.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 13:27 qgate_perf-0.3.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-12 13:27 qgate_perf-0.3.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1359 b- defN 23-Jun-12 13:27 qgate_perf-0.3.2.dist-info/RECORD
+17 files, 55892 bytes uncompressed, 15426 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: tests/test_dir.py
 Comment: 
 
 Filename: tests/test_run.py
 Comment: 
 
-Filename: qgate_perf-0.3.1.dist-info/LICENSE
+Filename: qgate_perf-0.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: qgate_perf-0.3.1.dist-info/METADATA
+Filename: qgate_perf-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: qgate_perf-0.3.1.dist-info/WHEEL
+Filename: qgate_perf-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: qgate_perf-0.3.1.dist-info/top_level.txt
+Filename: qgate_perf-0.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: qgate_perf-0.3.1.dist-info/RECORD
+Filename: qgate_perf-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qgate_perf/file_format.py

```diff
@@ -4,14 +4,15 @@
     PRF_TYPE="type"
 
     # header
     PRF_HDR_TYPE="headr"
     PRF_HDR_LABEL="label"
     PRF_HDR_BULK="bulk"
     PRF_HDR_AVIALABLE_CPU="available_cpu"
+    PRF_HDR_HOST="host"
     PRF_HDR_NOW="now"
 
     # detail
     PRF_DETAIL_TYPE="detail"
     PRF_DETAIL_PROCESSID="processid"
     PRF_DETAIL_CALLS="calls"
     PRF_DETAIL_COUNT="count"
```

## qgate_perf/parallel_executor.py

```diff
@@ -3,14 +3,15 @@
 from multiprocessing import Process
 import multiprocessing
 import threading
 import datetime
 import time
 from concurrent.futures import ThreadPoolExecutor
 import concurrent.futures
+import socket
 import json
 from qgate_perf.file_format import FileFormat
 from qgate_perf.run_setup import RunSetup
 from qgate_perf.bundle_helper import BundleHelper
 from qgate_perf.executor_helper import ExecutorHelper
 from qgate_perf.parallel_probe import ParallelProbe
 from qgate_perf.run_return import RunReturn
@@ -110,21 +111,31 @@
         self._start_tasks = datetime.datetime.utcnow()
         self._print(file, f"############### {self._start_tasks.isoformat(' ')} ###############")
         out = {
             FileFormat.PRF_TYPE: FileFormat.PRF_HDR_TYPE,
             FileFormat.PRF_HDR_LABEL: self._label if self._label is not None else "Noname",
             FileFormat.PRF_HDR_BULK: [run_setup._bulk_row, run_setup._bulk_col],
             FileFormat.PRF_HDR_AVIALABLE_CPU: multiprocessing.cpu_count(),
+            FileFormat.PRF_HDR_HOST: self._host(),
             FileFormat.PRF_HDR_NOW: self._start_tasks.isoformat(' ')
         }
         self._print(file, json.dumps(out))
 
-    def _print_footer(self, file):
-        self._print(file,
-                    f"############### Duration: {round((datetime.datetime.utcnow() - self._start_tasks).total_seconds(), 1)} seconds ###############")
+    def _host(self):
+        """ Return information about the host in format (host_name/ip addr)"""
+        try:
+            host=socket.gethostname()
+            ip=socket.gethostbyname(host)
+        except Exception:
+            pass
+        return f"{host}/{ip}"
+
+        def _print_footer(self, file):
+            self._print(file,
+                        f"############### Duration: {round((datetime.datetime.utcnow() - self._start_tasks).total_seconds(), 1)} seconds ###############")
 
     def _print_detail(self, file, run_setup: RunSetup, return_dict, processes, threads, group=''):
         sum_time = 0
         sum_deviation = 0
         sum_call = 0
         count = 0
```

## qgate_perf/version.py

```diff
@@ -1,5 +1,5 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
-__version__ = '0.3.1'
+__version__ = '0.3.2'
```

## Comparing `qgate_perf-0.3.1.dist-info/LICENSE` & `qgate_perf-0.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qgate_perf-0.3.1.dist-info/METADATA` & `qgate_perf-0.3.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-perf
-Version: 0.3.1
+Version: 0.3.2
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
```

## Comparing `qgate_perf-0.3.1.dist-info/RECORD` & `qgate_perf-0.3.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 qgate_perf/__init__.py,sha256=1_WzwjEn3Ro-VrDe9uO1r2TbTq6YPSaErStlN5aF3_4,40
 qgate_perf/bundle_helper.py,sha256=utcDeo0unCzru68FJnl5tRBjumv56dNEg6Kdc6SHGkg,428
 qgate_perf/executor_helper.py,sha256=kGCih4ZnCgdzYcTXuhAUbPt-_hHyMzE5f7OzB6L4HVQ,5714
-qgate_perf/file_format.py,sha256=D8j13sUIXkhe0vZDVAuvEoRJEvf3RXzrTzymTIbkYWw,1053
-qgate_perf/parallel_executor.py,sha256=_FUF4yW-ibNvp__TlISJxC6eIzVHmpxCIg-F1Za2RAk,14335
+qgate_perf/file_format.py,sha256=aKJhV27opg9qsMvkDnubbE_YbOiik0ScuiUB1aabA1c,1078
+qgate_perf/parallel_executor.py,sha256=vpwiQXWutoYcsfdYQYmgM_cE8lvamlLm7t8XtEwpkEY,14690
 qgate_perf/parallel_probe.py,sha256=D1TuHfYxoZxXa1xXhXk4uyRKmNOEoUtSc0dkZ6Yqe1U,5431
 qgate_perf/run_return.py,sha256=3hFZ5cH47R1nq7_13JG2WLhwdipBCao-qDtdfeuoXx4,384
 qgate_perf/run_setup.py,sha256=hCpvZak-7VEyuDRgh_IqJx6VYcUDqTkXi1a27V8ddsI,1824
-qgate_perf/version.py,sha256=WmhG-8eUHEDazjEKAAZt47qxvCDQLCDpFi2vsMdjHDs,215
+qgate_perf/version.py,sha256=z7z_15UB_8CLJZ5ROisz05Nr6qnUBJEGZVy_LH2nuBs,215
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_dir.py,sha256=NFNu4S6gZhJ7F_wuiYfl_pAXlgx8bUbwNr6UYMKG7e8,731
 tests/test_run.py,sha256=H-F3LWXBdZr4ciSvmtDLVD4c__Ut3Dw2SLuctaklSho,5367
-qgate_perf-0.3.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-qgate_perf-0.3.1.dist-info/METADATA,sha256=2FbVf7Lt6sHjl0mTogKPGOFSORU8zQkhiQrA8p6F3Nw,6964
-qgate_perf-0.3.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-qgate_perf-0.3.1.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
-qgate_perf-0.3.1.dist-info/RECORD,,
+qgate_perf-0.3.2.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+qgate_perf-0.3.2.dist-info/METADATA,sha256=oL8CwKEzdqPoO_H9QDPP2-7UH9yIojT8ZLVwaW9L7OA,6964
+qgate_perf-0.3.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+qgate_perf-0.3.2.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
+qgate_perf-0.3.2.dist-info/RECORD,,
```

