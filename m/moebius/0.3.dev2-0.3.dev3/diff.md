# Comparing `tmp/moebius-0.3.dev2.tar.gz` & `tmp/moebius-0.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moebius-0.3.dev2.tar", last modified: Mon Jun 12 17:14:45 2023, max compression
+gzip compressed data, was "moebius-0.3.dev3.tar", last modified: Mon Jun 12 17:20:59 2023, max compression
```

## Comparing `moebius-0.3.dev2.tar` & `moebius-0.3.dev3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:14:45.729024 moebius-0.3.dev2/
--rw-rw-rw-   0 root         (0) root         (0)    11337 2023-06-09 11:23:50.000000 moebius-0.3.dev2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7458 2023-06-12 17:14:45.729024 moebius-0.3.dev2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6011 2023-06-12 17:12:17.000000 moebius-0.3.dev2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:14:45.728024 moebius-0.3.dev2/moebius.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7458 2023-06-12 17:14:45.000000 moebius-0.3.dev2/moebius.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-12 17:14:45.000000 moebius-0.3.dev2/moebius.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 17:14:45.000000 moebius-0.3.dev2/moebius.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-12 17:14:45.000000 moebius-0.3.dev2/moebius.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-12 17:14:45.000000 moebius-0.3.dev2/moebius.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1911 2023-06-12 17:14:31.000000 moebius-0.3.dev2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 17:14:45.729024 moebius-0.3.dev2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:20:59.885966 moebius-0.3.dev3/
+-rw-rw-rw-   0 root         (0) root         (0)    11337 2023-06-09 11:23:50.000000 moebius-0.3.dev3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7458 2023-06-12 17:20:59.884966 moebius-0.3.dev3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6011 2023-06-12 17:12:17.000000 moebius-0.3.dev3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:20:59.884966 moebius-0.3.dev3/moebius.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7458 2023-06-12 17:20:59.000000 moebius-0.3.dev3/moebius.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-12 17:20:59.000000 moebius-0.3.dev3/moebius.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 17:20:59.000000 moebius-0.3.dev3/moebius.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-12 17:20:59.000000 moebius-0.3.dev3/moebius.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-12 17:20:59.000000 moebius-0.3.dev3/moebius.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2023-06-12 17:20:46.000000 moebius-0.3.dev3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 17:20:59.885966 moebius-0.3.dev3/setup.cfg
```

### Comparing `moebius-0.3.dev2/LICENSE` & `moebius-0.3.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `moebius-0.3.dev2/PKG-INFO` & `moebius-0.3.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: moebius
-Version: 0.3.dev2
+Version: 0.3.dev3
 Summary: Python package for optimizing peptide sequences using Bayesian optimization (BO)
 Author-email: Jerome Eberhardt <jerome.eberhardt@unibas.ch>, Markus Lill <markus.lill@unibas.ch>, Torsten Schwede <tosten.schwede@unibas.ch>
 License: Apache-2.0
 Project-URL: Homepage, https://git.scicore.unibas.ch/schwede/mobius
-Project-URL: Documentation, https://mobius.readthedocs.io/en/master/
+Project-URL: Documentation, https://mobius.readthedocs.io/en/latest/
 Project-URL: Source, https://git.scicore.unibas.ch/schwede/mobius
 Keywords: drug design,peptide,Bayesian optimization,HELM
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `moebius-0.3.dev2/README.md` & `moebius-0.3.dev3/README.md`

 * *Files identical despite different names*

### Comparing `moebius-0.3.dev2/moebius.egg-info/PKG-INFO` & `moebius-0.3.dev3/moebius.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: moebius
-Version: 0.3.dev2
+Version: 0.3.dev3
 Summary: Python package for optimizing peptide sequences using Bayesian optimization (BO)
 Author-email: Jerome Eberhardt <jerome.eberhardt@unibas.ch>, Markus Lill <markus.lill@unibas.ch>, Torsten Schwede <tosten.schwede@unibas.ch>
 License: Apache-2.0
 Project-URL: Homepage, https://git.scicore.unibas.ch/schwede/mobius
-Project-URL: Documentation, https://mobius.readthedocs.io/en/master/
+Project-URL: Documentation, https://mobius.readthedocs.io/en/latest/
 Project-URL: Source, https://git.scicore.unibas.ch/schwede/mobius
 Keywords: drug design,peptide,Bayesian optimization,HELM
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `moebius-0.3.dev2/pyproject.toml` & `moebius-0.3.dev3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "moebius"
-version = "0.3.dev2"
+version = "0.3.dev3"
 description = "Python package for optimizing peptide sequences using Bayesian optimization (BO)"
 authors = [
     { name = "Jerome Eberhardt", email = "jerome.eberhardt@unibas.ch" },
     { name = "Markus Lill", email = "markus.lill@unibas.ch" },
     { name = "Torsten Schwede", email = "tosten.schwede@unibas.ch" },
 ]
 readme = "README.md"
@@ -49,15 +49,15 @@
     "torch",
     "ray",
     "mhfp"
 ]
 
 [project.urls] 
 "Homepage" = "https://git.scicore.unibas.ch/schwede/mobius"
-"Documentation" = "https://mobius.readthedocs.io/en/master/"
+"Documentation" = "https://mobius.readthedocs.io/en/latest/"
 "Source" = "https://git.scicore.unibas.ch/schwede/mobius"
 
 [tool.setuptools]
 py-modules = ['mobius']
 
 [build-system]
 requires = ["setuptools >= 40.6.0", "wheel"]
```

