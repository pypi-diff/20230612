# Comparing `tmp/ceva-0.0.1.tar.gz` & `tmp/ceva-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ceva-0.0.1.tar", last modified: Mon Jun 12 04:30:07 2023, max compression
+gzip compressed data, was "ceva-1.0.0.tar", last modified: Mon Jun 12 07:00:26 2023, max compression
```

## Comparing `ceva-0.0.1.tar` & `ceva-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 tmn       (1000) tmn       (1000)        0 2023-06-12 04:30:07.656798 ceva-0.0.1/
--rw-rw-r--   0 tmn       (1000) tmn       (1000)     1023 2023-06-12 04:29:06.000000 ceva-0.0.1/CMakeLists.txt
--rw-rw-r--   0 tmn       (1000) tmn       (1000)      192 2023-06-12 04:30:07.656798 ceva-0.0.1/PKG-INFO
--rw-rw-r--   0 tmn       (1000) tmn       (1000)      553 2023-06-12 04:05:20.000000 ceva-0.0.1/README.md
-drwxrwxr-x   0 tmn       (1000) tmn       (1000)        0 2023-06-12 04:30:07.656798 ceva-0.0.1/ceva.egg-info/
--rw-rw-r--   0 tmn       (1000) tmn       (1000)      192 2023-06-12 04:30:07.000000 ceva-0.0.1/ceva.egg-info/PKG-INFO
--rw-rw-r--   0 tmn       (1000) tmn       (1000)      705 2023-06-12 04:30:07.000000 ceva-0.0.1/ceva.egg-info/SOURCES.txt
--rw-rw-r--   0 tmn       (1000) tmn       (1000)        1 2023-06-12 04:30:07.000000 ceva-0.0.1/ceva.egg-info/dependency_links.txt
--rw-rw-r--   0 tmn       (1000) tmn       (1000)        1 2023-06-12 04:30:07.000000 ceva-0.0.1/ceva.egg-info/not-zip-safe
--rw-rw-r--   0 tmn       (1000) tmn       (1000)       20 2023-06-12 04:30:07.000000 ceva-0.0.1/ceva.egg-info/requires.txt
--rw-rw-r--   0 tmn       (1000) tmn       (1000)        5 2023-06-12 04:30:07.000000 ceva-0.0.1/ceva.egg-info/top_level.txt
-drwxrwxr-x   0 tmn       (1000) tmn       (1000)        0 2023-06-12 04:30:07.652798 ceva-0.0.1/include/
-drwxrwxr-x   0 tmn       (1000) tmn       (1000)        0 2023-06-12 04:30:07.652798 ceva-0.0.1/include/basalt/
-drwxrwxr-x   0 tmn       (1000) tmn       (1000)        0 2023-06-12 04:30:07.656798 ceva-0.0.1/include/basalt/spline/
--rwxrwxr-x   0 tmn       (1000) tmn       (1000)     8681 2023-06-12 04:04:34.000000 ceva-0.0.1/include/basalt/spline/calib_bias.hpp
--rwxrwxr-x   0 tmn       (1000) tmn       (1000)     5086 2023-06-12 04:04:34.000000 ceva-0.0.1/include/basalt/spline/ceres_local_param.hpp
--rwxrwxr-x   0 tmn       (1000) tmn       (1000)    10238 2023-06-12 04:04:34.000000 ceva-0.0.1/include/basalt/spline/ceres_spline_helper.h
--rwxrwxr-x   0 tmn       (1000) tmn       (1000)    10366 2023-06-12 04:04:34.000000 ceva-0.0.1/include/basalt/spline/ceres_spline_helper_jet.h
--rwxrwxr-x   0 tmn       (1000) tmn       (1000)    14340 2023-06-12 04:04:34.000000 ceva-0.0.1/include/basalt/spline/rd_spline.h
--rwxrwxr-x   0 tmn       (1000) tmn       (1000)    25834 2023-06-12 04:04:34.000000 ceva-0.0.1/include/basalt/spline/se3_spline.h
--rwxrwxr-x   0 tmn       (1000) tmn       (1000)    28575 2023-06-12 04:04:34.000000 ceva-0.0.1/include/basalt/spline/so3_spline.h
--rwxrwxr-x   0 tmn       (1000) tmn       (1000)     4873 2023-06-12 04:04:34.000000 ceva-0.0.1/include/basalt/spline/spline_common.h
--rwxrwxr-x   0 tmn       (1000) tmn       (1000)     3277 2023-06-12 04:04:34.000000 ceva-0.0.1/include/basalt/spline/spline_segment.h
-drwxrwxr-x   0 tmn       (1000) tmn       (1000)        0 2023-06-12 04:30:07.656798 ceva-0.0.1/include/basalt/utils/
--rwxrwxr-x   0 tmn       (1000) tmn       (1000)     3958 2023-06-12 04:04:34.000000 ceva-0.0.1/include/basalt/utils/assert.h
--rwxrwxr-x   0 tmn       (1000) tmn       (1000)     3125 2023-06-12 04:04:34.000000 ceva-0.0.1/include/basalt/utils/eigen_utils.hpp
--rwxrwxr-x   0 tmn       (1000) tmn       (1000)    17734 2023-06-12 04:04:34.000000 ceva-0.0.1/include/basalt/utils/sophus_utils.hpp
--rw-rw-r--   0 tmn       (1000) tmn       (1000)      417 2023-06-12 04:05:20.000000 ceva-0.0.1/package.xml
-drwxrwxr-x   0 tmn       (1000) tmn       (1000)        0 2023-06-12 04:30:07.656798 ceva-0.0.1/scripts/
--rw-rw-r--   0 tmn       (1000) tmn       (1000)     3103 2023-06-12 04:09:01.000000 ceva-0.0.1/scripts/test.ipynb
--rwxrwxr-x   0 tmn       (1000) tmn       (1000)      119 2023-06-12 04:05:30.000000 ceva-0.0.1/scripts/test.py
--rw-rw-r--   0 tmn       (1000) tmn       (1000)       38 2023-06-12 04:30:07.656798 ceva-0.0.1/setup.cfg
--rw-rw-r--   0 tmn       (1000) tmn       (1000)     5720 2023-06-12 04:05:20.000000 ceva-0.0.1/setup.py
+drwxrwxr-x   0 tmn       (1000) tmn       (1000)        0 2023-06-12 07:00:26.010161 ceva-1.0.0/
+-rw-rw-r--   0 tmn       (1000) tmn       (1000)      873 2023-06-12 06:44:15.000000 ceva-1.0.0/CMakeLists.txt
+-rw-rw-r--   0 tmn       (1000) tmn       (1000)      192 2023-06-12 07:00:26.010161 ceva-1.0.0/PKG-INFO
+-rw-rw-r--   0 tmn       (1000) tmn       (1000)      535 2023-06-12 06:52:12.000000 ceva-1.0.0/README.md
+drwxrwxr-x   0 tmn       (1000) tmn       (1000)        0 2023-06-12 07:00:26.006161 ceva-1.0.0/ceva.egg-info/
+-rw-rw-r--   0 tmn       (1000) tmn       (1000)      192 2023-06-12 07:00:25.000000 ceva-1.0.0/ceva.egg-info/PKG-INFO
+-rw-rw-r--   0 tmn       (1000) tmn       (1000)      705 2023-06-12 07:00:25.000000 ceva-1.0.0/ceva.egg-info/SOURCES.txt
+-rw-rw-r--   0 tmn       (1000) tmn       (1000)        1 2023-06-12 07:00:25.000000 ceva-1.0.0/ceva.egg-info/dependency_links.txt
+-rw-rw-r--   0 tmn       (1000) tmn       (1000)        1 2023-06-12 06:44:37.000000 ceva-1.0.0/ceva.egg-info/not-zip-safe
+-rw-rw-r--   0 tmn       (1000) tmn       (1000)       20 2023-06-12 07:00:25.000000 ceva-1.0.0/ceva.egg-info/requires.txt
+-rw-rw-r--   0 tmn       (1000) tmn       (1000)        5 2023-06-12 07:00:25.000000 ceva-1.0.0/ceva.egg-info/top_level.txt
+drwxrwxr-x   0 tmn       (1000) tmn       (1000)        0 2023-06-12 07:00:26.006161 ceva-1.0.0/include/
+drwxrwxr-x   0 tmn       (1000) tmn       (1000)        0 2023-06-12 07:00:26.006161 ceva-1.0.0/include/basalt/
+drwxrwxr-x   0 tmn       (1000) tmn       (1000)        0 2023-06-12 07:00:26.006161 ceva-1.0.0/include/basalt/spline/
+-rwxrwxr-x   0 tmn       (1000) tmn       (1000)     8681 2023-06-12 04:04:34.000000 ceva-1.0.0/include/basalt/spline/calib_bias.hpp
+-rwxrwxr-x   0 tmn       (1000) tmn       (1000)     5086 2023-06-12 04:04:34.000000 ceva-1.0.0/include/basalt/spline/ceres_local_param.hpp
+-rwxrwxr-x   0 tmn       (1000) tmn       (1000)    10238 2023-06-12 04:04:34.000000 ceva-1.0.0/include/basalt/spline/ceres_spline_helper.h
+-rwxrwxr-x   0 tmn       (1000) tmn       (1000)    10366 2023-06-12 04:04:34.000000 ceva-1.0.0/include/basalt/spline/ceres_spline_helper_jet.h
+-rwxrwxr-x   0 tmn       (1000) tmn       (1000)    14340 2023-06-12 04:04:34.000000 ceva-1.0.0/include/basalt/spline/rd_spline.h
+-rwxrwxr-x   0 tmn       (1000) tmn       (1000)    25834 2023-06-12 04:04:34.000000 ceva-1.0.0/include/basalt/spline/se3_spline.h
+-rwxrwxr-x   0 tmn       (1000) tmn       (1000)    28575 2023-06-12 04:04:34.000000 ceva-1.0.0/include/basalt/spline/so3_spline.h
+-rwxrwxr-x   0 tmn       (1000) tmn       (1000)     4873 2023-06-12 04:04:34.000000 ceva-1.0.0/include/basalt/spline/spline_common.h
+-rwxrwxr-x   0 tmn       (1000) tmn       (1000)     3277 2023-06-12 04:04:34.000000 ceva-1.0.0/include/basalt/spline/spline_segment.h
+drwxrwxr-x   0 tmn       (1000) tmn       (1000)        0 2023-06-12 07:00:26.010161 ceva-1.0.0/include/basalt/utils/
+-rwxrwxr-x   0 tmn       (1000) tmn       (1000)     3958 2023-06-12 04:04:34.000000 ceva-1.0.0/include/basalt/utils/assert.h
+-rwxrwxr-x   0 tmn       (1000) tmn       (1000)     3125 2023-06-12 04:04:34.000000 ceva-1.0.0/include/basalt/utils/eigen_utils.hpp
+-rwxrwxr-x   0 tmn       (1000) tmn       (1000)    17734 2023-06-12 04:04:34.000000 ceva-1.0.0/include/basalt/utils/sophus_utils.hpp
+-rw-rw-r--   0 tmn       (1000) tmn       (1000)      417 2023-06-12 04:05:20.000000 ceva-1.0.0/package.xml
+drwxrwxr-x   0 tmn       (1000) tmn       (1000)        0 2023-06-12 07:00:26.010161 ceva-1.0.0/scripts/
+-rw-rw-r--   0 tmn       (1000) tmn       (1000)     3103 2023-06-12 04:09:01.000000 ceva-1.0.0/scripts/test.ipynb
+-rwxrwxr-x   0 tmn       (1000) tmn       (1000)      119 2023-06-12 04:05:30.000000 ceva-1.0.0/scripts/test.py
+-rw-rw-r--   0 tmn       (1000) tmn       (1000)       38 2023-06-12 07:00:26.010161 ceva-1.0.0/setup.cfg
+-rw-rw-r--   0 tmn       (1000) tmn       (1000)     5720 2023-06-12 07:00:18.000000 ceva-1.0.0/setup.py
```

### Comparing `ceva-0.0.1/ceva.egg-info/SOURCES.txt` & `ceva-1.0.0/ceva.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ceva-0.0.1/include/basalt/spline/calib_bias.hpp` & `ceva-1.0.0/include/basalt/spline/calib_bias.hpp`

 * *Files identical despite different names*

### Comparing `ceva-0.0.1/include/basalt/spline/ceres_local_param.hpp` & `ceva-1.0.0/include/basalt/spline/ceres_local_param.hpp`

 * *Files identical despite different names*

### Comparing `ceva-0.0.1/include/basalt/spline/ceres_spline_helper.h` & `ceva-1.0.0/include/basalt/spline/ceres_spline_helper.h`

 * *Files identical despite different names*

### Comparing `ceva-0.0.1/include/basalt/spline/ceres_spline_helper_jet.h` & `ceva-1.0.0/include/basalt/spline/ceres_spline_helper_jet.h`

 * *Files identical despite different names*

### Comparing `ceva-0.0.1/include/basalt/spline/rd_spline.h` & `ceva-1.0.0/include/basalt/spline/rd_spline.h`

 * *Files identical despite different names*

### Comparing `ceva-0.0.1/include/basalt/spline/se3_spline.h` & `ceva-1.0.0/include/basalt/spline/se3_spline.h`

 * *Files identical despite different names*

### Comparing `ceva-0.0.1/include/basalt/spline/so3_spline.h` & `ceva-1.0.0/include/basalt/spline/so3_spline.h`

 * *Files identical despite different names*

### Comparing `ceva-0.0.1/include/basalt/spline/spline_common.h` & `ceva-1.0.0/include/basalt/spline/spline_common.h`

 * *Files identical despite different names*

### Comparing `ceva-0.0.1/include/basalt/spline/spline_segment.h` & `ceva-1.0.0/include/basalt/spline/spline_segment.h`

 * *Files identical despite different names*

### Comparing `ceva-0.0.1/include/basalt/utils/assert.h` & `ceva-1.0.0/include/basalt/utils/assert.h`

 * *Files identical despite different names*

### Comparing `ceva-0.0.1/include/basalt/utils/eigen_utils.hpp` & `ceva-1.0.0/include/basalt/utils/eigen_utils.hpp`

 * *Files identical despite different names*

### Comparing `ceva-0.0.1/include/basalt/utils/sophus_utils.hpp` & `ceva-1.0.0/include/basalt/utils/sophus_utils.hpp`

 * *Files identical despite different names*

### Comparing `ceva-0.0.1/scripts/test.ipynb` & `ceva-1.0.0/scripts/test.ipynb`

 * *Files identical despite different names*

### Comparing `ceva-0.0.1/setup.py` & `ceva-1.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         )
 
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="ceva",
-    version="0.0.1",
+    version="1.0.0",
     author="MCD VIRAL",
     author_email="mcdviral@gmail.com",
     description="A test project using pybind11 and CMake",
     long_description="",
     ext_modules=[CMakeExtension("ceva")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
```

