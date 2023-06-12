# Comparing `tmp/thumbtack_client-0.3.0.tar.gz` & `tmp/thumbtack_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/thumbtack_client-0.3.0.tar", last modified: Fri Dec  4 14:27:58 2020, max compression
+gzip compressed data, was "thumbtack_client-0.4.0.tar", last modified: Mon Jun 12 19:16:33 2023, max compression
```

## Comparing `thumbtack_client-0.3.0.tar` & `thumbtack_client-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-04 14:27:58.000000 thumbtack_client-0.3.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11368 2020-12-04 14:27:18.000000 thumbtack_client-0.3.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      164 2020-12-04 14:27:18.000000 thumbtack_client-0.3.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1946 2020-12-04 14:27:58.000000 thumbtack_client-0.3.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      730 2020-12-04 14:27:18.000000 thumbtack_client-0.3.0/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2020-12-04 14:27:18.000000 thumbtack_client-0.3.0/dev-requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-04 14:27:58.000000 thumbtack_client-0.3.0/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      613 2020-12-04 14:27:18.000000 thumbtack_client-0.3.0/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)      686 2020-12-04 14:27:18.000000 thumbtack_client-0.3.0/docs/api.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1386 2020-12-04 14:27:18.000000 thumbtack_client-0.3.0/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      265 2020-12-04 14:27:18.000000 thumbtack_client-0.3.0/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      174 2020-12-04 14:27:18.000000 thumbtack_client-0.3.0/docs/thumbtack-client.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      118 2020-12-04 14:27:18.000000 thumbtack_client-0.3.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      253 2020-12-04 14:27:58.000000 thumbtack_client-0.3.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2146 2020-12-04 14:27:18.000000 thumbtack_client-0.3.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-04 14:27:58.000000 thumbtack_client-0.3.0/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-04 14:27:58.000000 thumbtack_client-0.3.0/src/thumbtack_client/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1574 2020-12-04 14:27:18.000000 thumbtack_client-0.3.0/src/thumbtack_client/MountedDiskImage.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5671 2020-12-04 14:27:18.000000 thumbtack_client-0.3.0/src/thumbtack_client/MountedDiskImageVolume.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       52 2020-12-04 14:27:18.000000 thumbtack_client-0.3.0/src/thumbtack_client/ThumbtackClientException.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4838 2020-12-04 14:27:18.000000 thumbtack_client-0.3.0/src/thumbtack_client/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-04 14:27:58.000000 thumbtack_client-0.3.0/src/thumbtack_client.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1946 2020-12-04 14:27:58.000000 thumbtack_client-0.3.0/src/thumbtack_client.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      586 2020-12-04 14:27:58.000000 thumbtack_client-0.3.0/src/thumbtack_client.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-12-04 14:27:58.000000 thumbtack_client-0.3.0/src/thumbtack_client.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      151 2020-12-04 14:27:58.000000 thumbtack_client-0.3.0/src/thumbtack_client.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       17 2020-12-04 14:27:58.000000 thumbtack_client-0.3.0/src/thumbtack_client.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-04 14:27:58.000000 thumbtack_client-0.3.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      685 2020-12-04 14:27:18.000000 thumbtack_client-0.3.0/tests/test_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      294 2020-12-04 14:27:18.000000 thumbtack_client-0.3.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 19:16:33.021521 thumbtack_client-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)    11368 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      164 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-06-12 19:16:33.021521 thumbtack_client-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      730 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/dev-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 19:16:33.017521 thumbtack_client-0.4.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      613 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/docs/api.rst
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      265 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/docs/thumbtack-client.rst
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      253 2023-06-12 19:16:33.021521 thumbtack_client-0.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 19:16:33.017521 thumbtack_client-0.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 19:16:33.021521 thumbtack_client-0.4.0/src/thumbtack_client/
+-rw-r--r--   0 root         (0) root         (0)       58 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/src/thumbtack_client/DuplicateMountAttemptException.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/src/thumbtack_client/MountedDiskImage.py
+-rw-r--r--   0 root         (0) root         (0)     5670 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/src/thumbtack_client/MountedDiskImageVolume.py
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/src/thumbtack_client/ThumbtackClientException.py
+-rw-r--r--   0 root         (0) root         (0)     8498 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/src/thumbtack_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 19:16:33.021521 thumbtack_client-0.4.0/src/thumbtack_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-06-12 19:16:32.000000 thumbtack_client-0.4.0/src/thumbtack_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      641 2023-06-12 19:16:33.000000 thumbtack_client-0.4.0/src/thumbtack_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 19:16:32.000000 thumbtack_client-0.4.0/src/thumbtack_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-12 19:16:32.000000 thumbtack_client-0.4.0/src/thumbtack_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-12 19:16:32.000000 thumbtack_client-0.4.0/src/thumbtack_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 19:16:33.021521 thumbtack_client-0.4.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)      294 2023-06-12 19:16:29.000000 thumbtack_client-0.4.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `thumbtack_client-0.3.0/LICENSE` & `thumbtack_client-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thumbtack_client-0.3.0/PKG-INFO` & `thumbtack_client-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thumbtack_client
-Version: 0.3.0
+Version: 0.4.0
 Summary: Connect to a Thumbtack Server.
 Home-page: https://github.com/mitre/thumbtack-client
 Author: The MITRE Corporation
 Author-email: thumbtack@mitre.org
 License: Apache 2.0
 Description: 
         .. image:: https://travis-ci.org/mitre/thumbtack-client.svg?branch=master
```

### Comparing `thumbtack_client-0.3.0/README.rst` & `thumbtack_client-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `thumbtack_client-0.3.0/docs/Makefile` & `thumbtack_client-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `thumbtack_client-0.3.0/docs/api.rst` & `thumbtack_client-0.4.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `thumbtack_client-0.3.0/docs/conf.py` & `thumbtack_client-0.4.0/docs/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,74 @@
 # -*- coding: utf-8 -*-
 
-project = 'thumbtack-client'
-copyright = '2019, The MITRE Corporation'
-author = 'The MITRE Corporation'
+project = "thumbtack-client"
+copyright = "2019, The MITRE Corporation"
+author = "The MITRE Corporation"
 
-version = '0.3.0'
-release = '0.3.0'
+version = "0.4.0"
+release = "0.4.0"
 
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.napoleon',
-    'sphinx.ext.viewcode',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.viewcode",
 ]
 
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
-source_suffix = '.rst'
+source_suffix = ".rst"
 
-master_doc = 'index'
+master_doc = "index"
 
 language = None
 
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 
-html_theme = 'sphinx_rtd_theme'
+html_theme = "sphinx_rtd_theme"
 html_theme_options = {
     # 'canonical_url': '',
     # 'analytics_id': '',
     # 'logo_only': False,
-    'display_version': True,
-    'prev_next_buttons_location': 'bottom',
+    "display_version": True,
+    "prev_next_buttons_location": "bottom",
     # 'style_external_links': False,
     # 'vcs_pageview_mode': '',
     # Toc options
-    'collapse_navigation': False,
-    'sticky_navigation': True,
-    'navigation_depth': 2,
+    "collapse_navigation": False,
+    "sticky_navigation": True,
+    "navigation_depth": 2,
     # 'includehidden': True,
     # 'titles_only': False
 }
 
-htmlhelp_basename = 'thumbtack-clientdoc'
+htmlhelp_basename = "thumbtack-clientdoc"
 
 latex_elements = {}
 
 latex_documents = [
-    (master_doc, 'thumbtack-client.tex', 'thumbtack-client Documentation',
-     'The MITRE Corporation', 'manual'),
+    (
+        master_doc,
+        "thumbtack-client.tex",
+        "thumbtack-client Documentation",
+        "The MITRE Corporation",
+        "manual",
+    ),
 ]
 
 man_pages = [
-    (master_doc, 'thumbtack-client', 'thumbtack-client Documentation',
-     [author], 1)
+    (master_doc, "thumbtack-client", "thumbtack-client Documentation", [author], 1)
 ]
 
 texinfo_documents = [
-    (master_doc, 'thumbtack-client', 'thumbtack-client Documentation',
-     author, 'thumbtack-client', 'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "thumbtack-client",
+        "thumbtack-client Documentation",
+        author,
+        "thumbtack-client",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
```

### Comparing `thumbtack_client-0.3.0/setup.py` & `thumbtack_client-0.4.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,87 @@
 import io
 import os
 
 from setuptools import setup, find_packages
 
 # Package meta-data.
-NAME = 'thumbtack_client'
-DESCRIPTION = 'Connect to a Thumbtack Server.'
-URL = 'https://github.com/mitre/thumbtack-client'
-EMAIL = 'thumbtack@mitre.org'
-AUTHOR = 'The MITRE Corporation'
-LICENSE = 'Apache 2.0'
-REQUIRES_PYTHON = '>=2.7.0'
-VERSION = '0.3.0'
+NAME = "thumbtack_client"
+DESCRIPTION = "Connect to a Thumbtack Server."
+URL = "https://github.com/mitre/thumbtack-client"
+EMAIL = "thumbtack@mitre.org"
+AUTHOR = "The MITRE Corporation"
+LICENSE = "Apache 2.0"
+REQUIRES_PYTHON = ">=2.7.0"
+VERSION = "0.4.0"
 
-REQUIRED = [
-    'requests'
-]
+REQUIRED = ["requests"]
 
 doc_requires = [
-    'sphinx',
+    "sphinx",
 ]
 
 test_requires = [
-    'coverage',
-    'pytest',
-    'pytest-cov',
-    'responses',
+    "coverage",
+    "pytest",
+    "pytest-cov",
+    "responses",
 ]
 
-dev_requires = doc_requires + test_requires + [
-    'bumpversion',
-    'check-manifest',
-    # test_requires are installed into every tox environment, so we don't
-    # want to include tox there.
-    'tox',
-]
+dev_requires = (
+    doc_requires
+    + test_requires
+    + [
+        "bumpversion",
+        "check-manifest",
+        # test_requires are installed into every tox environment, so we don't
+        # want to include tox there.
+        "tox",
+    ]
+)
 
 EXTRAS = {
-    'dev': dev_requires,
-    'docs': doc_requires,
-    'test': test_requires,
+    "dev": dev_requires,
+    "docs": doc_requires,
+    "test": test_requires,
 }
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 try:
-    with io.open(os.path.join(here, 'README.rst'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
+    with io.open(os.path.join(here, "README.rst"), encoding="utf-8") as f:
+        long_description = "\n" + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 setup(
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
     license=LICENSE,
     long_description=long_description,
-    long_description_content_type='text/x-rst',
+    long_description_content_type="text/x-rst",
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Developers',
-        'Topic :: Security',
-        'Topic :: System :: Filesystems',
-        'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7'
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "Topic :: Security",
+        "Topic :: System :: Filesystems",
+        "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: Python :: 2",
+        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
     ],
-    keywords='imagemounter api thumbtack',
+    keywords="imagemounter api thumbtack",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
 )
```

### Comparing `thumbtack_client-0.3.0/src/thumbtack_client/MountedDiskImage.py` & `thumbtack_client-0.4.0/src/thumbtack_client/MountedDiskImage.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,9 +27,13 @@
         mounted_disk_obj : dict
             This dictionary should be refactored into its individual components.
             It is defined in the resources.py file as `disk_fields`.
         """
         self.mountpoint = mounted_disk_obj["mountpoint"]
         self.name = mounted_disk_obj["name"]
         self.volumes = [MountedDiskImageVolume(v) for v in mounted_disk_obj["volumes"]]
+        if mounted_disk_obj["paths"] is not None and "nbd" in mounted_disk_obj["paths"].keys():
+            self.device = mounted_disk_obj["paths"]["nbd"]
+        else:
+            self.device = None
         # only volumes with a non-empty mountpoint
         self.mounted_volumes = [v for v in self.volumes if v.mountpoint]
```

### Comparing `thumbtack_client-0.3.0/src/thumbtack_client/MountedDiskImageVolume.py` & `thumbtack_client-0.4.0/src/thumbtack_client/MountedDiskImageVolume.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     def walk(self, file_filter=None):
         """Walks through every file in a given mountpoint directory.
 
         Parameters
         ----------
         file_filter : callable, optional
             A callable that accepts `mounted_file_path_on_disk` and returns a boolean
-            of whether to yield that file.  For example, you can call
+            of whether to yield that file. For example, you can call
             `volume.walk(lambda x: x.endswith(".exe"))` to find all of the files
             with the `.exe` extension.
 
         Yields
         ------
         tuple (str, str)
             A tuple that contains (absolute path, path in volume)
@@ -76,16 +76,16 @@
         ...     print(file_path_within_volume)
         """
         for dirpath, _, filenames in os.walk(self.mountpoint):
             for f in filenames:
                 full_path = os.path.join(dirpath, f)
                 if file_filter is None or file_filter(full_path):
                     # remove mounted prefix; eg '/tmp/thumbtack/im_x30_s3s'
-                    path_within_volume = os.path.join(*full_path.split(os.path.sep)[4:])
-                    yield (full_path, path_within_volume)
+                    path_within_volume = os.path.relpath(full_path, start=self.mountpoint)
+                    yield full_path, path_within_volume
 
     def safe_walk(self, file_filter=None):
         """Walks through every file in a given mountpoint directory, skipping broken files.
 
         This is the preferred method over :meth:`~thumbtack.resources.MountedDiskImageVolume.walk()`
         since there are more checks to ensure that files are accessible. It skips broken
         symlinks, files that can't be read, and named pipes.
```

### Comparing `thumbtack_client-0.3.0/src/thumbtack_client.egg-info/PKG-INFO` & `thumbtack_client-0.4.0/src/thumbtack_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thumbtack-client
-Version: 0.3.0
+Version: 0.4.0
 Summary: Connect to a Thumbtack Server.
 Home-page: https://github.com/mitre/thumbtack-client
 Author: The MITRE Corporation
 Author-email: thumbtack@mitre.org
 License: Apache 2.0
 Description: 
         .. image:: https://travis-ci.org/mitre/thumbtack-client.svg?branch=master
```

### Comparing `thumbtack_client-0.3.0/src/thumbtack_client.egg-info/SOURCES.txt` & `thumbtack_client-0.4.0/src/thumbtack_client.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 setup.py
 tox.ini
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/index.rst
 docs/thumbtack-client.rst
+src/thumbtack_client/DuplicateMountAttemptException.py
 src/thumbtack_client/MountedDiskImage.py
 src/thumbtack_client/MountedDiskImageVolume.py
 src/thumbtack_client/ThumbtackClientException.py
 src/thumbtack_client/__init__.py
 src/thumbtack_client.egg-info/PKG-INFO
 src/thumbtack_client.egg-info/SOURCES.txt
 src/thumbtack_client.egg-info/dependency_links.txt
```

### Comparing `thumbtack_client-0.3.0/tests/test_client.py` & `thumbtack_client-0.4.0/tests/test_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,27 @@
 def client():
     return thumbtack_client.ThumbtackClient()
 
 
 def test_smoke():
     assert thumbtack_client.MountedDiskImage.MountedDiskImage is not None
 
+@responses.activate
+def test_list_images_empty(client):
+    responses.add(responses.GET, 'http://127.0.0.1:8208/images', '[]')
+
+    response = client.list_images()
+    assert response == []
+
+@responses.activate
+def test_list_images_populated(client):
+    responses.add(responses.GET, 'http://127.0.0.1:8208/images', '[1, 2, 3]')
+
+    response = client.list_images()
+    assert len(response) > 0
 
 @responses.activate
 def test_list_mounts_empty(client):
     responses.add(responses.GET, 'http://127.0.0.1:8208/mounts/', '[]')
 
     response = client.list_mounted_images()
     assert response == []
```

