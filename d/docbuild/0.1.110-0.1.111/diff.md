# Comparing `tmp/docbuild-0.1.110.tar.gz` & `tmp/docbuild-0.1.111.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docbuild-0.1.110.tar", last modified: Wed May 17 08:35:29 2023, max compression
+gzip compressed data, was "docbuild-0.1.111.tar", last modified: Mon Jun 12 10:35:57 2023, max compression
```

## Comparing `docbuild-0.1.110.tar` & `docbuild-0.1.111.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-17 08:35:29.606260 docbuild-0.1.110/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-05-17 08:35:29.606097 docbuild-0.1.110/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.110/README.md
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-17 08:35:29.602373 docbuild-0.1.110/docbuild/
--rw-r--r--   0 moran      (501) staff       (20)       63 2023-05-17 08:35:03.000000 docbuild-0.1.110/docbuild/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      439 2023-04-20 11:04:19.000000 docbuild-0.1.110/docbuild/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     5392 2023-04-19 07:35:54.000000 docbuild-0.1.110/docbuild/graph.py
--rw-r--r--   0 moran      (501) staff       (20)     4478 2023-04-19 09:10:05.000000 docbuild-0.1.110/docbuild/hocr_parser.py
--rw-r--r--   0 moran      (501) staff       (20)     6911 2023-05-17 08:35:13.000000 docbuild-0.1.110/docbuild/page_creator.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-17 08:35:29.604707 docbuild-0.1.110/docbuild/paragraph_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.110/docbuild/paragraph_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.110/docbuild/paragraph_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     6831 2023-04-20 11:03:50.000000 docbuild-0.1.110/docbuild/paragraph_detection/paragraph_extractor.py
--rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.110/docbuild/paragraph_detection/paragraph_sorter.py
--rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.110/docbuild/paragraph_detection/two_columns.py
--rw-r--r--   0 moran      (501) staff       (20)     6087 2023-05-08 09:07:21.000000 docbuild-0.1.110/docbuild/textract_parser.py
--rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.110/docbuild/utils.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-17 08:35:29.605722 docbuild-0.1.110/docbuild/visual_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.110/docbuild/visual_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)    12923 2023-05-09 11:47:03.000000 docbuild-0.1.110/docbuild/visual_detection/bordered_table_extraction.py
--rw-r--r--   0 moran      (501) staff       (20)      218 2023-04-30 11:54:41.000000 docbuild-0.1.110/docbuild/visual_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)    16349 2023-05-11 14:30:30.000000 docbuild-0.1.110/docbuild/visual_detection/vis_line_detection.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-05-17 08:35:29.603377 docbuild-0.1.110/docbuild.egg-info/
--rw-r--r--   0 moran      (501) staff       (20)      566 2023-05-17 08:35:29.000000 docbuild-0.1.110/docbuild.egg-info/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)      741 2023-05-17 08:35:29.000000 docbuild-0.1.110/docbuild.egg-info/SOURCES.txt
--rw-r--r--   0 moran      (501) staff       (20)        1 2023-05-17 08:35:29.000000 docbuild-0.1.110/docbuild.egg-info/dependency_links.txt
--rw-r--r--   0 moran      (501) staff       (20)       97 2023-05-17 08:35:29.000000 docbuild-0.1.110/docbuild.egg-info/requires.txt
--rw-r--r--   0 moran      (501) staff       (20)        9 2023-05-17 08:35:29.000000 docbuild-0.1.110/docbuild.egg-info/top_level.txt
--rw-r--r--   0 moran      (501) staff       (20)       38 2023-05-17 08:35:29.606365 docbuild-0.1.110/setup.cfg
--rw-r--r--   0 moran      (501) staff       (20)      856 2023-05-17 08:34:58.000000 docbuild-0.1.110/setup.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-12 10:35:57.781215 docbuild-0.1.111/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-06-12 10:35:57.780849 docbuild-0.1.111/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)       81 2023-04-19 09:08:24.000000 docbuild-0.1.111/README.md
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-12 10:35:57.770877 docbuild-0.1.111/docbuild/
+-rw-r--r--   0 moran      (501) staff       (20)       63 2023-06-12 10:35:46.000000 docbuild-0.1.111/docbuild/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      438 2023-06-11 11:52:15.000000 docbuild-0.1.111/docbuild/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     6297 2023-06-11 16:15:35.000000 docbuild-0.1.111/docbuild/graph.py
+-rw-r--r--   0 moran      (501) staff       (20)     4479 2023-06-11 11:17:19.000000 docbuild-0.1.111/docbuild/hocr_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)     7417 2023-06-12 10:32:35.000000 docbuild-0.1.111/docbuild/page_creator.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-12 10:35:57.774225 docbuild-0.1.111/docbuild/paragraph_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:00:49.000000 docbuild-0.1.111/docbuild/paragraph_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      175 2023-04-19 06:33:46.000000 docbuild-0.1.111/docbuild/paragraph_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     6831 2023-06-08 11:20:02.000000 docbuild-0.1.111/docbuild/paragraph_detection/paragraph_extractor.py
+-rw-r--r--   0 moran      (501) staff       (20)     2416 2023-04-19 06:16:08.000000 docbuild-0.1.111/docbuild/paragraph_detection/paragraph_sorter.py
+-rw-r--r--   0 moran      (501) staff       (20)     2703 2023-04-19 06:00:43.000000 docbuild-0.1.111/docbuild/paragraph_detection/two_columns.py
+-rw-r--r--   0 moran      (501) staff       (20)     6062 2023-06-11 11:17:19.000000 docbuild-0.1.111/docbuild/textract_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)      816 2023-04-19 06:53:00.000000 docbuild-0.1.111/docbuild/utils.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-12 10:35:57.779859 docbuild-0.1.111/docbuild/visual_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-04-19 06:03:44.000000 docbuild-0.1.111/docbuild/visual_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)    16698 2023-06-11 16:15:54.000000 docbuild-0.1.111/docbuild/visual_detection/bordered_table_extraction.py
+-rw-r--r--   0 moran      (501) staff       (20)    23226 2023-06-11 16:15:35.000000 docbuild-0.1.111/docbuild/visual_detection/borderless_table_extraction.py
+-rw-r--r--   0 moran      (501) staff       (20)      257 2023-06-11 11:52:24.000000 docbuild-0.1.111/docbuild/visual_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)    16302 2023-06-11 16:15:35.000000 docbuild-0.1.111/docbuild/visual_detection/vis_line_detection.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-06-12 10:35:57.772315 docbuild-0.1.111/docbuild.egg-info/
+-rw-r--r--   0 moran      (501) staff       (20)      566 2023-06-12 10:35:57.000000 docbuild-0.1.111/docbuild.egg-info/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)      798 2023-06-12 10:35:57.000000 docbuild-0.1.111/docbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 moran      (501) staff       (20)        1 2023-06-12 10:35:57.000000 docbuild-0.1.111/docbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 moran      (501) staff       (20)       97 2023-06-12 10:35:57.000000 docbuild-0.1.111/docbuild.egg-info/requires.txt
+-rw-r--r--   0 moran      (501) staff       (20)        9 2023-06-12 10:35:57.000000 docbuild-0.1.111/docbuild.egg-info/top_level.txt
+-rw-r--r--   0 moran      (501) staff       (20)       38 2023-06-12 10:35:57.781273 docbuild-0.1.111/setup.cfg
+-rw-r--r--   0 moran      (501) staff       (20)      857 2023-06-12 10:35:51.000000 docbuild-0.1.111/setup.py
```

### Comparing `docbuild-0.1.110/PKG-INFO` & `docbuild-0.1.111/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.110
+Version: 0.1.111
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.110/docbuild/graph.py` & `docbuild-0.1.111/docbuild/graph.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from docstruct.text_block import Paragraph, TextBlock
+from typing import Callable
 
 
 class Node:
     def __init__(self, data: object):
         self.data: object = data
         self.neighbors: list[Node] = []
 
@@ -25,23 +26,19 @@
     ) -> list[list[Node]]:
         if nodes_order is None:
             nodes_order = self.nodes
         visited = set()
         connected_components: list[list[Node]] = []
         for node in nodes_order:
             if node not in visited:
-                connected_component = self.get_connected_component(
-                    node, visited
-                )
+                connected_component = self.get_connected_component(node, visited)
                 connected_components.append(connected_component)
         return connected_components
 
-    def get_connected_component(
-        self, node: Node, visited: set[Node]
-    ) -> list[Node]:
+    def get_connected_component(self, node: Node, visited: set[Node]) -> list[Node]:
         stack = [node]
         connected_component = []
         while stack:
             current = stack.pop()
             if current not in visited:
                 visited.add(current)
                 connected_component.append(current)
@@ -119,20 +116,16 @@
 
 
 class ParaGraph(Graph):
     def __init__(self, nodes: list[Node], paragraphs: list[Paragraph]):
         super(ParaGraph, self).__init__(nodes)
         self.paragraphs = paragraphs
         first_lines = [paragraph.get_children()[0] for paragraph in paragraphs]
-        pre_sort_paragraphs_indexes = TextBlock.sort(
-            first_lines, return_indexes=True
-        )
-        self.pre_sort = [
-            self.nodes[index] for index in pre_sort_paragraphs_indexes
-        ]
+        pre_sort_paragraphs_indexes = TextBlock.sort(first_lines, return_indexes=True)
+        self.pre_sort = [self.nodes[index] for index in pre_sort_paragraphs_indexes]
 
     def paragraph_sort(self) -> list[Node]:
         num_nodes = len(self.nodes)
         in_degree = [0 for _ in range(num_nodes)]
         for node in range(num_nodes):
             for neighbor in self.nodes[node].neighbors:
                 in_degree[neighbor.data] += 1
@@ -156,7 +149,33 @@
 
             if len(queue) == 0 and len(sorted_nodes) < num_nodes:
                 for node in self.pre_sort:
                     if node not in sorted_nodes:
                         queue.append(self.nodes[node.data])
                         break
         return [node.data for node in sorted_nodes]
+    
+
+
+class GraphGenerator:
+    def __init__(self, items: list[object], are_adjacent: Callable):
+        self.items = items
+        self.are_adjacent = are_adjacent
+
+    def generate_directed_graph(self) -> Graph:
+        nodes = [Node(i) for i in range(len(self.items))]
+        for i, item_i in enumerate(self.items):
+            for j, item_j in enumerate(self.items):
+                if self.are_adjacent(item_i, item_j):
+                    nodes[i].add_neighbor(nodes[j])
+        return Graph(nodes)
+
+    def generate_undirected_graph(self) -> Graph:
+        nodes = [Node(i) for i in range(len(self.items))]
+        for i in range(len(self.items)):
+            for j in range(i + 1, len(self.items)):
+                item_i = self.items[i]
+                item_j = self.items[j]
+                if self.are_adjacent(item_i, item_j):
+                    nodes[i].add_neighbor(nodes[j])
+                    nodes[j].add_neighbor(nodes[i])
+        return Graph(nodes)
```

### Comparing `docbuild-0.1.110/docbuild/hocr_parser.py` & `docbuild-0.1.111/docbuild/hocr_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from bs4 import BeautifulSoup, Tag
 from docstruct import BoundingBox, Line, Page, Paragraph, Word
 import re
 from .constants import BBOX_PATTERN
 import logging
 
+
 class HocrParser:
 
     """
     This class is used to parse hocr files into a page structure.
     """
 
     def __init__(self, hocr_file_path: str):
```

### Comparing `docbuild-0.1.110/docbuild/page_creator.py` & `docbuild-0.1.111/docbuild/page_creator.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 import cv2
 from docstruct import Page, TextBlock, Word, Line, Paragraph, Table
 
 from .textract_parser import TextractParser
 from .paragraph_detection.paragraph_extractor import ParagraphExtractor
 from .paragraph_detection.paragraph_sorter import sort_areas
 from .visual_detection.bordered_table_extraction import BorderedTableExtractor
+from .visual_detection.borderless_table_extraction import BorderlessTableExtractor
 from .visual_detection.vis_line_detection import VisLineDetector
 from .utils import get_average_character_height, get_average_character_width
 from .constants import SORT_LINE_VERTICAL_SCALE
 
+
 class PageCreator:
     def __init__(
         self,
         image_path: str,
         textract_response: dict = None,
         words: list[Word] = None,
         debug: bool = False,
@@ -73,21 +75,19 @@
             ]
             line.set_children(non_table_words)
             line.set_length()
             line.set_bounding_box()
             non_empty_lines.append(line)
         return non_empty_lines
 
-    def get_lines(
-        self, words: list[Word], space_threshold: float
-    ) -> list[Line]:
+    def get_lines(self, words: list[Word], space_threshold: float) -> list[Line]:
         """
         Parse the lines
         """
-        words = TextBlock.sort(words, height_scale = SORT_LINE_VERTICAL_SCALE)
+        words = TextBlock.sort(words, height_scale=SORT_LINE_VERTICAL_SCALE)
         group_words = []
         start = 0
 
         for i in range(len(words) - 1):
             current_x = words[i].bounding_box.get_right()
             next_x = words[i + 1].bounding_box.get_left()
             current_ver_seg = words[i].bounding_box.get_vertical_segment()
@@ -99,72 +99,74 @@
             group_words.append(words[start : i + 1])
             start = i + 1
         group_words.append(words[start:])
         return [Line(children=group) for group in group_words]
 
     def get_tables(self, words: list[Word]) -> list[Table]:
         try:
-            avg_word_size_ver = get_average_character_height(words) 
-            avg_word_size_hor = (
-                avg_word_size_ver * self.image_height / self.image_width
-            )
+            avg_word_size_ver = get_average_character_height(words)
+            avg_word_size_hor = avg_word_size_ver * self.image_height / self.image_width
             image_length_threshold = int(avg_word_size_ver * self.image_height)
-            
+
             ver_threshold = avg_word_size_ver
             hor_threshold = avg_word_size_hor
-            vis_line_detector = VisLineDetector(
-                image_path=self.image_path, words=words
-            )
+            vis_line_detector = VisLineDetector(image_path=self.image_path, words=words)
             hor_lines, ver_lines = vis_line_detector.detect_lines(
                 hor_threshold, ver_threshold, image_length_threshold
             )
-            
+
             table_detector = BorderedTableExtractor(
                 words,
                 hor_lines,
                 ver_lines,
                 hor_threshold,
                 ver_threshold,
             )
-
             tables = table_detector.detect_tables()
             return tables
         except Exception as e:
             logging.error(f"Error: {e}")
             return []
 
     def create_page(self) -> Page:
-
         if self.words is not None:
             words = self.words
             avg_char_width = get_average_character_width(words)
             lines = self.get_lines(words, space_threshold=3 * avg_char_width)
 
         else:
             parser = TextractParser(self.textract_response)
             lines = parser.parse_response()
-            lines = TextBlock.sort(lines, height_scale = SORT_LINE_VERTICAL_SCALE)
+            lines = TextBlock.sort(lines, height_scale=SORT_LINE_VERTICAL_SCALE)
             words = [word for line in lines for word in line.children]
         if not words:
-            return Page()
+            return Page(children=[], width=self.image_width, height=self.image_height)
         tables = self.get_tables(words)
+
+        table_words = list(itertools.chain(*(table.get_all(Word) for table in tables)))
+        lines = self.remove_table_words_from_lines(lines, set(table_words))
+
+        borderless_table_detector = BorderlessTableExtractor(
+            lines,
+            max_forced_lines=5,
+            remove_singles_at_bottom_rows=False,
+        )
+        borderless_tables = borderless_table_detector.extract_tables()
+        tables.extend(borderless_tables)
+
         table_words = list(
-            itertools.chain(*(table.get_all(Word) for table in tables))
+            itertools.chain(*(table.get_all(Word) for table in borderless_tables))
         )
         lines = self.remove_table_words_from_lines(lines, set(table_words))
-        lines_paragraphs = self.extract_paragraphs(
-            lines=lines, lines_segments=True
-        )
+        lines_paragraphs = self.extract_paragraphs(lines=lines, lines_segments=True)
         height_offset = self.space_distribution(lines_paragraphs)
-        paragraphs = self.extract_paragraphs(
-            lines=lines, height_offset=height_offset
-        )
+        paragraphs = self.extract_paragraphs(lines=lines, height_offset=height_offset)
         areas = paragraphs + tables
         areas = sort_areas(areas)
-        page = Page(children=areas)
+        page = Page(children=areas, width=self.image_width, height=self.image_height)
         page.set_bounding_box()
         page.set_length()
         return page
 
     @staticmethod
     def round_up(n: float, decimals: float = 0) -> float:
         multiplier = 10**decimals
```

### Comparing `docbuild-0.1.110/docbuild/paragraph_detection/paragraph_extractor.py` & `docbuild-0.1.111/docbuild/paragraph_detection/paragraph_extractor.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.110/docbuild/paragraph_detection/paragraph_sorter.py` & `docbuild-0.1.111/docbuild/paragraph_detection/paragraph_sorter.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.110/docbuild/paragraph_detection/two_columns.py` & `docbuild-0.1.111/docbuild/paragraph_detection/two_columns.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.110/docbuild/textract_parser.py` & `docbuild-0.1.111/docbuild/textract_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def __init__(self, textract_response: dict):
         self.textract_response = textract_response
         self.validate_args()
         self.words: list[dict] = []
         self.lines: list[dict] = []
         self.map_id_to_block_dict: dict[str, dict] = {}
         self.map_id_to_block_object: dict[str, TextBlock] = {}
-        
+
     def validate_args(self):
         """
         Validate the arguments
         """
         if not type(self.textract_response) == dict:
             raise ValueError("textract_response must be a dict")
 
@@ -53,53 +53,53 @@
 
     def get_non_space_slices(self, word: Word) -> list[slice]:
         space_indexes = [i for i, char in enumerate(word.text) if char.isspace()]
         space_indexes.insert(0, -1)
         space_indexes.append(len(word.text))
         non_space_slices = []
         for i in range(len(space_indexes) - 1):
-            if space_indexes[i+1] == space_indexes[i] + 1:
+            if space_indexes[i + 1] == space_indexes[i] + 1:
                 continue
-            current_slice = slice(space_indexes[i]+1, space_indexes[i+1])
+            current_slice = slice(space_indexes[i] + 1, space_indexes[i + 1])
             non_space_slices.append(current_slice)
 
         return non_space_slices
 
     def split_word_by_space(self, word: Word) -> list[Word]:
         """
         Split a word by space
         """
         non_space_slices = self.get_non_space_slices(word)
         characters = word.children
         splitted_words = []
         for slice in non_space_slices:
             current_chars = characters[slice]
-            current_bbox = BoundingBox.compose_bounding_boxes([char.bounding_box for char in current_chars])
+            current_bbox = BoundingBox.compose_bounding_boxes(
+                [char.bounding_box for char in current_chars]
+            )
             current_text = word.text[slice]
             current_word = Word(text=current_text, bounding_box=current_bbox)
             splitted_words.append(current_word)
         return splitted_words
 
     def get_line(self, block_dict: dict) -> Line:
         """
         Get a line object from a block dict
         """
         bb = self.get_bounding_box(block_dict)
-        line = Line(bounding_box=bb)
         children_id = self.get_children_id(block_dict)
         words = [self.map_id_to_block_object[child_id] for child_id in children_id]
         non_space_words = []
         for word in words:
             if self.to_split_word_by_space(word):
                 splitted_words = self.split_word_by_space(word)
-                non_space_words.extend(splitted_words)  
+                non_space_words.extend(splitted_words)
             else:
                 non_space_words.append(word)
-        
-        line.set_children(non_space_words)
+        line = Line(children=non_space_words)
         return line
 
     def word_is_printed(self, word_dict: dict) -> bool:
         """
         Check if a block dict is printed
         """
         return word_dict["TextType"] == "PRINTED"
@@ -170,8 +170,7 @@
         self.words, self.lines = self.split_blocks_by_type(self.textract_response)
         self.map_id_to_block_dict = self.get_map_id_to_block_dict(
             self.textract_response
         )
         self.map_id_to_block_object = self.parse_words(self.words)
         lines = self.parse_lines(self.lines)
         return lines
-
```

### Comparing `docbuild-0.1.110/docbuild/utils.py` & `docbuild-0.1.111/docbuild/utils.py`

 * *Files identical despite different names*

### Comparing `docbuild-0.1.110/docbuild/visual_detection/bordered_table_extraction.py` & `docbuild-0.1.111/docbuild/visual_detection/bordered_table_extraction.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 from typing import Optional
 import attr
 import numpy as np
 
-from docstruct import Word, TableCell, Table, BoundingBox, Segment, VisLine, VisLineOrientation
+from docstruct import (
+    Word,
+    Line,
+    TableCell,
+    TableColumn,
+    Table,
+    BoundingBox,
+    Segment,
+    VisLine,
+    VisLineOrientation,
+    TextBlock,
+    TableType,
+)
 from ..graph import Node, Graph, BipartiteGraph
-from .constants import GRID_COVER_RATIO_THRESHOLD, IS_GRID_THRESHOLD
+from .constants import (
+    GRID_COVER_RATIO_THRESHOLD,
+    IS_GRID_THRESHOLD,
+    BORDERED_TABLE_MAX_NUMBER_OF_LINES,
+)
 
 
 @attr.s(auto_attribs=True)
 class CellOfLines:
     left: VisLine
     right: VisLine
     top: VisLine
@@ -28,14 +44,32 @@
         # top to bottom
         self.hor_lines = sorted(hor_lines, key=lambda line: line.axis, reverse=True)
         # left to right
         self.ver_lines = sorted(ver_lines, key=lambda line: line.axis)
 
         self.hor_threshold = hor_threshold
         self.ver_threshold = ver_threshold
+        self.table_words = self.get_table_words(words, self.hor_lines, self.ver_lines)
+
+    def get_table_words(
+        self, words: list[Word], hor_lines: list[VisLine], ver_lines: list[VisLine]
+    ) -> list[Word]:
+        if len(hor_lines) <= 1 or len(ver_lines) <= 1:
+            return []
+        top = hor_lines[0].axis
+        bottom = hor_lines[-1].axis
+        left = ver_lines[0].axis
+        right = ver_lines[-1].axis
+        table_bbox = BoundingBox(left=left, top=top, right=right, bottom=bottom)
+        table_words = []
+        for word in words:
+            center = word.bounding_box.get_center()
+            if table_bbox.contains_point(center):
+                table_words.append(word)
+        return table_words
 
     def group_lines_by_axis(
         self, lines: list[VisLine], length_threshold: float
     ) -> list[list[VisLine]]:
         """Assuming the lines are sorted by axis"""
         if not lines:
             return []
@@ -92,15 +126,14 @@
             length_threshold=0,
         )
         return first_bb.intersect(second_bb)
 
     def filter_lines_by_cycles(
         self, hor_nodes: list[Node], ver_nodes: list[Node]
     ) -> tuple[list[Node], list[Node]]:
-
         filtered_hor_nodes = set()
         filtered_ver_nodes = set()
         for top in hor_nodes:
             for j, left in enumerate(top.neighbors):
                 for k in range(j + 1, len(top.neighbors)):
                     right = top.neighbors[k]
                     intersection_nodes = set(left.neighbors).intersection(
@@ -147,56 +180,68 @@
                 hor_cycle_lines, self.hor_threshold / 2
             )
             grouped_ver_lines = self.group_lines_by_axis(
                 ver_cycle_lines, self.ver_threshold / 2
             )
             if len(grouped_hor_lines) < 2 or len(grouped_ver_lines) < 2:
                 continue
-            table_grid = TableGrid(grouped_hor_lines, grouped_ver_lines)
+            table_grid = TableGrid(
+                grouped_hor_lines, grouped_ver_lines, self.table_words
+            )
 
             table: Table = table_grid.detect_table(
                 self.hor_lines, self.ver_lines, self.hor_threshold, self.ver_threshold
             )
             if table is None:
                 continue
-            table.group_words_into_cells(self.words)
             tables.append(table)
 
         return tables
 
 
 class TableGrid:
     def __init__(
         self,
         grouped_hor_lines: list[list[VisLine]],
         grouped_ver_lines: list[list[VisLine]],
+        words: list[Word],
     ):
         self.grouped_hor_lines = grouped_hor_lines
         self.grouped_ver_lines = grouped_ver_lines
-
+        self.words = words
         self.m = len(grouped_hor_lines) - 1
         self.n = len(grouped_ver_lines) - 1
 
         self.hor_lines_grid = np.zeros((self.m + 1, self.n), dtype=bool)
         self.ver_lines_grid = np.zeros((self.m, self.n + 1), dtype=bool)
 
         self.hor_axis_values = self.get_axis_values(self.grouped_hor_lines)
         self.ver_axis_values = self.get_axis_values(self.grouped_ver_lines)
+        pass
+
+    def filter_words_inside_cell(
+        self, table_words: list[Word], cell_bbox: BoundingBox
+    ) -> list[Word]:
+        cell_words = []
+        for word in table_words:
+            center = word.bounding_box.get_center()
+            if cell_bbox.contains_point(center):
+                cell_words.append(word)
+        return cell_words
 
     def get_axis_values(self, grouped_lines: list[list[VisLine]]) -> list[float]:
         axis_values = []
         for lines in grouped_lines:
             axis = VisLine.get_weighted_average_axis(lines)
             axis_values.append(axis)
         return axis_values
 
     def fill_lines_grid(
         self, axis_values, all_lines_grouped: list[list[VisLine]], is_hor: bool
-    ):  
-        
+    ):
         for k in range(len(all_lines_grouped)):
             segments = [
                 Segment(left=line.start, right=line.end)
                 for line in all_lines_grouped[k]
             ]
             for l in range(len(axis_values) - 1):
                 grid_segment = Segment(
@@ -257,14 +302,40 @@
                 for delta_x in (-1, 1):
                     if 0 <= j + delta_x < self.n:
                         neighbor_node = map_indexes_to_nodes[(i, j + delta_x)]
                         if not self.ver_lines_grid[i][j + delta_x]:
                             current_node.add_neighbor(neighbor_node)
         return graph
 
+    def compose_cell_words_to_lines(self, words: list[Word]) -> list[Line]:
+        sorted_words = TextBlock.sort(words)
+        lines_children = {}
+        for word in sorted_words:
+            parent = word.get_parent()
+            if parent not in lines_children:
+                lines_children[parent] = []
+            lines_children[parent].append(word)
+        lines = []
+        for line_children in lines_children.values():
+            line = Line(children=line_children)
+            line.set_bounding_box()
+            line.set_length()
+            lines.append(line)
+        return lines
+
+    def validate_number_of_lines_in_cells(self, cells: list[TableCell]) -> bool:
+        for cell in cells:
+            number_of_lines_condition = (
+                len(cell.children) > BORDERED_TABLE_MAX_NUMBER_OF_LINES
+            )
+            row_number_condition = cell.row_index > 0
+            if number_of_lines_condition and row_number_condition:
+                return False
+        return True
+
     def get_cells(self, graph: Graph) -> list[TableCell]:
         connected_components = graph.get_connected_components()
         cells = []
         for component in connected_components:
             indexes = [node.data for node in component]
             min_i, max_i = (
                 min(indexes, key=lambda x: x[0])[0],
@@ -277,16 +348,19 @@
             if (max_i - min_i + 1) * (max_j - min_j + 1) == len(component):
                 bounding_box = BoundingBox(
                     left=self.ver_axis_values[min_j],
                     right=self.ver_axis_values[max_j + 1],
                     top=self.hor_axis_values[min_i],
                     bottom=self.hor_axis_values[max_i + 1],
                 )
+                cell_words = self.filter_words_inside_cell(self.words, bounding_box)
+                cell_lines = self.compose_cell_words_to_lines(cell_words)
                 cell = TableCell(
                     bounding_box=bounding_box,
+                    children=cell_lines,
                     row_index=min_i,
                     col_index=min_j,
                     row_span=max_i - min_i + 1,
                     col_span=max_j - min_j + 1,
                 )
                 cells.append(cell)
             else:
@@ -294,50 +368,81 @@
                     i, j = node.data
                     bounding_box = BoundingBox(
                         left=self.ver_axis_values[j],
                         right=self.ver_axis_values[j + 1],
                         top=self.hor_axis_values[i],
                         bottom=self.hor_axis_values[i + 1],
                     )
+                    cell_words = self.filter_words_inside_cell(self.words, bounding_box)
+                    cell_lines = self.compose_cell_words_to_lines(cell_words)
                     cell = TableCell(
                         bounding_box=bounding_box,
+                        children=cell_lines,
                         row_index=i,
                         col_index=j,
                         row_span=1,
                         col_span=1,
                     )
                     cells.append(cell)
         return cells
-    
+
+    def get_columns(self, cells: list[TableCell]) -> list[TableColumn]:
+        num_columns = max(cell.col_index for cell in cells) + 1
+
+        columns: list[list[TableCell]] = [None] * num_columns
+
+        for cell in cells:
+            if columns[cell.col_index] is None:
+                columns[cell.col_index] = []
+            columns[cell.col_index].append(cell)
+        for column in columns:
+            if column is None:
+                continue
+            column.sort(key=lambda cell: cell.row_index)
+        return [
+            TableColumn(children=column) for column in columns if column is not None
+        ]
+
     @staticmethod
     def truth_ratio(matrix: np.ndarray) -> float:
         return np.count_nonzero(matrix) / matrix.size
-    
+
     def is_grid(self):
         hor_cover = TableGrid.truth_ratio(self.hor_lines_grid)
         ver_cover = TableGrid.truth_ratio(self.ver_lines_grid)
         return hor_cover > IS_GRID_THRESHOLD and ver_cover > IS_GRID_THRESHOLD
-    
+
+    def non_trivial_table(self, cells: list[TableCell]) -> bool:
+        if len(cells) <= 1:
+            return False
+        num_rows = max(cell.row_index + cell.row_span for cell in cells)
+        num_cols = max(cell.col_index + cell.col_span for cell in cells)
+        return num_rows > 1 and num_cols > 1
+
     def detect_table(
         self,
         all_hor_lines: list[VisLine],
         all_ver_lines: list[VisLine],
         hor_threshold: float,
         ver_threshold: float,
     ) -> Optional[Table]:
-
         all_hor_lines_grouped = self.group_lines_by_axis_values(
             self.hor_axis_values, all_hor_lines, hor_threshold
         )
         all_ver_lines_grouped = self.group_lines_by_axis_values(
             self.ver_axis_values, all_ver_lines, ver_threshold
         )
-        
+
         self.fill_lines_grid(self.ver_axis_values, all_hor_lines_grouped, is_hor=True)
         self.fill_lines_grid(self.hor_axis_values, all_ver_lines_grouped, is_hor=False)
         if not self.is_grid():
             return None
         graph = self.get_graph()
         cells = self.get_cells(graph)
-        if len(cells) <= 1:
+        if not self.validate_number_of_lines_in_cells(cells):
+            return None
+        if not self.non_trivial_table(cells):
             return None
-        return Table(cells=cells)
+        columns = self.get_columns(cells)
+
+        table = Table(children=columns)
+        return table
```

### Comparing `docbuild-0.1.110/docbuild/visual_detection/vis_line_detection.py` & `docbuild-0.1.111/docbuild/visual_detection/vis_line_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
                     line_word_pairs.add((line, word))
         intersecting_lines = set()
 
         for line, word in line_word_pairs:
             # if self.old_intersect(line, word):
             if line.intersect_bounding_box(
                 word.bounding_box.scale(width_scale=1, height_scale=0.9)
-                # word.bounding_box.scale(scale_x=1, scale_y=1)
+                
             ):
                 intersecting_lines.add(line)
         non_intersecting_lines = []
         for line in self.lines:
             if line not in intersecting_lines:
                 non_intersecting_lines.append(line)
         horizontal_lines = [line for line in non_intersecting_lines if line.is_hor()]
```

### Comparing `docbuild-0.1.110/docbuild.egg-info/PKG-INFO` & `docbuild-0.1.111/docbuild.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docbuild
-Version: 0.1.110
+Version: 0.1.111
 Summary: A package for building a document from a textract response, for more information see the docstruct package
 Home-page: https://github.com/smrt-co/docbuild
 Author: Moran Nechushtan, Serah Tapia, Shlomo Agishtein
 Author-email: moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `docbuild-0.1.110/docbuild.egg-info/SOURCES.txt` & `docbuild-0.1.111/docbuild.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,9 +15,10 @@
 docbuild/paragraph_detection/__init__.py
 docbuild/paragraph_detection/constants.py
 docbuild/paragraph_detection/paragraph_extractor.py
 docbuild/paragraph_detection/paragraph_sorter.py
 docbuild/paragraph_detection/two_columns.py
 docbuild/visual_detection/__init__.py
 docbuild/visual_detection/bordered_table_extraction.py
+docbuild/visual_detection/borderless_table_extraction.py
 docbuild/visual_detection/constants.py
 docbuild/visual_detection/vis_line_detection.py
```

### Comparing `docbuild-0.1.110/setup.py` & `docbuild-0.1.111/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name="docbuild",
-    version="0.1.110",
+    version="0.1.111",
     description="A package for building a document from a textract response, for more information see the docstruct package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Moran Nechushtan, Serah Tapia, Shlomo Agishtein",
     author_email="moran.n@trullion.com, serah@trullion.com, shlomo@trullion.com",
     url="https://github.com/smrt-co/docbuild",
     packages=setuptools.find_packages(),
     install_requires=[
         "attrs>=22.0.0",
         "numpy==1.23.2",
         "beautifulsoup4>=4.11.1",
         "opencv-contrib-python==4.6.0.66",
-        "python-dotenv"
+        "python-dotenv",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
 )
```

