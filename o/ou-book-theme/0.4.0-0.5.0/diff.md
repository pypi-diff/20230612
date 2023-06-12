# Comparing `tmp/ou_book_theme-0.4.0.tar.gz` & `tmp/ou_book_theme-0.5.0.tar.gz`

## Comparing `ou_book_theme-0.4.0.tar` & `ou_book_theme-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0    10849 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/package-lock.json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/package.json
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/rollup.config.js
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/__about__.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/__init__.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/scripts/activity.js
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/scripts/external-link.js
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/scripts/index.js
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/styles/_activity.scss
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/styles/_external-link.scss
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/styles/_time.scss
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/styles/_variables.scss
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/styles/_where-next.scss
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/assets/styles/index.scss
--rw-r--r--   0        0        0    22428 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/cli/__init__.py
--rw-r--r--   0        0        0    40533 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/cli/mermaid-cli/package-lock.json
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/cli/mermaid-cli/package.json
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/extensions/__init__.py
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/extensions/activity.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/extensions/time.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/extensions/where_next.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/theme/ou_book_theme/theme.conf
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/theme/ou_book_theme/static/images/favicon.svg
--rw-r--r--   0        0        0    13489 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/theme/ou_book_theme/static/images/logo.svg
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/theme/ou_book_theme/static/scripts/ou-book-theme.js
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/ou_book_theme/theme/ou_book_theme/static/styles/ou-book-theme.css
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/.gitignore
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/README.md
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 ou_book_theme-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0    10849 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/package-lock.json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/package.json
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/rollup.config.js
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/__about__.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/__init__.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/scripts/activity.js
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/scripts/external-link.js
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/scripts/index.js
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/styles/_activity.scss
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/styles/_external-link.scss
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/styles/_time.scss
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/styles/_variables.scss
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/styles/_where-next.scss
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/assets/styles/index.scss
+-rw-r--r--   0        0        0    24010 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/cli/__init__.py
+-rw-r--r--   0        0        0    40533 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/cli/mermaid-cli/package-lock.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/cli/mermaid-cli/package.json
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/extensions/__init__.py
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/extensions/activity.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/extensions/time.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/extensions/where_next.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/theme.conf
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/static/images/favicon.svg
+-rw-r--r--   0        0        0    13489 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/static/images/logo.svg
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/static/scripts/ou-book-theme.js
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/static/styles/ou-book-theme.css
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/.gitignore
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/README.md
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 ou_book_theme-0.5.0/PKG-INFO
```

### Comparing `ou_book_theme-0.4.0/package-lock.json` & `ou_book_theme-0.5.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.4.0/rollup.config.js` & `ou_book_theme-0.5.0/rollup.config.js`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.4.0/ou_book_theme/__init__.py` & `ou_book_theme-0.5.0/ou_book_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.4.0/ou_book_theme/assets/styles/_activity.scss` & `ou_book_theme-0.5.0/ou_book_theme/assets/styles/_activity.scss`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.4.0/ou_book_theme/assets/styles/_where-next.scss` & `ou_book_theme-0.5.0/ou_book_theme/assets/styles/_where-next.scss`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.4.0/ou_book_theme/cli/__init__.py` & `ou_book_theme-0.5.0/ou_book_theme/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -351,22 +351,26 @@
         <UnknownTag><xsl:value-of select="name(.)"/></UnknownTag>
     </xsl:template>
 </xsl:stylesheet>''')
     transform = etree.XSLT(stylesheet)
     return transform(xpath_single(node, '/document/section')).getroot()
 
 
-def create_introduction(input_base: str, root: etree.Element, block: int, part: dict, chapter: dict) -> None:
+def create_introduction(input_base: str, root: etree.Element, chapter: dict) -> None:
     """Create the introduction structure."""
     with open(path.join(input_base, f'{chapter["file"]}.xml')) as in_f:
         doc = etree.parse(in_f)
-        root.append(transform_content(
+        introduction = transform_content(
             doc,
             root_node='Introduction'
-        ))
+        )
+        if 'sections' in chapter:
+            for section in chapter['sections']:
+                create_section(input_base, introduction, section)
+        root.append(introduction)
 
 
 def create_section(input_base: str, root: etree.Element, section: dict) -> None:
     """Create the structure for a single section, which writes to a single part file."""
     with open(path.join(input_base, f'{section["file"]}.xml')) as in_f:
         doc = etree.parse(in_f)
         section = transform_content(
@@ -386,24 +390,24 @@
         )
         if 'sections' in chapter:
             for section in chapter['sections']:
                 create_section(input_base, session, section)
         root.append(session)
 
 
-def create_unit(config: dict, root: etree.Element, part: dict, input_base: str, block: int) -> None:
+def create_unit(config: dict, root: etree.Element, part: dict, input_base: str, unit_id: str, unit_title: str) -> None:
     """Create a single unit."""
     unit = etree.Element('Unit')
     root.append(unit)
-    unit.append(create_text_node('UnitID', f'Block {block}: {config["ou"]["block_title"]}'))
-    unit.append(create_text_node('UnitTitle', f'{part["caption"]}: $PART_TITLE'))
+    unit.append(create_text_node('UnitID', unit_id))
+    unit.append(create_text_node('UnitTitle', unit_title))
     unit.append(create_text_node('ByLine', config['author']))
     for chapter_idx, chapter in enumerate(part['chapters']):
         if chapter_idx == 0:
-            create_introduction(input_base, unit, block, part, chapter)
+            create_introduction(input_base, unit, chapter)
         else:
             create_session(input_base, unit, chapter)
 
 
 def create_frontmatter(root: etree.Element, config: dict) -> None:
     """Create the frontmatter XML structure."""
     frontmatter = etree.XML(f'''\
@@ -448,37 +452,35 @@
     </Standard>
   </Imprint>
 </FrontMatter>
 ''')
     root.append(frontmatter)
 
 
-def create_root(config: dict, part_idx: int) -> etree.Element:
+def create_root(config: dict, file_id: str, title: str) -> etree.Element:
     """Create the root structure."""
     module_code = config['ou']['module_code']
     module_title = config['ou']['module_title']
-    block = int(config['ou']['block'])
-    presentation = config['ou']['presentation']
 
     root = etree.Element('Item')
     root.attrib['TextType'] = 'CompleteItem'
     root.attrib['SchemaVersion'] = '2.0'
-    root.attrib['id'] = f'X_{module_code.lower()}_b{block}_p{part_idx}_{presentation.lower()}'
+    root.attrib['id'] = file_id
     root.attrib['Template'] = 'Generic_A4_Unnumbered'
     root.attrib['Rendering'] = 'VLE2 staff (learn3)'
     root.attrib['DiscussionAlias'] = 'Comment'
     root.attrib['Autonumber'] = 'false'
     root.attrib['vleglossary'] = 'manual'
     meta = etree.Element('meta')
-    meta.attrib['content'] = f'{module_code} Block {block}, Part {part_idx}: $PART_TITLE'
+    meta.attrib['content'] = title
     root.append(meta)
     root.append(create_text_node('CourseCode', module_code))
     root.append(create_text_node('CourseTitle', module_title))
     root.append(etree.Element('ItemID'))
-    root.append(create_text_node('ItemTitle', f'Block {block}, Part {part_idx}: $PART_TITLE'))
+    root.append(create_text_node('ItemTitle', title))
 
     return root
 
 
 @app.command()
 def convert_to_ouxml(source: str, regenerate: bool=False, numbering_from: int=1):
     """Convert the content into OU XML."""
@@ -506,26 +508,62 @@
         with open(path.join(source, '_toc.yml')) as in_f:
             toc = safe_load(in_f)
         progress.update(clearing_task, completed=2)
         with open(path.join(source, '_config.yml')) as in_f:
             config = safe_load(in_f)
         progress.update(clearing_task, completed=3)
 
-        main_task = progress.add_task('Converting', total=len(toc['parts']))
-        module_code = config['ou']['module_code']
-        block = int(config['ou']['block'])
-        presentation = config['ou']['presentation']
-        for part_idx, part in enumerate(toc['parts']):
-            part_idx = numbering_from + part_idx
-            root = create_root(config, part_idx)
+        if 'parts' in toc:
+            main_task = progress.add_task('Converting', total=len(toc['parts']))
+            module_code = config['ou']['module_code']
+            block = int(config['ou']['block'])
+            presentation = config['ou']['presentation']
+            for part_idx, part in enumerate(toc['parts']):
+                part_idx = numbering_from + part_idx
+                root = create_root(
+                    config,
+                    f'X_{module_code.lower()}_b{block}_p{part_idx}_{presentation.lower()}',
+                    f'{module_code} Block {block}, Part {part_idx}: $PART_TITLE'
+                )
+                create_frontmatter(root, config)
+                create_unit(
+                    config,
+                    root,
+                    part,
+                    input_base,
+                    f'Block {block}: {config["ou"]["block_title"]}',
+                    f'{part["caption"]}: $PART_TITLE',
+                )
+                part_title = xpath_single(root, '/Item/Unit/Introduction/Title/text()')
+                apply_fixes(config, source, root, module_code, block, part_idx, presentation, {'session': 0, 'section': 0, 'figure': 0, 'table': 0}, part_title)
+                with open(path.join(output_base, f'{module_code.lower()}_b{block}_p{part_idx}_{presentation.lower()}.xml'), 'wb') as out_f:
+                    out_f.write(etree.tostring(root, pretty_print=True, encoding='utf-8', xml_declaration=True))
+                progress.update(main_task, advance=1)
+        else:
+            main_task = progress.add_task('Converting', total=1)
+            module_code = config['ou']['module_code']
+            block = config['ou']['block']
+            presentation = config['ou']['presentation']
+            root = create_root(
+                config,
+                f'X_{module_code.lower()}_{block.lower()}_{presentation.lower()}',
+                f'{module_code} {block}: $PART_TITLE'
+            )
             create_frontmatter(root, config)
-            create_unit(config, root, part, input_base, block)
+            create_unit(
+                config,
+                root,
+                toc,
+                input_base,
+                f'{block}: $PART_TITLE',
+                f'{module_code} {block}: $PART_TITLE'
+            )
             part_title = xpath_single(root, '/Item/Unit/Introduction/Title/text()')
-            apply_fixes(config, source, root, module_code, block, part_idx, presentation, {'session': 0, 'section': 0, 'figure': 0, 'table': 0}, part_title)
-            with open(path.join(output_base, f'{module_code.lower()}_b{block}_p{part_idx}_{presentation.lower()}.xml'), 'wb') as out_f:
+            apply_fixes(config, source, root, module_code, block, 0, presentation, {'session': 0, 'section': 0, 'figure': 0, 'table': 0}, part_title)
+            with open(path.join(output_base, f'{module_code.lower()}_{block.lower()}.xml'), 'wb') as out_f:
                 out_f.write(etree.tostring(root, pretty_print=True, encoding='utf-8', xml_declaration=True))
             progress.update(main_task, advance=1)
 
 
 @app.command()
 def version():
     """Print the current version."""
```

### Comparing `ou_book_theme-0.4.0/ou_book_theme/cli/mermaid-cli/package-lock.json` & `ou_book_theme-0.5.0/ou_book_theme/cli/mermaid-cli/package-lock.json`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.4.0/ou_book_theme/extensions/activity.py` & `ou_book_theme-0.5.0/ou_book_theme/extensions/activity.py`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.4.0/ou_book_theme/extensions/time.py` & `ou_book_theme-0.5.0/ou_book_theme/extensions/time.py`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.4.0/ou_book_theme/extensions/where_next.py` & `ou_book_theme-0.5.0/ou_book_theme/extensions/where_next.py`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.4.0/ou_book_theme/theme/ou_book_theme/static/images/favicon.svg` & `ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/static/images/favicon.svg`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.4.0/ou_book_theme/theme/ou_book_theme/static/images/logo.svg` & `ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.4.0/ou_book_theme/theme/ou_book_theme/static/scripts/ou-book-theme.js` & `ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/static/scripts/ou-book-theme.js`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.4.0/ou_book_theme/theme/ou_book_theme/static/styles/ou-book-theme.css` & `ou_book_theme-0.5.0/ou_book_theme/theme/ou_book_theme/static/styles/ou-book-theme.css`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.4.0/pyproject.toml` & `ou_book_theme-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ou_book_theme-0.4.0/PKG-INFO` & `ou_book_theme-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ou-book-theme
-Version: 0.4.0
+Version: 0.5.0
 Project-URL: Documentation, https://github.com/unknown/ou-book-theme#readme
 Project-URL: Issues, https://github.com/unknown/ou-book-theme/issues
 Project-URL: Source, https://github.com/unknown/ou-book-theme
 Author-email: Mark Hall <mark.hall@open.ac.uk>
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

