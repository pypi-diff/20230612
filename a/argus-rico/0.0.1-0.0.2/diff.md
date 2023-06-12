# Comparing `tmp/argus-rico-0.0.1.tar.gz` & `tmp/argus-rico-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argus-rico-0.0.1.tar", max compression
+gzip compressed data, was "argus-rico-0.0.2.tar", max compression
```

## Comparing `argus-rico-0.0.1.tar` & `argus-rico-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-05-24 01:07:47.899290 argus-rico-0.0.1/LICENSE
--rw-r--r--   0        0        0      997 2023-06-08 14:37:07.980765 argus-rico-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2774 2023-06-01 16:13:51.632879 argus-rico-0.0.1/src/argus_rico/__init__.py
--rw-r--r--   0        0        0     1648 2023-06-06 21:37:20.105317 argus-rico-0.0.1/src/argus_rico/cli.py
--rw-r--r--   0        0        0      572 2023-06-05 21:00:52.783870 argus-rico-0.0.1/src/argus_rico/consumer.py
--rw-r--r--   0        0        0     2060 2023-06-01 16:11:29.554552 argus-rico-0.0.1/src/argus_rico/heartbeat.py
--rw-r--r--   0        0        0     3005 2023-06-01 16:14:33.051455 argus-rico-0.0.1/src/argus_rico/image_loader.py
--rw-r--r--   0        0        0      262 2023-06-01 16:13:33.996363 argus-rico-0.0.1/src/argus_rico/models/__init__.py
--rw-r--r--   0        0        0     8111 2023-06-05 21:00:38.471216 argus-rico-0.0.1/src/argus_rico/models/evr_image.py
--rw-r--r--   0        0        0     2740 2023-05-30 19:09:44.627119 argus-rico-0.0.1/src/argus_rico/producer.py
--rw-r--r--   0        0        0        0 2023-05-24 02:25:05.761919 argus-rico-0.0.1/src/argus_rico/py.typed
--rw-r--r--   0        0        0     2462 2023-05-30 19:02:20.465845 argus-rico-0.0.1/src/argus_rico/raw_streamer.py
--rw-r--r--   0        0        0     3597 2023-05-30 17:24:56.799724 argus-rico-0.0.1/src/argus_rico/schemas/raw_candidate.avsc
--rw-r--r--   0        0        0     1419 2023-05-30 19:45:04.544625 argus-rico-0.0.1/src/argus_rico/slack.py
--rw-r--r--   0        0        0     1300 2023-06-08 14:55:47.082269 argus-rico-0.0.1/setup.py
--rw-r--r--   0        0        0     1044 2023-06-08 14:55:47.082469 argus-rico-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-24 01:07:47.899290 argus-rico-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1287 2023-06-12 16:38:56.432646 argus-rico-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2765 2023-06-12 16:35:31.667188 argus-rico-0.0.2/src/argus_rico/__init__.py
+-rw-r--r--   0        0        0     1648 2023-06-12 16:35:31.667312 argus-rico-0.0.2/src/argus_rico/cli.py
+-rw-r--r--   0        0        0      572 2023-06-05 21:00:52.783870 argus-rico-0.0.2/src/argus_rico/consumer.py
+-rw-r--r--   0        0        0      792 2023-06-12 16:35:31.667436 argus-rico-0.0.2/src/argus_rico/efte_runner.py
+-rw-r--r--   0        0        0     2060 2023-06-12 16:35:31.667549 argus-rico-0.0.2/src/argus_rico/heartbeat.py
+-rw-r--r--   0        0        0     4505 2023-06-12 16:35:31.667685 argus-rico-0.0.2/src/argus_rico/images.py
+-rw-r--r--   0        0        0      262 2023-06-12 16:35:31.667792 argus-rico-0.0.2/src/argus_rico/models/__init__.py
+-rw-r--r--   0        0        0     8111 2023-06-12 16:35:31.667921 argus-rico-0.0.2/src/argus_rico/models/evr_image.py
+-rw-r--r--   0        0        0     2740 2023-06-12 16:35:31.668047 argus-rico-0.0.2/src/argus_rico/producer.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:35:31.668081 argus-rico-0.0.2/src/argus_rico/py.typed
+-rw-r--r--   0        0        0     2462 2023-06-12 16:35:31.668225 argus-rico-0.0.2/src/argus_rico/raw_streamer.py
+-rw-r--r--   0        0        0     3597 2023-06-12 16:35:31.668377 argus-rico-0.0.2/src/argus_rico/schemas/raw_candidate.avsc
+-rw-r--r--   0        0        0     6838 2023-06-12 16:35:31.668525 argus-rico-0.0.2/src/argus_rico/slack.py
+-rw-r--r--   0        0        0     1363 2023-06-12 16:45:57.794383 argus-rico-0.0.2/setup.py
+-rw-r--r--   0        0        0     1085 2023-06-12 16:45:57.794625 argus-rico-0.0.2/PKG-INFO
```

### Comparing `argus-rico-0.0.1/LICENSE` & `argus-rico-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.1/pyproject.toml` & `argus-rico-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 [tool.poetry]
 name = "argus-rico"
-version = "0.0.1"
+version = "0.0.2"
 description = "Transient alert generation and database interaction for Argus and Evryscope"
 authors = ["Hank Corbett"]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<4.0"
-python-dotenv = "^0.18.0"
+python = "^3.10,<3.11"
+python-dotenv = "^0.19.0"
 fastavro = "^1.4.12"
-pyarrow = "^8.0.0"
+pyarrow = ">=10.0.0"
 confluent-kafka = "^2.1.1"
 fastapi = "^0.95.2"
 rich = "^13.3.5"
 click = "^8.1.3"
 black = "^23.3.0"
 orjson = "^3.8.13"
 slack-bolt = "^1.18.0"
 blosc = "^1.11.1"
 astropy = "^5.3"
 pymongo = "^4.3.3"
 pydantic = "^1.10.8"
 geojson-pydantic = "^0.6.2"
 numpy = "^1.24.3"
 ipython = "^8.14.0"
+sanitize-filename = "^1.2.0"
+# efte = { git = "git@github.com:corbettht/efte.git", branch = "master", optional=true}
+# hera = { git = "git@github.com:argus-hdps/hera.git", branch = "main", optional=true}
+pymongoarrow = "^0.7.0"
+
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
 mypy = "^0.931"
 isort = "^5.10.1"
 flake8 = "^4.0.1"
 Sphinx = "^7.0.1"
 pre-commit = "^3.3.2"
 
+[tool.poetry.extras]
+# efte = ["efte"]
+# hera = ["hera"]
+
 
 [tool.poetry.scripts]
 rico = "rico.cli:main"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
```

### Comparing `argus-rico-0.0.1/src/argus_rico/__init__.py` & `argus-rico-0.0.2/src/argus_rico/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Evryscope-Argus Transient Reporter."""
 
 __author__ = """Hank Corbett"""
 __email__ = "htc@unc.edu"
-__version__ = "0.1.0"
+__version__ = "0.0.2"
 
 __all__ = ["RicoHeartBeat", "RawStreamer", "EVRImageLoader"]
 
 import logging
 import os
 
 from dotenv import load_dotenv
@@ -28,15 +28,15 @@
 
     SLACK_SIGNING_SECRET = os.environ.get("SLACK_SIGNING_SECRET") or None
     SLACK_BOT_TOKEN = os.environ.get("SLACK_BOT_TOKEN") or None
     SLACK_PORT = os.environ.get("SLACK_PORT") or 3000
 
     LOCAL_ADDR = os.environ.get("LOCAL_ADDR") or "127.0.0.1"
 
-    KAFKA_ADDR = os.environ.get("KAFKA_ADDR") or "152.2.38.172"
+    KAFKA_ADDR = os.environ.get("KAFKA_ADDR") or "127.0.0.1"
     KAFKA_PORT = os.environ.get("KAFKA_PORT") or "9092"
     HBEAT_TOPIC = os.environ.get("HBEAT_TOPIC") or "rico.heartbeat"
     RAW_TOPIC_BASE = os.environ.get("RAW_TOPIC_BASE") or "rico.candidates.raw"
     EVR_IMAGE_TOPIC = os.environ.get("RAW_TOPIC_BASE") or "rico.images.evr"
 
     MONGODB_URI = os.environ.get("MONGODB_URI") or None
     MONGO_DBNAME = os.environ.get("MONGO_DBNAME") or "hdps"
@@ -74,9 +74,9 @@
 get_logger(__name__).addHandler(logging.StreamHandler())
 
 # Silenced
 # get_logger(__name__).addHandler(logging.NullHandler())
 
 
 from .heartbeat import RicoHeartBeat  # noqa: E402
-from .image_loader import EVRImageLoader  # noqa: E402
+from .images import EVRImageLoader  # noqa: E402
 from .raw_streamer import RawStreamer  # noqa: E402
```

### Comparing `argus-rico-0.0.1/src/argus_rico/cli.py` & `argus-rico-0.0.2/src/argus_rico/cli.py`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.1/src/argus_rico/consumer.py` & `argus-rico-0.0.2/src/argus_rico/consumer.py`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.1/src/argus_rico/heartbeat.py` & `argus-rico-0.0.2/src/argus_rico/heartbeat.py`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.1/src/argus_rico/models/evr_image.py` & `argus-rico-0.0.2/src/argus_rico/models/evr_image.py`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.1/src/argus_rico/producer.py` & `argus-rico-0.0.2/src/argus_rico/producer.py`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.1/src/argus_rico/raw_streamer.py` & `argus-rico-0.0.2/src/argus_rico/raw_streamer.py`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.1/src/argus_rico/schemas/raw_candidate.avsc` & `argus-rico-0.0.2/src/argus_rico/schemas/raw_candidate.avsc`

 * *Files identical despite different names*

### Comparing `argus-rico-0.0.1/setup.py` & `argus-rico-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,37 +18,39 @@
  'confluent-kafka>=2.1.1,<3.0.0',
  'fastapi>=0.95.2,<0.96.0',
  'fastavro>=1.4.12,<2.0.0',
  'geojson-pydantic>=0.6.2,<0.7.0',
  'ipython>=8.14.0,<9.0.0',
  'numpy>=1.24.3,<2.0.0',
  'orjson>=3.8.13,<4.0.0',
- 'pyarrow>=8.0.0,<9.0.0',
+ 'pyarrow>=10.0.0',
  'pydantic>=1.10.8,<2.0.0',
  'pymongo>=4.3.3,<5.0.0',
- 'python-dotenv>=0.18.0,<0.19.0',
+ 'pymongoarrow>=0.7.0,<0.8.0',
+ 'python-dotenv>=0.19.0,<0.20.0',
  'rich>=13.3.5,<14.0.0',
+ 'sanitize-filename>=1.2.0,<2.0.0',
  'slack-bolt>=1.18.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['rico = rico.cli:main']}
 
 setup_kwargs = {
     'name': 'argus-rico',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Transient alert generation and database interaction for Argus and Evryscope',
     'long_description': None,
     'author': 'Hank Corbett',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.10,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `argus-rico-0.0.1/PKG-INFO` & `argus-rico-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: argus-rico
-Version: 0.0.1
+Version: 0.0.2
 Summary: Transient alert generation and database interaction for Argus and Evryscope
 Author: Hank Corbett
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: astropy (>=5.3,<6.0)
 Requires-Dist: black (>=23.3.0,<24.0.0)
 Requires-Dist: blosc (>=1.11.1,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: confluent-kafka (>=2.1.1,<3.0.0)
 Requires-Dist: fastapi (>=0.95.2,<0.96.0)
 Requires-Dist: fastavro (>=1.4.12,<2.0.0)
 Requires-Dist: geojson-pydantic (>=0.6.2,<0.7.0)
 Requires-Dist: ipython (>=8.14.0,<9.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: orjson (>=3.8.13,<4.0.0)
-Requires-Dist: pyarrow (>=8.0.0,<9.0.0)
+Requires-Dist: pyarrow (>=10.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
-Requires-Dist: python-dotenv (>=0.18.0,<0.19.0)
+Requires-Dist: pymongoarrow (>=0.7.0,<0.8.0)
+Requires-Dist: python-dotenv (>=0.19.0,<0.20.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
+Requires-Dist: sanitize-filename (>=1.2.0,<2.0.0)
 Requires-Dist: slack-bolt (>=1.18.0,<2.0.0)
```

