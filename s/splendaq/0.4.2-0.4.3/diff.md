# Comparing `tmp/splendaq-0.4.2.tar.gz` & `tmp/splendaq-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splendaq-0.4.2.tar", last modified: Fri Jun  9 17:18:01 2023, max compression
+gzip compressed data, was "splendaq-0.4.3.tar", last modified: Mon Jun 12 21:19:55 2023, max compression
```

## Comparing `splendaq-0.4.2.tar` & `splendaq-0.4.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.279411 splendaq-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.271411 splendaq-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.271411 splendaq-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-09 17:17:50.000000 splendaq-0.4.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-09 17:17:50.000000 splendaq-0.4.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-09 17:17:50.000000 splendaq-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-09 17:17:50.000000 splendaq-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-09 17:17:50.000000 splendaq-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-09 17:18:01.279411 splendaq-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-09 17:17:50.000000 splendaq-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 17:17:50.000000 splendaq-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-09 17:18:01.279411 splendaq-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-09 17:17:50.000000 splendaq-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.271411 splendaq-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.271411 splendaq-0.4.2/src/splendaq/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 17:18:01.000000 splendaq-0.4.2/src/splendaq/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.275411 splendaq-0.4.2/src/splendaq/daq/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18531 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/daq/_log_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/daq/_offline_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/daq/_oscilloscope.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/daq/_sequencer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.275411 splendaq-0.4.2/src/splendaq/io/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/io/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.275411 splendaq-0.4.2/src/splendaq/io/_liconvert/
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/io/_liconvert/COPYING.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)   716536 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/io/_liconvert/liconvert_linux
--rwxr-xr-x   0 runner    (1001) docker     (123)   629104 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/io/_liconvert/liconvert_macos
--rw-r--r--   0 runner    (1001) docker     (123)   689928 2023-06-09 17:17:50.000000 splendaq-0.4.2/src/splendaq/io/_liconvert/liconvert_windows.exe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.275411 splendaq-0.4.2/src/splendaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-09 17:18:01.000000 splendaq-0.4.2/src/splendaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-09 17:18:01.000000 splendaq-0.4.2/src/splendaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:18:01.000000 splendaq-0.4.2/src/splendaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-09 17:18:01.000000 splendaq-0.4.2/src/splendaq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:18:01.000000 splendaq-0.4.2/src/splendaq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 17:18:01.000000 splendaq-0.4.2/src/splendaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 17:18:01.000000 splendaq-0.4.2/src/splendaq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.271411 splendaq-0.4.2/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.279411 splendaq-0.4.2/tutorials/daq/
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-06-09 17:17:50.000000 splendaq-0.4.2/tutorials/daq/dc_oscilloscope.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-06-09 17:17:50.000000 splendaq-0.4.2/tutorials/daq/event_building.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-06-09 17:17:50.000000 splendaq-0.4.2/tutorials/daq/logging_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-06-09 17:17:50.000000 splendaq-0.4.2/tutorials/daq/running_the_sequencer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-09 17:17:50.000000 splendaq-0.4.2/tutorials/daq/sequencer_settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:18:01.279411 splendaq-0.4.2/tutorials/io/
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-09 17:17:50.000000 splendaq-0.4.2/tutorials/io/read_files.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-06-09 17:17:50.000000 splendaq-0.4.2/tutorials/io/write_files.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.116008 splendaq-0.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.092008 splendaq-0.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.096008 splendaq-0.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-12 21:19:39.000000 splendaq-0.4.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-12 21:19:39.000000 splendaq-0.4.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-12 21:19:39.000000 splendaq-0.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-12 21:19:39.000000 splendaq-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-12 21:19:39.000000 splendaq-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-12 21:19:55.116008 splendaq-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-12 21:19:39.000000 splendaq-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 21:19:39.000000 splendaq-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-12 21:19:55.116008 splendaq-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-12 21:19:39.000000 splendaq-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.092008 splendaq-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.096008 splendaq-0.4.3/src/splendaq/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 21:19:55.000000 splendaq-0.4.3/src/splendaq/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.104008 splendaq-0.4.3/src/splendaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18531 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/daq/_log_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24319 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/daq/_offline_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/daq/_oscilloscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/daq/_sequencer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.104008 splendaq-0.4.3/src/splendaq/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/io/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.112008 splendaq-0.4.3/src/splendaq/io/_liconvert/
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/io/_liconvert/COPYING.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)   716536 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/io/_liconvert/liconvert_linux
+-rwxr-xr-x   0 runner    (1001) docker     (123)   629104 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/io/_liconvert/liconvert_macos
+-rw-r--r--   0 runner    (1001) docker     (123)   689928 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/io/_liconvert/liconvert_windows.exe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.100008 splendaq-0.4.3/src/splendaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-12 21:19:55.000000 splendaq-0.4.3/src/splendaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-12 21:19:55.000000 splendaq-0.4.3/src/splendaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:19:55.000000 splendaq-0.4.3/src/splendaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-12 21:19:55.000000 splendaq-0.4.3/src/splendaq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:19:54.000000 splendaq-0.4.3/src/splendaq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-12 21:19:55.000000 splendaq-0.4.3/src/splendaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 21:19:55.000000 splendaq-0.4.3/src/splendaq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.092008 splendaq-0.4.3/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.112008 splendaq-0.4.3/tutorials/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-06-12 21:19:39.000000 splendaq-0.4.3/tutorials/daq/dc_oscilloscope.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-06-12 21:19:39.000000 splendaq-0.4.3/tutorials/daq/event_building.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-06-12 21:19:39.000000 splendaq-0.4.3/tutorials/daq/logging_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-06-12 21:19:39.000000 splendaq-0.4.3/tutorials/daq/running_the_sequencer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-12 21:19:39.000000 splendaq-0.4.3/tutorials/daq/sequencer_settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.116008 splendaq-0.4.3/tutorials/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-12 21:19:39.000000 splendaq-0.4.3/tutorials/io/read_files.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-06-12 21:19:39.000000 splendaq-0.4.3/tutorials/io/write_files.ipynb
```

### Comparing `splendaq-0.4.2/.github/workflows/python-package.yml` & `splendaq-0.4.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/.github/workflows/python-publish.yml` & `splendaq-0.4.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/.gitignore` & `splendaq-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/LICENSE` & `splendaq-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/PKG-INFO` & `splendaq-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splendaq
-Version: 0.4.2
+Version: 0.4.3
 Summary: Generalized offline data acquisition with a focus on the Moku
 Home-page: https://github.com/splendor-collab/splendaq
 Author: SPLENDOR Collaboration
 Maintainer: SPLENDOR Collaboration
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `splendaq-0.4.2/README.md` & `splendaq-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/setup.cfg` & `splendaq-0.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/src/splendaq/_cli.py` & `splendaq-0.4.3/src/splendaq/_cli.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/src/splendaq/daq/_log_data.py` & `splendaq-0.4.3/src/splendaq/daq/_log_data.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/src/splendaq/daq/_offline_trigger.py` & `splendaq-0.4.3/src/splendaq/daq/_offline_trigger.py`

 * *Files 4% similar despite different names*

```diff
@@ -357,15 +357,15 @@
         filts[:, :cut_len//2] = 0
         filts[:, -(cut_len//2) + (cut_len + 1) % 2:] = 0
 
         return filts
 
 
     @staticmethod
-    def _smart_trigger(trace, threshold):
+    def _smart_trigger(trace, threshold, mergewindow):
         """
         Method for carrying out a "smart" triggering algorithm, where
         the turn on threshold is specified, and the turn off threshold
         is the smaller of the turn on threshold and 1/e times the
         maximum OF amplitude.
 
         """
@@ -399,18 +399,34 @@
                 ind1 = ind_off_init
 
             ind_list.append([ind0, ind1])
 
         if len(ind_list)==0:
             return []
 
-        return np.vstack(ind_list)
+        ind_array = np.vstack(ind_list)
 
+        if mergewindow is not None:
+            ind_array_flat = ind_array.flatten()
+            arr = (ind_array_flat[1:] - ind_array_flat[:-1])[1::2] < mergewindow
 
-    def acquire_pulses(self, template, psd, threshold, tchan):
+            inds_keep = [0]
+            for ii, b in enumerate(arr):
+                if ~b:
+                    inds_keep.extend([2 * ii + 1, 2 * ii + 2])
+            inds_keep.append(-1)
+
+            ind_array_out = ind_array_flat[inds_keep].reshape(len(inds_keep)//2, 2)
+
+            return ind_array_out
+
+        return ind_array
+
+
+    def acquire_pulses(self, template, psd, threshold, tchan, mergewindow=None):
         """
         Method to carry out the offline triggering algorithm based on
         the OF formalism in time domain. Only trigeers on one specified
         channel.
 
         Parameters
         ----------
@@ -425,16 +441,22 @@
             10-sigma threshold. If positive, it is assumed that events
             with amplitudes above this value will be extracted. If
             negative, then events with amplitudes below this value
             will be extracted.
         tchan : int
             The channel, designated by array index, to set a threshold
             on and extract events with amplitudes above the threshold.
+        mergewindow : int, NoneType, optional
+            Window within which to merge triggers, in units of number of
+            time bins. Defaults to no merging. It is not recommended to
+            set this to above half of a trace length, as substantial
+            dead time may be accrued.
         
         """
+
         self._template = template
         self._psd = psd
         self._nthreshold = threshold
         self._tchan = tchan
 
         self._initialize_filter()
         self._threshold = self._nthreshold * self._resolution
@@ -469,19 +491,19 @@
             
             filtered = self._filter_traces(data)
 
             for kk, filt in enumerate(filtered):
 
                 if posthreshold:
                     ranges = EventBuilder._smart_trigger(
-                        filt, self._threshold,
+                        filt, self._threshold, mergewindow,
                     )
                 else:
                     ranges = EventBuilder._smart_trigger(
-                        -filt, -self._threshold,
+                        -filt, -self._threshold, mergewindow,
                     )
 
                 if len(ranges)==0:
                     break
 
                 for ind0, ind1 in zip(ranges[:, 0], ranges[:, 1]):
                     indmax = ind0 + np.argmax(filt[ind0:ind1])
```

### Comparing `splendaq-0.4.2/src/splendaq/daq/_oscilloscope.py` & `splendaq-0.4.3/src/splendaq/daq/_oscilloscope.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/src/splendaq/daq/_sequencer.py` & `splendaq-0.4.3/src/splendaq/daq/_sequencer.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/src/splendaq/io/_io.py` & `splendaq-0.4.3/src/splendaq/io/_io.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/src/splendaq/io/_liconvert/COPYING.txt` & `splendaq-0.4.3/src/splendaq/io/_liconvert/COPYING.txt`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/src/splendaq/io/_liconvert/liconvert_linux` & `splendaq-0.4.3/src/splendaq/io/_liconvert/liconvert_linux`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/src/splendaq/io/_liconvert/liconvert_macos` & `splendaq-0.4.3/src/splendaq/io/_liconvert/liconvert_macos`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/src/splendaq/io/_liconvert/liconvert_windows.exe` & `splendaq-0.4.3/src/splendaq/io/_liconvert/liconvert_windows.exe`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/src/splendaq.egg-info/PKG-INFO` & `splendaq-0.4.3/src/splendaq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splendaq
-Version: 0.4.2
+Version: 0.4.3
 Summary: Generalized offline data acquisition with a focus on the Moku
 Home-page: https://github.com/splendor-collab/splendaq
 Author: SPLENDOR Collaboration
 Maintainer: SPLENDOR Collaboration
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `splendaq-0.4.2/src/splendaq.egg-info/SOURCES.txt` & `splendaq-0.4.3/src/splendaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/tutorials/daq/dc_oscilloscope.ipynb` & `splendaq-0.4.3/tutorials/daq/dc_oscilloscope.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/tutorials/daq/event_building.ipynb` & `splendaq-0.4.3/tutorials/daq/event_building.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999291383219955%*

 * *Differences: {"'cells'": "{15: {'source': {insert: [(5, '    mergewindow=None, # save all triggered events, set "*

 * *            "to a positive integer to merge events that are within this window\\n')]}}}"}*

```diff
@@ -233,14 +233,15 @@
             "outputs": [],
             "source": [
                 "EB.acquire_pulses(\n",
                 "    template,\n",
                 "    psd,\n",
                 "    20, # 20-sigma threshold\n",
                 "    0, # trigger on channel index 0\n",
+                "    mergewindow=None, # save all triggered events, set to a positive integer to merge events that are within this window\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1426e3e5-9959-490a-831a-40f09064498e",
             "metadata": {},
```

### Comparing `splendaq-0.4.2/tutorials/daq/logging_data.ipynb` & `splendaq-0.4.3/tutorials/daq/logging_data.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/tutorials/daq/running_the_sequencer.ipynb` & `splendaq-0.4.3/tutorials/daq/running_the_sequencer.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/tutorials/daq/sequencer_settings.yaml` & `splendaq-0.4.3/tutorials/daq/sequencer_settings.yaml`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/tutorials/io/read_files.ipynb` & `splendaq-0.4.3/tutorials/io/read_files.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.2/tutorials/io/write_files.ipynb` & `splendaq-0.4.3/tutorials/io/write_files.ipynb`

 * *Files identical despite different names*

