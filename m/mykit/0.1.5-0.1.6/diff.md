# Comparing `tmp/mykit-0.1.5.tar.gz` & `tmp/mykit-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mykit-0.1.5.tar", last modified: Mon Jun 12 16:32:25 2023, max compression
+gzip compressed data, was "mykit-0.1.6.tar", last modified: Mon Jun 12 16:51:26 2023, max compression
```

## Comparing `mykit-0.1.5.tar` & `mykit-0.1.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 16:32:25.538090 mykit-0.1.5/
--rw-rw-rw-   0        0        0     1097 2023-04-10 22:01:23.000000 mykit-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     2926 2023-06-12 16:32:25.535090 mykit-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1984 2023-06-12 14:07:52.000000 mykit-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 16:32:25.154018 mykit-0.1.5/mykit/
--rw-rw-rw-   0        0        0      204 2023-06-12 13:37:25.000000 mykit-0.1.5/mykit/__init__.py
--rw-rw-rw-   0        0        0      123 2023-06-12 16:18:47.000000 mykit-0.1.5/mykit/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 16:32:25.377049 mykit-0.1.5/mykit/app/
--rw-rw-rw-   0        0        0     4152 2023-06-12 13:55:45.000000 mykit-0.1.5/mykit/app/arrow.py
--rw-rw-rw-   0        0        0    12892 2023-06-12 14:04:51.000000 mykit-0.1.5/mykit/app/button.py
--rw-rw-rw-   0        0        0     9010 2023-06-12 14:04:57.000000 mykit-0.1.5/mykit/app/label.py
--rw-rw-rw-   0        0        0    28006 2023-06-12 14:05:24.000000 mykit-0.1.5/mykit/app/slider.py
-drwxrwxrwx   0        0        0        0 2023-06-12 16:32:25.437064 mykit-0.1.5/mykit/kit/
--rw-rw-rw-   0        0        0     2965 2023-06-12 13:39:03.000000 mykit-0.1.5/mykit/kit/color.py
--rw-rw-rw-   0        0        0     5809 2023-06-12 11:57:08.000000 mykit-0.1.5/mykit/kit/ffmpeg.py
-drwxrwxrwx   0        0        0        0 2023-06-12 16:32:25.470075 mykit-0.1.5/mykit/kit/graph/
--rw-rw-rw-   0        0        0    16521 2023-06-12 12:03:05.000000 mykit-0.1.5/mykit/kit/graph/graph2d.py
-drwxrwxrwx   0        0        0        0 2023-06-12 16:32:25.473074 mykit-0.1.5/mykit/kit/keycrate/
--rw-rw-rw-   0        0        0     6473 2023-06-12 14:01:25.000000 mykit-0.1.5/mykit/kit/keycrate/__init__.py
--rw-rw-rw-   0        0        0     2741 2023-06-12 12:12:05.000000 mykit-0.1.5/mykit/kit/math.py
-drwxrwxrwx   0        0        0        0 2023-06-12 16:32:25.496084 mykit-0.1.5/mykit/kit/neuralnet/
--rw-rw-rw-   0        0        0     7320 2023-06-12 14:05:32.000000 mykit-0.1.5/mykit/kit/neuralnet/dense.py
--rw-rw-rw-   0        0        0    15109 2023-06-12 14:05:43.000000 mykit-0.1.5/mykit/kit/neuralnet/genetic.py
--rw-rw-rw-   0        0        0     3039 2023-05-06 18:30:49.000000 mykit-0.1.5/mykit/kit/noise.py
--rw-rw-rw-   0        0        0     4253 2023-05-18 13:55:09.000000 mykit-0.1.5/mykit/kit/path.py
-drwxrwxrwx   0        0        0        0 2023-06-12 16:32:25.503082 mykit-0.1.5/mykit/kit/quick_visual/
--rw-rw-rw-   0        0        0      841 2023-06-12 14:06:19.000000 mykit-0.1.5/mykit/kit/quick_visual/plot2d.py
--rw-rw-rw-   0        0        0      403 2023-06-11 18:43:02.000000 mykit-0.1.5/mykit/kit/text.py
--rw-rw-rw-   0        0        0     2453 2023-06-12 11:34:47.000000 mykit-0.1.5/mykit/kit/time.py
--rw-rw-rw-   0        0        0     3156 2023-05-18 13:20:09.000000 mykit-0.1.5/mykit/kit/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 16:32:25.363051 mykit-0.1.5/mykit.egg-info/
--rw-rw-rw-   0        0        0     2926 2023-06-12 16:32:24.000000 mykit-0.1.5/mykit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      622 2023-06-12 16:32:25.000000 mykit-0.1.5/mykit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 16:32:24.000000 mykit-0.1.5/mykit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-12 16:32:24.000000 mykit-0.1.5/mykit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2023-06-12 16:32:24.000000 mykit-0.1.5/mykit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-12 16:32:24.000000 mykit-0.1.5/mykit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1119 2023-06-12 16:31:00.000000 mykit-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 16:32:25.539092 mykit-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 16:51:26.179941 mykit-0.1.6/
+-rw-rw-rw-   0        0        0     1097 2023-04-10 22:01:23.000000 mykit-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     3098 2023-06-12 16:51:26.175939 mykit-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1984 2023-06-12 14:07:52.000000 mykit-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 16:51:25.992894 mykit-0.1.6/mykit/
+-rw-rw-rw-   0        0        0      204 2023-06-12 13:37:25.000000 mykit-0.1.6/mykit/__init__.py
+-rw-rw-rw-   0        0        0      134 2023-06-12 16:47:42.000000 mykit-0.1.6/mykit/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:51:26.100920 mykit-0.1.6/mykit/app/
+-rw-rw-rw-   0        0        0     4152 2023-06-12 13:55:45.000000 mykit-0.1.6/mykit/app/arrow.py
+-rw-rw-rw-   0        0        0    12892 2023-06-12 14:04:51.000000 mykit-0.1.6/mykit/app/button.py
+-rw-rw-rw-   0        0        0     9010 2023-06-12 14:04:57.000000 mykit-0.1.6/mykit/app/label.py
+-rw-rw-rw-   0        0        0    28006 2023-06-12 14:05:24.000000 mykit-0.1.6/mykit/app/slider.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:51:26.143932 mykit-0.1.6/mykit/kit/
+-rw-rw-rw-   0        0        0     2965 2023-06-12 13:39:03.000000 mykit-0.1.6/mykit/kit/color.py
+-rw-rw-rw-   0        0        0     5809 2023-06-12 11:57:08.000000 mykit-0.1.6/mykit/kit/ffmpeg.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:51:26.147931 mykit-0.1.6/mykit/kit/graph/
+-rw-rw-rw-   0        0        0    16521 2023-06-12 12:03:05.000000 mykit-0.1.6/mykit/kit/graph/graph2d.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:51:26.156941 mykit-0.1.6/mykit/kit/keycrate/
+-rw-rw-rw-   0        0        0     6473 2023-06-12 14:01:25.000000 mykit-0.1.6/mykit/kit/keycrate/__init__.py
+-rw-rw-rw-   0        0        0     2741 2023-06-12 12:12:05.000000 mykit-0.1.6/mykit/kit/math.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:51:26.164942 mykit-0.1.6/mykit/kit/neuralnet/
+-rw-rw-rw-   0        0        0     7320 2023-06-12 14:05:32.000000 mykit-0.1.6/mykit/kit/neuralnet/dense.py
+-rw-rw-rw-   0        0        0    15109 2023-06-12 14:05:43.000000 mykit-0.1.6/mykit/kit/neuralnet/genetic.py
+-rw-rw-rw-   0        0        0     3039 2023-05-06 18:30:49.000000 mykit-0.1.6/mykit/kit/noise.py
+-rw-rw-rw-   0        0        0     4253 2023-05-18 13:55:09.000000 mykit-0.1.6/mykit/kit/path.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:51:26.172939 mykit-0.1.6/mykit/kit/quick_visual/
+-rw-rw-rw-   0        0        0      841 2023-06-12 14:06:19.000000 mykit-0.1.6/mykit/kit/quick_visual/plot2d.py
+-rw-rw-rw-   0        0        0      403 2023-06-11 18:43:02.000000 mykit-0.1.6/mykit/kit/text.py
+-rw-rw-rw-   0        0        0     2453 2023-06-12 11:34:47.000000 mykit-0.1.6/mykit/kit/time.py
+-rw-rw-rw-   0        0        0     3156 2023-05-18 13:20:09.000000 mykit-0.1.6/mykit/kit/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:51:26.084921 mykit-0.1.6/mykit.egg-info/
+-rw-rw-rw-   0        0        0     3098 2023-06-12 16:51:25.000000 mykit-0.1.6/mykit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      622 2023-06-12 16:51:25.000000 mykit-0.1.6/mykit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 16:51:25.000000 mykit-0.1.6/mykit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-12 16:51:25.000000 mykit-0.1.6/mykit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-06-12 16:51:25.000000 mykit-0.1.6/mykit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 16:51:25.000000 mykit-0.1.6/mykit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1255 2023-06-12 16:49:24.000000 mykit-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 16:51:26.180941 mykit-0.1.6/setup.cfg
```

### Comparing `mykit-0.1.5/LICENSE` & `mykit-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/PKG-INFO` & `mykit-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python utility library
 Author-email: Nicholas Valentinus <nvfastplease@gmail.com>
-License: MIT License
-Project-URL: repo, https://github.com/nvfp/mykit
+License: MIT
+Project-URL: homepage, https://nvfp.github.io/mykit
+Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: tracker, https://github.com/nvfp/mykit/issues
+Project-URL: repo, https://github.com/nvfp/mykit
+Project-URL: changelog, https://nvfp.github.io/mykit/changelog
 Keywords: python,toolkit,mykit
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mykit-0.1.5/README.md` & `mykit-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/mykit/app/arrow.py` & `mykit-0.1.6/mykit/app/arrow.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/mykit/app/button.py` & `mykit-0.1.6/mykit/app/button.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/mykit/app/label.py` & `mykit-0.1.6/mykit/app/label.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/mykit/app/slider.py` & `mykit-0.1.6/mykit/app/slider.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/mykit/kit/color.py` & `mykit-0.1.6/mykit/kit/color.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/mykit/kit/ffmpeg.py` & `mykit-0.1.6/mykit/kit/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/mykit/kit/graph/graph2d.py` & `mykit-0.1.6/mykit/kit/graph/graph2d.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/mykit/kit/keycrate/__init__.py` & `mykit-0.1.6/mykit/kit/keycrate/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/mykit/kit/math.py` & `mykit-0.1.6/mykit/kit/math.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/mykit/kit/neuralnet/dense.py` & `mykit-0.1.6/mykit/kit/neuralnet/dense.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/mykit/kit/neuralnet/genetic.py` & `mykit-0.1.6/mykit/kit/neuralnet/genetic.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/mykit/kit/noise.py` & `mykit-0.1.6/mykit/kit/noise.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/mykit/kit/path.py` & `mykit-0.1.6/mykit/kit/path.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/mykit/kit/quick_visual/plot2d.py` & `mykit-0.1.6/mykit/kit/quick_visual/plot2d.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/mykit/kit/time.py` & `mykit-0.1.6/mykit/kit/time.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/mykit/kit/utils.py` & `mykit-0.1.6/mykit/kit/utils.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/mykit.egg-info/PKG-INFO` & `mykit-0.1.6/mykit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python utility library
 Author-email: Nicholas Valentinus <nvfastplease@gmail.com>
-License: MIT License
-Project-URL: repo, https://github.com/nvfp/mykit
+License: MIT
+Project-URL: homepage, https://nvfp.github.io/mykit
+Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: tracker, https://github.com/nvfp/mykit/issues
+Project-URL: repo, https://github.com/nvfp/mykit
+Project-URL: changelog, https://nvfp.github.io/mykit/changelog
 Keywords: python,toolkit,mykit
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mykit-0.1.5/mykit.egg-info/SOURCES.txt` & `mykit-0.1.6/mykit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mykit-0.1.5/pyproject.toml` & `mykit-0.1.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mykit"
-version = "0.1.5"
+version = "0.1.6"
 description = "Python utility library"
 readme = "README.md"
 requires-python = ">=3.7"
-license = {text = "MIT License"}
+license = {text = "MIT"}
 authors = [
   	{name = "Nicholas Valentinus", email = "nvfastplease@gmail.com"},
 ]
 keywords = ["python", "toolkit", "mykit"]
 classifiers = [
 	"Topic :: Scientific/Engineering",
     "License :: OSI Approved :: MIT License",
@@ -30,13 +30,16 @@
 dependencies = [
 	"numba>=0.55.2",
 	"numpy>=1.22.4"
 ]
 
 
 [project.urls]
-repo = "https://github.com/nvfp/mykit"
+homepage = "https://nvfp.github.io/mykit"
+documentation = "https://nvfp.github.io/mykit/docs"
 tracker = "https://github.com/nvfp/mykit/issues"
+repo = "https://github.com/nvfp/mykit"
+changelog = "https://nvfp.github.io/mykit/changelog"
 
 
 [project.scripts]
-mykit123foo = "mykit.__main__:main"
+mykit = "mykit.__main__:main"
```

