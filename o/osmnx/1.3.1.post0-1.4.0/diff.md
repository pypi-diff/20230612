# Comparing `tmp/osmnx-1.3.1.post0.tar.gz` & `tmp/osmnx-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osmnx-1.3.1.post0.tar", last modified: Fri May 26 21:13:03 2023, max compression
+gzip compressed data, was "osmnx-1.4.0.tar", last modified: Mon Jun 12 04:16:56 2023, max compression
```

## Comparing `osmnx-1.3.1.post0.tar` & `osmnx-1.4.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 geoff      (501) staff       (20)        0 2023-05-26 21:13:03.236554 osmnx-1.3.1.post0/
--rw-r--r--   0 geoff      (501) staff       (20)    19296 2023-05-26 20:50:26.000000 osmnx-1.3.1.post0/CHANGELOG.md
--rw-r--r--   0 geoff      (501) staff       (20)     1111 2022-12-22 03:13:01.000000 osmnx-1.3.1.post0/LICENSE.txt
--rw-r--r--   0 geoff      (501) staff       (20)       45 2022-12-14 16:25:06.000000 osmnx-1.3.1.post0/MANIFEST.in
--rw-r--r--   0 geoff      (501) staff       (20)     2324 2023-05-26 21:13:03.236627 osmnx-1.3.1.post0/PKG-INFO
--rw-r--r--   0 geoff      (501) staff       (20)     4357 2022-12-28 21:55:23.000000 osmnx-1.3.1.post0/README.md
-drwxr-xr-x   0 geoff      (501) staff       (20)        0 2023-05-26 21:13:03.235529 osmnx-1.3.1.post0/osmnx/
--rw-r--r--   0 geoff      (501) staff       (20)       73 2022-09-03 08:24:38.000000 osmnx-1.3.1.post0/osmnx/__init__.py
--rw-r--r--   0 geoff      (501) staff       (20)     1993 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/osmnx/_api.py
--rw-r--r--   0 geoff      (501) staff       (20)      505 2022-12-17 00:29:35.000000 osmnx-1.3.1.post0/osmnx/_errors.py
--rw-r--r--   0 geoff      (501) staff       (20)     1758 2022-12-17 00:29:35.000000 osmnx-1.3.1.post0/osmnx/_polygon_features.py
--rw-r--r--   0 geoff      (501) staff       (20)       58 2023-05-26 20:46:22.000000 osmnx-1.3.1.post0/osmnx/_version.py
--rw-r--r--   0 geoff      (501) staff       (20)    12165 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/osmnx/bearing.py
--rw-r--r--   0 geoff      (501) staff       (20)    17675 2023-05-11 18:07:46.000000 osmnx-1.3.1.post0/osmnx/distance.py
--rw-r--r--   0 geoff      (501) staff       (20)    29369 2023-05-22 03:49:01.000000 osmnx-1.3.1.post0/osmnx/downloader.py
--rw-r--r--   0 geoff      (501) staff       (20)     9178 2022-12-17 00:29:35.000000 osmnx-1.3.1.post0/osmnx/elevation.py
--rw-r--r--   0 geoff      (501) staff       (20)     5725 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/osmnx/folium.py
--rw-r--r--   0 geoff      (501) staff       (20)     8406 2023-01-14 20:32:17.000000 osmnx-1.3.1.post0/osmnx/geocoder.py
--rw-r--r--   0 geoff      (501) staff       (20)    39964 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/osmnx/geometries.py
--rw-r--r--   0 geoff      (501) staff       (20)    29082 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/osmnx/graph.py
--rw-r--r--   0 geoff      (501) staff       (20)    14242 2023-03-20 17:40:38.000000 osmnx-1.3.1.post0/osmnx/io.py
--rw-r--r--   0 geoff      (501) staff       (20)    15244 2023-05-24 23:37:40.000000 osmnx-1.3.1.post0/osmnx/osm_xml.py
--rw-r--r--   0 geoff      (501) staff       (20)    27017 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/osmnx/plot.py
--rw-r--r--   0 geoff      (501) staff       (20)     6343 2022-12-17 00:29:36.000000 osmnx-1.3.1.post0/osmnx/projection.py
--rw-r--r--   0 geoff      (501) staff       (20)     7996 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/osmnx/settings.py
--rw-r--r--   0 geoff      (501) staff       (20)    25685 2023-03-20 17:40:38.000000 osmnx-1.3.1.post0/osmnx/simplification.py
--rw-r--r--   0 geoff      (501) staff       (20)     9144 2023-05-22 03:49:01.000000 osmnx-1.3.1.post0/osmnx/speed.py
--rw-r--r--   0 geoff      (501) staff       (20)    12691 2022-12-22 03:13:01.000000 osmnx-1.3.1.post0/osmnx/stats.py
--rw-r--r--   0 geoff      (501) staff       (20)     6740 2022-12-17 00:29:36.000000 osmnx-1.3.1.post0/osmnx/truncate.py
--rw-r--r--   0 geoff      (501) staff       (20)    10547 2023-03-20 17:40:38.000000 osmnx-1.3.1.post0/osmnx/utils.py
--rw-r--r--   0 geoff      (501) staff       (20)    16245 2023-02-22 17:24:42.000000 osmnx-1.3.1.post0/osmnx/utils_geo.py
--rw-r--r--   0 geoff      (501) staff       (20)    17793 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/osmnx/utils_graph.py
-drwxr-xr-x   0 geoff      (501) staff       (20)        0 2023-05-26 21:13:03.236242 osmnx-1.3.1.post0/osmnx.egg-info/
--rw-r--r--   0 geoff      (501) staff       (20)     2324 2023-05-26 21:13:03.000000 osmnx-1.3.1.post0/osmnx.egg-info/PKG-INFO
--rw-r--r--   0 geoff      (501) staff       (20)      691 2023-05-26 21:13:03.000000 osmnx-1.3.1.post0/osmnx.egg-info/SOURCES.txt
--rw-r--r--   0 geoff      (501) staff       (20)        1 2023-05-26 21:13:03.000000 osmnx-1.3.1.post0/osmnx.egg-info/dependency_links.txt
--rw-r--r--   0 geoff      (501) staff       (20)      208 2023-05-26 21:13:03.000000 osmnx-1.3.1.post0/osmnx.egg-info/requires.txt
--rw-r--r--   0 geoff      (501) staff       (20)        6 2023-05-26 21:13:03.000000 osmnx-1.3.1.post0/osmnx.egg-info/top_level.txt
--rw-r--r--   0 geoff      (501) staff       (20)      110 2023-05-24 23:37:40.000000 osmnx-1.3.1.post0/requirements.txt
--rw-r--r--   0 geoff      (501) staff       (20)      405 2023-05-26 21:13:03.236984 osmnx-1.3.1.post0/setup.cfg
--rw-r--r--   0 geoff      (501) staff       (20)     3012 2023-05-26 20:46:40.000000 osmnx-1.3.1.post0/setup.py
-drwxr-xr-x   0 geoff      (501) staff       (20)        0 2023-05-26 21:13:03.236392 osmnx-1.3.1.post0/tests/
--rwxr-xr-x   0 geoff      (501) staff       (20)    20089 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/tests/test_osmnx.py
+drwxr-xr-x   0 geoff      (501) staff       (20)        0 2023-06-12 04:16:56.355613 osmnx-1.4.0/
+-rw-r--r--   0 geoff      (501) staff       (20)    20162 2023-06-12 04:14:56.000000 osmnx-1.4.0/CHANGELOG.md
+-rw-r--r--   0 geoff      (501) staff       (20)     1111 2022-12-22 03:13:01.000000 osmnx-1.4.0/LICENSE.txt
+-rw-r--r--   0 geoff      (501) staff       (20)       45 2022-12-14 16:25:06.000000 osmnx-1.4.0/MANIFEST.in
+-rw-r--r--   0 geoff      (501) staff       (20)     2400 2023-06-12 04:16:56.355682 osmnx-1.4.0/PKG-INFO
+-rw-r--r--   0 geoff      (501) staff       (20)     4477 2023-06-12 04:14:56.000000 osmnx-1.4.0/README.md
+drwxr-xr-x   0 geoff      (501) staff       (20)        0 2023-06-12 04:16:56.354583 osmnx-1.4.0/osmnx/
+-rw-r--r--   0 geoff      (501) staff       (20)       73 2022-09-03 08:24:38.000000 osmnx-1.4.0/osmnx/__init__.py
+-rw-r--r--   0 geoff      (501) staff       (20)     1990 2023-05-26 21:21:17.000000 osmnx-1.4.0/osmnx/_api.py
+-rw-r--r--   0 geoff      (501) staff       (20)      505 2022-12-17 00:29:35.000000 osmnx-1.4.0/osmnx/_errors.py
+-rw-r--r--   0 geoff      (501) staff       (20)     1758 2022-12-17 00:29:35.000000 osmnx-1.4.0/osmnx/_polygon_features.py
+-rw-r--r--   0 geoff      (501) staff       (20)       52 2023-06-12 04:14:56.000000 osmnx-1.4.0/osmnx/_version.py
+-rw-r--r--   0 geoff      (501) staff       (20)    10201 2023-06-07 21:57:18.000000 osmnx-1.4.0/osmnx/bearing.py
+-rw-r--r--   0 geoff      (501) staff       (20)    18742 2023-06-07 21:57:18.000000 osmnx-1.4.0/osmnx/distance.py
+-rw-r--r--   0 geoff      (501) staff       (20)    29369 2023-05-22 03:49:01.000000 osmnx-1.4.0/osmnx/downloader.py
+-rw-r--r--   0 geoff      (501) staff       (20)     9582 2023-06-07 21:57:18.000000 osmnx-1.4.0/osmnx/elevation.py
+-rw-r--r--   0 geoff      (501) staff       (20)     6811 2023-05-29 21:58:27.000000 osmnx-1.4.0/osmnx/folium.py
+-rw-r--r--   0 geoff      (501) staff       (20)     8401 2023-06-07 16:58:51.000000 osmnx-1.4.0/osmnx/geocoder.py
+-rw-r--r--   0 geoff      (501) staff       (20)    39543 2023-06-07 16:58:51.000000 osmnx-1.4.0/osmnx/geometries.py
+-rw-r--r--   0 geoff      (501) staff       (20)    29141 2023-06-03 07:30:43.000000 osmnx-1.4.0/osmnx/graph.py
+-rw-r--r--   0 geoff      (501) staff       (20)    14243 2023-05-29 21:58:27.000000 osmnx-1.4.0/osmnx/io.py
+-rw-r--r--   0 geoff      (501) staff       (20)    15202 2023-06-03 07:30:43.000000 osmnx-1.4.0/osmnx/osm_xml.py
+-rw-r--r--   0 geoff      (501) staff       (20)    31933 2023-06-07 16:17:03.000000 osmnx-1.4.0/osmnx/plot.py
+-rw-r--r--   0 geoff      (501) staff       (20)     6384 2023-06-07 17:42:53.000000 osmnx-1.4.0/osmnx/projection.py
+-rw-r--r--   0 geoff      (501) staff       (20)     8038 2023-05-26 21:21:17.000000 osmnx-1.4.0/osmnx/settings.py
+-rw-r--r--   0 geoff      (501) staff       (20)    25685 2023-03-20 17:40:38.000000 osmnx-1.4.0/osmnx/simplification.py
+-rw-r--r--   0 geoff      (501) staff       (20)     9554 2023-06-07 21:57:18.000000 osmnx-1.4.0/osmnx/speed.py
+-rw-r--r--   0 geoff      (501) staff       (20)    12691 2022-12-22 03:13:01.000000 osmnx-1.4.0/osmnx/stats.py
+-rw-r--r--   0 geoff      (501) staff       (20)     6740 2022-12-17 00:29:36.000000 osmnx-1.4.0/osmnx/truncate.py
+-rw-r--r--   0 geoff      (501) staff       (20)    10548 2023-05-29 21:58:27.000000 osmnx-1.4.0/osmnx/utils.py
+-rw-r--r--   0 geoff      (501) staff       (20)    16281 2023-06-07 21:57:18.000000 osmnx-1.4.0/osmnx/utils_geo.py
+-rw-r--r--   0 geoff      (501) staff       (20)    18237 2023-05-29 21:58:27.000000 osmnx-1.4.0/osmnx/utils_graph.py
+drwxr-xr-x   0 geoff      (501) staff       (20)        0 2023-06-12 04:16:56.355327 osmnx-1.4.0/osmnx.egg-info/
+-rw-r--r--   0 geoff      (501) staff       (20)     2400 2023-06-12 04:16:56.000000 osmnx-1.4.0/osmnx.egg-info/PKG-INFO
+-rw-r--r--   0 geoff      (501) staff       (20)      691 2023-06-12 04:16:56.000000 osmnx-1.4.0/osmnx.egg-info/SOURCES.txt
+-rw-r--r--   0 geoff      (501) staff       (20)        1 2023-06-12 04:16:56.000000 osmnx-1.4.0/osmnx.egg-info/dependency_links.txt
+-rw-r--r--   0 geoff      (501) staff       (20)      241 2023-06-12 04:16:56.000000 osmnx-1.4.0/osmnx.egg-info/requires.txt
+-rw-r--r--   0 geoff      (501) staff       (20)        6 2023-06-12 04:16:56.000000 osmnx-1.4.0/osmnx.egg-info/top_level.txt
+-rw-r--r--   0 geoff      (501) staff       (20)       82 2023-06-12 04:14:56.000000 osmnx-1.4.0/requirements.txt
+-rw-r--r--   0 geoff      (501) staff       (20)      405 2023-06-12 04:16:56.356003 osmnx-1.4.0/setup.cfg
+-rw-r--r--   0 geoff      (501) staff       (20)     3143 2023-06-12 04:14:56.000000 osmnx-1.4.0/setup.py
+drwxr-xr-x   0 geoff      (501) staff       (20)        0 2023-06-12 04:16:56.355461 osmnx-1.4.0/tests/
+-rwxr-xr-x   0 geoff      (501) staff       (20)    20890 2023-06-07 21:57:18.000000 osmnx-1.4.0/tests/test_osmnx.py
```

### Comparing `osmnx-1.3.1.post0/CHANGELOG.md` & `osmnx-1.4.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,26 @@
 # Change log
 
+## TBD
+
+  - adopt NEP 29 policy for minimum required Python and NumPy versions
+
+## 1.4.0 (2023-06-11)
+
+  - verify edge weight attribute values before solving shortest paths
+  - provide consistent error when no data elements are returned from Overpass
+  - add route_to_gdf function to utils_graph module to return a GeoDataFrame of the edges in a path
+  - deprecate the get_route_edge_attributes function in favor of the new route_to_gdf function
+  - deprecate folium module in favor of using geopandas.GeoDataFrame.explore directly
+  - deprecate precision parameter in bearing, distance, elevation, and speed modules' functions
+  - deprecate utils_geo.round_geometry_coords function
+  - move plot_orientation function from bearing module to plot module
+  - make matplotlib an optional dependency required only for the plot module
+  - drop pyproj package dependency
+
 ## 1.3.1.post0 (2023-05-26)
 
   - add Python 3.8 compatibility back for one final release
 
 ## 1.3.1 (2023-05-24)
 
   - improve DNS resolution when using proxies or on networks blocking DNS-over-HTTPS
```

### Comparing `osmnx-1.3.1.post0/LICENSE.txt` & `osmnx-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1.post0/PKG-INFO` & `osmnx-1.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: osmnx
-Version: 1.3.1.post0
+Version: 1.4.0
 Summary: Retrieve, model, analyze, and visualize OpenStreetMap street networks and other spatial data
 Home-page: https://github.com/gboeing/osmnx
 Author: Geoff Boeing
 Author-email: boeing@usc.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: GIS
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: GIS
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: all
 Provides-Extra: entropy
 Provides-Extra: nearest_neighbor
+Provides-Extra: visualization
 Provides-Extra: raster
-Provides-Extra: web_map
 License-File: LICENSE.txt
 
 
 **OSMnx** is a Python package that lets you download spatial data and
 model, project, visualize, and analyze real-world street networks from
 OpenStreetMap's APIs. Users can download and model walkable, drivable, or
 bikeable urban networks with a single line of Python code, and then easily
```

### Comparing `osmnx-1.3.1.post0/README.md` & `osmnx-1.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [![PyPI Version](https://badge.fury.io/py/osmnx.svg)](https://badge.fury.io/py/osmnx)
-[![PyPI Downloads](https://img.shields.io/pypi/dm/osmnx.svg)](https://badge.fury.io/py/osmnx)
+[![PyPI Downloads](https://static.pepy.tech/personalized-badge/osmnx?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=downloads)](https://pepy.tech/project/osmnx)
 [![Anaconda Downloads](https://anaconda.org/conda-forge/osmnx/badges/downloads.svg)](https://anaconda.org/conda-forge/osmnx)
 [![Documentation Status](https://readthedocs.org/projects/osmnx/badge/?version=latest)](https://osmnx.readthedocs.io/)
 [![Build Status](https://github.com/gboeing/osmnx/workflows/tests/badge.svg?branch=main)](https://github.com/gboeing/osmnx/actions?query=workflow%3A%22tests%22)
 [![Coverage Status](https://codecov.io/gh/gboeing/osmnx/branch/main/graph/badge.svg)](https://codecov.io/gh/gboeing/osmnx)
 
 # OSMnx
 
-**OSMnx** is a Python package that lets you download geospatial data from OpenStreetMap and model, project, visualize, and analyze real-world street networks and any other geospatial geometries. You can download and model walkable, drivable, or bikeable urban networks with a single line of Python code then easily analyze and visualize them. You can just as easily download and work with other infrastructure types, amenities/points of interest, building footprints, elevation data, street bearings/orientations, and speed/travel time.
+**OSMnx** is a Python package that lets you download geospatial data from OpenStreetMap and model, project, visualize, and analyze real-world street networks and any other geospatial geometries. You can download and model walkable, drivable, or bikeable urban networks with a single line of Python code then easily analyze and visualize them. You can just as easily download and work with other infrastructure types, amenities/points of interest, building footprints, elevation data, street bearings/orientations, and speed/travel time. OSMnx is pronounced as the initialism: "oh-ess-em-en-ecks".
 
 If you use OSMnx in your work, please cite the journal article.
 
 **Citation info**: Boeing, G. 2017. "[OSMnx: New Methods for Acquiring, Constructing, Analyzing, and Visualizing Complex Street Networks](https://geoffboeing.com/publications/osmnx-complex-street-networks/)." *Computers, Environment and Urban Systems* 65, 126-139. doi:10.1016/j.compenvurbsys.2017.05.004
 
 
 ## Getting Started
@@ -25,32 +25,31 @@
 *What can I do with OSMnx?* Check out recent [projects](https://geoffboeing.com/2018/03/osmnx-features-roundup/) and blog posts that use OSMnx.
 
 *I have a usage question.* Please ask it on [StackOverflow](https://stackoverflow.com/search?q=osmnx).
 
 
 ## Features
 
-OSMnx is built on top of [GeoPandas](https://geopandas.org/), [NetworkX](https://networkx.org/), and [matplotlib](https://matplotlib.org/) and interacts with [OpenStreetMap](https://www.openstreetmap.org/) APIs to:
+OSMnx is built on top of [NetworkX](https://networkx.org/) and [GeoPandas](https://geopandas.org/), and interacts with [OpenStreetMap](https://www.openstreetmap.org/) APIs to:
 
   * Download and model street networks or other networked infrastructure anywhere in the world with a single line of code
   * Download any other spatial geometries, place boundaries, building footprints, or points of interest as a GeoDataFrame
   * Download by city name, polygon, bounding box, or point/address + network distance
   * Download drivable, walkable, bikeable, or all street networks
   * Download node elevations and calculate edge grades (inclines)
   * Impute missing speeds and calculate graph edge travel times
   * Simplify and correct the network's topology to clean-up nodes and consolidate intersections
   * Fast map-matching of points, routes, or trajectories to nearest graph edges or nodes
   * Save networks to disk as shapefiles, GeoPackages, and GraphML
   * Save/load street network to/from a local .osm XML file
   * Conduct topological and spatial analyses to automatically calculate dozens of indicators
   * Calculate and visualize street bearings and orientations
   * Calculate and visualize shortest-path routes that minimize distance, travel time, elevation, etc
-  * Visualize street networks as a static map or interactive Leaflet web map
+  * Explore street networks as a static map or interactive web map
   * Visualize travel distance and travel time with isoline and isochrone maps
   * Plot figure-ground diagrams of street networks and building footprints
 
 All of these features are demonstrated in the [examples](https://github.com/gboeing/osmnx-examples) repo and documented in the [documentation](https://osmnx.readthedocs.io/). Feature development details are in the [change log](CHANGELOG.md). Read the [journal article](https://geoffboeing.com/publications/osmnx-complex-street-networks/) for further technical details.
 
 ## License
 
 OSMnx is licensed under the MIT license. OpenStreetMap's open data [license](https://www.openstreetmap.org/copyright/) requires that derivative works provide proper attribution.
-
```

### Comparing `osmnx-1.3.1.post0/osmnx/_api.py` & `osmnx-1.4.0/osmnx/_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Expose most common parts of public API directly in `osmnx.` namespace."""
 
 from .bearing import add_edge_bearings
 from .bearing import orientation_entropy
-from .bearing import plot_orientation
 from .distance import k_shortest_paths
 from .distance import nearest_edges
 from .distance import nearest_nodes
 from .distance import shortest_path
 from .elevation import add_edge_grades
 from .elevation import add_node_elevations_google
 from .elevation import add_node_elevations_raster
@@ -32,14 +31,15 @@
 from .io import save_graphml
 from .osm_xml import save_graph_xml
 from .plot import plot_figure_ground
 from .plot import plot_footprints
 from .plot import plot_graph
 from .plot import plot_graph_route
 from .plot import plot_graph_routes
+from .plot import plot_orientation
 from .projection import project_gdf
 from .projection import project_graph
 from .simplification import consolidate_intersections
 from .simplification import simplify_graph
 from .speed import add_edge_speeds
 from .speed import add_edge_travel_times
 from .stats import basic_stats
```

### Comparing `osmnx-1.3.1.post0/osmnx/_polygon_features.py` & `osmnx-1.4.0/osmnx/_polygon_features.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1.post0/osmnx/bearing.py` & `osmnx-1.4.0/osmnx/bearing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """Calculate graph edge bearings."""
 
-import matplotlib.pyplot as plt
+from warnings import warn
+
 import networkx as nx
 import numpy as np
 
+from . import plot
 from . import projection
 
 # scipy is an optional dependency for entropy calculation
 try:
     import scipy
 except ImportError:  # pragma: no cover
     scipy = None
 
 
 def calculate_bearing(lat1, lng1, lat2, lng2):
     """
     Calculate the compass bearing(s) between pairs of lat-lng points.
 
-    Vectorized function to calculate (initial) bearings between two points'
+    Vectorized function to calculate initial bearings between two points'
     coordinates or between arrays of points' coordinates. Expects coordinates
-    in decimal degrees. Bearing represents angle in degrees (clockwise)
-    between north and the geodesic line from point 1 to point 2.
+    in decimal degrees. Bearing represents the clockwise angle in degrees
+    between north and the geodesic line from (lat1, lng1) to (lat2, lng2).
 
     Parameters
     ----------
     lat1 : float or numpy.array of float
         first point's latitude coordinate
     lng1 : float or numpy.array of float
         first point's longitude coordinate
@@ -48,15 +50,15 @@
     x = np.cos(lat1) * np.sin(lat2) - np.sin(lat1) * np.cos(lat2) * np.cos(d_lng)
     initial_bearing = np.degrees(np.arctan2(y, x))
 
     # normalize to 0-360 degrees to get compass bearing
     return initial_bearing % 360
 
 
-def add_edge_bearings(G, precision=1):
+def add_edge_bearings(G, precision=None):
     """
     Add compass `bearing` attributes to all graph edges.
 
     Vectorized function to calculate (initial) bearing from origin node to
     destination node for each edge in a directed, unprojected graph then add
     these bearings as new edge attributes. Bearing represents angle in degrees
     (clockwise) between north and the geodesic line from the origin node to
@@ -64,21 +66,29 @@
     undefined.
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
         unprojected graph
     precision : int
-        decimal precision to round bearing
+        deprecated, do not use
 
     Returns
     -------
     G : networkx.MultiDiGraph
         graph with edge bearing attributes
     """
+    if precision is None:
+        precision = 1
+    else:
+        warn(
+            "the `precision` parameter is deprecated and will be removed in a future release",
+            stacklevel=2,
+        )
+
     if projection.is_projected(G.graph["crs"]):  # pragma: no cover
         raise ValueError("graph must be unprojected to add edge bearings")
 
     # extract edge IDs and corresponding coordinates from their nodes
     uvk = [(u, v, k) for u, v, k in G.edges if u != v]
     x = G.nodes(data="x")
     y = G.nodes(data="y")
@@ -231,122 +241,72 @@
     alpha=0.7,
     title=None,
     title_y=1.05,
     title_font=None,
     xtick_font=None,
 ):
     """
-    Plot a polar histogram of a spatial network's bidirectional edge bearings.
+    Do not use: deprecated.
 
-    Ignores self-loop edges as their bearings are undefined.
-
-    For more info see: Boeing, G. 2019. "Urban Spatial Order: Street Network
-    Orientation, Configuration, and Entropy." Applied Network Science, 4 (1),
-    67. https://doi.org/10.1007/s41109-019-0189-1
+    The plot_orientation function moved to the plot module. Calling it via the
+    bearing module will raise an error in a future release.
 
     Parameters
     ----------
     Gu : networkx.MultiGraph
-        undirected, unprojected graph with `bearing` attributes on each edge
+        deprecated, do not use
     num_bins : int
-        number of bins; for example, if `num_bins=36` is provided, then each
-        bin will represent 10° around the compass
+        deprecated, do not use
     min_length : float
-        ignore edges with `length` attributes less than `min_length`
+        deprecated, do not use
     weight : string
-        if not None, weight edges' bearings by this (non-null) edge attribute
+        deprecated, do not use
     ax : matplotlib.axes.PolarAxesSubplot
-        if not None, plot on this preexisting axis; must have projection=polar
+        deprecated, do not use
     figsize : tuple
-        if ax is None, create new figure with size (width, height)
+        deprecated, do not use
     area : bool
-        if True, set bar length so area is proportional to frequency,
-        otherwise set bar length so height is proportional to frequency
+        deprecated, do not use
     color : string
-        color of histogram bars
+        deprecated, do not use
     edgecolor : string
-        color of histogram bar edges
+        deprecated, do not use
     linewidth : float
-        width of histogram bar edges
+        deprecated, do not use
     alpha : float
-        opacity of histogram bars
+        deprecated, do not use
     title : string
-        title for plot
+        deprecated, do not use
     title_y : float
-        y position to place title
+        deprecated, do not use
     title_font : dict
-        the title's fontdict to pass to matplotlib
+        deprecated, do not use
     xtick_font : dict
-        the xtick labels' fontdict to pass to matplotlib
+        deprecated, do not use
 
     Returns
     -------
     fig, ax : tuple
         matplotlib figure, axis
     """
-    if title_font is None:
-        title_font = {"family": "DejaVu Sans", "size": 24, "weight": "bold"}
-    if xtick_font is None:
-        xtick_font = {
-            "family": "DejaVu Sans",
-            "size": 10,
-            "weight": "bold",
-            "alpha": 1.0,
-            "zorder": 3,
-        }
-
-    # get the bearings' distribution's bin counts and edges
-    bin_counts, bin_edges = _bearings_distribution(Gu, num_bins, min_length, weight)
-
-    # positions: where to center each bar. ignore the last bin edge, because
-    # it's the same as the first (i.e., 0° = 360°)
-    positions = np.radians(bin_edges[:-1])
-
-    # width: make bars fill the circumference without gaps or overlaps
-    width = 2 * np.pi / num_bins
-
-    # radius: how long to make each bar
-    bin_frequency = bin_counts / bin_counts.sum()
-    if area:
-        # set bar length so area is proportional to frequency
-        radius = np.sqrt(bin_frequency)
-    else:
-        # set bar length so height is proportional to frequency
-        radius = bin_frequency
-
-    # create ax (if necessary) then set N at top and go clockwise
-    if ax is None:
-        fig, ax = plt.subplots(figsize=figsize, subplot_kw={"projection": "polar"})
-    else:
-        fig = ax.figure
-    ax.set_theta_zero_location("N")
-    ax.set_theta_direction("clockwise")
-    ax.set_ylim(top=radius.max())
-
-    # configure the y-ticks and remove their labels
-    ax.set_yticks(np.linspace(0, radius.max(), 5))
-    ax.set_yticklabels(labels="")
-
-    # configure the x-ticks and their labels
-    xticklabels = ["N", "", "E", "", "S", "", "W", ""]
-    ax.set_xticks(ax.get_xticks())
-    ax.set_xticklabels(labels=xticklabels, fontdict=xtick_font)
-    ax.tick_params(axis="x", which="major", pad=-2)
-
-    # draw the bars
-    ax.bar(
-        positions,
-        height=radius,
-        width=width,
-        align="center",
-        bottom=0,
-        zorder=2,
+    warn(
+        "The `plot_orientation` function moved to the `plot` module. Calling it "
+        "via the `bearing` module will cause an exception in a future release.",
+        stacklevel=2,
+    )
+    return plot.plot_orientation(
+        Gu,
+        num_bins=num_bins,
+        min_length=min_length,
+        weight=weight,
+        ax=ax,
+        figsize=figsize,
+        area=area,
         color=color,
         edgecolor=edgecolor,
         linewidth=linewidth,
         alpha=alpha,
+        title=title,
+        title_y=title_y,
+        title_font=title_font,
+        xtick_font=xtick_font,
     )
-
-    if title:
-        ax.set_title(title, y=title_y, fontdict=title_font)
-    fig.tight_layout()
-    return fig, ax
```

### Comparing `osmnx-1.3.1.post0/osmnx/distance.py` & `osmnx-1.4.0/osmnx/distance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Calculate distances and shortest paths and find nearest node/edge(s) to point(s)."""
 
 import itertools
 import multiprocessing as mp
+from warnings import warn
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 from shapely.geometry import Point
 from shapely.strtree import STRtree
 
@@ -97,15 +98,15 @@
     dist : float or numpy.array of float
         distance from each (x1, y1) to each (x2, y2) in coordinates' units
     """
     # pythagorean theorem
     return ((x1 - x2) ** 2 + (y1 - y2) ** 2) ** 0.5
 
 
-def add_edge_lengths(G, precision=3, edges=None):
+def add_edge_lengths(G, precision=None, edges=None):
     """
     Add `length` attribute (in meters) to each edge.
 
     Vectorized function to calculate great-circle distance between each edge's
     incident nodes. Ensure graph is in unprojected coordinates, and
     unsimplified to get accurate distances.
 
@@ -122,24 +123,32 @@
     (such as is the case with an unsimplified graph).
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
         unprojected, unsimplified input graph
     precision : int
-        decimal precision to round lengths
+        deprecated, do not use
     edges : tuple
         tuple of (u, v, k) tuples representing subset of edges to add length
         attributes to. if None, add lengths to all edges.
 
     Returns
     -------
     G : networkx.MultiDiGraph
         graph with edge length attributes
     """
+    if precision is None:
+        precision = 3
+    else:
+        warn(
+            "the `precision` parameter is deprecated and will be removed in a future release",
+            stacklevel=2,
+        )
+
     if edges is None:
         uvk = tuple(G.edges)
     else:
         uvk = edges
 
     # extract edge IDs and corresponding coordinates from their nodes
     x = G.nodes(data="x")
@@ -405,44 +414,47 @@
 
     Returns
     -------
     path : list
         list of node IDs constituting the shortest path, or, if orig and dest
         are lists, then a list of path lists
     """
+    _verify_edge_attribute(G, weight)
+
+    # if neither orig nor dest is iterable, just return the shortest path
     if not (hasattr(orig, "__iter__") or hasattr(dest, "__iter__")):
-        # if neither orig nor dest is iterable, just return the shortest path
         return _single_shortest_path(G, orig, dest, weight)
 
+    # if both orig and dest are iterables, ensure they have same lengths
     elif hasattr(orig, "__iter__") and hasattr(dest, "__iter__"):
-        # if both orig and dest are iterables ensure they have same lengths
         if len(orig) != len(dest):  # pragma: no cover
             raise ValueError("orig and dest must contain same number of elements")
 
         if cpus is None:
             cpus = mp.cpu_count()
         cpus = min(cpus, mp.cpu_count())
         utils.log(f"Solving {len(orig)} paths with {cpus} CPUs...")
 
+        # if single-threading, calculate each shortest path one at a time
         if cpus == 1:
-            # if single-threading, calculate each shortest path one at a time
             paths = [_single_shortest_path(G, o, d, weight) for o, d in zip(orig, dest)]
+
+        # if multi-threading, calculate shortest paths in parallel
         else:
-            # if multi-threading, calculate shortest paths in parallel
             args = ((G, o, d, weight) for o, d in zip(orig, dest))
             pool = mp.Pool(cpus)
             sma = pool.starmap_async(_single_shortest_path, args)
             paths = sma.get()
             pool.close()
             pool.join()
 
         return paths
 
+    # if only one of orig or dest is iterable and the other is not
     else:  # pragma: no cover
-        # if only one of orig or dest is iterable and the other is not
         raise ValueError("orig and dest must either both be iterable or neither must be iterable")
 
 
 def k_shortest_paths(G, orig, dest, k, weight="length"):
     """
     Solve `k` shortest paths from an origin node to a destination node.
 
@@ -465,10 +477,38 @@
 
     Returns
     -------
     paths : generator
         a generator of `k` shortest paths ordered by total weight. each path
         is a list of node IDs.
     """
+    _verify_edge_attribute(G, weight)
     paths_gen = nx.shortest_simple_paths(utils_graph.get_digraph(G, weight), orig, dest, weight)
     for path in itertools.islice(paths_gen, 0, k):
         yield path
+
+
+def _verify_edge_attribute(G, attr):
+    """
+    Verify attribute values are numeric and non-null across graph edges.
+
+    Raises a `ValueError` if attribute contains non-numeric values and raises
+    a warning if attribute is missing or null on any edges.
+
+    Parameters
+    ----------
+    G : networkx.MultiDiGraph
+        input graph
+    attr : string
+        edge attribute to verify
+
+    Returns
+    -------
+    None
+    """
+    try:
+        values = np.array(tuple(G.edges(data=attr)))[:, 2]
+        values_float = values.astype(float)
+        if np.isnan(values_float).any():
+            warn(f"The attribute {attr!r} is missing or null on some edges.", stacklevel=2)
+    except ValueError:
+        raise ValueError(f"The edge attribute {attr!r} contains non-numeric values.")
```

### Comparing `osmnx-1.3.1.post0/osmnx/downloader.py` & `osmnx-1.4.0/osmnx/downloader.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1.post0/osmnx/elevation.py` & `osmnx-1.4.0/osmnx/elevation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Get node elevations and calculate edge grades."""
 
 import multiprocessing as mp
 import time
 from hashlib import sha1
 from pathlib import Path
+from warnings import warn
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 import requests
 
 from . import downloader
@@ -109,15 +110,15 @@
 
 
 def add_node_elevations_google(
     G,
     api_key,
     max_locations_per_batch=350,
     pause_duration=0,
-    precision=3,
+    precision=None,
     url_template="https://maps.googleapis.com/maps/api/elevation/json?locations={}&key={}",
 ):  # pragma: no cover
     """
     Add `elevation` (meters) attribute to each node using a web service.
 
     By default, this uses the Google Maps Elevation API but you can optionally
     use an equivalent API with the same interface and response format, such as
@@ -137,25 +138,33 @@
         max number of coordinate pairs to submit in each API call (if this is
         too high, the server will reject the request because its character
         limit exceeds the max allowed)
     pause_duration : float
         time to pause between API calls, which can be increased if you get
         rate limited
     precision : int
-        decimal precision to round elevation values
+        deprecated, do not use
     url_template : string
         a URL string template for the API endpoint, containing exactly two
         parameters: `locations` and `key`; for example, for Open Topo Data:
-        "https://api.opentopodata.org/v1/aster30m?locations={}&key={}"
+        `"https://api.opentopodata.org/v1/aster30m?locations={}&key={}"`
 
     Returns
     -------
     G : networkx.MultiDiGraph
         graph with node elevation attributes
     """
+    if precision is None:
+        precision = 3
+    else:
+        warn(
+            "the `precision` parameter is deprecated and will be removed in a future release",
+            stacklevel=2,
+        )
+
     # make a pandas series of all the nodes' coordinates as 'lat,lng'
     # round coordinates to 5 decimal places (approx 1 meter) to be able to fit
     # in more locations per API call
     node_points = pd.Series(
         {node: f'{data["y"]:.5f},{data["x"]:.5f}' for node, data in G.nodes(data=True)}
     )
     n_calls = int(np.ceil(len(node_points) / max_locations_per_batch))
@@ -203,15 +212,15 @@
     df["elevation"] = df["elevation"].round(precision)
     nx.set_node_attributes(G, name="elevation", values=df["elevation"].to_dict())
     utils.log("Added elevation data from API to all nodes.")
 
     return G
 
 
-def add_edge_grades(G, add_absolute=True, precision=3):
+def add_edge_grades(G, add_absolute=True, precision=None):
     """
     Add `grade` attribute to each graph edge.
 
     Vectorized function to calculate the directed grade (ie, rise over run)
     for each edge in the graph and add it to the edge as an attribute. Nodes
     must already have `elevation` attributes to use this function.
 
@@ -221,21 +230,29 @@
     Parameters
     ----------
     G : networkx.MultiDiGraph
         input graph with `elevation` node attribute
     add_absolute : bool
         if True, also add absolute value of grade as `grade_abs` attribute
     precision : int
-        decimal precision to round grade values
+        deprecated, do not use
 
     Returns
     -------
     G : networkx.MultiDiGraph
         graph with edge `grade` (and optionally `grade_abs`) attributes
     """
+    if precision is None:
+        precision = 3
+    else:
+        warn(
+            "the `precision` parameter is deprecated and will be removed in a future release",
+            stacklevel=2,
+        )
+
     elev_lookup = G.nodes(data="elevation")
     u, v, k, lengths = zip(*G.edges(keys=True, data="length"))
     uvk = tuple(zip(u, v, k))
 
     # calculate edges' elevation changes from u to v then divide by lengths
     elevs = np.array([(elev_lookup[u], elev_lookup[v]) for u, v, k in uvk])
     grades = ((elevs[:, 1] - elevs[:, 0]) / np.array(lengths)).round(precision)
```

### Comparing `osmnx-1.3.1.post0/osmnx/folium.py` & `osmnx-1.4.0/osmnx/folium.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,18 @@
-"""Create interactive Leaflet web maps of graphs and routes via folium."""
+"""Create interactive Leaflet web maps of graphs and routes via folium.
+
+This module is deprecated. Do not use. It will be removed in a future release.
+You can generate and explore interactive web maps of graph nodes, edges,
+and/or routes automatically using GeoPandas.GeoDataFrame.explore instead, for
+example like: `ox.graph_to_gdfs(G, nodes=False).explore()`. See the OSMnx
+usage example repo for complete details and demonstrations.
+"""
 
 import json
+from warnings import warn
 
 from . import utils_graph
 
 # folium is an optional dependency for the folium plotting functions
 try:
     import folium
 except ImportError:  # pragma: no cover
@@ -17,41 +25,50 @@
     popup_attribute=None,
     tiles="cartodbpositron",
     zoom=1,
     fit_bounds=True,
     **kwargs,
 ):
     """
-    Plot a graph as an interactive Leaflet web map.
+    Do not use: deprecated.
 
-    Note that anything larger than a small city can produce a large web map
-    file that is slow to render in your browser.
+    You can generate and explore interactive web maps of graph nodes, edges,
+    and/or routes automatically using GeoPandas.GeoDataFrame.explore instead,
+    for example like: `ox.graph_to_gdfs(G, nodes=False).explore()`. See the
+    OSMnx usage example repo for complete details and demonstrations.
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
-        input graph
+        deprecated
     graph_map : folium.folium.Map
-        if not None, plot the graph on this preexisting folium map object
+        deprecated
     popup_attribute : string
-        edge attribute to display in a pop-up when an edge is clicked
+        deprecated
     tiles : string
-        name of a folium tileset
+        deprecated
     zoom : int
-        initial zoom level for the map
+        deprecated
     fit_bounds : bool
-        if True, fit the map to the boundaries of the graph's edges
+        deprecated
     kwargs
-        keyword arguments to pass to folium.PolyLine(), see folium docs for
-        options (for example `color="#333333", weight=5, opacity=0.7`)
+        deprecated
 
     Returns
     -------
     folium.folium.Map
     """
+    warn(
+        "The `folium` module has been deprecated and will be removed in a future release. "
+        "You can generate and explore interactive web maps of graph nodes, edges, "
+        "and/or routes automatically using GeoPandas.GeoDataFrame.explore instead, "
+        "for example like: `ox.graph_to_gdfs(G, nodes=False).explore()`. See the "
+        "OSMnx usage example repo for complete details and demonstrations.",
+        stacklevel=2,
+    )
     # create gdf of all graph edges
     gdf_edges = utils_graph.graph_to_gdfs(G, nodes=False)
     return _plot_folium(gdf_edges, graph_map, popup_attribute, tiles, zoom, fit_bounds, **kwargs)
 
 
 def plot_route_folium(
     G,
@@ -60,40 +77,52 @@
     popup_attribute=None,
     tiles="cartodbpositron",
     zoom=1,
     fit_bounds=True,
     **kwargs,
 ):
     """
-    Plot a route as an interactive Leaflet web map.
+    Do not use: deprecated.
+
+    You can generate and explore interactive web maps of graph nodes, edges,
+    and/or routes automatically using GeoPandas.GeoDataFrame.explore instead,
+    for example like: `ox.graph_to_gdfs(G, nodes=False).explore()`. See the
+    OSMnx usage example repo for complete details and demonstrations.
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
-        input graph
+        deprecated
     route : list
-        the route as a list of nodes
+        deprecated
     route_map : folium.folium.Map
-        if not None, plot the route on this preexisting folium map object
+        deprecated
     popup_attribute : string
-        edge attribute to display in a pop-up when an edge is clicked
+        deprecated
     tiles : string
-        name of a folium tileset
+        deprecated
     zoom : int
-        initial zoom level for the map
+        deprecated
     fit_bounds : bool
-        if True, fit the map to the boundaries of the route's edges
+        deprecated
     kwargs
-        keyword arguments to pass to folium.PolyLine(), see folium docs for
-        options (for example `color="#cc0000", weight=5, opacity=0.7`)
+        deprecated
 
     Returns
     -------
     folium.folium.Map
     """
+    warn(
+        "The `folium` module has been deprecated and will be removed in a future release. "
+        "You can generate and explore interactive web maps of graph nodes, edges, "
+        "and/or routes automatically using GeoPandas.GeoDataFrame.explore instead, "
+        "for example like: `ox.graph_to_gdfs(G, nodes=False).explore()`. See the "
+        "OSMnx usage example repo for complete details and demonstrations.",
+        stacklevel=2,
+    )
     # create gdf of the route edges in order
     node_pairs = zip(route[:-1], route[1:])
     uvk = ((u, v, min(G[u][v].items(), key=lambda k: k[1]["length"])[0]) for u, v in node_pairs)
     gdf_edges = utils_graph.graph_to_gdfs(G.subgraph(route), nodes=False).loc[uvk]
     return _plot_folium(gdf_edges, route_map, popup_attribute, tiles, zoom, fit_bounds, **kwargs)
```

### Comparing `osmnx-1.3.1.post0/osmnx/geocoder.py` & `osmnx-1.4.0/osmnx/geocoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from . import projection
 from . import settings
 from . import utils
 
 
 def geocode(query):
     """
-    Geocode a query string to (lat, lng) with the Nominatim geocoder.
+    Geocode a query string to (lat, lng) with the Nominatim API.
 
     Parameters
     ----------
     query : string
         the query string to geocode
 
     Returns
```

### Comparing `osmnx-1.3.1.post0/osmnx/geometries.py` & `osmnx-1.4.0/osmnx/geometries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Download geospatial entities' geometries and attributes from OpenStreetMap.
 
-Retrieve points of interest, building footprints, or any other objects from
-OSM, including their geometries and attribute data, and construct a
-GeoDataFrame of them. You can use this module to query for nodes, ways, and
-relations (the latter of type "multipolygon" or "boundary" only) by passing a
-dictionary of desired tags/values.
+Retrieve points of interest, building footprints, transit lines/stops, or any
+other objects from OSM, including their geometries and attribute data, and
+construct a GeoDataFrame of them. You can use this module to query for nodes,
+ways, and relations (the latter of type "multipolygon" or "boundary" only) by
+passing a dictionary of desired tags/values.
 """
 
 import logging as lg
 import warnings
 
 import geopandas as gpd
 import numpy as np
@@ -25,14 +25,15 @@
 
 from . import downloader
 from . import geocoder
 from . import osm_xml
 from . import settings
 from . import utils
 from . import utils_geo
+from ._errors import EmptyOverpassResponse
 from ._polygon_features import _polygon_features
 
 
 def geometries_from_bbox(north, south, east, west, tags):
     """
     Create a GeoDataFrame of OSM entities within a N, S, E, W bounding box.
 
@@ -348,124 +349,115 @@
     Returns
     -------
     gdf : geopandas.GeoDataFrame
         GeoDataFrame of geometries and their associated tags
     """
     elements_count = sum(len(rj["elements"]) for rj in response_jsons)
 
-    # if there are no elements in the responses
+    # make sure we got data back from the server request(s)
     if elements_count == 0:
-        # create an empty GeoDataFrame
-        gdf = gpd.GeoDataFrame()
+        msg = (
+            "There are no data elements in the server response. Check log and query location/tags."
+        )
+        raise EmptyOverpassResponse(msg)
+
+    # begin processing the elements retrieved from the server
+    utils.log(f"Converting {elements_count} elements in JSON responses to geometries")
+
+    # Dictionaries to hold nodes and complete geometries
+    coords = {}
+    geometries = {}
+
+    # Set to hold the unique IDs of elements that do not have tags
+    untagged_element_ids = set()
+
+    # identify which relation types to parse to (multi)polygons
+    relation_types = {"boundary", "multipolygon"}
+
+    # extract geometries from the downloaded osm data
+    for response_json in response_jsons:
+        # Parses the JSON of OSM nodes, ways and (multipolygon) relations
+        # to dictionaries of coordinates, Shapely Points, LineStrings,
+        # Polygons and MultiPolygons
+        for element in response_json["elements"]:
+            # id numbers are only unique within element types
+            # create unique id from combination of type and id
+            unique_id = f"{element['type']}/{element['id']}"
+
+            # add elements that are not nodes and that are without tags or
+            # with empty tags to the untagged_element_ids set (untagged
+            # nodes are not added to the geometries dict at all)
+            if (element["type"] != "node") and (("tags" not in element) or (not element["tags"])):
+                untagged_element_ids.add(unique_id)
+
+            if element["type"] == "node":
+                # Parse all nodes to coords
+                coords[element["id"]] = _parse_node_to_coords(element=element)
+
+                # If the node has tags and the tags are not empty parse it
+                # to a Point. Empty check is necessary for JSONs created
+                # from XML where nodes without tags are assigned tags={}
+                if "tags" in element and len(element["tags"]) > 0:
+                    point = _parse_node_to_point(element=element)
+                    geometries[unique_id] = point
+
+            elif element["type"] == "way":
+                # Parse all ways to linestrings or polygons
+                linestring_or_polygon = _parse_way_to_linestring_or_polygon(
+                    element=element, coords=coords
+                )
+                geometries[unique_id] = linestring_or_polygon
+
+            elif (
+                element["type"] == "relation" and element.get("tags").get("type") in relation_types
+            ):
+                # parse relations to (multi)polygons
+                multipolygon = _parse_relation_to_multipolygon(
+                    element=element, geometries=geometries
+                )
+                geometries[unique_id] = multipolygon
+
+    utils.log(f"{len(geometries)} geometries created in the dict")
+
+    # remove untagged elements from the final dict of geometries
+    for untagged_element_id in untagged_element_ids:
+        geometries.pop(untagged_element_id, None)
+
+    utils.log(f"{len(untagged_element_ids)} untagged geometries removed")
+
+    # Create GeoDataFrame
+    gdf = gpd.GeoDataFrame.from_dict(geometries, orient="index")
+
+    # ensure gdf has a geometry col before assigning crs
+    if "geometry" not in gdf.columns:
+        # if there is no geometry column, create a null column
         gdf["geometry"] = np.nan
-        gdf.set_geometry("geometry")
-        gdf.crs = settings.default_crs
+    gdf.set_geometry("geometry")
 
-        # log a warning
-        utils.log("No data elements: check query tags and location.", level=lg.WARNING)
-        return gdf
-
-    # else if there were elements in the response
-    else:
-        utils.log(f"Converting {elements_count} elements in JSON responses to geometries")
-
-        # Dictionaries to hold nodes and complete geometries
-        coords = {}
-        geometries = {}
-
-        # Set to hold the unique IDs of elements that do not have tags
-        untagged_element_ids = set()
-
-        # identify which relation types to parse to (multi)polygons
-        relation_types = {"boundary", "multipolygon"}
-
-        # extract geometries from the downloaded osm data
-        for response_json in response_jsons:
-            # Parses the JSON of OSM nodes, ways and (multipolygon) relations
-            # to dictionaries of coordinates, Shapely Points, LineStrings,
-            # Polygons and MultiPolygons
-            for element in response_json["elements"]:
-                # id numbers are only unique within element types
-                # create unique id from combination of type and id
-                unique_id = f"{element['type']}/{element['id']}"
-
-                # add elements that are not nodes and that are without tags or
-                # with empty tags to the untagged_element_ids set (untagged
-                # nodes are not added to the geometries dict at all)
-                if (element["type"] != "node") and (
-                    ("tags" not in element) or (not element["tags"])
-                ):
-                    untagged_element_ids.add(unique_id)
-
-                if element["type"] == "node":
-                    # Parse all nodes to coords
-                    coords[element["id"]] = _parse_node_to_coords(element=element)
-
-                    # If the node has tags and the tags are not empty parse it
-                    # to a Point. Empty check is necessary for JSONs created
-                    # from XML where nodes without tags are assigned tags={}
-                    if "tags" in element and len(element["tags"]) > 0:
-                        point = _parse_node_to_point(element=element)
-                        geometries[unique_id] = point
-
-                elif element["type"] == "way":
-                    # Parse all ways to linestrings or polygons
-                    linestring_or_polygon = _parse_way_to_linestring_or_polygon(
-                        element=element, coords=coords
-                    )
-                    geometries[unique_id] = linestring_or_polygon
-
-                elif (
-                    element["type"] == "relation"
-                    and element.get("tags").get("type") in relation_types
-                ):
-                    # parse relations to (multi)polygons
-                    multipolygon = _parse_relation_to_multipolygon(
-                        element=element, geometries=geometries
-                    )
-                    geometries[unique_id] = multipolygon
-
-        utils.log(f"{len(geometries)} geometries created in the dict")
-
-        # remove untagged elements from the final dict of geometries
-        for untagged_element_id in untagged_element_ids:
-            geometries.pop(untagged_element_id, None)
-
-        utils.log(f"{len(untagged_element_ids)} untagged geometries removed")
-
-        # Create GeoDataFrame
-        gdf = gpd.GeoDataFrame.from_dict(geometries, orient="index")
-
-        # ensure gdf has a geometry col before assigning crs
-        if "geometry" not in gdf.columns:
-            # if there is no geometry column, create a null column
-            gdf["geometry"] = np.nan
-        gdf.set_geometry("geometry")
-
-        # Set default crs
-        gdf.crs = settings.default_crs
-
-        # Apply .buffer(0) to any invalid geometries
-        gdf = _buffer_invalid_geometries(gdf)
-
-        # Filter final gdf to requested tags and query polygon
-        gdf = _filter_gdf_by_polygon_and_tags(gdf, polygon=polygon, tags=tags)
-
-        # bug in geopandas <0.9 raises a TypeError if trying to plot empty
-        # geometries but missing geometries (gdf['geometry'] = None) cannot be
-        # projected e.g. gdf.to_crs(). Remove rows with empty (e.g. Point())
-        # or missing (e.g. None) geometry, and suppress gpd warning caused by
-        # calling gdf["geometry"].isna() on GeoDataFrame with empty geometries
-        if not gdf.empty:
-            warnings.filterwarnings("ignore", "GeoSeries.isna", UserWarning)
-            gdf = gdf[~(gdf["geometry"].is_empty | gdf["geometry"].isna())].copy()
-            warnings.resetwarnings()
+    # Set default crs
+    gdf.crs = settings.default_crs
 
-        utils.log(f"{len(gdf)} geometries in the final GeoDataFrame")
-        return gdf
+    # Apply .buffer(0) to any invalid geometries
+    gdf = _buffer_invalid_geometries(gdf)
+
+    # Filter final gdf to requested tags and query polygon
+    gdf = _filter_gdf_by_polygon_and_tags(gdf, polygon=polygon, tags=tags)
+
+    # bug in geopandas <0.9 raises a TypeError if trying to plot empty
+    # geometries but missing geometries (gdf['geometry'] = None) cannot be
+    # projected e.g. gdf.to_crs(). Remove rows with empty (e.g. Point())
+    # or missing (e.g. None) geometry, and suppress gpd warning caused by
+    # calling gdf["geometry"].isna() on GeoDataFrame with empty geometries
+    if not gdf.empty:
+        warnings.filterwarnings("ignore", "GeoSeries.isna", UserWarning)
+        gdf = gdf[~(gdf["geometry"].is_empty | gdf["geometry"].isna())].copy()
+        warnings.resetwarnings()
+
+    utils.log(f"{len(gdf)} geometries in the final GeoDataFrame")
+    return gdf
 
 
 def _parse_node_to_coords(element):
     """
     Parse coordinates from a node in the overpass response.
 
     The coords are only used to create LineStrings and Polygons.
@@ -680,15 +672,15 @@
 
 
 def _parse_relation_to_multipolygon(element, geometries):
     """
     Parse multipolygon from OSM relation (type:MultiPolygon).
 
     See more information about relations from OSM documentation:
-    http://wiki.openstreetmap.org/wiki/Relation
+    https://wiki.openstreetmap.org/wiki/Relation
 
     Parameters
     ----------
     element : dict
         element type "relation" from overpass response JSON
     geometries : dict
         dict containing all linestrings and polygons generated from OSM ways
```

### Comparing `osmnx-1.3.1.post0/osmnx/graph.py` & `osmnx-1.4.0/osmnx/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Graph creation functions."""
 
 import itertools
-import warnings
+from warnings import warn
 
 import networkx as nx
 from shapely.geometry import MultiPolygon
 from shapely.geometry import Polygon
 
 from . import distance
 from . import downloader
@@ -477,19 +477,19 @@
             G = simplification.simplify_graph(G)
 
         # count how many physical streets connect to each intersection/deadend
         # note this will be somewhat inaccurate due to periphery effects, so
         # it's best to parameterize function with clean_periphery=True
         spn = stats.count_streets_per_node(G)
         nx.set_node_attributes(G, values=spn, name="street_count")
-        msg = (
+        warn(
             "the graph-level street_count attribute will likely be inaccurate "
-            "when you set clean_periphery=False"
+            "when you set clean_periphery=False",
+            stacklevel=2,
         )
-        warnings.warn(msg, stacklevel=1)
 
     utils.log(f"graph_from_polygon returned graph with {len(G)} nodes and {len(G.edges)} edges")
     return G
 
 
 def graph_from_xml(filepath, bidirectional=False, simplify=True, retain_all=False):
     """
@@ -547,15 +547,16 @@
     -------
     G : networkx.MultiDiGraph
     """
     utils.log("Creating graph from downloaded OSM data...")
 
     # make sure we got data back from the server request(s)
     if not any(rj["elements"] for rj in response_jsons):  # pragma: no cover
-        raise EmptyOverpassResponse("There are no data elements in the response JSON")
+        msg = "There are no data elements in the server response. Check log and query location/filters."
+        raise EmptyOverpassResponse(msg)
 
     # create the graph as a MultiDiGraph and set its meta-attributes
     metadata = {
         "created_date": utils.ts(),
         "created_with": f"OSMnx {__version__}",
         "crs": settings.default_crs,
     }
@@ -663,15 +664,15 @@
 def _is_path_one_way(path, bidirectional, oneway_values):
     """
     Determine if a path of nodes allows travel in only one direction.
 
     Parameters
     ----------
     path : dict
-        a path's tag:value attribute data
+        a path's `tag:value` attribute data
     bidirectional : bool
         whether this is a bi-directional network type
     oneway_values : set
         the values OSM uses in its 'oneway' tag to denote True
 
     Returns
     -------
@@ -711,15 +712,15 @@
 def _is_path_reversed(path, reversed_values):
     """
     Determine if the order of nodes in a path should be reversed.
 
     Parameters
     ----------
     path : dict
-        a path's tag:value attribute data
+        a path's `tag:value` attribute data
     reversed_values : set
         the values OSM uses in its 'oneway' tag to denote travel can only
         occur in the opposite direction of the node order
 
     Returns
     -------
     bool
@@ -735,15 +736,15 @@
     Add a list of paths to the graph as edges.
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
         graph to add paths to
     paths : list
-        list of paths' tag:value attribute data dicts
+        list of paths' `tag:value` attribute data dicts
     bidirectional : bool
         if True, create bi-directional edges for one-way streets
 
     Returns
     -------
     None
     """
```

### Comparing `osmnx-1.3.1.post0/osmnx/io.py` & `osmnx-1.4.0/osmnx/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Serialize graphs to/from files on disk."""
 
 import ast
-import warnings
 from pathlib import Path
+from warnings import warn
 
 import networkx as nx
 import pandas as pd
 from shapely import wkt
 
 from . import settings
 from . import utils
@@ -80,19 +80,19 @@
         retain original oneway and to/from information as edge attributes; if
         True, save one edge for each directed edge in the graph
 
     Returns
     -------
     None
     """
-    warnings.warn(
+    warn(
         "The `save_graph_shapefile` function is deprecated and will be removed "
         "in a future release. Instead, use the `save_graph_geopackage` function "
         "to save graphs as GeoPackage files for subsequent GIS analysis.",
-        stacklevel=1,
+        stacklevel=2,
     )
 
     # default filepath if none was provided
     if filepath is None:
         filepath = Path(settings.data_folder) / "graph_shapefile"
     else:
         filepath = Path(filepath)
```

### Comparing `osmnx-1.3.1.post0/osmnx/osm_xml.py` & `osmnx-1.4.0/osmnx/osm_xml.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Read/write .osm formatted XML files."""
-
 import bz2
 import xml.sax
 from pathlib import Path
+from warnings import warn
 from xml.etree import ElementTree as etree
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 
 from . import settings
@@ -15,17 +15,16 @@
 
 
 class _OSMContentHandler(xml.sax.handler.ContentHandler):
     """
     SAX content handler for OSM XML.
 
     Used to build an Overpass-like response JSON object in self.object. For
-    format notes, see
-    http://wiki.openstreetmap.org/wiki/OSM_XML#OSM_XML_file_format_notes and
-    http://overpass-api.de/output_formats.html#json
+    format notes, see https://overpass-api.de/ and
+    https://wiki.openstreetmap.org/wiki/OSM_XML#OSM_XML_file_format_notes
     """
 
     def __init__(self):
         self._element = None
         self.object = {"elements": []}
 
     def startElement(self, name, attrs):
@@ -180,21 +179,19 @@
     else:
         filepath = Path(filepath)
 
     # if save folder does not already exist, create it
     filepath.parent.mkdir(parents=True, exist_ok=True)
 
     if not settings.all_oneway:  # pragma: no cover
-        import warnings
-
-        msg = (
+        warn(
             "In order for save_graph_xml to behave properly the graph must "
-            "have been created with the `all_oneway` setting set to True."
+            "have been created with the `all_oneway` setting set to True.",
+            stacklevel=2,
         )
-        warnings.warn(msg, stacklevel=1)
 
     try:
         gdf_nodes, gdf_edges = data
     except ValueError:
         gdf_nodes, gdf_edges = utils_graph.graph_to_gdfs(
             data, node_geometry=False, fill_edge_geometry=False
         )
```

### Comparing `osmnx-1.3.1.post0/osmnx/plot.py` & `osmnx-1.4.0/osmnx/plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-"""Plot spatial geometries, street networks, and routes."""
+"""Visualize spatial footprints, street networks, routes, and orientations."""
 
 from pathlib import Path
 
-import matplotlib.cm as cm
-import matplotlib.colors as colors
-import matplotlib.pyplot as plt
 import networkx as nx
 import numpy as np
 import pandas as pd
-from matplotlib import colormaps
 
+from . import bearing
 from . import graph
 from . import projection
 from . import settings
 from . import simplification
 from . import utils
 from . import utils_geo
 from . import utils_graph
 
+# matplotlib is an optional dependency needed for visualization
+try:
+    import matplotlib.cm as cm
+    import matplotlib.colors as colors
+    import matplotlib.pyplot as plt
+    from matplotlib import colormaps
+except ImportError:  # pragma: no cover
+    cm = colors = plt = colormaps = None
+
 
 def get_colors(n, cmap="viridis", start=0.0, stop=1.0, alpha=1.0, return_hex=False):
     """
     Get `n` evenly-spaced colors from a matplotlib colormap.
 
     Parameters
     ----------
@@ -39,14 +45,15 @@
         if True, convert RGBa colors to HTML-like hexadecimal RGB strings. if
         False, return colors as (R, G, B, alpha) tuples.
 
     Returns
     -------
     color_list : list
     """
+    _verify_mpl()
     color_list = [colormaps[cmap](x) for x in np.linspace(start, stop, n)]
     if return_hex:
         color_list = [colors.to_hex(c) for c in color_list]
     else:
         color_list = [(r, g, b, alpha) for r, g, b, _ in color_list]
     return color_list
 
@@ -79,14 +86,15 @@
         (requires unique bin edges). if False, bin into equal-spaced bins.
 
     Returns
     -------
     node_colors : pandas.Series
         series labels are node IDs and values are colors
     """
+    _verify_mpl()
     vals = pd.Series(nx.get_node_attributes(G, attr))
     return _get_colors_by_value(vals, num_bins, cmap, start, stop, na_color, equal_size)
 
 
 def get_edge_colors_by_attr(
     G, attr, num_bins=None, cmap="viridis", start=0, stop=1, na_color="none", equal_size=False
 ):
@@ -115,14 +123,15 @@
         (requires unique bin edges). if False, bin into equal-spaced bins.
 
     Returns
     -------
     edge_colors : pandas.Series
         series labels are edge IDs (u, v, key) and values are colors
     """
+    _verify_mpl()
     vals = pd.Series(nx.get_edge_attributes(G, attr))
     return _get_colors_by_value(vals, num_bins, cmap, start, stop, na_color, equal_size)
 
 
 def plot_graph(
     G,
     ax=None,
@@ -140,15 +149,15 @@
     close=False,
     save=False,
     filepath=None,
     dpi=300,
     bbox=None,
 ):
     """
-    Plot a graph.
+    Visualize a graph.
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
         input graph
     ax : matplotlib axis
         if not None, plot on this preexisting axis
@@ -191,14 +200,15 @@
         from spatial extents of plotted geometries.
 
     Returns
     -------
     fig, ax : tuple
         matplotlib figure, axis
     """
+    _verify_mpl()
     max_node_size = max(node_size) if hasattr(node_size, "__iter__") else node_size
     max_edge_lw = max(edge_linewidth) if hasattr(edge_linewidth, "__iter__") else edge_linewidth
     if max_node_size <= 0 and max_edge_lw <= 0:  # pragma: no cover
         raise ValueError("Either node_size or edge_linewidth must be > 0 to plot something.")
 
     # create fig, ax as needed
     utils.log("Begin plotting the graph...")
@@ -251,15 +261,15 @@
     route_linewidth=4,
     route_alpha=0.5,
     orig_dest_size=100,
     ax=None,
     **pg_kwargs,
 ):
     """
-    Plot a route along a graph.
+    Visualize a route along a graph.
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
         input graph
     route : list
         route as a list of node IDs
@@ -278,14 +288,15 @@
         keyword arguments to pass to plot_graph
 
     Returns
     -------
     fig, ax : tuple
         matplotlib figure, axis
     """
+    _verify_mpl()
     if ax is None:
         # plot the graph but not the route, and override any user show/close
         # args for now: we'll do that later
         override = {"show", "save", "close"}
         kwargs = {k: v for k, v in pg_kwargs.items() if k not in override}
         fig, ax = plot_graph(G, show=False, save=False, close=False, **kwargs)
     else:
@@ -318,15 +329,15 @@
     kwargs = {k: v for k, v in pg_kwargs.items() if k in sas_kwargs}
     fig, ax = _save_and_show(fig, ax, **kwargs)
     return fig, ax
 
 
 def plot_graph_routes(G, routes, route_colors="r", route_linewidths=4, **pgr_kwargs):
     """
-    Plot several routes along a graph.
+    Visualize several routes along a graph.
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
         input graph
     routes : list
         routes as a list of lists of node IDs
@@ -338,14 +349,16 @@
         keyword arguments to pass to plot_graph_route
 
     Returns
     -------
     fig, ax : tuple
         matplotlib figure, axis
     """
+    _verify_mpl()
+
     # check for valid arguments
     if not all(isinstance(r, list) for r in routes):  # pragma: no cover
         raise ValueError("routes must be a list of route lists")
     if len(routes) < 2:  # pragma: no cover
         raise ValueError("You must pass more than 1 route")
     if isinstance(route_colors, str):
         route_colors = [route_colors] * len(routes)
@@ -437,14 +450,15 @@
         keyword arguments to pass to plot_graph
 
     Returns
     -------
     fig, ax : tuple
         matplotlib figure, axis
     """
+    _verify_mpl()
     multiplier = 1.2
 
     # if user did not pass in custom street widths, create a dict of defaults
     if street_widths is None:
         street_widths = {
             "footway": 1.5,
             "steps": 1.5,
@@ -569,15 +583,15 @@
     save=False,
     show=True,
     close=False,
     filepath=None,
     dpi=600,
 ):
     """
-    Plot a GeoDataFrame of geospatial entities' footprints.
+    Visualize a GeoDataFrame of geospatial entities' footprints.
 
     Parameters
     ----------
     gdf : geopandas.GeoDataFrame
         GeoDataFrame of footprints (shapely Polygons and MultiPolygons)
     ax : axis
         if not None, plot on this preexisting axis
@@ -609,14 +623,16 @@
         if save is True, the resolution of saved file
 
     Returns
     -------
     fig, ax : tuple
         matplotlib figure, axis
     """
+    _verify_mpl()
+
     if ax is None:
         fig, ax = plt.subplots(figsize=figsize, facecolor=bgcolor, frameon=False)
         ax.set_facecolor(bgcolor)
     else:
         fig = ax.figure
 
     # retain only Polygons and MultiPolygons, then plot
@@ -633,14 +649,151 @@
 
     # configure axis appearance, save/show figure as specified, and return
     ax = _config_ax(ax, gdf.crs, (north, south, east, west), 0)
     fig, ax = _save_and_show(fig, ax, save, show, close, filepath, dpi)
     return fig, ax
 
 
+def plot_orientation(
+    Gu,
+    num_bins=36,
+    min_length=0,
+    weight=None,
+    ax=None,
+    figsize=(5, 5),
+    area=True,
+    color="#003366",
+    edgecolor="k",
+    linewidth=0.5,
+    alpha=0.7,
+    title=None,
+    title_y=1.05,
+    title_font=None,
+    xtick_font=None,
+):
+    """
+    Plot a polar histogram of a spatial network's bidirectional edge bearings.
+
+    Ignores self-loop edges as their bearings are undefined.
+
+    For more info see: Boeing, G. 2019. "Urban Spatial Order: Street Network
+    Orientation, Configuration, and Entropy." Applied Network Science, 4 (1),
+    67. https://doi.org/10.1007/s41109-019-0189-1
+
+    Parameters
+    ----------
+    Gu : networkx.MultiGraph
+        undirected, unprojected graph with `bearing` attributes on each edge
+    num_bins : int
+        number of bins; for example, if `num_bins=36` is provided, then each
+        bin will represent 10° around the compass
+    min_length : float
+        ignore edges with `length` attributes less than `min_length`
+    weight : string
+        if not None, weight edges' bearings by this (non-null) edge attribute
+    ax : matplotlib.axes.PolarAxesSubplot
+        if not None, plot on this preexisting axis; must have projection=polar
+    figsize : tuple
+        if ax is None, create new figure with size (width, height)
+    area : bool
+        if True, set bar length so area is proportional to frequency,
+        otherwise set bar length so height is proportional to frequency
+    color : string
+        color of histogram bars
+    edgecolor : string
+        color of histogram bar edges
+    linewidth : float
+        width of histogram bar edges
+    alpha : float
+        opacity of histogram bars
+    title : string
+        title for plot
+    title_y : float
+        y position to place title
+    title_font : dict
+        the title's fontdict to pass to matplotlib
+    xtick_font : dict
+        the xtick labels' fontdict to pass to matplotlib
+
+    Returns
+    -------
+    fig, ax : tuple
+        matplotlib figure, axis
+    """
+    _verify_mpl()
+
+    if title_font is None:
+        title_font = {"family": "DejaVu Sans", "size": 24, "weight": "bold"}
+    if xtick_font is None:
+        xtick_font = {
+            "family": "DejaVu Sans",
+            "size": 10,
+            "weight": "bold",
+            "alpha": 1.0,
+            "zorder": 3,
+        }
+
+    # get the bearings' distribution's bin counts and edges
+    bin_counts, bin_edges = bearing._bearings_distribution(Gu, num_bins, min_length, weight)
+
+    # positions: where to center each bar. ignore the last bin edge, because
+    # it's the same as the first (i.e., 0° = 360°)
+    positions = np.radians(bin_edges[:-1])
+
+    # width: make bars fill the circumference without gaps or overlaps
+    width = 2 * np.pi / num_bins
+
+    # radius: how long to make each bar
+    bin_frequency = bin_counts / bin_counts.sum()
+    if area:
+        # set bar length so area is proportional to frequency
+        radius = np.sqrt(bin_frequency)
+    else:
+        # set bar length so height is proportional to frequency
+        radius = bin_frequency
+
+    # create ax (if necessary) then set N at top and go clockwise
+    if ax is None:
+        fig, ax = plt.subplots(figsize=figsize, subplot_kw={"projection": "polar"})
+    else:
+        fig = ax.figure
+    ax.set_theta_zero_location("N")
+    ax.set_theta_direction("clockwise")
+    ax.set_ylim(top=radius.max())
+
+    # configure the y-ticks and remove their labels
+    ax.set_yticks(np.linspace(0, radius.max(), 5))
+    ax.set_yticklabels(labels="")
+
+    # configure the x-ticks and their labels
+    xticklabels = ["N", "", "E", "", "S", "", "W", ""]
+    ax.set_xticks(ax.get_xticks())
+    ax.set_xticklabels(labels=xticklabels, fontdict=xtick_font)
+    ax.tick_params(axis="x", which="major", pad=-2)
+
+    # draw the bars
+    ax.bar(
+        positions,
+        height=radius,
+        width=width,
+        align="center",
+        bottom=0,
+        zorder=2,
+        color=color,
+        edgecolor=edgecolor,
+        linewidth=linewidth,
+        alpha=alpha,
+    )
+
+    if title:
+        ax.set_title(title, y=title_y, fontdict=title_font)
+    fig.tight_layout()
+    return fig, ax
+
+
 def _get_colors_by_value(vals, num_bins, cmap, start, stop, na_color, equal_size):
     """
     Map colors to the values in a series.
 
     Parameters
     ----------
     vals : pandas.Series
@@ -806,7 +959,21 @@
         ax.set_aspect("equal")
     else:
         # if not projected, conform aspect ratio to not stretch plot
         cos_lat = np.cos((south + north) / 2 / 180 * np.pi)
         ax.set_aspect(1 / cos_lat)
 
     return ax
+
+
+def _verify_mpl():
+    """
+    Verify that matplotlib is installed and successfully imported.
+
+    Returns
+    -------
+    None
+    """
+    if cm is None or colors is None or plt is None or colormaps is None:  # pragma: no cover
+        raise ImportError(
+            "matplotlib must be installed as an optional dependency for visualization"
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `osmnx-1.3.1.post0/osmnx/projection.py` & `osmnx-1.4.0/osmnx/projection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """Project spatial geometries and spatial networks."""
 
 import geopandas as gpd
 import numpy as np
-from pyproj import CRS
 
 from . import settings
 from . import utils
 from . import utils_graph
 
 
 def is_projected(crs):
     """
     Determine if a coordinate reference system is projected or not.
 
-    This is a convenience wrapper around the pyproj.CRS.is_projected function.
-
     Parameters
     ----------
     crs : string or pyproj.CRS
-        the coordinate reference system
+        the identifier of the coordinate reference system, which can be
+        anything accepted by pyproj.CRS.from_user_input() such as an authority
+        string or a WKT string
 
     Returns
     -------
     projected : bool
         True if crs is projected, otherwise False
     """
-    return CRS.from_user_input(crs).is_projected
+    return gpd.GeoSeries(crs=crs).crs.is_projected
 
 
 def project_geometry(geometry, crs=None, to_crs=None, to_latlong=False):
     """
     Project a shapely geometry from its current CRS to another.
 
     If to_crs is None, project to the UTM CRS for the UTM zone in which the
```

### Comparing `osmnx-1.3.1.post0/osmnx/settings.py` & `osmnx-1.4.0/osmnx/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Global settings that can be configured by the user.
 
 all_oneway : bool
-    If True, forces all ways to be loaded as oneway ways, preserving the
-    original order of nodes stored in the OSM way XML. This also retains
+    Only use if specifically saving to .osm XML file with the `save_graph_xml`
+    function. If True, forces all ways to be loaded as oneway ways, preserving
+    the original order of nodes stored in the OSM way XML. This also retains
     original OSM string values for oneway attribute values, rather than
-    converting them to a True/False bool. Only use if specifically saving to
-    .osm XML file with the `save_graph_xml` function. Default is `False`.
+    converting them to a True/False bool. Default is `False`.
 bidirectional_network_types : list
     Network types for which a fully bidirectional graph will be created.
     Default is `["walk"]`.
 cache_folder : string or pathlib.Path
-    Path to folder in which to save/load HTTP response cache. Default is
-    `"./cache"`.
+    Path to folder in which to save/load HTTP response cache, if the
+    `use_cache` setting equals `True`. Default is `"./cache"`.
 cache_only_mode : bool
     If True, download network data from Overpass then raise a
     `CacheOnlyModeInterrupt` error for user to catch. This prevents graph
     building from taking place and instead just saves OSM response data to
     cache. Useful for sequentially caching lots of raw data (as you can
     only query Overpass one request at a time) then using the local cache to
     quickly build many graphs simultaneously with multiprocessing. Default is
```

### Comparing `osmnx-1.3.1.post0/osmnx/simplification.py` & `osmnx-1.4.0/osmnx/simplification.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1.post0/osmnx/speed.py` & `osmnx-1.4.0/osmnx/speed.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Calculate graph edge speeds and travel times."""
 
 import re
+from warnings import warn
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 
 from . import utils_graph
 
 
-def add_edge_speeds(G, hwy_speeds=None, fallback=None, precision=1, agg=np.mean):
+def add_edge_speeds(G, hwy_speeds=None, fallback=None, precision=None, agg=np.mean):
     """
     Add edge speeds (km per hour) to graph as new `speed_kph` edge attributes.
 
     By default, this imputes free-flow travel speeds for all edges via the
     mean `maxspeed` value of the edges of each highway type. For highway types
     in the graph that have no `maxspeed` value on any edge, it assigns the
     mean of all `maxspeed` values in graph.
@@ -42,25 +43,33 @@
         assigned the mean preexisting speed value of all edges of that highway
         type.
     fallback : numeric
         default speed value (km per hour) to assign to edges whose highway
         type did not appear in `hwy_speeds` and had no preexisting speed
         values on any edge
     precision : int
-        decimal precision to round speed_kph
+        deprecated, do not use
     agg : function
         aggregation function to impute missing values from observed values.
         the default is numpy.mean, but you might also consider for example
         numpy.median, numpy.nanmedian, or your own custom function
 
     Returns
     -------
     G : networkx.MultiDiGraph
         graph with speed_kph attributes on all edges
     """
+    if precision is None:
+        precision = 1
+    else:
+        warn(
+            "the `precision` parameter is deprecated and will be removed in a future release",
+            stacklevel=2,
+        )
+
     if fallback is None:
         fallback = np.nan
 
     edges = utils_graph.graph_to_gdfs(G, nodes=False, fill_edge_geometry=False)
 
     # collapse any highway lists (can happen during graph simplification)
     # into string values simply by keeping just the first element of the list
@@ -117,35 +126,43 @@
     # add speed kph attribute to graph edges
     edges["speed_kph"] = speed_kph.round(precision).values
     nx.set_edge_attributes(G, values=edges["speed_kph"], name="speed_kph")
 
     return G
 
 
-def add_edge_travel_times(G, precision=1):
+def add_edge_travel_times(G, precision=None):
     """
     Add edge travel time (seconds) to graph as new `travel_time` edge attributes.
 
     Calculates free-flow travel time along each edge, based on `length` and
     `speed_kph` attributes. Note: run `add_edge_speeds` first to generate the
     `speed_kph` attribute. All edges must have `length` and `speed_kph`
     attributes and all their values must be non-null.
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
         input graph
     precision : int
-        decimal precision to round travel_time
+        deprecated, do not use
 
     Returns
     -------
     G : networkx.MultiDiGraph
         graph with travel_time attributes on all edges
     """
+    if precision is None:
+        precision = 1
+    else:
+        warn(
+            "the `precision` parameter is deprecated and will be removed in a future release",
+            stacklevel=2,
+        )
+
     edges = utils_graph.graph_to_gdfs(G, nodes=False)
 
     # verify edge length and speed_kph attributes exist and contain no nulls
     if not ("length" in edges.columns and "speed_kph" in edges.columns):  # pragma: no cover
         raise KeyError("all edges must have `length` and `speed_kph` attributes.")
     else:
         if (
```

### Comparing `osmnx-1.3.1.post0/osmnx/stats.py` & `osmnx-1.4.0/osmnx/stats.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1.post0/osmnx/truncate.py` & `osmnx-1.4.0/osmnx/truncate.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1.post0/osmnx/utils.py` & `osmnx-1.4.0/osmnx/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """General utility functions."""
 
 import datetime as dt
 import logging as lg
 import os
 import sys
 import unicodedata
-import warnings
 from contextlib import redirect_stdout
 from pathlib import Path
+from warnings import warn
 
 from . import settings
 
 
 def citation():
     """
     Print the OSMnx package's citation information.
@@ -185,20 +185,20 @@
     useful_tags_way : list
         deprecated
 
     Returns
     -------
     None
     """
-    warnings.warn(
+    warn(
         "The `utils.config` function is deprecated and will be removed in a "
         "future release. Instead, use the `settings` module directly to "
         "configure a global setting's value. For example, "
         "`ox.settings.log_console=True`.",
-        stacklevel=1,
+        stacklevel=2,
     )
 
     # set each global setting to the argument value
     settings.all_oneway = all_oneway
     settings.bidirectional_network_types = bidirectional_network_types
     settings.cache_folder = cache_folder
     settings.cache_only_mode = cache_only_mode
```

### Comparing `osmnx-1.3.1.post0/osmnx/utils_geo.py` & `osmnx-1.4.0/osmnx/utils_geo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Geospatial utility functions."""
 
-import warnings
+from warnings import warn
 
 import networkx as nx
 import numpy as np
 from shapely.geometry import LineString
 from shapely.geometry import MultiLineString
 from shapely.geometry import MultiPoint
 from shapely.geometry import MultiPolygon
@@ -38,17 +38,15 @@
     Returns
     -------
     points : geopandas.GeoSeries
         the sampled points, multi-indexed by (u, v, key) of the edge from
         which each point was drawn
     """
     if nx.is_directed(G):  # pragma: no cover
-        warnings.warn(
-            "graph should be undirected to not oversample bidirectional edges", stacklevel=1
-        )
+        warn("graph should be undirected to not oversample bidirectional edges", stacklevel=2)
     gdf_edges = utils_graph.graph_to_gdfs(G, nodes=False)[["geometry", "length"]]
     weights = gdf_edges["length"] / gdf_edges["length"].sum()
     idx = np.random.choice(gdf_edges.index, size=n, p=weights)
     lines = gdf_edges.loc[idx, "geometry"]
     return lines.interpolate(np.random.rand(n), normalized=True)
 
 
@@ -195,27 +193,32 @@
     shapely.geometry.MultiLineString
     """
     return MultiLineString([_round_linestring_coords(ls, precision) for ls in mls.geoms])
 
 
 def round_geometry_coords(geom, precision):
     """
-    Round the coordinates of a shapely geometry to some decimal precision.
+    Do not use: deprecated.
 
     Parameters
     ----------
     geom : shapely.geometry.geometry {Point, MultiPoint, LineString, MultiLineString, Polygon, MultiPolygon}
-        the geometry to round the coordinates of
+        deprecated, do not use
     precision : int
-        decimal precision to round coordinates to
+        deprecated, do not use
 
     Returns
     -------
     shapely.geometry.geometry
     """
+    warn(
+        "the `round_geometry_coords` function is deprecated and will be removed in a future release",
+        stacklevel=2,
+    )
+
     if isinstance(geom, Point):
         return _round_point_coords(geom, precision)
 
     elif isinstance(geom, MultiPoint):
         return _round_multipoint_coords(geom, precision)
 
     elif isinstance(geom, LineString):
```

### Comparing `osmnx-1.3.1.post0/osmnx/utils_graph.py` & `osmnx-1.4.0/osmnx/utils_graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Graph utility functions."""
 
 import itertools
-import warnings
+from warnings import warn
 
 import geopandas as gpd
 import networkx as nx
 import numpy as np
 import pandas as pd
 from shapely.geometry import LineString
 from shapely.geometry import Point
@@ -144,18 +144,18 @@
         try:
             all_x_match = (gdf_nodes.geometry.x == gdf_nodes["x"]).all()
             all_y_match = (gdf_nodes.geometry.y == gdf_nodes["y"]).all()
             assert all_x_match and all_y_match
         except (AssertionError, ValueError):  # pragma: no cover
             # AssertionError if x/y coords don't match geometry column
             # ValueError if geometry column contains non-point geometry types
-            warnings.warn(
+            warn(
                 "discarding the gdf_nodes geometry column, though its "
                 "values differ from the coordinates in the x and y columns",
-                stacklevel=1,
+                stacklevel=2,
             )
         gdf_nodes = gdf_nodes.drop(columns=gdf_nodes.geometry.name)
 
     # create graph and add graph-level attribute dict
     if graph_attrs is None:
         graph_attrs = {"crs": gdf_edges.crs}
     G = nx.MultiDiGraph(**graph_attrs)
@@ -175,42 +175,68 @@
     for col in gdf_nodes.columns:
         nx.set_node_attributes(G, name=col, values=gdf_nodes[col].dropna())
 
     utils.log("Created graph from node/edge GeoDataFrames")
     return G
 
 
+def route_to_gdf(G, route, weight="length"):
+    """
+    Return a GeoDataFrame of the edges in a path, in order.
+
+    Parameters
+    ----------
+    G : networkx.MultiDiGraph
+        input graph
+    route : list
+        list of node IDs constituting the path
+    weight : string
+        if there are parallel edges between two nodes, choose lowest weight
+
+    Returns
+    -------
+    gdf_edges : geopandas.GeoDataFrame
+        GeoDataFrame of the edges
+    """
+    pairs = zip(route[:-1], route[1:])
+    uvk = ((u, v, min(G[u][v].items(), key=lambda i: i[1][weight])[0]) for u, v in pairs)
+    return graph_to_gdfs(G.subgraph(route), nodes=False).loc[uvk]
+
+
 def get_route_edge_attributes(
     G, route, attribute=None, minimize_key="length", retrieve_default=None
 ):
     """
-    Get a list of attribute values for each edge in a path.
+    Do not use: deprecated.
+
+    Use the `route_to_gdf` function instead.
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
-        input graph
+        deprecated
     route : list
-        list of nodes IDs constituting the path
+        deprecated
     attribute : string
-        the name of the attribute to get the value of for each edge. If None,
-        the complete data dict is returned for each edge.
+        deprecated
     minimize_key : string
-        if there are parallel edges between two nodes, select the one with the
-        lowest value of minimize_key
+        deprecated
     retrieve_default : Callable[Tuple[Any, Any], Any]
-        function called with the edge nodes as parameters to retrieve a
-        default value, if the edge does not contain the given attribute
-        (otherwise a `KeyError` is raised)
+        deprecated
 
     Returns
     -------
     attribute_values : list
-        list of edge attribute values
+        deprecated
     """
+    warn(
+        "The `get_route_edge_attributes` function has been deprecated and will "
+        "be removed in a future release. Use the `route_to_gdf` function instead.",
+        stacklevel=2,
+    )
     attribute_values = []
     for u, v in zip(route[:-1], route[1:]):
         # if there are parallel edges between two nodes, select the one with the
         # lowest value of minimize_key
         data = min(G.get_edge_data(u, v).values(), key=lambda x: x[minimize_key])
         if attribute is None:
             attribute_value = data
```

### Comparing `osmnx-1.3.1.post0/osmnx.egg-info/PKG-INFO` & `osmnx-1.4.0/osmnx.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: osmnx
-Version: 1.3.1.post0
+Version: 1.4.0
 Summary: Retrieve, model, analyze, and visualize OpenStreetMap street networks and other spatial data
 Home-page: https://github.com/gboeing/osmnx
 Author: Geoff Boeing
 Author-email: boeing@usc.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: GIS
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: GIS
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: all
 Provides-Extra: entropy
 Provides-Extra: nearest_neighbor
+Provides-Extra: visualization
 Provides-Extra: raster
-Provides-Extra: web_map
 License-File: LICENSE.txt
 
 
 **OSMnx** is a Python package that lets you download spatial data and
 model, project, visualize, and analyze real-world street networks from
 OpenStreetMap's APIs. Users can download and model walkable, drivable, or
 bikeable urban networks with a single line of Python code, and then easily
```

### Comparing `osmnx-1.3.1.post0/osmnx.egg-info/SOURCES.txt` & `osmnx-1.4.0/osmnx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1.post0/setup.py` & `osmnx-1.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,28 +29,29 @@
 .. _docs: https://osmnx.readthedocs.io
 .. _OSMnx\: New Methods for Acquiring, Constructing, Analyzing, and Visualizing Complex Street Networks: http://geoffboeing.com/publications/osmnx-complex-street-networks/
 """
 
 # list of classifiers from the PyPI classifiers trove
 CLASSIFIERS = [
     "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Intended Audience :: Science/Research",
-    "Topic :: Scientific/Engineering :: GIS",
-    "Topic :: Scientific/Engineering :: Visualization",
-    "Topic :: Scientific/Engineering :: Physics",
-    "Topic :: Scientific/Engineering :: Mathematics",
-    "Topic :: Scientific/Engineering :: Information Analysis",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Topic :: Scientific/Engineering :: GIS",
+    "Topic :: Scientific/Engineering :: Information Analysis",
+    "Topic :: Scientific/Engineering :: Mathematics",
+    "Topic :: Scientific/Engineering :: Physics",
+    "Topic :: Scientific/Engineering :: Visualization",
 ]
 
 DESC = (
     "Retrieve, model, analyze, and visualize OpenStreetMap street networks and other spatial data"
 )
 
 # only specify install_requires if not in RTD environment
@@ -59,27 +60,28 @@
 else:
     with open("requirements.txt") as f:
         INSTALL_REQUIRES = [line.strip() for line in f.readlines()]
 
 # now call setup
 setup(
     name="osmnx",
-    version="1.3.1.post0",
+    version="1.4.0",
     description=DESC,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/x-rst",
     classifiers=CLASSIFIERS,
     url="https://github.com/gboeing/osmnx",
     author="Geoff Boeing",
     author_email="boeing@usc.edu",
     license="MIT",
     platforms="any",
     packages=["osmnx"],
     python_requires=">=3.8",
     install_requires=INSTALL_REQUIRES,
     extras_require={
+        "all": ["gdal", "matplotlib", "rasterio", "scikit-learn", "scipy"],
         "entropy": ["scipy"],
         "nearest_neighbor": ["scikit-learn", "scipy"],
+        "visualization": ["matplotlib"],
         "raster": ["gdal", "rasterio"],
-        "web_map": ["folium"],
     },
 )
```

### Comparing `osmnx-1.3.1.post0/tests/test_osmnx.py` & `osmnx-1.4.0/tests/test_osmnx.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,28 +110,31 @@
 
 def test_stats():
     # create graph, add a new node, add bearings, project it
     G = ox.graph_from_place(place1, network_type="all")
     G.add_node(0, x=location_point[1], y=location_point[0])
     _ = ox.bearing.calculate_bearing(0, 0, 1, 1)
     G = ox.add_edge_bearings(G)
+    G = ox.add_edge_bearings(G, precision=2)
     G_proj = ox.project_graph(G)
     G_proj = ox.distance.add_edge_lengths(G_proj, edges=tuple(G_proj.edges)[0:3])
+    G_proj = ox.distance.add_edge_lengths(G_proj, edges=tuple(G_proj.edges)[0:3], precision=2)
 
     # calculate stats
     cspn = ox.stats.count_streets_per_node(G)
     stats = ox.basic_stats(G)
     stats = ox.basic_stats(G, area=1000)
     stats = ox.basic_stats(G_proj, area=1000, clean_int_tol=15)
 
     # calculate entropy
     Gu = ox.get_undirected(G)
     entropy = ox.bearing.orientation_entropy(Gu, weight="length")
     fig, ax = ox.bearing.plot_orientation(Gu, area=True, title="Title")
-    fig, ax = ox.bearing.plot_orientation(Gu, ax=ax, area=False, title="Title")
+    fig, ax = ox.plot_orientation(Gu, area=True, title="Title")
+    fig, ax = ox.plot_orientation(Gu, ax=ax, area=False, title="Title")
 
     # test cleaning and rebuilding graph
     G_clean = ox.consolidate_intersections(G_proj, tolerance=10, rebuild_graph=True, dead_ends=True)
     G_clean = ox.consolidate_intersections(
         G_proj, tolerance=10, rebuild_graph=True, reconnect_edges=False
     )
     G_clean = ox.consolidate_intersections(G_proj, tolerance=10, rebuild_graph=False)
@@ -194,23 +197,25 @@
 
     # add node elevations from multiple raster files
     G = ox.elevation.add_node_elevations_raster(G, rasters)
     assert pd.notnull(pd.Series(dict(G.nodes(data="elevation")))).all()
 
     # add edge grades and their absolute values
     G = ox.add_edge_grades(G, add_absolute=True)
+    G = ox.add_edge_grades(G, add_absolute=True, precision=2)
 
 
 def test_routing():
     G = ox.graph_from_address(address=address, dist=500, dist_type="bbox", network_type="bike")
 
     # give each edge speed and travel time attributes
     G = ox.add_edge_speeds(G)
-    G = ox.add_edge_speeds(G, hwy_speeds={"motorway": 100})
+    G = ox.add_edge_speeds(G, hwy_speeds={"motorway": 100}, precision=2)
     G = ox.add_edge_travel_times(G)
+    G = ox.add_edge_travel_times(G, precision=2)
 
     # test value cleaning
     assert _clean_maxspeed("100,2") == 100.2
     assert _clean_maxspeed("100.2") == 100.2
     assert _clean_maxspeed("100 km/h") == 100.0
     assert _clean_maxspeed("100 mph") == pytest.approx(160.934)
     assert _clean_maxspeed("60|100") == 80
@@ -221,15 +226,26 @@
     orig_x = np.array([-122.404771])
     dest_x = np.array([-122.401429])
     orig_y = np.array([37.794302])
     dest_y = np.array([37.794987])
     orig_node = ox.distance.nearest_nodes(G, orig_x, orig_y)[0]
     dest_node = ox.distance.nearest_nodes(G, dest_x, dest_y)[0]
 
+    # test non-numeric weight (should raise ValueError)
+    try:
+        route = ox.shortest_path(G, orig_node, dest_node, weight="highway")
+        raise AssertionError()
+    except ValueError:
+        pass
+    # test missing weight (should raise warning)
+    route = ox.shortest_path(G, orig_node, dest_node, weight="time")
+    # test good weight
     route = ox.shortest_path(G, orig_node, dest_node, weight="travel_time")
+
+    route_edges = ox.utils_graph.route_to_gdf(G, route, "travel_time")
     attributes = ox.utils_graph.get_route_edge_attributes(G, route)
     attributes = ox.utils_graph.get_route_edge_attributes(G, route, "travel_time")
 
     fig, ax = ox.plot_graph_route(G, route, save=True)
 
     # test multiple origins-destinations
     n = 5
@@ -476,16 +492,19 @@
         dist=500,
         dist_type="network",
         network_type="all_private",
     )
 
 
 def test_geometries():
-    # geometries_from_bbox - bounding box query to return empty GeoDataFrame
-    gdf = ox.geometries_from_bbox(0.009, -0.009, 0.009, -0.009, tags={"building": True})
+    # geometries_from_bbox - bounding box query to return no data
+    try:
+        gdf = ox.geometries_from_bbox(0.009, -0.009, 0.009, -0.009, tags={"building": True})
+    except ox._errors.EmptyOverpassResponse:
+        pass
 
     # geometries_from_bbox - successful
     north, south, east, west = ox.utils_geo.bbox_from_point(location_point, dist=500)
     tags = {"landuse": True, "building": True, "highway": True}
     gdf = ox.geometries_from_bbox(north, south, east, west, tags=tags)
     fig, ax = ox.plot_footprints(gdf)
     fig, ax = ox.plot_footprints(gdf, ax=ax, bbox=(10, 0, 10, 0))
```

