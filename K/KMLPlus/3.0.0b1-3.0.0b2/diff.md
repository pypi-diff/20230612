# Comparing `tmp/KMLPlus-3.0.0b1.tar.gz` & `tmp/KMLPlus-3.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KMLPlus-3.0.0b1.tar", last modified: Thu Jun  1 17:55:21 2023, max compression
+gzip compressed data, was "KMLPlus-3.0.0b2.tar", last modified: Mon Jun 12 15:15:00 2023, max compression
```

## Comparing `KMLPlus-3.0.0b1.tar` & `KMLPlus-3.0.0b2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 17:55:21.798368 KMLPlus-3.0.0b1/
-drwxrwxrwx   0        0        0        0 2023-06-01 17:55:21.789357 KMLPlus-3.0.0b1/KMLPlus.egg-info/
--rw-rw-rw-   0        0        0    11555 2023-06-01 17:55:21.000000 KMLPlus-3.0.0b1/KMLPlus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-06-01 17:55:21.000000 KMLPlus-3.0.0b1/KMLPlus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 17:55:21.000000 KMLPlus-3.0.0b1/KMLPlus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-01 17:55:21.000000 KMLPlus-3.0.0b1/KMLPlus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2022-08-16 13:56:01.000000 KMLPlus-3.0.0b1/LICENSE
--rw-rw-rw-   0        0        0    11555 2023-06-01 17:55:21.797367 KMLPlus-3.0.0b1/PKG-INFO
--rw-rw-rw-   0        0        0    10998 2023-06-01 17:11:25.000000 KMLPlus-3.0.0b1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 17:55:21.793363 KMLPlus-3.0.0b1/kmlplus/
--rw-rw-rw-   0        0        0        0 2023-05-26 14:38:48.000000 KMLPlus-3.0.0b1/kmlplus/__init__.py
--rw-rw-rw-   0        0        0    23313 2023-06-01 17:02:09.000000 KMLPlus-3.0.0b1/kmlplus/geo.py
--rw-rw-rw-   0        0        0     3157 2023-06-01 16:07:02.000000 KMLPlus-3.0.0b1/kmlplus/interface.py
--rw-rw-rw-   0        0        0    10477 2023-06-01 17:55:14.000000 KMLPlus-3.0.0b1/kmlplus/kml.py
--rw-rw-rw-   0        0        0    21374 2023-06-01 16:07:02.000000 KMLPlus-3.0.0b1/kmlplus/shapes.py
--rw-rw-rw-   0        0        0     3924 2023-05-26 10:58:29.000000 KMLPlus-3.0.0b1/kmlplus/util.py
--rw-rw-rw-   0        0        0       42 2023-06-01 17:55:21.798368 KMLPlus-3.0.0b1/setup.cfg
--rw-rw-rw-   0        0        0      779 2023-06-01 17:55:14.000000 KMLPlus-3.0.0b1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 17:55:21.796367 KMLPlus-3.0.0b1/test/
--rw-rw-rw-   0        0        0        0 2022-08-16 13:56:01.000000 KMLPlus-3.0.0b1/test/__init__.py
--rw-rw-rw-   0        0        0     9603 2023-06-01 17:00:43.000000 KMLPlus-3.0.0b1/test/test_geo.py
--rw-rw-rw-   0        0        0     5365 2023-06-01 17:02:31.000000 KMLPlus-3.0.0b1/test/test_shapes.py
--rw-rw-rw-   0        0        0     4161 2023-06-01 15:57:55.000000 KMLPlus-3.0.0b1/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:00.601815 KMLPlus-3.0.0b2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:00.601815 KMLPlus-3.0.0b2/KMLPlus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-12 15:15:00.000000 KMLPlus-3.0.0b2/KMLPlus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-12 15:15:00.000000 KMLPlus-3.0.0b2/KMLPlus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:15:00.000000 KMLPlus-3.0.0b2/KMLPlus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 15:15:00.000000 KMLPlus-3.0.0b2/KMLPlus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-12 15:15:00.601815 KMLPlus-3.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:00.601815 KMLPlus-3.0.0b2/kmlplus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/kmlplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23511 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/kmlplus/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/kmlplus/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/kmlplus/kml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20811 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/kmlplus/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/kmlplus/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:15:00.601815 KMLPlus-3.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:00.601815 KMLPlus-3.0.0b2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/test/test_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/test/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-12 15:14:45.000000 KMLPlus-3.0.0b2/test/test_util.py
```

### Comparing `KMLPlus-3.0.0b1/KMLPlus.egg-info/PKG-INFO` & `KMLPlus-3.0.0b2/KMLPlus.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,344 +1,340 @@
-Metadata-Version: 2.1
-Name: KMLPlus
-Version: 3.0.0b1
-Summary: A Python library for creating 3d floating polygons and circles in .kml for Google Earth.
-Home-page: https://github.com/MHenderson1988/kmlplus
-Author: Mark Henderson
-Author-email: mark.henderson1988@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-KML+
-===
-
-KML+ (KMLPlus) is library of code for Python which allows the user to easily process_points standard and 'floating'
-Polygons, Circles and Arcs.
-
----
-
-Table of Contents
------------------
-
-1. [Who is this for](#who-is-this-for)
-2. [Installing](#installing)
-3. [Usage](#usage)
-    - [Recommendations](#recommendations)
-    - [Coordinates](#coordinates)
-    - [Coordinates containing Arcs](#coordinates-containing-arcs)
-4. [Classes and functions](#classes-and-functions)
-    - [KmlPlus](#kmlplus-class)
-      - [KmlPlus (functions)](#kmlplus-functions)
-        - [linestring](#linestring)
-        - [polyhedron](#polyhedron)
-        - [circle](#circle)
-        - [cylinder](#cylinder)
-        - [point](#point)
-5. [Acknowledgements](#acknowledgements)
-
----
-
-Who is this for
----------------
-
-This is for anyone who wishes to easily render polygons, especially 'floating' or curved polygons within Google Earth.
-
-I work in the aviation industry and needed a reliable way to process_points models of our airspace. It its useful for
-creating models of airways and controlled airspace. It can be used for anything that takes your fancy!
-
-![Prestwick airspace example](img/egpk_airspace_sideon.png)
-
-![Floating polygon example](img/floating_polygon_1.jpg)
-
----
-
-Installing
-----------
-
-### Pip
-
-```
-pip install kmlplus==2.1.0  <--- last stable release
-pip install kmlplus <--- Current v3.0.0-beta.1
-```
-
-### Clone
-
-```
-git clone https://github.com/MHenderson1988/kmlplus.git
-
-# Or
-
-git clone git@github.com:MHenderson1988/kmlplus.git
-```
-
-### Running tests
-
-```
-python -m unittest
-```
-
----
-
-Usage
------
-
-### Recommendations
-
-KML+ easily integrates with the fantastic [Simplekml](https://pypi.org/project/simplekml/) library and I highly
-recommend using it in conjunction with KML+ for the best experience.
-
-#### Coordinates
-
-Coordinates should always be passed as a single or multiple strings within a list in x, y, z(optional) format. Both
-Degrees Minutes Seconds (DDMMSS.ss) and Decimal Degres (DD.dd) are accepted. DMS should be suffixed with N, W, S or E.
-Decimal degrees are suffixed using -/+ convention.
-
-While a coordinate string must be passed using the same type of coordinate, lists can contain a mixture of DMS and DD
-coordinates and will convert appropriately.
-
-If no z value is provided, defaults to 0.0.
-
-Example 
-
-```
-[
-    '553124N 0045830W',
-    '552040N 0042722W',
-    '551848N 0044702W',
-    '553124N 0045830W'
-]
-```
-
-#### Coordinates containing Arcs
-
-When creating a curved segment of a polygon, the string should be passed as follows -
-
-'start=[starting_coordinate], end=[ending_coordinate], centre=[centre_coordinate],
-direction=[clockwise/anticlockwise]'
-
-Example -
-
-```
-[
-     'start=54.32111 -3.98721, end=54.13447 -3.89329, centre=54.31667 -3.41806, direction=anticlockwise',
-     '54.13444 -3.89333',
-     '54.17417 -4.14556',
-     'start=54.17418 -4.14551, end=54.23696 -4.17352, centre=54.31667 -3.41806, direction=clockwise',
-     '54.23694 -4.17361',
-     '54.32111 -3.98722',
-]
-```
-
-### Classes and functions
-
-v3.0 has stripped back to one single class which contains functions to process_points points, circles, cylinders,
-polygons, polyhedrons and linestrings.
-
-#### KmlPlus (Class)
-
-```
-from kmlplus.kml import KmlPlus
-
-KmlPlus(self, save_name='KmlPlus', output_path=None)
-```
-
-KmlPlus is the class through which you process_points your 2D and 3D geometries.
-
-* save_name accepts a string and is used for naming the resulting .kml file.
-* output_path accepts a string representing the directory the resulting .kml shall be saved to.
-
-#### KmlPlus (functions)
-
-linestring(coordinate_list, **kwargs)
-
-The linestring function updates the kml file with a KML linestring feature.
-
-```
-from kmlplus.kml import KmlPlus
-
-"""
-
-        Args:
-            coordinate_list (list): A list containing a single coordinate
-        Keyword Args:
-            fol (str): A string to name the folder in which the point is stored.
-            linestring_name (str): String to name the LineString object
-            colour_hex (str): String representing a colour hex
-            extrude (int): 1 or 0, Whether to extrude the point
-            width(int): Line width
-            altitude_mode(str): Accepts simplekml Altitude mode options
-
-
-        Returns:
-            None
-
-  """
-
-kml_file = KmlPlus('Point Styling.kml')
-kml_file.linestring(coordinates_list)
-```
-
-polyhedron(coordinate_list, **kwargs)
-
-Updates the KmlFile with a polyhedron based upon the coordinates and optional upper and lower limits.
-
-```
-"""
-
-        Args:
-            coordinate_list (list): A list of coordinates
-        Keyword Args:
-            fol (str): A string to name the folder in which the point is stored.
-            lower_layer (float): Height in FT of the lower layer
-            upper_layer (float): Height in FT of the upper layer
-            lower_polygon_name (str): Lower polygon object name
-            upper_polygon_name (str): Upper polygon object name
-            colour_hex (str): String representing a colour hex
-            fill (str): 1 or 0, whether or not to fill the polygon
-            outline (str): 1 or 0, whether to include outline of polygon
-            extrude (str): 1 or 0, Whether to extrude the point
-            altitude_mode (str): Accepts simplekml Altitude mode options
-
-        Returns:
-            None
-        """
-        
-kml_file = KmlPlus('Point Styling.kml')
-kml_file.polyhedron(coordinates_list, lower_layer = 2000, upper_layer = 5000)
-```
-
-circle(coordinate_list, radius, **kwargs)
-
-Creates a 2D circle. Coordinate list contains a single set of coordinates in x, y, z format.
-
-```
-"""
-
-        Args:
-            coordinate_list (list): A list containing a single set of coordinates which is the centre point of the circle
-            radius (float): The radius of the circle
-        Keyword Args:
-            fol (str): Name of the folder in which the KML objects are stored.
-            name (str): What to name the Circle object
-            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
-               Defaults to 'NM'
-            colour_hex (str): String representing a colour hex
-            extrude (int): 1 or 0, Whether to extrude the point
-            altitude_mode (str): Accepts simplekml Altitude mode options
-
-        Returns:
-            None
-
-        """
-        
-kml_file = KmlPlus('Point Styling.kml')
-kml_file.circle(coordinates_list, 500)
-```
-
-cylinder(coordinate_list, radius, **kwargs)
-
-Creates a Cylinder from a single set of coordinates within a list.
-
-```
-"""
-
-        Args:
-            coordinate_list: A list containing a single set of coordinates representing the centre of the circle
-            radius: The radius of the circle
-        Keyword Args:
-            lower_layer (float): Height/Altitude of the lower layer
-            upper_layer (float): Height/Altitude of the upper layer
-            sample (int): How many points to use when creating the circles which make up the cylinder
-            lower_circle_name (str): Lower circle object name
-            upper_circle_name (str): Upper circle object name
-            fol (str): Name of the folder in which the KML objects are stored.
-            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
-              Defaults to 'NM'
-            colour_hex (str): String representing a colour hex
-            fill (str): 1 or 0, whether or not to fill the polygon
-            outline (str): 1 or 0, whether to include outline of polygon
-            altitude_mode (str): Accepts simplekml Altitude mode options
-
-        Returns:
-            None
-        """
-
-kml_file = KmlPlus('Point Styling.kml')
-kml_file.cylinder(coordinates_list, 500, lower_layer=50, upper_layer=500)   
-
-```
-
-point(coordinate_list, **kwargs)
-
-Creates a single point from a single set of coordinates stored in a list in x, y, z format.
-
-```
-
-"""
-
-        Args:
-            coordinate_list (list): A list containing a single coordinate
-
-        Keyword Args:
-            fol (str): A string to name the folder in which the point is stored.
-            point_name (str): String to name the point object
-            colour_hex (str): String representing a colour hex
-            extrude (int): 1 or 0, Whether to extrude the point
-            altitude_mode (str): Accepts simplekml Altitude mode options
-
-
-        Returns:
-            None
-
-        """
-        point = PointFactory(coordinate_list).process_coordinates()
-
-        fol = self.kml.newfolder(name=kwargs.get('fol', 'KmlPlus Point'))
-
-        pnt = fol.newpoint(name=kwargs.get('point_name', 'KmlPlus Point'))
-        pnt.coords = [(point[0].x, point[0].y, point[0].z)]
-        pnt.style.color = kwargs.get('colour_hex', '7Fc0c0c0')
-        pnt.extrude = kwargs.get('extrude', 0)
-        pnt.altitudemode = kwargs.get('altitude_mode', simplekml.AltitudeMode.relativetoground)
-
-        self.kml.save(self.save_name)
-
-kml_file = KmlPlus('Point Styling.kml')
-kml_file.point(coordinates_list)   
-```
-
-### Example script
-
-```
-    kml_file = KmlPlus(file_name='Point Styling.kml')
-
-    kml_file.linestring(test_data.birmingham_cta_9, uom='FT')
-    kml_file.cylinder(test_data.beccles_parachute, 50000, upper_layer=5000)
-    kml_file.point(test_data.beccles_parachute)
-
-    kml_file.polyhedron(test_data.birmingham_cta_10, lower_layer=6500, upper_layer=10500,
-                        name='Birmingham CTA 10')
-    kml_file.polyhedron(test_data.birmingham_cta_9, lower_layer=6500, upper_layer=8500,
-                        name='Birmingham CTA 9')
-
-    kml_file.polyhedron(test_data.prestwick_cta_1, lower_layer=1500, upper_layer=5500, name='Prestwick CTA 1')
-    kml_file.polyhedron(test_data.prestwick_cta_2, lower_layer=2000, upper_layer=5500, name='Prestwick CTA 2')
-    kml_file.polyhedron(test_data.prestwick_cta_3, lower_layer=3000, upper_layer=5500, name='Prestwick CTA 3')
-    kml_file.polyhedron(test_data.prestwick_cta_4, lower_layer=3000, upper_layer=5500, name='Prestwick CTA 4')
-    kml_file.polyhedron(test_data.prestwick_cta_5, lower_layer=3500, upper_layer=5500, name='Prestwick CTA 5')
-    kml_file.polyhedron(test_data.prestwick_cta_6, lower_layer=4000, upper_layer=5500, name='Prestwick CTA 6')
-    kml_file.polyhedron(test_data.prestwick_ctr, upper_layer=5500, name='Prestwick CTR')
-    kml_file.polyhedron(test_data.test_airspace, upper_layer=50000, lower_layer=0, name='EG D406C ESKMEALS')
-```
-
-## Acknowledgements
-
-- [Simplekml](https://pypi.org/project/simplekml/) - for creating an awesome library which has helped me process_points
-  many things and also inspiring me to write this library.`
-
+Metadata-Version: 2.1
+Name: KMLPlus
+Version: 3.0.0b2
+Summary: A Python library for creating 3d floating polygons and circles in .kml for Google Earth.
+Home-page: https://github.com/MHenderson1988/kmlplus
+Author: Mark Henderson
+Author-email: mark.henderson1988@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+KML+
+===
+
+KML+ (KMLPlus) is library of code for Python which allows the user to easily process_points standard and 'floating'
+Polygons, Circles and Arcs.
+
+---
+
+Table of Contents
+-----------------
+
+1. [Who is this for](#who-is-this-for)
+2. [Installing](#installing)
+3. [Usage](#usage)
+    - [Recommendations](#recommendations)
+    - [Coordinates](#coordinates)
+    - [Coordinates containing Arcs](#coordinates-containing-arcs)
+4. [Classes and functions](#classes-and-functions)
+    - [KmlPlus](#kmlplus-class)
+        - [KmlPlus (functions)](#kmlplus-functions)
+            - [linestring](#linestring)
+            - [polyhedron](#polyhedron)
+            - [circle](#circle)
+            - [cylinder](#cylinder)
+            - [point](#point)
+5. [Acknowledgements](#acknowledgements)
+
+---
+
+Who is this for
+---------------
+
+This is for anyone who wishes to easily render polygons, especially 'floating' or curved polygons within Google Earth.
+
+I work in the aviation industry and needed a reliable way to process_points models of our airspace. It its useful for
+creating models of airways and controlled airspace. It can be used for anything that takes your fancy!
+
+![Prestwick airspace example](img/egpk_airspace_sideon.png)
+
+![Floating polygon example](img/floating_polygon_1.jpg)
+
+---
+
+Installing
+----------
+
+### Pip
+
+```
+pip install kmlplus==2.1.0  <--- last stable release
+pip install kmlplus==3.0.0b1 <--- Current v3.0.0-beta.1
+```
+
+### Clone
+
+```
+git clone https://github.com/MHenderson1988/kmlplus.git
+
+# Or
+
+git clone git@github.com:MHenderson1988/kmlplus.git
+```
+
+### Running tests
+
+```
+python -m unittest
+```
+
+---
+
+Usage v3
+-----
+
+### Recommendations
+
+KML+ easily integrates with the fantastic [Simplekml](https://pypi.org/project/simplekml/) library and I highly
+recommend using it in conjunction with KML+ for the best experience.
+
+#### Coordinates
+
+Coordinates should always be passed as a single or multiple strings within a list in x, y, z(optional) format. Both
+Degrees Minutes Seconds (DDMMSS.ss) and Decimal Degres (DD.dd) are accepted. DMS should be suffixed with N, W, S or E.
+Decimal degrees are suffixed using -/+ convention.
+
+While a coordinate string must be passed using the same type of coordinate, lists can contain a mixture of DMS and DD
+coordinates and will convert appropriately.
+
+If no z value is provided, defaults to 0.0.
+
+Example
+
+```
+[
+    '553124N 0045830W',
+    '552040N 0042722W',
+    '551848N 0044702W',
+    '553124N 0045830W'
+]
+```
+
+#### Coordinates containing Arcs
+
+When creating a curved segment of a polygon, the string should be passed as follows -
+
+'start=[starting_coordinate], end=[ending_coordinate], centre=[centre_coordinate], direction=[clockwise/anticlockwise]'
+
+Example -
+
+```
+[
+     'start=54.32111 -3.98721, end=54.13447 -3.89329, centre=54.31667 -3.41806, direction=anticlockwise',
+     '54.13444 -3.89333',
+     '54.17417 -4.14556',
+     'start=54.17418 -4.14551, end=54.23696 -4.17352, centre=54.31667 -3.41806, direction=clockwise',
+     '54.23694 -4.17361',
+     '54.32111 -3.98722',
+]
+```
+
+### Classes and functions
+
+v3.0 has stripped back to one single class which contains functions to process_points points, circles, cylinders,
+polygons, polyhedrons and linestrings.
+
+#### KmlPlus (Class)
+
+```
+from kmlplus.kml import KmlPlus
+
+KmlPlus(self, save_name='KmlPlus', output_path=None)
+```
+
+KmlPlus is the class through which you process_points your 2D and 3D geometries.
+
+* save_name accepts a string and is used for naming the resulting .kml file.
+* output_path accepts a string representing the directory the resulting .kml shall be saved to.
+
+#### KmlPlus (functions)
+
+linestring(coordinate_list, **kwargs)
+
+The linestring function updates the kml file with a KML linestring feature.
+
+```
+from kmlplus.kml import KmlPlus
+
+"""
+
+        Args:
+            coordinate_list (list): A list containing a single coordinate
+        Keyword Args:
+            fol (str): A string to name the folder in which the point is stored.
+            linestring_name (str): String to name the LineString object
+            colour_hex (str): String representing a colour hex
+            extrude (int): 1 or 0, Whether to extrude the point
+            width(int): Line width
+            altitude_mode(str): Accepts simplekml Altitude mode options
+
+
+        Returns:
+            None
+
+  """
+
+kml_file = KmlPlus('Point Styling.kml')
+kml_file.linestring(coordinates_list)
+```
+
+polyhedron(coordinate_list, **kwargs)
+
+Updates the KmlFile with a polyhedron based upon the coordinates and optional upper and lower limits.
+
+```
+"""
+
+        Args:
+            coordinate_list (list): A list of coordinates
+        Keyword Args:
+            fol (str): A string to name the folder in which the point is stored.
+            lower_layer (float): Height in FT of the lower layer
+            upper_layer (float): Height in FT of the upper layer
+            lower_polygon_name (str): Lower polygon object name
+            upper_polygon_name (str): Upper polygon object name
+            colour_hex (str): String representing a colour hex
+            fill (str): 1 or 0, whether or not to fill the polygon
+            outline (str): 1 or 0, whether to include outline of polygon
+            extrude (str): 1 or 0, Whether to extrude the point
+            altitude_mode (str): Accepts simplekml Altitude mode options
+
+        Returns:
+            None
+        """
+        
+kml_file = KmlPlus('Point Styling.kml')
+kml_file.polyhedron(coordinates_list, lower_layer = 2000, upper_layer = 5000)
+```
+
+circle(coordinate_list, radius, **kwargs)
+
+Creates a 2D circle. Coordinate list contains a single set of coordinates in x, y, z format.
+
+```
+"""
+
+        Args:
+            coordinate_list (list): A list containing a single set of coordinates which is the centre point of the circle
+            radius (float): The radius of the circle
+        Keyword Args:
+            fol (str): Name of the folder in which the KML objects are stored.
+            name (str): What to name the Circle object
+            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
+               Defaults to 'NM'
+            colour_hex (str): String representing a colour hex
+            extrude (int): 1 or 0, Whether to extrude the point
+            altitude_mode (str): Accepts simplekml Altitude mode options
+
+        Returns:
+            None
+
+        """
+        
+kml_file = KmlPlus('Point Styling.kml')
+kml_file.circle(coordinates_list, 500)
+```
+
+cylinder(coordinate_list, radius, **kwargs)
+
+Creates a Cylinder from a single set of coordinates within a list.
+
+```
+"""
+
+        Args:
+            coordinate_list: A list containing a single set of coordinates representing the centre of the circle
+            radius: The radius of the circle
+        Keyword Args:
+            lower_layer (float): Height/Altitude of the lower layer
+            upper_layer (float): Height/Altitude of the upper layer
+            sample (int): How many points to use when creating the circles which make up the cylinder
+            lower_circle_name (str): Lower circle object name
+            upper_circle_name (str): Upper circle object name
+            fol (str): Name of the folder in which the KML objects are stored.
+            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
+              Defaults to 'NM'
+            colour_hex (str): String representing a colour hex
+            fill (str): 1 or 0, whether or not to fill the polygon
+            outline (str): 1 or 0, whether to include outline of polygon
+            altitude_mode (str): Accepts simplekml Altitude mode options
+
+        Returns:
+            None
+        """
+
+kml_file = KmlPlus('Point Styling.kml')
+kml_file.cylinder(coordinates_list, 500, lower_layer=50, upper_layer=500)   
+
+```
+
+point(coordinate_list, **kwargs)
+
+Creates a single point from a single set of coordinates stored in a list in x, y, z format.
+
+```
+
+"""
+
+        Args:
+            coordinate_list (list): A list containing a single coordinate
+
+        Keyword Args:
+            fol (str): A string to name the folder in which the point is stored.
+            point_name (str): String to name the point object
+            colour_hex (str): String representing a colour hex
+            extrude (int): 1 or 0, Whether to extrude the point
+            altitude_mode (str): Accepts simplekml Altitude mode options
+
+
+        Returns:
+            None
+
+        """
+        point = PointFactory(coordinate_list).process_coordinates()
+
+        fol = self.kml.newfolder(name=kwargs.get('fol', 'KmlPlus Point'))
+
+        pnt = fol.newpoint(name=kwargs.get('point_name', 'KmlPlus Point'))
+        pnt.coords = [(point[0].x, point[0].y, point[0].z)]
+        pnt.style.color = kwargs.get('colour_hex', '7Fc0c0c0')
+        pnt.extrude = kwargs.get('extrude', 0)
+        pnt.altitudemode = kwargs.get('altitude_mode', simplekml.AltitudeMode.relativetoground)
+
+        self.kml.save(self.save_name)
+
+kml_file = KmlPlus('Point Styling.kml')
+kml_file.point(coordinates_list)   
+```
+
+### Example script
+
+```
+    kml_file = KmlPlus(file_name='Point Styling.kml')
+
+    kml_file.linestring(test_data.birmingham_cta_9, uom='FT')
+    kml_file.cylinder(test_data.beccles_parachute, 50000, upper_layer=5000)
+    kml_file.point(test_data.beccles_parachute)
+
+    kml_file.polyhedron(test_data.birmingham_cta_10, lower_layer=6500, upper_layer=10500,
+                        name='Birmingham CTA 10')
+    kml_file.polyhedron(test_data.birmingham_cta_9, lower_layer=6500, upper_layer=8500,
+                        name='Birmingham CTA 9')
+
+    kml_file.polyhedron(test_data.prestwick_cta_1, lower_layer=1500, upper_layer=5500, name='Prestwick CTA 1')
+    kml_file.polyhedron(test_data.prestwick_cta_2, lower_layer=2000, upper_layer=5500, name='Prestwick CTA 2')
+    kml_file.polyhedron(test_data.prestwick_cta_3, lower_layer=3000, upper_layer=5500, name='Prestwick CTA 3')
+    kml_file.polyhedron(test_data.prestwick_cta_4, lower_layer=3000, upper_layer=5500, name='Prestwick CTA 4')
+    kml_file.polyhedron(test_data.prestwick_cta_5, lower_layer=3500, upper_layer=5500, name='Prestwick CTA 5')
+    kml_file.polyhedron(test_data.prestwick_cta_6, lower_layer=4000, upper_layer=5500, name='Prestwick CTA 6')
+    kml_file.polyhedron(test_data.prestwick_ctr, upper_layer=5500, name='Prestwick CTR')
+    kml_file.polyhedron(test_data.test_airspace, upper_layer=50000, lower_layer=0, name='EG D406C ESKMEALS')
+```
+
+## Acknowledgements
+
+- [Simplekml](https://pypi.org/project/simplekml/) - for creating an awesome library which has helped me process_points
+  many things and also inspiring me to write this library.`
```

### Comparing `KMLPlus-3.0.0b1/LICENSE` & `KMLPlus-3.0.0b2/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Mark Henderson
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Mark Henderson
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `KMLPlus-3.0.0b1/PKG-INFO` & `KMLPlus-3.0.0b2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,344 +1,340 @@
-Metadata-Version: 2.1
-Name: KMLPlus
-Version: 3.0.0b1
-Summary: A Python library for creating 3d floating polygons and circles in .kml for Google Earth.
-Home-page: https://github.com/MHenderson1988/kmlplus
-Author: Mark Henderson
-Author-email: mark.henderson1988@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-KML+
-===
-
-KML+ (KMLPlus) is library of code for Python which allows the user to easily process_points standard and 'floating'
-Polygons, Circles and Arcs.
-
----
-
-Table of Contents
------------------
-
-1. [Who is this for](#who-is-this-for)
-2. [Installing](#installing)
-3. [Usage](#usage)
-    - [Recommendations](#recommendations)
-    - [Coordinates](#coordinates)
-    - [Coordinates containing Arcs](#coordinates-containing-arcs)
-4. [Classes and functions](#classes-and-functions)
-    - [KmlPlus](#kmlplus-class)
-      - [KmlPlus (functions)](#kmlplus-functions)
-        - [linestring](#linestring)
-        - [polyhedron](#polyhedron)
-        - [circle](#circle)
-        - [cylinder](#cylinder)
-        - [point](#point)
-5. [Acknowledgements](#acknowledgements)
-
----
-
-Who is this for
----------------
-
-This is for anyone who wishes to easily render polygons, especially 'floating' or curved polygons within Google Earth.
-
-I work in the aviation industry and needed a reliable way to process_points models of our airspace. It its useful for
-creating models of airways and controlled airspace. It can be used for anything that takes your fancy!
-
-![Prestwick airspace example](img/egpk_airspace_sideon.png)
-
-![Floating polygon example](img/floating_polygon_1.jpg)
-
----
-
-Installing
-----------
-
-### Pip
-
-```
-pip install kmlplus==2.1.0  <--- last stable release
-pip install kmlplus <--- Current v3.0.0-beta.1
-```
-
-### Clone
-
-```
-git clone https://github.com/MHenderson1988/kmlplus.git
-
-# Or
-
-git clone git@github.com:MHenderson1988/kmlplus.git
-```
-
-### Running tests
-
-```
-python -m unittest
-```
-
----
-
-Usage
------
-
-### Recommendations
-
-KML+ easily integrates with the fantastic [Simplekml](https://pypi.org/project/simplekml/) library and I highly
-recommend using it in conjunction with KML+ for the best experience.
-
-#### Coordinates
-
-Coordinates should always be passed as a single or multiple strings within a list in x, y, z(optional) format. Both
-Degrees Minutes Seconds (DDMMSS.ss) and Decimal Degres (DD.dd) are accepted. DMS should be suffixed with N, W, S or E.
-Decimal degrees are suffixed using -/+ convention.
-
-While a coordinate string must be passed using the same type of coordinate, lists can contain a mixture of DMS and DD
-coordinates and will convert appropriately.
-
-If no z value is provided, defaults to 0.0.
-
-Example 
-
-```
-[
-    '553124N 0045830W',
-    '552040N 0042722W',
-    '551848N 0044702W',
-    '553124N 0045830W'
-]
-```
-
-#### Coordinates containing Arcs
-
-When creating a curved segment of a polygon, the string should be passed as follows -
-
-'start=[starting_coordinate], end=[ending_coordinate], centre=[centre_coordinate],
-direction=[clockwise/anticlockwise]'
-
-Example -
-
-```
-[
-     'start=54.32111 -3.98721, end=54.13447 -3.89329, centre=54.31667 -3.41806, direction=anticlockwise',
-     '54.13444 -3.89333',
-     '54.17417 -4.14556',
-     'start=54.17418 -4.14551, end=54.23696 -4.17352, centre=54.31667 -3.41806, direction=clockwise',
-     '54.23694 -4.17361',
-     '54.32111 -3.98722',
-]
-```
-
-### Classes and functions
-
-v3.0 has stripped back to one single class which contains functions to process_points points, circles, cylinders,
-polygons, polyhedrons and linestrings.
-
-#### KmlPlus (Class)
-
-```
-from kmlplus.kml import KmlPlus
-
-KmlPlus(self, save_name='KmlPlus', output_path=None)
-```
-
-KmlPlus is the class through which you process_points your 2D and 3D geometries.
-
-* save_name accepts a string and is used for naming the resulting .kml file.
-* output_path accepts a string representing the directory the resulting .kml shall be saved to.
-
-#### KmlPlus (functions)
-
-linestring(coordinate_list, **kwargs)
-
-The linestring function updates the kml file with a KML linestring feature.
-
-```
-from kmlplus.kml import KmlPlus
-
-"""
-
-        Args:
-            coordinate_list (list): A list containing a single coordinate
-        Keyword Args:
-            fol (str): A string to name the folder in which the point is stored.
-            linestring_name (str): String to name the LineString object
-            colour_hex (str): String representing a colour hex
-            extrude (int): 1 or 0, Whether to extrude the point
-            width(int): Line width
-            altitude_mode(str): Accepts simplekml Altitude mode options
-
-
-        Returns:
-            None
-
-  """
-
-kml_file = KmlPlus('Point Styling.kml')
-kml_file.linestring(coordinates_list)
-```
-
-polyhedron(coordinate_list, **kwargs)
-
-Updates the KmlFile with a polyhedron based upon the coordinates and optional upper and lower limits.
-
-```
-"""
-
-        Args:
-            coordinate_list (list): A list of coordinates
-        Keyword Args:
-            fol (str): A string to name the folder in which the point is stored.
-            lower_layer (float): Height in FT of the lower layer
-            upper_layer (float): Height in FT of the upper layer
-            lower_polygon_name (str): Lower polygon object name
-            upper_polygon_name (str): Upper polygon object name
-            colour_hex (str): String representing a colour hex
-            fill (str): 1 or 0, whether or not to fill the polygon
-            outline (str): 1 or 0, whether to include outline of polygon
-            extrude (str): 1 or 0, Whether to extrude the point
-            altitude_mode (str): Accepts simplekml Altitude mode options
-
-        Returns:
-            None
-        """
-        
-kml_file = KmlPlus('Point Styling.kml')
-kml_file.polyhedron(coordinates_list, lower_layer = 2000, upper_layer = 5000)
-```
-
-circle(coordinate_list, radius, **kwargs)
-
-Creates a 2D circle. Coordinate list contains a single set of coordinates in x, y, z format.
-
-```
-"""
-
-        Args:
-            coordinate_list (list): A list containing a single set of coordinates which is the centre point of the circle
-            radius (float): The radius of the circle
-        Keyword Args:
-            fol (str): Name of the folder in which the KML objects are stored.
-            name (str): What to name the Circle object
-            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
-               Defaults to 'NM'
-            colour_hex (str): String representing a colour hex
-            extrude (int): 1 or 0, Whether to extrude the point
-            altitude_mode (str): Accepts simplekml Altitude mode options
-
-        Returns:
-            None
-
-        """
-        
-kml_file = KmlPlus('Point Styling.kml')
-kml_file.circle(coordinates_list, 500)
-```
-
-cylinder(coordinate_list, radius, **kwargs)
-
-Creates a Cylinder from a single set of coordinates within a list.
-
-```
-"""
-
-        Args:
-            coordinate_list: A list containing a single set of coordinates representing the centre of the circle
-            radius: The radius of the circle
-        Keyword Args:
-            lower_layer (float): Height/Altitude of the lower layer
-            upper_layer (float): Height/Altitude of the upper layer
-            sample (int): How many points to use when creating the circles which make up the cylinder
-            lower_circle_name (str): Lower circle object name
-            upper_circle_name (str): Upper circle object name
-            fol (str): Name of the folder in which the KML objects are stored.
-            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
-              Defaults to 'NM'
-            colour_hex (str): String representing a colour hex
-            fill (str): 1 or 0, whether or not to fill the polygon
-            outline (str): 1 or 0, whether to include outline of polygon
-            altitude_mode (str): Accepts simplekml Altitude mode options
-
-        Returns:
-            None
-        """
-
-kml_file = KmlPlus('Point Styling.kml')
-kml_file.cylinder(coordinates_list, 500, lower_layer=50, upper_layer=500)   
-
-```
-
-point(coordinate_list, **kwargs)
-
-Creates a single point from a single set of coordinates stored in a list in x, y, z format.
-
-```
-
-"""
-
-        Args:
-            coordinate_list (list): A list containing a single coordinate
-
-        Keyword Args:
-            fol (str): A string to name the folder in which the point is stored.
-            point_name (str): String to name the point object
-            colour_hex (str): String representing a colour hex
-            extrude (int): 1 or 0, Whether to extrude the point
-            altitude_mode (str): Accepts simplekml Altitude mode options
-
-
-        Returns:
-            None
-
-        """
-        point = PointFactory(coordinate_list).process_coordinates()
-
-        fol = self.kml.newfolder(name=kwargs.get('fol', 'KmlPlus Point'))
-
-        pnt = fol.newpoint(name=kwargs.get('point_name', 'KmlPlus Point'))
-        pnt.coords = [(point[0].x, point[0].y, point[0].z)]
-        pnt.style.color = kwargs.get('colour_hex', '7Fc0c0c0')
-        pnt.extrude = kwargs.get('extrude', 0)
-        pnt.altitudemode = kwargs.get('altitude_mode', simplekml.AltitudeMode.relativetoground)
-
-        self.kml.save(self.save_name)
-
-kml_file = KmlPlus('Point Styling.kml')
-kml_file.point(coordinates_list)   
-```
-
-### Example script
-
-```
-    kml_file = KmlPlus(file_name='Point Styling.kml')
-
-    kml_file.linestring(test_data.birmingham_cta_9, uom='FT')
-    kml_file.cylinder(test_data.beccles_parachute, 50000, upper_layer=5000)
-    kml_file.point(test_data.beccles_parachute)
-
-    kml_file.polyhedron(test_data.birmingham_cta_10, lower_layer=6500, upper_layer=10500,
-                        name='Birmingham CTA 10')
-    kml_file.polyhedron(test_data.birmingham_cta_9, lower_layer=6500, upper_layer=8500,
-                        name='Birmingham CTA 9')
-
-    kml_file.polyhedron(test_data.prestwick_cta_1, lower_layer=1500, upper_layer=5500, name='Prestwick CTA 1')
-    kml_file.polyhedron(test_data.prestwick_cta_2, lower_layer=2000, upper_layer=5500, name='Prestwick CTA 2')
-    kml_file.polyhedron(test_data.prestwick_cta_3, lower_layer=3000, upper_layer=5500, name='Prestwick CTA 3')
-    kml_file.polyhedron(test_data.prestwick_cta_4, lower_layer=3000, upper_layer=5500, name='Prestwick CTA 4')
-    kml_file.polyhedron(test_data.prestwick_cta_5, lower_layer=3500, upper_layer=5500, name='Prestwick CTA 5')
-    kml_file.polyhedron(test_data.prestwick_cta_6, lower_layer=4000, upper_layer=5500, name='Prestwick CTA 6')
-    kml_file.polyhedron(test_data.prestwick_ctr, upper_layer=5500, name='Prestwick CTR')
-    kml_file.polyhedron(test_data.test_airspace, upper_layer=50000, lower_layer=0, name='EG D406C ESKMEALS')
-```
-
-## Acknowledgements
-
-- [Simplekml](https://pypi.org/project/simplekml/) - for creating an awesome library which has helped me process_points
-  many things and also inspiring me to write this library.`
-
+Metadata-Version: 2.1
+Name: KMLPlus
+Version: 3.0.0b2
+Summary: A Python library for creating 3d floating polygons and circles in .kml for Google Earth.
+Home-page: https://github.com/MHenderson1988/kmlplus
+Author: Mark Henderson
+Author-email: mark.henderson1988@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+KML+
+===
+
+KML+ (KMLPlus) is library of code for Python which allows the user to easily process_points standard and 'floating'
+Polygons, Circles and Arcs.
+
+---
+
+Table of Contents
+-----------------
+
+1. [Who is this for](#who-is-this-for)
+2. [Installing](#installing)
+3. [Usage](#usage)
+    - [Recommendations](#recommendations)
+    - [Coordinates](#coordinates)
+    - [Coordinates containing Arcs](#coordinates-containing-arcs)
+4. [Classes and functions](#classes-and-functions)
+    - [KmlPlus](#kmlplus-class)
+        - [KmlPlus (functions)](#kmlplus-functions)
+            - [linestring](#linestring)
+            - [polyhedron](#polyhedron)
+            - [circle](#circle)
+            - [cylinder](#cylinder)
+            - [point](#point)
+5. [Acknowledgements](#acknowledgements)
+
+---
+
+Who is this for
+---------------
+
+This is for anyone who wishes to easily render polygons, especially 'floating' or curved polygons within Google Earth.
+
+I work in the aviation industry and needed a reliable way to process_points models of our airspace. It its useful for
+creating models of airways and controlled airspace. It can be used for anything that takes your fancy!
+
+![Prestwick airspace example](img/egpk_airspace_sideon.png)
+
+![Floating polygon example](img/floating_polygon_1.jpg)
+
+---
+
+Installing
+----------
+
+### Pip
+
+```
+pip install kmlplus==2.1.0  <--- last stable release
+pip install kmlplus==3.0.0b1 <--- Current v3.0.0-beta.1
+```
+
+### Clone
+
+```
+git clone https://github.com/MHenderson1988/kmlplus.git
+
+# Or
+
+git clone git@github.com:MHenderson1988/kmlplus.git
+```
+
+### Running tests
+
+```
+python -m unittest
+```
+
+---
+
+Usage v3
+-----
+
+### Recommendations
+
+KML+ easily integrates with the fantastic [Simplekml](https://pypi.org/project/simplekml/) library and I highly
+recommend using it in conjunction with KML+ for the best experience.
+
+#### Coordinates
+
+Coordinates should always be passed as a single or multiple strings within a list in x, y, z(optional) format. Both
+Degrees Minutes Seconds (DDMMSS.ss) and Decimal Degres (DD.dd) are accepted. DMS should be suffixed with N, W, S or E.
+Decimal degrees are suffixed using -/+ convention.
+
+While a coordinate string must be passed using the same type of coordinate, lists can contain a mixture of DMS and DD
+coordinates and will convert appropriately.
+
+If no z value is provided, defaults to 0.0.
+
+Example
+
+```
+[
+    '553124N 0045830W',
+    '552040N 0042722W',
+    '551848N 0044702W',
+    '553124N 0045830W'
+]
+```
+
+#### Coordinates containing Arcs
+
+When creating a curved segment of a polygon, the string should be passed as follows -
+
+'start=[starting_coordinate], end=[ending_coordinate], centre=[centre_coordinate], direction=[clockwise/anticlockwise]'
+
+Example -
+
+```
+[
+     'start=54.32111 -3.98721, end=54.13447 -3.89329, centre=54.31667 -3.41806, direction=anticlockwise',
+     '54.13444 -3.89333',
+     '54.17417 -4.14556',
+     'start=54.17418 -4.14551, end=54.23696 -4.17352, centre=54.31667 -3.41806, direction=clockwise',
+     '54.23694 -4.17361',
+     '54.32111 -3.98722',
+]
+```
+
+### Classes and functions
+
+v3.0 has stripped back to one single class which contains functions to process_points points, circles, cylinders,
+polygons, polyhedrons and linestrings.
+
+#### KmlPlus (Class)
+
+```
+from kmlplus.kml import KmlPlus
+
+KmlPlus(self, save_name='KmlPlus', output_path=None)
+```
+
+KmlPlus is the class through which you process_points your 2D and 3D geometries.
+
+* save_name accepts a string and is used for naming the resulting .kml file.
+* output_path accepts a string representing the directory the resulting .kml shall be saved to.
+
+#### KmlPlus (functions)
+
+linestring(coordinate_list, **kwargs)
+
+The linestring function updates the kml file with a KML linestring feature.
+
+```
+from kmlplus.kml import KmlPlus
+
+"""
+
+        Args:
+            coordinate_list (list): A list containing a single coordinate
+        Keyword Args:
+            fol (str): A string to name the folder in which the point is stored.
+            linestring_name (str): String to name the LineString object
+            colour_hex (str): String representing a colour hex
+            extrude (int): 1 or 0, Whether to extrude the point
+            width(int): Line width
+            altitude_mode(str): Accepts simplekml Altitude mode options
+
+
+        Returns:
+            None
+
+  """
+
+kml_file = KmlPlus('Point Styling.kml')
+kml_file.linestring(coordinates_list)
+```
+
+polyhedron(coordinate_list, **kwargs)
+
+Updates the KmlFile with a polyhedron based upon the coordinates and optional upper and lower limits.
+
+```
+"""
+
+        Args:
+            coordinate_list (list): A list of coordinates
+        Keyword Args:
+            fol (str): A string to name the folder in which the point is stored.
+            lower_layer (float): Height in FT of the lower layer
+            upper_layer (float): Height in FT of the upper layer
+            lower_polygon_name (str): Lower polygon object name
+            upper_polygon_name (str): Upper polygon object name
+            colour_hex (str): String representing a colour hex
+            fill (str): 1 or 0, whether or not to fill the polygon
+            outline (str): 1 or 0, whether to include outline of polygon
+            extrude (str): 1 or 0, Whether to extrude the point
+            altitude_mode (str): Accepts simplekml Altitude mode options
+
+        Returns:
+            None
+        """
+        
+kml_file = KmlPlus('Point Styling.kml')
+kml_file.polyhedron(coordinates_list, lower_layer = 2000, upper_layer = 5000)
+```
+
+circle(coordinate_list, radius, **kwargs)
+
+Creates a 2D circle. Coordinate list contains a single set of coordinates in x, y, z format.
+
+```
+"""
+
+        Args:
+            coordinate_list (list): A list containing a single set of coordinates which is the centre point of the circle
+            radius (float): The radius of the circle
+        Keyword Args:
+            fol (str): Name of the folder in which the KML objects are stored.
+            name (str): What to name the Circle object
+            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
+               Defaults to 'NM'
+            colour_hex (str): String representing a colour hex
+            extrude (int): 1 or 0, Whether to extrude the point
+            altitude_mode (str): Accepts simplekml Altitude mode options
+
+        Returns:
+            None
+
+        """
+        
+kml_file = KmlPlus('Point Styling.kml')
+kml_file.circle(coordinates_list, 500)
+```
+
+cylinder(coordinate_list, radius, **kwargs)
+
+Creates a Cylinder from a single set of coordinates within a list.
+
+```
+"""
+
+        Args:
+            coordinate_list: A list containing a single set of coordinates representing the centre of the circle
+            radius: The radius of the circle
+        Keyword Args:
+            lower_layer (float): Height/Altitude of the lower layer
+            upper_layer (float): Height/Altitude of the upper layer
+            sample (int): How many points to use when creating the circles which make up the cylinder
+            lower_circle_name (str): Lower circle object name
+            upper_circle_name (str): Upper circle object name
+            fol (str): Name of the folder in which the KML objects are stored.
+            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
+              Defaults to 'NM'
+            colour_hex (str): String representing a colour hex
+            fill (str): 1 or 0, whether or not to fill the polygon
+            outline (str): 1 or 0, whether to include outline of polygon
+            altitude_mode (str): Accepts simplekml Altitude mode options
+
+        Returns:
+            None
+        """
+
+kml_file = KmlPlus('Point Styling.kml')
+kml_file.cylinder(coordinates_list, 500, lower_layer=50, upper_layer=500)   
+
+```
+
+point(coordinate_list, **kwargs)
+
+Creates a single point from a single set of coordinates stored in a list in x, y, z format.
+
+```
+
+"""
+
+        Args:
+            coordinate_list (list): A list containing a single coordinate
+
+        Keyword Args:
+            fol (str): A string to name the folder in which the point is stored.
+            point_name (str): String to name the point object
+            colour_hex (str): String representing a colour hex
+            extrude (int): 1 or 0, Whether to extrude the point
+            altitude_mode (str): Accepts simplekml Altitude mode options
+
+
+        Returns:
+            None
+
+        """
+        point = PointFactory(coordinate_list).process_coordinates()
+
+        fol = self.kml.newfolder(name=kwargs.get('fol', 'KmlPlus Point'))
+
+        pnt = fol.newpoint(name=kwargs.get('point_name', 'KmlPlus Point'))
+        pnt.coords = [(point[0].x, point[0].y, point[0].z)]
+        pnt.style.color = kwargs.get('colour_hex', '7Fc0c0c0')
+        pnt.extrude = kwargs.get('extrude', 0)
+        pnt.altitudemode = kwargs.get('altitude_mode', simplekml.AltitudeMode.relativetoground)
+
+        self.kml.save(self.save_name)
+
+kml_file = KmlPlus('Point Styling.kml')
+kml_file.point(coordinates_list)   
+```
+
+### Example script
+
+```
+    kml_file = KmlPlus(file_name='Point Styling.kml')
+
+    kml_file.linestring(test_data.birmingham_cta_9, uom='FT')
+    kml_file.cylinder(test_data.beccles_parachute, 50000, upper_layer=5000)
+    kml_file.point(test_data.beccles_parachute)
+
+    kml_file.polyhedron(test_data.birmingham_cta_10, lower_layer=6500, upper_layer=10500,
+                        name='Birmingham CTA 10')
+    kml_file.polyhedron(test_data.birmingham_cta_9, lower_layer=6500, upper_layer=8500,
+                        name='Birmingham CTA 9')
+
+    kml_file.polyhedron(test_data.prestwick_cta_1, lower_layer=1500, upper_layer=5500, name='Prestwick CTA 1')
+    kml_file.polyhedron(test_data.prestwick_cta_2, lower_layer=2000, upper_layer=5500, name='Prestwick CTA 2')
+    kml_file.polyhedron(test_data.prestwick_cta_3, lower_layer=3000, upper_layer=5500, name='Prestwick CTA 3')
+    kml_file.polyhedron(test_data.prestwick_cta_4, lower_layer=3000, upper_layer=5500, name='Prestwick CTA 4')
+    kml_file.polyhedron(test_data.prestwick_cta_5, lower_layer=3500, upper_layer=5500, name='Prestwick CTA 5')
+    kml_file.polyhedron(test_data.prestwick_cta_6, lower_layer=4000, upper_layer=5500, name='Prestwick CTA 6')
+    kml_file.polyhedron(test_data.prestwick_ctr, upper_layer=5500, name='Prestwick CTR')
+    kml_file.polyhedron(test_data.test_airspace, upper_layer=50000, lower_layer=0, name='EG D406C ESKMEALS')
+```
+
+## Acknowledgements
+
+- [Simplekml](https://pypi.org/project/simplekml/) - for creating an awesome library which has helped me process_points
+  many things and also inspiring me to write this library.`
```

### Comparing `KMLPlus-3.0.0b1/README.md` & `KMLPlus-3.0.0b2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,327 +1,326 @@
-KML+
-===
-
-KML+ (KMLPlus) is library of code for Python which allows the user to easily process_points standard and 'floating'
-Polygons, Circles and Arcs.
-
----
-
-Table of Contents
------------------
-
-1. [Who is this for](#who-is-this-for)
-2. [Installing](#installing)
-3. [Usage](#usage)
-    - [Recommendations](#recommendations)
-    - [Coordinates](#coordinates)
-    - [Coordinates containing Arcs](#coordinates-containing-arcs)
-4. [Classes and functions](#classes-and-functions)
-    - [KmlPlus](#kmlplus-class)
-      - [KmlPlus (functions)](#kmlplus-functions)
-        - [linestring](#linestring)
-        - [polyhedron](#polyhedron)
-        - [circle](#circle)
-        - [cylinder](#cylinder)
-        - [point](#point)
-5. [Acknowledgements](#acknowledgements)
-
----
-
-Who is this for
----------------
-
-This is for anyone who wishes to easily render polygons, especially 'floating' or curved polygons within Google Earth.
-
-I work in the aviation industry and needed a reliable way to process_points models of our airspace. It its useful for
-creating models of airways and controlled airspace. It can be used for anything that takes your fancy!
-
-![Prestwick airspace example](img/egpk_airspace_sideon.png)
-
-![Floating polygon example](img/floating_polygon_1.jpg)
-
----
-
-Installing
-----------
-
-### Pip
-
-```
-pip install kmlplus==2.1.0  <--- last stable release
-pip install kmlplus <--- Current v3.0.0-beta.1
-```
-
-### Clone
-
-```
-git clone https://github.com/MHenderson1988/kmlplus.git
-
-# Or
-
-git clone git@github.com:MHenderson1988/kmlplus.git
-```
-
-### Running tests
-
-```
-python -m unittest
-```
-
----
-
-Usage
------
-
-### Recommendations
-
-KML+ easily integrates with the fantastic [Simplekml](https://pypi.org/project/simplekml/) library and I highly
-recommend using it in conjunction with KML+ for the best experience.
-
-#### Coordinates
-
-Coordinates should always be passed as a single or multiple strings within a list in x, y, z(optional) format. Both
-Degrees Minutes Seconds (DDMMSS.ss) and Decimal Degres (DD.dd) are accepted. DMS should be suffixed with N, W, S or E.
-Decimal degrees are suffixed using -/+ convention.
-
-While a coordinate string must be passed using the same type of coordinate, lists can contain a mixture of DMS and DD
-coordinates and will convert appropriately.
-
-If no z value is provided, defaults to 0.0.
-
-Example 
-
-```
-[
-    '553124N 0045830W',
-    '552040N 0042722W',
-    '551848N 0044702W',
-    '553124N 0045830W'
-]
-```
-
-#### Coordinates containing Arcs
-
-When creating a curved segment of a polygon, the string should be passed as follows -
-
-'start=[starting_coordinate], end=[ending_coordinate], centre=[centre_coordinate],
-direction=[clockwise/anticlockwise]'
-
-Example -
-
-```
-[
-     'start=54.32111 -3.98721, end=54.13447 -3.89329, centre=54.31667 -3.41806, direction=anticlockwise',
-     '54.13444 -3.89333',
-     '54.17417 -4.14556',
-     'start=54.17418 -4.14551, end=54.23696 -4.17352, centre=54.31667 -3.41806, direction=clockwise',
-     '54.23694 -4.17361',
-     '54.32111 -3.98722',
-]
-```
-
-### Classes and functions
-
-v3.0 has stripped back to one single class which contains functions to process_points points, circles, cylinders,
-polygons, polyhedrons and linestrings.
-
-#### KmlPlus (Class)
-
-```
-from kmlplus.kml import KmlPlus
-
-KmlPlus(self, save_name='KmlPlus', output_path=None)
-```
-
-KmlPlus is the class through which you process_points your 2D and 3D geometries.
-
-* save_name accepts a string and is used for naming the resulting .kml file.
-* output_path accepts a string representing the directory the resulting .kml shall be saved to.
-
-#### KmlPlus (functions)
-
-linestring(coordinate_list, **kwargs)
-
-The linestring function updates the kml file with a KML linestring feature.
-
-```
-from kmlplus.kml import KmlPlus
-
-"""
-
-        Args:
-            coordinate_list (list): A list containing a single coordinate
-        Keyword Args:
-            fol (str): A string to name the folder in which the point is stored.
-            linestring_name (str): String to name the LineString object
-            colour_hex (str): String representing a colour hex
-            extrude (int): 1 or 0, Whether to extrude the point
-            width(int): Line width
-            altitude_mode(str): Accepts simplekml Altitude mode options
-
-
-        Returns:
-            None
-
-  """
-
-kml_file = KmlPlus('Point Styling.kml')
-kml_file.linestring(coordinates_list)
-```
-
-polyhedron(coordinate_list, **kwargs)
-
-Updates the KmlFile with a polyhedron based upon the coordinates and optional upper and lower limits.
-
-```
-"""
-
-        Args:
-            coordinate_list (list): A list of coordinates
-        Keyword Args:
-            fol (str): A string to name the folder in which the point is stored.
-            lower_layer (float): Height in FT of the lower layer
-            upper_layer (float): Height in FT of the upper layer
-            lower_polygon_name (str): Lower polygon object name
-            upper_polygon_name (str): Upper polygon object name
-            colour_hex (str): String representing a colour hex
-            fill (str): 1 or 0, whether or not to fill the polygon
-            outline (str): 1 or 0, whether to include outline of polygon
-            extrude (str): 1 or 0, Whether to extrude the point
-            altitude_mode (str): Accepts simplekml Altitude mode options
-
-        Returns:
-            None
-        """
-        
-kml_file = KmlPlus('Point Styling.kml')
-kml_file.polyhedron(coordinates_list, lower_layer = 2000, upper_layer = 5000)
-```
-
-circle(coordinate_list, radius, **kwargs)
-
-Creates a 2D circle. Coordinate list contains a single set of coordinates in x, y, z format.
-
-```
-"""
-
-        Args:
-            coordinate_list (list): A list containing a single set of coordinates which is the centre point of the circle
-            radius (float): The radius of the circle
-        Keyword Args:
-            fol (str): Name of the folder in which the KML objects are stored.
-            name (str): What to name the Circle object
-            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
-               Defaults to 'NM'
-            colour_hex (str): String representing a colour hex
-            extrude (int): 1 or 0, Whether to extrude the point
-            altitude_mode (str): Accepts simplekml Altitude mode options
-
-        Returns:
-            None
-
-        """
-        
-kml_file = KmlPlus('Point Styling.kml')
-kml_file.circle(coordinates_list, 500)
-```
-
-cylinder(coordinate_list, radius, **kwargs)
-
-Creates a Cylinder from a single set of coordinates within a list.
-
-```
-"""
-
-        Args:
-            coordinate_list: A list containing a single set of coordinates representing the centre of the circle
-            radius: The radius of the circle
-        Keyword Args:
-            lower_layer (float): Height/Altitude of the lower layer
-            upper_layer (float): Height/Altitude of the upper layer
-            sample (int): How many points to use when creating the circles which make up the cylinder
-            lower_circle_name (str): Lower circle object name
-            upper_circle_name (str): Upper circle object name
-            fol (str): Name of the folder in which the KML objects are stored.
-            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
-              Defaults to 'NM'
-            colour_hex (str): String representing a colour hex
-            fill (str): 1 or 0, whether or not to fill the polygon
-            outline (str): 1 or 0, whether to include outline of polygon
-            altitude_mode (str): Accepts simplekml Altitude mode options
-
-        Returns:
-            None
-        """
-
-kml_file = KmlPlus('Point Styling.kml')
-kml_file.cylinder(coordinates_list, 500, lower_layer=50, upper_layer=500)   
-
-```
-
-point(coordinate_list, **kwargs)
-
-Creates a single point from a single set of coordinates stored in a list in x, y, z format.
-
-```
-
-"""
-
-        Args:
-            coordinate_list (list): A list containing a single coordinate
-
-        Keyword Args:
-            fol (str): A string to name the folder in which the point is stored.
-            point_name (str): String to name the point object
-            colour_hex (str): String representing a colour hex
-            extrude (int): 1 or 0, Whether to extrude the point
-            altitude_mode (str): Accepts simplekml Altitude mode options
-
-
-        Returns:
-            None
-
-        """
-        point = PointFactory(coordinate_list).process_coordinates()
-
-        fol = self.kml.newfolder(name=kwargs.get('fol', 'KmlPlus Point'))
-
-        pnt = fol.newpoint(name=kwargs.get('point_name', 'KmlPlus Point'))
-        pnt.coords = [(point[0].x, point[0].y, point[0].z)]
-        pnt.style.color = kwargs.get('colour_hex', '7Fc0c0c0')
-        pnt.extrude = kwargs.get('extrude', 0)
-        pnt.altitudemode = kwargs.get('altitude_mode', simplekml.AltitudeMode.relativetoground)
-
-        self.kml.save(self.save_name)
-
-kml_file = KmlPlus('Point Styling.kml')
-kml_file.point(coordinates_list)   
-```
-
-### Example script
-
-```
-    kml_file = KmlPlus(file_name='Point Styling.kml')
-
-    kml_file.linestring(test_data.birmingham_cta_9, uom='FT')
-    kml_file.cylinder(test_data.beccles_parachute, 50000, upper_layer=5000)
-    kml_file.point(test_data.beccles_parachute)
-
-    kml_file.polyhedron(test_data.birmingham_cta_10, lower_layer=6500, upper_layer=10500,
-                        name='Birmingham CTA 10')
-    kml_file.polyhedron(test_data.birmingham_cta_9, lower_layer=6500, upper_layer=8500,
-                        name='Birmingham CTA 9')
-
-    kml_file.polyhedron(test_data.prestwick_cta_1, lower_layer=1500, upper_layer=5500, name='Prestwick CTA 1')
-    kml_file.polyhedron(test_data.prestwick_cta_2, lower_layer=2000, upper_layer=5500, name='Prestwick CTA 2')
-    kml_file.polyhedron(test_data.prestwick_cta_3, lower_layer=3000, upper_layer=5500, name='Prestwick CTA 3')
-    kml_file.polyhedron(test_data.prestwick_cta_4, lower_layer=3000, upper_layer=5500, name='Prestwick CTA 4')
-    kml_file.polyhedron(test_data.prestwick_cta_5, lower_layer=3500, upper_layer=5500, name='Prestwick CTA 5')
-    kml_file.polyhedron(test_data.prestwick_cta_6, lower_layer=4000, upper_layer=5500, name='Prestwick CTA 6')
-    kml_file.polyhedron(test_data.prestwick_ctr, upper_layer=5500, name='Prestwick CTR')
-    kml_file.polyhedron(test_data.test_airspace, upper_layer=50000, lower_layer=0, name='EG D406C ESKMEALS')
-```
-
-## Acknowledgements
-
-- [Simplekml](https://pypi.org/project/simplekml/) - for creating an awesome library which has helped me process_points
-  many things and also inspiring me to write this library.`
+KML+
+===
+
+KML+ (KMLPlus) is library of code for Python which allows the user to easily process_points standard and 'floating'
+Polygons, Circles and Arcs.
+
+---
+
+Table of Contents
+-----------------
+
+1. [Who is this for](#who-is-this-for)
+2. [Installing](#installing)
+3. [Usage](#usage)
+    - [Recommendations](#recommendations)
+    - [Coordinates](#coordinates)
+    - [Coordinates containing Arcs](#coordinates-containing-arcs)
+4. [Classes and functions](#classes-and-functions)
+    - [KmlPlus](#kmlplus-class)
+        - [KmlPlus (functions)](#kmlplus-functions)
+            - [linestring](#linestring)
+            - [polyhedron](#polyhedron)
+            - [circle](#circle)
+            - [cylinder](#cylinder)
+            - [point](#point)
+5. [Acknowledgements](#acknowledgements)
+
+---
+
+Who is this for
+---------------
+
+This is for anyone who wishes to easily render polygons, especially 'floating' or curved polygons within Google Earth.
+
+I work in the aviation industry and needed a reliable way to process_points models of our airspace. It its useful for
+creating models of airways and controlled airspace. It can be used for anything that takes your fancy!
+
+![Prestwick airspace example](img/egpk_airspace_sideon.png)
+
+![Floating polygon example](img/floating_polygon_1.jpg)
+
+---
+
+Installing
+----------
+
+### Pip
+
+```
+pip install kmlplus==2.1.0  <--- last stable release
+pip install kmlplus==3.0.0b1 <--- Current v3.0.0-beta.1
+```
+
+### Clone
+
+```
+git clone https://github.com/MHenderson1988/kmlplus.git
+
+# Or
+
+git clone git@github.com:MHenderson1988/kmlplus.git
+```
+
+### Running tests
+
+```
+python -m unittest
+```
+
+---
+
+Usage v3
+-----
+
+### Recommendations
+
+KML+ easily integrates with the fantastic [Simplekml](https://pypi.org/project/simplekml/) library and I highly
+recommend using it in conjunction with KML+ for the best experience.
+
+#### Coordinates
+
+Coordinates should always be passed as a single or multiple strings within a list in x, y, z(optional) format. Both
+Degrees Minutes Seconds (DDMMSS.ss) and Decimal Degres (DD.dd) are accepted. DMS should be suffixed with N, W, S or E.
+Decimal degrees are suffixed using -/+ convention.
+
+While a coordinate string must be passed using the same type of coordinate, lists can contain a mixture of DMS and DD
+coordinates and will convert appropriately.
+
+If no z value is provided, defaults to 0.0.
+
+Example
+
+```
+[
+    '553124N 0045830W',
+    '552040N 0042722W',
+    '551848N 0044702W',
+    '553124N 0045830W'
+]
+```
+
+#### Coordinates containing Arcs
+
+When creating a curved segment of a polygon, the string should be passed as follows -
+
+'start=[starting_coordinate], end=[ending_coordinate], centre=[centre_coordinate], direction=[clockwise/anticlockwise]'
+
+Example -
+
+```
+[
+     'start=54.32111 -3.98721, end=54.13447 -3.89329, centre=54.31667 -3.41806, direction=anticlockwise',
+     '54.13444 -3.89333',
+     '54.17417 -4.14556',
+     'start=54.17418 -4.14551, end=54.23696 -4.17352, centre=54.31667 -3.41806, direction=clockwise',
+     '54.23694 -4.17361',
+     '54.32111 -3.98722',
+]
+```
+
+### Classes and functions
+
+v3.0 has stripped back to one single class which contains functions to process_points points, circles, cylinders,
+polygons, polyhedrons and linestrings.
+
+#### KmlPlus (Class)
+
+```
+from kmlplus.kml import KmlPlus
+
+KmlPlus(self, save_name='KmlPlus', output_path=None)
+```
+
+KmlPlus is the class through which you process_points your 2D and 3D geometries.
+
+* save_name accepts a string and is used for naming the resulting .kml file.
+* output_path accepts a string representing the directory the resulting .kml shall be saved to.
+
+#### KmlPlus (functions)
+
+linestring(coordinate_list, **kwargs)
+
+The linestring function updates the kml file with a KML linestring feature.
+
+```
+from kmlplus.kml import KmlPlus
+
+"""
+
+        Args:
+            coordinate_list (list): A list containing a single coordinate
+        Keyword Args:
+            fol (str): A string to name the folder in which the point is stored.
+            linestring_name (str): String to name the LineString object
+            colour_hex (str): String representing a colour hex
+            extrude (int): 1 or 0, Whether to extrude the point
+            width(int): Line width
+            altitude_mode(str): Accepts simplekml Altitude mode options
+
+
+        Returns:
+            None
+
+  """
+
+kml_file = KmlPlus('Point Styling.kml')
+kml_file.linestring(coordinates_list)
+```
+
+polyhedron(coordinate_list, **kwargs)
+
+Updates the KmlFile with a polyhedron based upon the coordinates and optional upper and lower limits.
+
+```
+"""
+
+        Args:
+            coordinate_list (list): A list of coordinates
+        Keyword Args:
+            fol (str): A string to name the folder in which the point is stored.
+            lower_layer (float): Height in FT of the lower layer
+            upper_layer (float): Height in FT of the upper layer
+            lower_polygon_name (str): Lower polygon object name
+            upper_polygon_name (str): Upper polygon object name
+            colour_hex (str): String representing a colour hex
+            fill (str): 1 or 0, whether or not to fill the polygon
+            outline (str): 1 or 0, whether to include outline of polygon
+            extrude (str): 1 or 0, Whether to extrude the point
+            altitude_mode (str): Accepts simplekml Altitude mode options
+
+        Returns:
+            None
+        """
+        
+kml_file = KmlPlus('Point Styling.kml')
+kml_file.polyhedron(coordinates_list, lower_layer = 2000, upper_layer = 5000)
+```
+
+circle(coordinate_list, radius, **kwargs)
+
+Creates a 2D circle. Coordinate list contains a single set of coordinates in x, y, z format.
+
+```
+"""
+
+        Args:
+            coordinate_list (list): A list containing a single set of coordinates which is the centre point of the circle
+            radius (float): The radius of the circle
+        Keyword Args:
+            fol (str): Name of the folder in which the KML objects are stored.
+            name (str): What to name the Circle object
+            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
+               Defaults to 'NM'
+            colour_hex (str): String representing a colour hex
+            extrude (int): 1 or 0, Whether to extrude the point
+            altitude_mode (str): Accepts simplekml Altitude mode options
+
+        Returns:
+            None
+
+        """
+        
+kml_file = KmlPlus('Point Styling.kml')
+kml_file.circle(coordinates_list, 500)
+```
+
+cylinder(coordinate_list, radius, **kwargs)
+
+Creates a Cylinder from a single set of coordinates within a list.
+
+```
+"""
+
+        Args:
+            coordinate_list: A list containing a single set of coordinates representing the centre of the circle
+            radius: The radius of the circle
+        Keyword Args:
+            lower_layer (float): Height/Altitude of the lower layer
+            upper_layer (float): Height/Altitude of the upper layer
+            sample (int): How many points to use when creating the circles which make up the cylinder
+            lower_circle_name (str): Lower circle object name
+            upper_circle_name (str): Upper circle object name
+            fol (str): Name of the folder in which the KML objects are stored.
+            uom (str): The unit of measurement of the radius. Accepted arguments are 'FT', 'NM', 'MI', 'KM' and 'M'.
+              Defaults to 'NM'
+            colour_hex (str): String representing a colour hex
+            fill (str): 1 or 0, whether or not to fill the polygon
+            outline (str): 1 or 0, whether to include outline of polygon
+            altitude_mode (str): Accepts simplekml Altitude mode options
+
+        Returns:
+            None
+        """
+
+kml_file = KmlPlus('Point Styling.kml')
+kml_file.cylinder(coordinates_list, 500, lower_layer=50, upper_layer=500)   
+
+```
+
+point(coordinate_list, **kwargs)
+
+Creates a single point from a single set of coordinates stored in a list in x, y, z format.
+
+```
+
+"""
+
+        Args:
+            coordinate_list (list): A list containing a single coordinate
+
+        Keyword Args:
+            fol (str): A string to name the folder in which the point is stored.
+            point_name (str): String to name the point object
+            colour_hex (str): String representing a colour hex
+            extrude (int): 1 or 0, Whether to extrude the point
+            altitude_mode (str): Accepts simplekml Altitude mode options
+
+
+        Returns:
+            None
+
+        """
+        point = PointFactory(coordinate_list).process_coordinates()
+
+        fol = self.kml.newfolder(name=kwargs.get('fol', 'KmlPlus Point'))
+
+        pnt = fol.newpoint(name=kwargs.get('point_name', 'KmlPlus Point'))
+        pnt.coords = [(point[0].x, point[0].y, point[0].z)]
+        pnt.style.color = kwargs.get('colour_hex', '7Fc0c0c0')
+        pnt.extrude = kwargs.get('extrude', 0)
+        pnt.altitudemode = kwargs.get('altitude_mode', simplekml.AltitudeMode.relativetoground)
+
+        self.kml.save(self.save_name)
+
+kml_file = KmlPlus('Point Styling.kml')
+kml_file.point(coordinates_list)   
+```
+
+### Example script
+
+```
+    kml_file = KmlPlus(file_name='Point Styling.kml')
+
+    kml_file.linestring(test_data.birmingham_cta_9, uom='FT')
+    kml_file.cylinder(test_data.beccles_parachute, 50000, upper_layer=5000)
+    kml_file.point(test_data.beccles_parachute)
+
+    kml_file.polyhedron(test_data.birmingham_cta_10, lower_layer=6500, upper_layer=10500,
+                        name='Birmingham CTA 10')
+    kml_file.polyhedron(test_data.birmingham_cta_9, lower_layer=6500, upper_layer=8500,
+                        name='Birmingham CTA 9')
+
+    kml_file.polyhedron(test_data.prestwick_cta_1, lower_layer=1500, upper_layer=5500, name='Prestwick CTA 1')
+    kml_file.polyhedron(test_data.prestwick_cta_2, lower_layer=2000, upper_layer=5500, name='Prestwick CTA 2')
+    kml_file.polyhedron(test_data.prestwick_cta_3, lower_layer=3000, upper_layer=5500, name='Prestwick CTA 3')
+    kml_file.polyhedron(test_data.prestwick_cta_4, lower_layer=3000, upper_layer=5500, name='Prestwick CTA 4')
+    kml_file.polyhedron(test_data.prestwick_cta_5, lower_layer=3500, upper_layer=5500, name='Prestwick CTA 5')
+    kml_file.polyhedron(test_data.prestwick_cta_6, lower_layer=4000, upper_layer=5500, name='Prestwick CTA 6')
+    kml_file.polyhedron(test_data.prestwick_ctr, upper_layer=5500, name='Prestwick CTR')
+    kml_file.polyhedron(test_data.test_airspace, upper_layer=50000, lower_layer=0, name='EG D406C ESKMEALS')
+```
+
+## Acknowledgements
+
+- [Simplekml](https://pypi.org/project/simplekml/) - for creating an awesome library which has helped me process_points
+  many things and also inspiring me to write this library.`
```

### Comparing `KMLPlus-3.0.0b1/kmlplus/shapes.py` & `KMLPlus-3.0.0b2/kmlplus/shapes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,611 +1,612 @@
-from typing import Union
-
-from kmlplus.geo import PointFactory, Point
-from kmlplus.interface import ICircle, ILocation, I3DObject, IPolygon, ICylinder, I2DObject
-
-
-class Circle(ICircle, I2DObject):
-    """
-    Plots the coordinates for a 2D circular object.
-
-    Args:
-        centre (str): A string representing the central coordinate (focus) of the circle.
-        radius (float): The radius of the circle to be draw
-
-    Keyword Args:
-        radius_uom (str): Unit of measure for the radius. Accepts and defaults to metres ('M'), statute miles ('MI'),
-         kilometres ('KM') and nautical miles ('NM')
-        uom (str): Unit of measure for elevation. Accepts and defaults to feet ('FT') and metres ('M')
-    """
-
-    def __init__(self, centre: list, radius: float, **kwargs):
-        self.radius_uom: str = kwargs.get('radius_uom', 'M')
-        self.uom: str = kwargs.get('uom', 'FT')
-        self.z: float = kwargs.get('z', None)
-        self.sample: int = kwargs.get('sample', 100)
-        self.centre: ILocation = self.plot_centre(centre)
-        self.radius: float = radius
-        self.point_list: list[ILocation] = self.process_points()
-
-    def __eq__(self, another_circle: ICircle) -> bool:
-        if self.centre and self.radius == another_circle.centre and another_circle.radius:
-            return True
-        else:
-            return False
-
-    def __len__(self) -> int:
-        return len(self.point_list)
-
-    def __iter__(self):
-        self.n = 0
-        return self
-
-    def __next__(self):
-        if self.n < len(self.point_list):
-            result = self.point_list[self.n]
-            self.n += 1
-            return result
-        else:
-            raise StopIteration
-
-    def __getitem__(self, index):
-        return self.point_list[index]
-
-    def __setitem__(self, index, point) -> None:
-        if isinstance(point, Point):
-            self.point_list[index] = point
-        else:
-            raise TypeError('Polygon will only accept objects of type kmlplus.geo.Point')
-
-    @property
-    def z(self) -> float:
-        return self._z
-
-    @z.setter
-    def z(self, value):
-        if not value:
-            self._z = None
-        elif isinstance(value, float):
-            conversion_dict = {'FT': 0.3048, 'M': 1}
-            self._z = value * conversion_dict[self.uom]
-        else:
-            self.z = float(value)
-
-    @property
-    def sample(self) -> int:
-        return self._sample
-
-    @sample.setter
-    def sample(self, value: int) -> None:
-        if isinstance(value, int):
-            self._sample = value
-        else:
-            self._sample = int(value)
-
-    @property
-    def centre(self) -> ILocation:
-        return self._centre
-
-    @centre.setter
-    def centre(self, a_point: ILocation):
-        if isinstance(a_point, Point):
-            self._centre = a_point
-        else:
-            raise TypeError('Centre must be passed a kmlplus.geo.Point object.')
-
-    @property
-    def radius(self) -> float:
-        return self._radius
-
-    @radius.setter
-    def radius(self, a_radius: Union[float, int, str]):
-        if a_radius > 0 and isinstance(a_radius, float):
-            self._radius = a_radius
-        elif a_radius > 0:
-            try:
-                converted_radius = float(a_radius)
-                self._radius = converted_radius
-            except TypeError:
-                print('Radius must be a float or type which can be converted to float eg int or string.')
-        else:
-            raise ValueError(
-                'Radius must be greater than 0 and of type float or other type which can be cast to float.')
-
-    def plot_centre(self, central_location: list[str]) -> ILocation:
-        """
-        Takes the list passed at construction and creates an ILocation object to represent it
-
-        Args:
-            central_location (list): List with a single string representing x, y, z coordinate
-
-        Returns:
-            coordinates(ILocation): ILocation object representing the focus of the circle.
-        """
-        coordinates = PointFactory(central_location, uom=self.uom).process_coordinates()[0]
-        return coordinates
-
-    def process_points(self) -> list[ILocation]:
-        """
-        Plots and creates each ILocation point of the circle.
-
-        Returns:
-            point_list (list[ILocation]): List of ILocation objects which form the circle.
-        """
-        point_list = []
-
-        start_bearing = 0
-        bearing_increment = 360 / self.sample
-
-        for n in range(0, self.sample + 1):
-            if self.z:
-                z = self.z
-            else:
-                z = self.centre.z
-
-            point = Point.from_point_bearing_and_distance(self.centre, start_bearing, self.radius, z=z,
-                                                          uom=self.uom, radius_uom=self.radius_uom)
-            point_list.append(point)
-            start_bearing -= bearing_increment
-
-        return point_list
-
-    def to_kml(self) -> list[tuple]:
-        """
-        Processes ILocation objects to give kml formatted string output
-
-        Returns:
-            circle (list[tuple]): A list of tuples containing x, y, z coordinate strings.
-        """
-        point_list = []
-
-        start_bearing = 0
-        bearing_increment = 360 / self.sample
-
-        for n in range(0, self.sample + 1):
-            point = Point.from_point_bearing_and_distance(self.centre, start_bearing, self.radius, z=self.z)
-            point_list.append(point)
-            start_bearing -= bearing_increment
-
-        # kml tuples
-        circle = [(p.x, p.y, p.z) for p in point_list]
-
-        return circle
-
-
-class Cylinder(I3DObject, ICylinder):
-    """
-    Represents a 3D cylindrical object. Top and bottom layers are made up of 2x Circle objects of equal sample size.
-
-    Args:
-        lower_coordinates (list[str]): List of string representations of coordinates.
-        upper_coordinates (list[str]): List of string representations of coordinates
-
-    Keyword Args:
-        radius_uom (str): Unit of measure for the radius. Accepts and defaults to metres ('M'), statute miles ('MI'),
-         kilometres ('KM') and nautical miles ('NM')
-        uom (str): Unit of measure for elevation. Accepts and defaults to feet ('FT') and metres ('M')
-        lower_radius (float): Overrides any radius in the string for the lower circle.
-        upper_radius (float): Overrides any radius in the string for the upper circle.
-
-    """
-
-    def __init__(self, lower_coordinates: list, upper_coordinates: list, **kwargs):
-        self.uom = kwargs.get('uom', 'FT')
-        self.sample = kwargs.get('sample', 100)
-        self.radius_uom = kwargs.get('radius_uom', 'M')
-        self.lower_radius = lower_coordinates[1]
-        self.upper_radius = upper_coordinates[1]
-        self.lower_layer = self.create_layer(
-            (lower_coordinates[0], self.lower_radius),
-            kwargs.get('lower_layer', None)
-        )
-        self._upper_layer = self.create_layer(
-            (upper_coordinates[0], self.upper_radius),
-            kwargs.get('upper_layer', None)
-        )
-        self._sides = self.generate_sides()
-
-    @property
-    def lower_radius(self) -> float:
-        return self._lower_radius
-
-    @lower_radius.setter
-    def lower_radius(self, value: float):
-        if isinstance(value, (int, float)):
-            self._lower_radius = value
-        else:
-            try:
-                value = float(value)
-                self.lower_radius = value
-            except TypeError:
-                print('Radius must be given as float, int or a castable type.')
-
-    @property
-    def upper_radius(self) -> float:
-        return self._upper_radius
-
-    @upper_radius.setter
-    def upper_radius(self, value: float):
-        if isinstance(value, (int, float)):
-            self._upper_radius = value
-        else:
-            try:
-                value = float(value)
-                self.upper_radius = value
-            except TypeError:
-                print('Radius must be given as float, int or a castable type.')
-
-    @property
-    def sides(self) -> list:
-        return self._sides
-
-    @sides.setter
-    def sides(self, sides: list):
-        if isinstance(sides, list):
-            self._sides = sides
-        else:
-            raise TypeError('Sides can only be passed in a list')
-
-    @property
-    def lower_layer(self) -> ICircle:
-        return self._lower_layer
-
-    @lower_layer.setter
-    def lower_layer(self, circle: ICircle):
-        if isinstance(circle, ICircle):
-            self._lower_layer = circle
-        else:
-            raise TypeError('Cylinder layers must be type ICircle')
-
-    @property
-    def upper_layer(self) -> ICircle:
-        return self._upper_layer
-
-    @upper_layer.setter
-    def upper_layer(self, circle: ICircle):
-        if isinstance(circle, ICircle):
-            self._upper_layer = circle
-        else:
-            raise TypeError('Cylinder layers must be type ICircle')
-
-    def to_kml(self) -> Union[tuple[list, list, list]]:
-        """
-        Returns kml formatted coordinates in a list for the lower layer, upper layer and sides.
-        Returns:
-            lower, upper, sides (tuple[list, list, list]): Lists of kml formatted tuples.
-
-        """
-        lower = [(p.x, p.y, p.z) for p in self.lower_layer]
-        upper = [(p.x, p.y, p.z) for p in self.upper_layer]
-        sides = []
-
-        for polygon in self.sides:
-            holding_list = []
-            for point_list in polygon:
-                holding_list.append((point_list.x, point_list.y, point_list.z))
-            sides.append(holding_list)
-
-        return lower, upper, sides
-
-    def create_layer(self, coordinate_list: tuple[list[str, float, int]], layer_height) -> ICircle:
-        """
-        Creates a 2D circle to act as the top or bottom layer of the cylinder
-        Args:
-            coordinate_list (tuple[list[str, float, int]]): Contains string information for coordinate and radius
-            layer_height: The z value of the layer
-
-        Returns:
-            circle (ICircle): A circle object
-        """
-        if layer_height:
-            circle = Circle(coordinate_list[0], coordinate_list[1], z=layer_height, uom=self.uom,
-                            radius_uom=self.radius_uom)
-        else:
-            circle = Circle(coordinate_list[0], coordinate_list[1], uom=self.uom, radius_uom=self.radius_uom)
-        return circle
-
-    def generate_sides(self) -> list[IPolygon]:
-        """
-        Creates the sides of the cylinder. Requires both layers to contain the same amount of points.
-
-        Returns:
-            side_coordinates (list[IPolygon]): A list of polygons joining the upper and lower layers together.
-
-        Raises:
-            IndexError: If lower layer and upper layer do not have the same quantity of points.
-        """
-        if len(self.lower_layer) != len(self.upper_layer):
-            raise IndexError(f'Lower and upper polygon must contain the same amount of points.  Point count - lower'
-                             f'polygon: {len(self.lower_layer)} upper polygon: {len(self.upper_layer)}')
-        else:
-            side_coordinates = []
-            i = 0
-            while i < len(self.lower_layer) - 1:
-                polygon_coordinate_list = [self.lower_layer.point_list[i].__str__(), self.lower_layer[i + 1].__str__(),
-                                           self.upper_layer[i + 1].__str__(), self.upper_layer[i].__str__(),
-                                           self.lower_layer[i].__str__()]
-
-                side_coordinates.append(Polygon(polygon_coordinate_list, uom=self.uom))
-
-                i += 1
-
-            return side_coordinates
-
-
-class Polygon(IPolygon, I2DObject):
-    """
-    Creates a polygon made of 2 or more vertices
-
-    Args:
-        coordinate_list (list[str]): A list of strings representing coordinates of vertices.
-
-    Keyword Args:
-        uom (str): Unit of measure for elevation, FT or M
-        z (float): Override all string elevation values with a single blanket value.
-    """
-
-    def __init__(self, coordinate_list: list, **kwargs: str):
-        self.uom = kwargs.get('uom', 'FT')
-        self.z = kwargs.get('z', None)
-        self.point_list = self.process_points(coordinate_list)
-        self.centroid = self.calculate_centroid()
-
-    def __len__(self) -> int:
-        return len(self.point_list)
-
-    def __iter__(self):
-        self.n = 0
-        return self
-
-    def __next__(self):
-        if self.n < len(self.point_list):
-            result = self.point_list[self.n]
-            self.n += 1
-            return result
-        else:
-            raise StopIteration
-
-    def __getitem__(self, index):
-        return self.point_list[index]
-
-    def __setitem__(self, index, point):
-        if isinstance(point, Point):
-            self.point_list[index] = point
-        else:
-            raise TypeError('Polygon will only accept objects of type kmlplus.geo.Point')
-
-    def __eq__(self, another_2D_object: I2DObject) -> bool:
-        return self.__len__() != another_2D_object.__len__()
-
-    @property
-    def z(self):
-        return self._z
-
-    @z.setter
-    def z(self, value):
-        if not value:
-            self._z = None
-        elif isinstance(value, float):
-            conversion_dict = {'FT': 0.3048, 'M': 1}
-            self._z = value * conversion_dict[self.uom]
-        else:
-            self.z = float(value)
-
-    @property
-    def point_list(self):
-        return self._point_list
-
-    @point_list.setter
-    def point_list(self, a_point_list: list):
-        if len(a_point_list) > 2 and isinstance(a_point_list, list):
-            # Close the polygon, if it is not already
-            if a_point_list[0] != a_point_list[-1]:
-                first_vertice = a_point_list[0]
-                a_point_list.append(first_vertice)
-            self._point_list = a_point_list
-        else:
-            raise ValueError('Cannot process_points a polygon from less than 2 points')
-
-    def calculate_centroid(self) -> ILocation:
-        """
-        Calculates the centre (centroid) of the polygon's area. This is used for sorting the polygons so that they are
-        drawn correctly in Google Earth.
-
-        Returns:
-            point (ILocation)
-        """
-        latitude_total, longitude_total = 0, 0
-        for coordinate_instance in self.point_list:
-            latitude_total += coordinate_instance.y
-            longitude_total += coordinate_instance.x
-        latitude_average, longitude_average = latitude_total / len(self.point_list), \
-                                              longitude_total / len(self.point_list)
-
-        point = Point(latitude_average, longitude_average)
-        return point
-
-    def calculate_bearing_from_centroid(self, point: ILocation) -> ILocation:
-        """
-        Calculates the bearing to the point from the centre of the polygon (Centroid)
-
-        Args:
-            point (ILocation): The point to find the bearing to
-
-        Returns:
-            bearing (float): The bearing in degrees
-
-        """
-        bearing = point.get_bearing(self.centroid)
-        return bearing
-
-    def process_points(self, point_list: list[str]) -> list[ILocation]:
-        """
-        Creates ILocation objects from the list of coordinates supplied.
-        Args:
-            point_list (list[str]): A list of coordinate information in string format
-
-        Returns:
-            points (list[ILocation]): A list of ILocation objects representing the vertices of the polygon
-        """
-        points = PointFactory(
-            point_list,
-            z=self._z,
-            uom=self.uom
-        ).process_coordinates()
-
-        return points
-
-
-class Polyhedron(I3DObject):
-    """
-    A Polyhedron (3D object) comprised of a lower layer, upper layer and sides.
-
-    Args:
-        lower_coordinates (list[str]): A list of str representation of coordinates.
-        upper_coordinates (list[str]): A list of str representation of coordinates.
-
-    Keyword Args:
-        uom = Unit of measure for elevation, FT or M
-    """
-
-    def __init__(self, lower_coordinates: list[str], upper_coordinates: list[str], **kwargs: str):
-        self.uom = kwargs.get('uom', 'FT')
-        self.lower_layer = self.create_layer(lower_coordinates, kwargs.get('lower_layer', None))
-        self.upper_layer = self.create_layer(upper_coordinates, kwargs.get('upper_layer', None))
-        self.sides = self.generate_sides()
-
-    @property
-    def lower_layer(self) -> I2DObject:
-        return self._lower_layer
-
-    @lower_layer.setter
-    def lower_layer(self, a_polygon: I2DObject):
-        if isinstance(a_polygon, I2DObject):
-            self._lower_layer = a_polygon
-        else:
-            raise TypeError('Lower layer must be a type of I2DObject')
-
-    @property
-    def upper_layer(self):
-        return self._upper_layer
-
-    @upper_layer.setter
-    def upper_layer(self, a_polygon):
-        self._upper_layer = a_polygon
-
-    @property
-    def sides(self):
-        return self._sides
-
-    @sides.setter
-    def sides(self, sides: list):
-        if isinstance(sides, list):
-            self._sides = sides
-        else:
-            raise TypeError('Sides can only be passed in a list')
-
-    def to_kml(self) -> tuple:
-        """
-        Processes the upper, lower layers and sides. Converts their data to a KML friendly format.
-
-        Returns:
-            lower, upper, sides (tuple):
-        """
-        lower = [(p.x, p.y, p.z) for p in self.lower_layer]
-        upper = [(p.x, p.y, p.z) for p in self.upper_layer]
-        sides = []
-
-        for polygon in self.sides:
-            holding_list = []
-            for point_list in polygon:
-                holding_list.append((point_list.x, point_list.y, point_list.z))
-            sides.append(holding_list)
-
-        return lower, upper, sides
-
-    def create_layer(self, coordinate_list: list[str], layer_height: str) -> IPolygon:
-        """
-        Creates a layer for the polygon
-        Args:
-            coordinate_list (list): List containing a string of coordinate information
-            layer_height (str): The elevation value of the layer
-
-        Returns:
-
-        """
-        if layer_height:
-            poly = Polygon(coordinate_list, z=layer_height, uom=self.uom)
-        else:
-            poly = Polygon(coordinate_list)
-        return poly
-
-    def generate_sides(self) -> list[IPolygon]:
-        """
-        Creates the side polygons to connect the upper and lower layers. Requires upper and lower layers to have
-        matching amount of vertices
-
-        Returns:
-            side_coordinates (list[IPolygon]): List of polygons which make up the sides of the polyhedron.
-        """
-        if len(self.lower_layer) != len(self.upper_layer):
-            raise IndexError(f'Lower and upper polygon must contain the same amount of points.  Point count - lower '
-                             f'polygon: {len(self.lower_layer)} upper polygon: {len(self.upper_layer)}')
-        else:
-            side_coordinates = []
-            i = 0
-            while i < len(self.lower_layer) - 1:
-                polygon_coordinate_list = [self.lower_layer[i].__str__(), self.lower_layer[i + 1].__str__(),
-                                           self.upper_layer[i + 1].__str__(), self.upper_layer[i].__str__(),
-                                           self.lower_layer[i].__str__()]
-
-                side_polygon = Polygon(polygon_coordinate_list, uom=self.uom)
-
-                side_coordinates.append(side_polygon)
-
-                i += 1
-
-            return side_coordinates
-
-
-class LineString(I2DObject):
-    """
-    Represents a kml LineString.
-
-    Args:
-        coordinate_list (list[str]): A list containing two or more strings representing coordinates
-
-    Keyword Args:
-        uom (str): Unit of measure for elevation, FT or M.
-    """
-
-    def __init__(self, coordinate_list, **kwargs):
-        self.uom = kwargs.get('uom', 'FT')
-        self.point_list = self.create(coordinate_list)
-
-    def __len__(self):
-        return len(self.point_list)
-
-    def __iter__(self):
-        self.n = 0
-        return self
-
-    def __next__(self):
-        if self.n < len(self.point_list):
-            result = self.point_list[self.n]
-            self.n += 1
-            return result
-        else:
-            raise StopIteration
-
-    def __getitem__(self, index):
-        return self.point_list[index]
-
-    def __setitem__(self, index, point):
-        if isinstance(point, Point):
-            self.point_list[index] = point
-        else:
-            raise TypeError('Polygon will only accept objects of type kmlplus.geo.Point')
-
-    def create(self, coordinate_list: list[str]) -> list[ILocation]:
-        point_list = PointFactory(coordinate_list, uom=self.uom).process_coordinates()
-        return point_list
+from typing import Union
+
+from kmlplus.geo import PointFactory, Point
+from kmlplus.interface import ICircle, ILocation, I3DObject, IPolygon, ICylinder, I2DObject
+
+
+class Circle(ICircle, I2DObject):
+    """
+    Plots the coordinates for a 2D circular object.
+
+    Args:
+        centre (str): A string representing the central coordinate (focus) of the circle.
+        radius (float): The radius of the circle to be draw
+
+    Keyword Args:
+        radius_uom (str): Unit of measure for the radius. Accepts and defaults to metres ('M'), statute miles ('MI'),
+         kilometres ('KM') and nautical miles ('NM')
+        uom (str): Unit of measure for elevation. Accepts and defaults to feet ('FT') and metres ('M')
+    """
+
+    def __init__(self, centre: list, radius: float, **kwargs):
+        self.radius_uom: str = kwargs.get('radius_uom', 'M')
+        self.uom: str = kwargs.get('uom', 'FT')
+        self.z: float = kwargs.get('z', None)
+        self.sample: int = kwargs.get('sample', 100)
+        self.centre: ILocation = self.plot_centre(centre)
+        self.radius: float = radius
+        self.point_list: list[ILocation] = self.process_points()
+
+    def __eq__(self, another_circle: ICircle) -> bool:
+        if self.centre and self.radius == another_circle.centre and another_circle.radius:
+            return True
+        else:
+            return False
+
+    def __len__(self) -> int:
+        return len(self.point_list)
+
+    def __iter__(self):
+        self.n = 0
+        return self
+
+    def __next__(self):
+        if self.n < len(self.point_list):
+            result = self.point_list[self.n]
+            self.n += 1
+            return result
+        else:
+            raise StopIteration
+
+    def __getitem__(self, index):
+        return self.point_list[index]
+
+    def __setitem__(self, index, point) -> None:
+        if isinstance(point, Point):
+            self.point_list[index] = point
+        else:
+            raise TypeError('Polygon will only accept objects of type kmlplus.geo.Point')
+
+    @property
+    def z(self) -> float:
+        return self._z
+
+    @z.setter
+    def z(self, value):
+        if not value:
+            self._z = None
+        elif isinstance(value, float):
+            conversion_dict = {'FT': 0.3048, 'M': 1}
+            self._z = value * conversion_dict[self.uom]
+        else:
+            self.z = float(value)
+
+    @property
+    def sample(self) -> int:
+        return self._sample
+
+    @sample.setter
+    def sample(self, value: int) -> None:
+        if isinstance(value, int):
+            self._sample = value
+        else:
+            self._sample = int(value)
+
+    @property
+    def centre(self) -> ILocation:
+        return self._centre
+
+    @centre.setter
+    def centre(self, a_point: ILocation):
+        if isinstance(a_point, Point):
+            self._centre = a_point
+        else:
+            raise TypeError('Centre must be passed a kmlplus.geo.Point object.')
+
+    @property
+    def radius(self) -> float:
+        return self._radius
+
+    @radius.setter
+    def radius(self, a_radius: Union[float, int, str]):
+        if a_radius > 0 and isinstance(a_radius, float):
+            self._radius = a_radius
+        elif a_radius > 0:
+            try:
+                converted_radius = float(a_radius)
+                self._radius = converted_radius
+            except TypeError:
+                print('Radius must be a float or type which can be converted to float eg int or string.')
+        else:
+            raise ValueError(
+                'Radius must be greater than 0 and of type float or other type which can be cast to float.')
+
+    def plot_centre(self, central_location: list[str]) -> ILocation:
+        """
+        Takes the list passed at construction and creates an ILocation object to represent it
+
+        Args:
+            central_location (list): List with a single string representing x, y, z coordinate
+
+        Returns:
+            coordinates(ILocation): ILocation object representing the focus of the circle.
+        """
+        coordinates = PointFactory(central_location, uom=self.uom).process_coordinates()[0]
+        return coordinates
+
+    def process_points(self) -> list[ILocation]:
+        """
+        Plots and creates each ILocation point of the circle.
+
+        Returns:
+            point_list (list[ILocation]): List of ILocation objects which form the circle.
+        """
+        point_list = []
+
+        start_bearing = 0
+        bearing_increment = 360 / self.sample
+
+        for n in range(0, self.sample + 1):
+            if self.z:
+                z = self.z
+            else:
+                z = self.centre.z
+
+            point = Point.from_point_bearing_and_distance(self.centre, start_bearing, self.radius, z=z,
+                                                          uom=self.uom, radius_uom=self.radius_uom)
+            point_list.append(point)
+            start_bearing -= bearing_increment
+
+        return point_list
+
+    def to_kml(self) -> list[tuple]:
+        """
+        Processes ILocation objects to give kml formatted string output
+
+        Returns:
+            circle (list[tuple]): A list of tuples containing x, y, z coordinate strings.
+        """
+        point_list = []
+
+        start_bearing = 0
+        bearing_increment = 360 / self.sample
+
+        for n in range(0, self.sample + 1):
+            point = Point.from_point_bearing_and_distance(self.centre, start_bearing, self.radius, z=self.z)
+            point_list.append(point)
+            start_bearing -= bearing_increment
+
+        # kml tuples
+        circle = [(p.x, p.y, p.z) for p in point_list]
+
+        return circle
+
+
+class Cylinder(I3DObject, ICylinder):
+    """
+    Represents a 3D cylindrical object. Top and bottom layers are made up of 2x Circle objects of equal sample size.
+
+    Args:
+        lower_coordinates (list[str]): List of string representations of coordinates.
+        upper_coordinates (list[str]): List of string representations of coordinates
+
+    Keyword Args:
+        radius_uom (str): Unit of measure for the radius. Accepts and defaults to metres ('M'), statute miles ('MI'),
+         kilometres ('KM') and nautical miles ('NM')
+        uom (str): Unit of measure for elevation. Accepts and defaults to feet ('FT') and metres ('M')
+        lower_radius (float): Overrides any radius in the string for the lower circle.
+        upper_radius (float): Overrides any radius in the string for the upper circle.
+
+    """
+
+    def __init__(self, lower_coordinates: list, upper_coordinates: list, **kwargs):
+        self.uom = kwargs.get('uom', 'FT')
+        self.sample = kwargs.get('sample', 100)
+        self.radius_uom = kwargs.get('radius_uom', 'M')
+        self.lower_radius = lower_coordinates[1]
+        self.upper_radius = upper_coordinates[1]
+        self.lower_layer = self.create_layer(
+            (lower_coordinates[0], self.lower_radius),
+            kwargs.get('lower_layer', None)
+        )
+        self._upper_layer = self.create_layer(
+            (upper_coordinates[0], self.upper_radius),
+            kwargs.get('upper_layer', None)
+        )
+        self._sides = self.generate_sides()
+
+    @property
+    def lower_radius(self) -> float:
+        return self._lower_radius
+
+    @lower_radius.setter
+    def lower_radius(self, value: float):
+        if isinstance(value, (int, float)):
+            self._lower_radius = value
+        else:
+            try:
+                value = float(value)
+                self.lower_radius = value
+            except TypeError:
+                print('Radius must be given as float, int or a castable type.')
+
+    @property
+    def upper_radius(self) -> float:
+        return self._upper_radius
+
+    @upper_radius.setter
+    def upper_radius(self, value: float):
+        if isinstance(value, (int, float)):
+            self._upper_radius = value
+        else:
+            try:
+                value = float(value)
+                self.upper_radius = value
+            except TypeError:
+                print('Radius must be given as float, int or a castable type.')
+
+    @property
+    def sides(self) -> list:
+        return self._sides
+
+    @sides.setter
+    def sides(self, sides: list):
+        if isinstance(sides, list):
+            self._sides = sides
+        else:
+            raise TypeError('Sides can only be passed in a list')
+
+    @property
+    def lower_layer(self) -> ICircle:
+        return self._lower_layer
+
+    @lower_layer.setter
+    def lower_layer(self, circle: ICircle):
+        if isinstance(circle, ICircle):
+            self._lower_layer = circle
+        else:
+            raise TypeError('Cylinder layers must be type ICircle')
+
+    @property
+    def upper_layer(self) -> ICircle:
+        return self._upper_layer
+
+    @upper_layer.setter
+    def upper_layer(self, circle: ICircle):
+        if isinstance(circle, ICircle):
+            self._upper_layer = circle
+        else:
+            raise TypeError('Cylinder layers must be type ICircle')
+
+    def to_kml(self) -> Union[tuple[list, list, list]]:
+        """
+        Returns kml formatted coordinates in a list for the lower layer, upper layer and sides.
+        Returns:
+            lower, upper, sides (tuple[list, list, list]): Lists of kml formatted tuples.
+
+        """
+        lower = [(p.x, p.y, p.z) for p in self.lower_layer]
+        upper = [(p.x, p.y, p.z) for p in self.upper_layer]
+        sides = []
+
+        for polygon in self.sides:
+            holding_list = []
+            for point_list in polygon:
+                holding_list.append((point_list.x, point_list.y, point_list.z))
+            sides.append(holding_list)
+
+        return lower, upper, sides
+
+    def create_layer(self, coordinate_list: tuple[list[str, float, int]], layer_height) -> ICircle:
+        """
+        Creates a 2D circle to act as the top or bottom layer of the cylinder
+        Args:
+            coordinate_list (tuple[list[str, float, int]]): Contains string information for coordinate and radius
+            layer_height: The z value of the layer
+
+        Returns:
+            circle (ICircle): A circle object
+        """
+        if layer_height:
+            circle = Circle(coordinate_list[0], coordinate_list[1], z=layer_height, uom=self.uom,
+                            radius_uom=self.radius_uom)
+        else:
+            circle = Circle(coordinate_list[0], coordinate_list[1], uom=self.uom, radius_uom=self.radius_uom)
+        return circle
+
+    def generate_sides(self) -> list[ICircle]:
+        """
+        Creates the sides of the cylinder. Requires both layers to contain the same amount of points.
+
+        Returns:
+            side_coordinates (list[IPolygon]): A list of polygons joining the upper and lower layers together.
+
+        Raises:
+            IndexError: If lower layer and upper layer do not have the same quantity of points.
+        """
+        if len(self.lower_layer) != len(self.upper_layer):
+            raise IndexError(f'Lower and upper polygon must contain the same amount of points.  Point count - lower'
+                             f'polygon: {len(self.lower_layer)} upper polygon: {len(self.upper_layer)}')
+        else:
+            side_coordinates = []
+            i = 0
+            while i < len(self.lower_layer) - 1:
+                polygon_coordinate_list = [self.lower_layer.point_list[i].__str__(), self.lower_layer[i + 1].__str__(),
+                                           self.upper_layer[i + 1].__str__(), self.upper_layer[i].__str__(),
+                                           self.lower_layer[i].__str__()]
+
+                side_coordinates.append(Polygon(polygon_coordinate_list, uom=self.uom))
+
+                i += 1
+
+            return side_coordinates
+
+
+class Polygon(IPolygon, I2DObject):
+    """
+    Creates a polygon made of 2 or more vertices
+
+    Args:
+        coordinate_list (list[str]): A list of strings representing coordinates of vertices.
+
+    Keyword Args:
+        uom (str): Unit of measure for elevation, FT or M
+        z (float): Override all string elevation values with a single blanket value.
+    """
+
+    def __init__(self, coordinate_list: list, **kwargs: str):
+        self.uom = kwargs.get('uom', 'FT')
+        self.z = kwargs.get('z', None)
+        self.point_list = self.process_points(coordinate_list)
+        self.centroid = self.calculate_centroid()
+
+    def __len__(self) -> int:
+        return len(self.point_list)
+
+    def __iter__(self):
+        self.n = 0
+        return self
+
+    def __next__(self):
+        if self.n < len(self.point_list):
+            result = self.point_list[self.n]
+            self.n += 1
+            return result
+        else:
+            raise StopIteration
+
+    def __getitem__(self, index):
+        return self.point_list[index]
+
+    def __setitem__(self, index, point):
+        if isinstance(point, Point):
+            self.point_list[index] = point
+        else:
+            raise TypeError('Polygon will only accept objects of type kmlplus.geo.Point')
+
+    def __eq__(self, another_2D_object: I2DObject) -> bool:
+        return self.__len__() != another_2D_object.__len__()
+
+    @property
+    def z(self):
+        return self._z
+
+    @z.setter
+    def z(self, value):
+        if not value:
+            self._z = None
+        elif isinstance(value, float):
+            conversion_dict = {'FT': 0.3048, 'M': 1}
+            self._z = value * conversion_dict[self.uom]
+        else:
+            self.z = float(value)
+
+    @property
+    def point_list(self):
+        return self._point_list
+
+    @point_list.setter
+    def point_list(self, a_point_list: list):
+        if len(a_point_list) > 2 and isinstance(a_point_list, list):
+            # Close the polygon, if it is not already
+            if a_point_list[0] != a_point_list[-1]:
+                first_vertice = a_point_list[0]
+                a_point_list.append(first_vertice)
+            self._point_list = a_point_list
+        else:
+            raise ValueError('Cannot process_points a polygon from less than 2 points')
+
+    def calculate_centroid(self) -> ILocation:
+        """
+        Calculates the centre (centroid) of the polygon's area. This is used for sorting the polygons so that they are
+        drawn correctly in Google Earth.
+
+        Returns:
+            point (ILocation)
+        """
+        latitude_total, longitude_total = 0, 0
+        for coordinate_instance in self.point_list:
+            latitude_total += coordinate_instance.y
+            longitude_total += coordinate_instance.x
+        latitude_average, longitude_average = latitude_total / len(self.point_list), \
+                                              longitude_total / len(self.point_list)
+
+        point = Point(latitude_average, longitude_average)
+        return point
+
+    def calculate_bearing_from_centroid(self, point: ILocation) -> ILocation:
+        """
+        Calculates the bearing to the point from the centre of the polygon (Centroid)
+
+        Args:
+            point (ILocation): The point to find the bearing to
+
+        Returns:
+            bearing (float): The bearing in degrees
+
+        """
+        bearing = point.get_bearing(self.centroid)
+        return bearing
+
+    def process_points(self, point_list: list[str]) -> list[ILocation]:
+        """
+        Creates ILocation objects from the list of coordinates supplied.
+        Args:
+            point_list (list[str]): A list of coordinate information in string format
+
+        Returns:
+            points (list[ILocation]): A list of ILocation objects representing the vertices of the polygon
+        """
+        points = PointFactory(
+            point_list,
+            z=self._z,
+            uom=self.uom
+        ).process_coordinates()
+
+        return points
+
+
+class Polyhedron(I3DObject):
+    """
+    A Polyhedron (3D object) comprised of a lower layer, upper layer and sides.
+
+    Args:
+        lower_coordinates (list[str]): A list of str representation of coordinates.
+        upper_coordinates (list[str]): A list of str representation of coordinates.
+
+    Keyword Args:
+        uom = Unit of measure for elevation, FT or M
+    """
+
+    def __init__(self, lower_coordinates: list[str], upper_coordinates: list[str], **kwargs: str):
+        self.uom = kwargs.get('uom', 'FT')
+        self.lower_layer = self.create_layer(lower_coordinates, kwargs.get('lower_layer', None))
+        self.upper_layer = self.create_layer(upper_coordinates, kwargs.get('upper_layer', None))
+        self.sides = self.generate_sides()
+
+    @property
+    def lower_layer(self) -> I2DObject:
+        return self._lower_layer
+
+    @lower_layer.setter
+    def lower_layer(self, a_polygon: I2DObject):
+        if isinstance(a_polygon, I2DObject):
+            self._lower_layer = a_polygon
+        else:
+            raise TypeError('Lower layer must be a type of I2DObject')
+
+    @property
+    def upper_layer(self):
+        return self._upper_layer
+
+    @upper_layer.setter
+    def upper_layer(self, a_polygon):
+        self._upper_layer = a_polygon
+
+    @property
+    def sides(self):
+        return self._sides
+
+    @sides.setter
+    def sides(self, sides: list):
+        if isinstance(sides, list):
+            self._sides = sides
+        else:
+            raise TypeError('Sides can only be passed in a list')
+
+    def to_kml(self) -> tuple:
+        """
+        Processes the upper, lower layers and sides. Converts their data to a KML friendly format.
+
+        Returns:
+            lower, upper, sides (tuple):
+        """
+        lower = [(p.x, p.y, p.z) for p in self.lower_layer]
+        upper = [(p.x, p.y, p.z) for p in self.upper_layer]
+        sides = []
+
+        for polygon in self.sides:
+            holding_list = []
+            for point_list in polygon:
+                holding_list.append((point_list.x, point_list.y, point_list.z))
+            sides.append(holding_list)
+
+        return lower, upper, sides
+
+    def create_layer(self, coordinate_list: list[str], layer_height: str) -> IPolygon:
+        """
+        Creates a layer for the polygon
+        Args:
+            coordinate_list (list): List containing a string of coordinate information
+            layer_height (str): The elevation value of the layer
+
+        Returns:
+
+        """
+        if layer_height:
+            poly = Polygon(coordinate_list, z=layer_height, uom=self.uom)
+        else:
+            poly = Polygon(coordinate_list)
+        return poly
+
+    def generate_sides(self) -> list[IPolygon]:
+        """
+        Creates the side polygons to connect the upper and lower layers. Requires upper and lower layers to have
+        matching amount of vertices
+
+        Returns:
+            side_coordinates (list[IPolygon]): List of polygons which make up the sides of the polyhedron.
+        """
+        if len(self.lower_layer) != len(self.upper_layer):
+            raise IndexError(f'Lower and upper polygon must contain the same amount of points.  Point count - lower '
+                             f'polygon: {len(self.lower_layer)} upper polygon: {len(self.upper_layer)}')
+        else:
+            side_coordinates = []
+            i = 0
+            while i < len(self.lower_layer) - 1:
+                polygon_coordinate_list = [self.lower_layer[i].__str__(), self.lower_layer[i + 1].__str__(),
+                                           self.upper_layer[i + 1].__str__(), self.upper_layer[i].__str__(),
+                                           self.lower_layer[i].__str__()]
+
+                side_polygon = Polygon(polygon_coordinate_list, uom=self.uom)
+
+                side_coordinates.append(side_polygon)
+
+                i += 1
+
+            return side_coordinates
+
+
+class LineString(I2DObject):
+    """
+    Represents a kml LineString.
+
+    Args:
+        coordinate_list (list[str]): A list containing two or more strings representing coordinates
+
+    Keyword Args:
+        uom (str): Unit of measure for elevation, FT or M.
+    """
+
+    def __init__(self, coordinate_list, **kwargs):
+        self.uom = kwargs.get('uom', 'FT')
+        self.z = kwargs.get('z', None)
+        self.point_list = self.create(coordinate_list)
+
+    def __len__(self):
+        return len(self.point_list)
+
+    def __iter__(self):
+        self.n = 0
+        return self
+
+    def __next__(self):
+        if self.n < len(self.point_list):
+            result = self.point_list[self.n]
+            self.n += 1
+            return result
+        else:
+            raise StopIteration
+
+    def __getitem__(self, index):
+        return self.point_list[index]
+
+    def __setitem__(self, index, point):
+        if isinstance(point, Point):
+            self.point_list[index] = point
+        else:
+            raise TypeError('Polygon will only accept objects of type kmlplus.geo.Point')
+
+    def create(self, coordinate_list: list[str]) -> list[ILocation]:
+        point_list = PointFactory(coordinate_list, uom=self.uom, z=self.z).process_coordinates()
+        return point_list
```

### Comparing `KMLPlus-3.0.0b1/kmlplus/util.py` & `KMLPlus-3.0.0b2/kmlplus/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-import re
-
-
-def dms_to_decimal(latitude_or_longitude):
-    slice_dms = get_dms_slice_dict(latitude_or_longitude)
-    calculated_dms_dict = calculate_dms_to_decimal(slice_dms)
-
-    # Using formula - DD + MM / 60 + SS.ss / 3600
-    decimal_coordinate = calculated_dms_dict['degrees'] + (calculated_dms_dict['minutes'] +
-                                                           calculated_dms_dict['seconds'])
-
-    if slice_dms['hemisphere'] == 'S' or slice_dms['hemisphere'] == 'W':
-        decimal_coordinate = -abs(decimal_coordinate)
-
-    return decimal_coordinate
-
-
-def get_dms_slice_dict(latitude_or_longitude_string):
-    hemisphere = latitude_or_longitude_string[-1]
-
-    if hemisphere == 'W' or hemisphere == 'E':
-        degrees = int(latitude_or_longitude_string[0:3])
-        minutes = int(latitude_or_longitude_string[3:5])
-        seconds = float(latitude_or_longitude_string[5:-1])
-
-    elif hemisphere == 'N' or hemisphere == 'S':
-        degrees = int(latitude_or_longitude_string[0:2])
-        minutes = int(latitude_or_longitude_string[2:4])
-        seconds = float(latitude_or_longitude_string[4:-1])
-
-    else:
-        raise ValueError('DMS coordinates must indicate which hemisphere they belong to by appending N, E, S or W' \
-                         'to the end of the coordinate.  No other format currently accepted')
-
-    slice_dict = {'degrees': degrees, 'minutes': minutes, 'seconds': seconds, 'hemisphere': hemisphere}
-
-    return slice_dict
-
-
-def calculate_dms_to_decimal(dms_sliced_dict):
-    degrees = dms_sliced_dict['degrees']
-    minutes = dms_sliced_dict['minutes'] / 60
-    seconds = dms_sliced_dict['seconds'] / 3600
-
-    calculated_dms_dict = {'degrees': degrees, 'minutes': minutes, 'seconds': seconds,
-                           'hemisphere': dms_sliced_dict['hemisphere']}
-
-    return calculated_dms_dict
-
-
-def get_earth_radius(**kwargs) -> float:
-    uom_dict = {'km': 6378.14, 'mi': 3963.19, 'nm': 3443.92, 'm': 6378140.00}
-    return uom_dict[kwargs.pop('uom', 'km')]
-
-
-def contains_z_value(coordinate_string: str):
-    coordinate_string.split(' ')
-    if len(coordinate_string) == 3:
-        return True
-    elif len(coordinate_string) == 2:
-        return False
-    else:
-        raise ValueError('Coordinate string must contain at least two valid coordinates of the same type and an,'
-                         ' optional height z value, separated by a comma separator')
-
-
-def detect_coordinate_type(coordinate_string):
-    split_list = coordinate_string.split(' ')
-
-    def match_regex(string_to_match):
-        regex_dict = {'dms': '^\d{6,7}[.]\d{1,}\D{1}$|^\d{6,7}\D{1}$',
-                      'dd': '^[-?|+?]?\d{1,3}[.]\d+$'}
-
-        if re.match(regex_dict['dms'], string_to_match):
-            return 'dms'
-        elif re.match(regex_dict['dd'], string_to_match):
-            return 'dd'
-        else:
-            raise ValueError('Only valid DMS or decimal degree coordinate pairs are accepted.')
-
-    def equal_type(type_1: str, type_2: str):
-        if type_1 == type_2:
-            return type_1
-        else:
-            raise ValueError('Both latitude and longitude must be the same type.  Both DMS or both DD.')
-
-    lat_type = match_regex(split_list[0].strip())
-    lon_type = match_regex(split_list[1].strip())
-
-    if equal_type(lat_type, lon_type):
-        return lat_type
-    else:
-        raise ValueError('Latitude and longitude must both be the same type.  ie - both decimal degrees; dms'
-                         'or UTM')
-
-
-def point_or_segment(coordinate_string: str):
-    if '=' in coordinate_string:
-        return 'curvedsegment'
-    else:
-        return 'point'
-
-
-def split_segment_string(string):
-    split_list = string.split(', ')
-    segment_dict = {item.split('=')[0]: item.split('=')[1] for item in split_list}
-    return segment_dict
+import re
+
+
+def dms_to_decimal(latitude_or_longitude):
+    slice_dms = get_dms_slice_dict(latitude_or_longitude)
+    calculated_dms_dict = calculate_dms_to_decimal(slice_dms)
+
+    # Using formula - DD + MM / 60 + SS.ss / 3600
+    decimal_coordinate = calculated_dms_dict['degrees'] + (calculated_dms_dict['minutes'] +
+                                                           calculated_dms_dict['seconds'])
+
+    if slice_dms['hemisphere'] == 'S' or slice_dms['hemisphere'] == 'W':
+        decimal_coordinate = -abs(decimal_coordinate)
+
+    return decimal_coordinate
+
+
+def get_dms_slice_dict(latitude_or_longitude_string):
+    hemisphere = latitude_or_longitude_string[-1]
+
+    if hemisphere == 'W' or hemisphere == 'E':
+        degrees = int(latitude_or_longitude_string[0:3])
+        minutes = int(latitude_or_longitude_string[3:5])
+        seconds = float(latitude_or_longitude_string[5:-1])
+
+    elif hemisphere == 'N' or hemisphere == 'S':
+        degrees = int(latitude_or_longitude_string[0:2])
+        minutes = int(latitude_or_longitude_string[2:4])
+        seconds = float(latitude_or_longitude_string[4:-1])
+
+    else:
+        raise ValueError('DMS coordinates must indicate which hemisphere they belong to by appending N, E, S or W' \
+                         'to the end of the coordinate.  No other format currently accepted')
+
+    slice_dict = {'degrees': degrees, 'minutes': minutes, 'seconds': seconds, 'hemisphere': hemisphere}
+
+    return slice_dict
+
+
+def calculate_dms_to_decimal(dms_sliced_dict):
+    degrees = dms_sliced_dict['degrees']
+    minutes = dms_sliced_dict['minutes'] / 60
+    seconds = dms_sliced_dict['seconds'] / 3600
+
+    calculated_dms_dict = {'degrees': degrees, 'minutes': minutes, 'seconds': seconds,
+                           'hemisphere': dms_sliced_dict['hemisphere']}
+
+    return calculated_dms_dict
+
+
+def get_earth_radius(**kwargs) -> float:
+    uom_dict = {'km': 6378.14, 'mi': 3963.19, 'nm': 3443.92, 'm': 6378140.00}
+    return uom_dict[kwargs.pop('uom', 'km')]
+
+
+def contains_z_value(coordinate_string: str):
+    coordinate_string.split(' ')
+    if len(coordinate_string) == 3:
+        return True
+    elif len(coordinate_string) == 2:
+        return False
+    else:
+        raise ValueError('Coordinate string must contain at least two valid coordinates of the same type and an,'
+                         ' optional height z value, separated by a comma separator')
+
+
+def detect_coordinate_type(coordinate_string):
+    split_list = coordinate_string.split(' ')
+
+    def match_regex(string_to_match):
+        regex_dict = {'dms': '^\d{6,7}[.]\d{1,}\D{1}$|^\d{6,7}\D{1}$',
+                      'dd': '^[-?|+?]?\d{1,3}[.]\d+|[-?|+?]?\d{1,3}$'}
+
+        if re.match(regex_dict['dms'], string_to_match):
+            return 'dms'
+        elif re.match(regex_dict['dd'], string_to_match):
+            return 'dd'
+        else:
+            raise ValueError('Only valid DMS or decimal degree coordinate pairs are accepted.')
+
+    def equal_type(type_1: str, type_2: str):
+        if type_1 == type_2:
+            return type_1
+        else:
+            raise ValueError('Both latitude and longitude must be the same type.  Both DMS or both DD.')
+
+    lat_type = match_regex(split_list[0].strip())
+    lon_type = match_regex(split_list[1].strip())
+
+    if equal_type(lat_type, lon_type):
+        return lat_type
+    else:
+        raise ValueError('Latitude and longitude must both be the same type.  ie - both decimal degrees; dms'
+                         'or UTM')
+
+
+def point_or_segment(coordinate_string: str):
+    if '=' in coordinate_string:
+        return 'curvedsegment'
+    else:
+        return 'point'
+
+
+def split_segment_string(string):
+    split_list = string.split(', ')
+    segment_dict = {item.split('=')[0]: item.split('=')[1] for item in split_list}
+    return segment_dict
```

### Comparing `KMLPlus-3.0.0b1/test/test_geo.py` & `KMLPlus-3.0.0b2/test/test_geo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,204 +1,234 @@
-from unittest import TestCase
-
-from kmlplus import util
-from kmlplus.geo import Point, PointFactory, ClockwiseCurvedSegment, AnticlockwiseCurvedSegment, CurvedSegmentFactory
-
-
-class TestPoint(TestCase):
-    def setUp(self):
-        self.test_point_1 = Point.from_dms('551206.00N', '0045206.234W')
-        self.test_point_2 = Point.from_dms('501206.00N', '0045206.234W')
-        self.test_midpoint = Point.find_midpoint(self.test_point_1, self.test_point_2)
-
-    def test_from_dms(self):
-        test_obj = Point.from_dms('551206.00N', '0045206.234W')
-        self.assertEqual(test_obj.y, 55.20166666666667)
-        self.assertEqual(test_obj.x, -4.868398333333333)
-        self.assertEqual(test_obj.z, 0)
-
-        test_obj = Point.from_dms('501206.00N', '0045206.234W', z=383, distance_uom='M')
-        self.assertEqual(test_obj.y, 50.20166666666667)
-        self.assertEqual(test_obj.x, -4.868398333333333)
-        self.assertAlmostEqual(test_obj.z, 383.0, delta=5)
-
-        test_obj = Point.from_dms('501206.00N', '0045206.234W', z=383, uom='M', distance_uom='M')
-        self.assertEqual(test_obj.y, 50.20166666666667)
-        self.assertEqual(test_obj.x, -4.868398333333333)
-        self.assertEqual(test_obj.z, 383.0)
-
-    def test_find_midpoint(self):
-        mp = Point.find_midpoint(self.test_point_1, self.test_point_2)
-        self.assertAlmostEqual(52.701666666667, mp.y, delta=0.0000001)
-        self.assertAlmostEqual(-4.8683983333333, mp.x, delta=0.0000001)
-
-    def test_from_point_bearing_and_distance(self):
-        test_obj = Point.from_dms('551206.00N', '0045206.23W')
-        test_result = Point.from_point_bearing_and_distance(test_obj, 180.00, 383.00, distance_uom='NM')
-
-        self.assertAlmostEqual(48.821944, test_result.y, delta=0.01)
-        self.assertAlmostEqual(-4.868333, test_result.x, delta=0.01)
-
-    def test_get_distance(self):
-        # test km
-        test_obj = Point.from_dms('551206.00N', '0045206.234W')
-        distance = test_obj.get_distance(Point.from_dms('501206.00N', '0045206.234W'))
-        self.assertEqual(556402.304538113, distance)
-
-        # test miles
-        test_obj = Point.from_dms('551206.00N', '0045206.234W')
-        distance = test_obj.get_distance(Point.from_dms('501206.00N', '0045206.234W', distance_uom='KM'))
-        self.assertEqual(556402.304538113, distance)
-
-    def test_get_bearing(self):
-        result = self.test_point_1.get_bearing(self.test_point_2)
-        self.assertEqual(180, result)
-
-        result = self.test_point_2.get_bearing(self.test_point_1)
-        self.assertEqual(0, result)
-
-        result = self.test_midpoint.get_bearing(self.test_point_1)
-        self.assertEqual(0, result)
-
-        result = self.test_midpoint.get_bearing(self.test_point_2)
-        self.assertEqual(180, result)
-
-    def test_get_inverse_bearing(self):
-        inverse_bearing = self.test_point_1.get_inverse_bearing(self.test_point_2)
-        self.assertEqual(0, inverse_bearing)
-
-        inverse_bearing = self.test_point_2.get_inverse_bearing(self.test_point_1)
-        self.assertEqual(180, inverse_bearing)
-
-        inverse_bearing = self.test_midpoint.get_inverse_bearing(self.test_point_2)
-        self.assertEqual(0, inverse_bearing)
-
-        inverse_bearing = self.test_midpoint.get_inverse_bearing(self.test_point_1)
-        self.assertEqual(180, inverse_bearing)
-
-
-class TestPointFactory(TestCase):
-    def setUp(self):
-        self.pf = PointFactory(['22.323232 -4.287282', '23.323232 -5.328723', '22.112333 -6.23789238923'])
-
-    def test_process_coordinates(self):
-        test_dd = self.pf.process_coordinates()
-        for i in range(len(test_dd)):
-            self.assertTrue(isinstance(test_dd[i], Point))
-
-        # Test that dms coordinates are correctly returned as decimal degrees.
-        test_dms = self.pf.process_coordinates()
-        type_result = util.detect_coordinate_type(f'{test_dms[0].y} {test_dms[0].x}')
-        self.assertEqual(type_result, 'dd')
-
-    def test_populate_point_list(self):
-        test_point_list = self.pf.populate_point_list()
-        self.assertTrue(isinstance(test_point_list, list))
-
-    def test_process_string(self):
-        no_height = '22.323232 -4.287282'
-        with_height = '22.323232 -4.287282 8'
-
-        dms_test = '521244N 0056555W'
-
-        no_height_obj = self.pf.process_string(no_height, 'dd')
-        with_height_obj = self.pf.process_string(with_height, 'dd')
-        dms_obj = self.pf.process_string(dms_test, 'dms')
-
-        self.assertTrue(isinstance(no_height_obj, Point))
-        self.assertTrue(isinstance(with_height_obj, Point))
-        self.assertTrue(isinstance(dms_obj, Point))
-
-        self.assertEqual(no_height_obj.z, 0.0)
-        self.assertEqual(with_height_obj.z, 8.0)
-        self.assertEqual(dms_obj.y, 52.21222222222222)
-
-
-class TestCurvedSegmentFactory(TestCase):
-    def test_process_segment(self):
-        c_cs = CurvedSegmentFactory('start=522423N 0042354W, end=522428N 0042254W, direction=clockwise,' \
-                                    ' centre=502211N 0043212W, sample=50').process_segment()
-        ac_cs = CurvedSegmentFactory('start=522423N 0042354W, end=522428N 0042254W, direction=anticlockwise,' \
-                                     ' centre=502211N 0043212W, sample=50').process_segment()
-        self.assertTrue(isinstance(c_cs, ClockwiseCurvedSegment))
-        self.assertTrue(isinstance(ac_cs, AnticlockwiseCurvedSegment))
-
-    def test_generate_segment(self):
-        c_cs = CurvedSegmentFactory('start=522423N 0042354W, end=522428N 0042254W, direction=clockwise,' \
-                                    ' centre=502211N 0043212W, sample=50').generate_segment()
-        ac_cs = CurvedSegmentFactory('start=522423N 0042354W, end=522428N 0042254W, direction=anticlockwise,' \
-                                     ' centre=502211N 0043212W, sample=50').generate_segment()
-        self.assertTrue(len(c_cs) == 52)
-        self.assertTrue(len(ac_cs) == 52)
-        for i in c_cs:
-            self.assertTrue(isinstance(i, Point))
-        for i in ac_cs:
-            self.assertTrue(isinstance(i, Point))
-
-
-class TestClockwiseCurvedSegment(TestCase):
-    def setUp(self):
-        self.test_obj = ClockwiseCurvedSegment(Point.from_dms('551206.00N', '0045206.234W'),
-                                               Point.from_dms('501206.00N', '0045206.234W'),
-                                               'FT',
-                                               sample=100)
-        self.inverse_test_obj = ClockwiseCurvedSegment(Point.from_dms('501206.00N', '0045206.234W'),
-                                                       Point.from_dms('551206.00N', '0045206.234W'),
-                                                       'FT',
-                                                       sample=2)
-
-    def test_get_points(self):
-        result = self.test_obj.get_points()
-        self.assertEqual(len(result), 102)
-
-        # Check start and end points are accurately computed
-        # Delta 7 implies tolerance of 1.11cm
-        self.assertAlmostEqual(result[0].y, 55.20166666666667, delta=7)
-        self.assertAlmostEqual(result[0].x, -4.868398333333333, delta=7)
-
-        self.assertAlmostEqual(result[99].y, 50.20166666666667, delta=7)
-        self.assertAlmostEqual(result[99].x, -4.868398333333333, delta=7)
-
-        # As this is moving clockwise, the longitude should increase due to the arc as its moving easterly.
-        self.assertTrue(result[0].x < result[49].x)
-
-    def test_get_bearing_increments(self):
-        result = self.test_obj.get_bearing_increment()
-        self.assertEqual(result, 1.7821782178217822)
-
-        result = self.inverse_test_obj.get_bearing_increment()
-        self.assertEqual(result, 60)
-
-
-class TestAnticlockwiseCurvedSegment(TestCase):
-    def setUp(self):
-        self.test_obj = AnticlockwiseCurvedSegment(Point.from_dms('551206.00N', '0045206.234W'),
-                                                   Point.from_dms('501206.00N', '0045206.234W'),
-                                                   'FT',
-                                                   sample=100)
-
-        self.inverse_test_obj = AnticlockwiseCurvedSegment(Point.from_dms('501206.00N', '0045206.234W'),
-                                                           Point.from_dms('551206.00N', '0045206.234W'),
-                                                           'FT',
-                                                           sample=100)
-
-    def test_get_points(self):
-        result = self.test_obj.get_points()
-        self.assertEqual(len(result), 102)
-
-        # Check start and end points are accurately computed
-        # Delta 7 implies tolerance of 1.11cm
-        self.assertAlmostEqual(result[0].y, 55.20166666666667, delta=7)
-        self.assertAlmostEqual(result[0].x, -4.868398333333333, delta=7)
-
-        self.assertAlmostEqual(result[99].y, 50.20166666666667, delta=7)
-        self.assertAlmostEqual(result[99].x, -4.868398333333333, delta=7)
-
-        # As this is moving anti-clockwise, the longitude should decrease due to the arc as its moving westerly.
-        self.assertTrue(result[0].x > result[49].x)
-
-    def test_get_bearing_increments(self):
-        result = self.test_obj.get_bearing_increment()
-        self.assertEqual(1.7821782178217822, result)
-
-        result = self.inverse_test_obj.get_bearing_increment()
-        self.assertEqual(1.7821782178217822, result)
+from unittest import TestCase
+
+from kmlplus import util
+from kmlplus.geo import Point, PointFactory, ClockwiseCurvedSegment, AnticlockwiseCurvedSegment, CurvedSegmentFactory
+
+
+class TestPoint(TestCase):
+    def setUp(self):
+        self.test_point_1 = Point.from_dms('551206.00N', '0045206.234W')
+        self.test_point_2 = Point.from_dms('501206.00N', '0045206.234W')
+        self.test_midpoint = Point.find_midpoint(self.test_point_1, self.test_point_2)
+
+    def test_from_dms(self):
+        test_obj = Point.from_dms('551206.00N', '0045206.234W')
+        self.assertEqual(test_obj.y, 55.20166666666667)
+        self.assertEqual(test_obj.x, -4.868398333333333)
+        self.assertEqual(test_obj.z, 0)
+
+        test_obj = Point.from_dms('501206.00N', '0045206.234W', z=383, distance_uom='m')
+        self.assertEqual(test_obj.y, 50.20166666666667)
+        self.assertEqual(test_obj.x, -4.868398333333333)
+        self.assertAlmostEqual(test_obj.z, 383.0, delta=5)
+
+        test_obj = Point.from_dms('501206.00N', '0045206.234W', z=383, uom='M', distance_uom='m')
+        self.assertEqual(test_obj.y, 50.20166666666667)
+        self.assertEqual(test_obj.x, -4.868398333333333)
+        self.assertEqual(test_obj.z, 383.0)
+
+    def test_find_midpoint(self):
+        mp = Point.find_midpoint(self.test_point_1, self.test_point_2)
+        self.assertAlmostEqual(52.701666666667, mp.y, delta=0.0000001)
+        self.assertAlmostEqual(-4.8683983333333, mp.x, delta=0.0000001)
+
+    def test_from_point_bearing_and_distance(self):
+        test_obj = Point.from_dms('551206.00N', '0045206.23W')
+        test_result = Point.from_point_bearing_and_distance(test_obj, 180.00, 383.00, distance_uom='nm')
+
+        self.assertAlmostEqual(48.821944, test_result.y, delta=0.01)
+        self.assertAlmostEqual(-4.868333, test_result.x, delta=0.01)
+
+    def test_get_distance(self):
+        # test km
+        test_obj = Point.from_dms('551206.00N', '0045206.234W')
+        distance = test_obj.get_distance(Point.from_dms('501206.00N', '0045206.234W'))
+        self.assertEqual(556402.304538113, distance)
+
+        # test miles
+        test_obj = Point.from_dms('551206.00N', '0045206.234W')
+        distance = test_obj.get_distance(Point.from_dms('501206.00N', '0045206.234W', distance_uom='km'))
+        self.assertEqual(556402.304538113, distance)
+
+    def test_get_bearing(self):
+        result = self.test_point_1.get_bearing(self.test_point_2)
+        self.assertEqual(180, result)
+
+        result = self.test_point_2.get_bearing(self.test_point_1)
+        self.assertEqual(0, result)
+
+        result = self.test_midpoint.get_bearing(self.test_point_1)
+        self.assertEqual(0, result)
+
+        result = self.test_midpoint.get_bearing(self.test_point_2)
+        self.assertEqual(180, result)
+
+    def test_get_inverse_bearing(self):
+        inverse_bearing = self.test_point_1.get_inverse_bearing(self.test_point_2)
+        self.assertEqual(0, inverse_bearing)
+
+        inverse_bearing = self.test_point_2.get_inverse_bearing(self.test_point_1)
+        self.assertEqual(180, inverse_bearing)
+
+        inverse_bearing = self.test_midpoint.get_inverse_bearing(self.test_point_2)
+        self.assertEqual(0, inverse_bearing)
+
+        inverse_bearing = self.test_midpoint.get_inverse_bearing(self.test_point_1)
+        self.assertEqual(180, inverse_bearing)
+
+
+class TestPointFactory(TestCase):
+    def setUp(self):
+        self.pf = PointFactory(['22.323232 -4.287282', '23.323232 -5.328723', '22.112333 -6.23789238923'])
+
+    def test_process_coordinates(self):
+        test_dd = self.pf.process_coordinates()
+        for i in range(len(test_dd)):
+            self.assertTrue(isinstance(test_dd[i], Point))
+
+        # Test that dms coordinates are correctly returned as decimal degrees.
+        test_dms = self.pf.process_coordinates()
+        type_result = util.detect_coordinate_type(f'{test_dms[0].y} {test_dms[0].x}')
+        self.assertEqual(type_result, 'dd')
+
+    def test_populate_point_list(self):
+        test_point_list = self.pf.populate_point_list()
+        self.assertTrue(isinstance(test_point_list, list))
+        self.assertEqual(3, len(test_point_list))
+
+    def test_create_curved_segment(self):
+        test_segment = self.pf.create_curved_segment('start=553322N 0043322W, centre=502211N 0043222W, end=510000N '
+                                                     '0040010W, direction=clockwise')
+
+        self.assertTrue(isinstance(test_segment, list))
+        self.assertEqual(102, len(test_segment))
+        for i in test_segment:
+            self.assertTrue(isinstance(i, Point))
+            self.assertEqual(0, i.z)
+
+    def test_process_string(self):
+        no_height = '22.323232 -4.287282'
+        with_height = '22.323232 -4.287282 8'
+
+        dms_test = '521244N 0056555W'
+
+        no_height_obj = self.pf.process_string(no_height)
+        with_height_obj = self.pf.process_string(with_height)
+        dms_obj = self.pf.process_string(dms_test)
+
+        self.assertTrue(isinstance(no_height_obj, Point))
+        self.assertTrue(isinstance(with_height_obj, Point))
+        self.assertTrue(isinstance(dms_obj, Point))
+
+        self.assertEqual(no_height_obj.z, 0.0)
+        self.assertEqual(with_height_obj.z, 8.0)
+        self.assertEqual(dms_obj.y, 52.21222222222222)
+
+    def test_process_x_y(self):
+        dd_xy = '22.323232 -4.287282'
+        dms_xy = '521244N 0056555W 50'
+
+        dd_xy_obj = self.pf.process_x_y(dd_xy.split(' '), getattr(Point, 'from_decimal_degrees'))
+        dms_xy_obj = self.pf.process_x_y(dms_xy.split(' '), getattr(Point, 'from_dms'))
+
+        self.assertTrue(isinstance(dd_xy_obj, Point))
+        self.assertTrue(isinstance(dms_xy_obj, Point))
+        self.assertEqual(0, dd_xy_obj.z)
+        self.assertEqual(0, dms_xy_obj.z)
+
+    def test_process_x_y_z(self):
+        with_height = '22.323232 -4.287282 8'
+        dms_xyz_obj = self.pf.process_x_y_z(with_height.split(' '), getattr(Point, 'from_decimal_degrees'))
+
+        self.assertTrue(isinstance(dms_xyz_obj, Point))
+        self.assertEqual(8.0, dms_xyz_obj.z)
+
+
+class TestCurvedSegmentFactory(TestCase):
+    def test_process_segment(self):
+        c_cs = CurvedSegmentFactory('start=522423N 0042354W, end=522428N 0042254W, direction=clockwise,' \
+                                    ' centre=502211N 0043212W, sample=50').process_segment()
+        ac_cs = CurvedSegmentFactory('start=522423N 0042354W, end=522428N 0042254W, direction=anticlockwise,' \
+                                     ' centre=502211N 0043212W, sample=50').process_segment()
+        self.assertTrue(isinstance(c_cs, ClockwiseCurvedSegment))
+        self.assertTrue(isinstance(ac_cs, AnticlockwiseCurvedSegment))
+
+    def test_generate_segment(self):
+        c_cs = CurvedSegmentFactory('start=522423N 0042354W, end=522428N 0042254W, direction=clockwise,' \
+                                    ' centre=502211N 0043212W, sample=50').generate_segment()
+        ac_cs = CurvedSegmentFactory('start=522423N 0042354W, end=522428N 0042254W, direction=anticlockwise,' \
+                                     ' centre=502211N 0043212W, sample=50').generate_segment()
+        self.assertTrue(len(c_cs) == 52)
+        self.assertTrue(len(ac_cs) == 52)
+        for i in c_cs:
+            self.assertTrue(isinstance(i, Point))
+        for i in ac_cs:
+            self.assertTrue(isinstance(i, Point))
+
+
+class TestClockwiseCurvedSegment(TestCase):
+    def setUp(self):
+        self.test_obj = ClockwiseCurvedSegment(Point.from_dms('551206.00N', '0045206.234W'),
+                                               Point.from_dms('501206.00N', '0045206.234W'),
+                                               'FT',
+                                               sample=100)
+        self.inverse_test_obj = ClockwiseCurvedSegment(Point.from_dms('501206.00N', '0045206.234W'),
+                                                       Point.from_dms('551206.00N', '0045206.234W'),
+                                                       'FT',
+                                                       sample=2)
+
+    def test_get_points(self):
+        result = self.test_obj.get_points()
+        self.assertEqual(len(result), 102)
+
+        # Check start and end points are accurately computed
+        # Delta 7 implies tolerance of 1.11cm
+        self.assertAlmostEqual(result[0].y, 55.20166666666667, delta=7)
+        self.assertAlmostEqual(result[0].x, -4.868398333333333, delta=7)
+
+        self.assertAlmostEqual(result[99].y, 50.20166666666667, delta=7)
+        self.assertAlmostEqual(result[99].x, -4.868398333333333, delta=7)
+
+        # As this is moving clockwise, the longitude should increase due to the arc as its moving easterly.
+        self.assertTrue(result[0].x < result[49].x)
+
+    def test_get_bearing_increments(self):
+        result = self.test_obj.get_bearing_increment()
+        self.assertEqual(result, 1.7821782178217822)
+
+        result = self.inverse_test_obj.get_bearing_increment()
+        self.assertEqual(result, 60)
+
+
+class TestAnticlockwiseCurvedSegment(TestCase):
+    def setUp(self):
+        self.test_obj = AnticlockwiseCurvedSegment(Point.from_dms('551206.00N', '0045206.234W'),
+                                                   Point.from_dms('501206.00N', '0045206.234W'),
+                                                   'FT',
+                                                   sample=100)
+
+        self.inverse_test_obj = AnticlockwiseCurvedSegment(Point.from_dms('501206.00N', '0045206.234W'),
+                                                           Point.from_dms('551206.00N', '0045206.234W'),
+                                                           'FT',
+                                                           sample=100)
+
+    def test_get_points(self):
+        result = self.test_obj.get_points()
+        self.assertEqual(len(result), 102)
+
+        # Check start and end points are accurately computed
+        # Delta 7 implies tolerance of 1.11cm
+        self.assertAlmostEqual(result[0].y, 55.20166666666667, delta=7)
+        self.assertAlmostEqual(result[0].x, -4.868398333333333, delta=7)
+
+        self.assertAlmostEqual(result[99].y, 50.20166666666667, delta=7)
+        self.assertAlmostEqual(result[99].x, -4.868398333333333, delta=7)
+
+        # As this is moving anti-clockwise, the longitude should decrease due to the arc as its moving westerly.
+        self.assertTrue(result[0].x > result[49].x)
+
+    def test_get_bearing_increments(self):
+        result = self.test_obj.get_bearing_increment()
+        self.assertEqual(1.7821782178217822, result)
+
+        result = self.inverse_test_obj.get_bearing_increment()
+        self.assertEqual(1.7821782178217822, result)
```

### Comparing `KMLPlus-3.0.0b1/test/test_shapes.py` & `KMLPlus-3.0.0b2/test/test_shapes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,122 @@
-from unittest import TestCase
-
-from kmlplus.geo import Point
-from kmlplus.shapes import Circle, Polygon, Polyhedron
-
-
-class TestCircle(TestCase):
-    def setUp(self):
-        self.circle_height_args = Circle('55.1111 -3.2311 10', 10, sample=100, uom='M')
-        self.circle_height_kwargs = Circle('28.132212 2.332782', 10, sample=150, z=20, uom='M')
-
-    def test_create(self):
-        self.assertTrue(isinstance(self.circle_height_args.point_list, list))
-        self.assertEqual(len(self.circle_height_args.point_list), 101)
-        self.assertTrue(isinstance(self.circle_height_args.point_list[2], Point))
-        for i in self.circle_height_args.point_list:
-            self.assertEqual(10, i.z)
-
-        self.assertTrue(isinstance(self.circle_height_kwargs.point_list, list))
-        self.assertEqual(len(self.circle_height_kwargs.point_list), 151)
-        self.assertTrue(isinstance(self.circle_height_kwargs.point_list[2], Point))
-        for i in self.circle_height_kwargs.point_list:
-            self.assertEqual(i.z, 20)
-
-        # Test uom effects
-        c = Circle('55.1111 -3.2311 10', 10, sample=100, uom='FT')
-        for i in c:
-            self.assertEqual(10, i.z)
-
-        c = Circle('55.1111 -3.2311 10', 25, z=250, sample=100, uom='M')
-        for i in c:
-            self.assertEqual(250, i.z)
-
-
-class TestPolygon(TestCase):
-    def setUp(self):
-        pass
-
-    def test_new_layer(self):
-        test_coordinates_no_height = ['22.323232 -4.287282', '23.323232 -5.328723', '22.112333 -6.23789238923']
-        test_coordinates_with_height = ['22.323232 -4.287282 100', '23.323232 -5.328723 150',
-                                        '22.112333 -6.23789238923 200']
-        test_coordinates_with_height_override = ['22.323232 -4.287282', '23.323232 -5.328723',
-                                                 '22.112333 -6.23789238923']
-        test_coordinates_with_cw_arc = ['22.23232 -3.232323 0', 'start=21.23211 -4.122121, end=22.054541 -4.1111, z=15,'
-                                                                ' direction=clockwise']
-        test_coordinates_with_ccw_arc = ['22.23232 -3.232323 0', 'start=21.23211 -4.122121, end=22.054541 -4.1111, '
-                                                                 'z=15, direction=anticlockwise']
-        test_dms = ['554433N 0010203W', '443322N 0000102W', '443322N 0010102E']
-
-        # Tests for coordinates with no z value provided. Should default to 0.
-        result_no_height = Polygon(test_coordinates_no_height)
-
-        self.assertTrue(isinstance(result_no_height, Polygon))
-        self.assertEqual(len(result_no_height), 4)
-        for i in result_no_height:
-            self.assertEqual(i.z, 0)
-            self.assertTrue(isinstance(i, Point))
-
-        # Tests for coordinates with a user provided z value.
-        result_with_height = Polygon(test_coordinates_with_height)
-
-        self.assertTrue(isinstance(result_with_height, Polygon))
-        self.assertEqual(len(result_with_height), 4)
-        for i in result_with_height:
-            self.assertTrue(isinstance(i, Point))
-            self.assertNotEqual(i.z, 0.0)
-
-        # Test results for coordinates with height overridden.
-        result_with_height_override = Polygon(test_coordinates_with_height_override, z=500.11)
-
-        self.assertTrue(isinstance(result_with_height_override, Polygon))
-        self.assertEqual(len(result_with_height_override), 4)
-        for i in result_with_height_override:
-            self.assertTrue(isinstance(i, Point))
-            self.assertEqual(152.43352800000002, i.z)
-
-        # Test with DMS
-        result_dms_no_height = Polygon(test_dms)
-        self.assertTrue(isinstance(result_dms_no_height, Polygon))
-        self.assertEqual(4, len(result_dms_no_height))
-        for i in result_dms_no_height:
-            self.assertTrue(isinstance(i, Point))
-            self.assertEqual(0, i.z)
-
-        # Test with DD and curved segment
-        result_dd_arc = Polygon(test_coordinates_with_cw_arc)
-        self.assertTrue(isinstance(result_dd_arc, Polygon))
-        self.assertTrue(len(result_dd_arc) > 100)
-        for i in result_dd_arc:
-            self.assertTrue(isinstance(i, Point))
-            self.assertEqual(0, i.z)
-
-        result_dd_arc = Polygon(test_coordinates_with_ccw_arc)
-        self.assertTrue(isinstance(result_dd_arc, Polygon))
-        self.assertTrue(len(result_dd_arc) > 100)
-        for i in result_dd_arc:
-            self.assertTrue(isinstance(i, Point))
-            self.assertEqual(0, i.z)
-
-
-class TestThreeDimensionShape(TestCase):
-
-    def test_generate_sides(self):
-        test_list = ['22.323232 -4.287282 20', '23.323232 -5.328723', '22.112333 -6.23789238923',
-                     '22.323232 -4.287282 20']
-        poly = Polyhedron(test_list, test_list, upper_layer=100)
-        self.assertTrue(isinstance(poly, Polyhedron))
-        self.assertTrue(isinstance(poly.sides, list))
-        self.assertEqual(4, len(poly.sides))
-
-    def test_to_kml(self):
-        test_list = ['22.323232 -4.287282 20', '23.323232 -5.328723', '22.112333 -6.23789238923']
-        poly = Polyhedron(test_list, test_list, upper_layer=100)
-        lower, upper, sides = poly.to_kml()
-
-        self.assertTrue(isinstance(lower, list))
+from unittest import TestCase
+
+from kmlplus.geo import Point
+from kmlplus.shapes import Circle, Polygon, Polyhedron
+
+
+class TestCircle(TestCase):
+    def setUp(self):
+        self.circle_height_args = Circle('55.1111 -3.2311 10', 10, sample=100, uom='M')
+        self.circle_height_kwargs = Circle('28.132212 2.332782', 10, sample=150, z=20, uom='M')
+
+    def test_create(self):
+        self.assertTrue(isinstance(self.circle_height_args.point_list, list))
+        self.assertEqual(len(self.circle_height_args.point_list), 101)
+        self.assertTrue(isinstance(self.circle_height_args.point_list[2], Point))
+        for i in self.circle_height_args.point_list:
+            self.assertEqual(10, i.z)
+
+        self.assertTrue(isinstance(self.circle_height_kwargs.point_list, list))
+        self.assertEqual(len(self.circle_height_kwargs.point_list), 151)
+        self.assertTrue(isinstance(self.circle_height_kwargs.point_list[2], Point))
+        for i in self.circle_height_kwargs.point_list:
+            self.assertEqual(i.z, 20)
+
+        # Test uom effects
+        c = Circle('55.1111 -3.2311 10', 10, sample=100, uom='FT')
+        for i in c:
+            self.assertEqual(10, i.z)
+
+        c = Circle('55.1111 -3.2311 10', 25, z=250, sample=100, uom='M')
+        for i in c:
+            self.assertEqual(250, i.z)
+
+
+class TestPolygon(TestCase):
+    def setUp(self):
+        pass
+
+    def test_new_layer(self):
+        test_coordinates_no_height = ['22.323232 -4.287282', '23.323232 -5.328723', '22.112333 -6.23789238923']
+        test_coordinates_with_height = ['22.323232 -4.287282 100', '23.323232 -5.328723 150',
+                                        '22.112333 -6.23789238923 200']
+        test_coordinates_with_height_override = ['22.323232 -4.287282', '23.323232 -5.328723',
+                                                 '22.112333 -6.23789238923']
+        test_coordinates_with_cw_arc = ['22.23232 -3.232323 0', 'start=21.23211 -4.122121, end=22.054541 -4.1111, z=15,'
+                                                                ' direction=clockwise']
+        test_coordinates_with_ccw_arc = ['22.23232 -3.232323 0', 'start=21.23211 -4.122121, end=22.054541 -4.1111, '
+                                                                 'z=15, direction=anticlockwise']
+        test_dms = ['554433N 0010203W', '443322N 0000102W', '443322N 0010102E']
+
+        # Tests for coordinates with no z value provided. Should default to 0.
+        result_no_height = Polygon(test_coordinates_no_height)
+
+        self.assertTrue(isinstance(result_no_height, Polygon))
+        self.assertEqual(len(result_no_height), 4)
+        for i in result_no_height:
+            self.assertEqual(i.z, 0)
+            self.assertTrue(isinstance(i, Point))
+
+        # Tests for coordinates with a user provided z value.
+        result_with_height = Polygon(test_coordinates_with_height)
+
+        self.assertTrue(isinstance(result_with_height, Polygon))
+        self.assertEqual(len(result_with_height), 4)
+        for i in result_with_height:
+            self.assertTrue(isinstance(i, Point))
+            self.assertNotEqual(i.z, 0.0)
+
+        # Test results for coordinates with height overridden.
+        result_with_height_override = Polygon(test_coordinates_with_height_override, z=500.11)
+
+        self.assertTrue(isinstance(result_with_height_override, Polygon))
+        self.assertEqual(len(result_with_height_override), 4)
+        for i in result_with_height_override:
+            self.assertTrue(isinstance(i, Point))
+            self.assertEqual(152.43352800000002, i.z)
+
+        # Test with DMS
+        result_dms_no_height = Polygon(test_dms)
+        self.assertTrue(isinstance(result_dms_no_height, Polygon))
+        self.assertEqual(4, len(result_dms_no_height))
+        for i in result_dms_no_height:
+            self.assertTrue(isinstance(i, Point))
+            self.assertEqual(0, i.z)
+
+        # Test with DD and curved segment
+        result_dd_arc = Polygon(test_coordinates_with_cw_arc)
+        self.assertTrue(isinstance(result_dd_arc, Polygon))
+        self.assertTrue(len(result_dd_arc) > 100)
+        for i in result_dd_arc:
+            self.assertTrue(isinstance(i, Point))
+            self.assertEqual(0, i.z)
+
+        result_dd_arc = Polygon(test_coordinates_with_ccw_arc)
+        self.assertTrue(isinstance(result_dd_arc, Polygon))
+        self.assertTrue(len(result_dd_arc) > 100)
+        for i in result_dd_arc:
+            self.assertTrue(isinstance(i, Point))
+            self.assertEqual(0, i.z)
+
+
+class TestThreeDimensionShape(TestCase):
+
+    def test_generate_sides(self):
+        test_list = ['22.323232 -4.287282 20', '23.323232 -5.328723', '22.112333 -6.23789238923',
+                     '22.323232 -4.287282 20']
+        poly = Polyhedron(test_list, test_list, upper_layer=100)
+        self.assertTrue(isinstance(poly, Polyhedron))
+        self.assertTrue(isinstance(poly.sides, list))
+        self.assertEqual(4, len(poly.sides))
+
+    def test_to_kml(self):
+        test_list = ['22.323232 -4.287282 20', '23.323232 -5.328723', '22.112333 -6.23789238923']
+        poly = Polyhedron(test_list, test_list, upper_layer=100)
+        lower, upper, sides = poly.to_kml()
+
+        self.assertTrue(isinstance(lower, list))
+
+
+class TestLineString(TestCase):
+    def test_create(self):
+        coordinates = ['554433N 0031113W', '440000S 110202']
```

