# Comparing `tmp/textual_select-0.3.3.tar.gz` & `tmp/textual_select-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual_select-0.3.3.tar", max compression
+gzip compressed data, was "textual_select-0.3.4.tar", max compression
```

## Comparing `textual_select-0.3.3.tar` & `textual_select-0.3.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1075 2022-12-16 09:32:48.719192 textual_select-0.3.3/LICENSE
--rw-r--r--   0        0        0     1783 2023-03-08 07:43:06.459166 textual_select-0.3.3/README.md
--rw-r--r--   0        0        0     1032 2023-03-27 07:08:50.810977 textual_select-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       70 2022-12-23 07:21:50.314230 textual_select-0.3.3/textual_select/__init__.py
--rw-r--r--   0        0        0    10507 2023-03-27 07:08:27.587236 textual_select-0.3.3/textual_select/_select.py
--rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 textual_select-0.3.3/setup.py
--rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 textual_select-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-12-16 09:32:48.719192 textual_select-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2077 2023-06-12 13:18:16.649498 textual_select-0.3.4/README.md
+-rw-r--r--   0        0        0     1032 2023-06-12 13:19:56.224412 textual_select-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0       70 2022-12-23 07:21:50.314230 textual_select-0.3.4/textual_select/__init__.py
+-rw-r--r--   0        0        0    10508 2023-06-12 13:11:48.234188 textual_select-0.3.4/textual_select/_select.py
+-rw-r--r--   0        0        0     2827 1970-01-01 00:00:00.000000 textual_select-0.3.4/setup.py
+-rw-r--r--   0        0        0     3231 1970-01-01 00:00:00.000000 textual_select-0.3.4/PKG-INFO
```

### Comparing `textual_select-0.3.3/LICENSE` & `textual_select-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `textual_select-0.3.3/pyproject.toml` & `textual_select-0.3.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textual-select"
-version = "0.3.3"
+version = "0.3.4"
 description = "A select widget (aka dropdown) for Textual."
 authors = ["Mischa Schindowski <mschindowski@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "textual_select"}]
 repository = "https://github.com/mitosch/textual-select"
 keywords = ["textual", "textual select", "textual dropdown"]
```

### Comparing `textual_select-0.3.3/textual_select/_select.py` & `textual_select-0.3.4/textual_select/_select.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         )
         self.select_list = select_list
 
     def on_blur(self) -> None:
         self.select_list.display = False
 
     def on_list_item__child_clicked(self, event: ListItem._ChildClicked) -> None:
-        super().on_list_item__child_clicked(event)
+        super()._on_list_item__child_clicked(event)
 
         self.select_list.select_highlighted_item()
         self.select_list.display = False
 
 
 class SelectList(Widget):
     """The dropdown list which is opened at the input."""
```

### Comparing `textual_select-0.3.3/setup.py` & `textual_select-0.3.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['textual>=0.14.0']
 
 setup_kwargs = {
     'name': 'textual-select',
-    'version': '0.3.3',
+    'version': '0.3.4',
     'description': 'A select widget (aka dropdown) for Textual.',
-    'long_description': '# Textual: Select\n\nA simple select widget (aka dropdown) for [textual](https://github.com/Textualize/textual) with an optional search field.\n\n![select_focus](https://user-images.githubusercontent.com/922559/209305346-6b8971b1-7a3a-4424-bdf8-c439b9d74e28.png)\n\n![select_open](https://user-images.githubusercontent.com/922559/209305349-84f39432-b1e4-405e-8854-a8d7a33230ae.png)\n\n![select_search](https://user-images.githubusercontent.com/922559/209305352-9ad2e7c1-9dc6-435f-b1bd-8dba5f5b2642.png)\n\n\n## Usage\n\n```python\nfrom textual_select import Select\n\ndropdown_data = [\n    {"value": 0, "text": "Pick-Up"},\n    {"value": 1, "text": "SUV"},\n    {"value": 2, "text": "Hatchback"},\n    {"value": 3, "text": "Crossover"},\n    {"value": 4, "text": "Convertible"},\n    {"value": 5, "text": "Sedan"},\n    {"value": 6, "text": "Sports Car"},\n    {"value": 7, "text": "Coupe"},\n    {"value": 8, "text": "Minivan"}\n]\n\nSelect(\n    placeholder="please select",\n    items=dropdown_data,\n    list_mount="#main_container"\n)\n```\n\n## Installation\n\n```bash\npip install textual-select\n```\n\nRequires textual 0.11.0 or later.\n\n## Limitations\n\nThis textual widget is in early stage and has some limitations:\n\n* It needs a specific mount point (`list_mount`) where the dropdown list\n  shall appear. This is needed because the container widget with the select\n  itself could be too small. Maybe in future versions this will no longer\n  needed.\n* It can only open below, not above: Make sure to reserve space below the\n  dropdown.\n* The dropdown list has a fixed height of 5 entries. This will be configurable\n  in future versions.\n\n## Similar Widgets\n\n* If you are looking for an autocomplete, please refer to\n  [textual-autocomplete](https://github.com/darrenburns/textual-autocomplete)\n  by Darren Burns.\n',
+    'long_description': '# Textual: Select\n\nIMPORTANT: Since version 0.24.0 Textual implemented a native dropdown. I strongly\nrecommend to use the native version. This repository will slowly die. More information\nat the [Blog Post about Select control](https://textual.textualize.io/blog/2023/05/08/textual-0240-adds-a-select-control/).\n\nA simple select widget (aka dropdown) for [textual](https://github.com/Textualize/textual) with an optional search field.\n\n![select_focus](https://user-images.githubusercontent.com/922559/209305346-6b8971b1-7a3a-4424-bdf8-c439b9d74e28.png)\n\n![select_open](https://user-images.githubusercontent.com/922559/209305349-84f39432-b1e4-405e-8854-a8d7a33230ae.png)\n\n![select_search](https://user-images.githubusercontent.com/922559/209305352-9ad2e7c1-9dc6-435f-b1bd-8dba5f5b2642.png)\n\n\n## Usage\n\n```python\nfrom textual_select import Select\n\ndropdown_data = [\n    {"value": 0, "text": "Pick-Up"},\n    {"value": 1, "text": "SUV"},\n    {"value": 2, "text": "Hatchback"},\n    {"value": 3, "text": "Crossover"},\n    {"value": 4, "text": "Convertible"},\n    {"value": 5, "text": "Sedan"},\n    {"value": 6, "text": "Sports Car"},\n    {"value": 7, "text": "Coupe"},\n    {"value": 8, "text": "Minivan"}\n]\n\nSelect(\n    placeholder="please select",\n    items=dropdown_data,\n    list_mount="#main_container"\n)\n```\n\n## Installation\n\n```bash\npip install textual-select\n```\n\nRequires textual 0.11.0 or later.\n\n## Limitations\n\nThis textual widget is in early stage and has some limitations:\n\n* It needs a specific mount point (`list_mount`) where the dropdown list\n  shall appear. This is needed because the container widget with the select\n  itself could be too small. Maybe in future versions this will no longer\n  needed.\n* It can only open below, not above: Make sure to reserve space below the\n  dropdown.\n* The dropdown list has a fixed height of 5 entries. This will be configurable\n  in future versions.\n\n## Similar Widgets\n\n* If you are looking for an autocomplete, please refer to\n  [textual-autocomplete](https://github.com/darrenburns/textual-autocomplete)\n  by Darren Burns.\n',
     'author': 'Mischa Schindowski',
     'author_email': 'mschindowski@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mitosch/textual-select',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `textual_select-0.3.3/PKG-INFO` & `textual_select-0.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-select
-Version: 0.3.3
+Version: 0.3.4
 Summary: A select widget (aka dropdown) for Textual.
 Home-page: https://github.com/mitosch/textual-select
 License: MIT
 Keywords: textual,textual select,textual dropdown
 Author: Mischa Schindowski
 Author-email: mschindowski@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -24,14 +24,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: textual (>=0.14.0)
 Project-URL: Repository, https://github.com/mitosch/textual-select
 Description-Content-Type: text/markdown
 
 # Textual: Select
 
+IMPORTANT: Since version 0.24.0 Textual implemented a native dropdown. I strongly
+recommend to use the native version. This repository will slowly die. More information
+at the [Blog Post about Select control](https://textual.textualize.io/blog/2023/05/08/textual-0240-adds-a-select-control/).
+
 A simple select widget (aka dropdown) for [textual](https://github.com/Textualize/textual) with an optional search field.
 
 ![select_focus](https://user-images.githubusercontent.com/922559/209305346-6b8971b1-7a3a-4424-bdf8-c439b9d74e28.png)
 
 ![select_open](https://user-images.githubusercontent.com/922559/209305349-84f39432-b1e4-405e-8854-a8d7a33230ae.png)
 
 ![select_search](https://user-images.githubusercontent.com/922559/209305352-9ad2e7c1-9dc6-435f-b1bd-8dba5f5b2642.png)
```

