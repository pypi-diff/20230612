# Comparing `tmp/psdist-0.1.6.tar.gz` & `tmp/psdist-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psdist-0.1.6.tar", last modified: Wed Jun  7 16:49:28 2023, max compression
+gzip compressed data, was "psdist-0.1.7.tar", last modified: Mon Jun 12 17:10:16 2023, max compression
```

## Comparing `psdist-0.1.6.tar` & `psdist-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-07 16:49:28.933718 psdist-0.1.6/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1070 2022-11-29 16:42:20.000000 psdist-0.1.6/LICENSE
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1078 2023-06-07 16:49:28.933603 psdist-0.1.6/PKG-INFO
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      619 2023-06-02 22:01:08.000000 psdist-0.1.6/README.md
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-07 16:49:28.932302 psdist-0.1.6/psdist/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       95 2023-03-02 16:46:32.000000 psdist-0.1.6/psdist/__init__.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4925 2023-01-17 23:20:27.000000 psdist-0.1.6/psdist/ap.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    12828 2023-06-02 13:20:42.000000 psdist-0.1.6/psdist/cloud.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1247 2023-01-17 19:53:50.000000 psdist-0.1.6/psdist/data.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    18125 2023-06-07 16:45:05.000000 psdist-0.1.6/psdist/image.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       53 2023-05-24 15:51:53.000000 psdist-0.1.6/psdist/sampling.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1344 2023-03-02 16:46:32.000000 psdist-0.1.6/psdist/utils.py
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-07 16:49:28.933450 psdist-0.1.6/psdist/visualization/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      156 2023-03-02 16:46:32.000000 psdist-0.1.6/psdist/visualization/__init__.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    16087 2023-06-05 16:13:18.000000 psdist-0.1.6/psdist/visualization/cloud.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    36316 2023-05-24 15:50:44.000000 psdist-0.1.6/psdist/visualization/grid.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    22591 2023-06-02 17:03:58.000000 psdist-0.1.6/psdist/visualization/image.py
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4152 2023-03-02 16:46:32.000000 psdist-0.1.6/psdist/visualization/visualization.py
-drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-07 16:49:28.932847 psdist-0.1.6/psdist.egg-info/
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1078 2023-06-07 16:49:28.000000 psdist-0.1.6/psdist.egg-info/PKG-INFO
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      455 2023-06-07 16:49:28.000000 psdist-0.1.6/psdist.egg-info/SOURCES.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        1 2023-06-07 16:49:28.000000 psdist-0.1.6/psdist.egg-info/dependency_links.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      110 2023-06-07 16:49:28.000000 psdist-0.1.6/psdist.egg-info/requires.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        7 2023-06-07 16:49:28.000000 psdist-0.1.6/psdist.egg-info/top_level.txt
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      716 2023-06-07 16:48:31.000000 psdist-0.1.6/pyproject.toml
--rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       38 2023-06-07 16:49:28.933756 psdist-0.1.6/setup.cfg
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-12 17:10:16.765851 psdist-0.1.7/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1070 2022-11-29 16:42:20.000000 psdist-0.1.7/LICENSE
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1078 2023-06-12 17:10:16.765692 psdist-0.1.7/PKG-INFO
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      619 2023-06-02 22:01:08.000000 psdist-0.1.7/README.md
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-12 17:10:16.763278 psdist-0.1.7/psdist/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       95 2023-03-02 16:46:32.000000 psdist-0.1.7/psdist/__init__.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4925 2023-01-17 23:20:27.000000 psdist-0.1.7/psdist/ap.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    13670 2023-06-12 16:59:09.000000 psdist-0.1.7/psdist/cloud.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1247 2023-01-17 19:53:50.000000 psdist-0.1.7/psdist/data.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    18125 2023-06-07 16:45:05.000000 psdist-0.1.7/psdist/image.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       53 2023-05-24 15:51:53.000000 psdist-0.1.7/psdist/sampling.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1789 2023-06-12 15:19:15.000000 psdist-0.1.7/psdist/utils.py
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-12 17:10:16.765308 psdist-0.1.7/psdist/visualization/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      156 2023-03-02 16:46:32.000000 psdist-0.1.7/psdist/visualization/__init__.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    16683 2023-06-12 16:10:44.000000 psdist-0.1.7/psdist/visualization/cloud.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    36316 2023-05-24 15:50:44.000000 psdist-0.1.7/psdist/visualization/grid.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)    22591 2023-06-02 17:03:58.000000 psdist-0.1.7/psdist/visualization/image.py
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     4152 2023-03-02 16:46:32.000000 psdist-0.1.7/psdist/visualization/visualization.py
+drwxr-xr-x   0 46h      (766147688) ORNL\Domain Users (1551083765)        0 2023-06-12 17:10:16.763929 psdist-0.1.7/psdist.egg-info/
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)     1078 2023-06-12 17:10:16.000000 psdist-0.1.7/psdist.egg-info/PKG-INFO
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      455 2023-06-12 17:10:16.000000 psdist-0.1.7/psdist.egg-info/SOURCES.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        1 2023-06-12 17:10:16.000000 psdist-0.1.7/psdist.egg-info/dependency_links.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      110 2023-06-12 17:10:16.000000 psdist-0.1.7/psdist.egg-info/requires.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)        7 2023-06-12 17:10:16.000000 psdist-0.1.7/psdist.egg-info/top_level.txt
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)      716 2023-06-12 17:09:46.000000 psdist-0.1.7/pyproject.toml
+-rw-r--r--   0 46h      (766147688) ORNL\Domain Users (1551083765)       38 2023-06-12 17:10:16.765902 psdist-0.1.7/setup.cfg
```

### Comparing `psdist-0.1.6/LICENSE` & `psdist-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `psdist-0.1.6/PKG-INFO` & `psdist-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psdist
-Version: 0.1.6
+Version: 0.1.7
 Summary: Analysis/visualization of phase space distributions
 Author-email: Austin Hoover <ahoover1218@gmail.com>
 Project-URL: homepage, https://github.com/austin-hoover/psdist
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `psdist-0.1.6/README.md` & `psdist-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `psdist-0.1.6/psdist/ap.py` & `psdist-0.1.7/psdist/ap.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.6/psdist/cloud.py` & `psdist-0.1.7/psdist/cloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Functions for point clouds."""
 import numpy as np
 import scipy.interpolate
+import scipy.special
 import scipy.stats
 
 from psdist import ap
+import psdist.utils as utils
 from psdist.utils import array_like
 from psdist.utils import centers_from_edges
 from psdist.utils import cov2corr
 from psdist.utils import random_selection
 
 
 # Analysis
@@ -423,33 +425,41 @@
 
 # Density estimation
 # ------------------------------------------------------------------------------
 
 
 def histogram_bin_edges(X, bins=10, limits=None):
     """Multi-dimensional histogram bin edges."""
+    if X.ndim == 1:
+        return np.histogram_bin_edges(X, bins, limits)
     if not array_like(bins):
         bins = X.shape[1] * [bins]
     if not array_like(limits):
         limits = X.shape[1] * [limits]
     return [
         np.histogram_bin_edges(X[:, i], bins[i], limits[i]) 
         for i in range(X.shape[1])
     ]
 
 
 def histogram(X, bins=10, limits=None, centers=False):
     """Multi-dimensional histogram."""
-    edges = histogram_bin_edges(X, bins=bins, limits=limits)
-    hist, edges = np.histogramdd(X, edges)
+    if X.ndim == 1:
+        bins = np.histogram_bin_edges(X, bins, limits)
+        hist, _ = np.histogram(X, bins=bins)
+        if centers:
+            bins = centers_from_edges(bins)
+        return hist, bins
+    
+    bins = histogram_bin_edges(X, bins=bins, limits=limits)
+    hist, _ = np.histogramdd(X, bins)
     if centers:
-        return hist, [centers_from_edges(e) for e in edges]
-    else:
-        return hist, edges
-
+        bins = [centers_from_edges(b) for b in bins]
+    return hist, bins
+    
 
 def gaussian_kde(X, **kws):
     """Gaussian kernel density estimation (KDE).
 
     This function just calls `scipy.stats.gaussian_kde`.
 
     Parameters
@@ -461,7 +471,25 @@
 
     Returns
     -------
     estimator : scipy.stats.gaussian_kde
         The density estimator.
     """
     return scipy.stats.gaussian_kde(X.T, **kws)
+
+
+def radial_histogram(X, axis=None, **kws):
+    if axis is None:
+        axis = tuple(range(X.shape[1]))
+    radii = get_radii(X[:, axis])
+    _centers = False
+    if "centers" in kws:
+        _centers = kws.pop("centers")
+        
+    hist, bins = histogram(radii, **kws)
+    for i in range(len(bins) - 1):
+        rmin = bins[i]
+        rmax = bins[i + 1]
+        hist[i] = hist[i] / utils.volume_sphere_shell(rmin=rmin, rmax=rmax, n=len(axis))
+    if _centers:
+        bins = centers_from_edges(bins)
+    return hist, bins
```

### Comparing `psdist-0.1.6/psdist/data.py` & `psdist-0.1.7/psdist/data.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.6/psdist/image.py` & `psdist-0.1.7/psdist/image.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.6/psdist/utils.py` & `psdist-0.1.7/psdist/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import scipy.special
 
 
 def centers_from_edges(edges):
     """Compute bin centers from evenly spaced bin edges."""
     return 0.5 * (edges[:-1] + edges[1:])
 
 
@@ -41,8 +42,23 @@
     """Compute correlation matrix from covariance matrix."""
     D = np.sqrt(np.diag(cov_mat.diagonal()))
     Dinv = np.linalg.inv(D)
     return np.linalg.multi_dot([Dinv, cov_mat, Dinv])
 
 
 def array_like(a):
-    return np.ndim(np.array(a, dtype=object)) > 0
+    return np.ndim(np.array(a, dtype=object)) > 0
+
+
+def surface_area_sphere(r=1.0, n=3):
+    factor = (2.0 * np.pi ** (0.5 * (n + 1))) 
+    factor = factor / scipy.special.gamma(0.5 * (n + 1))
+    return factor * (r ** n)
+
+
+def volume_sphere(r=1.0, n=3):
+    factor = (np.pi ** (0.5 * n)) / scipy.special.gamma(1.0 + 0.5 * n)
+    return factor * (r ** n)
+
+
+def volume_sphere_shell(rmin=0.0, rmax=1.0, n=3):
+    return volume_sphere(r=rmax, n=n) - volume_sphere(r=rmin, n=n)
```

### Comparing `psdist-0.1.6/psdist/visualization/cloud.py` & `psdist-0.1.7/psdist/visualization/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,14 +288,16 @@
 
 
 def proj2d_interactive_slice(
     data=None,
     limits=None,
     default_ind=(0, 1),
     slice_type="int",
+    plot_res=64,
+    slice_res=16,
     dims=None,
     units=None,
     autolim_kws=None,
     fig_kws=None,
     **plot_kws,
 ):
     """2D partial projection with interactive slicing.
@@ -308,14 +310,17 @@
         comparision. There is no limit on the number of figures!
     limits : list[(min, max)]
         Limits along each axis.
     default_ind : (i, j)
         Default view axis.
     slice_type : {'int', 'range'}
         Whether to slice one index along the axis or a range of indices.
+    plot_res, slice_res : int
+        Default grid resolution for plotting/slicing. These can be updated using
+        the interactive widgets.
     dims, units : list[str], shape (n,)
         Dimension names and units.
     autolim_kws : dict
         Key word arguments passed to `auto_limits`.
     fig_kws : dict
         Key word arguments passed to `proplot.subplots`.
     **plot_kws
@@ -348,24 +353,24 @@
     for dim, unit in zip(dims, units):
         dims_units.append(f"{dim}" + f" [{unit}]" if unit != "" else dim)
 
     # Widgets
     dim1 = widgets.Dropdown(options=dims, index=default_ind[0], description="dim 1")
     dim2 = widgets.Dropdown(options=dims, index=default_ind[1], description="dim 2")
     n_bins = widgets.BoundedIntText(
-        value=32,
+        value=slice_res,
         min=2,
-        max=150,
+        max=200,
         step=1,
         description="slice res",
     )    
     n_bins_plot = widgets.BoundedIntText(
-        value=50,
+        value=plot_res,
         min=2,
-        max=250,
+        max=350,
         step=1,
         description="plot res",
     )    
     autobin = widgets.Checkbox(description="auto plot res", value=False)
     log = widgets.Checkbox(description="log", value=False)
     sliders, checks = [], []
     for k in range(n_dims):
@@ -420,15 +425,15 @@
     def update(**kws):
         dim1 = kws["dim1"]
         dim2 = kws["dim2"]
         n_bins = kws["n_bins"]
         n_bins_plot = kws["n_bins_plot"]
         autobin = kws["autobin"]
 
-        # Update the slider ranges based on n_bins.
+        # Update the slider ranges/values based on n_bins.
         for slider in sliders:
             slider.max = n_bins - 1
 
         # Collect slice indices.
         ind, checks = [], []
         for i in range(1, n_dims + 1):
             if f"check{i}" in kws:
@@ -467,14 +472,21 @@
                 return
 
         # Update plotting key word arguments.
         if plot_kws["kind"] != "scatter":
             plot_kws["bins"] = "auto" if autobin else n_bins_plot
             plot_kws["limits"] = [limits[axis_view[0]], limits[axis_view[1]]]
             plot_kws["norm"] = "log" if kws["log"] else None
+            
+            # Temporary bug fix. (If we check and then uncheck "log", and 
+            # the colorbar has minor ticks, the tick label formatter will
+            # remain in "log" mode forever after.)
+            if "colorbar_kw" in plot_kws:
+                if "tickminor" in plot_kws["colorbar_kw"] and not kws["log"]:
+                    plot_kws["colorbar_kw"]["formatter"] = None
 
         # Plot the selected points.
         fig, axs = pplt.subplots(ncols=n_data, **fig_kws)
         for ax, _X in zip(axs, _data):
             plot2d(_X[:, axis_view], ax=ax, **plot_kws)
         axs.format(xlabel=dims_units[axis_view[0]], ylabel=dims_units[axis_view[1]])
         plt.show()
```

### Comparing `psdist-0.1.6/psdist/visualization/grid.py` & `psdist-0.1.7/psdist/visualization/grid.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.6/psdist/visualization/image.py` & `psdist-0.1.7/psdist/visualization/image.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.6/psdist/visualization/visualization.py` & `psdist-0.1.7/psdist/visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `psdist-0.1.6/psdist.egg-info/PKG-INFO` & `psdist-0.1.7/psdist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psdist
-Version: 0.1.6
+Version: 0.1.7
 Summary: Analysis/visualization of phase space distributions
 Author-email: Austin Hoover <ahoover1218@gmail.com>
 Project-URL: homepage, https://github.com/austin-hoover/psdist
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `psdist-0.1.6/pyproject.toml` & `psdist-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psdist"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Austin Hoover", email="ahoover1218@gmail.com" },
 ]
 description = "Analysis/visualization of phase space distributions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

