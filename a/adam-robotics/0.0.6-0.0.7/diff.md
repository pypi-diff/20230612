# Comparing `tmp/adam-robotics-0.0.6.tar.gz` & `tmp/adam-robotics-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adam-robotics-0.0.6.tar", last modified: Thu Feb  2 11:04:55 2023, max compression
+gzip compressed data, was "adam-robotics-0.0.7.tar", last modified: Mon Jun 12 16:53:53 2023, max compression
```

## Comparing `adam-robotics-0.0.6.tar` & `adam-robotics-0.0.7.tar`

### file list

```diff
@@ -1,53 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-02 11:04:55.829202 adam-robotics-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-02 11:04:55.821202 adam-robotics-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-02 11:04:55.825202 adam-robotics-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      713 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/.github/workflows/pypi-ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)      687 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)    26526 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     7645 2023-02-02 11:04:55.829202 adam-robotics-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7058 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-02 11:04:55.825202 adam-robotics-0.0.6/examples/
--rw-r--r--   0 runner    (1001) docker     (122)    18970 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/examples/iCub_example_casadi.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      963 2023-02-02 11:04:55.829202 adam-robotics-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-02 11:04:55.821202 adam-robotics-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-02 11:04:55.825202 adam-robotics-0.0.6/src/adam/
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-02 11:04:55.825202 adam-robotics-0.0.6/src/adam/casadi/
--rw-r--r--   0 runner    (1001) docker     (122)      261 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/casadi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5918 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/casadi/casadi_like.py
--rw-r--r--   0 runner    (1001) docker     (122)     5736 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/casadi/computations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-02 11:04:55.825202 adam-robotics-0.0.6/src/adam/core/
--rw-r--r--   0 runner    (1001) docker     (122)      270 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19066 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/core/rbd_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (122)     9432 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/core/spatial_math.py
--rw-r--r--   0 runner    (1001) docker     (122)     5654 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/core/urdf_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-02 11:04:55.825202 adam-robotics-0.0.6/src/adam/geometry/
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2415 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/geometry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-02 11:04:55.825202 adam-robotics-0.0.6/src/adam/jax/
--rw-r--r--   0 runner    (1001) docker     (122)      261 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7090 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/jax/computations.py
--rw-r--r--   0 runner    (1001) docker     (122)     6085 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/jax/jax_like.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-02 11:04:55.825202 adam-robotics-0.0.6/src/adam/numpy/
--rw-r--r--   0 runner    (1001) docker     (122)      261 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7326 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/numpy/computations.py
--rw-r--r--   0 runner    (1001) docker     (122)     6265 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/numpy/numpy_like.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-02 11:04:55.825202 adam-robotics-0.0.6/src/adam/pytorch/
--rw-r--r--   0 runner    (1001) docker     (122)      261 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7409 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/pytorch/computations.py
--rw-r--r--   0 runner    (1001) docker     (122)     6559 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/src/adam/pytorch/torch_like.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-02 11:04:55.825202 adam-robotics-0.0.6/src/adam_robotics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7645 2023-02-02 11:04:55.000000 adam-robotics-0.0.6/src/adam_robotics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-02-02 11:04:55.000000 adam-robotics-0.0.6/src/adam_robotics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-02 11:04:55.000000 adam-robotics-0.0.6/src/adam_robotics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-02-02 11:04:55.000000 adam-robotics-0.0.6/src/adam_robotics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-02-02 11:04:55.000000 adam-robotics-0.0.6/src/adam_robotics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-02 11:04:55.829202 adam-robotics-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     6254 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/tests/test_CasADi_computations.py
--rw-r--r--   0 runner    (1001) docker     (122)     6236 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/tests/test_Jax_computations.py
--rw-r--r--   0 runner    (1001) docker     (122)     6194 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/tests/test_NumPy_computations.py
--rw-r--r--   0 runner    (1001) docker     (122)     6803 2023-02-02 11:04:43.000000 adam-robotics-0.0.6/tests/test_pytorch_computations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:53.700896 adam-robotics-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:53.692896 adam-robotics-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:53.696896 adam-robotics-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      713 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1674 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/.github/workflows/conda-forge-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/.github/workflows/pypi-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)    26526 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     7776 2023-06-12 16:53:53.700896 adam-robotics-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7189 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/ci_env.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:53.696896 adam-robotics-0.0.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)    19219 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/examples/iCub_example_casadi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      976 2023-06-12 16:53:53.704896 adam-robotics-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:53.692896 adam-robotics-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:53.696896 adam-robotics-0.0.7/src/adam/
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:53.696896 adam-robotics-0.0.7/src/adam/casadi/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/casadi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6273 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/casadi/casadi_like.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6518 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/casadi/computations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:53.696896 adam-robotics-0.0.7/src/adam/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13667 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/core/rbd_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11041 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/core/spatial_math.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:53.700896 adam-robotics-0.0.7/src/adam/geometry/
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2415 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/geometry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:53.700896 adam-robotics-0.0.7/src/adam/jax/
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7356 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/jax/computations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6229 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/jax/jax_like.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:53.700896 adam-robotics-0.0.7/src/adam/model/
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/model/abc_factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4321 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:53.700896 adam-robotics-0.0.7/src/adam/model/std_factories/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/model/std_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2996 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/model/std_factories/std_joint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/model/std_factories/std_link.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1899 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/model/std_factories/std_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4745 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/model/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:53.700896 adam-robotics-0.0.7/src/adam/numpy/
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7503 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/numpy/computations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6321 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/numpy/numpy_like.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:53.700896 adam-robotics-0.0.7/src/adam/parametric/
+-rw-r--r--   0 runner    (1001) docker     (122)     6501 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/parametric/computations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:53.700896 adam-robotics-0.0.7/src/adam/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7600 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/pytorch/computations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6797 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/src/adam/pytorch/torch_like.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:53.700896 adam-robotics-0.0.7/src/adam_robotics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7776 2023-06-12 16:53:53.000000 adam-robotics-0.0.7/src/adam_robotics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-06-12 16:53:53.000000 adam-robotics-0.0.7/src/adam_robotics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 16:53:53.000000 adam-robotics-0.0.7/src/adam_robotics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-06-12 16:53:53.000000 adam-robotics-0.0.7/src/adam_robotics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-12 16:53:53.000000 adam-robotics-0.0.7/src/adam_robotics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 16:53:53.700896 adam-robotics-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     6289 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/tests/test_CasADi_computations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6314 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/tests/test_Jax_computations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6229 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/tests/test_NumPy_computations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6877 2023-06-12 16:53:43.000000 adam-robotics-0.0.7/tests/test_pytorch_computations.py
```

### Comparing `adam-robotics-0.0.6/.github/workflows/black.yml` & `adam-robotics-0.0.7/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `adam-robotics-0.0.6/.github/workflows/pypi-ci.yml` & `adam-robotics-0.0.7/.github/workflows/pypi-ci.yml`

 * *Files identical despite different names*

### Comparing `adam-robotics-0.0.6/.github/workflows/tests.yml` & `adam-robotics-0.0.7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `adam-robotics-0.0.6/.gitignore` & `adam-robotics-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `adam-robotics-0.0.6/LICENSE` & `adam-robotics-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adam-robotics-0.0.6/PKG-INFO` & `adam-robotics-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adam-robotics
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automatic Differentiation for rigid-body-dynamics AlgorithMs
 Home-page: https://github.com/ami-iit/ADAM
 Author: Giuseppe L'Erario
 Author-email: gl.giuseppelerario@gmail.com
 Keywords: robotics,urdf,rigid body dynamics,featherstone,automatic-differentiation,optimization,casadi,jax,pytorch,reinforcement-learning,motion-planning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -114,45 +114,55 @@
 git clone https://github.com/ami-iit/ADAM.git
 cd ADAM
 pip install .[selected-interface]
 ```
 
 ### Installation with conda
 
+#### Installation from conda-forge package
+
+```bash
+mamba create -n adamenv -c conda-forge adam-robotics
+```
+
+If you want to use `jax` or `pytorch`, just install the corresponding package as well.
+
+#### Installation from repo
+
 Install in a conda environment the required dependencies:
 
 - **Jax** interface dependencies:
 
   ```bash
-  mamba create -n adamenv -c conda-forge -c robostack jax numpy lxml prettytable matplotlib ros-noetic-urdfdom-py
+  mamba create -n adamenv -c conda-forge jax numpy lxml prettytable matplotlib urdfdom-py
   ```
 
 - **CasADi** interface dependencies:
 
   ```bash
-  mamba create -n adamenv -c conda-forge -c robostack casadi numpy lxml prettytable matplotlib ros-noetic-urdfdom-py
+  mamba create -n adamenv -c conda-forge casadi numpy lxml prettytable matplotlib urdfdom-py
   ```
 
 - **PyTorch** interface dependencies:
 
   ```bash
-  mamba create -n adamenv -c conda-forge -c robostack pytorch numpy lxml prettytable matplotlib ros-noetic-urdfdom-py
+  mamba create -n adamenv -c conda-forge pytorch numpy lxml prettytable matplotlib urdfdom-py
   ```
 
 - **ALL** interfaces dependencies:
 
   ```bash
-  mamba create -n adamenv -c conda-forge -c robostack jax casadi pytorch numpy lxml prettytable matplotlib ros-noetic-urdfdom-py
+  mamba create -n adamenv -c conda-forge jax casadi pytorch numpy lxml prettytable matplotlib urdfdom-py
   ```
 
 Activate the environment, clone the repo and install the library:
 
 ```bash
 mamba activate adamenv
-git clone https://github.com/dic-iit/ADAM.git
+git clone https://github.com/ami-iit/ADAM.git
 cd ADAM
 pip install --no-deps .
 ```
 
 ## 🚀 Usage
 
 The following are small snippets of the use of ADAM. More examples are arriving!
```

### Comparing `adam-robotics-0.0.6/README.md` & `adam-robotics-0.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -97,45 +97,55 @@
 git clone https://github.com/ami-iit/ADAM.git
 cd ADAM
 pip install .[selected-interface]
 ```
 
 ### Installation with conda
 
+#### Installation from conda-forge package
+
+```bash
+mamba create -n adamenv -c conda-forge adam-robotics
+```
+
+If you want to use `jax` or `pytorch`, just install the corresponding package as well.
+
+#### Installation from repo
+
 Install in a conda environment the required dependencies:
 
 - **Jax** interface dependencies:
 
   ```bash
-  mamba create -n adamenv -c conda-forge -c robostack jax numpy lxml prettytable matplotlib ros-noetic-urdfdom-py
+  mamba create -n adamenv -c conda-forge jax numpy lxml prettytable matplotlib urdfdom-py
   ```
 
 - **CasADi** interface dependencies:
 
   ```bash
-  mamba create -n adamenv -c conda-forge -c robostack casadi numpy lxml prettytable matplotlib ros-noetic-urdfdom-py
+  mamba create -n adamenv -c conda-forge casadi numpy lxml prettytable matplotlib urdfdom-py
   ```
 
 - **PyTorch** interface dependencies:
 
   ```bash
-  mamba create -n adamenv -c conda-forge -c robostack pytorch numpy lxml prettytable matplotlib ros-noetic-urdfdom-py
+  mamba create -n adamenv -c conda-forge pytorch numpy lxml prettytable matplotlib urdfdom-py
   ```
 
 - **ALL** interfaces dependencies:
 
   ```bash
-  mamba create -n adamenv -c conda-forge -c robostack jax casadi pytorch numpy lxml prettytable matplotlib ros-noetic-urdfdom-py
+  mamba create -n adamenv -c conda-forge jax casadi pytorch numpy lxml prettytable matplotlib urdfdom-py
   ```
 
 Activate the environment, clone the repo and install the library:
 
 ```bash
 mamba activate adamenv
-git clone https://github.com/dic-iit/ADAM.git
+git clone https://github.com/ami-iit/ADAM.git
 cd ADAM
 pip install --no-deps .
 ```
 
 ## 🚀 Usage
 
 The following are small snippets of the use of ADAM. More examples are arriving!
```

### Comparing `adam-robotics-0.0.6/examples/iCub_example_casadi.ipynb` & `adam-robotics-0.0.7/examples/iCub_example_casadi.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9838635531135531%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'import icub_models')], delete: [4]}}, 1: "*

 * *            "{'attachments': OrderedDict()}, 2: {'source': {insert: [(0, 'urdf_path = "*

 * *            'icub_models.get_model_file("iCubGazeboV2_5")\\n\')], delete: [0]}}, 3: '*

 * *            "{'attachments': OrderedDict()}, 5: {'attachments': OrderedDict()}, 7: {'attachments': "*

 * *            "OrderedDict()}, 9: {'attachments': OrderedDict()}, 11: {'attachments': "*

 * *            "OrderedDict()}, 13: {'attachments': OrderedDict()},  […]*

```diff
@@ -6,45 +6,47 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from adam.casadi.computations import KinDynComputations\n",
                 "from adam.geometry import utils\n",
                 "import numpy as np\n",
                 "import casadi as cs\n",
-                "import gym_ignition_models"
+                "import icub_models"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Import the robot .urdf"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 18,
             "metadata": {},
             "outputs": [],
             "source": [
-                "urdf_path = gym_ignition_models.get_model_file(\"iCubGazeboV2_5\")\n",
+                "urdf_path = icub_models.get_model_file(\"iCubGazeboV2_5\")\n",
                 "# The joint list\n",
                 "joints_name_list = [\n",
                 "    'torso_pitch', 'torso_roll', 'torso_yaw', 'l_shoulder_pitch',\n",
                 "    'l_shoulder_roll', 'l_shoulder_yaw', 'l_elbow', 'r_shoulder_pitch',\n",
                 "    'r_shoulder_roll', 'r_shoulder_yaw', 'r_elbow', 'l_hip_pitch', 'l_hip_roll',\n",
                 "    'l_hip_yaw', 'l_knee', 'l_ankle_pitch', 'l_ankle_roll', 'r_hip_pitch',\n",
                 "    'r_hip_roll', 'r_hip_yaw', 'r_knee', 'r_ankle_pitch', 'r_ankle_roll'\n",
                 "]\n",
                 "# Specify the root link\n",
                 "root_link = 'root_link'\n",
                 "kinDyn = KinDynComputations(urdf_path, joints_name_list, root_link)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The class `KinDynComputations` contains some algorithms for computing kinematics and dynamics quantities."
             ]
         },
         {
@@ -59,14 +61,15 @@
                 "H_b = utils.H_from_Pos_RPY(xyz, rpy)\n",
                 "v_b = (np.random.rand(6) - 0.5) * 5\n",
                 "s = (np.random.rand(len(joints_name_list)) - 0.5) * 5\n",
                 "s_dot = (np.random.rand(len(joints_name_list)) - 0.5) * 5"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Mass Matrix"
             ]
         },
         {
@@ -114,14 +117,15 @@
             ],
             "source": [
                 "M = kinDyn.mass_matrix_fun()\n",
                 "print('Mass matrix:\\n', cs.DM(M(H_b, s)))"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Centroidal Momentum Matrix"
             ]
         },
         {
@@ -146,14 +150,15 @@
             ],
             "source": [
                 "Jcm = kinDyn.centroidal_momentum_matrix_fun()\n",
                 "print('Centroidal Momentum Matrix:\\n', cs.DM(Jcm(H_b, s)))"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Center of mass position"
             ]
         },
         {
@@ -172,14 +177,15 @@
             ],
             "source": [
                 "CoM = kinDyn.CoM_position_fun()\n",
                 "print('Center of Mass position:\\n', cs.DM(CoM(H_b, s)))"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Total Mass"
             ]
         },
         {
@@ -197,14 +203,15 @@
                 }
             ],
             "source": [
                 "print('Total mass:\\n', kinDyn.get_total_mass())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Jacobian"
             ]
         },
         {
@@ -229,14 +236,15 @@
             ],
             "source": [
                 "J = kinDyn.jacobian_fun('l_sole')\n",
                 "print('Jacobian of the left sole:\\n', cs.DM(J(H_b, s)))"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Relative jacobian"
             ]
         },
         {
@@ -261,14 +269,15 @@
             ],
             "source": [
                 "J_r = kinDyn.relative_jacobian_fun('l_sole')\n",
                 "print('Jacobian between the root link and left sole:\\n', cs.DM(J_r(s)))"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Forward kinematics"
             ]
         },
         {
@@ -291,14 +300,15 @@
             ],
             "source": [
                 "H = kinDyn.forward_kinematics_fun('l_sole')\n",
                 "print('Forward kinematics to the left sole:\\n', cs.DM(H(H_b, s)))"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Bias force term"
             ]
         },
         {
@@ -317,14 +327,15 @@
             ],
             "source": [
                 "h = kinDyn.bias_force_fun()\n",
                 "print('Bias force term:\\n', cs.DM(h(H_b, s, v_b, s_dot)))"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Coriolis term"
             ]
         },
         {
@@ -343,14 +354,15 @@
             ],
             "source": [
                 "C = kinDyn.coriolis_term_fun()\n",
                 "print('Coriolis force term:\\n', cs.DM(C(H_b, s, v_b, s_dot)))"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Gravity term"
             ]
         },
         {
@@ -388,15 +400,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.10"
+            "version": "3.10.11"
         },
         "metadata": {
             "interpreter": {
                 "hash": "1aaa65760776477b200513a4708dfe8112d71af684253b4518b287658553a52c"
             }
         },
         "orig_nbformat": 3
```

### Comparing `adam-robotics-0.0.6/setup.cfg` & `adam-robotics-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,17 @@
 test = 
 	jax
 	jaxlib
 	casadi
 	torch
 	pytest
 	idyntree
-	gym-ignition-models
+	icub-models
 	black
+	gym-ignition-models
 all = 
 	jax
 	jaxlib
 	casadi
 	torch
 
 [tool:pytest]
```

### Comparing `adam-robotics-0.0.6/src/adam/casadi/casadi_like.py` & `adam-robotics-0.0.7/src/adam/casadi/casadi_like.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,31 +4,34 @@
 
 from dataclasses import dataclass
 from typing import Union
 
 import casadi as cs
 import numpy.typing as npt
 
-from adam.core.spatial_math import ArrayLike
+from adam.core.spatial_math import ArrayLike, ArrayLikeFactory, SpatialMath
+from adam.numpy import NumpyLike
 
 
 @dataclass
 class CasadiLike(ArrayLike):
+    """Wrapper class for Casadi types"""
+
     array: Union[cs.SX, cs.DM]
 
     def __matmul__(self, other: Union["CasadiLike", npt.ArrayLike]) -> "CasadiLike":
         """Overrides @ operator"""
-        if type(self) is type(other):
+        if type(other) in [CasadiLike, NumpyLike]:
             return CasadiLike(self.array @ other.array)
         else:
             return CasadiLike(self.array @ other)
 
     def __rmatmul__(self, other: Union["CasadiLike", npt.ArrayLike]) -> "CasadiLike":
         """Overrides @ operator"""
-        if type(self) is type(other):
+        if type(other) in [CasadiLike, NumpyLike]:
             return CasadiLike(other.array @ self.array)
         else:
             return CasadiLike(other @ self.array)
 
     def __mul__(self, other: Union["CasadiLike", npt.ArrayLike]) -> "CasadiLike":
         """Overrides * operator"""
         if type(self) is type(other):
@@ -94,69 +97,63 @@
     def T(self) -> "CasadiLike":
         """
         Returns:
             CasadiLike: Transpose of the array
         """
         return CasadiLike(self.array.T)
 
+
+class CasadiLikeFactory(ArrayLikeFactory):
     @staticmethod
     def zeros(*x: int) -> "CasadiLike":
         """
         Returns:
             CasadiLike: Matrix of zeros of dim *x
         """
         return CasadiLike(cs.SX.zeros(*x))
 
     @staticmethod
-    def vertcat(*x) -> "CasadiLike":
-        """
-        Returns:
-            CasadiLike:  vertical concatenation of elements
-        """
-        # here the logic is a bit convoluted: x is a tuple containing CasadiLike
-        # cs.vertcat accepts *args. A list of cs types is created extracting the value
-        # from the CasadiLike stored in the tuple x.
-        # Then the list is unpacked with the * operator.
-        y = [xi.array if isinstance(xi, CasadiLike) else xi for xi in x]
-        return CasadiLike(cs.vertcat(*y))
-
-    @staticmethod
     def eye(x: int) -> "CasadiLike":
         """
         Args:
             x (int): matrix dimension
 
         Returns:
             CasadiLike: Identity matrix
         """
         return CasadiLike(cs.SX.eye(x))
 
     @staticmethod
+    def array(*x) -> "CasadiLike":
+        """
+        Returns:
+            CasadiLike: Vector wrapping *x
+        """
+        return CasadiLike(cs.DM(*x))
+
+
+class SpatialMath(SpatialMath):
+    def __init__(self):
+        super().__init__(CasadiLikeFactory)
+
+    @staticmethod
     def skew(x: Union["CasadiLike", npt.ArrayLike]) -> "CasadiLike":
         """
         Args:
             x (Union[CasadiLike, npt.ArrayLike]): 3D vector
 
         Returns:
             CasadiLike: the skew symmetric matrix from x
         """
         if isinstance(x, CasadiLike):
             return CasadiLike(cs.skew(x.array))
         else:
             return CasadiLike(cs.skew(x))
 
     @staticmethod
-    def array(*x) -> "CasadiLike":
-        """
-        Returns:
-            CasadiLike: Vector wrapping *x
-        """
-        return CasadiLike(cs.DM(*x))
-
-    @staticmethod
     def sin(x: npt.ArrayLike) -> "CasadiLike":
         """
         Args:
             x (npt.ArrayLike): angle value
 
         Returns:
             CasadiLike: the sin value of x
@@ -181,7 +178,25 @@
             x (npt.ArrayLike): vector
             y (npt.ArrayLike): vector
 
         Returns:
             CasadiLike: outer product between x and y
         """
         return CasadiLike(cs.np.outer(x, y))
+
+    @staticmethod
+    def vertcat(*x) -> "CasadiLike":
+        """
+        Returns:
+            CasadiLike:  vertical concatenation of elements
+        """
+        # here the logic is a bit convoluted: x is a tuple containing CasadiLike
+        # cs.vertcat accepts *args. A list of cs types is created extracting the value
+        # from the CasadiLike stored in the tuple x.
+        # Then the list is unpacked with the * operator.
+        y = [xi.array if isinstance(xi, CasadiLike) else xi for xi in x]
+        return CasadiLike(cs.vertcat(*y))
+
+
+if __name__ == "__main__":
+    math = SpatialMath()
+    print(math.eye(3))
```

### Comparing `adam-robotics-0.0.6/src/adam/casadi/computations.py` & `adam-robotics-0.0.7/src/adam/casadi/computations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright (C) 2021 Istituto Italiano di Tecnologia (IIT). All rights reserved.
 # This software may be modified and distributed under the terms of the
 # GNU Lesser General Public License v2.1 or any later version.
 
 import casadi as cs
 import numpy as np
 
-from adam.casadi.casadi_like import CasadiLike
-from adam.core.rbd_algorithms import RBDAlgorithms
+from adam.casadi.casadi_like import SpatialMath
+from adam.core import RBDAlgorithms
+from adam.model import Model, URDFModelFactory
 
 
-class KinDynComputations(RBDAlgorithms, CasadiLike):
+class KinDynComputations:
     """This is a small class that retrieves robot quantities represented in a symbolic fashion using CasADi
     in mixed representation, for Floating Base systems - as humanoid robots.
     """
 
     def __init__(
         self,
         urdfstring: str,
@@ -24,130 +25,150 @@
     ) -> None:
         """
         Args:
             urdfstring (str): path of the urdf
             joints_name_list (list): list of the actuated joints
             root_link (str, optional): the first link. Defaults to 'root_link'.
         """
-        super().__init__(
-            urdfstring=urdfstring,
-            joints_name_list=joints_name_list,
-            root_link=root_link,
-            gravity=gravity,
-        )
+        math = SpatialMath()
+        factory = URDFModelFactory(path=urdfstring, math=math)
+        model = Model.build(factory=factory, joints_name_list=joints_name_list)
+        self.rbdalgos = RBDAlgorithms(model=model, math=math)
+        self.NDoF = self.rbdalgos.NDoF
+        self.g = gravity
         self.f_opts = f_opts
 
     def mass_matrix_fun(self) -> cs.Function:
         """Returns the Mass Matrix functions computed the CRBA
 
         Returns:
             M (casADi function): Mass Matrix
         """
         T_b = cs.SX.sym("T_b", 4, 4)
         s = cs.SX.sym("s", self.NDoF)
-        [M, _] = super().crba(T_b, s)
+        [M, _] = self.rbdalgos.crba(T_b, s)
         return cs.Function("M", [T_b, s], [M.array], self.f_opts)
 
     def centroidal_momentum_matrix_fun(self) -> cs.Function:
         """Returns the Centroidal Momentum Matrix functions computed the CRBA
 
         Returns:
             Jcc (casADi function): Centroidal Momentum matrix
         """
         T_b = cs.SX.sym("T_b", 4, 4)
         s = cs.SX.sym("s", self.NDoF)
-        [_, Jcm] = super().crba(T_b, s)
+        [_, Jcm] = self.rbdalgos.crba(T_b, s)
         return cs.Function("Jcm", [T_b, s], [Jcm.array], self.f_opts)
 
     def forward_kinematics_fun(self, frame: str) -> cs.Function:
         """Computes the forward kinematics relative to the specified frame
 
         Args:
             frame (str): The frame to which the fk will be computed
 
         Returns:
             T_fk (casADi function): The fk represented as Homogenous transformation matrix
         """
         s = cs.SX.sym("s", self.NDoF)
         T_b = cs.SX.sym("T_b", 4, 4)
-        T_fk = super().forward_kinematics(frame, T_b, s)
+        T_fk = self.rbdalgos.forward_kinematics(frame, T_b, s)
         return cs.Function("T_fk", [T_b, s], [T_fk.array], self.f_opts)
 
     def jacobian_fun(self, frame: str) -> cs.Function:
         """Returns the Jacobian relative to the specified frame
 
         Args:
             frame (str): The frame to which the jacobian will be computed
 
         Returns:
             J_tot (casADi function): The Jacobian relative to the frame
         """
         s = cs.SX.sym("s", self.NDoF)
         T_b = cs.SX.sym("T_b", 4, 4)
-        J_tot = super().jacobian(frame, T_b, s)
+        J_tot = self.rbdalgos.jacobian(frame, T_b, s)
         return cs.Function("J_tot", [T_b, s], [J_tot.array], self.f_opts)
 
     def relative_jacobian_fun(self, frame: str) -> cs.Function:
         """Returns the Jacobian between the root link and a specified frame frames
 
         Args:
             frame (str): The tip of the chain
 
         Returns:
             J (casADi function): The Jacobian between the root and the frame
         """
         s = cs.SX.sym("s", self.NDoF)
-        J = super().relative_jacobian(frame, s)
+        J = self.rbdalgos.relative_jacobian(frame, s)
         return cs.Function("J", [s], [J.array], self.f_opts)
 
     def CoM_position_fun(self) -> cs.Function:
         """Returns the CoM positon
 
         Returns:
             com (casADi function): The CoM position
         """
         s = cs.SX.sym("s", self.NDoF)
         T_b = cs.SX.sym("T_b", 4, 4)
-        com_pos = super().CoM_position(T_b, s)
+        com_pos = self.rbdalgos.CoM_position(T_b, s)
         return cs.Function("CoM_pos", [T_b, s], [com_pos.array], self.f_opts)
 
     def bias_force_fun(self) -> cs.Function:
         """Returns the bias force of the floating-base dynamics equation,
         using a reduced RNEA (no acceleration and external forces)
 
         Returns:
             h (casADi function): the bias force
         """
         T_b = cs.SX.sym("T_b", 4, 4)
         s = cs.SX.sym("s", self.NDoF)
         v_b = cs.SX.sym("v_b", 6)
         s_dot = cs.SX.sym("s_dot", self.NDoF)
-        h = super().rnea(T_b, s, v_b, s_dot, self.g)
+        h = self.rbdalgos.rnea(T_b, s, v_b, s_dot, self.g)
         return cs.Function("h", [T_b, s, v_b, s_dot], [h.array], self.f_opts)
 
     def coriolis_term_fun(self) -> cs.Function:
         """Returns the coriolis term of the floating-base dynamics equation,
         using a reduced RNEA (no acceleration and external forces)
 
         Returns:
             C (casADi function): the Coriolis term
         """
         T_b = cs.SX.sym("T_b", 4, 4)
         q = cs.SX.sym("q", self.NDoF)
         v_b = cs.SX.sym("v_b", 6)
         q_dot = cs.SX.sym("q_dot", self.NDoF)
         # set in the bias force computation the gravity term to zero
-        C = super().rnea(T_b, q, v_b, q_dot, np.zeros(6))
+        C = self.rbdalgos.rnea(T_b, q, v_b, q_dot, np.zeros(6))
         return cs.Function("C", [T_b, q, v_b, q_dot], [C.array], self.f_opts)
 
     def gravity_term_fun(self) -> cs.Function:
         """Returns the gravity term of the floating-base dynamics equation,
         using a reduced RNEA (no acceleration and external forces)
 
         Returns:
             G (casADi function): the gravity term
         """
         T_b = cs.SX.sym("T_b", 4, 4)
         q = cs.SX.sym("q", self.NDoF)
         # set in the bias force computation the velocity to zero
-        G = super().rnea(T_b, q, np.zeros(6), np.zeros(self.NDoF), self.g)
+        G = self.rbdalgos.rnea(T_b, q, np.zeros(6), np.zeros(self.NDoF), self.g)
         return cs.Function("G", [T_b, q], [G.array], self.f_opts)
+
+    def forward_kinematics(self, frame, T_b, s) -> cs.Function:
+        """Computes the forward kinematics relative to the specified frame
+
+        Args:
+            frame (str): The frame to which the fk will be computed
+
+        Returns:
+            T_fk (casADi function): The fk represented as Homogenous transformation matrix
+        """
+
+        return self.rbdalgos.forward_kinematics(frame, T_b, s)
+
+    def get_total_mass(self) -> float:
+        """Returns the total mass of the robot
+
+        Returns:
+            mass: The total mass
+        """
+        return self.rbdalgos.get_total_mass()
```

### Comparing `adam-robotics-0.0.6/src/adam/core/spatial_math.py` & `adam-robotics-0.0.7/src/adam/core/spatial_math.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,122 @@
 import abc
 
-import numpy as np
 import numpy.typing as npt
 
 
 class ArrayLike(abc.ABC):
     """Abstract class for a generic Array wrapper. Every method should be implemented for every data type."""
 
+    """This class has to implemented the following operators: """
+
+    @abc.abstractmethod
+    def __add__(self, other):
+        pass
+
+    @abc.abstractmethod
+    def __radd__(self, other):
+        pass
+
+    @abc.abstractmethod
+    def __sub__(self, other):
+        pass
+
+    @abc.abstractmethod
+    def __rsub__(self, other):
+        pass
+
+    @abc.abstractmethod
+    def __mul__(self, other):
+        pass
+
+    @abc.abstractmethod
+    def __rmul__(self, other):
+        pass
+
+    @abc.abstractmethod
+    def __matmul__(self, other):
+        pass
+
+    @abc.abstractmethod
+    def __rmatmul__(self, other):
+        pass
+
     @abc.abstractmethod
-    def zeros(x: npt.ArrayLike) -> npt.ArrayLike:
+    def __neg__(self):
+        pass
+
+    @abc.abstractmethod
+    def __getitem__(self, item):
+        pass
+
+    @abc.abstractmethod
+    def __setitem__(self, key, value):
+        pass
+
+    @abc.abstractmethod
+    def __truediv__(self, other):
+        pass
+
+    @abc.abstractproperty
+    def T(self):
+        """
+        Returns: Transpose of the array
+        """
+        pass
+
+
+class ArrayLikeFactory(abc.ABC):
+    """Abstract class for a generic Array wrapper. Every method should be implemented for every data type."""
+
+    @abc.abstractmethod
+    def zeros(self, x: npt.ArrayLike) -> npt.ArrayLike:
         """
         Args:
             x (npt.ArrayLike): matrix dimension
 
         Returns:
             npt.ArrayLike: zero matrix of dimension x
         """
         pass
 
     @abc.abstractmethod
-    def vertcat(x: npt.ArrayLike) -> npt.ArrayLike:
+    def eye(self, x: npt.ArrayLike) -> npt.ArrayLike:
         """
         Args:
-            x (npt.ArrayLike): elements
+            x (npt.ArrayLike): matrix dimension
 
         Returns:
-            npt.ArrayLike: vertical concatenation of elements x
+            npt.ArrayLike: identity matrix of dimension x
         """
         pass
 
+
+class SpatialMath:
+    """Class implementing the main geometric functions used for computing rigid-body algorithm
+
+    Args:
+        ArrayLike: abstract class describing a generic Array wrapper. It needs to be implemented for every data type
+
+    """
+
+    def __init__(self, factory: ArrayLikeFactory):
+        self._factory = factory
+
+    @property
+    def factory(self) -> ArrayLikeFactory:
+        return self._factory
+
     @abc.abstractmethod
-    def eye(x: npt.ArrayLike) -> npt.ArrayLike:
+    def vertcat(x: npt.ArrayLike) -> npt.ArrayLike:
         """
         Args:
-            x (npt.ArrayLike): matrix dimension
+            x (npt.ArrayLike): elements
 
         Returns:
-            npt.ArrayLike: identity matrix of dimension x
+            npt.ArrayLike: vertical concatenation of elements x
         """
         pass
 
     @abc.abstractmethod
     def sin(x: npt.ArrayLike) -> npt.ArrayLike:
         """
         Args:
@@ -58,94 +134,84 @@
             x (npt.ArrayLike): angle value
 
         Returns:
             npt.ArrayLike: cos value of angle x
         """
         pass
 
+    @abc.abstractmethod
+    def skew(x):
+        pass
 
-class SpatialMath(ArrayLike):
-    """Class implementing the main geometric functions used for computing rigid-body algorithm
-
-    Args:
-        ArrayLike: abstract class describing a generic Array wrapper. It needs to be implemented for every data type
-
-    """
-
-    @classmethod
-    def R_from_axis_angle(cls, axis: npt.ArrayLike, q: npt.ArrayLike) -> npt.ArrayLike:
+    def R_from_axis_angle(self, axis: npt.ArrayLike, q: npt.ArrayLike) -> npt.ArrayLike:
         """
         Args:
             axis (npt.ArrayLike): axis vector
             q (npt.ArrayLike): angle value
 
         Returns:
             npt.ArrayLike: rotation matrix from axis-angle representation
         """
-        cq, sq = cls.cos(q), cls.sin(q)
+        cq, sq = self.cos(q), self.sin(q)
         return (
-            cq * (cls.eye(3) - cls.outer(axis, axis))
-            + sq * cls.skew(axis)
-            + cls.outer(axis, axis)
+            cq * (self.factory.eye(3) - self.outer(axis, axis))
+            + sq * self.skew(axis)
+            + self.outer(axis, axis)
         )
 
-    @classmethod
-    def Rx(cls, q: npt.ArrayLike) -> npt.ArrayLike:
+    def Rx(self, q: npt.ArrayLike) -> npt.ArrayLike:
         """
         Args:
             q (npt.ArrayLike): angle value
 
         Returns:
             npt.ArrayLike: rotation matrix around x axis
         """
-        R = cls.eye(3)
-        cq, sq = cls.cos(q), cls.sin(q)
+        R = self.factory.eye(3)
+        cq, sq = self.cos(q), self.sin(q)
         R[1, 1] = cq
         R[1, 2] = -sq
         R[2, 1] = sq
         R[2, 2] = cq
         return R
 
-    @classmethod
-    def Ry(cls, q: npt.ArrayLike) -> npt.ArrayLike:
+    def Ry(self, q: npt.ArrayLike) -> npt.ArrayLike:
         """
         Args:
             q (npt.ArrayLike): angle value
 
         Returns:
             npt.ArrayLike: rotation matrix around y axis
         """
-        R = cls.eye(3)
-        cq, sq = cls.cos(q), cls.sin(q)
+        R = self.factory.eye(3)
+        cq, sq = self.cos(q), self.sin(q)
         R[0, 0] = cq
         R[0, 2] = sq
         R[2, 0] = -sq
         R[2, 2] = cq
         return R
 
-    @classmethod
-    def Rz(cls, q: npt.ArrayLike) -> npt.ArrayLike:
+    def Rz(self, q: npt.ArrayLike) -> npt.ArrayLike:
         """
         Args:
             q (npt.ArrayLike): angle value
 
         Returns:
             npt.ArrayLike: rotation matrix around z axis
         """
-        R = cls.eye(3)
-        cq, sq = cls.cos(q), cls.sin(q)
+        R = self.factory.eye(3)
+        cq, sq = self.cos(q), self.sin(q)
         R[0, 0] = cq
         R[0, 1] = -sq
         R[1, 0] = sq
         R[1, 1] = cq
         return R
 
-    @classmethod
     def H_revolute_joint(
-        cls,
+        self,
         xyz: npt.ArrayLike,
         rpy: npt.ArrayLike,
         axis: npt.ArrayLike,
         q: npt.ArrayLike,
     ) -> npt.ArrayLike:
         """
         Args:
@@ -153,23 +219,22 @@
             rpy (npt.ArrayLike): joint orientation in the urdf
             axis (npt.ArrayLike): joint axis in the urdf
             q (npt.ArrayLike): joint angle value
 
         Returns:
             npt.ArrayLike: Homogeneous transform
         """
-        T = cls.eye(4)
-        R = cls.R_from_RPY(rpy) @ cls.R_from_axis_angle(axis, q)
+        T = self.factory.eye(4)
+        R = self.R_from_RPY(rpy) @ self.R_from_axis_angle(axis, q)
         T[:3, :3] = R
         T[:3, 3] = xyz
         return T
 
-    @classmethod
     def H_prismatic_joint(
-        cls,
+        self,
         xyz: npt.ArrayLike,
         rpy: npt.ArrayLike,
         axis: npt.ArrayLike,
         q: npt.ArrayLike,
     ) -> npt.ArrayLike:
         """
         Args:
@@ -177,49 +242,46 @@
             rpy (npt.ArrayLike): joint orientation in the urdf
             axis (npt.ArrayLike): joint axis in the urdf
             q (npt.ArrayLike): joint angle value
 
         Returns:
             npt.ArrayLike: Homogeneous transform
         """
-        T = cls.eye(4)
-        R = cls.R_from_RPY(rpy)
+        T = self.factory.eye(4)
+        R = self.R_from_RPY(rpy)
         T[:3, :3] = R
-        T[:3, 3] = xyz + q * cls.array(axis)
+        T[:3, 3] = xyz + q * self.factory.array(axis)
         return T
 
-    @classmethod
-    def H_from_Pos_RPY(cls, xyz: npt.ArrayLike, rpy: npt.ArrayLike) -> npt.ArrayLike:
+    def H_from_Pos_RPY(self, xyz: npt.ArrayLike, rpy: npt.ArrayLike) -> npt.ArrayLike:
         """
         Args:
             xyz (npt.ArrayLike): translation vector
             rpy (npt.ArrayLike): rotation as rpy angles
 
         Returns:
             npt.ArrayLike: Homegeneous transform
         """
-        T = cls.eye(4)
-        T[:3, :3] = cls.R_from_RPY(rpy)
+        T = self.factory.eye(4)
+        T[:3, :3] = self.R_from_RPY(rpy)
         T[:3, 3] = xyz
         return T
 
-    @classmethod
-    def R_from_RPY(cls, rpy: npt.ArrayLike) -> npt.ArrayLike:
+    def R_from_RPY(self, rpy: npt.ArrayLike) -> npt.ArrayLike:
         """
         Args:
            rpy (npt.ArrayLike): rotation as rpy angles
 
         Returns:
             npt.ArrayLike: Rotation matrix
         """
-        return cls.Rz(rpy[2]) @ cls.Ry(rpy[1]) @ cls.Rx(rpy[0])
+        return self.Rz(rpy[2]) @ self.Ry(rpy[1]) @ self.Rx(rpy[0])
 
-    @classmethod
     def X_revolute_joint(
-        cls,
+        self,
         xyz: npt.ArrayLike,
         rpy: npt.ArrayLike,
         axis: npt.ArrayLike,
         q: npt.ArrayLike,
     ) -> npt.ArrayLike:
         """
         Args:
@@ -228,22 +290,21 @@
             axis (npt.ArrayLike): joint axis in the urdf
             q (npt.ArrayLike): joint angle value
 
         Returns:
             npt.ArrayLike: Spatial transform of a revolute joint given its rotation angle
         """
         # TODO: give Featherstone reference
-        T = cls.H_revolute_joint(xyz, rpy, axis, q)
+        T = self.H_revolute_joint(xyz, rpy, axis, q)
         R = T[:3, :3].T
         p = -T[:3, :3].T @ T[:3, 3]
-        return cls.spatial_transform(R, p)
+        return self.spatial_transform(R, p)
 
-    @classmethod
     def X_prismatic_joint(
-        cls,
+        self,
         xyz: npt.ArrayLike,
         rpy: npt.ArrayLike,
         axis: npt.ArrayLike,
         q: npt.ArrayLike,
     ) -> npt.ArrayLike:
         """
         Args:
@@ -251,96 +312,106 @@
             rpy (npt.ArrayLike): joint orientation in the urdf
             axis (npt.ArrayLike): joint axis in the urdf
             q (npt.ArrayLike): joint angle value
 
         Returns:
             npt.ArrayLike: Spatial transform of a prismatic joint given its increment
         """
-        T = cls.H_prismatic_joint(xyz, rpy, axis, q)
+        T = self.H_prismatic_joint(xyz, rpy, axis, q)
         R = T[:3, :3].T
         p = -T[:3, :3].T @ T[:3, 3]
-        return cls.spatial_transform(R, p)
+        return self.spatial_transform(R, p)
 
-    @classmethod
-    def X_fixed_joint(cls, xyz: npt.ArrayLike, rpy: npt.ArrayLike) -> npt.ArrayLike:
+    def X_fixed_joint(self, xyz: npt.ArrayLike, rpy: npt.ArrayLike) -> npt.ArrayLike:
         """
         Args:
             xyz (npt.ArrayLike): joint origin in the urdf
             rpy (npt.ArrayLike): joint orientation in the urdf
 
         Returns:
             npt.ArrayLike: Spatial transform of a fixed joint
         """
-        T = cls.H_from_Pos_RPY(xyz, rpy)
+        T = self.H_from_Pos_RPY(xyz, rpy)
         R = T[:3, :3].T
         p = -T[:3, :3].T @ T[:3, 3]
-        return cls.spatial_transform(R, p)
-
-    @classmethod
-    def spatial_transform(cls, R: npt.ArrayLike, p: npt.ArrayLike) -> npt.ArrayLike:
-        """_summary_
+        return self.spatial_transform(R, p)
 
+    def spatial_transform(self, R: npt.ArrayLike, p: npt.ArrayLike) -> npt.ArrayLike:
+        """
         Args:
             R (npt.ArrayLike): Rotation matrix
             p (npt.ArrayLike): translation vector
 
         Returns:
             npt.ArrayLike: spatial transform
         """
-        X = cls.zeros(6, 6)
+        X = self.factory.zeros(6, 6)
         X[:3, :3] = R
         X[3:, 3:] = R
-        X[:3, 3:] = cls.skew(p) @ R
+        X[:3, 3:] = self.skew(p) @ R
         return X
 
-    @classmethod
     def spatial_inertia(
-        cls, I: npt.ArrayLike, mass: npt.ArrayLike, c: npt.ArrayLike, rpy: npt.ArrayLike
+        self,
+        I: npt.ArrayLike,
+        mass: npt.ArrayLike,
+        c: npt.ArrayLike,
+        rpy: npt.ArrayLike,
     ) -> npt.ArrayLike:
         """
         Args:
             I (npt.ArrayLike): inertia values from urdf
             mass (npt.ArrayLike): mass value from urdf
             c (npt.ArrayLike): origin of the link from urdf
             rpy (npt.ArrayLike): orientation of the link from the urdf
 
         Returns:
             npt.ArrayLike: the 6x6 inertia matrix expressed at the origin of the link (with rotation)
         """
-        IO = cls.zeros(6, 6)
-        Sc = cls.skew(c)
-        R = cls.R_from_RPY(rpy)
-        inertia_matrix = cls.array(
+        IO = self.factory.zeros(6, 6)
+        Sc = self.skew(c)
+        R = self.R_from_RPY(rpy)
+        inertia_matrix = self.factory.array(
             [[I.ixx, I.ixy, I.ixz], [I.ixy, I.iyy, I.iyz], [I.ixz, I.iyz, I.izz]]
         )
 
         IO[3:, 3:] = R @ inertia_matrix @ R.T + mass * Sc @ Sc.T
         IO[3:, :3] = mass * Sc
         IO[:3, 3:] = mass * Sc.T
-        IO[:3, :3] = cls.eye(3) * mass
+        IO[:3, :3] = self.factory.eye(3) * mass
         return IO
 
-    @classmethod
-    def spatial_skew(cls, v: npt.ArrayLike) -> npt.ArrayLike:
+    def spatial_skew(self, v: npt.ArrayLike) -> npt.ArrayLike:
         """
         Args:
             v (npt.ArrayLike): 6D vector
 
         Returns:
             npt.ArrayLike: spatial skew matrix
         """
-        X = cls.zeros(6, 6)
-        X[:3, :3] = cls.skew(v[3:])
-        X[:3, 3:] = cls.skew(v[:3])
-        X[3:, 3:] = cls.skew(v[3:])
+        X = self.factory.zeros(6, 6)
+        X[:3, :3] = self.skew(v[3:])
+        X[:3, 3:] = self.skew(v[:3])
+        X[3:, 3:] = self.skew(v[3:])
         return X
 
-    @classmethod
-    def spatial_skew_star(cls, v: npt.ArrayLike) -> npt.ArrayLike:
+    def spatial_skew_star(self, v: npt.ArrayLike) -> npt.ArrayLike:
         """
         Args:
             v (npt.ArrayLike): 6D vector
 
         Returns:
             npt.ArrayLike: negative spatial skew matrix traspose
         """
-        return -cls.spatial_skew(v).T
+        return -self.spatial_skew(v).T
+
+    def adjoint(self, R: npt.ArrayLike) -> npt.ArrayLike:
+        """
+        Args:
+            R (npt.ArrayLike): Rotation matrix
+        Returns:
+            npt.ArrayLike: adjoint matrix
+        """
+        X = self.factory.eye(6)
+        X[:3, :3] = R.T
+        X[3:6, 3:6] = R.T
+        return X
```

### Comparing `adam-robotics-0.0.6/src/adam/geometry/utils.py` & `adam-robotics-0.0.7/src/adam/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `adam-robotics-0.0.6/src/adam/jax/computations.py` & `adam-robotics-0.0.7/src/adam/jax/computations.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 # GNU Lesser General Public License v2.1 or any later version.
 
 import jax.numpy as jnp
 import numpy as np
 from jax import grad, jit, vmap
 
 from adam.core.rbd_algorithms import RBDAlgorithms
-from adam.jax.jax_like import JaxLike
+from adam.jax.jax_like import SpatialMath
+from adam.model import Model, URDFModelFactory
 
 
-class KinDynComputations(RBDAlgorithms, JaxLike):
+class KinDynComputations:
     """This is a small class that retrieves robot quantities using Jax
     in mixed representation, for Floating Base systems - as humanoid robots.
     """
 
     def __init__(
         self,
         urdfstring: str,
@@ -24,75 +25,77 @@
     ) -> None:
         """
         Args:
             urdfstring (str): path of the urdf
             joints_name_list (list): list of the actuated joints
             root_link (str, optional): the first link. Defaults to 'root_link'.
         """
-        super().__init__(
-            urdfstring=urdfstring,
-            joints_name_list=joints_name_list,
-            root_link=root_link,
-            gravity=gravity,
-        )
+        math = SpatialMath()
+        factory = URDFModelFactory(path=urdfstring, math=math)
+        model = Model.build(factory=factory, joints_name_list=joints_name_list)
+        self.rbdalgos = RBDAlgorithms(model=model, math=math)
+        self.NDoF = self.rbdalgos.NDoF
+        self.g = gravity
 
     def mass_matrix(self, base_transform: jnp.array, joint_positions: jnp.array):
         """Returns the Mass Matrix functions computed the CRBA
 
         Args:
             base_transform (jnp.array): The homogenous transform from base to world frame
             joint_positions (jnp.array): The joints position
 
         Returns:
             M (jax): Mass Matrix
         """
-        [M, _] = super().crba(base_transform, joint_positions)
+        [M, _] = self.rbdalgos.crba(base_transform, joint_positions)
         return M.array
 
     def centroidal_momentum_matrix(
         self, base_transform: jnp.array, joint_positions: jnp.array
     ):
         """Returns the Centroidal Momentum Matrix functions computed the CRBA
 
         Args:
             base_transform (jnp.array): The homogenous transform from base to world frame
             joint_positions (jnp.array): The joints position
 
         Returns:
             Jcc (jnp.array): Centroidal Momentum matrix
         """
-        [_, Jcm] = self.crba(base_transform, joint_positions)
+        [_, Jcm] = self.rbdalgos.crba(base_transform, joint_positions)
         return Jcm.array
 
     def relative_jacobian(self, frame: str, joint_positions: jnp.array):
         """Returns the Jacobian between the root link and a specified frame frames
 
         Args:
             frame (str): The tip of the chain
             joint_positions (jnp.array): The joints position
 
         Returns:
             J (jnp.array): The Jacobian between the root and the frame
         """
-        return super().relative_jacobian(frame, joint_positions).array
+        return self.rbdalgos.relative_jacobian(frame, joint_positions).array
 
     def forward_kinematics(
         self, frame: str, base_transform: jnp.array, joint_positions: jnp.array
     ):
         """Computes the forward kinematics relative to the specified frame
 
         Args:
             frame (str): The frame to which the fk will be computed
             base_transform (jnp.array): The homogenous transform from base to world frame
             joint_positions (jnp.array): The joints position
 
         Returns:
             T_fk (jnp.array): The fk represented as Homogenous transformation matrix
         """
-        return super().forward_kinematics(frame, base_transform, joint_positions).array
+        return self.rbdalgos.forward_kinematics(
+            frame, base_transform, joint_positions
+        ).array
 
     def forward_kinematics_fun(self, frame):
         return lambda T, joint_positions: self.forward_kinematics(
             frame, T, joint_positions
         )
 
     def jacobian(self, frame: str, base_transform, joint_positions):
@@ -102,15 +105,15 @@
             base_transform (jnp.array): The homogenous transform from base to world frame
             s (jnp.array): The joints position
             frame (str): The frame to which the jacobian will be computed
 
         Returns:
             J_tot (jnp.array): The Jacobian relative to the frame
         """
-        return super().jacobian(frame, base_transform, joint_positions).array
+        return self.rbdalgos.jacobian(frame, base_transform, joint_positions).array
 
     def bias_force(
         self,
         base_transform: jnp.array,
         joint_positions: jnp.array,
         base_velocity: jnp.array,
         s_dot: jnp.array,
@@ -123,19 +126,17 @@
             joint_positions (jnp.array): The joints position
             base_velocity (jnp.array): The base velocity in mixed representation
             s_dot (jnp.array): The joints velocity
 
         Returns:
             h (jnp.array): the bias force
         """
-        return (
-            super()
-            .rnea(base_transform, joint_positions, base_velocity, s_dot, self.g)
-            .array.squeeze()
-        )
+        return self.rbdalgos.rnea(
+            base_transform, joint_positions, base_velocity, s_dot, self.g
+        ).array.squeeze()
 
     def coriolis_term(
         self,
         base_transform: jnp.array,
         joint_positions: jnp.array,
         base_velocity: jnp.array,
         s_dot: jnp.array,
@@ -148,57 +149,59 @@
             joint_positions (jnp.array): The joints position
             base_velocity (jnp.array): The base velocity in mixed representation
             s_dot (jnp.array): The joints velocity
 
         Returns:
             C (jnp.array): the Coriolis term
         """
-        return (
-            super()
-            .rnea(
-                base_transform,
-                joint_positions,
-                base_velocity.reshape(6, 1),
-                s_dot,
-                np.zeros(6),
-            )
-            .array.squeeze()
-        )
+        return self.rbdalgos.rnea(
+            base_transform,
+            joint_positions,
+            base_velocity.reshape(6, 1),
+            s_dot,
+            np.zeros(6),
+        ).array.squeeze()
 
     def gravity_term(
         self, base_transform: jnp.array, joint_positions: jnp.array
     ) -> jnp.array:
         """Returns the gravity term of the floating-base dynamics ejoint_positionsuation,
         using a reduced RNEA (no acceleration and external forces)
 
         Args:
             base_transform (jnp.array): The homogenous transform from base to world frame
             joint_positions (jnp.array): The joints position
 
         Returns:
             G (jnp.array): the gravity term
         """
-        return (
-            super()
-            .rnea(
-                base_transform,
-                joint_positions,
-                np.zeros(6).reshape(6, 1),
-                np.zeros(self.NDoF),
-                self.g,
-            )
-            .array.squeeze()
-        )
+        return self.rbdalgos.rnea(
+            base_transform,
+            joint_positions,
+            np.zeros(6).reshape(6, 1),
+            np.zeros(self.NDoF),
+            self.g,
+        ).array.squeeze()
 
     def CoM_position(
         self, base_transform: jnp.array, joint_positions: jnp.array
     ) -> jnp.array:
         """Returns the CoM positon
 
         Args:
             base_transform (jnp.array): The homogenous transform from base to world frame
             joint_positions (jnp.array): The joints position
 
         Returns:
             com (jnp.array): The CoM position
         """
-        return super().CoM_position(base_transform, joint_positions).array.squeeze()
+        return self.rbdalgos.CoM_position(
+            base_transform, joint_positions
+        ).array.squeeze()
+
+    def get_total_mass(self) -> float:
+        """Returns the total mass of the robot
+
+        Returns:
+            mass: The total mass
+        """
+        return self.rbdalgos.get_total_mass()
```

### Comparing `adam-robotics-0.0.6/src/adam/jax/jax_like.py` & `adam-robotics-0.0.7/src/adam/jax/jax_like.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,30 @@
 
 from dataclasses import dataclass
 from typing import Union
 
 import jax.numpy as jnp
 import numpy.typing as npt
 
-from adam.core.spatial_math import ArrayLike
+from adam.core.spatial_math import ArrayLike, ArrayLikeFactory, SpatialMath
+from adam.numpy import NumpyLike
 
 
 @dataclass
 class JaxLike(ArrayLike):
     """Wrapper class for Jax types"""
 
     array: jnp.array
 
     def __setitem__(self, idx, value: Union["JaxLike", npt.ArrayLike]):
         """Overrides set item operator"""
         if type(self) is type(value):
-            value.array = jnp.squeeze(value.array)
-            try:
-                self.array = self.array.at[idx].set(value.array)
-            except:
-                self.array = self.array.at[idx].set(value.array.reshape(-1, 1))
+            self.array = self.array.at[idx].set(
+                value.array.reshape(self.array[idx].shape)
+            )
         else:
             self.array = self.array.at[idx].set(value)
 
     def __getitem__(self, idx) -> "JaxLike":
         """Overrides get item operator"""
         return JaxLike(self.array[idx])
 
@@ -45,23 +44,25 @@
         Returns:
             JaxLike: transpose of the array
         """
         return JaxLike(self.array.T)
 
     def __matmul__(self, other: Union["JaxLike", npt.ArrayLike]) -> "JaxLike":
         """Overrides @ operator"""
-        if type(self) is not type(other):
+        if type(other) in [JaxLike, NumpyLike]:
+            return JaxLike(self.array @ other.array)
+        else:
             return JaxLike(self.array @ jnp.array(other))
-        return JaxLike(self.array @ other.array)
 
     def __rmatmul__(self, other: Union["JaxLike", npt.ArrayLike]) -> "JaxLike":
         """Overrides @ operator"""
-        if type(self) is not type(other):
-            return JaxLike(jnp.array(other) @ self.array)
-        return JaxLike(other.array @ self.array)
+        if type(other) in [JaxLike, NumpyLike]:
+            return JaxLike(other.array * self.array)
+        else:
+            return JaxLike(jnp.array(other) * self.array)
 
     def __mul__(self, other: Union["JaxLike", npt.ArrayLike]) -> "JaxLike":
         """Overrides * operator"""
         if type(self) is not type(other):
             return JaxLike(self.array * other)
         return JaxLike(self.array * other.array)
 
@@ -87,78 +88,60 @@
         """Overrides + operator"""
         if type(self) is not type(other):
             return JaxLike(self.array.squeeze() + other.squeeze())
         return JaxLike(self.array.squeeze() + other.array.squeeze())
 
     def __sub__(self, other: Union["JaxLike", npt.ArrayLike]) -> "JaxLike":
         """Overrides - operator"""
+
         if type(self) is not type(other):
             return JaxLike(self.array.squeeze() - other.squeeze())
         return JaxLike(self.array.squeeze() - other.array.squeeze())
 
     def __rsub__(self, other: Union["JaxLike", npt.ArrayLike]) -> "JaxLike":
         """Overrides - operator"""
         if type(self) is not type(other):
-            return JaxLike(self.array.squeeze() - other.squeeze())
-        return JaxLike(self.array.squeeze() - other.array.squeeze())
+            return JaxLike(other.squeeze() - self.array.squeeze())
+        return JaxLike(other.array.squeeze() - self.array.squeeze())
 
     def __neg__(self) -> "JaxLike":
         """Overrides - operator"""
         return JaxLike(-self.array)
 
+
+class JaxLikeFactory(ArrayLikeFactory):
     @staticmethod
     def zeros(*x) -> "JaxLike":
         """
         Returns:
             JaxLike: Matrix of zeros of dim *x
         """
         return JaxLike(jnp.zeros(x))
 
     @staticmethod
-    def vertcat(*x) -> "JaxLike":
-        """
-        Returns:
-            JaxLike: Vertical concatenation of elements
-        """
-        if isinstance(x[0], JaxLike):
-            v = jnp.vstack([x[i].array for i in range(len(x))]).reshape(-1, 1)
-        else:
-            v = jnp.vstack([x[i] for i in range(len(x))]).reshape(-1, 1)
-        return JaxLike(v)
-
-    @staticmethod
     def eye(x) -> "JaxLike":
         """
         Returns:
             JaxLike: Identity matrix of dimension x
         """
         return JaxLike(jnp.eye(x))
 
     @staticmethod
-    def skew(x: Union["JaxLike", npt.ArrayLike]) -> "JaxLike":
-        """
-        Args:
-            x (Union[JaxLike, npt.ArrayLike]): vector
-
-        Returns:
-            JaxLike: the skew symmetric matrix from x
-        """
-        if not isinstance(x, JaxLike):
-            return -jnp.cross(jnp.array(x), jnp.eye(3), axisa=0, axisb=0)
-        x = x.array
-        return JaxLike(-jnp.cross(jnp.array(x), jnp.eye(3), axisa=0, axisb=0))
-
-    @staticmethod
     def array(*x) -> "JaxLike":
         """
         Returns:
             JaxLike: Vector wrapping *x
         """
         return JaxLike(jnp.array(x))
 
+
+class SpatialMath(SpatialMath):
+    def __init__(self):
+        super().__init__(JaxLikeFactory())
+
     @staticmethod
     def sin(x: npt.ArrayLike) -> "JaxLike":
         """
         Args:
             x (npt.ArrayLike): angle value
 
         Returns:
@@ -186,7 +169,33 @@
 
         Returns:
             JaxLike: outer product between x and y
         """
         x = jnp.array(x)
         y = jnp.array(y)
         return JaxLike(jnp.outer(x, y))
+
+    @staticmethod
+    def skew(x: Union["JaxLike", npt.ArrayLike]) -> "JaxLike":
+        """
+        Args:
+            x (Union[JaxLike, npt.ArrayLike]): vector
+
+        Returns:
+            JaxLike: the skew symmetric matrix from x
+        """
+        if not isinstance(x, JaxLike):
+            return -jnp.cross(jnp.array(x), jnp.eye(3), axisa=0, axisb=0)
+        x = x.array
+        return JaxLike(-jnp.cross(jnp.array(x), jnp.eye(3), axisa=0, axisb=0))
+
+    @staticmethod
+    def vertcat(*x) -> "JaxLike":
+        """
+        Returns:
+            JaxLike: Vertical concatenation of elements
+        """
+        if isinstance(x[0], JaxLike):
+            v = jnp.vstack([x[i].array for i in range(len(x))]).reshape(-1, 1)
+        else:
+            v = jnp.vstack([x[i] for i in range(len(x))]).reshape(-1, 1)
+        return JaxLike(v)
```

### Comparing `adam-robotics-0.0.6/src/adam/numpy/computations.py` & `adam-robotics-0.0.7/src/adam/numpy/computations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright (C) 2021 Istituto Italiano di Tecnologia (IIT). All rights reserved.
 # This software may be modified and distributed under the terms of the
 # GNU Lesser General Public License v2.1 or any later version.
 
 import numpy as np
 
 from adam.core.rbd_algorithms import RBDAlgorithms
-from adam.numpy.numpy_like import NumpyLike
+from adam.model import Model, URDFModelFactory
+from adam.numpy.numpy_like import SpatialMath
 
 
-class KinDynComputations(RBDAlgorithms, NumpyLike):
+class KinDynComputations:
     """This is a small class that retrieves robot quantities using NumPy
     in mixed representation, for Floating Base systems - as humanoid robots.
     """
 
     def __init__(
         self,
         urdfstring: str,
@@ -22,49 +23,49 @@
     ) -> None:
         """
         Args:
             urdfstring (str): path of the urdf
             joints_name_list (list): list of the actuated joints
             root_link (str, optional): the first link. Defaults to 'root_link'.
         """
-        super().__init__(
-            urdfstring=urdfstring,
-            joints_name_list=joints_name_list,
-            root_link=root_link,
-            gravity=gravity,
-        )
+        math = SpatialMath()
+        factory = URDFModelFactory(path=urdfstring, math=math)
+        model = Model.build(factory=factory, joints_name_list=joints_name_list)
+        self.rbdalgos = RBDAlgorithms(model=model, math=math)
+        self.NDoF = model.NDoF
+        self.g = gravity
 
     def mass_matrix(
         self, base_transform: np.ndarray, joint_positions: np.ndarray
     ) -> np.ndarray:
         """Returns the Mass Matrix functions computed the CRBA
 
         Args:
             base_transform (np.ndarray): The homogenous transform from base to world frame
             joint_positions (np.ndarray): The joints position
 
         Returns:
             M (np.ndarray): Mass Matrix
         """
-        [M, _] = super().crba(base_transform, joint_positions)
+        [M, _] = self.rbdalgos.crba(base_transform, joint_positions)
         return M.array
 
     def centroidal_momentum_matrix(
         self, base_transform: np.ndarray, s: np.ndarray
     ) -> np.ndarray:
         """Returns the Centroidal Momentum Matrix functions computed the CRBA
 
         Args:
             base_transform (np.ndarray): The homogenous transform from base to world frame
             joint_positions (np.ndarray): The joint positions
 
         Returns:
             Jcc (np.ndarray): Centroidal Momentum matrix
         """
-        [_, Jcm] = super().crba(base_transform, s)
+        [_, Jcm] = self.rbdalgos.crba(base_transform, s)
         return Jcm.array
 
     def forward_kinematics(
         self, frame: str, base_transform: np.ndarray, joint_positions: np.ndarray
     ) -> np.ndarray:
         """Computes the forward kinematics relative to the specified frame
 
@@ -72,60 +73,62 @@
             frame (str): The frame to which the fk will be computed
             base_transform (np.ndarray): The homogenous transform from base to world frame
             joint_positions (np.ndarray): The joints position
 
         Returns:
             T_fk (np.ndarray): The fk represented as Homogenous transformation matrix
         """
-        return (
-            super()
-            .forward_kinematics(frame, base_transform, joint_positions)
-            .array.squeeze()
-        )
+        return self.rbdalgos.forward_kinematics(
+            frame, base_transform, joint_positions
+        ).array.squeeze()
 
     def jacobian(
         self, frame: str, base_transform: np.ndarray, joint_positions: np.ndarray
     ) -> np.ndarray:
         """Returns the Jacobian relative to the specified frame
 
         Args:
             frame (str): The frame to which the jacobian will be computed
             base_transform (np.ndarray): The homogenous transform from base to world frame
             joint_positions (np.ndarray): The joints position
 
         Returns:
             J_tot (np.ndarray): The Jacobian relative to the frame
         """
-        return super().jacobian(frame, base_transform, joint_positions).array.squeeze()
+        return self.rbdalgos.jacobian(
+            frame, base_transform, joint_positions
+        ).array.squeeze()
 
     def relative_jacobian(self, frame: str, joint_positions: np.ndarray) -> np.ndarray:
         """Returns the Jacobian between the root link and a specified frame frames
 
         Args:
             frame (str): The tip of the chain
             joint_positions (np.ndarray): The joints position
 
         Returns:
             J (np.ndarray): The Jacobian between the root and the frame
         """
-        return super().relative_jacobian(frame, joint_positions).array
+        return self.rbdalgos.relative_jacobian(frame, joint_positions).array
 
     def CoM_position(
         self, base_transform: np.ndarray, joint_positions: np.ndarray
     ) -> np.ndarray:
         """Returns the CoM positon
 
         Args:
             base_transform (np.ndarray): The homogenous transform from base to world frame
             joint_positions (np.ndarray): The joints position
 
         Returns:
             CoM (np.ndarray): The CoM position
         """
-        return super().CoM_position(base_transform, joint_positions).array.squeeze()
+        return self.rbdalgos.CoM_position(
+            base_transform, joint_positions
+        ).array.squeeze()
 
     def bias_force(
         self,
         base_transform: np.ndarray,
         joint_positions: np.ndarray,
         base_velocity: np.ndarray,
         joint_velocities: np.ndarray,
@@ -138,25 +141,21 @@
             joint_positions (np.ndarray): The joints position
             base_velocity (np.ndarray): The base velocity in mixed representation
             joint_velocities (np.ndarray): The joint velocities
 
         Returns:
             h (np.ndarray): the bias force
         """
-        return (
-            super()
-            .rnea(
-                base_transform,
-                joint_positions,
-                base_velocity.reshape(6, 1),
-                joint_velocities,
-                self.g,
-            )
-            .array.squeeze()
-        )
+        return self.rbdalgos.rnea(
+            base_transform,
+            joint_positions,
+            base_velocity.reshape(6, 1),
+            joint_velocities,
+            self.g,
+        ).array.squeeze()
 
     def coriolis_term(
         self,
         base_transform: np.ndarray,
         joint_positions: np.ndarray,
         base_velocity: np.ndarray,
         joint_velocities: np.ndarray,
@@ -170,43 +169,43 @@
             base_velocity (np.ndarray): The base velocity in mixed representation
             joint_velocities (np.ndarray): The joint velocities
 
         Returns:
             C (np.ndarray): the Coriolis term
         """
         # set in the bias force computation the gravity term to zero
-        return (
-            super()
-            .rnea(
-                base_transform,
-                joint_positions,
-                base_velocity.reshape(6, 1),
-                joint_velocities,
-                np.zeros(6),
-            )
-            .array.squeeze()
-        )
+        return self.rbdalgos.rnea(
+            base_transform,
+            joint_positions,
+            base_velocity.reshape(6, 1),
+            joint_velocities,
+            np.zeros(6),
+        ).array.squeeze()
 
     def gravity_term(
         self, base_transform: np.ndarray, joint_positions: np.ndarray
     ) -> np.ndarray:
         """Returns the gravity term of the floating-base dynamics equation,
         using a reduced RNEA (no acceleration and external forces)
 
         Args:
             base_transform (np.ndarray): The homogenous transform from base to world frame
             joint_positions (np.ndarray): The joints position
 
         Returns:
             G (np.ndarray): the gravity term
         """
-        return (
-            super()
-            .rnea(
-                base_transform,
-                joint_positions,
-                np.zeros(6).reshape(6, 1),
-                np.zeros(self.NDoF),
-                self.g,
-            )
-            .array.squeeze()
-        )
+        return self.rbdalgos.rnea(
+            base_transform,
+            joint_positions,
+            np.zeros(6).reshape(6, 1),
+            np.zeros(self.NDoF),
+            self.g,
+        ).array.squeeze()
+
+    def get_total_mass(self) -> float:
+        """Returns the total mass of the robot
+
+        Returns:
+            mass: The total mass
+        """
+        return self.rbdalgos.get_total_mass()
```

### Comparing `adam-robotics-0.0.6/src/adam/numpy/numpy_like.py` & `adam-robotics-0.0.7/src/adam/numpy/numpy_like.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,27 @@
 
 from dataclasses import dataclass
 from typing import Union
 
 import numpy as np
 import numpy.typing as npt
 
-from adam.core.spatial_math import ArrayLike
+from adam.core.spatial_math import ArrayLike, ArrayLikeFactory, SpatialMath
 
 
 @dataclass
 class NumpyLike(ArrayLike):
     """Class wrapping NumPy types"""
 
     array: np.ndarray
 
     def __setitem__(self, idx, value: Union["NumpyLike", npt.ArrayLike]) -> "NumpyLike":
         """Overrides set item operator"""
         if type(self) is type(value):
-            value.array = np.squeeze(value.array)
-            try:
-                self.array[idx] = value.array
-            except:
-                self.array[idx] = value.array.reshape(-1, 1)
+            self.array[idx] = value.array.reshape(self.array[idx].shape)
         else:
             self.array[idx] = value
 
     def __getitem__(self, idx) -> "NumpyLike":
         """Overrides get item operator"""
         return NumpyLike(self.array[idx])
 
@@ -99,74 +95,55 @@
         if type(self) is not type(other):
             return NumpyLike(self.array.squeeze() - other.squeeze())
         return NumpyLike(self.array.squeeze() - other.array.squeeze())
 
     def __rsub__(self, other: Union["NumpyLike", npt.ArrayLike]) -> "NumpyLike":
         """Overrides - operator"""
         if type(self) is not type(other):
-            return NumpyLike(self.array.squeeze() - other.squeeze())
-        return NumpyLike(self.array.squeeze() - other.array.squeeze())
+            return NumpyLike(other.squeeze() - self.array.squeeze())
+        return NumpyLike(other.array.squeeze() - self.array.squeeze())
 
     def __neg__(self):
         """Overrides - operator"""
         return NumpyLike(-self.array)
 
+
+class NumpyLikeFactory(ArrayLikeFactory):
     @staticmethod
     def zeros(*x) -> "NumpyLike":
         """
         Returns:
             NumpyLike: zero matrix of dimension x
         """
         return NumpyLike(np.zeros(x))
 
     @staticmethod
-    def vertcat(*x: Union["NumpyLike", npt.ArrayLike]) -> "NumpyLike":
-        """
-        Returns:
-            NumpyLike: vertical concatenation of x
-        """
-        if isinstance(x[0], NumpyLike):
-            v = np.vstack([x[i].array for i in range(len(x))]).reshape(-1, 1)
-        else:
-            v = np.vstack([x[i] for i in range(len(x))]).reshape(-1, 1)
-        return NumpyLike(v)
-
-    @staticmethod
     def eye(x: int) -> "NumpyLike":
         """
         Args:
             x (int): matrix dimension
 
         Returns:
             NumpyLike: Identity matrix of dimension x
         """
         return NumpyLike(np.eye(x))
 
     @staticmethod
-    def skew(x: Union["NumpyLike", npt.ArrayLike]) -> "NumpyLike":
-        """
-        Args:
-            x (Union[NumpyLike, npt.ArrayLike]): vector
-
-        Returns:
-            NumpyLike:  the skew symmetric matrix from x
-        """
-        if not isinstance(x, NumpyLike):
-            return -np.cross(np.array(x), np.eye(3), axisa=0, axisb=0)
-        x = x.array
-        return NumpyLike(-np.cross(np.array(x), np.eye(3), axisa=0, axisb=0))
-
-    @staticmethod
     def array(*x) -> "NumpyLike":
         """
         Returns:
             NumpyLike: Vector wrapping *x
         """
         return NumpyLike(np.array(x))
 
+
+class SpatialMath(SpatialMath):
+    def __init__(self):
+        super().__init__(NumpyLikeFactory())
+
     @staticmethod
     def sin(x: npt.ArrayLike) -> "NumpyLike":
         """
         Args:
             x (npt.ArrayLike): angle value
 
         Returns:
@@ -194,7 +171,33 @@
 
         Returns:
             NumpyLike: outer product of x and y
         """
         x = np.array(x)
         y = np.array(y)
         return NumpyLike(np.outer(x, y))
+
+    @staticmethod
+    def vertcat(*x: Union["NumpyLike", npt.ArrayLike]) -> "NumpyLike":
+        """
+        Returns:
+            NumpyLike: vertical concatenation of x
+        """
+        if isinstance(x[0], NumpyLike):
+            v = np.vstack([x[i].array for i in range(len(x))]).reshape(-1, 1)
+        else:
+            v = np.vstack([x[i] for i in range(len(x))]).reshape(-1, 1)
+        return NumpyLike(v)
+
+    @staticmethod
+    def skew(x: Union["NumpyLike", npt.ArrayLike]) -> "NumpyLike":
+        """
+        Args:
+            x (Union[NumpyLike, npt.ArrayLike]): vector
+
+        Returns:
+            NumpyLike:  the skew symmetric matrix from x
+        """
+        if not isinstance(x, NumpyLike):
+            return -np.cross(np.array(x), np.eye(3), axisa=0, axisb=0)
+        x = x.array
+        return NumpyLike(-np.cross(np.array(x), np.eye(3), axisa=0, axisb=0))
```

### Comparing `adam-robotics-0.0.6/src/adam/pytorch/computations.py` & `adam-robotics-0.0.7/src/adam/pytorch/computations.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 # This software may be modified and distributed under the terms of the
 # GNU Lesser General Public License v2.1 or any later version.
 
 import numpy as np
 import torch
 
 from adam.core.rbd_algorithms import RBDAlgorithms
-from adam.pytorch.torch_like import TorchLike
+from adam.model import Model, URDFModelFactory
+from adam.pytorch.torch_like import SpatialMath
 
 
-class KinDynComputations(RBDAlgorithms, TorchLike):
+class KinDynComputations:
     """This is a small class that retrieves robot quantities using Pytorch
     in mixed representation, for Floating Base systems - as humanoid robots.
     """
 
     def __init__(
         self,
         urdfstring: str,
@@ -23,49 +24,49 @@
     ) -> None:
         """
         Args:
             urdfstring (str): path of the urdf
             joints_name_list (list): list of the actuated joints
             root_link (str, optional): the first link. Defaults to 'root_link'.
         """
-        super().__init__(
-            urdfstring=urdfstring,
-            joints_name_list=joints_name_list,
-            root_link=root_link,
-            gravity=gravity,
-        )
+        math = SpatialMath()
+        factory = URDFModelFactory(path=urdfstring, math=math)
+        model = Model.build(factory=factory, joints_name_list=joints_name_list)
+        self.rbdalgos = RBDAlgorithms(model=model, math=math)
+        self.NDoF = self.rbdalgos.NDoF
+        self.g = gravity
 
     def mass_matrix(
         self, base_transform: torch.Tensor, s: torch.Tensor
     ) -> torch.Tensor:
         """Returns the Mass Matrix functions computed the CRBA
 
         Args:
             base_transform (torch.tensor): The homogenous transform from base to world frame
             s (torch.tensor): The joints position
 
         Returns:
             M (torch.tensor): Mass Matrix
         """
-        [M, _] = super().crba(base_transform, s)
+        [M, _] = self.rbdalgos.crba(base_transform, s)
         return M.array
 
     def centroidal_momentum_matrix(
         self, base_transform: torch.Tensor, s: torch.Tensor
     ) -> torch.Tensor:
         """Returns the Centroidal Momentum Matrix functions computed the CRBA
 
         Args:
             base_transform (torch.tensor): The homogenous transform from base to world frame
             s (torch.tensor): The joints position
 
         Returns:
             Jcc (torch.tensor): Centroidal Momentum matrix
         """
-        [_, Jcm] = super().crba(base_transform, s)
+        [_, Jcm] = self.rbdalgos.crba(base_transform, s)
         return Jcm.array
 
     def forward_kinematics(
         self, frame, base_transform: torch.Tensor, s: torch.Tensor
     ) -> torch.Tensor:
         """Computes the forward kinematics relative to the specified frame
 
@@ -74,15 +75,15 @@
             base_transform (torch.tensor): The homogenous transform from base to world frame
             s (torch.tensor): The joints position
 
         Returns:
             T_fk (torch.tensor): The fk represented as Homogenous transformation matrix
         """
         return (
-            super().forward_kinematics(
+            self.rbdalgos.forward_kinematics(
                 frame, torch.FloatTensor(base_transform), torch.FloatTensor(s)
             )
         ).array
 
     def jacobian(
         self, frame: str, base_transform: torch.Tensor, joint_positions: torch.Tensor
     ) -> torch.Tensor:
@@ -92,41 +93,43 @@
             frame (str): The frame to which the jacobian will be computed
             base_transform (torch.tensor): The homogenous transform from base to world frame
             joint_positions (torch.tensor): The joints position
 
         Returns:
             J_tot (torch.tensor): The Jacobian relative to the frame
         """
-        return super().jacobian(frame, base_transform, joint_positions).array
+        return self.rbdalgos.jacobian(frame, base_transform, joint_positions).array
 
     def relative_jacobian(self, frame, joint_positions: torch.Tensor) -> torch.Tensor:
         """Returns the Jacobian between the root link and a specified frame frames
 
         Args:
             frame (str): The tip of the chain
             joint_positions (torch.tensor): The joints position
 
         Returns:
             J (torch.tensor): The Jacobian between the root and the frame
         """
-        return super().relative_jacobian(frame, joint_positions).array
+        return self.rbdalgos.relative_jacobian(frame, joint_positions).array
 
     def CoM_position(
         self, base_transform: torch.Tensor, joint_positions: torch.Tensor
     ) -> torch.Tensor:
         """Returns the CoM positon
 
         Args:
             base_transform (torch.tensor): The homogenous transform from base to world frame
             joint_positions (torch.tensor): The joints position
 
         Returns:
             com (torch.tensor): The CoM position
         """
-        return super().CoM_position(base_transform, joint_positions).array.squeeze()
+        return self.rbdalgos.CoM_position(
+            base_transform, joint_positions
+        ).array.squeeze()
 
     def bias_force(
         self,
         base_transform: torch.Tensor,
         s: torch.Tensor,
         base_velocity: torch.Tensor,
         joint_velocities: torch.Tensor,
@@ -139,25 +142,21 @@
             s (torch.tensor): The joints position
             base_velocity (torch.tensor): The base velocity in mixed representation
             joint_velocities (torch.tensor): The joints velocity
 
         Returns:
             h (torch.tensor): the bias force
         """
-        return (
-            super()
-            .rnea(
-                base_transform,
-                s,
-                base_velocity.reshape(6, 1),
-                joint_velocities,
-                self.g,
-            )
-            .array.squeeze()
-        )
+        return self.rbdalgos.rnea(
+            base_transform,
+            s,
+            base_velocity.reshape(6, 1),
+            joint_velocities,
+            self.g,
+        ).array.squeeze()
 
     def coriolis_term(
         self,
         base_transform: torch.Tensor,
         joint_positions: torch.Tensor,
         base_velocity: torch.Tensor,
         joint_velocities: torch.Tensor,
@@ -171,43 +170,43 @@
             base_velocity (torch.tensor): The base velocity in mixed representation
             joint_velocities (torch.tensor): The joints velocity
 
         Returns:
             C (torch.tensor): the Coriolis term
         """
         # set in the bias force computation the gravity term to zero
-        return (
-            super()
-            .rnea(
-                base_transform,
-                joint_positions,
-                base_velocity.reshape(6, 1),
-                joint_velocities,
-                torch.zeros(6),
-            )
-            .array.squeeze()
-        )
+        return self.rbdalgos.rnea(
+            base_transform,
+            joint_positions,
+            base_velocity.reshape(6, 1),
+            joint_velocities,
+            torch.zeros(6),
+        ).array.squeeze()
 
     def gravity_term(
         self, base_transform: torch.Tensor, base_positions: torch.Tensor
     ) -> torch.Tensor:
         """Returns the gravity term of the floating-base dynamics ejoint_positionsuation,
         using a reduced RNEA (no acceleration and external forces)
 
         Args:
             base_transform (torch.tensor): The homogenous transform from base to world frame
             base_positions (torch.tensor): The joints position
 
         Returns:
             G (torch.tensor): the gravity term
         """
-        return (
-            super()
-            .rnea(
-                base_transform,
-                base_positions,
-                torch.zeros(6).reshape(6, 1),
-                torch.zeros(self.NDoF),
-                torch.FloatTensor(self.g),
-            )
-            .array.squeeze()
-        )
+        return self.rbdalgos.rnea(
+            base_transform,
+            base_positions,
+            torch.zeros(6).reshape(6, 1),
+            torch.zeros(self.NDoF),
+            torch.FloatTensor(self.g),
+        ).array.squeeze()
+
+    def get_total_mass(self) -> float:
+        """Returns the total mass of the robot
+
+        Returns:
+            mass: The total mass
+        """
+        return self.rbdalgos.get_total_mass()
```

### Comparing `adam-robotics-0.0.6/src/adam/pytorch/torch_like.py` & `adam-robotics-0.0.7/src/adam/pytorch/torch_like.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,31 +4,28 @@
 
 from dataclasses import dataclass
 from typing import Union
 
 import numpy.typing as ntp
 import torch
 
-from adam.core.spatial_math import ArrayLike
+from adam.core.spatial_math import ArrayLike, ArrayLikeFactory, SpatialMath
+from adam.numpy import NumpyLike
 
 
 @dataclass
 class TorchLike(ArrayLike):
     """Class wrapping pyTorch types"""
 
     array: torch.Tensor
 
     def __setitem__(self, idx, value: Union["TorchLike", ntp.ArrayLike]) -> "TorchLike":
         """Overrides set item operator"""
         if type(self) is type(value):
-            value.array = torch.squeeze(value.array)
-            try:
-                self.array[idx] = value.array
-            except:
-                self.array[idx] = value.array.reshape(-1, 1)
+            self.array[idx] = value.array.reshape(self.array[idx].shape)
         else:
             self.array[idx] = torch.FloatTensor(value)
 
     def __getitem__(self, idx):
         """Overrides get item operator"""
         return TorchLike(self.array[idx])
 
@@ -41,29 +38,32 @@
 
     @property
     def T(self) -> "TorchLike":
         """
         Returns:
             TorchLike: transpose of array
         """
-        return TorchLike(self.array.T)
+        if len(self.array.shape) != 1:
+            return TorchLike(self.array.mT)
+        x = self.array
+        return TorchLike(x.permute(*torch.arange(x.ndim - 1, -1, -1)))
 
     def __matmul__(self, other: Union["TorchLike", ntp.ArrayLike]) -> "TorchLike":
         """Overrides @ operator"""
         if type(self) is type(other):
-            return TorchLike(self.array @ other.array)
+            return TorchLike(self.array @ other.array.float())
         else:
-            return TorchLike(self.array @ torch.FloatTensor(other))
+            return TorchLike(self.array @ torch.tensor(other).float())
 
     def __rmatmul__(self, other: Union["TorchLike", ntp.ArrayLike]) -> "TorchLike":
         """Overrides @ operator"""
         if type(self) is type(other):
             return TorchLike(other.array @ self.array)
         else:
-            return TorchLike(torch.FloatTensor(other) @ self.array)
+            return TorchLike(torch.tensor(other).float() @ self.array)
 
     def __mul__(self, other: Union["TorchLike", ntp.ArrayLike]) -> "TorchLike":
         """Overrides * operator"""
         if type(self) is type(other):
             return TorchLike(self.array * other.array)
         else:
             return TorchLike(self.array * other)
@@ -108,73 +108,48 @@
         else:
             return TorchLike(other.squeeze() - self.array.squeeze())
 
     def __neg__(self) -> "TorchLike":
         """Overrides - operator"""
         return TorchLike(-self.array)
 
+
+class TorchLikeFactory(ArrayLikeFactory):
     @staticmethod
     def zeros(*x: int) -> "TorchLike":
         """
         Returns:
             TorchLike: zero matrix of dimension *x
         """
         return TorchLike(torch.zeros(x).float())
 
     @staticmethod
-    def vertcat(*x: ntp.ArrayLike) -> "TorchLike":
-        """
-        Returns:
-            TorchLike: vertical concatenation of x
-        """
-        if isinstance(x[0], TorchLike):
-            v = torch.vstack([x[i].array for i in range(len(x))]).reshape(-1, 1)
-        else:
-            v = torch.FloatTensor(x).reshape(-1, 1)
-        return TorchLike(v)
-
-    @staticmethod
     def eye(x: int) -> "TorchLike":
         """
         Args:
             x (int): dimension
 
         Returns:
             TorchLike: identity matrix of dimension x
         """
         return TorchLike(torch.eye(x).float())
 
     @staticmethod
-    def skew(x: Union["TorchLike", ntp.ArrayLike]) -> "TorchLike":
-        """
-        Args:
-            x (Union[TorchLike, ntp.ArrayLike]): vector
-
-        Returns:
-            TorchLike: skew matrix from x
-        """
-        if not isinstance(x, TorchLike):
-            return TorchLike(
-                torch.FloatTensor(
-                    [[0, -x[2], x[1]], [x[2], 0, -x[0]], [-x[1], x[0], 0]]
-                )
-            )
-        x = x.array
-        return TorchLike(
-            torch.FloatTensor([[0, -x[2], x[1]], [x[2], 0, -x[0]], [-x[1], x[0], 0]])
-        )
-
-    @staticmethod
     def array(*x: ntp.ArrayLike) -> "TorchLike":
         """
         Returns:
             TorchLike: vector wrapping x
         """
         return TorchLike(torch.FloatTensor(x))
 
+
+class SpatialMath(SpatialMath):
+    def __init__(self):
+        super().__init__(TorchLikeFactory())
+
     @staticmethod
     def sin(x: ntp.ArrayLike) -> "TorchLike":
         """
         Args:
             x (ntp.ArrayLike): angle value
 
         Returns:
@@ -202,7 +177,39 @@
             x (ntp.ArrayLike): vector
             y (ntp.ArrayLike): vector
 
         Returns:
             TorchLike: outer product of x and y
         """
         return TorchLike(torch.outer(torch.tensor(x), torch.tensor(y)))
+
+    @staticmethod
+    def skew(x: Union["TorchLike", ntp.ArrayLike]) -> "TorchLike":
+        """
+        Args:
+            x (Union[TorchLike, ntp.ArrayLike]): vector
+
+        Returns:
+            TorchLike: skew matrix from x
+        """
+        if not isinstance(x, TorchLike):
+            return TorchLike(
+                torch.FloatTensor(
+                    [[0, -x[2], x[1]], [x[2], 0, -x[0]], [-x[1], x[0], 0]]
+                )
+            )
+        x = x.array
+        return TorchLike(
+            torch.FloatTensor([[0, -x[2], x[1]], [x[2], 0, -x[0]], [-x[1], x[0], 0]])
+        )
+
+    @staticmethod
+    def vertcat(*x: ntp.ArrayLike) -> "TorchLike":
+        """
+        Returns:
+            TorchLike: vertical concatenation of x
+        """
+        if isinstance(x[0], TorchLike):
+            v = torch.vstack([x[i].array for i in range(len(x))]).reshape(-1, 1)
+        else:
+            v = torch.FloatTensor(x).reshape(-1, 1)
+        return TorchLike(v)
```

### Comparing `adam-robotics-0.0.6/src/adam_robotics.egg-info/PKG-INFO` & `adam-robotics-0.0.7/src/adam_robotics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adam-robotics
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automatic Differentiation for rigid-body-dynamics AlgorithMs
 Home-page: https://github.com/ami-iit/ADAM
 Author: Giuseppe L'Erario
 Author-email: gl.giuseppelerario@gmail.com
 Keywords: robotics,urdf,rigid body dynamics,featherstone,automatic-differentiation,optimization,casadi,jax,pytorch,reinforcement-learning,motion-planning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -114,45 +114,55 @@
 git clone https://github.com/ami-iit/ADAM.git
 cd ADAM
 pip install .[selected-interface]
 ```
 
 ### Installation with conda
 
+#### Installation from conda-forge package
+
+```bash
+mamba create -n adamenv -c conda-forge adam-robotics
+```
+
+If you want to use `jax` or `pytorch`, just install the corresponding package as well.
+
+#### Installation from repo
+
 Install in a conda environment the required dependencies:
 
 - **Jax** interface dependencies:
 
   ```bash
-  mamba create -n adamenv -c conda-forge -c robostack jax numpy lxml prettytable matplotlib ros-noetic-urdfdom-py
+  mamba create -n adamenv -c conda-forge jax numpy lxml prettytable matplotlib urdfdom-py
   ```
 
 - **CasADi** interface dependencies:
 
   ```bash
-  mamba create -n adamenv -c conda-forge -c robostack casadi numpy lxml prettytable matplotlib ros-noetic-urdfdom-py
+  mamba create -n adamenv -c conda-forge casadi numpy lxml prettytable matplotlib urdfdom-py
   ```
 
 - **PyTorch** interface dependencies:
 
   ```bash
-  mamba create -n adamenv -c conda-forge -c robostack pytorch numpy lxml prettytable matplotlib ros-noetic-urdfdom-py
+  mamba create -n adamenv -c conda-forge pytorch numpy lxml prettytable matplotlib urdfdom-py
   ```
 
 - **ALL** interfaces dependencies:
 
   ```bash
-  mamba create -n adamenv -c conda-forge -c robostack jax casadi pytorch numpy lxml prettytable matplotlib ros-noetic-urdfdom-py
+  mamba create -n adamenv -c conda-forge jax casadi pytorch numpy lxml prettytable matplotlib urdfdom-py
   ```
 
 Activate the environment, clone the repo and install the library:
 
 ```bash
 mamba activate adamenv
-git clone https://github.com/dic-iit/ADAM.git
+git clone https://github.com/ami-iit/ADAM.git
 cd ADAM
 pip install --no-deps .
 ```
 
 ## 🚀 Usage
 
 The following are small snippets of the use of ADAM. More examples are arriving!
```

### Comparing `adam-robotics-0.0.6/tests/test_CasADi_computations.py` & `adam-robotics-0.0.7/tests/test_CasADi_computations.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 import idyntree.swig as idyntree
 import numpy as np
 import pytest
 
 from adam.casadi import KinDynComputations
 from adam.geometry import utils
 
-model_path = gym_ignition_models.get_model_file("iCubGazeboV2_5")
+np.random.seed(42)
+
+model_path = str(gym_ignition_models.get_model_file("iCubGazeboV2_5"))
 
 joints_name_list = [
     "torso_pitch",
     "torso_roll",
     "torso_yaw",
     "l_shoulder_pitch",
     "l_shoulder_roll",
@@ -72,15 +74,15 @@
 base_vel = (np.random.rand(6) - 0.5) * 5
 # joints quantitites
 joints_val = (np.random.rand(n_dofs) - 0.5) * 5
 joints_dot_val = (np.random.rand(n_dofs) - 0.5) * 5
 
 # set iDynTree kinDyn
 H_b_idyn = H_from_Pos_RPY_idyn(xyz, rpy)
-vb = idyntree.Twist()
+vb = idyntree.Twist.Zero()
 [vb.setVal(i, base_vel[i]) for i in range(6)]
 
 s = idyntree.VectorDynSize(n_dofs)
 [s.setVal(i, joints_val[i]) for i in range(n_dofs)]
 s_dot = idyntree.VectorDynSize(n_dofs)
 [s_dot.setVal(i, joints_dot_val[i]) for i in range(n_dofs)]
 
@@ -186,15 +188,15 @@
     )
     C = comp.coriolis_term_fun()
     C_test = cs.DM(C(H_b, s_, vb_, s_dot_))
     assert C_iDyn_np - C_test == pytest.approx(0.0, abs=1e-4)
 
 
 def test_gravity_term():
-    vb0 = idyntree.Twist()
+    vb0 = idyntree.Twist.Zero()
     s_dot0 = idyntree.VectorDynSize(n_dofs)
     kinDyn.setRobotState(H_b_idyn, s, vb0, s_dot0, g)
     G_iDyn = idyntree.FreeFloatingGeneralizedTorques(kinDyn.model())
     assert kinDyn.generalizedBiasForces(G_iDyn)
     G_iDyn_np = np.concatenate(
         (G_iDyn.baseWrench().toNumPy(), G_iDyn.jointTorques().toNumPy())
     )
```

### Comparing `adam-robotics-0.0.6/tests/test_Jax_computations.py` & `adam-robotics-0.0.7/tests/test_Jax_computations.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,23 @@
 import logging
 
 import gym_ignition_models
 import idyntree.swig as idyntree
 import jax.numpy as jnp
 import numpy as np
 import pytest
+from jax import config
 
 from adam.geometry import utils
 from adam.jax import KinDynComputations
 
-model_path = gym_ignition_models.get_model_file("iCubGazeboV2_5")
+np.random.seed(42)
+config.update("jax_enable_x64", True)
+
+model_path = str(gym_ignition_models.get_model_file("iCubGazeboV2_5"))
 
 joints_name_list = [
     "torso_pitch",
     "torso_roll",
     "torso_yaw",
     "l_shoulder_pitch",
     "l_shoulder_roll",
@@ -72,15 +76,15 @@
 base_vel = (np.random.rand(6) - 0.5) * 5
 # joints quantitites
 joints_val = (np.random.rand(n_dofs) - 0.5) * 5
 joints_dot_val = (np.random.rand(n_dofs) - 0.5) * 5
 
 # set iDynTree kinDyn
 H_b_idyn = H_from_Pos_RPY_idyn(xyz, rpy)
-vb = idyntree.Twist()
+vb = idyntree.Twist.Zero()
 [vb.setVal(i, base_vel[i]) for i in range(6)]
 
 s = idyntree.VectorDynSize(n_dofs)
 s = s.FromPython(joints_val)
 s_dot = idyntree.VectorDynSize(n_dofs)
 s_dot = s_dot.FromPython(joints_dot_val)
 
@@ -91,20 +95,20 @@
 # set ADAM
 H_b = utils.H_from_Pos_RPY(xyz, rpy)
 vb_ = base_vel
 s_ = joints_val
 s_dot_ = joints_dot_val
 
 
-def test_mass_matrix():
-    mass_mx = idyntree.MatrixDynSize()
-    kinDyn.getFreeFloatingMassMatrix(mass_mx)
-    mass_mxNumpy = mass_mx.toNumPy()
-    mass_test = comp.mass_matrix(H_b, s_)
-    assert np.asarray(mass_test) - mass_mxNumpy == pytest.approx(0.0, abs=1e-5)
+# def test_mass_matrix():
+mass_mx = idyntree.MatrixDynSize()
+kinDyn.getFreeFloatingMassMatrix(mass_mx)
+mass_mxNumpy = mass_mx.toNumPy()
+mass_test = comp.mass_matrix(H_b, s_)
+assert np.asarray(mass_test) - mass_mxNumpy == pytest.approx(0.0, abs=1e-5)
 
 
 def test_CMM():
     cmm_idyntree = idyntree.MatrixDynSize()
     kinDyn.getCentroidalTotalMomentumJacobian(cmm_idyntree)
     cmm_idyntreeNumpy = cmm_idyntree.toNumPy()
     Jcm_test = comp.centroidal_momentum_matrix(H_b, s_)
@@ -181,15 +185,15 @@
 
 
 def test_gravity_term():
     kinDyn2 = idyntree.KinDynComputations()
     kinDyn2.loadRobotModel(robot_iDyn.model())
     kinDyn2.setFloatingBase(root_link)
     kinDyn2.setFrameVelocityRepresentation(idyntree.MIXED_REPRESENTATION)
-    vb0 = idyntree.Twist()
+    vb0 = idyntree.Twist.Zero()
     s_dot0 = idyntree.VectorDynSize(n_dofs)
     kinDyn2.setRobotState(H_b_idyn, s, vb0, s_dot0, g)
     G_iDyn = idyntree.FreeFloatingGeneralizedTorques(kinDyn2.model())
     assert kinDyn2.generalizedBiasForces(G_iDyn)
     G_iDyn_np = np.concatenate(
         (G_iDyn.baseWrench().toNumPy(), G_iDyn.jointTorques().toNumPy())
     )
```

### Comparing `adam-robotics-0.0.6/tests/test_NumPy_computations.py` & `adam-robotics-0.0.7/tests/test_NumPy_computations.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 import idyntree.swig as idyntree
 import numpy as np
 import pytest
 
 from adam.geometry import utils
 from adam.numpy import KinDynComputations
 
-model_path = gym_ignition_models.get_model_file("iCubGazeboV2_5")
+np.random.seed(42)
+
+model_path = str(gym_ignition_models.get_model_file("iCubGazeboV2_5"))
 
 joints_name_list = [
     "torso_pitch",
     "torso_roll",
     "torso_yaw",
     "l_shoulder_pitch",
     "l_shoulder_roll",
@@ -71,15 +73,15 @@
 base_vel = (np.random.rand(6) - 0.5) * 5
 # joints quantitites
 joints_val = (np.random.rand(n_dofs) - 0.5) * 5
 joints_dot_val = (np.random.rand(n_dofs) - 0.5) * 5
 
 # set iDynTree kinDyn
 H_b_idyn = H_from_Pos_RPY_idyn(xyz, rpy)
-vb = idyntree.Twist()
+vb = idyntree.Twist.Zero()
 [vb.setVal(i, base_vel[i]) for i in range(6)]
 
 s = idyntree.VectorDynSize(n_dofs)
 [s.setVal(i, joints_val[i]) for i in range(n_dofs)]
 s_dot = idyntree.VectorDynSize(n_dofs)
 [s_dot.setVal(i, joints_dot_val[i]) for i in range(n_dofs)]
 
@@ -180,15 +182,15 @@
 
 
 def test_gravity_term():
     kinDyn2 = idyntree.KinDynComputations()
     kinDyn2.loadRobotModel(robot_iDyn.model())
     kinDyn2.setFloatingBase(root_link)
     kinDyn2.setFrameVelocityRepresentation(idyntree.MIXED_REPRESENTATION)
-    vb0 = idyntree.Twist()
+    vb0 = idyntree.Twist.Zero()
     s_dot0 = idyntree.VectorDynSize(n_dofs)
     kinDyn2.setRobotState(H_b_idyn, s, vb0, s_dot0, g)
     G_iDyn = idyntree.FreeFloatingGeneralizedTorques(kinDyn2.model())
     assert kinDyn2.generalizedBiasForces(G_iDyn)
     G_iDyn_np = np.concatenate(
         (G_iDyn.baseWrench().toNumPy(), G_iDyn.jointTorques().toNumPy())
     )
```

### Comparing `adam-robotics-0.0.6/tests/test_pytorch_computations.py` & `adam-robotics-0.0.7/tests/test_pytorch_computations.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 import numpy as np
 import pytest
 import torch
 
 from adam.geometry import utils
 from adam.pytorch import KinDynComputations
 
-model_path = gym_ignition_models.get_model_file("iCubGazeboV2_5")
+np.random.seed(42)
+torch.set_default_dtype(torch.float64)
+
+model_path = str(gym_ignition_models.get_model_file("iCubGazeboV2_5"))
 
 joints_name_list = [
     "torso_pitch",
     "torso_roll",
     "torso_yaw",
     "l_shoulder_pitch",
     "l_shoulder_roll",
@@ -72,15 +75,15 @@
 base_vel = (np.random.rand(6) - 0.5) * 5
 # joints quantitites
 joints_val = (np.random.rand(n_dofs) - 0.5) * 5
 joints_dot_val = (np.random.rand(n_dofs) - 0.5) * 5
 
 # set iDynTree kinDyn
 H_b_idyn = H_from_Pos_RPY_idyn(xyz, rpy)
-vb = idyntree.Twist()
+vb = idyntree.Twist.Zero()
 [vb.setVal(i, base_vel[i]) for i in range(6)]
 
 s = idyntree.VectorDynSize(n_dofs)
 [s.setVal(i, joints_val[i]) for i in range(n_dofs)]
 s_dot = idyntree.VectorDynSize(n_dofs)
 [s_dot.setVal(i, joints_dot_val[i]) for i in range(n_dofs)]
 
@@ -181,15 +184,15 @@
 
 
 def test_gravity_term():
     kinDyn2 = idyntree.KinDynComputations()
     kinDyn2.loadRobotModel(robot_iDyn.model())
     kinDyn2.setFloatingBase(root_link)
     kinDyn2.setFrameVelocityRepresentation(idyntree.MIXED_REPRESENTATION)
-    vb0 = idyntree.Twist()
+    vb0 = idyntree.Twist.Zero()
     s_dot0 = idyntree.VectorDynSize(n_dofs)
     kinDyn2.setRobotState(H_b_idyn, s, vb0, s_dot0, g)
     G_iDyn = idyntree.FreeFloatingGeneralizedTorques(kinDyn2.model())
     assert kinDyn2.generalizedBiasForces(G_iDyn)
     G_iDyn_np = np.concatenate(
         (G_iDyn.baseWrench().toNumPy(), G_iDyn.jointTorques().toNumPy())
     )
```

