# Comparing `tmp/FoKL-1.2.0.tar.gz` & `tmp/FoKL-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FoKL-1.2.0.tar", last modified: Fri Jun  9 18:49:09 2023, max compression
+gzip compressed data, was "FoKL-1.2.6.tar", last modified: Mon Jun 12 16:13:12 2023, max compression
```

## Comparing `FoKL-1.2.0.tar` & `FoKL-1.2.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:49:09.812375 FoKL-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:49:09.808375 FoKL-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:49:09.808375 FoKL-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 18:49:00.000000 FoKL-1.2.0/.github/workflows/python-publish.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:49:09.808375 FoKL-1.2.0/Examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:49:09.808375 FoKL-1.2.0/Examples/Lorenz/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:49:00.000000 FoKL-1.2.0/Examples/Lorenz/ReadMe.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:49:09.808375 FoKL-1.2.0/Examples/Sinusoid/
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-09 18:49:00.000000 FoKL-1.2.0/Examples/Sinusoid/DATA_nois.csv
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 18:49:00.000000 FoKL-1.2.0/Examples/Sinusoid/ReadMe.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-09 18:49:00.000000 FoKL-1.2.0/Examples/Sinusoid/X.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-09 18:49:00.000000 FoKL-1.2.0/Examples/Sinusoid/Y.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-09 18:49:00.000000 FoKL-1.2.0/Examples/Sinusoid/python_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-09 18:49:00.000000 FoKL-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-09 18:49:09.812375 FoKL-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 18:49:00.000000 FoKL-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-09 18:49:00.000000 FoKL-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-09 18:49:09.812375 FoKL-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:49:09.808375 FoKL-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:49:09.812375 FoKL-1.2.0/src/FoKL/
--rw-r--r--   0 runner    (1001) docker     (123)    34582 2023-06-09 18:49:00.000000 FoKL-1.2.0/src/FoKL/FoKLRoutines.py
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-06-09 18:49:00.000000 FoKL-1.2.0/src/FoKL/GP_Integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:49:00.000000 FoKL-1.2.0/src/FoKL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-09 18:49:00.000000 FoKL-1.2.0/src/FoKL/coverage3.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-09 18:49:00.000000 FoKL-1.2.0/src/FoKL/emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-09 18:49:00.000000 FoKL-1.2.0/src/FoKL/gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-09 18:49:00.000000 FoKL-1.2.0/src/FoKL/splineConvert500.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:49:09.812375 FoKL-1.2.0/src/FoKL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-09 18:49:09.000000 FoKL-1.2.0/src/FoKL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-09 18:49:09.000000 FoKL-1.2.0/src/FoKL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:49:09.000000 FoKL-1.2.0/src/FoKL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-09 18:49:09.000000 FoKL-1.2.0/src/FoKL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 18:49:09.000000 FoKL-1.2.0/src/FoKL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:13:12.168571 FoKL-1.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:13:12.156571 FoKL-1.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:13:12.160570 FoKL-1.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-12 16:12:57.000000 FoKL-1.2.6/.github/workflows/python-publish.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:13:12.160570 FoKL-1.2.6/Examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:13:12.160570 FoKL-1.2.6/Examples/Lorenz/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:12:57.000000 FoKL-1.2.6/Examples/Lorenz/ReadMe.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:13:12.164571 FoKL-1.2.6/Examples/Sinusoid/
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-12 16:12:57.000000 FoKL-1.2.6/Examples/Sinusoid/DATA_nois.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 16:12:57.000000 FoKL-1.2.6/Examples/Sinusoid/ReadMe.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-12 16:12:57.000000 FoKL-1.2.6/Examples/Sinusoid/X.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-12 16:12:57.000000 FoKL-1.2.6/Examples/Sinusoid/Y.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-12 16:12:57.000000 FoKL-1.2.6/Examples/Sinusoid/python_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-12 16:12:57.000000 FoKL-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-12 16:13:12.168571 FoKL-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-12 16:12:57.000000 FoKL-1.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-12 16:12:57.000000 FoKL-1.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-12 16:13:12.168571 FoKL-1.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:13:12.160570 FoKL-1.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:13:12.164571 FoKL-1.2.6/src/FoKL/
+-rw-r--r--   0 runner    (1001) docker     (123)    34582 2023-06-12 16:12:57.000000 FoKL-1.2.6/src/FoKL/FoKLRoutines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-06-12 16:12:57.000000 FoKL-1.2.6/src/FoKL/GP_Integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:12:57.000000 FoKL-1.2.6/src/FoKL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-12 16:12:57.000000 FoKL-1.2.6/src/FoKL/coverage3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-12 16:12:57.000000 FoKL-1.2.6/src/FoKL/emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-12 16:12:57.000000 FoKL-1.2.6/src/FoKL/gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-12 16:12:57.000000 FoKL-1.2.6/src/FoKL/splineConvert500.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:13:12.168571 FoKL-1.2.6/src/FoKL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-12 16:13:12.000000 FoKL-1.2.6/src/FoKL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-12 16:13:12.000000 FoKL-1.2.6/src/FoKL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:13:12.000000 FoKL-1.2.6/src/FoKL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-12 16:13:12.000000 FoKL-1.2.6/src/FoKL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-12 16:13:12.000000 FoKL-1.2.6/src/FoKL.egg-info/top_level.txt
```

### Comparing `FoKL-1.2.0/Examples/Sinusoid/DATA_nois.csv` & `FoKL-1.2.6/Examples/Sinusoid/DATA_nois.csv`

 * *Files identical despite different names*

### Comparing `FoKL-1.2.0/Examples/Sinusoid/X.csv` & `FoKL-1.2.6/Examples/Sinusoid/X.csv`

 * *Files identical despite different names*

### Comparing `FoKL-1.2.0/Examples/Sinusoid/Y.csv` & `FoKL-1.2.6/Examples/Sinusoid/Y.csv`

 * *Files identical despite different names*

### Comparing `FoKL-1.2.0/Examples/Sinusoid/python_test.py` & `FoKL-1.2.6/Examples/Sinusoid/python_test.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.2.0/LICENSE` & `FoKL-1.2.6/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 derek-slack
+Copyright (c) 2023 David Mebane, Kyle Hayes and Derek Slack
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `FoKL-1.2.0/pyproject.toml` & `FoKL-1.2.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [project]
 name = "FoKL"
 authors = [
     {name = "ESMS Group", email = "derek.slack.001@gmail.com"},
 ]
 description = "Karhunen Loève decomposed Gaussian processes with forward variable selection"
-readme = "ReadMe.md"
+readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "requests",
     'importlib-metadata; python_version<"3.8"',
```

### Comparing `FoKL-1.2.0/setup.cfg` & `FoKL-1.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `FoKL-1.2.0/src/FoKL/FoKLRoutines.py` & `FoKL-1.2.6/src/FoKL/FoKLRoutines.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.2.0/src/FoKL/GP_Integrate.py` & `FoKL-1.2.6/src/FoKL/GP_Integrate.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.2.0/src/FoKL/coverage3.py` & `FoKL-1.2.6/src/FoKL/coverage3.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.2.0/src/FoKL/emulator.py` & `FoKL-1.2.6/src/FoKL/emulator.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.2.0/src/FoKL/gibbs.py` & `FoKL-1.2.6/src/FoKL/gibbs.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.2.0/src/FoKL/splineConvert500.py` & `FoKL-1.2.6/src/FoKL/splineConvert500.py`

 * *Files identical despite different names*

### Comparing `FoKL-1.2.0/src/FoKL.egg-info/SOURCES.txt` & `FoKL-1.2.6/src/FoKL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

