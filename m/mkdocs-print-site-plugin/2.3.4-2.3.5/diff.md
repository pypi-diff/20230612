# Comparing `tmp/mkdocs-print-site-plugin-2.3.4.tar.gz` & `tmp/mkdocs-print-site-plugin-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-print-site-plugin-2.3.4.tar", last modified: Wed Jun  1 11:12:01 2022, max compression
+gzip compressed data, was "mkdocs-print-site-plugin-2.3.5.tar", last modified: Mon Jun 12 08:52:07 2023, max compression
```

## Comparing `mkdocs-print-site-plugin-2.3.4.tar` & `mkdocs-print-site-plugin-2.3.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 11:12:01.745347 mkdocs-print-site-plugin-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-06-01 11:12:01.745347 mkdocs-print-site-plugin-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2529 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 11:12:01.737347 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 11:12:01.741347 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/
--rw-r--r--   0 runner    (1001) docker     (121)     3477 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site-enum-headings1.css
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site-enum-headings2.css
--rw-r--r--   0 runner    (1001) docker     (121)     1444 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site-enum-headings3.css
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site-enum-headings4.css
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site-enum-headings5.css
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site-enum-headings6.css
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site-material.css
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site-mkdocs.css
--rw-r--r--   0 runner    (1001) docker     (121)     5463 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site.css
--rw-r--r--   0 runner    (1001) docker     (121)     1570 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/exclude.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 11:12:01.741347 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/js/
--rw-r--r--   0 runner    (1001) docker     (121)     4515 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/js/print-site.js
--rw-r--r--   0 runner    (1001) docker     (121)    16921 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     9147 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 11:12:01.741347 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/templates/cover_page.tpl
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/templates/print_site_banner.tpl
--rw-r--r--   0 runner    (1001) docker     (121)     8832 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      863 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 11:12:01.741347 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-06-01 11:12:01.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-06-01 11:12:01.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-01 11:12:01.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-06-01 11:12:01.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-06-01 11:12:01.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-01 11:12:01.000000 mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-01 11:12:01.745347 mkdocs-print-site-plugin-2.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 11:12:01.741347 mkdocs-print-site-plugin-2.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9196 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/tests/test_building.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/tests/test_exclude.py
--rw-r--r--   0 runner    (1001) docker     (121)     7564 2022-06-01 11:11:26.000000 mkdocs-print-site-plugin-2.3.4/tests/test_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:52:07.287180 mkdocs-print-site-plugin-2.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-12 08:52:07.287180 mkdocs-print-site-plugin-2.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:52:07.283180 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:52:07.287180 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings1.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings2.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings3.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings4.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings5.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings6.css
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-material.css
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-mkdocs.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/exclude.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:52:07.287180 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/js/print-site.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17143 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:52:07.287180 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/templates/cover_page.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/templates/print_site_banner.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:52:07.283180 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-12 08:52:07.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-12 08:52:07.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:52:07.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-12 08:52:07.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 08:52:07.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 08:52:07.000000 mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 08:52:07.287180 mkdocs-print-site-plugin-2.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:52:07.287180 mkdocs-print-site-plugin-2.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/tests/test_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/tests/test_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-12 08:51:27.000000 mkdocs-print-site-plugin-2.3.5/tests/test_urls.py
```

### Comparing `mkdocs-print-site-plugin-2.3.4/LICENSE` & `mkdocs-print-site-plugin-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/PKG-INFO` & `mkdocs-print-site-plugin-2.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: mkdocs-print-site-plugin
-Version: 2.3.4
+Version: 2.3.5
 Summary: MkDocs plugin that combines all pages into one, allowing for easy export to PDF and standalone HTML.
 Home-page: https://github.com/timvink/mkdocs-print-site-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin print pdf
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -72,9 +71,7 @@
 ## Documentation
 
 Available at [timvink.github.io/mkdocs-print-site-plugin](https://timvink.github.io/mkdocs-print-site-plugin/).
 
 ## Contributing
 
 Contributions are very welcome! Start by reading the [contribution guidelines](https://timvink.github.io/mkdocs-print-site-plugin/contributing.html).
-
-
```

### Comparing `mkdocs-print-site-plugin-2.3.4/README.md` & `mkdocs-print-site-plugin-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site-enum-headings1.css` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings1.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site-enum-headings2.css` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings2.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site-enum-headings3.css` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings3.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site-enum-headings4.css` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings4.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site-enum-headings5.css` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings5.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site-enum-headings6.css` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-enum-headings6.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site-material.css` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-material.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site-mkdocs.css` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site-mkdocs.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/css/print-site.css` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/css/print-site.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/exclude.py` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/exclude.py`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/js/print-site.js` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/js/print-site.js`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/plugin.py` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from mkdocs.structure.files import File
 from mkdocs.structure.pages import Page
 from mkdocs.utils import write_file, copy_file, get_relative_url, warning_filter
 from mkdocs.exceptions import PluginError
 
 from mkdocs_print_site_plugin.renderer import Renderer
 from mkdocs_print_site_plugin.utils import flatten_nav, get_theme_name
+from mkdocs_print_site_plugin.urls import is_external
 
 logger = logging.getLogger("mkdocs.plugins")
 logger.addFilter(warning_filter)
 
 HERE = os.path.dirname(os.path.abspath(__file__))
 
 
@@ -227,17 +228,22 @@
                     if not match.group() == "<h1":
                         msg = f"The page {page.title} ({page.file.src_path}) does not start with a level 1 heading."
                         msg += "This is required for print page Table of Contents and/or enumeration of headings."
                         raise AssertionError(msg)
 
         # Link to the PDF version of the entire site on a page.
         if self.config.get("path_to_pdf") != "":
-            page.url_to_pdf = get_relative_url(
-                self.config.get("path_to_pdf"), page.file.url
-            )
+            pdf_url = self.config.get("path_to_pdf")
+            if is_external(pdf_url):
+                page.url_to_pdf = pdf_url
+            else:
+                breakpoint()
+                page.url_to_pdf = get_relative_url(
+                    pdf_url, page.file.url
+                )
 
         return html
 
     def on_page_context(self, context, page, config, nav, **kwargs):
         """
         The page_context event is called after the context for a page is created.
```

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/renderer.py` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/renderer.py`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/templates/cover_page.tpl` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/templates/cover_page.tpl`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/templates/print_site_banner.tpl` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/templates/print_site_banner.tpl`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/urls.py` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin/utils.py` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin.egg-info/PKG-INFO` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: mkdocs-print-site-plugin
-Version: 2.3.4
+Version: 2.3.5
 Summary: MkDocs plugin that combines all pages into one, allowing for easy export to PDF and standalone HTML.
 Home-page: https://github.com/timvink/mkdocs-print-site-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin print pdf
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -72,9 +71,7 @@
 ## Documentation
 
 Available at [timvink.github.io/mkdocs-print-site-plugin](https://timvink.github.io/mkdocs-print-site-plugin/).
 
 ## Contributing
 
 Contributions are very welcome! Start by reading the [contribution guidelines](https://timvink.github.io/mkdocs-print-site-plugin/contributing.html).
-
-
```

### Comparing `mkdocs-print-site-plugin-2.3.4/mkdocs_print_site_plugin.egg-info/SOURCES.txt` & `mkdocs-print-site-plugin-2.3.5/mkdocs_print_site_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/setup.py` & `mkdocs-print-site-plugin-2.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = ""
     for line in f:
         long_description += line
 
 
 setup(
     name="mkdocs-print-site-plugin",
-    version="2.3.4",
+    version="2.3.5",
     description="MkDocs plugin that combines all pages into one, allowing for easy export to PDF and standalone HTML.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs plugin print pdf",
     url="https://github.com/timvink/mkdocs-print-site-plugin",
     author="Tim Vink",
     author_email="vinktim@gmail.com",
```

### Comparing `mkdocs-print-site-plugin-2.3.4/tests/test_building.py` & `mkdocs-print-site-plugin-2.3.5/tests/test_building.py`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.4/tests/test_urls.py` & `mkdocs-print-site-plugin-2.3.5/tests/test_urls.py`

 * *Files identical despite different names*

