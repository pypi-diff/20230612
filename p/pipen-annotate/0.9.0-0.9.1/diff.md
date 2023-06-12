# Comparing `tmp/pipen_annotate-0.9.0.tar.gz` & `tmp/pipen_annotate-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_annotate-0.9.0.tar", max compression
+gzip compressed data, was "pipen_annotate-0.9.1.tar", max compression
```

## Comparing `pipen_annotate-0.9.0.tar` & `pipen_annotate-0.9.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-06-09 06:19:04.092303 pipen_annotate-0.9.0/LICENSE
--rw-r--r--   0        0        0     1592 2023-06-09 06:19:04.092303 pipen_annotate-0.9.0/README.md
--rw-r--r--   0        0        0      108 2023-06-09 06:19:04.092303 pipen_annotate-0.9.0/pipen_annotate/__init__.py
--rw-r--r--   0        0        0     7736 2023-06-09 06:19:04.092303 pipen_annotate-0.9.0/pipen_annotate/annotate.py
--rw-r--r--   0        0        0    14710 2023-06-09 06:19:04.092303 pipen_annotate-0.9.0/pipen_annotate/sections.py
--rw-r--r--   0        0        0     1525 2023-06-09 06:19:04.092303 pipen_annotate-0.9.0/pipen_annotate/utils.py
--rw-r--r--   0        0        0      959 2023-06-09 06:19:04.092303 pipen_annotate-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     2375 1970-01-01 00:00:00.000000 pipen_annotate-0.9.0/setup.py
--rw-r--r--   0        0        0     2168 1970-01-01 00:00:00.000000 pipen_annotate-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-12 07:03:12.113928 pipen_annotate-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1592 2023-06-12 07:03:12.113928 pipen_annotate-0.9.1/README.md
+-rw-r--r--   0        0        0      108 2023-06-12 07:03:12.113928 pipen_annotate-0.9.1/pipen_annotate/__init__.py
+-rw-r--r--   0        0        0     7724 2023-06-12 07:03:12.113928 pipen_annotate-0.9.1/pipen_annotate/annotate.py
+-rw-r--r--   0        0        0    14710 2023-06-12 07:03:12.113928 pipen_annotate-0.9.1/pipen_annotate/sections.py
+-rw-r--r--   0        0        0     1525 2023-06-12 07:03:12.113928 pipen_annotate-0.9.1/pipen_annotate/utils.py
+-rw-r--r--   0        0        0      959 2023-06-12 07:03:12.113928 pipen_annotate-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2375 1970-01-01 00:00:00.000000 pipen_annotate-0.9.1/setup.py
+-rw-r--r--   0        0        0     2168 1970-01-01 00:00:00.000000 pipen_annotate-0.9.1/PKG-INFO
```

### Comparing `pipen_annotate-0.9.0/LICENSE` & `pipen_annotate-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipen_annotate-0.9.0/README.md` & `pipen_annotate-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pipen_annotate-0.9.0/pipen_annotate/annotate.py` & `pipen_annotate-0.9.1/pipen_annotate/annotate.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,17 +108,17 @@
 
 def _update_annotation(
     base: OrderedDiot | None,
     other: OrderedDiot,
 ) -> OrderedDiot:
     """Update the annotation with another annotation."""
     if base is None:
-        base = OrderedDiot(diot_nest=False)
-    else:
-        base = base.copy()
+        return other
+
+    base = other.__class__(base, diot_nest=False)
 
     for key, value in other.items():
         section_class = SECTION_TYPES.get(key)
         if key not in base or section_class is None:
             base[key] = value
         else:
             base[key] = section_class.update_parsed(base[key], value)
@@ -250,15 +250,15 @@
             return cls
 
         # If the class has no docstring, inherit from base class
         cls.__doc__ = indent_text(base.__doc__, indent)
         return cls
 
     base_annotated = annotate(base)
-    docstr = Liquid(docstr, from_file=False).render(base=base_annotated)
+    docstr = Liquid(docstr, from_file=False).render(**base_annotated)
     cls.__doc__ = indent_text(docstr, indent)
 
     return cls
 
 
 annotate.register_section = _register_section
 annotate.unregister_section = _unregister_section
```

### Comparing `pipen_annotate-0.9.0/pipen_annotate/sections.py` & `pipen_annotate-0.9.1/pipen_annotate/sections.py`

 * *Files identical despite different names*

### Comparing `pipen_annotate-0.9.0/pipen_annotate/utils.py` & `pipen_annotate-0.9.1/pipen_annotate/utils.py`

 * *Files identical despite different names*

### Comparing `pipen_annotate-0.9.0/pyproject.toml` & `pipen_annotate-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-annotate"
-version = "0.9.0"
+version = "0.9.1"
 description = "Use docstring to annotate pipen processes"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.build]
 generate-setup-file = true
```

### Comparing `pipen_annotate-0.9.0/setup.py` & `pipen_annotate-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pipen>=0.10,<0.11']
 
 setup_kwargs = {
     'name': 'pipen-annotate',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Use docstring to annotate pipen processes',
     'long_description': '# pipen-annotate\n\nUse docstring to annotate [pipen](https://github.com/pwwang/pipen) processes\n\n## Installation\n\n```shell\npip install -U pipen-annotate\n```\n\n## Usage\n\n```python\nfrom pprint import pprint\nfrom pipen import Proc\nfrom pipen_annotate import annotate\n\n\nclass Process(Proc):\n    """Short description\n\n    Long description\n\n    Input:\n        infile: An input file\n        invar: An input variable\n\n    Output:\n        outfile: The output file\n\n    Envs:\n        ncores: Number of cores\n    """\n    input = "infile:file, invar"\n    output = "outfile:file:output.txt"\n    args = {\'ncores\': 1}\n\nannotated = annotate(Process)\n# prints:\n{\'Envs\': {\'ncores\': {\'attrs\': OrderedDiot([(\'default\', 1)]),\n                     \'help\': \'Number of cores\',\n                     \'terms\': OrderedDiot([])}},\n \'Input\': {\'infile\': {\'attrs\': {\'action\': \'extend\',\n                                \'itype\': \'file\',\n                                \'nargs\': \'+\'},\n                      \'help\': \'An input file\',\n                      \'terms\': OrderedDiot([])},\n           \'invar\': {\'attrs\': {\'action\': \'extend\',\n                               \'itype\': \'var\',\n                               \'nargs\': \'+\'},\n                     \'help\': \'An input variable\',\n                     \'terms\': OrderedDiot([])}},\n \'Output\': {\'outfile\': {\'attrs\': {\'default\': \'output.txt\',\n                                  \'otype\': \'file\'},\n                        \'help\': \'The output file\',\n                        \'terms\': OrderedDiot([])}},\n \'Summary\': {\'long\': \'Long description\\n\',\n             \'short\': \'Short description\'}}\n```\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pipen_annotate-0.9.0/PKG-INFO` & `pipen_annotate-0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-annotate
-Version: 0.9.0
+Version: 0.9.1
 Summary: Use docstring to annotate pipen processes
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

