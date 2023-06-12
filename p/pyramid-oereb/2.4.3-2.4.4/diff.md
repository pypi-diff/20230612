# Comparing `tmp/pyramid_oereb-2.4.3.tar.gz` & `tmp/pyramid_oereb-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyramid_oereb-2.4.3.tar", last modified: Mon Apr 24 05:24:19 2023, max compression
+gzip compressed data, was "pyramid_oereb-2.4.4.tar", last modified: Mon Jun 12 13:20:10 2023, max compression
```

## Comparing `pyramid_oereb-2.4.3.tar` & `pyramid_oereb-2.4.4.tar`

### file list

```diff
@@ -1,231 +1,231 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.318411 pyramid_oereb-2.4.3/
--rw-r--r--   0 runner    (1001) docker     (122)    11663 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-04-24 05:24:19.318411 pyramid_oereb-2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6044 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.278410 pyramid_oereb-2.4.3/dev/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.278410 pyramid_oereb-2.4.3/dev/config/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/dev/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2680 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/dev/config/create_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.278410 pyramid_oereb-2.4.3/dev/database/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/dev/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8875 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/dev/database/load_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.278410 pyramid_oereb-2.4.3/pyramid_oereb/
--rw-r--r--   0 runner    (1001) docker     (122)     2495 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.282410 pyramid_oereb-2.4.3/pyramid_oereb/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)     3155 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.282410 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9772 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/create_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.282410 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/interlis_2_3/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/interlis_2_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2546 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/interlis_2_3/hook_methods.py
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/interlis_2_3/interlis_2_3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.282410 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/interlis_2_3/models/
--rw-r--r--   0 runner    (1001) docker     (122)      444 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/interlis_2_3/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27504 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/interlis_2_3/models/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.282410 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/interlis_2_3/sources/
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/interlis_2_3/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25565 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/interlis_2_3/sources/plr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.282410 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/oereblex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/oereblex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2650 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/oereblex/create_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.282410 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/oereblex/models/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/oereblex/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5780 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/oereblex/models/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.286410 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/oereblex/sources/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/oereblex/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12446 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/oereblex/sources/document.py
--rw-r--r--   0 runner    (1001) docker     (122)     6906 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/oereblex/sources/plr_oereblex.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.286410 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/create_tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/hook_methods.py
--rw-r--r--   0 runner    (1001) docker     (122)    13819 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/load_legend_entries.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.286410 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/models/
--rw-r--r--   0 runner    (1001) docker     (122)    19881 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15565 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/models/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     3839 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/models/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.290411 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1917 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/address.py
--rw-r--r--   0 runner    (1001) docker     (122)      942 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/availability.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/data_integration.py
--rw-r--r--   0 runner    (1001) docker     (122)      905 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/disclaimer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2097 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/document.py
--rw-r--r--   0 runner    (1001) docker     (122)      714 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/document_types.py
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/general_information.py
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/glossary.py
--rw-r--r--   0 runner    (1001) docker     (122)      812 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/law_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1532 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/legend.py
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/logo.py
--rw-r--r--   0 runner    (1001) docker     (122)      764 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/map_layering.py
--rw-r--r--   0 runner    (1001) docker     (122)     1168 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/municipality.py
--rw-r--r--   0 runner    (1001) docker     (122)      979 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/office.py
--rw-r--r--   0 runner    (1001) docker     (122)    31430 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/plr.py
--rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/real_estate.py
--rw-r--r--   0 runner    (1001) docker     (122)      827 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/real_estate_type.py
--rw-r--r--   0 runner    (1001) docker     (122)      803 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/theme.py
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/theme_document.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.290411 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/swisstopo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/swisstopo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3467 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/swisstopo/address.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.290411 pyramid_oereb-2.4.3/pyramid_oereb/contrib/print_proxy/
--rw-r--r--   0 runner    (1001) docker     (122)      452 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/print_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.290411 pyramid_oereb-2.4.3/pyramid_oereb/contrib/print_proxy/mapfish_print/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/print_proxy/mapfish_print/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36918 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/print_proxy/mapfish_print/mapfish_print.py
--rw-r--r--   0 runner    (1001) docker     (122)     4350 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/print_proxy/mapfish_print/toc_pages.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.294411 pyramid_oereb-2.4.3/pyramid_oereb/contrib/print_proxy/xml_2_pdf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/print_proxy/xml_2_pdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5132 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/print_proxy/xml_2_pdf/xml_2_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.294411 pyramid_oereb-2.4.3/pyramid_oereb/contrib/stats/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/stats/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.294411 pyramid_oereb-2.4.3/pyramid_oereb/contrib/stats/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/stats/scripts/create_stats_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.294411 pyramid_oereb-2.4.3/pyramid_oereb/contrib/stats/scripts/templates/
--rw-r--r--   0 runner    (1001) docker     (122)     5488 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/contrib/stats/scripts/templates/views.sql.mako
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.294411 pyramid_oereb-2.4.3/pyramid_oereb/core/
--rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4384 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/b64.py
--rw-r--r--   0 runner    (1001) docker     (122)    66765 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/config.py
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/exception.py
--rw-r--r--   0 runner    (1001) docker     (122)     6433 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/hook_methods.py
--rw-r--r--   0 runner    (1001) docker     (122)    15094 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.298411 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/
--rw-r--r--   0 runner    (1001) docker     (122)      419 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2422 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/address.py
--rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/availability.py
--rw-r--r--   0 runner    (1001) docker     (122)     2103 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/data_integration.py
--rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/disclaimer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/document.py
--rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/document_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     8107 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)     2095 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/general_information.py
--rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/glossary.py
--rw-r--r--   0 runner    (1001) docker     (122)     2124 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/law_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/logo.py
--rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/map_layering.py
--rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/municipality.py
--rw-r--r--   0 runner    (1001) docker     (122)     1976 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/office.py
--rw-r--r--   0 runner    (1001) docker     (122)     4320 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/real_estate.py
--rw-r--r--   0 runner    (1001) docker     (122)     2059 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/real_estate_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     1966 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/theme.py
--rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/readers/theme_document.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.306411 pyramid_oereb-2.4.3/pyramid_oereb/core/records/
--rw-r--r--   0 runner    (1001) docker     (122)      435 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/address.py
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/availability.py
--rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/data_integration.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/disclaimer.py
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/document_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     8638 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/documents.py
--rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/embeddable.py
--rw-r--r--   0 runner    (1001) docker     (122)     5844 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)     1128 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/general_information.py
--rw-r--r--   0 runner    (1001) docker     (122)    11019 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/glossary.py
--rw-r--r--   0 runner    (1001) docker     (122)     4312 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/image.py
--rw-r--r--   0 runner    (1001) docker     (122)      933 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/law_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/logo.py
--rw-r--r--   0 runner    (1001) docker     (122)      813 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/map_layering.py
--rw-r--r--   0 runner    (1001) docker     (122)      917 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/municipality.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/office.py
--rw-r--r--   0 runner    (1001) docker     (122)    11463 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/plr.py
--rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/real_estate.py
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/real_estate_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/theme.py
--rw-r--r--   0 runner    (1001) docker     (122)      961 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/theme_document.py
--rw-r--r--   0 runner    (1001) docker     (122)    12591 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/records/view_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.306411 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/
--rw-r--r--   0 runner    (1001) docker     (122)     7841 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.306411 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/capabilities/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/capabilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.274410 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/capabilities/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.306411 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/capabilities/templates/xml/
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/capabilities/templates/xml/capabilities.xml
--rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/capabilities/xml_.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.306411 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22110 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/json_.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.274410 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.310411 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/
--rw-r--r--   0 runner    (1001) docker     (122)      324 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/article.xml
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/data_source.xml
--rw-r--r--   0 runner    (1001) docker     (122)      326 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/disclaimer.xml
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/document.xml
--rw-r--r--   0 runner    (1001) docker     (122)      292 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/document_type.xml
--rw-r--r--   0 runner    (1001) docker     (122)     5218 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/extract.xml
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/general_information.xml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.310411 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/geometry/
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/geometry/line.xml
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/geometry/point.xml
--rw-r--r--   0 runner    (1001) docker     (122)      427 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/geometry/polygon.xml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/geometry.xml
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/glossary.xml
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/law_status.xml
--rw-r--r--   0 runner    (1001) docker     (122)      715 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/legend_entry.xml
--rw-r--r--   0 runner    (1001) docker     (122)      258 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/localized_image.xml
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/localized_text.xml
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/multilingual_text.xml
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/office.xml
--rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/public_law_restriction.xml
--rw-r--r--   0 runner    (1001) docker     (122)     2664 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/real_estate.xml
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/real_estate_type.xml
--rw-r--r--   0 runner    (1001) docker     (122)      527 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/specific_geometry.xml
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/theme.xml
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/view_service.xml
--rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/xml_.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.310411 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/getegrid/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/getegrid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.274410 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/getegrid/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.310411 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/getegrid/templates/xml/
--rw-r--r--   0 runner    (1001) docker     (122)     1917 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/getegrid/templates/xml/getegrid.xml
--rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/getegrid/xml_.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.314411 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/versions/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.274410 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/versions/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.314411 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/versions/templates/xml/
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/versions/templates/xml/versions.xml
--rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/versions/xml_.py
--rw-r--r--   0 runner    (1001) docker     (122)     4207 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.318411 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/address.py
--rw-r--r--   0 runner    (1001) docker     (122)      760 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/availability.py
--rw-r--r--   0 runner    (1001) docker     (122)      796 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/data_integration.py
--rw-r--r--   0 runner    (1001) docker     (122)      759 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/disclaimer.py
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/document.py
--rw-r--r--   0 runner    (1001) docker     (122)      773 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/document_types.py
--rw-r--r--   0 runner    (1001) docker     (122)      837 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/general_information.py
--rw-r--r--   0 runner    (1001) docker     (122)      704 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/glossary.py
--rw-r--r--   0 runner    (1001) docker     (122)      875 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/law_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/legend.py
--rw-r--r--   0 runner    (1001) docker     (122)      690 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/logo.py
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/map_layering.py
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/municipality.py
--rw-r--r--   0 runner    (1001) docker     (122)      684 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/office.py
--rw-r--r--   0 runner    (1001) docker     (122)     4185 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/plr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/real_estate.py
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/real_estate_type.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/theme.py
--rw-r--r--   0 runner    (1001) docker     (122)      764 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/sources/theme_document.py
--rw-r--r--   0 runner    (1001) docker     (122)     2579 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/url.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.318411 pyramid_oereb-2.4.3/pyramid_oereb/core/views/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36217 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/pyramid_oereb/core/views/webservice.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 05:24:19.282410 pyramid_oereb-2.4.3/pyramid_oereb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-04-24 05:24:19.000000 pyramid_oereb-2.4.3/pyramid_oereb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9138 2023-04-24 05:24:19.000000 pyramid_oereb-2.4.3/pyramid_oereb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 05:24:19.000000 pyramid_oereb-2.4.3/pyramid_oereb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      718 2023-04-24 05:24:19.000000 pyramid_oereb-2.4.3/pyramid_oereb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 05:24:19.000000 pyramid_oereb-2.4.3/pyramid_oereb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      714 2023-04-24 05:24:19.000000 pyramid_oereb-2.4.3/pyramid_oereb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-24 05:24:19.000000 pyramid_oereb-2.4.3/pyramid_oereb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      327 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-24 05:24:19.318411 pyramid_oereb-2.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2702 2023-04-24 05:24:09.000000 pyramid_oereb-2.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.677971 pyramid_oereb-2.4.4/
+-rw-r--r--   0 runner    (1001) docker     (122)    11815 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    18771 2023-06-12 13:20:10.677971 pyramid_oereb-2.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6044 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.645971 pyramid_oereb-2.4.4/dev/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/dev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.645971 pyramid_oereb-2.4.4/dev/config/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/dev/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2680 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/dev/config/create_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.645971 pyramid_oereb-2.4.4/dev/database/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/dev/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8875 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/dev/database/load_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.645971 pyramid_oereb-2.4.4/pyramid_oereb/
+-rw-r--r--   0 runner    (1001) docker     (122)     2495 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.649971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)     3155 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.649971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9772 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/create_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.649971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/interlis_2_3/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/interlis_2_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2546 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/interlis_2_3/hook_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/interlis_2_3/interlis_2_3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.649971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/interlis_2_3/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      444 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/interlis_2_3/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27504 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/interlis_2_3/models/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.653971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/interlis_2_3/sources/
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/interlis_2_3/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25565 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/interlis_2_3/sources/plr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.653971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/oereblex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/oereblex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2650 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/oereblex/create_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.653971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/oereblex/models/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/oereblex/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5780 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/oereblex/models/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.653971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/oereblex/sources/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/oereblex/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12446 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/oereblex/sources/document.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6906 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/oereblex/sources/plr_oereblex.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.653971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/create_tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/hook_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13819 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/load_legend_entries.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.657971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/models/
+-rw-r--r--   0 runner    (1001) docker     (122)    19881 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15565 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/models/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3839 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/models/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.661971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1917 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/address.py
+-rw-r--r--   0 runner    (1001) docker     (122)      942 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/availability.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/data_integration.py
+-rw-r--r--   0 runner    (1001) docker     (122)      905 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/disclaimer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2097 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/document.py
+-rw-r--r--   0 runner    (1001) docker     (122)      714 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/document_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/general_information.py
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/glossary.py
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/law_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1532 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/legend.py
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/logo.py
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/map_layering.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1168 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/municipality.py
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/office.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31430 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/plr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/real_estate.py
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/real_estate_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)      803 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/theme.py
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/theme_document.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.661971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/swisstopo/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/swisstopo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3467 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/swisstopo/address.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.661971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/print_proxy/
+-rw-r--r--   0 runner    (1001) docker     (122)      452 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/print_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.665971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/print_proxy/mapfish_print/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/print_proxy/mapfish_print/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36918 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/print_proxy/mapfish_print/mapfish_print.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4350 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/print_proxy/mapfish_print/toc_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.665971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/print_proxy/xml_2_pdf/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/print_proxy/xml_2_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5132 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/print_proxy/xml_2_pdf/xml_2_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.665971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/stats/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/stats/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.665971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/stats/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/stats/scripts/create_stats_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.665971 pyramid_oereb-2.4.4/pyramid_oereb/contrib/stats/scripts/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     5488 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/contrib/stats/scripts/templates/views.sql.mako
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.665971 pyramid_oereb-2.4.4/pyramid_oereb/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4384 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/b64.py
+-rw-r--r--   0 runner    (1001) docker     (122)    67356 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7444 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/hook_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15094 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.665971 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2422 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/address.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/availability.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2103 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/data_integration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/disclaimer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/document.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/document_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8107 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2095 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/general_information.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/glossary.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2124 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/law_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/logo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/map_layering.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/municipality.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1976 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/office.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4320 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/real_estate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2059 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/real_estate_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1966 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/theme.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/readers/theme_document.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.669971 pyramid_oereb-2.4.4/pyramid_oereb/core/records/
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/address.py
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/availability.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1585 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/data_integration.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/disclaimer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/document_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8638 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/documents.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/embeddable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5844 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1128 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/general_information.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11019 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/glossary.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4312 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)      933 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/law_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/logo.py
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/map_layering.py
+-rw-r--r--   0 runner    (1001) docker     (122)      917 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/municipality.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/office.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11463 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/plr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/real_estate.py
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/real_estate_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/theme.py
+-rw-r--r--   0 runner    (1001) docker     (122)      961 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/theme_document.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12591 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/records/view_service.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.669971 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/
+-rw-r--r--   0 runner    (1001) docker     (122)     9279 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.669971 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/capabilities/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/capabilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.637971 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/capabilities/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.669971 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/capabilities/templates/xml/
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/capabilities/templates/xml/capabilities.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/capabilities/xml_.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.669971 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21535 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/json_.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.641971 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.673971 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/article.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/data_source.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/disclaimer.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/document.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/document_type.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     5009 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/extract.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/general_information.xml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.673971 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/geometry/
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/geometry/line.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/geometry/point.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/geometry/polygon.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/geometry.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/glossary.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/law_status.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      715 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/legend_entry.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/localized_image.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/localized_text.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/multilingual_text.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/office.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/public_law_restriction.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     2664 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/real_estate.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/real_estate_type.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      527 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/specific_geometry.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/theme.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/view_service.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     3135 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/xml_.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.673971 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/getegrid/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/getegrid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.641971 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/getegrid/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.673971 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/getegrid/templates/xml/
+-rw-r--r--   0 runner    (1001) docker     (122)     1917 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/getegrid/templates/xml/getegrid.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/getegrid/xml_.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.673971 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/versions/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.641971 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/versions/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.673971 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/versions/templates/xml/
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/versions/templates/xml/versions.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/versions/xml_.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4207 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.677971 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/address.py
+-rw-r--r--   0 runner    (1001) docker     (122)      760 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/availability.py
+-rw-r--r--   0 runner    (1001) docker     (122)      796 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/data_integration.py
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/disclaimer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/document.py
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/document_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/general_information.py
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/glossary.py
+-rw-r--r--   0 runner    (1001) docker     (122)      875 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/law_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/legend.py
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/logo.py
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/map_layering.py
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/municipality.py
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/office.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4185 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/plr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/real_estate.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/real_estate_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/theme.py
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/sources/theme_document.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2579 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/url.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.677971 pyramid_oereb-2.4.4/pyramid_oereb/core/views/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36217 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/pyramid_oereb/core/views/webservice.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:20:10.649971 pyramid_oereb-2.4.4/pyramid_oereb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    18771 2023-06-12 13:20:10.000000 pyramid_oereb-2.4.4/pyramid_oereb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9138 2023-06-12 13:20:10.000000 pyramid_oereb-2.4.4/pyramid_oereb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 13:20:10.000000 pyramid_oereb-2.4.4/pyramid_oereb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      718 2023-06-12 13:20:10.000000 pyramid_oereb-2.4.4/pyramid_oereb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 13:20:10.000000 pyramid_oereb-2.4.4/pyramid_oereb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      712 2023-06-12 13:20:10.000000 pyramid_oereb-2.4.4/pyramid_oereb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-12 13:20:10.000000 pyramid_oereb-2.4.4/pyramid_oereb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-06-12 13:20:10.677971 pyramid_oereb-2.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2702 2023-06-12 13:19:59.000000 pyramid_oereb-2.4.4/setup.py
```

### Comparing `pyramid_oereb-2.4.3/CHANGES.rst` & `pyramid_oereb-2.4.4/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+2.4.4
+-----
+- Add option for a hook method for LogoRef URLs (#929, #1744)
+- Various minor library upgrades (urllib, requests, SQLAlchemy, geoalchemy2)
+
 2.4.3
 -----
 - Add support for newest oereblex API (via geolink-formatter, #1703)
 - Various minor library upgrades (SQLAlchemy, geoalchemy, psycopg2, pypdf)
 
 2.4.2
 -----
```

### Comparing `pyramid_oereb-2.4.3/LICENSE.txt` & `pyramid_oereb-2.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/PKG-INFO` & `pyramid_oereb-2.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyramid_oereb
-Version: 2.4.3
+Version: 2.4.4
 Summary: pyramid_oereb, extension for pyramid web frame work to provide a basic server part for the oereb project
 Home-page: https://github.com/openoereb/pyramid_oereb
 Author: François Voisard
 Author-email: francois.voisard@ne.ch
 License: BSD 2
 Keywords: pyramid oereb
 Classifier: Development Status :: 5 - Production/Stable
@@ -172,14 +172,19 @@
    :alt: Codacy Badge
    :target: https://app.codacy.com/gh/openoereb/pyramid_oereb?utm_source=github.com&utm_medium=referral&utm_content=openoereb/pyramid_oereb&utm_campaign=Badge_Grade_Settings
 
 
 Changelog
 =========
 
+2.4.4
+-----
+- Add option for a hook method for LogoRef URLs (#929, #1744)
+- Various minor library upgrades (urllib, requests, SQLAlchemy, geoalchemy2)
+
 2.4.3
 -----
 - Add support for newest oereblex API (via geolink-formatter, #1703)
 - Various minor library upgrades (SQLAlchemy, geoalchemy, psycopg2, pypdf)
 
 2.4.2
 -----
```

### Comparing `pyramid_oereb-2.4.3/README.rst` & `pyramid_oereb-2.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/dev/config/create_yaml.py` & `pyramid_oereb-2.4.4/dev/config/create_yaml.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/dev/database/load_sample_data.py` & `pyramid_oereb-2.4.4/dev/database/load_sample_data.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/__init__.py` & `pyramid_oereb-2.4.4/pyramid_oereb/__init__.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/__init__.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/__init__.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/create_tables.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/create_tables.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/interlis_2_3/hook_methods.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/interlis_2_3/hook_methods.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/interlis_2_3/interlis_2_3_utils.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/interlis_2_3/interlis_2_3_utils.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/interlis_2_3/models/theme.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/interlis_2_3/models/theme.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/interlis_2_3/sources/__init__.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/interlis_2_3/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/interlis_2_3/sources/plr.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/interlis_2_3/sources/plr.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/oereblex/create_tables.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/oereblex/create_tables.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/oereblex/models/theme.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/oereblex/models/theme.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/oereblex/sources/document.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/oereblex/sources/document.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/oereblex/sources/plr_oereblex.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/oereblex/sources/plr_oereblex.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/__init__.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/create_tables.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/create_tables.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/hook_methods.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/hook_methods.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/load_legend_entries.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/load_legend_entries.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/models/__init__.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/models/main.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/models/main.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/models/theme.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/models/theme.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/__init__.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/address.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/address.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/availability.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/availability.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/data_integration.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/data_integration.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/disclaimer.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/disclaimer.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/document.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/document.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/document_types.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/document_types.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/general_information.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/general_information.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/glossary.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/glossary.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/law_status.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/law_status.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/legend.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/legend.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/logo.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/logo.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/map_layering.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/map_layering.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/municipality.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/municipality.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/office.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/office.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/plr.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/plr.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/real_estate.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/real_estate.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/real_estate_type.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/real_estate_type.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/theme.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/theme.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/standard/sources/theme_document.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/standard/sources/theme_document.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/data_sources/swisstopo/address.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/data_sources/swisstopo/address.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/print_proxy/mapfish_print/mapfish_print.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/print_proxy/mapfish_print/mapfish_print.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/print_proxy/mapfish_print/toc_pages.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/print_proxy/mapfish_print/toc_pages.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/print_proxy/xml_2_pdf/xml_2_pdf.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/print_proxy/xml_2_pdf/xml_2_pdf.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/stats/decorators.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/stats/decorators.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/stats/scripts/create_stats_tables.py` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/stats/scripts/create_stats_tables.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/contrib/stats/scripts/templates/views.sql.mako` & `pyramid_oereb-2.4.4/pyramid_oereb/contrib/stats/scripts/templates/views.sql.mako`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/__init__.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/adapter.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/adapter.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/b64.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/b64.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/config.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -726,14 +726,33 @@
         Returns:
             str: Code of confedertaion logo provided in config.
         """
 
         return Config.get_logo_lookup('confederation')
 
     @staticmethod
+    def get_logo_hooks():
+        """
+        Returns the hook methods specified in config file.
+
+        Returns:
+            list: list of hook methods provided in config in dotted names.
+
+        Raises:
+            ConfigurationError
+        """
+
+        logo_config = Config.get_logo_config()
+        if logo_config is None:
+            raise ConfigurationError("Missing configuration for logos")
+        if logo_config.get('hooks') is None:
+            raise ConfigurationError("Missing configuration for logos hook methods")
+        return logo_config.get('hooks')
+
+    @staticmethod
     def init_document_types():
         """
         Initiates all document types configured in the config file.
 
         Raises:
             ProgrammingError
         """
```

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/hook_methods.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/hook_methods.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import re
 from mako.template import Template
 from pyramid.path import AssetResolver
 from functools import cmp_to_key
 
 from pyramid_oereb import route_prefix
+from pyramid_oereb.core import get_multilingual_element
 from pyramid_oereb.core.records.office import OfficeRecord
 
 
 def get_symbol(params, theme_config):
     """
     This is a dummy method only to define what is expected by the real implementation.
 
@@ -44,14 +45,54 @@
         '{0}/image/symbol'.format(route_prefix),
         theme_code=record.theme.code,
         extension=record.symbol.extension,
         _query=query
     )
 
 
+def get_logo_ref(request, logo_code, language, image_dict):
+    """
+    Returns the link to the logos.
+
+    Args:
+        request (pyramid.request.Request): The current request instance.
+        logo_code (str): Code of logo, eg. bs or ch.
+        language (str): language of extract.
+        image_dict (dict): dict of image
+
+    Returns:
+        uri: the link to the logos.
+    """
+
+    return request.route_url(
+        '{0}/image/logo'.format(route_prefix),
+        logo=logo_code,
+        language=language,
+        extension=get_multilingual_element(
+                image_dict,
+                language
+            ).extension
+    )
+
+
+def get_qr_code_ref(request, qr_code_ref):
+    """
+    Returns the link for the qr_code.
+
+    Args:
+        request (pyramid.request.Request): The current request instance.
+        qr_code_ref (str): The string of qr-code url.
+
+    Returns:
+        uri: the link to the qr_code.
+    """
+
+    return qr_code_ref
+
+
 def get_surveying_data_provider(real_estate):
     """
 
     Args:
         real_estate (pyramid_oereb.lib.records.real_estate.RealEstateRecord): The real estate for which the
             provider of the surveying data should be delivered.
     Returns:
```

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/processor.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/processor.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/address.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/address.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/availability.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/availability.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/data_integration.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/data_integration.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/disclaimer.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/disclaimer.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/document.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/document.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/document_types.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/document_types.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/extract.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/extract.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/general_information.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/general_information.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/glossary.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/glossary.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/law_status.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/law_status.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/logo.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/logo.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/map_layering.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/map_layering.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/municipality.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/municipality.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/office.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/office.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/real_estate.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/real_estate.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/real_estate_type.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/real_estate_type.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/theme.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/theme.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/readers/theme_document.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/readers/theme_document.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/address.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/address.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/availability.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/availability.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/data_integration.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/data_integration.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/disclaimer.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/disclaimer.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/document_types.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/document_types.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/documents.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/documents.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/embeddable.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/embeddable.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/extract.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/extract.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/general_information.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/general_information.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/geometry.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/geometry.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/glossary.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/glossary.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/image.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/image.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/law_status.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/law_status.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/logo.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/logo.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/map_layering.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/map_layering.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/municipality.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/municipality.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/office.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/office.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/plr.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/plr.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/real_estate.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/real_estate.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/real_estate_type.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/real_estate_type.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/theme.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/theme.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/theme_document.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/theme_document.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/records/view_service.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/records/view_service.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/__init__.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -49,14 +49,54 @@
                 method = DottedNameResolver().resolve(plr.get('hooks').get('get_symbol_ref'))
         if callable(method):
             return method(request, record)
         log.error('No "get_symbol_ref" method found for theme {}'.format(record.theme.code))
         raise HTTPServerError()
 
     @classmethod
+    def get_logo_ref(cls, request, logo_code, language, image_dict):
+        """
+        Returns the link to the symbol of the specified logo.
+
+        Args:
+            request (pyramid.request.Request): The current request instance.
+            logo_code (str): Code of logo, eg. bs or ch.
+            language (str): language of extract.
+            image_dict (dict): dict of image
+
+        Returns:
+            uri: The link to the symbol for the specified logo.
+        """
+        method = None
+        method = DottedNameResolver().resolve(Config.get_logo_hooks().get('get_logo_ref'))
+        if callable(method):
+            return method(request, logo_code, language, image_dict)
+        log.error('No "get_logo_ref" method found for logos')
+        raise HTTPServerError()
+
+    @classmethod
+    def get_qr_code_ref(cls, request, qr_code_ref):
+        """
+        Returns the link for the qr_code.
+
+        Args:
+            request (pyramid.request.Request): The current request instance.
+            qr_code_ref (str): The string of qr-code url.
+
+        Returns:
+            uri: the link to the qr_code.
+        """
+        method = None
+        method = DottedNameResolver().resolve(Config.get_logo_hooks().get('get_qr_code_ref'))
+        if callable(method):
+            return method(request, qr_code_ref)
+        log.error('No "get_qr_code_ref" method found for logos')
+        raise HTTPServerError()
+
+    @classmethod
     def get_response(cls, system):
         """
         Returns the response object if available.
 
         Args:
             system (dict): The available system properties.
```

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/capabilities/templates/xml/capabilities.xml` & `pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/capabilities/templates/xml/capabilities.xml`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/capabilities/xml_.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/capabilities/xml_.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/json_.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/json_.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from json import dumps
 
 from pyramid.request import Request
 from pyramid.response import Response
 from pyramid.testing import DummyRequest
 
-from pyramid_oereb import Config, route_prefix
+from pyramid_oereb import Config
 from pyramid_oereb.core import get_multilingual_element
 from pyramid_oereb.core.records.documents import DocumentRecord
 from pyramid_oereb.core.records.theme import ThemeRecord
 from pyramid_oereb.core.sources.plr import PlrRecord
 
 from pyramid_oereb.core.renderer import Base
 from pyramid_oereb.core.views.webservice import Parameter
@@ -115,52 +115,43 @@
                         extract.municipality_logo.image_dict,
                         self._language
                     ).encode(),
                 'QRCode': extract.qr_code.encode()
             })
         else:
             extract_dict.update({
-                'LogoPLRCadastreRef': self._request.route_url(
-                    '{0}/image/logo'.format(route_prefix),
-                    logo='oereb',
-                    language=self._language,
-                    extension=get_multilingual_element(
-                            extract.logo_plr_cadastre.image_dict,
-                            self._language
-                        ).extension
-                ),
-                'FederalLogoRef': self._request.route_url(
-                    '{0}/image/logo'.format(route_prefix),
-                    logo='confederation',
-                    language=self._language,
-                    extension=get_multilingual_element(
-                            extract.federal_logo.image_dict,
-                            self._language
-                        ).extension
-                ),
-                'CantonalLogoRef': self._request.route_url(
-                    '{0}/image/logo'.format(route_prefix),
-                    logo='canton',
-                    language=self._language,
-                    extension=get_multilingual_element(
-                            extract.cantonal_logo.image_dict,
-                            self._language
-                        ).extension
-                ),
-                'MunicipalityLogoRef': self._request.route_url(
-                    '{0}/image/logo'.format(route_prefix),
-                    logo='municipality',
-                    language=self._language,
-                    extension=get_multilingual_element(
-                            extract.municipality_logo.image_dict,
-                            self._language
-                        ).extension
-                ) + '?fosnr={}'.format(extract.real_estate.fosnr),
-                'QRCodeRef': extract.qr_code_ref
-            })
+                'LogoPLRCadastreRef': self.get_logo_ref(
+                        self._request,
+                        'oereb',
+                        self._language,
+                        extract.logo_plr_cadastre.image_dict
+                    ),
+                'FederalLogoRef': self.get_logo_ref(
+                        self._request,
+                        'confederation',
+                        self._language,
+                        extract.federal_logo.image_dict
+                    ),
+                'CantonalLogoRef': self.get_logo_ref(
+                        self._request,
+                        'canton',
+                        self._language,
+                        extract.cantonal_logo.image_dict
+                    ),
+                'MunicipalityLogoRef': self.get_logo_ref(
+                        self._request,
+                        'municipality',
+                        self._language,
+                        extract.municipality_logo.image_dict
+                    ) + '?fosnr={}'.format(extract.real_estate.fosnr),
+                'QRCodeRef': self.get_qr_code_ref(
+                        self._request,
+                        extract.qr_code_ref
+                    )
+                })
 
         if extract.electronic_signature is not None:
             extract_dict['ElectronicSignature'] = extract.electronic_signature
 
         if isinstance(extract.general_information, list) and len(extract.general_information) > 0:
             general_information = list()
             for info in extract.general_information:
```

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/document.xml` & `pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/document.xml`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/extract.xml` & `pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/extract.xml`

 * *Files 24% similar despite different names*

```diff
@@ -61,20 +61,20 @@
         <data:LogoPLRCadastre>${get_multilingual_element(extract.logo_plr_cadastre.image_dict, language).encode()}</data:LogoPLRCadastre>
         <data:FederalLogo>${get_multilingual_element(extract.federal_logo.image_dict, language).encode()}</data:FederalLogo>
         <data:CantonalLogo>${get_multilingual_element(extract.cantonal_logo.image_dict, language).encode()}</data:CantonalLogo>
         <data:MunicipalityLogo>${get_multilingual_element(extract.municipality_logo.image_dict, language).encode()}</data:MunicipalityLogo>
         <data:ExtractIdentifier>${extract.extract_identifier}</data:ExtractIdentifier>
         <data:QRCode>${extract.qr_code.encode()}</data:QRCode>
     %else:
-        <data:LogoPLRCadastreRef>${request.route_url('{0}/image/logo'.format(route_prefix), logo='oereb', language=language, extension=get_multilingual_element(extract.logo_plr_cadastre.image_dict, language).extension) | x}</data:LogoPLRCadastreRef>
-        <data:FederalLogoRef>${request.route_url('{0}/image/logo'.format(route_prefix), logo='confederation', language=language, extension=get_multilingual_element(extract.federal_logo.image_dict, language).extension) | x}</data:FederalLogoRef>
-        <data:CantonalLogoRef>${request.route_url('{0}/image/logo'.format(route_prefix), logo='canton', language=language, extension=get_multilingual_element(extract.cantonal_logo.image_dict, language).extension) | x}</data:CantonalLogoRef>
-        <data:MunicipalityLogoRef>${request.route_url('{0}/image/logo'.format(route_prefix), logo='municipality', language=language, extension=get_multilingual_element(extract.municipality_logo.image_dict, language).extension) + '?fosnr={}'.format(extract.real_estate.fosnr) | x}</data:MunicipalityLogoRef>
+        <data:LogoPLRCadastreRef>${get_logo_ref(request=request, logo_code='oereb', language=language, image_dict=extract.logo_plr_cadastre.image_dict) | x}</data:LogoPLRCadastreRef>
+        <data:FederalLogoRef>${get_logo_ref(request=request, logo_code='confederation', language=language, image_dict=extract.logo_plr_cadastre.image_dict) | x}</data:FederalLogoRef>
+        <data:CantonalLogoRef>${get_logo_ref(request=request, logo_code='canton', language=language, image_dict=extract.logo_plr_cadastre.image_dict) | x}</data:CantonalLogoRef>
+        <data:MunicipalityLogoRef>${get_logo_ref(request=request, logo_code='municipality', language=language, image_dict=extract.logo_plr_cadastre.image_dict) + '?fosnr={}'.format(extract.real_estate.fosnr) | x}</data:MunicipalityLogoRef>
         <data:ExtractIdentifier>${extract.extract_identifier}</data:ExtractIdentifier>
-        <data:QRCodeRef>${extract.qr_code_ref}</data:QRCodeRef>
+        <data:QRCodeRef>${get_qr_code_ref(request=request, qr_code_ref=extract.qr_code_ref) | x}</data:QRCodeRef>
     %endif
     %for general_information in extract.general_information:
         <%include file="general_information.xml" args="general_information=general_information"/>
     %endfor
         %for glossary in sorted_glossaries:
         <%include file="glossary.xml" args="glossary=glossary"/>
         %endfor
```

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/legend_entry.xml` & `pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/legend_entry.xml`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/office.xml` & `pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/office.xml`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/public_law_restriction.xml` & `pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/public_law_restriction.xml`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/real_estate.xml` & `pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/real_estate.xml`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/specific_geometry.xml` & `pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/specific_geometry.xml`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/templates/xml/view_service.xml` & `pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/templates/xml/view_service.xml`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/extract/xml_.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/extract/xml_.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,10 +79,12 @@
             'params': params,
             'sort_by_localized_text': self.sort_by_localized_text,
             'localized': self.get_localized_text,
             'multilingual': self.get_multilingual_text,
             'get_localized_image': self.get_localized_image,
             'request': self._request,
             'get_symbol_ref': self.get_symbol_ref,
+            'get_logo_ref': self.get_logo_ref,
+            'get_qr_code_ref': self.get_qr_code_ref,
             'date_format': '%Y-%m-%dT%H:%M:%S'
         })
         return content
```

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/getegrid/templates/xml/getegrid.xml` & `pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/getegrid/templates/xml/getegrid.xml`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/getegrid/xml_.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/getegrid/xml_.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/versions/templates/xml/versions.xml` & `pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/versions/templates/xml/versions.xml`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/renderer/versions/xml_.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/renderer/versions/xml_.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/routes.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/routes.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/__init__.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/address.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/address.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/availability.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/availability.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/data_integration.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/data_integration.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/disclaimer.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/disclaimer.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/document.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/document.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/document_types.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/document_types.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/general_information.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/general_information.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/glossary.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/glossary.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/law_status.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/law_status.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/legend.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/legend.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/logo.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/logo.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/map_layering.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/map_layering.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/municipality.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/municipality.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/office.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/office.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/plr.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/plr.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/real_estate.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/real_estate.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/real_estate_type.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/real_estate_type.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/theme.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/theme.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/sources/theme_document.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/sources/theme_document.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/url.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/url.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb/core/views/webservice.py` & `pyramid_oereb-2.4.4/pyramid_oereb/core/views/webservice.py`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb.egg-info/PKG-INFO` & `pyramid_oereb-2.4.4/pyramid_oereb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyramid-oereb
-Version: 2.4.3
+Version: 2.4.4
 Summary: pyramid_oereb, extension for pyramid web frame work to provide a basic server part for the oereb project
 Home-page: https://github.com/openoereb/pyramid_oereb
 Author: François Voisard
 Author-email: francois.voisard@ne.ch
 License: BSD 2
 Keywords: pyramid oereb
 Classifier: Development Status :: 5 - Production/Stable
@@ -172,14 +172,19 @@
    :alt: Codacy Badge
    :target: https://app.codacy.com/gh/openoereb/pyramid_oereb?utm_source=github.com&utm_medium=referral&utm_content=openoereb/pyramid_oereb&utm_campaign=Badge_Grade_Settings
 
 
 Changelog
 =========
 
+2.4.4
+-----
+- Add option for a hook method for LogoRef URLs (#929, #1744)
+- Various minor library upgrades (urllib, requests, SQLAlchemy, geoalchemy2)
+
 2.4.3
 -----
 - Add support for newest oereblex API (via geolink-formatter, #1703)
 - Various minor library upgrades (SQLAlchemy, geoalchemy, psycopg2, pypdf)
 
 2.4.2
 -----
```

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb.egg-info/SOURCES.txt` & `pyramid_oereb-2.4.4/pyramid_oereb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb.egg-info/entry_points.txt` & `pyramid_oereb-2.4.4/pyramid_oereb.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pyramid_oereb-2.4.3/pyramid_oereb.egg-info/requires.txt` & `pyramid_oereb-2.4.4/pyramid_oereb.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,36 +16,36 @@
 mako-render
 requests
 geolink-formatter
 pyconizer
 c2cwsgiutils[standard]
 
 [recommend]
-pypdf==3.8.1
+pypdf==3.9.1
 filetype==1.2.0
-geoalchemy2==0.13.2
+geoalchemy2==0.13.3
 pyramid==2.0.1
 pyramid-debugtoolbar==4.10
 qrcode==7.4.2
 image==1.5.33
 shapely==2.0.1
-SQLAlchemy==2.0.10
+SQLAlchemy==2.0.15
 pyaml-env==1.2.1
-urllib3==1.26.15
+urllib3==2.0.3
 waitress==2.1.2
 pyreproj==2.0.0
 mako-render==0.1.0
-requests==2.28.2
+requests==2.31.0
 geolink-formatter==2.0.4
 pyconizer==0.1.4
 c2cwsgiutils[standard]==5.2.2
 
 [testing]
 jsonschema==4.17.3
 lxml==4.9.2
 pytest==7.3.1
-pytest-cov==4.0.0
+pytest-cov==4.1.0
 pytest-ordering==0.6
-requests-mock==1.10.0
+requests-mock==1.11.0
 responses==0.23.1
 webtest==3.0.0
 pillow==9.5.0
```

### Comparing `pyramid_oereb-2.4.3/setup.py` & `pyramid_oereb-2.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 with open('tests-requirements.txt') as f:
     re_ = a = re.compile(r'(.+)==')
     tests_require = f.read().splitlines()
 
 setup(
     name='pyramid_oereb',
-    version='2.4.3',
+    version='2.4.4',
     description='pyramid_oereb, extension for pyramid web frame work to provide '
             'a basic server part for the oereb project',
     long_description='{readme}\n\n{changes}'.format(readme=README, changes=CHANGES),
     long_description_content_type='text/x-rst',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

