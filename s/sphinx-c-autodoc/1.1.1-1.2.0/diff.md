# Comparing `tmp/sphinx-c-autodoc-1.1.1.tar.gz` & `tmp/sphinx_c_autodoc-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-c-autodoc-1.1.1.tar", last modified: Wed Dec 21 17:11:27 2022, max compression
+gzip compressed data, was "sphinx_c_autodoc-1.2.0.tar", max compression
```

## Comparing `sphinx-c-autodoc-1.1.1.tar` & `sphinx_c_autodoc-1.2.0.tar`

### file list

```diff
@@ -1,34 +1,17 @@
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2022-12-21 17:11:27.941039 sphinx-c-autodoc-1.1.1/
--rw-r--r--   0 nick      (1000) nick      (1000)     1071 2022-12-18 01:41:34.000000 sphinx-c-autodoc-1.1.1/LICENSE-MIT
--rw-r--r--   0 nick      (1000) nick      (1000)     3236 2022-12-21 17:11:27.940039 sphinx-c-autodoc-1.1.1/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)     2571 2022-12-21 17:11:05.000000 sphinx-c-autodoc-1.1.1/README.rst
--rw-r--r--   0 nick      (1000) nick      (1000)       38 2022-12-21 17:11:27.941039 sphinx-c-autodoc-1.1.1/setup.cfg
--rw-r--r--   0 nick      (1000) nick      (1000)     1383 2022-12-21 17:11:05.000000 sphinx-c-autodoc-1.1.1/setup.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2022-12-21 17:11:27.936039 sphinx-c-autodoc-1.1.1/src/
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2022-12-21 17:11:27.937039 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/
--rw-r--r--   0 nick      (1000) nick      (1000)    26901 2022-12-20 02:38:44.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/__init__.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2022-12-21 17:11:27.939039 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/apidoc/
--rw-r--r--   0 nick      (1000) nick      (1000)     7095 2022-12-18 01:41:34.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/apidoc/__init__.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2022-12-21 17:11:27.939039 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/apidoc/templates/
--rw-r--r--   0 nick      (1000) nick      (1000)       72 2022-12-18 01:41:34.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/apidoc/templates/header.rst.jinja2
--rw-r--r--   0 nick      (1000) nick      (1000)       57 2022-12-18 01:41:34.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/apidoc/templates/source.rst.jinja2
--rw-r--r--   0 nick      (1000) nick      (1000)      131 2022-12-18 01:41:34.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/apidoc/templates/toc.rst.jinja2
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2022-12-21 17:11:27.940039 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/clang/
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-18 01:41:34.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/clang/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)      514 2022-12-18 01:41:34.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/clang/comments.py
--rw-r--r--   0 nick      (1000) nick      (1000)     5875 2022-12-20 02:38:44.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/clang/patches.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2022-12-21 17:11:27.940039 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/domains/
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-18 01:41:34.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/domains/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1393 2022-12-18 01:41:34.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/domains/c.py
--rw-r--r--   0 nick      (1000) nick      (1000)    35413 2022-12-20 02:38:44.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/loader.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2022-12-21 17:11:27.940039 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/napoleon/
--rw-r--r--   0 nick      (1000) nick      (1000)     6275 2022-12-20 02:38:44.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/napoleon/__init__.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2022-12-21 17:11:27.940039 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/viewcode/
--rw-r--r--   0 nick      (1000) nick      (1000)    15732 2022-12-20 02:38:44.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/viewcode/__init__.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2022-12-21 17:11:27.938039 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc.egg-info/
--rw-r--r--   0 nick      (1000) nick      (1000)     3236 2022-12-21 17:11:27.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc.egg-info/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)      841 2022-12-21 17:11:27.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc.egg-info/SOURCES.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        1 2022-12-21 17:11:27.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc.egg-info/dependency_links.txt
--rw-r--r--   0 nick      (1000) nick      (1000)       65 2022-12-21 17:11:27.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc.egg-info/entry_points.txt
--rw-r--r--   0 nick      (1000) nick      (1000)       36 2022-12-21 17:11:27.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc.egg-info/requires.txt
--rw-r--r--   0 nick      (1000) nick      (1000)       17 2022-12-21 17:11:27.000000 sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1071 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/LICENSE-MIT
+-rw-r--r--   0        0        0     2669 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/README.rst
+-rw-r--r--   0        0        0     1187 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    26897 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/__init__.py
+-rw-r--r--   0        0        0     7095 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/apidoc/__init__.py
+-rw-r--r--   0        0        0       72 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/apidoc/templates/header.rst.jinja2
+-rw-r--r--   0        0        0       57 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/apidoc/templates/source.rst.jinja2
+-rw-r--r--   0        0        0      131 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/apidoc/templates/toc.rst.jinja2
+-rw-r--r--   0        0        0        0 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/clang/__init__.py
+-rw-r--r--   0        0        0      514 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/clang/comments.py
+-rw-r--r--   0        0        0     5875 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/clang/patches.py
+-rw-r--r--   0        0        0        0 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/domains/__init__.py
+-rw-r--r--   0        0        0     1393 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/domains/c.py
+-rw-r--r--   0        0        0    35622 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/loader.py
+-rw-r--r--   0        0        0     6275 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/napoleon/__init__.py
+-rw-r--r--   0        0        0    15732 2023-06-12 02:09:37.019971 sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/viewcode/__init__.py
+-rw-r--r--   0        0        0     3869 1970-01-01 00:00:00.000000 sphinx_c_autodoc-1.2.0/PKG-INFO
```

### Comparing `sphinx-c-autodoc-1.1.1/LICENSE-MIT` & `sphinx_c_autodoc-1.2.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `sphinx-c-autodoc-1.1.1/PKG-INFO` & `sphinx_c_autodoc-1.2.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: sphinx-c-autodoc
-Version: 1.1.1
-Summary: A sphinx autodoc extension for c modules
-Home-page: https://sphinx-c-autodoc.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/speedyleion/sphinx-c-autodoc
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: Framework :: Sphinx :: Extension
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE-MIT
-
 sphinx-c-autodoc
 ================
 
 |build-status| |coverage| |black| |docs|
 
 Dual-licensed under MIT or the `UNLICENSE <https://unlicense.org>`_.
 
@@ -48,23 +32,25 @@
 
 .. code-block:: rst
 
     .. autocfunction:: my_c_file.c::my_adding_function
 
 With the resulting documentation output of:
 
-.. code-block:: rst
-
-    .. c:function:: int my_adding_function(int a, int b)
+.. Note this isn't using the c:function directive because that doesn't work on
+   pypi
 
+int my_adding_function(int a, int b) 
     A simple function that adds.
 
-    :param a: The initial value
-    :param b: The value to add to `a`
-    :returns: The sum of `a` and `b`
+    :Parameters:
+        * **a** - The initial value
+        * **b** - The value to add to `a`
+
+    :Returns: The sum of `a` and `b`
 
 .. _autodoc: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html
 .. _Sphinx: https://www.sphinx-doc.org/en/master/index.html
 
 Requires
 --------
```

### Comparing `sphinx-c-autodoc-1.1.1/README.rst` & `sphinx_c_autodoc-1.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: sphinx-c-autodoc
+Version: 1.2.0
+Summary: A sphinx autodoc extension for c modules
+Home-page: https://github.com/speedyleion/sphinx-c-autodoc
+License: MIT License, The Unlicense (Unlicense)
+Author: Nick
+Author-email: speedyleion@users.noreply.github.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Sphinx :: Extension
+Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: beautifulsoup4
+Requires-Dist: clang (>=6)
+Requires-Dist: sphinx (>=3.1)
+Project-URL: Documentation, https://sphinx-c-autodoc.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/speedyleion/sphinx-c-autodoc
+Description-Content-Type: text/x-rst
+
 sphinx-c-autodoc
 ================
 
 |build-status| |coverage| |black| |docs|
 
 Dual-licensed under MIT or the `UNLICENSE <https://unlicense.org>`_.
 
@@ -32,21 +60,25 @@
 
 .. code-block:: rst
 
     .. autocfunction:: my_c_file.c::my_adding_function
 
 With the resulting documentation output of:
 
-.. c:function:: int my_adding_function(int a, int b)
+.. Note this isn't using the c:function directive because that doesn't work on
+   pypi
 
+int my_adding_function(int a, int b) 
     A simple function that adds.
 
-    :param a: The initial value
-    :param b: The value to add to `a`
-    :returns: The sum of `a` and `b`
+    :Parameters:
+        * **a** - The initial value
+        * **b** - The value to add to `a`
+
+    :Returns: The sum of `a` and `b`
 
 .. _autodoc: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html
 .. _Sphinx: https://www.sphinx-doc.org/en/master/index.html
 
 Requires
 --------
 
@@ -83,7 +115,8 @@
 
 .. inclusion_end
 
 Full Documentation
 ------------------
 
 The complete documentation can be found at https://sphinx-c-autodoc.readthedocs.io/en/latest
+
```

### Comparing `sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/__init__.py` & `sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,15 @@
 
         TODO not implemented yet.
         The user can override the skipping decision by connecting to the
         ``autodoc-skip-member`` event.
         """
         ret = []
         isattr = False
-        for (membername, member) in members:
+        for membername, member in members:
             if not want_all:
                 ret.append((membername, member, isattr))
             elif member.doc or self.options.undoc_members:
                 if member.is_public() or self.options.private_members:
                     ret.append((membername, member, isattr))
         return ret
 
@@ -639,15 +639,15 @@
         """Filter the given member list.
 
         For structures if they are documented then all members provided are
         documented.
         """
         ret = []
         isattr = False
-        for (membername, member) in members:
+        for membername, member in members:
             ret.append((membername, member, isattr))
         return ret
 
 
 class CEnumDocumenter(CTypeDocumenter):
     """
     The documenter for the autocenum directive.
```

### Comparing `sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/apidoc/__init__.py` & `sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/apidoc/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/clang/comments.py` & `sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/clang/comments.py`

 * *Files identical despite different names*

### Comparing `sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/clang/patches.py` & `sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/clang/patches.py`

 * *Files identical despite different names*

### Comparing `sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/domains/c.py` & `sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/domains/c.py`

 * *Files identical despite different names*

### Comparing `sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/loader.py` & `sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -728,25 +728,25 @@
 }
 
 
 def object_from_cursor(cursor: Cursor) -> Optional[DocumentedObject]:
     """
     Create an instance from a :class:`cindex.Cursor`
     """
-    # Spelling is always good on the "primary" node.
+    # Prior to clang 16, anonymous constructs would have an empty `spelling` and
+    # `displayname`. Clang 16 began naming anonymous constructs as:
+    #   "<construct> (anonymous at # <path_to_c_file>:<lineno>)"
+    # So need to look at the type spelling to determine if a construct is anonymous
     name = cursor.spelling
-
-    if not name:
+    if any(anon in cursor.type.spelling for anon in ("anonymous at", "unnamed at")):
         # An anonymous construct which isn't contained in a typedef will have a
         # type spelling of:
         # "<construct> (anonymous at # <path_to_c_file>:<lineno>)"
         # Typedef's should be handled by the get_nested_node() function
-        if cursor.kind in ALLOWED_ANONYMOUS and any(
-            anon in cursor.type.spelling for anon in ("anonymous at", "unnamed at")
-        ):
+        if cursor.kind in ALLOWED_ANONYMOUS:
             filename = os.path.basename(cursor.location.file.name)
             # remove the extension from the filename since the '.' is not a
             # valid c identifier. splitext will remove the trailing most
             # extension so if this file is multi dotted it will fail, just use
             # partition and grab the first part.
             filename, _, _ = filename.partition(".")
             name = f"anon_{filename}_{cursor.hash}"
```

### Comparing `sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/napoleon/__init__.py` & `sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/napoleon/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-c-autodoc-1.1.1/src/sphinx_c_autodoc/viewcode/__init__.py` & `sphinx_c_autodoc-1.2.0/src/sphinx_c_autodoc/viewcode/__init__.py`

 * *Files identical despite different names*

