# Comparing `tmp/gtempco2-0.0.2.tar.gz` & `tmp/gtempco2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtempco2-0.0.2.tar", last modified: Mon Jun 12 04:43:43 2023, max compression
+gzip compressed data, was "gtempco2-0.0.3.tar", last modified: Mon Jun 12 05:00:28 2023, max compression
```

## Comparing `gtempco2-0.0.2.tar` & `gtempco2-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-12 04:43:43.618582 gtempco2-0.0.2/
--rw-r--r--   0 yt        (1000) yt        (1000)     1780 2023-06-12 04:43:43.617761 gtempco2-0.0.2/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     1249 2023-06-12 04:40:13.000000 gtempco2-0.0.2/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-06-12 04:43:43.618582 gtempco2-0.0.2/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      951 2023-06-12 04:42:39.000000 gtempco2-0.0.2/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-12 04:43:43.601524 gtempco2-0.0.2/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-12 04:43:43.616707 gtempco2-0.0.2/src/gtempco2.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1780 2023-06-12 04:43:43.000000 gtempco2-0.0.2/src/gtempco2.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      217 2023-06-12 04:43:43.000000 gtempco2-0.0.2/src/gtempco2.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-06-12 04:43:43.000000 gtempco2-0.0.2/src/gtempco2.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       44 2023-06-12 04:43:43.000000 gtempco2-0.0.2/src/gtempco2.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        9 2023-06-12 04:43:43.000000 gtempco2-0.0.2/src/gtempco2.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     2702 2023-06-12 01:39:39.000000 gtempco2-0.0.2/src/gtempco2.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-12 05:00:28.966033 gtempco2-0.0.3/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1780 2023-06-12 05:00:28.964908 gtempco2-0.0.3/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)     1249 2023-06-12 04:59:29.000000 gtempco2-0.0.3/README.md
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-06-12 05:00:28.966033 gtempco2-0.0.3/setup.cfg
+-rw-r--r--   0 yt        (1000) yt        (1000)      951 2023-06-12 05:00:03.000000 gtempco2-0.0.3/setup.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-12 05:00:28.957749 gtempco2-0.0.3/src/
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-12 05:00:28.964471 gtempco2-0.0.3/src/gtempco2.egg-info/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1780 2023-06-12 05:00:28.000000 gtempco2-0.0.3/src/gtempco2.egg-info/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      217 2023-06-12 05:00:28.000000 gtempco2-0.0.3/src/gtempco2.egg-info/SOURCES.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-06-12 05:00:28.000000 gtempco2-0.0.3/src/gtempco2.egg-info/dependency_links.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       44 2023-06-12 05:00:28.000000 gtempco2-0.0.3/src/gtempco2.egg-info/entry_points.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        9 2023-06-12 05:00:28.000000 gtempco2-0.0.3/src/gtempco2.egg-info/top_level.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)     2702 2023-06-12 04:57:51.000000 gtempco2-0.0.3/src/gtempco2.py
```

### Comparing `gtempco2-0.0.2/PKG-INFO` & `gtempco2-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtempco2
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for displaying global temperature and co2
 Home-page: https://github.com/ytakefuji/gtempco2
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/gtempco2
 Platform: UNKNOWN
@@ -26,20 +26,20 @@
 
 $ pip install gtempco2
 
 To run gtempco2, the user-specified time period such as start-date and end-date is needed to plot a graph of the global temperature and co2 from start-date to end-date. 
 
 The format of them is as follows.
 
-For example, 1978-03 indicates March 1978 when NOAA started the measurement of the global co2.
+For example, 1958-03 indicates March 1958 when NOAA started the measurement of the global co2.
 
 <pre>
 $ gtempco2
 enter start_date: e.g. 1960-04
-co2 measurement started from 1978-03
+co2 measurement started from 1958-03
 yyyy-mo: 1960-06
 enter end_date: e.g. 2023-04
 yyyy-mo: 1965-06
 start_date= 1960-06 end_date= 1965-06
 </pre>
 
 The system will ask the start-date and end-date. The result will be shown and saved in the directory as follows.
```

### Comparing `gtempco2-0.0.2/README.md` & `gtempco2-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 
 $ pip install gtempco2
 
 To run gtempco2, the user-specified time period such as start-date and end-date is needed to plot a graph of the global temperature and co2 from start-date to end-date. 
 
 The format of them is as follows.
 
-For example, 1978-03 indicates March 1978 when NOAA started the measurement of the global co2.
+For example, 1958-03 indicates March 1958 when NOAA started the measurement of the global co2.
 
 <pre>
 $ gtempco2
 enter start_date: e.g. 1960-04
-co2 measurement started from 1978-03
+co2 measurement started from 1958-03
 yyyy-mo: 1960-06
 enter end_date: e.g. 2023-04
 yyyy-mo: 1965-06
 start_date= 1960-06 end_date= 1965-06
 </pre>
 
 The system will ask the start-date and end-date. The result will be shown and saved in the directory as follows.
```

### Comparing `gtempco2-0.0.2/setup.py` & `gtempco2-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gtempco2",
-    version="0.0.2",
+    version="0.0.3",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for displaying global temperature and co2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/gtempco2",
     project_urls={
```

### Comparing `gtempco2-0.0.2/src/gtempco2.egg-info/PKG-INFO` & `gtempco2-0.0.3/src/gtempco2.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtempco2
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for displaying global temperature and co2
 Home-page: https://github.com/ytakefuji/gtempco2
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/gtempco2
 Platform: UNKNOWN
@@ -26,20 +26,20 @@
 
 $ pip install gtempco2
 
 To run gtempco2, the user-specified time period such as start-date and end-date is needed to plot a graph of the global temperature and co2 from start-date to end-date. 
 
 The format of them is as follows.
 
-For example, 1978-03 indicates March 1978 when NOAA started the measurement of the global co2.
+For example, 1958-03 indicates March 1958 when NOAA started the measurement of the global co2.
 
 <pre>
 $ gtempco2
 enter start_date: e.g. 1960-04
-co2 measurement started from 1978-03
+co2 measurement started from 1958-03
 yyyy-mo: 1960-06
 enter end_date: e.g. 2023-04
 yyyy-mo: 1965-06
 start_date= 1960-06 end_date= 1965-06
 </pre>
 
 The system will ask the start-date and end-date. The result will be shown and saved in the directory as follows.
```

### Comparing `gtempco2-0.0.2/src/gtempco2.py` & `gtempco2-0.0.3/src/gtempco2.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import matplotlib.pyplot as plt
 from matplotlib.ticker import MaxNLocator
 from scipy import stats
 import subprocess as sp
 
 def main():
  print('enter start_date: e.g. 1960-04')
- print('co2 measurement started from 1978-03')
+ print('co2 measurement started from 1958-03')
  start=input('yyyy-mo: ')
  print('enter end_date: e.g. 2023-04')
  end=input('yyyy-mo: ')
  print('start_date=',start,'end_date=',end)
  sp.call('wget -nc https://www.ncei.noaa.gov/data/noaa-global-surface-temperature/v5.1/access/timeseries/aravg.mon.land_ocean.90S.90N.v5.1.0.202304.asc', shell=True)
  d=pd.read_csv('aravg.mon.land_ocean.90S.90N.v5.1.0.202304.asc',sep='\\s+',header=None)
  d=d.iloc[:, :3]
```

