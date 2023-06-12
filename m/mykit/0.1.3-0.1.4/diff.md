# Comparing `tmp/mykit-0.1.3.tar.gz` & `tmp/mykit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mykit-0.1.3.tar", last modified: Mon Jun 12 14:22:06 2023, max compression
+gzip compressed data, was "mykit-0.1.4.tar", last modified: Mon Jun 12 15:27:33 2023, max compression
```

## Comparing `mykit-0.1.3.tar` & `mykit-0.1.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.258652 mykit-0.1.3/
--rw-rw-rw-   0        0        0     1097 2023-04-10 22:01:23.000000 mykit-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     3832 2023-06-12 14:22:06.255653 mykit-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1984 2023-06-12 14:07:52.000000 mykit-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.005598 mykit-0.1.3/mykit/
--rw-rw-rw-   0        0        0      204 2023-06-12 13:37:25.000000 mykit-0.1.3/mykit/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-12 13:35:43.000000 mykit-0.1.3/mykit/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.182640 mykit-0.1.3/mykit/app/
--rw-rw-rw-   0        0        0     4152 2023-06-12 13:55:45.000000 mykit-0.1.3/mykit/app/arrow.py
--rw-rw-rw-   0        0        0    12892 2023-06-12 14:04:51.000000 mykit-0.1.3/mykit/app/button.py
--rw-rw-rw-   0        0        0     9010 2023-06-12 14:04:57.000000 mykit-0.1.3/mykit/app/label.py
--rw-rw-rw-   0        0        0    28006 2023-06-12 14:05:24.000000 mykit-0.1.3/mykit/app/slider.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.220646 mykit-0.1.3/mykit/kit/
--rw-rw-rw-   0        0        0     2965 2023-06-12 13:39:03.000000 mykit-0.1.3/mykit/kit/color.py
--rw-rw-rw-   0        0        0     5809 2023-06-12 11:57:08.000000 mykit-0.1.3/mykit/kit/ffmpeg.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.225647 mykit-0.1.3/mykit/kit/graph/
--rw-rw-rw-   0        0        0    16521 2023-06-12 12:03:05.000000 mykit-0.1.3/mykit/kit/graph/graph2d.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.233650 mykit-0.1.3/mykit/kit/keycrate/
--rw-rw-rw-   0        0        0     6473 2023-06-12 14:01:25.000000 mykit-0.1.3/mykit/kit/keycrate/__init__.py
--rw-rw-rw-   0        0        0     2741 2023-06-12 12:12:05.000000 mykit-0.1.3/mykit/kit/math.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.244653 mykit-0.1.3/mykit/kit/neuralnet/
--rw-rw-rw-   0        0        0     7320 2023-06-12 14:05:32.000000 mykit-0.1.3/mykit/kit/neuralnet/dense.py
--rw-rw-rw-   0        0        0    15109 2023-06-12 14:05:43.000000 mykit-0.1.3/mykit/kit/neuralnet/genetic.py
--rw-rw-rw-   0        0        0     3039 2023-05-06 18:30:49.000000 mykit-0.1.3/mykit/kit/noise.py
--rw-rw-rw-   0        0        0     4253 2023-05-18 13:55:09.000000 mykit-0.1.3/mykit/kit/path.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.252652 mykit-0.1.3/mykit/kit/quick_visual/
--rw-rw-rw-   0        0        0      841 2023-06-12 14:06:19.000000 mykit-0.1.3/mykit/kit/quick_visual/plot2d.py
--rw-rw-rw-   0        0        0      403 2023-06-11 18:43:02.000000 mykit-0.1.3/mykit/kit/text.py
--rw-rw-rw-   0        0        0     2453 2023-06-12 11:34:47.000000 mykit-0.1.3/mykit/kit/time.py
--rw-rw-rw-   0        0        0     3156 2023-05-18 13:20:09.000000 mykit-0.1.3/mykit/kit/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.070614 mykit-0.1.3/mykit.egg-info/
--rw-rw-rw-   0        0        0     3832 2023-06-12 14:22:05.000000 mykit-0.1.3/mykit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2023-06-12 14:22:05.000000 mykit-0.1.3/mykit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 14:22:05.000000 mykit-0.1.3/mykit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-12 14:22:05.000000 mykit-0.1.3/mykit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      688 2023-06-12 14:19:03.000000 mykit-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 14:22:06.259653 mykit-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 15:27:33.649030 mykit-0.1.4/
+-rw-rw-rw-   0        0        0     1097 2023-04-10 22:01:23.000000 mykit-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     4180 2023-06-12 15:27:33.645027 mykit-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1984 2023-06-12 14:07:52.000000 mykit-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 15:27:33.385963 mykit-0.1.4/mykit/
+-rw-rw-rw-   0        0        0      204 2023-06-12 13:37:25.000000 mykit-0.1.4/mykit/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-12 15:25:34.000000 mykit-0.1.4/mykit/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:27:33.540002 mykit-0.1.4/mykit/app/
+-rw-rw-rw-   0        0        0     4152 2023-06-12 13:55:45.000000 mykit-0.1.4/mykit/app/arrow.py
+-rw-rw-rw-   0        0        0    12892 2023-06-12 14:04:51.000000 mykit-0.1.4/mykit/app/button.py
+-rw-rw-rw-   0        0        0     9010 2023-06-12 14:04:57.000000 mykit-0.1.4/mykit/app/label.py
+-rw-rw-rw-   0        0        0    28006 2023-06-12 14:05:24.000000 mykit-0.1.4/mykit/app/slider.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:27:33.605017 mykit-0.1.4/mykit/kit/
+-rw-rw-rw-   0        0        0     2965 2023-06-12 13:39:03.000000 mykit-0.1.4/mykit/kit/color.py
+-rw-rw-rw-   0        0        0     5809 2023-06-12 11:57:08.000000 mykit-0.1.4/mykit/kit/ffmpeg.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:27:33.615023 mykit-0.1.4/mykit/kit/graph/
+-rw-rw-rw-   0        0        0    16521 2023-06-12 12:03:05.000000 mykit-0.1.4/mykit/kit/graph/graph2d.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:27:33.622022 mykit-0.1.4/mykit/kit/keycrate/
+-rw-rw-rw-   0        0        0     6473 2023-06-12 14:01:25.000000 mykit-0.1.4/mykit/kit/keycrate/__init__.py
+-rw-rw-rw-   0        0        0     2741 2023-06-12 12:12:05.000000 mykit-0.1.4/mykit/kit/math.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:27:33.631024 mykit-0.1.4/mykit/kit/neuralnet/
+-rw-rw-rw-   0        0        0     7320 2023-06-12 14:05:32.000000 mykit-0.1.4/mykit/kit/neuralnet/dense.py
+-rw-rw-rw-   0        0        0    15109 2023-06-12 14:05:43.000000 mykit-0.1.4/mykit/kit/neuralnet/genetic.py
+-rw-rw-rw-   0        0        0     3039 2023-05-06 18:30:49.000000 mykit-0.1.4/mykit/kit/noise.py
+-rw-rw-rw-   0        0        0     4253 2023-05-18 13:55:09.000000 mykit-0.1.4/mykit/kit/path.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:27:33.638026 mykit-0.1.4/mykit/kit/quick_visual/
+-rw-rw-rw-   0        0        0      841 2023-06-12 14:06:19.000000 mykit-0.1.4/mykit/kit/quick_visual/plot2d.py
+-rw-rw-rw-   0        0        0      403 2023-06-11 18:43:02.000000 mykit-0.1.4/mykit/kit/text.py
+-rw-rw-rw-   0        0        0     2453 2023-06-12 11:34:47.000000 mykit-0.1.4/mykit/kit/time.py
+-rw-rw-rw-   0        0        0     3156 2023-05-18 13:20:09.000000 mykit-0.1.4/mykit/kit/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:27:33.489988 mykit-0.1.4/mykit.egg-info/
+-rw-rw-rw-   0        0        0     4180 2023-06-12 15:27:33.000000 mykit-0.1.4/mykit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2023-06-12 15:27:33.000000 mykit-0.1.4/mykit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 15:27:33.000000 mykit-0.1.4/mykit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 15:27:33.000000 mykit-0.1.4/mykit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1242 2023-06-12 15:25:22.000000 mykit-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 15:27:33.650029 mykit-0.1.4/setup.cfg
```

### Comparing `mykit-0.1.3/LICENSE` & `mykit-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/PKG-INFO` & `mykit-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python utility library
 Author-email: Nicholas Valentinus <nvfastplease@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Nicholas Valentinus
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,18 +24,25 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: repo, https://github.com/nvfp/mykit
 Project-URL: tracker, https://github.com/nvfp/mykit/issues
 Keywords: python,toolkit,mykit
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # myKit
```

### Comparing `mykit-0.1.3/README.md` & `mykit-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/mykit/app/arrow.py` & `mykit-0.1.4/mykit/app/arrow.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/mykit/app/button.py` & `mykit-0.1.4/mykit/app/button.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/mykit/app/label.py` & `mykit-0.1.4/mykit/app/label.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/mykit/app/slider.py` & `mykit-0.1.4/mykit/app/slider.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/mykit/kit/color.py` & `mykit-0.1.4/mykit/kit/color.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/mykit/kit/ffmpeg.py` & `mykit-0.1.4/mykit/kit/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/mykit/kit/graph/graph2d.py` & `mykit-0.1.4/mykit/kit/graph/graph2d.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/mykit/kit/keycrate/__init__.py` & `mykit-0.1.4/mykit/kit/keycrate/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/mykit/kit/math.py` & `mykit-0.1.4/mykit/kit/math.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/mykit/kit/neuralnet/dense.py` & `mykit-0.1.4/mykit/kit/neuralnet/dense.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/mykit/kit/neuralnet/genetic.py` & `mykit-0.1.4/mykit/kit/neuralnet/genetic.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/mykit/kit/noise.py` & `mykit-0.1.4/mykit/kit/noise.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/mykit/kit/path.py` & `mykit-0.1.4/mykit/kit/path.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/mykit/kit/quick_visual/plot2d.py` & `mykit-0.1.4/mykit/kit/quick_visual/plot2d.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/mykit/kit/time.py` & `mykit-0.1.4/mykit/kit/time.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/mykit/kit/utils.py` & `mykit-0.1.4/mykit/kit/utils.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/mykit.egg-info/PKG-INFO` & `mykit-0.1.4/mykit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python utility library
 Author-email: Nicholas Valentinus <nvfastplease@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Nicholas Valentinus
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,18 +24,25 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: repo, https://github.com/nvfp/mykit
 Project-URL: tracker, https://github.com/nvfp/mykit/issues
 Keywords: python,toolkit,mykit
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # myKit
```

### Comparing `mykit-0.1.3/mykit.egg-info/SOURCES.txt` & `mykit-0.1.4/mykit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mykit-0.1.3/pyproject.toml` & `mykit-0.1.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,48 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mykit"
-version = "0.1.3"
+version = "0.1.4"
 description = "Python utility library"
 authors = [
   {name = "Nicholas Valentinus", email = "nvfastplease@gmail.com"},
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 classifiers = [
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
+	"Topic :: Scientific/Engineering",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+	"Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3 :: Only",
+    "Natural Language :: English"
 ]
 keywords = ["python", "toolkit", "mykit"]
 
 
+[metadata]
+author = "Nicholas Valentinus"
+home_page = "https://github.com/nvfp/mykit"
+license = "MIT"
+
+[options]
+packages = ["mykit123xyz456abc"]
+include_package_data = true
+install_requires = [
+	"numba>=0.55.2",
+	"numpy>=1.22.4"
+]
+
+
 [project.urls]
 repo = "https://github.com/nvfp/mykit"
 tracker = "https://github.com/nvfp/mykit/issues"
```

