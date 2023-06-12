# Comparing `tmp/pygfx-0.1.8.tar.gz` & `tmp/pygfx-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygfx-0.1.8.tar", last modified: Tue Apr 12 19:25:40 2022, max compression
+gzip compressed data, was "pygfx-0.1.9.tar", last modified: Wed Apr 20 11:08:16 2022, max compression
```

## Comparing `pygfx-0.1.8.tar` & `pygfx-0.1.9.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 19:25:40.783541 pygfx-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-04-12 19:25:31.000000 pygfx-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5823 2022-04-12 19:25:40.783541 pygfx-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5173 2022-04-12 19:25:31.000000 pygfx-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 19:25:40.775540 pygfx-0.1.8/pygfx/
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 19:25:40.779541 pygfx-0.1.8/pygfx/cameras/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/cameras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4016 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/cameras/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/cameras/_orthographic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2624 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/cameras/_perspective.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 19:25:40.779541 pygfx-0.1.8/pygfx/controllers/
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/controllers/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6989 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/controllers/_orbit.py
--rw-r--r--   0 runner    (1001) docker     (121)     4959 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/controllers/_panzoom.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 19:25:40.779541 pygfx-0.1.8/pygfx/geometries/
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/geometries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5594 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/geometries/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3168 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/geometries/_box.py
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/geometries/_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     6705 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/geometries/_cylinder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/geometries/_plane.py
--rw-r--r--   0 runner    (1001) docker     (121)    10205 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/geometries/_polyhedron.py
--rw-r--r--   0 runner    (1001) docker     (121)     2278 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/geometries/_sphere.py
--rw-r--r--   0 runner    (1001) docker     (121)     7103 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/geometries/_toroidal.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/geometries/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 19:25:40.779541 pygfx-0.1.8/pygfx/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/helpers/_axes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4211 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/helpers/_box.py
--rw-r--r--   0 runner    (1001) docker     (121)    30183 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/helpers/_gizmo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/helpers/_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 19:25:40.779541 pygfx-0.1.8/pygfx/linalg/
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/linalg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/linalg/cylindrical.py
--rw-r--r--   0 runner    (1001) docker     (121)     5407 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/linalg/euler.py
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/linalg/matrix3.py
--rw-r--r--   0 runner    (1001) docker     (121)    25021 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/linalg/matrix4.py
--rw-r--r--   0 runner    (1001) docker     (121)     9488 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/linalg/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/linalg/spherical.py
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/linalg/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12745 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/linalg/vector3.py
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/linalg/vector4.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 19:25:40.779541 pygfx-0.1.8/pygfx/materials/
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4012 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/materials/_background.py
--rw-r--r--   0 runner    (1001) docker     (121)     5461 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/materials/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/materials/_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     3439 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/materials/_line.py
--rw-r--r--   0 runner    (1001) docker     (121)     9634 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/materials/_mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)     3271 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/materials/_points.py
--rw-r--r--   0 runner    (1001) docker     (121)     2555 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/materials/_volume.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 19:25:40.783541 pygfx-0.1.8/pygfx/objects/
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15719 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/objects/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    13118 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/objects/_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/objects/_instanced.py
--rw-r--r--   0 runner    (1001) docker     (121)     4150 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/objects/_more.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 19:25:40.783541 pygfx-0.1.8/pygfx/renderers/
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4358 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 19:25:40.783541 pygfx-0.1.8/pygfx/renderers/svg/
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/svg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/svg/_svgrenderer.py
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/svg/linerender.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 19:25:40.783541 pygfx-0.1.8/pygfx/renderers/wgpu/
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/wgpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27097 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/wgpu/_blender.py
--rw-r--r--   0 runner    (1001) docker     (121)     9332 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/wgpu/_flusher.py
--rw-r--r--   0 runner    (1001) docker     (121)    21920 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/wgpu/_pipelinebuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)    32565 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/wgpu/_renderer.py
--rw-r--r--   0 runner    (1001) docker     (121)    27048 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/wgpu/_shadercomposer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6713 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/wgpu/_update.py
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/wgpu/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6061 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/wgpu/backgroundrender.py
--rw-r--r--   0 runner    (1001) docker     (121)     9678 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/wgpu/imagerender.py
--rw-r--r--   0 runner    (1001) docker     (121)    28574 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/wgpu/linerender.py
--rw-r--r--   0 runner    (1001) docker     (121)    30530 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/wgpu/meshrender.py
--rw-r--r--   0 runner    (1001) docker     (121)    10364 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/wgpu/pointsrender.py
--rw-r--r--   0 runner    (1001) docker     (121)    24231 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/renderers/wgpu/volumerender.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 19:25:40.783541 pygfx-0.1.8/pygfx/resources/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7355 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/resources/_buffer.py
--rw-r--r--   0 runner    (1001) docker     (121)    12125 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/resources/_texture.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 19:25:40.783541 pygfx-0.1.8/pygfx/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    51540 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/utils/_cmdata_mpl.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/utils/cm.py
--rw-r--r--   0 runner    (1001) docker     (121)    12712 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/utils/color.py
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/utils/show.py
--rw-r--r--   0 runner    (1001) docker     (121)     2188 2022-04-12 19:25:31.000000 pygfx-0.1.8/pygfx/utils/viewport.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 19:25:40.775540 pygfx-0.1.8/pygfx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5823 2022-04-12 19:25:40.000000 pygfx-0.1.8/pygfx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2301 2022-04-12 19:25:40.000000 pygfx-0.1.8/pygfx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-12 19:25:40.000000 pygfx-0.1.8/pygfx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-04-12 19:25:40.000000 pygfx-0.1.8/pygfx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-12 19:25:40.000000 pygfx-0.1.8/pygfx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-12 19:25:40.000000 pygfx-0.1.8/pygfx.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-04-12 19:25:40.787541 pygfx-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-04-12 19:25:31.000000 pygfx-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.576012 pygfx-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-04-20 11:08:07.000000 pygfx-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     6059 2022-04-20 11:08:16.576012 pygfx-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5364 2022-04-20 11:08:07.000000 pygfx-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.568012 pygfx-0.1.9/pygfx/
+-rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.568012 pygfx-0.1.9/pygfx/cameras/
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/cameras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4016 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/cameras/_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/cameras/_orthographic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2624 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/cameras/_perspective.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.568012 pygfx-0.1.9/pygfx/controllers/
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/controllers/_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/controllers/_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5707 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/controllers/_panzoom.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.572012 pygfx-0.1.9/pygfx/geometries/
+-rw-r--r--   0 runner    (1001) docker     (121)      728 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5594 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3168 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/_box.py
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6705 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/_cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/_plane.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10205 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/_polyhedron.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2278 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7103 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/_toroidal.py
+-rw-r--r--   0 runner    (1001) docker     (121)      471 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/geometries/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.572012 pygfx-0.1.9/pygfx/helpers/
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/helpers/_axes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4211 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/helpers/_box.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30183 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/helpers/_gizmo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/helpers/_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.572012 pygfx-0.1.9/pygfx/linalg/
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/cylindrical.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5407 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/euler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      675 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/matrix3.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25021 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/matrix4.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9488 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/spherical.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12745 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/vector3.py
+-rw-r--r--   0 runner    (1001) docker     (121)      866 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/linalg/vector4.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.572012 pygfx-0.1.9/pygfx/materials/
+-rw-r--r--   0 runner    (1001) docker     (121)      871 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4012 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/materials/_background.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5461 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/materials/_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/materials/_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3439 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/materials/_line.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9634 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/materials/_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3271 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/materials/_points.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2555 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/materials/_volume.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.572012 pygfx-0.1.9/pygfx/objects/
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15719 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/objects/_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14690 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/objects/_events.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/objects/_instanced.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4150 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/objects/_more.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.572012 pygfx-0.1.9/pygfx/renderers/
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4358 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.572012 pygfx-0.1.9/pygfx/renderers/svg/
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/svg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/svg/_svgrenderer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      676 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/svg/linerender.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.576012 pygfx-0.1.9/pygfx/renderers/wgpu/
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27254 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/_blender.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9330 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/_flusher.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21920 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/_pipelinebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32563 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26709 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/_shadercomposer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6713 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/_update.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2393 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6052 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/backgroundrender.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9669 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/imagerender.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28530 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/linerender.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30402 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/meshrender.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10356 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/pointsrender.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24215 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/renderers/wgpu/volumerender.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.576012 pygfx-0.1.9/pygfx/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7355 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/resources/_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12125 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/resources/_texture.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.576012 pygfx-0.1.9/pygfx/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51540 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/utils/_cmdata_mpl.py
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/utils/cm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12712 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/utils/show.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2188 2022-04-20 11:08:07.000000 pygfx-0.1.9/pygfx/utils/viewport.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 11:08:16.568012 pygfx-0.1.9/pygfx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6059 2022-04-20 11:08:16.000000 pygfx-0.1.9/pygfx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2301 2022-04-20 11:08:16.000000 pygfx-0.1.9/pygfx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 11:08:16.000000 pygfx-0.1.9/pygfx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-04-20 11:08:16.000000 pygfx-0.1.9/pygfx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-20 11:08:16.000000 pygfx-0.1.9/pygfx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 11:08:16.000000 pygfx-0.1.9/pygfx.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-04-20 11:08:16.576012 pygfx-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-04-20 11:08:07.000000 pygfx-0.1.9/setup.py
```

### Comparing `pygfx-0.1.8/LICENSE` & `pygfx-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/PKG-INFO` & `pygfx-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: pygfx
-Version: 0.1.8
+Version: 0.1.9
 Summary: A threejs-like render engine based on wgpu
 Home-page: https://github.com/pygfx/pygfx
 Author: Almar Klein
 Author-email: almar.klein@gmail.com
 License: BSD 2-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: examples
 License-File: LICENSE
 
 [![CI](https://github.com/pygfx/pygfx/workflows/CI/badge.svg)](https://github.com/pygfx/pygfx/actions)
 [![Documentation Status](https://readthedocs.org/projects/pygfx/badge/?version=latest)](https://pygfx.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/pygfx.svg)](https://badge.fury.io/py/pygfx)
 
 # pygfx
@@ -107,14 +109,19 @@
 ## Current status
 
 Under development, many things can change.
 
 
 ## Testing examples
 
+The test suite is divided into two parts; unit tests for the core, and unit tests for the examples.
+
+* `pytest -v tests` runs the core unit tests.
+* `pytest -v examples` tests the examples.
+
 There are two types of tests for examples included with pygfx:
 
 ### Type 1: Checking if examples can run
 
 When running the test suite, pytest will run every example in a subprocess,
 to see if it can run and exit cleanly. You can opt out of this mechanism by including the comment
 `# run_example = false` in the module.
```

### Comparing `pygfx-0.1.8/README.md` & `pygfx-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,19 @@
 ## Current status
 
 Under development, many things can change.
 
 
 ## Testing examples
 
+The test suite is divided into two parts; unit tests for the core, and unit tests for the examples.
+
+* `pytest -v tests` runs the core unit tests.
+* `pytest -v examples` tests the examples.
+
 There are two types of tests for examples included with pygfx:
 
 ### Type 1: Checking if examples can run
 
 When running the test suite, pytest will run every example in a subprocess,
 to see if it can run and exit cleanly. You can opt out of this mechanism by including the comment
 `# run_example = false` in the module.
```

### Comparing `pygfx-0.1.8/pygfx/__init__.py` & `pygfx-0.1.9/pygfx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from .utils.color import Color
 from .utils.show import show
 from .utils.viewport import Viewport
 from .utils import cm
 
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 version_info = tuple(map(int, __version__.split(".")))
 
 
 # Elements of this library are derived from three.js, original license
 # at time of writing copied here:
 # ---
 # The MIT License
```

### Comparing `pygfx-0.1.8/pygfx/cameras/_base.py` & `pygfx-0.1.9/pygfx/cameras/_base.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/cameras/_orthographic.py` & `pygfx-0.1.9/pygfx/cameras/_orthographic.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/cameras/_perspective.py` & `pygfx-0.1.9/pygfx/cameras/_perspective.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/controllers/_base.py` & `pygfx-0.1.9/pygfx/controllers/_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 from ..utils.viewport import Viewport
 from ..renderers import Renderer
 
 
 class Controller:
     """Base camera controller."""
 
+    def get_view(self):
+        raise NotImplementedError()
+
+    def handle_event(self, event, viewport, camera):
+        raise NotImplementedError()
+
+    def save_state(self):
+        raise NotImplementedError()
+
+    def load_state(self, state=None):
+        raise NotImplementedError()
+
     def update_camera(self, camera: "Camera") -> "Controller":
         """Update the transform of the camera with the internal transform."""
         rot, pos, zoom = self.get_view()
         camera.rotation.copy(rot)
         camera.position.copy(pos)
         camera.zoom = zoom
         return self
@@ -27,17 +39,14 @@
             lambda event: self.handle_event(event, viewport, camera),
             "pointer_down",
             "pointer_move",
             "pointer_up",
             "wheel",
         )
 
-    def handle_event(self, event, viewport, camera):
-        raise NotImplementedError()
-
 
 def get_screen_vectors_in_world_cords(
     center_world: Vector3, scene_size: Tuple[float, float], camera: "Camera"
 ) -> Tuple[Vector3, Vector3]:
     """Given a reference center location (in 3D world coordinates)
     Get the vectors corresponding to the x and y direction in screen coordinates.
     These vectors are scaled so that they can simply be multiplied with the
```

### Comparing `pygfx-0.1.8/pygfx/controllers/_orbit.py` & `pygfx-0.1.9/pygfx/controllers/_orbit.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,21 +41,52 @@
         self._orbit_up = Vector3(0, 1, 0)
         self._s = Spherical()
 
         # Initialize orientation
         self.look_at(eye, target, up)
         self._initial_distance = self.distance
 
+        # Save initial state
+        self.save_state()
+
+    def save_state(self):
+        self._saved_state = {
+            "rotation": self.rotation.clone(),
+            "distance": self.distance,
+            "target": self.target.clone(),
+            "up": self.up.clone(),
+            "zoom_changes_distance": self.zoom_changes_distance,
+            "zoom_value": self.zoom_value,
+            "min_zoom": self.min_zoom,
+            "initial_distance": self._initial_distance,
+        }
+        return self._saved_state
+
+    def load_state(self, state=None):
+        state = state or self._saved_state
+        self.rotation = state["rotation"].clone()
+        self.distance = state["distance"]
+        self.target = state["target"].clone()
+        self.up = state["up"].clone()
+        self.zoom_changes_distance = state["zoom_changes_distance"]
+        self.zoom_value = state["zoom_value"]
+        self.min_zoom = state["min_zoom"]
+        self.initial_distance = state["initial_distance"]
+        self._update_up_quats()
+
+    def _update_up_quats(self):
+        self._up_quat = Quaternion().set_from_unit_vectors(self.up, self._orbit_up)
+        self._up_quat_inv = self._up_quat.clone().inverse()
+
     def look_at(self, eye: Vector3, target: Vector3, up: Vector3) -> Controller:
         self.distance = eye.distance_to(target)
         self.target = target
         self.up = up
         self.rotation.set_from_rotation_matrix(self._m.look_at(eye, target, up))
-        self._up_quat = Quaternion().set_from_unit_vectors(self.up, self._orbit_up)
-        self._up_quat_inv = self._up_quat.clone().inverse()
+        self._update_up_quats()
         return self
 
     def pan(self, vec3: Vector3) -> Controller:
         """Pan in 3D world coordinates."""
         self.target.add(vec3)
         return self
```

### Comparing `pygfx-0.1.8/pygfx/controllers/_panzoom.py` & `pygfx-0.1.9/pygfx/controllers/_panzoom.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,14 +32,37 @@
         # Temp objects (to avoid garbage collection)
         self._m = Matrix4()
         self._v = Vector3()
 
         # Initialize orientation
         self.look_at(eye, target, up)
 
+        # Save initial state
+        self.save_state()
+
+    def save_state(self):
+        self._saved_state = {
+            "rotation": self.rotation.clone(),
+            "distance": self.distance,
+            "target": self.target.clone(),
+            "up": self.up.clone(),
+            "zoom_value": self.zoom_value,
+            "min_zoom": self.min_zoom,
+        }
+        return self._saved_state
+
+    def load_state(self, state=None):
+        state = state or self._saved_state
+        self.rotation = state["rotation"].clone()
+        self.distance = state["distance"]
+        self.target = state["target"].clone()
+        self.up = state["up"].clone()
+        self.zoom_value = state["zoom_value"]
+        self.min_zoom = state["min_zoom"]
+
     def look_at(self, eye: Vector3, target: Vector3, up: Vector3) -> Controller:
         self.distance = eye.distance_to(target)
         self.target = target
         self.up = up
         self.rotation.set_from_rotation_matrix(self._m.look_at(eye, target, up))
         return self
```

### Comparing `pygfx-0.1.8/pygfx/geometries/__init__.py` & `pygfx-0.1.9/pygfx/geometries/__init__.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/geometries/_base.py` & `pygfx-0.1.9/pygfx/geometries/_base.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/geometries/_box.py` & `pygfx-0.1.9/pygfx/geometries/_box.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/geometries/_compat.py` & `pygfx-0.1.9/pygfx/geometries/_compat.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/geometries/_cylinder.py` & `pygfx-0.1.9/pygfx/geometries/_cylinder.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/geometries/_plane.py` & `pygfx-0.1.9/pygfx/geometries/_plane.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/geometries/_polyhedron.py` & `pygfx-0.1.9/pygfx/geometries/_polyhedron.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/geometries/_sphere.py` & `pygfx-0.1.9/pygfx/geometries/_sphere.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/geometries/_toroidal.py` & `pygfx-0.1.9/pygfx/geometries/_toroidal.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/helpers/_axes.py` & `pygfx-0.1.9/pygfx/helpers/_axes.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/helpers/_box.py` & `pygfx-0.1.9/pygfx/helpers/_box.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/helpers/_gizmo.py` & `pygfx-0.1.9/pygfx/helpers/_gizmo.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/helpers/_grid.py` & `pygfx-0.1.9/pygfx/helpers/_grid.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/linalg/euler.py` & `pygfx-0.1.9/pygfx/linalg/euler.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/linalg/matrix3.py` & `pygfx-0.1.9/pygfx/linalg/matrix3.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/linalg/matrix4.py` & `pygfx-0.1.9/pygfx/linalg/matrix4.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/linalg/quaternion.py` & `pygfx-0.1.9/pygfx/linalg/quaternion.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/linalg/spherical.py` & `pygfx-0.1.9/pygfx/linalg/spherical.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/linalg/utils.py` & `pygfx-0.1.9/pygfx/linalg/utils.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/linalg/vector3.py` & `pygfx-0.1.9/pygfx/linalg/vector3.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/linalg/vector4.py` & `pygfx-0.1.9/pygfx/linalg/vector4.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/materials/__init__.py` & `pygfx-0.1.9/pygfx/materials/__init__.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/materials/_background.py` & `pygfx-0.1.9/pygfx/materials/_background.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/materials/_base.py` & `pygfx-0.1.9/pygfx/materials/_base.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/materials/_image.py` & `pygfx-0.1.9/pygfx/materials/_image.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/materials/_line.py` & `pygfx-0.1.9/pygfx/materials/_line.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/materials/_mesh.py` & `pygfx-0.1.9/pygfx/materials/_mesh.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/materials/_points.py` & `pygfx-0.1.9/pygfx/materials/_points.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/materials/_volume.py` & `pygfx-0.1.9/pygfx/materials/_volume.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/objects/_base.py` & `pygfx-0.1.9/pygfx/objects/_base.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/objects/_events.py` & `pygfx-0.1.9/pygfx/objects/_events.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     # Keyboard
     KEY_DOWN = "key_down"
     KEY_UP = "key_up"
     # Pointer
     POINTER_DOWN = "pointer_down"
     POINTER_MOVE = "pointer_move"
     POINTER_UP = "pointer_up"
+    POINTER_ENTER = "pointer_enter"
+    POINTER_LEAVE = "pointer_leave"
     CLICK = "click"
     DOUBLE_CLICK = "double_click"
     # Wheel
     WHEEL = "wheel"
     # Window
     CLOSE = "close"
     RESIZE = "resize"
@@ -146,34 +148,35 @@
         self.modifiers = modifiers or ()
         self.ntouches = ntouches
         self.touches = touches or {}
         self.pick_info = pick_info or {}
         self.clicks = clicks
         self.pointer_id = pointer_id
 
-    def copy(self, type, clicks):
-        result = PointerEvent(
-            type=type,
+    def copy(self, **kwargs):
+        values = dict(
+            type=self.type,
             x=self.x,
             y=self.y,
             button=self.button,
             buttons=self.buttons,
             modifiers=self.modifiers,
             ntouches=self.ntouches,
             touches=self.touches,
             pick_info=self.pick_info,
-            clicks=clicks,
+            clicks=self.clicks,
             pointer_id=self.pointer_id,
             bubbles=self.bubbles,
             target=self.target,
             cancelled=self.cancelled,
             time_stamp=self.time_stamp,
             root=self.root,
         )
-        return result
+        values.update(kwargs)
+        return PointerEvent(**values)
 
 
 class WheelEvent(PointerEvent):
     def __init__(self, *args, dx, dy, **kwargs):
         super().__init__(*args, **kwargs)
         self.dx = dx
         self.dy = dy
@@ -291,14 +294,16 @@
 
 
 class RootEventHandler(EventTarget):
     """Root event handler for the Pygfx event system."""
 
     # Dictionary to track clicks, keyed on pointer_id
     click_tracker = {}
+    # Dictionary to track targets, keyed on pointer_id
+    target_tracker = {}
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def dispatch_event(self, event: Event):
         """Dispatch the given event.
 
@@ -329,15 +334,38 @@
             captured_target = EventTarget.pointer_captures.get(pointer_id)
             # Encountered an event with pointer_id while there is a
             # capture active, so don't bubble, and retarget the event
             # to the captured target
             event._retarget(captured_target)
             event.stop_propagation()
 
+        # Current target is either something that was under the pointer, or nothing
+        # in which case we set the target to the root event handler (self)
         target = event.target or self
+
+        # Update the target tracker on all `pointer_move` events
+        if event.type == EventType.POINTER_MOVE:
+            # Get the previous target for this pointer (if any)
+            previous_target_ref = RootEventHandler.target_tracker.get(pointer_id)
+            previous_target = (previous_target_ref and previous_target_ref()) or None
+            # Check if the target has changed since the previous move event
+            if previous_target is not target:
+                # Update the current target for this pointer
+                RootEventHandler.target_tracker[pointer_id] = (
+                    target and ref(target)
+                ) or None
+                if previous_target is not None:
+                    # Dispatch a `pointer_leave` event for the previous target
+                    ev = event.copy(type="pointer_leave", target=previous_target)
+                    self.dispatch_event(ev)
+                # Dispatch a `pointer_enter` event for the new target
+                ev = event.copy(type="pointer_enter")
+                self.dispatch_event(ev)
+
+        # Dispatch the event to target and bubble up the hierarchy
         while target:
             # Update the current target
             event._update_current_target(target)
             target.handle_event(event)
             if pointer_id is not None and pointer_id in EventTarget.pointer_captures:
                 event._retarget(target)
                 event.stop_propagation()
@@ -380,12 +408,14 @@
             tracked_click = RootEventHandler.click_tracker.get(pointer_id)
             if tracked_click and (
                 tracked_click["target"] is not None
                 and tracked_click["target"]() is not None
                 and tracked_click["target"]() is event.target
                 or (tracked_click["target"] is None and event.target is None)
             ):
-                ev = event.copy("click", tracked_click["count"])
+                ev = event.copy(type="click", clicks=tracked_click["count"])
                 self.dispatch_event(ev)
                 if tracked_click["count"] == 2:
-                    double_ev = event.copy("double_click", tracked_click["count"])
+                    double_ev = event.copy(
+                        type="double_click", clicks=tracked_click["count"]
+                    )
                     self.dispatch_event(double_ev)
```

### Comparing `pygfx-0.1.8/pygfx/objects/_instanced.py` & `pygfx-0.1.9/pygfx/objects/_instanced.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/objects/_more.py` & `pygfx-0.1.9/pygfx/objects/_more.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/renderers/_base.py` & `pygfx-0.1.9/pygfx/renderers/_base.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/renderers/svg/_svgrenderer.py` & `pygfx-0.1.9/pygfx/renderers/svg/_svgrenderer.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/renderers/svg/linerender.py` & `pygfx-0.1.9/pygfx/renderers/svg/linerender.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/renderers/wgpu/_blender.py` & `pygfx-0.1.9/pygfx/renderers/wgpu/_blender.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,54 +85,55 @@
                 "blend": None,
                 "write_mask": wgpu.ColorWrite.ALL,
             },
         ]
 
     def get_color_attachments(self, blender, clear_color):
         if clear_color:
-            color_load_value = 0, 0, 0, 0
-            pick_load_value = 0, 0, 0, 0
+            color_load_op = pick_load_op = wgpu.LoadOp.clear
         else:
-            color_load_value = wgpu.LoadOp.load
-            pick_load_value = wgpu.LoadOp.load
+            color_load_op = pick_load_op = wgpu.LoadOp.load
 
         return [
             {
                 "view": blender.color_view,
                 "resolve_target": None,
-                "load_value": color_load_value,
+                "clear_value": (0, 0, 0, 0),
+                "load_op": color_load_op,
                 "store_op": wgpu.StoreOp.store,
             },
             {
                 "view": blender.pick_view,
                 "resolve_target": None,
-                "load_value": pick_load_value,
+                "clear_value": (0, 0, 0, 0),
+                "load_op": pick_load_op,
                 "store_op": wgpu.StoreOp.store,
             },
         ]
 
     def get_depth_descriptor(self, blender):
         return {
             "format": blender.depth_format,
             "depth_write_enabled": True,
             "depth_compare": wgpu.CompareFunction.less,
         }
 
     def get_depth_attachment(self, blender):
         return {
             "view": blender.depth_view,
-            "depth_load_value": 1.0,
+            "depth_clear_value": 1.0,
+            "depth_load_op": wgpu.LoadOp.clear,
             "depth_store_op": wgpu.StoreOp.store,
         }
 
     def get_shader_code(self, blender):
         return """
         struct FragmentOutput {
-            [[location(0)]] color: vec4<f32>;
-            [[location(1)]] pick: vec4<u32>;
+            @location(0) color: vec4<f32>,
+            @location(1) pick: vec4<u32>,
         };
         fn get_fragment_output(depth: f32, color: vec4<f32>) -> FragmentOutput {
             if (color.a < 1.0) { discard; }
             var out : FragmentOutput;
             out.color = vec4<f32>(color.rgb, 1.0);
             return out;
         }
@@ -143,16 +144,16 @@
     """A pass that considers all fragments opaque."""
 
     render_mask = 3  # opaque end transparent
 
     def get_shader_code(self, blender):
         return """
         struct FragmentOutput {
-            [[location(0)]] color: vec4<f32>;
-            [[location(1)]] pick: vec4<u32>;
+            @location(0) color: vec4<f32>,
+            @location(1) pick: vec4<u32>,
         };
         fn get_fragment_output(depth: f32, color: vec4<f32>) -> FragmentOutput {
             var out : FragmentOutput;
             out.color = vec4<f32>(color.rgb, 1.0);  // always opaque
             return out;
         }
         """
@@ -181,16 +182,16 @@
             },
         ]
 
     def get_shader_code(self, blender):
         # Take depth into account, but don't treat transparent fragments differently
         return """
         struct FragmentOutput {
-            [[location(0)]] color: vec4<f32>;
-            [[location(1)]] pick: vec4<u32>;
+            @location(0) color: vec4<f32>,
+            @location(1) pick: vec4<u32>,
         };
         fn get_fragment_output(depth: f32, color: vec4<f32>) -> FragmentOutput {
             var out : FragmentOutput;
             out.color = vec4<f32>(color.rgb * color.a, color.a);
             return out;
         }
         """
@@ -219,37 +220,37 @@
 
     def get_color_attachments(self, blender, clear_color):
         # Renders into the color_view, which is already cleared in an earlier pass
         return [
             {
                 "view": blender.color_view,
                 "resolve_target": None,
-                "load_value": wgpu.LoadOp.load,
+                "load_op": wgpu.LoadOp.load,
                 "store_op": wgpu.StoreOp.store,
             },
         ]
 
     def get_depth_descriptor(self, blender):
         return {
             "format": blender.depth_format,
             "depth_write_enabled": False,
             "depth_compare": wgpu.CompareFunction.less,
         }
 
     def get_depth_attachment(self, blender):
         return {
             "view": blender.depth_view,
-            "depth_load_value": wgpu.LoadOp.load,
+            "depth_load_op": wgpu.LoadOp.load,
             "depth_store_op": wgpu.StoreOp.discard,
         }
 
     def get_shader_code(self, blender):
         return """
         struct FragmentOutput {
-            [[location(0)]] color: vec4<f32>;
+            @location(0) color: vec4<f32>,
         };
         fn get_fragment_output(depth: f32, color: vec4<f32>) -> FragmentOutput {
             if (color.a <= 0.0) { discard; }
             var out : FragmentOutput;
             out.color = vec4<f32>(color.rgb * color.a, color.a);
             return out;
         }
@@ -304,50 +305,52 @@
                 },
                 "write_mask": wgpu.ColorWrite.ALL,
             },
         ]
 
     def get_color_attachments(self, blender, clear_color):
         # We always clear, the clear_color only really applies to the main color buffer.
-        accum_load_value = 0, 0, 0, 0
-        reveal_load_value = 1, 0, 0, 0
+        accum_clear_value = 0, 0, 0, 0
+        reveal_clear_value = 1, 0, 0, 0
         return [
             {
                 "view": blender.accum_view,
                 "resolve_target": None,
-                "load_value": accum_load_value,
+                "clear_value": accum_clear_value,
+                "load_op": wgpu.logger.clear,
                 "store_op": wgpu.StoreOp.store,
             },
             {
                 "view": blender.reveal_view,
                 "resolve_target": None,
-                "load_value": reveal_load_value,
+                "clear_value": reveal_clear_value,
+                "load_op": wgpu.logger.clear,
                 "store_op": wgpu.StoreOp.store,
             },
         ]
 
     def get_depth_descriptor(self, blender):
         return {
             "format": blender.depth_format,
             "depth_write_enabled": False,
             "depth_compare": wgpu.CompareFunction.less,
         }
 
     def get_depth_attachment(self, blender):
         return {
             "view": blender.depth_view,
-            "depth_load_value": wgpu.LoadOp.load,
+            "depth_load_op": wgpu.LoadOp.load,
             "depth_store_op": wgpu.StoreOp.discard,
         }
 
     def get_shader_code(self, blender):
         return """
         struct FragmentOutput {
-            [[location(0)]] accum: vec4<f32>;
-            [[location(1)]] reveal: f32;
+            @location(0) accum: vec4<f32>,
+            @location(1) reveal: f32,
         };
         fn get_fragment_output(depth: f32, color: vec4<f32>) -> FragmentOutput {
             if (color.a <= 0.0) { discard; }
             let premultiplied = color.rgb * color.a;
             let alpha = color.a;  // could take user-specified transmittance into account
             WEIGHT_CODE
             var out : FragmentOutput;
@@ -378,43 +381,44 @@
                 },
                 "write_mask": wgpu.ColorWrite.ALL,
             },
         ]
 
     def get_color_attachments(self, blender, clear_color):
         # We always clear, the clear_color only really applies to the main color buffer.
-        color_load_value = 0, 0, 0, 0
         return [
             {
                 "view": blender.frontcolor_view,
                 "resolve_target": None,
-                "load_value": color_load_value,
+                "clear_value": (0, 0, 0, 0),
+                "load_op": wgpu.LoadOp.clear,
                 "store_op": wgpu.StoreOp.store,
             },
         ]
 
     def get_depth_descriptor(self, blender):
         return {
             "format": blender.depth_format,
             "depth_write_enabled": True,
             "depth_compare": wgpu.CompareFunction.less,
         }
 
     def get_depth_attachment(self, blender):
         return {
             "view": blender.depth_view,
-            "depth_load_value": 1.0,
+            "depth_clear_value": 1.0,
+            "depth_load_op": wgpu.LoadOp.clear,
             "depth_store_op": wgpu.StoreOp.store,
         }
 
     def get_shader_code(self, blender):
         return """
         struct FragmentOutput {
-            [[location(0)]] color: vec4<f32>;
-            [[location(1)]] pick: vec4<u32>;
+            @location(0) color: vec4<f32>,
+            @location(1) pick: vec4<u32>,
         };
         fn get_fragment_output(depth: f32, color: vec4<f32>) -> FragmentOutput {
             if (color.a <= 0.0 || color.a >= 1.0) { discard; }
             var out : FragmentOutput;
             out.color = vec4<f32>(color.rgb * color.a, color.a);
             return out;
         }
@@ -529,25 +533,25 @@
 
         # Render
         render_pass = command_encoder.begin_render_pass(
             color_attachments=[
                 {
                     "view": self.color_view,
                     "resolve_target": None,
-                    "load_value": wgpu.LoadOp.load,
+                    "load_op": wgpu.LoadOp.load,
                     "store_op": wgpu.StoreOp.store,
                 }
             ],
             depth_stencil_attachment=None,
             occlusion_query_set=None,
         )
         render_pass.set_pipeline(render_pipeline)
         render_pass.set_bind_group(0, bind_group, [], 0, 99)
         render_pass.draw(4, 1)
-        render_pass.end_pass()
+        render_pass.end()
 
         return [command_encoder.finish()]
 
     def _create_combination_pipeline(self, device):
         """Overload this to setup the specific combiner-pass."""
         return None, None
 
@@ -646,17 +650,17 @@
                     "alpha": (bf.one, bf.one_minus_src_alpha, bo.add),
                     "color": (bf.one, bf.one_minus_src_alpha, bo.add),
                 },
             },
         ]
 
         bindings_code = """
-            [[group(0), binding(0)]]
+            @group(0) @binding(0)
             var r_accum: texture_2d<f32>;
-            [[group(0), binding(1)]]
+            @group(0) @binding(1)
             var r_reveal: texture_2d<f32>;
         """
 
         fragment_code = """
             let epsilon = 0.00001;
 
             // Sample
@@ -756,19 +760,19 @@
                     "alpha": (bf.one, bf.one_minus_src_alpha, bo.add),
                     "color": (bf.one, bf.one_minus_src_alpha, bo.add),
                 },
             },
         ]
 
         bindings_code = """
-            [[group(0), binding(0)]]
+            @group(0) @binding(0)
             var r_accum: texture_2d<f32>;
-            [[group(0), binding(1)]]
+            @group(0) @binding(1)
             var r_reveal: texture_2d<f32>;
-            [[group(0), binding(2)]]
+            @group(0) @binding(2)
             var r_frontcolor: texture_2d<f32>;
         """
 
         fragment_code = """
             let epsilon = 0.00001;
 
             // Sample
```

### Comparing `pygfx-0.1.8/pygfx/renderers/wgpu/_flusher.py` & `pygfx-0.1.9/pygfx/renderers/wgpu/_flusher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import wgpu
 import numpy as np
 
 
 FULL_QUAD_SHADER = """
     struct VertexInput {
-        [[builtin(vertex_index)]] index: u32;
+        @builtin(vertex_index) index: u32,
     };
     struct Varyings {
-        [[location(0)]] texcoord: vec2<f32>;
-        [[builtin(position)]] position: vec4<f32>;
+        @location(0) texcoord: vec2<f32>,
+        @builtin(position) position: vec4<f32>,
     };
     struct FragmentOutput {
-        [[location(0)]] color: vec4<f32>;
+        @location(0) color: vec4<f32>,
     };
 
     BINDINGS_CODE
 
-    [[stage(vertex)]]
+    @stage(vertex)
     fn vs_main(in: VertexInput) -> Varyings {
         var positions = array<vec2<f32>,4>(
             vec2<f32>(0.0, 1.0), vec2<f32>(0.0, 0.0), vec2<f32>(1.0, 1.0), vec2<f32>(1.0, 0.0)
         );
         let pos = positions[in.index];
         var varyings: Varyings;
         varyings.texcoord = vec2<f32>(pos.x, 1.0 - pos.y);
         varyings.position = vec4<f32>(pos * 2.0 - 1.0, 0.0, 1.0);
         return varyings;
     }
 
-    [[stage(fragment)]]
+    @stage(fragment)
     fn fs_main(varyings: Varyings) -> FragmentOutput {
         var out : FragmentOutput;
         let texcoord = varyings.texcoord;  // for textureSample
         let texindex = vec2<i32>(varyings.position.xy);  // for textureLoad
 
         FRAGMENT_CODE
 
@@ -149,39 +149,40 @@
         )
 
         render_pass = command_encoder.begin_render_pass(
             color_attachments=[
                 {
                     "view": dst_color_tex,
                     "resolve_target": None,
-                    "load_value": (0, 0, 0, 0),  # LoadOp.load or color
+                    "clear_value": (0, 0, 0, 0),
+                    "load_op": wgpu.LoadOp.clear,
                     "store_op": wgpu.StoreOp.store,
                 }
             ],
             depth_stencil_attachment=None,
         )
         render_pass.set_pipeline(render_pipeline)
         render_pass.set_bind_group(0, bind_group, [], 0, 99)
         render_pass.draw(4, 1)
-        render_pass.end_pass()
+        render_pass.end()
 
         return [command_encoder.finish()]
 
     def _create_pipeline(self, src_texture_view, dst_format):
         device = self._device
 
         bindings_code = """
             struct Render {
-                size: vec2<f32>;
-                sigma: f32;
-                support: i32;
+                size: vec2<f32>,
+                sigma: f32,
+                support: i32,
             };
-            [[group(0), binding(0)]]
+            @group(0) @binding(0)
             var<uniform> u_render: Render;
-            [[group(0), binding(1)]]
+            @group(0) @binding(1)
             var r_color: texture_2d<f32>;
         """
 
         fragment_code = """
             // Get info about the smoothing
             let sigma = u_render.sigma;
             let support = min(5, u_render.support);
```

### Comparing `pygfx-0.1.8/pygfx/renderers/wgpu/_pipelinebuilder.py` & `pygfx-0.1.9/pygfx/renderers/wgpu/_pipelinebuilder.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/renderers/wgpu/_renderer.py` & `pygfx-0.1.9/pygfx/renderers/wgpu/_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -573,17 +573,17 @@
         for wobject, wobject_pipeline in wobject_tuples:
             for pinfo in wobject_pipeline.get("compute_pipelines", ()):
                 compute_pass.set_pipeline(pinfo["pipeline"])
                 for bind_group_id, bind_group in enumerate(pinfo["bind_groups"]):
                     compute_pass.set_bind_group(
                         bind_group_id, bind_group, [], 0, 999999
                     )
-                compute_pass.dispatch(*pinfo["index_args"])
+                compute_pass.dispatch_workgroups(*pinfo["index_args"])
 
-        compute_pass.end_pass()
+        compute_pass.end()
 
         # ----- render pipelines
 
         for pass_index in range(blender.get_pass_count()):
 
             color_attachments = blender.get_color_attachments(pass_index, clear_color)
             depth_attachment = blender.get_depth_attachment(pass_index)
@@ -591,15 +591,15 @@
             if not color_attachments:
                 continue
 
             render_pass = command_encoder.begin_render_pass(
                 color_attachments=color_attachments,
                 depth_stencil_attachment={
                     **depth_attachment,
-                    "stencil_load_value": wgpu.LoadOp.load,
+                    "stencil_load_op": wgpu.LoadOp.load,
                     "stencil_store_op": wgpu.StoreOp.store,
                 },
                 occlusion_query_set=None,
             )
             render_pass.set_viewport(*physical_viewport)
 
             for wobject, wobject_pipeline in wobject_tuples:
@@ -620,15 +620,15 @@
                     if pinfo["index_buffer"] is not None:
                         ibuffer = pinfo["index_buffer"]
                         render_pass.set_index_buffer(ibuffer, 0, ibuffer.size)
                         render_pass.draw_indexed(*pinfo["index_args"])
                     else:
                         render_pass.draw(*pinfo["index_args"])
 
-            render_pass.end_pass()
+            render_pass.end()
 
         return [command_encoder.finish()]
 
     def _update_stdinfo_buffer(self, camera, physical_size, logical_size):
         # Update the stdinfo buffer's data
         stdinfo_data = self._shared.stdinfo_buffer.data
         stdinfo_data["cam_transform"].flat = camera.matrix_world_inverse.elements
```

### Comparing `pygfx-0.1.8/pygfx/renderers/wgpu/_shadercomposer.py` & `pygfx-0.1.9/pygfx/renderers/wgpu/_shadercomposer.py`

 * *Files 5% similar despite different names*

```diff
@@ -176,27 +176,27 @@
                         )
                     lines[linenr] = indent + "// " + line_s
 
     # Build and insert the struct
     if struct_insert_pos is not None:
         # Maybe we should move up a bit
         if struct_insert_pos > 0:
-            if lines[struct_insert_pos - 1].lstrip().startswith("[["):
+            if lines[struct_insert_pos - 1].lstrip().startswith("@"):
                 struct_insert_pos -= 1
         # First divide into slot-based and builtins
         used_varyings = set(used_varyings)
         used_builtins = used_varyings.intersection(builtin_varyings)
         used_slots = used_varyings.difference(used_builtins)
         used_slots = list(sorted(used_slots))
         # Build struct
         struct_lines = ["struct Varyings {"]
         for slotnr, name in enumerate(used_slots):
-            struct_lines.append(f"    [[location({slotnr})]] {name} : {types[name]};")
+            struct_lines.append(f"    @location({slotnr}) {name} : {types[name]},")
         for name in sorted(used_builtins):
-            struct_lines.append(f"    [[builtin({name})]] {name} : {types[name]};")
+            struct_lines.append(f"    @builtin({name}) {name} : {types[name]},")
         struct_lines.append("};\n")
         # Apply indentation and insert
         line = lines[struct_insert_pos]
         indent = line[: len(line) - len(line.lstrip())]
         struct_lines = [indent + line for line in struct_lines]
         lines.insert(struct_insert_pos, "\n".join(struct_lines))
     else:
@@ -239,15 +239,15 @@
             depth_is_set = True
             if struct_linrnr >= 0:
                 break
 
     if depth_is_set:
         if struct_linrnr < 0:
             raise TypeError("FragmentOutput definition not found.")
-        depth_field = "    [[builtin(frag_depth)]] depth : f32;"
+        depth_field = "    @builtin(frag_depth) depth : f32,"
         line = lines[struct_linrnr]
         indent = line[: len(line) - len(line.lstrip())]
         lines.insert(struct_linrnr + 1, indent + depth_field)
 
     return "\n".join(lines)
 
 
@@ -429,21 +429,21 @@
                 raise TypeError(f"Cannot establish alignment of wgsl type: {wgsl_type}")
             if offset % alignment != 0:
                 # If this happens, our array_from_shadertype() has failed.
                 raise TypeError(
                     f"Struct alignment error: {binding.name}.{fieldname} alignment must be {alignment}"
                 )
 
-            code += f"\n            {fieldname}: {wgsl_type};"
+            code += f"\n            {fieldname}: {wgsl_type},"
 
         code += "\n        };"
         self._typedefs[structname] = code
 
         code = f"""
-        [[group({bindgroup}), binding({index})]]
+        @group({bindgroup}) @binding({index})
         var<uniform> {binding.name}: {structname};
         """.rstrip()
         self._binding_codes[binding.name] = code
 
     def _define_buffer(self, bindgroup, index, binding):
 
         # Get format, and split in the scalar part and the number of channels
@@ -477,61 +477,52 @@
             element_type1 = scalar_type
             element_type2 = f"vec{nchannels}<{scalar_type}>"
             stride = 4
         else:
             element_type1 = element_type2 = f"vec{nchannels}<{scalar_type}>"
             stride = 4 * nchannels
 
-        # Prepare some names
-        typename = "Buffer_" + element_type1.replace("<", "").replace(">", "")
-        type_modifier = "read" if "read_only" in binding.type else "read_write"
-
-        # Produce the type definition
-        code = f"""
-        struct {typename} {{
-            data: [[stride({stride})]] array<{element_type1}>;
-        }};
-        """.rstrip()
-        self._typedefs[typename] = code
+        stride  # not actually used anymore in wgsl?
 
         # Produce the binding code and accessor function
+        type_modifier = "read" if "read_only" in binding.type else "read_write"
         code = f"""
-        [[group({bindgroup}), binding({index})]]
-        var<storage, {type_modifier}> {binding.name}: {typename};
+        @group({bindgroup}) @binding({index})
+        var<storage, {type_modifier}> {binding.name}: array<{element_type1}>;
         fn load_{binding.name} (i: i32) -> {element_type2} {{
         """.rstrip()
         if element_type1 == element_type2:
-            code += f" return {binding.name}.data[i];"
+            code += f" return {binding.name}[i];"
         elif nchannels == 2:
-            code += f" return {element_type2}( {binding.name}.data[i * 2], {binding.name}.data[i * 2 + 1] );"
+            code += f" return {element_type2}( {binding.name}[i * 2], {binding.name}[i * 2 + 1] );"
         elif nchannels == 3:
-            code += f" return {element_type2}( {binding.name}.data[i * 3], {binding.name}.data[i * 3 + 1], {binding.name}.data[i * 3 + 2] );"
+            code += f" return {element_type2}( {binding.name}[i * 3], {binding.name}[i * 3 + 1], {binding.name}[i * 3 + 2] );"
         else:  # nchannels == 4
-            code += f" return {element_type2}( {binding.name}.data[i * 4], {binding.name}.data[i * 4 + 1], {binding.name}.data[i * 4 + 2], {binding.name}.data[i * 4 + 3] );"
+            code += f" return {element_type2}( {binding.name}[i * 4], {binding.name}[i * 4 + 1], {binding.name}[i * 4 + 2], {binding.name}[i * 4 + 3] );"
         code += " }"
         self._binding_codes[binding.name] = code
 
     def _define_sampler(self, bindgroup, index, binding):
         code = f"""
-        [[group({bindgroup}), binding({index})]]
+        @group({bindgroup}) @binding({index})
         var {binding.name}: sampler;
         """.rstrip()
         self._binding_codes[binding.name] = code
 
     def _define_texture(self, bindgroup, index, binding):
         texture = binding.resource  # or view
         format = to_texture_format(texture.format)
         if "norm" in format or "float" in format:
             format = "f32"
         elif "uint" in format:
             format = "u32"
         else:
             format = "i32"
         code = f"""
-        [[group({bindgroup}), binding({index})]]
+        @group({bindgroup}) @binding({index})
         var {binding.name}: texture_{texture.view_dim}<{format}>;
         """.rstrip()
         self._binding_codes[binding.name] = code
 
 
 class WorldObjectShader(BaseShader):
     """A base shader for world objects. This class implements common functions
```

### Comparing `pygfx-0.1.8/pygfx/renderers/wgpu/_update.py` & `pygfx-0.1.9/pygfx/renderers/wgpu/_update.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/renderers/wgpu/_utils.py` & `pygfx-0.1.9/pygfx/renderers/wgpu/_utils.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/renderers/wgpu/backgroundrender.py` & `pygfx-0.1.9/pygfx/renderers/wgpu/backgroundrender.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,19 +68,19 @@
             + self.fragment_shader()
         )
 
     def vertex_shader(self):
         return """
 
         struct VertexInput {
-            [[builtin(vertex_index)]] index : u32;
+            @builtin(vertex_index) index : u32,
         };
 
 
-        [[stage(vertex)]]
+        @stage(vertex)
         fn vs_main(in: VertexInput) -> Varyings {
             var varyings: Varyings;
             // Define positions at the four corners of the viewport, at the largest depth
             var positions = array<vec2<f32>, 4>(
                 vec2<f32>(-1.0, -1.0),
                 vec2<f32>( 1.0, -1.0),
                 vec2<f32>(-1.0,  1.0),
@@ -105,15 +105,15 @@
             $$ endif
             return varyings;
         }
         """
 
     def fragment_shader(self):
         return """
-        [[stage(fragment)]]
+        @stage(fragment)
         fn fs_main(varyings: Varyings) -> FragmentOutput {
             var final_color : vec4<f32>;
             $$ if texture_dim
                 $$ if texture_dim == '2d'
                     let color = textureSample(r_tex, r_sampler, varyings.texcoord.xy);
                 $$ elif texture_dim == 'cube'
                     let color = textureSample(r_tex, r_sampler, varyings.texcoord.xyz);
```

### Comparing `pygfx-0.1.8/pygfx/renderers/wgpu/imagerender.py` & `pygfx-0.1.9/pygfx/renderers/wgpu/imagerender.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,17 +164,17 @@
 
 class BaseImageShader(WorldObjectShader):
     def image_helpers(self):
         return (
             sampled_value_to_color
             + """
         struct ImGeometry {
-            indices: array<i32,6>;
-            positions: array<vec3<f32>,4>;
-            texcoords: array<vec2<f32>,4>;
+            indices: array<i32,6>,
+            positions: array<vec3<f32>,4>,
+            texcoords: array<vec2<f32>,4>,
         };
 
         fn get_im_geometry() -> ImGeometry {
             let size = textureDimensions(t_img);
             var geo: ImGeometry;
 
             geo.indices = array<i32,6>(0, 1, 2,   3, 2, 1);
@@ -220,19 +220,19 @@
             + self.fragment_shader()
         )
 
     def vertex_shader(self):
         return """
 
         struct VertexInput {
-            [[builtin(vertex_index)]] vertex_index : u32;
+            @builtin(vertex_index) vertex_index : u32,
         };
 
 
-        [[stage(vertex)]]
+        @stage(vertex)
         fn vs_main(in: VertexInput) -> Varyings {
 
             var geo = get_im_geometry();
 
             // Select what face we're at
             let index = i32(in.vertex_index);
             let i0 = geo.indices[index];
@@ -249,15 +249,15 @@
             return varyings;
         }
         """
 
     def fragment_shader(self):
         return """
 
-        [[stage(fragment)]]
+        @stage(fragment)
         fn fs_main(varyings: Varyings) -> FragmentOutput {
             let sizef = vec2<f32>(textureDimensions(t_img));
             let value = sample_im(varyings.texcoord.xy, sizef);
             let color = sampled_value_to_color(value);
             let albeido = color.rgb;
 
             let final_color = vec4<f32>(albeido, color.a * u_material.opacity);
```

### Comparing `pygfx-0.1.8/pygfx/renderers/wgpu/linerender.py` & `pygfx-0.1.9/pygfx/renderers/wgpu/linerender.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,28 +168,28 @@
 
     def more_definitions(self):
         return """
 
         let PI: f32 = 3.14159265359;
 
         struct VertexInput {
-            [[builtin(vertex_index)]] index : u32;
+            @builtin(vertex_index) index : u32,
         };
 
         struct VertexFuncOutput {
-            i: i32;
-            pos: vec4<f32>;
-            thickness_p: f32;
-            vec_from_node_p: vec2<f32>;
+            i: i32,
+            pos: vec4<f32>,
+            thickness_p: f32,
+            vec_from_node_p: vec2<f32>,
         };
 
         struct FragmentOutput {
-            [[location(0)]] color: vec4<f32>;
-            [[location(1)]] pick: vec4<i32>;
-            [[builtin(frag_depth)]] depth : f32;
+            @location(0) color: vec4<f32>,
+            @location(1) pick: vec4<i32>,
+            @builtin(frag_depth) depth : f32,
         };
         """
 
     def helpers(self):
         return """
 
         fn get_point_ndc(index:i32) -> vec4<f32> {
@@ -206,15 +206,15 @@
             core = self.vertex_shader_segment()
         else:
             core = self.vertex_shader_line()
 
         return (
             core
             + """
-        [[stage(vertex)]]
+        @stage(vertex)
         fn vs_main(in: VertexInput) -> Varyings {
 
             let index = i32(in.index);
             let screen_factor = u_stdinfo.logical_size.xy / 2.0;
             let l2p:f32 = u_stdinfo.physical_size.x / u_stdinfo.logical_size.x;
             let extra_thick = {{ '0.5' if aa else '0.0' }} / l2p;
             let half_thickness:f32 = u_material.thickness * 0.5 + extra_thick;  // logical pixels
@@ -335,15 +335,15 @@
                 // This is the first point on the line: create a cap.
                 v1 = v2;
                 nc = normalize(vec2<f32>(v2.y, -v2.x));
                 nd = -nc;
                 na = nd;
                 nb = nd - normalize(v2);
                 ne = nc - normalize(v2);
-            } elseif (i == u_renderer.last_i) {
+            } else if (i == u_renderer.last_i) {
                 // This is the last point on the line: create a cap.
                 v2 = v1;
                 na = normalize(vec2<f32>(v1.y, -v1.x));
                 nb = -na;
                 ne = nb + normalize(v1);
                 nc = na + normalize(v1);
                 nd = na;
@@ -493,15 +493,15 @@
             out.vec_from_node_p = vec2<f32>(0.0, 0.0);
             return out;
         }
         """
 
     def fragment_shader(self):
         return """
-        [[stage(fragment)]]
+        @stage(fragment)
         fn fs_main(varyings: Varyings) -> FragmentOutput {
 
             // Discard fragments outside of the radius. This is what makes round
             // joins and caps. If we ever want bevel or miter joins, we should
             // change the vertex positions a bit, and drop these lines below.
             let dist_to_node_p = length(varyings.vec_from_node_p);
             if (dist_to_node_p > varyings.thickness_p * 0.5) {
@@ -639,34 +639,34 @@
             + self.fragment_shader()
         )
 
     def vertex_shader(self):
         return """
 
         struct VertexInput {
-            [[location(0)]] pos : vec3<f32>;
+            @location(0) pos : vec3<f32>,
             $$ if color_mode == 'vertex'
                 $$ if vertex_color_channels == 1
-                [[location(1)]] color : f32;
+                @location(1) color : f32,
                 $$ else
-                [[location(1)]] color : vec{{ vertex_color_channels }}<f32>;
+                @location(1) color : vec{{ vertex_color_channels }}<f32>,
                 $$ endif
             $$ elif color_mode == 'map'
                 $$ if colormap_dim == '1d'
-                [[location(1)]] texcoord : f32;
+                @location(1) texcoord : f32,
                 $$ elif colormap_dim == '2d'
-                [[location(1)]] texcoord : vec2<f32>;
+                @location(1) texcoord : vec2<f32>,
                 $$ else
-                [[location(1)]] texcoord : vec3<f32>;
+                @location(1) texcoord : vec3<f32>,
                 $$ endif
             $$ endif
-            [[builtin(vertex_index)]] index : u32;
+            @builtin(vertex_index) index : u32,
         };
 
-        [[stage(vertex)]]
+        @stage(vertex)
         fn vs_main(in: VertexInput) -> Varyings {
 
             let wpos = u_wobject.world_transform * vec4<f32>(in.pos.xyz, 1.0);
             let npos = u_stdinfo.projection_transform * u_stdinfo.cam_transform * wpos;
 
             var varyings: Varyings;
             varyings.position = vec4<f32>(npos);
@@ -694,15 +694,15 @@
 
             return varyings;
         }
         """
 
     def fragment_shader(self):
         return """
-        [[stage(fragment)]]
+        @stage(fragment)
         fn fs_main(varyings: Varyings) -> FragmentOutput {
 
             $$ if color_mode == 'vertex'
                 let color = varyings.color;
             $$ elif color_mode == 'map'
                 let color = sample_colormap(varyings.texcoord);
             $$ else
```

### Comparing `pygfx-0.1.8/pygfx/renderers/wgpu/meshrender.py` & `pygfx-0.1.9/pygfx/renderers/wgpu/meshrender.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,34 +168,31 @@
             + self.fragment_shader()
         )
 
     def vertex_shader(self):
         return """
 
         struct VertexInput {
-            [[builtin(vertex_index)]] vertex_index : u32;
+            @builtin(vertex_index) vertex_index : u32,
             $$ if instanced
-            [[builtin(instance_index)]] instance_index : u32;
+            @builtin(instance_index) instance_index : u32,
             $$ endif
         };
 
         $$ if instanced
         struct InstanceInfo {
-            transform: mat4x4<f32>;
-            id: u32;
+            transform: mat4x4<f32>,
+            id: u32,
         };
-        struct InstanceInfos {
-            data: [[stride(80)]] array<InstanceInfo>;
-        };
-        [[group(1), binding(0)]]
-        var<storage,read> s_instance_infos: InstanceInfos;
+        @group(1) @binding(0)
+        var<storage,read> s_instance_infos: array<InstanceInfo>;
         $$ endif
 
 
-        [[stage(vertex)]]
+        @stage(vertex)
         fn vs_main(in: VertexInput) -> Varyings {
 
             // Select what face we're at
             let index = i32(in.vertex_index);
             let face_index = index / 3;
             var sub_index = index % 3;
 
@@ -205,15 +202,15 @@
 
             // Sample
             let ii = load_s_indices(face_index);
             let i0 = i32(ii[sub_index]);
 
             // Get world transform
             $$ if instanced
-                let instance_info = s_instance_infos.data[in.instance_index];
+                let instance_info = s_instance_infos[in.instance_index];
                 let world_transform = u_wobject.world_transform * instance_info.transform;
             $$ else
                 let world_transform = u_wobject.world_transform;
             $$ endif
 
             // Get vertex position
             let raw_pos = load_s_positions(i0);
@@ -304,19 +301,19 @@
 
     """
 
     def vertex_shader_normal_lines(self):
         return """
 
         struct VertexInput {
-            [[builtin(vertex_index)]] vertex_index : u32;
+            @builtin(vertex_index) vertex_index : u32,
         };
 
 
-        [[stage(vertex)]]
+        @stage(vertex)
         fn vs_main(in: VertexInput) -> Varyings {
             let index = i32(in.vertex_index);
             let r = index % 2;
             let i0 = (index - r) / 2;
 
             let raw_pos = load_s_positions(i0);
             let raw_normal = load_s_normals(i0);
@@ -343,16 +340,16 @@
             return varyings;
         }
         """
 
     def fragment_shader(self):
         return """
 
-        [[stage(fragment)]]
-        fn fs_main(varyings: Varyings, [[builtin(front_facing)]] is_front: bool) -> FragmentOutput {
+        @stage(fragment)
+        fn fs_main(varyings: Varyings, @builtin(front_facing) is_front: bool) -> FragmentOutput {
 
             $$ if color_mode == 'vertex'
                 let color_value = varyings.color;
                 let albeido = color_value.rgb;
             $$ elif color_mode == 'map'
                 let color_value = sample_colormap(varyings.texcoord);
                 let albeido = color_value.rgb;  // no more colormap
@@ -550,19 +547,19 @@
             + self.fragment_shader()
         )
 
     def vertex_shader(self):
         return """
 
         struct VertexInput {
-            [[builtin(vertex_index)]] vertex_index : u32;
+            @builtin(vertex_index) vertex_index : u32,
         };
 
 
-        [[stage(vertex)]]
+        @stage(vertex)
         fn vs_main(in: VertexInput) -> Varyings {
 
             // This vertex shader uses VertexId and storage buffers instead of
             // vertex buffers. It creates 6 vertices for each face in the mesh,
             // drawn with triangle-list. For the faces that cross the plane, we
             // draw a (thick) line segment with round caps (we need 6 verts for that).
             // Other faces become degenerate triangles.
@@ -714,15 +711,15 @@
             return varyings;
         }
         """
 
     def fragment_shader(self):
         return """
 
-        [[stage(fragment)]]
+        @stage(fragment)
         fn fs_main(varyings: Varyings) -> FragmentOutput {
             var out: FragmentOutput;
 
             // Discart fragments that are too far from the centerline. This makes round caps.
             // Note that we operate in physical pixels here.
             let distx = max(0.0, abs(varyings.dist2center.x) - 0.5 * varyings.segment_length);
             let dist = length(vec2<f32>(distx, varyings.dist2center.y));
```

### Comparing `pygfx-0.1.8/pygfx/renderers/wgpu/pointsrender.py` & `pygfx-0.1.9/pygfx/renderers/wgpu/pointsrender.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,19 +143,19 @@
             + self.fragment_shader()
         )
 
     def vertex_shader(self):
         return """
 
         struct VertexInput {
-            [[builtin(vertex_index)]] vertex_index : u32;
+            @builtin(vertex_index) vertex_index : u32,
         };
 
 
-        [[stage(vertex)]]
+        @stage(vertex)
         fn vs_main(in: VertexInput) -> Varyings {
 
             let index = i32(in.vertex_index);
             let i0 = index / 6;
             let sub_index = index % 6;
 
             let raw_pos = load_s_positions(i0);
@@ -217,15 +217,15 @@
         }
         """
 
     def fragment_shader(self):
         # Also see See https://github.com/vispy/vispy/blob/master/vispy/visuals/markers.py
         return """
 
-        [[stage(fragment)]]
+        @stage(fragment)
         fn fs_main(varyings: Varyings) -> FragmentOutput {
             var final_color : vec4<f32>;
 
             let d = length(varyings.pointcoord);
             let aa_width = 1.0;
 
             $$ if per_vertex_sizes
@@ -241,15 +241,15 @@
             $$ else
                 let color = u_material.color;
             $$ endif
 
             $$ if type == 'circle'
                 if (d <= size - 0.5 * aa_width) {
                     final_color = color;
-                } elseif (d <= size + 0.5 * aa_width) {
+                } else if (d <= size + 0.5 * aa_width) {
                     let alpha1 = 0.5 + (size - d) / aa_width;
                     let alpha2 = pow(alpha1, 2.0);  // this works better
                     final_color = vec4<f32>(color.rgb, color.a * alpha2);
                 } else {
                     discard;
                 }
             $$ elif type == "gaussian"
```

### Comparing `pygfx-0.1.8/pygfx/renderers/wgpu/volumerender.py` & `pygfx-0.1.9/pygfx/renderers/wgpu/volumerender.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,17 +106,17 @@
 
 class BaseVolumeShader(WorldObjectShader):
     def volume_helpers(self):
         return (
             sampled_value_to_color
             + """
         struct VolGeometry {
-            indices: array<i32,36>;
-            positions: array<vec3<f32>,8>;
-            texcoords: array<vec3<f32>,8>;
+            indices: array<i32,36>,
+            positions: array<vec3<f32>,8>,
+            texcoords: array<vec3<f32>,8>,
         };
 
         fn get_vol_geometry() -> VolGeometry {
             let size = textureDimensions(t_img);
             var geo: VolGeometry;
 
             geo.indices = array<i32,36>(
@@ -174,19 +174,19 @@
             + self.fragment_shader()
         )
 
     def vertex_shader(self):
         return """
 
         struct VertexInput {
-            [[builtin(vertex_index)]] vertex_index : u32;
+            @builtin(vertex_index) vertex_index : u32,
         };
 
 
-        [[stage(vertex)]]
+        @stage(vertex)
         fn vs_main(in: VertexInput) -> Varyings {
 
             // Our geometry is implicitly defined by the volume dimensions.
             var geo = get_vol_geometry();
 
             // This layout is like this:
             //
@@ -292,15 +292,15 @@
                     if (i != i_last && intersect_flags[i] == 1) {
                         if (ed2pl[i][0] == plane_index) {
                             vertices[iter] = intersect_positions[i];
                             texcoords[iter] = intersect_texcoords[i];
                             plane_index = ed2pl[i][1];
                             i_last = i;
                             break;
-                        } elseif (ed2pl[i][1] == plane_index) {
+                        } else if (ed2pl[i][1] == plane_index) {
                             vertices[iter] = intersect_positions[i];
                             texcoords[iter] = intersect_texcoords[i];
                             plane_index = ed2pl[i][0];
                             i_last = i;
                             break;
                         }
                     }
@@ -330,15 +330,15 @@
             return varyings;
         }
         """
 
     def fragment_shader(self):
         return """
 
-        [[stage(fragment)]]
+        @stage(fragment)
         fn fs_main(varyings: Varyings) -> FragmentOutput {
             let sizef = vec3<f32>(textureDimensions(t_img));
             let value = sample_vol(varyings.texcoord.xyz, sizef);
             let color = sampled_value_to_color(value);
             let albeido = color.rgb;
             let final_color = vec4<f32>(albeido, color.a * u_material.opacity);
 
@@ -373,18 +373,18 @@
             + self.fragment_shader()
         )
 
     def vertex_shader(self):
         return """
 
         struct VertexInput {
-            [[builtin(vertex_index)]] vertex_index : u32;
+            @builtin(vertex_index) vertex_index : u32,
         };
 
-        [[stage(vertex)]]
+        @stage(vertex)
         fn vs_main(in: VertexInput) -> Varyings {
 
             // Our geometry is implicitly defined by the volume dimensions.
             var geo = get_vol_geometry();
 
             // Select what face we're at
             let index = i32(in.vertex_index);
@@ -425,15 +425,15 @@
 
             return varyings;
         }
         """
 
     def fragment_shader(self):
         return """
-        [[stage(fragment)]]
+        @stage(fragment)
         fn fs_main(varyings: Varyings) -> FragmentOutput {
 
             // Get size of the volume
             let sizef = vec3<f32>(textureDimensions(t_img));
 
             // Determine the stepsize as a float in pixels.
             // This value should be between ~ 0.1 and 1. Smaller values yield better
@@ -504,16 +504,16 @@
 
     def render_function(self):
         # Triage over different render modes. Only one mode so far :)
         f = getattr(self, "render_mode_" + self.kwargs["mode"].lower(), "mip")
 
         preamble = """
         struct RenderOutput {
-            color: vec4<f32>;
-            coord: vec3<f32>;
+            color: vec4<f32>,
+            coord: vec3<f32>,
         };
         """
 
         return preamble + f()
 
     def render_mode_mip(self):
 
@@ -557,15 +557,15 @@
                 let value2 = sample_vol(coord2, sizef);
                 let ref1 = value1.r;
                 let ref2 = value2.r;
                 if (ref1 >= the_ref) {  // deliberate larger-equal
                     the_ref = ref1;
                     the_coord = coord1;
                     the_value = value1;
-                } elseif (ref2 > the_ref) {
+                } else if (ref2 > the_ref) {
                     the_ref = ref2;
                     the_coord = coord2;
                     the_value = value2;
                 }
             }
 
             // Colormapping
```

### Comparing `pygfx-0.1.8/pygfx/resources/_buffer.py` & `pygfx-0.1.9/pygfx/resources/_buffer.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/resources/_texture.py` & `pygfx-0.1.9/pygfx/resources/_texture.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/utils/__init__.py` & `pygfx-0.1.9/pygfx/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/utils/_cmdata_mpl.py` & `pygfx-0.1.9/pygfx/utils/_cmdata_mpl.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/utils/color.py` & `pygfx-0.1.9/pygfx/utils/color.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/utils/show.py` & `pygfx-0.1.9/pygfx/utils/show.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx/utils/viewport.py` & `pygfx-0.1.9/pygfx/utils/viewport.py`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/pygfx.egg-info/PKG-INFO` & `pygfx-0.1.9/pygfx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: pygfx
-Version: 0.1.8
+Version: 0.1.9
 Summary: A threejs-like render engine based on wgpu
 Home-page: https://github.com/pygfx/pygfx
 Author: Almar Klein
 Author-email: almar.klein@gmail.com
 License: BSD 2-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: examples
 License-File: LICENSE
 
 [![CI](https://github.com/pygfx/pygfx/workflows/CI/badge.svg)](https://github.com/pygfx/pygfx/actions)
 [![Documentation Status](https://readthedocs.org/projects/pygfx/badge/?version=latest)](https://pygfx.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/pygfx.svg)](https://badge.fury.io/py/pygfx)
 
 # pygfx
@@ -107,14 +109,19 @@
 ## Current status
 
 Under development, many things can change.
 
 
 ## Testing examples
 
+The test suite is divided into two parts; unit tests for the core, and unit tests for the examples.
+
+* `pytest -v tests` runs the core unit tests.
+* `pytest -v examples` tests the examples.
+
 There are two types of tests for examples included with pygfx:
 
 ### Type 1: Checking if examples can run
 
 When running the test suite, pytest will run every example in a subprocess,
 to see if it can run and exit cleanly. You can opt out of this mechanism by including the comment
 `# run_example = false` in the module.
```

### Comparing `pygfx-0.1.8/pygfx.egg-info/SOURCES.txt` & `pygfx-0.1.9/pygfx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygfx-0.1.8/setup.py` & `pygfx-0.1.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,27 +8,50 @@
 
 with open(f"{NAME}/__init__.py") as fh:
     VERSION = re.search(r"__version__ = \"(.*?)\"", fh.read()).group(1)
 
 
 runtime_deps = [
     "numpy",
-    "wgpu>=0.7.6,<0.8.0",
+    "wgpu>=0.8.0,<0.9.0",
     "Jinja2",
 ]
 
+extras_require = {
+    "dev": [
+        "black",
+        "flake8",
+        "flake8-black",
+        "pep8-naming",
+        "pytest",
+        "setuptools",
+        "wheel",
+        "twine",
+        "imageio",
+    ],
+    "examples": [
+        "pytest",
+        "PySide6",
+        "imageio",
+        "imageio-ffmpeg>=0.4.7",
+        "scikit-image",
+        "trimesh",
+    ],
+}
+
 
 setup(
     name=NAME,
     version=VERSION,
     packages=find_packages(
         exclude=["tests", "tests.*", "examples", "examples.*", "exp", "exp.*"]
     ),
     python_requires=">=3.7.0",
     install_requires=runtime_deps,
+    extras_require=extras_require,
     license="BSD 2-Clause",
     description=SUMMARY,
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Almar Klein",
     author_email="almar.klein@gmail.com",
     url="https://github.com/pygfx/pygfx",
```

