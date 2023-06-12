# Comparing `tmp/cairocffi-1.5.1.tar.gz` & `tmp/cairocffi-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cairocffi-1.5.1.tar", last modified: Sat Apr 15 07:25:44 2023, max compression
+gzip compressed data, was "cairocffi-1.6.0.tar", last modified: Mon Jun 12 08:13:48 2023, max compression
```

## Comparing `cairocffi-1.5.1.tar` & `cairocffi-1.6.0.tar`

### file list

```diff
@@ -1,46 +1,35 @@
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-04-15 07:25:44.517513 cairocffi-1.5.1/
--rw-r--r--   0 lize      (1000) lize      (1000)     1534 2020-10-29 21:18:23.000000 cairocffi-1.5.1/LICENSE
--rw-r--r--   0 lize      (1000) lize      (1000)       22 2023-03-25 08:13:29.000000 cairocffi-1.5.1/MANIFEST.in
--rw-r--r--   0 lize      (1000) lize      (1000)     4610 2023-04-15 07:25:44.517513 cairocffi-1.5.1/PKG-INFO
--rw-r--r--   0 lize      (1000) lize      (1000)     1612 2023-03-25 08:13:29.000000 cairocffi-1.5.1/README.rst
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-04-15 07:25:44.515513 cairocffi-1.5.1/cairocffi/
--rw-r--r--   0 lize      (1000) lize      (1000)     4034 2023-04-15 07:22:16.000000 cairocffi-1.5.1/cairocffi/__init__.py
--rw-r--r--   0 lize      (1000) lize      (1000)    55889 2023-03-25 08:13:29.000000 cairocffi-1.5.1/cairocffi/constants.py
--rw-r--r--   0 lize      (1000) lize      (1000)    84791 2022-10-03 08:01:47.000000 cairocffi-1.5.1/cairocffi/context.py
--rw-r--r--   0 lize      (1000) lize      (1000)     4174 2023-04-15 07:12:26.000000 cairocffi-1.5.1/cairocffi/ffi_build.py
--rw-r--r--   0 lize      (1000) lize      (1000)    19493 2020-10-29 21:18:23.000000 cairocffi-1.5.1/cairocffi/fonts.py
--rw-r--r--   0 lize      (1000) lize      (1000)     8064 2020-10-29 21:18:23.000000 cairocffi-1.5.1/cairocffi/matrix.py
--rw-r--r--   0 lize      (1000) lize      (1000)    12978 2020-10-29 21:18:23.000000 cairocffi-1.5.1/cairocffi/patterns.py
--rw-r--r--   0 lize      (1000) lize      (1000)     7260 2023-04-15 07:08:00.000000 cairocffi-1.5.1/cairocffi/pixbuf.py
--rw-r--r--   0 lize      (1000) lize      (1000)    57999 2023-03-25 08:13:29.000000 cairocffi-1.5.1/cairocffi/surfaces.py
--rw-r--r--   0 lize      (1000) lize      (1000)    46873 2023-03-11 07:55:03.000000 cairocffi-1.5.1/cairocffi/test_cairo.py
--rw-r--r--   0 lize      (1000) lize      (1000)      405 2023-03-11 07:55:03.000000 cairocffi-1.5.1/cairocffi/test_numpy.py
--rw-r--r--   0 lize      (1000) lize      (1000)     2398 2023-03-11 07:55:03.000000 cairocffi-1.5.1/cairocffi/test_pixbuf.py
--rw-r--r--   0 lize      (1000) lize      (1000)     6338 2023-03-11 07:55:03.000000 cairocffi-1.5.1/cairocffi/test_xcb.py
--rw-r--r--   0 lize      (1000) lize      (1000)     2023 2023-04-14 22:15:06.000000 cairocffi-1.5.1/cairocffi/xcb.py
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-04-15 07:25:44.516513 cairocffi-1.5.1/cairocffi.egg-info/
--rw-r--r--   0 lize      (1000) lize      (1000)     4610 2023-04-15 07:25:44.000000 cairocffi-1.5.1/cairocffi.egg-info/PKG-INFO
--rw-r--r--   0 lize      (1000) lize      (1000)      821 2023-04-15 07:25:44.000000 cairocffi-1.5.1/cairocffi.egg-info/SOURCES.txt
--rw-r--r--   0 lize      (1000) lize      (1000)        1 2023-04-15 07:25:44.000000 cairocffi-1.5.1/cairocffi.egg-info/dependency_links.txt
--rw-r--r--   0 lize      (1000) lize      (1000)      106 2023-04-15 07:25:44.000000 cairocffi-1.5.1/cairocffi.egg-info/requires.txt
--rw-r--r--   0 lize      (1000) lize      (1000)       10 2023-04-15 07:25:44.000000 cairocffi-1.5.1/cairocffi.egg-info/top_level.txt
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-04-15 07:25:44.516513 cairocffi-1.5.1/docs/
--rw-r--r--   0 lize      (1000) lize      (1000)    21215 2020-10-29 21:18:23.000000 cairocffi-1.5.1/docs/api.rst
--rw-r--r--   0 lize      (1000) lize      (1000)     4335 2020-10-29 21:18:23.000000 cairocffi-1.5.1/docs/cffi_api.rst
--rw-r--r--   0 lize      (1000) lize      (1000)       54 2023-03-11 07:55:03.000000 cairocffi-1.5.1/docs/changelog.rst
--rw-r--r--   0 lize      (1000) lize      (1000)      555 2020-10-29 21:18:23.000000 cairocffi-1.5.1/docs/conf.py
--rw-r--r--   0 lize      (1000) lize      (1000)      139 2020-10-29 21:18:23.000000 cairocffi-1.5.1/docs/index.rst
--rw-r--r--   0 lize      (1000) lize      (1000)     5446 2021-10-04 10:06:33.000000 cairocffi-1.5.1/docs/overview.rst
--rw-r--r--   0 lize      (1000) lize      (1000)     1234 2020-10-29 21:18:23.000000 cairocffi-1.5.1/docs/pixbuf.rst
--rw-r--r--   0 lize      (1000) lize      (1000)      273 2020-10-29 21:18:23.000000 cairocffi-1.5.1/docs/xcb.rst
--rw-r--r--   0 lize      (1000) lize      (1000)     1709 2023-04-15 07:08:00.000000 cairocffi-1.5.1/pyproject.toml
--rw-r--r--   0 lize      (1000) lize      (1000)       38 2023-04-15 07:25:44.517513 cairocffi-1.5.1/setup.cfg
-drwxr-xr-x   0 lize      (1000) lize      (1000)        0 2023-04-15 07:25:44.517513 cairocffi-1.5.1/utils/
--rw-r--r--   0 lize      (1000) lize      (1000)      953 2023-04-15 07:17:22.000000 cairocffi-1.5.1/utils/build.py
--rw-r--r--   0 lize      (1000) lize      (1000)      777 2020-10-29 21:18:23.000000 cairocffi-1.5.1/utils/cairo_coverage.py
--rw-r--r--   0 lize      (1000) lize      (1000)     1390 2020-10-29 21:18:23.000000 cairocffi-1.5.1/utils/cairocffi_to_pycairo.py
--rw-r--r--   0 lize      (1000) lize      (1000)      756 2020-10-29 21:18:23.000000 cairocffi-1.5.1/utils/compare_pycairo.py
--rw-r--r--   0 lize      (1000) lize      (1000)     3001 2023-03-25 08:13:29.000000 cairocffi-1.5.1/utils/mkconstants.py
--rw-r--r--   0 lize      (1000) lize      (1000)     1853 2020-10-29 21:18:23.000000 cairocffi-1.5.1/utils/pango_example.py
--rw-r--r--   0 lize      (1000) lize      (1000)     1056 2020-10-29 21:18:23.000000 cairocffi-1.5.1/utils/pycairo_to_cairocffi.py
--rw-r--r--   0 lize      (1000) lize      (1000)      999 2023-03-11 07:55:03.000000 cairocffi-1.5.1/utils/tests.py
+-rw-r--r--   0        0        0     1534 2020-10-29 21:18:23.141438 cairocffi-1.6.0/LICENSE
+-rw-r--r--   0        0        0       22 2023-03-25 08:13:29.041670 cairocffi-1.6.0/MANIFEST.in
+-rw-r--r--   0        0        0     8872 2023-06-12 08:09:43.992397 cairocffi-1.6.0/NEWS.rst
+-rw-r--r--   0        0        0     1612 2023-03-25 08:13:29.048670 cairocffi-1.6.0/README.rst
+-rw-r--r--   0        0        0     4023 2023-06-12 08:00:06.780849 cairocffi-1.6.0/cairocffi/__init__.py
+-rw-r--r--   0        0        0    55889 2023-03-25 08:13:29.050670 cairocffi-1.6.0/cairocffi/constants.py
+-rw-r--r--   0        0        0    84791 2022-10-03 08:01:47.993857 cairocffi-1.6.0/cairocffi/context.py
+-rw-r--r--   0        0        0     3571 2023-06-12 07:59:33.181255 cairocffi-1.6.0/cairocffi/ffi.py
+-rw-r--r--   0        0        0    19493 2020-10-29 21:18:23.142438 cairocffi-1.6.0/cairocffi/fonts.py
+-rw-r--r--   0        0        0     8064 2020-10-29 21:18:23.142438 cairocffi-1.6.0/cairocffi/matrix.py
+-rw-r--r--   0        0        0    12978 2020-10-29 21:18:23.142438 cairocffi-1.6.0/cairocffi/patterns.py
+-rw-r--r--   0        0        0     7256 2023-06-12 07:59:33.181255 cairocffi-1.6.0/cairocffi/pixbuf.py
+-rw-r--r--   0        0        0    57999 2023-03-25 08:13:29.052671 cairocffi-1.6.0/cairocffi/surfaces.py
+-rw-r--r--   0        0        0    46873 2023-03-11 07:55:03.040563 cairocffi-1.6.0/cairocffi/test_cairo.py
+-rw-r--r--   0        0        0      405 2023-03-11 07:55:03.040563 cairocffi-1.6.0/cairocffi/test_numpy.py
+-rw-r--r--   0        0        0     2398 2023-03-11 07:55:03.040563 cairocffi-1.6.0/cairocffi/test_pixbuf.py
+-rw-r--r--   0        0        0     6338 2023-03-11 07:55:03.040563 cairocffi-1.6.0/cairocffi/test_xcb.py
+-rw-r--r--   0        0        0     2023 2023-04-14 22:15:06.224429 cairocffi-1.6.0/cairocffi/xcb.py
+-rw-r--r--   0        0        0    21215 2020-10-29 21:18:23.143438 cairocffi-1.6.0/docs/api.rst
+-rw-r--r--   0        0        0     4335 2020-10-29 21:18:23.143438 cairocffi-1.6.0/docs/cffi_api.rst
+-rw-r--r--   0        0        0       54 2023-03-11 07:55:03.041563 cairocffi-1.6.0/docs/changelog.rst
+-rw-r--r--   0        0        0      555 2020-10-29 21:18:23.144438 cairocffi-1.6.0/docs/conf.py
+-rw-r--r--   0        0        0      139 2020-10-29 21:18:23.144438 cairocffi-1.6.0/docs/index.rst
+-rw-r--r--   0        0        0     5446 2021-10-04 10:06:33.130910 cairocffi-1.6.0/docs/overview.rst
+-rw-r--r--   0        0        0     1234 2020-10-29 21:18:23.144438 cairocffi-1.6.0/docs/pixbuf.rst
+-rw-r--r--   0        0        0      273 2020-10-29 21:18:23.144438 cairocffi-1.6.0/docs/xcb.rst
+-rw-r--r--   0        0        0     1936 2023-06-12 07:59:33.182255 cairocffi-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      777 2020-10-29 21:18:23.144438 cairocffi-1.6.0/utils/cairo_coverage.py
+-rw-r--r--   0        0        0     1390 2020-10-29 21:18:23.144438 cairocffi-1.6.0/utils/cairocffi_to_pycairo.py
+-rw-r--r--   0        0        0      756 2020-10-29 21:18:23.144438 cairocffi-1.6.0/utils/compare_pycairo.py
+-rw-r--r--   0        0        0     3001 2023-03-25 08:13:29.052671 cairocffi-1.6.0/utils/mkconstants.py
+-rw-r--r--   0        0        0     1853 2020-10-29 21:18:23.144438 cairocffi-1.6.0/utils/pango_example.py
+-rw-r--r--   0        0        0     1056 2020-10-29 21:18:23.144438 cairocffi-1.6.0/utils/pycairo_to_cairocffi.py
+-rw-r--r--   0        0        0      999 2023-03-11 07:55:03.041563 cairocffi-1.6.0/utils/tests.py
+-rw-r--r--   0        0        0     3319 1970-01-01 00:00:00.000000 cairocffi-1.6.0/PKG-INFO
```

### Comparing `cairocffi-1.5.1/LICENSE` & `cairocffi-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/README.rst` & `cairocffi-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/cairocffi/__init__.py` & `cairocffi-1.6.0/cairocffi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 """
 
 import sys
 from ctypes.util import find_library
 
 from . import constants
-from ._generated.ffi import ffi
+from .ffi import ffi
 
-VERSION = __version__ = '1.5.1'
+VERSION = __version__ = '1.6.0'
 # supported version of cairo, used to be pycairo version too:
 version = '1.17.2'
 version_info = (1, 17, 2)
 
 
 def dlopen(ffi, library_names, filenames):
     """Try various names for the same library, for different platforms."""
```

### Comparing `cairocffi-1.5.1/cairocffi/constants.py` & `cairocffi-1.6.0/cairocffi/constants.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/cairocffi/context.py` & `cairocffi-1.6.0/cairocffi/context.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/cairocffi/ffi_build.py` & `cairocffi-1.6.0/cairocffi/ffi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-    cairocffi.ffi_build
-    ~~~~~~~~~~~~~~~~~~~
+    cairocffi.ffi
+    ~~~~~~~~~~~~~
 
     Build the cffi bindings
 
     :copyright: Copyright 2013-2019 by Simon Sapin
     :license: BSD, see LICENSE for details.
 
 """
@@ -17,35 +17,29 @@
 # Path hack to import constants when this file is exec'd by setuptools
 constants_spec = spec_from_file_location(
     'constants', Path(__file__).parent.joinpath('constants.py')
 )
 constants = module_from_spec(constants_spec)
 constants_spec.loader.exec_module(constants)
 
-# Create an empty _generated folder if needed
-generated = Path(__file__).parent / '_generated'
-generated.mkdir(exist_ok=True)
-
 # Primary cffi definitions
 ffi = FFI()
-ffi.set_source('cairocffi._generated.ffi', None)
 ffi.cdef(constants._CAIRO_HEADERS)
 
 # include xcffib cffi definitions for cairo xcb support
 try:
-    from xcffib.ffi_build import ffi as xcb_ffi
+    from xcffib.ffi import ffi as xcb_ffi
 except ImportError:
     pass
 else:
     ffi.include(xcb_ffi)
     ffi.cdef(constants._CAIRO_XCB_HEADERS)
 
 # gdk pixbuf cffi definitions
 ffi_pixbuf = FFI()
-ffi_pixbuf.set_source('cairocffi._generated.ffi_pixbuf', None)
 ffi_pixbuf.include(ffi)
 ffi_pixbuf.cdef('''
     typedef unsigned long   gsize;
     typedef unsigned int    guint32;
     typedef unsigned int    guint;
     typedef unsigned char   guchar;
     typedef char            gchar;
@@ -98,21 +92,7 @@
 
 
     void              g_object_ref                   (gpointer object);
     void              g_object_unref                 (gpointer object);
     void              g_error_free                   (GError *error);
     void              g_type_init                    (void);
 ''')
-
-
-def compile():
-    ffi.compile()
-    ffi_path = generated / 'ffi.py'
-    ffi_path.write_text('# flake8: noqa\n' + ffi_path.read_text())
-    ffi_pixbuf.compile()
-    ffi_pixbuf_path = generated / 'ffi_pixbuf.py'
-    ffi_pixbuf_path.write_text(
-        '# flake8: noqa\n' + ffi_pixbuf_path.read_text())
-
-
-if __name__ == '__main__':
-    compile()
```

### Comparing `cairocffi-1.5.1/cairocffi/fonts.py` & `cairocffi-1.6.0/cairocffi/fonts.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/cairocffi/matrix.py` & `cairocffi-1.6.0/cairocffi/matrix.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/cairocffi/patterns.py` & `cairocffi-1.6.0/cairocffi/patterns.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/cairocffi/pixbuf.py` & `cairocffi-1.6.0/cairocffi/pixbuf.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import sys
 from array import array
 from functools import partial
 from io import BytesIO
 
 from . import Context, ImageSurface, constants, dlopen
-from ._generated.ffi_pixbuf import ffi
+from .ffi import ffi_pixbuf as ffi
 
 __all__ = ['decode_to_image_surface']
 
 gdk_pixbuf = dlopen(
     ffi, ('gdk_pixbuf-2.0', 'libgdk_pixbuf-2.0-0'),
     ('libgdk_pixbuf-2.0.so.0', 'libgdk_pixbuf-2.0.0.dylib',
      'libgdk_pixbuf-2.0-0.dll'))
```

### Comparing `cairocffi-1.5.1/cairocffi/surfaces.py` & `cairocffi-1.6.0/cairocffi/surfaces.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/cairocffi/test_cairo.py` & `cairocffi-1.6.0/cairocffi/test_cairo.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/cairocffi/test_pixbuf.py` & `cairocffi-1.6.0/cairocffi/test_pixbuf.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/cairocffi/test_xcb.py` & `cairocffi-1.6.0/cairocffi/test_xcb.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/cairocffi/xcb.py` & `cairocffi-1.6.0/cairocffi/xcb.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/docs/api.rst` & `cairocffi-1.6.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/docs/cffi_api.rst` & `cairocffi-1.6.0/docs/cffi_api.rst`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/docs/conf.py` & `cairocffi-1.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/docs/overview.rst` & `cairocffi-1.6.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/docs/pixbuf.rst` & `cairocffi-1.6.0/docs/pixbuf.rst`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/pyproject.toml` & `cairocffi-1.6.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 [build-system]
-requires = ["setuptools >= 61.0.0", "cffi >= 1.1.0"]
-build-backend = "build"
-backend-path = ["utils"]
+requires = ['flit_core >=3.2,<4']
+build-backend = 'flit_core.buildapi'
 
 [project]
-name = "cairocffi"
-description = "cffi-based cairo bindings for Python"
-readme = {file = "README.rst", content-type = "text/x-rst"}
-requires-python = ">=3.7"
-license = {file = "LICENSE"}
-keywords = ["cairo", "cffi", "binding"]
-authors = [
-    {name = "Simon Sapin", email = "contact@courtbouillon.org"}
+name = 'cairocffi'
+description = 'cffi-based cairo bindings for Python'
+keywords = ['cairo', 'cffi', 'binding']
+authors = [{name = 'Simon Sapin', email = 'contact@courtbouillon.org'}]
+maintainers = [{name = 'CourtBouillon', email = 'contact@courtbouillon.org'}]
+requires-python = '>=3.7'
+readme = {file = 'README.rst', content-type = 'text/x-rst'}
+license = {file = 'LICENSE'}
+dependencies = [
+    'cffi >= 1.1.0',
 ]
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: BSD License",
-    "Operating System :: POSIX :: Linux",
-    "Operating System :: MacOS :: MacOS X",
-    "Operating System :: Microsoft :: Windows",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Topic :: Multimedia :: Graphics"
-]
-dependencies = [
-    "cffi >= 1.1.0"
+    'Development Status :: 5 - Production/Stable',
+    'Intended Audience :: Developers',
+    'License :: OSI Approved :: BSD License',
+    'Operating System :: POSIX :: Linux',
+    'Operating System :: MacOS :: MacOS X',
+    'Operating System :: Microsoft :: Windows',
+    'Programming Language :: Python :: 3 :: Only',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Topic :: Multimedia :: Graphics',
 ]
-dynamic = ["version"]
+dynamic = ['version']
 
 [tool.setuptools.dynamic]
-version = {attr = "cairocffi.VERSION"}
+version = {attr = 'cairocffi.VERSION'}
 
 [project.urls]
-Documentation = "https://cairocffi.readthedocs.io/"
-Code = "https://github.com/Kozea/cairocffi/"
-Issues = "https://github.com/Kozea/cairocffi/issues"
-Donation = "https://opencollective.com/courtbouillon"
+Documentation = 'https://cairocffi.readthedocs.io/'
+Code = 'https://github.com/Kozea/cairocffi/'
+Issues = 'https://github.com/Kozea/cairocffi/issues'
+Changelog = 'https://cairocffi.readthedocs.io/en/stable/changelog.html'
+Donation = 'https://opencollective.com/courtbouillon'
 
 [project.optional-dependencies]
-doc = ["sphinx", "sphinx_rtd_theme"]
-test = ["pytest", "flake8", "isort", "numpy", "pikepdf"]
-xcb = ["xcffib >= 0.3.2"]
-
-[tool.pytest.ini_options]
-addopts = "--pyargs cairocffi"
-norecursedirs = "build dist .cache .eggs .git"
+doc = ['sphinx', 'sphinx_rtd_theme']
+test = ['pytest', 'flake8', 'isort', 'numpy', 'pikepdf']
+xcb = ['xcffib >= 1.4.0']
+
+[tool.flit.sdist]
+exclude = ['.*']
+
+[tool.coverage.run]
+branch = true
+include = ['cairocffi/*']
+
+[tool.coverage.report]
+exclude_lines = ['pragma: no cover', 'def __repr__', 'raise NotImplementedError']
+omit = ['.*']
 
 [tool.isort]
-default_section = "FIRSTPARTY"
+default_section = 'FIRSTPARTY'
 multi_line_output = 4
```

### Comparing `cairocffi-1.5.1/utils/cairo_coverage.py` & `cairocffi-1.6.0/utils/cairo_coverage.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/utils/cairocffi_to_pycairo.py` & `cairocffi-1.6.0/utils/cairocffi_to_pycairo.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/utils/compare_pycairo.py` & `cairocffi-1.6.0/utils/compare_pycairo.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/utils/mkconstants.py` & `cairocffi-1.6.0/utils/mkconstants.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/utils/pango_example.py` & `cairocffi-1.6.0/utils/pango_example.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/utils/pycairo_to_cairocffi.py` & `cairocffi-1.6.0/utils/pycairo_to_cairocffi.py`

 * *Files identical despite different names*

### Comparing `cairocffi-1.5.1/utils/tests.py` & `cairocffi-1.6.0/utils/tests.py`

 * *Files identical despite different names*

