# Comparing `tmp/cmem_plugin_kafka-1.2.0rc4.tar.gz` & `tmp/cmem_plugin_kafka-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_kafka-1.2.0rc4.tar", max compression
+gzip compressed data, was "cmem_plugin_kafka-1.3.0.tar", max compression
```

## Comparing `cmem_plugin_kafka-1.2.0rc4.tar` & `cmem_plugin_kafka-1.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11334 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/LICENSE
--rw-r--r--   0        0        0     3733 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/README-public.md
--rw-r--r--   0        0        0        0 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/__init__.py
--rw-r--r--   0        0        0     4432 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/constants.py
--rw-r--r--   0        0        0    14682 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/kafka_handlers.py
--rw-r--r--   0        0        0    11743 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/utils.py
--rw-r--r--   0        0        0        0 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/workflow/__init__.py
--rw-r--r--   0        0        0    11640 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/workflow/consumer.py
--rw-r--r--   0        0        0     9739 2023-06-02 06:59:45.948679 cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/workflow/producer.py
--rw-r--r--   0        0        0     2268 2023-06-02 07:00:13.677158 cmem_plugin_kafka-1.2.0rc4/pyproject.toml
--rw-r--r--   0        0        0     4918 1970-01-01 00:00:00.000000 cmem_plugin_kafka-1.2.0rc4/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3733 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/README-public.md
+-rw-r--r--   0        0        0        0 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/__init__.py
+-rw-r--r--   0        0        0     4432 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/constants.py
+-rw-r--r--   0        0        0    14682 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/kafka_handlers.py
+-rw-r--r--   0        0        0    11743 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/utils.py
+-rw-r--r--   0        0        0        0 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/workflow/__init__.py
+-rw-r--r--   0        0        0    11640 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/workflow/consumer.py
+-rw-r--r--   0        0        0     9739 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/workflow/producer.py
+-rw-r--r--   0        0        0     2203 2023-06-12 09:30:15.957696 cmem_plugin_kafka-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 cmem_plugin_kafka-1.3.0/PKG-INFO
```

### Comparing `cmem_plugin_kafka-1.2.0rc4/LICENSE` & `cmem_plugin_kafka-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.2.0rc4/README-public.md` & `cmem_plugin_kafka-1.3.0/README-public.md`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/constants.py` & `cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/constants.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/kafka_handlers.py` & `cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/kafka_handlers.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/utils.py` & `cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/utils.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/workflow/consumer.py` & `cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/workflow/consumer.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.2.0rc4/cmem_plugin_kafka/workflow/producer.py` & `cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/workflow/producer.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.2.0rc4/pyproject.toml` & `cmem_plugin_kafka-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-kafka"
-version = "1.2.0rc4"
+version = "1.3.0"
 license = "Apache-2.0"
 description = "Send and receive messages from Apache Kafka."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -24,17 +24,14 @@
 confluent-kafka = [
     { version = "1.9.2" },
     # before you publish, comment out this next line
     # { markers = "sys_platform == 'darwin'", url = "https://files.pythonhosted.org/packages/fb/16/d04dded73439266a3dbcd585f1128483dcf509e039bacd93642ac5de97d4/confluent-kafka-1.8.2.tar.gz"}
 ]
 defusedxml = "^0.7.1"
 json-stream = "2.3.0"
-python-snappy = "^0.6.1"
-zstandard = "^0.21.0"
-lz4 = "^4.3.2"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
 black = "^23.3.0"
 coverage = "^7.2.3"
 defusedxml = "^0.7.1"
 flake8-formatter-junit-xml = "^0.0.6"
```

### Comparing `cmem_plugin_kafka-1.2.0rc4/PKG-INFO` & `cmem_plugin_kafka-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-kafka
-Version: 1.2.0rc4
+Version: 1.3.0
 Summary: Send and receive messages from Apache Kafka.
 Home-page: https://github.com/eccenca/cmem-plugin-kafka
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,kafka,kafka-producer,kafka-consumer
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Requires-Python: >=3.9,<4.0
@@ -17,17 +17,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: cmem-plugin-base (>=3.1.0,<4.0.0)
 Requires-Dist: confluent-kafka (==1.9.2)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: json-stream (==2.3.0)
-Requires-Dist: lz4 (>=4.3.2,<5.0.0)
-Requires-Dist: python-snappy (>=0.6.1,<0.7.0)
-Requires-Dist: zstandard (>=0.21.0,<0.22.0)
 Description-Content-Type: text/markdown
 
 # cmem-plugin-kafka
 
 Send and receive messages from Apache Kafka.
 
 This is a plugin for [eccenca](https://eccenca.com) [Corporate Memory](https://documentation.eccenca.com).
```

