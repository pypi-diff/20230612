# Comparing `tmp/captif_cpx_config-0.5.tar.gz` & `tmp/captif_cpx_config-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_config-0.5.tar", max compression
+gzip compressed data, was "captif_cpx_config-0.6.tar", max compression
```

## Comparing `captif_cpx_config-0.5.tar` & `captif_cpx_config-0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2023-06-09 00:45:40.220634 captif_cpx_config-0.5/LICENSE
--rw-r--r--   0        0        0       19 2023-06-09 00:45:40.220634 captif_cpx_config-0.5/README.md
--rw-r--r--   0        0        0       44 2023-06-09 00:45:40.220634 captif_cpx_config-0.5/captif_cpx_config/__init__.py
--rw-r--r--   0        0        0     4112 2023-06-09 00:45:40.220634 captif_cpx_config-0.5/captif_cpx_config/metadata.py
--rw-r--r--   0        0        0      521 2023-06-09 00:45:40.220634 captif_cpx_config-0.5/pyproject.toml
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 captif_cpx_config-0.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-12 00:08:10.640101 captif_cpx_config-0.6/LICENSE
+-rw-r--r--   0        0        0       19 2023-06-12 00:08:10.644101 captif_cpx_config-0.6/README.md
+-rw-r--r--   0        0        0       44 2023-06-12 00:08:10.644101 captif_cpx_config-0.6/captif_cpx_config/__init__.py
+-rw-r--r--   0        0        0     4089 2023-06-12 00:08:10.644101 captif_cpx_config-0.6/captif_cpx_config/metadata.py
+-rw-r--r--   0        0        0      522 2023-06-12 00:08:10.644101 captif_cpx_config-0.6/pyproject.toml
+-rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 captif_cpx_config-0.6/PKG-INFO
```

### Comparing `captif_cpx_config-0.5/LICENSE` & `captif_cpx_config-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `captif_cpx_config-0.5/captif_cpx_config/metadata.py` & `captif_cpx_config-0.6/captif_cpx_config/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     )
 
 
 class DeviceCorrections(BaseModel):
     frequency_hz: list[condecimal(decimal_places=1)] = Field(
         description="list third-octave band centre frequencies in Hz",
     )
-    correction_db: list[condecimal(decimal_places=2)] = Field(
+    correction_db: list[float] = Field(
         description="list of device corrections in dB",
     )
 
 
 class WheelBayDetails(BaseModel):
     wheel_bay_name: Literal["left", "right"] = Field(
         description="wheel bay name ('left' or 'right')",
```

### Comparing `captif_cpx_config-0.5/pyproject.toml` & `captif_cpx_config-0.6/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "captif-cpx-config"
-version = "0.5"
+version = "0.6"
 description = ""
 authors = ["John Bull <john.bull@nzta.govt.nz>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "captif_cpx_config"}]
 
 [tool.poetry.dependencies]
@@ -14,12 +14,12 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 pytest-randomly = "^3.12.0"
 black = "^23.3.0"
 flake8 = "^6.0.0"
-captif-cpx-db = "^0.6"
+captif-cpx-db = ">=0.7"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `captif_cpx_config-0.5/PKG-INFO` & `captif_cpx_config-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captif-cpx-config
-Version: 0.5
+Version: 0.6
 Summary: 
 License: MIT
 Author: John Bull
 Author-email: john.bull@nzta.govt.nz
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

