# Comparing `tmp/oda_integral_wrapper-1.4.45.tar.gz` & `tmp/oda_integral_wrapper-1.4.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oda_integral_wrapper-1.4.45.tar", last modified: Tue May 16 21:00:46 2023, max compression
+gzip compressed data, was "oda_integral_wrapper-1.4.46.tar", last modified: Mon Jun 12 08:59:37 2023, max compression
```

## Comparing `oda_integral_wrapper-1.4.45.tar` & `oda_integral_wrapper-1.4.46.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-05-16 21:00:46.508206 oda_integral_wrapper-1.4.45/
--rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)     1175 2021-02-19 13:03:51.000000 oda_integral_wrapper-1.4.45/LICENSE.rst
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      338 2023-05-16 21:00:46.508206 oda_integral_wrapper-1.4.45/PKG-INFO
--rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)     1890 2021-03-04 23:47:29.000000 oda_integral_wrapper-1.4.45/README.md
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-05-16 21:00:46.508206 oda_integral_wrapper-1.4.45/oda_integral_wrapper/
--rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)      794 2021-04-28 13:12:46.000000 oda_integral_wrapper-1.4.45/oda_integral_wrapper/__init__.py
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    15570 2021-10-08 11:47:27.000000 oda_integral_wrapper-1.4.45/oda_integral_wrapper/fit_cyclotron.py
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     6114 2022-06-17 12:23:32.000000 oda_integral_wrapper-1.4.45/oda_integral_wrapper/fitimage.py
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     8623 2021-04-30 07:41:48.000000 oda_integral_wrapper-1.4.45/oda_integral_wrapper/get_osa10_11_factor.py
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     3238 2022-08-05 07:47:15.000000 oda_integral_wrapper-1.4.45/oda_integral_wrapper/itime.py
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    18094 2023-05-16 20:59:58.000000 oda_integral_wrapper-1.4.45/oda_integral_wrapper/planning.py
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    79198 2023-04-06 16:39:21.000000 oda_integral_wrapper-1.4.45/oda_integral_wrapper/wrapper.py
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-05-16 21:00:46.508206 oda_integral_wrapper-1.4.45/oda_integral_wrapper.egg-info/
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      338 2023-05-16 21:00:46.000000 oda_integral_wrapper-1.4.45/oda_integral_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      502 2023-05-16 21:00:46.000000 oda_integral_wrapper-1.4.45/oda_integral_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        1 2023-05-16 21:00:46.000000 oda_integral_wrapper-1.4.45/oda_integral_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)       92 2023-05-16 21:00:46.000000 oda_integral_wrapper-1.4.45/oda_integral_wrapper.egg-info/requires.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)       21 2023-05-16 21:00:46.000000 oda_integral_wrapper-1.4.45/oda_integral_wrapper.egg-info/top_level.txt
--rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)       79 2023-05-16 21:00:46.508206 oda_integral_wrapper-1.4.45/setup.cfg
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1197 2023-05-16 21:00:06.000000 oda_integral_wrapper-1.4.45/setup.py
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-06-12 08:59:37.744507 oda_integral_wrapper-1.4.46/
+-rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)     1175 2021-02-19 13:03:51.000000 oda_integral_wrapper-1.4.46/LICENSE.rst
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      338 2023-06-12 08:59:37.744507 oda_integral_wrapper-1.4.46/PKG-INFO
+-rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)     1890 2021-03-04 23:47:29.000000 oda_integral_wrapper-1.4.46/README.md
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-06-12 08:59:37.744507 oda_integral_wrapper-1.4.46/oda_integral_wrapper/
+-rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)      794 2021-04-28 13:12:46.000000 oda_integral_wrapper-1.4.46/oda_integral_wrapper/__init__.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    15570 2021-10-08 11:47:27.000000 oda_integral_wrapper-1.4.46/oda_integral_wrapper/fit_cyclotron.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     6114 2022-06-17 12:23:32.000000 oda_integral_wrapper-1.4.46/oda_integral_wrapper/fitimage.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     8623 2021-04-30 07:41:48.000000 oda_integral_wrapper-1.4.46/oda_integral_wrapper/get_osa10_11_factor.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     3238 2022-08-05 07:47:15.000000 oda_integral_wrapper-1.4.46/oda_integral_wrapper/itime.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    18443 2023-06-07 16:12:26.000000 oda_integral_wrapper-1.4.46/oda_integral_wrapper/planning.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    79198 2023-04-06 16:39:21.000000 oda_integral_wrapper-1.4.46/oda_integral_wrapper/wrapper.py
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-06-12 08:59:37.744507 oda_integral_wrapper-1.4.46/oda_integral_wrapper.egg-info/
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      338 2023-06-12 08:59:37.000000 oda_integral_wrapper-1.4.46/oda_integral_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      502 2023-06-12 08:59:37.000000 oda_integral_wrapper-1.4.46/oda_integral_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        1 2023-06-12 08:59:37.000000 oda_integral_wrapper-1.4.46/oda_integral_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)       92 2023-06-12 08:59:37.000000 oda_integral_wrapper-1.4.46/oda_integral_wrapper.egg-info/requires.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)       21 2023-06-12 08:59:37.000000 oda_integral_wrapper-1.4.46/oda_integral_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)       79 2023-06-12 08:59:37.744507 oda_integral_wrapper-1.4.46/setup.cfg
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1197 2023-06-07 16:15:25.000000 oda_integral_wrapper-1.4.46/setup.py
```

### Comparing `oda_integral_wrapper-1.4.45/LICENSE.rst` & `oda_integral_wrapper-1.4.46/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `oda_integral_wrapper-1.4.45/README.md` & `oda_integral_wrapper-1.4.46/README.md`

 * *Files identical despite different names*

### Comparing `oda_integral_wrapper-1.4.45/oda_integral_wrapper/__init__.py` & `oda_integral_wrapper-1.4.46/oda_integral_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `oda_integral_wrapper-1.4.45/oda_integral_wrapper/fit_cyclotron.py` & `oda_integral_wrapper-1.4.46/oda_integral_wrapper/fit_cyclotron.py`

 * *Files identical despite different names*

### Comparing `oda_integral_wrapper-1.4.45/oda_integral_wrapper/fitimage.py` & `oda_integral_wrapper-1.4.46/oda_integral_wrapper/fitimage.py`

 * *Files identical despite different names*

### Comparing `oda_integral_wrapper-1.4.45/oda_integral_wrapper/get_osa10_11_factor.py` & `oda_integral_wrapper-1.4.46/oda_integral_wrapper/get_osa10_11_factor.py`

 * *Files identical despite different names*

### Comparing `oda_integral_wrapper-1.4.45/oda_integral_wrapper/itime.py` & `oda_integral_wrapper-1.4.46/oda_integral_wrapper/itime.py`

 * *Files identical despite different names*

### Comparing `oda_integral_wrapper-1.4.45/oda_integral_wrapper/planning.py` & `oda_integral_wrapper-1.4.46/oda_integral_wrapper/planning.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,17 +114,26 @@
     if len(pods) == 0:
         raise Exception("no pointing definition as " + pt + ' or ' + pt+'.gz')
     print("Found pods ", pods)
     pod = pods[-1]
     return getter(pod)
 
 
-def get_pod(revid):
+def get_pod(revid, upper_range=16):
+    """gets a POD file from auxiliary files
+
+    Args:
+        revid (str): REvolution ID, e.g.  0102 2524 0080
+        upper_range (int, optional): It will loop to search POD with names up to upper_range and retain the upper one. Defaults to 16.
+
+    Returns:
+        list: POD LIST of entries in the fits file
+    """    
     pod_list = []
-    for num in range(1, 10):
+    for num in range(1, upper_range):
         pod_test = pvphase_url + "/aux/org/%s/pod_%s_%04d.fits" % (revid, revid, num)
         try:
             ff = fits.open(pod_test)
             pod_list.append(pod_test)
             ff.close()
         except:
             print(pod_test + " not found")
```

### Comparing `oda_integral_wrapper-1.4.45/oda_integral_wrapper/wrapper.py` & `oda_integral_wrapper-1.4.46/oda_integral_wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `oda_integral_wrapper-1.4.45/setup.py` & `oda_integral_wrapper-1.4.46/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 print('packs', packs)
 
 include_package_data = True
 
 scripts_list = glob.glob('./bin/*')
 setup(name='oda_integral_wrapper',
-      version="1.4.45",
+      version="1.4.46",
       description='wrapper for INTEGRAL analysis using the API plugin for CDCI online data analysis',
       author='Carlo Ferrigno',
       author_email='carlo.ferrigno@unige.ch',
       url="https://gitlab.astro.unige.ch/oda/api-clients/oda_api_wrapper",
       scripts=scripts_list,
       packages=packs,
       package_data={'oda_integral_wrapper': ['config_dir/*']},
```

