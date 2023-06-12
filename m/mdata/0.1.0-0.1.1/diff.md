# Comparing `tmp/mdata-0.1.0.tar.gz` & `tmp/mdata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdata-0.1.0.tar", max compression
+gzip compressed data, was "mdata-0.1.1.tar", max compression
```

## Comparing `mdata-0.1.0.tar` & `mdata-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,57 @@
--rw-r--r--   0        0        0      710 2023-05-03 10:03:16.066169 mdata-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      245 2023-04-24 14:51:54.968086 mdata-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-24 08:17:06.548381 mdata-0.1.0/src/mdata/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 09:02:31.524432 mdata-0.1.0/src/mdata/conversions/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 09:02:40.138181 mdata-0.1.0/src/mdata/conversions/ocel/__init__.py
--rw-r--r--   0        0        0      136 2023-05-03 09:08:07.317496 mdata-0.1.0/src/mdata/conversions/ocel/ocel_export.py
--rw-r--r--   0        0        0       39 2023-04-24 13:25:09.331919 mdata-0.1.0/src/mdata/core/__init__.py
--rw-r--r--   0        0        0      201 2023-04-24 13:25:10.017148 mdata-0.1.0/src/mdata/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      928 2023-05-02 08:49:05.625504 mdata-0.1.0/src/mdata/core/__pycache__/df_utils.cpython-310.pyc
--rw-r--r--   0        0        0    16246 2023-05-02 08:49:05.625504 mdata-0.1.0/src/mdata/core/__pycache__/machine_data_def.cpython-310.pyc
--rw-r--r--   0        0        0     4015 2023-04-24 12:44:59.436143 mdata-0.1.0/src/mdata/core/__pycache__/raw.cpython-310.pyc
--rw-r--r--   0        0        0      427 2023-05-02 08:49:05.536425 mdata-0.1.0/src/mdata/core/df_utils.py
--rw-r--r--   0        0        0        0 2023-04-24 11:51:58.667588 mdata-0.1.0/src/mdata/core/extensions/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 11:52:16.779473 mdata-0.1.0/src/mdata/core/extensions/multiplicity.py
--rw-r--r--   0        0        0       33 2023-04-25 10:08:45.579433 mdata-0.1.0/src/mdata/core/joining.py
--rw-r--r--   0        0        0    13977 2023-05-02 08:49:05.552144 mdata-0.1.0/src/mdata/core/machine_data_def.py
--rw-r--r--   0        0        0     4522 2023-04-24 12:44:58.719703 mdata-0.1.0/src/mdata/core/raw.py
--rw-r--r--   0        0        0        0 2023-04-24 08:17:06.533690 mdata-0.1.0/src/mdata/file_formats/__init__.py
--rw-r--r--   0        0        0      163 2023-04-24 08:17:21.637608 mdata-0.1.0/src/mdata/file_formats/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1428 2023-05-03 09:17:02.880910 mdata-0.1.0/src/mdata/file_formats/__pycache__/io_utils.cpython-310.pyc
--rw-r--r--   0        0        0     2353 2023-05-03 09:17:02.880910 mdata-0.1.0/src/mdata/file_formats/__pycache__/validity_checking_utils.cpython-310.pyc
--rw-r--r--   0        0        0      229 2023-05-03 09:08:07.301921 mdata-0.1.0/src/mdata/file_formats/csv/__init__.py
--rw-r--r--   0        0        0      373 2023-05-03 09:17:02.852997 mdata-0.1.0/src/mdata/file_formats/csv/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2738 2023-05-03 09:17:02.868645 mdata-0.1.0/src/mdata/file_formats/csv/__pycache__/checking.cpython-310.pyc
--rw-r--r--   0        0        0     1680 2023-05-03 09:17:02.880910 mdata-0.1.0/src/mdata/file_formats/csv/__pycache__/exporting.cpython-310.pyc
--rw-r--r--   0        0        0     2033 2023-05-03 09:25:39.745733 mdata-0.1.0/src/mdata/file_formats/csv/__pycache__/importing.cpython-310.pyc
--rw-r--r--   0        0        0      403 2023-05-03 08:54:22.483484 mdata-0.1.0/src/mdata/file_formats/csv/__pycache__/shared.cpython-310.pyc
--rw-r--r--   0        0        0     2231 2023-05-03 09:08:07.291230 mdata-0.1.0/src/mdata/file_formats/csv/checking.py
--rw-r--r--   0        0        0     1368 2023-05-03 09:08:07.285328 mdata-0.1.0/src/mdata/file_formats/csv/exporting.py
--rw-r--r--   0        0        0     2120 2023-05-03 09:23:24.697178 mdata-0.1.0/src/mdata/file_formats/csv/importing.py
--rw-r--r--   0        0        0      164 2023-05-03 08:54:22.395411 mdata-0.1.0/src/mdata/file_formats/csv/shared.py
--rw-r--r--   0        0        0      145 2023-04-27 12:35:27.078537 mdata-0.1.0/src/mdata/file_formats/hdf/__init__.py
--rw-r--r--   0        0        0      276 2023-04-27 12:35:59.963859 mdata-0.1.0/src/mdata/file_formats/hdf/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1210 2023-05-02 14:57:01.339712 mdata-0.1.0/src/mdata/file_formats/hdf/__pycache__/exporting.cpython-310.pyc
--rw-r--r--   0        0        0     1128 2023-04-28 08:17:45.922546 mdata-0.1.0/src/mdata/file_formats/hdf/__pycache__/importing.cpython-310.pyc
--rw-r--r--   0        0        0      190 2023-04-21 14:16:55.019498 mdata-0.1.0/src/mdata/file_formats/hdf/checking.py
--rw-r--r--   0        0        0     1357 2023-05-02 14:35:35.521662 mdata-0.1.0/src/mdata/file_formats/hdf/exporting.py
--rw-r--r--   0        0        0     1352 2023-04-27 13:23:32.829096 mdata-0.1.0/src/mdata/file_formats/hdf/importing.py
--rw-r--r--   0        0        0     1199 2023-05-03 09:08:07.280125 mdata-0.1.0/src/mdata/file_formats/io_utils.py
--rw-r--r--   0        0        0     1912 2023-05-03 09:08:07.309089 mdata-0.1.0/src/mdata/file_formats/validity_checking_utils.py
--rw-r--r--   0        0        0        0 2023-04-24 13:23:03.881748 mdata-0.1.0/src/mdata/visualization/__init__.py
--rw-r--r--   0        0        0      164 2023-04-25 11:27:37.791876 mdata-0.1.0/src/mdata/visualization/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3289 2023-05-02 14:34:17.149336 mdata-0.1.0/src/mdata/visualization/__pycache__/plotting.cpython-310.pyc
--rw-r--r--   0        0        0     3275 2023-05-03 09:36:30.632424 mdata-0.1.0/src/mdata/visualization/plotting.py
--rw-r--r--   0        0        0      269 2023-04-24 13:27:36.152567 mdata-0.1.0/src/mdata/visualization/textual.py
--rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 mdata-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      748 2023-06-12 10:06:57.700377 mdata-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      335 2023-05-24 11:21:39.824410 mdata-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 08:17:06.548381 mdata-0.1.1/src/mdata/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 14:47:33.159982 mdata-0.1.1/src/mdata/analysis/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-19 08:45:38.105261 mdata-0.1.1/src/mdata/analysis/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      983 2023-05-19 08:57:03.979460 mdata-0.1.1/src/mdata/analysis/__pycache__/frequency.cpython-310.pyc
+-rw-r--r--   0        0        0      811 2023-05-19 08:57:03.895576 mdata-0.1.1/src/mdata/analysis/frequency.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:02:31.524432 mdata-0.1.1/src/mdata/conversions/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:02:40.138181 mdata-0.1.1/src/mdata/conversions/ocel/__init__.py
+-rw-r--r--   0        0        0      628 2023-05-15 11:42:34.414564 mdata-0.1.1/src/mdata/conversions/ocel/ocel_export.py
+-rw-r--r--   0        0        0       93 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/core/__init__.py
+-rw-r--r--   0        0        0      269 2023-06-06 12:51:51.634919 mdata-0.1.1/src/mdata/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      928 2023-05-02 08:49:05.625504 mdata-0.1.1/src/mdata/core/__pycache__/df_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2528 2023-06-09 07:53:36.177943 mdata-0.1.1/src/mdata/core/__pycache__/factory.cpython-310.pyc
+-rw-r--r--   0        0        0    25359 2023-06-09 09:11:52.707247 mdata-0.1.1/src/mdata/core/__pycache__/machine_data_def.cpython-310.pyc
+-rw-r--r--   0        0        0     4554 2023-06-09 07:53:36.194313 mdata-0.1.1/src/mdata/core/__pycache__/raw.cpython-310.pyc
+-rw-r--r--   0        0        0     2275 2023-06-06 14:36:56.531531 mdata-0.1.1/src/mdata/core/__pycache__/util.cpython-310.pyc
+-rw-r--r--   0        0        0      427 2023-05-02 08:49:05.536425 mdata-0.1.1/src/mdata/core/df_utils.py
+-rw-r--r--   0        0        0        0 2023-04-24 11:51:58.667588 mdata-0.1.1/src/mdata/core/extensions/__init__.py
+-rw-r--r--   0        0        0      166 2023-05-25 08:35:08.557253 mdata-0.1.1/src/mdata/core/extensions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7266 2023-06-09 08:03:27.599571 mdata-0.1.1/src/mdata/core/extensions/__pycache__/multiplicity.cpython-310.pyc
+-rw-r--r--   0        0        0     5949 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/core/extensions/multiplicity.py
+-rw-r--r--   0        0        0     2555 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/core/factory.py
+-rw-r--r--   0        0        0    23958 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/core/machine_data_def.py
+-rw-r--r--   0        0        0     5913 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/core/raw.py
+-rw-r--r--   0        0        0     2034 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/core/util.py
+-rw-r--r--   0        0        0      197 2023-05-17 08:59:22.605542 mdata-0.1.1/src/mdata/file_formats/__init__.py
+-rw-r--r--   0        0        0      423 2023-05-17 09:17:42.509792 mdata-0.1.1/src/mdata/file_formats/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2121 2023-05-26 09:19:56.195531 mdata-0.1.1/src/mdata/file_formats/__pycache__/io_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2598 2023-05-04 13:47:40.526847 mdata-0.1.1/src/mdata/file_formats/__pycache__/validity_checking_utils.cpython-310.pyc
+-rw-r--r--   0        0        0      265 2023-05-04 14:37:13.900246 mdata-0.1.1/src/mdata/file_formats/csv/__init__.py
+-rw-r--r--   0        0        0      427 2023-05-04 14:37:18.586529 mdata-0.1.1/src/mdata/file_formats/csv/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3118 2023-06-09 07:53:36.166471 mdata-0.1.1/src/mdata/file_formats/csv/__pycache__/checking.cpython-310.pyc
+-rw-r--r--   0        0        0     2403 2023-05-11 09:07:39.679690 mdata-0.1.1/src/mdata/file_formats/csv/__pycache__/exporting.cpython-310.pyc
+-rw-r--r--   0        0        0     2672 2023-06-09 07:53:36.194313 mdata-0.1.1/src/mdata/file_formats/csv/__pycache__/importing.cpython-310.pyc
+-rw-r--r--   0        0        0      403 2023-05-03 08:54:22.483484 mdata-0.1.1/src/mdata/file_formats/csv/__pycache__/shared.cpython-310.pyc
+-rw-r--r--   0        0        0     3155 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/file_formats/csv/checking.py
+-rw-r--r--   0        0        0     2317 2023-05-11 09:02:15.344654 mdata-0.1.1/src/mdata/file_formats/csv/exporting.py
+-rw-r--r--   0        0        0     3141 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/file_formats/csv/importing.py
+-rw-r--r--   0        0        0      164 2023-05-03 08:54:22.395411 mdata-0.1.1/src/mdata/file_formats/csv/shared.py
+-rw-r--r--   0        0        0      145 2023-04-27 12:35:27.078537 mdata-0.1.1/src/mdata/file_formats/hdf/__init__.py
+-rw-r--r--   0        0        0      276 2023-04-27 12:35:59.963859 mdata-0.1.1/src/mdata/file_formats/hdf/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1392 2023-06-09 10:14:18.666516 mdata-0.1.1/src/mdata/file_formats/hdf/__pycache__/exporting.cpython-310.pyc
+-rw-r--r--   0        0        0     1079 2023-06-09 07:53:36.194313 mdata-0.1.1/src/mdata/file_formats/hdf/__pycache__/importing.cpython-310.pyc
+-rw-r--r--   0        0        0      190 2023-04-21 14:16:55.019498 mdata-0.1.1/src/mdata/file_formats/hdf/checking.py
+-rw-r--r--   0        0        0     1236 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/file_formats/hdf/exporting.py
+-rw-r--r--   0        0        0     1303 2023-06-12 10:06:09.238462 mdata-0.1.1/src/mdata/file_formats/hdf/importing.py
+-rw-r--r--   0        0        0     2183 2023-06-12 10:06:09.254151 mdata-0.1.1/src/mdata/file_formats/io_utils.py
+-rw-r--r--   0        0        0     1953 2023-05-04 13:47:40.474562 mdata-0.1.1/src/mdata/file_formats/validity_checking_utils.py
+-rw-r--r--   0        0        0      155 2023-05-22 11:21:08.266604 mdata-0.1.1/src/mdata/visualization/__init__.py
+-rw-r--r--   0        0        0      355 2023-05-22 11:21:08.475981 mdata-0.1.1/src/mdata/visualization/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1387 2023-06-06 12:53:23.808361 mdata-0.1.1/src/mdata/visualization/__pycache__/matplot.cpython-310.pyc
+-rw-r--r--   0        0        0     6654 2023-06-09 10:23:17.455905 mdata-0.1.1/src/mdata/visualization/__pycache__/plotting.cpython-310.pyc
+-rw-r--r--   0        0        0     1102 2023-06-12 10:06:09.254151 mdata-0.1.1/src/mdata/visualization/matplot.py
+-rw-r--r--   0        0        0     7745 2023-06-12 10:06:09.254151 mdata-0.1.1/src/mdata/visualization/plotting.py
+-rw-r--r--   0        0        0      269 2023-04-24 13:27:36.152567 mdata-0.1.1/src/mdata/visualization/textual.py
+-rw-r--r--   0        0        0     1165 1970-01-01 00:00:00.000000 mdata-0.1.1/PKG-INFO
```

### Comparing `mdata-0.1.0/pyproject.toml` & `mdata-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [tool.poetry]
 name = "mdata"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Leah Tacke genannt Unterberg <leah.tgu@pads.rwth-aachen.de>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["data format", "machine data"]
 exclude = ["files/", "test/"]
 
 [tool.poetry.dependencies]
+pandas = {version = "^1.5"} # after v2.0, extras = ["all"]
 python = "^3.9"
-pandas = { version = "^1.5", extras = ["performance", "all"] }
 jupyter = "^1.0"
 matplotlib = "^3.7.1"
-bokeh = "^2.4.3"
-plotly = "^5.14.1"
-tables = "^3.8.0"
+seaborn = "*"
+plotly = "^5.15"
 tsdownsample = "^0.1.2"
-pm4py = "^2.7.3"
+#pm4py = "^2.7.4"
+tables = "^3.8.0"
+numba = "*"
+numexpr = "*"
+bottleneck = "*"
 
 [[tool.poetry.source]]
 name = "testpypi"
 url = "https://test.pypi.org/"
 default = false
 secondary = true
```

### Comparing `mdata-0.1.0/src/mdata/core/__pycache__/df_utils.cpython-310.pyc` & `mdata-0.1.1/src/mdata/core/__pycache__/df_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mdata-0.1.0/src/mdata/core/__pycache__/raw.cpython-310.pyc` & `mdata-0.1.1/src/mdata/core/__pycache__/raw.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 24 12:44:58 2023 UTC, .py size: 4522 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,251 +1,285 @@
-00000000: 6f0d 0d0a 0000 0000 ca79 4664 aa11 0000  o........yFd....
+00000000: 6f0d 0d0a 0000 0000 59da 8264 1917 0000  o.......Y..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0173 e200 0000 6400  .....@...s....d.
+00000020: 0008 0000 0040 0000 0173 f400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 5a03 6403 6404 6c04 6d05 5a05 0100 6403  Z.d.d.l.m.Z...d.
-00000050: 6405 6c06 6d07 5a07 6d08 5a08 6d09 5a09  d.l.m.Z.m.Z.m.Z.
+00000040: 5a03 6400 6402 6c04 5a05 6403 6404 6c06  Z.d.d.l.Z.d.d.l.
+00000050: 6d07 5a07 0100 6403 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
-00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 0100 6507  m.Z.m.Z.m.Z...e.
-00000080: 6a11 6406 6507 6a12 6407 6507 6a13 6408  j.d.e.j.d.e.j.d.
-00000090: 6507 6a14 6409 6904 5a15 6516 6517 6515  e.j.d.i.Z.e.e.e.
-000000a0: 6a18 6507 8302 8301 5a19 6510 6a1a 640a  j.e.....Z.e.j.d.
-000000b0: 6510 6a1b 640b 6902 5a1c 651d 6517 651c  e.j.d.i.Z.e.e.e.
-000000c0: 6a18 6510 8302 8301 5a1e 640c 640d 8400  j.e.....Z.d.d...
-000000d0: 5a1f 6520 6509 650a 6602 1900 5a21 6503  Z.e e.e.f...Z!e.
-000000e0: 6a22 5a23 641f 6412 6413 8404 5a24 6420  j"Z#d.d.d...Z$d 
-000000f0: 6415 6416 8404 5a25 6421 6419 641a 8404  d.d...Z%d!d.d...
-00000100: 5a26 6422 641d 641e 8404 5a27 6402 5300  Z&d"d.d...Z'd.S.
-00000110: 2923 e900 0000 0029 01da 0b61 6e6e 6f74  )#.....)...annot
-00000120: 6174 696f 6e73 4ee9 0100 0000 2901 da13  ationsN.....)...
-00000130: 6465 7269 7665 5f63 6174 6567 6f72 6963  derive_categoric
-00000140: 616c 7329 0ada 0a4d 4443 6f6e 6365 7074  als)...MDConcept
-00000150: 73da 1962 6173 655f 6d61 6368 696e 655f  s..base_machine_
-00000160: 6461 7461 5f63 6f6c 756d 6e73 da11 5469  data_columns..Ti
-00000170: 6d65 7365 7269 6573 5479 7065 4b65 79da  meseriesTypeKey.
-00000180: 1754 696d 6573 6572 6965 7346 6561 7475  .TimeseriesFeatu
-00000190: 7265 4c61 6265 6c73 da06 4865 6164 6572  reLabels..Header
-000001a0: da19 4576 656e 7454 696d 6573 6572 6965  ..EventTimeserie
-000001b0: 7343 6f6c 6c65 6374 696f 6eda 1f4d 6561  sCollection..Mea
-000001c0: 7375 7265 6d65 6e74 5469 6d65 7365 7269  surementTimeseri
-000001d0: 6573 436f 6c6c 6563 7469 6f6e da0b 4d61  esCollection..Ma
-000001e0: 6368 696e 6544 6174 61da 1b54 696d 6573  chineData..Times
-000001f0: 6572 6965 7343 6f6c 6c65 6374 696f 6e46  eriesCollectionF
-00000200: 6163 746f 7279 da0f 4d61 6368 696e 6544  actory..MachineD
-00000210: 6174 6154 7970 65da 0474 696d 65da 066f  ataType..time..o
-00000220: 626a 6563 74da 0474 7970 65da 056c 6162  bject..type..lab
-00000230: 656c da01 45da 014d 6301 0000 0000 0000  el..E..Mc.......
-00000240: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
-00000250: 0173 1800 0000 6401 6402 8400 7400 6403  .s....d.d...t.d.
-00000260: 7c00 6403 1700 8302 4400 8301 5300 2904  |.d.....D...S.).
-00000270: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
-00000280: 0000 0400 0000 5300 0001 7316 0000 0067  ......S...s....g
-00000290: 007c 005d 077d 0164 007c 019b 009d 0291  .|.].}.d.|......
-000002a0: 0271 0253 0029 015a 0266 5fa9 0029 02da  .q.S.).Z.f_..)..
-000002b0: 022e 30da 0169 7215 0000 0072 1500 0000  ..0..ir....r....
-000002c0: fa39 433a 5c55 7365 7273 5c4c 6561 685c  .9C:\Users\Leah\
-000002d0: 5079 6368 6172 6d50 726f 6a65 6374 735c  PycharmProjects\
-000002e0: 6d64 6174 615c 7372 635c 6d64 6174 615c  mdata\src\mdata\
-000002f0: 636f 7265 5c72 6177 2e70 79da 0a3c 6c69  core\raw.py..<li
-00000300: 7374 636f 6d70 3e1b 0000 00f3 0200 0000  stcomp>.........
-00000310: 1600 7a2c 6765 6e5f 6665 6174 7572 655f  ..z,gen_feature_
-00000320: 636f 6c75 6d6e 5f6e 616d 6573 2e3c 6c6f  column_names.<lo
-00000330: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00000340: 7203 0000 0029 01da 0572 616e 6765 2901  r....)...range).
-00000350: da01 6e72 1500 0000 7215 0000 0072 1800  ..nr....r....r..
-00000360: 0000 da18 6765 6e5f 6665 6174 7572 655f  ....gen_feature_
-00000370: 636f 6c75 6d6e 5f6e 616d 6573 1a00 0000  column_names....
-00000380: 7302 0000 0018 0172 1d00 0000 da02 6d64  s......r......md
-00000390: 720c 0000 00da 0672 6574 7572 6eda 0d52  r......return..R
-000003a0: 6177 4865 6164 6572 5479 7065 6301 0000  awHeaderTypec...
-000003b0: 0000 0000 0000 0000 0004 0000 0005 0000  ................
-000003c0: 0043 0000 0173 2e00 0000 6900 7d01 7c00  .C...s....i.}.|.
-000003d0: a000 a100 4400 5d0e 7d02 7c02 6a01 7d03  ....D.].}.|.j.}.
-000003e0: 7402 7c03 6a03 8301 7c01 7c03 a004 a100  t.|.j...|.|.....
-000003f0: 3c00 7106 7c01 5300 a901 4e29 05da 1369  <.q.|.S...N)...i
-00000400: 7465 725f 616c 6c5f 7469 6d65 7365 7269  ter_all_timeseri
-00000410: 6573 da0f 7469 6d65 7365 7269 6573 5f74  es..timeseries_t
-00000420: 7970 65da 0574 7570 6c65 da08 6665 6174  ype..tuple..feat
-00000430: 7572 6573 5a05 6173 6b65 7929 0472 1e00  uresZ.askey).r..
-00000440: 0000 da06 6865 6164 6572 da10 7479 7065  ....header..type
-00000450: 645f 7469 6d65 7365 7269 6573 da02 7474  d_timeseries..tt
-00000460: 7215 0000 0072 1500 0000 7218 0000 00da  r....r....r.....
-00000470: 1563 6f6e 7665 7274 5f74 6f5f 7261 775f  .convert_to_raw_
-00000480: 6865 6164 6572 2300 0000 730a 0000 0004  header#...s.....
-00000490: 010c 0106 0114 0104 0172 2900 0000 da0b  .........r).....
-000004a0: 5261 7744 6174 6154 7970 6563 0100 0000  RawDataTypec....
-000004b0: 0000 0000 0000 0000 0600 0000 0900 0000  ................
-000004c0: 0300 0001 73be 0000 0074 0074 0164 0164  ....s....t.t.d.d
-000004d0: 0284 007c 00a0 02a1 0083 0283 017d 0167  ...|.........}.g
-000004e0: 007d 027c 00a0 02a1 0044 005d 357d 037c  .}.|.....D.]5}.|
-000004f0: 036a 037d 047c 036a 0489 0088 006a 0564  .j.}.|.j.....j.d
-00000500: 0364 048d 0144 005d 2689 017c 02a0 0674  .d...D.]&..|...t
-00000510: 0788 0174 086a 09a0 0aa1 0083 0274 0788  ...t.j.......t..
-00000520: 0174 086a 0ba0 0aa1 0083 027c 046a 0ca0  .t.j.......|.j..
-00000530: 0aa1 007c 046a 0d67 0487 0087 0166 0264  ...|.j.g.....f.d
-00000540: 0564 0684 087c 046a 0e44 0083 0117 00a1  .d...|.j.D......
-00000550: 0101 0071 1f71 1174 0f6a 107c 0274 1174  ...q.q.t.j.|.t.t
-00000560: 127c 0183 0117 0064 0764 088d 037d 057c  .|.....d.d...}.|
-00000570: 056a 1374 1474 086a 0919 0064 0364 098d  .j.t.t.j...d.d..
-00000580: 0201 007c 0553 0029 0a4e 6301 0000 0000  ...|.S.).Nc.....
-00000590: 0000 0000 0000 0001 0000 0002 0000 0053  ...............S
-000005a0: 0000 0173 0a00 0000 7400 7c00 6a01 8301  ...s....t.|.j...
-000005b0: 5300 7221 0000 0029 02da 036c 656e 7223  S.r!...)...lenr#
-000005c0: 0000 0029 015a 0d6d 645f 7469 6d65 7365  ...).Z.md_timese
-000005d0: 7269 6573 7215 0000 0072 1500 0000 7218  riesr....r....r.
-000005e0: 0000 00da 083c 6c61 6d62 6461 3e2c 0000  .....<lambda>,..
-000005f0: 0073 0200 0000 0a00 7a25 636f 6e76 6572  .s......z%conver
-00000600: 745f 746f 5f72 6177 5f64 6174 612e 3c6c  t_to_raw_data.<l
-00000610: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e54  ocals>.<lambda>T
-00000620: 2901 da05 696e 6465 7863 0100 0000 0000  )...indexc......
-00000630: 0000 0000 0000 0200 0000 0500 0000 1300  ................
-00000640: 0001 7320 0000 0067 007c 005d 0c7d 017c  ..s ...g.|.].}.|
-00000650: 0188 006a 0076 0072 0274 0188 017c 0183  ...j.v.r.t...|..
-00000660: 0291 0271 0253 0072 1500 0000 2902 da07  ...q.S.r....)...
-00000670: 636f 6c75 6d6e 73da 0767 6574 6174 7472  columns..getattr
-00000680: 2902 7216 0000 00da 0166 a902 da02 6466  ).r......f....df
-00000690: da03 7475 7072 1500 0000 7218 0000 0072  ..tupr....r....r
-000006a0: 1900 0000 3400 0000 7308 0000 0006 0002  ....4...s.......
-000006b0: 0108 0210 fd7a 2763 6f6e 7665 7274 5f74  .....z'convert_t
-000006c0: 6f5f 7261 775f 6461 7461 2e3c 6c6f 6361  o_raw_data.<loca
-000006d0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 46a9  ls>.<listcomp>F.
-000006e0: 0272 2e00 0000 da04 636f 7079 2901 da07  .r......copy)...
-000006f0: 696e 706c 6163 6529 15da 036d 6178 da03  inplace)...max..
-00000700: 6d61 7072 2200 0000 7223 0000 0072 3200  mapr"...r#...r2.
-00000710: 0000 5a0a 6974 6572 7475 706c 6573 da06  ..Z.itertuples..
-00000720: 6170 7065 6e64 722f 0000 0072 0500 0000  appendr/...r....
-00000730: da04 5469 6d65 da06 6173 5f73 7472 da06  ..Time..as_str..
-00000740: 4f62 6a65 6374 7211 0000 0072 1200 0000  Objectr....r....
-00000750: 7225 0000 00da 0270 64da 0944 6174 6146  r%.....pd..DataF
-00000760: 7261 6d65 da1d 6261 7365 5f72 6177 5f6d  rame..base_raw_m
-00000770: 6163 6869 6e65 5f64 6174 615f 636f 6c75  achine_data_colu
-00000780: 6d6e 7372 1d00 0000 5a0b 736f 7274 5f76  mnsr....Z.sort_v
-00000790: 616c 7565 73da 1043 4f4c 554d 4e5f 4e41  alues..COLUMN_NA
-000007a0: 4d45 5f44 4943 5429 0672 1e00 0000 5a0c  ME_DICT).r....Z.
-000007b0: 6d61 785f 6665 6174 7572 6573 da04 726f  max_features..ro
-000007c0: 7773 7227 0000 0072 2800 0000 da03 7265  wsr'...r(.....re
-000007d0: 7372 1500 0000 7231 0000 0072 1800 0000  sr....r1...r....
-000007e0: da13 636f 6e76 6572 745f 746f 5f72 6177  ..convert_to_raw
-000007f0: 5f64 6174 612b 0000 0073 2a00 0000 1601  _data+...s*.....
-00000800: 0401 0c01 0601 0601 1001 0401 2401 0401  ............$...
-00000810: 02ff 0c01 0402 04fe 02ff 06ff 02ff 1007  ................
-00000820: 0201 06ff 1402 0401 7243 0000 00da 1366  ........rC.....f
-00000830: 6561 7475 7265 5f64 6566 696e 6974 696f  eature_definitio
-00000840: 6e73 7209 0000 0063 0100 0000 0000 0000  nsr....c........
-00000850: 0000 0000 0100 0000 0300 0000 4300 0001  ............C...
-00000860: 730a 0000 0074 00a0 017c 00a1 0153 0072  s....t...|...S.r
-00000870: 2100 0000 2902 7209 0000 005a 0866 726f  !...).r....Z.fro
-00000880: 6d5f 7261 7729 0172 4400 0000 7215 0000  m_raw).rD...r...
-00000890: 0072 1500 0000 7218 0000 00da 1663 7265  .r....r......cre
-000008a0: 6174 655f 6865 6164 6572 5f66 726f 6d5f  ate_header_from_
-000008b0: 7261 773e 0000 0073 0200 0000 0a01 7245  raw>...s......rE
-000008c0: 0000 00da 0872 6177 5f64 6174 61da 0a72  .....raw_data..r
-000008d0: 6177 5f68 6561 6465 7263 0200 0000 0000  aw_headerc......
-000008e0: 0000 0000 0000 1400 0000 0700 0000 4300  ..............C.
-000008f0: 0001 736e 0100 0074 007c 0183 017d 0267  ..sn...t.|...}.g
-00000900: 0067 0002 027d 037d 0474 017c 0074 0274  .g...}.}.t.|.t.t
-00000910: 036a 0474 056a 0674 056a 0774 056a 0867  .j.t.j.t.j.t.j.g
-00000920: 0383 0283 027d 0564 0164 0284 0074 03a0  .....}.d.d...t..
-00000930: 09a1 0044 0083 017d 0674 0a6a 0b7c 0074  ...D...}.t.j.|.t
-00000940: 0c64 0364 048d 037d 077c 076a 0d7c 0664  .d.d...}.|.j.|.d
-00000950: 0364 058d 0201 007c 076a 0e7c 0564 0664  .d.....|.j.|.d.d
-00000960: 078d 027d 077c 07a0 0f64 0864 0967 02a1  ...}.|...d.d.g..
-00000970: 016a 10a0 09a1 0044 005d 5e5c 027d 087d  .j.....D.]^\.}.}
-00000980: 097c 085c 027d 0a7d 0b7c 026a 117c 0a7c  .|.\.}.}.|.j.|.|
-00000990: 0b66 0219 007d 0c7c 0c6a 127d 0d74 137c  .f...}.|.j.}.t.|
-000009a0: 0d83 017d 0e74 147c 0e83 017d 0f74 0a6a  ...}.t.|...}.t.j
-000009b0: 157c 076a 167c 0974 1766 0219 007c 006a  .|.j.|.t.f...|.j
-000009c0: 167c 097c 0f66 0219 0067 0264 0364 0a64  .|.|.f...g.d.d.d
-000009d0: 0b8d 03a0 187c 09a1 017d 1064 0c64 0284  .....|...}.d.d..
-000009e0: 0074 197c 0f7c 0d83 0244 0083 017d 117c  .t.|.|...D...}.|
-000009f0: 106a 0d7c 1164 0364 058d 0201 0074 1aa0  .j.|.d.d.....t..
-00000a00: 1b7c 0ca1 017c 1083 017d 1274 1c7c 1274  .|...|...}.t.|.t
-00000a10: 1d83 0272 957c 03a0 1e7c 12a1 0101 0071  ...r.|...|.....q
-00000a20: 4174 1c7c 1274 1f83 0272 9f7c 04a0 1e7c  At.|.t...r.|...|
-00000a30: 12a1 0101 0071 4174 2074 217c 076a 2283  .....qAt t!|.j".
-00000a40: 01a0 2374 17a1 0183 017d 137c 076a 247c  ..#t.....}.|.j$|
-00000a50: 1364 0364 058d 0201 0074 257c 037c 047c  .d.d.....t%|.|.|
-00000a60: 0783 0353 0029 0d4e 6301 0000 0000 0000  ...S.).Nc.......
-00000a70: 0000 0000 0003 0000 0005 0000 0053 0000  .............S..
-00000a80: 0173 1a00 0000 6900 7c00 5d09 5c02 7d01  .s....i.|.].\.}.
-00000a90: 7d02 7c02 7c01 a000 a100 9302 7102 5300  }.|.|.......q.S.
-00000aa0: 7215 0000 0029 0172 3b00 0000 2903 7216  r....).r;...).r.
-00000ab0: 0000 00da 036e 6577 da03 6f6c 6472 1500  .....new..oldr..
-00000ac0: 0000 7215 0000 0072 1800 0000 da0a 3c64  ..r....r......<d
-00000ad0: 6963 7463 6f6d 703e 4a00 0000 7302 0000  ictcomp>J...s...
-00000ae0: 001a 007a 3063 7265 6174 655f 6d61 6368  ...z0create_mach
-00000af0: 696e 655f 6461 7461 5f66 726f 6d5f 7261  ine_data_from_ra
-00000b00: 772e 3c6c 6f63 616c 733e 2e3c 6469 6374  w.<locals>.<dict
-00000b10: 636f 6d70 3e54 7234 0000 0029 0272 2e00  comp>Tr4...).r..
-00000b20: 0000 7236 0000 0046 2901 7235 0000 0072  ..r6...F).r5...r
-00000b30: 1100 0000 7212 0000 0072 0300 0000 2902  ....r....r....).
-00000b40: 7235 0000 00da 0461 7869 7363 0100 0000  r5.....axisc....
-00000b50: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00000b60: 5300 0001 7316 0000 0069 007c 005d 075c  S...s....i.|.].\
-00000b70: 027d 017d 027c 017c 0293 0271 0253 0072  .}.}.|.|...q.S.r
-00000b80: 1500 0000 7215 0000 0029 0372 1600 0000  ....r....).r....
-00000b90: 7249 0000 0072 4800 0000 7215 0000 0072  rI...rH...r....r
-00000ba0: 1500 0000 7218 0000 0072 4a00 0000 5d00  ....r....rJ...].
-00000bb0: 0000 721a 0000 0029 2672 4500 0000 7204  ..r....)&rE...r.
-00000bc0: 0000 0072 3800 0000 7240 0000 00da 0367  ...r8...r@.....g
-00000bd0: 6574 7205 0000 0072 3c00 0000 da05 4c61  etr....r<.....La
-00000be0: 6265 6cda 0454 7970 65da 0569 7465 6d73  bel..Type..items
-00000bf0: 723d 0000 0072 3e00 0000 723f 0000 00da  r=...r>...r?....
-00000c00: 0672 656e 616d 65da 0661 7374 7970 65da  .rename..astype.
-00000c10: 0767 726f 7570 6279 da06 6772 6f75 7073  .groupby..groups
-00000c20: 7244 0000 0072 2500 0000 722b 0000 0072  rD...r%...r+...r
-00000c30: 1d00 0000 da06 636f 6e63 6174 da03 6c6f  ......concat..lo
-00000c40: 6372 0600 0000 5a09 7365 745f 696e 6465  cr....Z.set_inde
-00000c50: 78da 037a 6970 720d 0000 005a 0866 6f72  x..zipr....Z.for
-00000c60: 5f74 7970 65da 0a69 7369 6e73 7461 6e63  _type..isinstanc
-00000c70: 6572 0a00 0000 7239 0000 0072 0b00 0000  er....r9...r....
-00000c80: da04 6c69 7374 da03 7365 7472 2e00 0000  ..list..setr....
-00000c90: da0a 6469 6666 6572 656e 6365 5a04 6472  ..differenceZ.dr
-00000ca0: 6f70 720c 0000 0029 1472 4600 0000 7247  opr....).rF...rG
-00000cb0: 0000 0072 2600 0000 5a04 6d64 6573 5a04  ...r&...Z.mdesZ.
-00000cc0: 6d64 6d73 da0a 6361 7465 676f 7269 6573  mdms..categories
-00000cd0: 5a12 6261 7365 5f63 6f6c 756d 5f6d 6170  Z.base_colum_map
-00000ce0: 7069 6e67 5a07 6f76 6572 616c 6cda 0567  pingZ.overall..g
-00000cf0: 726f 7570 da03 6964 785a 0374 7079 7212  roup..idxZ.tpyr.
-00000d00: 0000 0072 2300 0000 5a15 6163 7475 616c  ...r#...Z.actual
-00000d10: 5f66 6561 7475 7265 5f6c 6162 656c 735a  _feature_labelsZ
-00000d20: 0d66 6561 7475 7265 5f63 6f75 6e74 5a1a  .feature_countZ.
-00000d30: 706c 6163 6568 6f6c 6465 725f 6665 6174  placeholder_feat
-00000d40: 7572 655f 6c61 6265 6c73 7232 0000 005a  ure_labelsr2...Z
-00000d50: 0d72 656e 616d 696e 675f 6469 6374 5a0d  .renaming_dictZ.
-00000d60: 7473 5f63 6f6c 6c65 6374 696f 6eda 1070  ts_collection..p
-00000d70: 6c61 6365 686f 6c64 6572 5f63 6f6c 7372  laceholder_colsr
-00000d80: 1500 0000 7215 0000 0072 1800 0000 da1c  ....r....r......
-00000d90: 6372 6561 7465 5f6d 6163 6869 6e65 5f64  create_machine_d
-00000da0: 6174 615f 6672 6f6d 5f72 6177 4200 0000  ata_from_rawB...
-00000db0: 733e 0000 0008 010a 0204 0216 0104 ff12  s>..............
-00000dc0: 0310 020e 010e 011c 0208 010e 0106 0108  ................
-00000dd0: 0108 011e 0104 0104 ff06 0102 ff14 070e  ................
-00000de0: 020e 010a 010c 010a 010a 0102 8014 020e  ................
-00000df0: 010c 0272 5f00 0000 2904 721e 0000 0072  ...r_...).r....r
-00000e00: 0c00 0000 721f 0000 0072 2000 0000 2904  ....r....r ...).
-00000e10: 721e 0000 0072 0c00 0000 721f 0000 0072  r....r....r....r
-00000e20: 2a00 0000 2904 7244 0000 0072 2000 0000  *...).rD...r ...
-00000e30: 721f 0000 0072 0900 0000 2904 7246 0000  r....r....).rF..
-00000e40: 0072 2a00 0000 7247 0000 0072 2000 0000  .r*...rG...r ...
-00000e50: 2928 da0a 5f5f 6675 7475 7265 5f5f 7202  )(..__future__r.
-00000e60: 0000 005a 0670 616e 6461 7372 3d00 0000  ...Z.pandasr=...
-00000e70: 5a08 6466 5f75 7469 6c73 7204 0000 005a  Z.df_utilsr....Z
-00000e80: 106d 6163 6869 6e65 5f64 6174 615f 6465  .machine_data_de
-00000e90: 6672 0500 0000 7206 0000 0072 0700 0000  fr....r....r....
-00000ea0: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-00000eb0: 0b00 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
-00000ec0: 0000 0072 3a00 0000 723c 0000 0072 4e00  ...r:...r<...rN.
-00000ed0: 0000 724d 0000 0072 4000 0000 7258 0000  ..rM...r@...rX..
-00000ee0: 0072 3800 0000 724c 0000 0072 3f00 0000  .r8...rL...r?...
-00000ef0: 7213 0000 0072 1400 0000 5a17 4d41 4348  r....r....Z.MACH
-00000f00: 494e 455f 4441 5441 5f54 5950 4553 5f44  INE_DATA_TYPES_D
-00000f10: 4943 5472 5900 0000 da16 7261 775f 6d61  ICTrY.....raw_ma
-00000f20: 6368 696e 655f 6461 7461 5f74 7970 6573  chine_data_types
-00000f30: 721d 0000 00da 0464 6963 7472 2000 0000  r......dictr ...
-00000f40: 723e 0000 0072 2a00 0000 7229 0000 0072  r>...r*...r)...r
-00000f50: 4300 0000 7245 0000 0072 5f00 0000 7215  C...rE...r_...r.
-00000f60: 0000 0072 1500 0000 7215 0000 0072 1800  ...r....r....r..
-00000f70: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000f80: 732a 0000 000c 0008 020c 0230 0106 0606  s*.........0....
-00000f90: 0106 0106 0104 fb10 0706 0306 0104 fe10  ................
-00000fa0: 0408 030c 0506 010a 030a 080a 130e 04    ...............
+00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
+00000080: 0100 6509 6a12 6406 6509 6a13 6407 6509  ..e.j.d.e.j.d.e.
+00000090: 6a14 6408 6509 6a15 6409 6904 5a16 6517  j.d.e.j.d.i.Z.e.
+000000a0: 6518 6516 6a19 6509 6a1a 8302 8301 5a1b  e.e.j.e.j.....Z.
+000000b0: 6511 6a1c 640a 6511 6a1d 640b 6902 5a1e  e.j.d.e.j.d.i.Z.
+000000c0: 651f 6518 651e 6a19 6511 6a20 8302 8301  e.e.e.j.e.j ....
+000000d0: 5a21 640c 640d 8400 5a22 6523 650a 650b  Z!d.d...Z"e#e.e.
+000000e0: 6602 1900 5a24 6505 6a25 5a26 6421 6412  f...Z$e.j%Z&d!d.
+000000f0: 6413 8404 5a27 6422 6415 6416 8404 5a28  d...Z'd"d.d...Z(
+00000100: 6422 6417 6418 8404 5a29 6423 641b 641c  d"d.d...Z)d#d.d.
+00000110: 8404 5a2a 6424 641f 6420 8404 5a2b 6402  ..Z*d$d.d ..Z+d.
+00000120: 5300 2925 e900 0000 0029 01da 0b61 6e6e  S.)%.....)...ann
+00000130: 6f74 6174 696f 6e73 4ee9 0100 0000 2901  otationsN.....).
+00000140: da13 6465 7269 7665 5f63 6174 6567 6f72  ..derive_categor
+00000150: 6963 616c 7329 09da 0a4d 4443 6f6e 6365  icals)...MDConce
+00000160: 7074 73da 1154 696d 6573 6572 6965 7354  pts..TimeseriesT
+00000170: 7970 654b 6579 da17 5469 6d65 7365 7269  ypeKey..Timeseri
+00000180: 6573 4665 6174 7572 654c 6162 656c 73da  esFeatureLabels.
+00000190: 0648 6561 6465 72da 1945 7665 6e74 5469  .Header..EventTi
+000001a0: 6d65 7365 7269 6573 436f 6c6c 6563 7469  meseriesCollecti
+000001b0: 6f6e da1f 4d65 6173 7572 656d 656e 7454  on..MeasurementT
+000001c0: 696d 6573 6572 6965 7343 6f6c 6c65 6374  imeseriesCollect
+000001d0: 696f 6eda 0b4d 6163 6869 6e65 4461 7461  ion..MachineData
+000001e0: da1b 5469 6d65 7365 7269 6573 436f 6c6c  ..TimeseriesColl
+000001f0: 6563 7469 6f6e 4661 6374 6f72 79da 104d  ectionFactory..M
+00000200: 6163 6869 6e65 4461 7461 5479 7065 73da  achineDataTypes.
+00000210: 0474 696d 65da 066f 626a 6563 74da 0474  .time..object..t
+00000220: 7970 65da 056c 6162 656c da01 45da 014d  ype..label..E..M
+00000230: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000240: 0005 0000 0043 0000 0173 1800 0000 6401  .....C...s....d.
+00000250: 6402 8400 7400 6403 7c00 6403 1700 8302  d...t.d.|.d.....
+00000260: 4400 8301 5300 2904 4e63 0100 0000 0000  D...S.).Nc......
+00000270: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
+00000280: 0001 7316 0000 0067 007c 005d 077d 0164  ..s....g.|.].}.d
+00000290: 007c 019b 009d 0291 0271 0253 0029 01da  .|.......q.S.)..
+000002a0: 0266 5fa9 0029 02da 022e 30da 0169 7215  .f_..)....0..ir.
+000002b0: 0000 0072 1500 0000 fa39 433a 5c55 7365  ...r.....9C:\Use
+000002c0: 7273 5c4c 6561 685c 5079 6368 6172 6d50  rs\Leah\PycharmP
+000002d0: 726f 6a65 6374 735c 6d64 6174 615c 7372  rojects\mdata\sr
+000002e0: 635c 6d64 6174 615c 636f 7265 5c72 6177  c\mdata\core\raw
+000002f0: 2e70 79da 0a3c 6c69 7374 636f 6d70 3e1c  .py..<listcomp>.
+00000300: 0000 00f3 0200 0000 1600 7a2c 6765 6e5f  ..........z,gen_
+00000310: 6665 6174 7572 655f 636f 6c75 6d6e 5f6e  feature_column_n
+00000320: 616d 6573 2e3c 6c6f 6361 6c73 3e2e 3c6c  ames.<locals>.<l
+00000330: 6973 7463 6f6d 703e 7203 0000 0029 01da  istcomp>r....)..
+00000340: 0572 616e 6765 2901 da01 6e72 1500 0000  .range)...nr....
+00000350: 7215 0000 0072 1800 0000 da18 6765 6e5f  r....r......gen_
+00000360: 6665 6174 7572 655f 636f 6c75 6d6e 5f6e  feature_column_n
+00000370: 616d 6573 1b00 0000 7302 0000 0018 0172  ames....s......r
+00000380: 1d00 0000 da02 6d64 720b 0000 00da 0672  ......mdr......r
+00000390: 6574 7572 6eda 0d52 6177 4865 6164 6572  eturn..RawHeader
+000003a0: 5479 7065 6301 0000 0000 0000 0000 0000  Typec...........
+000003b0: 0004 0000 0005 0000 0043 0000 0173 2e00  .........C...s..
+000003c0: 0000 6900 7d01 7c00 a000 a100 4400 5d0e  ..i.}.|.....D.].
+000003d0: 7d02 7c02 6a01 7d03 7402 7c03 6a03 8301  }.|.j.}.t.|.j...
+000003e0: 7c01 7c03 a004 a100 3c00 7106 7c01 5300  |.|.....<.q.|.S.
+000003f0: a901 4e29 05da 1369 7465 725f 616c 6c5f  ..N)...iter_all_
+00000400: 7469 6d65 7365 7269 6573 da0f 7469 6d65  timeseries..time
+00000410: 7365 7269 6573 5f74 7970 65da 0574 7570  series_type..tup
+00000420: 6c65 da08 6665 6174 7572 6573 da05 6173  le..features..as
+00000430: 6b65 7929 0472 1e00 0000 da06 6865 6164  key).r......head
+00000440: 6572 da10 7479 7065 645f 7469 6d65 7365  er..typed_timese
+00000450: 7269 6573 da02 7474 7215 0000 0072 1500  ries..ttr....r..
+00000460: 0000 7218 0000 00da 1563 6f6e 7665 7274  ..r......convert
+00000470: 5f74 6f5f 7261 775f 6865 6164 6572 2300  _to_raw_header#.
+00000480: 0000 730a 0000 0004 010c 0106 0114 0104  ..s.............
+00000490: 0172 2a00 0000 da0b 5261 7744 6174 6154  .r*.....RawDataT
+000004a0: 7970 6563 0100 0000 0000 0000 0000 0000  ypec............
+000004b0: 0600 0000 0500 0000 4300 0001 7394 0000  ........C...s...
+000004c0: 0074 0074 0164 0164 0284 007c 00a0 02a1  .t.t.d.d...|....
+000004d0: 0083 0283 017d 0174 036a 047c 006a 0564  .....}.t.j.|.j.d
+000004e0: 0364 048d 027d 0274 066a 077c 0274 087c  .d...}.t.j.|.t.|
+000004f0: 0183 013c 007c 00a0 02a1 0044 005d 217d  ...<.|.....D.]!}
+00000500: 037c 036a 097d 0474 0874 0a7c 036a 0b6a  .|.j.}.t.t.|.j.j
+00000510: 0c83 0183 017d 057c 046a 0d64 0064 0085  .....}.|.j.d.d..
+00000520: 0274 0e7c 036a 0b6a 0c83 0166 0219 006a  .t.|.j.j...f...j
+00000530: 0f7c 026a 0d7c 046a 107c 0566 023c 0071  .|.j.|.j.|.f.<.q
+00000540: 1e74 116a 1274 087c 0183 0117 007c 025f  .t.j.t.|.....|._
+00000550: 137c 0253 0029 054e 6301 0000 0000 0000  .|.S.).Nc.......
+00000560: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
+00000570: 01f3 0a00 0000 7400 7c00 6a01 8301 5300  ......t.|.j...S.
+00000580: 7221 0000 00a9 02da 036c 656e 7223 0000  r!.......lenr#..
+00000590: 00a9 015a 0d6d 645f 7469 6d65 7365 7269  ...Z.md_timeseri
+000005a0: 6573 7215 0000 0072 1500 0000 7218 0000  esr....r....r...
+000005b0: 00da 083c 6c61 6d62 6461 3e2c 0000 00f3  ...<lambda>,....
+000005c0: 0200 0000 0a00 7a25 636f 6e76 6572 745f  ......z%convert_
+000005d0: 746f 5f72 6177 5f64 6174 612e 3c6c 6f63  to_raw_data.<loc
+000005e0: 616c 733e 2e3c 6c61 6d62 6461 3e54 a901  als>.<lambda>T..
+000005f0: da04 636f 7079 2914 da03 6d61 78da 036d  ..copy)...max..m
+00000600: 6170 7222 0000 00da 0270 64da 0944 6174  apr".....pd..Dat
+00000610: 6146 7261 6d65 da0b 696e 6465 785f 6672  aFrame..index_fr
+00000620: 616d 65da 026e 70da 034e 414e 721d 0000  ame..np..NANr...
+00000630: 00da 0264 6672 2e00 0000 7223 0000 0072  ...dfr....r#...r
+00000640: 2500 0000 da03 6c6f 63da 046c 6973 74da  %.....loc..list.
+00000650: 0676 616c 7565 73da 0569 6e64 6578 7205  .values..indexr.
+00000660: 0000 00da 0c62 6173 655f 636f 6c75 6d6e  .....base_column
+00000670: 73da 0763 6f6c 756d 6e73 2906 721e 0000  s..columns).r...
+00000680: 00da 0c6d 6178 5f66 6561 7475 7265 73da  ...max_features.
+00000690: 0372 6573 da03 7473 6372 3b00 0000 da02  .res..tscr;.....
+000006a0: 6373 7215 0000 0072 1500 0000 7218 0000  csr....r....r...
+000006b0: 00da 1363 6f6e 7665 7274 5f74 6f5f 7261  ...convert_to_ra
+000006c0: 775f 6461 7461 2b00 0000 7312 0000 0016  w_data+...s.....
+000006d0: 0110 080e 010c 0306 0110 012a 0110 0204  ...........*....
+000006e0: 0472 4600 0000 6301 0000 0000 0000 0000  .rF...c.........
+000006f0: 0000 0006 0000 0008 0000 0003 0000 0173  ...............s
+00000700: b000 0000 7400 7401 6401 6402 8400 7c00  ....t.t.d.d...|.
+00000710: a002 a100 8302 8301 7d01 6700 7d02 7c00  ........}.g.}.|.
+00000720: a002 a100 4400 5d2f 7d03 7c03 6a03 7d04  ....D.]/}.|.j.}.
+00000730: 7c03 6a04 8900 8800 6a05 6403 6404 8d01  |.j.....j.d.d...
+00000740: 4400 5d20 8901 7c02 a006 7407 8801 7408  D.] ..|...t...t.
+00000750: 6a09 8302 7407 8801 7408 6a0a 8302 7c04  j...t...t.j...|.
+00000760: 6a0b 7c04 6a0c 6704 8700 8701 6602 6405  j.|.j.g.....f.d.
+00000770: 6406 8408 7c04 6a0d 4400 8301 1700 a101  d...|.j.D.......
+00000780: 0100 711f 7111 740e 6a0f 7c02 7410 7411  ..q.q.t.j.|.t.t.
+00000790: 7c01 8301 1700 6407 8d02 7d05 7c05 6a12  |.....d...}.|.j.
+000007a0: 7413 7408 6a09 1900 6403 6408 8d02 0100  t.t.j...d.d.....
+000007b0: 7c05 5300 2909 4e63 0100 0000 0000 0000  |.S.).Nc........
+000007c0: 0000 0000 0100 0000 0200 0000 5300 0001  ............S...
+000007d0: 722c 0000 0072 2100 0000 722d 0000 0072  r,...r!...r-...r
+000007e0: 2f00 0000 7215 0000 0072 1500 0000 7218  /...r....r....r.
+000007f0: 0000 0072 3000 0000 4500 0000 7231 0000  ...r0...E...r1..
+00000800: 007a 2c63 6f6e 7665 7274 5f74 6f5f 7261  .z,convert_to_ra
+00000810: 775f 6461 7461 5f6c 6567 6163 792e 3c6c  w_data_legacy.<l
+00000820: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e54  ocals>.<lambda>T
+00000830: 2901 723f 0000 0063 0100 0000 0000 0000  ).r?...c........
+00000840: 0000 0000 0200 0000 0500 0000 1300 0001  ................
+00000850: 7320 0000 0067 007c 005d 0c7d 017c 0188  s ...g.|.].}.|..
+00000860: 006a 0076 0072 0274 0188 017c 0183 0291  .j.v.r.t...|....
+00000870: 0271 0253 0072 1500 0000 2902 7241 0000  .q.S.r....).rA..
+00000880: 00da 0767 6574 6174 7472 2902 7216 0000  ...getattr).r...
+00000890: 00da 0166 a902 723b 0000 00da 0374 7570  ...f..r;.....tup
+000008a0: 7215 0000 0072 1800 0000 7219 0000 004d  r....r....r....M
+000008b0: 0000 0073 0800 0000 0600 0201 0802 10fd  ...s............
+000008c0: 7a2e 636f 6e76 6572 745f 746f 5f72 6177  z.convert_to_raw
+000008d0: 5f64 6174 615f 6c65 6761 6379 2e3c 6c6f  _data_legacy.<lo
+000008e0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+000008f0: 2901 7241 0000 0029 01da 0769 6e70 6c61  ).rA...)...inpla
+00000900: 6365 2914 7234 0000 0072 3500 0000 7222  ce).r4...r5...r"
+00000910: 0000 0072 2300 0000 723b 0000 00da 0a69  ...r#...r;.....i
+00000920: 7465 7274 7570 6c65 73da 0661 7070 656e  tertuples..appen
+00000930: 6472 4700 0000 7205 0000 00da 0454 696d  drG...r......Tim
+00000940: 65da 064f 626a 6563 7472 1000 0000 7211  e..Objectr....r.
+00000950: 0000 0072 2500 0000 7236 0000 0072 3700  ...r%...r6...r7.
+00000960: 0000 da1d 6261 7365 5f72 6177 5f6d 6163  ....base_raw_mac
+00000970: 6869 6e65 5f64 6174 615f 636f 6c75 6d6e  hine_data_column
+00000980: 7372 1d00 0000 da0b 736f 7274 5f76 616c  sr......sort_val
+00000990: 7565 73da 1043 4f4c 554d 4e5f 4e41 4d45  ues..COLUMN_NAME
+000009a0: 5f44 4943 5429 0672 1e00 0000 7242 0000  _DICT).r....rB..
+000009b0: 00da 0472 6f77 7372 2800 0000 7229 0000  ...rowsr(...r)..
+000009c0: 0072 4300 0000 7215 0000 0072 4900 0000  .rC...r....rI...
+000009d0: 7218 0000 00da 1a63 6f6e 7665 7274 5f74  r......convert_t
+000009e0: 6f5f 7261 775f 6461 7461 5f6c 6567 6163  o_raw_data_legac
+000009f0: 7944 0000 0073 2600 0000 1601 0401 0c01  yD...s&.........
+00000a00: 0601 0601 1001 0401 1801 0401 02ff 0c01  ................
+00000a10: 0402 04fe 02ff 06ff 02ff 1607 1401 0401  ................
+00000a20: 7254 0000 00da 1366 6561 7475 7265 5f64  rT.....feature_d
+00000a30: 6566 696e 6974 696f 6e73 7208 0000 0063  efinitionsr....c
+00000a40: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000a50: 0300 0000 4300 0001 730a 0000 0074 00a0  ....C...s....t..
+00000a60: 017c 00a1 0153 0072 2100 0000 2902 7208  .|...S.r!...).r.
+00000a70: 0000 00da 0866 726f 6d5f 7261 7729 0172  .....from_raw).r
+00000a80: 5500 0000 7215 0000 0072 1500 0000 7218  U...r....r....r.
+00000a90: 0000 00da 1663 7265 6174 655f 6865 6164  .....create_head
+00000aa0: 6572 5f66 726f 6d5f 7261 7756 0000 0073  er_from_rawV...s
+00000ab0: 0200 0000 0a01 7257 0000 00da 0872 6177  ......rW.....raw
+00000ac0: 5f64 6174 61da 0a72 6177 5f68 6561 6465  _data..raw_heade
+00000ad0: 7263 0200 0000 0000 0000 0000 0000 1400  rc..............
+00000ae0: 0000 0700 0000 4300 0001 737e 0100 0074  ......C...s~...t
+00000af0: 007c 0183 017d 0267 0067 0002 027d 037d  .|...}.g.g...}.}
+00000b00: 0474 017c 0074 0274 036a 0474 056a 0674  .t.|.t.t.j.t.j.t
+00000b10: 056a 0774 056a 0867 0383 0283 027d 0564  .j.t.j.g.....}.d
+00000b20: 0164 0284 0074 03a0 09a1 0044 0083 017d  .d...t.....D...}
+00000b30: 0674 0a6a 0b7c 0074 0c64 0364 048d 037d  .t.j.|.t.d.d...}
+00000b40: 077c 076a 0d7c 0664 0364 058d 0201 007c  .|.j.|.d.d.....|
+00000b50: 076a 0e7c 0564 0664 078d 027d 077c 07a0  .j.|.d.d...}.|..
+00000b60: 0f74 0374 056a 0819 0074 0374 056a 0719  .t.t.j...t.t.j..
+00000b70: 0067 02a1 016a 10a0 09a1 0044 005d 5f5c  .g...j.....D.]_\
+00000b80: 027d 087d 097c 085c 027d 0a7d 0b7c 026a  .}.}.|.\.}.}.|.j
+00000b90: 117c 0a7c 0b66 0219 007d 0c7c 0c6a 127d  .|.|.f...}.|.j.}
+00000ba0: 0d74 137c 0d83 017d 0e74 147c 0e83 017d  .t.|...}.t.|...}
+00000bb0: 0f74 0a6a 157c 076a 167c 0974 056a 1766  .t.j.|.j.|.t.j.f
+00000bc0: 0219 007c 006a 167c 097c 0f66 0219 0067  ...|.j.|.|.f...g
+00000bd0: 0264 0364 0864 098d 03a0 187c 09a1 017d  .d.d.d.....|...}
+00000be0: 1064 0a64 0284 0074 197c 0f7c 0d83 0244  .d.d...t.|.|...D
+00000bf0: 0083 017d 117c 106a 0d7c 1164 0364 058d  ...}.|.j.|.d.d..
+00000c00: 0201 0074 1aa0 1b7c 0ca1 017c 1083 017d  ...t...|...|...}
+00000c10: 1274 1c7c 1274 1d83 0272 9c7c 03a0 1e7c  .t.|.t...r.|...|
+00000c20: 12a1 0101 0071 4774 1c7c 1274 1f83 0272  .....qGt.|.t...r
+00000c30: a67c 04a0 1e7c 12a1 0101 0071 4774 2074  .|...|.....qGt t
+00000c40: 217c 076a 2283 01a0 2374 056a 17a1 0183  !|.j"...#t.j....
+00000c50: 017d 137c 076a 247c 1364 0364 058d 0201  .}.|.j$|.d.d....
+00000c60: 0074 257c 037c 047c 0783 0353 0029 0b4e  .t%|.|.|...S.).N
+00000c70: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00000c80: 0004 0000 0053 0000 0173 1600 0000 6900  .....S...s....i.
+00000c90: 7c00 5d07 5c02 7d01 7d02 7c02 7c01 9302  |.].\.}.}.|.|...
+00000ca0: 7102 5300 7215 0000 0072 1500 0000 2903  q.S.r....r....).
+00000cb0: 7216 0000 00da 036e 6577 da03 6f6c 6472  r......new..oldr
+00000cc0: 1500 0000 7215 0000 0072 1800 0000 da0a  ....r....r......
+00000cd0: 3c64 6963 7463 6f6d 703e 6200 0000 721a  <dictcomp>b...r.
+00000ce0: 0000 007a 3063 7265 6174 655f 6d61 6368  ...z0create_mach
+00000cf0: 696e 655f 6461 7461 5f66 726f 6d5f 7261  ine_data_from_ra
+00000d00: 772e 3c6c 6f63 616c 733e 2e3c 6469 6374  w.<locals>.<dict
+00000d10: 636f 6d70 3e54 2902 7241 0000 0072 3300  comp>T).rA...r3.
+00000d20: 0000 2902 7241 0000 0072 4b00 0000 4672  ..).rA...rK...Fr
+00000d30: 3200 0000 7203 0000 0029 0272 3300 0000  2...r....).r3...
+00000d40: da04 6178 6973 6301 0000 0000 0000 0000  ..axisc.........
+00000d50: 0000 0003 0000 0004 0000 0053 0000 0173  ...........S...s
+00000d60: 1600 0000 6900 7c00 5d07 5c02 7d01 7d02  ....i.|.].\.}.}.
+00000d70: 7c01 7c02 9302 7102 5300 7215 0000 0072  |.|...q.S.r....r
+00000d80: 1500 0000 2903 7216 0000 0072 5b00 0000  ....).r....r[...
+00000d90: 725a 0000 0072 1500 0000 7215 0000 0072  rZ...r....r....r
+00000da0: 1800 0000 725c 0000 0075 0000 0072 1a00  ....r\...u...r..
+00000db0: 0000 2926 7257 0000 0072 0400 0000 7235  ..)&rW...r....r5
+00000dc0: 0000 0072 5200 0000 da03 6765 7472 0500  ...rR.....getr..
+00000dd0: 0000 724f 0000 00da 054c 6162 656c da04  ..rO.....Label..
+00000de0: 5479 7065 da05 6974 656d 7372 3600 0000  Type..itemsr6...
+00000df0: 7237 0000 0072 5000 0000 da06 7265 6e61  r7...rP.....rena
+00000e00: 6d65 da06 6173 7479 7065 da07 6772 6f75  me..astype..grou
+00000e10: 7062 79da 0667 726f 7570 7372 5500 0000  pby..groupsrU...
+00000e20: 7225 0000 0072 2e00 0000 721d 0000 00da  r%...r....r.....
+00000e30: 0663 6f6e 6361 7472 3c00 0000 7240 0000  .concatr<...r@..
+00000e40: 00da 0973 6574 5f69 6e64 6578 da03 7a69  ...set_index..zi
+00000e50: 7072 0c00 0000 da08 666f 725f 7479 7065  pr......for_type
+00000e60: da0a 6973 696e 7374 616e 6365 7209 0000  ..isinstancer...
+00000e70: 0072 4d00 0000 720a 0000 0072 3d00 0000  .rM...r....r=...
+00000e80: da03 7365 7472 4100 0000 da0a 6469 6666  ..setrA.....diff
+00000e90: 6572 656e 6365 da04 6472 6f70 720b 0000  erence..dropr...
+00000ea0: 0029 1472 5800 0000 7259 0000 0072 2700  .).rX...rY...r'.
+00000eb0: 0000 5a04 6d64 6573 5a04 6d64 6d73 da0a  ..Z.mdesZ.mdms..
+00000ec0: 6361 7465 676f 7269 6573 5a12 6261 7365  categoriesZ.base
+00000ed0: 5f63 6f6c 756d 5f6d 6170 7069 6e67 5a07  _colum_mappingZ.
+00000ee0: 6f76 6572 616c 6cda 0567 726f 7570 da03  overall..group..
+00000ef0: 6964 785a 0374 7079 7211 0000 0072 2300  idxZ.tpyr....r#.
+00000f00: 0000 5a15 6163 7475 616c 5f66 6561 7475  ..Z.actual_featu
+00000f10: 7265 5f6c 6162 656c 735a 0d66 6561 7475  re_labelsZ.featu
+00000f20: 7265 5f63 6f75 6e74 5a1a 706c 6163 6568  re_countZ.placeh
+00000f30: 6f6c 6465 725f 6665 6174 7572 655f 6c61  older_feature_la
+00000f40: 6265 6c73 723b 0000 005a 0d72 656e 616d  belsr;...Z.renam
+00000f50: 696e 675f 6469 6374 5a0d 7473 5f63 6f6c  ing_dictZ.ts_col
+00000f60: 6c65 6374 696f 6eda 1070 6c61 6365 686f  lection..placeho
+00000f70: 6c64 6572 5f63 6f6c 7372 1500 0000 7215  lder_colsr....r.
+00000f80: 0000 0072 1800 0000 da1c 6372 6561 7465  ...r......create
+00000f90: 5f6d 6163 6869 6e65 5f64 6174 615f 6672  _machine_data_fr
+00000fa0: 6f6d 5f72 6177 5a00 0000 733e 0000 0008  om_rawZ...s>....
+00000fb0: 010a 0204 0216 0104 ff12 0310 020e 010e  ................
+00000fc0: 0128 0208 010e 0106 0108 0108 0120 0104  .(........... ..
+00000fd0: 0104 ff06 0102 ff14 070e 020e 010a 010c  ................
+00000fe0: 010a 010a 0102 8016 020e 010c 0272 7200  .............rr.
+00000ff0: 0000 2904 721e 0000 0072 0b00 0000 721f  ..).r....r....r.
+00001000: 0000 0072 2000 0000 2904 721e 0000 0072  ...r ...).r....r
+00001010: 0b00 0000 721f 0000 0072 2b00 0000 2904  ....r....r+...).
+00001020: 7255 0000 0072 2000 0000 721f 0000 0072  rU...r ...r....r
+00001030: 0800 0000 2904 7258 0000 0072 2b00 0000  ....).rX...r+...
+00001040: 7259 0000 0072 2000 0000 292c da0a 5f5f  rY...r ...),..__
+00001050: 6675 7475 7265 5f5f 7202 0000 00da 056e  future__r......n
+00001060: 756d 7079 7239 0000 00da 0670 616e 6461  umpyr9.....panda
+00001070: 7372 3600 0000 da08 6466 5f75 7469 6c73  sr6.....df_utils
+00001080: 7204 0000 00da 106d 6163 6869 6e65 5f64  r......machine_d
+00001090: 6174 615f 6465 6672 0500 0000 7206 0000  ata_defr....r...
+000010a0: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
+000010b0: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+000010c0: 0d00 0000 724e 0000 0072 4f00 0000 7260  ....rN...rO...r`
+000010d0: 0000 0072 5f00 0000 7252 0000 0072 3d00  ...r_...rR...r=.
+000010e0: 0000 7235 0000 0072 5e00 0000 7240 0000  ..r5...r^...r@..
+000010f0: 0072 5000 0000 7212 0000 0072 1300 0000  .rP...r....r....
+00001100: 5a17 4d41 4348 494e 455f 4441 5441 5f54  Z.MACHINE_DATA_T
+00001110: 5950 4553 5f44 4943 5472 6b00 0000 da0a  YPES_DICTrk.....
+00001120: 6261 7365 5f74 7970 6573 da16 7261 775f  base_types..raw_
+00001130: 6d61 6368 696e 655f 6461 7461 5f74 7970  machine_data_typ
+00001140: 6573 721d 0000 00da 0464 6963 7472 2000  esr......dictr .
+00001150: 0000 7237 0000 0072 2b00 0000 722a 0000  ..r7...r+...r*..
+00001160: 0072 4600 0000 7254 0000 0072 5700 0000  .rF...rT...rW...
+00001170: 7272 0000 0072 1500 0000 7215 0000 0072  rr...r....r....r
+00001180: 1500 0000 7218 0000 00da 083c 6d6f 6475  ....r......<modu
+00001190: 6c65 3e01 0000 0073 2e00 0000 0c00 0802  le>....s........
+000011a0: 0801 0c02 2c01 0606 0601 0601 0601 04fb  ....,...........
+000011b0: 1207 0603 0601 04fe 1204 0803 0c04 0601  ................
+000011c0: 0a03 0a08 0a19 0a12 0e04                 ..........
```

### Comparing `mdata-0.1.0/src/mdata/core/raw.py` & `mdata-0.1.1/src/mdata/core/raw.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,88 @@
 from __future__ import annotations
 
+import numpy as np
 import pandas as pd
 
 from .df_utils import derive_categoricals
-from .machine_data_def import MDConcepts, base_machine_data_columns, TimeseriesTypeKey, TimeseriesFeatureLabels, Header, \
+from .machine_data_def import MDConcepts, TimeseriesTypeKey, TimeseriesFeatureLabels, Header, \
     EventTimeseriesCollection, MeasurementTimeseriesCollection, MachineData, TimeseriesCollectionFactory, \
-    MachineDataType
+    MachineDataTypes
 
 COLUMN_NAME_DICT = {
     # internal to external label mapping
     MDConcepts.Time: 'time',
     MDConcepts.Object: 'object',
     MDConcepts.Type: 'type',
     MDConcepts.Label: 'label'
 }
-base_raw_machine_data_columns = list(map(COLUMN_NAME_DICT.get, MDConcepts))
+base_raw_machine_data_columns = list(map(COLUMN_NAME_DICT.get, MDConcepts.base_columns))
 
 MACHINE_DATA_TYPES_DICT = {
-    MachineDataType.E: 'E',
-    MachineDataType.M: 'M'
+    MachineDataTypes.E: 'E',
+    MachineDataTypes.M: 'M'
 }
-raw_machine_data_types = set(map(MACHINE_DATA_TYPES_DICT.get, MachineDataType))
+raw_machine_data_types = set(map(MACHINE_DATA_TYPES_DICT.get, MachineDataTypes.base_types))
 
 
 def gen_feature_column_names(n):
     return [f'f_{i}' for i in range(1, n + 1)]
 
 
-
 RawHeaderType = dict[TimeseriesTypeKey, TimeseriesFeatureLabels]
 RawDataType = pd.DataFrame
 
 
 def convert_to_raw_header(md: MachineData) -> RawHeaderType:
     header = {}
     for typed_timeseries in md.iter_all_timeseries():
         tt = typed_timeseries.timeseries_type
         header[tt.askey()] = tuple(tt.features)
     return header
 
 
 def convert_to_raw_data(md: MachineData) -> RawDataType:
     max_features = max(map(lambda md_timeseries: len(md_timeseries.timeseries_type), md.iter_all_timeseries()))
+    #dfs = [pd.DataFrame(tsc.df[base_machine_data_columns + list(tsc.timeseries_type.features)], copy=False) for tsc in
+    #       md.iter_all_timeseries()]
+    #for df, tsc in zip(dfs, md.iter_all_timeseries()):
+    #    df.columns = base_machine_data_columns + gen_feature_column_names(len(tsc.timeseries_type.features))
+    #res = md.index_frame.join((df.drop(base_machine_data_columns, axis=1) for df in dfs), how='inner')
+    # TODO CHANGE BACK
+
+    res = pd.DataFrame(md.index_frame, copy=True)#.reindex(columns=))
+    res[gen_feature_column_names(max_features)] = np.NAN
+
+    #res.columns = base_raw_machine_data_columns + gen_feature_column_names(max_features)
+    for tsc in md.iter_all_timeseries():
+        df = tsc.df
+        cs = gen_feature_column_names(len(tsc.timeseries_type.features))
+        res.loc[df.index, cs] = df.loc[:, list(tsc.timeseries_type.features)].values
+
+    res.columns = MDConcepts.base_columns + gen_feature_column_names(max_features)
+    #res = pd.concat(dfs, ignore_index=True, copy=False, verify_integrity=False, join='inner') # TODO check copying
+
+    #res.sort_values(COLUMN_NAME_DICT[MDConcepts.Time], ascending=True, inplace=True)
+    return res
+
+
+def convert_to_raw_data_legacy(md: MachineData) -> RawDataType:
+    max_features = max(map(lambda md_timeseries: len(md_timeseries.timeseries_type), md.iter_all_timeseries()))
     rows = []
     for typed_timeseries in md.iter_all_timeseries():
         tt = typed_timeseries.timeseries_type
         df = typed_timeseries.df
         for tup in df.itertuples(index=True):
             rows.append(
-                [getattr(tup, MDConcepts.Time.as_str()), getattr(tup, MDConcepts.Object.as_str()), tt.type.as_str(),
+                [getattr(tup, MDConcepts.Time), getattr(tup, MDConcepts.Object), tt.type,
                  tt.label] + [getattr(tup, f)
                               for f in
                               tt.features if
                               f in df.columns])
-    res = pd.DataFrame(rows, columns=(base_raw_machine_data_columns + gen_feature_column_names(max_features)),
-                       copy=False)
+    res = pd.DataFrame(rows, columns=(base_raw_machine_data_columns + gen_feature_column_names(max_features)))
     res.sort_values(COLUMN_NAME_DICT[MDConcepts.Time], inplace=True)
     return res
 
 
 def create_header_from_raw(feature_definitions: RawHeaderType) -> Header:
     return Header.from_raw(feature_definitions)
 
@@ -67,27 +91,27 @@
     header = create_header_from_raw(raw_header)
 
     mdes, mdms = [], []
 
     categories = derive_categoricals(raw_data,
                                      map(COLUMN_NAME_DICT.get, [MDConcepts.Object, MDConcepts.Label, MDConcepts.Type]))
 
-    base_colum_mapping = {old: new.as_str() for new, old in COLUMN_NAME_DICT.items()}
+    base_colum_mapping = {old: new for new, old in COLUMN_NAME_DICT.items()}
 
     overall = pd.DataFrame(raw_data, columns=base_raw_machine_data_columns, copy=True)
     overall.rename(columns=base_colum_mapping, inplace=True)
     overall = overall.astype(categories, copy=False)
 
-    for group, idx in overall.groupby(['type', 'label']).groups.items():
+    for group, idx in overall.groupby([COLUMN_NAME_DICT[MDConcepts.Type], COLUMN_NAME_DICT[MDConcepts.Label]]).groups.items():
         tpy, label = group
         timeseries_type = header.feature_definitions[tpy, label]
         actual_feature_labels = timeseries_type.features
         feature_count = len(actual_feature_labels)
         placeholder_feature_labels = gen_feature_column_names(feature_count)
-        df = pd.concat([overall.loc[idx, base_machine_data_columns], raw_data.loc[idx, placeholder_feature_labels]],
+        df = pd.concat([overall.loc[idx, MDConcepts.base_columns], raw_data.loc[idx, placeholder_feature_labels]],
                        copy=True, axis=1).set_index(idx)
         # relevant_cols = list(base_machine_data_columns) + placeholder_feature_labels
         # df = pd.DataFrame(raw_data.loc[idx, relevant_cols], copy=True)
         # not a good idea in case of duplicates
         # df.set_index('time', inplace=True, verify_integrity=True, drop=False)
         # df = df.astype(categories, copy=False)
         renaming_dict = {old: new for old, new in zip(placeholder_feature_labels, actual_feature_labels)}
@@ -95,11 +119,11 @@
         df.rename(columns=renaming_dict, inplace=True)
         ts_collection = TimeseriesCollectionFactory.for_type(timeseries_type)(df)
         if isinstance(ts_collection, EventTimeseriesCollection):
             mdes.append(ts_collection)
         elif isinstance(ts_collection, MeasurementTimeseriesCollection):
             mdms.append(ts_collection)
 
-    placeholder_cols = list(set(overall.columns).difference(base_machine_data_columns))
+    placeholder_cols = list(set(overall.columns).difference(MDConcepts.base_columns))
     overall.drop(columns=placeholder_cols, inplace=True)
 
     return MachineData(mdes, mdms, overall)
```

### Comparing `mdata-0.1.0/src/mdata/file_formats/__pycache__/validity_checking_utils.cpython-310.pyc` & `mdata-0.1.1/src/mdata/file_formats/__pycache__/validity_checking_utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May  3 09:08:07 2023 UTC, .py size: 1912 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,148 +1,163 @@
-00000000: 6f0d 0d0a 0000 0000 7724 5264 7807 0000  o.......w$Rdx...
+00000000: 6f0d 0d0a 0000 0000 7cb7 5364 a107 0000  o.......|.Sd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 c800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 4700 6402 6403  m.Z.m.Z...G.d.d.
 00000050: 8400 6403 6506 8303 5a07 4700 6404 6405  ..d.e...Z.G.d.d.
 00000060: 8400 6405 6507 8303 5a08 4700 6406 6407  ..d.e...Z.G.d.d.
 00000070: 8400 6407 6507 8303 5a09 4700 6408 6409  ..d.e...Z.G.d.d.
 00000080: 8400 6409 6508 8303 5a0a 4700 640a 640b  ..d.e...Z.G.d.d.
 00000090: 8400 640b 6508 8303 5a0b 4700 640c 640d  ..d.e...Z.G.d.d.
-000000a0: 8400 640d 6509 8303 5a0c 4700 640e 640f  ..d.e...Z.G.d.d.
-000000b0: 8400 640f 6509 8303 5a0d 6410 6411 8400  ..d.e...Z.d.d...
-000000c0: 5a0e 6412 6501 6413 6502 6604 6414 6415  Z.d.e.d.e.f.d.d.
-000000d0: 8404 5a0f 6413 6502 6602 6416 6417 8404  ..Z.d.e.f.d.d...
-000000e0: 5a10 6418 5300 2919 e900 0000 0029 05da  Z.d.S.)......)..
-000000f0: 0d52 6177 4865 6164 6572 5479 7065 da0b  .RawHeaderType..
-00000100: 5261 7744 6174 6154 7970 65da 1663 7265  RawDataType..cre
-00000110: 6174 655f 6865 6164 6572 5f66 726f 6d5f  ate_header_from_
-00000120: 7261 77da 1867 656e 5f66 6561 7475 7265  raw..gen_feature
-00000130: 5f63 6f6c 756d 6e5f 6e61 6d65 73da 1d62  _column_names..b
-00000140: 6173 655f 7261 775f 6d61 6368 696e 655f  ase_raw_machine_
-00000150: 6461 7461 5f63 6f6c 756d 6e73 6300 0000  data_columnsc...
-00000160: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-00000170: 0040 0000 00f3 0c00 0000 6500 5a01 6400  .@........e.Z.d.
-00000180: 5a02 6401 5300 2902 da19 5661 6c69 6469  Z.d.S.)...Validi
-00000190: 7479 4368 6563 6b69 6e67 4578 6365 7074  tyCheckingExcept
-000001a0: 696f 6e4e a903 da08 5f5f 6e61 6d65 5f5f  ionN....__name__
-000001b0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-000001c0: 7175 616c 6e61 6d65 5f5f a900 720d 0000  qualname__..r...
-000001d0: 0072 0d00 0000 fa55 433a 5c55 7365 7273  .r.....UC:\Users
-000001e0: 5c4c 6561 685c 5079 6368 6172 6d50 726f  \Leah\PycharmPro
-000001f0: 6a65 6374 735c 6d64 6174 615c 7372 635c  jects\mdata\src\
-00000200: 6d64 6174 615c 6669 6c65 5f66 6f72 6d61  mdata\file_forma
-00000210: 7473 5c76 616c 6964 6974 795f 6368 6563  ts\validity_chec
-00000220: 6b69 6e67 5f75 7469 6c73 2e70 7972 0800  king_utils.pyr..
-00000230: 0000 0500 0000 f304 0000 0008 0004 0172  ...............r
-00000240: 0800 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000250: 0000 0000 0001 0000 0040 0000 0072 0700  .........@...r..
-00000260: 0000 2902 da1a 5379 6e74 6163 7469 6356  ..)...SyntacticV
-00000270: 616c 6964 6974 7945 7863 6570 7469 6f6e  alidityException
-00000280: 4e72 0900 0000 720d 0000 0072 0d00 0000  Nr....r....r....
-00000290: 720d 0000 0072 0e00 0000 7210 0000 0009  r....r....r.....
-000002a0: 0000 0072 0f00 0000 7210 0000 0063 0000  ...r....r....c..
-000002b0: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-000002c0: 0000 4000 0000 7207 0000 0029 02da 1953  ..@...r....)...S
-000002d0: 656d 616e 7469 6356 616c 6964 6974 7945  emanticValidityE
-000002e0: 7863 6570 7469 6f6e 4e72 0900 0000 720d  xceptionNr....r.
-000002f0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000300: 0000 7211 0000 000d 0000 0072 0f00 0000  ..r........r....
-00000310: 7211 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000320: 0000 0000 0000 0100 0000 4000 0000 7207  ..........@...r.
-00000330: 0000 0029 02da 1c4d 616c 666f 726d 6564  ...)...Malformed
-00000340: 4865 6164 6572 4669 6c65 4578 6365 7074  HeaderFileExcept
-00000350: 696f 6e4e 7209 0000 0072 0d00 0000 720d  ionNr....r....r.
-00000360: 0000 0072 0d00 0000 720e 0000 0072 1200  ...r....r....r..
-00000370: 0000 1100 0000 720f 0000 0072 1200 0000  ......r....r....
-00000380: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000390: 0001 0000 0040 0000 0072 0700 0000 2902  .....@...r....).
-000003a0: da1a 4d61 6c66 6f72 6d65 6444 6174 6146  ..MalformedDataF
-000003b0: 696c 6545 7863 6570 7469 6f6e 4e72 0900  ileExceptionNr..
-000003c0: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-000003d0: 0072 0e00 0000 7213 0000 0015 0000 0072  .r....r........r
-000003e0: 0f00 0000 7213 0000 0063 0000 0000 0000  ....r....c......
-000003f0: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
-00000400: 0000 7207 0000 0029 02da 1249 6e73 7566  ..r....)...Insuf
-00000410: 6669 6369 656e 7448 6561 6465 724e 7209  ficientHeaderNr.
-00000420: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
-00000430: 0000 720e 0000 0072 1400 0000 1900 0000  ..r....r........
-00000440: 720f 0000 0072 1400 0000 6300 0000 0000  r....r....c.....
-00000450: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
-00000460: 0000 0072 0700 0000 2902 da1a 496e 636f  ...r....)...Inco
-00000470: 6e73 6973 7465 6e74 5469 6d65 7365 7269  nsistentTimeseri
-00000480: 6573 5479 7065 4e72 0900 0000 720d 0000  esTypeNr....r...
-00000490: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
-000004a0: 7215 0000 001d 0000 0072 0f00 0000 7215  r........r....r.
-000004b0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000004c0: 0200 0000 0400 0000 4300 0000 7318 0000  ........C...s...
-000004d0: 0074 0074 017c 006a 0283 01a0 0374 04a1  .t.t.|.j.....t..
-000004e0: 0183 017d 017c 0153 0029 014e 2905 da06  ...}.|.S.).N)...
-000004f0: 736f 7274 6564 da03 7365 74da 0763 6f6c  sorted..set..col
-00000500: 756d 6e73 da0a 6469 6666 6572 656e 6365  umns..difference
-00000510: 7206 0000 0029 02da 0264 66da 1070 6c61  r....)...df..pla
-00000520: 6365 686f 6c64 6572 5f63 6f6c 7372 0d00  ceholder_colsr..
-00000530: 0000 720d 0000 0072 0e00 0000 da14 6765  ..r....r......ge
-00000540: 745f 706c 6163 6568 6f6c 6465 725f 636f  t_placeholder_co
-00000550: 6c73 2100 0000 7304 0000 0014 0104 0172  ls!...s........r
-00000560: 1c00 0000 da06 6865 6164 6572 da04 6461  ......header..da
-00000570: 7461 6302 0000 0000 0000 0000 0000 000c  tac.............
-00000580: 0000 0005 0000 0043 0000 0073 be00 0000  .......C...s....
-00000590: 7400 7c00 8301 7d00 7401 7c01 8301 7d02  t.|...}.t.|...}.
-000005a0: 7402 7403 7c02 8301 8301 7d03 7c01 a004  t.t.|.....}.|...
-000005b0: 6401 6402 6702 a101 6a05 a006 a100 4400  d.d.g...j.....D.
-000005c0: 5d44 5c02 7d04 7d05 7c04 5c02 7d06 7d07  ]D\.}.}.|.\.}.}.
-000005d0: 7c06 7c07 6602 7c00 6a07 7601 7229 7408  |.|.f.|.j.v.r)t.
-000005e0: 8201 7c00 6a07 7c06 7c07 6602 1900 6a09  ..|.j.|.|.f...j.
-000005f0: 7d08 7403 7c08 8301 7d09 740a 7c02 8301  }.t.|...}.t.|...
-00000600: 4400 5d22 5c02 7d0a 7d0b 7c0b 7c03 7c0a  D.]"\.}.}.|.|.|.
-00000610: 1900 6b02 7345 4a00 8201 7c0a 7c09 6b00  ..k.sEJ...|.|.k.
-00000620: 724a 0900 7c0a 7c09 6b05 725b 7c01 6a0b  rJ..|.|.k.r[|.j.
-00000630: 7c05 7c0b 6602 1900 a00c a100 a00d a100  |.|.f...........
-00000640: 735b 740e 8201 7139 7118 6403 5300 2904  s[t...q9q.d.S.).
-00000650: 4eda 0474 7970 65da 056c 6162 656c 5429  N..type..labelT)
-00000660: 0f72 0400 0000 721c 0000 0072 0500 0000  .r....r....r....
-00000670: da03 6c65 6eda 0767 726f 7570 6279 da06  ..len..groupby..
-00000680: 6772 6f75 7073 da05 6974 656d 73da 1366  groups..items..f
-00000690: 6561 7475 7265 5f64 6566 696e 6974 696f  eature_definitio
-000006a0: 6e73 7214 0000 00da 0866 6561 7475 7265  nsr......feature
-000006b0: 73da 0965 6e75 6d65 7261 7465 da03 6c6f  s..enumerate..lo
-000006c0: 63da 0469 736e 61da 0361 6c6c 7215 0000  c..isna..allr...
-000006d0: 0029 0c72 1d00 0000 721e 0000 0072 1b00  .).r....r....r..
-000006e0: 0000 da0a 746f 5f62 655f 636f 6c73 da05  ....to_be_cols..
-000006f0: 6772 6f75 70da 0369 6478 da03 7470 7972  group..idx..tpyr
-00000700: 2000 0000 da01 665a 0566 5f6c 656e da01   .....fZ.f_len..
-00000710: 69da 0163 720d 0000 0072 0d00 0000 720e  i..cr....r....r.
-00000720: 0000 00da 1f63 6865 636b 5f68 6561 6465  .....check_heade
-00000730: 725f 6461 7461 5f63 6f6d 7061 7469 6269  r_data_compatibi
-00000740: 6c69 7479 2600 0000 7324 0000 0008 0108  lity&...s$......
-00000750: 010c 011c 0108 010e 0104 0110 0108 0110  ................
-00000760: 0110 0108 0102 021e 0104 0102 8002 fa04  ................
-00000770: 0772 3200 0000 6301 0000 0000 0000 0000  .r2...c.........
-00000780: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
-00000790: 2800 0000 6401 6400 6c00 7d01 7c01 6a01  (...d.d.l.}.|.j.
-000007a0: 6a02 6a03 a004 7c00 6402 1900 a101 7312  j.j...|.d.....s.
-000007b0: 7405 6403 8301 8201 6400 5300 2904 4e72  t.d.....d.S.).Nr
-000007c0: 0100 0000 da04 7469 6d65 7a2b 5469 6d65  ......timez+Time
-000007d0: 2063 6f6c 756d 6e20 636f 756c 6420 6e6f   column could no
-000007e0: 7420 6265 2070 6172 7365 6420 6173 2064  t be parsed as d
-000007f0: 6174 6574 696d 6529 06da 1970 616e 6461  atetime)...panda
-00000800: 732e 636f 7265 2e64 7479 7065 732e 636f  s.core.dtypes.co
-00000810: 6d6d 6f6e da04 636f 7265 da06 6474 7970  mmon..core..dtyp
-00000820: 6573 da06 636f 6d6d 6f6e da13 6973 5f64  es..common..is_d
-00000830: 6174 6574 696d 6536 345f 6474 7970 6572  atetime64_dtyper
-00000840: 1300 0000 2902 721e 0000 00da 0670 616e  ....).r......pan
-00000850: 6461 7372 0d00 0000 720d 0000 0072 0e00  dasr....r....r..
-00000860: 0000 da11 6368 6563 6b5f 7469 6d65 5f63  ....check_time_c
-00000870: 6f6c 756d 6e3a 0000 0073 0800 0000 0801  olumn:...s......
-00000880: 1401 0801 04ff 723a 0000 004e 2911 da0e  ......r:...N)...
-00000890: 6d64 6174 612e 636f 7265 2e72 6177 7202  mdata.core.rawr.
-000008a0: 0000 0072 0300 0000 7204 0000 0072 0500  ...r....r....r..
-000008b0: 0000 7206 0000 00da 0945 7863 6570 7469  ..r......Excepti
-000008c0: 6f6e 7208 0000 0072 1000 0000 7211 0000  onr....r....r...
-000008d0: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
-000008e0: 7215 0000 0072 1c00 0000 7232 0000 0072  r....r....r2...r
-000008f0: 3a00 0000 720d 0000 0072 0d00 0000 720d  :...r....r....r.
-00000900: 0000 0072 0e00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000910: 653e 0100 0000 7316 0000 001c 0010 0410  e>....s.........
-00000920: 0410 0410 0410 0410 0410 0408 0412 0512  ................
-00000930: 14                                       .
+000000a0: 8400 640d 6508 8303 5a0c 4700 640e 640f  ..d.e...Z.G.d.d.
+000000b0: 8400 640f 6509 8303 5a0d 4700 6410 6411  ..d.e...Z.G.d.d.
+000000c0: 8400 6411 6509 8303 5a0e 6412 6413 8400  ..d.e...Z.d.d...
+000000d0: 5a0f 6414 6501 6415 6502 6604 6416 6417  Z.d.e.d.e.f.d.d.
+000000e0: 8404 5a10 6415 6502 6602 6418 6419 8404  ..Z.d.e.f.d.d...
+000000f0: 5a11 641a 5300 291b e900 0000 0029 05da  Z.d.S.)......)..
+00000100: 0d52 6177 4865 6164 6572 5479 7065 da0b  .RawHeaderType..
+00000110: 5261 7744 6174 6154 7970 65da 1663 7265  RawDataType..cre
+00000120: 6174 655f 6865 6164 6572 5f66 726f 6d5f  ate_header_from_
+00000130: 7261 77da 1867 656e 5f66 6561 7475 7265  raw..gen_feature
+00000140: 5f63 6f6c 756d 6e5f 6e61 6d65 73da 1d62  _column_names..b
+00000150: 6173 655f 7261 775f 6d61 6368 696e 655f  ase_raw_machine_
+00000160: 6461 7461 5f63 6f6c 756d 6e73 6300 0000  data_columnsc...
+00000170: 0000 0000 0000 0000 0000 0000 0001 0000  ................
+00000180: 0040 0000 00f3 0c00 0000 6500 5a01 6400  .@........e.Z.d.
+00000190: 5a02 6401 5300 2902 da19 5661 6c69 6469  Z.d.S.)...Validi
+000001a0: 7479 4368 6563 6b69 6e67 4578 6365 7074  tyCheckingExcept
+000001b0: 696f 6e4e a903 da08 5f5f 6e61 6d65 5f5f  ionN....__name__
+000001c0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+000001d0: 7175 616c 6e61 6d65 5f5f a900 720d 0000  qualname__..r...
+000001e0: 0072 0d00 0000 fa55 433a 5c55 7365 7273  .r.....UC:\Users
+000001f0: 5c4c 6561 685c 5079 6368 6172 6d50 726f  \Leah\PycharmPro
+00000200: 6a65 6374 735c 6d64 6174 615c 7372 635c  jects\mdata\src\
+00000210: 6d64 6174 615c 6669 6c65 5f66 6f72 6d61  mdata\file_forma
+00000220: 7473 5c76 616c 6964 6974 795f 6368 6563  ts\validity_chec
+00000230: 6b69 6e67 5f75 7469 6c73 2e70 7972 0800  king_utils.pyr..
+00000240: 0000 0500 0000 f304 0000 0008 0004 0172  ...............r
+00000250: 0800 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000260: 0000 0000 0001 0000 0040 0000 0072 0700  .........@...r..
+00000270: 0000 2902 da1a 5379 6e74 6163 7469 6356  ..)...SyntacticV
+00000280: 616c 6964 6974 7945 7863 6570 7469 6f6e  alidityException
+00000290: 4e72 0900 0000 720d 0000 0072 0d00 0000  Nr....r....r....
+000002a0: 720d 0000 0072 0e00 0000 7210 0000 0009  r....r....r.....
+000002b0: 0000 0072 0f00 0000 7210 0000 0063 0000  ...r....r....c..
+000002c0: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+000002d0: 0000 4000 0000 7207 0000 0029 02da 1953  ..@...r....)...S
+000002e0: 656d 616e 7469 6356 616c 6964 6974 7945  emanticValidityE
+000002f0: 7863 6570 7469 6f6e 4e72 0900 0000 720d  xceptionNr....r.
+00000300: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000310: 0000 7211 0000 000d 0000 0072 0f00 0000  ..r........r....
+00000320: 7211 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000330: 0000 0000 0000 0100 0000 4000 0000 7207  ..........@...r.
+00000340: 0000 0029 02da 1b55 6e73 7570 706f 7274  ...)...Unsupport
+00000350: 6564 4865 6164 6572 4669 6c65 466f 726d  edHeaderFileForm
+00000360: 6174 4e72 0900 0000 720d 0000 0072 0d00  atNr....r....r..
+00000370: 0000 720d 0000 0072 0e00 0000 7212 0000  ..r....r....r...
+00000380: 0011 0000 0072 0f00 0000 7212 0000 0063  .....r....r....c
+00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000003a0: 0100 0000 4000 0000 7207 0000 0029 02da  ....@...r....)..
+000003b0: 1c4d 616c 666f 726d 6564 4865 6164 6572  .MalformedHeader
+000003c0: 4669 6c65 4578 6365 7074 696f 6e4e 7209  FileExceptionNr.
+000003d0: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
+000003e0: 0000 720e 0000 0072 1300 0000 1500 0000  ..r....r........
+000003f0: 720f 0000 0072 1300 0000 6300 0000 0000  r....r....c.....
+00000400: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+00000410: 0000 0072 0700 0000 2902 da1a 4d61 6c66  ...r....)...Malf
+00000420: 6f72 6d65 6444 6174 6146 696c 6545 7863  ormedDataFileExc
+00000430: 6570 7469 6f6e 4e72 0900 0000 720d 0000  eptionNr....r...
+00000440: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
+00000450: 7214 0000 0019 0000 0072 0f00 0000 7214  r........r....r.
+00000460: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000470: 0000 0000 0100 0000 4000 0000 7207 0000  ........@...r...
+00000480: 0029 02da 1249 6e73 7566 6669 6369 656e  .)...Insufficien
+00000490: 7448 6561 6465 724e 7209 0000 0072 0d00  tHeaderNr....r..
+000004a0: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+000004b0: 0072 1500 0000 1d00 0000 720f 0000 0072  .r........r....r
+000004c0: 1500 0000 6300 0000 0000 0000 0000 0000  ....c...........
+000004d0: 0000 0000 0001 0000 0040 0000 0072 0700  .........@...r..
+000004e0: 0000 2902 da1a 496e 636f 6e73 6973 7465  ..)...Inconsiste
+000004f0: 6e74 5469 6d65 7365 7269 6573 5479 7065  ntTimeseriesType
+00000500: 4e72 0900 0000 720d 0000 0072 0d00 0000  Nr....r....r....
+00000510: 720d 0000 0072 0e00 0000 7216 0000 0021  r....r....r....!
+00000520: 0000 0072 0f00 0000 7216 0000 0063 0100  ...r....r....c..
+00000530: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00000540: 0000 4300 0000 7310 0000 0064 0164 0284  ..C...s....d.d..
+00000550: 007c 006a 0044 0083 0153 0029 034e 6301  .|.j.D...S.).Nc.
+00000560: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000570: 0000 0053 0000 0073 1800 0000 6700 7c00  ...S...s....g.|.
+00000580: 5d08 7d01 7c01 7400 7601 7202 7c01 9102  ].}.|.t.v.r.|...
+00000590: 7102 5300 720d 0000 0029 0172 0600 0000  q.S.r....).r....
+000005a0: 2902 da02 2e30 da01 6372 0d00 0000 720d  )....0..cr....r.
+000005b0: 0000 0072 0e00 0000 da0a 3c6c 6973 7463  ...r......<listc
+000005c0: 6f6d 703e 2600 0000 7302 0000 0018 007a  omp>&...s......z
+000005d0: 2867 6574 5f70 6c61 6365 686f 6c64 6572  (get_placeholder
+000005e0: 5f63 6f6c 732e 3c6c 6f63 616c 733e 2e3c  _cols.<locals>.<
+000005f0: 6c69 7374 636f 6d70 3e29 01da 0763 6f6c  listcomp>)...col
+00000600: 756d 6e73 2901 da02 6466 720d 0000 0072  umns)...dfr....r
+00000610: 0d00 0000 720e 0000 00da 1467 6574 5f70  ....r......get_p
+00000620: 6c61 6365 686f 6c64 6572 5f63 6f6c 7325  laceholder_cols%
+00000630: 0000 0073 0200 0000 1001 721c 0000 00da  ...s......r.....
+00000640: 0668 6561 6465 72da 0464 6174 6163 0200  .header..datac..
+00000650: 0000 0000 0000 0000 0000 0c00 0000 0500  ................
+00000660: 0000 4300 0000 73be 0000 0074 007c 0083  ..C...s....t.|..
+00000670: 017d 0074 017c 0183 017d 0274 0274 037c  .}.t.|...}.t.t.|
+00000680: 0283 0183 017d 037c 01a0 0464 0164 0267  .....}.|...d.d.g
+00000690: 02a1 016a 05a0 06a1 0044 005d 445c 027d  ...j.....D.]D\.}
+000006a0: 047d 057c 045c 027d 067d 077c 067c 0766  .}.|.\.}.}.|.|.f
+000006b0: 027c 006a 0776 0172 2974 0882 017c 006a  .|.j.v.r)t...|.j
+000006c0: 077c 067c 0766 0219 006a 097d 0874 037c  .|.|.f...j.}.t.|
+000006d0: 0883 017d 0974 0a7c 0283 0144 005d 225c  ...}.t.|...D.]"\
+000006e0: 027d 0a7d 0b7c 0b7c 037c 0a19 006b 0273  .}.}.|.|.|...k.s
+000006f0: 454a 0082 017c 0a7c 096b 0072 4a09 007c  EJ...|.|.k.rJ..|
+00000700: 0a7c 096b 0572 5b7c 016a 0b7c 057c 0b66  .|.k.r[|.j.|.|.f
+00000710: 0219 00a0 0ca1 00a0 0da1 0073 5b74 0e82  ...........s[t..
+00000720: 0171 3971 1864 0353 0029 044e da04 7479  .q9q.d.S.).N..ty
+00000730: 7065 da05 6c61 6265 6c54 290f 7204 0000  pe..labelT).r...
+00000740: 0072 1c00 0000 7205 0000 00da 036c 656e  .r....r......len
+00000750: da07 6772 6f75 7062 79da 0667 726f 7570  ..groupby..group
+00000760: 73da 0569 7465 6d73 da13 6665 6174 7572  s..items..featur
+00000770: 655f 6465 6669 6e69 7469 6f6e 7372 1500  e_definitionsr..
+00000780: 0000 da08 6665 6174 7572 6573 da09 656e  ....features..en
+00000790: 756d 6572 6174 65da 036c 6f63 da04 6973  umerate..loc..is
+000007a0: 6e61 da03 616c 6c72 1600 0000 290c 721d  na..allr....).r.
+000007b0: 0000 0072 1e00 0000 da10 706c 6163 6568  ...r......placeh
+000007c0: 6f6c 6465 725f 636f 6c73 da0a 746f 5f62  older_cols..to_b
+000007d0: 655f 636f 6c73 da05 6772 6f75 70da 0369  e_cols..group..i
+000007e0: 6478 da03 7470 7972 2000 0000 da01 66da  dx..tpyr .....f.
+000007f0: 0566 5f6c 656e da01 6972 1800 0000 720d  .f_len..ir....r.
+00000800: 0000 0072 0d00 0000 720e 0000 00da 1f63  ...r....r......c
+00000810: 6865 636b 5f68 6561 6465 725f 6461 7461  heck_header_data
+00000820: 5f63 6f6d 7061 7469 6269 6c69 7479 2900  _compatibility).
+00000830: 0000 7324 0000 0008 0108 010c 011c 0108  ..s$............
+00000840: 010e 0104 0110 0108 0110 0110 0108 0102  ................
+00000850: 021e 0104 0102 8002 fa04 0772 3300 0000  ...........r3...
+00000860: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000870: 0004 0000 0043 0000 0073 2800 0000 6401  .....C...s(...d.
+00000880: 6400 6c00 7d01 7c01 6a01 6a02 6a03 a004  d.l.}.|.j.j.j...
+00000890: 7c00 6402 1900 a101 7312 7405 6403 8301  |.d.....s.t.d...
+000008a0: 8201 6400 5300 2904 4e72 0100 0000 da04  ..d.S.).Nr......
+000008b0: 7469 6d65 7a2b 5469 6d65 2063 6f6c 756d  timez+Time colum
+000008c0: 6e20 636f 756c 6420 6e6f 7420 6265 2070  n could not be p
+000008d0: 6172 7365 6420 6173 2064 6174 6574 696d  arsed as datetim
+000008e0: 6529 06da 1970 616e 6461 732e 636f 7265  e)...pandas.core
+000008f0: 2e64 7479 7065 732e 636f 6d6d 6f6e da04  .dtypes.common..
+00000900: 636f 7265 da06 6474 7970 6573 da06 636f  core..dtypes..co
+00000910: 6d6d 6f6e da17 6973 5f64 6174 6574 696d  mmon..is_datetim
+00000920: 6536 345f 616e 795f 6474 7970 6572 1400  e64_any_dtyper..
+00000930: 0000 2902 721e 0000 00da 0670 616e 6461  ..).r......panda
+00000940: 7372 0d00 0000 720d 0000 0072 0e00 0000  sr....r....r....
+00000950: da11 6368 6563 6b5f 7469 6d65 5f63 6f6c  ..check_time_col
+00000960: 756d 6e3d 0000 0073 0800 0000 0801 1401  umn=...s........
+00000970: 0801 04ff 723b 0000 004e 2912 da0e 6d64  ....r;...N)...md
+00000980: 6174 612e 636f 7265 2e72 6177 7202 0000  ata.core.rawr...
+00000990: 0072 0300 0000 7204 0000 0072 0500 0000  .r....r....r....
+000009a0: 7206 0000 00da 0945 7863 6570 7469 6f6e  r......Exception
+000009b0: 7208 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
+000009c0: 1200 0000 7213 0000 0072 1400 0000 7215  ....r....r....r.
+000009d0: 0000 0072 1600 0000 721c 0000 0072 3300  ...r....r....r3.
+000009e0: 0000 723b 0000 0072 0d00 0000 720d 0000  ..r;...r....r...
+000009f0: 0072 0d00 0000 720e 0000 00da 083c 6d6f  .r....r......<mo
+00000a00: 6475 6c65 3e01 0000 0073 1800 0000 1c00  dule>....s......
+00000a10: 1004 1004 1004 1004 1004 1004 1004 1004  ................
+00000a20: 0804 1204 1214                           ......
```

### Comparing `mdata-0.1.0/src/mdata/file_formats/csv/__pycache__/exporting.cpython-310.pyc` & `mdata-0.1.1/src/mdata/file_formats/csv/__pycache__/exporting.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May  3 09:08:07 2023 UTC, .py size: 1368 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,105 +1,151 @@
-00000000: 6f0d 0d0a 0000 0000 7724 5264 5805 0000  o.......w$RdX...
+00000000: 6f0d 0d0a 0000 0000 17af 5c64 0d09 0000  o.........\d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a04 0100 6400 6403 6c02  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6405 6406 6c08 6d09 5a09 0100 6407  ..d.d.l.m.Z...d.
 00000070: 6505 6a0a 6602 6408 6409 8404 5a0b 6407  e.j.f.d.d...Z.d.
 00000080: 6505 6a0a 6602 640a 640b 8404 5a0c 640c  e.j.f.d.d...Z.d.
-00000090: 6505 6a0d 6602 640d 640e 8404 5a0e 6413  e.j.f.d.d...Z.d.
+00000090: 6505 6a0d 6602 640d 640e 8404 5a0e 6417  e.j.f.d.d...Z.d.
 000000a0: 6410 6504 6a0f 6602 6411 6412 8405 5a10  d.e.j.f.d.d...Z.
-000000b0: 6401 5300 2914 e900 0000 004e 2901 da10  d.S.)......N)...
-000000c0: 6d61 6368 696e 655f 6461 7461 5f64 6566  machine_data_def
-000000d0: 2901 da03 7261 7729 01da 0869 6f5f 7574  )...raw)...io_ut
-000000e0: 696c 73e9 0100 0000 2901 da10 6d6b 5f66  ils.....)...mk_f
-000000f0: 696c 656e 616d 655f 7061 6972 da06 6865  ilename_pair..he
-00000100: 6164 6572 6302 0000 0000 0000 0000 0000  aderc...........
-00000110: 0007 0000 0008 0000 0043 0000 0073 8000  .........C...s..
-00000120: 0000 7400 a001 7c00 a101 0100 7400 a002  ..t...|.....t...
-00000130: 7c00 6401 a102 7d00 7403 7c00 6402 8302  |.d...}.t.|.d...
-00000140: 8f26 7d02 7404 6a05 7c02 6403 6404 8d02  .&}.t.j.|.d.d...
-00000150: 7d03 7c01 a006 a100 4400 5d11 5c02 5c02  }.|.....D.].\.\.
-00000160: 7d04 7d05 7d06 7c03 a007 7c04 7c05 6702  }.}.}.|...|.|.g.
-00000170: 7408 7c06 8301 1700 a101 0100 711c 5700  t.|.........q.W.
-00000180: 6400 0400 0400 8303 0100 6400 5300 3100  d.........d.S.1.
-00000190: 7339 7701 0100 0100 0100 5900 0100 6400  s9w.......Y...d.
-000001a0: 5300 2905 4efa 042e 6373 76da 0177 da05  S.).N...csv..w..
-000001b0: 6578 6365 6c29 01da 0764 6961 6c65 6374  excel)...dialect
-000001c0: 2909 7204 0000 00da 1765 6e73 7572 655f  ).r......ensure_
-000001d0: 6469 7265 6374 6f72 795f 6578 6973 7473  directory_exists
-000001e0: da0a 656e 7375 7265 5f65 7874 da04 6f70  ..ensure_ext..op
-000001f0: 656e da03 6373 76da 0677 7269 7465 72da  en..csv..writer.
-00000200: 0569 7465 6d73 da08 7772 6974 6572 6f77  .items..writerow
-00000210: da04 6c69 7374 2907 da04 7061 7468 7207  ..list)...pathr.
-00000220: 0000 005a 0763 7376 6669 6c65 7210 0000  ...Z.csvfiler...
-00000230: 00da 0374 7079 da05 6c61 6265 6cda 0a61  ...tpy..label..a
-00000240: 7474 7269 6275 7465 73a9 0072 1800 0000  ttributes..r....
-00000250: fa4b 433a 5c55 7365 7273 5c4c 6561 685c  .KC:\Users\Leah\
-00000260: 5079 6368 6172 6d50 726f 6a65 6374 735c  PycharmProjects\
-00000270: 6d64 6174 615c 7372 635c 6d64 6174 615c  mdata\src\mdata\
-00000280: 6669 6c65 5f66 6f72 6d61 7473 5c63 7376  file_formats\csv
-00000290: 5c65 7870 6f72 7469 6e67 2e70 79da 1077  \exporting.py..w
-000002a0: 7269 7465 5f72 6177 5f68 6561 6465 720a  rite_raw_header.
-000002b0: 0000 0073 1000 0000 0a01 0c01 0c01 0e01  ...s............
-000002c0: 1401 1801 02ff 22fe 721a 0000 0063 0200  ......".r....c..
-000002d0: 0000 0000 0000 0000 0000 0300 0000 0800  ................
-000002e0: 0000 4300 0000 7352 0000 0074 00a0 017c  ..C...sR...t...|
-000002f0: 00a1 0101 0074 00a0 027c 0064 01a1 027d  .....t...|.d...}
-00000300: 0074 037c 0064 0283 028f 0f7d 0274 04a0  .t.|.d.....}.t..
-00000310: 057c 017c 02a1 0201 0057 0064 0004 0004  .|.|.....W.d....
-00000320: 0083 0301 0064 0053 0031 0073 2277 0101  .....d.S.1.s"w..
-00000330: 0001 0001 0059 0001 0064 0053 0029 034e  .....Y...d.S.).N
-00000340: 7a05 2e6a 736f 6e72 0900 0000 2906 7204  z..jsonr....).r.
-00000350: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000360: 0000 da04 6a73 6f6e da04 6475 6d70 2903  ....json..dump).
-00000370: 7214 0000 0072 0700 0000 da04 6669 6c65  r....r......file
-00000380: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-00000390: 1577 7269 7465 5f72 6177 5f68 6561 6465  .write_raw_heade
-000003a0: 725f 6a73 6f6e 1300 0000 730a 0000 000a  r_json....s.....
-000003b0: 010c 010c 010e 0122 ff72 1e00 0000 da02  .......".r......
-000003c0: 6466 6302 0000 0000 0000 0000 0000 0002  dfc.............
-000003d0: 0000 0004 0000 0043 0000 0073 2800 0000  .......C...s(...
-000003e0: 7400 a001 7c00 a101 0100 7400 a002 7c00  t...|.....t...|.
-000003f0: 6401 a102 7d00 7c01 6a03 7c00 6402 6403  d...}.|.j.|.d.d.
-00000400: 8d02 0100 6400 5300 2904 4e72 0800 0000  ....d.S.).Nr....
-00000410: 4629 01da 0569 6e64 6578 2904 7204 0000  F)...index).r...
-00000420: 0072 0c00 0000 720d 0000 00da 0674 6f5f  .r....r......to_
-00000430: 6373 7629 0272 1400 0000 721f 0000 0072  csv).r....r....r
-00000440: 1800 0000 7218 0000 0072 1900 0000 da0e  ....r....r......
-00000450: 7772 6974 655f 7261 775f 6461 7461 1a00  write_raw_data..
-00000460: 0000 7306 0000 000a 010c 0112 0172 2200  ..s..........r".
-00000470: 0000 720f 0000 00da 026d 6463 0300 0000  ..r......mdc....
-00000480: 0000 0000 0000 0000 0600 0000 0500 0000  ................
-00000490: 4300 0000 7354 0000 0074 007c 007c 0264  C...sT...t.|.|.d
-000004a0: 018d 025c 027d 037d 0474 01a0 027c 01a1  ...\.}.}.t...|..
-000004b0: 017d 057c 0264 026b 0272 1774 037c 037c  .}.|.d.k.r.t.|.|
-000004c0: 0583 0201 006e 097c 0264 036b 0272 2074  .....n.|.d.k.r t
-000004d0: 047c 007c 0583 0201 0074 057c 0474 01a0  .|.|.....t.|.t..
-000004e0: 067c 01a1 0183 0201 0064 0053 0029 044e  .|.......d.S.).N
-000004f0: 2901 da0b 6865 6164 6572 5f74 7970 6572  )...header_typer
-00000500: 0f00 0000 721b 0000 0029 0772 0600 0000  ....r....).r....
-00000510: 7203 0000 00da 1563 6f6e 7665 7274 5f74  r......convert_t
-00000520: 6f5f 7261 775f 6865 6164 6572 721a 0000  o_raw_headerr...
-00000530: 0072 1e00 0000 7222 0000 00da 1363 6f6e  .r....r".....con
-00000540: 7665 7274 5f74 6f5f 7261 775f 6461 7461  vert_to_raw_data
-00000550: 2906 7214 0000 0072 2300 0000 7224 0000  ).r....r#...r$..
-00000560: 00da 0b68 6561 6465 725f 6669 6c65 da09  ...header_file..
-00000570: 6461 7461 5f66 696c 65da 0a72 6177 5f68  data_file..raw_h
-00000580: 6561 6465 7272 1800 0000 7218 0000 0072  eaderr....r....r
-00000590: 1900 0000 da12 7772 6974 655f 6d61 6368  ......write_mach
-000005a0: 696e 655f 6461 7461 2000 0000 730e 0000  ine_data ...s...
-000005b0: 0010 010a 0108 010c 0108 010a 0114 0172  ...............r
-000005c0: 2a00 0000 2901 720f 0000 0029 1172 0f00  *...).r....).r..
-000005d0: 0000 721b 0000 00da 0a6d 6461 7461 2e63  ..r......mdata.c
-000005e0: 6f72 6572 0200 0000 da03 6d64 6472 0300  orer......mddr..
-000005f0: 0000 5a12 6d64 6174 612e 6669 6c65 5f66  ..Z.mdata.file_f
-00000600: 6f72 6d61 7473 7204 0000 00da 0673 6861  ormatsr......sha
-00000610: 7265 6472 0600 0000 da0d 5261 7748 6561  redr......RawHea
-00000620: 6465 7254 7970 6572 1a00 0000 721e 0000  derTyper....r...
-00000630: 00da 0b52 6177 4461 7461 5479 7065 7222  ...RawDataTyper"
-00000640: 0000 00da 0b4d 6163 6869 6e65 4461 7461  .....MachineData
-00000650: 722a 0000 0072 1800 0000 7218 0000 0072  r*...r....r....r
-00000660: 1800 0000 7219 0000 00da 083c 6d6f 6475  ....r......<modu
-00000670: 6c65 3e01 0000 0073 1400 0000 0800 0801  le>....s........
-00000680: 0c02 0c01 0c01 0c01 1003 1009 1007 1606  ................
+000000b0: 6417 6410 6504 6a0f 6602 6413 6414 8405  d.d.e.j.f.d.d...
+000000c0: 5a11 6410 6504 6a0f 6602 6415 6416 8404  Z.d.e.j.f.d.d...
+000000d0: 5a12 6401 5300 2918 e900 0000 004e 2901  Z.d.S.)......N).
+000000e0: da10 6d61 6368 696e 655f 6461 7461 5f64  ..machine_data_d
+000000f0: 6566 2901 da03 7261 7729 01da 0869 6f5f  ef)...raw)...io_
+00000100: 7574 696c 73e9 0100 0000 2901 da10 6d6b  utils.....)...mk
+00000110: 5f66 696c 656e 616d 655f 7061 6972 da06  _filename_pair..
+00000120: 6865 6164 6572 6302 0000 0000 0000 0000  headerc.........
+00000130: 0000 0008 0000 0008 0000 0043 0000 0073  ...........C...s
+00000140: 8600 0000 7400 a001 7c00 a101 0100 7400  ....t...|.....t.
+00000150: a002 7c00 6401 a102 7d00 7403 7c00 6402  ..|.d...}.t.|.d.
+00000160: 6403 6404 6405 8d04 8f26 7d02 7404 a005  d.d.d....&}.t...
+00000170: 7c02 a101 7d03 7c01 a006 a100 4400 5d13  |...}.|.....D.].
+00000180: 5c02 5c02 7d04 7d05 7d06 7c04 7c05 6702  \.\.}.}.}.|.|.g.
+00000190: 7407 7c06 8301 1700 7d07 7c03 a008 7c07  t.|.....}.|...|.
+000001a0: a101 0100 711d 5700 6400 0400 0400 8303  ....q.W.d.......
+000001b0: 0100 6400 5300 3100 733c 7701 0100 0100  ..d.S.1.s<w.....
+000001c0: 0100 5900 0100 6400 5300 2906 4efa 042e  ..Y...d.S.).N...
+000001d0: 6373 76da 0177 da00 7a05 7574 662d 3829  csv..w..z.utf-8)
+000001e0: 02da 076e 6577 6c69 6e65 da08 656e 636f  ...newline..enco
+000001f0: 6469 6e67 2909 7204 0000 00da 1765 6e73  ding).r......ens
+00000200: 7572 655f 6469 7265 6374 6f72 795f 6578  ure_directory_ex
+00000210: 6973 7473 da0a 656e 7375 7265 5f65 7874  ists..ensure_ext
+00000220: da04 6f70 656e da03 6373 76da 0677 7269  ..open..csv..wri
+00000230: 7465 72da 0569 7465 6d73 da04 6c69 7374  ter..items..list
+00000240: da08 7772 6974 6572 6f77 2908 da04 7061  ..writerow)...pa
+00000250: 7468 7207 0000 005a 0763 7376 6669 6c65  thr....Z.csvfile
+00000260: 7211 0000 00da 0374 7079 da05 6c61 6265  r......tpy..labe
+00000270: 6cda 0a61 7474 7269 6275 7465 73da 0372  l..attributes..r
+00000280: 6f77 a900 721a 0000 00fa 4b43 3a5c 5573  ow..r.....KC:\Us
+00000290: 6572 735c 4c65 6168 5c50 7963 6861 726d  ers\Leah\Pycharm
+000002a0: 5072 6f6a 6563 7473 5c6d 6461 7461 5c73  Projects\mdata\s
+000002b0: 7263 5c6d 6461 7461 5c66 696c 655f 666f  rc\mdata\file_fo
+000002c0: 726d 6174 735c 6373 765c 6578 706f 7274  rmats\csv\export
+000002d0: 696e 672e 7079 da10 7772 6974 655f 7261  ing.py..write_ra
+000002e0: 775f 6865 6164 6572 0a00 0000 7312 0000  w_header....s...
+000002f0: 000a 010c 0112 010a 0114 0110 010c 0102  ................
+00000300: fe22 fe72 1c00 0000 6302 0000 0000 0000  .".r....c.......
+00000310: 0000 0000 0006 0000 0008 0000 0043 0000  .............C..
+00000320: 0073 c400 0000 7400 a001 7c00 a101 0100  .s....t...|.....
+00000330: 7400 a002 7c00 6401 a102 7d00 7403 7c00  t...|.d...}.t.|.
+00000340: 6402 8302 8f48 7d02 6900 6900 6403 9c02  d....H}.i.i.d...
+00000350: 7d03 7c01 a004 a100 4400 5d2f 5c02 7d04  }.|.....D.]/\.}.
+00000360: 7d05 7c04 6404 1900 7405 6a06 7405 6a07  }.|.d...t.j.t.j.
+00000370: 6a08 1900 6b02 7234 7409 7c05 8301 7c03  j...k.r4t.|...|.
+00000380: 6405 1900 7c04 6406 1900 3c00 711a 7c04  d...|.d...<.q.|.
+00000390: 6404 1900 7405 6a06 7405 6a07 6a0a 1900  d...t.j.t.j.j...
+000003a0: 6b02 7249 7409 7c05 8301 7c03 6407 1900  k.rIt.|...|.d...
+000003b0: 7c04 6406 1900 3c00 711a 740b a00c 7c03  |.d...<.q.t...|.
+000003c0: 7c02 a102 0100 5700 6400 0400 0400 8303  |.....W.d.......
+000003d0: 0100 6400 5300 3100 735b 7701 0100 0100  ..d.S.1.s[w.....
+000003e0: 0100 5900 0100 6400 5300 2908 4e7a 052e  ..Y...d.S.).Nz..
+000003f0: 6a73 6f6e 7209 0000 0029 02fa 0b65 7665  jsonr....)...eve
+00000400: 6e74 2d74 7970 6573 fa11 6d65 6173 7572  nt-types..measur
+00000410: 656d 656e 742d 7479 7065 7372 0100 0000  ement-typesr....
+00000420: 721d 0000 0072 0500 0000 721e 0000 0029  r....r....r....)
+00000430: 0d72 0400 0000 720d 0000 0072 0e00 0000  .r....r....r....
+00000440: 720f 0000 0072 1200 0000 7203 0000 00da  r....r....r.....
+00000450: 174d 4143 4849 4e45 5f44 4154 415f 5459  .MACHINE_DATA_TY
+00000460: 5045 535f 4449 4354 da10 4d61 6368 696e  PES_DICT..Machin
+00000470: 6544 6174 6154 7970 6573 da01 4572 1300  eDataTypes..Er..
+00000480: 0000 da01 4dda 046a 736f 6eda 0464 756d  ....M..json..dum
+00000490: 7029 0672 1500 0000 7207 0000 00da 0466  p).r....r......f
+000004a0: 696c 65da 0372 6573 5a06 7474 5f6b 6579  ile..resZ.tt_key
+000004b0: da02 6673 721a 0000 0072 1a00 0000 721b  ..fsr....r....r.
+000004c0: 0000 00da 1577 7269 7465 5f72 6177 5f68  .....write_raw_h
+000004d0: 6561 6465 725f 6a73 6f6e 1400 0000 7318  eader_json....s.
+000004e0: 0000 000a 010c 010c 010a 0110 0116 0116  ................
+000004f0: 0116 0114 0102 800e 0122 f972 2800 0000  .........".r(...
+00000500: da02 6466 6302 0000 0000 0000 0000 0000  ..dfc...........
+00000510: 0002 0000 0004 0000 0043 0000 0073 2800  .........C...s(.
+00000520: 0000 7400 a001 7c00 a101 0100 7400 a002  ..t...|.....t...
+00000530: 7c00 6401 a102 7d00 7c01 6a03 7c00 6402  |.d...}.|.j.|.d.
+00000540: 6403 8d02 0100 6400 5300 2904 4e72 0800  d.....d.S.).Nr..
+00000550: 0000 4629 01da 0569 6e64 6578 2904 7204  ..F)...index).r.
+00000560: 0000 0072 0d00 0000 720e 0000 00da 0674  ...r....r......t
+00000570: 6f5f 6373 7629 0272 1500 0000 7229 0000  o_csv).r....r)..
+00000580: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00000590: da0e 7772 6974 655f 7261 775f 6461 7461  ..write_raw_data
+000005a0: 2100 0000 7306 0000 000a 010c 0112 0172  !...s..........r
+000005b0: 2c00 0000 7210 0000 00da 026d 6463 0300  ,...r......mdc..
+000005c0: 0000 0000 0000 0000 0000 0600 0000 0500  ................
+000005d0: 0000 4300 0000 7354 0000 0074 007c 007c  ..C...sT...t.|.|
+000005e0: 0264 018d 025c 027d 037d 0474 01a0 027c  .d...\.}.}.t...|
+000005f0: 01a1 017d 057c 0264 026b 0272 1774 037c  ...}.|.d.k.r.t.|
+00000600: 037c 0583 0201 006e 097c 0264 036b 0272  .|.....n.|.d.k.r
+00000610: 2074 047c 037c 0583 0201 0074 057c 0474   t.|.|.....t.|.t
+00000620: 01a0 067c 01a1 0183 0201 0064 0053 00a9  ...|.......d.S..
+00000630: 044e 2901 da0b 6865 6164 6572 5f74 7970  .N)...header_typ
+00000640: 6572 1000 0000 7223 0000 0029 0772 0600  er....r#...).r..
+00000650: 0000 7203 0000 00da 1563 6f6e 7665 7274  ..r......convert
+00000660: 5f74 6f5f 7261 775f 6865 6164 6572 721c  _to_raw_headerr.
+00000670: 0000 0072 2800 0000 722c 0000 00da 1363  ...r(...r,.....c
+00000680: 6f6e 7665 7274 5f74 6f5f 7261 775f 6461  onvert_to_raw_da
+00000690: 7461 2906 7215 0000 0072 2d00 0000 722f  ta).r....r-...r/
+000006a0: 0000 00da 0b68 6561 6465 725f 6669 6c65  .....header_file
+000006b0: da09 6461 7461 5f66 696c 65da 0a72 6177  ..data_file..raw
+000006c0: 5f68 6561 6465 7272 1a00 0000 721a 0000  _headerr....r...
+000006d0: 0072 1b00 0000 da12 7772 6974 655f 6d61  .r......write_ma
+000006e0: 6368 696e 655f 6461 7461 2700 0000 730e  chine_data'...s.
+000006f0: 0000 0010 010a 0108 010c 0108 010a 0114  ................
+00000700: 0172 3500 0000 6303 0000 0000 0000 0000  .r5...c.........
+00000710: 0000 0006 0000 0004 0000 0043 0000 0073  ...........C...s
+00000720: 4a00 0000 7400 7c00 7c02 6401 8d02 5c02  J...t.|.|.d...\.
+00000730: 7d03 7d04 7401 a002 7c01 a101 7d05 7c02  }.}.t...|...}.|.
+00000740: 6402 6b02 7218 7403 7c03 7c05 8302 0100  d.k.r.t.|.|.....
+00000750: 6400 5300 7c02 6403 6b02 7223 7404 7c03  d.S.|.d.k.r#t.|.
+00000760: 7c05 8302 0100 6400 5300 6400 5300 722e  |.....d.S.d.S.r.
+00000770: 0000 0029 0572 0600 0000 7203 0000 0072  ...).r....r....r
+00000780: 3000 0000 721c 0000 0072 2800 0000 2906  0...r....r(...).
+00000790: 7215 0000 0072 2d00 0000 722f 0000 0072  r....r-...r/...r
+000007a0: 3200 0000 da01 5f72 3400 0000 721a 0000  2....._r4...r...
+000007b0: 0072 1a00 0000 721b 0000 00da 1177 7269  .r....r......wri
+000007c0: 7465 5f68 6561 6465 725f 6f6e 6c79 3100  te_header_only1.
+000007d0: 0000 730e 0000 0010 010a 0108 010e 0108  ..s.............
+000007e0: 010e 0104 ff72 3700 0000 6302 0000 0000  .....r7...c.....
+000007f0: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
+00000800: 0000 0073 2000 0000 7400 7c00 8301 5c02  ...s ...t.|...\.
+00000810: 7d02 7d03 7401 7c03 7402 a003 7c01 a101  }.}.t.|.t...|...
+00000820: 8302 0100 6400 5300 2901 4e29 0472 0600  ....d.S.).N).r..
+00000830: 0000 722c 0000 0072 0300 0000 7231 0000  ..r,...r....r1..
+00000840: 0029 0472 1500 0000 722d 0000 0072 3600  .).r....r-...r6.
+00000850: 0000 7233 0000 0072 1a00 0000 721a 0000  ..r3...r....r...
+00000860: 0072 1b00 0000 da0f 7772 6974 655f 6461  .r......write_da
+00000870: 7461 5f6f 6e6c 793a 0000 0073 0400 0000  ta_only:...s....
+00000880: 0c01 1401 7238 0000 0029 0172 1000 0000  ....r8...).r....
+00000890: 2913 7210 0000 0072 2300 0000 da0a 6d64  ).r....r#.....md
+000008a0: 6174 612e 636f 7265 7202 0000 00da 036d  ata.corer......m
+000008b0: 6464 7203 0000 005a 126d 6461 7461 2e66  ddr....Z.mdata.f
+000008c0: 696c 655f 666f 726d 6174 7372 0400 0000  ile_formatsr....
+000008d0: da06 7368 6172 6564 7206 0000 00da 0d52  ..sharedr......R
+000008e0: 6177 4865 6164 6572 5479 7065 721c 0000  awHeaderTyper...
+000008f0: 0072 2800 0000 da0b 5261 7744 6174 6154  .r(.....RawDataT
+00000900: 7970 6572 2c00 0000 da0b 4d61 6368 696e  yper,.....Machin
+00000910: 6544 6174 6172 3500 0000 7237 0000 0072  eDatar5...r7...r
+00000920: 3800 0000 721a 0000 0072 1a00 0000 721a  8...r....r....r.
+00000930: 0000 0072 1b00 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000940: 653e 0100 0000 7318 0000 0008 0008 010c  e>....s.........
+00000950: 020c 010c 010c 0110 0310 0a10 0d12 0612  ................
+00000960: 0a14 09                                  ...
```

### Comparing `mdata-0.1.0/src/mdata/file_formats/csv/checking.py` & `mdata-0.1.1/src/mdata/file_formats/csv/checking.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import csv
-
 from mdata.core.raw import raw_machine_data_types
-from .importing import read_raw_data, read_machine_data, read_machine_data_from_canonical_basename, read_raw_header
+from .importing import read_raw_data, read_machine_data, read_machine_data_from_canonical_basename
 from .. import io_utils
 from ..validity_checking_utils import *
 
 
 def is_valid_canonical_file_pair(base_path):
     try:
         read_machine_data_from_canonical_basename(base_path, validity_checking=True)
@@ -18,44 +16,68 @@
     try:
         read_machine_data(header_path, data_path, validity_checking=True)
     except ValidityCheckingException:
         return False
     return True
 
 
-def check_if_valid_header_definition_file(path):
+def check_if_readable_header_definition_file(path):
     seen_labels = set()
-    for row in io_utils.read_csv_lines_from(path):
+    try:
+        lines_from = io_utils.read_csv_lines_from(path)
+    except Exception as e:
+        raise MalformedHeaderFileException('Unparsable csv: ' + str(e) + '.')
+    for row in lines_from:
+        key = tuple(row[:2])
         if len(row) < 2:
             raise MalformedHeaderFileException('Incomplete timeseries type specification.')
-        if row[0] not in raw_machine_data_types:
-            raise MalformedHeaderFileException('Unrecognized observation type.')
-        key = row[0], row[1]
         if key in seen_labels:
             raise MalformedHeaderFileException('Duplicate timeseries type specification.')
         seen_labels.add(key)
-    raw = read_raw_header(path)
-    check_if_valid_raw_header(raw)
+    return True
+
+
+def check_if_readable_header_definition_file_json(path):
+    d = io_utils.read_json_dict_from(path)
+    if d is None:
+        raise MalformedHeaderFileException('Unparsable json.')
+    for typ in ['event-types', 'measurement-types']:
+        seen_labels = set()
+        if typ in d:
+            for label in d[typ]:
+                if label in seen_labels:
+                    # json load swallows duplicates, so this can never happen
+                    raise MalformedHeaderFileException('Duplicate timeseries type specification.')
+                seen_labels.add(label)
+                if not isinstance(d[typ][label], list):
+                    raise MalformedHeaderFileException('Incomplete timeseries type specification.')
     return True
 
 
 def check_if_valid_raw_header(raw_header):
-    if any(v is None for v in raw_header.values()):
-        raise MalformedHeaderFileException('Empty timeseries type specification.')
+    seen_labels = set()
+    for key, fs in raw_header.items():
+        typ, label = key
+        if fs is None:
+            raise MalformedHeaderFileException('Empty timeseries type specification.')
+        if typ not in raw_machine_data_types:
+            raise MalformedHeaderFileException('Unrecognized observation type.')
+        seen_labels.add(key)
     return True
 
 
 def check_if_valid_data_file(path):
     df = read_raw_data(path)
     check_if_valid_raw_data(df)
     return True
 
 
 def check_if_valid_raw_data(df):
     if any(c not in df.columns for c in base_raw_machine_data_columns):
-        raise MalformedDataFileException(f'Data is missing base column(s): {set(base_raw_machine_data_columns) - set(df.columns)}.')
+        raise MalformedDataFileException(
+            f'Data is missing base column(s): {set(base_raw_machine_data_columns) - set(df.columns)}.')
     check_time_column(df)
     placeholder_cols = get_placeholder_cols(df)
     to_be_cols = gen_feature_column_names(len(placeholder_cols))
     if any(a != b for a, b in zip(placeholder_cols, to_be_cols)):
         raise MalformedDataFileException('Placeholder feature columns have unexpected labels.')
     return True
```

### Comparing `mdata-0.1.0/src/mdata/file_formats/csv/exporting.py` & `mdata-0.1.1/src/mdata/file_formats/csv/exporting.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,34 +6,55 @@
 from mdata.file_formats import io_utils
 from .shared import mk_filename_pair
 
 
 def write_raw_header(path, header: raw.RawHeaderType):
     io_utils.ensure_directory_exists(path)
     path = io_utils.ensure_ext(path, '.csv')
-    with open(path, 'w') as csvfile:
-        writer = csv.writer(csvfile, dialect='excel')
+    with open(path, 'w', newline='', encoding='utf-8') as csvfile:
+        writer = csv.writer(csvfile)
         for (tpy, label), attributes in header.items():
-            writer.writerow([tpy, label] + list(attributes))
+            row = [tpy, label] + list(attributes)
+            writer.writerow(row)
 
 
 def write_raw_header_json(path, header: raw.RawHeaderType):
     io_utils.ensure_directory_exists(path)
     path = io_utils.ensure_ext(path, '.json')
     with open(path, 'w') as file:
-        json.dump(header, file)
+        res = {'event-types': {}, 'measurement-types': {}}
+        for tt_key, fs in header.items():
+            if tt_key[0] == raw.MACHINE_DATA_TYPES_DICT[raw.MachineDataTypes.E]:
+                res['event-types'][tt_key[1]] = list(fs)
+            elif tt_key[0] == raw.MACHINE_DATA_TYPES_DICT[raw.MachineDataTypes.M]:
+                res['measurement-types'][tt_key[1]] = list(fs)
+        json.dump(res, file)
 
 
 def write_raw_data(path, df: raw.RawDataType):
     io_utils.ensure_directory_exists(path)
     path = io_utils.ensure_ext(path, '.csv')
     df.to_csv(path, index=False)
 
 
 def write_machine_data(path, md: mdd.MachineData, header_type='csv'):
     header_file, data_file = mk_filename_pair(path, header_type=header_type)
     raw_header = raw.convert_to_raw_header(md)
     if header_type == 'csv':
         write_raw_header(header_file, raw_header)
     elif header_type == 'json':
-        write_raw_header_json(path, raw_header)
+        write_raw_header_json(header_file, raw_header)
+    write_raw_data(data_file, raw.convert_to_raw_data(md))
+
+
+def write_header_only(path, md: mdd.MachineData, header_type='csv'):
+    header_file, _ = mk_filename_pair(path, header_type=header_type)
+    raw_header = raw.convert_to_raw_header(md)
+    if header_type == 'csv':
+        write_raw_header(header_file, raw_header)
+    elif header_type == 'json':
+        write_raw_header_json(header_file, raw_header)
+
+
+def write_data_only(path, md: mdd.MachineData):
+    _, data_file = mk_filename_pair(path)
     write_raw_data(data_file, raw.convert_to_raw_data(md))
```

### Comparing `mdata-0.1.0/src/mdata/file_formats/csv/importing.py` & `mdata-0.1.1/src/mdata/file_formats/csv/importing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,77 @@
 import json
+import os.path
+from typing import Literal
 
 import pandas as pd
 
-from mdata.core import machine_data_def as mdd, raw
+from mdata.core import machine_data_def as mdd
 from mdata.core import raw
 from mdata.file_formats import io_utils
 from mdata.file_formats.csv.shared import mk_filename_pair
 
 
 def read_raw_data(path) -> raw.RawDataType:
     # path = ensure_ext(path, '.csv', override_ext=False)
     df = pd.read_csv(path)
     df[raw.COLUMN_NAME_DICT[raw.MDConcepts.Time]] = pd.to_datetime(
         df[raw.COLUMN_NAME_DICT[raw.MDConcepts.Time]])
     return df
 
 
-def read_machine_data(header_path, data_path, validity_checking=True, header_type='csv') -> mdd.MachineData:
+def read_machine_data(header_path, data_path, validity_checking=True, header_type: Literal['infer', 'csv', 'json']='infer') -> mdd.MachineData:
+    if header_type == 'infer':
+        header_type = os.path.splitext(header_path)[1][1:]
+    if header_type not in ['csv', 'json']:
+        from mdata.file_formats.validity_checking_utils import UnsupportedHeaderFileFormat
+        raise UnsupportedHeaderFileFormat(header_type)
     if validity_checking:
         if header_type == 'csv':
-            from .checking import check_if_valid_header_definition_file
-            check_if_valid_header_definition_file(header_path)
+            from .checking import check_if_readable_header_definition_file
+            check_if_readable_header_definition_file(header_path)
+        if header_type == 'json':
+            from .checking import check_if_readable_header_definition_file_json
+            check_if_readable_header_definition_file_json(header_path)
 
     raw_header: raw.RawHeaderType = None
     if header_type == 'csv':
         raw_header = read_raw_header(header_path)
     elif header_type == 'json':
         raw_header = read_raw_header_json(header_path)
+
+    if validity_checking:
+        from .checking import check_if_valid_raw_header
+        check_if_valid_raw_header(raw_header)
+
     raw_data = read_raw_data(data_path)
 
     if validity_checking:
-        from .checking import check_if_valid_raw_header, check_if_valid_raw_data
+        from .checking import check_if_valid_raw_data
         from mdata.file_formats.validity_checking_utils import check_header_data_compatibility
-        check_if_valid_raw_header(raw_header)
         check_if_valid_raw_data(raw_data)
         check_header_data_compatibility(raw_header, raw_data)
 
     return raw.create_machine_data_from_raw(raw_data, raw_header)
 
 
-def read_machine_data_from_canonical_basename(basepath, validity_checking=True, header_type='csv') -> mdd.MachineData:
+def read_machine_data_from_canonical_basename(basepath, validity_checking=True, header_type: Literal['csv', 'json']='csv') -> mdd.MachineData:
     header_file, data_file = mk_filename_pair(basepath, header_type=header_type)
     return read_machine_data(header_file, data_file, validity_checking=validity_checking, header_type=header_type)
 
 
 def read_raw_header_json(path) -> raw.RawHeaderType:
-    return json.load(path)
+    d = io_utils.read_json_dict_from(path)
+    res = {}
+    if 'event-types' in d:
+        for et, fs in d['event-types'].items():
+            res[raw.MACHINE_DATA_TYPES_DICT[raw.MachineDataTypes.E], et] = tuple(fs)
+    if 'measurement-types' in d:
+        for mt, fs in d['measurement-types'].items():
+            res[raw.MACHINE_DATA_TYPES_DICT[raw.MachineDataTypes.M], mt] = tuple(fs)
+    return res
 
 
 def read_raw_header(path) -> raw.RawHeaderType:
     metadata = {}
     for row in io_utils.read_csv_lines_from(path):
         metadata[row[0], row[1]] = tuple(row[2:]) if len(row) > 2 else []
     return metadata
```

### Comparing `mdata-0.1.0/src/mdata/file_formats/hdf/importing.py` & `mdata-0.1.1/src/mdata/file_formats/hdf/importing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import pandas as pd
 
-from mdata.file_formats import io_utils
 from mdata.core import machine_data_def as mdd
 
+
 def read_machine_data_h5(filename) -> mdd.MachineData:
     # ext = io_utils.ensure_ext(filename, '.h5', override_ext=False)
     with pd.HDFStore(filename, mode='r') as store:
         measurements, events = [], []
         rel_groups = next(store.walk('/'))[1]
         if 'events' in rel_groups:
             (path, groups, leaves) = next(store.walk('/events'))
             for label in leaves:
                 key = '/'.join([path, label])
                 df: pd.DataFrame = store.get(key)
-                ets = mdd.EventTimeseriesCollection(mdd.EventTimeseriesType(label, mdd.only_feature_columns(df.columns)),
-                                                    df)
+                ets = mdd.EventTimeseriesCollection(
+                    mdd.EventTimeseriesType(label, mdd.only_feature_columns(df.columns)),
+                    df)
                 events.append(ets)
         if 'measurements' in rel_groups:
             (path, groups, leaves) = next(store.walk('/measurements'))
             for label in leaves:
                 key = '/'.join([path, label])
                 df: pd.DataFrame = store.get(key)
                 mts = mdd.MeasurementTimeseriesCollection(
```

### Comparing `mdata-0.1.0/src/mdata/file_formats/validity_checking_utils.py` & `mdata-0.1.1/src/mdata/file_formats/validity_checking_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,18 @@
     pass
 
 
 class SemanticValidityException(ValidityCheckingException):
     pass
 
 
+class UnsupportedHeaderFileFormat(SyntacticValidityException):
+    pass
+
+
 class MalformedHeaderFileException(SyntacticValidityException):
     pass
 
 
 class MalformedDataFileException(SyntacticValidityException):
     pass
 
@@ -27,16 +31,15 @@
 
 
 class InconsistentTimeseriesType(SemanticValidityException):
     pass
 
 
 def get_placeholder_cols(df):
-    placeholder_cols = sorted(set(df.columns).difference(base_raw_machine_data_columns))
-    return placeholder_cols
+    return [c for c in df.columns if c not in base_raw_machine_data_columns]
 
 
 def check_header_data_compatibility(header: RawHeaderType, data: RawDataType):
     header = create_header_from_raw(header)
     placeholder_cols = get_placeholder_cols(data)
     to_be_cols = gen_feature_column_names(len(placeholder_cols))
     for group, idx in data.groupby(['type', 'label']).groups.items():
@@ -53,9 +56,9 @@
             if i >= f_len and not data.loc[idx, c].isna().all():
                 raise InconsistentTimeseriesType
     return True
 
 
 def check_time_column(data: RawDataType):
     import pandas.core.dtypes.common
-    if not pandas.core.dtypes.common.is_datetime64_dtype(data['time']):
+    if not pandas.core.dtypes.common.is_datetime64_any_dtype(data['time']):
         raise MalformedDataFileException('Time column could not be parsed as datetime')
```

### Comparing `mdata-0.1.0/PKG-INFO` & `mdata-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: mdata
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Keywords: data format,machine data
 Author: Leah Tacke genannt Unterberg
 Author-email: leah.tgu@pads.rwth-aachen.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bokeh (>=2.4.3,<3.0.0)
+Requires-Dist: bottleneck
 Requires-Dist: jupyter (>=1.0,<2.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: pandas[all,performance] (>=1.5,<2.0)
-Requires-Dist: plotly (>=5.14.1,<6.0.0)
-Requires-Dist: pm4py (>=2.7.3,<3.0.0)
+Requires-Dist: numba
+Requires-Dist: numexpr
+Requires-Dist: pandas (>=1.5,<2.0)
+Requires-Dist: plotly (>=5.15,<6.0)
+Requires-Dist: seaborn
 Requires-Dist: tables (>=3.8.0,<4.0.0)
 Requires-Dist: tsdownsample (>=0.1.2,<0.2.0)
 Description-Content-Type: text/markdown
 
 This is the official machine data format package.
 
 It supports csv importing, exporting and format compliance checking.
 Machine data is parsed into a python object that provides typed views on the contained measurement and event timeseries.
 
+For a brief overview, see [machine_data_format.pdf](files/info/machine_data_format.pdf).
```

