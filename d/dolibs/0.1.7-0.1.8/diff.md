# Comparing `tmp/dolibs-0.1.7.tar.gz` & `tmp/dolibs-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolibs-0.1.7.tar", last modified: Wed Jun  7 14:46:26 2023, max compression
+gzip compressed data, was "dolibs-0.1.8.tar", last modified: Mon Jun 12 08:59:31 2023, max compression
```

## Comparing `dolibs-0.1.7.tar` & `dolibs-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-07 14:46:26.781478 dolibs-0.1.7/
--rw-r--r--   0 leandro    (501) staff       (20)      298 2023-06-07 14:46:26.781351 dolibs-0.1.7/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)     1152 2023-05-03 10:26:07.000000 dolibs-0.1.7/README.md
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-07 14:46:26.780469 dolibs-0.1.7/dolibs/
--rw-r--r--   0 leandro    (501) staff       (20)        0 2023-04-12 09:31:04.000000 dolibs-0.1.7/dolibs/__init__.py
--rw-r--r--   0 leandro    (501) staff       (20)     4596 2023-06-07 14:46:07.000000 dolibs-0.1.7/dolibs/dewpoint.py
--rw-r--r--   0 leandro    (501) staff       (20)     4591 2023-05-03 09:47:15.000000 dolibs-0.1.7/dolibs/skintemp.py
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-07 14:46:26.781168 dolibs-0.1.7/dolibs.egg-info/
--rw-r--r--   0 leandro    (501) staff       (20)      298 2023-06-07 14:46:26.000000 dolibs-0.1.7/dolibs.egg-info/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)      224 2023-06-07 14:46:26.000000 dolibs-0.1.7/dolibs.egg-info/SOURCES.txt
--rw-r--r--   0 leandro    (501) staff       (20)        1 2023-06-07 14:46:26.000000 dolibs-0.1.7/dolibs.egg-info/dependency_links.txt
--rw-r--r--   0 leandro    (501) staff       (20)       71 2023-06-07 14:46:26.000000 dolibs-0.1.7/dolibs.egg-info/requires.txt
--rw-r--r--   0 leandro    (501) staff       (20)        7 2023-06-07 14:46:26.000000 dolibs-0.1.7/dolibs.egg-info/top_level.txt
--rw-r--r--   0 leandro    (501) staff       (20)       38 2023-06-07 14:46:26.781528 dolibs-0.1.7/setup.cfg
--rw-r--r--   0 leandro    (501) staff       (20)      599 2023-06-07 14:46:23.000000 dolibs-0.1.7/setup.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-12 08:59:31.886454 dolibs-0.1.8/
+-rw-r--r--   0 leandro    (501) staff       (20)      298 2023-06-12 08:59:31.886331 dolibs-0.1.8/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)     1152 2023-05-03 10:26:07.000000 dolibs-0.1.8/README.md
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-12 08:59:31.885362 dolibs-0.1.8/dolibs/
+-rw-r--r--   0 leandro    (501) staff       (20)        0 2023-04-12 09:31:04.000000 dolibs-0.1.8/dolibs/__init__.py
+-rw-r--r--   0 leandro    (501) staff       (20)     4596 2023-06-12 08:58:55.000000 dolibs-0.1.8/dolibs/dewpoint.py
+-rw-r--r--   0 leandro    (501) staff       (20)     4591 2023-05-03 09:47:15.000000 dolibs-0.1.8/dolibs/skintemp.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-12 08:59:31.886119 dolibs-0.1.8/dolibs.egg-info/
+-rw-r--r--   0 leandro    (501) staff       (20)      298 2023-06-12 08:59:31.000000 dolibs-0.1.8/dolibs.egg-info/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)      224 2023-06-12 08:59:31.000000 dolibs-0.1.8/dolibs.egg-info/SOURCES.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        1 2023-06-12 08:59:31.000000 dolibs-0.1.8/dolibs.egg-info/dependency_links.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       71 2023-06-12 08:59:31.000000 dolibs-0.1.8/dolibs.egg-info/requires.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        7 2023-06-12 08:59:31.000000 dolibs-0.1.8/dolibs.egg-info/top_level.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       38 2023-06-12 08:59:31.886503 dolibs-0.1.8/setup.cfg
+-rw-r--r--   0 leandro    (501) staff       (20)      599 2023-06-12 08:59:18.000000 dolibs-0.1.8/setup.py
```

### Comparing `dolibs-0.1.7/README.md` & `dolibs-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `dolibs-0.1.7/dolibs/dewpoint.py` & `dolibs-0.1.8/dolibs/dewpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         print('open nc file')
         nc_file = basepath+'/dewpointtemp_'+str(year_in)+'_'+str(month_in)+'.nc'
         print('Loading dataset')
         ds = xr.open_dataset(nc_file).load()
 
         print('Calculate daily temperature and transform in Celsius')
         daily_data = ds.resample(time='d').mean()
-        daily_data_celsius = daily_data.skt - 273.15
+        daily_data_celsius = daily_data.d2m - 273.15
 
         print('Start cube elaboration')
         #always skip last retrieved day cause it could be incomplete
         for i in range((len(daily_data_celsius) - 1)):
             dout = daily_data_celsius[i,:,:]
             dout.rio.write_crs("EPSG:4326", inplace=True).rio.to_raster(nc_file+'_out_'+str((i+1))+'.tiff')
             #set file and form data for post call
```

### Comparing `dolibs-0.1.7/dolibs/skintemp.py` & `dolibs-0.1.8/dolibs/skintemp.py`

 * *Files identical despite different names*

### Comparing `dolibs-0.1.7/setup.py` & `dolibs-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 setup(
     name='dolibs',
     packages=find_packages(include=['dolibs']),
-    version='0.1.7',
+    version='0.1.8',
     url='https://github.com/n3tmaster/ERA5_procedures',
     description='Library for importing ERA5 Copernicus data into Drought Observatory platform',
     author='Leandro Rocchi - CNR',
     author_email='leandro.rocchi@cnr.it',
     license='MIT',
     install_requires=['cdsapi','scipy','netcdf4','rioxarray','numpy','xarray','sqlalchemy','psycopg2-binary'],
     setup_requires=['pytest-runner'],
```

