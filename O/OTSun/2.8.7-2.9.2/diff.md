# Comparing `tmp/OTSun-2.8.7.tar.gz` & `tmp/OTSun-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OTSun-2.8.7.tar", last modified: Fri May 14 14:59:07 2021, max compression
+gzip compressed data, was "OTSun-2.9.2.tar", last modified: Wed Nov 16 19:54:35 2022, max compression
```

## Comparing `OTSun-2.8.7.tar` & `OTSun-2.9.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 cardona    (501) staff       (20)        0 2021-05-14 14:59:07.000000 OTSun-2.8.7/
--rw-r--r--   0 cardona    (501) staff       (20)       48 2019-07-20 06:01:10.000000 OTSun-2.8.7/MANIFEST.in
-drwxr-xr-x   0 cardona    (501) staff       (20)        0 2021-05-14 14:59:07.000000 OTSun-2.8.7/OTSun.egg-info/
--rw-r--r--   0 cardona    (501) staff       (20)     1489 2021-05-14 14:59:07.000000 OTSun-2.8.7/OTSun.egg-info/PKG-INFO
--rw-r--r--   0 cardona    (501) staff       (20)      406 2021-05-14 14:59:07.000000 OTSun-2.8.7/OTSun.egg-info/SOURCES.txt
--rw-r--r--   0 cardona    (501) staff       (20)        1 2021-05-14 14:59:07.000000 OTSun-2.8.7/OTSun.egg-info/dependency_links.txt
--rw-r--r--   0 cardona    (501) staff       (20)       31 2021-05-14 14:59:07.000000 OTSun-2.8.7/OTSun.egg-info/requires.txt
--rw-r--r--   0 cardona    (501) staff       (20)        6 2021-05-14 14:59:07.000000 OTSun-2.8.7/OTSun.egg-info/top_level.txt
--rw-r--r--   0 cardona    (501) staff       (20)     1489 2021-05-14 14:59:07.000000 OTSun-2.8.7/PKG-INFO
--rw-r--r--   0 cardona    (501) staff       (20)      962 2020-10-26 12:35:06.000000 OTSun-2.8.7/README.md
-drwxr-xr-x   0 cardona    (501) staff       (20)        0 2021-05-14 14:59:07.000000 OTSun-2.8.7/otsun/
--rw-r--r--   0 cardona    (501) staff       (20)      326 2019-12-06 11:04:50.000000 OTSun-2.8.7/otsun/__init__.py
--rw-r--r--   0 cardona    (501) staff       (20)      497 2021-05-14 14:59:07.000000 OTSun-2.8.7/otsun/_version.py
--rw-r--r--   0 cardona    (501) staff       (20)     4187 2020-06-19 09:26:08.000000 OTSun-2.8.7/otsun/experiments.py
--rw-r--r--   0 cardona    (501) staff       (20)      136 2020-06-19 09:27:18.000000 OTSun-2.8.7/otsun/logging_unit.py
--rw-r--r--   0 cardona    (501) staff       (20)    54946 2021-02-24 10:11:29.000000 OTSun-2.8.7/otsun/materials.py
--rw-r--r--   0 cardona    (501) staff       (20)     8331 2020-10-26 12:01:40.000000 OTSun-2.8.7/otsun/math.py
--rw-r--r--   0 cardona    (501) staff       (20)    14365 2021-04-27 11:56:45.000000 OTSun-2.8.7/otsun/movements.py
--rw-r--r--   0 cardona    (501) staff       (20)    20454 2021-04-18 15:26:02.000000 OTSun-2.8.7/otsun/optics.py
--rw-r--r--   0 cardona    (501) staff       (20)     2806 2020-06-19 15:05:56.000000 OTSun-2.8.7/otsun/outputs.py
--rw-r--r--   0 cardona    (501) staff       (20)    12805 2021-01-21 09:57:51.000000 OTSun-2.8.7/otsun/ray.py
--rw-r--r--   0 cardona    (501) staff       (20)     6581 2020-10-28 10:20:23.000000 OTSun-2.8.7/otsun/scene.py
--rw-r--r--   0 cardona    (501) staff       (20)    13032 2021-01-24 20:42:23.000000 OTSun-2.8.7/otsun/source.py
--rw-r--r--   0 cardona    (501) staff       (20)      209 2021-05-14 14:59:07.000000 OTSun-2.8.7/setup.cfg
--rw-r--r--   0 cardona    (501) staff       (20)      746 2021-02-24 09:49:29.000000 OTSun-2.8.7/setup.py
--rw-r--r--   0 cardona    (501) staff       (20)    68611 2019-07-20 06:00:06.000000 OTSun-2.8.7/versioneer.py
+drwxr-xr-x   0 cardona    (501) staff       (20)        0 2022-11-16 19:54:35.684135 OTSun-2.9.2/
+-rw-r--r--   0 cardona    (501) staff       (20)     1082 2017-11-03 07:21:22.000000 OTSun-2.9.2/LICENSE.md
+-rw-r--r--   0 cardona    (501) staff       (20)       48 2019-07-20 06:01:10.000000 OTSun-2.9.2/MANIFEST.in
+drwxr-xr-x   0 cardona    (501) staff       (20)        0 2022-11-16 19:54:35.680375 OTSun-2.9.2/OTSun.egg-info/
+-rw-r--r--   0 cardona    (501) staff       (20)     1291 2022-11-16 19:54:35.000000 OTSun-2.9.2/OTSun.egg-info/PKG-INFO
+-rw-r--r--   0 cardona    (501) staff       (20)      417 2022-11-16 19:54:35.000000 OTSun-2.9.2/OTSun.egg-info/SOURCES.txt
+-rw-r--r--   0 cardona    (501) staff       (20)        1 2022-11-16 19:54:35.000000 OTSun-2.9.2/OTSun.egg-info/dependency_links.txt
+-rw-r--r--   0 cardona    (501) staff       (20)       31 2022-11-16 19:54:35.000000 OTSun-2.9.2/OTSun.egg-info/requires.txt
+-rw-r--r--   0 cardona    (501) staff       (20)        6 2022-11-16 19:54:35.000000 OTSun-2.9.2/OTSun.egg-info/top_level.txt
+-rw-r--r--   0 cardona    (501) staff       (20)     1291 2022-11-16 19:54:35.684203 OTSun-2.9.2/PKG-INFO
+-rw-r--r--   0 cardona    (501) staff       (20)      962 2020-10-26 12:35:06.000000 OTSun-2.9.2/README.md
+drwxr-xr-x   0 cardona    (501) staff       (20)        0 2022-11-16 19:54:35.684655 OTSun-2.9.2/otsun/
+-rw-r--r--   0 cardona    (501) staff       (20)      453 2022-01-06 18:25:42.000000 OTSun-2.9.2/otsun/__init__.py
+-rw-r--r--   0 cardona    (501) staff       (20)      497 2022-11-16 19:54:35.684688 OTSun-2.9.2/otsun/_version.py
+-rw-r--r--   0 cardona    (501) staff       (20)     4187 2020-06-19 09:26:08.000000 OTSun-2.9.2/otsun/experiments.py
+-rw-r--r--   0 cardona    (501) staff       (20)      136 2020-06-19 09:27:18.000000 OTSun-2.9.2/otsun/logging_unit.py
+-rw-r--r--   0 cardona    (501) staff       (20)    54946 2021-06-02 17:48:38.000000 OTSun-2.9.2/otsun/materials.py
+-rw-r--r--   0 cardona    (501) staff       (20)     8331 2020-10-26 12:01:40.000000 OTSun-2.9.2/otsun/math.py
+-rw-r--r--   0 cardona    (501) staff       (20)    14233 2022-04-01 11:12:29.000000 OTSun-2.9.2/otsun/movements.py
+-rw-r--r--   0 cardona    (501) staff       (20)    20458 2022-01-04 12:10:22.000000 OTSun-2.9.2/otsun/optics.py
+-rw-r--r--   0 cardona    (501) staff       (20)     2806 2020-06-19 15:05:56.000000 OTSun-2.9.2/otsun/outputs.py
+-rw-r--r--   0 cardona    (501) staff       (20)    13254 2022-10-25 10:26:12.000000 OTSun-2.9.2/otsun/ray.py
+-rw-r--r--   0 cardona    (501) staff       (20)     6583 2022-09-29 15:36:15.000000 OTSun-2.9.2/otsun/scene.py
+-rw-r--r--   0 cardona    (501) staff       (20)    13267 2022-06-25 09:24:56.000000 OTSun-2.9.2/otsun/source.py
+-rw-r--r--   0 cardona    (501) staff       (20)      209 2022-11-16 19:54:35.684519 OTSun-2.9.2/setup.cfg
+-rw-r--r--   0 cardona    (501) staff       (20)      746 2021-02-24 09:49:29.000000 OTSun-2.9.2/setup.py
+-rw-r--r--   0 cardona    (501) staff       (20)    68611 2019-07-20 06:00:06.000000 OTSun-2.9.2/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `OTSun-2.8.7/OTSun.egg-info/PKG-INFO` & `OTSun-2.9.2/OTSun.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: OTSun
-Version: 2.8.7
+Version: 2.9.2
 Summary: Analyzer of sun collectors
 Home-page: https://github.com/bielcardona/OTSun
 Author: Gabriel Cardona, Ramon Pujol
 Author-email: gabriel.cardona@uib.es, ramon.pujol@uib.es
 License: MIT
-Description: [![PyPI version](https://badge.fury.io/py/OTSun.svg)](https://badge.fury.io/py/OTSun)
-        
-        ![OTSun logo](logo_OTSun.png)
-        
-        # OTSun
-        
-        OTSun is a python package that uses the Monte Carlo Forward Ray Tracing for the optical analysis of Solar Thermal Collectors and Solar Cells. 
-        
-        ## Installation
-        
-        The package can be installed either from pypi:
-        `pip install otsun` or downloaded installed with `python setup.py install`.
-        
-        In order to use the package the libraries of FreeCAD (https://www.freecadweb.org/) must be available and included in your python path.
-        
-        ## Documentation
-        
-        The documentation of the module is available at http://otsun.readthedocs.io/
-        
-        ## How to cite OTSun?
-        
-        If you need to cite OTSun, please use the following reference:
-        
-        * Cardona G, Pujol-Nadal R (2020) OTSun, a python package for the optical analysis of solar-thermal collectors and photovoltaic cells with arbitrary geometry. PLoS ONE 15(10): e0240735. https://doi.org/10.1371/journal.pone.0240735
-        
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+[![PyPI version](https://badge.fury.io/py/OTSun.svg)](https://badge.fury.io/py/OTSun)
+
+![OTSun logo](logo_OTSun.png)
+
+# OTSun
+
+OTSun is a python package that uses the Monte Carlo Forward Ray Tracing for the optical analysis of Solar Thermal Collectors and Solar Cells. 
+
+## Installation
+
+The package can be installed either from pypi:
+`pip install otsun` or downloaded installed with `python setup.py install`.
+
+In order to use the package the libraries of FreeCAD (https://www.freecadweb.org/) must be available and included in your python path.
+
+## Documentation
+
+The documentation of the module is available at http://otsun.readthedocs.io/
+
+## How to cite OTSun?
+
+If you need to cite OTSun, please use the following reference:
+
+* Cardona G, Pujol-Nadal R (2020) OTSun, a python package for the optical analysis of solar-thermal collectors and photovoltaic cells with arbitrary geometry. PLoS ONE 15(10): e0240735. https://doi.org/10.1371/journal.pone.0240735
```

### Comparing `OTSun-2.8.7/PKG-INFO` & `OTSun-2.9.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: OTSun
-Version: 2.8.7
+Version: 2.9.2
 Summary: Analyzer of sun collectors
 Home-page: https://github.com/bielcardona/OTSun
 Author: Gabriel Cardona, Ramon Pujol
 Author-email: gabriel.cardona@uib.es, ramon.pujol@uib.es
 License: MIT
-Description: [![PyPI version](https://badge.fury.io/py/OTSun.svg)](https://badge.fury.io/py/OTSun)
-        
-        ![OTSun logo](logo_OTSun.png)
-        
-        # OTSun
-        
-        OTSun is a python package that uses the Monte Carlo Forward Ray Tracing for the optical analysis of Solar Thermal Collectors and Solar Cells. 
-        
-        ## Installation
-        
-        The package can be installed either from pypi:
-        `pip install otsun` or downloaded installed with `python setup.py install`.
-        
-        In order to use the package the libraries of FreeCAD (https://www.freecadweb.org/) must be available and included in your python path.
-        
-        ## Documentation
-        
-        The documentation of the module is available at http://otsun.readthedocs.io/
-        
-        ## How to cite OTSun?
-        
-        If you need to cite OTSun, please use the following reference:
-        
-        * Cardona G, Pujol-Nadal R (2020) OTSun, a python package for the optical analysis of solar-thermal collectors and photovoltaic cells with arbitrary geometry. PLoS ONE 15(10): e0240735. https://doi.org/10.1371/journal.pone.0240735
-        
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+[![PyPI version](https://badge.fury.io/py/OTSun.svg)](https://badge.fury.io/py/OTSun)
+
+![OTSun logo](logo_OTSun.png)
+
+# OTSun
+
+OTSun is a python package that uses the Monte Carlo Forward Ray Tracing for the optical analysis of Solar Thermal Collectors and Solar Cells. 
+
+## Installation
+
+The package can be installed either from pypi:
+`pip install otsun` or downloaded installed with `python setup.py install`.
+
+In order to use the package the libraries of FreeCAD (https://www.freecadweb.org/) must be available and included in your python path.
+
+## Documentation
+
+The documentation of the module is available at http://otsun.readthedocs.io/
+
+## How to cite OTSun?
+
+If you need to cite OTSun, please use the following reference:
+
+* Cardona G, Pujol-Nadal R (2020) OTSun, a python package for the optical analysis of solar-thermal collectors and photovoltaic cells with arbitrary geometry. PLoS ONE 15(10): e0240735. https://doi.org/10.1371/journal.pone.0240735
```

### Comparing `OTSun-2.8.7/README.md` & `OTSun-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `OTSun-2.8.7/otsun/experiments.py` & `OTSun-2.9.2/otsun/experiments.py`

 * *Files identical despite different names*

### Comparing `OTSun-2.8.7/otsun/materials.py` & `OTSun-2.9.2/otsun/materials.py`

 * *Files identical despite different names*

### Comparing `OTSun-2.8.7/otsun/math.py` & `OTSun-2.9.2/otsun/math.py`

 * *Files identical despite different names*

### Comparing `OTSun-2.8.7/otsun/movements.py` & `OTSun-2.9.2/otsun/movements.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,21 +62,19 @@
 
 
 def axial_rotation_from_axis_vector_and_image(axis_origin, axis_dir, vector0, vector1):
     angle = vector0.getAngle(vector1)
     return axial_rotation_from_axis_and_angle(axis_origin, axis_dir, angle)
 
 
-def biaxial_rotation_from_vector_and_image(
-        origin, vector_horizontal, vector_vertical,
-        current_normal, desired_normal):
-    # First rotate around vector_vertical, so that the image of vector_horizontal is orthogonal
+def biaxial_rotation_from_vector_and_image(origin, vector_v, vector_h, current_normal, desired_normal):
+    # First rotate around vector_h, so that the image of vector_v is orthogonal
     # to desired_normal
-    image_vector_horizontal = desired_normal.cross(vector_vertical)
-    g1 = axial_rotation_from_vector_and_image(origin, vector_horizontal, image_vector_horizontal)
+    image_vector_horizontal = desired_normal.cross(vector_h)
+    g1 = axial_rotation_from_vector_and_image(origin, vector_v, image_vector_horizontal)
     new_normal = apply_movement_to_vector(g1, current_normal)
     g2 = axial_rotation_from_vector_and_image(origin, new_normal, desired_normal)
     return g2.multiply(g1)
 
 
 def get_labels(obj):
     """Gets the different labels of a given FreeCAD object"""
@@ -135,45 +133,40 @@
 
 @traced(logger)
 class TwoOrthogonalAxialJoint(Joint):
     """
     Class used to represent joints with two orthogonal axis
     """
 
-    def __init__(self, axis_origin, axis_vector_horizontal, axis_vector_vertical=None):
+    def __init__(self, axis_origin, axis_vector_vertical, axis_vector_horizontal):
         self.axis_origin = axis_origin
+        self.axis_vector_vertical = axis_vector_vertical
         self.axis_vector_horizontal = axis_vector_horizontal
-        if axis_vector_vertical is None:
-            self.axis_vector_vertical = Base.Vector(0, 0, 1)
-        else:
-            self.axis_vector_vertical = axis_vector_vertical
 
     def compute_rotation_to_point(self, target, normal, light_direction):
         """
         Computes a rotation so that ray in the direction of light_direction is reflected and hits the target.
         """
         pointing = target - self.axis_origin
         pointing.normalize()
         light_unit = light_direction * 1.0
         light_unit.normalize()
         desired_normal = pointing - light_unit
-        return biaxial_rotation_from_vector_and_image(
-            self.axis_origin, self.axis_vector_horizontal, self.axis_vector_vertical,
-            normal, desired_normal)
+        return biaxial_rotation_from_vector_and_image(self.axis_origin, self.axis_vector_vertical,
+                                                      self.axis_vector_horizontal, normal, desired_normal)
 
     def compute_rotation_to_direction(self, normal, light_direction):
         """
         Computes a rotation so that ray in the direction of light_direction is returned to its origin.
         """
         light_unit = light_direction * 1.0
         light_unit.normalize()
         desired_normal = light_unit * (-1.0)
-        return biaxial_rotation_from_vector_and_image(
-            self.axis_origin, self.axis_vector_horizontal, self.axis_vector_vertical,
-            normal, desired_normal)
+        return biaxial_rotation_from_vector_and_image(self.axis_origin, self.axis_vector_vertical,
+                                                      self.axis_vector_horizontal, normal, desired_normal)
 
 
 @traced(logger)
 class CentralJoint(Joint):
     """
     Class used to represent joints that rotate around a point
     """
```

### Comparing `OTSun-2.8.7/otsun/optics.py` & `OTSun-2.9.2/otsun/optics.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         u = myrandom()
         if k_ran < k:
             theta = (-2. * sigma_1 ** 2. * np.log(u)) ** 0.5 / 1000.0 / rad
         else:
             theta = (-2. * sigma_2 ** 2. * np.log(u)) ** 0.5 / 1000.0 / rad
         v = self.direction
         axis_1 = normal.cross(self.direction)
-        rotation_1 = Base.Rotation(axis_1, theta)
+        rotation_1 = Base.Rotation(axis_1, 2 * theta)
         new_v1 = rotation_1.multVec(v)
         u = myrandom()
         phi = 360. * u
         axis_2 = v
         rotation_2 = Base.Rotation(axis_2, phi)
         new_v2 = rotation_2.multVec(new_v1)
         polarization_vector = self.polarization
```

### Comparing `OTSun-2.8.7/otsun/outputs.py` & `OTSun-2.9.2/otsun/outputs.py`

 * *Files identical despite different names*

### Comparing `OTSun-2.8.7/otsun/ray.py` & `OTSun-2.9.2/otsun/ray.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
             direction,
             Phenomenon.JUST_STARTED,
             vacuum_medium
         )
         self.optical_states = [state]
         self.current_solid = None
         self.last_normal = None
+        self.last_touched_face = None
         self.wavelength = wavelength
         self.energy = energy
         self.polarization_vectors = [polarization_vector]
         self.finished = False
         self.Th_absorbed = False
         self.PV_values = []
         self.PV_absorbed = []
@@ -192,31 +193,40 @@
         bb1 = shape_segment.BoundBox
         candidates = self.scene.faces
         feasible_faces = 0
         filtered_faces_1 = 0
         filtered_faces_2 = 0
         feasible_but_empty = 0
         for face in candidates:
+            if face == self.last_touched_face:
+                continue
             bb2 = face.BoundBox
             if not _ray_may_intersect_bb(bb2, p0, direction):
                 filtered_faces_1 += 1
                 continue
             if not _bb_intersects(bb1, bb2):
                 filtered_faces_2 += 1
                 continue
             feasible_faces += 1
             punts = face.section(shape_segment).Vertexes
             if not punts:
                 feasible_but_empty += 1
                 # logger.debug("feasible face but empty intersection")
-            for punt in punts:
-                intersections.append([punt.Point, face])
+            # material = self.scene.materials[face]
+            if face in self.scene.materials:
+                for punt in punts:
+                    intersections.append([punt.Point, face])
+            else:
+                for punt in punts:
+                    if p0.distanceToPoint(punt.Point) > self.scene.epsilon:
+                        intersections.append([punt.Point, face])
+
         logger.debug(f"Found {len(intersections)} points in {feasible_faces} faces. Filtered {filtered_faces_1}+{filtered_faces_2}. Feasible but empty {feasible_but_empty}")
-        intersections = [punt_cara for punt_cara in intersections if
-                         p0.distanceToPoint(punt_cara[0]) > 0] # self.scene.epsilon]
+#        intersections = [punt_cara for punt_cara in intersections if
+#                         p0.distanceToPoint(punt_cara[0]) > self.scene.epsilon]
         if not intersections:
             logger.debug("No true intersection found with scene")
             return p1, None
         closest_pair = min(intersections,
                            key=lambda pair: self.weighted_distance(p0, pair))
         return tuple(closest_pair)
 
@@ -305,14 +315,15 @@
             logger.debug("Ray running. Hop %s, %s, Solid %s", count, self,
                         self.scene.name_of_solid.get(self.current_solid, "Void"))
             count += 1
 
             # Find next intersection
             # Update points
             point, face = self.next_intersection()
+            self.last_touched_face = face
             self.points.append(point)
             if not face:
                 self.finished = True
                 self.Th_absorbed = False
                 break
 
             # Update energy
```

### Comparing `OTSun-2.8.7/otsun/scene.py` & `OTSun-2.9.2/otsun/scene.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             # self.faces.extend(faces)
             # # self.materials[obj] = material ## Cal?
             if not self.boundbox:
                 self.boundbox = obj.Shape.BoundBox
             else:
                 self.boundbox.add(obj.Shape.BoundBox)
 
-        self.remove_duplicate_faces()
+        # self.remove_duplicate_faces()
 
         self.diameter = self.boundbox.DiagonalLength
 
     def recompute_boundbox(self):
         """
         Recomputes the boundbox, so that all objects are contained in it
         """
```

### Comparing `OTSun-2.8.7/otsun/source.py` & `OTSun-2.9.2/otsun/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,22 +338,26 @@
         Function that interpolates by straight line segments the input data
     """
     CSR = CircumSolarRatio
     SD = 4.65
     # Solar Disk in mrad
     SS = 43.6
     # Solar Size in mrad
-    a1 = _calculate_a1(CSR, SD)
-    #     normalization constant for the disk region
-    a2 = _calculate_a2(CSR, SD, SS)
-    #    normalization constant for the circumsolar region
-    CDF_Disk_Region = _calculate_CDF_disk_region(a1, SD)
+    a2 = None # _calculate_a2(CSR, SD, SS)
+    CDF_Disk_Region = None # _calculate_CDF_disk_region(a1, SD)
     #    Buie distribution for the disk region
     u_values = np.arange(0.0, 1.001, 0.001)
     dist_values = []
     for u in u_values:
-        if u < 1.0 - CSR:
+        if u <= 1.0 - CSR:
+            if CDF_Disk_Region is None:
+                a1 = _calculate_a1(CSR, SD)
+                #     normalization constant for the disk region
+                CDF_Disk_Region = _calculate_CDF_disk_region(a1, SD)
             dist_values.append(_th_solar_disk_region(u, CDF_Disk_Region) / 1000.0 * 180.0 / np.pi)
         else:
+            if a2 is None:
+                a2 = _calculate_a2(CSR, SD, SS)
+                #    normalization constant for the circumsolar region
             dist_values.append(_th_circumsolar_region(u, CSR, SD, a2) / 1000.0 * 180.0 / np.pi)
     f = tabulated_function(u_values, dist_values)
     return f
```

### Comparing `OTSun-2.8.7/setup.py` & `OTSun-2.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `OTSun-2.8.7/versioneer.py` & `OTSun-2.9.2/versioneer.py`

 * *Files identical despite different names*

