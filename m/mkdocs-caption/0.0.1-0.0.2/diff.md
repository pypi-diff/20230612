# Comparing `tmp/mkdocs_caption-0.0.1.tar.gz` & `tmp/mkdocs_caption-0.0.2.tar.gz`

## Comparing `mkdocs_caption-0.0.1.tar` & `mkdocs_caption-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.1/src/mkdocs_caption/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.1/src/mkdocs_caption/_version.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.1/src/mkdocs_caption/config.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.1/src/mkdocs_caption/custom.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.1/src/mkdocs_caption/helper.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.1/src/mkdocs_caption/image.py
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.1/src/mkdocs_caption/plugin.py
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.1/src/mkdocs_caption/table.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.1/LICENSE
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.1/README.md
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     8537 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/src/mkdocs_caption/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/src/mkdocs_caption/_version.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/src/mkdocs_caption/config.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/src/mkdocs_caption/custom.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/src/mkdocs_caption/helper.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/src/mkdocs_caption/image.py
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/src/mkdocs_caption/plugin.py
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/src/mkdocs_caption/table.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/LICENSE
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/README.md
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8537 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.2/PKG-INFO
```

### Comparing `mkdocs_caption-0.0.1/src/mkdocs_caption/config.py` & `mkdocs_caption-0.0.2/src/mkdocs_caption/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_caption-0.0.1/src/mkdocs_caption/custom.py` & `mkdocs_caption-0.0.2/src/mkdocs_caption/custom.py`

 * *Files 13% similar despite different names*

```diff
@@ -55,18 +55,20 @@
     figure_element = etree.Element("figure", None, None)
     figure_element.attrib.update(caption_element.attrib)
     # wrap target element
     target_element.addprevious(figure_element)
     figure_element.insert(0, target_element)
 
     # add caption
-    fig_caption_element = etree.Element("figcaption", None, None)
-    fig_caption_element.text = (
-        f"{config.caption_prefix.format(identifier = identifier, index = index)} {caption_element.text}"
-    )
+    caption_prefix = config.caption_prefix.format(identifier=identifier, index=index)
+    try:
+        fig_caption_element = etree.fromstring(f"<figcaption>{caption_prefix} {caption_element.text}</figcaption>")
+    except etree.XMLSyntaxError as e:
+        e.msg = f"Invalid XML in caption: {caption_element.text}"
+        raise e
     figure_element.append(fig_caption_element)
 
     figure_id = caption_element.attrib.get("id", config.identifier.format(identifier=identifier, index=index))
     figure_element.attrib["id"] = figure_id
     update_references(tree, figure_id, config.reference_text.format(identifier=identifier, index=index))
     a_wrapper.remove(caption_element)
     parent = a_wrapper.getparent()
```

### Comparing `mkdocs_caption-0.0.1/src/mkdocs_caption/helper.py` & `mkdocs_caption-0.0.2/src/mkdocs_caption/helper.py`

 * *Files identical despite different names*

### Comparing `mkdocs_caption-0.0.1/src/mkdocs_caption/image.py` & `mkdocs_caption-0.0.2/src/mkdocs_caption/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,15 +47,18 @@
     index = config.start_index
     for img_element in tree.xpath("//p/a/img|//p/img"):
         title = img_element.get("title", img_element.get("alt", None))
         custom_id = img_element.get("id", config.identifier.format(index=index, identifier="figure"))
         update_references(
             tree,
             custom_id,
-            config.reference_text.format(index=index, identifier="figure"),
+            config.reference_text.format(index=index, identifier="Figure"),
         )
-        if title is not None:
-            caption_element = etree.Element("figcaption", None, None)
+        if title:
             caption_prefix = config.caption_prefix.format(index=index, identifier="Figure")
-            caption_element.text = f"{caption_prefix} {title}"
+            try:
+                caption_element = etree.fromstring(f"<figcaption>{caption_prefix} {title}</figcaption>")
+            except etree.XMLSyntaxError as e:
+                e.msg = f"Invalid XML in caption: {title}"
+                raise e
             wrap_image(img_element, custom_id, caption_element, config.position)
             index += config.increment_index
```

### Comparing `mkdocs_caption-0.0.1/src/mkdocs_caption/plugin.py` & `mkdocs_caption-0.0.2/src/mkdocs_caption/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_caption-0.0.1/src/mkdocs_caption/table.py` & `mkdocs_caption-0.0.2/src/mkdocs_caption/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,27 +60,29 @@
 
     Args:
         tree: The root element of the XML tree.
         table_element: The table element to add the caption to.
         caption_element: The caption element to use for the caption text.
         index: The index of the table element.
     """
-    table_caption_element = etree.Element("caption", None, None)
-    table_caption_element.text = (
-        f"{config.caption_prefix.format(index=index, identifier='Table')} {caption_element.text}"
-    )
+    caption_prefix = config.caption_prefix.format(index=index, identifier="Table")
+    try:
+        table_caption_element = etree.fromstring(f"<caption>{caption_prefix} {caption_element.text}</caption>")
+    except etree.XMLSyntaxError as e:
+        e.msg = f"Invalid XML in caption: {caption_element.text}"
+        raise e
     table_element.insert(0, table_caption_element)
 
     if "cols" in caption_element.attrib:
         table_element.insert(0, _create_colgroups(caption_element.attrib["cols"]))
         caption_element.attrib.pop("cols")
     table_element.attrib.update(caption_element.attrib)
     table_id = table_element.attrib.get("id", config.identifier.format(index=index, identifier="table"))
     table_element.attrib["id"] = table_id
-    update_references(tree, table_id, config.reference_text.format(index=index, identifier="table"))
+    update_references(tree, table_id, config.reference_text.format(index=index, identifier="Table"))
 
 
 def postprocess_html(tree: etree._Element, config: IdentifierCaption) -> None:
     """Handle custom captions in an XML tree.
 
     This function takes an XML tree and replaces all custom captions in the tree
     with custom HTML tags.
```

### Comparing `mkdocs_caption-0.0.1/LICENSE` & `mkdocs_caption-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_caption-0.0.1/README.md` & `mkdocs_caption-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_caption-0.0.1/pyproject.toml` & `mkdocs_caption-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mkdocs_caption-0.0.1/PKG-INFO` & `mkdocs_caption-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-caption
-Version: 0.0.1
+Version: 0.0.2
 Project-URL: Documentation, https://github.com/tobiasah/mkdocs-caption#readme
 Project-URL: Issues, https://github.com/tobiasah/mkdocs-caption/issues
 Project-URL: Source, https://github.com/tobiasah/mkdocs-caption
 Author-email: Tobias Ahrens <tobias.ahrens@posteo.de>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-caption Version: 0.0.1 Project-URL:
+Metadata-Version: 2.1 Name: mkdocs-caption Version: 0.0.2 Project-URL:
 Documentation, https://github.com/tobiasah/mkdocs-caption#readme Project-URL:
 Issues, https://github.com/tobiasah/mkdocs-caption/issues Project-URL: Source,
 https://github.com/tobiasah/mkdocs-caption Author-email: Tobias Ahrens
 ahrens@posteo.de> License-Expression: MIT License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

