# Comparing `tmp/python-takauma-0.5.3.tar.gz` & `tmp/python-takauma-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-takauma-0.5.3.tar", last modified: Thu Jun  1 11:16:40 2023, max compression
+gzip compressed data, was "python-takauma-0.5.4.tar", last modified: Mon Jun 12 06:13:39 2023, max compression
```

## Comparing `python-takauma-0.5.3.tar` & `python-takauma-0.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-01 11:16:40.990776 python-takauma-0.5.3/
--rw-r--r--   0 aha        (501) staff       (20)      254 2023-06-01 11:16:40.990588 python-takauma-0.5.3/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)     2229 2020-05-15 10:48:55.000000 python-takauma-0.5.3/README.md
--rw-r--r--   0 aha        (501) staff       (20)       80 2023-06-01 11:13:49.000000 python-takauma-0.5.3/pyproject.toml
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-01 11:16:40.989229 python-takauma-0.5.3/python_takauma.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)      254 2023-06-01 11:16:40.000000 python-takauma-0.5.3/python_takauma.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      393 2023-06-01 11:16:40.000000 python-takauma-0.5.3/python_takauma.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-01 11:16:40.000000 python-takauma-0.5.3/python_takauma.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)     2697 2023-06-01 11:16:40.000000 python-takauma-0.5.3/python_takauma.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)        1 2020-05-14 20:09:27.000000 python-takauma-0.5.3/python_takauma.egg-info/not-zip-safe
--rw-r--r--   0 aha        (501) staff       (20)       47 2023-06-01 11:16:40.000000 python-takauma-0.5.3/python_takauma.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)        8 2023-06-01 11:16:40.000000 python-takauma-0.5.3/python_takauma.egg-info/top_level.txt
--rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-01 11:16:40.990818 python-takauma-0.5.3/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)      569 2020-05-29 15:42:32.000000 python-takauma-0.5.3/setup.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-01 11:16:40.990379 python-takauma-0.5.3/takauma/
--rw-r--r--   0 aha        (501) staff       (20)     2086 2023-06-01 11:05:49.000000 python-takauma-0.5.3/takauma/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)     1715 2021-08-23 14:02:04.000000 python-takauma-0.5.3/takauma/hakemisto.py
--rw-r--r--   0 aha        (501) staff       (20)     2931 2022-03-09 07:37:11.000000 python-takauma-0.5.3/takauma/jakelu.py
--rw-r--r--   0 aha        (501) staff       (20)     1361 2020-05-22 14:28:49.000000 python-takauma-0.5.3/takauma/luokka.py
--rw-r--r--   0 aha        (501) staff       (20)     4465 2021-08-23 14:02:04.000000 python-takauma-0.5.3/takauma/moduuli.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:13:39.608798 python-takauma-0.5.4/
+-rw-r--r--   0 aha        (501) staff       (20)      254 2023-06-12 06:13:39.608567 python-takauma-0.5.4/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)     2229 2020-05-15 10:48:55.000000 python-takauma-0.5.4/README.md
+-rw-r--r--   0 aha        (501) staff       (20)       80 2023-06-01 11:13:49.000000 python-takauma-0.5.4/pyproject.toml
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:13:39.607220 python-takauma-0.5.4/python_takauma.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)      254 2023-06-12 06:13:39.000000 python-takauma-0.5.4/python_takauma.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      393 2023-06-12 06:13:39.000000 python-takauma-0.5.4/python_takauma.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-12 06:13:39.000000 python-takauma-0.5.4/python_takauma.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)     2846 2023-06-12 06:13:39.000000 python-takauma-0.5.4/python_takauma.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)        1 2020-05-14 20:09:27.000000 python-takauma-0.5.4/python_takauma.egg-info/not-zip-safe
+-rw-r--r--   0 aha        (501) staff       (20)       33 2023-06-12 06:13:39.000000 python-takauma-0.5.4/python_takauma.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)        8 2023-06-12 06:13:39.000000 python-takauma-0.5.4/python_takauma.egg-info/top_level.txt
+-rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-12 06:13:39.608847 python-takauma-0.5.4/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)      474 2023-06-07 07:46:38.000000 python-takauma-0.5.4/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-12 06:13:39.608323 python-takauma-0.5.4/takauma/
+-rw-r--r--   0 aha        (501) staff       (20)     2086 2023-06-01 11:05:49.000000 python-takauma-0.5.4/takauma/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)     1715 2021-08-23 14:02:04.000000 python-takauma-0.5.4/takauma/hakemisto.py
+-rw-r--r--   0 aha        (501) staff       (20)     2931 2022-03-09 07:37:11.000000 python-takauma-0.5.4/takauma/jakelu.py
+-rw-r--r--   0 aha        (501) staff       (20)     1361 2020-05-22 14:28:49.000000 python-takauma-0.5.4/takauma/luokka.py
+-rw-r--r--   0 aha        (501) staff       (20)     4465 2021-08-23 14:02:04.000000 python-takauma-0.5.4/takauma/moduuli.py
```

### Comparing `python-takauma-0.5.3/README.md` & `python-takauma-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `python-takauma-0.5.3/python_takauma.egg-info/historia.json` & `python-takauma-0.5.4/python_takauma.egg-info/historia.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {'insert': "[(0, OrderedDict([('revisio', '1ee94f2d9b90b23427bfba7d68795dac5e0e1836'), ('versio', "*

 * *           "'0.5.4'), ('kuvaus', 'Päivitetty asennusmääritys')]))]"}*

```diff
@@ -1,9 +1,14 @@
 [
     {
+        "kuvaus": "P\u00e4ivitetty asennusm\u00e4\u00e4ritys",
+        "revisio": "1ee94f2d9b90b23427bfba7d68795dac5e0e1836",
+        "versio": "0.5.4"
+    },
+    {
         "kuvaus": "Lis\u00e4tty PEP-paketointim\u00e4\u00e4ritys",
         "revisio": "ce71cdde08740e31e1c96b1f8be50b4023da17fb",
         "versio": "0.5.3"
     },
     {
         "kuvaus": "Vaiennetaan varoitukset `__getattr__`-ylikuormitukseen liittyen",
         "revisio": "cb2947be6586a85bbbe7a6a1b3205095e4cdcd35",
```

### Comparing `python-takauma-0.5.3/takauma/__init__.py` & `python-takauma-0.5.4/takauma/__init__.py`

 * *Files identical despite different names*

### Comparing `python-takauma-0.5.3/takauma/hakemisto.py` & `python-takauma-0.5.4/takauma/hakemisto.py`

 * *Files identical despite different names*

### Comparing `python-takauma-0.5.3/takauma/jakelu.py` & `python-takauma-0.5.4/takauma/jakelu.py`

 * *Files identical despite different names*

### Comparing `python-takauma-0.5.3/takauma/luokka.py` & `python-takauma-0.5.4/takauma/luokka.py`

 * *Files identical despite different names*

### Comparing `python-takauma-0.5.3/takauma/moduuli.py` & `python-takauma-0.5.4/takauma/moduuli.py`

 * *Files identical despite different names*

