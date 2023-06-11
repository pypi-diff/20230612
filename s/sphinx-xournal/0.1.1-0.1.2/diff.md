# Comparing `tmp/sphinx_xournal-0.1.1.tar.gz` & `tmp/sphinx_xournal-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_xournal-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_xournal-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_xournal-0.1.1.tar` & `sphinx_xournal-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      268 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.1/.editorconfig
--rw-r--r--   0        0        0       62 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.1/.gitignore
--rw-r--r--   0        0        0     2336 2023-06-10 00:18:44.672258 sphinx_xournal-0.1.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      178 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.1/AUTHORS.rst
--rw-r--r--   0        0        0      306 2023-06-10 00:18:44.672258 sphinx_xournal-0.1.1/HISTORY.rst
--rw-r--r--   0        0        0     7642 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.1/LICENSE
--rw-r--r--   0        0        0      167 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.1/README.rst
--rw-r--r--   0        0        0     1222 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.1/docs/templates/pyproject.toml
--rw-r--r--   0        0        0     1052 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      283 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.1/requirements.txt
--rw-r--r--   0        0        0      241 2023-06-10 00:18:44.672258 sphinx_xournal-0.1.1/sphinx_xournal/__init__.py
--rw-r--r--   0        0        0     4045 2023-06-10 00:18:44.672258 sphinx_xournal-0.1.1/sphinx_xournal/convert.py
--rw-r--r--   0        0        0     1713 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.1/sphinx_xournal/directives.py
--rw-r--r--   0        0        0      825 2023-06-10 00:18:44.672258 sphinx_xournal-0.1.1/sphinx_xournal/exceptions.py
--rw-r--r--   0        0        0     1453 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.1/sphinx_xournal/main.py
--rw-r--r--   0        0        0        0 2023-06-10 00:29:20.406053 sphinx_xournal-0.1.1/sphinx_xournal/xournal.css
--rw-r--r--   0        0        0     3320 2023-06-09 14:52:42.777621 sphinx_xournal-0.1.1/tasks.py
--rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 sphinx_xournal-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      268 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.2/.editorconfig
+-rw-r--r--   0        0        0       62 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.2/.gitignore
+-rw-r--r--   0        0        0     2336 2023-06-10 00:18:44.672258 sphinx_xournal-0.1.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      178 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.2/AUTHORS.rst
+-rw-r--r--   0        0        0      372 2023-06-11 21:40:55.565686 sphinx_xournal-0.1.2/HISTORY.rst
+-rw-r--r--   0        0        0     7642 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1494 2023-06-11 21:40:55.565686 sphinx_xournal-0.1.2/README.rst
+-rw-r--r--   0        0        0     1222 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.2/docs/templates/pyproject.toml
+-rw-r--r--   0        0        0     1052 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      283 2023-06-09 14:52:42.773620 sphinx_xournal-0.1.2/requirements.txt
+-rw-r--r--   0        0        0      241 2023-06-11 21:40:55.565686 sphinx_xournal-0.1.2/sphinx_xournal/__init__.py
+-rw-r--r--   0        0        0     4045 2023-06-10 00:18:44.672258 sphinx_xournal-0.1.2/sphinx_xournal/convert.py
+-rw-r--r--   0        0        0     1713 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.2/sphinx_xournal/directives.py
+-rw-r--r--   0        0        0      825 2023-06-10 00:18:44.672258 sphinx_xournal-0.1.2/sphinx_xournal/exceptions.py
+-rw-r--r--   0        0        0     1453 2023-06-09 19:39:40.614842 sphinx_xournal-0.1.2/sphinx_xournal/main.py
+-rw-r--r--   0        0        0        0 2023-06-11 21:51:32.686856 sphinx_xournal-0.1.2/sphinx_xournal/xournal.css
+-rw-r--r--   0        0        0     3628 2023-06-11 21:40:55.565686 sphinx_xournal-0.1.2/tasks.py
+-rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 sphinx_xournal-0.1.2/PKG-INFO
```

### Comparing `sphinx_xournal-0.1.1/.gitlab-ci.yml` & `sphinx_xournal-0.1.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.1.1/LICENSE` & `sphinx_xournal-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.1.1/docs/templates/pyproject.toml` & `sphinx_xournal-0.1.2/docs/templates/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.1.1/pyproject.toml` & `sphinx_xournal-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.1.1/sphinx_xournal/convert.py` & `sphinx_xournal-0.1.2/sphinx_xournal/convert.py`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.1.1/sphinx_xournal/directives.py` & `sphinx_xournal-0.1.2/sphinx_xournal/directives.py`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.1.1/sphinx_xournal/exceptions.py` & `sphinx_xournal-0.1.2/sphinx_xournal/exceptions.py`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.1.1/sphinx_xournal/main.py` & `sphinx_xournal-0.1.2/sphinx_xournal/main.py`

 * *Files identical despite different names*

### Comparing `sphinx_xournal-0.1.1/tasks.py` & `sphinx_xournal-0.1.2/tasks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from pathlib import Path
 
 from invoke import task
 from jinja2 import Template
 
 
 @task
@@ -14,14 +15,22 @@
 
 @task(name="docs", aliases=("html", "documentation"))
 def docs_html(c, output_directory="build/html"):
     """Build the documentation in HTML form."""
     c.run(f"python3 -m sphinx docs {output_directory}")
 
 
+@task(name="preview", aliases=("rst",))
+def preview(c):
+    """Show a preview of the README file."""
+    rst_view = c.run(f"restview --listen=8888 --browser --pypi-strict README.rst", asynchronous=True, out_stream=sys.stdout)
+    print("Listening on http://localhost:8888/")
+    rst_view.join()
+
+
 @task
 def clean(c):
     """Remove all artefacts."""
     patterns = ["build", "docs/build"]
     for pattern in patterns:
         c.run(f"rm -rf {pattern}")
```

