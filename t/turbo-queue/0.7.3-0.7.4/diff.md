# Comparing `tmp/turbo_queue-0.7.3.tar.gz` & `tmp/turbo_queue-0.7.4.tar.gz`

## Comparing `turbo_queue-0.7.3.tar` & `turbo_queue-0.7.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/CHANGELOG.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/requirements.txt
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/docs/examples.md
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/docs/how_it_works.md
--rw-r--r--   0        0        0   412842 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/docs/monitor_queue.gif
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/docs/examples/kafka_data_pipeline/src/consumer.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/docs/examples/kafka_data_pipeline/src/main.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/docs/examples/kafka_data_pipeline/src/producer.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/docs/examples/kafka_data_pipeline/src/worker.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/src/turbo_queue/__init__.py
--rw-r--r--   0        0        0    15226 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/src/turbo_queue/_turbo_queue_kafka.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/src/turbo_queue/_turbo_queue_multi_task.py
--rw-r--r--   0        0        0    21910 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/src/turbo_queue/turbo_queue.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/LICENSE
--rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/README.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 turbo_queue-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/CHANGELOG.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/requirements.txt
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/docs/examples.md
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/docs/how_it_works.md
+-rw-r--r--   0        0        0   412842 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/docs/monitor_queue.gif
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/docs/examples/kafka_data_pipeline/src/consumer.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/docs/examples/kafka_data_pipeline/src/main.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/docs/examples/kafka_data_pipeline/src/producer.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/docs/examples/kafka_data_pipeline/src/worker.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/src/turbo_queue/__init__.py
+-rw-r--r--   0        0        0    15226 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/src/turbo_queue/_turbo_queue_kafka.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/src/turbo_queue/_turbo_queue_multi_task.py
+-rw-r--r--   0        0        0    22009 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/src/turbo_queue/turbo_queue.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/LICENSE
+-rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/README.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 turbo_queue-0.7.4/PKG-INFO
```

### Comparing `turbo_queue-0.7.3/CHANGELOG.md` & `turbo_queue-0.7.4/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
 ## [Unreleased]
 - improve logging
 - improve documentation
 - examples
 - process specific connectors
 
+## [0.7.4] - 2023-06-12
+
+### Added
+- Add method to enable batch age check task
+
 ## [0.7.3] - 2023-05-01
 
 ### Added
 - Add capability for Dequeue to properly resume after pause in process
 
 ## [0.7.2] - 2023-04-20
```

### Comparing `turbo_queue-0.7.3/docs/how_it_works.md` & `turbo_queue-0.7.4/docs/how_it_works.md`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.3/docs/monitor_queue.gif` & `turbo_queue-0.7.4/docs/monitor_queue.gif`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.3/docs/examples/kafka_data_pipeline/src/consumer.py` & `turbo_queue-0.7.4/docs/examples/kafka_data_pipeline/src/consumer.py`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.3/docs/examples/kafka_data_pipeline/src/main.py` & `turbo_queue-0.7.4/docs/examples/kafka_data_pipeline/src/main.py`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.3/docs/examples/kafka_data_pipeline/src/producer.py` & `turbo_queue-0.7.4/docs/examples/kafka_data_pipeline/src/producer.py`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.3/docs/examples/kafka_data_pipeline/src/worker.py` & `turbo_queue-0.7.4/docs/examples/kafka_data_pipeline/src/worker.py`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.3/src/turbo_queue/_turbo_queue_kafka.py` & `turbo_queue-0.7.4/src/turbo_queue/_turbo_queue_kafka.py`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.3/src/turbo_queue/_turbo_queue_multi_task.py` & `turbo_queue-0.7.4/src/turbo_queue/_turbo_queue_multi_task.py`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.3/src/turbo_queue/turbo_queue.py` & `turbo_queue-0.7.4/src/turbo_queue/turbo_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,14 +467,17 @@
     def check_time(self):
         """
         provides method to check the time the batch has been loading, and if exceeds timeout,
         roll to the next batch
         """
 
         return
+    
+    def activate_check_batch_age(self):
+        self.loop.create_task(self.check_batch_age())
 
     async def check_batch_age(self):
         await asyncio.sleep(self._max_batch_age)
         if (
             self._create_epoch + int(self._max_batch_age)
         ) < self.get_current_epoch_int():
             self._roll_next_batch()
```

### Comparing `turbo_queue-0.7.3/LICENSE` & `turbo_queue-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.3/README.md` & `turbo_queue-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.7.3/pyproject.toml` & `turbo_queue-0.7.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "turbo-queue"
-version = "0.7.3"
+version = "0.7.4"
 authors = [
   { name="Dave Waters", email="dave@1waters.com" },
 ]
 description = "A Python module to improve performance of multiprocessing queues"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `turbo_queue-0.7.3/PKG-INFO` & `turbo_queue-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo-queue
-Version: 0.7.3
+Version: 0.7.4
 Summary: A Python module to improve performance of multiprocessing queues
 Project-URL: Homepage, https://github.com/davewat/turbo-queue
 Project-URL: Bug Tracker, https://github.com/davewat/turbo-queue/issues
 Author-email: Dave Waters <dave@1waters.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

