# Comparing `tmp/pixelsort-cli-0.1.6.tar.gz` & `tmp/pixelsort-cli-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelsort-cli-0.1.6.tar", last modified: Tue Apr 18 21:10:10 2023, max compression
+gzip compressed data, was "pixelsort-cli-0.1.7.tar", last modified: Mon Jun 12 20:23:07 2023, max compression
```

## Comparing `pixelsort-cli-0.1.6.tar` & `pixelsort-cli-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:10.591190 pixelsort-cli-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-18 21:10:10.591190 pixelsort-cli-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:10:10.591190 pixelsort-cli-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:10.587190 pixelsort-cli-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:10.591190 pixelsort-cli-0.1.6/src/pixelsort/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/src/pixelsort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/src/pixelsort/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/src/pixelsort/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/src/pixelsort/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/src/pixelsort/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:10.591190 pixelsort-cli-0.1.6/src/pixelsort_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-18 21:10:10.000000 pixelsort-cli-0.1.6/src/pixelsort_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-18 21:10:10.000000 pixelsort-cli-0.1.6/src/pixelsort_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:10:10.000000 pixelsort-cli-0.1.6/src/pixelsort_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-18 21:10:10.000000 pixelsort-cli-0.1.6/src/pixelsort_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 21:10:10.000000 pixelsort-cli-0.1.6/src/pixelsort_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 21:10:10.000000 pixelsort-cli-0.1.6/src/pixelsort_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:10.591190 pixelsort-cli-0.1.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/test/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:23:07.765127 pixelsort-cli-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-12 20:22:54.000000 pixelsort-cli-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-12 20:23:07.765127 pixelsort-cli-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-12 20:22:54.000000 pixelsort-cli-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-12 20:22:54.000000 pixelsort-cli-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 20:23:07.765127 pixelsort-cli-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-12 20:22:54.000000 pixelsort-cli-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:23:07.761127 pixelsort-cli-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:23:07.761127 pixelsort-cli-0.1.7/src/pixelsort/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-12 20:22:54.000000 pixelsort-cli-0.1.7/src/pixelsort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-12 20:22:54.000000 pixelsort-cli-0.1.7/src/pixelsort/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-12 20:22:54.000000 pixelsort-cli-0.1.7/src/pixelsort/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-12 20:22:54.000000 pixelsort-cli-0.1.7/src/pixelsort/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:23:07.761127 pixelsort-cli-0.1.7/src/pixelsort_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-12 20:23:07.000000 pixelsort-cli-0.1.7/src/pixelsort_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-12 20:23:07.000000 pixelsort-cli-0.1.7/src/pixelsort_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:23:07.000000 pixelsort-cli-0.1.7/src/pixelsort_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-12 20:23:07.000000 pixelsort-cli-0.1.7/src/pixelsort_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-12 20:23:07.000000 pixelsort-cli-0.1.7/src/pixelsort_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 20:23:07.000000 pixelsort-cli-0.1.7/src/pixelsort_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:23:07.761127 pixelsort-cli-0.1.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-12 20:22:54.000000 pixelsort-cli-0.1.7/test/test_image.py
```

### Comparing `pixelsort-cli-0.1.6/LICENSE` & `pixelsort-cli-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pixelsort-cli-0.1.6/PKG-INFO` & `pixelsort-cli-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pixelsort-cli
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python CLI tool for sorting pixels in images.
 Author-email: Ferdinand Theil <f.p.theil@proton.me>
 Project-URL: Homepage, https://github.com/Blotz/pixelsort-cli
 Project-URL: Bug Tracker, https://github.com/Blotz/pixelsort-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # pixelsort cli
 
-![tests](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-package.yml/badge.svg)
-![package](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-publish.yml/badge.svg)
+[![tests](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-package.yml/badge.svg)](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-package.yml)
+[![package](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-publish.yml)
+[![CodeQL](https://github.com/Blotz/pixelsort-cli/actions/workflows/codeql.yml/badge.svg)](https://github.com/Blotz/pixelsort-cli/actions/workflows/codeql.yml)
 
 A simple python command line tool for sort pixels in an image.
 Based on the works of [Kim Asendorf](https://github.com/kimasendorf/ASDFPixelSort).
 
 The script blocks pixels into dark and light areas using a contrast mask.
 Then it sorts the pixels in a given direction via their luminance.
 
@@ -44,34 +45,36 @@
 ## Examples
 
 ```bash
 pixelsort --help
 ```
 
 ```bash
-usage: pixelsort [-h] [--threshold THRESHOLD] [--invert INVERT] [--reverse_sorting REVERSE_SORTING] [--output OUTPUT] image_path {up,down,left,right}
+usage: pixelsort [-h] [--threshold THRESHOLD] [--sort_brightest SORT_BRIGHTEST] [--reverse_sorting REVERSE_SORTING] [--output OUTPUT]
+                 image_path angle
 
-Command line tool for sorting pixels
+Command line tool for sorting pixels in images
 
 positional arguments:
   image_path            path to image
-  {up,down,left,right}  direction to sort pixels
+  angle                 angle that the image is sorted. 0° is up. [0, 360]
 
 options:
   -h, --help            show this help message and exit
   --threshold THRESHOLD
-                        threshold for contrast
-  --invert INVERT       invert the selected area
+                        threshold for contrast. [-1.0, 1.0] Default: 1.0
+  --sort_brightest SORT_BRIGHTEST
+                        Sort the brightest area of the image. Default: True
   --reverse_sorting REVERSE_SORTING
-                        reverse the sorting direction
+                        Sorts the pixels from lightest to darkest instead of darkest to lightest. Default: False
   --output OUTPUT       path to output file
 ```
 
 ```bash
-pixelsort  data/mountains.jpg right --threshold 1.2 --invert True --output out.png
+pixelsort data/mountains.jpg 90 --threshold 1.2
 ```
 
 ![example 1](https://raw.githubusercontent.com/Blotz/pixelsort-cli/main/data/example1.png)
 
 ---
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pixelsort-cli-0.1.6/README.md` & `pixelsort-cli-0.1.7/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # pixelsort cli
 
-![tests](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-package.yml/badge.svg)
-![package](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-publish.yml/badge.svg)
+[![tests](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-package.yml/badge.svg)](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-package.yml)
+[![package](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-publish.yml)
+[![CodeQL](https://github.com/Blotz/pixelsort-cli/actions/workflows/codeql.yml/badge.svg)](https://github.com/Blotz/pixelsort-cli/actions/workflows/codeql.yml)
 
 A simple python command line tool for sort pixels in an image.
 Based on the works of [Kim Asendorf](https://github.com/kimasendorf/ASDFPixelSort).
 
 The script blocks pixels into dark and light areas using a contrast mask.
 Then it sorts the pixels in a given direction via their luminance.
 
@@ -29,34 +30,36 @@
 ## Examples
 
 ```bash
 pixelsort --help
 ```
 
 ```bash
-usage: pixelsort [-h] [--threshold THRESHOLD] [--invert INVERT] [--reverse_sorting REVERSE_SORTING] [--output OUTPUT] image_path {up,down,left,right}
+usage: pixelsort [-h] [--threshold THRESHOLD] [--sort_brightest SORT_BRIGHTEST] [--reverse_sorting REVERSE_SORTING] [--output OUTPUT]
+                 image_path angle
 
-Command line tool for sorting pixels
+Command line tool for sorting pixels in images
 
 positional arguments:
   image_path            path to image
-  {up,down,left,right}  direction to sort pixels
+  angle                 angle that the image is sorted. 0° is up. [0, 360]
 
 options:
   -h, --help            show this help message and exit
   --threshold THRESHOLD
-                        threshold for contrast
-  --invert INVERT       invert the selected area
+                        threshold for contrast. [-1.0, 1.0] Default: 1.0
+  --sort_brightest SORT_BRIGHTEST
+                        Sort the brightest area of the image. Default: True
   --reverse_sorting REVERSE_SORTING
-                        reverse the sorting direction
+                        Sorts the pixels from lightest to darkest instead of darkest to lightest. Default: False
   --output OUTPUT       path to output file
 ```
 
 ```bash
-pixelsort  data/mountains.jpg right --threshold 1.2 --invert True --output out.png
+pixelsort data/mountains.jpg 90 --threshold 1.2
 ```
 
 ![example 1](https://raw.githubusercontent.com/Blotz/pixelsort-cli/main/data/example1.png)
 
 ---
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pixelsort-cli-0.1.6/pyproject.toml` & `pixelsort-cli-0.1.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pixelsort-cli"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
     {name = "Ferdinand Theil", email = "f.p.theil@proton.me"},
 ]
 description = "A Python CLI tool for sorting pixels in images."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    'numpy',
-    'opencv-python',
-    'filetype'
+    'numpy~=1.24.3',
+    'scipy~=1.10.1',
+    'opencv-python~=4.7.0.72',
+    'filetype~=1.2.0'
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Blotz/pixelsort-cli"
 "Bug Tracker" = "https://github.com/Blotz/pixelsort-cli/issues"
 
 [project.scripts]
 pixelsort = "pixelsort.__main__:main"
 
 [project.optional-dependencies]
 test = [
-    'pytest'
+    'pytest~=7.3.2'
 ]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
 testpaths = [
     "tests"
```

### Comparing `pixelsort-cli-0.1.6/src/pixelsort/cli.py` & `pixelsort-cli-0.1.7/src/pixelsort/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 """cli.py
 The main entry point of our application. 
 Handles all tui actions. 
 """
 
 import pathlib
 import filetype
+import logging
+
+logger = logging.getLogger(__name__)
 
 
 def valid_read_image_path(image_path: pathlib.Path) -> bool:
     """checks if the given path is a valid image path
 
     Args:
         image_path (pathlib.Path): the path to check
 
     Returns:
         bool: True if the path is valid, False otherwise
     """
     if not image_path.exists():
-        print("image path invalid: File does not exist")
+        logger.error("image path invalid: File does not exist")
         return False
 
     if not image_path.is_file():
-        print("image path invalid: Path does not point to File")
+        logger.error("image path invalid: Path does not point to File")
         return False
 
     if not filetype.is_image(image_path):
-        print("image path invalid: File is not image")
+        logger.error("image path invalid: File is not image")
         return False
     
     return True
 
 
 def valid_write_image_path(image_path: pathlib.Path) -> bool:
     """checks if the given path is a valid image path
@@ -38,19 +41,18 @@
         image_path (pathlib.Path): the path to check
 
     Returns:
         bool: True if the path is valid, False otherwise
     """
     # validate parent directory
     if not image_path.parent.exists():
-        print("output path invalid: Parent directory does not exist")
+        logger.error("output path invalid: Parent directory does not exist")
         return False
     
     if not image_path.parent.is_dir():
-        print("output path invalid: Parent directory is not a directory")
+        logger.error("output path invalid: Parent directory is not a directory")
         return False
 
-    # print warning if file already exists
     if image_path.exists():
-        print("WARNING: output file already exists. Overwriting file")
+        logger.warn("WARNING: output file already exists. Overwriting file")
     
     return True
```

### Comparing `pixelsort-cli-0.1.6/src/pixelsort/image.py` & `pixelsort-cli-0.1.7/src/pixelsort/image.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,67 @@
 """image.py
 All image processing functions
 """
-from pixelsort.direction import Direction
 import numpy as np
 import cv2
+import scipy
+import logging
 
+logger = logging.getLogger(__name__)
 
-def process_image(image: np.ndarray, direction: Direction, threshold: float, invert: bool, reverse_sort: bool) -> None:
-    """process the given image
+
+def process_image(image: np.ndarray, angle: float, threshold: float, sort_brightest: bool, reverse_sort: bool) -> np.ndarray:
+    """
+    Sorts the image in the given direction
 
     Args:
-        image (np.ndarray): the image to processed
-        direction (Direction): the direction to sort the pixels
-        threshold (float): the threshold for the contrast mask
-        invert (bool): True if the selected area should be inverted
-        reverse_sort (bool): True if the pixels should be sorted in reverse
+        image (np.ndarray): the image to sort
+        angle (float): the angle to sort the image
+        threshold (float): the threshold for contrast
+        sort_brightest (bool): sort the brightest area of the image
+        reverse_sort (bool): sort the pixels from lightest to darkest instead of darkest to lightest
+
+    Returns:
+        np.ndarray: the sorted image
     """
-    is_sort_reverse = direction in [Direction.UP, Direction.LEFT]
-    is_vertical = direction in [Direction.UP, Direction.DOWN]
 
-    print(f"Processing image with {direction.name} direction, threshold={threshold}, invert={invert}, reverse_sort={reverse_sort}")
+    logger.info(f"Processing image with angle={angle}, threshold={threshold}, sort_brightest={sort_brightest}, reverse_sort={reverse_sort}")
+
+    logger.debug("Rotating image...")
+    image_shape = np.shape(image)
+    image = scipy.ndimage.rotate(image, angle, mode='reflect')
 
+    logger.debug("Calculating areas of light and dark...")
     contrast: np.ndarray = create_contrast_mask(image, threshold)
-    if invert:  # invert image if sorting in reverse
+    if sort_brightest:  # invert image if we are trying to sort the brightest areas
         contrast: np.ndarray = cv2.bitwise_not(contrast)
-    # show_image(contrast)
-    # flip sort direction if sorting in reverse
-    if reverse_sort:
-        is_sort_reverse = not is_sort_reverse
-
-    if is_vertical:
-        for x in range(image.shape[1]):
-            column_contrast = contrast[:, x]
-            column_image = image[:, x]
-            process_slice(column_contrast, column_image, is_sort_reverse)
-    else:
-        for y in range(image.shape[0]):
-            row_contrast = contrast[y, :]
-            row_image = image[y, :]
-            process_slice(row_contrast, row_image, is_sort_reverse)
+    
+    logger.debug("Sorting image...")
+    for x in range(image.shape[1]):
+        column_contrast = contrast[:, x]
+        column_image = image[:, x]
+        process_slice(column_contrast, column_image, reverse_sort)
+
+    logger.debug("Unrotating...")
+    image = scipy.ndimage.rotate(image, -angle, mode='constant')
+    new_image_shape = np.shape(image)
+    image = image[int(new_image_shape[0]/2 - image_shape[0]/2):int(new_image_shape[0]/2 + image_shape[0]/2),
+                  int(new_image_shape[1]/2 - image_shape[1]/2):int(new_image_shape[1]/2 + image_shape[1]/2)]    
 
-    print("Done")
+    logger.info("Done!")
+    return image
 
 
-def process_slice(contrast_slice: np.ndarray, image_slice: np.ndarray, is_sort_reverse: bool) -> None:
+def process_slice(contrast_slice: np.ndarray, image_slice: np.ndarray, reverse: bool) -> None:
     """process a slice of the image
 
     Args:
         contrast_slice (np.ndarray): 1d slice of the contrast mask
         image_slice (np.ndarray): 1d slice of the image
-        is_sort_reverse (bool): True if the pixels should be sorted in reverse
+        reverse (bool): True if the pixels should be sorted in reverse
     """
     black_pixels, = np.where(contrast_slice == 0)
     white_pixels, = np.where(contrast_slice == 255)
 
     # loop through black pixels in this row
     while black_pixels.size > 0 or white_pixels.size > 0:
         # get the next black pixel
@@ -67,15 +75,15 @@
         # get the next white pixel
         if white_pixels.size == 0:  # no more white pixels
             x2 = contrast_slice.shape[0]
         else:
             x2 = white_pixels[0] - 1
 
         # sort pixels by luminance
-        sort_pixels(image_slice[x1:x2], reverse=is_sort_reverse)
+        sort_pixels(image_slice[x1:x2], reverse=reverse)
         # print(x1, x2, end=" ")
 
         # remove all black pixels before the next white pixel
         black_pixels = black_pixels[black_pixels > x2]
 
 
 def create_contrast_mask(image: np.ndarray, threshold: float) -> np.ndarray:
```

### Comparing `pixelsort-cli-0.1.6/src/pixelsort_cli.egg-info/PKG-INFO` & `pixelsort-cli-0.1.7/src/pixelsort_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pixelsort-cli
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python CLI tool for sorting pixels in images.
 Author-email: Ferdinand Theil <f.p.theil@proton.me>
 Project-URL: Homepage, https://github.com/Blotz/pixelsort-cli
 Project-URL: Bug Tracker, https://github.com/Blotz/pixelsort-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # pixelsort cli
 
-![tests](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-package.yml/badge.svg)
-![package](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-publish.yml/badge.svg)
+[![tests](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-package.yml/badge.svg)](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-package.yml)
+[![package](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-publish.yml)
+[![CodeQL](https://github.com/Blotz/pixelsort-cli/actions/workflows/codeql.yml/badge.svg)](https://github.com/Blotz/pixelsort-cli/actions/workflows/codeql.yml)
 
 A simple python command line tool for sort pixels in an image.
 Based on the works of [Kim Asendorf](https://github.com/kimasendorf/ASDFPixelSort).
 
 The script blocks pixels into dark and light areas using a contrast mask.
 Then it sorts the pixels in a given direction via their luminance.
 
@@ -44,34 +45,36 @@
 ## Examples
 
 ```bash
 pixelsort --help
 ```
 
 ```bash
-usage: pixelsort [-h] [--threshold THRESHOLD] [--invert INVERT] [--reverse_sorting REVERSE_SORTING] [--output OUTPUT] image_path {up,down,left,right}
+usage: pixelsort [-h] [--threshold THRESHOLD] [--sort_brightest SORT_BRIGHTEST] [--reverse_sorting REVERSE_SORTING] [--output OUTPUT]
+                 image_path angle
 
-Command line tool for sorting pixels
+Command line tool for sorting pixels in images
 
 positional arguments:
   image_path            path to image
-  {up,down,left,right}  direction to sort pixels
+  angle                 angle that the image is sorted. 0° is up. [0, 360]
 
 options:
   -h, --help            show this help message and exit
   --threshold THRESHOLD
-                        threshold for contrast
-  --invert INVERT       invert the selected area
+                        threshold for contrast. [-1.0, 1.0] Default: 1.0
+  --sort_brightest SORT_BRIGHTEST
+                        Sort the brightest area of the image. Default: True
   --reverse_sorting REVERSE_SORTING
-                        reverse the sorting direction
+                        Sorts the pixels from lightest to darkest instead of darkest to lightest. Default: False
   --output OUTPUT       path to output file
 ```
 
 ```bash
-pixelsort  data/mountains.jpg right --threshold 1.2 --invert True --output out.png
+pixelsort data/mountains.jpg 90 --threshold 1.2
 ```
 
 ![example 1](https://raw.githubusercontent.com/Blotz/pixelsort-cli/main/data/example1.png)
 
 ---
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

