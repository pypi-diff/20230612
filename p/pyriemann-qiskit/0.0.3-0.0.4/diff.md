# Comparing `tmp/pyriemann-qiskit-0.0.3.tar.gz` & `tmp/pyriemann-qiskit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriemann-qiskit-0.0.3.tar", last modified: Mon Jan 23 21:53:36 2023, max compression
+gzip compressed data, was "pyriemann-qiskit-0.0.4.tar", last modified: Mon Jun 12 08:34:15 2023, max compression
```

## Comparing `pyriemann-qiskit-0.0.3.tar` & `pyriemann-qiskit-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 21:53:36.679431 pyriemann-qiskit-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-01-23 21:53:27.000000 pyriemann-qiskit-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-23 21:53:27.000000 pyriemann-qiskit-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-01-23 21:53:36.679431 pyriemann-qiskit-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-01-23 21:53:27.000000 pyriemann-qiskit-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 21:53:36.675431 pyriemann-qiskit-0.0.3/pyriemann_qiskit/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-23 21:53:27.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-23 21:53:27.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    24813 2023-01-23 21:53:27.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit/classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 21:53:36.675431 pyriemann-qiskit-0.0.3/pyriemann_qiskit/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-01-23 21:53:27.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-01-23 21:53:27.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 21:53:36.679431 pyriemann-qiskit-0.0.3/pyriemann_qiskit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-01-23 21:53:27.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-01-23 21:53:27.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit/utils/docplex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-01-23 21:53:27.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit/utils/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-23 21:53:27.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit/utils/firebase_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-01-23 21:53:27.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit/utils/firebase_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-01-23 21:53:27.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit/utils/hyper_params_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-01-23 21:53:27.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-01-23 21:53:27.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit/utils/mean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 21:53:36.675431 pyriemann-qiskit-0.0.3/pyriemann_qiskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-01-23 21:53:36.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-01-23 21:53:36.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 21:53:36.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 21:53:36.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-01-23 21:53:36.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-23 21:53:36.000000 pyriemann-qiskit-0.0.3/pyriemann_qiskit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-23 21:53:36.679431 pyriemann-qiskit-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-01-23 21:53:27.000000 pyriemann-qiskit-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:34:15.181554 pyriemann-qiskit-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-06-12 08:34:15.181554 pyriemann-qiskit-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:34:15.177554 pyriemann-qiskit-0.0.4/pyriemann_qiskit/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28005 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit/classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:34:15.181554 pyriemann-qiskit-0.0.4/pyriemann_qiskit/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:34:15.181554 pyriemann-qiskit-0.0.4/pyriemann_qiskit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit/utils/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14044 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit/utils/docplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit/utils/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit/utils/firebase_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit/utils/firebase_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit/utils/hyper_params_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit/utils/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit/utils/quantum_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:34:15.181554 pyriemann-qiskit-0.0.4/pyriemann_qiskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-06-12 08:34:15.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-12 08:34:15.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:34:15.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:34:15.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-12 08:34:15.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-12 08:34:15.000000 pyriemann-qiskit-0.0.4/pyriemann_qiskit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-12 08:34:15.181554 pyriemann-qiskit-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:34:15.181554 pyriemann-qiskit-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/tests/test_docplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/tests/test_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/tests/test_utils_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/tests/test_utils_firebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/tests/test_utils_hyper_params_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-12 08:34:03.000000 pyriemann-qiskit-0.0.4/tests/test_utils_mean.py
```

### Comparing `pyriemann-qiskit-0.0.3/LICENSE` & `pyriemann-qiskit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriemann-qiskit-0.0.3/PKG-INFO` & `pyriemann-qiskit-0.0.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,187 +1,276 @@
 Metadata-Version: 2.1
 Name: pyriemann-qiskit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Qiskit wrapper for pyRiemann
 Home-page: https://pyriemann-qiskit.readthedocs.io
 Author: Gregoire Cattan
 Author-email: gcattan@hotmail.com
 License: BSD (3-clause)
 Project-URL: Documentation, https://pyriemann.readthedocs.io
 Project-URL: Source, https://github.com/pyRiemann/pyRiemann-qiskit
 Project-URL: Tracker, https://github.com/pyRiemann/pyRiemann-qiskit/issues/
 Platform: any
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: tests
+Provides-Extra: optim
 License-File: LICENSE
 
 # pyRiemann-qiskit
 
-Litterature on quantum computing suggests it may offer an advantage as compared
-with classical computing in terms of computational time and outcomes, such as
-for pattern recognition or when using limited training sets [1, 2].
-
-A ubiquitous library on quantum computing is Qiskit [3].
-Qiskit is an IBM library distributed under Apache 2.0 which provides both
-quantum algorithms and backends. A backend can be either your local machine
-or a remote machine, which one can emulates or be a quantum machine.
-Qiskit abstraction over the type of machine you want to use, make designing
-quantum algorithm seamless.
-
-Qiskit implements a quantum version of support vector
--like classifiers, known as quantum-enhanced support vector classifier (QSVC)
-and varitional quantum classifier (VQC) [4]. These classifiers likely offer
-an advantage over classical SVM in situations where the classification task
-is complex. Task complexity is raised by the encoding of the data into a
-quantum state, the number of available data and the quality of the data. An initial 
-study is available in [5], and it can be downloaded from [here](doc/Presentations/QuantumERPClassification.pdf).
-Although there is no study on this topic at the time of writting,
-this could be an interesting research direction to investigate BCI illiteracy.
-
-pyRiemann-qiskit implements a wrapper around QSVC and VQC, to use quantum
-classification with Riemannian geometry. A use case would be to use vectorized
-covariance matrices in the TangentSpace as an input for these classifiers,
-enabling a possible sandbox for researchers and engineers in the field.
-
-The remaining details some of the quantum drawbacks and will guide you through installation.
-Full documentation, including API description, is available at <https://pyriemann-qiskit.readthedocs.io/>.
-The repository also includes a [wiki](https://github.com/pyRiemann/pyRiemann-qiskit/wiki) where you can find additional information.
+Litterature on quantum computing suggests it may offer an advantage as compared with
+classical computing in terms of computational time and outcomes, such as for pattern
+recognition or when using limited training sets [1, 2].
+
+A ubiquitous library on quantum computing is Qiskit [3]. Qiskit is an IBM library
+distributed under Apache 2.0 which provides both quantum algorithms and backends. A
+backend can be either your local machine or a remote machine, which one can emulates or be
+a quantum machine. Qiskit abstraction over the type of machine you want to use, make
+designing quantum algorithm seamless.
+
+Qiskit implements a quantum version of support vector -like classifiers, known as
+quantum-enhanced support vector classifier (QSVC) and varitional quantum classifier (VQC)
+[4]. These classifiers likely offer an advantage over classical SVM in situations where
+the classification task is complex. Task complexity is raised by the encoding of the data
+into a quantum state, the number of available data and the quality of the data. An initial
+study is available in [5], and it can be downloaded from
+[here](doc/Presentations/QuantumERPClassification.pdf). Although there is no study on this
+topic at the time of writting, this could be an interesting research direction to
+investigate BCI illiteracy.
+
+pyRiemann-qiskit implements a wrapper around QSVC and VQC, to use quantum classification
+with Riemannian geometry. A use case would be to use vectorized covariance matrices in the
+tangent space as an input for these classifiers, enabling a possible sandbox for
+researchers and engineers in the field.
+
+The remaining details some of the quantum drawbacks and will guide you through
+installation. Full documentation, including API description, is available at
+<https://pyriemann-qiskit.readthedocs.io/>. The repository also includes a
+[wiki](https://github.com/pyRiemann/pyRiemann-qiskit/wiki) where you can find additional
+information.
 
 ## Quantum drawbacks
 
 - Limitation of the feature dimension
 
-    The number of qubits (and therefore the feature dimension) is limited to:
-    - 24 on a local quantum simulator, and up to:
-    - 5000 on a remote quantum simulator;
-    - 5 on free real quantum computers, and up to:
-    - 65 on exploratory quantum computers (not available for public use).
+  The number of qubits (and therefore the feature dimension) is limited to:
+
+  - 24 on a local quantum simulator, and up to:
+  - 5000 on a remote quantum simulator;
+  - 5 on free real quantum computers, and up to:
+  - 65 on exploratory quantum computers (not available for public use).
 
 - Time complexity
 
-    A higher number of trials or dimension increases time to completion of the quantum algorithm, especially when running on a local machine. This is why the number of trials is limited in the examples we provided. However, you should avoid such practices in your own analysis. 
-    
-    Although these aspects are less important in a remote backend, it may happen that the quantum algorithm is queued depending on the number of concurrent users.
+  A higher number of trials or dimension increases time to completion of the quantum
+  algorithm, especially when running on a local machine. This is why the number of trials
+  is limited in the examples we provided. However, you should avoid such practices in your
+  own analysis.
+
+  Although these aspects are less important in a remote backend, it may happen that the
+  quantum algorithm is queued depending on the number of concurrent users.
+
+  For all these aspects, the use of pyRiemann-qiskit should be limited to offline analysis
+  only.
 
-    For all these aspects, the use of pyRiemann-qiskit should be limited to offline analysis only.
-    
 ## References
 
-[1] A. Blance and M. Spannowsky,
-    ‘Quantum machine learning for particle physics using a variational quantum classifier’,
-    J. High Energ. Phys., vol. 2021, no. 2, p. 212, Feb. 2021,
-    doi: 10.1007/JHEP02(2021)212.
-
-[2] P. Rebentrost, M. Mohseni, and S. Lloyd,
-   ‘Quantum Support Vector Machine for Big Data Classification’,
-    Phys. Rev. Lett., vol. 113, no. 13, p. 130503, Sep. 2014,
-    doi: 10.1103/PhysRevLett.113.130503.
+[1] A. Blance and M. Spannowsky, ‘Quantum machine learning for particle physics using a
+variational quantum classifier’, J. High Energ. Phys., vol. 2021, no. 2, p. 212, Feb.
+2021, doi: 10.1007/JHEP02(2021)212.
+
+[2] P. Rebentrost, M. Mohseni, and S. Lloyd, ‘Quantum Support Vector Machine for Big Data
+Classification’, Phys. Rev. Lett., vol. 113, no. 13, p. 130503, Sep. 2014, doi:
+10.1103/PhysRevLett.113.130503.
 
 [3] H. Abraham et al., Qiskit: An Open-source Framework for Quantum Computing.
-    Zenodo, 2019. doi: 10.5281/zenodo.2562110.
+Zenodo, 2019. doi: 10.5281/zenodo.2562110.
 
-[4] V. Havlíček et al.,
-    ‘Supervised learning with quantum-enhanced feature spaces’,
-    Nature, vol. 567, no. 7747, pp. 209–212, Mar. 2019,
-    doi: 10.1038/s41586-019-0980-2.
-	
-[5] G. Cattan, A. Andreev,
-    First steps to the classification of ERPs using quantum computation,
-	NTB Berlin 2022 - International Forum on Neural Engineering & Brain Technologies, May 2022, Berlin, Germany,
-	hal: https://hal.archives-ouvertes.fr/hal-03672246/
+[4] V. Havlíček et al., ‘Supervised learning with quantum-enhanced feature spaces’,
+Nature, vol. 567, no. 7747, pp. 209–212, Mar. 2019, doi: 10.1038/s41586-019-0980-2.
 
+[5] G. Cattan, A. Andreev, First steps to the classification of ERPs using quantum
+computation, NTB Berlin 2022 - International Forum on Neural Engineering & Brain
+Technologies, May 2022, Berlin, Germany, hal:
+https://hal.archives-ouvertes.fr/hal-03672246/
+
+### How to cite?
+
+Anton Andreev, Grégoire Cattan, Sylvain Chevallier, and Quentin Barthélemy.
+‘PyRiemann-Qiskit: A Sandbox for Quantum Classification Experiments with Riemannian
+Geometry’. Research Ideas and Outcomes 9 (20 March 2023).
+https://doi.org/10.3897/rio.9.e101006.
 
 ## Installation
 
-_We recommend the use of [Anaconda](https://www.anaconda.com/) to manage python environements._ 
+_We recommend the use of [Anaconda](https://www.anaconda.com/) to manage python
+environements._
+
+`pyRiemann-qiskit` currently supports Windows, Mac and Linux OS with Python 3.7, 3.8 and
+3.9.
 
-`pyRiemann-qiskit` currently supports Windows, Mac and Linux OS with Python 3.7, 3.8 and 3.9.
+You can install `pyRiemann-qiskit` release from PyPI:
 
-As there is no stable version, you should clone this repository
-and install the package on your local machine using the `setup.py` script
+```
+pip install pyriemann-qiskit
+```
+
+The development version can be installed by cloning this repository and installing the
+package on your local machine using the `setup.py` script:
 
 ```
 python setup.py develop
 ```
 
 To check the installation, open a python shell and type:
 
 ```
 import pyriemann_qiskit
 ```
 
-To run a specific example on your local machine, you should install first dependencies for the documentation:
+To enable Qiskit GPU optimization when using quantum simulation, run:
+
+```
+pip install .[optim]
+```
+
+Note, Qiskit only provide binaries for Linux. For other platforms, or if you want to
+enable specific NVIDIA optimization for quantum, you need to build the binary
+[yourself](https://github.com/Qiskit/qiskit-aer/blob/main/CONTRIBUTING.md#building-with-gpu-support).
+
+To run a specific example on your local machine, you should install first dependencies for
+the documentation:
 
 ```
 pip install .[docs]
 ```
 
 Then you can run the python example of your choice like:
 
 ```
 python examples\ERP\classify_P300_bi.py
 ```
 
 ### Installation with docker
 
-We also offer the possibility to set up the dev environment within docker.
-To this end, we recommand to use `vscode` with the `Remote Containers` extension
-from Microsoft. 
+We also offer the possibility to set up the dev environment within docker. To this end, we
+recommand to use `vscode` with the `Remote Containers` extension from Microsoft.
 
-Once the installation is successful, just open the project in `vscode` and enter `F1`.
-In the search bar that opens, type `Rebuild and Reopen Container`.
+Once the installation is successful, just open the project in `vscode` and enter `F1`. In
+the search bar that opens, type `Rebuild and Reopen Container`.
 
-Wait for the container to build, and open a python shell within the container.
-Then ensure everything went smoothly by typing:
+Wait for the container to build, and open a python shell within the container. Then ensure
+everything went smoothly by typing:
 
 ```
 import pyriemann_qiskit
 ```
 
-## Contributor Guidelines
-
-Everyone is welcomed to contribute to this repository. There are two types of contributions:
-
-- [Raise an issue](https://github.com/pyRiemann/pyRiemann-qiskit/issues/new) on the repository.
-Issues can be either a bug report or an enhancement proposal. Note that it is necessary to register on
-GitHub before. There is no special template which is expected but, if you raise a defect please  provide as much details as possible.
-
-- [Raise a pull request](https://github.com/pyRiemann/pyRiemann-qiskit/compare). Fork the repository and work on your own branch. Then raise a pull request with your branch against master. As much as possible, we ask you to:
-    - avoid merging master into your branch. Always prefer git rebase.
-    - always provide full documentation of public method.
+Alternatively you can from the console (Windows or Linux) build the docker image from our
+Dockerfile. Go to the root folder of pyRiemann-qiskit and type:
 
-Code contribution (pull request) can be either on core functionalities, documentation or automation.
+```
+docker build -t pyrq .
+```
 
-- The core functionalies are based on `Python`, [pyRiemann](https://github.com/pyRiemann/pyRiemann), [Qiskit ML](https://github.com/Qiskit/qiskit-machine-learning) and follow the best practice from [scikit-learn](https://scikit-learn.org/stable/index.html). We use `flake8` for code formatting. `flake8` is installed with the testing dependencies (see below) or can be installed directly from `pip`:
+Next use `docker run --detach pyrq` to enter the pyRiemann-qiskit image.
 
-    ```
-    pip install flake8
-    ```
+If you wish, you can also download docker images directly from github docker registry:
+https://github.com/pyRiemann/pyRiemann-qiskit/pkgs/container/pyriemann-qiskit
 
-    To execute `flake8`, just type `flake8` from the root repository, and correct all errors related to your changes.
+They are pushed to the docker registry on each release.
 
-- The documentation is based on [Sphinx](https://www.sphinx-doc.org/en/master/).
-- Automation is based on `GitHub Action` and `pytest`. It consists in two automated workflows for running the example and the tests. To run the tests on your local machine, you should first install the dependencies for testing:
+## Contributor Guidelines
 
-    ```
-    pip install .[tests]
-    ```
+Everyone is welcomed to contribute to this repository. There are two types of
+contributions:
 
-    and then type `pytest` from the root repository. You can also specify a file like:
+- [Raise an issue](https://github.com/pyRiemann/pyRiemann-qiskit/issues/new) on the
+  repository. Issues can be either a bug report or an enhancement proposal. Note that it
+  is necessary to register on GitHub before. There is no special template which is
+  expected but, if you raise a defect please provide as much details as possible.
+
+- [Raise a pull request](https://github.com/pyRiemann/pyRiemann-qiskit/compare). Fork the
+  repository and work on your own branch. Then raise a pull request with your branch
+  against master. As much as possible, we ask you to:
+  - avoid merging master into your branch. Always prefer git rebase.
+  - always provide full documentation of public method.
+
+Code contribution (pull request) can be either on core functionalities, documentation or
+automation.
+
+- The core functionalies are based on `Python`,
+  [pyRiemann](https://github.com/pyRiemann/pyRiemann),
+  [Qiskit ML](https://github.com/Qiskit/qiskit-machine-learning) and follow the best
+  practice from [scikit-learn](https://scikit-learn.org/stable/index.html). We use
+  `flake8` for code formatting. `flake8` is installed with the testing dependencies (see
+  below) or can be installed directly from `pip`:
+
+  ```
+  pip install flake8
+  ```
 
-    ```
-    pytest tests/test_classification.py 
-    ```
+  To execute `flake8`, just type `flake8` from the root repository, and correct all errors
+  related to your changes.
 
-    Workflows are automatically triggered when you push a commit. However, the worflow for example execution is only triggered when you modify one of the examples or the documentation as the execution take a lot of time. You can enable [Github Actions](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/enabling-features-for-your-repository/managing-github-actions-settings-for-a-repository) in your fork to see the result of the CI pipeline. Results are also indicated at the end of your pull request when raised. However note, that workflows in the pull request need approval from the maintainers before being executed.
+- The documentation is based on [Sphinx](https://www.sphinx-doc.org/en/master/).
+- Automation is based on `GitHub Action` and `pytest`. It consists in two automated
+  workflows for running the example and the tests. To run the tests on your local machine,
+  you should first install the dependencies for testing:
+
+  ```
+  pip install .[tests]
+  ```
+
+  and then type `pytest` from the root repository. You can also specify a file like:
+
+  ```
+  pytest tests/test_classification.py
+  ```
+
+  Workflows are automatically triggered when you push a commit. However, the worflow for
+  example execution is only triggered when you modify one of the examples or the
+  documentation as the execution take a lot of time. You can enable
+  [Github Actions](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/enabling-features-for-your-repository/managing-github-actions-settings-for-a-repository)
+  in your fork to see the result of the CI pipeline. Results are also indicated at the end
+  of your pull request when raised. However note, that workflows in the pull request need
+  approval from the maintainers before being executed.
 
 # Troubleshooting
 
 ## Version of pyRiemann not updated
-There is a known issue when you install `pyRiemann-qiskit` in an environement where there is already `pyRiemann` installed. In such case, the `pyRiemann` version is not updated. Therefore before installing or updating `pyRiemann-qiskit`, we recommend to install `pyRiemann` as it follows:
+
+There is a known issue when you install `pyRiemann-qiskit` in an environement where there
+is already `pyRiemann` installed. In such case, the `pyRiemann` version is not updated.
+Therefore before installing or updating `pyRiemann-qiskit`, we recommend to install
+`pyRiemann` as it follows:
 
 ```
 pip uninstall pyriemann
 pip install pyriemann@git+https://github.com/pyRiemann/pyRiemann#egg=pyriemann
 ```
+
+## Firebase admin not loading
+
+In some environment, the firebase admin module is not loaded. There is two reasons:
+
+1. The protobuf package is missing an `__init__.py` file. You can fix this issue by adding
+   it manually as it is done in the DockerFile:
+
+```
+touch /usr/local/lib/python3.8/site-packages/protobuf-4.22.1-py3.8-linux-x86_64.egg/google/__init__.py
+```
+
+2. The Firestore service contains unused dependency to `google.cloud.location`. You can
+   fix this issue by removing the dependencies manually, as it is done in the DockerFile
+   too:
+
+```
+sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/client.py'
+sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/transports/base.py'
+sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/transports/grpc.py'
+sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/transports/grpc_asyncio.py'
+sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/transports/rest.py'
+sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/async_client.py'
+```
```

### Comparing `pyriemann-qiskit-0.0.3/README.md` & `pyriemann-qiskit-0.0.4/pyriemann_qiskit.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,169 +1,276 @@
+Metadata-Version: 2.1
+Name: pyriemann-qiskit
+Version: 0.0.4
+Summary: Qiskit wrapper for pyRiemann
+Home-page: https://pyriemann-qiskit.readthedocs.io
+Author: Gregoire Cattan
+Author-email: gcattan@hotmail.com
+License: BSD (3-clause)
+Project-URL: Documentation, https://pyriemann.readthedocs.io
+Project-URL: Source, https://github.com/pyRiemann/pyRiemann-qiskit
+Project-URL: Tracker, https://github.com/pyRiemann/pyRiemann-qiskit/issues/
+Platform: any
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: tests
+Provides-Extra: optim
+License-File: LICENSE
+
 # pyRiemann-qiskit
 
-Litterature on quantum computing suggests it may offer an advantage as compared
-with classical computing in terms of computational time and outcomes, such as
-for pattern recognition or when using limited training sets [1, 2].
-
-A ubiquitous library on quantum computing is Qiskit [3].
-Qiskit is an IBM library distributed under Apache 2.0 which provides both
-quantum algorithms and backends. A backend can be either your local machine
-or a remote machine, which one can emulates or be a quantum machine.
-Qiskit abstraction over the type of machine you want to use, make designing
-quantum algorithm seamless.
-
-Qiskit implements a quantum version of support vector
--like classifiers, known as quantum-enhanced support vector classifier (QSVC)
-and varitional quantum classifier (VQC) [4]. These classifiers likely offer
-an advantage over classical SVM in situations where the classification task
-is complex. Task complexity is raised by the encoding of the data into a
-quantum state, the number of available data and the quality of the data. An initial 
-study is available in [5], and it can be downloaded from [here](doc/Presentations/QuantumERPClassification.pdf).
-Although there is no study on this topic at the time of writting,
-this could be an interesting research direction to investigate BCI illiteracy.
-
-pyRiemann-qiskit implements a wrapper around QSVC and VQC, to use quantum
-classification with Riemannian geometry. A use case would be to use vectorized
-covariance matrices in the TangentSpace as an input for these classifiers,
-enabling a possible sandbox for researchers and engineers in the field.
-
-The remaining details some of the quantum drawbacks and will guide you through installation.
-Full documentation, including API description, is available at <https://pyriemann-qiskit.readthedocs.io/>.
-The repository also includes a [wiki](https://github.com/pyRiemann/pyRiemann-qiskit/wiki) where you can find additional information.
+Litterature on quantum computing suggests it may offer an advantage as compared with
+classical computing in terms of computational time and outcomes, such as for pattern
+recognition or when using limited training sets [1, 2].
+
+A ubiquitous library on quantum computing is Qiskit [3]. Qiskit is an IBM library
+distributed under Apache 2.0 which provides both quantum algorithms and backends. A
+backend can be either your local machine or a remote machine, which one can emulates or be
+a quantum machine. Qiskit abstraction over the type of machine you want to use, make
+designing quantum algorithm seamless.
+
+Qiskit implements a quantum version of support vector -like classifiers, known as
+quantum-enhanced support vector classifier (QSVC) and varitional quantum classifier (VQC)
+[4]. These classifiers likely offer an advantage over classical SVM in situations where
+the classification task is complex. Task complexity is raised by the encoding of the data
+into a quantum state, the number of available data and the quality of the data. An initial
+study is available in [5], and it can be downloaded from
+[here](doc/Presentations/QuantumERPClassification.pdf). Although there is no study on this
+topic at the time of writting, this could be an interesting research direction to
+investigate BCI illiteracy.
+
+pyRiemann-qiskit implements a wrapper around QSVC and VQC, to use quantum classification
+with Riemannian geometry. A use case would be to use vectorized covariance matrices in the
+tangent space as an input for these classifiers, enabling a possible sandbox for
+researchers and engineers in the field.
+
+The remaining details some of the quantum drawbacks and will guide you through
+installation. Full documentation, including API description, is available at
+<https://pyriemann-qiskit.readthedocs.io/>. The repository also includes a
+[wiki](https://github.com/pyRiemann/pyRiemann-qiskit/wiki) where you can find additional
+information.
 
 ## Quantum drawbacks
 
 - Limitation of the feature dimension
 
-    The number of qubits (and therefore the feature dimension) is limited to:
-    - 24 on a local quantum simulator, and up to:
-    - 5000 on a remote quantum simulator;
-    - 5 on free real quantum computers, and up to:
-    - 65 on exploratory quantum computers (not available for public use).
+  The number of qubits (and therefore the feature dimension) is limited to:
+
+  - 24 on a local quantum simulator, and up to:
+  - 5000 on a remote quantum simulator;
+  - 5 on free real quantum computers, and up to:
+  - 65 on exploratory quantum computers (not available for public use).
 
 - Time complexity
 
-    A higher number of trials or dimension increases time to completion of the quantum algorithm, especially when running on a local machine. This is why the number of trials is limited in the examples we provided. However, you should avoid such practices in your own analysis. 
-    
-    Although these aspects are less important in a remote backend, it may happen that the quantum algorithm is queued depending on the number of concurrent users.
+  A higher number of trials or dimension increases time to completion of the quantum
+  algorithm, especially when running on a local machine. This is why the number of trials
+  is limited in the examples we provided. However, you should avoid such practices in your
+  own analysis.
+
+  Although these aspects are less important in a remote backend, it may happen that the
+  quantum algorithm is queued depending on the number of concurrent users.
+
+  For all these aspects, the use of pyRiemann-qiskit should be limited to offline analysis
+  only.
 
-    For all these aspects, the use of pyRiemann-qiskit should be limited to offline analysis only.
-    
 ## References
 
-[1] A. Blance and M. Spannowsky,
-    ‘Quantum machine learning for particle physics using a variational quantum classifier’,
-    J. High Energ. Phys., vol. 2021, no. 2, p. 212, Feb. 2021,
-    doi: 10.1007/JHEP02(2021)212.
-
-[2] P. Rebentrost, M. Mohseni, and S. Lloyd,
-   ‘Quantum Support Vector Machine for Big Data Classification’,
-    Phys. Rev. Lett., vol. 113, no. 13, p. 130503, Sep. 2014,
-    doi: 10.1103/PhysRevLett.113.130503.
+[1] A. Blance and M. Spannowsky, ‘Quantum machine learning for particle physics using a
+variational quantum classifier’, J. High Energ. Phys., vol. 2021, no. 2, p. 212, Feb.
+2021, doi: 10.1007/JHEP02(2021)212.
+
+[2] P. Rebentrost, M. Mohseni, and S. Lloyd, ‘Quantum Support Vector Machine for Big Data
+Classification’, Phys. Rev. Lett., vol. 113, no. 13, p. 130503, Sep. 2014, doi:
+10.1103/PhysRevLett.113.130503.
 
 [3] H. Abraham et al., Qiskit: An Open-source Framework for Quantum Computing.
-    Zenodo, 2019. doi: 10.5281/zenodo.2562110.
+Zenodo, 2019. doi: 10.5281/zenodo.2562110.
 
-[4] V. Havlíček et al.,
-    ‘Supervised learning with quantum-enhanced feature spaces’,
-    Nature, vol. 567, no. 7747, pp. 209–212, Mar. 2019,
-    doi: 10.1038/s41586-019-0980-2.
-	
-[5] G. Cattan, A. Andreev,
-    First steps to the classification of ERPs using quantum computation,
-	NTB Berlin 2022 - International Forum on Neural Engineering & Brain Technologies, May 2022, Berlin, Germany,
-	hal: https://hal.archives-ouvertes.fr/hal-03672246/
+[4] V. Havlíček et al., ‘Supervised learning with quantum-enhanced feature spaces’,
+Nature, vol. 567, no. 7747, pp. 209–212, Mar. 2019, doi: 10.1038/s41586-019-0980-2.
 
+[5] G. Cattan, A. Andreev, First steps to the classification of ERPs using quantum
+computation, NTB Berlin 2022 - International Forum on Neural Engineering & Brain
+Technologies, May 2022, Berlin, Germany, hal:
+https://hal.archives-ouvertes.fr/hal-03672246/
+
+### How to cite?
+
+Anton Andreev, Grégoire Cattan, Sylvain Chevallier, and Quentin Barthélemy.
+‘PyRiemann-Qiskit: A Sandbox for Quantum Classification Experiments with Riemannian
+Geometry’. Research Ideas and Outcomes 9 (20 March 2023).
+https://doi.org/10.3897/rio.9.e101006.
 
 ## Installation
 
-_We recommend the use of [Anaconda](https://www.anaconda.com/) to manage python environements._ 
+_We recommend the use of [Anaconda](https://www.anaconda.com/) to manage python
+environements._
 
-`pyRiemann-qiskit` currently supports Windows, Mac and Linux OS with Python 3.7, 3.8 and 3.9.
+`pyRiemann-qiskit` currently supports Windows, Mac and Linux OS with Python 3.7, 3.8 and
+3.9.
 
-As there is no stable version, you should clone this repository
-and install the package on your local machine using the `setup.py` script
+You can install `pyRiemann-qiskit` release from PyPI:
+
+```
+pip install pyriemann-qiskit
+```
+
+The development version can be installed by cloning this repository and installing the
+package on your local machine using the `setup.py` script:
 
 ```
 python setup.py develop
 ```
 
 To check the installation, open a python shell and type:
 
 ```
 import pyriemann_qiskit
 ```
 
-To run a specific example on your local machine, you should install first dependencies for the documentation:
+To enable Qiskit GPU optimization when using quantum simulation, run:
+
+```
+pip install .[optim]
+```
+
+Note, Qiskit only provide binaries for Linux. For other platforms, or if you want to
+enable specific NVIDIA optimization for quantum, you need to build the binary
+[yourself](https://github.com/Qiskit/qiskit-aer/blob/main/CONTRIBUTING.md#building-with-gpu-support).
+
+To run a specific example on your local machine, you should install first dependencies for
+the documentation:
 
 ```
 pip install .[docs]
 ```
 
 Then you can run the python example of your choice like:
 
 ```
 python examples\ERP\classify_P300_bi.py
 ```
 
 ### Installation with docker
 
-We also offer the possibility to set up the dev environment within docker.
-To this end, we recommand to use `vscode` with the `Remote Containers` extension
-from Microsoft. 
+We also offer the possibility to set up the dev environment within docker. To this end, we
+recommand to use `vscode` with the `Remote Containers` extension from Microsoft.
 
-Once the installation is successful, just open the project in `vscode` and enter `F1`.
-In the search bar that opens, type `Rebuild and Reopen Container`.
+Once the installation is successful, just open the project in `vscode` and enter `F1`. In
+the search bar that opens, type `Rebuild and Reopen Container`.
 
-Wait for the container to build, and open a python shell within the container.
-Then ensure everything went smoothly by typing:
+Wait for the container to build, and open a python shell within the container. Then ensure
+everything went smoothly by typing:
 
 ```
 import pyriemann_qiskit
 ```
 
-## Contributor Guidelines
-
-Everyone is welcomed to contribute to this repository. There are two types of contributions:
-
-- [Raise an issue](https://github.com/pyRiemann/pyRiemann-qiskit/issues/new) on the repository.
-Issues can be either a bug report or an enhancement proposal. Note that it is necessary to register on
-GitHub before. There is no special template which is expected but, if you raise a defect please  provide as much details as possible.
-
-- [Raise a pull request](https://github.com/pyRiemann/pyRiemann-qiskit/compare). Fork the repository and work on your own branch. Then raise a pull request with your branch against master. As much as possible, we ask you to:
-    - avoid merging master into your branch. Always prefer git rebase.
-    - always provide full documentation of public method.
+Alternatively you can from the console (Windows or Linux) build the docker image from our
+Dockerfile. Go to the root folder of pyRiemann-qiskit and type:
 
-Code contribution (pull request) can be either on core functionalities, documentation or automation.
+```
+docker build -t pyrq .
+```
 
-- The core functionalies are based on `Python`, [pyRiemann](https://github.com/pyRiemann/pyRiemann), [Qiskit ML](https://github.com/Qiskit/qiskit-machine-learning) and follow the best practice from [scikit-learn](https://scikit-learn.org/stable/index.html). We use `flake8` for code formatting. `flake8` is installed with the testing dependencies (see below) or can be installed directly from `pip`:
+Next use `docker run --detach pyrq` to enter the pyRiemann-qiskit image.
 
-    ```
-    pip install flake8
-    ```
+If you wish, you can also download docker images directly from github docker registry:
+https://github.com/pyRiemann/pyRiemann-qiskit/pkgs/container/pyriemann-qiskit
 
-    To execute `flake8`, just type `flake8` from the root repository, and correct all errors related to your changes.
+They are pushed to the docker registry on each release.
 
-- The documentation is based on [Sphinx](https://www.sphinx-doc.org/en/master/).
-- Automation is based on `GitHub Action` and `pytest`. It consists in two automated workflows for running the example and the tests. To run the tests on your local machine, you should first install the dependencies for testing:
+## Contributor Guidelines
 
-    ```
-    pip install .[tests]
-    ```
+Everyone is welcomed to contribute to this repository. There are two types of
+contributions:
 
-    and then type `pytest` from the root repository. You can also specify a file like:
+- [Raise an issue](https://github.com/pyRiemann/pyRiemann-qiskit/issues/new) on the
+  repository. Issues can be either a bug report or an enhancement proposal. Note that it
+  is necessary to register on GitHub before. There is no special template which is
+  expected but, if you raise a defect please provide as much details as possible.
+
+- [Raise a pull request](https://github.com/pyRiemann/pyRiemann-qiskit/compare). Fork the
+  repository and work on your own branch. Then raise a pull request with your branch
+  against master. As much as possible, we ask you to:
+  - avoid merging master into your branch. Always prefer git rebase.
+  - always provide full documentation of public method.
+
+Code contribution (pull request) can be either on core functionalities, documentation or
+automation.
+
+- The core functionalies are based on `Python`,
+  [pyRiemann](https://github.com/pyRiemann/pyRiemann),
+  [Qiskit ML](https://github.com/Qiskit/qiskit-machine-learning) and follow the best
+  practice from [scikit-learn](https://scikit-learn.org/stable/index.html). We use
+  `flake8` for code formatting. `flake8` is installed with the testing dependencies (see
+  below) or can be installed directly from `pip`:
+
+  ```
+  pip install flake8
+  ```
 
-    ```
-    pytest tests/test_classification.py 
-    ```
+  To execute `flake8`, just type `flake8` from the root repository, and correct all errors
+  related to your changes.
 
-    Workflows are automatically triggered when you push a commit. However, the worflow for example execution is only triggered when you modify one of the examples or the documentation as the execution take a lot of time. You can enable [Github Actions](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/enabling-features-for-your-repository/managing-github-actions-settings-for-a-repository) in your fork to see the result of the CI pipeline. Results are also indicated at the end of your pull request when raised. However note, that workflows in the pull request need approval from the maintainers before being executed.
+- The documentation is based on [Sphinx](https://www.sphinx-doc.org/en/master/).
+- Automation is based on `GitHub Action` and `pytest`. It consists in two automated
+  workflows for running the example and the tests. To run the tests on your local machine,
+  you should first install the dependencies for testing:
+
+  ```
+  pip install .[tests]
+  ```
+
+  and then type `pytest` from the root repository. You can also specify a file like:
+
+  ```
+  pytest tests/test_classification.py
+  ```
+
+  Workflows are automatically triggered when you push a commit. However, the worflow for
+  example execution is only triggered when you modify one of the examples or the
+  documentation as the execution take a lot of time. You can enable
+  [Github Actions](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/enabling-features-for-your-repository/managing-github-actions-settings-for-a-repository)
+  in your fork to see the result of the CI pipeline. Results are also indicated at the end
+  of your pull request when raised. However note, that workflows in the pull request need
+  approval from the maintainers before being executed.
 
 # Troubleshooting
 
 ## Version of pyRiemann not updated
-There is a known issue when you install `pyRiemann-qiskit` in an environement where there is already `pyRiemann` installed. In such case, the `pyRiemann` version is not updated. Therefore before installing or updating `pyRiemann-qiskit`, we recommend to install `pyRiemann` as it follows:
+
+There is a known issue when you install `pyRiemann-qiskit` in an environement where there
+is already `pyRiemann` installed. In such case, the `pyRiemann` version is not updated.
+Therefore before installing or updating `pyRiemann-qiskit`, we recommend to install
+`pyRiemann` as it follows:
 
 ```
 pip uninstall pyriemann
 pip install pyriemann@git+https://github.com/pyRiemann/pyRiemann#egg=pyriemann
 ```
+
+## Firebase admin not loading
+
+In some environment, the firebase admin module is not loaded. There is two reasons:
+
+1. The protobuf package is missing an `__init__.py` file. You can fix this issue by adding
+   it manually as it is done in the DockerFile:
+
+```
+touch /usr/local/lib/python3.8/site-packages/protobuf-4.22.1-py3.8-linux-x86_64.egg/google/__init__.py
+```
+
+2. The Firestore service contains unused dependency to `google.cloud.location`. You can
+   fix this issue by removing the dependencies manually, as it is done in the DockerFile
+   too:
+
+```
+sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/client.py'
+sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/transports/base.py'
+sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/transports/grpc.py'
+sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/transports/grpc_asyncio.py'
+sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/transports/rest.py'
+sed -i 's/from google.cloud.location import locations_pb2//g' '/usr/local/lib/python3.8/site-packages/google_cloud_firestore-2.10.1-py3.8.egg/google/cloud/firestore_v1/services/firestore/async_client.py'
+```
```

### Comparing `pyriemann-qiskit-0.0.3/pyriemann_qiskit/classification.py` & `pyriemann-qiskit-0.0.4/pyriemann_qiskit/classification.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 """Module for classification function."""
 import numpy as np
 from sklearn.base import BaseEstimator, ClassifierMixin, TransformerMixin
 from sklearn.decomposition import PCA
 from sklearn.pipeline import make_pipeline
 from sklearn.svm import SVC
-from qiskit import BasicAer, IBMQ
+from qiskit_ibm_provider import IBMProvider, least_busy
 from qiskit.utils import QuantumInstance, algorithm_globals
 from qiskit.utils.quantum_instance import logger
-from qiskit.providers.ibmq import least_busy
 from qiskit_machine_learning.algorithms import QSVC, VQC, PegasosQSVC
 from qiskit_machine_learning.kernels.quantum_kernel import QuantumKernel
 from datetime import datetime
 import logging
-from .utils.hyper_params_factory import (gen_zz_feature_map,
-                                         gen_two_local,
-                                         get_spsa)
+from .utils.hyper_params_factory import gen_zz_feature_map, gen_two_local, get_spsa
+from .utils import get_provider, get_devices, get_simulator
 from pyriemann.estimation import XdawnCovariances
+from pyriemann.classification import MDM
 from pyriemann.tangentspace import TangentSpace
 from pyriemann_qiskit.datasets import get_feature_dimension
+from pyriemann_qiskit.utils import (
+    ClassicalOptimizer,
+    NaiveQAOAOptimizer,
+    set_global_optimizer,
+)
 
 logger.level = logging.INFO
 
 
 class QuanticClassifierBase(BaseEstimator, ClassifierMixin):
 
     """Quantum classification.
@@ -46,15 +50,15 @@
         - If true will run on local or remote backend
         (depending on q_account_token value).
         - If false, will perform classical computing instead
     q_account_token : string (default:None)
         If quantum==True and q_account_token provided,
         the classification task will be running on a IBM quantum backend.
         If `load_account` is provided, the classifier will use the previous
-        token saved with `IBMQ.save_account()`.
+        token saved with `IBMProvider.save_account()`.
     verbose : bool (default:True)
         If true will output all intermediate results and logs
     shots : int (default:1024)
         Number of repetitions of each circuit, for sampling
     gen_feature_map : Callable[int, QuantumCircuit | FeatureMap] \
                       (default : Callable[int, ZZFeatureMap])
         Function generating a feature map to encode data into a quantum state.
@@ -77,16 +81,22 @@
     ----------
     .. [1] H. Abraham et al., Qiskit:
            An Open-source Framework for Quantum Computing.
            Zenodo, 2019. doi: 10.5281/zenodo.2562110.
 
     """
 
-    def __init__(self, quantum=True, q_account_token=None, verbose=True,
-                 shots=1024, gen_feature_map=gen_zz_feature_map()):
+    def __init__(
+        self,
+        quantum=True,
+        q_account_token=None,
+        verbose=True,
+        shots=1024,
+        gen_feature_map=gen_zz_feature_map(),
+    ):
         self.verbose = verbose
         self._log("Initializing Quantum Classifier")
         self.q_account_token = q_account_token
         self.quantum = quantum
         self.shots = shots
         self.gen_feature_map = gen_feature_map
         # protected field for child classes
@@ -95,32 +105,34 @@
     def _init_quantum(self):
         if self.quantum:
             algorithm_globals.random_seed = datetime.now().microsecond
             self._log("seed = ", algorithm_globals.random_seed)
             if self.q_account_token:
                 self._log("Real quantum computation will be performed")
                 if not self.q_account_token == "load_account":
-                    IBMQ.delete_account()
-                    IBMQ.save_account(self.q_account_token)
-                IBMQ.load_account()
+                    IBMProvider.delete_account()
+                    IBMProvider.save_account(self.q_account_token)
+                IBMProvider.load_account()
                 self._log("Getting provider...")
-                self._provider = IBMQ.get_provider(hub='ibm-q')
+                self._provider = get_provider()
             else:
                 self._log("Quantum simulation will be performed")
-                self._backend = BasicAer.get_backend('qasm_simulator')
+                self._backend = get_simulator()
         else:
             self._log("Classical SVM will be performed")
 
     def _log(self, *values):
         if self.verbose:
             print("[QClass] ", *values)
 
     def _split_classes(self, X, y):
-        self._log("[Warning] Splitting first class from second class."
-                  "Only binary classification is supported.")
+        self._log(
+            "[Warning] Splitting first class from second class."
+            "Only binary classification is supported."
+        )
         X_class1 = X[y == self.classes_[1]]
         X_class0 = X[y == self.classes_[0]]
         return (X_class1, X_class0)
 
     def _map_classes_to_0_1(self, y):
         y_copy = y.copy()
         y_copy[y == self.classes_[0]] = 0
@@ -155,46 +167,45 @@
             The QuanticClassifierBase instance.
         """
         self._init_quantum()
 
         self._log("Fitting: ", X.shape)
         self.classes_ = np.unique(y)
         if len(self.classes_) != 2:
-            raise Exception("Only binary classification \
-                             is currently supported.")
+            raise Exception(
+                "Only binary classification \
+                             is currently supported."
+            )
 
         class1, class0 = self._split_classes(X, y)
         y = self._map_classes_to_0_1(y)
 
         self._training_input[self.classes_[1]] = class1
         self._training_input[self.classes_[0]] = class0
 
         n_features = get_feature_dimension(self._training_input)
         self._log("Feature dimension = ", n_features)
         self._feature_map = self.gen_feature_map(n_features)
         if self.quantum:
             if not hasattr(self, "_backend"):
-                def filters(device):
-                    return (
-                      device.configuration().n_qubits >= n_features
-                      and not device.configuration().simulator
-                      and device.status().operational)
-                devices = self._provider.backends(filters=filters)
+                devices = get_devices(self._provider, n_features)
                 try:
                     self._backend = least_busy(devices)
                 except Exception:
                     self._log("Devices are all busy. Getting the first one...")
                     self._backend = devices[0]
                 self._log("Quantum backend = ", self._backend)
             seed_sim = algorithm_globals.random_seed
             seed_trs = algorithm_globals.random_seed
-            self._quantum_instance = QuantumInstance(self._backend,
-                                                     shots=self.shots,
-                                                     seed_simulator=seed_sim,
-                                                     seed_transpiler=seed_trs)
+            self._quantum_instance = QuantumInstance(
+                self._backend,
+                shots=self.shots,
+                seed_simulator=seed_sim,
+                seed_transpiler=seed_trs,
+            )
         self._classifier = self._init_algo(n_features)
         self._train(X, y)
         return self
 
     def _init_algo(self, n_features):
         raise Exception("Init algo method was not implemented")
 
@@ -286,39 +297,43 @@
            doi: 10.48550/arXiv.2203.00031
 
     .. [5] S. Shalev-Shwartz, Y. Singer, and A. Cotter,
            ‘Pegasos: Primal Estimated sub-GrAdient SOlver for SVM’
 
     """
 
-    def __init__(self, gamma='scale', C=1.0, max_iter=None,
-                 pegasos=False, **parameters):
+    def __init__(
+        self, gamma="scale", C=1.0, max_iter=None, pegasos=False, **parameters
+    ):
         QuanticClassifierBase.__init__(self, **parameters)
         self.gamma = gamma
         self.C = C
         self.max_iter = max_iter
         self.pegasos = pegasos
 
     def _init_algo(self, n_features):
         self._log("SVM initiating algorithm")
         if self.quantum:
-            quantum_kernel = \
-                QuantumKernel(feature_map=self._feature_map,
-                              quantum_instance=self._quantum_instance)
+            quantum_kernel = QuantumKernel(
+                feature_map=self._feature_map, quantum_instance=self._quantum_instance
+            )
             if self.pegasos:
                 self._log("[Warning] `gamma` is not supported by PegasosQSVC")
                 num_steps = 1000 if self.max_iter is None else self.max_iter
-                classifier = PegasosQSVC(quantum_kernel=quantum_kernel,
-                                         C=self.C,
-                                         num_steps=num_steps)
+                classifier = PegasosQSVC(
+                    quantum_kernel=quantum_kernel, C=self.C, num_steps=num_steps
+                )
             else:
                 max_iter = -1 if self.max_iter is None else self.max_iter
-                classifier = QSVC(quantum_kernel=quantum_kernel,
-                                  gamma=self.gamma, C=self.C,
-                                  max_iter=max_iter)
+                classifier = QSVC(
+                    quantum_kernel=quantum_kernel,
+                    gamma=self.gamma,
+                    C=self.C,
+                    max_iter=max_iter,
+                )
         else:
             max_iter = -1 if self.max_iter is None else self.max_iter
             classifier = SVC(gamma=self.gamma, C=self.C, max_iter=max_iter)
         return classifier
 
     def predict_proba(self, X):
         """This method is implemented for compatibility purpose
@@ -335,16 +350,18 @@
         Returns
         -------
         prob : ndarray, shape (n_samples, n_classes)
             prob[n, 0] == True if the nth sample is assigned to 1st class;
             prob[n, 1] == True if the nth sample is assigned to 2nd class.
         """
         predicted_labels = self.predict(X)
-        ret = [np.array([c == self.classes_[0], c == self.classes_[1]])
-               for c in predicted_labels]
+        ret = [
+            np.array([c == self.classes_[0], c == self.classes_[1]])
+            for c in predicted_labels
+        ]
         return np.array(ret)
 
     def predict(self, X):
         """Calculates the predictions.
 
         Parameters
         ----------
@@ -402,31 +419,36 @@
            doi: 10.1038/s41586-019-0980-2.
 
     .. [3] \
         https://qiskit.org/documentation/machine-learning/stubs/qiskit_machine_learning.algorithms.VQC.html
 
     """
 
-    def __init__(self, optimizer=get_spsa(), gen_var_form=gen_two_local(),
-                 **parameters):
+    def __init__(
+        self, optimizer=get_spsa(), gen_var_form=gen_two_local(), **parameters
+    ):
         if "quantum" in parameters and not parameters["quantum"]:
-            raise ValueError("VQC can only run on a quantum \
-                              computer or simulator.")
+            raise ValueError(
+                "VQC can only run on a quantum \
+                              computer or simulator."
+            )
         QuanticClassifierBase.__init__(self, **parameters)
         self.optimizer = optimizer
         self.gen_var_form = gen_var_form
 
     def _init_algo(self, n_features):
         self._log("VQC training...")
         var_form = self.gen_var_form(n_features)
-        vqc = VQC(optimizer=self.optimizer,
-                  feature_map=self._feature_map,
-                  ansatz=var_form,
-                  quantum_instance=self._quantum_instance,
-                  num_qubits=n_features)
+        vqc = VQC(
+            optimizer=self.optimizer,
+            feature_map=self._feature_map,
+            ansatz=var_form,
+            quantum_instance=self._quantum_instance,
+            num_qubits=n_features,
+        )
         return vqc
 
     def _map_classes_to_0_1(self, y):
         # Label must be one-hot encoded for VQC
         y_copy = np.ndarray((y.shape[0], 2))
         y_copy[y == self.classes_[0]] = [1, 0]
         y_copy[y == self.classes_[1]] = [0, 1]
@@ -471,17 +493,113 @@
         pred : array, shape (n_samples,)
             Class labels for samples in X.
         """
         labels = self._predict(X)
         return self._map_0_1_to_classes(labels)
 
 
-class QuantumClassifierWithDefaultRiemannianPipeline(BaseEstimator,
-                                                     ClassifierMixin,
-                                                     TransformerMixin):
+class QuanticMDM(QuanticClassifierBase):
+
+    """Quantum-enhanced MDM
+
+    # This class is a convex implementation of the MDM [1]_,
+    # that can runs with quantum optimization.
+    # Only log-euclidian distance between trial and class prototypes
+    # is supported at the moment, but any type of metric
+    # can be used for centroid estimation.
+
+    Notes
+    -----
+    .. versionadded:: 0.0.4
+
+    Parameters
+    ----------
+    metric : string | dict, default={"mean": 'logeuclid', "distance": 'convex'}
+        The type of metric used for centroid and distance estimation.
+        see `mean_covariance` for the list of supported metric.
+        the metric could be a dict with two keys, `mean` and `distance` in
+        order to pass different metrics for the centroid estimation and the
+        distance estimation. Typical usecase is to pass 'logeuclid' metric for
+        the mean in order to boost the computional speed and 'riemann' for the
+        distance in order to keep the good sensitivity for the classification.
+
+    See Also
+    --------
+    QuanticClassifierBase
+    pyriemann.classification.MDM
+
+    References
+    ----------
+    .. [1] `Multiclass Brain-Computer Interface Classification by Riemannian
+        Geometry
+        <https://hal.archives-ouvertes.fr/hal-00681328>`_
+        A. Barachant, S. Bonnet, M. Congedo, and C. Jutten. IEEE Transactions
+        on Biomedical Engineering, vol. 59, no. 4, p. 920-928, 2012.
+    .. [2] `Riemannian geometry applied to BCI classification
+        <https://hal.archives-ouvertes.fr/hal-00602700/>`_
+        A. Barachant, S. Bonnet, M. Congedo and C. Jutten. 9th International
+        Conference Latent Variable Analysis and Signal Separation
+        (LVA/ICA 2010), LNCS vol. 6365, 2010, p. 629-636.
+    """
+
+    def __init__(
+        self, metric={"mean": "logeuclid", "distance": "convex"}, **parameters
+    ):
+        QuanticClassifierBase.__init__(self, **parameters)
+        self.metric = metric
+
+    def _init_algo(self, n_features):
+        self._log("Convex MDM initiating algorithm")
+        classifier = MDM(metric=self.metric)
+        if self.quantum:
+            self._optimizer = NaiveQAOAOptimizer(
+                quantum_instance=self._quantum_instance
+            )
+        else:
+            self._optimizer = ClassicalOptimizer()
+        set_global_optimizer(self._optimizer)
+        return classifier
+
+    def predict_proba(self, X):
+        """Return the probabilities associated with predictions.
+
+        Parameters
+        ----------
+        X : ndarray, shape (n_trials, n_channels, n_channels)
+            ndarray of trials.
+
+        Returns
+        -------
+        prob : ndarray, shape (n_samples, n_classes)
+            prob[n, 0] == True if the nth sample is assigned to 1st class;
+            prob[n, 1] == True if the nth sample is assigned to 2nd class.
+        """
+        return self._classifier.predict_proba(X)
+
+    def predict(self, X):
+        """Calculates the predictions.
+
+        Parameters
+        ----------
+        X : ndarray, shape (n_samples, n_features)
+            Input vector, where `n_samples` is the number of samples and
+            `n_features` is the number of features.
+
+        Returns
+        -------
+        pred : array, shape (n_samples,)
+            Class labels for samples in X.
+        """
+        labels = self._predict(X)
+        return self._map_0_1_to_classes(labels)
+
+
+class QuantumClassifierWithDefaultRiemannianPipeline(
+    BaseEstimator, ClassifierMixin, TransformerMixin
+):
 
     """Default pipeline with Riemann Geometry and a quantum classifier.
 
     Projects the data into the tangent space of the Riemannian manifold
     and applies quantum classification.
 
     The type of quantum classification (quantum SVM or VQC) depends on
@@ -556,20 +674,28 @@
         https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.rbf_kernel.html
 
     .. [2] \
         https://qiskit.org/documentation/stable/0.36/stubs/qiskit.circuit.library.NLocal.html
 
     """
 
-    def __init__(self, nfilter=1, dim_red=PCA(),
-                 gamma='scale', C=1.0, max_iter=None,
-                 shots=1024, feature_entanglement='full',
-                 feature_reps=2, spsa_trials=None, two_local_reps=None,
-                 params={}):
-
+    def __init__(
+        self,
+        nfilter=1,
+        dim_red=PCA(),
+        gamma="scale",
+        C=1.0,
+        max_iter=None,
+        shots=1024,
+        feature_entanglement="full",
+        feature_reps=2,
+        spsa_trials=None,
+        two_local_reps=None,
+        params={},
+    ):
         self.nfilter = nfilter
         self.dim_red = dim_red
         self.gamma = gamma
         self.C = C
         self.max_iter = max_iter
         self.shots = shots
         self.feature_entanglement = feature_entanglement
@@ -582,29 +708,37 @@
         is_quantum = shots is not None
 
         feature_map = gen_zz_feature_map(feature_reps, feature_entanglement)
         # verbose is passed as an additional parameter to quantum classifiers.
         self.verbose = "verbose" in params and params["verbose"]
         if is_vqc:
             self._log("QuanticVQC chosen.")
-            clf = QuanticVQC(optimizer=get_spsa(spsa_trials),
-                             gen_var_form=gen_two_local(two_local_reps),
-                             gen_feature_map=feature_map,
-                             shots=self.shots,
-                             quantum=is_quantum,
-                             **params)
+            clf = QuanticVQC(
+                optimizer=get_spsa(spsa_trials),
+                gen_var_form=gen_two_local(two_local_reps),
+                gen_feature_map=feature_map,
+                shots=self.shots,
+                quantum=is_quantum,
+                **params
+            )
         else:
             self._log("QuanticSVM chosen.")
-            clf = QuanticSVM(quantum=is_quantum, gamma=gamma, C=C,
-                             max_iter=max_iter,
-                             gen_feature_map=feature_map,
-                             shots=shots, **params)
-
-        self._pipe = make_pipeline(XdawnCovariances(nfilter=nfilter),
-                                   TangentSpace(), dim_red, clf)
+            clf = QuanticSVM(
+                quantum=is_quantum,
+                gamma=gamma,
+                C=C,
+                max_iter=max_iter,
+                gen_feature_map=feature_map,
+                shots=shots,
+                **params
+            )
+
+        self._pipe = make_pipeline(
+            XdawnCovariances(nfilter=nfilter), TangentSpace(), dim_red, clf
+        )
 
     def _log(self, trace):
         if self.verbose:
             print("[QuantumClassifierWithDefaultRiemannianPipeline] ", trace)
 
     def fit(self, X, y):
         """Train the riemann quantum classifier.
```

### Comparing `pyriemann-qiskit-0.0.3/pyriemann_qiskit/datasets/utils.py` & `pyriemann-qiskit-0.0.4/pyriemann_qiskit/datasets/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from warnings import warn
 import numpy as np
+
 try:
     from mne import io, read_events, pick_types, Epochs
     from mne.datasets import sample
 except Exception:
     warn("mne not available. get_mne_sample will fail.")
 from qiskit_machine_learning.datasets import ad_hoc_data
 from sklearn.datasets import make_classification
@@ -101,19 +102,15 @@
     y: ndarray, shape (n_samples,)
         Predicted target vector relative to X.
 
     """
 
     feature_dim = 2
     X, _, _, _ = ad_hoc_data(
-        training_size=30,
-        test_size=0,
-        n=feature_dim,
-        gap=0.3,
-        plot_data=False
+        training_size=30, test_size=0, n=feature_dim, gap=0.3, plot_data=False
     )
 
     y = np.concatenate(([0] * 30, [1] * 30))
 
     return (X, y)
 
 
@@ -129,16 +126,21 @@
     X : ndarray, shape (n_samples, n_features)
         Input vector, where `n_samples` is the number of samples and
         `n_features` is the number of features.
     y: ndarray, shape (n_samples,)
         Predicted target vector relative to X.
 
     """
-    X, y = make_classification(n_features=2, n_redundant=0, n_informative=2,
-                               random_state=1, n_clusters_per_class=1)
+    X, y = make_classification(
+        n_features=2,
+        n_redundant=0,
+        n_informative=2,
+        random_state=1,
+        n_clusters_per_class=1,
+    )
     rng = np.random.RandomState(2)
     X += 2 * rng.uniform(size=X.shape)
 
     return (X, y)
 
 
 def get_feature_dimension(dataset):
@@ -184,15 +186,15 @@
         if not isinstance(v, np.ndarray):
             v = np.asarray(v)
         return v.shape[1]
 
     return -1
 
 
-class MockDataset():
+class MockDataset:
     """A dataset with mock data.
 
     Parameters
     ----------
     dataset_gen : Callable[[], (List, List)]
         A function to generate datasets.
         The function accepts no parameters and returns a pair of lists.
@@ -221,14 +223,15 @@
         The subjects of the dataset.
 
     Notes
     -----
     .. versionadded:: 0.0.3
 
     """
+
     def __init__(self, dataset_gen, n_subjects: int):
         self.code_ = "MockDataset"
         self.subjects_ = range(n_subjects)
         self.data_ = {}
         for subject in self.subjects_:
             self.data_[subject] = dataset_gen()
```

### Comparing `pyriemann-qiskit-0.0.3/pyriemann_qiskit/utils/docplex.py` & `pyriemann-qiskit-0.0.4/pyriemann_qiskit/utils/docplex.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,26 +4,62 @@
 It is for example suitable for:
 - MDM optimization problem;
 - computation of matrices mean.
 """
 import math
 import numpy as np
 from docplex.mp.vartype import ContinuousVarType, IntegerVarType, BinaryVarType
-from qiskit import BasicAer
 from qiskit.utils import QuantumInstance
 from qiskit.algorithms import QAOA
-from qiskit_optimization.algorithms import (CobylaOptimizer,
-                                            MinimumEigenOptimizer)
+from qiskit_optimization.algorithms import CobylaOptimizer, MinimumEigenOptimizer
 from qiskit_optimization.converters import IntegerToBinary
 from qiskit_optimization.translators import from_docplex_mp
-from pyriemann_qiskit.utils import cov_to_corr_matrix
+from pyriemann_qiskit.utils import cov_to_corr_matrix, get_simulator
 
 
-def square_cont_mat_var(prob, channels,
-                        name='cont_covmat'):
+_global_optimizer = None
+
+
+def set_global_optimizer(optimizer):
+    """Set the value of the global optimizer
+
+    Parameters
+    ----------
+    optimizer: pyQiskitOptimizer
+      An instance of pyQiskitOptimizer.
+
+    Notes
+    -----
+    .. versionadded:: 0.0.4
+    """
+    _global_optimizer = optimizer  # noqa
+
+
+def get_global_optimizer(default):
+    """Get the value of the global optimizer
+
+    Parameters
+    ----------
+    default: pyQiskitOptimizer
+      An instance of pyQiskitOptimizer.
+      It will be returned by default if the global optimizer is None.
+
+    Returns
+    -------
+    optimizer : pyQiskitOptimizer
+        The global optimizer.
+
+    Notes
+    -----
+    .. versionadded:: 0.0.4
+    """
+    return _global_optimizer if _global_optimizer is not None else default
+
+
+def square_cont_mat_var(prob, channels, name="cont_covmat"):
     """Creates a 2-dimensional dictionary of continuous decision variables,
     indexed by pairs of key objects.
     The dictionary represents a square matrix of size
     len(channels) x len(channels).
     A key can be any Python object, with the exception of None.
 
     Parameters
@@ -49,21 +85,21 @@
     .. versionadded:: 0.0.2
 
     References
     ----------
     .. [1] \
         http://ibmdecisionoptimization.github.io/docplex-doc/mp/_modules/docplex/mp/model.html#Model
     """
-    ContinuousVarType.one_letter_symbol = lambda _: 'C'
-    return prob.continuous_var_matrix(keys1=channels, keys2=channels,
-                                      name=name, lb=-prob.infinity)
+    ContinuousVarType.one_letter_symbol = lambda _: "C"
+    return prob.continuous_var_matrix(
+        keys1=channels, keys2=channels, name=name, lb=-prob.infinity
+    )
 
 
-def square_int_mat_var(prob, channels, upper_bound=7,
-                       name='int_covmat'):
+def square_int_mat_var(prob, channels, upper_bound=7, name="int_covmat"):
     """Creates a 2-dimensional dictionary of integer decision variables,
     indexed by pairs of key objects.
     The dictionary represents a square matrix of size
     len(channels) x len(channels).
     A key can be any Python object, with the exception of None.
 
     Parameters
@@ -91,21 +127,21 @@
     .. versionadded:: 0.0.2
 
     References
     ----------
     .. [1] \
         http://ibmdecisionoptimization.github.io/docplex-doc/mp/_modules/docplex/mp/model.html#Model
     """
-    IntegerVarType.one_letter_symbol = lambda _: 'I'
-    return prob.integer_var_matrix(keys1=channels, keys2=channels,
-                                   name=name, lb=0, ub=upper_bound)
+    IntegerVarType.one_letter_symbol = lambda _: "I"
+    return prob.integer_var_matrix(
+        keys1=channels, keys2=channels, name=name, lb=0, ub=upper_bound
+    )
 
 
-def square_bin_mat_var(prob, channels,
-                       name='bin_covmat'):
+def square_bin_mat_var(prob, channels, name="bin_covmat"):
     """Creates a 2-dimensional dictionary of binary decision variables,
     indexed by pairs of key objects.
     The dictionary represents a square matrix of size
     len(channels) x len(channels).
     A key can be any Python object, with the exception of None.
 
     Parameters
@@ -131,31 +167,32 @@
     .. versionadded:: 0.0.2
 
     References
     ----------
     .. [1] \
         http://ibmdecisionoptimization.github.io/docplex-doc/mp/_modules/docplex/mp/model.html#Model
     """
-    BinaryVarType.one_letter_symbol = lambda _: 'B'
-    return prob.binary_var_matrix(keys1=channels, keys2=channels,
-                                  name=name)
+    BinaryVarType.one_letter_symbol = lambda _: "B"
+    return prob.binary_var_matrix(keys1=channels, keys2=channels, name=name)
 
 
-class pyQiskitOptimizer():
+class pyQiskitOptimizer:
 
     """Wrapper for Qiskit optimizer.
 
     This class is an abstract class which provides an interface
     for running our docplex model independently of the optimizer type
     (such as classical or quantum optimizer).
 
     Notes
     -----
     .. versionadded:: 0.0.2
+    .. versionchanged:: 0.0.4
     """
+
     def __init__(self):
         pass
 
     """Hook to apply some transformation on a covariance matrix.
 
     Parameters
     ----------
@@ -167,14 +204,15 @@
     transformed_covmat : ndarray, shape (n_features, n_features)
         A transformation of the covariance matrix.
 
     Notes
     -----
     .. versionadded:: 0.0.2
     """
+
     def convert_covmat(self, covmat):
         return covmat
 
     """Helper to create a docplex representation of a
     covariance matrix variable.
 
     Parameters
@@ -200,18 +238,19 @@
 
     References
     ----------
     .. [1] \
         http://ibmdecisionoptimization.github.io/docplex-doc/mp/_modules/docplex/mp/model.html#Model
 
     """
+
     def covmat_var(self, prob, channels, name):
         raise NotImplementedError()
 
-    def _solve_qp(self, qp):
+    def _solve_qp(self, qp, reshape=True):
         raise NotImplementedError()
 
     """Solve the docplex problem.
 
     Parameters
     ----------
     prob : Model
@@ -221,39 +260,68 @@
     -------
     result : OptimizationResult
         The result of the optimization.
 
     Notes
     -----
     .. versionadded:: 0.0.2
+    .. versionchanged:: 0.0.4
 
     References
     ----------
     .. [1] \
         http://ibmdecisionoptimization.github.io/docplex-doc/mp/_modules/docplex/mp/model.html#Model
 
     """
-    def solve(self, prob):
+
+    def solve(self, prob, reshape=True):
         qp = from_docplex_mp(prob)
-        return self._solve_qp(qp)
+        return self._solve_qp(qp, reshape)
+
+    """Helper to create a docplex representation of a
+    weight vector.
+
+    Parameters
+    ----------
+    prob : Model
+        An instance of the docplex model [1]_
+    classes : list
+        The classes.
+
+    Returns
+    -------
+    docplex_weights : dict
+        A vector of decision variables representing
+        our weights.
+
+    Notes
+    -----
+    .. versionadded:: 0.0.4
+
+    """
+
+    def get_weights(self, prob, classes):
+        raise NotImplementedError()
 
 
 class ClassicalOptimizer(pyQiskitOptimizer):
 
     """Wrapper for the classical Cobyla optimizer.
 
     Notes
     -----
     .. versionadded:: 0.0.2
+    .. versionchanged:: 0.0.4
 
     See Also
     --------
     pyQiskitOptimizer
 
     """
+
     def __init__(self):
         pyQiskitOptimizer.__init__(self)
 
     """Helper to create a docplex representation of a
     covariance matrix variable.
 
     Parameters
@@ -283,43 +351,81 @@
 
     References
     ----------
     .. [1] \
         http://ibmdecisionoptimization.github.io/docplex-doc/mp/_modules/docplex/mp/model.html#Model
 
     """
+
     def covmat_var(self, prob, channels, name):
         return square_cont_mat_var(prob, channels, name)
 
-    def _solve_qp(self, qp):
+    def _solve_qp(self, qp, reshape=True):
         result = CobylaOptimizer(rhobeg=0.01, rhoend=0.0001).solve(qp).x
-        n_channels = int(math.sqrt(result.shape[0]))
-        return np.reshape(result, (n_channels, n_channels))
+        if reshape:
+            n_channels = int(math.sqrt(result.shape[0]))
+            return np.reshape(result, (n_channels, n_channels))
+        return result
+
+    """Helper to create a docplex representation of a
+    weight vector.
+
+    Parameters
+    ----------
+    prob : Model
+        An instance of the docplex model [1]_
+    classes : list
+        The classes.
+
+    Returns
+    -------
+    docplex_weights : dict
+        A vector of continuous decision variables representing
+        our weights.
+
+    Notes
+    -----
+    .. versionadded:: 0.0.4
+
+    """
+
+    def get_weights(self, prob, classes):
+        w = prob.continuous_var_matrix(
+            keys1=[1], keys2=classes, name="weight", lb=0, ub=1
+        )
+        w = np.array([w[key] for key in w])
+        return w
 
 
 class NaiveQAOAOptimizer(pyQiskitOptimizer):
 
     """Wrapper for the quantum optimizer QAOA.
 
     Attributes
     ----------
     upper_bound : int (default: 7)
         The maximum integer value for matrix normalization.
+    backend: QuantumInstance (default: None)
+        A quantum backend instance.
+        If None, AerSimulator will be used.
 
     Notes
     -----
     .. versionadded:: 0.0.2
+    .. versionchanged:: 0.0.4
 
     See Also
     --------
     pyQiskitOptimizer
     """
-    def __init__(self, upper_bound=7):
+
+    def __init__(self, upper_bound=7, quantum_instance=None):
         pyQiskitOptimizer.__init__(self)
         self.upper_bound = upper_bound
+        self.quantum_instance = quantum_instance
 
     """Transform all values in the covariance matrix
     to integers.
 
     Example:
     0.123 -> 1230
 
@@ -334,14 +440,15 @@
         A transformation of the covariance matrix.
 
     Notes
     -----
     .. versionadded:: 0.0.2
 
     """
+
     def convert_covmat(self, covmat):
         corr = cov_to_corr_matrix(covmat)
         return np.round(corr * self.upper_bound, 0)
 
     """Helper to create a docplex representation of a
     covariance matrix variable.
 
@@ -372,21 +479,55 @@
 
     References
     ----------
     .. [1] \
         http://ibmdecisionoptimization.github.io/docplex-doc/mp/_modules/docplex/mp/model.html#Model
 
     """
+
     def covmat_var(self, prob, channels, name):
         return square_int_mat_var(prob, channels, self.upper_bound, name)
 
-    def _solve_qp(self, qp):
+    def _solve_qp(self, qp, reshape=True):
         conv = IntegerToBinary()
         qubo = conv.convert(qp)
-        backend = BasicAer.get_backend('statevector_simulator')
-        quantum_instance = QuantumInstance(backend)
-        qaoa_mes = QAOA(quantum_instance=quantum_instance,
-                        initial_point=[0., 0.])
+        if self.quantum_instance is None:
+            backend = get_simulator()
+            quantum_instance = QuantumInstance(backend)
+        else:
+            quantum_instance = self.quantum_instance
+        qaoa_mes = QAOA(quantum_instance=quantum_instance, initial_point=[0.0, 0.0])
         qaoa = MinimumEigenOptimizer(qaoa_mes)
         result = conv.interpret(qaoa.solve(qubo))
-        n_channels = int(math.sqrt(result.shape[0]))
-        return np.reshape(result, (n_channels, n_channels))
+        if reshape:
+            n_channels = int(math.sqrt(result.shape[0]))
+            return np.reshape(result, (n_channels, n_channels))
+        return result
+
+    """Helper to create a docplex representation of a
+    weight vector.
+
+    Parameters
+    ----------
+    prob : Model
+        An instance of the docplex model [1]_
+    classes : list
+        The classes.
+
+    Returns
+    -------
+    docplex_weights : dict
+        A vector of integer decision variables representing
+        our weights.
+
+    Notes
+    -----
+    .. versionadded:: 0.0.4
+
+    """
+
+    def get_weights(self, prob, classes):
+        w = prob.integer_var_matrix(
+            keys1=[1], keys2=classes, name="weight", lb=0, ub=self.upper_bound
+        )
+        w = np.array([w[key] for key in w])
+        return w
```

### Comparing `pyriemann-qiskit-0.0.3/pyriemann_qiskit/utils/filtering.py` & `pyriemann-qiskit-0.0.4/pyriemann_qiskit/utils/filtering.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,24 +113,25 @@
         """
         offset = 0 if self.is_even else 1
         return X[:, offset::2]
 
 
 class Vectorizer(BaseEstimator, TransformerMixin):
     """This is an auxiliary transformer that allows one to vectorize data
-    structures in a pipeline For instance, in the case of an X with
+    structures in a pipeline. For instance, in the case of an X with
     dimensions (n_samples, n_features, n_channels),
     one might be interested in a new data structure with dimensions
     (n_samples, n_features x n_channels)
 
     Notes
     -----
     .. versionadded:: 0.0.1
 
     """
+
     def __init__(self):
         pass
 
     def fit(self, X, y):
         """Fit the training data.
 
         Parameters
```

### Comparing `pyriemann-qiskit-0.0.3/pyriemann_qiskit/utils/hyper_params_factory.py` & `pyriemann-qiskit-0.0.4/pyriemann_qiskit/utils/hyper_params_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from qiskit.circuit.library import ZZFeatureMap
 from qiskit.algorithms.optimizers import SPSA
 from qiskit.circuit.library import TwoLocal
 import inspect
 
 
-def gen_zz_feature_map(reps=2, entanglement='linear'):
+def gen_zz_feature_map(reps=2, entanglement="linear"):
     """Return a callable that generate a ZZFeatureMap.
     A feature map encodes data into a quantum state.
     A ZZFeatureMap is a second-order Pauli-Z evolution circuit.
 
     Parameters
     ----------
     reps : int (default 2)
@@ -32,43 +32,67 @@
 
     References
     ----------
     .. [1] \
         https://qiskit.org/documentation/stable/0.19/stubs/qiskit.circuit.library.NLocal.html
     """
     if reps < 1:
-        raise ValueError("Parameter reps must be superior \
-                          or equal to 1 (Got %d)" % reps)
-
-    return lambda n_features: ZZFeatureMap(feature_dimension=n_features,
-                                           reps=reps,
-                                           entanglement=entanglement)
+        raise ValueError(
+            "Parameter reps must be superior \
+                          or equal to 1 (Got %d)"
+            % reps
+        )
+
+    return lambda n_features: ZZFeatureMap(
+        feature_dimension=n_features, reps=reps, entanglement=entanglement
+    )
 
 
 # Valid gates for two local circuits
-gates = ['ch', 'cx', 'cy', 'cz', 'crx', 'cry', 'crz',
-         'h', 'i', 'id', 'iden',
-         'rx', 'rxx', 'ry', 'ryy', 'rz', 'rzx', 'rzz',
-         's', 'sdg', 'swap',
-         'x', 'y', 'z', 't', 'tdg']
+gates = [
+    "ch",
+    "cx",
+    "cy",
+    "cz",
+    "crx",
+    "cry",
+    "crz",
+    "h",
+    "i",
+    "id",
+    "iden",
+    "rx",
+    "rxx",
+    "ry",
+    "ryy",
+    "rz",
+    "rzx",
+    "rzz",
+    "s",
+    "sdg",
+    "swap",
+    "x",
+    "y",
+    "z",
+    "t",
+    "tdg",
+]
 
 
 def _check_gates_in_blocks(blocks):
     if isinstance(blocks, list):
         for gate in blocks:
             if gate not in gates:
                 raise ValueError("Gate %s is not a valid gate" % gate)
     else:
         if blocks not in gates:
-            raise ValueError("Gate %s is not a valid gate"
-                             % blocks)
+            raise ValueError("Gate %s is not a valid gate" % blocks)
 
 
-def gen_two_local(reps=3, rotation_blocks=['ry', 'rz'],
-                  entanglement_blocks='cz'):
+def gen_two_local(reps=3, rotation_blocks=["ry", "rz"], entanglement_blocks="cz"):
     """Return a callable that generate a TwoLocal circuit.
     The two-local circuit is a parameterized circuit consisting
     of alternating rotation layers and entanglement layers [1]_.
 
     Parameters
     ----------
     reps : int (default 3)
@@ -94,24 +118,27 @@
 
     References
     ----------
     .. [1] \
         https://qiskit.org/documentation/stable/0.19/stubs/qiskit.circuit.library.TwoLocal.html
     """
     if reps < 1:
-        raise ValueError("Parameter reps must be superior \
-                          or equal to 1 (Got %d)" % reps)
+        raise ValueError(
+            "Parameter reps must be superior \
+                          or equal to 1 (Got %d)"
+            % reps
+        )
 
     _check_gates_in_blocks(rotation_blocks)
 
     _check_gates_in_blocks(entanglement_blocks)
 
-    return lambda n_features: TwoLocal(n_features,
-                                       rotation_blocks,
-                                       entanglement_blocks, reps=reps)
+    return lambda n_features: TwoLocal(
+        n_features, rotation_blocks, entanglement_blocks, reps=reps
+    )
 
 
 def get_spsa(max_trials=40, c=(None, None, None, None, 4.0)):
     """Return an instance of SPSA.
     SPSA [1, 2]_ is an algorithmic method for optimizing systems
     with multiple unknown parameters.
     For more details, see [3]_ and [4]_.
@@ -157,23 +184,36 @@
     spsa = SPSA(maxiter=max_trials)
     initial_point = [c[0]] if c[0] else [0]
     initial_pertubation = c[1] if c[1] else 0.2
     alpha = c[2] if c[2] else 0.602
     gamma = c[3] if c[3] else 0.101
     stability_constant = c[4] if c[4] else 0
 
-    def calibrate(loss, initial_point=initial_point,
-                  c=initial_pertubation,
-                  stability_constant=stability_constant,
-                  target_magnitude=None,
-                  alpha=alpha, gamma=gamma,
-                  modelspace=False, max_evals_grouped=1):
-        return SPSA.calibrate(loss, initial_point, c,
-                              stability_constant, target_magnitude,
-                              alpha, gamma, modelspace, max_evals_grouped)
+    def calibrate(
+        loss,
+        initial_point=initial_point,
+        c=initial_pertubation,
+        stability_constant=stability_constant,
+        target_magnitude=None,
+        alpha=alpha,
+        gamma=gamma,
+        modelspace=False,
+        max_evals_grouped=1,
+    ):
+        return SPSA.calibrate(
+            loss,
+            initial_point,
+            c,
+            stability_constant,
+            target_magnitude,
+            alpha,
+            gamma,
+            modelspace,
+            max_evals_grouped,
+        )
 
     spsa.calibrate = calibrate
     return spsa
 
 
 def get_spsa_parameters(spsa):
     """Return the default values of the `calibrate` method of
@@ -197,12 +237,14 @@
 
     References
     ----------
     .. [1] \
         https://qiskit.org/documentation/stable/0.36/stubs/qiskit.algorithms.optimizers.SPSA.calibrate.html
     """
     signature = inspect.signature(spsa.calibrate)
-    return (signature.parameters["initial_point"].default[0],
-            signature.parameters["c"].default,
-            signature.parameters["alpha"].default,
-            signature.parameters["gamma"].default,
-            signature.parameters["stability_constant"].default)
+    return (
+        signature.parameters["initial_point"].default[0],
+        signature.parameters["c"].default,
+        signature.parameters["alpha"].default,
+        signature.parameters["gamma"].default,
+        signature.parameters["stability_constant"].default,
+    )
```

### Comparing `pyriemann-qiskit-0.0.3/pyriemann_qiskit/utils/math.py` & `pyriemann-qiskit-0.0.4/pyriemann_qiskit/utils/math.py`

 * *Files identical despite different names*

### Comparing `pyriemann-qiskit-0.0.3/setup.py` & `pyriemann-qiskit-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,21 +29,25 @@
       project_urls={
           'Documentation': 'https://pyriemann.readthedocs.io',
           'Source': 'https://github.com/pyRiemann/pyRiemann-qiskit',
           'Tracker': 'https://github.com/pyRiemann/pyRiemann-qiskit/issues/',
       },
       platforms='any',
       python_requires=">=3.7",
-      install_requires=['cython', 'pyriemann==0.3',
-                        'qiskit_machine_learning==0.5.0',
-                        'qiskit-ibmq-provider==0.19.2',
-                        'qiskit-optimization==0.4.0',
-                        'cvxpy==1.2.3',
+      install_requires=['cython', 'pyriemann==0.4',
+                        'qiskit_machine_learning==0.6.1',
+                        'qiskit-ibm-provider==0.5.2',
+                        'qiskit-optimization==0.5.0',
+                        'qiskit-aer==0.12.0',
+                        'cvxpy==1.3.1',
                         'scipy==1.7.3',
                         'docplex>=2.21.207',
-                        'firebase_admin==6.0.1',
+                        'firebase_admin==6.1.0',
                         'tqdm'
                         ],
       extras_require={'docs': ['sphinx-gallery', 'sphinx-bootstrap_theme', 'numpydoc', 'mne', 'seaborn', 'moabb>=0.4.6'],
-                      'tests': ['pytest', 'seaborn', 'flake8', 'mne', 'pooch', 'tqdm']},
+                      'tests': ['pytest', 'seaborn', 'flake8', 'mne', 'pooch'],
+                      # GPU optimization not available on all platform.
+                      # See https://github.com/Qiskit/qiskit-aer/issues/929#issuecomment-691716936
+                      'optim': ['qiskit-aer-gpu==0.11.2']},
       zip_safe=False,
 )
```

