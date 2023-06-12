# Comparing `tmp/psl-2023.5.8.tar.gz` & `tmp/psl-2023.6.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psl-2023.5.8.tar", last modified: Mon May  8 13:05:37 2023, max compression
+gzip compressed data, was "psl-2023.6.12.tar", last modified: Mon Jun 12 13:05:37 2023, max compression
```

## Comparing `psl-2023.5.8.tar` & `psl-2023.6.12.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:05:37.747381 psl-2023.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-05-08 13:04:54.000000 psl-2023.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-08 13:04:54.000000 psl-2023.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-08 13:05:37.747381 psl-2023.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-08 13:04:54.000000 psl-2023.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:05:37.743381 psl-2023.5.8/psl/
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-08 13:05:05.000000 psl-2023.5.8/psl/__init__.py
--rw-------   0 runner    (1001) docker     (123)   109057 2023-05-08 13:05:05.000000 psl-2023.5.8/psl/psl.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:54.000000 psl-2023.5.8/psl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:05:37.747381 psl-2023.5.8/psl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-08 13:05:37.000000 psl-2023.5.8/psl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-08 13:05:37.000000 psl-2023.5.8/psl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:05:37.000000 psl-2023.5.8/psl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:05:22.000000 psl-2023.5.8/psl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-08 13:05:37.000000 psl-2023.5.8/psl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:05:37.747381 psl-2023.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-08 13:04:54.000000 psl-2023.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:05:37.263585 psl-2023.6.12/
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-06-12 13:05:02.000000 psl-2023.6.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 13:05:02.000000 psl-2023.6.12/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-12 13:05:37.263585 psl-2023.6.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-12 13:05:02.000000 psl-2023.6.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:05:37.263585 psl-2023.6.12/psl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-12 13:05:12.000000 psl-2023.6.12/psl/__init__.py
+-rw-------   0 runner    (1001) docker     (123)   109019 2023-06-12 13:05:12.000000 psl-2023.6.12/psl/psl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:05:02.000000 psl-2023.6.12/psl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:05:37.263585 psl-2023.6.12/psl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-12 13:05:37.000000 psl-2023.6.12/psl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-12 13:05:37.000000 psl-2023.6.12/psl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:05:37.000000 psl-2023.6.12/psl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:05:25.000000 psl-2023.6.12/psl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-12 13:05:37.000000 psl-2023.6.12/psl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:05:37.263585 psl-2023.6.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-12 13:05:02.000000 psl-2023.6.12/setup.py
```

### Comparing `psl-2023.5.8/LICENSE` & `psl-2023.6.12/LICENSE`

 * *Files identical despite different names*

### Comparing `psl-2023.5.8/PKG-INFO` & `psl-2023.6.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2023.5.8
+Version: 2023.6.12
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2023.5.8/README.md` & `psl-2023.6.12/README.md`

 * *Files identical despite different names*

### Comparing `psl-2023.5.8/psl/__init__.py` & `psl-2023.6.12/psl/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import pathlib
 import typing
 
-__version__ = "2023.5.8"
-__checksum__ = "76d72cafbb85dd7412b50757685c721d91c8a356"
+__version__ = "2023.6.12"
+__checksum__ = "5c35aaf6e7583a27a11d266425d198d0d92ddca6"
 __all__ = ["PUBLIC_SUFFIX_URL", "domain_suffixes", "Suffixes", "domain_can_set_cookie"]
 
 
 PUBLIC_SUFFIX_URL = "https://publicsuffix.org/list/public_suffix_list.dat"
 _PUBLIC_SUFFIX_PATH = pathlib.Path(__file__).parent / "psl.txt"
```

### Comparing `psl-2023.5.8/psl/psl.txt` & `psl-2023.6.12/psl/psl.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5691,15 +5691,14 @@
 ac.zw
 co.zw
 gov.zw
 mil.zw
 org.zw
 aaa
 aarp
-abarth
 abb
 abbott
 abbvie
 abc
 able
 abogado
 abudhabi
@@ -5718,15 +5717,14 @@
 agakhan
 agency
 aig
 airbus
 airforce
 airtel
 akdn
-alfaromeo
 alibaba
 alipay
 allfinanz
 allstate
 ally
 alsace
 alstom
@@ -6023,15 +6021,14 @@
 farmers
 fashion
 fast
 fedex
 feedback
 ferrari
 ferrero
-fiat
 fidelity
 fido
 film
 final
 finance
 financial
 fire
@@ -6230,15 +6227,14 @@
 kred
 kuokgroup
 kyoto
 lacaixa
 lamborghini
 lamer
 lancaster
-lancia
 land
 landrover
 lanxess
 lasalle
 lat
 latino
 latrobe
@@ -6293,15 +6289,14 @@
 mango
 map
 market
 marketing
 markets
 marriott
 marshalls
-maserati
 mattel
 mba
 mckinsey
 med
 media
 meet
 melbourne
```

### Comparing `psl-2023.5.8/psl.egg-info/PKG-INFO` & `psl-2023.6.12/psl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2023.5.8
+Version: 2023.6.12
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2023.5.8/setup.py` & `psl-2023.6.12/setup.py`

 * *Files identical despite different names*

