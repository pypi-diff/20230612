# Comparing `tmp/dockery-0.2.1.tar.gz` & `tmp/dockery-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockery-0.2.1.tar", last modified: Mon Jun 12 01:54:27 2023, max compression
+gzip compressed data, was "dockery-0.2.2.tar", last modified: Mon Jun 12 04:24:25 2023, max compression
```

## Comparing `dockery-0.2.1.tar` & `dockery-0.2.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1082 2023-06-12 01:54:18.163398 dockery-0.2.1/LICENSE
--rw-r--r--   0        0        0      551 2023-06-12 01:54:18.163398 dockery-0.2.1/README.md
--rw-r--r--   0        0        0      614 2023-06-12 01:54:27.251532 dockery-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 dockery-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-12 04:24:12.098149 dockery-0.2.2/LICENSE
+-rw-r--r--   0        0        0      665 2023-06-12 04:24:12.098149 dockery-0.2.2/README.md
+-rw-r--r--   0        0        0      614 2023-06-12 04:24:25.790712 dockery-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      998 1970-01-01 00:00:00.000000 dockery-0.2.2/PKG-INFO
```

### Comparing `dockery-0.2.1/LICENSE` & `dockery-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dockery-0.2.1/pyproject.toml` & `dockery-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dockery"
-version = "0.2.1"
+version = "0.2.2"
 description = "Graphical interface for Docker in your console"
 authors = [
     { name = "Mariano Carrazana", email = "marianocarrazana@gmail.com" },
 ]
 dependencies = [
     "docker>=6.1.3",
     "textual>=0.27.0",
```

### Comparing `dockery-0.2.1/PKG-INFO` & `dockery-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,56 @@
 Metadata-Version: 2.1
 Name: dockery
-Version: 0.2.1
+Version: 0.2.2
 Summary: Graphical interface for Docker in your console
 Author-Email: Mariano Carrazana <marianocarrazana@gmail.com>
 License: MIT
 Requires-Python: >=3.9
 Requires-Dist: docker>=6.1.3
 Requires-Dist: textual>=0.27.0
 Requires-Dist: click>=8.1.3
 Description-Content-Type: text/markdown
 
 # dockery
 
 Graphical interface for Docker in your console
 
-![capture1](https://github.com/marianocarrazana/dockery/assets/17238076/a97f7854-2961-4cab-8596-0f3e3d48224c)
-
-![capture2](https://github.com/marianocarrazana/dockery/assets/17238076/c656e616-387b-456d-a921-0d836ebaabc4)
+| ![capture1](https://github.com/marianocarrazana/dockery/assets/17238076/a97f7854-2961-4cab-8596-0f3e3d48224c) | ![capture2](https://github.com/marianocarrazana/dockery/assets/17238076/c656e616-387b-456d-a921-0d836ebaabc4) |
+|-|-|
 
 ## Installation
 
 ### From source
 
-```bash
+```shell
 git clone git@github.com:marianocarrazana/dockery.git
 cd dockery
 pip install -e .
 # update only:
 git pull
 ```
 
 ### From pip
 
-```bash
+```shell
 pip install dockery
 ```
 
 ## Usage
 
 Run on your console:
 
-```bash
+```shell
 dockery
 ```
 
+## Extra commands
+
+```shell
+dockery df
+dockery ps
+dockery volumes
+dockery images
+dockery stats
+```
+
 ## **Enjoy it!**
```

