# Comparing `tmp/telepath-0.3.tar.gz` & `tmp/telepath-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/telepath-0.3.tar", last modified: Tue Sep 13 08:50:30 2022, max compression
+gzip compressed data, was "telepath-0.3.1.tar", last modified: Mon Jun 12 11:52:04 2023, max compression
```

## Comparing `telepath-0.3.tar` & `telepath-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-09-13 08:50:30.209005 telepath-0.3/
--rw-r--r--   0 matthew    (501) staff       (20)      432 2022-09-13 08:37:33.000000 telepath-0.3/CHANGELOG.md
--rw-r--r--   0 matthew    (501) staff       (20)     1512 2021-02-10 13:19:47.000000 telepath-0.3/LICENSE
--rw-r--r--   0 matthew    (501) staff       (20)       57 2021-04-22 15:04:46.000000 telepath-0.3/MANIFEST.in
--rw-r--r--   0 matthew    (501) staff       (20)     1653 2022-09-13 08:50:30.209184 telepath-0.3/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)      797 2021-02-10 23:26:29.000000 telepath-0.3/README.md
--rw-r--r--   0 matthew    (501) staff       (20)       71 2022-09-13 08:50:30.209728 telepath-0.3/setup.cfg
--rw-r--r--   0 matthew    (501) staff       (20)     1174 2022-09-13 08:38:36.000000 telepath-0.3/setup.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-09-13 08:50:30.204449 telepath-0.3/telepath/
--rw-r--r--   0 matthew    (501) staff       (20)    12622 2022-09-13 08:30:34.000000 telepath-0.3/telepath/__init__.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-09-13 08:50:30.197787 telepath-0.3/telepath/static/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-09-13 08:50:30.198088 telepath-0.3/telepath/static/telepath/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-09-13 08:50:30.208268 telepath-0.3/telepath/static/telepath/js/
--rw-r--r--   0 matthew    (501) staff       (20)     4491 2021-04-22 15:11:09.000000 telepath-0.3/telepath/static/telepath/js/telepath.js
--rw-r--r--   0 matthew    (501) staff       (20)      122 2021-02-10 13:42:45.000000 telepath-0.3/telepath/test_settings.py
--rw-r--r--   0 matthew    (501) staff       (20)     9813 2022-09-13 08:30:34.000000 telepath-0.3/telepath/tests.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2022-09-13 08:50:30.207635 telepath-0.3/telepath.egg-info/
--rw-r--r--   0 matthew    (501) staff       (20)     1653 2022-09-13 08:50:29.000000 telepath-0.3/telepath.egg-info/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)      325 2022-09-13 08:50:29.000000 telepath-0.3/telepath.egg-info/SOURCES.txt
--rw-r--r--   0 matthew    (501) staff       (20)        1 2022-09-13 08:50:29.000000 telepath-0.3/telepath.egg-info/dependency_links.txt
--rw-r--r--   0 matthew    (501) staff       (20)       51 2022-09-13 08:50:29.000000 telepath-0.3/telepath.egg-info/requires.txt
--rw-r--r--   0 matthew    (501) staff       (20)        9 2022-09-13 08:50:29.000000 telepath-0.3/telepath.egg-info/top_level.txt
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-06-12 11:52:04.926576 telepath-0.3.1/
+-rw-r--r--   0 matthew    (501) staff       (20)      603 2023-06-12 11:45:07.000000 telepath-0.3.1/CHANGELOG.md
+-rw-r--r--   0 matthew    (501) staff       (20)     1512 2021-02-10 13:19:47.000000 telepath-0.3.1/LICENSE
+-rw-r--r--   0 matthew    (501) staff       (20)       57 2021-04-22 15:04:46.000000 telepath-0.3.1/MANIFEST.in
+-rw-r--r--   0 matthew    (501) staff       (20)     1574 2023-06-12 11:52:04.926752 telepath-0.3.1/PKG-INFO
+-rw-r--r--   0 matthew    (501) staff       (20)      797 2021-02-10 23:26:29.000000 telepath-0.3.1/README.md
+-rw-r--r--   0 matthew    (501) staff       (20)       71 2023-06-12 11:52:04.927495 telepath-0.3.1/setup.cfg
+-rw-r--r--   0 matthew    (501) staff       (20)     1176 2023-06-12 11:32:11.000000 telepath-0.3.1/setup.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-06-12 11:52:04.922506 telepath-0.3.1/telepath/
+-rw-r--r--   0 matthew    (501) staff       (20)    12614 2023-06-12 11:25:18.000000 telepath-0.3.1/telepath/__init__.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-06-12 11:52:04.917670 telepath-0.3.1/telepath/static/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-06-12 11:52:04.917826 telepath-0.3.1/telepath/static/telepath/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-06-12 11:52:04.925826 telepath-0.3.1/telepath/static/telepath/js/
+-rw-r--r--   0 matthew    (501) staff       (20)     4491 2021-04-22 15:11:09.000000 telepath-0.3.1/telepath/static/telepath/js/telepath.js
+-rw-r--r--   0 matthew    (501) staff       (20)      122 2021-02-10 13:42:45.000000 telepath-0.3.1/telepath/test_settings.py
+-rw-r--r--   0 matthew    (501) staff       (20)     9813 2022-09-13 08:30:34.000000 telepath-0.3.1/telepath/tests.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-06-12 11:52:04.924840 telepath-0.3.1/telepath.egg-info/
+-rw-r--r--   0 matthew    (501) staff       (20)     1574 2023-06-12 11:52:04.000000 telepath-0.3.1/telepath.egg-info/PKG-INFO
+-rw-r--r--   0 matthew    (501) staff       (20)      325 2023-06-12 11:52:04.000000 telepath-0.3.1/telepath.egg-info/SOURCES.txt
+-rw-r--r--   0 matthew    (501) staff       (20)        1 2023-06-12 11:52:04.000000 telepath-0.3.1/telepath.egg-info/dependency_links.txt
+-rw-r--r--   0 matthew    (501) staff       (20)       51 2023-06-12 11:52:04.000000 telepath-0.3.1/telepath.egg-info/requires.txt
+-rw-r--r--   0 matthew    (501) staff       (20)        9 2023-06-12 11:52:04.000000 telepath-0.3.1/telepath.egg-info/top_level.txt
```

### Comparing `telepath-0.3/LICENSE` & `telepath-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `telepath-0.3/PKG-INFO` & `telepath-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: telepath
-Version: 0.3
+Version: 0.3.1
 Summary: A library for exchanging data between Python and JavaScript
 Home-page: https://github.com/wagtail/telepath
 Author: Matthew Westcott
 Author-email: matthew.westcott@torchbox.com
 License: BSD
-Description: # telepath
-        
-        *telepath* is a Django library for exchanging data between Python and JavaScript, allowing you to build apps with rich client-side interfaces while keeping the business logic in server-side code.
-        
-        ## What does it do?
-        
-        It provides a mechanism for packing structured data, including Python objects, into a JSON-serializable format. This mechanism can be extended to support any Python class, by registering the class with a corresponding JavaScript implementation. The packed data can then be included in an HTTP response, and unpacked in JavaScript to obtain an equivalent data structure to the original. Think of it as [`pickle`](https://docs.python.org/3/library/pickle.html), but with the unpickling happening in the browser.
-        
-        Full documentation: https://wagtail.github.io/telepath/
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Django
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
+License-File: LICENSE
+
+# telepath
+
+*telepath* is a Django library for exchanging data between Python and JavaScript, allowing you to build apps with rich client-side interfaces while keeping the business logic in server-side code.
+
+## What does it do?
+
+It provides a mechanism for packing structured data, including Python objects, into a JSON-serializable format. This mechanism can be extended to support any Python class, by registering the class with a corresponding JavaScript implementation. The packed data can then be included in an HTTP response, and unpacked in JavaScript to obtain an equivalent data structure to the original. Think of it as [`pickle`](https://docs.python.org/3/library/pickle.html), but with the unpickling happening in the browser.
+
+Full documentation: https://wagtail.github.io/telepath/
```

### Comparing `telepath-0.3/README.md` & `telepath-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `telepath-0.3/setup.py` & `telepath-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name='telepath',
-    version='0.3',
+    version='0.3.1',
     description="A library for exchanging data between Python and JavaScript",
     author='Matthew Westcott',
     author_email='matthew.westcott@torchbox.com',
     url='https://github.com/wagtail/telepath',
     packages=["telepath"],
     include_package_data=True,
     license='BSD',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    python_requires=">=3.5",
+    python_requires=">=3.8",
     extras_require={
         'docs': [
             'mkdocs>=1.1,<1.2',
             'mkdocs-material>=6.2,<6.3',
         ],
     },
     classifiers=[
```

### Comparing `telepath-0.3/telepath/__init__.py` & `telepath-0.3.1/telepath/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,17 +336,17 @@
     def _build_new_node(self, obj):
         adapter = self.registry.find_adapter(type(obj))
         if adapter:
             return adapter.build_node(obj, self)
 
         # No adapter found; try special-case fallbacks
 
-        if isinstance(obj, Promise) and obj._delegate_text:
-            # object is a lazy translation object; handle as a string, translated to the currently
-            # active locale
+        if isinstance(obj, Promise):
+            # object is a lazy object (e.g. gettext_lazy result);
+            # handle as a string, translated to the currently active locale
             return StringNode(str(obj))
 
         # try handling as an iterable
         try:
             items = iter(obj)
         except TypeError:  # obj is not iterable
             raise UnpackableTypeError("don't know how to pack object: %r" % obj)
```

### Comparing `telepath-0.3/telepath/static/telepath/js/telepath.js` & `telepath-0.3.1/telepath/static/telepath/js/telepath.js`

 * *Files identical despite different names*

### Comparing `telepath-0.3/telepath/tests.py` & `telepath-0.3.1/telepath/tests.py`

 * *Files identical despite different names*

### Comparing `telepath-0.3/telepath.egg-info/PKG-INFO` & `telepath-0.3.1/telepath.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: telepath
-Version: 0.3
+Version: 0.3.1
 Summary: A library for exchanging data between Python and JavaScript
 Home-page: https://github.com/wagtail/telepath
 Author: Matthew Westcott
 Author-email: matthew.westcott@torchbox.com
 License: BSD
-Description: # telepath
-        
-        *telepath* is a Django library for exchanging data between Python and JavaScript, allowing you to build apps with rich client-side interfaces while keeping the business logic in server-side code.
-        
-        ## What does it do?
-        
-        It provides a mechanism for packing structured data, including Python objects, into a JSON-serializable format. This mechanism can be extended to support any Python class, by registering the class with a corresponding JavaScript implementation. The packed data can then be included in an HTTP response, and unpacked in JavaScript to obtain an equivalent data structure to the original. Think of it as [`pickle`](https://docs.python.org/3/library/pickle.html), but with the unpickling happening in the browser.
-        
-        Full documentation: https://wagtail.github.io/telepath/
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Django
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
+License-File: LICENSE
+
+# telepath
+
+*telepath* is a Django library for exchanging data between Python and JavaScript, allowing you to build apps with rich client-side interfaces while keeping the business logic in server-side code.
+
+## What does it do?
+
+It provides a mechanism for packing structured data, including Python objects, into a JSON-serializable format. This mechanism can be extended to support any Python class, by registering the class with a corresponding JavaScript implementation. The packed data can then be included in an HTTP response, and unpacked in JavaScript to obtain an equivalent data structure to the original. Think of it as [`pickle`](https://docs.python.org/3/library/pickle.html), but with the unpickling happening in the browser.
+
+Full documentation: https://wagtail.github.io/telepath/
```

