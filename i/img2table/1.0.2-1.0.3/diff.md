# Comparing `tmp/img2table-1.0.2.tar.gz` & `tmp/img2table-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/img2table-1.0.2.tar", last modified: Mon Jun  5 23:26:18 2023, max compression
+gzip compressed data, was "dist/img2table-1.0.3.tar", last modified: Mon Jun 12 19:39:34 2023, max compression
```

## Comparing `img2table-1.0.2.tar` & `img2table-1.0.3.tar`

### file list

```diff
@@ -1,305 +1,305 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-05 23:23:56.000000 img2table-1.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-05 23:23:56.000000 img2table-1.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-05 23:23:56.000000 img2table-1.0.2/.github/workflows/test_workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-05 23:23:56.000000 img2table-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-05 23:23:56.000000 img2table-1.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-06-05 23:26:18.000000 img2table-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17154 2023-06-05 23:23:56.000000 img2table-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-05 23:23:56.000000 img2table-1.0.2/activate_venv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-06-05 23:23:56.000000 img2table-1.0.2/examples/Basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-06-05 23:23:56.000000 img2table-1.0.2/examples/Implicit_rows.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   727975 2023-06-05 23:23:56.000000 img2table-1.0.2/examples/borderless.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/examples/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/examples/data/borderless/
--rw-r--r--   0 runner    (1001) docker     (123)    47122 2023-06-05 23:23:56.000000 img2table-1.0.2/examples/data/borderless/1.png
--rw-r--r--   0 runner    (1001) docker     (123)   177004 2023-06-05 23:23:56.000000 img2table-1.0.2/examples/data/borderless/2.png
--rw-r--r--   0 runner    (1001) docker     (123)   182800 2023-06-05 23:23:56.000000 img2table-1.0.2/examples/data/borderless/3.png
--rw-r--r--   0 runner    (1001) docker     (123)   132335 2023-06-05 23:23:56.000000 img2table-1.0.2/examples/data/borderless/4.png
--rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-06-05 23:23:56.000000 img2table-1.0.2/examples/data/borderless.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-06-05 23:23:56.000000 img2table-1.0.2/examples/data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-06-05 23:23:56.000000 img2table-1.0.2/examples/data/tables.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-05 23:23:56.000000 img2table-1.0.2/examples/data/tables.png
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-05 23:23:56.000000 img2table-1.0.2/examples/data/tables.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-05 23:23:56.000000 img2table-1.0.2/examples/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 23:23:56.000000 img2table-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-05 23:23:56.000000 img2table-1.0.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-05 23:23:56.000000 img2table-1.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-05 23:23:56.000000 img2table-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-05 23:26:18.000000 img2table-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-05 23:23:56.000000 img2table-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table/document/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/document/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/document/base/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/document/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/document/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/ocr/aws_textract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/ocr/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/ocr/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/ocr/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/ocr/easyocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/ocr/google_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/ocr/paddle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/ocr/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/ocr/tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/objects/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/objects/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/objects/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/objects/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/objects/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/bordered_tables/cells/identification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/bordered_tables/lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/borderless_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table/tables/processing/borderless_tables/column_delimiters/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/borderless_tables/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table/tables/processing/borderless_tables/rows/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/borderless_tables/rows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/borderless_tables/rows/coherency.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/borderless_tables/segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/borderless_tables/table/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/borderless_tables/table/table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-05 23:23:56.000000 img2table-1.0.2/src/img2table/tables/processing/text/titles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 23:26:18.000000 img2table-1.0.2/src/img2table.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/_mock_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/_mock_data/azure.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/_mock_data/tesseract_hocr.html
--rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/_mock_data/textract.json
--rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/_mock_data/vision.json
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/_mock_data/vision.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/document/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/document/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/document/base/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/document/base/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/document/base/test_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/document/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/document/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/document/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/document/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)   346353 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/document/image/test_data/dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/document/image/test_data/expected.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/document/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/document/image/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/document/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/document/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/document/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/document/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/document/pdf/test_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/ocr/aws_textract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/aws_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/aws_textract/test_aws_textract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/ocr/aws_textract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/aws_textract/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/aws_textract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/aws_textract/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/ocr/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/azure/test_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/ocr/azure/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/azure/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/azure/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/ocr/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/ocr/data/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/data/test_data/expected_table.json
--rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/data/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/data/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/data/test_ocr_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/ocr/easyocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/easyocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/ocr/easyocr/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/easyocr/test_data/ocr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/easyocr/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/easyocr/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/easyocr/test_easyocr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/ocr/google_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/google_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/ocr/google_vision/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/google_vision/test_data/expected_content.json
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/google_vision/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/google_vision/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/google_vision/test_google_vision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/ocr/paddle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/paddle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/ocr/paddle/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/paddle/test_data/hocr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/paddle/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/paddle/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/paddle/test_paddle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/ocr/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/ocr/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/pdf/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/pdf/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/pdf/test_pdf_ocr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/ocr/tesseract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/tesseract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/ocr/tesseract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/tesseract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/tesseract/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/ocr/tesseract/test_tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/image/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/image/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/image/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/objects/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/objects/test_data/expected_tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/objects/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/objects/test_data/tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/objects/test_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/objects/test_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/objects/test_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/objects/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/cells/test_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/cells/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/cells/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/lines/test_data/contours.json
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/lines/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/lines/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_data/cells.json
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/borderless_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/borderless_tables/test_borderless_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/borderless_tables/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/borderless_tables/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    50091 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/column_delimiters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/column_delimiters/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/rows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/rows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/rows/test_coherency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/rows/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/rows/test_data/rows.json
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/rows/test_rows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/segment_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/segment_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/segment_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    50091 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/table/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/table/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/table/test_data/rows.json
--rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/table/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/table/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/borderless_tables/table/test_table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/common/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/common/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/common/test_data/test.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/prepare_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/prepare_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/prepare_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/prepare_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/prepare_image/test_prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:26:18.000000 img2table-1.0.2/tests/tables/processing/text/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/text/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/text/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/text/test_data/test.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-05 23:23:56.000000 img2table-1.0.2/tests/tables/processing/text/test_titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:34.000000 img2table-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 19:37:19.000000 img2table-1.0.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-12 19:37:19.000000 img2table-1.0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-12 19:37:19.000000 img2table-1.0.3/.github/workflows/test_workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-12 19:37:19.000000 img2table-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-12 19:37:19.000000 img2table-1.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-06-12 19:39:34.000000 img2table-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-06-12 19:37:19.000000 img2table-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-12 19:37:19.000000 img2table-1.0.3/activate_venv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-06-12 19:37:19.000000 img2table-1.0.3/examples/Basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-06-12 19:37:19.000000 img2table-1.0.3/examples/Implicit_rows.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   727975 2023-06-12 19:37:19.000000 img2table-1.0.3/examples/borderless.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/examples/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/examples/data/borderless/
+-rw-r--r--   0 runner    (1001) docker     (123)    47122 2023-06-12 19:37:19.000000 img2table-1.0.3/examples/data/borderless/1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   177004 2023-06-12 19:37:19.000000 img2table-1.0.3/examples/data/borderless/2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   182800 2023-06-12 19:37:19.000000 img2table-1.0.3/examples/data/borderless/3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   132335 2023-06-12 19:37:19.000000 img2table-1.0.3/examples/data/borderless/4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-06-12 19:37:19.000000 img2table-1.0.3/examples/data/borderless.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-06-12 19:37:19.000000 img2table-1.0.3/examples/data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-06-12 19:37:19.000000 img2table-1.0.3/examples/data/tables.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 19:37:19.000000 img2table-1.0.3/examples/data/tables.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-12 19:37:19.000000 img2table-1.0.3/examples/data/tables.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-12 19:37:19.000000 img2table-1.0.3/examples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-12 19:37:19.000000 img2table-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-12 19:37:19.000000 img2table-1.0.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-12 19:37:19.000000 img2table-1.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-12 19:37:19.000000 img2table-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-12 19:39:34.000000 img2table-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 19:37:19.000000 img2table-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table/document/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/document/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/document/base/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/document/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/document/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/ocr/aws_textract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/ocr/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/ocr/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/ocr/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/ocr/easyocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/ocr/google_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/ocr/paddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/ocr/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/ocr/tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/objects/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/objects/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/objects/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/objects/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/objects/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/bordered_tables/cells/identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/bordered_tables/lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/borderless_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table/tables/processing/borderless_tables/column_delimiters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/borderless_tables/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table/tables/processing/borderless_tables/rows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/borderless_tables/rows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/borderless_tables/rows/coherency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/borderless_tables/segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/borderless_tables/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/borderless_tables/table/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/borderless_tables/table/table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-12 19:37:19.000000 img2table-1.0.3/src/img2table/tables/processing/text/titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 19:39:33.000000 img2table-1.0.3/src/img2table.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/_mock_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/_mock_data/azure.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/_mock_data/tesseract_hocr.html
+-rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/_mock_data/textract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/_mock_data/vision.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/_mock_data/vision.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/document/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/document/base/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/document/base/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/document/base/test_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/document/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/document/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/document/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/document/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)   346353 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/document/image/test_data/dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/document/image/test_data/expected.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/document/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/document/image/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/document/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/document/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/document/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/document/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/document/pdf/test_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/ocr/aws_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/aws_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/aws_textract/test_aws_textract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/ocr/aws_textract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/aws_textract/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/aws_textract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/aws_textract/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/ocr/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/azure/test_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/ocr/azure/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/azure/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/azure/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/ocr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/ocr/data/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/data/test_data/expected_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/data/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/data/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/data/test_ocr_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/ocr/easyocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/easyocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/ocr/easyocr/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/easyocr/test_data/ocr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/easyocr/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/easyocr/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/easyocr/test_easyocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/ocr/google_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/google_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/ocr/google_vision/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/google_vision/test_data/expected_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/google_vision/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/google_vision/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/google_vision/test_google_vision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/ocr/paddle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/paddle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/ocr/paddle/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/paddle/test_data/hocr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/paddle/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/paddle/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/paddle/test_paddle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/ocr/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/ocr/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/pdf/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/pdf/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/pdf/test_pdf_ocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/ocr/tesseract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/tesseract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/ocr/tesseract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/tesseract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/tesseract/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/ocr/tesseract/test_tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/tables/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/tables/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/image/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/image/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/image/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/tables/objects/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/objects/test_data/expected_tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/objects/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/objects/test_data/tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/objects/test_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/objects/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/objects/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/objects/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/cells/test_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/cells/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/cells/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/lines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/lines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/lines/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/lines/test_data/contours.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/lines/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/lines/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/lines/test_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_data/cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:33.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/borderless_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/borderless_tables/test_borderless_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:34.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/borderless_tables/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/borderless_tables/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50091 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:34.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/column_delimiters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:34.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/column_delimiters/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:34.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/rows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/rows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/rows/test_coherency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:34.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/rows/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/rows/test_data/rows.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/rows/test_rows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:34.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/segment_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/segment_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:34.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/segment_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50091 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:34.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:34.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/table/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/table/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/table/test_data/rows.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/table/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/table/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/borderless_tables/table/test_table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:34.000000 img2table-1.0.3/tests/tables/processing/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/common/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:34.000000 img2table-1.0.3/tests/tables/processing/common/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/common/test_data/test.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:34.000000 img2table-1.0.3/tests/tables/processing/prepare_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/prepare_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:34.000000 img2table-1.0.3/tests/tables/processing/prepare_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/prepare_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/prepare_image/test_prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:34.000000 img2table-1.0.3/tests/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:39:34.000000 img2table-1.0.3/tests/tables/processing/text/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/text/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/text/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/text/test_data/test.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-12 19:37:19.000000 img2table-1.0.3/tests/tables/processing/text/test_titles.py
```

### Comparing `img2table-1.0.2/LICENSE.txt` & `img2table-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/Makefile` & `img2table-1.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/PKG-INFO` & `img2table-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 1.0.2
+Version: 1.0.3
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image 
@@ -28,15 +28,14 @@
         
         
         ## Installation <a name="installation"></a>
         The library can be installed via pip:
         
         > <code>pip install img2table</code>: Standard installation, supporting Tesseract<br>
         > <code>pip install img2table[paddle]</code>: For usage with Paddle OCR (Python <= 3.10 only)<br>
-        > <code>pip install img2table[paddlegpu]</code>: For usage with Paddle OCR - GPU (Python <= 3.10 only)<br>
         > <code>pip install img2table[easyocr]</code>: For usage with EasyOCR<br>
         > <code>pip install img2table[gcp]</code>: For usage with Google Vision OCR<br>
         > <code>pip install img2table[aws]</code>: For usage with AWS Textract OCR<br>
         > <code>pip install img2table[azure]</code>: For usage with Azure Cognitive Services OCR
         
         ## Features <a name="features"></a>
         
@@ -189,14 +188,25 @@
         
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>lang : str, optional, default <code>"en"</code></dt>
         >    <dd style="font-style: italic;">Lang parameter used in Paddle for text extraction, check <a href="https://github.com/Mushroomcat9998/PaddleOCR/blob/main/doc/doc_en/multi_languages_en.md#5-support-languages-and-abbreviations">documentation for available languages</a></dd>
         ></dl>
         
+        <br>
+        <b>NB:</b> For usage of PaddleOCR with GPU, the CUDA specific version of paddlepaddle-gpu has to be installed by the user manually 
+        as stated in this <a href="https://github.com/PaddlePaddle/PaddleOCR/issues/7993">issue</a>.
+        
+        ```bash
+        # Example of installation with CUDA 11.8
+        pip install paddlepaddle-gpu==2.5.0rc1.post118 -f https://www.paddlepaddle.org.cn/whl/linux/mkl/avx/stable.html
+        pip install paddleocr img2table
+        ```
+        
+        
         *Released in version 0.0.13*
         <br>
         </details>
         
         
         <details>
         <summary>EasyOCR<a name="easyocr"></a></summary>
@@ -453,9 +463,8 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: gcp
 Provides-Extra: aws
 Provides-Extra: azure
 Provides-Extra: paddle
-Provides-Extra: paddlegpu
 Provides-Extra: easyocr
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 1.0.2 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 1.0.3 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
@@ -11,16 +11,14 @@
 file-formats) * [Usage](#usage) * [Documents](#documents) * [Images](#images-
 doc) * [PDF](#pdf-doc) * [Supported OCRs](#ocr) * [Table extraction](#table-
 extract) * [Excel export](#xlsx) * [Examples](#examples) * [Caveats / FYI]
 (#fyi) ## Installation  The library can be installed via pip: > pip install
 img2table: Standard installation, supporting Tesseract
 > pip install img2table[paddle]: For usage with Paddle OCR (Python <= 3.10
 only)
-> pip install img2table[paddlegpu]: For usage with Paddle OCR - GPU (Python <=
-3.10 only)
 > pip install img2table[easyocr]: For usage with EasyOCR
 > pip install img2table[gcp]: For usage with Google Vision OCR
 > pip install img2table[aws]: For usage with AWS Textract OCR
 > pip install img2table[azure]: For usage with Azure Cognitive Services OCR ##
 Features  * Table identification for images and PDF files, including bounding
 boxes at the table cell level * Handling of complex table structures such as
 merged cells * Handling of implicit rows - see [example](/examples/
@@ -78,15 +76,20 @@
 *Available for Python versions <= 3.10* PaddleOCR is an open-source OCR based
 on Deep Learning models.
 At first use, relevant languages models will be downloaded. ```python from
 img2table.ocr import PaddleOCR ocr = PaddleOCR(lang="en") ``` >
 *** Parameters ***
 >
 >
-*Released in version 0.0.13*
+
+NB: For usage of PaddleOCR with GPU, the CUDA specific version of paddlepaddle-
+gpu has to be installed by the user manually as stated in this issue. ```bash #
+Example of installation with CUDA 11.8 pip install paddlepaddle-
+gpu==2.5.0rc1.post118 -f https://www.paddlepaddle.org.cn/whl/linux/mkl/avx/
+stable.html pip install paddleocr img2table ``` *Released in version 0.0.13*
   EasyOCR
 EasyOCR is an open-source OCR based on Deep Learning models.
 At first use, relevant languages models will be downloaded. ```python from
 img2table.ocr import EasyOCR ocr = EasyOCR(lang=["en"]) ``` >
 *** Parameters ***
 >
 >
@@ -179,8 +182,8 @@
     * Table detection using only OpenCV processing can have some limitations.
       If the library fails to detect tables, you may check CNN based solutions
       like CascadeTabNet or the PaddleOCR_implementation.
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7, <3.12 Description-Content-Type: text/
 markdown Provides-Extra: gcp Provides-Extra: aws Provides-Extra: azure
-Provides-Extra: paddle Provides-Extra: paddlegpu Provides-Extra: easyocr
+Provides-Extra: paddle Provides-Extra: easyocr
```

### Comparing `img2table-1.0.2/README.md` & `img2table-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 
 ## Installation <a name="installation"></a>
 The library can be installed via pip:
 
 > <code>pip install img2table</code>: Standard installation, supporting Tesseract<br>
 > <code>pip install img2table[paddle]</code>: For usage with Paddle OCR (Python <= 3.10 only)<br>
-> <code>pip install img2table[paddlegpu]</code>: For usage with Paddle OCR - GPU (Python <= 3.10 only)<br>
 > <code>pip install img2table[easyocr]</code>: For usage with EasyOCR<br>
 > <code>pip install img2table[gcp]</code>: For usage with Google Vision OCR<br>
 > <code>pip install img2table[aws]</code>: For usage with AWS Textract OCR<br>
 > <code>pip install img2table[azure]</code>: For usage with Azure Cognitive Services OCR
 
 ## Features <a name="features"></a>
 
@@ -182,14 +181,25 @@
 
 > <h4>Parameters</h4>
 ><dl>
 >    <dt>lang : str, optional, default <code>"en"</code></dt>
 >    <dd style="font-style: italic;">Lang parameter used in Paddle for text extraction, check <a href="https://github.com/Mushroomcat9998/PaddleOCR/blob/main/doc/doc_en/multi_languages_en.md#5-support-languages-and-abbreviations">documentation for available languages</a></dd>
 ></dl>
 
+<br>
+<b>NB:</b> For usage of PaddleOCR with GPU, the CUDA specific version of paddlepaddle-gpu has to be installed by the user manually 
+as stated in this <a href="https://github.com/PaddlePaddle/PaddleOCR/issues/7993">issue</a>.
+
+```bash
+# Example of installation with CUDA 11.8
+pip install paddlepaddle-gpu==2.5.0rc1.post118 -f https://www.paddlepaddle.org.cn/whl/linux/mkl/avx/stable.html
+pip install paddleocr img2table
+```
+
+
 *Released in version 0.0.13*
 <br>
 </details>
 
 
 <details>
 <summary>EasyOCR<a name="easyocr"></a></summary>
```

#### html2text {}

```diff
@@ -7,16 +7,14 @@
 formats](#supported-file-formats) * [Usage](#usage) * [Documents](#documents) *
 [Images](#images-doc) * [PDF](#pdf-doc) * [Supported OCRs](#ocr) * [Table
 extraction](#table-extract) * [Excel export](#xlsx) * [Examples](#examples) *
 [Caveats / FYI](#fyi) ## Installation  The library can be installed via pip: >
 pip install img2table: Standard installation, supporting Tesseract
 > pip install img2table[paddle]: For usage with Paddle OCR (Python <= 3.10
 only)
-> pip install img2table[paddlegpu]: For usage with Paddle OCR - GPU (Python <=
-3.10 only)
 > pip install img2table[easyocr]: For usage with EasyOCR
 > pip install img2table[gcp]: For usage with Google Vision OCR
 > pip install img2table[aws]: For usage with AWS Textract OCR
 > pip install img2table[azure]: For usage with Azure Cognitive Services OCR ##
 Features  * Table identification for images and PDF files, including bounding
 boxes at the table cell level * Handling of complex table structures such as
 merged cells * Handling of implicit rows - see [example](/examples/
@@ -74,15 +72,20 @@
 *Available for Python versions <= 3.10* PaddleOCR is an open-source OCR based
 on Deep Learning models.
 At first use, relevant languages models will be downloaded. ```python from
 img2table.ocr import PaddleOCR ocr = PaddleOCR(lang="en") ``` >
 *** Parameters ***
 >
 >
-*Released in version 0.0.13*
+
+NB: For usage of PaddleOCR with GPU, the CUDA specific version of paddlepaddle-
+gpu has to be installed by the user manually as stated in this issue. ```bash #
+Example of installation with CUDA 11.8 pip install paddlepaddle-
+gpu==2.5.0rc1.post118 -f https://www.paddlepaddle.org.cn/whl/linux/mkl/avx/
+stable.html pip install paddleocr img2table ``` *Released in version 0.0.13*
   EasyOCR
 EasyOCR is an open-source OCR based on Deep Learning models.
 At first use, relevant languages models will be downloaded. ```python from
 img2table.ocr import EasyOCR ocr = EasyOCR(lang=["en"]) ``` >
 *** Parameters ***
 >
 >
```

### Comparing `img2table-1.0.2/examples/Basic_usage.ipynb` & `img2table-1.0.3/examples/Basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/examples/Implicit_rows.ipynb` & `img2table-1.0.3/examples/Implicit_rows.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/examples/borderless.ipynb` & `img2table-1.0.3/examples/borderless.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/examples/data/borderless/1.png` & `img2table-1.0.3/examples/data/borderless/1.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/examples/data/borderless/2.png` & `img2table-1.0.3/examples/data/borderless/2.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/examples/data/borderless/3.png` & `img2table-1.0.3/examples/data/borderless/3.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/examples/data/borderless/4.png` & `img2table-1.0.3/examples/data/borderless/4.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/examples/data/borderless.jpg` & `img2table-1.0.3/examples/data/borderless.jpg`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/examples/data/implicit.png` & `img2table-1.0.3/examples/data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/examples/data/tables.pdf` & `img2table-1.0.3/examples/data/tables.pdf`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/examples/data/tables.png` & `img2table-1.0.3/examples/data/tables.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/examples/data/tables.xlsx` & `img2table-1.0.3/examples/data/tables.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/examples/utils.py` & `img2table-1.0.3/examples/utils.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/__init__.py` & `img2table-1.0.3/src/img2table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/document/base/__init__.py` & `img2table-1.0.3/src/img2table/document/base/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/document/base/rotation.py` & `img2table-1.0.3/src/img2table/document/base/rotation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/document/image.py` & `img2table-1.0.3/src/img2table/document/image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/document/pdf.py` & `img2table-1.0.3/src/img2table/document/pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/ocr/aws_textract.py` & `img2table-1.0.3/src/img2table/ocr/aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/ocr/azure.py` & `img2table-1.0.3/src/img2table/ocr/azure.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/ocr/base.py` & `img2table-1.0.3/src/img2table/ocr/base.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/ocr/data.py` & `img2table-1.0.3/src/img2table/ocr/data.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/ocr/easyocr.py` & `img2table-1.0.3/src/img2table/ocr/easyocr.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/ocr/google_vision.py` & `img2table-1.0.3/src/img2table/ocr/google_vision.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/ocr/paddle.py` & `img2table-1.0.3/src/img2table/ocr/paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/ocr/pdf.py` & `img2table-1.0.3/src/img2table/ocr/pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/ocr/tesseract.py` & `img2table-1.0.3/src/img2table/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/__init__.py` & `img2table-1.0.3/src/img2table/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/image.py` & `img2table-1.0.3/src/img2table/tables/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from img2table.tables.processing.prepare_image import prepare_image
 from img2table.tables.processing.text.titles import get_title_tables
 
 
 @dataclass
 class TableImage:
     img: np.ndarray
-    dpi: int = 200
     ocr_df: "OCRDataframe" = None
     min_confidence: int = 50
     char_length: float = None
     median_line_sep: float = None
     contours: List[Cell] = None
     lines: List[Line] = None
     tables: List[Table] = None
@@ -63,16 +62,16 @@
     def extract_bordered_tables(self, implicit_rows: bool = True):
         """
         Identify and extract bordered tables from image
         :param implicit_rows: boolean indicating if implicit rows are splitted
         :return:
         """
         # Compute parameters for line detection
-        minLinLength = maxLineGap = round(0.33 * self.median_line_sep) if self.median_line_sep else self.dpi // 20
-        kernel_size = round(0.66 * self.median_line_sep) if self.median_line_sep else self.dpi // 10
+        minLinLength = maxLineGap = max(int(round(0.33 * self.median_line_sep)), 1) if self.median_line_sep else 10
+        kernel_size = max(int(round(0.66 * self.median_line_sep)), 1) if self.median_line_sep else 20
 
         # Detect rows in image
         h_lines, v_lines = detect_lines(image=self.img,
                                         contours=self.contours,
                                         char_length=self.char_length,
                                         rho=0.3,
                                         theta=np.pi / 180,
```

### Comparing `img2table-1.0.2/src/img2table/tables/metrics.py` & `img2table-1.0.3/src/img2table/tables/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     for c in cc:
         cv2.rectangle(black_img,
                       (c[cv2.CC_STAT_LEFT], c[cv2.CC_STAT_TOP]),
                       (c[cv2.CC_STAT_LEFT] + c[cv2.CC_STAT_WIDTH], c[cv2.CC_STAT_TOP] + c[cv2.CC_STAT_HEIGHT]),
                       (255, 255, 255), -1)
 
     # Dilate image
-    kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (round(char_length), 1))
+    kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (max(int(round(char_length)), 1), 1))
     dilate = cv2.dilate(black_img, kernel, iterations=1)
 
     # Find and map contours
     cnts, _ = cv2.findContours(dilate, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
 
     contours = list()
     for idx, cnt in enumerate(cnts):
```

### Comparing `img2table-1.0.2/src/img2table/tables/objects/__init__.py` & `img2table-1.0.3/src/img2table/tables/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/objects/extraction.py` & `img2table-1.0.3/src/img2table/tables/objects/extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/objects/line.py` & `img2table-1.0.3/src/img2table/tables/objects/line.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,14 +54,14 @@
         _x2 = max(self.x1, self.x2)
         _y1 = min(self.y1, self.y2)
         _y2 = max(self.y1, self.y2)
         self.x1, self.x2, self.y1, self.y2 = _x1, _x2, _y1, _y2
 
         # Correct "almost" horizontal or vertical rows
         if abs(self.angle) <= 5:
-            y_val = round((self.y1 + self.y2) / 2)
+            y_val = int(round((self.y1 + self.y2) / 2))
             self.y2 = self.y1 = y_val
         elif abs(self.angle - 90) <= 5:
-            x_val = round((self.x1 + self.x2) / 2)
+            x_val = int(round((self.x1 + self.x2) / 2))
             self.x2 = self.x1 = x_val
 
         return self
```

### Comparing `img2table-1.0.2/src/img2table/tables/objects/row.py` & `img2table-1.0.3/src/img2table/tables/objects/row.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/objects/table.py` & `img2table-1.0.3/src/img2table/tables/objects/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         if len(remaining_rows) > 1:
             # Check created gaps between rows
             gaps = [(id_row, id_next) for id_row, id_next in zip(remaining_rows, remaining_rows[1:])
                     if id_next - id_row > 1]
 
             for id_row, id_next in gaps:
                 # Normalize y value between rows
-                y_gap = round((self.items[id_row].y2 + self.items[id_next].y1) / 2)
+                y_gap = int(round((self.items[id_row].y2 + self.items[id_next].y1) / 2))
 
                 # Put y value in both rows
                 for c in self.items[id_row].items:
                     setattr(c, "y2", y_gap)
                 for c in self.items[id_next].items:
                     setattr(c, "y1", y_gap)
 
@@ -97,15 +97,15 @@
         if len(remaining_cols) > 1:
             # Check created gaps between columns
             gaps = [(id_col, id_next) for id_col, id_next in zip(remaining_cols, remaining_cols[1:])
                     if id_next - id_col > 1]
 
             for id_col, id_next in gaps:
                 # Normalize x value between columns
-                x_gap = round(np.mean([row.items[id_col].x2 + row.items[id_next].x1 for row in self.items]) / 2)
+                x_gap = int(round(np.mean([row.items[id_col].x2 + row.items[id_next].x1 for row in self.items]) / 2))
 
                 # Put y value in both columns
                 for row in self.items:
                     setattr(row.items[id_col], "x2", x_gap)
                     setattr(row.items[id_next], "x1", x_gap)
 
         # Remove columns
```

### Comparing `img2table-1.0.2/src/img2table/tables/processing/bordered_tables/cells/__init__.py` & `img2table-1.0.3/src/img2table/tables/processing/bordered_tables/cells/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/processing/bordered_tables/cells/deduplication.py` & `img2table-1.0.3/src/img2table/tables/processing/bordered_tables/cells/deduplication.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/processing/bordered_tables/cells/identification.py` & `img2table-1.0.3/src/img2table/tables/processing/bordered_tables/cells/identification.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/processing/bordered_tables/lines.py` & `img2table-1.0.3/src/img2table/tables/processing/bordered_tables/lines.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """
     # Get threshold on image and binary image
     blur = cv2.GaussianBlur(img, (3, 3), 0)
     thresh = cv2.adaptiveThreshold(blur, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY_INV, 21, 10)
     binary_thresh = cv2.adaptiveThreshold(255 - blur, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY_INV, 21, 10)
 
     # Mask on areas with dark background
-    blur_size = int(2 * char_length) + 1 - int(2 * char_length) % 2 if char_length else 11
+    blur_size = max(int(2 * char_length) + 1 - int(2 * char_length) % 2, 1) if char_length else 11
     blur = cv2.medianBlur(img, blur_size)
     mask = cv2.inRange(blur, 0, 100)
 
     # Get contours of dark areas
     contours, _ = cv2.findContours(mask, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
 
     # For each dark area, use binary threshold instead of regular threshold
@@ -47,15 +47,15 @@
     Dilate specific rows/columns of the threshold image in order to detect dotted rows
     :param thresh: threshold image array
     :param char_length: average character length in image
     :return: threshold image with dilated dotted rows
     """
     ### Horizontal case
     # Create dilated image
-    h_dilated = cv2.dilate(thresh, cv2.getStructuringElement(cv2.MORPH_RECT, (int(char_length // 2), 1)))
+    h_dilated = cv2.dilate(thresh, cv2.getStructuringElement(cv2.MORPH_RECT, (max(int(char_length // 2), 1), 1)))
 
     # Get rows with at least 2 times the average number of white pixels
     white_rows = np.where(np.mean(thresh, axis=1) > 2 * np.mean(thresh))[0].tolist()
 
     # Split into consecutive groups of rows and keep only small ones to avoid targeting text rows
     white_rows_cl = [list(map(itemgetter(1), g))
                      for k, g in groupby(enumerate(white_rows), lambda i_x: i_x[0] - i_x[1])]
@@ -67,15 +67,15 @@
     h_dilated[mask, :] = 0
 
     # Update threshold image
     thresh = np.maximum(thresh, h_dilated)
 
     ### Vertical case
     # Create dilated image
-    v_dilated = cv2.dilate(thresh, cv2.getStructuringElement(cv2.MORPH_RECT, (1, int(char_length // 2))))
+    v_dilated = cv2.dilate(thresh, cv2.getStructuringElement(cv2.MORPH_RECT, (1, max(int(char_length // 2), 1))))
 
     # Get columns with at least 2 times the average number of white pixels
     white_cols = np.where(np.mean(thresh, axis=0) > 2 * np.mean(thresh))[0].tolist()
 
     # Split into consecutive groups of columns and keep only small ones to avoid targeting text columns
     white_cols_cl = [list(map(itemgetter(1), g))
                      for k, g in groupby(enumerate(white_cols), lambda i_x: i_x[0] - i_x[1])]
@@ -138,21 +138,21 @@
                 sub_clusters[-1].append(line)
             # If the difference in vertical coordinates is too large, create a new sub cluster
             else:
                 sub_clusters.append([line])
 
         # Create rows from sub clusters
         for sub_cl in sub_clusters:
-            y_value = round(np.average([l.y1 for l in sub_cl],
-                                       weights=list(map(lambda l: l.length, sub_cl))))
+            y_value = int(round(np.average([l.y1 for l in sub_cl],
+                                           weights=list(map(lambda l: l.length, sub_cl)))))
             thickness = min(max(1, max(map(lambda l: l.y2, sub_cl)) - min(map(lambda l: l.y1, sub_cl))), 5)
             line = Line(x1=min(map(lambda l: l.x1, sub_cl)),
                         x2=max(map(lambda l: l.x2, sub_cl)),
-                        y1=y_value,
-                        y2=y_value,
+                        y1=int(y_value),
+                        y2=int(y_value),
                         thickness=thickness)
 
             if line.length > 0:
                 final_lines.append(line)
 
     # If not horizontal, transpose all rows
     if not horizontal:
```

### Comparing `img2table-1.0.2/src/img2table/tables/processing/bordered_tables/tables/__init__.py` & `img2table-1.0.3/src/img2table/tables/processing/bordered_tables/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py` & `img2table-1.0.3/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py` & `img2table-1.0.3/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                                      cell=row,
                                      margin=-5,
                                      blur_size=5,
                                      kernel_size=5,
                                      merge_vertically=True)
 
         # Compute vertical delimiters
-        vertical_delimiters = sorted([round((cnt_1.y2 + cnt_2.y1) / 2) for cnt_1, cnt_2 in zip(contours, contours[1:])])
+        vertical_delimiters = sorted([int(round((cnt_1.y2 + cnt_2.y1) / 2)) for cnt_1, cnt_2 in zip(contours, contours[1:])])
 
         # Split row into multiple rows from vertical delimiters
         list_splitted_rows += row.split_in_rows(vertical_delimiters=vertical_delimiters)
 
     return Table(rows=list_splitted_rows)
```

### Comparing `img2table-1.0.2/src/img2table/tables/processing/bordered_tables/tables/table_creation.py` & `img2table-1.0.3/src/img2table/tables/processing/bordered_tables/tables/table_creation.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,21 +18,21 @@
     # Compute table shape
     width = max(map(lambda c: c.x2, cluster_cells)) - min(map(lambda c: c.x1, cluster_cells))
     height = max(map(lambda c: c.y2, cluster_cells)) - min(map(lambda c: c.y1, cluster_cells))
 
     # Get list of existing horizontal values
     h_values = sorted(list(set([x_val for cell in cluster_cells for x_val in [cell.x1, cell.x2]])))
     # Compute delimiters by grouping close values together
-    h_delims = [round(np.mean(h_group)) for h_group in
+    h_delims = [int(round(np.mean(h_group))) for h_group in
                 np.split(h_values, np.where(np.diff(h_values) >= min(width * 0.02, 10))[0] + 1)]
 
     # Get list of existing vertical values
     v_values = sorted(list(set([y_val for cell in cluster_cells for y_val in [cell.y1, cell.y2]])))
     # Compute delimiters by grouping close values together
-    v_delims = [round(np.mean(v_group)) for v_group in
+    v_delims = [int(round(np.mean(v_group))) for v_group in
                 np.split(v_values, np.where(np.diff(v_values) >= min(height * 0.02, 10))[0] + 1)]
 
     # Normalize all cells
     normalized_cells = list()
     for cell in cluster_cells:
         normalized_cell = Cell(x1=sorted(h_delims, key=lambda d: abs(d - cell.x1)).pop(0),
                                x2=sorted(h_delims, key=lambda d: abs(d - cell.x2)).pop(0),
```

### Comparing `img2table-1.0.2/src/img2table/tables/processing/borderless_tables/__init__.py` & `img2table-1.0.3/src/img2table/tables/processing/borderless_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py` & `img2table-1.0.3/src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py` & `img2table-1.0.3/src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py` & `img2table-1.0.3/src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/processing/borderless_tables/model.py` & `img2table-1.0.3/src/img2table/tables/processing/borderless_tables/model.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/processing/borderless_tables/rows/__init__.py` & `img2table-1.0.3/src/img2table/tables/processing/borderless_tables/rows/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/processing/borderless_tables/rows/coherency.py` & `img2table-1.0.3/src/img2table/tables/processing/borderless_tables/rows/coherency.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py` & `img2table-1.0.3/src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/processing/borderless_tables/segment_image.py` & `img2table-1.0.3/src/img2table/tables/processing/borderless_tables/segment_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     :return: list of image segments as Cell objects
     """
     # Reprocess images
     blur = cv2.medianBlur(img, 5)
     thresh = cv2.Canny(blur, 0, 0)
 
     # Define kernel by using median line separation and character length
-    kernel_size = (max(int(2 * char_length), round(median_line_sep / 3)),
-                   round(median_line_sep / 3))
+    kernel_size = (max(int(2 * char_length), int(round(median_line_sep / 3)), 1),
+                   max(int(round(median_line_sep / 3)), 1))
 
     # Dilate to combine adjacent text contours
     kernel = cv2.getStructuringElement(cv2.MORPH_RECT, kernel_size)
     dilate = cv2.dilate(thresh, kernel, iterations=4)
 
     # Create new image by adding black borders
     margin = 10
@@ -86,15 +86,16 @@
     for l in lines:
         if l.horizontal:
             cv2.rectangle(thresh, (l.x1 - l.thickness, l.y1), (l.x2 + l.thickness, l.y2), (0, 0, 0), 3 * l.thickness)
         elif l.vertical:
             cv2.rectangle(thresh, (l.x1, l.y1 - l.thickness), (l.x2, l.y2 + l.thickness), (0, 0, 0), 2 * l.thickness)
 
     # Dilate to combine adjacent text contours
-    kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (int(1.5 * char_length), int(median_line_sep // 6)))
+    kernel = cv2.getStructuringElement(cv2.MORPH_RECT,
+                                       (max(int(1.5 * char_length), 1), max(int(median_line_sep // 6), 1)))
     dilate = cv2.dilate(thresh, kernel, iterations=1)
 
     # Find contours, highlight text areas, and extract ROIs
     cnts = cv2.findContours(dilate, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
     cnts = cnts[0] if len(cnts) == 2 else cnts[1]
 
     # Get list of contours
```

### Comparing `img2table-1.0.2/src/img2table/tables/processing/borderless_tables/table/__init__.py` & `img2table-1.0.3/src/img2table/tables/processing/borderless_tables/table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/processing/borderless_tables/table/headers.py` & `img2table-1.0.3/src/img2table/tables/processing/borderless_tables/table/headers.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/processing/borderless_tables/table/table_creation.py` & `img2table-1.0.3/src/img2table/tables/processing/borderless_tables/table/table_creation.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     :param table_rows: list of table rows
     :return: Table object
     """
     # Compute vertical delimiters from rows
     lines = sorted(table_rows, key=lambda l: l.v_center)
     y_min = min([line.y1 for line in lines])
     y_max = max([line.y2 for line in lines])
-    v_delims = [y_min] + [round((up.y2 + down.y1) / 2) for up, down in zip(lines, lines[1:])] + [y_max]
+    v_delims = [y_min] + [int(round((up.y2 + down.y1) / 2)) for up, down in zip(lines, lines[1:])] + [y_max]
 
     # Create cells for table
     list_cells = list()
     for y_top, y_bottom in zip(v_delims, v_delims[1:]):
         # Identify delimiters that correspond vertically to rows
         line_delims = [d for d in columns.delimiters if
                        min(d.y2, y_bottom) - max(d.y1, y_top) > (y_bottom - y_top) // 2]
```

### Comparing `img2table-1.0.2/src/img2table/tables/processing/common.py` & `img2table-1.0.3/src/img2table/tables/processing/common.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/processing/prepare_image.py` & `img2table-1.0.3/src/img2table/tables/processing/prepare_image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/src/img2table/tables/processing/text/titles.py` & `img2table-1.0.3/src/img2table/tables/processing/text/titles.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,17 +35,17 @@
             tb_cl.append([])
         tb_cl[-1].append(tb)
 
     # Identify relative zones for each title corresponding to each cluster
     final_tables = list()
     for id_cl, cluster in enumerate(tb_cl):
         # Compute horizontal boundaries of title
-        x_delimiters = [round((tb_1.x2 + tb_2.x1) / 2) for tb_1, tb_2 in zip(cluster, cluster[1:])]
-        x_delimiters = [max(10, round(cluster[0].x1 - 0.2 * cluster[0].width))] + x_delimiters + [width - 10]
-        x_delimiters = x_delimiters + [min(width - 10, round(cluster[-1].x2 + 0.2 * cluster[-1].width))]
+        x_delimiters = [int(round((tb_1.x2 + tb_2.x1) / 2)) for tb_1, tb_2 in zip(cluster, cluster[1:])]
+        x_delimiters = [max(10, int(round(cluster[0].x1 - 0.2 * cluster[0].width)))] + x_delimiters + [width - 10]
+        x_delimiters = x_delimiters + [min(width - 10, int(round(cluster[-1].x2 + 0.2 * cluster[-1].width)))]
         x_bounds = [(del_1, del_2) for del_1, del_2 in zip(x_delimiters, x_delimiters[1:])]
 
         # Compute vertical boundaries of title
         y_bounds = (max([tb.y2 for tb in tb_cl[id_cl - 1]]) if id_cl > 0 else 0, min([tb.y1 for tb in cluster]))
 
         # Fetch title for each table
         for id_tb, table in enumerate(cluster):
```

### Comparing `img2table-1.0.2/src/img2table.egg-info/PKG-INFO` & `img2table-1.0.3/src/img2table.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 1.0.2
+Version: 1.0.3
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image 
@@ -28,15 +28,14 @@
         
         
         ## Installation <a name="installation"></a>
         The library can be installed via pip:
         
         > <code>pip install img2table</code>: Standard installation, supporting Tesseract<br>
         > <code>pip install img2table[paddle]</code>: For usage with Paddle OCR (Python <= 3.10 only)<br>
-        > <code>pip install img2table[paddlegpu]</code>: For usage with Paddle OCR - GPU (Python <= 3.10 only)<br>
         > <code>pip install img2table[easyocr]</code>: For usage with EasyOCR<br>
         > <code>pip install img2table[gcp]</code>: For usage with Google Vision OCR<br>
         > <code>pip install img2table[aws]</code>: For usage with AWS Textract OCR<br>
         > <code>pip install img2table[azure]</code>: For usage with Azure Cognitive Services OCR
         
         ## Features <a name="features"></a>
         
@@ -189,14 +188,25 @@
         
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>lang : str, optional, default <code>"en"</code></dt>
         >    <dd style="font-style: italic;">Lang parameter used in Paddle for text extraction, check <a href="https://github.com/Mushroomcat9998/PaddleOCR/blob/main/doc/doc_en/multi_languages_en.md#5-support-languages-and-abbreviations">documentation for available languages</a></dd>
         ></dl>
         
+        <br>
+        <b>NB:</b> For usage of PaddleOCR with GPU, the CUDA specific version of paddlepaddle-gpu has to be installed by the user manually 
+        as stated in this <a href="https://github.com/PaddlePaddle/PaddleOCR/issues/7993">issue</a>.
+        
+        ```bash
+        # Example of installation with CUDA 11.8
+        pip install paddlepaddle-gpu==2.5.0rc1.post118 -f https://www.paddlepaddle.org.cn/whl/linux/mkl/avx/stable.html
+        pip install paddleocr img2table
+        ```
+        
+        
         *Released in version 0.0.13*
         <br>
         </details>
         
         
         <details>
         <summary>EasyOCR<a name="easyocr"></a></summary>
@@ -453,9 +463,8 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: gcp
 Provides-Extra: aws
 Provides-Extra: azure
 Provides-Extra: paddle
-Provides-Extra: paddlegpu
 Provides-Extra: easyocr
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 1.0.2 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 1.0.3 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
@@ -11,16 +11,14 @@
 file-formats) * [Usage](#usage) * [Documents](#documents) * [Images](#images-
 doc) * [PDF](#pdf-doc) * [Supported OCRs](#ocr) * [Table extraction](#table-
 extract) * [Excel export](#xlsx) * [Examples](#examples) * [Caveats / FYI]
 (#fyi) ## Installation  The library can be installed via pip: > pip install
 img2table: Standard installation, supporting Tesseract
 > pip install img2table[paddle]: For usage with Paddle OCR (Python <= 3.10
 only)
-> pip install img2table[paddlegpu]: For usage with Paddle OCR - GPU (Python <=
-3.10 only)
 > pip install img2table[easyocr]: For usage with EasyOCR
 > pip install img2table[gcp]: For usage with Google Vision OCR
 > pip install img2table[aws]: For usage with AWS Textract OCR
 > pip install img2table[azure]: For usage with Azure Cognitive Services OCR ##
 Features  * Table identification for images and PDF files, including bounding
 boxes at the table cell level * Handling of complex table structures such as
 merged cells * Handling of implicit rows - see [example](/examples/
@@ -78,15 +76,20 @@
 *Available for Python versions <= 3.10* PaddleOCR is an open-source OCR based
 on Deep Learning models.
 At first use, relevant languages models will be downloaded. ```python from
 img2table.ocr import PaddleOCR ocr = PaddleOCR(lang="en") ``` >
 *** Parameters ***
 >
 >
-*Released in version 0.0.13*
+
+NB: For usage of PaddleOCR with GPU, the CUDA specific version of paddlepaddle-
+gpu has to be installed by the user manually as stated in this issue. ```bash #
+Example of installation with CUDA 11.8 pip install paddlepaddle-
+gpu==2.5.0rc1.post118 -f https://www.paddlepaddle.org.cn/whl/linux/mkl/avx/
+stable.html pip install paddleocr img2table ``` *Released in version 0.0.13*
   EasyOCR
 EasyOCR is an open-source OCR based on Deep Learning models.
 At first use, relevant languages models will be downloaded. ```python from
 img2table.ocr import EasyOCR ocr = EasyOCR(lang=["en"]) ``` >
 *** Parameters ***
 >
 >
@@ -179,8 +182,8 @@
     * Table detection using only OpenCV processing can have some limitations.
       If the library fails to detect tables, you may check CNN based solutions
       like CascadeTabNet or the PaddleOCR_implementation.
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7, <3.12 Description-Content-Type: text/
 markdown Provides-Extra: gcp Provides-Extra: aws Provides-Extra: azure
-Provides-Extra: paddle Provides-Extra: paddlegpu Provides-Extra: easyocr
+Provides-Extra: paddle Provides-Extra: easyocr
```

### Comparing `img2table-1.0.2/src/img2table.egg-info/SOURCES.txt` & `img2table-1.0.3/src/img2table.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/_mock_data/azure.pkl` & `img2table-1.0.3/tests/_mock_data/azure.pkl`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/_mock_data/tesseract_hocr.html` & `img2table-1.0.3/tests/_mock_data/tesseract_hocr.html`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/_mock_data/textract.json` & `img2table-1.0.3/tests/_mock_data/textract.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/_mock_data/vision.json` & `img2table-1.0.3/tests/_mock_data/vision.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/_mock_data/vision.pkl` & `img2table-1.0.3/tests/_mock_data/vision.pkl`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/conftest.py` & `img2table-1.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/document/base/test_data/test.png` & `img2table-1.0.3/tests/document/base/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/document/base/test_rotation.py` & `img2table-1.0.3/tests/document/base/test_rotation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/document/image/test_data/blank.png` & `img2table-1.0.3/tests/document/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/document/image/test_data/dark.png` & `img2table-1.0.3/tests/document/image/test_data/dark.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/document/image/test_data/expected.xlsx` & `img2table-1.0.3/tests/document/image/test_data/expected.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/document/image/test_data/test.png` & `img2table-1.0.3/tests/document/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/document/image/test_image.py` & `img2table-1.0.3/tests/document/image/test_image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/document/pdf/test_data/test.pdf` & `img2table-1.0.3/tests/document/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/document/pdf/test_pdf.py` & `img2table-1.0.3/tests/document/pdf/test_pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/aws_textract/test_aws_textract.py` & `img2table-1.0.3/tests/ocr/aws_textract/test_aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/aws_textract/test_data/content.json` & `img2table-1.0.3/tests/ocr/aws_textract/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/aws_textract/test_data/ocr_df.csv` & `img2table-1.0.3/tests/ocr/aws_textract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/aws_textract/test_data/test.png` & `img2table-1.0.3/tests/ocr/aws_textract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/azure/test_azure.py` & `img2table-1.0.3/tests/ocr/azure/test_azure.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/azure/test_data/ocr_df.csv` & `img2table-1.0.3/tests/ocr/azure/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/azure/test_data/test.png` & `img2table-1.0.3/tests/ocr/azure/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/data/test_data/expected_table.json` & `img2table-1.0.3/tests/ocr/data/test_data/expected_table.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/data/test_data/ocr_df.csv` & `img2table-1.0.3/tests/ocr/data/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/data/test_ocr_data.py` & `img2table-1.0.3/tests/ocr/data/test_ocr_data.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/easyocr/test_data/ocr.json` & `img2table-1.0.3/tests/ocr/easyocr/test_data/ocr.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/easyocr/test_data/ocr_df.csv` & `img2table-1.0.3/tests/ocr/easyocr/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/easyocr/test_data/test.png` & `img2table-1.0.3/tests/ocr/easyocr/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/easyocr/test_easyocr.py` & `img2table-1.0.3/tests/ocr/easyocr/test_easyocr.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/google_vision/test_data/expected_content.json` & `img2table-1.0.3/tests/ocr/google_vision/test_data/expected_content.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/google_vision/test_data/ocr_df.csv` & `img2table-1.0.3/tests/ocr/google_vision/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/google_vision/test_data/test.png` & `img2table-1.0.3/tests/ocr/google_vision/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/google_vision/test_google_vision.py` & `img2table-1.0.3/tests/ocr/google_vision/test_google_vision.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/paddle/test_data/hocr.json` & `img2table-1.0.3/tests/ocr/paddle/test_data/hocr.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/paddle/test_data/ocr_df.csv` & `img2table-1.0.3/tests/ocr/paddle/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/paddle/test_data/test.png` & `img2table-1.0.3/tests/ocr/paddle/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/paddle/test_paddle.py` & `img2table-1.0.3/tests/ocr/paddle/test_paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/pdf/test_data/content.json` & `img2table-1.0.3/tests/ocr/pdf/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/pdf/test_data/ocr_df.csv` & `img2table-1.0.3/tests/ocr/pdf/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/pdf/test_data/test.pdf` & `img2table-1.0.3/tests/ocr/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/pdf/test_pdf_ocr.py` & `img2table-1.0.3/tests/ocr/pdf/test_pdf_ocr.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/tesseract/test_data/ocr_df.csv` & `img2table-1.0.3/tests/ocr/tesseract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/tesseract/test_data/test.png` & `img2table-1.0.3/tests/ocr/tesseract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/ocr/tesseract/test_tesseract.py` & `img2table-1.0.3/tests/ocr/tesseract/test_tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/image/test_data/blank.png` & `img2table-1.0.3/tests/tables/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/image/test_data/ocr.csv` & `img2table-1.0.3/tests/tables/image/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/image/test_data/test.png` & `img2table-1.0.3/tests/tables/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/image/test_image.py` & `img2table-1.0.3/tests/tables/image/test_image.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 
 def test_table_image():
     image = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
     ocr_df = OCRDataframe(pl.read_csv("test_data/ocr.csv", separator=";", encoding="utf-8").lazy())
 
     tb_image = TableImage(img=image,
-                          dpi=200,
                           ocr_df=ocr_df,
                           min_confidence=50)
 
     result = tb_image.extract_tables(implicit_rows=True)
 
     assert result[0].bbox == BBox(x1=35, y1=20, x2=770, y2=327)
     assert (len(result[0].content), len(result[0].content[0])) == (6, 3)
```

### Comparing `img2table-1.0.2/tests/tables/image/test_metrics.py` & `img2table-1.0.3/tests/tables/image/test_metrics.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/objects/test_data/expected_tables.json` & `img2table-1.0.3/tests/tables/objects/test_data/expected_tables.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/objects/test_data/ocr.csv` & `img2table-1.0.3/tests/tables/objects/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/objects/test_data/tables.json` & `img2table-1.0.3/tests/tables/objects/test_data/tables.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/objects/test_extraction.py` & `img2table-1.0.3/tests/tables/objects/test_extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/objects/test_line.py` & `img2table-1.0.3/tests/tables/objects/test_line.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/objects/test_row.py` & `img2table-1.0.3/tests/tables/objects/test_row.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/objects/test_table.py` & `img2table-1.0.3/tests/tables/objects/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/cells/test_cells.py` & `img2table-1.0.3/tests/tables/processing/bordered_tables/cells/test_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/cells/test_data/expected.csv` & `img2table-1.0.3/tests/tables/processing/bordered_tables/cells/test_data/expected.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/cells/test_data/lines.json` & `img2table-1.0.3/tests/tables/processing/bordered_tables/cells/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py` & `img2table-1.0.3/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/cells/test_identification_cells.py` & `img2table-1.0.3/tests/tables/processing/bordered_tables/cells/test_identification_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/lines/test_data/contours.json` & `img2table-1.0.3/tests/tables/processing/bordered_tables/lines/test_data/contours.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/lines/test_data/expected.json` & `img2table-1.0.3/tests/tables/processing/bordered_tables/lines/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/lines/test_data/test.png` & `img2table-1.0.3/tests/tables/processing/bordered_tables/lines/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/lines/test_lines.py` & `img2table-1.0.3/tests/tables/processing/bordered_tables/lines/test_lines.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py` & `img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json` & `img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_data/cells.json` & `img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_data/cells.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json` & `img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_data/expected.json` & `img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_data/implicit.png` & `img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json` & `img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_data/word_image.png` & `img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_data/word_image.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py` & `img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_table_creation.py` & `img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/bordered_tables/tables/test_tables.py` & `img2table-1.0.3/tests/tables/processing/bordered_tables/tables/test_tables.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/borderless_tables/test_borderless_tables.py` & `img2table-1.0.3/tests/tables/processing/borderless_tables/borderless_tables/test_borderless_tables.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png` & `img2table-1.0.3/tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py` & `img2table-1.0.3/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py` & `img2table-1.0.3/tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json` & `img2table-1.0.3/tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py` & `img2table-1.0.3/tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/rows/test_coherency.py` & `img2table-1.0.3/tests/tables/processing/borderless_tables/rows/test_coherency.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json` & `img2table-1.0.3/tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/rows/test_data/rows.json` & `img2table-1.0.3/tests/tables/processing/borderless_tables/rows/test_data/rows.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py` & `img2table-1.0.3/tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/rows/test_rows.py` & `img2table-1.0.3/tests/tables/processing/borderless_tables/rows/test_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/segment_image/test_data/test.png` & `img2table-1.0.3/tests/tables/processing/borderless_tables/segment_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py` & `img2table-1.0.3/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json` & `img2table-1.0.3/tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/table/test_data/rows.json` & `img2table-1.0.3/tests/tables/processing/borderless_tables/table/test_data/rows.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/table/test_headers.py` & `img2table-1.0.3/tests/tables/processing/borderless_tables/table/test_headers.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/table/test_table.py` & `img2table-1.0.3/tests/tables/processing/borderless_tables/table/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/borderless_tables/table/test_table_creation.py` & `img2table-1.0.3/tests/tables/processing/borderless_tables/table/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/common/test_common.py` & `img2table-1.0.3/tests/tables/processing/common/test_common.py`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/common/test_data/test.jpg` & `img2table-1.0.3/tests/tables/processing/common/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/prepare_image/test_data/test.png` & `img2table-1.0.3/tests/tables/processing/prepare_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/text/test_data/ocr.csv` & `img2table-1.0.3/tests/tables/processing/text/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/text/test_data/table.json` & `img2table-1.0.3/tests/tables/processing/text/test_data/table.json`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/text/test_data/test.jpg` & `img2table-1.0.3/tests/tables/processing/text/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-1.0.2/tests/tables/processing/text/test_titles.py` & `img2table-1.0.3/tests/tables/processing/text/test_titles.py`

 * *Files identical despite different names*

