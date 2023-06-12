# Comparing `tmp/american_options-0.0.1.tar.gz` & `tmp/american_options-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "american_options-0.0.1.tar", last modified: Tue May  2 21:35:43 2023, max compression
+gzip compressed data, was "dist\american_options-0.1.1.tar", last modified: Mon Jun 12 01:41:53 2023, max compression
```

## Comparing `american_options-0.0.1.tar` & `american_options-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 21:35:43.361743 american_options-0.0.1/
--rw-rw-rw-   0        0        0     1183 2023-05-02 21:35:43.360747 american_options-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      441 2023-05-02 18:22:15.000000 american_options-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 21:35:43.340799 american_options-0.0.1/american_options/
--rw-rw-rw-   0        0        0     1825 2023-05-02 17:28:27.000000 american_options-0.0.1/american_options/AMoption.py
--rw-rw-rw-   0        0        0       94 2023-05-02 17:31:37.000000 american_options-0.0.1/american_options/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:35:43.358751 american_options-0.0.1/american_options.egg-info/
--rw-rw-rw-   0        0        0     1183 2023-05-02 21:35:42.000000 american_options-0.0.1/american_options.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-05-02 21:35:43.000000 american_options-0.0.1/american_options.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 21:35:43.000000 american_options-0.0.1/american_options.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-02 21:35:43.000000 american_options-0.0.1/american_options.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 21:35:43.000000 american_options-0.0.1/american_options.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 21:35:43.361743 american_options-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1306 2023-05-02 21:27:58.000000 american_options-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 01:41:53.000000 american_options-0.1.1/
+-rw-rw-rw-   0        0        0     2510 2023-06-12 01:41:53.000000 american_options-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1777 2023-06-12 01:21:26.000000 american_options-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 01:41:53.000000 american_options-0.1.1/american_options/
+-rw-rw-rw-   0        0        0    34917 2023-06-12 00:23:55.000000 american_options-0.1.1/american_options/AMoption.py
+-rw-rw-rw-   0        0        0      191 2023-06-12 00:46:34.000000 american_options-0.1.1/american_options/__init__.py
+-rw-rw-rw-   0        0        0     4524 2023-06-11 22:01:15.000000 american_options-0.1.1/american_options/jump_diffusion.py
+-rw-rw-rw-   0        0        0     4198 2023-06-11 22:50:46.000000 american_options-0.1.1/american_options/payoffs.py
+-rw-rw-rw-   0        0        0     2333 2023-06-10 14:04:25.000000 american_options-0.1.1/american_options/próby.py
+-rw-rw-rw-   0        0        0     2638 2023-06-11 17:41:22.000000 american_options-0.1.1/american_options/sobol.py
+-rw-rw-rw-   0        0        0    10287 2023-06-11 22:52:35.000000 american_options-0.1.1/american_options/underlying.py
+drwxrwxrwx   0        0        0        0 2023-06-12 01:41:53.000000 american_options-0.1.1/american_options.egg-info/
+-rw-rw-rw-   0        0        0     2510 2023-06-12 01:41:53.000000 american_options-0.1.1/american_options.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-06-12 01:41:53.000000 american_options-0.1.1/american_options.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 01:41:53.000000 american_options-0.1.1/american_options.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-12 01:41:53.000000 american_options-0.1.1/american_options.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-12 01:41:53.000000 american_options-0.1.1/american_options.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 01:41:53.000000 american_options-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1425 2023-06-12 01:41:05.000000 american_options-0.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `american_options-0.0.1/setup.py` & `american_options-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,30 +9,34 @@
 # Get the long description on pypi from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="american_options",
-    version="0.0.1",
-    description="Demo library",
+    version="0.1.1",
+    description="library T-28h",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://american_options.readthedocs.io/",
     author="Przemysław Adamski, Katarzyna Hasal, Kacper Toczek",
     author_email="kat.hasal99@gmail.com",
     classifiers=[
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
     packages=["american_options"],
     include_package_data=True,
     install_requires=["numpy",
-                      "scipy"]
+                      "scipy",
+                      "chaospy",
+                      "pandas",
+                      "matplotlib",
+                      "sklearn",
+                      "tqdm"]
 )
```

