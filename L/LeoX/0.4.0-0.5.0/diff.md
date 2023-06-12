# Comparing `tmp/LeoX-0.4.0.tar.gz` & `tmp/LeoX-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/LeoX-0.4.0.tar", last modified: Wed May  4 07:39:51 2022, max compression
+gzip compressed data, was "dist/LeoX-0.5.0.tar", last modified: Mon Jun 12 15:50:00 2023, max compression
```

## Comparing `LeoX-0.4.0.tar` & `LeoX-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxrwxr-x   0 padawan   (1000) padawan   (1000)        0 2022-05-04 07:39:51.000000 LeoX-0.4.0/
--rw-rw-r--   0 padawan   (1000) padawan   (1000)     1083 2022-01-04 18:51:48.000000 LeoX-0.4.0/LICENSE
--rw-rw-r--   0 padawan   (1000) padawan   (1000)     8717 2022-05-04 07:39:51.000000 LeoX-0.4.0/PKG-INFO
--rw-rw-r--   0 padawan   (1000) padawan   (1000)       38 2022-05-04 07:39:51.000000 LeoX-0.4.0/setup.cfg
-drwxrwxr-x   0 padawan   (1000) padawan   (1000)        0 2022-05-04 07:39:51.000000 LeoX-0.4.0/lx/
--rw-rw-r--   0 padawan   (1000) padawan   (1000)     7217 2022-05-04 07:26:59.000000 LeoX-0.4.0/lx/omega.py
--rw-rw-r--   0 padawan   (1000) padawan   (1000)    31248 2022-05-04 07:26:59.000000 LeoX-0.4.0/lx/tools.py
--rw-rw-r--   0 padawan   (1000) padawan   (1000)     7244 2022-05-04 07:26:59.000000 LeoX-0.4.0/lx/__main__.py
--rw-rw-r--   0 padawan   (1000) padawan   (1000)     2241 2022-05-04 07:26:59.000000 LeoX-0.4.0/lx/batch_lx.py
--rw-rw-r--   0 padawan   (1000) padawan   (1000)        0 2022-01-04 18:51:48.000000 LeoX-0.4.0/lx/__init__.py
--rw-rw-r--   0 padawan   (1000) padawan   (1000)    12058 2022-05-04 07:26:59.000000 LeoX-0.4.0/lx/conf_search.py
--rw-rw-r--   0 padawan   (1000) padawan   (1000)     8079 2022-05-04 07:26:59.000000 LeoX-0.4.0/lx/ld.py
--rw-rw-r--   0 padawan   (1000) padawan   (1000)       62 2022-05-04 07:26:59.000000 LeoX-0.4.0/lx/__version__.py
-drwxrwxr-x   0 padawan   (1000) padawan   (1000)        0 2022-05-04 07:39:51.000000 LeoX-0.4.0/LeoX.egg-info/
--rw-rw-r--   0 padawan   (1000) padawan   (1000)        3 2022-05-04 07:39:51.000000 LeoX-0.4.0/LeoX.egg-info/top_level.txt
--rw-rw-r--   0 padawan   (1000) padawan   (1000)     8717 2022-05-04 07:39:51.000000 LeoX-0.4.0/LeoX.egg-info/PKG-INFO
--rw-rw-r--   0 padawan   (1000) padawan   (1000)        1 2022-05-04 07:39:51.000000 LeoX-0.4.0/LeoX.egg-info/dependency_links.txt
--rw-rw-r--   0 padawan   (1000) padawan   (1000)       12 2022-05-04 07:39:51.000000 LeoX-0.4.0/LeoX.egg-info/requires.txt
--rw-rw-r--   0 padawan   (1000) padawan   (1000)      322 2022-05-04 07:39:51.000000 LeoX-0.4.0/LeoX.egg-info/SOURCES.txt
--rw-rw-r--   0 padawan   (1000) padawan   (1000)       41 2022-05-04 07:39:51.000000 LeoX-0.4.0/LeoX.egg-info/entry_points.txt
--rw-rw-r--   0 padawan   (1000) padawan   (1000)     3578 2022-05-04 07:26:59.000000 LeoX-0.4.0/setup.py
--rw-rw-r--   0 padawan   (1000) padawan   (1000)     8347 2022-05-04 07:26:59.000000 LeoX-0.4.0/README.md
--rw-rw-r--   0 padawan   (1000) padawan   (1000)       26 2022-01-04 18:51:48.000000 LeoX-0.4.0/MANIFEST.in
+drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:50:00.893678 LeoX-0.5.0/
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       62 2022-06-01 08:59:44.000000 LeoX-0.5.0/.gitignore
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     1083 2021-09-27 19:02:46.000000 LeoX-0.5.0/LICENSE
+drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:50:00.665677 LeoX-0.5.0/LeoX.egg-info/
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     9626 2023-06-12 15:49:59.000000 LeoX-0.5.0/LeoX.egg-info/PKG-INFO
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)      402 2023-06-12 15:49:59.000000 LeoX-0.5.0/LeoX.egg-info/SOURCES.txt
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)        1 2023-06-12 15:49:59.000000 LeoX-0.5.0/LeoX.egg-info/dependency_links.txt
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       41 2023-06-12 15:49:59.000000 LeoX-0.5.0/LeoX.egg-info/entry_points.txt
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       19 2023-06-12 15:49:59.000000 LeoX-0.5.0/LeoX.egg-info/requires.txt
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)        3 2023-06-12 15:49:59.000000 LeoX-0.5.0/LeoX.egg-info/top_level.txt
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       26 2021-09-27 19:02:46.000000 LeoX-0.5.0/MANIFEST.in
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     9626 2023-06-12 15:50:00.892678 LeoX-0.5.0/PKG-INFO
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     8347 2022-06-01 08:59:44.000000 LeoX-0.5.0/README.md
+drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:50:00.672677 LeoX-0.5.0/batch_examples/
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)      174 2022-06-01 08:59:44.000000 LeoX-0.5.0/batch_examples/batch.sh
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)      326 2021-10-13 13:55:43.000000 LeoX-0.5.0/batch_examples/slurm.sh
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)      206 2022-06-01 08:59:44.000000 LeoX-0.5.0/batch_examples/ts.sh
+drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:50:00.888678 LeoX-0.5.0/lx/
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)        0 2021-09-27 19:02:46.000000 LeoX-0.5.0/lx/__init__.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     7484 2023-06-12 15:49:39.000000 LeoX-0.5.0/lx/__main__.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       62 2023-06-12 15:49:39.000000 LeoX-0.5.0/lx/__version__.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     2241 2022-06-01 08:59:44.000000 LeoX-0.5.0/lx/batch_lx.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)    11444 2023-06-12 15:49:39.000000 LeoX-0.5.0/lx/conf_search.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     8053 2023-05-03 15:29:51.000000 LeoX-0.5.0/lx/ld.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     7217 2022-06-01 08:59:44.000000 LeoX-0.5.0/lx/omega.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)    32940 2023-06-12 15:49:39.000000 LeoX-0.5.0/lx/tools.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       38 2023-06-12 15:50:00.894678 LeoX-0.5.0/setup.cfg
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     3588 2023-06-12 15:49:39.000000 LeoX-0.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `LeoX-0.4.0/LICENSE` & `LeoX-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LeoX-0.4.0/PKG-INFO` & `LeoX-0.5.0/LeoX.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,133 +1,130 @@
 Metadata-Version: 2.1
 Name: LeoX
-Version: 0.4.0
+Version: 0.5.0
 Summary: Spectrum simulations with TD(A)-DFT
 Home-page: https://github.com/LeonardoESousa/LeoX
 Author: Leonardo Evaristo de Sousa
 Author-email: leonardo.sousa137@gmail.com
 License: MIT
+Description: 
+        ﻿# LeoX - Light emission and exciton diffusion in organic molecules 
+        
+        [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+        [![license](https://img.shields.io/github/license/LeonardoESousa/LeoX?style=plastic)]()
+        [![down](https://img.shields.io/pypi/dm/LeoX)]()
+        [![maint](https://img.shields.io/maintenance/yes/2021)]()
+        [![commit](https://img.shields.io/github/last-commit/LeonardoESousa/LeoX?style=plastic)]()
+        
+        
+        
+        A package for absorption and fluorescence spectrum simulations using the nuclear ensemble method along with TD(A)-DFT. Estimation of singlet exciton properties (Förster radius, lifetime, diffusion length). Long-range separation parameter tuning. Stochastic conformational search.  Interfaces with the Gaussian (09 or 16) package.
+        
+        
+        Table of Contents
+        =================
+        <!--ts-->
+        * [Cite as:](#cite-as)
+        * [What does this program do?](#what-does-this-program-do)
+        * [What is necessary to use it?](#what-is-necessary-to-use-it)
+        * [How to install it?](#how-to-install-it)
+        * [How to use it?](#how-to-use-it)
+           
+        <!--te-->
+        
+        ## Cite as:
+        
+        > de Sousa, L. E., Bueno, F. T., e Silva, G. M., da Silva Filho, D. A., & de Oliveira Neto, P. H. (2019). Fast predictions of exciton diffusion length in organic materials. Journal of Materials Chemistry C, 7(14), 4066-4071.
+        
+        
+        ## What does this program do?
+        
+        1.  Spectrum simulation:
+            - Calculates Absorption and Fluorescence spectrum simulations using TD(A)-DFT.
+            - Calculations include vibrational contributions to the spectra. 
+            - Optionally, they may also include solvent effects either by PCM or by a state specific solvation model.
+        2.  Exciton properties:   
+            - Calculates Förster radius for transfers between two molecules of equal or different type.
+            - Calculates fluorescence lifetimes.
+            - Calculates singlet exciton diffusion lengths.
+        3.  Extra features:
+            - Tunes the w parameter of long-range separated functionals.
+            - Extracts last geometry from Gaussian log file.
+            - Runs a stochastic coformational search algorithm.
+        
+        
+        ## What is necessary to use it?
+        
+         -  The program requires that the Gaussian quantum chemistry software (G09 or G16) be installed, as it interfaces with it.
+        
+        -   The first step for running spectrum calculations or conformational searches is providing a Gaussian log file for a frequency calculation in the S0 state, if the goal is computing an absorption spectrum, or S1 state, if the objective is calculating a fluoresence spectrum. All frequencies must be real.  
+        
+        -   To obtain estimates for Förster radius, fluorescence lifetimes and singlet exciton diffusion lengths, it is necessary to first perform both absorption and emission spectra calculations for the molecule of interest.
+        
+        ## How to install it?
+        
+        Run:
+        
+        `pip install LeoX`
+        
+        Alternatively, clone the repository to your computer. Inside the LeoX folder, run:
+        
+        `pip install .`
+        
+        Depending on the operating system, the commands above may need to be replace by
+        
+        `pip3 install LeoX` or `pip3 install .`
+        
+        Once installed, you should be able to run the program from any folder by just using the `lx` command.
+        
+        ## How to use it?
+        
+        1. For spectrum simulations:
+        
+            - Create a folder for your project. Add the log file for the frequency calculation to your folder. Run the lx command. Choose option 1 and follow the instructions to select the parameters of the calculation.
+            - Add a bash script file to the folder to control execution. This file depends on which batch system you use. Examples for users of slurm or task spooler (ts) are presented [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples).
+            - Run the `lx` command again, choose option 2 and follow the instructions. Once the calculations are running, you may use option 4 to check the progress or option 9 to abort.
+            <img width="575" alt="LeoX1" src="https://user-images.githubusercontent.com/94139072/144780278-ef3b8ced-af82-4a9d-a8a5-667ebdcbdd71.png">
+        
+            - Once all calculations are done, run the `lx` command and choose option 3. Follow the instructions to set the parameters and the spectrum will be generated.
+            <img width="436" alt="LeoX2" src="https://user-images.githubusercontent.com/94139072/144780487-7d0a5800-c925-4dbc-8b88-041b6d7f35b3.png">
+            
+            - After the spectrum is generated, a file with the extension .lx will be created. For absorption spectra, the file will be named "cross_section.lx", whereas for fluorescence spectra, the file will be named "differential_rate.lx"
+            - It is possible to generate a spectrum with partially concluded calculations. Option 3 can be used multiple times without overwriting the previously generated spectrum. Each time a spectrum is generated, it will have a number at the beginning of the file name, such as "2cross_section.lx".
+            - Each spectrum file is expected to have three columns as indicated below, where the third column can be used to estimate if the amount of sampled geometries are enough for accurate spectrum simulation.
+            <img width="380" alt="LeoX3" src="https://user-images.githubusercontent.com/94139072/144781496-a7c1e1cc-56ea-4de4-85bd-6a0e7ed37d7e.png">
+        
+        
+        2. For exciton properties:
+        
+            - For exciton properties, you must first calculate the fluorescence and absorption spectra of the donor and acceptor molecules of interest to you. 
+            - Once this is done, copy the spectra to a folder and inside this folder run the `lx` command. Choose option 5. Follow the instructions to set the calculation parameters, exemplified below.  
+            <img width="450" alt="LeoX4" src="https://user-images.githubusercontent.com/94139072/144785795-70dec39b-c63d-41a7-9613-fcf4cd1c244f.png">
+           
+            - The correction for short distances takes into account the transition dipole moment of the donor molecule, extracted directly from the Gaussian log. Details can be obtained in the indicated published paper.
+            - A file called `ld.lx` will be generated with all the information.
+            <img width="450" alt="Captura de Tela 2021-12-06 às 01 13 13" src="https://user-images.githubusercontent.com/94139072/144786165-547a9a2e-cca3-434a-90a7-82c610d97d7e.png">
+        
+        
+            - Importantly, diffusion length estimates are only sensible if donor and acceptor molecules are of the same kind. To calculate the Förster radius for transfers between different molecules, you must provide the fluorescence spectrum of the donor molecule and the absorption spectrum of the acceptor molecule. The fluorescence lifetime shown will correspond to that of the donor molecule.  
+        
+        4. For conformational searches:
+            
+            - Create a folder. Add a frequency Gaussian .log file. Include also a bash script file according to your batch system (follow examples for slurm and task spooler [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples)). 
+            - Run the `lx` command in the folder and choose option 6. Follow the instructions to set the calculation parameters. 
+            - Answer the queries to determine the parameters of the conformational search (level of theory, initial temperature, temperature step, number of rounds, number of sampled geometries at each round). 
+            - Once the search starts running, the file conformation.lx will show the conformations found thus far, along with the average energies and Boltzmann populations at 300 K of each. 
+            - After the search is over, a folder named Conformers is created with the geometries of each conformer written to a gaussian input file that can be used for further optimization. 
+        
+        3. For range separation parameter tuning:
+        
+            - Create a folder. Add either a Gaussian .log file or .com file (for any kind of calculation). Include also a bash script file according to your batch system (follow examples for slurm and task spooler [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples)). 
+            - Run the `lx` command in the folder and choose option 7. Follow the instructions to set the calculation parameters. 
+            - You may choose between a relaxed on unrelaxed tuning procedure. In the case of the former, geometry optimizations are run for each range separation parameter value. In the case of unrelaxed tuning, the geometry provided in the .log or .com file will be used for all calculations. 
+         
+        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-﻿# LeoX - Light emission and exciton diffusion in organic molecules 
-
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-[![license](https://img.shields.io/github/license/LeonardoESousa/LeoX?style=plastic)]()
-[![down](https://img.shields.io/pypi/dm/LeoX)]()
-[![maint](https://img.shields.io/maintenance/yes/2021)]()
-[![commit](https://img.shields.io/github/last-commit/LeonardoESousa/LeoX?style=plastic)]()
-
-
-
-A package for absorption and fluorescence spectrum simulations using the nuclear ensemble method along with TD(A)-DFT. Estimation of singlet exciton properties (Förster radius, lifetime, diffusion length). Long-range separation parameter tuning. Stochastic conformational search.  Interfaces with the Gaussian (09 or 16) package.
-
-
-Table of Contents
-=================
-<!--ts-->
-* [Cite as:](#cite-as)
-* [What does this program do?](#what-does-this-program-do)
-* [What is necessary to use it?](#what-is-necessary-to-use-it)
-* [How to install it?](#how-to-install-it)
-* [How to use it?](#how-to-use-it)
-   
-<!--te-->
-
-## Cite as:
-
-> de Sousa, L. E., Bueno, F. T., e Silva, G. M., da Silva Filho, D. A., & de Oliveira Neto, P. H. (2019). Fast predictions of exciton diffusion length in organic materials. Journal of Materials Chemistry C, 7(14), 4066-4071.
-
-
-## What does this program do?
-
-1.  Spectrum simulation:
-    - Calculates Absorption and Fluorescence spectrum simulations using TD(A)-DFT.
-    - Calculations include vibrational contributions to the spectra. 
-    - Optionally, they may also include solvent effects either by PCM or by a state specific solvation model.
-2.  Exciton properties:   
-    - Calculates Förster radius for transfers between two molecules of equal or different type.
-    - Calculates fluorescence lifetimes.
-    - Calculates singlet exciton diffusion lengths.
-3.  Extra features:
-    - Tunes the w parameter of long-range separated functionals.
-    - Extracts last geometry from Gaussian log file.
-    - Runs a stochastic coformational search algorithm.
-
-
-## What is necessary to use it?
-
- -  The program requires that the Gaussian quantum chemistry software (G09 or G16) be installed, as it interfaces with it.
-
--   The first step for running spectrum calculations or conformational searches is providing a Gaussian log file for a frequency calculation in the S0 state, if the goal is computing an absorption spectrum, or S1 state, if the objective is calculating a fluoresence spectrum. All frequencies must be real.  
-
--   To obtain estimates for Förster radius, fluorescence lifetimes and singlet exciton diffusion lengths, it is necessary to first perform both absorption and emission spectra calculations for the molecule of interest.
-
-## How to install it?
-
-Run:
-
-`pip install LeoX`
-
-Alternatively, clone the repository to your computer. Inside the LeoX folder, run:
-
-`pip install .`
-
-Depending on the operating system, the commands above may need to be replace by
-
-`pip3 install LeoX` or `pip3 install .`
-
-Once installed, you should be able to run the program from any folder by just using the `lx` command.
-
-## How to use it?
-
-1. For spectrum simulations:
-
-    - Create a folder for your project. Add the log file for the frequency calculation to your folder. Run the lx command. Choose option 1 and follow the instructions to select the parameters of the calculation.
-    - Add a bash script file to the folder to control execution. This file depends on which batch system you use. Examples for users of slurm or task spooler (ts) are presented [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples).
-    - Run the `lx` command again, choose option 2 and follow the instructions. Once the calculations are running, you may use option 4 to check the progress or option 9 to abort.
-    <img width="575" alt="LeoX1" src="https://user-images.githubusercontent.com/94139072/144780278-ef3b8ced-af82-4a9d-a8a5-667ebdcbdd71.png">
-
-    - Once all calculations are done, run the `lx` command and choose option 3. Follow the instructions to set the parameters and the spectrum will be generated.
-    <img width="436" alt="LeoX2" src="https://user-images.githubusercontent.com/94139072/144780487-7d0a5800-c925-4dbc-8b88-041b6d7f35b3.png">
-    
-    - After the spectrum is generated, a file with the extension .lx will be created. For absorption spectra, the file will be named "cross_section.lx", whereas for fluorescence spectra, the file will be named "differential_rate.lx"
-    - It is possible to generate a spectrum with partially concluded calculations. Option 3 can be used multiple times without overwriting the previously generated spectrum. Each time a spectrum is generated, it will have a number at the beginning of the file name, such as "2cross_section.lx".
-    - Each spectrum file is expected to have three columns as indicated below, where the third column can be used to estimate if the amount of sampled geometries are enough for accurate spectrum simulation.
-    <img width="380" alt="LeoX3" src="https://user-images.githubusercontent.com/94139072/144781496-a7c1e1cc-56ea-4de4-85bd-6a0e7ed37d7e.png">
-
-
-2. For exciton properties:
-
-    - For exciton properties, you must first calculate the fluorescence and absorption spectra of the donor and acceptor molecules of interest to you. 
-    - Once this is done, copy the spectra to a folder and inside this folder run the `lx` command. Choose option 5. Follow the instructions to set the calculation parameters, exemplified below.  
-    <img width="450" alt="LeoX4" src="https://user-images.githubusercontent.com/94139072/144785795-70dec39b-c63d-41a7-9613-fcf4cd1c244f.png">
-   
-    - The correction for short distances takes into account the transition dipole moment of the donor molecule, extracted directly from the Gaussian log. Details can be obtained in the indicated published paper.
-    - A file called `ld.lx` will be generated with all the information.
-    <img width="450" alt="Captura de Tela 2021-12-06 às 01 13 13" src="https://user-images.githubusercontent.com/94139072/144786165-547a9a2e-cca3-434a-90a7-82c610d97d7e.png">
-
-
-    - Importantly, diffusion length estimates are only sensible if donor and acceptor molecules are of the same kind. To calculate the Förster radius for transfers between different molecules, you must provide the fluorescence spectrum of the donor molecule and the absorption spectrum of the acceptor molecule. The fluorescence lifetime shown will correspond to that of the donor molecule.  
-
-4. For conformational searches:
-    
-    - Create a folder. Add a frequency Gaussian .log file. Include also a bash script file according to your batch system (follow examples for slurm and task spooler [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples)). 
-    - Run the `lx` command in the folder and choose option 6. Follow the instructions to set the calculation parameters. 
-    - Answer the queries to determine the parameters of the conformational search (level of theory, initial temperature, temperature step, number of rounds, number of sampled geometries at each round). 
-    - Once the search starts running, the file conformation.lx will show the conformations found thus far, along with the average energies and Boltzmann populations at 300 K of each. 
-    - After the search is over, a folder named Conformers is created with the geometries of each conformer written to a gaussian input file that can be used for further optimization. 
-
-3. For range separation parameter tuning:
-
-    - Create a folder. Add either a Gaussian .log file or .com file (for any kind of calculation). Include also a bash script file according to your batch system (follow examples for slurm and task spooler [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples)). 
-    - Run the `lx` command in the folder and choose option 7. Follow the instructions to set the calculation parameters. 
-    - You may choose between a relaxed on unrelaxed tuning procedure. In the case of the former, geometry optimizations are run for each range separation parameter value. In the case of unrelaxed tuning, the geometry provided in the .log or .com file will be used for all calculations. 
- 
-
-
```

### Comparing `LeoX-0.4.0/lx/omega.py` & `LeoX-0.5.0/lx/omega.py`

 * *Files identical despite different names*

### Comparing `LeoX-0.4.0/lx/tools.py` & `LeoX-0.5.0/lx/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 import numpy as np
 import os
 import sys
 from scipy.stats import norm
 import time
 import subprocess
+import pandas as pd
 
 ##SOME CONSTANTS##############################################
 epsilon0 = 8.854187817e-12   #F/m
 hbar = 6.582119514e-16       #eV s
 hbar2 = 1.054571800e-34      #J s
 mass = 9.10938356e-31        #kg
 c = 299792458                #m/s
@@ -249,28 +250,42 @@
     try:
         os.mkdir('Geometries')
     except:
         pass        
     counter = start_counter()   
     print("\nGenerating geometries...\n")
     numbers, atomos, A = sample_geometries(freqlog,num_geoms,T)
-    with open('Magnitudes_{:.0f}K_.lx'.format(T), 'a') as file:
-        np.savetxt(file, numbers, delimiter='\t', fmt='%s')
+    F, M      = pega_freq(freqlog)
+    #convert numbers to dataframe
+    numbers = pd.DataFrame(numbers,columns=[f"mode_{i+1}" for i in range(np.shape(numbers)[1])])
+    #check if file exists
+    if os.path.isfile(f'Magnitudes_{T:.0f}K_.lx'):
+        data = pd.read_csv(f'Magnitudes_{T:.0f}K_.lx')
+        # get only columns with mode_ in the name
+        data = data.filter(regex='mode_')
+        #remove nan values
+        data = data.dropna()
+        # join data and numbers on axis 0
+        numbers = pd.concat([data,numbers],axis=0,ignore_index=True)
+    # concatenate frequencies and masses to numbers
+    numbers = pd.concat([pd.DataFrame(F,columns=['freq']),pd.DataFrame(M,columns=['mass']),numbers],axis=1)
+    numbers.to_csv(f'Magnitudes_{T:.0f}K_.lx',index=False)
     for n in range(0,np.shape(A)[1],3):
         Gfinal = A[:,n:n+3]  
         write_input(atomos,Gfinal,header.replace("UUUUU",str((n+3)//3)),bottom.replace("UUUUU",str((n+3)//3)),"Geometries/Geometry-"+str((n+3)//3+counter)+"-.com")
         progress = 100*((n+3)//3)/num_geoms
         text = "{:2.1f}%".format(progress)
         print(' ', text, "of the geometries done.",end="\r", flush=True)
     print("\n\nDone! Ready to run.")   
 ################################################################
             
 ##COLLECTS RESULTS############################################## 
 def gather_data(opc, tipo):
     files = [file for file in os.listdir('Geometries') if ".log" in file and "Geometr" in file ]    
+    files = [i for i in files if 'Normal termination' in open('Geometries/'+i, 'r').read()]
     files = sorted(files, key=lambda file: float(file.split("-")[1])) 
     with open("Samples.lx", 'w') as f:
         for file in files:
             num = file.split("-")[1]
             broadening = opc
             numeros, energies, fs, scfs = [], [], [], []
             corrected, total_corrected = -1, -1
@@ -334,64 +349,78 @@
             if new_arquivo in os.listdir('.'):
                 vers += 1
             else:
                 duplo = False
     return new_arquivo        
 ###############################################################
 
+##CALCULATES FLUORESCENCE LIFETIME IN S########################
+def calc_emi_rate(xd,yd,dyd):
+    #Integrates the emission spectrum
+    IntEmi = np.trapz(yd,xd)
+    taxa   = (1/hbar)*IntEmi
+    error  = (1/hbar)*np.sqrt(np.trapz((dyd**2),xd))
+    return taxa, error 
+###############################################################
+
 ##COMPUTES SPECTRA############################################# 
 def spectra(tipo, num_ex, nr):
     if tipo == "abs":
         constante = (np.pi*(e**2)*hbar)/(2*nr*mass*c*epsilon0)*10**(20)
     elif tipo == 'emi':
         constante = ((nr**2)*(e**2)/(2*np.pi*hbar*mass*(c**3)*epsilon0))
     V, O, S = [], [], []
     N = 0
     with open("Samples.lx", 'r') as f:
         for line in f:
             if "Geometry" in line:
                 N += 1
             elif "Excited State" in line and int(line.split()[2][:-1]) in num_ex:
                 line = line.split()
-                V.append(float(line[3]))
-                O.append(float(line[4]))
-                S.append(float(line[5]))
+                if float(line[3]) <= 0:
+                    print('Ignoring geom with negative vertical transition!')
+                    N -= 1
+                else: 
+                    V.append(float(line[3]))
+                    O.append(float(line[4]))
+                    S.append(float(line[5]))
     coms = start_counter()
     if len(V) == 0 or len(O) == 0:
         fatal_error("You need to run steps 1 and 2 first! Goodbye!")
     elif len(V) != coms*max(num_ex):
         print("Number of log files is less than the number of inputs. Something is not right! Computing the spectrum anyway...")
     V = np.array(V)
     O = np.array(O)
     S = np.array(S)
     if tipo == 'abs':
         espectro = (constante*O)
     else:
         espectro = (constante*(V**2)*O)
         tdm = calc_tdm(O,V)
-    x  = np.linspace(min(V)-3*max(S), max(V)+ 3*max(S), 200)
+    left = max(min(V)-3*max(S),0.001)
+    right = max(V)+ 3*max(S)
+    x  = np.linspace(left,right, int((right-left)/0.01))    
     if tipo == 'abs':
         arquivo = 'cross_section.lx'
         primeira = "{:8s} {:8s} {:8s}\n".format("#Energy(ev)", "cross_section(A^2)", "error")
     else:
         arquivo = 'differential_rate.lx'
         primeira = "{:4s} {:4s} {:4s} TDM={:.3f} au\n".format("#Energy(ev)", "diff_rate", "error",tdm)
     arquivo = naming(arquivo)
     y = espectro[:,np.newaxis]*gauss(x,V[:,np.newaxis],S[:,np.newaxis])
     mean_y =   np.sum(y,axis=0)/N 
     #Error estimate
     sigma  =   np.sqrt(np.sum((y-mean_y)**2,axis=0)/(N*(N-1))) 
-    
+
     if tipo == 'emi':
         #Emission rate calculations
-        from lx.ld import calc_lifetime
-        mean_lifetime, error_lifetime = calc_lifetime(x, mean_y,sigma) 
-        segunda = '# Fluorescence Lifetime: {:5.2e} +/- {:5.2e} s^-1\n'.format(mean_lifetime,error_lifetime)
+        mean_rate, error_rate = calc_emi_rate(x, mean_y,sigma) 
+        segunda = '# Total Rate S1 -> S0: {:5.2e} +/- {:5.2e} s^-1\n'.format(mean_rate,error_rate)
     else:
-        segunda = ''
+        segunda = '# Absorption from State: S0\n'
 
     print(N, "geometries considered.")     
     with open(arquivo, 'w') as f:
         f.write(primeira)
         f.write(segunda)
         for i in range(0,len(x)):
             text = "{:.6f} {:.6e} {:.6e}\n".format(x[i],mean_y[i], sigma[i])
@@ -579,27 +608,27 @@
         nproc  = default(nproc,'nproc={}. If ok, Enter. Otherwise, type it.\n'.format(nproc))
         mem    = default(mem,"mem={}. If ok, Enter. Otherwise, type it.\n".format(mem))
         T      = default(T,"Initial temperature is {} K. If ok, Enter. Otherwise, type it.\n".format(T))
         DT     = default(DT,"Temperature step is {} K. If ok, Enter. Otherwise, type it.\n".format(DT))
     script    = fetch_file('batch script',['.sh'])    
     num_geoms = input("Number of geometries sampled at each round?\n")
     rounds    = input("Number of rounds?\n")
-    limite    = input("Maximum number of jobs to be submitted simultaneously?\n")
+    numjobs   = input("Number of jobs in each batch?\n")
     gaussian  = input('g16 or g09?\n')
     try:
-        int(limite)
         int(num_geoms)
         int(rounds)
+        int(numjobs)
     except:
         fatal_error("These must be integers. Goodbye!")
     with open('limit.lx','w') as f:
-        f.write(str(limite))
+        f.write('Running')
     import subprocess
     folder = os.path.dirname(os.path.realpath(__file__)) 
-    subprocess.Popen(['nohup', 'python3', folder+'/conf_search.py', freqlog, base, nproc, mem, T, DT, num_geoms, rounds, script, gaussian, '&'])
+    subprocess.Popen(['nohup', 'python3', folder+'/conf_search.py', freqlog, base, nproc, mem, T, DT, num_geoms, rounds,numjobs, script, gaussian, '&'])
 ###############################################################
 
 
 ##FINDS SUITABLE VALUE FOR STD#################################    
 def detect_sigma():
     try:
         files = [i for i in os.listdir('.') if 'Magnitudes' in i and '.lx' in i]
@@ -801,14 +830,22 @@
             with open(log,'a') as f:
                 f.write('\n#Aborted!')
             sys.exit()
         time.sleep(30)    
 ###############################################################
 
 ##RUNS CALCULATIONS############################################
-def rodar_lista(lista, batch_file, gaussian, log): 
-    with open('cmd.sh', 'w') as f:
-        for file in lista:
-            f.write('{} {}\n'.format(gaussian,file))
-    subprocess.call(['bash', batch_file, 'cmd.sh']) 
+def rodar_lista(lista, batch_file, gaussian, log, num=1): 
+    #number of scripts is integer division of number of files by num
+    n = len(lista)//num
+    for i in range(n):
+        with open(f'cmd_{i}.sh', 'w') as f:
+            for file in lista[i*num:(i+1)*num]:
+                f.write('{} {}\n'.format(gaussian,file))
+        subprocess.call(['bash', batch_file, f'cmd_{i}.sh']) 
+    if len(lista)%num != 0:
+        with open(f'cmd_{n+1}.sh', 'w') as f:
+            for file in lista[n*num:]:
+                f.write('{} {}\n'.format(gaussian,file))
+        subprocess.call(['bash', batch_file, f'cmd_{n+1}.sh'])
     hold_watch(lista, log)
-###############################################################
+###############################################################
```

### Comparing `LeoX-0.4.0/lx/__main__.py` & `LeoX-0.5.0/lx/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,15 +99,20 @@
         print('Refractive index: {:.3f}\n'.format(nr))
         change = input('Are you satisfied with these parameters? y or n?\n')
         if change.lower() == 'n':
             opc = input("What is the standard deviation of the gaussians?\n")
             try:
                 opc = float(opc)
             except: 
-                lx.tools.fatal_error("It must be a number. Goodbye!")  
+                lx.tools.fatal_error("It must be a number. Goodbye!")
+            nr = input("What is the refractive index?\n")
+            try:
+                nr = float(nr)
+            except: 
+                lx.tools.fatal_error("It must be a number. Goodbye!") 
             tipo = input("What kind of spectrum? Type abs (absorption) or emi (emission)\n")
             if tipo != 'abs' and tipo != 'emi':
                 lx.tools.fatal_error('It must be either one. Goodbye!')
         tipo = tipo[:3]
         if tipo == 'abs':
             estados = input("How many excited states?\n")
             try:
@@ -140,17 +145,19 @@
         lx.tools.abort_batch()
     else:
         lx.tools.fatal_error("It must be one of the options... Goodbye!")
 
 def main():
     try:
         freqlog = sys.argv[1]
-        G, atomos = lx.tools.pega_geom(freqlog)    
+        G, atomos = lx.tools.pega_geom(freqlog)
+        print(len(atomos))
+        print('\n')    
         for i in range(len(atomos)):
-            print("{:2s}  {:.14f}  {:.14f}  {:.14f}".format(atomos[i],G[i,0],G[i,1],G[i,2]))
+            print("{:2s}  {:.7f}  {:.7f}  {:.7f}".format(atomos[i],G[i,0],G[i,1],G[i,2]))
     except:
         interface()
```

### Comparing `LeoX-0.4.0/lx/batch_lx.py` & `LeoX-0.5.0/lx/batch_lx.py`

 * *Files identical despite different names*

### Comparing `LeoX-0.4.0/lx/conf_search.py` & `LeoX-0.5.0/lx/conf_search.py`

 * *Files 17% similar despite different names*

```diff
@@ -60,255 +60,243 @@
         lx.tools.write_input(atomos,Gfinal,header.replace("UUUUU",str((n+3)//3)),bottom.replace("UUUUU",str((n+3)//3)),"Geometry-"+str((n+3)//3+counter)+"-.com")
         lista.append("Geometry-"+str((n+3)//3+counter)+"-.com") 
     return lista      
 ############################################################### 
 
 ##GETS ENERGY FROM THE ORIGINAL FREQ LOG FILE##################
 def get_energy_origin(freqlog):
+    exc = 0
     with open(freqlog, 'r') as f:
         for line in f:
             if 'SCF Done:' in line:
                 line = line.split()
                 scf  = float(line[4])*27.2114
+            elif 'Total Energy,' in line:
+                line = line.split()
+                exc  = float(line[4])*27.2114    
             elif 'Rotational constants' in line:
                 line = line.split()
                 rot  = [float(line[3]),float(line[4]),float(line[5])]    
             elif 'Normal termination' in line:
-                return scf, rot[0], rot[1], rot[2]
+                if exc != 0:
+                    scf = exc
+                return scf, np.array([rot[0], rot[1], rot[2]])
 ###############################################################
 
 ##GETS ENERGIES FROM OPT LOG FILES#############################
 def get_energies(folder,original_molecule):
-    nums,scfs,rotsx, rotsy, rotsz = [], [], [], [], []
+    nums,scfs,rots = [], [], []
     files = [i for i in os.listdir(folder) if '.log' in i and 'Geometry' in i]
     for file in files:
+        exc = 0
         if np.array_equal(original_molecule, fingerprint(file,folder)):
             with open(folder+'/'+file, 'r') as f:
                 num = float(file.split('-')[1])
                 for line in f:
                     if 'SCF Done:' in line:
                         line = line.split()
                         scf  = float(line[4])*27.2114
+                    elif 'Total Energy,' in line:
+                        line = line.split()
+                        exc  = float(line[4])*27.2114    
                     elif 'Rotational constants' in line:
                         line = line.split()
-                        rotx = float(line[3])
-                        roty = float(line[4])
-                        rotz = float(line[5])
+                        rot  = [float(line[3]),float(line[4]),float(line[5])]
                     elif 'Normal termination' in line:
+                        if exc != 0:
+                            scf = exc
                         scfs.append(scf)
                         nums.append(num)
-                        rotsx.append(rotx)
-                        rotsy.append(roty)
-                        rotsz.append(rotz)
+                        rots.append(rot)
+                        
     for file in files:
         try:
             shutil.move(file, 'Geometries/'+file)
             shutil.move(file[:-3]+'com', 'Geometries/'+file[:-3]+'com')
         except:
             pass
-    nums = np.array(nums)
-    scfs = np.array(scfs)
-    rotsx = np.array(rotsx)
-    rotsy = np.array(rotsy)
-    rotsz = np.array(rotsz)
-    return nums, scfs, rotsx, rotsy, rotsz
+    return np.array(nums), np.array(scfs), np.array(rots)
 ###############################################################
 
 def measure(vec1,vec2,cr):
     vec1 = np.array(vec1)     
     vec2 = np.array(vec2)
     cr   = np.array(cr)
     dist = max(abs(vec1 -vec2) - cr)
     distance =  np.heaviside(dist,0)   
     return distance
 
-##CLASSIFIES THE VARIOUS OPTIMIZED STRUCTURES##################
-def classify(nums,scfs,rotsx, rotsy, rotsz,cr0,first):
-    try:
-        assert not first
-        data = np.loadtxt('conformation.lx')
-        if len(np.shape(data)) > 1:
-            engs =  data[:,1].flatten()
-            rotx =  data[:,4].flatten()
-            roty =  data[:,5].flatten() 
-            rotz =  data[:,6].flatten()
-            last =  data[:,10].flatten()
-            crix =  data[:,7].flatten()
-            criy =  data[:,8].flatten()
-            criz =  data[:,9].flatten()
-            exam =  data[:,11].flatten()
-        else:
-            engs = np.array([data[1]])
-            rotx = np.array([data[4]])
-            roty = np.array([data[5]])
-            rotz = np.array([data[6]]) 
-            last = np.array([data[10]])
-            crix = np.array([data[7]])
-            criy = np.array([data[8]])
-            criz = np.array([data[9]])
-            exam = np.array([data[11]])
-    except:
-        rotx = np.array([])
-        roty = np.array([])
-        rotz = np.array([])
-        engs = np.array([])
-        last = np.array([])
-        crix = np.array([])
-        criy = np.array([])
-        criz = np.array([])
-        exam = np.array([])
-    new = []
-    for m in range(len(rotsx)):
-        distances = []   
-        ROTX = np.copy(rotx)
-        ROTY = np.copy(roty)
-        ROTZ = np.copy(rotz)
-        for n in range(len(ROTX)):
-            try:
-                cr = [max(min(2*crix[n],cr0[0]),cr0[0]),max(min(2*crix[n],cr0[1]),cr0[1]),max(min(2*crix[n],cr0[2]),cr0[2])]
-            except:
-                cr = cr0    
-            distance = measure([rotsx[m], rotsy[m], rotsz[m]], [ROTX[n],ROTY[n],ROTZ[n]],cr)
-            distances.append(distance)
-        try:
-            a = distances.index(0)
-            exam[a] = nums[m]
-            engs[a] = (last[a]*engs[a] + scfs[m])/(last[a]+1)
-            x2      = (last[a]*(crix[a]**2 +rotx[a]**2) + rotsx[m]**2)/(last[a]+1)
-            y2      = (last[a]*(criy[a]**2 +roty[a]**2) + rotsy[m]**2)/(last[a]+1)
-            z2      = (last[a]*(criz[a]**2 +rotz[a]**2) + rotsz[m]**2)/(last[a]+1)
-            rotx[a] = (last[a]*rotx[a] + rotsx[m])/(last[a]+1)
-            roty[a] = (last[a]*roty[a] + rotsy[m])/(last[a]+1)
-            rotz[a] = (last[a]*rotz[a] + rotsz[m])/(last[a]+1)    
-            crix[a] = np.sqrt(x2 -rotx[a]**2)
-            criy[a] = np.sqrt(y2 -roty[a]**2)
-            criz[a] = np.sqrt(z2 -rotz[a]**2)
-            last[a] += 1
-        except:
-            new.append(nums[m])
-            rotx  = np.append(rotx,rotsx[m])
-            roty  = np.append(roty,rotsy[m])
-            rotz  = np.append(rotz,rotsz[m])
-            crix  = np.append(crix,0)
-            criy  = np.append(criy,0)
-            criz  = np.append(criz,0) 
-            engs  = np.append(engs,scfs[m])
-            last  = np.append(last,1)
-            exam  = np.append(exam,nums[m])
-
-    try:
-        origin = random.choice(new)
-    except:
-        origin = 0
+class Conformation:
+    def __init__(self,rot,energy,identity,num) -> None:
+        self.rot = rot[np.newaxis,:]
+        self.energy = [energy]
+        self.identity = identity
+        self.std = rot/1000
+        self.num = [num]
+
+    def add_rot(self,rot,num,energy):
+        self.rot = np.vstack((self.rot,rot[np.newaxis,:]))
+        newstd = np.std(self.rot,axis=0)    
+        #get higher std
+        self.std = np.where(newstd > self.std, newstd, self.std)
+        self.num.append(num)
+        self.energy.append(energy)
+
+    def merge_rot(self,rot):
+        self.rot = np.vstack((self.rot,rot))
+        newstd = np.std(self.rot,axis=0)
+        #get higher std
+        self.std = np.where(newstd > self.std, newstd, self.std)
+
+
+    def get_avg(self):
+        return np.mean(self.rot,axis=0)  
+
+
+
+def internal_comparison(conformations):
+    remove = []
+    for i in range(len(conformations)-1):
+        for j in range(i+1,len(conformations)):
+            distance = measure(conformations[i].get_avg(),conformations[j].get_avg(),conformations[j].std+conformations[i].std)
+            if distance == 0:
+                conformations[i].num += conformations[j].num
+                conformations[i].energy += conformations[j].energy
+                conformations[i].merge_rot(conformations[j].rot)
+                remove.append(j)
+                break
+    # remove elements from list whose index is in remove
+    conformations = [i for j, i in enumerate(conformations) if j not in remove]
+    return conformations        
+     
+
+def classify(conformations,folder):
+    nums, scfs, rots = get_energies(folder,conformations[0].identity)
+    for i in range(rots.shape[0]):
+        for conformation in conformations:
+            distance = measure(rots[i,:],conformation.get_avg(),conformation.std)
+            if distance == 0:
+                conformation.add_rot(rots[i,:],nums[i],scfs[i])
+                break
+            conformations.append(Conformation(rots[i,:],scfs[i],conformations[0].identity,nums[i])) 
+    if len(conformations) > 1:
+        conformations  = internal_comparison(conformations)           
+    return conformations
+
+def write_report(conformations,round,total_rounds,temp):
+    engs = []
+    for conformation in conformations:
+        engs.append(np.mean(conformation.energy))
+    engs = np.array(engs)    
+    argsort = np.argsort(engs)
+    engs = engs[argsort]
+    #sort conformations as list
+    conformations = [conformations[i] for i in argsort]
+    deltae = engs - min(engs)
+    probs = np.exp(-(deltae)/(0.026))
+    probs = probs/sum(probs)
+
+    with open('conformation.lx','w') as f:
+        f.write('{:6}  {:10}  {:10}  {:12}  {:10}  {:10}  {:10}  {:10}  {:10}  {:10}  {:6}  {:6}\n'.format('#Group','Energy(eV)','DeltaE(eV)','Prob@300K(%)','Rot1','Rot2','Rot3','Std1','Std2','Std3','Number','Last'))
+        for i in range(len(conformations)):
+            rot = conformations[i].get_avg()
+            std = conformations[i].std
+            last = conformations[i].num[-1]
+            total= len(conformations[i].num)
+            f.write(f'{i+1:<6}  {engs[i]:<10.3f}  {deltae[i]:<10.3f}  {100*probs[i]:<12.1f}  {rot[0]:<10.7f}  {rot[1]:<10.7f}  {rot[2]:<10.7f}  {std[0]:<10.7f}  {std[1]:<10.7f}  {std[2]:<10.7f}  {total:<6.0f}  {last:<6.0f}\n')
+        f.write(f'\n#Round {round}/{total_rounds} Temperature: {temp} K')    
 
-    probs  = np.exp(-1*(engs - min(engs))/0.026)
-    probs  /= np.sum(probs)
-    args   = np.argsort(engs)
-    engs   = engs[args]
-    probs  = probs[args]
-    exam   = exam[args]
-    rotx   = rotx[args]   
-    roty   = roty[args]
-    rotz   = rotz[args]
-    crix   = crix[args]
-    criy   = criy[args]
-    criz   = criz[args]
-    last   = last[args]
-    
-    with open('conformation.lx', 'w') as f: 
-        f.write('{:6}  {:10}  {:10}  {:12}  {:10}  {:10}  {:10}  {:8}  {:8}  {:8}  {:6}  {:6}\n'.format('#Group','Energy(eV)','DeltaE(eV)','Prob@300K(%)','Rot1','Rot2','Rot3','Std1','Std2','Std3','Number','Last'))
-        for i in range(len(probs)):
-            f.write('{:<6}  {:<10.3f}  {:<10.3f}  {:<12.1f}  {:<10.7f}  {:<10.7f}  {:<10.7f}  {:<8.2e}  {:<8.2e}  {:<8.2e}  {:<6.0f}  {:<6.0f}\n'.format(i+1,engs[i],engs[i] -min(engs),100*probs[i],rotx[i],roty[i],rotz[i], crix[i], criy[i], criz[i], last[i],exam[i]))
-    return int(origin), exam
-###############################################################
 
 ##RUNS FREQ CALCULATION FOR NEW CONFORMATION###################
 def rodar_freq(origin,nproc,mem,base,cm,batch_file,gaussian):
-    geomlog = 'Geometries/Geometry-'+str(origin)+'-.log'
+    geomlog = f'Geometries/Geometry-{origin:.0f}-.log'
     G, atomos = lx.tools.pega_geom(geomlog) 
     header = "%nproc={}\n%mem={}\n# freq=(noraman) nosymm  {} \n\n{}\n\n{}\n".format(nproc,mem,base,'ABSSPCT',cm)
-    file = "Freq-"+str(origin)+"-.com"
+    file = f"Freq-{origin:.0f}-.com"
     lx.tools.write_input(atomos,G,header,'',file)
-    lx.tools.rodar_lista([file],batch_file,gaussian,'conformation.lx')
+    lx.tools.rodar_lista([file],batch_file,gaussian,'conformation.lx',1)
     log = file[:-3]+'log'
     with open(log, 'r') as f:
         for line in f:
             if 'Normal termination' in line:
                 return log
             elif 'Error termination' in line:
                 return None
 ###############################################################
 
-
 def main():
     freqlog   = sys.argv[1]
     base      = sys.argv[2]
     nproc     = sys.argv[3]
     mem       = sys.argv[4]
     T         = float(sys.argv[5])
     DT        = float(sys.argv[6])
     num_geoms = int(sys.argv[7])
     rounds    = int(sys.argv[8])
-    script    = sys.argv[9]
-    gaussian  = sys.argv[10]
-
+    numjobs   = int(sys.argv[9])
+    script    = sys.argv[10]
+    gaussian  = sys.argv[11]
+    T0 = T
     freq0 = freqlog
+    if 'td' in base.lower():
+        opt = '=loose'
+    else:
+        opt = ''    
+    
     try:
         os.mkdir('Geometries')
     except:
         pass    
-    original_molecule = fingerprint(freqlog,'.')
     cm        = lx.tools.get_cm(freqlog) 
-    header    = "%nproc={}\n%mem={}\n# opt nosymm  {} \n\n{}\n\n{}\n".format(nproc,mem,base,'ABSSPCT',cm)
-    scf, rotx, roty, rotz  = get_energy_origin(freqlog)
-    cr0 = [rotx/1000, roty/1000, rotz/1000]
-    origin, conformation = classify(np.array([0]),np.array([scf]), np.array([rotx]),np.array([roty]),np.array([rotz]),cr0,True)
+    header    = f"%nproc={nproc}\n%mem={mem}\n# opt{opt} nosymm  {base} \n\nTitle\n\n{cm}\n"
+    scf, rot = get_energy_origin(freqlog)
+    conformations = [Conformation(rot,scf,fingerprint(freqlog,'.'),0)]
     files = [i for i in os.listdir('Geometries') if 'Geometry' in i and '.log' in i]
     if len(files) > 0:
-        nums, scfs, rotsx, rotsy, rotsz = get_energies('Geometries',original_molecule)
-        origin, conformation  = classify(nums,scfs,rotsx,rotsy,rotsz,cr0,False)
+        conformations = classify(conformations,'Geometries')
+        write_report(conformations,0,rounds,T0)
     else:
         pass    
 
-    T0 = T
-
+    
+    groups = len(conformations)
     for i in range(rounds):
         lista      = make_geoms(freqlog, num_geoms, T0, header, '')
-        lx.tools.rodar_lista(lista,script, gaussian, 'conformation.lx')
-        nums, scfs, rotsx,rotsy,rotsz = get_energies('.',original_molecule)
-        origin, conformation  = classify(nums,scfs,rotsx,rotsy,rotsz,cr0,False)
-        with open('conformation.lx', 'a') as f:
-            f.write('\n#Round {}/{} Temperature: {} K'.format(i+1,rounds,T0))    
-        if origin != 0:
-            log  = rodar_freq(origin,nproc,mem,base,cm,script,gaussian)
+        lx.tools.rodar_lista(lista,script, gaussian, 'conformation.lx',numjobs)
+        conformations  = classify(conformations,'.')
+        write_report(conformations,i+1,rounds,T0)
+        
+        if len(conformations) != groups:
+            log  = rodar_freq(conformations[-1].num[-1],nproc,mem,base,cm,script,gaussian)
             if log != None:
                 freqlog = log
                 T0 = T
+            groups = len(conformations)    
         else:
             T0 += DT
 
     with open('conformation.lx', 'a') as f:
         f.write('\n#Search concluded!')
 
     try:
         os.mkdir('Conformers')
     except:
         pass    
 
-    for i in range(len(conformation)):
-        numero  = conformation[i]
+    for i in range(len(conformations)):
+        numero  = conformations[i].num[-1]
         if numero == 0:
             freqlog = freq0    
         else:
             freqlog = 'Geometries/Geometry-{:.0f}-.log'.format(numero) 
         _, _, nproc, mem, scrf, _ = lx.tools.busca_input(freqlog)
         cm = lx.tools.get_cm(freqlog)
         header = '%nproc={}\n%mem={}\n%chk=Group_{}_.chk\n# {} {} opt\n\nTITLE\n\n{}\n'.format(nproc,mem,i+1,'pm6',scrf,cm)
         G, atomos = lx.tools.pega_geom(freqlog)
-        lx.tools.write_input(atomos,G,header,'','Conformers/Group_{}_.com'.format(i+1))
+        lx.tools.write_input(atomos,G,header,'','Conformers/Geometry-{}-.com'.format(i+1))
     
 
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `LeoX-0.4.0/lx/ld.py` & `LeoX-0.5.0/lx/ld.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,17 @@
     #Finds the edges of interpolation
     minA = min(xa)
     minD = min(xd)
     maxA = max(xa)
     maxD = max(xd)
     MIN  = max(minA,minD)
     MAX  = min(maxA,maxD)
-
+    
+    if MIN > MAX:
+        return 0, 0 
     X = np.linspace(MIN, MAX, 1000)
     f1 = interp1d(xa, ya, kind='cubic')
     f2 = interp1d(xd, yd, kind='cubic')
     f3 = interp1d(xa, dya, kind='cubic')
     f4 = interp1d(xd, dyd, kind='cubic')
     
 
@@ -124,16 +126,15 @@
     un               = 1E-48 # unit factor 1 AA^6 = 1E-48 cm^6
     KTTA_cte, KTTA_error = KTTA_cte*un, KTTA_error*un  
     return KTTA_cte, KTTA_error
 ############################################################### 
 
 ##RETURNS ABS AND EMISSION TYPES###############################   
 def emi_abs_types(Abs,Emi):
-    with open(Abs, 'r') as f:
-        abs_type  = f.readlines()[1].split(':')[-1].strip()
+    abs_type  = 'S0'
     with open(Emi, 'r') as f:
         line = f.readlines()[1].split('->')
         emi_init  = line[0].split()[-1].strip()
         emi_final = line[1].split(':')[0].strip()
     return abs_type,emi_init,emi_final
 ###############################################################
```

### Comparing `LeoX-0.4.0/LeoX.egg-info/PKG-INFO` & `LeoX-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,133 +1,130 @@
 Metadata-Version: 2.1
 Name: LeoX
-Version: 0.4.0
+Version: 0.5.0
 Summary: Spectrum simulations with TD(A)-DFT
 Home-page: https://github.com/LeonardoESousa/LeoX
 Author: Leonardo Evaristo de Sousa
 Author-email: leonardo.sousa137@gmail.com
 License: MIT
+Description: 
+        ﻿# LeoX - Light emission and exciton diffusion in organic molecules 
+        
+        [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+        [![license](https://img.shields.io/github/license/LeonardoESousa/LeoX?style=plastic)]()
+        [![down](https://img.shields.io/pypi/dm/LeoX)]()
+        [![maint](https://img.shields.io/maintenance/yes/2021)]()
+        [![commit](https://img.shields.io/github/last-commit/LeonardoESousa/LeoX?style=plastic)]()
+        
+        
+        
+        A package for absorption and fluorescence spectrum simulations using the nuclear ensemble method along with TD(A)-DFT. Estimation of singlet exciton properties (Förster radius, lifetime, diffusion length). Long-range separation parameter tuning. Stochastic conformational search.  Interfaces with the Gaussian (09 or 16) package.
+        
+        
+        Table of Contents
+        =================
+        <!--ts-->
+        * [Cite as:](#cite-as)
+        * [What does this program do?](#what-does-this-program-do)
+        * [What is necessary to use it?](#what-is-necessary-to-use-it)
+        * [How to install it?](#how-to-install-it)
+        * [How to use it?](#how-to-use-it)
+           
+        <!--te-->
+        
+        ## Cite as:
+        
+        > de Sousa, L. E., Bueno, F. T., e Silva, G. M., da Silva Filho, D. A., & de Oliveira Neto, P. H. (2019). Fast predictions of exciton diffusion length in organic materials. Journal of Materials Chemistry C, 7(14), 4066-4071.
+        
+        
+        ## What does this program do?
+        
+        1.  Spectrum simulation:
+            - Calculates Absorption and Fluorescence spectrum simulations using TD(A)-DFT.
+            - Calculations include vibrational contributions to the spectra. 
+            - Optionally, they may also include solvent effects either by PCM or by a state specific solvation model.
+        2.  Exciton properties:   
+            - Calculates Förster radius for transfers between two molecules of equal or different type.
+            - Calculates fluorescence lifetimes.
+            - Calculates singlet exciton diffusion lengths.
+        3.  Extra features:
+            - Tunes the w parameter of long-range separated functionals.
+            - Extracts last geometry from Gaussian log file.
+            - Runs a stochastic coformational search algorithm.
+        
+        
+        ## What is necessary to use it?
+        
+         -  The program requires that the Gaussian quantum chemistry software (G09 or G16) be installed, as it interfaces with it.
+        
+        -   The first step for running spectrum calculations or conformational searches is providing a Gaussian log file for a frequency calculation in the S0 state, if the goal is computing an absorption spectrum, or S1 state, if the objective is calculating a fluoresence spectrum. All frequencies must be real.  
+        
+        -   To obtain estimates for Förster radius, fluorescence lifetimes and singlet exciton diffusion lengths, it is necessary to first perform both absorption and emission spectra calculations for the molecule of interest.
+        
+        ## How to install it?
+        
+        Run:
+        
+        `pip install LeoX`
+        
+        Alternatively, clone the repository to your computer. Inside the LeoX folder, run:
+        
+        `pip install .`
+        
+        Depending on the operating system, the commands above may need to be replace by
+        
+        `pip3 install LeoX` or `pip3 install .`
+        
+        Once installed, you should be able to run the program from any folder by just using the `lx` command.
+        
+        ## How to use it?
+        
+        1. For spectrum simulations:
+        
+            - Create a folder for your project. Add the log file for the frequency calculation to your folder. Run the lx command. Choose option 1 and follow the instructions to select the parameters of the calculation.
+            - Add a bash script file to the folder to control execution. This file depends on which batch system you use. Examples for users of slurm or task spooler (ts) are presented [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples).
+            - Run the `lx` command again, choose option 2 and follow the instructions. Once the calculations are running, you may use option 4 to check the progress or option 9 to abort.
+            <img width="575" alt="LeoX1" src="https://user-images.githubusercontent.com/94139072/144780278-ef3b8ced-af82-4a9d-a8a5-667ebdcbdd71.png">
+        
+            - Once all calculations are done, run the `lx` command and choose option 3. Follow the instructions to set the parameters and the spectrum will be generated.
+            <img width="436" alt="LeoX2" src="https://user-images.githubusercontent.com/94139072/144780487-7d0a5800-c925-4dbc-8b88-041b6d7f35b3.png">
+            
+            - After the spectrum is generated, a file with the extension .lx will be created. For absorption spectra, the file will be named "cross_section.lx", whereas for fluorescence spectra, the file will be named "differential_rate.lx"
+            - It is possible to generate a spectrum with partially concluded calculations. Option 3 can be used multiple times without overwriting the previously generated spectrum. Each time a spectrum is generated, it will have a number at the beginning of the file name, such as "2cross_section.lx".
+            - Each spectrum file is expected to have three columns as indicated below, where the third column can be used to estimate if the amount of sampled geometries are enough for accurate spectrum simulation.
+            <img width="380" alt="LeoX3" src="https://user-images.githubusercontent.com/94139072/144781496-a7c1e1cc-56ea-4de4-85bd-6a0e7ed37d7e.png">
+        
+        
+        2. For exciton properties:
+        
+            - For exciton properties, you must first calculate the fluorescence and absorption spectra of the donor and acceptor molecules of interest to you. 
+            - Once this is done, copy the spectra to a folder and inside this folder run the `lx` command. Choose option 5. Follow the instructions to set the calculation parameters, exemplified below.  
+            <img width="450" alt="LeoX4" src="https://user-images.githubusercontent.com/94139072/144785795-70dec39b-c63d-41a7-9613-fcf4cd1c244f.png">
+           
+            - The correction for short distances takes into account the transition dipole moment of the donor molecule, extracted directly from the Gaussian log. Details can be obtained in the indicated published paper.
+            - A file called `ld.lx` will be generated with all the information.
+            <img width="450" alt="Captura de Tela 2021-12-06 às 01 13 13" src="https://user-images.githubusercontent.com/94139072/144786165-547a9a2e-cca3-434a-90a7-82c610d97d7e.png">
+        
+        
+            - Importantly, diffusion length estimates are only sensible if donor and acceptor molecules are of the same kind. To calculate the Förster radius for transfers between different molecules, you must provide the fluorescence spectrum of the donor molecule and the absorption spectrum of the acceptor molecule. The fluorescence lifetime shown will correspond to that of the donor molecule.  
+        
+        4. For conformational searches:
+            
+            - Create a folder. Add a frequency Gaussian .log file. Include also a bash script file according to your batch system (follow examples for slurm and task spooler [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples)). 
+            - Run the `lx` command in the folder and choose option 6. Follow the instructions to set the calculation parameters. 
+            - Answer the queries to determine the parameters of the conformational search (level of theory, initial temperature, temperature step, number of rounds, number of sampled geometries at each round). 
+            - Once the search starts running, the file conformation.lx will show the conformations found thus far, along with the average energies and Boltzmann populations at 300 K of each. 
+            - After the search is over, a folder named Conformers is created with the geometries of each conformer written to a gaussian input file that can be used for further optimization. 
+        
+        3. For range separation parameter tuning:
+        
+            - Create a folder. Add either a Gaussian .log file or .com file (for any kind of calculation). Include also a bash script file according to your batch system (follow examples for slurm and task spooler [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples)). 
+            - Run the `lx` command in the folder and choose option 7. Follow the instructions to set the calculation parameters. 
+            - You may choose between a relaxed on unrelaxed tuning procedure. In the case of the former, geometry optimizations are run for each range separation parameter value. In the case of unrelaxed tuning, the geometry provided in the .log or .com file will be used for all calculations. 
+         
+        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-﻿# LeoX - Light emission and exciton diffusion in organic molecules 
-
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-[![license](https://img.shields.io/github/license/LeonardoESousa/LeoX?style=plastic)]()
-[![down](https://img.shields.io/pypi/dm/LeoX)]()
-[![maint](https://img.shields.io/maintenance/yes/2021)]()
-[![commit](https://img.shields.io/github/last-commit/LeonardoESousa/LeoX?style=plastic)]()
-
-
-
-A package for absorption and fluorescence spectrum simulations using the nuclear ensemble method along with TD(A)-DFT. Estimation of singlet exciton properties (Förster radius, lifetime, diffusion length). Long-range separation parameter tuning. Stochastic conformational search.  Interfaces with the Gaussian (09 or 16) package.
-
-
-Table of Contents
-=================
-<!--ts-->
-* [Cite as:](#cite-as)
-* [What does this program do?](#what-does-this-program-do)
-* [What is necessary to use it?](#what-is-necessary-to-use-it)
-* [How to install it?](#how-to-install-it)
-* [How to use it?](#how-to-use-it)
-   
-<!--te-->
-
-## Cite as:
-
-> de Sousa, L. E., Bueno, F. T., e Silva, G. M., da Silva Filho, D. A., & de Oliveira Neto, P. H. (2019). Fast predictions of exciton diffusion length in organic materials. Journal of Materials Chemistry C, 7(14), 4066-4071.
-
-
-## What does this program do?
-
-1.  Spectrum simulation:
-    - Calculates Absorption and Fluorescence spectrum simulations using TD(A)-DFT.
-    - Calculations include vibrational contributions to the spectra. 
-    - Optionally, they may also include solvent effects either by PCM or by a state specific solvation model.
-2.  Exciton properties:   
-    - Calculates Förster radius for transfers between two molecules of equal or different type.
-    - Calculates fluorescence lifetimes.
-    - Calculates singlet exciton diffusion lengths.
-3.  Extra features:
-    - Tunes the w parameter of long-range separated functionals.
-    - Extracts last geometry from Gaussian log file.
-    - Runs a stochastic coformational search algorithm.
-
-
-## What is necessary to use it?
-
- -  The program requires that the Gaussian quantum chemistry software (G09 or G16) be installed, as it interfaces with it.
-
--   The first step for running spectrum calculations or conformational searches is providing a Gaussian log file for a frequency calculation in the S0 state, if the goal is computing an absorption spectrum, or S1 state, if the objective is calculating a fluoresence spectrum. All frequencies must be real.  
-
--   To obtain estimates for Förster radius, fluorescence lifetimes and singlet exciton diffusion lengths, it is necessary to first perform both absorption and emission spectra calculations for the molecule of interest.
-
-## How to install it?
-
-Run:
-
-`pip install LeoX`
-
-Alternatively, clone the repository to your computer. Inside the LeoX folder, run:
-
-`pip install .`
-
-Depending on the operating system, the commands above may need to be replace by
-
-`pip3 install LeoX` or `pip3 install .`
-
-Once installed, you should be able to run the program from any folder by just using the `lx` command.
-
-## How to use it?
-
-1. For spectrum simulations:
-
-    - Create a folder for your project. Add the log file for the frequency calculation to your folder. Run the lx command. Choose option 1 and follow the instructions to select the parameters of the calculation.
-    - Add a bash script file to the folder to control execution. This file depends on which batch system you use. Examples for users of slurm or task spooler (ts) are presented [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples).
-    - Run the `lx` command again, choose option 2 and follow the instructions. Once the calculations are running, you may use option 4 to check the progress or option 9 to abort.
-    <img width="575" alt="LeoX1" src="https://user-images.githubusercontent.com/94139072/144780278-ef3b8ced-af82-4a9d-a8a5-667ebdcbdd71.png">
-
-    - Once all calculations are done, run the `lx` command and choose option 3. Follow the instructions to set the parameters and the spectrum will be generated.
-    <img width="436" alt="LeoX2" src="https://user-images.githubusercontent.com/94139072/144780487-7d0a5800-c925-4dbc-8b88-041b6d7f35b3.png">
-    
-    - After the spectrum is generated, a file with the extension .lx will be created. For absorption spectra, the file will be named "cross_section.lx", whereas for fluorescence spectra, the file will be named "differential_rate.lx"
-    - It is possible to generate a spectrum with partially concluded calculations. Option 3 can be used multiple times without overwriting the previously generated spectrum. Each time a spectrum is generated, it will have a number at the beginning of the file name, such as "2cross_section.lx".
-    - Each spectrum file is expected to have three columns as indicated below, where the third column can be used to estimate if the amount of sampled geometries are enough for accurate spectrum simulation.
-    <img width="380" alt="LeoX3" src="https://user-images.githubusercontent.com/94139072/144781496-a7c1e1cc-56ea-4de4-85bd-6a0e7ed37d7e.png">
-
-
-2. For exciton properties:
-
-    - For exciton properties, you must first calculate the fluorescence and absorption spectra of the donor and acceptor molecules of interest to you. 
-    - Once this is done, copy the spectra to a folder and inside this folder run the `lx` command. Choose option 5. Follow the instructions to set the calculation parameters, exemplified below.  
-    <img width="450" alt="LeoX4" src="https://user-images.githubusercontent.com/94139072/144785795-70dec39b-c63d-41a7-9613-fcf4cd1c244f.png">
-   
-    - The correction for short distances takes into account the transition dipole moment of the donor molecule, extracted directly from the Gaussian log. Details can be obtained in the indicated published paper.
-    - A file called `ld.lx` will be generated with all the information.
-    <img width="450" alt="Captura de Tela 2021-12-06 às 01 13 13" src="https://user-images.githubusercontent.com/94139072/144786165-547a9a2e-cca3-434a-90a7-82c610d97d7e.png">
-
-
-    - Importantly, diffusion length estimates are only sensible if donor and acceptor molecules are of the same kind. To calculate the Förster radius for transfers between different molecules, you must provide the fluorescence spectrum of the donor molecule and the absorption spectrum of the acceptor molecule. The fluorescence lifetime shown will correspond to that of the donor molecule.  
-
-4. For conformational searches:
-    
-    - Create a folder. Add a frequency Gaussian .log file. Include also a bash script file according to your batch system (follow examples for slurm and task spooler [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples)). 
-    - Run the `lx` command in the folder and choose option 6. Follow the instructions to set the calculation parameters. 
-    - Answer the queries to determine the parameters of the conformational search (level of theory, initial temperature, temperature step, number of rounds, number of sampled geometries at each round). 
-    - Once the search starts running, the file conformation.lx will show the conformations found thus far, along with the average energies and Boltzmann populations at 300 K of each. 
-    - After the search is over, a folder named Conformers is created with the geometries of each conformer written to a gaussian input file that can be used for further optimization. 
-
-3. For range separation parameter tuning:
-
-    - Create a folder. Add either a Gaussian .log file or .com file (for any kind of calculation). Include also a bash script file according to your batch system (follow examples for slurm and task spooler [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples)). 
-    - Run the `lx` command in the folder and choose option 7. Follow the instructions to set the calculation parameters. 
-    - You may choose between a relaxed on unrelaxed tuning procedure. In the case of the former, geometry optimizations are run for each range separation parameter value. In the case of unrelaxed tuning, the geometry provided in the .log or .com file will be used for all calculations. 
- 
-
-
```

### Comparing `LeoX-0.4.0/setup.py` & `LeoX-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 # Package meta-data.
 NAME = 'LeoX'
 DESCRIPTION = 'Spectrum simulations with TD(A)-DFT'
 URL = 'https://github.com/LeonardoESousa/LeoX'
 EMAIL = 'leonardo.sousa137@gmail.com'
 AUTHOR = 'Leonardo Evaristo de Sousa'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.4.0'
+VERSION = '0.5.0'
 
 # What packages are required for this module to be executed?
-REQUIRED = ['numpy', 'scipy']
+REQUIRED = ['numpy', 'scipy', 'pandas']
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

### Comparing `LeoX-0.4.0/README.md` & `LeoX-0.5.0/README.md`

 * *Files identical despite different names*

