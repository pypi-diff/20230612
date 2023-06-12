# Comparing `tmp/nemophoto-0.5.0.tar.gz` & `tmp/nemophoto-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nemophoto-0.5.0.tar", last modified: Wed May 17 06:50:04 2023, max compression
+gzip compressed data, was "dist/nemophoto-0.6.0.tar", last modified: Mon Jun 12 15:59:23 2023, max compression
```

## Comparing `nemophoto-0.5.0.tar` & `nemophoto-0.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-05-17 06:50:04.453790 nemophoto-0.5.0/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       51 2022-11-23 13:19:51.000000 nemophoto-0.5.0/.gitignore
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     1071 2021-10-01 13:50:37.000000 nemophoto-0.5.0/LICENSE
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       25 2021-10-30 15:21:47.000000 nemophoto-0.5.0/MANIFEST.in
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     7999 2023-05-17 06:50:04.451790 nemophoto-0.5.0/PKG-INFO
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     6722 2023-05-17 06:49:22.000000 nemophoto-0.5.0/README.md
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-05-17 06:50:04.372789 nemophoto-0.5.0/Tutorial/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)    20260 2023-05-17 06:49:22.000000 nemophoto-0.5.0/Tutorial/Tutorial.md
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-05-17 06:50:04.392790 nemophoto-0.5.0/batch_examples/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      315 2021-10-06 19:56:05.000000 nemophoto-0.5.0/batch_examples/qc.sh
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      245 2021-10-06 19:56:05.000000 nemophoto-0.5.0/batch_examples/slurm.sh
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      205 2022-11-23 13:19:52.000000 nemophoto-0.5.0/batch_examples/td.in
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      118 2022-11-23 13:19:53.000000 nemophoto-0.5.0/batch_examples/ts.sh
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-05-17 06:50:04.438790 nemophoto-0.5.0/nemo/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)        0 2021-10-07 12:24:10.000000 nemophoto-0.5.0/nemo/__init__.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     8440 2023-05-17 06:49:22.000000 nemophoto-0.5.0/nemo/__main__.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       62 2023-05-17 06:49:22.000000 nemophoto-0.5.0/nemo/__version__.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)    41306 2023-05-17 06:49:22.000000 nemophoto-0.5.0/nemo/analysis.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     2417 2022-11-23 13:19:53.000000 nemophoto-0.5.0/nemo/batch_lx.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)    18042 2022-11-23 13:19:53.000000 nemophoto-0.5.0/nemo/tools.py
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-05-17 06:50:04.449790 nemophoto-0.5.0/nemophoto.egg-info/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     7999 2023-05-17 06:50:03.000000 nemophoto-0.5.0/nemophoto.egg-info/PKG-INFO
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      459 2023-05-17 06:50:04.000000 nemophoto-0.5.0/nemophoto.egg-info/SOURCES.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)        1 2023-05-17 06:50:03.000000 nemophoto-0.5.0/nemophoto.egg-info/dependency_links.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       45 2023-05-17 06:50:03.000000 nemophoto-0.5.0/nemophoto.egg-info/entry_points.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       24 2023-05-17 06:50:03.000000 nemophoto-0.5.0/nemophoto.egg-info/requires.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)        5 2023-05-17 06:50:03.000000 nemophoto-0.5.0/nemophoto.egg-info/top_level.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       38 2023-05-17 06:50:04.453790 nemophoto-0.5.0/setup.cfg
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     3644 2023-05-17 06:49:22.000000 nemophoto-0.5.0/setup.py
+drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:59:23.847919 nemophoto-0.6.0/
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       51 2022-11-23 13:19:51.000000 nemophoto-0.6.0/.gitignore
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     1071 2021-10-01 13:50:37.000000 nemophoto-0.6.0/LICENSE
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       25 2021-10-30 15:21:47.000000 nemophoto-0.6.0/MANIFEST.in
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     7999 2023-06-12 15:59:23.845919 nemophoto-0.6.0/PKG-INFO
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     6722 2023-05-17 06:49:22.000000 nemophoto-0.6.0/README.md
+drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:59:23.613918 nemophoto-0.6.0/Tutorial/
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)    20260 2023-05-17 06:49:22.000000 nemophoto-0.6.0/Tutorial/Tutorial.md
+drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:59:23.670918 nemophoto-0.6.0/batch_examples/
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)      315 2021-10-06 19:56:05.000000 nemophoto-0.6.0/batch_examples/qc.sh
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)      245 2021-10-06 19:56:05.000000 nemophoto-0.6.0/batch_examples/slurm.sh
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)      205 2022-11-23 13:19:52.000000 nemophoto-0.6.0/batch_examples/td.in
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)      118 2022-11-23 13:19:53.000000 nemophoto-0.6.0/batch_examples/ts.sh
+drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:59:23.825919 nemophoto-0.6.0/nemo/
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)        0 2021-10-07 12:24:10.000000 nemophoto-0.6.0/nemo/__init__.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     8440 2023-05-17 06:49:22.000000 nemophoto-0.6.0/nemo/__main__.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       62 2023-06-12 15:56:49.000000 nemophoto-0.6.0/nemo/__version__.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)    41423 2023-06-12 15:51:10.000000 nemophoto-0.6.0/nemo/analysis.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     2417 2022-11-23 13:19:53.000000 nemophoto-0.6.0/nemo/batch_lx.py
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)    18058 2023-06-12 15:51:10.000000 nemophoto-0.6.0/nemo/tools.py
+drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:59:23.843919 nemophoto-0.6.0/nemophoto.egg-info/
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     7999 2023-06-12 15:59:22.000000 nemophoto-0.6.0/nemophoto.egg-info/PKG-INFO
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)      459 2023-06-12 15:59:23.000000 nemophoto-0.6.0/nemophoto.egg-info/SOURCES.txt
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)        1 2023-06-12 15:59:22.000000 nemophoto-0.6.0/nemophoto.egg-info/dependency_links.txt
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       45 2023-06-12 15:59:22.000000 nemophoto-0.6.0/nemophoto.egg-info/entry_points.txt
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       31 2023-06-12 15:59:22.000000 nemophoto-0.6.0/nemophoto.egg-info/requires.txt
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)        5 2023-06-12 15:59:22.000000 nemophoto-0.6.0/nemophoto.egg-info/top_level.txt
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)       38 2023-06-12 15:59:23.847919 nemophoto-0.6.0/setup.cfg
+-rw-r--r--   0 ledso    (251734) ecsvip   (15071)     3651 2023-06-12 15:56:49.000000 nemophoto-0.6.0/setup.py
```

### Comparing `nemophoto-0.5.0/LICENSE` & `nemophoto-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nemophoto-0.5.0/PKG-INFO` & `nemophoto-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemophoto
-Version: 0.5.0
+Version: 0.6.0
 Summary: Absorption, fluorescence, phosphorescence spectrum simulations and ISC rate calculations.
 Home-page: https://github.com/LeonardoESousa/NEMO
 Author: Leonardo Evaristo de Sousa
 Author-email: ledso@dtu.dk
 License: MIT
 Description: 
         # NEMO - Photophysics with the Nuclear Ensemble Method
```

### Comparing `nemophoto-0.5.0/README.md` & `nemophoto-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nemophoto-0.5.0/Tutorial/Tutorial.md` & `nemophoto-0.6.0/Tutorial/Tutorial.md`

 * *Files identical despite different names*

### Comparing `nemophoto-0.5.0/nemo/__main__.py` & `nemophoto-0.6.0/nemo/__main__.py`

 * *Files identical despite different names*

### Comparing `nemophoto-0.5.0/nemo/analysis.py` & `nemophoto-0.6.0/nemo/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -631,16 +631,16 @@
 
 def fix_absent_soc(data):
     columns = data.columns.values
     #check if at least one column contains soc_
     if any('soc_' in i for i in columns):
         return data
     else:
-        singlets = [i.split('_')[1] for i in columns if 'e_s' in i]
-        triplets = [i.split('_')[1] for i in columns if 'e_t' in i]        
+        singlets = [i.split('_')[1] for i in columns if 'e_s' in i and 'osc' not in i]
+        triplets = [i.split('_')[1] for i in columns if 'e_t' in i and 'osc' not in i]        
         for ss in singlets:
             for tt in triplets:
                 data[f'soc_{ss}_{tt}'] = 0
     return data            
 
 ###CALCULATES ISC AND EMISSION RATES & SPECTRA#########################################
 def rates(initial,dielec,data=None,ensemble_average=False, detailed=False):
@@ -791,15 +791,15 @@
     if detailed:
         return results, emi, breakdown
     else:
         return results, emi    
 #########################################################################################    
 
 ###COMPUTES ABSORPTION SPECTRA########################################################### 
-def absorption(initial,dielec,data=None, save=False, detailed=False):
+def absorption(initial,dielec,data=None, save=False, detailed=False, nstates=-1):
     if data is None:
         data        = gather_data(initial,save=True) 
         eps_i, nr_i = nemo.tools.get_nr()
         kbT         = nemo.tools.detect_sigma()
     else:
         eps_i  = data['eps'][0]
         nr_i   = data['nr'][0]
@@ -843,18 +843,19 @@
     lambda_b= np.take_along_axis(lambda_b,argsort,axis=1)
     ds      = np.take_along_axis(ds,argsort,axis=1)	
     Ltotal = np.sqrt(2*lambda_b*kbT + kbT**2)
     left   = max(np.min(DE-2*Ltotal),0.01)
     right  = np.max(DE+2*Ltotal)    
     x      = np.linspace(left,right,int((right-left)/0.01))
     # Add extra dimension to DE and Ltotal to match x shape
-    DE      = DE[:,:,np.newaxis]
-    Ltotal  = Ltotal[:,:,np.newaxis]
-    oscs  = oscs[:,:,np.newaxis]
-    lambda_b = lambda_b[:,:,np.newaxis]
+    nstates = min(nstates,DE.shape[1])
+    DE      = DE[:,:nstates,np.newaxis]
+    Ltotal  = Ltotal[:,:nstates,np.newaxis]
+    oscs  = oscs[:,:nstates,np.newaxis]
+    lambda_b = lambda_b[:,:nstates,np.newaxis]
     y      = constante*oscs*nemo.tools.gauss(x,(DE+lambda_b),Ltotal)
     N      = oscs.shape[0]
     mean_y = np.sum(y,axis=0)/N 
     #Error estimate
     sigma    = np.sqrt(np.sum((y-mean_y)**2,axis=0)/(N*(N-1))) 
     mean_y = mean_y.T
     sigma  = sigma.T
```

### Comparing `nemophoto-0.5.0/nemo/batch_lx.py` & `nemophoto-0.6.0/nemo/batch_lx.py`

 * *Files identical despite different names*

### Comparing `nemophoto-0.5.0/nemo/tools.py` & `nemophoto-0.6.0/nemo/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,14 +406,15 @@
         sigma = 0.026
     return sigma
 ###############################################################    
 
 ##FETCHES REFRACTIVE INDEX##################################### 
 def get_nr():
     nr = 1
+    epsilon = 1
     coms = [file for file in os.listdir("Geometries") if 'Geometr' in file and '.com' in file]
     with open('Geometries/'+coms[0],'r') as f:
         for line in f:
             if 'opticaldielectric' in line.lower():
                 nr = np.sqrt(float(line.split()[1]))    
             elif 'dielectric' in line.lower() and 'optical' not in line.lower():
                 epsilon = float(line.split()[1])
```

### Comparing `nemophoto-0.5.0/nemophoto.egg-info/PKG-INFO` & `nemophoto-0.6.0/nemophoto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemophoto
-Version: 0.5.0
+Version: 0.6.0
 Summary: Absorption, fluorescence, phosphorescence spectrum simulations and ISC rate calculations.
 Home-page: https://github.com/LeonardoESousa/NEMO
 Author: Leonardo Evaristo de Sousa
 Author-email: ledso@dtu.dk
 License: MIT
 Description: 
         # NEMO - Photophysics with the Nuclear Ensemble Method
```

### Comparing `nemophoto-0.5.0/setup.py` & `nemophoto-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 # Package meta-data.
 NAME = 'nemophoto'
 DESCRIPTION = 'Absorption, fluorescence, phosphorescence spectrum simulations and ISC rate calculations.'
 URL = 'https://github.com/LeonardoESousa/NEMO'
 EMAIL = 'ledso@dtu.dk'
 AUTHOR = 'Leonardo Evaristo de Sousa'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.5.0'
+VERSION = '0.6.0'
 
 # What packages are required for this module to be executed?
-REQUIRED = ['numpy', 'scipy', 'pandas', 'LeoX']
+REQUIRED = ['numpy', 'scipy', 'pandas', 'LeoX>=0.5.0']
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

