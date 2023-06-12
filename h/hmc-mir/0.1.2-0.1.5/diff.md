# Comparing `tmp/hmc_mir-0.1.2.tar.gz` & `tmp/hmc_mir-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmc_mir-0.1.2.tar", last modified: Tue Jun  6 20:01:41 2023, max compression
+gzip compressed data, was "hmc_mir-0.1.5.tar", last modified: Tue Jun  6 22:53:30 2023, max compression
```

## Comparing `hmc_mir-0.1.2.tar` & `hmc_mir-0.1.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.670144 hmc_mir-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.670144 hmc_mir-0.1.2/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.670144 hmc_mir-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.670144 hmc_mir-0.1.2/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/source/_templates/autosummary/function.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.670144 hmc_mir-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/src/hmc_mir/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/src/hmc_mir/align/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/align/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/align/dtw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/align/flex_dtw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/align/hstw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/align/nwtw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/src/hmc_mir/bootleg_score/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/bootleg_score/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29368 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/bootleg_score/bootleg_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/src/hmc_mir/tsm_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/tsm_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/src/hmc_mir/tsm_tools/tsm_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/src/hmc_mir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-06 20:01:41.000000 hmc_mir-0.1.2/src/hmc_mir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-06 20:01:41.000000 hmc_mir-0.1.2/src/hmc_mir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:01:41.000000 hmc_mir-0.1.2/src/hmc_mir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-06 20:01:41.000000 hmc_mir-0.1.2/src/hmc_mir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 20:01:41.000000 hmc_mir-0.1.2/src/hmc_mir.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:41.674144 hmc_mir-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:33.000000 hmc_mir-0.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:30.458599 hmc_mir-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:30.450599 hmc_mir-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:30.450599 hmc_mir-0.1.5/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:30.454599 hmc_mir-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-06 22:53:30.458599 hmc_mir-0.1.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:30.454599 hmc_mir-0.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:30.454599 hmc_mir-0.1.5/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:30.450599 hmc_mir-0.1.5/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:30.454599 hmc_mir-0.1.5/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/docs/source/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-06 22:53:30.458599 hmc_mir-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:30.450599 hmc_mir-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:30.454599 hmc_mir-0.1.5/src/hmc_mir/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/src/hmc_mir/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:30.458599 hmc_mir-0.1.5/src/hmc_mir/align/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/src/hmc_mir/align/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/src/hmc_mir/align/dtw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/src/hmc_mir/align/flex_dtw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/src/hmc_mir/align/hstw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/src/hmc_mir/align/nwtw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:30.458599 hmc_mir-0.1.5/src/hmc_mir/bootleg_score/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/src/hmc_mir/bootleg_score/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29368 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/src/hmc_mir/bootleg_score/bootleg_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:30.458599 hmc_mir-0.1.5/src/hmc_mir/tsm_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/src/hmc_mir/tsm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/src/hmc_mir/tsm_tools/tsm_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:30.454599 hmc_mir-0.1.5/src/hmc_mir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-06 22:53:30.000000 hmc_mir-0.1.5/src/hmc_mir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-06 22:53:30.000000 hmc_mir-0.1.5/src/hmc_mir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 22:53:30.000000 hmc_mir-0.1.5/src/hmc_mir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-06 22:53:30.000000 hmc_mir-0.1.5/src/hmc_mir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 22:53:30.000000 hmc_mir-0.1.5/src/hmc_mir.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:30.458599 hmc_mir-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 22:53:21.000000 hmc_mir-0.1.5/tests/__init__.py
```

### Comparing `hmc_mir-0.1.2/.github/scripts/release.py` & `hmc_mir-0.1.5/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.2/.github/workflows/docs.yml` & `hmc_mir-0.1.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.2/LICENSE` & `hmc_mir-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.2/PKG-INFO` & `hmc_mir-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmc_mir
-Version: 0.1.2
+Version: 0.1.5
 Summary: Collection of tools developed by HMCs MIR Lab
 Home-page: https://github.com/HMC-MIR/hmc-mir-tools
 Project-URL: Bug Tracker, https://github.com/HMC-MIR/hmc-mir-tools/issues
 Project-URL: Changelog, https://github.com/HMC-MIR/hmc-mir-tools/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `hmc_mir-0.1.2/docs/Makefile` & `hmc_mir-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.2/docs/make.bat` & `hmc_mir-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.2/docs/source/_templates/autosummary/class.rst` & `hmc_mir-0.1.5/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.2/docs/source/_templates/autosummary/module.rst` & `hmc_mir-0.1.5/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.2/docs/source/conf.py` & `hmc_mir-0.1.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.2/setup.cfg` & `hmc_mir-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.2/src/hmc_mir/align/dtw.py` & `hmc_mir-0.1.5/src/hmc_mir/align/dtw.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.2/src/hmc_mir/align/flex_dtw.py` & `hmc_mir-0.1.5/src/hmc_mir/align/flex_dtw.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.2/src/hmc_mir/align/hstw.py` & `hmc_mir-0.1.5/src/hmc_mir/align/hstw.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.2/src/hmc_mir/align/nwtw.py` & `hmc_mir-0.1.5/src/hmc_mir/align/nwtw.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.2/src/hmc_mir/bootleg_score/bootleg_score.py` & `hmc_mir-0.1.5/src/hmc_mir/bootleg_score/bootleg_score.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.2/src/hmc_mir/tsm_tools/tsm_tools.py` & `hmc_mir-0.1.5/src/hmc_mir/tsm_tools/tsm_tools.py`

 * *Files 23% similar despite different names*

```diff
@@ -262,8 +262,146 @@
     '''
     
     xh, xp, _, _ = harmonic_percussive_separation(x)
     xh_stretched = tsm_phase_vocoder(xh, alpha)
     xp_stretched = tsm_overlap_add(xp, alpha)
     y = mix_recordings(xh_stretched, xp_stretched)
     
+    return y
+
+def estimateIF_var(S, sr, timestamps):
+    '''
+    Estimates the instantaneous frequencies in an STFT-like matrix when the analysis frames
+    are not evenly spaced.
+    
+    Args:
+        S: the STFT-like matrix, should only contain the lower half of the frequency bins
+        sr: sampling rate
+        timestamps: timestamps corresponding to each STFT column (in sec)
+    
+    Returns:
+        A matrix containing the estimated instantaneous frequency at each time-frequency bin. This matrix should contain one less column than S.
+    '''
+    assert S.shape[1] == len(timestamps)
+#    hop_sec = hop_samples / sr
+    fft_size = (S.shape[0] - 1) * 2
+    w_nom = np.arange(S.shape[0]) * sr / fft_size * 2 * np.pi
+    w_nom = w_nom.reshape((-1,1))    
+    unwrapped = np.angle(S[:,1:]) - np.angle(S[:,0:-1]) - w_nom * (timestamps[1:] - timestamps[0:-1]).reshape((1,-1))
+    wrapped = (unwrapped + np.pi) % (2 * np.pi) - np.pi
+    w_if = w_nom + wrapped / (timestamps[1:] - timestamps[0:-1]).reshape((1,-1))
+    return w_if
+
+def tsmvar_overlap_add(x, alignment, L = 220, fs = 22050):
+    '''
+    Time stretches the input signal using the overlap-add method according to a given alignment.
+    Uses a synthesis hop size that is half the value of L.
+    
+    Args:
+        x: the input signal (orchestra only)
+        alignment: a 2xN matrix specifying the desired alignment in seconds.  The first row indicates the timestamp
+            in the input signal, and the last row indicates where in the output signal the instant should occur.
+        L: the length of each analysis frame in samples
+        fs: sample rate of input signal
+    
+    Returns: 
+        The variable time-stretched signal y
+    '''
+    assert(L % 2 == 0), "Frame length must be even."
+    Hs = L // 2
+
+    # determine interpolation points
+    target_dur = alignment[1,-1] # in sec
+    target_start = alignment[1,0] # if a subsequence alignment, output will be zero until target_start (in sec)
+    numFrames = int((target_dur * fs - L) // Hs) + 1
+    analysisFrames = np.zeros((L, numFrames))
+    interp_pts = np.interp(np.arange(numFrames)*Hs/fs, alignment[1,:], alignment[0,:]) # left edge of analysis windows
+    
+    # compute analysis frames    
+    for i in range(numFrames):
+        if i*Hs/fs >= target_start:
+            offset = int(np.round(interp_pts[i] * fs))
+            offset = min(offset, len(x) - L)
+            analysisFrames[:, i] = x[offset: offset + L]
+
+    # reconstruction
+    synthesisFrames = analysisFrames * hann_window(L).reshape((-1,1)) # use broadcasting
+    y = np.zeros(Hs * (numFrames-1) + L)
+    for i in range(numFrames):
+        offset = i * Hs
+        y[offset:offset+L] += synthesisFrames[:,i]
+            
+    return y
+
+def tsmvar_phase_vocoder(x, alignment, L = 2048, fs = 22050):
+    '''
+    Time stretches the input signal using a phase vocoder according to a given alignment.  
+    Uses a synthesis hop size that is one-fourth the value of L.
+    
+    Args:
+        x: the input signal
+        alignment: a 2xN matrix specifying the desired alignment in seconds.  The first row indicates the timestamp
+            in the input signal, and the last row indicates where in the output signal the instant should occur.
+        L: the length of each analysis frame in samples
+        fs: sampling rate
+    
+    Return:
+        The variable time-stretched signal y
+    '''
+    assert(L % 4 == 0), "Frame length must be divisible by four."
+    Hs = L // 4
+
+    # determine interpolation points
+    target_dur = alignment[1,-1] # in sec
+    target_start_frm = int(np.ceil(alignment[1,0] * fs / Hs)) # if a subsequence alignment, output will be zero until target_start_frm
+    numFrames = int((target_dur * fs - L) // Hs) + 1
+    analysisFrames = np.zeros((numFrames, L))
+    interp_pts = np.interp(np.arange(numFrames)*Hs/fs, alignment[1,:], alignment[0,:]) # left edge of analysis windows
+
+    # compute analysis frames
+    for i in range(numFrames):
+        if i >= target_start_frm:
+            offset = int(np.round(interp_pts[i] * fs))
+            offset = min(offset, len(x) - L)
+            analysisFrames[i,:] = x[offset: offset + L]
+
+    # compute STFT
+    window = hann_window(L)
+    analysisFrames = analysisFrames * window.reshape((1,-1))
+    Xfull = np.fft.fft(analysisFrames, axis=1)
+    halfLen = L//2 + 1
+    X = Xfull[:,0:halfLen].T
+   
+    # compute modified STFT
+    w_if = estimateIF_var(X[:,target_start_frm:], fs, interp_pts[target_start_frm:]) # only for active frames
+    phase_mod = np.zeros(X.shape)
+    phase_mod[:,target_start_frm] = np.angle(X[:,target_start_frm])
+    for i in range(target_start_frm + 1, phase_mod.shape[1]):
+        phase_mod[:,i] = phase_mod[:,i-1] + w_if[:,i-target_start_frm-1] * Hs / fs
+    Xmod = np.abs(X) * np.exp(1j * phase_mod)
+    
+    # signal reconstruction
+    y = invert_stft(Xmod, Hs, window)
+    #y = lb.core.istft(Xmod, hop_length=Hs, center=False)
+    
+    return y
+
+def tsmvar_hybrid(x, alignment, sr=22050):
+    '''
+    Time stretches the input signal using a hybrid method that combines overlap-add and phase vocoding.
+    The time stretch factor is specified at each time instant by the provided alignment.
+    
+    Args:
+        x: the input signal
+        alignment: a 2xN matrix specifying the desired alignment in seconds.  The first row indicates the timestamp
+            in the input signal, and the last row indicates where in the output signal the instant should occur.
+        sr: sampling rate
+    
+    Returns:
+        The variable time-stretched signal y
+    '''
+    xh, xp, _, _ = harmonic_percussive_separation(x)
+    xh_stretched = tsmvar_phase_vocoder(xh, alignment)
+    xp_stretched = tsmvar_overlap_add(xp, alignment)
+    y = mix_recordings(xh_stretched, xp_stretched)
+    
     return y
```

### Comparing `hmc_mir-0.1.2/src/hmc_mir.egg-info/PKG-INFO` & `hmc_mir-0.1.5/src/hmc_mir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmc-mir
-Version: 0.1.2
+Version: 0.1.5
 Summary: Collection of tools developed by HMCs MIR Lab
 Home-page: https://github.com/HMC-MIR/hmc-mir-tools
 Project-URL: Bug Tracker, https://github.com/HMC-MIR/hmc-mir-tools/issues
 Project-URL: Changelog, https://github.com/HMC-MIR/hmc-mir-tools/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `hmc_mir-0.1.2/src/hmc_mir.egg-info/SOURCES.txt` & `hmc_mir-0.1.5/src/hmc_mir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

