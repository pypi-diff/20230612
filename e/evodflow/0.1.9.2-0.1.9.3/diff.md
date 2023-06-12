# Comparing `tmp/evodflow-0.1.9.2.tar.gz` & `tmp/evodflow-0.1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evodflow-0.1.9.2.tar", last modified: Sun Jun 11 19:07:52 2023, max compression
+gzip compressed data, was "evodflow-0.1.9.3.tar", last modified: Sun Jun 11 19:15:15 2023, max compression
```

## Comparing `evodflow-0.1.9.2.tar` & `evodflow-0.1.9.3.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.745314 evodflow-0.1.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-11 19:07:52.745314 evodflow-0.1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.737313 evodflow-0.1.9.2/evodflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-11 19:07:52.000000 evodflow-0.1.9.2/evodflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-11 19:07:52.000000 evodflow-0.1.9.2/evodflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:07:52.000000 evodflow-0.1.9.2/evodflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-11 19:07:52.000000 evodflow-0.1.9.2/evodflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-11 19:07:52.000000 evodflow-0.1.9.2/evodflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 19:07:52.000000 evodflow-0.1.9.2/evodflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.741314 evodflow-0.1.9.2/evoflow/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/__info__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.741314 evodflow-0.1.9.2/evoflow/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/controller/common_step_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.741314 evodflow-0.1.9.2/evoflow/controller/data_manipulate/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/controller/data_manipulate/PdfFileOperator.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/controller/data_manipulate/PptxFileOperator.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/controller/data_manipulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/controller/data_manipulate/data_manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/controller/data_manipulate/excel_file_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/controller/data_manipulate/file_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/controller/data_manipulate/image_file_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/controller/log_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/controller/visualize_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.741314 evodflow-0.1.9.2/evoflow/entities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.741314 evodflow-0.1.9.2/evoflow/entities/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.741314 evodflow-0.1.9.2/evoflow/entities/common/step/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/common/step/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.741314 evodflow-0.1.9.2/evoflow/entities/common/step/browser/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/common/step/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/common/step/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.741314 evodflow-0.1.9.2/evoflow/entities/common/step/file_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/common/step/file_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/common/step/open_excel_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.741314 evodflow-0.1.9.2/evoflow/entities/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/core/base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/core/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/core/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/core/step_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/core/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.741314 evodflow-0.1.9.2/evoflow/entities/data_manipulate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/data_manipulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/data_manipulate/abstract_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.745314 evodflow-0.1.9.2/evoflow/entities/data_manipulate/file_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/data_manipulate/file_operator/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/data_manipulate/file_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/data_manipulate/file_operator/dataframe_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/data_manipulate/file_operator/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/data_manipulate/file_operator/image_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/data_manipulate/file_operator/pdf_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/data_manipulate/file_operator/pptx_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.745314 evodflow-0.1.9.2/evoflow/entities/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/exceptions/base_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/exceptions/evo_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/entities/global_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.745314 evodflow-0.1.9.2/evoflow/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/operators/base_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/operators/empty_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/operators/python_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.745314 evodflow-0.1.9.2/evoflow/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/services/abstract_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.745314 evodflow-0.1.9.2/evoflow/services/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/services/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/services/ocr/easy_ocr_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/services/ocr/ocr_service.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/services/ocr/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/services/ocr/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/services/service_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.745314 evodflow-0.1.9.2/evoflow/services/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/services/templates/item.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.745314 evodflow-0.1.9.2/evoflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/utils/create_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/utils/ultilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/evoflow/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 19:07:52.745314 evodflow-0.1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:52.745314 evodflow-0.1.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-11 19:07:40.000000 evodflow-0.1.9.2/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.931380 evodflow-0.1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-11 19:15:15.931380 evodflow-0.1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.923380 evodflow-0.1.9.3/evodflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-11 19:15:15.000000 evodflow-0.1.9.3/evodflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-11 19:15:15.000000 evodflow-0.1.9.3/evodflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:15:15.000000 evodflow-0.1.9.3/evodflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-11 19:15:15.000000 evodflow-0.1.9.3/evodflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-11 19:15:15.000000 evodflow-0.1.9.3/evodflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 19:15:15.000000 evodflow-0.1.9.3/evodflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.923380 evodflow-0.1.9.3/evoflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/__info__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.923380 evodflow-0.1.9.3/evoflow/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/controller/common_step_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.923380 evodflow-0.1.9.3/evoflow/controller/data_manipulate/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/controller/data_manipulate/PdfFileOperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/controller/data_manipulate/PptxFileOperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/controller/data_manipulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/controller/data_manipulate/data_manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/controller/data_manipulate/excel_file_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/controller/data_manipulate/file_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/controller/data_manipulate/image_file_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/controller/log_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/controller/visualize_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.923380 evodflow-0.1.9.3/evoflow/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.927380 evodflow-0.1.9.3/evoflow/entities/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.927380 evodflow-0.1.9.3/evoflow/entities/common/step/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/common/step/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.927380 evodflow-0.1.9.3/evoflow/entities/common/step/browser/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/common/step/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/common/step/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.927380 evodflow-0.1.9.3/evoflow/entities/common/step/file_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/common/step/file_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/common/step/open_excel_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.927380 evodflow-0.1.9.3/evoflow/entities/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/core/base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/core/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/core/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/core/step_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/core/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.927380 evodflow-0.1.9.3/evoflow/entities/data_manipulate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/data_manipulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/data_manipulate/abstract_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.927380 evodflow-0.1.9.3/evoflow/entities/data_manipulate/file_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/data_manipulate/file_operator/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/data_manipulate/file_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/data_manipulate/file_operator/dataframe_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/data_manipulate/file_operator/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/data_manipulate/file_operator/image_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/data_manipulate/file_operator/pdf_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/data_manipulate/file_operator/pptx_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.927380 evodflow-0.1.9.3/evoflow/entities/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/exceptions/base_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/exceptions/evo_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/entities/global_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.927380 evodflow-0.1.9.3/evoflow/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/operators/base_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/operators/empty_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/operators/python_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.927380 evodflow-0.1.9.3/evoflow/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/services/abstract_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.927380 evodflow-0.1.9.3/evoflow/services/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/services/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/services/ocr/easy_ocr_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/services/ocr/ocr_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/services/ocr/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/services/ocr/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/services/service_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.931380 evodflow-0.1.9.3/evoflow/services/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/services/templates/item.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.931380 evodflow-0.1.9.3/evoflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/utils/create_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/utils/ultilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/evoflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 19:15:15.931380 evodflow-0.1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:15.931380 evodflow-0.1.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-11 19:15:04.000000 evodflow-0.1.9.3/tests/test_base.py
```

### Comparing `evodflow-0.1.9.2/LICENSE` & `evodflow-0.1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/PKG-INFO` & `evodflow-0.1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evodflow
-Version: 0.1.9.2
+Version: 0.1.9.3
 Summary: Awesome evoflow created by maycuatroi
 Home-page: https://github.com/maycuatroi/evo-flow/
 Author: maycuatroi
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `evodflow-0.1.9.2/README.md` & `evodflow-0.1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evodflow.egg-info/PKG-INFO` & `evodflow-0.1.9.3/evodflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evodflow
-Version: 0.1.9.2
+Version: 0.1.9.3
 Summary: Awesome evoflow created by maycuatroi
 Home-page: https://github.com/maycuatroi/evo-flow/
 Author: maycuatroi
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `evodflow-0.1.9.2/evodflow.egg-info/SOURCES.txt` & `evodflow-0.1.9.3/evodflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/__init__.py` & `evodflow-0.1.9.3/evoflow/__init__.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/cli.py` & `evodflow-0.1.9.3/evoflow/cli.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/controller/data_manipulate/PdfFileOperator.py` & `evodflow-0.1.9.3/evoflow/controller/data_manipulate/PdfFileOperator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/controller/data_manipulate/PptxFileOperator.py` & `evodflow-0.1.9.3/evoflow/controller/data_manipulate/PptxFileOperator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/controller/data_manipulate/excel_file_operator.py` & `evodflow-0.1.9.3/evoflow/controller/data_manipulate/excel_file_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/controller/data_manipulate/file_operator.py` & `evodflow-0.1.9.3/evoflow/controller/data_manipulate/file_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/controller/data_manipulate/image_file_operator.py` & `evodflow-0.1.9.3/evoflow/controller/data_manipulate/image_file_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/controller/log_controller.py` & `evodflow-0.1.9.3/evoflow/controller/log_controller.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/entities/common/step/__init__.py` & `evodflow-0.1.9.3/evoflow/entities/common/step/__init__.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/entities/common/step/browser/__init__.py` & `evodflow-0.1.9.3/evoflow/entities/common/step/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/entities/common/step/downloader.py` & `evodflow-0.1.9.3/evoflow/entities/common/step/downloader.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/entities/common/step/open_excel_file.py` & `evodflow-0.1.9.3/evoflow/entities/common/step/open_excel_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/entities/core/base_object.py` & `evodflow-0.1.9.3/evoflow/entities/core/base_object.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/entities/core/condition.py` & `evodflow-0.1.9.3/evoflow/entities/core/condition.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/entities/core/job.py` & `evodflow-0.1.9.3/evoflow/entities/core/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,31 +66,29 @@
     def run(self, **kwargs):
         with Live(
             Panel(Columns([]), title=f"Running {self.name}"),
             refresh_per_second=20,
         ) as live:
             # live.update(Panel(spinners, title="Panel 2"))
 
-            # add
+            self.live_panel = live
             while True:
                 # do self.__run by new thread
                 self.__run(live=live, **kwargs)
 
-    def __run(self, live=None, **kwargs):
+    def __run(self, **kwargs):
         self.compile()
         logger.info(f"Running job: {self.name}")
         self.params_pool = kwargs
         step_generator = self.__step_generator()
 
         for step in step_generator:
             log_string = f"Running step : {step}"
             logger.info(log_string)
             step.prepare(**self.params_pool)
-            if live is not None:
-                self.__update_live(live)
             try:
                 action_params = inspect.getfullargspec(step.action).args
                 build_params = {}
                 for param in action_params:
                     if param == "self":
                         continue
                     build_params[param] = step.__dict__.get(param)
@@ -107,14 +105,15 @@
             self.stacks += step.get_next_steps(self.params_pool)
 
         self.finish()
 
         return last_result
 
     def __init__(self, name=None, start_step: Step = None, **kwargs):
+        self.live_panel = None # for progress monitor
         self.current_step = None
         self.__start_step: Step = start_step
         self.params_pool = {}
         self.__steps = []
         self.__running_steps = []
         if name is None:
             name = os.getenv("JOB_NAME")
@@ -243,15 +242,17 @@
 
     def add_running_step(self, step):
         self.__running_steps.append(step)
 
     def remove_running_step(self, step):
         self.__running_steps.remove(step)
 
-    def __update_live(self, live):
+    def update_status(self,**kwargs):
+        if self.live_panel is None:
+            return
         tree = Tree(self.name)
         running_steps = self.__running_steps
 
         tree_added_steps = []
 
         step_lists = [_ for _ in running_steps if isinstance(_, StepList)]
         single_steps = [_ for _ in running_steps if not isinstance(_, Step)]
@@ -269,8 +270,8 @@
                 tree_added_steps.append(sub_step)
         for step in single_steps:
             if step in tree_added_steps:
                 continue
             if step.is_running():
                 tree.add(Spinner("material", text=Text(step.name, style="blue")))
 
-        live.update(Panel(tree, title=f"Running {self.name}"))
+        self.live_panel.update(Panel(tree, title=f"Running {self.name}"))
```

### Comparing `evodflow-0.1.9.2/evoflow/entities/core/step.py` & `evodflow-0.1.9.3/evoflow/entities/core/step.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,25 +94,27 @@
 
     def end(self, **kwargs) -> dict:
         """
         Kết thúc step, kill các object không cần thiết để giải phóng bộ nhớ
         """
         self.status = self.STATUS_SUCCESS
         self.job.remove_running_step(self)
+        self.job.update_status()
         return self.params
 
     def prepare(self, **kwargs):
         """
         Chuẩn bị cho action, hàm prepare giúp chuẩn bị input để đẩy vào action()
         """
         for k, v in kwargs.items():
             setattr(self, k, v)
         self.params = kwargs
         self.job.add_running_step(self)
         self.status = self.STATUS_RUNNING
+        self.job.update_status()
 
     def __str__(self):
         return self.name
 
     def get_next_steps(self, params=None):
         next_steps = []
 
@@ -162,8 +164,8 @@
             self.status = self.STATUS_READY
         return True
 
     def is_running(self):
         """
         Check if step is running
         """
-        return self.status == self.STATUS_RUNNING
+        return self.status == self.STATUS_RUNNING
```

### Comparing `evodflow-0.1.9.2/evoflow/entities/core/step_list.py` & `evodflow-0.1.9.3/evoflow/entities/core/step_list.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/entities/core/transaction.py` & `evodflow-0.1.9.3/evoflow/entities/core/transaction.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/entities/core/workflow.py` & `evodflow-0.1.9.3/evoflow/entities/core/workflow.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/entities/data_manipulate/abstract_data.py` & `evodflow-0.1.9.3/evoflow/entities/data_manipulate/abstract_data.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/entities/data_manipulate/file_operator/dataframe_file.py` & `evodflow-0.1.9.3/evoflow/entities/data_manipulate/file_operator/dataframe_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/entities/data_manipulate/file_operator/file.py` & `evodflow-0.1.9.3/evoflow/entities/data_manipulate/file_operator/file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/entities/data_manipulate/file_operator/image_file.py` & `evodflow-0.1.9.3/evoflow/entities/data_manipulate/file_operator/image_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/entities/data_manipulate/file_operator/pdf_file.py` & `evodflow-0.1.9.3/evoflow/entities/data_manipulate/file_operator/pdf_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/entities/data_manipulate/file_operator/pptx_file.py` & `evodflow-0.1.9.3/evoflow/entities/data_manipulate/file_operator/pptx_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/entities/global_vars.py` & `evodflow-0.1.9.3/evoflow/entities/global_vars.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/operators/base_operator.py` & `evodflow-0.1.9.3/evoflow/operators/base_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/operators/empty_operator.py` & `evodflow-0.1.9.3/evoflow/operators/empty_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/operators/python_operator.py` & `evodflow-0.1.9.3/evoflow/operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/services/ocr/easy_ocr_engine.py` & `evodflow-0.1.9.3/evoflow/services/ocr/easy_ocr_engine.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/services/ocr/ocr_service.py` & `evodflow-0.1.9.3/evoflow/services/ocr/ocr_service.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/services/ocr/result.py` & `evodflow-0.1.9.3/evoflow/services/ocr/result.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/services/service_controller.py` & `evodflow-0.1.9.3/evoflow/services/service_controller.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/evoflow/utils/ultilities.py` & `evodflow-0.1.9.3/evoflow/utils/ultilities.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.9.2/setup.py` & `evodflow-0.1.9.3/setup.py`

 * *Files identical despite different names*

