# Comparing `tmp/micrompn-1.0.0.tar.gz` & `tmp/micrompn-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micrompn-1.0.0.tar", last modified: Thu Jun  8 19:59:53 2023, max compression
+gzip compressed data, was "micrompn-1.0.1.tar", last modified: Mon Jun 12 15:05:47 2023, max compression
```

## Comparing `micrompn-1.0.0.tar` & `micrompn-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,57 @@
-drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-08 19:59:53.043253 micrompn-1.0.0/
-drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-08 19:59:52.965708 micrompn-1.0.0/.github/
-drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-08 19:59:52.983001 micrompn-1.0.0/.github/workflows/
--rw-r--r--   0 rivers     (503) staff       (20)     1349 2023-06-08 16:56:07.000000 micrompn-1.0.0/.github/workflows/python-package.yml
--rw-r--r--   0 rivers     (503) staff       (20)     1393 2023-06-08 19:31:14.000000 micrompn-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 rivers     (503) staff       (20)        0 2023-06-08 18:58:15.000000 micrompn-1.0.0/MANIFEST.in
--rw-r--r--   0 rivers     (503) staff       (20)     8190 2023-06-08 19:59:53.042114 micrompn-1.0.0/PKG-INFO
--rw-r--r--   0 rivers     (503) staff       (20)     7533 2023-06-08 18:18:30.000000 micrompn-1.0.0/README.md
--rw-r--r--   0 rivers     (503) staff       (20)     6908 2023-04-07 10:36:45.000000 micrompn-1.0.0/licence.txt
-drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-08 19:59:52.998848 micrompn-1.0.0/micrompn/
--rw-r--r--   0 rivers     (503) staff       (20)      107 2023-06-08 18:52:49.000000 micrompn-1.0.0/micrompn/__init__.py
--rw-r--r--   0 rivers     (503) staff       (20)      160 2023-06-08 19:59:52.000000 micrompn-1.0.0/micrompn/_version.py
-drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-08 19:59:53.034437 micrompn-1.0.0/micrompn/data/
--rw-r--r--   0 rivers     (503) staff       (20)     2141 2023-04-26 15:35:56.000000 micrompn-1.0.0/micrompn/data/example1-output.csv
--rw-r--r--   0 rivers     (503) staff       (20)      400 2023-04-05 18:32:20.000000 micrompn-1.0.0/micrompn/data/example1_mapfile.toml
--rw-r--r--   0 rivers     (503) staff       (20)    83557 2023-04-10 14:57:36.000000 micrompn-1.0.0/micrompn/data/example1_plate_data.csv
--rw-r--r--   0 rivers     (503) staff       (20)    13984 2023-06-08 18:54:43.000000 micrompn-1.0.0/micrompn/main.py
--rw-r--r--   0 rivers     (503) staff       (20)    21909 2023-06-01 18:35:02.000000 micrompn-1.0.0/micrompn/mpn.py
-drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-08 19:59:53.027249 micrompn-1.0.0/micrompn.egg-info/
--rw-r--r--   0 rivers     (503) staff       (20)     8190 2023-06-08 19:59:52.000000 micrompn-1.0.0/micrompn.egg-info/PKG-INFO
--rw-r--r--   0 rivers     (503) staff       (20)      553 2023-06-08 19:59:52.000000 micrompn-1.0.0/micrompn.egg-info/SOURCES.txt
--rw-r--r--   0 rivers     (503) staff       (20)        1 2023-06-08 19:59:52.000000 micrompn-1.0.0/micrompn.egg-info/dependency_links.txt
--rw-r--r--   0 rivers     (503) staff       (20)       43 2023-06-08 19:59:52.000000 micrompn-1.0.0/micrompn.egg-info/entry_points.txt
--rw-r--r--   0 rivers     (503) staff       (20)       38 2023-06-08 19:59:52.000000 micrompn-1.0.0/micrompn.egg-info/requires.txt
--rw-r--r--   0 rivers     (503) staff       (20)        9 2023-06-08 19:59:52.000000 micrompn-1.0.0/micrompn.egg-info/top_level.txt
--rw-r--r--   0 rivers     (503) staff       (20)      985 2023-06-08 19:00:01.000000 micrompn-1.0.0/pyproject.toml
--rw-r--r--   0 rivers     (503) staff       (20)       90 2023-06-08 16:24:22.000000 micrompn-1.0.0/requirements.txt
--rw-r--r--   0 rivers     (503) staff       (20)       38 2023-06-08 19:59:53.043563 micrompn-1.0.0/setup.cfg
-drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-08 19:59:53.038974 micrompn-1.0.0/tests/
--rw-r--r--   0 rivers     (503) staff       (20)     4939 2023-06-01 19:04:09.000000 micrompn-1.0.0/tests/test_main.py
--rw-r--r--   0 rivers     (503) staff       (20)     8469 2023-06-08 16:52:34.000000 micrompn-1.0.0/tests/test_mpn.py
+drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-12 15:05:47.924329 micrompn-1.0.1/
+drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-12 15:05:47.608783 micrompn-1.0.1/.github/
+drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-12 15:05:47.686823 micrompn-1.0.1/.github/workflows/
+-rw-r--r--   0 rivers     (503) staff       (20)     1503 2023-06-12 14:38:28.000000 micrompn-1.0.1/.github/workflows/gchr-deploy.yml
+-rw-r--r--   0 rivers     (503) staff       (20)     1349 2023-06-08 16:56:07.000000 micrompn-1.0.1/.github/workflows/python-package.yml
+-rw-r--r--   0 rivers     (503) staff       (20)      264 2023-06-12 15:00:20.000000 micrompn-1.0.1/CHANGELOG.md
+-rw-r--r--   0 rivers     (503) staff       (20)       33 2023-06-12 13:27:13.000000 micrompn-1.0.1/MANIFEST.in
+-rw-r--r--   0 rivers     (503) staff       (20)     8273 2023-06-12 15:05:47.923171 micrompn-1.0.1/PKG-INFO
+-rw-r--r--   0 rivers     (503) staff       (20)     7616 2023-06-12 13:25:07.000000 micrompn-1.0.1/README.md
+drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-12 15:05:47.692854 micrompn-1.0.1/docker/
+-rw-r--r--   0 rivers     (503) staff       (20)      378 2023-06-12 14:22:55.000000 micrompn-1.0.1/docker/Dockerfile
+-rw-r--r--   0 rivers     (503) staff       (20)     6908 2023-04-07 10:36:45.000000 micrompn-1.0.1/licence.txt
+drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-12 15:05:47.751930 micrompn-1.0.1/micrompn/
+-rw-r--r--   0 rivers     (503) staff       (20)      107 2023-06-08 18:52:49.000000 micrompn-1.0.1/micrompn/__init__.py
+-rw-r--r--   0 rivers     (503) staff       (20)      160 2023-06-12 15:05:47.000000 micrompn-1.0.1/micrompn/_version.py
+drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-12 15:05:47.792143 micrompn-1.0.1/micrompn/data/
+drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-12 15:05:47.617725 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/
+drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-12 15:05:47.617050 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_384_mock/
+drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-12 15:05:47.818143 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_384_mock/384_4_samples/
+-rw-r--r--   0 rivers     (503) staff       (20)    10590 2023-06-12 13:25:07.000000 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_384_mock/384_4_samples/384_4_samples_horizontal_dilutions.csv
+-rw-r--r--   0 rivers     (503) staff       (20)      478 2023-06-12 13:25:07.000000 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_384_mock/384_4_samples/OUTFILE_384_4_samples_horizontal_dilutions.csv
+-rw-r--r--   0 rivers     (503) staff       (20)     1258 2023-06-12 13:25:07.000000 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_384_mock/384_4_samples/microplate_384_4_samples_horizontal_dilutions.txt
+drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-12 15:05:47.841148 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_384_mock/384_6_samples/
+-rw-r--r--   0 rivers     (503) staff       (20)    10110 2023-06-12 13:25:07.000000 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_384_mock/384_6_samples/384_6_samples_vertical_dilutions.csv
+-rw-r--r--   0 rivers     (503) staff       (20)      688 2023-06-12 13:25:07.000000 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_384_mock/384_6_samples/OUTFILE_384_6_samples_vertical_dilutions.csv
+-rw-r--r--   0 rivers     (503) staff       (20)     1288 2023-06-12 13:25:07.000000 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_384_mock/384_6_samples/microplate_384_6_samples_vertical_dilutions.txt
+drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-12 15:05:47.619570 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_96_mock/
+drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-12 15:05:47.862814 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_96_mock/96_2_samples_horizontal_dilutions/
+-rw-r--r--   0 rivers     (503) staff       (20)     2530 2023-06-12 13:25:07.000000 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_96_mock/96_2_samples_horizontal_dilutions/96_2_samples_horizontal_dilutions.csv
+-rw-r--r--   0 rivers     (503) staff       (20)      170 2023-06-12 13:25:07.000000 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_96_mock/96_2_samples_horizontal_dilutions/OUTFILE_96_2_samples_horizontal_dilutions.csv
+-rw-r--r--   0 rivers     (503) staff       (20)      813 2023-06-12 13:25:07.000000 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_96_mock/96_2_samples_horizontal_dilutions/microplate_96_2_samples_horizontal_dilutions.txt
+drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-12 15:05:47.869094 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_96_mock/96_2_samples_vertical_dilutions/
+-rw-r--r--   0 rivers     (503) staff       (20)     2530 2023-06-12 13:25:07.000000 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_96_mock/96_2_samples_vertical_dilutions/96_2_samples_vertical_dilutions.csv
+drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-12 15:05:47.895994 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_96_mock/96_3_samples_vertical_dilutions/
+-rw-r--r--   0 rivers     (503) staff       (20)     2530 2023-06-12 13:25:07.000000 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_96_mock/96_3_samples_vertical_dilutions/96_3_samples_vertical_dilutions.csv
+-rw-r--r--   0 rivers     (503) staff       (20)      254 2023-06-12 13:25:07.000000 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_96_mock/96_3_samples_vertical_dilutions/OUTFILE_96_2_samples_vertical_dilutions.csv
+-rw-r--r--   0 rivers     (503) staff       (20)      232 2023-06-12 13:25:07.000000 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_96_mock/96_3_samples_vertical_dilutions/OUTFILE_96_3_samples_vertical_dilutions.csv
+-rw-r--r--   0 rivers     (503) staff       (20)      795 2023-06-12 13:25:07.000000 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_96_mock/96_3_samples_vertical_dilutions/microplate_96_2_samples_vertical_dilutions.txt
+-rw-r--r--   0 rivers     (503) staff       (20)      825 2023-06-12 13:25:07.000000 micrompn-1.0.1/micrompn/data/additional_plate_layout_examples/micrompn_96_mock/96_3_samples_vertical_dilutions/microplate_96_3_samples_vertical_dilutions.txt
+-rw-r--r--   0 rivers     (503) staff       (20)     2141 2023-04-26 15:35:56.000000 micrompn-1.0.1/micrompn/data/example1-output.csv
+-rw-r--r--   0 rivers     (503) staff       (20)      400 2023-04-05 18:32:20.000000 micrompn-1.0.1/micrompn/data/example1_mapfile.toml
+-rw-r--r--   0 rivers     (503) staff       (20)    83557 2023-04-10 14:57:36.000000 micrompn-1.0.1/micrompn/data/example1_plate_data.csv
+-rw-r--r--   0 rivers     (503) staff       (20)    13984 2023-06-08 18:54:43.000000 micrompn-1.0.1/micrompn/main.py
+-rw-r--r--   0 rivers     (503) staff       (20)    21909 2023-06-01 18:35:02.000000 micrompn-1.0.1/micrompn/mpn.py
+drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-12 15:05:47.769190 micrompn-1.0.1/micrompn.egg-info/
+-rw-r--r--   0 rivers     (503) staff       (20)     8273 2023-06-12 15:05:47.000000 micrompn-1.0.1/micrompn.egg-info/PKG-INFO
+-rw-r--r--   0 rivers     (503) staff       (20)     2578 2023-06-12 15:05:47.000000 micrompn-1.0.1/micrompn.egg-info/SOURCES.txt
+-rw-r--r--   0 rivers     (503) staff       (20)        1 2023-06-12 15:05:47.000000 micrompn-1.0.1/micrompn.egg-info/dependency_links.txt
+-rw-r--r--   0 rivers     (503) staff       (20)       43 2023-06-12 15:05:47.000000 micrompn-1.0.1/micrompn.egg-info/entry_points.txt
+-rw-r--r--   0 rivers     (503) staff       (20)       38 2023-06-12 15:05:47.000000 micrompn-1.0.1/micrompn.egg-info/requires.txt
+-rw-r--r--   0 rivers     (503) staff       (20)        9 2023-06-12 15:05:47.000000 micrompn-1.0.1/micrompn.egg-info/top_level.txt
+-rw-r--r--   0 rivers     (503) staff       (20)     1030 2023-06-12 13:35:57.000000 micrompn-1.0.1/pyproject.toml
+-rw-r--r--   0 rivers     (503) staff       (20)       90 2023-06-08 16:24:22.000000 micrompn-1.0.1/requirements.txt
+-rw-r--r--   0 rivers     (503) staff       (20)       38 2023-06-12 15:05:47.924593 micrompn-1.0.1/setup.cfg
+drwxr-xr-x   0 rivers     (503) staff       (20)        0 2023-06-12 15:05:47.921516 micrompn-1.0.1/tests/
+-rw-r--r--   0 rivers     (503) staff       (20)     4939 2023-06-01 19:04:09.000000 micrompn-1.0.1/tests/test_main.py
+-rw-r--r--   0 rivers     (503) staff       (20)     8469 2023-06-08 16:52:34.000000 micrompn-1.0.1/tests/test_mpn.py
```

### Comparing `micrompn-1.0.0/.github/workflows/python-package.yml` & `micrompn-1.0.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `micrompn-1.0.0/PKG-INFO` & `micrompn-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: micrompn
-Version: 1.0.0
+Version: 1.0.1
 Summary: MicroMPN: Software to estimate Most Probable Number (MPN) bacterial abundance from microplates. 
 Author-email: "Adam R. Rivers" <adam.rivers@usda.gov>
 License: CC0
 Keywords: microbiology,mpn
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 [![Python package](https://github.com/USDA-ARS-GBRU/micrompn/actions/workflows/python-package.yml/badge.svg)](https://github.com/USDA-ARS-GBRU/micrompn/actions/workflows/python-package.yml)
+[![DOI](https://zenodo.org/badge/632734005.svg)](https://zenodo.org/badge/latestdoi/632734005)
 
 # MicroMPN: Software for automating most probable number (MPN) estimates from laboratory microplates
 
 
 ## Authors
 
 * Adam Rivers, United States Department of Agriculture, Agricultural Research Service
@@ -54,22 +55,26 @@
 Other Microbial Enumeration Techniques. R package version 0.3.0. <https://CRAN.R-project.org/package=MPN> .
 
 
 
 ## Installing
 
 
-The package can be installed from Github 
+1. To install from Github: 
 
 ```bash
   git clone git@github.com:USDA-ARS-GBRU/micrompn.git
   cd micrompn
   pip install .
 ```
+2. To install from PyPI:
 
+```bash
+pip install micrompn
+```
 
 ## Getting Started
 
 MicroMPN uses two types of files, a file specifying the layout of the plate and a file containing the data from the plate reader.
 
 1. ["Wellmap"](https://wellmap.readthedocs.io/en/latest/index.html)
 
@@ -101,20 +106,19 @@
 F.replicate = 6
 G.replicate = 7
 H.replicate = 8
 [block.12x8.'A1']
 sample = 1
 ```
 
-Example of the above TOML layout visualized graphically with the Wellmap command "wellmap.show("microplate.toml")
-
-![wellmap dilution](https://github.com/USDA-ARS-GBRU/MPN-RFU-microplate-assay-data-files/assets/68250738/995e55ca-3df7-4881-a87a-b5e4c57d161a)
+Example of the above TOML layout visualized graphically with the Wellmap command wellmap.show("microplate.toml")
 
-![wellmap replicate](https://github.com/USDA-ARS-GBRU/MPN-RFU-microplate-assay-data-files/assets/68250738/ef4308af-284b-47fa-9dcb-780b83a167ae)
+![wellmap replicate](https://github.com/USDA-ARS-GBRU/micrompn/assets/68250738/59f471f0-74e5-44f3-9518-4b287d439745)
 
+![wellmap dilution](https://github.com/USDA-ARS-GBRU/micrompn/assets/68250738/5a1d4203-f26e-46af-8d8c-24580c84e699)
 
 
 2. Plate reader CSV files
 
 - Plate reader data files vary by instrument but most allow the output of data in tabular format.
 
 - The named columns needed in a CSV are:
```

### Comparing `micrompn-1.0.0/README.md` & `micrompn-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 [![Python package](https://github.com/USDA-ARS-GBRU/micrompn/actions/workflows/python-package.yml/badge.svg)](https://github.com/USDA-ARS-GBRU/micrompn/actions/workflows/python-package.yml)
+[![DOI](https://zenodo.org/badge/632734005.svg)](https://zenodo.org/badge/latestdoi/632734005)
 
 # MicroMPN: Software for automating most probable number (MPN) estimates from laboratory microplates
 
 
 ## Authors
 
 * Adam Rivers, United States Department of Agriculture, Agricultural Research Service
@@ -38,22 +39,26 @@
 Other Microbial Enumeration Techniques. R package version 0.3.0. <https://CRAN.R-project.org/package=MPN> .
 
 
 
 ## Installing
 
 
-The package can be installed from Github 
+1. To install from Github: 
 
 ```bash
   git clone git@github.com:USDA-ARS-GBRU/micrompn.git
   cd micrompn
   pip install .
 ```
+2. To install from PyPI:
 
+```bash
+pip install micrompn
+```
 
 ## Getting Started
 
 MicroMPN uses two types of files, a file specifying the layout of the plate and a file containing the data from the plate reader.
 
 1. ["Wellmap"](https://wellmap.readthedocs.io/en/latest/index.html)
 
@@ -85,20 +90,19 @@
 F.replicate = 6
 G.replicate = 7
 H.replicate = 8
 [block.12x8.'A1']
 sample = 1
 ```
 
-Example of the above TOML layout visualized graphically with the Wellmap command "wellmap.show("microplate.toml")
-
-![wellmap dilution](https://github.com/USDA-ARS-GBRU/MPN-RFU-microplate-assay-data-files/assets/68250738/995e55ca-3df7-4881-a87a-b5e4c57d161a)
+Example of the above TOML layout visualized graphically with the Wellmap command wellmap.show("microplate.toml")
 
-![wellmap replicate](https://github.com/USDA-ARS-GBRU/MPN-RFU-microplate-assay-data-files/assets/68250738/ef4308af-284b-47fa-9dcb-780b83a167ae)
+![wellmap replicate](https://github.com/USDA-ARS-GBRU/micrompn/assets/68250738/59f471f0-74e5-44f3-9518-4b287d439745)
 
+![wellmap dilution](https://github.com/USDA-ARS-GBRU/micrompn/assets/68250738/5a1d4203-f26e-46af-8d8c-24580c84e699)
 
 
 2. Plate reader CSV files
 
 - Plate reader data files vary by instrument but most allow the output of data in tabular format.
 
 - The named columns needed in a CSV are:
```

### Comparing `micrompn-1.0.0/licence.txt` & `micrompn-1.0.1/licence.txt`

 * *Files identical despite different names*

### Comparing `micrompn-1.0.0/micrompn/data/example1-output.csv` & `micrompn-1.0.1/micrompn/data/example1-output.csv`

 * *Files identical despite different names*

### Comparing `micrompn-1.0.0/micrompn/data/example1_plate_data.csv` & `micrompn-1.0.1/micrompn/data/example1_plate_data.csv`

 * *Files identical despite different names*

### Comparing `micrompn-1.0.0/micrompn/main.py` & `micrompn-1.0.1/micrompn/main.py`

 * *Files identical despite different names*

### Comparing `micrompn-1.0.0/micrompn/mpn.py` & `micrompn-1.0.1/micrompn/mpn.py`

 * *Files identical despite different names*

### Comparing `micrompn-1.0.0/micrompn.egg-info/PKG-INFO` & `micrompn-1.0.1/micrompn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: micrompn
-Version: 1.0.0
+Version: 1.0.1
 Summary: MicroMPN: Software to estimate Most Probable Number (MPN) bacterial abundance from microplates. 
 Author-email: "Adam R. Rivers" <adam.rivers@usda.gov>
 License: CC0
 Keywords: microbiology,mpn
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 [![Python package](https://github.com/USDA-ARS-GBRU/micrompn/actions/workflows/python-package.yml/badge.svg)](https://github.com/USDA-ARS-GBRU/micrompn/actions/workflows/python-package.yml)
+[![DOI](https://zenodo.org/badge/632734005.svg)](https://zenodo.org/badge/latestdoi/632734005)
 
 # MicroMPN: Software for automating most probable number (MPN) estimates from laboratory microplates
 
 
 ## Authors
 
 * Adam Rivers, United States Department of Agriculture, Agricultural Research Service
@@ -54,22 +55,26 @@
 Other Microbial Enumeration Techniques. R package version 0.3.0. <https://CRAN.R-project.org/package=MPN> .
 
 
 
 ## Installing
 
 
-The package can be installed from Github 
+1. To install from Github: 
 
 ```bash
   git clone git@github.com:USDA-ARS-GBRU/micrompn.git
   cd micrompn
   pip install .
 ```
+2. To install from PyPI:
 
+```bash
+pip install micrompn
+```
 
 ## Getting Started
 
 MicroMPN uses two types of files, a file specifying the layout of the plate and a file containing the data from the plate reader.
 
 1. ["Wellmap"](https://wellmap.readthedocs.io/en/latest/index.html)
 
@@ -101,20 +106,19 @@
 F.replicate = 6
 G.replicate = 7
 H.replicate = 8
 [block.12x8.'A1']
 sample = 1
 ```
 
-Example of the above TOML layout visualized graphically with the Wellmap command "wellmap.show("microplate.toml")
-
-![wellmap dilution](https://github.com/USDA-ARS-GBRU/MPN-RFU-microplate-assay-data-files/assets/68250738/995e55ca-3df7-4881-a87a-b5e4c57d161a)
+Example of the above TOML layout visualized graphically with the Wellmap command wellmap.show("microplate.toml")
 
-![wellmap replicate](https://github.com/USDA-ARS-GBRU/MPN-RFU-microplate-assay-data-files/assets/68250738/ef4308af-284b-47fa-9dcb-780b83a167ae)
+![wellmap replicate](https://github.com/USDA-ARS-GBRU/micrompn/assets/68250738/59f471f0-74e5-44f3-9518-4b287d439745)
 
+![wellmap dilution](https://github.com/USDA-ARS-GBRU/micrompn/assets/68250738/5a1d4203-f26e-46af-8d8c-24580c84e699)
 
 
 2. Plate reader CSV files
 
 - Plate reader data files vary by instrument but most allow the output of data in tabular format.
 
 - The named columns needed in a CSV are:
```

### Comparing `micrompn-1.0.0/pyproject.toml` & `micrompn-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm[toml]>=7.1.0"]
 build-backend = "setuptools.build_meta"
 
+
+
 [project]
 name = "micrompn"
 authors = [
     {name = "Adam R. Rivers", email = "adam.rivers@usda.gov"},
 ]
 description = "MicroMPN: Software to estimate Most Probable Number (MPN) bacterial abundance from microplates. " 
 
@@ -30,8 +32,11 @@
 ]
 dynamic = ["version"]
 
 [project.scripts]
 micrompn = "micrompn:main"
 
 [tool.setuptools_scm]
-write_to = "micrompn/_version.py"
+write_to = "micrompn/_version.py"
+
+[tool.setuptools]
+packages = ['micrompn']
```

### Comparing `micrompn-1.0.0/tests/test_main.py` & `micrompn-1.0.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `micrompn-1.0.0/tests/test_mpn.py` & `micrompn-1.0.1/tests/test_mpn.py`

 * *Files identical despite different names*

