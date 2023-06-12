# Comparing `tmp/junkie-rfglab-2023.6.3.tar.gz` & `tmp/junkie-rfglab-2023.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junkie-rfglab-2023.6.3.tar", last modified: Mon Jun 12 02:19:47 2023, max compression
+gzip compressed data, was "junkie-rfglab-2023.6.4.tar", last modified: Mon Jun 12 02:31:48 2023, max compression
```

## Comparing `junkie-rfglab-2023.6.3.tar` & `junkie-rfglab-2023.6.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-12 02:19:47.349114 junkie-rfglab-2023.6.3/
--rw-r--r--   0 rodrigo    (501) staff       (20)    33148 2023-05-12 19:44:56.000000 junkie-rfglab-2023.6.3/LICENSE
--rw-r--r--   0 rodrigo    (501) staff       (20)     3537 2023-06-12 02:19:47.348986 junkie-rfglab-2023.6.3/PKG-INFO
--rw-r--r--   0 rodrigo    (501) staff       (20)     2949 2023-06-11 21:38:08.000000 junkie-rfglab-2023.6.3/README.md
--rw-r--r--   0 rodrigo    (501) staff       (20)    11354 2023-06-12 02:19:37.000000 junkie-rfglab-2023.6.3/junkie.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-12 02:19:47.348850 junkie-rfglab-2023.6.3/junkie_rfglab.egg-info/
--rw-r--r--   0 rodrigo    (501) staff       (20)     3537 2023-06-12 02:19:47.000000 junkie-rfglab-2023.6.3/junkie_rfglab.egg-info/PKG-INFO
--rw-r--r--   0 rodrigo    (501) staff       (20)      226 2023-06-12 02:19:47.000000 junkie-rfglab-2023.6.3/junkie_rfglab.egg-info/SOURCES.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)        1 2023-06-12 02:19:47.000000 junkie-rfglab-2023.6.3/junkie_rfglab.egg-info/dependency_links.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)       69 2023-06-12 02:19:47.000000 junkie-rfglab-2023.6.3/junkie_rfglab.egg-info/requires.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)        7 2023-06-12 02:19:47.000000 junkie-rfglab-2023.6.3/junkie_rfglab.egg-info/top_level.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)      840 2023-06-12 01:43:28.000000 junkie-rfglab-2023.6.3/pyproject.toml
--rw-r--r--   0 rodrigo    (501) staff       (20)       38 2023-06-12 02:19:47.349147 junkie-rfglab-2023.6.3/setup.cfg
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-12 02:31:48.507866 junkie-rfglab-2023.6.4/
+-rw-r--r--   0 rodrigo    (501) staff       (20)    33148 2023-05-12 19:44:56.000000 junkie-rfglab-2023.6.4/LICENSE
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3537 2023-06-12 02:31:48.507744 junkie-rfglab-2023.6.4/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2949 2023-06-11 21:38:08.000000 junkie-rfglab-2023.6.4/README.md
+-rw-r--r--   0 rodrigo    (501) staff       (20)    11583 2023-06-12 02:31:09.000000 junkie-rfglab-2023.6.4/junkie.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-12 02:31:48.507609 junkie-rfglab-2023.6.4/junkie_rfglab.egg-info/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3537 2023-06-12 02:31:48.000000 junkie-rfglab-2023.6.4/junkie_rfglab.egg-info/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) staff       (20)      226 2023-06-12 02:31:48.000000 junkie-rfglab-2023.6.4/junkie_rfglab.egg-info/SOURCES.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)        1 2023-06-12 02:31:48.000000 junkie-rfglab-2023.6.4/junkie_rfglab.egg-info/dependency_links.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)       69 2023-06-12 02:31:48.000000 junkie-rfglab-2023.6.4/junkie_rfglab.egg-info/requires.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)        7 2023-06-12 02:31:48.000000 junkie-rfglab-2023.6.4/junkie_rfglab.egg-info/top_level.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)      840 2023-06-12 01:43:28.000000 junkie-rfglab-2023.6.4/pyproject.toml
+-rw-r--r--   0 rodrigo    (501) staff       (20)       38 2023-06-12 02:31:48.507901 junkie-rfglab-2023.6.4/setup.cfg
```

### Comparing `junkie-rfglab-2023.6.3/LICENSE` & `junkie-rfglab-2023.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `junkie-rfglab-2023.6.3/PKG-INFO` & `junkie-rfglab-2023.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junkie-rfglab
-Version: 2023.6.3
+Version: 2023.6.4
 Summary: junkie is a JUpyter NotebooK Image Explorer
 Author-email: Rodrigo Fernandez-Gonzalez <rodrigo.fernandez.gonzalez@utoronto.ca>
 Project-URL: Homepage, https://bitbucket.com/rfg_lab/junkie
 Project-URL: Bug Tracker, https://bitbucket.com/rfg_lab/junkie/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `junkie-rfglab-2023.6.3/README.md` & `junkie-rfglab-2023.6.4/README.md`

 * *Files identical despite different names*

### Comparing `junkie-rfglab-2023.6.3/junkie.py` & `junkie-rfglab-2023.6.4/junkie.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import skimage
 import IPython.display as IPyd
 import ipywidgets as ipyw
 import matplotlib.pyplot as plt
 
-__version__: str = '2023.6.3'  # this must be here for pyproject.toml to find it.
+__version__: str = '2023.6.4'  # this must be here for pyproject.toml to find it.
 
 
 # You will need this line in your jupyter notebook: %matplotlib widget
 
 class junkie:
     """ 
     junkie: a JUpyter NotebooK Image Explorer
@@ -26,24 +26,29 @@
     channel_strs = tuple of strings to distinguish files from different channels 
       (if opening a multichannel image from a file sequence)
     cmap = default('gray'), string for the matplotlib colormap
     figsize = default(4,4), to set the size of the figure
     
     """
     
+    __version__ = __version__  # defines junkie.__version__
+
     next_figure_index: str = 1
     orientations = {'x-y': [0, 1, 2], 'z-x': [1, 2, 0], 'z-y': [2, 1, 0]}
     button_layout = {'width': 'auto', 'height': '32px'}
     button_style = {'font_size': '12px'}
     image_extensions: Tuple[str] = ('.tif', '.tiff', '.jpg', '.jpeg', '.gif', '.png', '.bmp')
     
     def __init__(self, volume: np.ndarray|str, channel_strs: Optional[Tuple[str]] = ('', ), cmap:str = 'gray', figsize: Tuple[int, int] =(4,4)):
         # if volume is a str, read it as an image.
         if isinstance(volume, str):
             volume = self.read_image(volume, channel_strs)
+            if volume is None:
+                # throw exception instead.
+                print(f'No volume found at that path. The current path is {os.path.curdir}.')
 
         plt.style.use('dark_background')
         self.volume: np.ndarray = volume
         self.slices: np.ndarray = None
 
         match self.volume.ndim:
             case 1:
```

### Comparing `junkie-rfglab-2023.6.3/junkie_rfglab.egg-info/PKG-INFO` & `junkie-rfglab-2023.6.4/junkie_rfglab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junkie-rfglab
-Version: 2023.6.3
+Version: 2023.6.4
 Summary: junkie is a JUpyter NotebooK Image Explorer
 Author-email: Rodrigo Fernandez-Gonzalez <rodrigo.fernandez.gonzalez@utoronto.ca>
 Project-URL: Homepage, https://bitbucket.com/rfg_lab/junkie
 Project-URL: Bug Tracker, https://bitbucket.com/rfg_lab/junkie/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `junkie-rfglab-2023.6.3/pyproject.toml` & `junkie-rfglab-2023.6.4/pyproject.toml`

 * *Files identical despite different names*

