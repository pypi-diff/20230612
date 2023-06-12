# Comparing `tmp/sensors_connectivity-1.4.1.tar.gz` & `tmp/sensors_connectivity-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensors_connectivity-1.4.1.tar", max compression
+gzip compressed data, was "sensors_connectivity-1.4.2.tar", max compression
```

## Comparing `sensors_connectivity-1.4.1.tar` & `sensors_connectivity-1.4.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1507 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/LICENSE
--rw-r--r--   0        0        0     6281 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/README.md
--rw-r--r--   0        0        0       24 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/__init__.py
--rw-r--r--   0        0        0     9099 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/config/README.md
--rw-r--r--   0        0        0       36 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/config/__init__.py
--rw-r--r--   0        0        0     1006 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/config/default.json
--rw-r--r--   0        0        0      938 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/config/logging.py
--rw-r--r--   0        0        0      824 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/config/logging_template.py
--rw-r--r--   0        0        0       94 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/constants.py
--rw-r--r--   0        0        0     5975 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/main.py
--rw-r--r--   0        0        0       51 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/drivers/__init__.py
--rw-r--r--   0        0        0      477 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/drivers/ping.py
--rw-r--r--   0        0        0     5754 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/drivers/sds011.py
--rw-r--r--   0        0        0      189 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/feeders/__init__.py
--rw-r--r--   0        0        0     9105 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/feeders/datalog_feeder.py
--rw-r--r--   0        0        0     1280 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/feeders/frontier_datalog.py
--rw-r--r--   0        0        0     1088 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/feeders/ifeeder.py
--rw-r--r--   0        0        0     3166 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/feeders/robonomics_feeder.py
--rw-r--r--   0        0        0      224 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/sensors/__init__.py
--rw-r--r--   0        0        0     1461 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/sensors/base.py
--rw-r--r--   0        0        0     2077 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/sensors/environmental_box.py
--rw-r--r--   0        0        0      643 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/sensors/lora_sensors.py
--rw-r--r--   0        0        0     1474 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/sensors/mobile_lab.py
--rw-r--r--   0        0        0     1427 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/sensors/sensor_sds011.py
--rw-r--r--   0        0        0      771 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/sensors/sensor_template.py
--rw-r--r--   0        0        0     2603 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/sensors/trackagro_sensor.py
--rw-r--r--   0        0        0      212 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/stations/__init__.py
--rw-r--r--   0        0        0     2238 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/stations/comstation.py
--rw-r--r--   0        0        0     4380 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/stations/httpstation.py
--rw-r--r--   0        0        0     1639 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/stations/istation.py
--rw-r--r--   0        0        0     4055 2023-05-21 13:08:32.864289 sensors_connectivity-1.4.1/connectivity/src/stations/mqttstation.py
--rw-r--r--   0        0        0     3089 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/connectivity/src/stations/trackargostation.py
--rw-r--r--   0        0        0       55 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/connectivity/utils/__init__.py
--rw-r--r--   0        0        0     2705 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/connectivity/utils/database.py
--rwxr-xr-x   0        0        0     3207 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/connectivity/utils/flash_firmware.py
--rwxr-xr-x   0        0        0     1825 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/connectivity/utils/generate_secrets.py
--rw-r--r--   0        0        0      391 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/connectivity/utils/get_mac.py
--rwxr-xr-x   0        0        0      553 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/connectivity/utils/py_generate_secrets.py
--rwxr-xr-x   0        0        0     2502 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/connectivity/utils/virtual-sensor.py
--rw-r--r--   0        0        0     1174 2023-05-21 13:08:32.868289 sensors_connectivity-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     7507 1970-01-01 00:00:00.000000 sensors_connectivity-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1507 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/LICENSE
+-rw-r--r--   0        0        0     6435 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/README.md
+-rw-r--r--   0        0        0       24 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/__init__.py
+-rw-r--r--   0        0        0     9099 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/config/README.md
+-rw-r--r--   0        0        0       36 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/config/__init__.py
+-rw-r--r--   0        0        0     1006 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/config/default.json
+-rw-r--r--   0        0        0      938 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/config/logging.py
+-rw-r--r--   0        0        0      824 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/config/logging_template.py
+-rw-r--r--   0        0        0       94 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/constants.py
+-rw-r--r--   0        0        0     5975 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/main.py
+-rw-r--r--   0        0        0       51 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/drivers/__init__.py
+-rw-r--r--   0        0        0      477 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/drivers/ping.py
+-rw-r--r--   0        0        0     5754 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/drivers/sds011.py
+-rw-r--r--   0        0        0      189 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/feeders/__init__.py
+-rw-r--r--   0        0        0     9105 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/feeders/datalog_feeder.py
+-rw-r--r--   0        0        0     1280 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/feeders/frontier_datalog.py
+-rw-r--r--   0        0        0     1088 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/feeders/ifeeder.py
+-rw-r--r--   0        0        0     3166 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/feeders/robonomics_feeder.py
+-rw-r--r--   0        0        0      224 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/sensors/__init__.py
+-rw-r--r--   0        0        0     1461 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/sensors/base.py
+-rw-r--r--   0        0        0     2077 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/sensors/environmental_box.py
+-rw-r--r--   0        0        0      643 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/sensors/lora_sensors.py
+-rw-r--r--   0        0        0     1474 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/sensors/mobile_lab.py
+-rw-r--r--   0        0        0     1427 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/sensors/sensor_sds011.py
+-rw-r--r--   0        0        0      771 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/sensors/sensor_template.py
+-rw-r--r--   0        0        0     2603 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/sensors/trackagro_sensor.py
+-rw-r--r--   0        0        0      212 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/stations/__init__.py
+-rw-r--r--   0        0        0     2238 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/stations/comstation.py
+-rw-r--r--   0        0        0     4380 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/stations/httpstation.py
+-rw-r--r--   0        0        0     1639 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/stations/istation.py
+-rw-r--r--   0        0        0     4055 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/stations/mqttstation.py
+-rw-r--r--   0        0        0     3089 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/src/stations/trackargostation.py
+-rw-r--r--   0        0        0       55 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/utils/__init__.py
+-rw-r--r--   0        0        0     2705 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/utils/database.py
+-rwxr-xr-x   0        0        0     3207 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/utils/flash_firmware.py
+-rwxr-xr-x   0        0        0     1825 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/utils/generate_secrets.py
+-rw-r--r--   0        0        0      391 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/utils/get_mac.py
+-rwxr-xr-x   0        0        0      553 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/utils/py_generate_secrets.py
+-rwxr-xr-x   0        0        0     2502 2023-06-12 10:48:06.671042 sensors_connectivity-1.4.2/connectivity/utils/virtual-sensor.py
+-rw-r--r--   0        0        0     1174 2023-06-12 10:48:06.675042 sensors_connectivity-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     7661 1970-01-01 00:00:00.000000 sensors_connectivity-1.4.2/PKG-INFO
```

### Comparing `sensors_connectivity-1.4.1/LICENSE` & `sensors_connectivity-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/README.md` & `sensors_connectivity-1.4.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,24 +15,26 @@
 wget https://dist.ipfs.io/go-ipfs/v0.8.0/go-ipfs_v0.8.0_linux-amd64.tar.gz
 tar -xzf go-ipfs_v0.8.0_linux-amd64.tar.gz
 cd go-ipfs
 sudo bash install.sh 
 ipfs init
 ```
 
+You need at least `Python3.10.0` to run this project.
+
 # Installation as PyPi package
 
 ```
 pip3 install py-sr25519-bindings
 pip3 install sensors-connectivity
 ```
 
 ## Configuration
 
-[Here](https://wiki.robonomics.network/docs/configuration-options-description/) you can find an article to set a proper configuration for your instance.
+[Here](https://robonomics.academy/en/learn/sensors-connectivity-course/sensors-connectivity-config-options/) you can find an article to set a proper configuration for your instance.
 
 ## Running
 
 First, launch IPFS daemon:
 
 ```
 ipfs daemon --enable-pubsub-experiment
@@ -60,19 +62,19 @@
 git clone https://github.com/airalab/sensors-connectivity
 cd sensors-connectivity
 poetry install
 ```
 
 ## Documentation
 
-To prepare a sensor for the work with the package follow instructions on [Robonomics Wiki](https://wiki.robonomics.network/docs/connect-sensor-to-robonomics/).
+To prepare a sensor for the work with the package follow instructions on [Robonomics Academy](https://robonomics.academy/en/learn/sensors-connectivity-course/setting-up-and-connecting-sensors/).
 
 ## Configuration
 
-[Here](https://wiki.robonomics.network/docs/configuration-options-description/) you can find an article to set a proper configuration for your instance.
+[Here](https://robonomics.academy/en/learn/sensors-connectivity-course/sensors-connectivity-config-options/) you can find an article to set a proper configuration for your instance.
 
 Make a copy of `default.json` and fill it using description from the article.
 
 You also can set a logging file. The default file for logs is `logging.py`, which uses `console` and `file` handler by default. Pay attention for the `file` handler. The template is stored in `connectivity/config/logging_template.py`. You can cpecify the path (`filename`), where your logs will be stored in (do not forget to create this directory if it doesn't exist). Default path for logs is `~/.logs`. You can figure any other handlers from the [library](https://docs.python.org/3.8/library/logging.html).
 
 ## Running
 
@@ -125,12 +127,12 @@
 > Note:
 python3-dev does not cover all versions for python3. The service needs at least python3.8, for that you may need to specify the version `sudo apt install python3.8-dev`.
 
 [Here](https://stackoverflow.com/a/21530768) you can find examples for other package managers.
 
 ### Python versions mismatch
 
-If during running `poetry install` comand you get `SolverProblemError`, which says "The current project's Python requirement (3.6.9) is not compatible with some of the required packages Python requirement:..", even though you have older version of python (e.g. python3.8), you may need to specify the python version poetry is using:
+If during running `poetry install` comand you get `SolverProblemError`, which says "The current project's Python requirement (3.6.9) is not compatible with some of the required packages Python requirement:..", even though you have older version of python (e.g. python3.10.9), you may need to specify the python version poetry is using:
 
 ```
-poetry env use python3.8
+poetry env use python3.10.9
 ```
```

### Comparing `sensors_connectivity-1.4.1/connectivity/config/README.md` & `sensors_connectivity-1.4.2/connectivity/config/README.md`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/config/default.json` & `sensors_connectivity-1.4.2/connectivity/config/default.json`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/config/logging.py` & `sensors_connectivity-1.4.2/connectivity/config/logging.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/config/logging_template.py` & `sensors_connectivity-1.4.2/connectivity/config/logging_template.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/main.py` & `sensors_connectivity-1.4.2/connectivity/main.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/src/drivers/sds011.py` & `sensors_connectivity-1.4.2/connectivity/src/drivers/sds011.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/src/feeders/datalog_feeder.py` & `sensors_connectivity-1.4.2/connectivity/src/feeders/datalog_feeder.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/src/feeders/frontier_datalog.py` & `sensors_connectivity-1.4.2/connectivity/src/feeders/frontier_datalog.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/src/feeders/ifeeder.py` & `sensors_connectivity-1.4.2/connectivity/src/feeders/ifeeder.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/src/feeders/robonomics_feeder.py` & `sensors_connectivity-1.4.2/connectivity/src/feeders/robonomics_feeder.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/src/sensors/base.py` & `sensors_connectivity-1.4.2/connectivity/src/sensors/base.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/src/sensors/environmental_box.py` & `sensors_connectivity-1.4.2/connectivity/src/sensors/environmental_box.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/src/sensors/lora_sensors.py` & `sensors_connectivity-1.4.2/connectivity/src/sensors/lora_sensors.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/src/sensors/mobile_lab.py` & `sensors_connectivity-1.4.2/connectivity/src/sensors/mobile_lab.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/src/sensors/sensor_sds011.py` & `sensors_connectivity-1.4.2/connectivity/src/sensors/sensor_sds011.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/src/sensors/sensor_template.py` & `sensors_connectivity-1.4.2/connectivity/src/sensors/sensor_template.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/src/sensors/trackagro_sensor.py` & `sensors_connectivity-1.4.2/connectivity/src/sensors/trackagro_sensor.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/src/stations/comstation.py` & `sensors_connectivity-1.4.2/connectivity/src/stations/comstation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/src/stations/httpstation.py` & `sensors_connectivity-1.4.2/connectivity/src/stations/httpstation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/src/stations/istation.py` & `sensors_connectivity-1.4.2/connectivity/src/stations/istation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/src/stations/mqttstation.py` & `sensors_connectivity-1.4.2/connectivity/src/stations/mqttstation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/src/stations/trackargostation.py` & `sensors_connectivity-1.4.2/connectivity/src/stations/trackargostation.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/utils/database.py` & `sensors_connectivity-1.4.2/connectivity/utils/database.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/utils/flash_firmware.py` & `sensors_connectivity-1.4.2/connectivity/utils/flash_firmware.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/utils/generate_secrets.py` & `sensors_connectivity-1.4.2/connectivity/utils/generate_secrets.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/utils/py_generate_secrets.py` & `sensors_connectivity-1.4.2/connectivity/utils/py_generate_secrets.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/connectivity/utils/virtual-sensor.py` & `sensors_connectivity-1.4.2/connectivity/utils/virtual-sensor.py`

 * *Files identical despite different names*

### Comparing `sensors_connectivity-1.4.1/pyproject.toml` & `sensors_connectivity-1.4.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sensors_connectivity"
-version = "1.4.1"
+version = "1.4.2"
 description = "Robonomics package to read data from sensors and publish to different output channels"
 authors = [
     "Vadim Manaenko <vadim.razorq@gmail.com>",
     "Mariia Bystramovich <m.bystramovich@gmail.com>",
 ]
 license = "BSD 3-Clause License"
```

### Comparing `sensors_connectivity-1.4.1/PKG-INFO` & `sensors_connectivity-1.4.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensors-connectivity
-Version: 1.4.1
+Version: 1.4.2
 Summary: Robonomics package to read data from sensors and publish to different output channels
 Home-page: https://github.com/airalab/sensors-connectivity
 License: BSD 3-Clause License
 Author: Vadim Manaenko
 Author-email: vadim.razorq@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
@@ -44,24 +44,26 @@
 wget https://dist.ipfs.io/go-ipfs/v0.8.0/go-ipfs_v0.8.0_linux-amd64.tar.gz
 tar -xzf go-ipfs_v0.8.0_linux-amd64.tar.gz
 cd go-ipfs
 sudo bash install.sh 
 ipfs init
 ```
 
+You need at least `Python3.10.0` to run this project.
+
 # Installation as PyPi package
 
 ```
 pip3 install py-sr25519-bindings
 pip3 install sensors-connectivity
 ```
 
 ## Configuration
 
-[Here](https://wiki.robonomics.network/docs/configuration-options-description/) you can find an article to set a proper configuration for your instance.
+[Here](https://robonomics.academy/en/learn/sensors-connectivity-course/sensors-connectivity-config-options/) you can find an article to set a proper configuration for your instance.
 
 ## Running
 
 First, launch IPFS daemon:
 
 ```
 ipfs daemon --enable-pubsub-experiment
@@ -89,19 +91,19 @@
 git clone https://github.com/airalab/sensors-connectivity
 cd sensors-connectivity
 poetry install
 ```
 
 ## Documentation
 
-To prepare a sensor for the work with the package follow instructions on [Robonomics Wiki](https://wiki.robonomics.network/docs/connect-sensor-to-robonomics/).
+To prepare a sensor for the work with the package follow instructions on [Robonomics Academy](https://robonomics.academy/en/learn/sensors-connectivity-course/setting-up-and-connecting-sensors/).
 
 ## Configuration
 
-[Here](https://wiki.robonomics.network/docs/configuration-options-description/) you can find an article to set a proper configuration for your instance.
+[Here](https://robonomics.academy/en/learn/sensors-connectivity-course/sensors-connectivity-config-options/) you can find an article to set a proper configuration for your instance.
 
 Make a copy of `default.json` and fill it using description from the article.
 
 You also can set a logging file. The default file for logs is `logging.py`, which uses `console` and `file` handler by default. Pay attention for the `file` handler. The template is stored in `connectivity/config/logging_template.py`. You can cpecify the path (`filename`), where your logs will be stored in (do not forget to create this directory if it doesn't exist). Default path for logs is `~/.logs`. You can figure any other handlers from the [library](https://docs.python.org/3.8/library/logging.html).
 
 ## Running
 
@@ -154,13 +156,13 @@
 > Note:
 python3-dev does not cover all versions for python3. The service needs at least python3.8, for that you may need to specify the version `sudo apt install python3.8-dev`.
 
 [Here](https://stackoverflow.com/a/21530768) you can find examples for other package managers.
 
 ### Python versions mismatch
 
-If during running `poetry install` comand you get `SolverProblemError`, which says "The current project's Python requirement (3.6.9) is not compatible with some of the required packages Python requirement:..", even though you have older version of python (e.g. python3.8), you may need to specify the python version poetry is using:
+If during running `poetry install` comand you get `SolverProblemError`, which says "The current project's Python requirement (3.6.9) is not compatible with some of the required packages Python requirement:..", even though you have older version of python (e.g. python3.10.9), you may need to specify the python version poetry is using:
 
 ```
-poetry env use python3.8
+poetry env use python3.10.9
 ```
```

