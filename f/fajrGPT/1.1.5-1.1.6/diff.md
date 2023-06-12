# Comparing `tmp/fajrGPT-1.1.5.tar.gz` & `tmp/fajrGPT-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.1.5.tar", last modified: Mon Jun 12 01:17:07 2023, max compression
+gzip compressed data, was "fajrGPT-1.1.6.tar", last modified: Mon Jun 12 01:18:23 2023, max compression
```

## Comparing `fajrGPT-1.1.5.tar` & `fajrGPT-1.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-12 01:17:07.623749 fajrGPT-1.1.5/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.1.5/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-06-12 01:17:07.623575 fajrGPT-1.1.5/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.1.5/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-12 01:17:07.622355 fajrGPT-1.1.5/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.1.5/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-1.1.5/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)     8175 2023-06-12 01:16:17.000000 fajrGPT-1.1.5/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-12 01:17:07.623351 fajrGPT-1.1.5/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-06-12 01:17:07.000000 fajrGPT-1.1.5/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-06-12 01:17:07.000000 fajrGPT-1.1.5/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-06-12 01:17:07.000000 fajrGPT-1.1.5/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-06-12 01:17:07.000000 fajrGPT-1.1.5/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       54 2023-06-12 01:17:07.000000 fajrGPT-1.1.5/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-06-12 01:17:07.000000 fajrGPT-1.1.5/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-06-12 01:17:07.623789 fajrGPT-1.1.5/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-06-12 01:16:47.000000 fajrGPT-1.1.5/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-12 01:18:23.893493 fajrGPT-1.1.6/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.1.6/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-06-12 01:18:23.893287 fajrGPT-1.1.6/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.1.6/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-12 01:18:23.889788 fajrGPT-1.1.6/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.1.6/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-1.1.6/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)     8176 2023-06-12 01:17:52.000000 fajrGPT-1.1.6/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-12 01:18:23.892795 fajrGPT-1.1.6/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-06-12 01:18:23.000000 fajrGPT-1.1.6/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-06-12 01:18:23.000000 fajrGPT-1.1.6/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-06-12 01:18:23.000000 fajrGPT-1.1.6/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-06-12 01:18:23.000000 fajrGPT-1.1.6/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       54 2023-06-12 01:18:23.000000 fajrGPT-1.1.6/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-06-12 01:18:23.000000 fajrGPT-1.1.6/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-06-12 01:18:23.893542 fajrGPT-1.1.6/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-06-12 01:18:04.000000 fajrGPT-1.1.6/setup.py
```

### Comparing `fajrGPT-1.1.5/LICENSE` & `fajrGPT-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.1.5/PKG-INFO` & `fajrGPT-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.1.5
+Version: 1.1.6
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.1.5/README.md` & `fajrGPT-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.1.5/fajrGPT/quran_metadata.py` & `fajrGPT-1.1.6/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.1.5/fajrGPT/wake.py` & `fajrGPT-1.1.6/fajrGPT/wake.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         print(f'{output}.mp3 has already been downloaded and converted.')
 
 def countdown(hours):
     countdown_seconds = float(hours) * 60 * 60
     # use tqdm to display the countdown progress
     print('\n\n\n\n ---------------- BEGINNING COUNTDOWN ---------------- \n\n\n\n')
     # print the current time in HH:MM format
-    print(f'\n\START TIME: {time.strftime("%H:%M", time.localtime())}\n\n')
+    print(f'\n\nSTART TIME: {time.strftime("%H:%M", time.localtime())}\n\n')
     for i in tqdm(range(int(countdown_seconds))):
         time.sleep(1)
     print('\n\n\n\n ---------------- COUNTDOWN COMPLETE ----------------')
     # print the current time in HH:MM format
     print(f'\n\nEND TIME: {time.strftime("%H:%M", time.localtime())}\n\n')
 
 def get_verses_and_explanations():
```

### Comparing `fajrGPT-1.1.5/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.1.6/fajrGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.1.5
+Version: 1.1.6
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.1.5/setup.py` & `fajrGPT-1.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.1.5",
+    version="1.1.6",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

