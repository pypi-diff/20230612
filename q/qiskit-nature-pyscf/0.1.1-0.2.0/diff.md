# Comparing `tmp/qiskit-nature-pyscf-0.1.1.tar.gz` & `tmp/qiskit-nature-pyscf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qiskit-nature-pyscf-0.1.1.tar", last modified: Wed Apr 26 21:41:33 2023, max compression
+gzip compressed data, was "qiskit-nature-pyscf-0.2.0.tar", last modified: Mon Jun 12 15:42:08 2023, max compression
```

## Comparing `qiskit-nature-pyscf-0.1.1.tar` & `qiskit-nature-pyscf-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf/qiskit_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:41:33.000000 qiskit-nature-pyscf-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/test/nature_pyscf_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/test/test_qiskit_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-26 21:41:18.000000 qiskit-nature-pyscf-0.1.1/test/test_readme_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:42:08.575063 qiskit-nature-pyscf-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-12 15:41:58.000000 qiskit-nature-pyscf-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-12 15:41:58.000000 qiskit-nature-pyscf-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-12 15:42:08.575063 qiskit-nature-pyscf-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-12 15:41:58.000000 qiskit-nature-pyscf-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-12 15:41:58.000000 qiskit-nature-pyscf-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:42:08.575063 qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 15:41:58.000000 qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-12 15:41:58.000000 qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 15:41:58.000000 qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-06-12 15:41:58.000000 qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf/pyscf_ground_state_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-06-12 15:41:58.000000 qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf/qiskit_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-12 15:41:58.000000 qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:42:08.575063 qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-12 15:42:08.000000 qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-12 15:42:08.000000 qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:42:08.000000 qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:42:08.000000 qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 15:42:08.000000 qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 15:42:08.000000 qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 15:41:58.000000 qiskit-nature-pyscf-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:42:08.575063 qiskit-nature-pyscf-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-12 15:41:58.000000 qiskit-nature-pyscf-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:42:08.575063 qiskit-nature-pyscf-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-12 15:41:58.000000 qiskit-nature-pyscf-0.2.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-12 15:41:58.000000 qiskit-nature-pyscf-0.2.0/test/nature_pyscf_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-12 15:41:58.000000 qiskit-nature-pyscf-0.2.0/test/test_pyscf_ground_state_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-12 15:41:58.000000 qiskit-nature-pyscf-0.2.0/test/test_qiskit_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-12 15:41:58.000000 qiskit-nature-pyscf-0.2.0/test/test_readme_sample.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `qiskit-nature-pyscf-0.1.1/LICENSE.txt` & `qiskit-nature-pyscf-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-nature-pyscf-0.1.1/PKG-INFO` & `qiskit-nature-pyscf-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: qiskit-nature-pyscf
-Version: 0.1.1
+Version: 0.2.0
 Summary: Qiskit Nature PySCF: Third-party integration plugin of Qiskit Nature + PySCF.
 Home-page: https://github.com/qiskit-community/qiskit-nature-pyscf
 Author: Qiskit Nature PySCF Development Team
 Author-email: hello@qiskit.org
 License: Apache-2.0
+Project-URL: Bug Tracker, https://github.com/qiskit-community/qiskit-nature-pyscf/issues
+Project-URL: Documentation, https://qiskit-community.github.io/qiskit-nature-pyscf/
+Project-URL: Source Code, https://github.com/qiskit-community/qiskit-nature-pyscf
 Keywords: qiskit sdk quantum nature chemistry physics pyscf
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Qiskit Nature PySCF
 
@@ -103,15 +107,15 @@
 
 cas.run()
 ```
 
 More detailed documentation can be found at
 [Documentation](https://qiskit-community.github.io/qiskit-nature-pyscf/). For more detailed 
 explanations we recommend to check out the documentation of
-[PySCF](https://pyscf.org/) and [Qiskit Nature](https://qiskit.org/documentation/nature/).
+[PySCF](https://pyscf.org/) and [Qiskit Nature](https://qiskit.org/ecosystem/nature/).
 
 
 ## Citation
 
 If you use this plugin, please cite the following references:
 
 - PySCF, as per [these instructions](https://github.com/pyscf/pyscf#citing-pyscf).
```

### Comparing `qiskit-nature-pyscf-0.1.1/README.md` & `qiskit-nature-pyscf-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 cas.run()
 ```
 
 More detailed documentation can be found at
 [Documentation](https://qiskit-community.github.io/qiskit-nature-pyscf/). For more detailed 
 explanations we recommend to check out the documentation of
-[PySCF](https://pyscf.org/) and [Qiskit Nature](https://qiskit.org/documentation/nature/).
+[PySCF](https://pyscf.org/) and [Qiskit Nature](https://qiskit.org/ecosystem/nature/).
 
 
 ## Citation
 
 If you use this plugin, please cite the following references:
 
 - PySCF, as per [these instructions](https://github.com/pyscf/pyscf#citing-pyscf).
```

### Comparing `qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf/qiskit_solver.py` & `qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf/qiskit_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         algorithm = GroundStateEigensolver(mapper, vqe)
 
         cas.fcisolver = QiskitSolver(algorithm)
 
         cas.run()
 
     For more details please to the documentation of [PySCF](https://pyscf.org/) and
-    [Qiskit Nature](https://qiskit.org/documentation/nature/).
+    [Qiskit Nature](https://qiskit.org/ecosystem/nature/).
 
     An instance of this class has the following attributes:
 
     Attributes:
         solver: a ground-state solver provided by Qiskit Nature. This must be supplied by the user
             prior to running the algorithm.
         density: an ElectronicDensity provided by Qiskit Nature. This is only available after the
```

### Comparing `qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf/version.py` & `qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2022.
+# (C) Copyright IBM 2022, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
-"""Contains the Nature PySCF version."""
+"""Contains the Qiskit Nature PySCF version."""
 
 import os
 import subprocess
 
 ROOT_DIR = os.path.dirname(os.path.abspath(__file__))
 QISKIT_DIR = os.path.dirname(ROOT_DIR)
```

### Comparing `qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/PKG-INFO` & `qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: qiskit-nature-pyscf
-Version: 0.1.1
+Version: 0.2.0
 Summary: Qiskit Nature PySCF: Third-party integration plugin of Qiskit Nature + PySCF.
 Home-page: https://github.com/qiskit-community/qiskit-nature-pyscf
 Author: Qiskit Nature PySCF Development Team
 Author-email: hello@qiskit.org
 License: Apache-2.0
+Project-URL: Bug Tracker, https://github.com/qiskit-community/qiskit-nature-pyscf/issues
+Project-URL: Documentation, https://qiskit-community.github.io/qiskit-nature-pyscf/
+Project-URL: Source Code, https://github.com/qiskit-community/qiskit-nature-pyscf
 Keywords: qiskit sdk quantum nature chemistry physics pyscf
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Qiskit Nature PySCF
 
@@ -103,15 +107,15 @@
 
 cas.run()
 ```
 
 More detailed documentation can be found at
 [Documentation](https://qiskit-community.github.io/qiskit-nature-pyscf/). For more detailed 
 explanations we recommend to check out the documentation of
-[PySCF](https://pyscf.org/) and [Qiskit Nature](https://qiskit.org/documentation/nature/).
+[PySCF](https://pyscf.org/) and [Qiskit Nature](https://qiskit.org/ecosystem/nature/).
 
 
 ## Citation
 
 If you use this plugin, please cite the following references:
 
 - PySCF, as per [these instructions](https://github.com/pyscf/pyscf#citing-pyscf).
```

### Comparing `qiskit-nature-pyscf-0.1.1/qiskit_nature_pyscf.egg-info/SOURCES.txt` & `qiskit-nature-pyscf-0.2.0/qiskit_nature_pyscf.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 qiskit_nature_pyscf/VERSION.txt
 qiskit_nature_pyscf/__init__.py
 qiskit_nature_pyscf/py.typed
+qiskit_nature_pyscf/pyscf_ground_state_solver.py
 qiskit_nature_pyscf/qiskit_solver.py
 qiskit_nature_pyscf/version.py
 qiskit_nature_pyscf.egg-info/PKG-INFO
 qiskit_nature_pyscf.egg-info/SOURCES.txt
 qiskit_nature_pyscf.egg-info/dependency_links.txt
 qiskit_nature_pyscf.egg-info/not-zip-safe
 qiskit_nature_pyscf.egg-info/requires.txt
 qiskit_nature_pyscf.egg-info/top_level.txt
 test/__init__.py
 test/nature_pyscf_test_case.py
+test/test_pyscf_ground_state_solver.py
 test/test_qiskit_solver.py
 test/test_readme_sample.py
```

### Comparing `qiskit-nature-pyscf-0.1.1/setup.py` & `qiskit-nature-pyscf-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2022.
+# (C) Copyright IBM 2022, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
-import setuptools
 import inspect
-import sys
 import os
 import re
+import sys
 
-with open('requirements.txt') as f:
-    REQUIREMENTS = f.read().splitlines()
+import setuptools
 
-if not hasattr(setuptools, 'find_namespace_packages') or not inspect.ismethod(setuptools.find_namespace_packages):
-    print("Your setuptools version:'{}' does not support PEP 420 (find_namespace_packages). "
-          "Upgrade it to version >='40.1.0' and repeat install.".format(setuptools.__version__))
-    sys.exit(1)
+with open("requirements.txt", "r", encoding="utf-8") as f:
+    REQUIREMENTS = f.read().splitlines()
 
 VERSION_PATH = os.path.join(os.path.dirname(__file__), "qiskit_nature_pyscf", "VERSION.txt")
-with open(VERSION_PATH, "r") as version_file:
+with open(VERSION_PATH, "r", encoding="utf-8") as version_file:
     VERSION = version_file.read().strip()
 
 # Read long description from README.
 README_PATH = os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md")
-with open(README_PATH) as readme_file:
+with open(README_PATH, "r", encoding="utf-8") as readme_file:
     README = re.sub(
         "<!--- long-description-skip-begin -->.*<!--- long-description-skip-end -->",
         "",
         readme_file.read(),
         flags=re.S | re.M,
     )
 
 setuptools.setup(
-    name='qiskit-nature-pyscf',
+    name="qiskit-nature-pyscf",
     version=VERSION,
-    description='Qiskit Nature PySCF: Third-party integration plugin of Qiskit Nature + PySCF.',
+    description="Qiskit Nature PySCF: Third-party integration plugin of Qiskit Nature + PySCF.",
     long_description=README,
     long_description_content_type="text/markdown",
-    url='https://github.com/qiskit-community/qiskit-nature-pyscf',
-    author='Qiskit Nature PySCF Development Team',
-    author_email='hello@qiskit.org',
-    license='Apache-2.0',
+    url="https://github.com/qiskit-community/qiskit-nature-pyscf",
+    author="Qiskit Nature PySCF Development Team",
+    author_email="hello@qiskit.org",
+    license="Apache-2.0",
     classifiers=[
         "Environment :: Console",
         "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: MacOS",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Topic :: Scientific/Engineering"
+        "Programming Language :: Python :: 3.11",
+        "Topic :: Scientific/Engineering",
     ],
-    keywords='qiskit sdk quantum nature chemistry physics pyscf',
-    packages=setuptools.find_packages(include=['qiskit_nature_pyscf', 'qiskit_nature_pyscf.*']),
+    keywords="qiskit sdk quantum nature chemistry physics pyscf",
+    packages=setuptools.find_packages(include=["qiskit_nature_pyscf", "qiskit_nature_pyscf.*"]),
     install_requires=REQUIREMENTS,
     include_package_data=True,
     python_requires=">=3.7",
-    zip_safe=False
+    project_urls={
+        "Bug Tracker": "https://github.com/qiskit-community/qiskit-nature-pyscf/issues",
+        "Documentation": "https://qiskit-community.github.io/qiskit-nature-pyscf/",
+        "Source Code": "https://github.com/qiskit-community/qiskit-nature-pyscf",
+    },
+    zip_safe=False,
 )
```

### Comparing `qiskit-nature-pyscf-0.1.1/test/__init__.py` & `qiskit-nature-pyscf-0.2.0/test/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2018, 2022.
+# (C) Copyright IBM 2018, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
-""" Nature PySCF test packages """
+""" Qiskit Nature PySCF test packages """
 
 from .nature_pyscf_test_case import QiskitNaturePySCFTestCase
 
 __all__ = ["QiskitNaturePySCFTestCase"]
```

### Comparing `qiskit-nature-pyscf-0.1.1/test/nature_pyscf_test_case.py` & `qiskit-nature-pyscf-0.2.0/test/nature_pyscf_test_case.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # This code is part of Qiskit.
 #
-# (C) Copyright IBM 2022.
+# (C) Copyright IBM 2022, 2023.
 #
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
-"""Nature PySCF Test Case"""
+"""Qiskit Nature PySCF Test Case"""
 
 from typing import Optional
 from abc import ABC
 import warnings
 import inspect
 import logging
 import os
@@ -30,15 +30,15 @@
 
 
 # disable warning messages
 # warnings.warn = _noop
 
 
 class QiskitNaturePySCFTestCase(unittest.TestCase, ABC):
-    """Nature PySCF Test Case"""
+    """Qiskit Nature PySCF Test Case"""
 
     moduleName = None
     log = None
 
     def setUp(self) -> None:
         warnings.filterwarnings("default", category=DeprecationWarning)
         self._started_at = time.time()
```

### Comparing `qiskit-nature-pyscf-0.1.1/test/test_qiskit_solver.py` & `qiskit-nature-pyscf-0.2.0/test/test_qiskit_solver.py`

 * *Files identical despite different names*

### Comparing `qiskit-nature-pyscf-0.1.1/test/test_readme_sample.py` & `qiskit-nature-pyscf-0.2.0/test/test_readme_sample.py`

 * *Files identical despite different names*

