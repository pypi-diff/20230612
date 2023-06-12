# Comparing `tmp/autoconf-2023.7.7.1.tar.gz` & `tmp/autoconf-2023.7.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoconf-2023.7.7.1.tar", last modified: Wed Jun  7 09:39:48 2023, max compression
+gzip compressed data, was "autoconf-2023.7.7.2.tar", last modified: Wed Jun  7 09:57:56 2023, max compression
```

## Comparing `autoconf-2023.7.7.1.tar` & `autoconf-2023.7.7.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:39:48.383722 autoconf-2023.7.7.1/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:39:48.323163 autoconf-2023.7.7.1/.github/
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:39:48.342875 autoconf-2023.7.7.1/.github/workflows/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1233 2022-12-19 16:33:00.000000 autoconf-2023.7.7.1/.github/workflows/main.yml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18883 2022-12-19 11:17:33.000000 autoconf-2023.7.7.1/CODE_OF_CONDUCT.md
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1091 2020-11-16 18:50:14.000000 autoconf-2023.7.7.1/LICENSE
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      498 2022-03-30 15:09:13.000000 autoconf-2023.7.7.1/MANIFEST.in
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      774 2023-06-07 09:39:48.383722 autoconf-2023.7.7.1/PKG-INFO
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       14 2020-11-16 18:50:14.000000 autoconf-2023.7.7.1/README.rst
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:39:48.354874 autoconf-2023.7.7.1/autoconf/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      345 2023-06-07 09:38:14.000000 autoconf-2023.7.7.1/autoconf/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1425 2023-01-10 08:25:59.000000 autoconf-2023.7.7.1/autoconf/class_path.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10747 2023-01-16 16:39:25.000000 autoconf-2023.7.7.1/autoconf/conf.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3936 2023-03-21 17:55:51.000000 autoconf-2023.7.7.1/autoconf/dictable.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6511 2023-06-05 20:27:21.000000 autoconf-2023.7.7.1/autoconf/directory_config.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       93 2021-02-08 19:43:27.000000 autoconf-2023.7.7.1/autoconf/exc.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:39:48.361874 autoconf-2023.7.7.1/autoconf/json_prior/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:01:19.000000 autoconf-2023.7.7.1/autoconf/json_prior/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6536 2022-11-29 14:08:25.000000 autoconf-2023.7.7.1/autoconf/json_prior/config.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2121 2023-01-10 08:25:59.000000 autoconf-2023.7.7.1/autoconf/json_prior/generate.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:39:48.366874 autoconf-2023.7.7.1/autoconf/mock/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-03-01 14:51:44.000000 autoconf-2023.7.7.1/autoconf/mock/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1918 2023-01-10 08:25:59.000000 autoconf-2023.7.7.1/autoconf/mock/mock_real.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:39:48.371875 autoconf-2023.7.7.1/autoconf/tools/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-09-01 16:48:20.000000 autoconf-2023.7.7.1/autoconf/tools/__init__.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      582 2023-01-10 08:25:59.000000 autoconf-2023.7.7.1/autoconf/tools/decorators.py
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:39:48.381413 autoconf-2023.7.7.1/autoconf.egg-info/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      557 2023-06-07 09:39:47.000000 autoconf-2023.7.7.1/autoconf.egg-info/SOURCES.txt
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2022-02-07 19:21:33.000000 autoconf-2023.7.7.1/eden.yaml
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       51 2022-12-19 11:26:44.000000 autoconf-2023.7.7.1/requirements.txt
-drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:39:48.380413 autoconf-2023.7.7.1/scripts/
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      758 2022-11-29 18:29:27.000000 autoconf-2023.7.7.1/scripts/convert_config.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1108 2022-12-02 15:56:28.000000 autoconf-2023.7.7.1/scripts/convert_prior_configs.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      518 2023-01-10 08:25:59.000000 autoconf-2023.7.7.1/scripts/edenise.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)      334 2020-11-16 18:50:14.000000 autoconf-2023.7.7.1/scripts/generate_priors.py
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)       63 2023-06-07 09:39:48.384722 autoconf-2023.7.7.1/setup.cfg
--rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1486 2023-06-07 09:39:16.000000 autoconf-2023.7.7.1/setup.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:57:56.823350 autoconf-2023.7.7.2/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:57:56.771529 autoconf-2023.7.7.2/.github/
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:57:56.788354 autoconf-2023.7.7.2/.github/workflows/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1233 2022-12-19 16:33:00.000000 autoconf-2023.7.7.2/.github/workflows/main.yml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    18883 2022-12-19 11:17:33.000000 autoconf-2023.7.7.2/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1091 2020-11-16 18:50:14.000000 autoconf-2023.7.7.2/LICENSE
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      498 2022-03-30 15:09:13.000000 autoconf-2023.7.7.2/MANIFEST.in
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      774 2023-06-07 09:57:56.823350 autoconf-2023.7.7.2/PKG-INFO
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       14 2020-11-16 18:50:14.000000 autoconf-2023.7.7.2/README.rst
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:57:56.798379 autoconf-2023.7.7.2/autoconf/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      345 2023-06-07 09:57:30.000000 autoconf-2023.7.7.2/autoconf/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1425 2023-01-10 08:25:59.000000 autoconf-2023.7.7.2/autoconf/class_path.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)    10747 2023-01-16 16:39:25.000000 autoconf-2023.7.7.2/autoconf/conf.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     3936 2023-03-21 17:55:51.000000 autoconf-2023.7.7.2/autoconf/dictable.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6511 2023-06-05 20:27:21.000000 autoconf-2023.7.7.2/autoconf/directory_config.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       93 2021-02-08 19:43:27.000000 autoconf-2023.7.7.2/autoconf/exc.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:57:56.804389 autoconf-2023.7.7.2/autoconf/json_prior/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2020-11-10 18:01:19.000000 autoconf-2023.7.7.2/autoconf/json_prior/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     6536 2022-11-29 14:08:25.000000 autoconf-2023.7.7.2/autoconf/json_prior/config.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     2121 2023-01-10 08:25:59.000000 autoconf-2023.7.7.2/autoconf/json_prior/generate.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:57:56.808352 autoconf-2023.7.7.2/autoconf/mock/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-03-01 14:51:44.000000 autoconf-2023.7.7.2/autoconf/mock/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1918 2023-01-10 08:25:59.000000 autoconf-2023.7.7.2/autoconf/mock/mock_real.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:57:56.813350 autoconf-2023.7.7.2/autoconf/tools/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2021-09-01 16:48:20.000000 autoconf-2023.7.7.2/autoconf/tools/__init__.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      582 2023-01-10 08:25:59.000000 autoconf-2023.7.7.2/autoconf/tools/decorators.py
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:57:56.822385 autoconf-2023.7.7.2/autoconf.egg-info/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      557 2023-06-07 09:57:56.000000 autoconf-2023.7.7.2/autoconf.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       38 2022-02-07 19:21:33.000000 autoconf-2023.7.7.2/eden.yaml
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       51 2022-12-19 11:26:44.000000 autoconf-2023.7.7.2/requirements.txt
+drwxrwxrwx   0 jammy     (1000) jammy     (1000)        0 2023-06-07 09:57:56.820350 autoconf-2023.7.7.2/scripts/
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      758 2022-11-29 18:29:27.000000 autoconf-2023.7.7.2/scripts/convert_config.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1108 2022-12-02 15:56:28.000000 autoconf-2023.7.7.2/scripts/convert_prior_configs.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      518 2023-01-10 08:25:59.000000 autoconf-2023.7.7.2/scripts/edenise.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)      334 2020-11-16 18:50:14.000000 autoconf-2023.7.7.2/scripts/generate_priors.py
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)       63 2023-06-07 09:57:56.824350 autoconf-2023.7.7.2/setup.cfg
+-rwxrwxrwx   0 jammy     (1000) jammy     (1000)     1486 2023-06-07 09:57:48.000000 autoconf-2023.7.7.2/setup.py
```

### Comparing `autoconf-2023.7.7.1/.github/workflows/main.yml` & `autoconf-2023.7.7.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `autoconf-2023.7.7.1/CODE_OF_CONDUCT.md` & `autoconf-2023.7.7.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `autoconf-2023.7.7.1/LICENSE` & `autoconf-2023.7.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autoconf-2023.7.7.1/PKG-INFO` & `autoconf-2023.7.7.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoconf
-Version: 2023.7.7.1
+Version: 2023.7.7.2
 Summary: PyAuto Configration
 Home-page: https://github.com/rhayes777/PyAutoConf
 Author: James Nightingale and Richard Hayes
 Author-email: richard@rghsoftware.co.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
```

### Comparing `autoconf-2023.7.7.1/autoconf/class_path.py` & `autoconf-2023.7.7.2/autoconf/class_path.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.7.7.1/autoconf/conf.py` & `autoconf-2023.7.7.2/autoconf/conf.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.7.7.1/autoconf/dictable.py` & `autoconf-2023.7.7.2/autoconf/dictable.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.7.7.1/autoconf/directory_config.py` & `autoconf-2023.7.7.2/autoconf/directory_config.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.7.7.1/autoconf/json_prior/config.py` & `autoconf-2023.7.7.2/autoconf/json_prior/config.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.7.7.1/autoconf/json_prior/generate.py` & `autoconf-2023.7.7.2/autoconf/json_prior/generate.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.7.7.1/autoconf/mock/mock_real.py` & `autoconf-2023.7.7.2/autoconf/mock/mock_real.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.7.7.1/autoconf/tools/decorators.py` & `autoconf-2023.7.7.2/autoconf/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.7.7.1/autoconf.egg-info/SOURCES.txt` & `autoconf-2023.7.7.2/autoconf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoconf-2023.7.7.1/scripts/convert_config.py` & `autoconf-2023.7.7.2/scripts/convert_config.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.7.7.1/scripts/convert_prior_configs.py` & `autoconf-2023.7.7.2/scripts/convert_prior_configs.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.7.7.1/scripts/edenise.py` & `autoconf-2023.7.7.2/scripts/edenise.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.7.7.1/setup.py` & `autoconf-2023.7.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = file.read()
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
 setup(
     name="autoconf",
-    version=environ.get("VERSION", "2023.7.7.1"),
+    version=environ.get("VERSION", "2023.7.7.2"),
     description="PyAuto Configration",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/rhayes777/PyAutoConf",
     author="James Nightingale and Richard Hayes",
     author_email="richard@rghsoftware.co.uk",
     include_package_data=True,
```

