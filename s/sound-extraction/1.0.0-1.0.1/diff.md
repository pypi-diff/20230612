# Comparing `tmp/sound-extraction-1.0.0.tar.gz` & `tmp/sound-extraction-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sound-extraction-1.0.0.tar", last modified: Fri Jun  9 18:09:36 2023, max compression
+gzip compressed data, was "dist\sound-extraction-1.0.1.tar", last modified: Mon Jun 12 18:18:52 2023, max compression
```

## Comparing `sound-extraction-1.0.0.tar` & `sound-extraction-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 18:09:36.876803 sound-extraction-1.0.0/
--rw-rw-rw-   0        0        0      683 2023-06-09 18:09:36.875701 sound-extraction-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4889 2023-06-06 18:56:03.000000 sound-extraction-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 18:09:36.877687 sound-extraction-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1078 2023-06-09 18:04:53.000000 sound-extraction-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 18:09:36.872709 sound-extraction-1.0.0/sound_extraction.egg-info/
--rw-rw-rw-   0        0        0      683 2023-06-09 18:09:36.000000 sound-extraction-1.0.0/sound_extraction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-06-09 18:09:36.000000 sound-extraction-1.0.0/sound_extraction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 18:09:36.000000 sound-extraction-1.0.0/sound_extraction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      153 2023-06-09 18:09:36.000000 sound-extraction-1.0.0/sound_extraction.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 18:09:36.000000 sound-extraction-1.0.0/sound_extraction.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 18:18:52.978063 sound-extraction-1.0.1/
+-rw-rw-rw-   0        0        0     1087 2023-06-12 17:14:00.000000 sound-extraction-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      964 2023-06-12 18:18:52.977094 sound-extraction-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4889 2023-06-06 18:56:03.000000 sound-extraction-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 18:18:52.978063 sound-extraction-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1524 2023-06-12 18:17:23.000000 sound-extraction-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:18:52.949159 sound-extraction-1.0.1/sound-extraction/
+drwxrwxrwx   0        0        0        0 2023-06-12 18:18:52.975071 sound-extraction-1.0.1/sound-extraction/sound_extraction.egg-info/
+-rw-rw-rw-   0        0        0      964 2023-06-12 18:18:52.000000 sound-extraction-1.0.1/sound-extraction/sound_extraction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-12 18:18:52.000000 sound-extraction-1.0.1/sound-extraction/sound_extraction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 18:18:52.000000 sound-extraction-1.0.1/sound-extraction/sound_extraction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-12 18:18:52.000000 sound-extraction-1.0.1/sound-extraction/sound_extraction.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      153 2023-06-12 18:18:52.000000 sound-extraction-1.0.1/sound-extraction/sound_extraction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 18:18:52.000000 sound-extraction-1.0.1/sound-extraction/sound_extraction.egg-info/top_level.txt
```

### Comparing `sound-extraction-1.0.0/README.md` & `sound-extraction-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sound-extraction-1.0.0/setup.py` & `sound-extraction-1.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,36 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sound-extraction',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
     install_requires=[
         'certifi==2023.5.7',
         'cffi==1.15.1',
         'load-dotenv==0.1.0',
         'numpy==1.24.3',
         'pycparser==2.21',
         'python-dotenv==1.0.0',
         'sentry-sdk==1.25.1',
         'soundfile==0.12.1',
         'urllib3==2.0.3',
     ],
+    entry_points={
+        'console_scripts': [
+            'sound-extraction = sound_extraction:main',
+        ],
+    },
+    classifiers=[
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    package_dir={'': 'sound-extraction'},
     description="Slice and segment your audio files easily with open source Python program. Our tool enables you to perform analytical workflows by creating segments based on recording start time and desired duration. Share and manipulate the recordings at ease.Slice and segment your audio files easily with open source Python program. Our tool enables you to perform analytical workflows by creating segments based on recording start time and desired duration. Share and manipulate the recordings at ease.",
     author="Prayag Shah",
     author_email="prayagshah07@gmail.com",
     url="https://github.com/prayagnshah/Sound-Extraction",
 
 )
```

