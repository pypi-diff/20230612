# Comparing `tmp/genWizard-0.0.1.tar.gz` & `tmp/genWizard-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genWizard-0.0.1.tar", last modified: Mon Jun 12 19:46:23 2023, max compression
+gzip compressed data, was "genWizard-0.0.2.tar", last modified: Mon Jun 12 20:07:36 2023, max compression
```

## Comparing `genWizard-0.0.1.tar` & `genWizard-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yvonkim    (501) staff       (20)        0 2023-06-12 19:46:23.889182 genWizard-0.0.1/
--rw-r--r--   0 yvonkim    (501) staff       (20)       66 2023-06-04 08:46:43.000000 genWizard-0.0.1/.gitattributes
--rw-r--r--   0 yvonkim    (501) staff       (20)      155 2023-06-12 09:36:43.000000 genWizard-0.0.1/CHANGELOG.txt
--rw-r--r--   0 yvonkim    (501) staff       (20)     1065 2023-06-12 09:38:56.000000 genWizard-0.0.1/LICENSE.txt
--rw-r--r--   0 yvonkim    (501) staff       (20)       49 2023-06-12 19:01:04.000000 genWizard-0.0.1/MANIFEST.in
--rw-r--r--   0 yvonkim    (501) staff       (20)      741 2023-06-12 19:46:23.887914 genWizard-0.0.1/PKG-INFO
--rw-r--r--   0 yvonkim    (501) staff       (20)       86 2023-06-12 09:38:56.000000 genWizard-0.0.1/README.txt
-drwxr-xr-x   0 yvonkim    (501) staff       (20)        0 2023-06-12 19:46:23.782957 genWizard-0.0.1/genWizard.egg-info/
--rw-r--r--   0 yvonkim    (501) staff       (20)      741 2023-06-12 19:46:23.000000 genWizard-0.0.1/genWizard.egg-info/PKG-INFO
--rw-r--r--   0 yvonkim    (501) staff       (20)      325 2023-06-12 19:46:23.000000 genWizard-0.0.1/genWizard.egg-info/SOURCES.txt
--rw-r--r--   0 yvonkim    (501) staff       (20)        1 2023-06-12 19:46:23.000000 genWizard-0.0.1/genWizard.egg-info/dependency_links.txt
--rw-r--r--   0 yvonkim    (501) staff       (20)        7 2023-06-12 19:46:23.000000 genWizard-0.0.1/genWizard.egg-info/requires.txt
--rw-r--r--   0 yvonkim    (501) staff       (20)        8 2023-06-12 19:46:23.000000 genWizard-0.0.1/genWizard.egg-info/top_level.txt
-drwxr-xr-x   0 yvonkim    (501) staff       (20)        0 2023-06-12 19:46:23.879974 genWizard-0.0.1/modules/
--rw-r--r--   0 yvonkim    (501) staff       (20)        0 2023-06-12 19:33:40.000000 genWizard-0.0.1/modules/__init__.py
--rw-r--r--   0 yvonkim    (501) staff       (20)     2039 2023-06-12 08:57:22.000000 genWizard-0.0.1/modules/database_manager.py
--rw-r--r--   0 yvonkim    (501) staff       (20)      649 2023-06-12 09:38:56.000000 genWizard-0.0.1/modules/expander.py
--rw-r--r--   0 yvonkim    (501) staff       (20)     1236 2023-06-12 18:48:46.000000 genWizard-0.0.1/modules/generator.py
--rw-r--r--   0 yvonkim    (501) staff       (20)       38 2023-06-12 19:46:23.889607 genWizard-0.0.1/setup.cfg
--rw-r--r--   0 yvonkim    (501) staff       (20)      727 2023-06-12 19:46:20.000000 genWizard-0.0.1/setup.py
+drwxr-xr-x   0 yvonkim    (501) staff       (20)        0 2023-06-12 20:07:36.361067 genWizard-0.0.2/
+-rw-r--r--   0 yvonkim    (501) staff       (20)       66 2023-06-04 08:46:43.000000 genWizard-0.0.2/.gitattributes
+-rw-r--r--   0 yvonkim    (501) staff       (20)      155 2023-06-12 09:36:43.000000 genWizard-0.0.2/CHANGELOG.txt
+-rw-r--r--   0 yvonkim    (501) staff       (20)     1065 2023-06-12 09:38:56.000000 genWizard-0.0.2/LICENSE.txt
+-rw-r--r--   0 yvonkim    (501) staff       (20)       49 2023-06-12 19:01:04.000000 genWizard-0.0.2/MANIFEST.in
+-rw-r--r--   0 yvonkim    (501) staff       (20)     5567 2023-06-12 20:07:36.360504 genWizard-0.0.2/PKG-INFO
+-rw-r--r--   0 yvonkim    (501) staff       (20)     4912 2023-06-12 20:00:41.000000 genWizard-0.0.2/README.txt
+drwxr-xr-x   0 yvonkim    (501) staff       (20)        0 2023-06-12 20:07:36.354697 genWizard-0.0.2/genWizard.egg-info/
+-rw-r--r--   0 yvonkim    (501) staff       (20)     5567 2023-06-12 20:07:36.000000 genWizard-0.0.2/genWizard.egg-info/PKG-INFO
+-rw-r--r--   0 yvonkim    (501) staff       (20)      325 2023-06-12 20:07:36.000000 genWizard-0.0.2/genWizard.egg-info/SOURCES.txt
+-rw-r--r--   0 yvonkim    (501) staff       (20)        1 2023-06-12 20:07:36.000000 genWizard-0.0.2/genWizard.egg-info/dependency_links.txt
+-rw-r--r--   0 yvonkim    (501) staff       (20)        7 2023-06-12 20:07:36.000000 genWizard-0.0.2/genWizard.egg-info/requires.txt
+-rw-r--r--   0 yvonkim    (501) staff       (20)        8 2023-06-12 20:07:36.000000 genWizard-0.0.2/genWizard.egg-info/top_level.txt
+drwxr-xr-x   0 yvonkim    (501) staff       (20)        0 2023-06-12 20:07:36.359350 genWizard-0.0.2/modules/
+-rw-r--r--   0 yvonkim    (501) staff       (20)        0 2023-06-12 19:33:40.000000 genWizard-0.0.2/modules/__init__.py
+-rw-r--r--   0 yvonkim    (501) staff       (20)     2039 2023-06-12 08:57:22.000000 genWizard-0.0.2/modules/database_manager.py
+-rw-r--r--   0 yvonkim    (501) staff       (20)      649 2023-06-12 09:38:56.000000 genWizard-0.0.2/modules/expander.py
+-rw-r--r--   0 yvonkim    (501) staff       (20)     1236 2023-06-12 18:48:46.000000 genWizard-0.0.2/modules/generator.py
+-rw-r--r--   0 yvonkim    (501) staff       (20)       38 2023-06-12 20:07:36.362184 genWizard-0.0.2/setup.cfg
+-rw-r--r--   0 yvonkim    (501) staff       (20)      727 2023-06-12 20:07:33.000000 genWizard-0.0.2/setup.py
```

### Comparing `genWizard-0.0.1/LICENSE.txt` & `genWizard-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genWizard-0.0.1/modules/database_manager.py` & `genWizard-0.0.2/modules/database_manager.py`

 * *Files identical despite different names*

### Comparing `genWizard-0.0.1/modules/expander.py` & `genWizard-0.0.2/modules/expander.py`

 * *Files identical despite different names*

### Comparing `genWizard-0.0.1/modules/generator.py` & `genWizard-0.0.2/modules/generator.py`

 * *Files identical despite different names*

### Comparing `genWizard-0.0.1/setup.py` & `genWizard-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='genWizard',
-    version='0.0.1',
+    version='0.0.2',
     description='genWizard allows for versatile usage of openAI generation and prompting management.',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='https://github.com/ykim336/genWizard',
     license='MIT',
     classifiers=classifiers,
     keywords='machine learning',
     author='Isaac Moon',
```

