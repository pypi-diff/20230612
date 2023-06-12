# Comparing `tmp/agency-0.1.1.tar.gz` & `tmp/agency-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agency-0.1.1.tar", last modified: Fri Oct 29 14:53:50 2021, max compression
+gzip compressed data, was "agency-0.1.2.tar", last modified: Fri Oct 29 15:19:34 2021, max compression
```

## Comparing `agency-0.1.1.tar` & `agency-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2021-04-14 06:59:31.651589 agency-0.1.1/LICENSE
--rw-r--r--   0        0        0      139 2021-10-29 09:13:56.407047 agency-0.1.1/agency/__init__.py
--rw-r--r--   0        0        0       98 2021-10-29 09:03:38.952576 agency-0.1.1/agency/enums.py
--rw-r--r--   0        0        0      742 2021-10-29 09:04:45.696843 agency-0.1.1/agency/models.py
--rw-r--r--   0        0        0     1651 2021-10-29 09:26:03.009955 agency-0.1.1/agency/parser.py
--rw-r--r--   0        0        0      338 2021-10-29 14:53:39.616622 agency-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      657 2021-10-29 14:53:50.129482 agency-0.1.1/setup.py
--rw-r--r--   0        0        0      421 2021-10-29 14:53:50.129883 agency-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2021-04-14 06:59:31.651589 agency-0.1.2/LICENSE
+-rw-r--r--   0        0        0      139 2021-10-29 09:13:56.407047 agency-0.1.2/agency/__init__.py
+-rw-r--r--   0        0        0       98 2021-10-29 09:03:38.952576 agency-0.1.2/agency/enums.py
+-rw-r--r--   0        0        0      742 2021-10-29 09:04:45.696843 agency-0.1.2/agency/models.py
+-rw-r--r--   0        0        0     1651 2021-10-29 09:26:03.009955 agency-0.1.2/agency/parser.py
+-rw-r--r--   0        0        0      338 2021-10-29 15:19:31.694833 agency-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      657 2021-10-29 15:19:34.801976 agency-0.1.2/setup.py
+-rw-r--r--   0        0        0      421 2021-10-29 15:19:34.802168 agency-0.1.2/PKG-INFO
```

### Comparing `agency-0.1.1/LICENSE` & `agency-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agency-0.1.1/agency/models.py` & `agency-0.1.2/agency/models.py`

 * *Files identical despite different names*

### Comparing `agency-0.1.1/agency/parser.py` & `agency-0.1.2/agency/parser.py`

 * *Files identical despite different names*

### Comparing `agency-0.1.1/setup.py` & `agency-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['enumb>=0.1.2,<0.2.0', 'parse>=1.19.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'agency',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'User Agent parsing and creation',
     'long_description': None,
     'author': 'Tom Bulled',
     'author_email': '26026015+tombulled@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

