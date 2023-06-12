# Comparing `tmp/sintef-pyshop-1.4.1.tar.gz` & `tmp/sintef-pyshop-1.4.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sintef-pyshop-1.4.1.tar", last modified: Mon Jun 12 12:43:47 2023, max compression
+gzip compressed data, was "sintef-pyshop-1.4.1a0.tar", last modified: Tue Jun  6 15:06:22 2023, max compression
```

## Comparing `sintef-pyshop-1.4.1.tar` & `sintef-pyshop-1.4.1a0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:43:47.810413 sintef-pyshop-1.4.1/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6010 2023-06-12 12:43:47.810413 sintef-pyshop-1.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4952 2023-06-08 08:52:22.000000 sintef-pyshop-1.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:43:47.795413 sintef-pyshop-1.4.1/pyshop/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1/pyshop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:43:47.798413 sintef-pyshop-1.4.1/pyshop/helpers/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1/pyshop/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1/pyshop/helpers/commands.py
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1/pyshop/helpers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     5040 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1/pyshop/helpers/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1/pyshop/helpers/typing_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:43:47.801413 sintef-pyshop-1.4.1/pyshop/lp_model/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1/pyshop/lp_model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2195 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1/pyshop/lp_model/index.py
--rw-rw-rw-   0 root         (0) root         (0)     2555 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1/pyshop/lp_model/lp_model.py
--rw-rw-rw-   0 root         (0) root         (0)    10661 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1/pyshop/lp_model/row.py
--rw-rw-rw-   0 root         (0) root         (0)     9366 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1/pyshop/lp_model/var.py
--rw-rw-rw-   0 root         (0) root         (0)    13751 2023-06-08 08:57:15.000000 sintef-pyshop-1.4.1/pyshop/shop_runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:43:47.806413 sintef-pyshop-1.4.1/pyshop/shopcore/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1/pyshop/shopcore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2330 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1/pyshop/shopcore/command_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    24862 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1/pyshop/shopcore/model_builder.py
--rw-rw-rw-   0 root         (0) root         (0)    12969 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1/pyshop/shopcore/script_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    14831 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1/pyshop/shopcore/shop_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1611 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1/pyshop/shopcore/shop_rest.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 12:43:47.810413 sintef-pyshop-1.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1882 2023-06-07 13:27:40.000000 sintef-pyshop-1.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:43:47.807413 sintef-pyshop-1.4.1/sintef_pyshop.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6010 2023-06-12 12:43:47.000000 sintef-pyshop-1.4.1/sintef_pyshop.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      790 2023-06-12 12:43:47.000000 sintef-pyshop-1.4.1/sintef_pyshop.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 12:43:47.000000 sintef-pyshop-1.4.1/sintef_pyshop.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-12 12:43:47.000000 sintef-pyshop-1.4.1/sintef_pyshop.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-12 12:43:47.000000 sintef-pyshop-1.4.1/sintef_pyshop.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:43:47.809413 sintef-pyshop-1.4.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)      724 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1/tests/test_helpers_command.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1/tests/test_helpers_time.py
--rw-rw-rw-   0 root         (0) root         (0)     7580 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1/tests/test_shop_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.775214 sintef-pyshop-1.4.1a0/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5299 2023-06-06 15:06:22.775214 sintef-pyshop-1.4.1a0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4239 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.763214 sintef-pyshop-1.4.1a0/pyshop/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/pyshop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.764214 sintef-pyshop-1.4.1a0/pyshop/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/pyshop/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/pyshop/helpers/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-05-10 06:30:20.000000 sintef-pyshop-1.4.1a0/pyshop/helpers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     5040 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/helpers/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/helpers/typing_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.766214 sintef-pyshop-1.4.1a0/pyshop/lp_model/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/lp_model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/lp_model/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     2555 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/lp_model/lp_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    10661 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/lp_model/row.py
+-rw-rw-rw-   0 root         (0) root         (0)     9366 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/lp_model/var.py
+-rw-rw-rw-   0 root         (0) root         (0)    13751 2023-06-06 09:55:12.000000 sintef-pyshop-1.4.1a0/pyshop/shop_runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.770214 sintef-pyshop-1.4.1a0/pyshop/shopcore/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2330 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/command_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    24862 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/model_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    12969 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/script_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    14831 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/shop_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/pyshop/shopcore/shop_rest.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 15:06:22.775214 sintef-pyshop-1.4.1a0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1859 2023-06-06 15:06:11.000000 sintef-pyshop-1.4.1a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.772214 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5299 2023-06-06 15:06:22.000000 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      790 2023-06-06 15:06:22.000000 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 15:06:22.000000 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-06 15:06:22.000000 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-06 15:06:22.000000 sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:06:22.774214 sintef-pyshop-1.4.1a0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      724 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/tests/test_helpers_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/tests/test_helpers_time.py
+-rw-rw-rw-   0 root         (0) root         (0)     7580 2023-05-10 06:30:21.000000 sintef-pyshop-1.4.1a0/tests/test_shop_api.py
```

### Comparing `sintef-pyshop-1.4.1/LICENSE` & `sintef-pyshop-1.4.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/PKG-INFO` & `sintef-pyshop-1.4.1a0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sintef-pyshop
-Version: 1.4.1
+Version: 1.4.1a0
 Summary: Python interface to SHOP
 Home-page: http://www.sintef.no/programvare/SHOP
 Author: SINTEF Energy Research
 Author-email: support.energy@sintef.no
 License: MIT
 Project-URL: Documentation, https://shop.sintef.energy/documentation/tutorials/pyshop/
 Project-URL: Source, https://gitlab.sintef.no/energy/shop/pyshop
@@ -21,71 +21,52 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyshop
-
 Status:
 
-[![Latest Release](https://gitlab.sintef.no/energy/shop/pyshop/-/badges/release.svg)](https://gitlab.sintef.no/energy/shop/pyshop/-/releases)
-[![build status](https://gitlab.sintef.no/energy/shop/pyshop/badges/main/pipeline.svg?key_text=main)](https://gitlab.sintef.no/energy/shop/pyshop/-/commits/main)
-[![coverage report](https://gitlab.sintef.no/energy/shop/pyshop/badges/main/coverage.svg)](https://gitlab.sintef.no/energy/shop/pyshop/-/commits/main)
+[![CI](https://github.com/sintef-energy/pyshop/actions/workflows/pytest.yml/badge.svg)](https://github.com/sintef-energy/pyshop/actions/workflows/pytest.yml)
+[![codecov](https://codecov.io/gh/sintef-energy/pyshop/branch/main/graph/badge.svg?token=FYASF5O90D)](https://codecov.io/gh/sintef-energy/pyshop/branch/main/)
 
 The nicest python interface to SHOP!
 
 SHOP (Short-term Hydro Operation Planning) is a modeling tool for short-term hydro operation planning developed by SINTEF Energy Research in Trondheim, Norway. SHOP is used for both scientific and commerical purposes, please visit the [SHOP home page](https://www.sintef.no/en/software/shop/) for further information and inquiries regarding access and use.
 
 The pyshop package is an open source python wrapper for SHOP, and requires the proper SHOP binaries to function (see step 2).
 
 ## 1 Installing pyshop
-
-We currently offer two ways to use pyshop:
-
-1. Install pyshop through pypi (simple and quick)
-2. Install pyshop through Sintef's Gitlab Package Registry (useful if you want to avoid public registries)
-
-### Install pyshop using pypi
-
 The pyshop package can be installed using pip, the package installer for python. Please visit the [pip home page](https://pip.pypa.io/en/stable/) for installation and any pip related issues. You can install the official pyshop release through the terminal command:
 
 `pip install sintef-pyshop`
 
 You can also clone this repository and install the latest development version. To do this, open a terminal in the cloned pyshop directory and give the command:
 
 `pip install .`
 
 You should now see pyshop appear in the list of installed python modules when typing:
 
 `pip list`
 
-### Install pyshop using Gitlab Package Registry
-
-Create a [personal access token.](https://gitlab.sintef.no/help/user/profile/personal_access_tokens)
-
-Run the command below with your personal access token:
-`pip install sintef-pyshop --index-url https://__token__:<your_personal_token>@gitlab.sintef.no/api/v4/projects/4012/packages/pypi/simple`
-
-## 2 Download the desired SHOP binaries for your system
+## 2 Download the desired SHOP binaries for your system 
 
 > NOTE: You may not distribute the cplex library as it requires end user license
 
 The SHOP core is separate from the pyshop package, and must be downloaded separately. The latest SHOP binaries are found on the [SHOP Portal](https://shop.sintef.energy/files/). Access to the portal must be granted by SINTEF Energy Research.
 
 The following binaries are required for pyshop to run:
 
 Windows:
-
 - cplex2010.dll
 - shop_cplex_interface.dll
 - shop_pybind.pyd
 
 Linux:
-
 - libcplex2010.so
 - shop_cplex_interface.so
 - shop_pybind.so
 
 The solver specific binary is listed as cplex2010 here, but will change as new CPLEX versions become available. It is also possible to use the GUROBI and OSI solvers with SHOP. Note that the shop_cplex_interface.so used to contain the CPLEX binaries in the Linux distribution before SHOP version 14.3, and so older SHOP versions do not require the separate libcplex2010.so file.
 
 ## 3 Environment and license file
@@ -95,17 +76,17 @@
 The `ICC_COMMAND_PATH` is also the default place pyshop will look for the SHOP binaries mentioned in step 2. If the binaries are placed elsewhere, the keyword argument `solver_path` must be used when a ShopSession instance is created to ensure the correct binaries are loaded. Note that SHOP versions older than 14.4.0.5 reqiuire libcplex2010.so to be placed in the '/lib' directory when running pyshop in a Linux environment. From version 14.4.0.5, the libcplex2010.so can be placed in the same directory as the other SHOP bionaries.
 
 ## 4 Running SHOP
 
 Now that pyshop is installed, the SHOP binaries are downloaded, and the license file and binary paths are located, it is possible to run SHOP in python using pyshop:
 
     import pyshop as pys
-
+    
     shop = pys.ShopSession(license_path="C:/License/File/Path", solver_path="C:/SHOP/versions/14")
-
+    
     #Set time resolution
     #Build topolgy
     #Add temporal input
     #Run model
     #Retreive results
 
 Please visit the SHOP Portal for a detailed [tutorial](https://shop.sintef.energy/documentation/tutorials/pyshop/) and several [examples](https://shop.sintef.energy/documentation/examples/) using pyshop.
```

### Comparing `sintef-pyshop-1.4.1/README.md` & `sintef-pyshop-1.4.1a0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,46 @@
 # pyshop
-
 Status:
 
-[![Latest Release](https://gitlab.sintef.no/energy/shop/pyshop/-/badges/release.svg)](https://gitlab.sintef.no/energy/shop/pyshop/-/releases)
-[![build status](https://gitlab.sintef.no/energy/shop/pyshop/badges/main/pipeline.svg?key_text=main)](https://gitlab.sintef.no/energy/shop/pyshop/-/commits/main)
-[![coverage report](https://gitlab.sintef.no/energy/shop/pyshop/badges/main/coverage.svg)](https://gitlab.sintef.no/energy/shop/pyshop/-/commits/main)
+[![CI](https://github.com/sintef-energy/pyshop/actions/workflows/pytest.yml/badge.svg)](https://github.com/sintef-energy/pyshop/actions/workflows/pytest.yml)
+[![codecov](https://codecov.io/gh/sintef-energy/pyshop/branch/main/graph/badge.svg?token=FYASF5O90D)](https://codecov.io/gh/sintef-energy/pyshop/branch/main/)
 
 The nicest python interface to SHOP!
 
 SHOP (Short-term Hydro Operation Planning) is a modeling tool for short-term hydro operation planning developed by SINTEF Energy Research in Trondheim, Norway. SHOP is used for both scientific and commerical purposes, please visit the [SHOP home page](https://www.sintef.no/en/software/shop/) for further information and inquiries regarding access and use.
 
 The pyshop package is an open source python wrapper for SHOP, and requires the proper SHOP binaries to function (see step 2).
 
 ## 1 Installing pyshop
-
-We currently offer two ways to use pyshop:
-
-1. Install pyshop through pypi (simple and quick)
-2. Install pyshop through Sintef's Gitlab Package Registry (useful if you want to avoid public registries)
-
-### Install pyshop using pypi
-
 The pyshop package can be installed using pip, the package installer for python. Please visit the [pip home page](https://pip.pypa.io/en/stable/) for installation and any pip related issues. You can install the official pyshop release through the terminal command:
 
 `pip install sintef-pyshop`
 
 You can also clone this repository and install the latest development version. To do this, open a terminal in the cloned pyshop directory and give the command:
 
 `pip install .`
 
 You should now see pyshop appear in the list of installed python modules when typing:
 
 `pip list`
 
-### Install pyshop using Gitlab Package Registry
-
-Create a [personal access token.](https://gitlab.sintef.no/help/user/profile/personal_access_tokens)
-
-Run the command below with your personal access token:
-`pip install sintef-pyshop --index-url https://__token__:<your_personal_token>@gitlab.sintef.no/api/v4/projects/4012/packages/pypi/simple`
-
-## 2 Download the desired SHOP binaries for your system
+## 2 Download the desired SHOP binaries for your system 
 
 > NOTE: You may not distribute the cplex library as it requires end user license
 
 The SHOP core is separate from the pyshop package, and must be downloaded separately. The latest SHOP binaries are found on the [SHOP Portal](https://shop.sintef.energy/files/). Access to the portal must be granted by SINTEF Energy Research.
 
 The following binaries are required for pyshop to run:
 
 Windows:
-
 - cplex2010.dll
 - shop_cplex_interface.dll
 - shop_pybind.pyd
 
 Linux:
-
 - libcplex2010.so
 - shop_cplex_interface.so
 - shop_pybind.so
 
 The solver specific binary is listed as cplex2010 here, but will change as new CPLEX versions become available. It is also possible to use the GUROBI and OSI solvers with SHOP. Note that the shop_cplex_interface.so used to contain the CPLEX binaries in the Linux distribution before SHOP version 14.3, and so older SHOP versions do not require the separate libcplex2010.so file.
 
 ## 3 Environment and license file
@@ -69,17 +50,17 @@
 The `ICC_COMMAND_PATH` is also the default place pyshop will look for the SHOP binaries mentioned in step 2. If the binaries are placed elsewhere, the keyword argument `solver_path` must be used when a ShopSession instance is created to ensure the correct binaries are loaded. Note that SHOP versions older than 14.4.0.5 reqiuire libcplex2010.so to be placed in the '/lib' directory when running pyshop in a Linux environment. From version 14.4.0.5, the libcplex2010.so can be placed in the same directory as the other SHOP bionaries.
 
 ## 4 Running SHOP
 
 Now that pyshop is installed, the SHOP binaries are downloaded, and the license file and binary paths are located, it is possible to run SHOP in python using pyshop:
 
     import pyshop as pys
-
+    
     shop = pys.ShopSession(license_path="C:/License/File/Path", solver_path="C:/SHOP/versions/14")
-
+    
     #Set time resolution
     #Build topolgy
     #Add temporal input
     #Run model
     #Retreive results
 
 Please visit the SHOP Portal for a detailed [tutorial](https://shop.sintef.energy/documentation/tutorials/pyshop/) and several [examples](https://shop.sintef.energy/documentation/examples/) using pyshop.
```

### Comparing `sintef-pyshop-1.4.1/pyshop/helpers/commands.py` & `sintef-pyshop-1.4.1a0/pyshop/helpers/commands.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/pyshop/helpers/time.py` & `sintef-pyshop-1.4.1a0/pyshop/helpers/time.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/pyshop/helpers/timeseries.py` & `sintef-pyshop-1.4.1a0/pyshop/helpers/timeseries.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/pyshop/helpers/typing_annotations.py` & `sintef-pyshop-1.4.1a0/pyshop/helpers/typing_annotations.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/pyshop/lp_model/index.py` & `sintef-pyshop-1.4.1a0/pyshop/lp_model/index.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/pyshop/lp_model/lp_model.py` & `sintef-pyshop-1.4.1a0/pyshop/lp_model/lp_model.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/pyshop/lp_model/row.py` & `sintef-pyshop-1.4.1a0/pyshop/lp_model/row.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/pyshop/lp_model/var.py` & `sintef-pyshop-1.4.1a0/pyshop/lp_model/var.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/pyshop/shop_runner.py` & `sintef-pyshop-1.4.1a0/pyshop/shop_runner.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/pyshop/shopcore/command_builder.py` & `sintef-pyshop-1.4.1a0/pyshop/shopcore/command_builder.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/pyshop/shopcore/model_builder.py` & `sintef-pyshop-1.4.1a0/pyshop/shopcore/model_builder.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/pyshop/shopcore/script_generator.py` & `sintef-pyshop-1.4.1a0/pyshop/shopcore/script_generator.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/pyshop/shopcore/shop_api.py` & `sintef-pyshop-1.4.1a0/pyshop/shopcore/shop_api.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/pyshop/shopcore/shop_rest.py` & `sintef-pyshop-1.4.1a0/pyshop/shopcore/shop_rest.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/setup.py` & `sintef-pyshop-1.4.1a0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import os
 import pathlib
 from distutils.core import setup
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(name='sintef-pyshop',
-      version=os.getenv('CI_COMMIT_TAG'),
+      version='1.4.1-alpha',
       author='SINTEF Energy Research',
       description='Python interface to SHOP',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages=['pyshop',
                 'pyshop.helpers',
                 'pyshop.shopcore',
```

### Comparing `sintef-pyshop-1.4.1/sintef_pyshop.egg-info/PKG-INFO` & `sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sintef-pyshop
-Version: 1.4.1
+Version: 1.4.1a0
 Summary: Python interface to SHOP
 Home-page: http://www.sintef.no/programvare/SHOP
 Author: SINTEF Energy Research
 Author-email: support.energy@sintef.no
 License: MIT
 Project-URL: Documentation, https://shop.sintef.energy/documentation/tutorials/pyshop/
 Project-URL: Source, https://gitlab.sintef.no/energy/shop/pyshop
@@ -21,71 +21,52 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyshop
-
 Status:
 
-[![Latest Release](https://gitlab.sintef.no/energy/shop/pyshop/-/badges/release.svg)](https://gitlab.sintef.no/energy/shop/pyshop/-/releases)
-[![build status](https://gitlab.sintef.no/energy/shop/pyshop/badges/main/pipeline.svg?key_text=main)](https://gitlab.sintef.no/energy/shop/pyshop/-/commits/main)
-[![coverage report](https://gitlab.sintef.no/energy/shop/pyshop/badges/main/coverage.svg)](https://gitlab.sintef.no/energy/shop/pyshop/-/commits/main)
+[![CI](https://github.com/sintef-energy/pyshop/actions/workflows/pytest.yml/badge.svg)](https://github.com/sintef-energy/pyshop/actions/workflows/pytest.yml)
+[![codecov](https://codecov.io/gh/sintef-energy/pyshop/branch/main/graph/badge.svg?token=FYASF5O90D)](https://codecov.io/gh/sintef-energy/pyshop/branch/main/)
 
 The nicest python interface to SHOP!
 
 SHOP (Short-term Hydro Operation Planning) is a modeling tool for short-term hydro operation planning developed by SINTEF Energy Research in Trondheim, Norway. SHOP is used for both scientific and commerical purposes, please visit the [SHOP home page](https://www.sintef.no/en/software/shop/) for further information and inquiries regarding access and use.
 
 The pyshop package is an open source python wrapper for SHOP, and requires the proper SHOP binaries to function (see step 2).
 
 ## 1 Installing pyshop
-
-We currently offer two ways to use pyshop:
-
-1. Install pyshop through pypi (simple and quick)
-2. Install pyshop through Sintef's Gitlab Package Registry (useful if you want to avoid public registries)
-
-### Install pyshop using pypi
-
 The pyshop package can be installed using pip, the package installer for python. Please visit the [pip home page](https://pip.pypa.io/en/stable/) for installation and any pip related issues. You can install the official pyshop release through the terminal command:
 
 `pip install sintef-pyshop`
 
 You can also clone this repository and install the latest development version. To do this, open a terminal in the cloned pyshop directory and give the command:
 
 `pip install .`
 
 You should now see pyshop appear in the list of installed python modules when typing:
 
 `pip list`
 
-### Install pyshop using Gitlab Package Registry
-
-Create a [personal access token.](https://gitlab.sintef.no/help/user/profile/personal_access_tokens)
-
-Run the command below with your personal access token:
-`pip install sintef-pyshop --index-url https://__token__:<your_personal_token>@gitlab.sintef.no/api/v4/projects/4012/packages/pypi/simple`
-
-## 2 Download the desired SHOP binaries for your system
+## 2 Download the desired SHOP binaries for your system 
 
 > NOTE: You may not distribute the cplex library as it requires end user license
 
 The SHOP core is separate from the pyshop package, and must be downloaded separately. The latest SHOP binaries are found on the [SHOP Portal](https://shop.sintef.energy/files/). Access to the portal must be granted by SINTEF Energy Research.
 
 The following binaries are required for pyshop to run:
 
 Windows:
-
 - cplex2010.dll
 - shop_cplex_interface.dll
 - shop_pybind.pyd
 
 Linux:
-
 - libcplex2010.so
 - shop_cplex_interface.so
 - shop_pybind.so
 
 The solver specific binary is listed as cplex2010 here, but will change as new CPLEX versions become available. It is also possible to use the GUROBI and OSI solvers with SHOP. Note that the shop_cplex_interface.so used to contain the CPLEX binaries in the Linux distribution before SHOP version 14.3, and so older SHOP versions do not require the separate libcplex2010.so file.
 
 ## 3 Environment and license file
@@ -95,17 +76,17 @@
 The `ICC_COMMAND_PATH` is also the default place pyshop will look for the SHOP binaries mentioned in step 2. If the binaries are placed elsewhere, the keyword argument `solver_path` must be used when a ShopSession instance is created to ensure the correct binaries are loaded. Note that SHOP versions older than 14.4.0.5 reqiuire libcplex2010.so to be placed in the '/lib' directory when running pyshop in a Linux environment. From version 14.4.0.5, the libcplex2010.so can be placed in the same directory as the other SHOP bionaries.
 
 ## 4 Running SHOP
 
 Now that pyshop is installed, the SHOP binaries are downloaded, and the license file and binary paths are located, it is possible to run SHOP in python using pyshop:
 
     import pyshop as pys
-
+    
     shop = pys.ShopSession(license_path="C:/License/File/Path", solver_path="C:/SHOP/versions/14")
-
+    
     #Set time resolution
     #Build topolgy
     #Add temporal input
     #Run model
     #Retreive results
 
 Please visit the SHOP Portal for a detailed [tutorial](https://shop.sintef.energy/documentation/tutorials/pyshop/) and several [examples](https://shop.sintef.energy/documentation/examples/) using pyshop.
```

### Comparing `sintef-pyshop-1.4.1/sintef_pyshop.egg-info/SOURCES.txt` & `sintef-pyshop-1.4.1a0/sintef_pyshop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/tests/test_helpers_command.py` & `sintef-pyshop-1.4.1a0/tests/test_helpers_command.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/tests/test_helpers_time.py` & `sintef-pyshop-1.4.1a0/tests/test_helpers_time.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.4.1/tests/test_shop_api.py` & `sintef-pyshop-1.4.1a0/tests/test_shop_api.py`

 * *Files identical despite different names*

