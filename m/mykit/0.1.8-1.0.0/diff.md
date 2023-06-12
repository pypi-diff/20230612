# Comparing `tmp/mykit-0.1.8.tar.gz` & `tmp/mykit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mykit-0.1.8.tar", last modified: Mon Jun 12 17:45:39 2023, max compression
+gzip compressed data, was "mykit-1.0.0.tar", last modified: Mon Jun 12 18:23:13 2023, max compression
```

## Comparing `mykit-0.1.8.tar` & `mykit-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 17:45:39.023746 mykit-0.1.8/
--rw-rw-rw-   0        0        0     1097 2023-04-10 22:01:23.000000 mykit-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     3097 2023-06-12 17:45:39.023746 mykit-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1984 2023-06-12 14:07:52.000000 mykit-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 17:45:38.783685 mykit-0.1.8/mykit/
--rw-rw-rw-   0        0        0      204 2023-06-12 13:37:25.000000 mykit-0.1.8/mykit/__init__.py
--rw-rw-rw-   0        0        0      134 2023-06-12 16:47:42.000000 mykit-0.1.8/mykit/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:45:38.942724 mykit-0.1.8/mykit/app/
--rw-rw-rw-   0        0        0     4152 2023-06-12 13:55:45.000000 mykit-0.1.8/mykit/app/arrow.py
--rw-rw-rw-   0        0        0    12892 2023-06-12 14:04:51.000000 mykit-0.1.8/mykit/app/button.py
--rw-rw-rw-   0        0        0     9010 2023-06-12 14:04:57.000000 mykit-0.1.8/mykit/app/label.py
--rw-rw-rw-   0        0        0    28006 2023-06-12 14:05:24.000000 mykit-0.1.8/mykit/app/slider.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:45:38.996739 mykit-0.1.8/mykit/kit/
--rw-rw-rw-   0        0        0     2965 2023-06-12 13:39:03.000000 mykit-0.1.8/mykit/kit/color.py
--rw-rw-rw-   0        0        0     5809 2023-06-12 11:57:08.000000 mykit-0.1.8/mykit/kit/ffmpeg.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:45:39.002744 mykit-0.1.8/mykit/kit/graph/
--rw-rw-rw-   0        0        0    16521 2023-06-12 12:03:05.000000 mykit-0.1.8/mykit/kit/graph/graph2d.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:45:39.006740 mykit-0.1.8/mykit/kit/keycrate/
--rw-rw-rw-   0        0        0     6473 2023-06-12 14:01:25.000000 mykit-0.1.8/mykit/kit/keycrate/__init__.py
--rw-rw-rw-   0        0        0     2741 2023-06-12 12:12:05.000000 mykit-0.1.8/mykit/kit/math.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:45:39.016749 mykit-0.1.8/mykit/kit/neuralnet/
--rw-rw-rw-   0        0        0     7320 2023-06-12 14:05:32.000000 mykit-0.1.8/mykit/kit/neuralnet/dense.py
--rw-rw-rw-   0        0        0    15109 2023-06-12 14:05:43.000000 mykit-0.1.8/mykit/kit/neuralnet/genetic.py
--rw-rw-rw-   0        0        0     3039 2023-05-06 18:30:49.000000 mykit-0.1.8/mykit/kit/noise.py
--rw-rw-rw-   0        0        0     4253 2023-05-18 13:55:09.000000 mykit-0.1.8/mykit/kit/path.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:45:39.020745 mykit-0.1.8/mykit/kit/quick_visual/
--rw-rw-rw-   0        0        0      841 2023-06-12 14:06:19.000000 mykit-0.1.8/mykit/kit/quick_visual/plot2d.py
--rw-rw-rw-   0        0        0      403 2023-06-11 18:43:02.000000 mykit-0.1.8/mykit/kit/text.py
--rw-rw-rw-   0        0        0     2453 2023-06-12 11:34:47.000000 mykit-0.1.8/mykit/kit/time.py
--rw-rw-rw-   0        0        0     3156 2023-05-18 13:20:09.000000 mykit-0.1.8/mykit/kit/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:45:38.926720 mykit-0.1.8/mykit.egg-info/
--rw-rw-rw-   0        0        0     3097 2023-06-12 17:45:38.000000 mykit-0.1.8/mykit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-06-12 17:45:38.000000 mykit-0.1.8/mykit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 17:45:38.000000 mykit-0.1.8/mykit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-12 17:45:38.000000 mykit-0.1.8/mykit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2023-06-12 17:45:38.000000 mykit-0.1.8/mykit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-12 17:45:38.000000 mykit-0.1.8/mykit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1188 2023-06-12 17:45:19.000000 mykit-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      161 2023-06-12 17:45:39.027745 mykit-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-06-12 16:59:26.000000 mykit-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:23:13.758348 mykit-1.0.0/
+-rw-rw-rw-   0        0        0     1097 2023-04-10 22:01:23.000000 mykit-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3669 2023-06-12 18:23:13.759348 mykit-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2556 2023-06-12 18:17:04.000000 mykit-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 18:23:13.556296 mykit-1.0.0/mykit/
+-rw-rw-rw-   0        0        0      223 2023-06-12 18:01:09.000000 mykit-1.0.0/mykit/__init__.py
+-rw-rw-rw-   0        0        0      346 2023-06-12 18:02:00.000000 mykit-1.0.0/mykit/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:23:13.692330 mykit-1.0.0/mykit/app/
+-rw-rw-rw-   0        0        0     4152 2023-06-12 13:55:45.000000 mykit-1.0.0/mykit/app/arrow.py
+-rw-rw-rw-   0        0        0    12892 2023-06-12 14:04:51.000000 mykit-1.0.0/mykit/app/button.py
+-rw-rw-rw-   0        0        0     9010 2023-06-12 14:04:57.000000 mykit-1.0.0/mykit/app/label.py
+-rw-rw-rw-   0        0        0    28006 2023-06-12 14:05:24.000000 mykit-1.0.0/mykit/app/slider.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:23:13.730340 mykit-1.0.0/mykit/kit/
+-rw-rw-rw-   0        0        0     2965 2023-06-12 13:39:03.000000 mykit-1.0.0/mykit/kit/color.py
+-rw-rw-rw-   0        0        0     5809 2023-06-12 11:57:08.000000 mykit-1.0.0/mykit/kit/ffmpeg.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:23:13.733341 mykit-1.0.0/mykit/kit/graph/
+-rw-rw-rw-   0        0        0    16521 2023-06-12 12:03:05.000000 mykit-1.0.0/mykit/kit/graph/graph2d.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:23:13.739342 mykit-1.0.0/mykit/kit/keycrate/
+-rw-rw-rw-   0        0        0     6473 2023-06-12 14:01:25.000000 mykit-1.0.0/mykit/kit/keycrate/__init__.py
+-rw-rw-rw-   0        0        0     2741 2023-06-12 12:12:05.000000 mykit-1.0.0/mykit/kit/math.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:23:13.748345 mykit-1.0.0/mykit/kit/neuralnet/
+-rw-rw-rw-   0        0        0     7320 2023-06-12 14:05:32.000000 mykit-1.0.0/mykit/kit/neuralnet/dense.py
+-rw-rw-rw-   0        0        0    15109 2023-06-12 14:05:43.000000 mykit-1.0.0/mykit/kit/neuralnet/genetic.py
+-rw-rw-rw-   0        0        0     3039 2023-05-06 18:30:49.000000 mykit-1.0.0/mykit/kit/noise.py
+-rw-rw-rw-   0        0        0     4253 2023-05-18 13:55:09.000000 mykit-1.0.0/mykit/kit/path.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:23:13.752346 mykit-1.0.0/mykit/kit/quick_visual/
+-rw-rw-rw-   0        0        0      863 2023-06-12 17:50:58.000000 mykit-1.0.0/mykit/kit/quick_visual/plot2d.py
+-rw-rw-rw-   0        0        0      403 2023-06-11 18:43:02.000000 mykit-1.0.0/mykit/kit/text.py
+-rw-rw-rw-   0        0        0     2453 2023-06-12 11:34:47.000000 mykit-1.0.0/mykit/kit/time.py
+-rw-rw-rw-   0        0        0     3156 2023-05-18 13:20:09.000000 mykit-1.0.0/mykit/kit/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:23:13.664322 mykit-1.0.0/mykit.egg-info/
+-rw-rw-rw-   0        0        0     3669 2023-06-12 18:23:13.000000 mykit-1.0.0/mykit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-06-12 18:23:13.000000 mykit-1.0.0/mykit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 18:23:13.000000 mykit-1.0.0/mykit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-12 18:23:13.000000 mykit-1.0.0/mykit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-06-12 18:23:13.000000 mykit-1.0.0/mykit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 18:23:13.000000 mykit-1.0.0/mykit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1188 2023-06-12 17:47:07.000000 mykit-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      161 2023-06-12 18:23:13.762347 mykit-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-06-12 16:59:26.000000 mykit-1.0.0/setup.py
```

### Comparing `mykit-0.1.8/LICENSE` & `mykit-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-0.1.8/PKG-INFO` & `mykit-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 0.1.8
+Version: 1.0.0
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: report bugs, https://github.com/nvfp/mykit/issues
@@ -24,30 +24,49 @@
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # myKit
 
+[![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
+[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
+
+Python utility toolkit.
 
 
 ## Installation
 
+```sh
+pip install mykit
+```
 
 
 ## Usage
 
+```python
+from mykit.kit.text import byteFmt
+from mykit.app.arrow import Arrow
+from mykit.app.slider import Slider
+
+
+x = byteFmt(3141592653589793)
+print(x)  # 2.79 PiB
+```
 
 
 ## FAQ
 
+- 
 
 
 ## Changelog
 
+- 1.0.0 (June 12, 2023):
+    - `kit/quick_visual/plot2d.py`: changed argument name: `graph2d_cfg` -> `cfg`
 - 0.1.3 (June 12, 2023):
     - removed `get_gray` from `mykit/mykit/kit/color.py`
     - transform `mykit/mykit/kit/gui/button/` -> `mykit/mykit/app/button.py`
     - transform `mykit/mykit/kit/gui/label/` -> `mykit/mykit/app/label.py`
     - transform `mykit/mykit/kit/gui/slider/` -> `mykit/mykit/app/slider.py`
     - transform `mykit/mykit/kit/gui/shape/` -> `mykit/mykit/app/arrow.py`
     - transform `mykit/mykit/kit/neuralnet/dense/` -> `mykit/mykit/kit/neuralnet/dense.py`
```

### Comparing `mykit-0.1.8/mykit/app/arrow.py` & `mykit-1.0.0/mykit/app/arrow.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.8/mykit/app/button.py` & `mykit-1.0.0/mykit/app/button.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.8/mykit/app/label.py` & `mykit-1.0.0/mykit/app/label.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.8/mykit/app/slider.py` & `mykit-1.0.0/mykit/app/slider.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.8/mykit/kit/color.py` & `mykit-1.0.0/mykit/kit/color.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.8/mykit/kit/ffmpeg.py` & `mykit-1.0.0/mykit/kit/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.8/mykit/kit/graph/graph2d.py` & `mykit-1.0.0/mykit/kit/graph/graph2d.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.8/mykit/kit/keycrate/__init__.py` & `mykit-1.0.0/mykit/kit/keycrate/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.8/mykit/kit/math.py` & `mykit-1.0.0/mykit/kit/math.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.8/mykit/kit/neuralnet/dense.py` & `mykit-1.0.0/mykit/kit/neuralnet/dense.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.8/mykit/kit/neuralnet/genetic.py` & `mykit-1.0.0/mykit/kit/neuralnet/genetic.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.8/mykit/kit/noise.py` & `mykit-1.0.0/mykit/kit/noise.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.8/mykit/kit/path.py` & `mykit-1.0.0/mykit/kit/path.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.8/mykit/kit/quick_visual/plot2d.py` & `mykit-1.0.0/mykit/kit/quick_visual/plot2d.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import tkinter as _tk
-from typing import Optional as _Optional
 
-from mykit.kit.graph.graph2d import graph2d as _graph2d
+from mykit.kit.graph.graph2d import Graph2D as _Graph2D
 
 
 def plot2d(
     points: list[tuple[float, float]],
     xspan = 0.80,
     yspan = 0.65,
-    graph2d_cfg: dict = {}
+    cfg: dict = {}
 ):
+    """`cfg`: extra configurations for Graph2D"""
 
     root = _tk.Tk()
     root.attributes('-fullscreen', True)
 
     mon_width = root.winfo_screenwidth()
     mon_height = root.winfo_screenheight()
 
     page = _tk.Canvas(width=mon_width, height=mon_height, bg='#121212', highlightthickness=0, borderwidth=0)
     page.place(x=0, y=0)
 
+    _Graph2D.set_page(page)
+
 
     WIDTH = mon_width*xspan
     HEIGHT = mon_height*yspan
     TL_X = (mon_width - WIDTH)/2
     TL_Y = (mon_height - HEIGHT)/2
-    _graph2d(page, points, width=WIDTH, height=HEIGHT, pos=(TL_X, TL_Y), **graph2d_cfg)
+    _Graph2D(points, width=WIDTH, height=HEIGHT, tl_x=TL_X, tl_y=TL_Y, **cfg)
 
 
     root.bind('<Escape>', lambda e: root.destroy())
     root.mainloop()
```

### Comparing `mykit-0.1.8/mykit/kit/time.py` & `mykit-1.0.0/mykit/kit/time.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.8/mykit/kit/utils.py` & `mykit-1.0.0/mykit/kit/utils.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.8/mykit.egg-info/PKG-INFO` & `mykit-1.0.0/mykit.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 0.1.8
+Version: 1.0.0
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: report bugs, https://github.com/nvfp/mykit/issues
@@ -24,30 +24,49 @@
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # myKit
 
+[![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
+[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
+
+Python utility toolkit.
 
 
 ## Installation
 
+```sh
+pip install mykit
+```
 
 
 ## Usage
 
+```python
+from mykit.kit.text import byteFmt
+from mykit.app.arrow import Arrow
+from mykit.app.slider import Slider
+
+
+x = byteFmt(3141592653589793)
+print(x)  # 2.79 PiB
+```
 
 
 ## FAQ
 
+- 
 
 
 ## Changelog
 
+- 1.0.0 (June 12, 2023):
+    - `kit/quick_visual/plot2d.py`: changed argument name: `graph2d_cfg` -> `cfg`
 - 0.1.3 (June 12, 2023):
     - removed `get_gray` from `mykit/mykit/kit/color.py`
     - transform `mykit/mykit/kit/gui/button/` -> `mykit/mykit/app/button.py`
     - transform `mykit/mykit/kit/gui/label/` -> `mykit/mykit/app/label.py`
     - transform `mykit/mykit/kit/gui/slider/` -> `mykit/mykit/app/slider.py`
     - transform `mykit/mykit/kit/gui/shape/` -> `mykit/mykit/app/arrow.py`
     - transform `mykit/mykit/kit/neuralnet/dense/` -> `mykit/mykit/kit/neuralnet/dense.py`
```

### Comparing `mykit-0.1.8/mykit.egg-info/SOURCES.txt` & `mykit-1.0.0/mykit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mykit-0.1.8/pyproject.toml` & `mykit-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mykit"
-version = "0.1.8"
+version = "1.0.0"
 description = "Python utility library"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

