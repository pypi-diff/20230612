# Comparing `tmp/glue-small-multiples-1.1.2.tar.gz` & `tmp/glue-small-multiples-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue-small-multiples-1.1.2.tar", last modified: Thu May 11 13:39:04 2023, max compression
+gzip compressed data, was "glue-small-multiples-1.2.1.tar", last modified: Mon Jun 12 19:16:39 2023, max compression
```

## Comparing `glue-small-multiples-1.1.2.tar` & `glue-small-multiples-1.2.1.tar`

### file list

```diff
@@ -1,35 +1,42 @@
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-05-11 13:39:04.696155 glue-small-multiples-1.1.2/
--rw-r--r--   0 jfoster    (501) staff       (20)     1820 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/.gitignore
--rw-r--r--   0 jfoster    (501) staff       (20)      229 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/CHANGES.md
--rw-r--r--   0 jfoster    (501) staff       (20)     1023 2023-05-11 13:39:04.696248 glue-small-multiples-1.1.2/PKG-INFO
--rw-r--r--   0 jfoster    (501) staff       (20)      259 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/README.md
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-05-11 13:39:04.693801 glue-small-multiples-1.1.2/glue_small_multiples/
--rw-r--r--   0 jfoster    (501) staff       (20)      145 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/__init__.py
--rw-r--r--   0 jfoster    (501) staff       (20)    16789 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/layer_artist.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-05-11 13:39:04.695490 glue-small-multiples-1.1.2/glue_small_multiples/qt/
--rw-r--r--   0 jfoster    (501) staff       (20)        0 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/__init__.py
--rw-r--r--   0 jfoster    (501) staff       (20)    10367 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/layer_style_editor.py
--rw-r--r--   0 jfoster    (501) staff       (20)    31901 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/layer_style_editor.ui
--rw-r--r--   0 jfoster    (501) staff       (20)      643 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/options_widget.py
--rw-r--r--   0 jfoster    (501) staff       (20)    11451 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/options_widget.ui
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-05-11 13:39:04.695945 glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/
--rw-r--r--   0 jfoster    (501) staff       (20)        0 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/__init__.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-05-11 13:39:04.696056 glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/data/
--rw-r--r--   0 jfoster    (501) staff       (20)    16046 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/data/penguins.csv
--rw-r--r--   0 jfoster    (501) staff       (20)     3070 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/test_axes.py
--rw-r--r--   0 jfoster    (501) staff       (20)     6886 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/test_data_viewer.py
--rw-r--r--   0 jfoster    (501) staff       (20)     2562 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/test_save_restore.py
--rw-r--r--   0 jfoster    (501) staff       (20)    12146 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/viewer.py
--rw-r--r--   0 jfoster    (501) staff       (20)    12287 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/state.py
--rw-r--r--   0 jfoster    (501) staff       (20)     1127 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/utils.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-05-11 13:39:04.694715 glue-small-multiples-1.1.2/glue_small_multiples.egg-info/
--rw-r--r--   0 jfoster    (501) staff       (20)     1023 2023-05-11 13:39:04.000000 glue-small-multiples-1.1.2/glue_small_multiples.egg-info/PKG-INFO
--rw-r--r--   0 jfoster    (501) staff       (20)      984 2023-05-11 13:39:04.000000 glue-small-multiples-1.1.2/glue_small_multiples.egg-info/SOURCES.txt
--rw-r--r--   0 jfoster    (501) staff       (20)        1 2023-05-11 13:39:04.000000 glue-small-multiples-1.1.2/glue_small_multiples.egg-info/dependency_links.txt
--rw-r--r--   0 jfoster    (501) staff       (20)       65 2023-05-11 13:39:04.000000 glue-small-multiples-1.1.2/glue_small_multiples.egg-info/entry_points.txt
--rw-r--r--   0 jfoster    (501) staff       (20)        1 2023-05-11 13:39:04.000000 glue-small-multiples-1.1.2/glue_small_multiples.egg-info/not-zip-safe
--rw-r--r--   0 jfoster    (501) staff       (20)       47 2023-05-11 13:39:04.000000 glue-small-multiples-1.1.2/glue_small_multiples.egg-info/requires.txt
--rw-r--r--   0 jfoster    (501) staff       (20)       21 2023-05-11 13:39:04.000000 glue-small-multiples-1.1.2/glue_small_multiples.egg-info/top_level.txt
--rw-r--r--   0 jfoster    (501) staff       (20)      149 2023-05-11 13:34:45.000000 glue-small-multiples-1.1.2/pyproject.toml
--rw-r--r--   0 jfoster    (501) staff       (20)     1074 2023-05-11 13:39:04.696574 glue-small-multiples-1.1.2/setup.cfg
--rw-r--r--   0 jfoster    (501) staff       (20)      397 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:39.810871 glue-small-multiples-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:39.810871 glue-small-multiples-1.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:39.810871 glue-small-multiples-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/.github/workflows/update-changelog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-12 19:16:39.810871 glue-small-multiples-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:39.810871 glue-small-multiples-1.2.1/glue_small_multiples/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/glue_small_multiples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/glue_small_multiples/layer_artist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:39.810871 glue-small-multiples-1.2.1/glue_small_multiples/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/glue_small_multiples/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/glue_small_multiples/qt/layer_style_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31901 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/glue_small_multiples/qt/layer_style_editor.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/glue_small_multiples/qt/options_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/glue_small_multiples/qt/options_widget.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:39.810871 glue-small-multiples-1.2.1/glue_small_multiples/qt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/glue_small_multiples/qt/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:39.810871 glue-small-multiples-1.2.1/glue_small_multiples/qt/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/glue_small_multiples/qt/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16046 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/glue_small_multiples/qt/tests/data/penguins.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/glue_small_multiples/qt/tests/test_axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/glue_small_multiples/qt/tests/test_data_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/glue_small_multiples/qt/tests/test_save_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/glue_small_multiples/qt/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12732 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/glue_small_multiples/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/glue_small_multiples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:39.810871 glue-small-multiples-1.2.1/glue_small_multiples.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-12 19:16:39.000000 glue-small-multiples-1.2.1/glue_small_multiples.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-12 19:16:39.000000 glue-small-multiples-1.2.1/glue_small_multiples.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:16:39.000000 glue-small-multiples-1.2.1/glue_small_multiples.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-12 19:16:39.000000 glue-small-multiples-1.2.1/glue_small_multiples.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:16:39.000000 glue-small-multiples-1.2.1/glue_small_multiples.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-12 19:16:39.000000 glue-small-multiples-1.2.1/glue_small_multiples.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-12 19:16:39.000000 glue-small-multiples-1.2.1/glue_small_multiples.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-12 19:16:39.814871 glue-small-multiples-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-12 19:15:38.000000 glue-small-multiples-1.2.1/tox.ini
```

### Comparing `glue-small-multiples-1.1.2/.gitignore` & `glue-small-multiples-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `glue-small-multiples-1.1.2/PKG-INFO` & `glue-small-multiples-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: glue-small-multiples
-Version: 1.1.2
+Version: 1.2.1
 Summary: A viewer for small multiples
 Home-page: https://www.gluesolutions.io
 Author: glue solutions, inc.
 Author-email: jfoster@gluesolutions.io
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: qt
 Provides-Extra: test
+Provides-Extra: qt
+Provides-Extra: glue
 
 # small multiples
 
 Add a small-multiples viewer to glue, allowing for the easy comparison of different partitions or facets of a dataset.
 
 ![Example Image](https://user-images.githubusercontent.com/3639698/191285037-598dc355-d185-4a23-99d8-318429272c4b.png)
```

### Comparing `glue-small-multiples-1.1.2/glue_small_multiples/layer_artist.py` & `glue-small-multiples-1.2.1/glue_small_multiples/layer_artist.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,109 +1,160 @@
 import numpy as np
 from echo import keep_in_sync
 
-from glue.core import BaseData, Subset
-from glue.utils import defer_draw, ensure_numerical, datetime64_to_mpl
+from glue.core import Subset
+from glue.utils import defer_draw, ensure_numerical
 from glue.core.exceptions import IncompatibleAttribute
 
 from glue.viewers.matplotlib.layer_artist import MatplotlibLayerArtist
 from glue.viewers.scatter.layer_artist import ScatterLayerArtist
-from glue.viewers.scatter.state import ScatterLayerState
 from glue.viewers.scatter.layer_artist import set_mpl_artist_cmap
 
 from glue_small_multiples.utils import PanTrackerMixin
 from glue_small_multiples.state import SmallMultiplesLayerState, FacetScatterLayerState
 
-__all__ = ['SmallMultiplesLayerArtist', 'FacetScatterLayerArtist']
+__all__ = ["SmallMultiplesLayerArtist", "FacetScatterLayerArtist"]
 
 
 # TODO: Just import these and update them with anything new
-CMAP_PROPERTIES = set(['cmap_mode', 'cmap_att', 'cmap_vmin', 'cmap_vmax', 'cmap'])
-MARKER_PROPERTIES = set(['size_mode', 'size_att', 'size_vmin', 'size_vmax', 'size_scaling', 'size', 'fill'])
-LINE_PROPERTIES = set(['linewidth', 'linestyle'])
-DENSITY_PROPERTIES = set(['dpi', 'stretch', 'density_contrast'])
-VISUAL_PROPERTIES = (CMAP_PROPERTIES | MARKER_PROPERTIES | DENSITY_PROPERTIES |
-                     LINE_PROPERTIES | set(['color', 'alpha', 'zorder', 'visible']))
-
-DATA_PROPERTIES = set(['layer', 'x_att', 'y_att', 'cmap_mode', 'size_mode', 'density_map',
-                       'xerr_att', 'yerr_att', 'xerr_visible', 'yerr_visible',
-                       'vector_visible', 'vx_att', 'vy_att', 'vector_arrowhead', 'vector_mode',
-                       'vector_origin', 'line_visible', 'markers_visible', 'vector_scaling',
-                       'col_facet_att'])
+CMAP_PROPERTIES = set(["cmap_mode", "cmap_att", "cmap_vmin", "cmap_vmax", "cmap"])
+MARKER_PROPERTIES = set(
+    ["size_mode", "size_att", "size_vmin", "size_vmax", "size_scaling", "size", "fill"]
+)
+LINE_PROPERTIES = set(["linewidth", "linestyle"])
+DENSITY_PROPERTIES = set(["dpi", "stretch", "density_contrast"])
+VISUAL_PROPERTIES = (
+    CMAP_PROPERTIES
+    | MARKER_PROPERTIES
+    | DENSITY_PROPERTIES
+    | LINE_PROPERTIES
+    | set(["color", "alpha", "zorder", "visible"])
+)
+
+DATA_PROPERTIES = set(
+    [
+        "layer",
+        "x_att",
+        "y_att",
+        "cmap_mode",
+        "size_mode",
+        "density_map",
+        "xerr_att",
+        "yerr_att",
+        "xerr_visible",
+        "yerr_visible",
+        "vector_visible",
+        "vx_att",
+        "vy_att",
+        "vector_arrowhead",
+        "vector_mode",
+        "vector_origin",
+        "line_visible",
+        "markers_visible",
+        "vector_scaling",
+        "col_facet_att",
+    ]
+)
+
 
 class SmallMultiplesLayerArtist(MatplotlibLayerArtist, PanTrackerMixin):
-    """
-    """
-    
+    """ """
+
     _layer_state_cls = SmallMultiplesLayerState
 
     def __init__(self, axes, viewer_state, layer_state=None, layer=None):
         super().__init__(axes, viewer_state, layer_state=layer_state, layer=layer)
         self.scatter_layer_artists = []
         self.scatter_layer_artists_syncs = []
         self.axes_subplots = None
 
         self._viewer_state.add_global_callback(self._update_scatter)
         self.state.add_global_callback(self._update_scatter)
 
     def _set_axes(self):
-
-        #import ipdb; ipdb.set_trace()
+        # import ipdb; ipdb.set_trace()
         if self._viewer_state.axes_subplots is not None:
             self.axes_subplots = self._viewer_state.axes_subplots
 
         if self.axes_subplots is None:
             return
 
         for sla in self.scatter_layer_artists:
             self._viewer_state.layers.remove(sla.state)
             sla.clear()
             sla.remove()
 
         self.scatter_layer_artists = []
         self.scatter_layer_artists_syncs = []
 
-
         flat_axes = self.axes_subplots.flatten()
-        flat_facet_masks = [item for sublist in self._viewer_state.data_facet_masks for item in sublist]
-        flat_facet_subsets = [item for sublist in self._viewer_state.data_facet_subsets for item in sublist]
+        flat_facet_masks = [
+            item for sublist in self._viewer_state.data_facet_masks for item in sublist
+        ]
+        flat_facet_subsets = [
+            item
+            for sublist in self._viewer_state.data_facet_subsets
+            for item in sublist
+        ]
         if len(flat_axes) != len(flat_facet_masks):
-            return 
+            return
 
-        for ax, facet_mask, facet_subset in zip(flat_axes, flat_facet_masks, 
-                                                flat_facet_subsets):
-            sla = FacetScatterLayerArtist(ax, self._viewer_state, layer=self.layer, 
-                                          facet_mask=facet_mask, facet_subset=facet_subset, 
-                                          scatter_state = self.state)
+        for ax, facet_mask, facet_subset in zip(
+            flat_axes, flat_facet_masks, flat_facet_subsets
+        ):
+            sla = FacetScatterLayerArtist(
+                ax,
+                self._viewer_state,
+                layer=self.layer,
+                facet_mask=facet_mask,
+                facet_subset=facet_subset,
+                scatter_state=self.state,
+            )
             self.scatter_layer_artists.append(sla)
-            for visual_property in (CMAP_PROPERTIES | MARKER_PROPERTIES | LINE_PROPERTIES | set(['color', 'alpha', 'zorder', 'visible'])):
-                sla_sync = keep_in_sync(self.state, visual_property, sla.state, visual_property)
+            for visual_property in (
+                CMAP_PROPERTIES
+                | MARKER_PROPERTIES
+                | LINE_PROPERTIES
+                | set(["color", "alpha", "zorder", "visible"])
+            ):
+                sla_sync = keep_in_sync(
+                    self.state, visual_property, sla.state, visual_property
+                )
                 self.scatter_layer_artists_syncs.append(sla_sync)
 
             sla._update_scatter(force=True)
 
     @defer_draw
     def _update_scatter(self, force=False, **kwargs):
-        if (self._viewer_state.x_att is None or
-                self._viewer_state.y_att is None or
-                ((self._viewer_state.col_facet_att is None) and 
-                (self._viewer_state.row_facet_att is None)) or
-                self._viewer_state.reference_data is None or
-                self.state.layer is None):
+        if (
+            self._viewer_state.x_att is None
+            or self._viewer_state.y_att is None
+            or (
+                (self._viewer_state.col_facet_att is None)
+                and (self._viewer_state.row_facet_att is None)
+            )
+            or self._viewer_state.reference_data is None
+            or self.state.layer is None
+        ):
             return
 
         changed = set() if force else self.pop_changed_properties()
-        if force or any(prop in changed for prop in ('col_facet_att','row_facet_att','num_rows','num_cols')):
+        if force or any(
+            prop in changed
+            for prop in ("col_facet_att", "row_facet_att", "num_rows", "num_cols")
+        ):
             self._set_axes()
 
     @defer_draw
     def update(self):
         self._update_scatter()
         for sla in self.scatter_layer_artists:
-            sla.state.zorder = self.state.zorder # zorder gets updated with ignore_callbacks -- force sync here
+            sla.state.zorder = (
+                self.state.zorder
+            )  # zorder gets updated with ignore_callbacks -- force sync here
             sla.update()
         self.redraw()
 
     def remove(self):
         # Clean up the density artist to avoid circular references to do a
         # reference to the self.histogram2d method in density artist.
         self.density_artist = None
@@ -112,109 +163,127 @@
             sla.clear()
             sla.remove()
         self.scatter_layer_artists = []
         self.scatter_layer_artists_syncs = []
         super(SmallMultiplesLayerArtist, self).remove()
 
     def clear(self):
-
         for sla in self.scatter_layer_artists:
             sla.clear()
         super(SmallMultiplesLayerArtist, self).remove()
 
-
     def redraw(self):
-        pass # There is nothing to actually draw for this artist
+        pass  # There is nothing to actually draw for this artist
 
 
 class FacetScatterLayerArtist(ScatterLayerArtist):
     """
     A custom ScatterLayerArtist that knows how to trim the data
     appropriately based on a facet_mask
     """
-    
+
     _layer_state_cls = FacetScatterLayerState
-    
-    def __init__(self, axes, viewer_state, layer_state=None, layer=None, 
-                 facet_mask=None, facet_subset=None, scatter_state=None):
-        self.density_artist = None # Hack to avoid an AttributeError because density_artist does
-                                   # not get fully initialized before a callback fires
+
+    def __init__(
+        self,
+        axes,
+        viewer_state,
+        layer_state=None,
+        layer=None,
+        facet_mask=None,
+        facet_subset=None,
+        scatter_state=None,
+    ):
+        self.density_artist = (
+            None  # Hack to avoid an AttributeError because density_artist does
+        )
+        # not get fully initialized before a callback fires
         super().__init__(axes, viewer_state, layer_state=layer_state, layer=layer)
 
         self.state.facet_mask = facet_mask
         self.state.facet_subset = facet_subset
         self.state._update_title()
         self.facet_mask = self.state.facet_mask
         if scatter_state is not None:
             self.state.update_from_state(scatter_state)
 
     @defer_draw
     def _update_scatter(self, force=False, **kwargs):
-        if (self._viewer_state.x_att is None or
-                self._viewer_state.y_att is None or
-                self._viewer_state.col_facet_att is None or
-                self._viewer_state.reference_data is None or
-                self.state.layer is None):
+        if (
+            self._viewer_state.x_att is None
+            or self._viewer_state.y_att is None
+            or self._viewer_state.col_facet_att is None
+            or self._viewer_state.reference_data is None
+            or self.state.layer is None
+        ):
             return
 
         changed = set() if force else self.pop_changed_properties()
 
         if force or len(changed & DATA_PROPERTIES) > 0:
             self._update_data()
             force = True
 
         if force or len(changed & VISUAL_PROPERTIES) > 0:
             self._update_visual_attributes(changed, force=force)
 
-
     @defer_draw
     def _update_data(self):
         if len(self.mpl_artists) == 0:
             return
         try:
             if not self.state.density_map:
                 if isinstance(self.layer, Subset):
                     # TODO: This is not a very efficient way to do this calculation, if that matters
                     # There are a fair number of calls here with empty subsets, and maybe
                     # we could short-circuit some of them
-                    xsubset_state = self.layer.subset_state & self.state.facet_subset.subset_state
-                    subset = Subset(self.layer.data,label=f"temp") 
+                    xsubset_state = (
+                        self.layer.subset_state & self.state.facet_subset.subset_state
+                    )
+                    subset = Subset(self.layer.data, label="temp")
                     subset.subset_state = xsubset_state
-                    masked_x = ensure_numerical(subset[self._viewer_state.x_att].ravel())
+                    masked_x = ensure_numerical(
+                        subset[self._viewer_state.x_att].ravel()
+                    )
                 else:
                     x = ensure_numerical(self.layer[self._viewer_state.x_att].ravel())
                     masked_x = np.ma.masked_where(self.facet_mask, x)
 
         except (IncompatibleAttribute, IndexError):
             self.disable_invalid_attributes(self._viewer_state.x_att)
             return
         else:
             self.enable()
 
         try:
             if not self.state.density_map:
-                if isinstance(self.layer, Subset): # This is not a very efficient way to do this
-                    ysubset_state = self.layer.subset_state & self.state.facet_subset.subset_state
-                    subset = Subset(self.layer.data,label=f"temp") 
+                if isinstance(
+                    self.layer, Subset
+                ):  # This is not a very efficient way to do this
+                    ysubset_state = (
+                        self.layer.subset_state & self.state.facet_subset.subset_state
+                    )
+                    subset = Subset(self.layer.data, label="temp")
                     subset.subset_state = ysubset_state
-                    masked_y = ensure_numerical(subset[self._viewer_state.y_att].ravel())
+                    masked_y = ensure_numerical(
+                        subset[self._viewer_state.y_att].ravel()
+                    )
                 else:
                     y = ensure_numerical(self.layer[self._viewer_state.y_att].ravel())
                     masked_y = np.ma.masked_where(self.facet_mask, y)
 
         except (IncompatibleAttribute, IndexError):
             self.disable_invalid_attributes(self._viewer_state.y_att)
             return
         else:
             self.enable()
 
         self.axes.set_title(self.state.title)
 
         if self.state.markers_visible:
-
             if self.state.density_map:
                 # We don't use x, y here because we actually make use of the
                 # ability of the density artist to call a custom histogram
                 # method which is defined on this class and does the data
                 # access.
                 self.plot_artist.set_data([], [])
                 self.scatter_artist.set_offsets(np.zeros((0, 2)))
@@ -226,141 +295,157 @@
                     self.plot_artist.set_data(masked_x, masked_y)
                 else:
                     offsets = np.vstack((masked_x, masked_y)).transpose()
                     self.scatter_artist.set_offsets(offsets)
         else:
             self.plot_artist.set_data([], [])
             self.scatter_artist.set_offsets(np.zeros((0, 2)))
-    
+
     @defer_draw
     def _update_visual_attributes(self, changed, force=False):
-
         if not self.enabled:
             return
 
         if self.state.markers_visible:
             if self.state.density_map:
-                if self.state.cmap_mode == 'Fixed':
-                    if force or 'color' in changed or 'cmap_mode' in changed:
+                if self.state.cmap_mode == "Fixed":
+                    if force or "color" in changed or "cmap_mode" in changed:
                         self.density_artist.set_color(self.state.color)
-                        self.density_artist.set_clim(self.density_auto_limits.min,
-                                                     self.density_auto_limits.max)
+                        self.density_artist.set_clim(
+                            self.density_auto_limits.min, self.density_auto_limits.max
+                        )
                 elif force or any(prop in changed for prop in CMAP_PROPERTIES):
                     c = ensure_numerical(self.layer[self.state.cmap_att].ravel())
                     if self.facet_mask is not None:
                         c = np.ma.masked_where(self.facet_mask, c)
                     set_mpl_artist_cmap(self.density_artist, c, self.state)
-    
-                if force or 'stretch' in changed:
-                    self.density_artist.set_norm(ImageNormalize(stretch=STRETCHES[self.state.stretch]()))
-    
-                if force or 'dpi' in changed:
+
+                if force or "dpi" in changed:
                     self.density_artist.set_dpi(self._viewer_state.dpi)
-    
-                if force or 'density_contrast' in changed:
+
+                if force or "density_contrast" in changed:
                     self.density_auto_limits.contrast = self.state.density_contrast
                     self.density_artist.stale = True
             else:
                 if self._use_plot_artist():
-                    if force or 'color' in changed or 'fill' in changed:
+                    if force or "color" in changed or "fill" in changed:
                         if self.state.fill:
-                            self.plot_artist.set_markeredgecolor('none')
+                            self.plot_artist.set_markeredgecolor("none")
                             self.plot_artist.set_markerfacecolor(self.state.color)
                         else:
                             self.plot_artist.set_markeredgecolor(self.state.color)
-                            self.plot_artist.set_markerfacecolor('none')
+                            self.plot_artist.set_markerfacecolor("none")
 
-                    if force or 'size' in changed or 'size_scaling' in changed:
-                        self.plot_artist.set_markersize(self.state.size *
-                                                        self.state.size_scaling)
+                    if force or "size" in changed or "size_scaling" in changed:
+                        self.plot_artist.set_markersize(
+                            self.state.size * self.state.size_scaling
+                        )
 
                 else:
-
                     # TEMPORARY: Matplotlib has a bug that causes set_alpha to
                     # change the colors back: https://github.com/matplotlib/matplotlib/issues/8953
-                    if 'alpha' in changed:
+                    if "alpha" in changed:
                         force = True
 
-                    if self.state.cmap_mode == 'Fixed':
-                        if force or 'color' in changed or 'cmap_mode' in changed or 'fill' in changed:
+                    if self.state.cmap_mode == "Fixed":
+                        if (
+                            force
+                            or "color" in changed
+                            or "cmap_mode" in changed
+                            or "fill" in changed
+                        ):
                             self.scatter_artist.set_array(None)
                             if self.state.fill:
                                 self.scatter_artist.set_facecolors(self.state.color)
-                                self.scatter_artist.set_edgecolors('none')
+                                self.scatter_artist.set_edgecolors("none")
                             else:
-                                self.scatter_artist.set_facecolors('none')
+                                self.scatter_artist.set_facecolors("none")
                                 self.scatter_artist.set_edgecolors(self.state.color)
-                    elif force or any(prop in changed for prop in CMAP_PROPERTIES) or 'fill' in changed:
+                    elif (
+                        force
+                        or any(prop in changed for prop in CMAP_PROPERTIES)
+                        or "fill" in changed
+                    ):
                         self.scatter_artist.set_edgecolors(None)
                         self.scatter_artist.set_facecolors(None)
                         c = ensure_numerical(self.layer[self.state.cmap_att].ravel())
                         if self.facet_mask is not None:
                             c = np.ma.masked_where(self.facet_mask, c)
 
                         set_mpl_artist_cmap(self.scatter_artist, c, self.state)
                         if self.state.fill:
-                            self.scatter_artist.set_edgecolors('none')
+                            self.scatter_artist.set_edgecolors("none")
                         else:
-                            self.scatter_artist.set_facecolors('none')
+                            self.scatter_artist.set_facecolors("none")
 
                     if force or any(prop in changed for prop in MARKER_PROPERTIES):
-
-                        if self.state.size_mode == 'Fixed':
+                        if self.state.size_mode == "Fixed":
                             s = self.state.size * self.state.size_scaling
-                            s = np.broadcast_to(s, self.scatter_artist.get_sizes().shape)
+                            s = np.broadcast_to(
+                                s, self.scatter_artist.get_sizes().shape
+                            )
                         else:
-                            s = ensure_numerical(self.layer[self.state.size_att].ravel())
+                            s = ensure_numerical(
+                                self.layer[self.state.size_att].ravel()
+                            )
                             if self.facet_mask is not None:
                                 s = np.ma.masked_where(self.facet_mask, s)
 
-                            s = ((s - self.state.size_vmin) /
-                                 (self.state.size_vmax - self.state.size_vmin))
+                            s = (s - self.state.size_vmin) / (
+                                self.state.size_vmax - self.state.size_vmin
+                            )
                             # The following ensures that the sizes are in the
                             # range 3 to 30 before the final size_scaling.
                             np.clip(s, 0, 1, out=s)
                             s *= 0.95
                             s += 0.05
-                            s *= (30 * self.state.size_scaling)
+                            s *= 30 * self.state.size_scaling
 
                         # Note, we need to square here because for scatter, s is actually
                         # proportional to the marker area, not radius.
-                        self.scatter_artist.set_sizes(s ** 2)
-
-        for artist in [self.scatter_artist, self.plot_artist,
-                       self.vector_artist, self.line_collection,
-                       self.density_artist]:
+                        self.scatter_artist.set_sizes(s**2)
 
+        for artist in [
+            self.scatter_artist,
+            self.plot_artist,
+            self.vector_artist,
+            self.line_collection,
+            self.density_artist,
+        ]:
             if artist is None:
                 continue
 
-            if force or 'alpha' in changed:
+            if force or "alpha" in changed:
                 artist.set_alpha(self.state.alpha)
 
-            if force or 'zorder' in changed:
+            if force or "zorder" in changed:
                 artist.set_zorder(self.state.zorder)
 
-            if force or 'visible' in changed:
+            if force or "visible" in changed:
                 # We need to hide the density artist if it is not needed because
                 # otherwise it might still show even if there is no data as the
                 # neutral/zero color might not be white.
                 if artist is self.density_artist:
-                    artist.set_visible(self.state.visible and
-                                       self.state.density_map and
-                                       self.state.markers_visible)
+                    artist.set_visible(
+                        self.state.visible
+                        and self.state.density_map
+                        and self.state.markers_visible
+                    )
                 else:
                     artist.set_visible(self.state.visible)
         if self._use_plot_artist():
             self.scatter_artist.set_visible(False)
         else:
             self.plot_artist.set_visible(False)
         self.redraw()
 
     def compute_density_map(self, *args, **kwargs):
         try:
             density_map = self.state.compute_density_map(*args, **kwargs)
         except IncompatibleAttribute:
-            self.disable_invalid_attributes(self._viewer_state.x_att,
-                                            self._viewer_state.y_att)
+            self.disable_invalid_attributes(
+                self._viewer_state.x_att, self._viewer_state.y_att
+            )
             return np.array([[np.nan]])
         else:
             self.enable()
         return density_map
```

### Comparing `glue-small-multiples-1.1.2/glue_small_multiples/qt/layer_style_editor.py` & `glue-small-multiples-1.2.1/glue_small_multiples/qt/layer_style_editor.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,55 +8,65 @@
 from glue.core import BaseData
 from echo.qt import autoconnect_callbacks_to_qt, connect_value
 from glue.utils.qt import load_ui, fix_tab_widget_fontsize
 from glue.core.exceptions import IncompatibleAttribute
 
 
 class SmallMultiplesLayerStyleEditor(QtWidgets.QWidget):
-
     def __init__(self, layer, parent=None):
-
         super(SmallMultiplesLayerStyleEditor, self).__init__(parent=parent)
 
-        self.ui = load_ui('layer_style_editor.ui', self,
-                          directory=os.path.dirname(__file__))
-
-        connect_kwargs = {'alpha': dict(value_range=(0, 1)),
-                          'size_scaling': dict(value_range=(0.1, 10), log=True),
-                          'density_contrast': dict(value_range=(0, 1)),
-                          'vector_scaling': dict(value_range=(0.1, 10), log=True)}
-        self._connections = autoconnect_callbacks_to_qt(layer.state, self.ui, connect_kwargs)
-
-        self._connection_dpi = connect_value(layer.state.viewer_state, 'dpi', self.ui.value_dpi,
-                                             value_range=(12, 144), log=True)
+        self.ui = load_ui(
+            "layer_style_editor.ui", self, directory=os.path.dirname(__file__)
+        )
+
+        connect_kwargs = {
+            "alpha": dict(value_range=(0, 1)),
+            "size_scaling": dict(value_range=(0.1, 10), log=True),
+            "density_contrast": dict(value_range=(0, 1)),
+            "vector_scaling": dict(value_range=(0.1, 10), log=True),
+        }
+        self._connections = autoconnect_callbacks_to_qt(
+            layer.state, self.ui, connect_kwargs
+        )
+
+        self._connection_dpi = connect_value(
+            layer.state.viewer_state,
+            "dpi",
+            self.ui.value_dpi,
+            value_range=(12, 144),
+            log=True,
+        )
 
         fix_tab_widget_fontsize(self.ui.tab_widget)
 
         self.layer_state = layer.state
 
-        self.layer_state.add_callback('markers_visible', self._update_markers_visible)
-        self.layer_state.add_callback('line_visible', self._update_line_visible)
-        self.layer_state.add_callback('xerr_visible', self._update_xerr_visible)
-        self.layer_state.add_callback('yerr_visible', self._update_yerr_visible)
-        self.layer_state.add_callback('vector_visible', self._update_vectors_visible)
-
-        self.layer_state.add_callback('cmap_mode', self._update_cmap_mode)
-        self.layer_state.add_callback('size_mode', self._update_size_mode)
-        self.layer_state.add_callback('vector_mode', self._update_vector_mode)
-
-        self.layer_state.add_callback('density_map', self._update_size_mode)
-        self.layer_state.add_callback('density_map', self._update_warnings)
-        self.layer_state.add_callback('density_map', self._update_checkboxes)
-
-        self.layer_state.viewer_state.add_callback('x_att', self._update_checkboxes)
-        self.layer_state.viewer_state.add_callback('y_att', self._update_checkboxes)
-        if hasattr(self.layer_state.viewer_state, 'plot_mode'):
-            self.layer_state.viewer_state.add_callback('plot_mode', self._update_vectors_visible)
+        self.layer_state.add_callback("markers_visible", self._update_markers_visible)
+        self.layer_state.add_callback("line_visible", self._update_line_visible)
+        self.layer_state.add_callback("xerr_visible", self._update_xerr_visible)
+        self.layer_state.add_callback("yerr_visible", self._update_yerr_visible)
+        self.layer_state.add_callback("vector_visible", self._update_vectors_visible)
+
+        self.layer_state.add_callback("cmap_mode", self._update_cmap_mode)
+        self.layer_state.add_callback("size_mode", self._update_size_mode)
+        self.layer_state.add_callback("vector_mode", self._update_vector_mode)
+
+        self.layer_state.add_callback("density_map", self._update_size_mode)
+        self.layer_state.add_callback("density_map", self._update_warnings)
+        self.layer_state.add_callback("density_map", self._update_checkboxes)
+
+        self.layer_state.viewer_state.add_callback("x_att", self._update_checkboxes)
+        self.layer_state.viewer_state.add_callback("y_att", self._update_checkboxes)
+        if hasattr(self.layer_state.viewer_state, "plot_mode"):
+            self.layer_state.viewer_state.add_callback(
+                "plot_mode", self._update_vectors_visible
+            )
 
-        self.layer_state.add_callback('layer', self._update_warnings)
+        self.layer_state.add_callback("layer", self._update_warnings)
 
         self._update_markers_visible()
         self._update_line_visible()
         self._update_xerr_visible()
         self._update_yerr_visible()
         self._update_vectors_visible()
 
@@ -65,60 +75,64 @@
         self._update_cmap_mode()
 
         self._update_checkboxes()
 
         self._update_warnings()
 
     def _update_warnings(self, *args):
-
         if self.layer_state.layer is None:
             n_points = 0
         else:
             n_points = np.product(self.layer_state.layer.shape)
 
         warning = " (may be slow given data size)"
 
-        for combo, threshold in [(self.ui.combosel_size_mode, 10000),
-                                 (self.ui.combosel_cmap_mode, 50000)]:
-
+        for combo, threshold in [
+            (self.ui.combosel_size_mode, 10000),
+            (self.ui.combosel_cmap_mode, 50000),
+        ]:
             if n_points > threshold and not self.layer_state.density_map:
                 for item in range(combo.count()):
                     text = combo.itemText(item)
-                    if text != 'Fixed':
+                    if text != "Fixed":
                         combo.setItemText(item, text + warning)
                         combo.setItemData(item, QtGui.QBrush(Qt.red), Qt.TextColorRole)
             else:
                 for item in range(combo.count()):
                     text = combo.itemText(item)
-                    if text != 'Fixed':
+                    if text != "Fixed":
                         if warning in text:
-                            combo.setItemText(item, text.replace(warning, ''))
+                            combo.setItemText(item, text.replace(warning, ""))
                             combo.setItemData(item, QtGui.QBrush(), Qt.TextColorRole)
 
         if n_points > 10000:
             self.ui.label_warning_errorbar.show()
         else:
             self.ui.label_warning_errorbar.hide()
 
         if n_points > 10000:
             self.ui.label_warning_vector.show()
         else:
             self.ui.label_warning_vector.hide()
 
     def _update_size_mode(self, size_mode=None):
-
-        visible = not self.layer_state.density_map and not self.layer_state.size_mode == 'Fixed'
+        visible = (
+            not self.layer_state.density_map
+            and not self.layer_state.size_mode == "Fixed"
+        )
         self.ui.label_size_attribute.setVisible(visible)
         self.ui.combosel_size_att.setVisible(visible)
         self.ui.label_size_limits.setVisible(visible)
         self.ui.valuetext_size_vmin.setVisible(visible)
         self.ui.valuetext_size_vmax.setVisible(visible)
         self.ui.button_flip_size.setVisible(visible)
 
-        visible = not self.layer_state.density_map and self.layer_state.size_mode == 'Fixed'
+        visible = (
+            not self.layer_state.density_map and self.layer_state.size_mode == "Fixed"
+        )
         self.ui.value_size.setVisible(visible)
 
         density = self.layer_state.density_map
         self.ui.value_dpi.setVisible(density)
         self.ui.label_dpi.setVisible(density)
         self.ui.label_stretch.setVisible(density)
         self.ui.combosel_stretch.setVisible(density)
@@ -142,75 +156,93 @@
         self.ui.value_dpi.setEnabled(self.layer_state.markers_visible)
         self.ui.combosel_stretch.setEnabled(self.layer_state.markers_visible)
         self.ui.label_size_scaling.setEnabled(self.layer_state.markers_visible)
         self.ui.combosel_points_mode.setEnabled(self.layer_state.markers_visible)
         self.ui.value_density_contrast.setEnabled(self.layer_state.markers_visible)
 
     def _update_checkboxes(self, *args):
-
         if isinstance(self.layer_state.layer, BaseData):
             layer = self.layer_state.layer
         else:
             layer = self.layer_state.layer.data
 
         try:
-            x_datetime = layer.get_kind(self.layer_state.viewer_state.x_att) == 'datetime'
+            x_datetime = (
+                layer.get_kind(self.layer_state.viewer_state.x_att) == "datetime"
+            )
         except IncompatibleAttribute:
             x_datetime = False
 
         try:
-            y_datetime = layer.get_kind(self.layer_state.viewer_state.y_att) == 'datetime'
+            y_datetime = (
+                layer.get_kind(self.layer_state.viewer_state.y_att) == "datetime"
+            )
         except IncompatibleAttribute:
             y_datetime = False
 
-        for checkbox in [self.ui.bool_line_visible, self.ui.bool_xerr_visible,
-                         self.ui.bool_yerr_visible, self.ui.bool_vector_visible]:
+        for checkbox in [
+            self.ui.bool_line_visible,
+            self.ui.bool_xerr_visible,
+            self.ui.bool_yerr_visible,
+            self.ui.bool_vector_visible,
+        ]:
             if self.layer_state.density_map:
                 checkbox.setEnabled(False)
-                checkbox.setToolTip('Not available with density map')
+                checkbox.setToolTip("Not available with density map")
             else:
-                if ((x_datetime and checkbox in (self.ui.bool_xerr_visible, self.ui.bool_vector_visible)) or
-                       (y_datetime and checkbox in (self.ui.bool_yerr_visible, self.ui.bool_vector_visible))):
+                if (
+                    x_datetime
+                    and checkbox
+                    in (self.ui.bool_xerr_visible, self.ui.bool_vector_visible)
+                ) or (
+                    y_datetime
+                    and checkbox
+                    in (self.ui.bool_yerr_visible, self.ui.bool_vector_visible)
+                ):
                     checkbox.setEnabled(False)
-                    checkbox.setToolTip('Not available when using datetime attribute')
+                    checkbox.setToolTip("Not available when using datetime attribute")
                 else:
                     checkbox.setEnabled(True)
-                    checkbox.setToolTip('')
+                    checkbox.setToolTip("")
 
     def _update_line_visible(self, *args):
         self.ui.value_linewidth.setEnabled(self.layer_state.line_visible)
         self.ui.combosel_linestyle.setEnabled(self.layer_state.line_visible)
 
     def _update_xerr_visible(self, *args):
         self.ui.combosel_xerr_att.setEnabled(self.layer_state.xerr_visible)
 
     def _update_yerr_visible(self, *args):
         self.ui.combosel_yerr_att.setEnabled(self.layer_state.yerr_visible)
 
     def _update_vectors_visible(self, *args):
         viewer_state = self.layer_state.viewer_state
-        is_rect = not hasattr(viewer_state, 'plot_mode') or viewer_state.plot_mode == 'rectilinear'
-        self.ui.combosel_vector_mode.setEnabled(self.layer_state.vector_visible and is_rect)
+        is_rect = (
+            not hasattr(viewer_state, "plot_mode")
+            or viewer_state.plot_mode == "rectilinear"
+        )
+        self.ui.combosel_vector_mode.setEnabled(
+            self.layer_state.vector_visible and is_rect
+        )
         self.ui.combosel_vx_att.setEnabled(self.layer_state.vector_visible)
         self.ui.combosel_vy_att.setEnabled(self.layer_state.vector_visible)
         self.ui.value_vector_scaling.setEnabled(self.layer_state.vector_visible)
         self.ui.combosel_vector_origin.setEnabled(self.layer_state.vector_visible)
         self.ui.bool_vector_arrowhead.setEnabled(self.layer_state.vector_visible)
 
     def _update_vector_mode(self, vector_mode=None):
-        if self.layer_state.vector_mode == 'Cartesian':
-            self.ui.label_vector_x.setText('vx')
-            self.ui.label_vector_y.setText('vy')
-        elif self.layer_state.vector_mode == 'Polar':
-            self.ui.label_vector_x.setText('angle (deg)')
-            self.ui.label_vector_y.setText('length')
+        if self.layer_state.vector_mode == "Cartesian":
+            self.ui.label_vector_x.setText("vx")
+            self.ui.label_vector_y.setText("vy")
+        elif self.layer_state.vector_mode == "Polar":
+            self.ui.label_vector_x.setText("angle (deg)")
+            self.ui.label_vector_y.setText("length")
 
     def _update_cmap_mode(self, cmap_mode=None):
-
-        if self.layer_state.cmap_mode == 'Fixed':
+        if self.layer_state.cmap_mode == "Fixed":
             self.ui.label_cmap_attribute.hide()
             self.ui.combosel_cmap_att.hide()
             self.ui.label_cmap_limits.hide()
             self.ui.valuetext_cmap_vmin.hide()
             self.ui.valuetext_cmap_vmax.hide()
             self.ui.button_flip_cmap.hide()
             self.ui.combodata_cmap.hide()
```

### Comparing `glue-small-multiples-1.1.2/glue_small_multiples/qt/layer_style_editor.ui` & `glue-small-multiples-1.2.1/glue_small_multiples/qt/layer_style_editor.ui`

 * *Files identical despite different names*

### Comparing `glue-small-multiples-1.1.2/glue_small_multiples/qt/options_widget.py` & `glue-small-multiples-1.2.1/glue_small_multiples/qt/options_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 
 from qtpy import QtWidgets
 
 from echo.qt import autoconnect_callbacks_to_qt
 from glue.utils.qt import load_ui, fix_tab_widget_fontsize
 
-class SmallMultiplesOptionsWidget(QtWidgets.QWidget):
 
+class SmallMultiplesOptionsWidget(QtWidgets.QWidget):
     def __init__(self, viewer_state, session, parent=None):
         super(SmallMultiplesOptionsWidget, self).__init__(parent=parent)
 
-        self.ui = load_ui('options_widget.ui', self,
-                          directory=os.path.dirname(__file__))
-        
+        self.ui = load_ui(
+            "options_widget.ui", self, directory=os.path.dirname(__file__)
+        )
+
         fix_tab_widget_fontsize(self.ui.tab_widget)
-        
+
         self._connections = autoconnect_callbacks_to_qt(viewer_state, self.ui)
 
         self.viewer_state = viewer_state
```

### Comparing `glue-small-multiples-1.1.2/glue_small_multiples/qt/options_widget.ui` & `glue-small-multiples-1.2.1/glue_small_multiples/qt/options_widget.ui`

 * *Files identical despite different names*

### Comparing `glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/data/penguins.csv` & `glue-small-multiples-1.2.1/glue_small_multiples/qt/tests/data/penguins.csv`

 * *Files identical despite different names*

### Comparing `glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/test_axes.py` & `glue-small-multiples-1.2.1/glue_small_multiples/qt/tests/test_axes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,69 @@
-# pylint: disable=I0011,W0613,W0201,W0212,E1101,E1103
-
 import os
-from collections import Counter
 
-import pytest
-import numpy as np
-from numpy.testing import assert_allclose, assert_equal
 from glue.core import data_factories as df
 from glue.app.qt import GlueApplication
-from glue.core.subset import AndState
-from glue.core.roi import RectangularROI
-from glue.config import colormaps
-from glue.utils.qt import process_events
-from glue.core.state import GlueUnSerializer
 from glue.utils.qt import process_events
 
 from glue_small_multiples.qt.viewer import SmallMultiplesViewer
 
-DATA = os.path.join(os.path.dirname(__file__), 'data')
+DATA = os.path.join(os.path.dirname(__file__), "data")
 NUM_ADELIE = 152
 NUM_CHINSTRAP = 68
 NUM_GENTOO = 124
 
-"""
-Next steps:
-
-Make subset creation work on other axes
-Figure out why subsets do not display on the third/final? facet plot
 
-"""
+CMAP_PROPERTIES = set(["cmap_mode", "cmap_att", "cmap_vmin", "cmap_vmax", "cmap"])
+MARKER_PROPERTIES = set(
+    ["size_mode", "size_att", "size_vmin", "size_vmax", "size_scaling", "size", "fill"]
+)
+LINE_PROPERTIES = set(["linewidth", "linestyle"])
 
-CMAP_PROPERTIES = set(['cmap_mode', 'cmap_att', 'cmap_vmin', 'cmap_vmax', 'cmap'])
-MARKER_PROPERTIES = set(['size_mode', 'size_att', 'size_vmin', 'size_vmax', 'size_scaling', 'size', 'fill'])
-LINE_PROPERTIES = set(['linewidth', 'linestyle'])
 
 class TestSmallMultiplesViewer(object):
-    
     def setup_method(self, method):
         self.app = GlueApplication()
         self.session = self.app.session
         self.hub = self.session.hub
         self.data_collection = self.session.data_collection
-        penguins = df.load_data(os.path.join(DATA, 'penguins.csv'))
+        penguins = df.load_data(os.path.join(DATA, "penguins.csv"))
         self.penguin_data = penguins
         self.data_collection.append(self.penguin_data)
         self.viewer = self.app.new_data_viewer(SmallMultiplesViewer)
         self.viewer.add_data(self.penguin_data)
 
     def test_basic(self):
         viewer_state = self.viewer.state
         process_events()
 
         assert len(self.viewer.layers[0].scatter_layer_artists) == 3
         assert len(self.viewer.state.layers) == 4
         yo = self.viewer.layers[0].scatter_layer_artists[0]
-                
-        x,y = yo.plot_artist.get_data()
-        unmasked_x = x[x.mask == False]
+
+        x, y = yo.plot_artist.get_data()
+        unmasked_x = x[~x.mask]
         assert len(unmasked_x) > 10
 
-        viewer_state.x_att = self.penguin_data.id['bill_length_mm']
-        viewer_state.y_att = self.penguin_data.id['bill_depth_mm']
-        
+        viewer_state.x_att = self.penguin_data.id["bill_length_mm"]
+        viewer_state.y_att = self.penguin_data.id["bill_depth_mm"]
+
         yo = self.viewer.layers[0].scatter_layer_artists[1]
-                
-        x,y = yo.plot_artist.get_data()
-        unmasked_x = x[x.mask == False]
+
+        x, y = yo.plot_artist.get_data()
+        unmasked_x = x[~x.mask]
         assert len(unmasked_x) > 10
 
-        viewer_state.row_facet_att = self.penguin_data.id['island']
+        viewer_state.row_facet_att = self.penguin_data.id["island"]
         process_events()
 
         assert len(self.viewer.layers) == 1
         assert len(self.viewer.state.layers) == 10
         assert len(self.viewer.layers[0].scatter_layer_artists) == 9
-        #assert viewer_state.data_facet_masks[0].count() == NUM_ADELIE
-        #assert viewer_state.data_facet_masks[1].count() == NUM_CHINSTRAP
-        #assert viewer_state.data_facet_masks[2].count() == NUM_GENTOO
-
-        #The following seems to work in the GUI but not in test?
-        #viewer_state.row_facet_att = self.penguin_data.id['sex']
-        #process_events(wait=2)
-        #assert len(self.viewer.layers) == 1
-        #assert len(self.viewer.state.layers) == 7
+        # assert viewer_state.data_facet_masks[0].count() == NUM_ADELIE
+        # assert viewer_state.data_facet_masks[1].count() == NUM_CHINSTRAP
+        # assert viewer_state.data_facet_masks[2].count() == NUM_GENTOO
+
+        # The following seems to work in the GUI but not in test?
+        # viewer_state.row_facet_att = self.penguin_data.id['sex']
+        # process_events(wait=2)
+        # assert len(self.viewer.layers) == 1
+        # assert len(self.viewer.state.layers) == 7
```

### Comparing `glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/test_data_viewer.py` & `glue-small-multiples-1.2.1/glue_small_multiples/qt/tests/test_data_viewer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,177 +1,188 @@
-# pylint: disable=I0011,W0613,W0201,W0212,E1101,E1103
-
 import os
-from collections import Counter
 
-import pytest
 import numpy as np
-from numpy.testing import assert_allclose, assert_equal
 from glue.core import data_factories as df
 from glue.app.qt import GlueApplication
 from glue.core.subset import AndState
 from glue.core.roi import RectangularROI
 from glue.config import colormaps
 from glue.utils.qt import process_events
 from glue.core.state import GlueUnSerializer
 
 from ..viewer import SmallMultiplesViewer
 
-DATA = os.path.join(os.path.dirname(__file__), 'data')
+DATA = os.path.join(os.path.dirname(__file__), "data")
 NUM_ADELIE = 152
 NUM_CHINSTRAP = 68
 NUM_GENTOO = 124
 
-
-CMAP_PROPERTIES = set(['cmap_mode', 'cmap_att', 'cmap_vmin', 'cmap_vmax', 'cmap'])
-MARKER_PROPERTIES = set(['size_mode', 'size_att', 'size_vmin', 'size_vmax', 'size_scaling', 'size', 'fill'])
-LINE_PROPERTIES = set(['linewidth', 'linestyle'])
+CMAP_PROPERTIES = set(["cmap_mode", "cmap_att", "cmap_vmin", "cmap_vmax", "cmap"])
+MARKER_PROPERTIES = set(
+    ["size_mode", "size_att", "size_vmin", "size_vmax", "size_scaling", "size", "fill"]
+)
+LINE_PROPERTIES = set(["linewidth", "linestyle"])
 
 
 class TestSmallMultiplesViewer(object):
-    
-    
     def setup_method(self, method):
         self.app = GlueApplication()
         self.session = self.app.session
         self.hub = self.session.hub
         self.data_collection = self.session.data_collection
-        penguins = df.load_data(os.path.join(DATA, 'penguins.csv'))
+        penguins = df.load_data(os.path.join(DATA, "penguins.csv"))
         self.penguin_data = penguins
         self.data_collection.append(self.penguin_data)
         self.viewer = self.app.new_data_viewer(SmallMultiplesViewer)
         self.viewer.add_data(self.penguin_data)
 
-        
     def test_basic(self):
         viewer_state = self.viewer.state
 
-        viewer_state.x_att = self.penguin_data.id['bill_length_mm']
-        viewer_state.y_att = self.penguin_data.id['bill_depth_mm']
+        viewer_state.x_att = self.penguin_data.id["bill_length_mm"]
+        viewer_state.y_att = self.penguin_data.id["bill_depth_mm"]
 
-        viewer_state.col_facet_att = self.penguin_data.id['species']
+        viewer_state.col_facet_att = self.penguin_data.id["species"]
 
-        assert len(self.viewer.layers) == 1 # Just one dataset
-        assert len(viewer_state.layers) == 4 # We have 4 layers here: one SmallMultiplesLayerArtist and 3 FacetScatterLayerArtist
+        assert len(self.viewer.layers) == 1  # Just one dataset
+        assert (
+            len(viewer_state.layers) == 4
+        )  # We have 4 layers here: one SmallMultiplesLayerArtist and 3 FacetScatterLayerArtist
         assert len(self.viewer.layers[0].scatter_layer_artists) == 3
         adelie = viewer_state.data_facet_masks[0][0]
         chinstrap = viewer_state.data_facet_masks[0][1]
         gentoo = viewer_state.data_facet_masks[0][2]
 
         assert np.size(adelie) - np.count_nonzero(adelie) == NUM_ADELIE
         assert np.size(chinstrap) - np.count_nonzero(chinstrap) == NUM_CHINSTRAP
         assert np.size(gentoo) - np.count_nonzero(gentoo) == NUM_GENTOO
-        #assert len(viewer_state.layers_data) == 3
+        # assert len(viewer_state.layers_data) == 3
 
     def test_layer_styles(self):
         """
         Make sure all the style code runs
         and that our layer artists stay in sync with the
         overall layer state
         """
 
         viewer_state = self.viewer.state
         layer_state = self.viewer.layers[0].state
-        layer_state.style = 'Scatter'
+        layer_state.style = "Scatter"
 
-        layer_state.size_mode = 'Linear'
-        layer_state.size_att = self.penguin_data.id['bill_length_mm']
+        layer_state.size_mode = "Linear"
+        layer_state.size_att = self.penguin_data.id["bill_length_mm"]
         layer_state.size_vmin = 1.2
-        layer_state.size_vmax = 4.
+        layer_state.size_vmax = 4.0
         layer_state.size_scaling = 2
 
-        layer_state.cmap_mode = 'Linear'
-        layer_state.cmap_att = self.penguin_data.id['bill_depth_mm']
+        layer_state.cmap_mode = "Linear"
+        layer_state.cmap_att = self.penguin_data.id["bill_depth_mm"]
         layer_state.cmap_vmin = -1
-        layer_state.cmap_vmax = 2.
+        layer_state.cmap_vmax = 2.0
         layer_state.cmap = colormaps.members[3][1]
 
         # Check inverting works
-        layer_state.cmap_vmin = 3.
-
-        layer_state.size_mode = 'Fixed'
+        layer_state.cmap_vmin = 3.0
 
+        layer_state.size_mode = "Fixed"
 
-        layer_state.style = 'Line'
+        layer_state.style = "Line"
         layer_state.linewidth = 3
-        layer_state.linestyle = 'dashed'
-        
-        for i in (0,1,2):
-            assert self.viewer.layers[0].scatter_layer_artists[i].state.size_mode == layer_state.size_mode
-            assert self.viewer.layers[0].scatter_layer_artists[i].state.size_vmin == layer_state.size_vmin
-            assert self.viewer.layers[0].scatter_layer_artists[i].state.cmap == layer_state.cmap
-
-        viewer_state.col_facet_att = self.penguin_data.id['sex']
-        for i in (0,1,2):
-            assert self.viewer.layers[0].scatter_layer_artists[i].state.size_mode == layer_state.size_mode
-            assert self.viewer.layers[0].scatter_layer_artists[i].state.size_vmin == layer_state.size_vmin
-            assert self.viewer.layers[0].scatter_layer_artists[i].state.cmap == layer_state.cmap
+        layer_state.linestyle = "dashed"
 
+        for i in (0, 1, 2):
+            assert (
+                self.viewer.layers[0].scatter_layer_artists[i].state.size_mode
+                == layer_state.size_mode
+            )
+            assert (
+                self.viewer.layers[0].scatter_layer_artists[i].state.size_vmin
+                == layer_state.size_vmin
+            )
+            assert (
+                self.viewer.layers[0].scatter_layer_artists[i].state.cmap
+                == layer_state.cmap
+            )
+
+        viewer_state.col_facet_att = self.penguin_data.id["sex"]
+        for i in (0, 1, 2):
+            assert (
+                self.viewer.layers[0].scatter_layer_artists[i].state.size_mode
+                == layer_state.size_mode
+            )
+            assert (
+                self.viewer.layers[0].scatter_layer_artists[i].state.size_vmin
+                == layer_state.size_vmin
+            )
+            assert (
+                self.viewer.layers[0].scatter_layer_artists[i].state.cmap
+                == layer_state.cmap
+            )
 
     def test_apply_roi(self):
         viewer_state = self.viewer.state
 
-        viewer_state.x_att = self.penguin_data.id['bill_length_mm']
-        viewer_state.y_att = self.penguin_data.id['bill_depth_mm']
-        viewer_state.col_facet_att = self.penguin_data.id['species']
+        viewer_state.x_att = self.penguin_data.id["bill_length_mm"]
+        viewer_state.y_att = self.penguin_data.id["bill_depth_mm"]
+        viewer_state.col_facet_att = self.penguin_data.id["species"]
 
         roi = RectangularROI(34, 50, 20, 22)
 
         assert len(self.viewer.layers) == 1
         self.viewer.apply_roi(roi)
-        
+
         assert len(self.viewer.layers) == 2
         assert len(self.penguin_data.subsets) == 1
         state = self.penguin_data.subsets[0].subset_state
         assert isinstance(state, AndState)
 
-        
         subset_sla = self.viewer.layers[1].scatter_layer_artists[0]
         backgr_sla = self.viewer.layers[0].scatter_layer_artists[0]
         # We should NOT have to do this
-        #yo._update_data()
-        #yo.redraw()
-        
+        # yo._update_data()
+        # yo.redraw()
+
         subset_master = self.viewer.layers[1]
         backgr_master = self.viewer.layers[0]
         assert subset_master.zorder > backgr_master.zorder
 
-        x,y = subset_sla.plot_artist.get_data()
-        #unmasked_x = x[x.mask == False]
+        x, y = subset_sla.plot_artist.get_data()
+        # unmasked_x = x[x.mask == False]
         assert len(x) == 14
         assert subset_sla.zorder > backgr_sla.zorder
-        
-
 
     def test_session_save_and_restore(self, tmpdir):
         viewer_state = self.viewer.state
         layer_state = self.viewer.layers[0].state
 
-        viewer_state.x_att = self.penguin_data.id['bill_length_mm']
-        viewer_state.y_att = self.penguin_data.id['bill_depth_mm']
-        viewer_state.col_facet_att = self.penguin_data.id['species']
-        layer_state.cmap_mode = 'Linear'
-        layer_state.cmap_att = self.penguin_data.id['bill_length_mm']
+        viewer_state.x_att = self.penguin_data.id["bill_length_mm"]
+        viewer_state.y_att = self.penguin_data.id["bill_depth_mm"]
+        viewer_state.col_facet_att = self.penguin_data.id["species"]
+        layer_state.cmap_mode = "Linear"
+        layer_state.cmap_att = self.penguin_data.id["bill_length_mm"]
         assert len(self.viewer._toolbars) == 1
         process_events()
-        filename = tmpdir.join('test_multi_session.glu').strpath
+        filename = tmpdir.join("test_multi_session.glu").strpath
 
         self.session.application.save_session(filename)
 
-        with open(filename, 'r') as f:
+        with open(filename, "r") as f:
             session = f.read()
 
         state = GlueUnSerializer.loads(session)
-        ga = state.object('__main__')
+        ga = state.object("__main__")
 
         dc = ga.session.data_collection
         viewer = ga.viewers[0][0]
-        assert viewer.state.x_att is dc[0].id['bill_length_mm']
-        assert viewer.state.col_facet_att is dc[0].id['species']
-        assert viewer.layers[0].scatter_layer_artists[0].state.size_mode == layer_state.size_mode
+        assert viewer.state.x_att is dc[0].id["bill_length_mm"]
+        assert viewer.state.col_facet_att is dc[0].id["species"]
+        assert (
+            viewer.layers[0].scatter_layer_artists[0].state.size_mode
+            == layer_state.size_mode
+        )
         assert len(viewer.layers) == 1
         assert len(viewer.layers[0].scatter_layer_artists) == 3
         assert np.sum(~viewer_state.data_facet_masks[0][0]) == NUM_ADELIE
         assert np.sum(~viewer_state.data_facet_masks[0][1]) == NUM_CHINSTRAP
         assert np.sum(~viewer_state.data_facet_masks[0][2]) == NUM_GENTOO
         assert len(viewer._toolbars) == 1
         assert viewer.layers[0].state.cmap_mode == layer_state.cmap_mode
```

### Comparing `glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/test_save_restore.py` & `glue-small-multiples-1.2.1/glue_small_multiples/qt/tests/test_save_restore.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,85 +1,78 @@
-import os
-import pytest
-import numpy as np
 from glue.core import Data
 from glue.app.qt import GlueApplication
 from glue.core.state import GlueUnSerializer
-from glue.utils.qt import process_events
-
-from glue.core.roi import RectangularROI
-
-from numpy.testing import assert_allclose, assert_equal
 
 from glue_small_multiples.qt.viewer import SmallMultiplesViewer
 
-class TestSmallMultiplesViewer(object):
 
+class TestSmallMultiplesViewer(object):
     def setup_method(self, method):
-    
-        self.data = Data(label='d1', x=[13.4, 2.3, 20.1, 8.6],
-                         y=[1.2, 6.7, 12.3, 15.0], a=['a', 'a', 'b', 'b'],
-                         b = ['x', 'y', 'x', 'y'])
+        self.data = Data(
+            label="d1",
+            x=[13.4, 2.3, 20.1, 8.6],
+            y=[1.2, 6.7, 12.3, 15.0],
+            a=["a", "a", "b", "b"],
+            b=["x", "y", "x", "y"],
+        )
 
         self.app = GlueApplication()
         self.session = self.app.session
         self.hub = self.session.hub
 
         self.data_collection = self.session.data_collection
         self.data_collection.append(self.data)
 
         self.viewer = self.app.new_data_viewer(SmallMultiplesViewer)
 
     def test_basic(self):
-    
         viewer_state = self.viewer.state
-        
+
         # Check defaults when we add data
         self.viewer.add_data(self.data)
 
-        viewer_state.x_att = self.data.id['x']
-        viewer_state.y_att = self.data.id['y']
+        viewer_state.x_att = self.data.id["x"]
+        viewer_state.y_att = self.data.id["y"]
 
-        viewer_state.col_facet_att = self.data.id['a']
-        viewer_state.row_facet_att = self.data.id['b']
+        viewer_state.col_facet_att = self.data.id["a"]
+        viewer_state.row_facet_att = self.data.id["b"]
 
-        assert viewer_state.x_att is self.data.id['x']
-        assert viewer_state.y_att is self.data.id['y']
-        assert viewer_state.col_facet_att is self.data.id['a']
-        assert viewer_state.row_facet_att is self.data.id['b']
+        assert viewer_state.x_att is self.data.id["x"]
+        assert viewer_state.y_att is self.data.id["y"]
+        assert viewer_state.col_facet_att is self.data.id["a"]
+        assert viewer_state.row_facet_att is self.data.id["b"]
 
         assert len(viewer_state.layers) == 5
 
     def test_session_save_and_restore(self, tmpdir):
-    
         viewer_state = self.viewer.state
-        
+
         # Check defaults when we add data
         self.viewer.add_data(self.data)
 
-        viewer_state.x_att = self.data.id['x']
-        viewer_state.y_att = self.data.id['y']
+        viewer_state.x_att = self.data.id["x"]
+        viewer_state.y_att = self.data.id["y"]
 
-        viewer_state.col_facet_att = self.data.id['a']
-        viewer_state.row_facet_att = self.data.id['b']
+        viewer_state.col_facet_att = self.data.id["a"]
+        viewer_state.row_facet_att = self.data.id["b"]
 
-        filename = tmpdir.join('test_qtl_session.glu').strpath
+        filename = tmpdir.join("test_qtl_session.glu").strpath
 
         self.session.application.save_session(filename)
 
-        with open(filename, 'r') as f:
+        with open(filename, "r") as f:
             session = f.read()
         state = GlueUnSerializer.loads(session)
 
-        ga = state.object('__main__')
+        ga = state.object("__main__")
 
         dc = ga.session.data_collection
 
         viewer = ga.viewers[0][0]
         viewer_state = viewer.state
 
-        assert viewer.state.col_facet_att is dc[0].id['a']
+        assert viewer.state.col_facet_att is dc[0].id["a"]
 
         assert id(viewer_state.axes_subplots) == id(viewer.axes_array)
         assert len(viewer_state.layers) == 5
 
         ga.close()
```

### Comparing `glue-small-multiples-1.1.2/glue_small_multiples/qt/viewer.py` & `glue-small-multiples-1.2.1/glue_small_multiples/qt/viewer.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,84 +2,88 @@
 
 from echo import delay_callback
 
 from glue.config import viewer_tool
 from glue.core import roi
 from glue.core.subset import roi_to_subset_state
 
-from glue.utils import nonpartial, defer_draw, decorate_all_methods
+from glue.utils import defer_draw, decorate_all_methods
 from glue.viewers.matplotlib.qt.data_viewer import MatplotlibDataViewer
-from glue.viewers.matplotlib.toolbar_mode import RectangleMode, ToolbarModeBase
+from glue.viewers.matplotlib.toolbar_mode import ToolbarModeBase
+from glue.core.roi_pretransforms import ProjectionMplTransform
 
 from glue.viewers.scatter.viewer import MatplotlibScatterMixin
-from glue.core.util import update_ticks
-from glue.viewers.common.viewer import get_layer_artist_from_registry
 
 from glue_small_multiples.utils import PanTrackerMixin
 from glue_small_multiples.layer_artist import SmallMultiplesLayerArtist
 from glue_small_multiples.state import SmallMultiplesViewerState
 from glue_small_multiples.qt.layer_style_editor import SmallMultiplesLayerStyleEditor
 from glue_small_multiples.qt.options_widget import SmallMultiplesOptionsWidget
 
-__all__ = ['MultiplePossibleRoiModeBase', 'MultiplePossibleRoiMode', 
-            'FacetRectangleMode', 'SmallMultiplesViewer']
+__all__ = [
+    "MultiplePossibleRoiModeBase",
+    "MultiplePossibleRoiMode",
+    "FacetRectangleMode",
+    "SmallMultiplesViewer",
+]
 
 
 class MultiplePossibleRoiModeBase(ToolbarModeBase):
     """
     Base class for defining ROIs. ROIs accessible via the roi() method
 
     See RoiMode and ClickRoiMode subclasses for interaction details
 
     An roi_callback function can be provided. When ROIs are finalized (i.e.
     fully defined), this function will be called with the RoiMode object as the
     argument. Clients can use RoiMode.roi() to retrieve the new ROI, and take
     the appropriate action. By default, roi_callback will default to calling an
     ``apply_roi`` method on the data viewer.
     """
+
     persistent = False  # clear the shape when drawing completes?
     disable_on_finalize = True
 
     def __init__(self, viewer, **kwargs):
         """
         Parameters
         ----------
         roi_callback : `func`
             Function that will be called when the ROI is finished being
             defined.
         """
 
         def apply_mode(mode):
             self.viewer.apply_roi(self.roi(), self._col_axis_num, self._row_axis_num)
-        self._roi_callback = kwargs.pop('roi_callback', apply_mode)
+
+        self._roi_callback = kwargs.pop("roi_callback", apply_mode)
         super(MultiplePossibleRoiModeBase, self).__init__(viewer, **kwargs)
         self._roi_tools = []
         self._roi_tool = None
-        self._row_axis_num = 0 
-        self._col_axis_num = 0 
+        self._row_axis_num = 0
+        self._col_axis_num = 0
 
     def close(self, *args):
         self._roi_callback = None
         super(MultiplePossibleRoiModeBase, self).close()
 
     def activate(self):
         # For persistent ROIs, the user might e.g. pan and zoom around before
         # the selection is finalized. The Matplotlib ROIs cache the image
         # background to make things more efficient, but if the user pans/zooms
         # we need to make sure we reset the background.
         # TODO: Re-enable this for multiple patches
         # The following attempt leaves behind patches when
-        # switching facets 
-        #for _roi_tool in self._roi_tools:
+        # switching facets
+        # for _roi_tool in self._roi_tools:
         #    if getattr(_roi_tool, '_mid_selection', False):
         #        _roi_tool._reset_background()
         #    _roi_tool._sync_patch()
         super(MultiplePossibleRoiModeBase, self).activate()
-    
-    
+
     def roi(self):
         """
         The ROI defined by this mouse mode
 
         Returns
         -------
         list of roi : :class:`~glue.core.roi.Roi`
@@ -95,81 +99,76 @@
             self._roi_tool.finalize_selection(event)
         if self._roi_callback is not None:
             self._roi_callback(self)
         if self.disable_on_finalize:
             self.viewer.toolbar.active_tool = None
 
     def clear(self):
-
         for _roi_tool in self._roi_tools:
             _roi_tool.reset()
 
 
 class MultiplePossibleRoiMode(MultiplePossibleRoiModeBase):
     """
     Define Roi Modes via click+drag events.
 
     ROIs are updated continuously on click+drag events, and finalized on each
     mouse release
     """
 
-    status_tip = "CLICK and DRAG to define selection, CTRL-CLICK and DRAG to move selection"
+    status_tip = (
+        "CLICK and DRAG to define selection, CTRL-CLICK and DRAG to move selection"
+    )
 
     def __init__(self, viewer, **kwargs):
-
         super(MultiplePossibleRoiMode, self).__init__(viewer, **kwargs)
 
         self._start_event = None
         self._drag = False
 
     def _update_drag(self, event):
-
         if self._drag or self._start_event is None:
             return
 
-        dx = abs(event.x - self._start_event.x)
-        dy = abs(event.y - self._start_event.y)
-
         status = self._roi_tool.start_selection(self._start_event)
 
         # If start_selection returns False, the selection has not been
         # started and we should abort, so we set self._drag to False in
         # this case.
         self._drag = True if status is None else status
 
     def press(self, event):
-
         self._start_event = event
         super(MultiplePossibleRoiMode, self).press(event)
 
     def move(self, event):
         i = 0
-        for axes,_roi_tool in zip(self._axes_array.flatten(),self._roi_tools):
+        for axes, _roi_tool in zip(self._axes_array.flatten(), self._roi_tools):
             if event.inaxes == axes:
                 self._roi_tool = _roi_tool
-                self._col_axis_num, self._row_axis_num = np.unravel_index(i,self._axes_array.shape)
+                self._col_axis_num, self._row_axis_num = np.unravel_index(
+                    i, self._axes_array.shape
+                )
                 break
-            i+=1
+            i += 1
 
         self._update_drag(event)
         if self._drag:
             self._roi_tool.update_selection(event)
         super(MultiplePossibleRoiMode, self).move(event)
 
     def release(self, event):
-
         if self._drag:
             self._finish_roi(event)
         self._drag = False
         self._start_event = None
         super(MultiplePossibleRoiMode, self).release(event)
 
     def key(self, event):
-
-        if event.key == 'escape':
+        if event.key == "escape":
             for _roi_tool in self._roi_tools:
                 try:
                     self._roi_tool.abort_selection(event)
                 except IndexError:
                     pass
             self._drag = False
             self._drawing = False
@@ -180,92 +179,108 @@
 @viewer_tool
 class FacetRectangleMode(MultiplePossibleRoiMode):
     """
     Defines a Rectangular ROI, accessible via the :meth:`~RectangleMode.roi`
     method
 
     This kind of thing assumes that we have a single self._roi_tool
-    But I think what we want is a list of _roi_tools 
+    But I think what we want is a list of _roi_tools
     """
 
-    icon = 'glue_square'
-    tool_id = 'select:facetrectangle'
-    action_text = 'Rectangular ROI'
-    tool_tip = 'Define a rectangular region of interest'
-    shortcut = 'R'
+    icon = "glue_square"
+    tool_id = "select:facetrectangle"
+    action_text = "Rectangular ROI"
+    tool_tip = "Define a rectangular region of interest"
+    shortcut = "R"
 
     def __init__(self, viewer, **kwargs):
         super(FacetRectangleMode, self).__init__(viewer, **kwargs)
-        data_space = not hasattr(viewer.state, 'plot_mode') or viewer.state.plot_mode == 'rectilinear'
-        self._axes_array = getattr(viewer, 'axes_array', None)
+        data_space = (
+            not hasattr(viewer.state, "plot_mode")
+            or viewer.state.plot_mode == "rectilinear"
+        )
+        self._axes_array = getattr(viewer, "axes_array", None)
         self._roi_tools = []
         if self._axes_array is None:
             return
         for axes in self._axes_array.flatten():
             self._roi_tools.append(roi.MplRectangularROI(axes, data_space=data_space))
 
 
 @decorate_all_methods(defer_draw)
-class SmallMultiplesViewer(MatplotlibScatterMixin, MatplotlibDataViewer, PanTrackerMixin):
-    
-    LABEL = 'Small Multiples Viewer'
-    
+class SmallMultiplesViewer(
+    MatplotlibScatterMixin, MatplotlibDataViewer, PanTrackerMixin
+):
+    LABEL = "Small Multiples Viewer"
+
     _layer_style_widget_cls = SmallMultiplesLayerStyleEditor
     _state_cls = SmallMultiplesViewerState
 
     _options_cls = SmallMultiplesOptionsWidget
     _data_artist_cls = SmallMultiplesLayerArtist
     _subset_artist_cls = SmallMultiplesLayerArtist
 
-    tools = ['select:facetrectangle']
+    tools = ["select:facetrectangle"]
 
     def __init__(self, session, parent=None, state=None):
         proj = None if not state or not state.plot_mode else state.plot_mode
-        MatplotlibDataViewer.__init__(self, session, parent=parent, state=state, projection=proj)
+        MatplotlibDataViewer.__init__(
+            self, session, parent=parent, state=state, projection=proj
+        )
         if self.axes is not None and self.figure is not None:
             self.figure.delaxes(self.axes)
-        self.axes_array = self.figure.subplots(self.state.num_rows, self.state.num_cols,
-                                               sharex=True, sharey=True, squeeze=False)
+        self.axes_array = self.figure.subplots(
+            self.state.num_rows,
+            self.state.num_cols,
+            sharex=True,
+            sharey=True,
+            squeeze=False,
+        )
         self.axes = self.axes_array[0][0]
 
         MatplotlibScatterMixin.setup_callbacks(self)
 
-        self.state.add_callback('num_cols', self._configure_axes_array, priority=9999)
-        self.state.add_callback('num_rows', self._configure_axes_array, priority=9999)
+        self.state.add_callback("num_cols", self._configure_axes_array, priority=9999)
+        self.state.add_callback("num_rows", self._configure_axes_array, priority=9999)
         if state is not None:
             self.state._set_axes_subplots(axes_subplots=self.axes_array)
-            self.state._update_num_rows_cols() # This sets our data_facets
+            self.state._update_num_rows_cols()  # This sets our data_facets
             self._configure_axes_array(force=True)
             self.remove_all_toolbars()
 
-
     def _configure_axes_array(self, force=False, *args):
-
-        with delay_callback(self.state, 'num_cols','num_cols'):
+        with delay_callback(self.state, "num_cols", "num_cols"):
             """
             I took some of this code from _update_projection
             in scatter._update_projection
             """
             # If the axes are the right shape we should just return
-            if (self.axes_array.shape == (self.state.num_rows, self.state.num_cols)) and not force:
+            if (
+                self.axes_array.shape == (self.state.num_rows, self.state.num_cols)
+            ) and not force:
                 return
 
             for ax in self.figure.axes:
                 self.figure.delaxes(ax)
             self.redraw()
 
-            self.axes_array = self.figure.subplots(self.state.num_rows, self.state.num_cols, 
-                                                   sharex=True, sharey=True, squeeze=False)
+            self.axes_array = self.figure.subplots(
+                self.state.num_rows,
+                self.state.num_cols,
+                sharex=True,
+                sharey=True,
+                squeeze=False,
+            )
             self.axes = self.axes_array[0][0]
-            #if not force:
+            # if not force:
             self.remove_all_toolbars()
             self.initialize_toolbar()
             self.state._set_axes_subplots(axes_subplots=self.axes_array)
-            self.axes.callbacks.connect('xlim_changed', self.limits_from_mpl)
-            self.axes.callbacks.connect('ylim_changed', self.limits_from_mpl)
+            self.axes.callbacks.connect("xlim_changed", self.limits_from_mpl)
+            self.axes.callbacks.connect("ylim_changed", self.limits_from_mpl)
             self.update_x_axislabel()
             self.update_y_axislabel()
             self.update_x_ticklabel()
             self.update_y_ticklabel()
             self.state.x_log = self.state.y_log = False
             self.state.reset_limits()
 
@@ -275,46 +290,46 @@
             # We need to update the tick marks
             # to account for the radians/degrees switch in polar mode
             # Also need to add/remove axis labels as necessary
             self._update_axes()
 
             self.figure.canvas.draw_idle()
 
-
     def get_layer_artist(self, cls, layer=None, layer_state=None):
         return cls(self.axes_array, self.state, layer=layer, layer_state=layer_state)
 
     def apply_roi(self, roi, col_axis_num=0, row_axis_num=0, override_mode=None):
         self.redraw()
-        
+
         if len(self.layers) == 0:
             return
 
-        x_date = 'datetime' in self.state.x_kinds
-        y_date = 'datetime' in self.state.y_kinds
-
-        #if x_date or y_date:
-        #   roi = roi.transformed(xfunc=mpl_to_datetime64 if x_date else None,
-        #                          yfunc=mpl_to_datetime64 if y_date else None)
-
-        use_transform = False#self.state.plot_mode != 'rectilinear'
-        subset_state = roi_to_subset_state(roi,
-                                           x_att=self.state.x_att, x_categories=self.state.x_categories,
-                                           y_att=self.state.y_att, y_categories=self.state.y_categories,
-                                           use_pretransform=use_transform)
+        use_transform = False  # self.state.plot_mode != 'rectilinear'
+        subset_state = roi_to_subset_state(
+            roi,
+            x_att=self.state.x_att,
+            x_categories=self.state.x_categories,
+            y_att=self.state.y_att,
+            y_categories=self.state.y_categories,
+            use_pretransform=use_transform,
+        )
         if use_transform:
-            subset_state.pretransform = ProjectionMplTransform(self.state.plot_mode,
-                                                               self.axes.get_xlim(),
-                                                               self.axes.get_ylim(),
-                                                               self.axes.get_xscale(),
-                                                               self.axes.get_yscale())
-        facet_state = self.state.data_facet_subsets[col_axis_num][row_axis_num].subset_state #We need to get this index back from the roi_tool
+            subset_state.pretransform = ProjectionMplTransform(
+                self.state.plot_mode,
+                self.axes.get_xlim(),
+                self.axes.get_ylim(),
+                self.axes.get_xscale(),
+                self.axes.get_yscale(),
+            )
+        facet_state = self.state.data_facet_subsets[col_axis_num][
+            row_axis_num
+        ].subset_state  # We need to get this index back from the roi_tool
         subset_state = subset_state & facet_state
         self.apply_subset_state(subset_state, override_mode=override_mode)
 
     def draw_legend(self, *args):
-        #Old legend logic does not work
+        # Old legend logic does not work
         pass
 
     def _on_resize(self, *args):
-        #Neither does the aspect_ratio call
+        # Neither does the aspect_ratio call
         pass
```

### Comparing `glue-small-multiples-1.1.2/glue_small_multiples/state.py` & `glue-small-multiples-1.2.1/glue_small_multiples/state.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import numpy as np
-from matplotlib.projections import get_projection_names
 
-from echo import delay_callback, CallbackProperty
-from glue.viewers.matplotlib.state import (MatplotlibDataViewerState,
-                                           MatplotlibLayerState,
-                                           DeferredDrawCallbackProperty as DDCProperty,
-                                           DeferredDrawSelectionCallbackProperty as DDSCProperty)
-from glue.core.state_objects import StateAttributeLimitsHelper
+from glue.viewers.matplotlib.state import (
+    DeferredDrawCallbackProperty as DDCProperty,
+    DeferredDrawSelectionCallbackProperty as DDSCProperty,
+)
 from glue.config import session_patch
-from glue.viewers.scatter.state import ScatterLayerState
-from glue.core.data_combo_helper import ManualDataComboHelper, ComponentIDComboHelper, ComboHelper
+from glue.core.data_combo_helper import ManualDataComboHelper, ComponentIDComboHelper
 from glue.core.subset import Subset
-from glue.utils import defer_draw, decorate_all_methods, ensure_numerical
 from glue.viewers.scatter.state import ScatterLayerState, ScatterViewerState
 
 
-__all__ = ['FacetSubset', 'SmallMultiplesViewerState', 'FacetScatterLayerState', 'SmallMultiplesLayerState']
+__all__ = [
+    "FacetSubset",
+    "SmallMultiplesViewerState",
+    "FacetScatterLayerState",
+    "SmallMultiplesLayerState",
+]
+
 
 class FacetSubset(Subset):
     """A convenience class to prevent facet subset labels from
     getting the extra disambiguation stuff.
     """
+
     def __init__(self, data, color=None, alpha=0.5, label=None):
         super().__init__(data, color=color, alpha=alpha, label=label)
 
     @property
     def label(self):
-        """ Convenience access to subset's label """
+        """Convenience access to subset's label"""
         return self._label
 
     @label.setter
     def label(self, value):
         """Do not disambiguate these subsets."""
         self._label = value
 
@@ -38,126 +40,184 @@
 class SmallMultiplesViewerState(ScatterViewerState):
     """
     State for a Small Multiples Viewer
 
     The user can chose to facet on one or two categorical attributes.
     Ideally we should allow them to facet on integer attributes too.
     """
-    col_facet_att = DDSCProperty(docstring='The attribute to facet columns by', default_index=0) #Specifying default_index with a ComboHelper with none does not work
-    row_facet_att = DDSCProperty(docstring='The attribute to facet rows by', default_index=1)
+
+    col_facet_att = DDSCProperty(
+        docstring="The attribute to facet columns by", default_index=0
+    )  # Specifying default_index with a ComboHelper with none does not work
+    row_facet_att = DDSCProperty(
+        docstring="The attribute to facet rows by", default_index=1
+    )
     # We should be able to make these spinners in the GUI that cannot go below 1
-    max_num_cols = DDCProperty(5, docstring='The maximum number of columns to show')
-    max_num_rows = DDCProperty(5, docstring='The maximum number of rows to show')
+    max_num_cols = DDCProperty(5, docstring="The maximum number of columns to show")
+    max_num_rows = DDCProperty(5, docstring="The maximum number of rows to show")
 
     num_cols = DDCProperty(1, docstring="The number of columns to display in the grid")
     num_rows = DDCProperty(1, docstring="The number of rows to display in the grid")
 
-    reference_data = DDSCProperty(docstring='The dataset being displayed')
+    reference_data = DDSCProperty(docstring="The dataset being displayed")
 
     def __init__(self, **kwargs):
         self.axes_subplots = None
 
         super().__init__()
-        self.data_facet_masks = [] # We can only initialize this if we have a dataset defined
+        self.data_facet_masks = (
+            []
+        )  # We can only initialize this if we have a dataset defined
         self.data_facet_subsets = []
         self.temp_num_cols = 0
         self.temp_num_rows = 0
-        self.ref_data_helper = ManualDataComboHelper(self, 'reference_data')
-        self.col_facet_att_helper = ComponentIDComboHelper(self, 'col_facet_att', categorical=True, numeric=False)
-        self.row_facet_att_helper = ComponentIDComboHelper(self, 'row_facet_att', categorical=True, numeric=False, none=True)
+        self.ref_data_helper = ManualDataComboHelper(self, "reference_data")
+        self.col_facet_att_helper = ComponentIDComboHelper(
+            self, "col_facet_att", categorical=True, numeric=False
+        )
+        self.row_facet_att_helper = ComponentIDComboHelper(
+            self, "row_facet_att", categorical=True, numeric=False, none=True
+        )
         self.update_from_dict(kwargs)
 
-        self.add_callback('col_facet_att', self._update_num_rows_cols, priority=10000)
-        self.add_callback('row_facet_att', self._update_num_rows_cols, priority=10000)
-        self.add_callback('reference_data', self._update_num_rows_cols, priority=10000)
-        self.add_callback('max_num_cols', self._update_num_rows_cols, priority=10000) #This should be linked to a QSpinBox to force integers
-        self.add_callback('max_num_rows', self._update_num_rows_cols, priority=10000)
+        self.add_callback("col_facet_att", self._update_num_rows_cols, priority=10000)
+        self.add_callback("row_facet_att", self._update_num_rows_cols, priority=10000)
+        self.add_callback("reference_data", self._update_num_rows_cols, priority=10000)
+        self.add_callback(
+            "max_num_cols", self._update_num_rows_cols, priority=10000
+        )  # This should be linked to a QSpinBox to force integers
+        self.add_callback("max_num_rows", self._update_num_rows_cols, priority=10000)
 
         self._facets_changed()
 
     def _set_axes_subplots(self, axes_subplots=None):
         if axes_subplots is None:
             return
         self.axes_subplots = axes_subplots
 
     def _update_num_rows_cols(self, *args):
-        #with delay_callback(self, 'num_cols', 'num_rows'):
+        # with delay_callback(self, 'num_cols', 'num_rows'):
 
-        if (self.reference_data is None) or (self.max_num_rows is None) or (self.max_num_cols is None):
+        if (
+            (self.reference_data is None)
+            or (self.max_num_rows is None)
+            or (self.max_num_cols is None)
+        ):
             return
 
         if self.col_facet_att is not None:
-            self.temp_num_cols = min(int(self.max_num_cols), len(self.reference_data[self.col_facet_att].categories))
+            self.temp_num_cols = min(
+                int(self.max_num_cols),
+                len(self.reference_data[self.col_facet_att].categories),
+            )
         else:
             self.temp_num_cols = 1
         if self.row_facet_att is not None:
-            self.temp_num_rows = min(int(self.max_num_rows), len(self.reference_data[self.row_facet_att].categories))
+            self.temp_num_rows = min(
+                int(self.max_num_rows),
+                len(self.reference_data[self.row_facet_att].categories),
+            )
         else:
             self.temp_num_rows = 1
 
         self._facets_changed()
-        if (self.num_cols != self.temp_num_cols) or (self.num_rows != self.temp_num_rows):
+        if (self.num_cols != self.temp_num_cols) or (
+            self.num_rows != self.temp_num_rows
+        ):
             self.num_cols = self.temp_num_cols
             self.num_rows = self.temp_num_rows
 
     def _facets_changed(self, *args):
-
-        if ((self.col_facet_att is None) and (self.row_facet_att is None)) or (self.reference_data is  None):
+        if ((self.col_facet_att is None) and (self.row_facet_att is None)) or (
+            self.reference_data is None
+        ):
             return
 
         self.data_facet_masks = []
         self.data_facet_subsets = []
         # We create both a simple mask and a subset representing the facet.
         # This is redundant, but the Density mode really wants a subset
         # and the regular/point mode wants a precomputed mask
         # TODO: Remove this redundancy
         try:
-            col_facet_masks  = []
+            col_facet_masks = []
             col_facet_subsets = []
             if self.col_facet_att is not None:
-                for col_i in range(self.temp_num_cols): 
-                    col_facet = self.reference_data[self.col_facet_att].categories[col_i]
+                for col_i in range(self.temp_num_cols):
+                    col_facet = self.reference_data[self.col_facet_att].categories[
+                        col_i
+                    ]
                     col_facet_data = self.reference_data[self.col_facet_att].ravel()
-                    col_facet_mask = np.ma.masked_where(col_facet_data != col_facet, col_facet_data)
-                    facet_state = self.reference_data.id[self.col_facet_att] == col_facet
-                    subset = FacetSubset(self.reference_data,label=f"{self.col_facet_att.label}={col_facet}") 
+                    col_facet_mask = np.ma.masked_where(
+                        col_facet_data != col_facet, col_facet_data
+                    )
+                    facet_state = (
+                        self.reference_data.id[self.col_facet_att] == col_facet
+                    )
+                    subset = FacetSubset(
+                        self.reference_data,
+                        label=f"{self.col_facet_att.label}={col_facet}",
+                    )
                     subset.subset_state = facet_state
                     col_facet_subsets.append(subset)
                     col_facet_masks.append(col_facet_mask)
             else:
-                col_facet_masks = [np.ma.masked_where(False, self.reference_data[self.row_facet_att].ravel())]
-                facet_state = self.reference_data.id[self.row_facet_att] != '***' # FIXME -- this is a hack to get the full subset
-                subset = FacetSubset(self.reference_data, label=f" ") 
+                col_facet_masks = [
+                    np.ma.masked_where(
+                        False, self.reference_data[self.row_facet_att].ravel()
+                    )
+                ]
+                facet_state = (
+                    self.reference_data.id[self.row_facet_att] != "***"
+                )  # FIXME -- this is a hack to get the full subset
+                subset = FacetSubset(self.reference_data, label=" ")
                 subset.subset_state = facet_state
                 col_facet_subsets.append(subset)
 
-            row_facet_masks  = []
+            row_facet_masks = []
             row_facet_subsets = []
             if self.row_facet_att is not None:
                 row_facet_masks = []
                 for row_i in range(self.temp_num_rows):
-                    row_facet = self.reference_data[self.row_facet_att].categories[row_i]
+                    row_facet = self.reference_data[self.row_facet_att].categories[
+                        row_i
+                    ]
                     row_facet_data = self.reference_data[self.row_facet_att].ravel()
-                    row_facet_mask = np.ma.masked_where(row_facet_data != row_facet, row_facet_data)
-                    facet_state = self.reference_data.id[self.row_facet_att] == row_facet
-                    subset = FacetSubset(self.reference_data,label=f"{self.row_facet_att.label}={row_facet}") 
+                    row_facet_mask = np.ma.masked_where(
+                        row_facet_data != row_facet, row_facet_data
+                    )
+                    facet_state = (
+                        self.reference_data.id[self.row_facet_att] == row_facet
+                    )
+                    subset = FacetSubset(
+                        self.reference_data,
+                        label=f"{self.row_facet_att.label}={row_facet}",
+                    )
                     subset.subset_state = facet_state
                     row_facet_subsets.append(subset)
                     row_facet_masks.append(row_facet_mask)
             else:
-                row_facet_masks = [np.ma.masked_where(False, self.reference_data[self.col_facet_att].ravel())]
-                facet_state = self.reference_data.id[self.col_facet_att] != '***' # FIXME -- this is a hack to get the full subset
-                subset = FacetSubset(self.reference_data, label=f" ") 
+                row_facet_masks = [
+                    np.ma.masked_where(
+                        False, self.reference_data[self.col_facet_att].ravel()
+                    )
+                ]
+                facet_state = (
+                    self.reference_data.id[self.col_facet_att] != "***"
+                )  # FIXME -- this is a hack to get the full subset
+                subset = FacetSubset(self.reference_data, label=" ")
                 subset.subset_state = facet_state
                 row_facet_subsets.append(subset)
 
             for row_facet_subset in row_facet_subsets:
                 col = []
                 for col_facet_subset in col_facet_subsets:
-                    facet_subset_state = row_facet_subset.subset_state & col_facet_subset.subset_state
+                    facet_subset_state = (
+                        row_facet_subset.subset_state & col_facet_subset.subset_state
+                    )
                     col.append(facet_subset_state)
                 self.data_facet_subsets.append(col)
 
             for row_facet_mask in row_facet_masks:
                 col = []
                 for col_facet_mask in col_facet_masks:
                     facet_mask = row_facet_mask.mask | col_facet_mask.mask
@@ -169,15 +229,15 @@
 
     def _layers_changed(self, *args):
         """
         This probably isn't really correct for ref_data
         """
 
         layers_data = self.layers_data
-        layers_data_cache = getattr(self, '_layers_data_cache', [])
+        layers_data_cache = getattr(self, "_layers_data_cache", [])
 
         if layers_data == layers_data_cache:
             return
 
         self.ref_data_helper.set_multiple_data(layers_data)
         self.x_att_helper.set_multiple_data(layers_data)
         self.y_att_helper.set_multiple_data(layers_data)
@@ -188,76 +248,84 @@
 
 
 class FacetScatterLayerState(ScatterLayerState):
     """A simple superclass for the Facet subsets
     to add titles on the axes and custom density
     map logic.
     """
+
     def __init__(self, viewer_state=None, layer=None, **kwargs):
         super().__init__(viewer_state=viewer_state, layer=layer)
-            #self.update_from_dict(kwargs)
+        # self.update_from_dict(kwargs)
 
     def _update_title(self):
         # TODO: title should be a callback property?
         try:
             self.title = self.facet_subset.label
-        except AttributeError: #This is for an AndState
-            state1 = str(self.facet_subset.state1).strip("()").replace('==','=')
-            if '***' in state1: # FIXME: Hack for empty subset
+        except AttributeError:  # This is for an AndState
+            state1 = str(self.facet_subset.state1).strip("()").replace("==", "=")
+            if "***" in state1:  # FIXME: Hack for empty subset
                 state1 = None
-            state2 = str(self.facet_subset.state2).strip("()").replace('==','=')
-            if '***' in state2: # FIXME: Hack for empty subset
+            state2 = str(self.facet_subset.state2).strip("()").replace("==", "=")
+            if "***" in state2:  # FIXME: Hack for empty subset
                 state2 = None
             if state1 and state2:
-                self.title  = f"{state1} and {state2}"
+                self.title = f"{state1} and {state2}"
             else:
                 self.title = state1 or state2
 
     def compute_density_map(self, bins=None, range=None):
         if not self.markers_visible or not self.density_map:
             return np.zeros(bins)
-        
+
         if isinstance(self.layer, Subset):
             data = self.layer.data
             subset_state = self.layer.subset_state & self.facet_subset.subset_state
         else:
             data = self.layer
             subset_state = self.facet_subset.subset_state
-        count = data.compute_histogram([self.viewer_state.y_att, self.viewer_state.x_att],
-                                        subset_state=subset_state, bins=bins,
-                                        log=(self.viewer_state.y_log, self.viewer_state.x_log),
-                                        range=range)
-        if self.cmap_mode == 'Fixed':
+        count = data.compute_histogram(
+            [self.viewer_state.y_att, self.viewer_state.x_att],
+            subset_state=subset_state,
+            bins=bins,
+            log=(self.viewer_state.y_log, self.viewer_state.x_log),
+            range=range,
+        )
+        if self.cmap_mode == "Fixed":
             return count
         else:
-            total = data.compute_histogram([self.viewer_state.y_att, self.viewer_state.x_att],
-                                            subset_state=subset_state, bins=bins,
-                                            weights=self.cmap_att,
-                                            log=(self.viewer_state.y_log, self.viewer_state.x_log),
-                                            range=range)
+            total = data.compute_histogram(
+                [self.viewer_state.y_att, self.viewer_state.x_att],
+                subset_state=subset_state,
+                bins=bins,
+                weights=self.cmap_att,
+                log=(self.viewer_state.y_log, self.viewer_state.x_log),
+                range=range,
+            )
             return total / count
 
 
 @session_patch(priority=0)
 def strip_out_facet_subset_states(rec):
-    """ We regenerate FacetScatterLayerState objects
+    """We regenerate FacetScatterLayerState objects
     from the other state objects so we remove them
     from the session file.
 
     TODO: Write custom save/restore functions for
     FacetScatterLayerState objects so we don't have
     to patch the session file.
     """
     for key, value in rec.items():
-        if 'CallbackList' in key:
-            layers = value.get('values',[])
+        if "CallbackList" in key:
+            layers = value.get("values", [])
             if layers:
-                value['values'] = [x for x in layers if "FacetScatterLayer" not in x]
-    rec = dict((k,v) for k, v in rec.items() if "FacetScatterLayer" not in k)
+                value["values"] = [x for x in layers if "FacetScatterLayer" not in x]
+    rec = dict((k, v) for k, v in rec.items() if "FacetScatterLayer" not in k)
 
 
 class SmallMultiplesLayerState(ScatterLayerState):
     """
     Currently this is the same as ScatterLayerState
     """
+
     def __init__(self, viewer_state=None, layer=None, **kwargs):
-        super().__init__(viewer_state=viewer_state, layer=layer, **kwargs)
+        super().__init__(viewer_state=viewer_state, layer=layer, **kwargs)
```

### Comparing `glue-small-multiples-1.1.2/glue_small_multiples/utils.py` & `glue-small-multiples-1.2.1/glue_small_multiples/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 class PanTrackerMixin:
     """
     Helper class that tracks drag events when using the pan/zoom mode in the matplotlib toolbar.
-    
+
     The `panning` holds whether the user is currently panning+zooming, and the `on_pan_end` method
     (a no-op that can be overloaded) is called immediately after a pan+zoom ends.
-    
+
     This can be used to skip expensive operations during pan+zoom, to keep that interaction fluid.
     """
+
     def init_pan_tracking(self, axes):
         self.panning = False
         self.__axes = axes
-        axes.figure.canvas.mpl_connect('button_press_event', self._on_press)
-        axes.figure.canvas.mpl_connect('button_release_event', self._on_release)
-    
+        axes.figure.canvas.mpl_connect("button_press_event", self._on_press)
+        axes.figure.canvas.mpl_connect("button_release_event", self._on_release)
+
     def _on_press(self, event=None, force=False):
         try:
             mode = self.__axes.figure.canvas.toolbar.mode
         except AttributeError:  # pragma: nocover
             return
-        self.panning = mode == 'pan/zoom'
-    
+        self.panning = mode == "pan/zoom"
+
     def _on_release(self, event=None):
         was_panning = self.panning
         self.panning = False
-    
+
         if was_panning:
             self.on_pan_end()
-    
+
     def on_pan_end(self):
         pass
```

### Comparing `glue-small-multiples-1.1.2/glue_small_multiples.egg-info/PKG-INFO` & `glue-small-multiples-1.2.1/glue_small_multiples.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: glue-small-multiples
-Version: 1.1.2
+Version: 1.2.1
 Summary: A viewer for small multiples
 Home-page: https://www.gluesolutions.io
 Author: glue solutions, inc.
 Author-email: jfoster@gluesolutions.io
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: qt
 Provides-Extra: test
+Provides-Extra: qt
+Provides-Extra: glue
 
 # small multiples
 
 Add a small-multiples viewer to glue, allowing for the easy comparison of different partitions or facets of a dataset.
 
 ![Example Image](https://user-images.githubusercontent.com/3639698/191285037-598dc355-d185-4a23-99d8-318429272c4b.png)
```

### Comparing `glue-small-multiples-1.1.2/setup.cfg` & `glue-small-multiples-1.2.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -4,40 +4,44 @@
 author = glue solutions, inc.
 author_email = jfoster@gluesolutions.io
 classifiers = 
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Visualization
 	License :: OSI Approved :: BSD License
 description = A viewer for small multiples
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 zip_safe = False
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 setup_requires = setuptools_scm
-install_requires = 
-	glue-core>=1.6
 
 [options.entry_points]
 glue.plugins = 
 	glue_small_multiples = glue_small_multiples:setup
 
 [options.extras_require]
-qt = 
-	PyQt5>=5.9
 test = 
 	pytest
+	pytest-qt
+	pytest-faulthandler
+	mock
+qt = 
+	PyQt5>=5.9
+glue = 
+	glue-core
 
 [options.package_data]
 * = *.png, *.ui, *.glu, *.hdf5, *.fits, *.xlsx, *.txt, *.csv, *.svg, *.vot, *.bgz, *.tbi
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

