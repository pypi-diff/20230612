# Comparing `tmp/marko-1.3.1.tar.gz` & `tmp/marko-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marko-1.3.1.tar", last modified: Fri Jun  9 08:55:13 2023, max compression
+gzip compressed data, was "marko-2.0.0.tar", last modified: Mon Jun 12 03:58:36 2023, max compression
```

## Comparing `marko-1.3.1.tar` & `marko-2.0.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0     1067 2023-06-09 08:55:03.195424 marko-1.3.1/LICENSE
--rw-r--r--   0        0        0     3505 2023-06-09 08:55:03.195424 marko-1.3.1/README.md
--rw-r--r--   0        0        0     5127 2023-06-09 08:55:03.195424 marko-1.3.1/marko/__init__.py
--rw-r--r--   0        0        0      333 2023-06-09 08:55:03.195424 marko-1.3.1/marko/__main__.py
--rw-r--r--   0        0        0     3805 2023-06-09 08:55:03.195424 marko-1.3.1/marko/ast_renderer.py
--rw-r--r--   0        0        0    20405 2023-06-09 08:55:03.195424 marko-1.3.1/marko/block.py
--rw-r--r--   0        0        0     2500 2023-06-09 08:55:03.199424 marko-1.3.1/marko/cli.py
--rw-r--r--   0        0        0      793 2023-06-09 08:55:03.199424 marko-1.3.1/marko/element.py
--rw-r--r--   0        0        0      105 2023-06-09 08:55:03.199424 marko-1.3.1/marko/ext/__init__.py
--rw-r--r--   0        0        0     1832 2023-06-09 08:55:03.199424 marko-1.3.1/marko/ext/codehilite.py
--rw-r--r--   0        0        0     3159 2023-06-09 08:55:03.199424 marko-1.3.1/marko/ext/footnote.py
--rw-r--r--   0        0        0     2758 2023-06-09 08:55:03.199424 marko-1.3.1/marko/ext/gfm/__init__.py
--rw-r--r--   0        0        0     7120 2023-06-09 08:55:03.199424 marko-1.3.1/marko/ext/gfm/elements.py
--rw-r--r--   0        0        0     5132 2023-06-09 08:55:03.199424 marko-1.3.1/marko/ext/latex_renderer.py
--rw-r--r--   0        0        0      988 2023-06-09 08:55:03.199424 marko-1.3.1/marko/ext/pangu.py
--rw-r--r--   0        0        0     2544 2023-06-09 08:55:03.199424 marko-1.3.1/marko/ext/toc.py
--rw-r--r--   0        0        0     7670 2023-06-09 08:55:03.199424 marko-1.3.1/marko/helpers.py
--rw-r--r--   0        0        0     5029 2023-06-09 08:55:03.199424 marko-1.3.1/marko/html_renderer.py
--rw-r--r--   0        0        0     5542 2023-06-09 08:55:03.199424 marko-1.3.1/marko/inline.py
--rw-r--r--   0        0        0    17695 2023-06-09 08:55:03.199424 marko-1.3.1/marko/inline_parser.py
--rw-r--r--   0        0        0     5669 2023-06-09 08:55:03.199424 marko-1.3.1/marko/md_renderer.py
--rw-r--r--   0        0        0     4562 2023-06-09 08:55:03.199424 marko-1.3.1/marko/parser.py
--rw-r--r--   0        0        0     3308 2023-06-09 08:55:03.199424 marko-1.3.1/marko/patterns.py
--rw-r--r--   0        0        0        0 2023-06-09 08:55:03.199424 marko-1.3.1/marko/py.typed
--rw-r--r--   0        0        0     3392 2023-06-09 08:55:03.199424 marko-1.3.1/marko/renderer.py
--rw-r--r--   0        0        0     1367 2023-06-09 08:55:03.199424 marko-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1844 2023-06-09 08:55:03.199424 marko-1.3.1/tests/__init__.py
--rw-r--r--   0        0        0     2175 2023-06-09 08:55:03.199424 marko-1.3.1/tests/benchmark.py
--rw-r--r--   0        0        0     6879 2023-06-09 08:55:03.199424 marko-1.3.1/tests/normalize.py
--rw-r--r--   0        0        0    13117 2023-06-09 08:55:03.199424 marko-1.3.1/tests/samples/jquery.md
--rw-r--r--   0        0        0     2566 2023-06-09 08:55:03.199424 marko-1.3.1/tests/samples/syntax.md
--rw-r--r--   0        0        0   204971 2023-06-09 08:55:03.203425 marko-1.3.1/tests/spec/commonmark.txt
--rw-r--r--   0        0        0   216867 2023-06-09 08:55:03.203425 marko-1.3.1/tests/spec/gfm.txt
--rw-r--r--   0        0        0      483 2023-06-09 08:55:03.199424 marko-1.3.1/tests/spec.sh
--rw-r--r--   0        0        0     4280 2023-06-09 08:55:03.203425 marko-1.3.1/tests/test_basic.py
--rw-r--r--   0        0        0     3371 2023-06-09 08:55:03.203425 marko-1.3.1/tests/test_ext.py
--rw-r--r--   0        0        0     1745 2023-06-09 08:55:03.203425 marko-1.3.1/tests/test_helpers.py
--rw-r--r--   0        0        0     7590 2023-06-09 08:55:03.203425 marko-1.3.1/tests/test_latex.py
--rw-r--r--   0        0        0     2619 2023-06-09 08:55:03.203425 marko-1.3.1/tests/test_spec.py
--rw-r--r--   0        0        0     4343 1970-01-01 00:00:00.000000 marko-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-12 03:58:28.651901 marko-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3474 2023-06-12 03:58:28.651901 marko-2.0.0/README.md
+-rw-r--r--   0        0        0     5334 2023-06-12 03:58:28.651901 marko-2.0.0/marko/__init__.py
+-rw-r--r--   0        0        0      333 2023-06-12 03:58:28.651901 marko-2.0.0/marko/__main__.py
+-rw-r--r--   0        0        0     3857 2023-06-12 03:58:28.651901 marko-2.0.0/marko/ast_renderer.py
+-rw-r--r--   0        0        0    20818 2023-06-12 03:58:28.651901 marko-2.0.0/marko/block.py
+-rw-r--r--   0        0        0     2500 2023-06-12 03:58:28.651901 marko-2.0.0/marko/cli.py
+-rw-r--r--   0        0        0      793 2023-06-12 03:58:28.651901 marko-2.0.0/marko/element.py
+-rw-r--r--   0        0        0      105 2023-06-12 03:58:28.651901 marko-2.0.0/marko/ext/__init__.py
+-rw-r--r--   0        0        0     1803 2023-06-12 03:58:28.651901 marko-2.0.0/marko/ext/codehilite.py
+-rw-r--r--   0        0        0     3220 2023-06-12 03:58:28.651901 marko-2.0.0/marko/ext/footnote.py
+-rw-r--r--   0        0        0     2807 2023-06-12 03:58:28.651901 marko-2.0.0/marko/ext/gfm/__init__.py
+-rw-r--r--   0        0        0     7117 2023-06-12 03:58:28.651901 marko-2.0.0/marko/ext/gfm/elements.py
+-rw-r--r--   0        0        0     5372 2023-06-12 03:58:28.651901 marko-2.0.0/marko/ext/latex_renderer.py
+-rw-r--r--   0        0        0     1017 2023-06-12 03:58:28.651901 marko-2.0.0/marko/ext/pangu.py
+-rw-r--r--   0        0        0     2470 2023-06-12 03:58:28.651901 marko-2.0.0/marko/ext/toc.py
+-rw-r--r--   0        0        0     3543 2023-06-12 03:58:28.651901 marko-2.0.0/marko/helpers.py
+-rw-r--r--   0        0        0     4980 2023-06-12 03:58:28.651901 marko-2.0.0/marko/html_renderer.py
+-rw-r--r--   0        0        0     5048 2023-06-12 03:58:28.651901 marko-2.0.0/marko/inline.py
+-rw-r--r--   0        0        0    18303 2023-06-12 03:58:28.651901 marko-2.0.0/marko/inline_parser.py
+-rw-r--r--   0        0        0     5695 2023-06-12 03:58:28.651901 marko-2.0.0/marko/md_renderer.py
+-rw-r--r--   0        0        0     5090 2023-06-12 03:58:28.651901 marko-2.0.0/marko/parser.py
+-rw-r--r--   0        0        0     3308 2023-06-12 03:58:28.651901 marko-2.0.0/marko/patterns.py
+-rw-r--r--   0        0        0        0 2023-06-12 03:58:28.651901 marko-2.0.0/marko/py.typed
+-rw-r--r--   0        0        0     3374 2023-06-12 03:58:28.651901 marko-2.0.0/marko/renderer.py
+-rw-r--r--   0        0        0     5030 2023-06-12 03:58:28.651901 marko-2.0.0/marko/source.py
+-rw-r--r--   0        0        0     1601 2023-06-12 03:58:36.951881 marko-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1844 2023-06-12 03:58:28.655901 marko-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     2175 2023-06-12 03:58:28.655901 marko-2.0.0/tests/benchmark.py
+-rw-r--r--   0        0        0     6879 2023-06-12 03:58:28.655901 marko-2.0.0/tests/normalize.py
+-rw-r--r--   0        0        0    13117 2023-06-12 03:58:28.655901 marko-2.0.0/tests/samples/jquery.md
+-rw-r--r--   0        0        0     2566 2023-06-12 03:58:28.655901 marko-2.0.0/tests/samples/syntax.md
+-rw-r--r--   0        0        0      483 2023-06-12 03:58:28.655901 marko-2.0.0/tests/spec.sh
+-rw-r--r--   0        0        0   204971 2023-06-12 03:58:28.655901 marko-2.0.0/tests/spec/commonmark.txt
+-rw-r--r--   0        0        0   216867 2023-06-12 03:58:28.655901 marko-2.0.0/tests/spec/gfm.txt
+-rw-r--r--   0        0        0     4325 2023-06-12 03:58:28.655901 marko-2.0.0/tests/test_basic.py
+-rw-r--r--   0        0        0     3397 2023-06-12 03:58:28.655901 marko-2.0.0/tests/test_ext.py
+-rw-r--r--   0        0        0     1770 2023-06-12 03:58:28.655901 marko-2.0.0/tests/test_helpers.py
+-rw-r--r--   0        0        0     7590 2023-06-12 03:58:28.655901 marko-2.0.0/tests/test_latex.py
+-rw-r--r--   0        0        0     2619 2023-06-12 03:58:28.655901 marko-2.0.0/tests/test_spec.py
+-rw-r--r--   0        0        0     4450 1970-01-01 00:00:00.000000 marko-2.0.0/PKG-INFO
```

### Comparing `marko-1.3.1/LICENSE` & `marko-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marko-1.3.1/README.md` & `marko-2.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -7,26 +7,23 @@
 [![Documentation Status](https://img.shields.io/readthedocs/marko-py.svg?logo=readthedocs)](https://marko-py.readthedocs.io/en/latest/?badge=latest)
 [![CommonMark Spec](https://img.shields.io/badge/CommonMark-0.30-blue.svg)][spec]
 
 ![Build Status](https://github.com/frostming/marko/workflows/Tests/badge.svg)
 [![codecov](https://codecov.io/gh/frostming/marko/branch/master/graph/badge.svg)](https://codecov.io/gh/frostming/marko)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/b785f5b3fa7c4d93a02372d31b3f73b1)](https://www.codacy.com/app/frostming/marko?utm_source=github.com&utm_medium=referral&utm_content=frostming/marko&utm_campaign=Badge_Grade)
 
-Marko is a markdown parser written in pure Python that complies with [CommonMark's spec v0.30][spec].
-It is designed to be highly extensible, see [Extensions](#extensions) for details.
+Marko is a pure Python markdown parser that adheres to the specifications of [CommonMark's spec v0.30][spec]. It has been designed with high extensibility in mind, as detailed in the [Extensions](#extensions) section.
 
 Marko requires Python 3.7 or higher.
 
 ## Why Marko
 
-Among all implementations of Python's markdown parser, it is a common issue that user can't easily extend it to add his own features. Furthermore, [Python-Markdown][pymd] and [mistune][mistune] don't comply with CommonMark's spec. It is a good reason for me to develop a new markdown parser.
+Of all the Python markdown parsers available, a common issue is the difficulty for users to add their own features. Additionally, both [Python-Markdown][pymd] and [mistune][mistune] do not comply with CommonMark specifications. This has prompted me to develop a new markdown parser.
 
-Respecting that Marko complies with CommonMark's spec at the same time, which is a super complicated spec, Marko's performance will be affected. However, using a parser
-which doesn't comply with the CommonMark spec may give you unexpected rendered results from time to time.
-A benchmark result shows that Marko is 3 times slower than [Python-Markdown][pymd], but a bit faster than [Commonmark-py][cmpy], much slower than [mistune][mistune]. If performance is a bigger concern to you than spec compliance, you'd better choose another parser.
+Marko's compliance with the complex CommonMark specification can impact its performance. However, using a parser that does not adhere to this spec may result in unexpected rendering outcomes. According to benchmark results, Marko is three times slower than Python-Markdown but slightly faster than Commonmark-py and significantly slower than mistune. If prioritizing performance over spec compliance is crucial for you, it would be best to opt for another parser.
 
 [spec]: https://spec.commonmark.org/0.30/
 [pymd]: https://github.com/waylan/Python-Markdown
 [mistune]: https://github.com/lepture/mistune
 [cmpy]: https://github.com/rtfd/CommonMark-py
 
 ## Use Marko
@@ -49,21 +46,21 @@
 
 ## Extensions
 
 It is super easy to use an extension:
 
 ```python
 from marko import Markdown
-from marko.ext.footnote import Footnote
+from marko.ext.footnote import make_extension
 # Add footnote extension
-markdown = Markdown(extensions=[Footnote])
+markdown = Markdown(extensions=[make_extension()])
 # Or you can just:
 markdown = Markdown(extensions=['footnote'])
 # Alternatively you can register an extension later
-markdown.use(Footnote)
+markdown.use(make_extension())
 ```
 
 An example of using an extension with the command-line version of Marko:
 
 ```
 $ cat this_has_footnote.txt | marko -e footnote > hi_world.html
 ```
```

### Comparing `marko-1.3.1/marko/__init__.py` & `marko-2.0.0/marko/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,49 +9,52 @@
  Licensed under MIT.
  Created by Frost Ming<mianghong@gmail.com>
 """
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Iterable, cast
 
-from .helpers import load_extension
+from .helpers import MarkoExtension, load_extension
 from .html_renderer import HTMLRenderer
 from .parser import Parser
 from .renderer import Renderer
 
 if TYPE_CHECKING:
     from .block import Document
     from .parser import ElementType
 
-__version__ = "1.3.1"
+__version__ = "2.0.0"
 
 
 class SetupDone(Exception):
     def __str__(self) -> str:
         return "Unable to register more extensions after setup done."
 
 
 class Markdown:
     """The main class to convert markdown documents.
 
     Attributes:
         * parser: an instance of :class:`marko.parser.Parser`
         * renderer: an instance of :class:`marko.renderer.Renderer`
 
-    :param parser: a subclass :class:`marko.parser.Parser`.
-    :param renderer: a subclass :class:`marko.renderer.Renderer`.
+    :param parser: a subclass of :class:`marko.parser.Parser`.
+    :param renderer: a subclass of :class:`marko.renderer.Renderer`.
     :param extensions: a list of extensions to register on the object.
         See document of :meth:`Markdown.use()`.
+
+    .. note::
+        This class is not thread-safe. Create a new instance for each thread.
     """
 
     def __init__(
         self,
         parser: type[Parser] = Parser,
         renderer: type[Renderer] = HTMLRenderer,
-        extensions: Iterable[str | object] | None = None,
+        extensions: Iterable[str | MarkoExtension] | None = None,
     ) -> None:
         if not issubclass(parser, Parser):
             raise TypeError("parser must be a subclass of Parser.")
         self._base_parser = parser
         self._parser_mixins: list[type] = []
 
         if not issubclass(renderer, Renderer):
@@ -60,57 +63,55 @@
         self._renderer_mixins: list[type] = []
 
         self._extra_elements: list[ElementType] = []
         self._setup_done = False
         if extensions:
             self.use(*extensions)
 
-    def use(self, *extensions: str | object) -> None:
+    def use(self, *extensions: str | MarkoExtension) -> None:
         r"""Register extensions to Markdown object.
         An extension should be either an object providing ``elements``, `parser_mixins``
         , ``renderer_mixins`` or all attributes, or a string representing the
         corresponding extension in ``marko.ext`` module.
 
-        :param \*extensions: extension object or string.
+        :param \*extensions: string or :class:`marko.helpers.MarkoExtension` object.
 
         .. note:: Marko uses a mixin based extension system, the order of extensions
             matters: An extension preceding in order will have higher priorty.
         """
         if self._setup_done:
             raise SetupDone()
         for extension in extensions:
             if isinstance(extension, str):
                 extension = load_extension(extension)
 
-            self._parser_mixins = (
-                cast("list[type]", getattr(extension, "parser_mixins", []))
-                + self._parser_mixins
-            )
-            self._renderer_mixins = (
-                cast("list[type]", getattr(extension, "renderer_mixins", []))
-                + self._renderer_mixins
-            )
-            self._extra_elements.extend(
-                cast("list[ElementType]", getattr(extension, "elements", []))
-            )
+            self._parser_mixins = extension.parser_mixins + self._parser_mixins
+            self._renderer_mixins = extension.renderer_mixins + self._renderer_mixins
+            self._extra_elements.extend(extension.elements)
 
     def _setup_extensions(self) -> None:
         """Install all extensions and set things up."""
         if self._setup_done:
             return
-        self.parser: Parser = type(
-            "MarkdownParser", tuple(self._parser_mixins) + (self._base_parser,), {}
-        )()
+        self.parser = cast(
+            Parser,
+            type(
+                "MarkdownParser", tuple(self._parser_mixins) + (self._base_parser,), {}
+            )(),
+        )
         for e in self._extra_elements:
             self.parser.add_element(e)
-        self.renderer: Renderer = type(
-            "MarkdownRenderer",
-            tuple(self._renderer_mixins) + (self._base_renderer,),
-            {},
-        )()
+        self.renderer = cast(
+            Renderer,
+            type(
+                "MarkdownRenderer",
+                tuple(self._renderer_mixins) + (self._base_renderer,),
+                {},
+            )(),
+        )
         self._setup_done = True
 
     def convert(self, text: str) -> str:
         """Parse and render the given text."""
         return self.render(self.parse(text))
 
     def __call__(self, text: str) -> str:
@@ -118,21 +119,22 @@
 
     def parse(self, text: str) -> Document:
         """Call ``self.parser.parse(text)``.
 
         Override this to preprocess text or handle parsed result.
         """
         self._setup_extensions()
-        return cast("Document", self.parser.parse(text))
+        return self.parser.parse(text)
 
     def render(self, parsed: Document) -> str:
         """Call ``self.renderer.render(text)``.
 
         Override this to handle parsed result.
         """
+        self._setup_extensions()
         self.renderer.root_node = parsed
         with self.renderer as r:
             return r.render(parsed)
 
 
 # Inner instance, use the bare convert/parse/render function instead
 _markdown = Markdown()
@@ -159,7 +161,20 @@
 def render(parsed: Document) -> str:
     """Render the parsed object to text.
 
     :param parsed: the parsed object
     :returns: the rendered result.
     """
     return _markdown.render(parsed)
+
+
+__all__ = [
+    "MarkoExtension",
+    "Markdown",
+    "convert",
+    "parse",
+    "render",
+    "load_extension",
+    "Parser",
+    "Renderer",
+    "HTMLRenderer",
+]
```

### Comparing `marko-1.3.1/marko/ast_renderer.py` & `marko-2.0.0/marko/ast_renderer.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,26 +99,27 @@
             lines.append(" " * self.indent + '<?xml version="1.0" encoding="UTF-8"?>')
             lines.append(
                 " " * self.indent + '<!DOCTYPE document SYSTEM "CommonMark.dtd">'
             )
         attrs = {
             k: v
             for k, v in element.__dict__.items()
-            if not k.startswith("_") and k != "children"
+            if not k.startswith("_") and k not in ("body", "children")
         }
         attr_str = "".join(f' {k}="{v}"' for k, v in attrs.items())
         element_name = camel_to_snake_case(element.__class__.__name__)
         lines.append(" " * self.indent + f"<{element_name}{attr_str}>")
-        if getattr(element, "children", None):
+        children = getattr(element, "body", None) or getattr(element, "children", None)
+        if children:
             self.indent += 2
-            if isinstance(element.children, str):  # type: ignore
+            if isinstance(children, str):  # type: ignore
                 lines.append(
                     " " * self.indent
-                    + HTMLRenderer.escape_html(json.dumps(element.children)[1:-1])  # type: ignore
+                    + HTMLRenderer.escape_html(json.dumps(children)[1:-1])  # type: ignore
                 )
             else:
-                lines.extend(self.render(child) for child in element.children)  # type: ignore
+                lines.extend(self.render(child) for child in children)  # type: ignore
             self.indent -= 2
             lines.append(" " * self.indent + f"</{element_name}>")
         else:
             lines[-1] = lines[-1][:-1] + " />"
         return "\n".join(lines)
```

### Comparing `marko-1.3.1/marko/block.py` & `marko-2.0.0/marko/block.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 Block level elements
 """
 from __future__ import annotations
 
 import re
-from typing import Any, Match, Pattern, cast
+from typing import TYPE_CHECKING, Any, Match, NamedTuple, Sequence, cast
 
 from . import inline, inline_parser, patterns
 from .element import Element
-from .helpers import Source, find_next, normalize_label, partition_by_spaces
-from .parser import Parser
+from .helpers import find_next, normalize_label, partition_by_spaces
+
+if TYPE_CHECKING:
+    from .source import Source
 
 __all__ = (
     "Document",
     "CodeBlock",
     "Heading",
     "List",
     "ListItem",
@@ -27,21 +29,23 @@
     "Paragraph",
 )
 
 
 class BlockElement(Element):
     """Any block element should inherit this class"""
 
+    #: An attribute to hold the children
+    children: Sequence[Element] = []
     #: Use to denote the precedence in parsing
     priority = 5
     #: if True, it won't be included in parsing process but produced by other elements
     #: other elements instead.
     virtual = False
-    #: Whether children are parsed as inline elements.
-    inline_children = False
+    #: If not empty, the body needs to be parsed as inline elements
+    inline_body: str = ""
     #: If true, will replace the element which it derives from.
     override = False
     _prefix = ""
 
     @classmethod
     def match(cls, source: Source) -> Any:
         """Test if the source matches the element at current position.
@@ -58,42 +62,27 @@
         passed to ``__init__`` method afterwards. Inline parsing, if any, should also
         be performed here.
 
         :param source: the ``Source`` object of the content to be parsed
         """
         raise NotImplementedError()
 
-    def parse_inline(self) -> None:
-        """Inline parsing is postponed so that all link references
-        are seen before that.
-        """
-        if self.inline_children:
-            self.children = parser.parse_inline(self.children)  # type: ignore
-        elif isinstance(getattr(self, "children", None), list):
-            for child in self.children:
-                if isinstance(child, BlockElement):
-                    child.parse_inline()
-
     def __lt__(self, o: BlockElement) -> bool:
         return self.priority < o.priority
 
 
 class Document(BlockElement):
     """Document node element."""
 
     _prefix = ""
     virtual = True
 
-    def __init__(self, text: str) -> None:
+    def __init__(self) -> None:
+        super().__init__()
         self.link_ref_defs: dict[str, tuple[str, str]] = {}
-        source = Source(text)
-        inline._root_node = self  # type: ignore
-        with source.under_state(self):
-            self.children = parser.parse(source)  # type: ignore
-        self.parse_inline()
 
 
 class BlankLine(BlockElement):
     """Blank lines"""
 
     priority = 5
 
@@ -117,42 +106,41 @@
     """Heading element: (### Hello\n)"""
 
     priority = 6
     pattern = re.compile(
         r" {0,3}(#{1,6})((?=\s)[^\n]*?|[^\n\S]*)(?:(?<=\s)(?<!\\)#+)?[^\n\S]*$\n?",
         flags=re.M,
     )
-    inline_children = True
 
     def __init__(self, match: Match[str]) -> None:
         self.level = len(match.group(1))
-        self.children = match.group(2).strip()
+        self.inline_body = match.group(2).strip()
 
     @classmethod
     def match(cls, source: Source) -> Match[str] | None:
         return source.expect_re(cls.pattern)
 
     @classmethod
     def parse(cls, source: Source) -> Match[str] | None:
         m = source.match
         source.consume()
         return m
 
 
 class SetextHeading(BlockElement):
     """Setext heading: (Hello\n===\n)
+
     It can only be created by Paragraph.parse.
     """
 
     virtual = True
-    inline_children = True
 
     def __init__(self, lines: list[str]) -> None:
         self.level = 1 if lines.pop().strip()[0] == "=" else 2
-        self.children = "".join(line.lstrip() for line in lines).strip()
+        self.inline_body = "".join(line.lstrip() for line in lines).strip()
 
 
 class CodeBlock(BlockElement):
     """Indented code block: (    this is a code block\n)"""
 
     priority = 4
 
@@ -164,33 +152,35 @@
     @classmethod
     def match(cls, source: Source) -> str:
         line = source.next_line(False)
         prefix = source.prefix + " {4}"
         if isinstance(source.state, Quote):
             # requires five spaces to prefix
             prefix = source.prefix[:-1] + " {4}"
-        return cls.strip_prefix(line, prefix)  # type: ignore
+        line = cls.strip_prefix(line, prefix)
+        source.context.code_line = line
+        return line
 
     @classmethod
     def parse(cls, source: Source) -> str:
         prefix = source.prefix + " {4}"
-        lines = [cls.match(source)]
+        lines = [source.context.code_line]
         source.consume()
         source.anchor()
         while not source.exhausted:
             line = source.next_line()
             if line is not None and not line.strip():
                 source.consume()
                 stripped_line = cls.strip_prefix(line, prefix)
                 if stripped_line:
                     lines.append(stripped_line)
                 else:
                     lines.append("\n")
             elif cls.match(source):
-                lines.append(cls.match(source))
+                lines.append(source.context.code_line)
                 source.consume()
                 source.anchor()
             else:
                 source.reset()
                 break
         return "".join(lines).rstrip("\n") + "\n"
 
@@ -212,15 +202,20 @@
 
 
 class FencedCode(BlockElement):
     """Fenced code block: (```python\nhello\n```\n)"""
 
     priority = 7
     pattern = re.compile(r"( {,3})(`{3,}|~{3,})[^\n\S]*(.*?)$", re.M)
-    _parse_info: tuple[str, str, str, str] = ("", "", "", "")
+
+    class ParseInfo(NamedTuple):
+        prefix: str
+        leading: str
+        lang: str
+        extra: str
 
     def __init__(self, match: tuple[str, str, str]) -> None:
         self.lang = inline.Literal.strip_backslash(match[0])
         self.extra = match[1]
         self.children = [inline.RawText(match[2], False)]
 
     @classmethod
@@ -228,38 +223,39 @@
         m = source.expect_re(cls.pattern)
         if not m:
             return None
         prefix, leading, info = m.groups()
         if leading[0] == "`" and "`" in info:
             return None
         lang, _, extra = partition_by_spaces(info)
-        cls._parse_info = prefix, leading, lang, extra
+        source.context.code_info = cls.ParseInfo(prefix, leading, lang, extra)
         return m
 
     @classmethod
     def parse(cls, source: Source) -> tuple[str, str, str]:
         source.next_line()
         source.consume()
         lines = []
+        parse_info: FencedCode.ParseInfo = source.context.code_info
         while not source.exhausted:
             line = source.next_line()
             if line is None:
                 break
             source.consume()
             m = re.match(r" {,3}(~+|`+)[^\n\S]*$", line, flags=re.M)
-            if m and cls._parse_info[1] in m.group(1):
+            if m and parse_info.leading in m.group(1):
                 break
 
-            prefix_len = source.match_prefix(cls._parse_info[0], line)
+            prefix_len = source.match_prefix(parse_info.prefix, line)
             if prefix_len >= 0:
                 line = line[prefix_len:]
             else:
                 line = line.lstrip()
             lines.append(line)
-        return cls._parse_info[2], cls._parse_info[3], "".join(lines)
+        return parse_info.lang, parse_info.extra, "".join(lines)
 
 
 class ThematicBreak(BlockElement):
     """Horizontal rules: (----\n)"""
 
     priority = 8
     pattern = re.compile(r" {,3}([-_*][^\n\S]*){3,}$\n?", flags=re.M)
@@ -277,151 +273,158 @@
         return cls()
 
 
 class HTMLBlock(BlockElement):
     """HTML blocks, parsed as it is"""
 
     priority = 5
-    _end_cond: Pattern[str] | None = None
 
     def __init__(self, lines: str) -> None:
-        self.children = lines
+        self.body = lines
 
     @classmethod
     def match(cls, source: Source) -> int | bool:
+        source.context.html_end = None
         if source.expect_re(r"(?i) {,3}<(script|pre|style|textarea)[>\s]"):
             assert source.match
-            cls._end_cond = re.compile(rf"(?i)</{source.match.group(1)}>")
+            source.context.html_end = re.compile(rf"(?i)</{source.match.group(1)}>")
             return 1
         if source.expect_re(r" {,3}<!--"):
-            cls._end_cond = re.compile(r"-->")
+            source.context.html_end = re.compile(r"-->")
             return 2
         if source.expect_re(r" {,3}<\?"):
-            cls._end_cond = re.compile(r"\?>")
+            source.context.html_end = re.compile(r"\?>")
             return 3
         if source.expect_re(r" {,3}<!"):
-            cls._end_cond = re.compile(r">")
+            source.context.html_end = re.compile(r">")
             return 4
         if source.expect_re(r" {,3}<!\[CDATA\["):
-            cls._end_cond = re.compile(r"\]\]>")
+            source.context.html_end = re.compile(r"\]\]>")
             return 5
         block_tag = r"(?:{})".format("|".join(patterns.tags))
         if source.expect_re(r"(?im) {,3}</?%s(?: +|/?>|$)" % block_tag):
-            cls._end_cond = None
+            source.context.html_end = None
             return 6
         if source.expect_re(
             r"(?m) {,3}(<%(tag)s(?:%(attr)s)*[^\n\S]*/?>|</%(tag)s[^\n\S]*>)[^\n\S]*$"
             % {"tag": patterns.tag_name, "attr": patterns.attribute_no_lf}
         ):
-            cls._end_cond = None
+            source.context.html_end = None
             return 7
 
         return False
 
     @classmethod
     def parse(cls, source: Source) -> str:
         lines = []
         while not source.exhausted:
             line = source.next_line()
             if line is None:
                 break
             lines.append(line)
-            if cls._end_cond is not None:
-                if cls._end_cond.search(line):
+            if source.context.html_end is not None:
+                if source.context.html_end.search(line):
                     source.consume()
                     break
             elif line.strip() == "":
                 lines.pop()
                 break
             source.consume()
         return "".join(lines)
 
 
 class Paragraph(BlockElement):
     """A paragraph element"""
 
     priority = 1
     pattern = re.compile(r"[^\n]+$\n?", flags=re.M)
-    inline_children = True
 
     def __init__(self, lines: list[str]) -> None:
         str_lines = "".join(line.lstrip() for line in lines).rstrip("\n")
-        self.children = str_lines
+        self.inline_body = str_lines
         self._tight = False
 
     @classmethod
     def match(cls, source: Source) -> bool:
         return source.expect_re(cls.pattern) is not None
 
     @staticmethod
     def is_setext_heading(line: str) -> bool:
         return re.match(r" {,3}(=+|-+)[^\n\S]*$", line) is not None
 
     @classmethod
     def break_paragraph(cls, source: Source, lazy: bool = False) -> bool:
-        assert isinstance(parser, Parser)
-        if (
-            parser.block_elements["Quote"].match(source)
-            or parser.block_elements["Heading"].match(source)
-            or parser.block_elements["BlankLine"].match(source)
-            or parser.block_elements["FencedCode"].match(source)
-        ):
-            return True
-        if (
-            lazy
-            and isinstance(source.state, List)
-            and parser.block_elements["ListItem"].match(source)
-        ):
-            return True
-        if parser.block_elements["List"].match(source):
-            result = parser.block_elements["ListItem"].parse_leading(
-                source.next_line().rstrip(), 0
-            )
-            if lazy or (result[1][:-1] == "1" or result[1] in "*-+") and result[3]:
+        parser = source.parser
+        prev_match = source.match
+        try:
+            if (
+                parser.block_elements["Quote"].match(source)
+                or parser.block_elements["Heading"].match(source)
+                or parser.block_elements["BlankLine"].match(source)
+                or parser.block_elements["FencedCode"].match(source)
+            ):
                 return True
-        html_type = parser.block_elements["HTMLBlock"].match(source)
-        if html_type and html_type != 7:
-            return True
-        if parser.block_elements["ThematicBreak"].match(source):
-            if not lazy and cls.is_setext_heading(source.next_line()):
-                return False
-            return True
-        return False
+            if (
+                lazy
+                and isinstance(source.state, List)
+                and parser.block_elements["ListItem"].match(source)
+            ):
+                return True
+            if parser.block_elements["List"].match(source):
+                result = cast(
+                    "type[ListItem]", parser.block_elements["ListItem"]
+                ).parse_leading(source.next_line().rstrip(), 0)
+                if lazy or (result[1][:-1] == "1" or result[1] in "*-+") and result[3]:
+                    return True
+            html_type = parser.block_elements["HTMLBlock"].match(source)
+            if html_type and html_type != 7:
+                return True
+            if parser.block_elements["ThematicBreak"].match(source):
+                if not lazy and cls.is_setext_heading(source.next_line()):
+                    return False
+                return True
+            return False
+        finally:
+            source.match = prev_match
 
     @classmethod
-    def parse(cls, source: Source) -> list[str]:
-        lines = [source.next_line()]
+    def parse(cls, source: Source) -> list[str] | SetextHeading:
+        lines = [cast(str, source.next_line())]
         source.consume()
         end_parse = False
         while not source.exhausted and not end_parse:
             if cls.break_paragraph(source):
                 break
             line = source.next_line()
             # the prefix is matched and not breakers
             if line:
                 lines.append(line)
                 source.consume()
                 if cls.is_setext_heading(line):
-                    return parser.block_elements["SetextHeading"](lines)  # type: ignore
+                    return cast(
+                        "type[SetextHeading]",
+                        source.parser.block_elements["SetextHeading"],
+                    )(lines)
             else:
                 # check lazy continuation, store the previous state stack
                 states = source._states[:]
                 while len(source._states) > 1:
                     source.pop_state()
-                    if source.next_line():
+                    next_line = source.next_line()
+                    if next_line:
                         # matches the prefix, quit the loop
                         if cls.break_paragraph(source, True):
                             # stop the whole parsing
                             end_parse = True
                         else:
-                            lines.append(source.next_line())
+                            lines.append(next_line)
                             source.consume()
                         break
                 source._states = states
-        return lines  # type: ignore
+        return lines
 
 
 class Quote(BlockElement):
     """block quote element: (> hello world)"""
 
     priority = 6
     _prefix = r" {,3}>[^\n\S]?"
@@ -430,54 +433,61 @@
     def match(cls, source: Source) -> Match[str] | None:
         return source.expect_re(r" {,3}>")
 
     @classmethod
     def parse(cls, source: Source) -> Quote:
         state = cls()
         with source.under_state(state):
-            state.children = parser.parse(source)  # type: ignore
+            state.children = source.parser.parse_source(source)
         return state
 
 
 class List(BlockElement):
     """List block element"""
 
     priority = 6
     _prefix = ""
     pattern = re.compile(r" {,3}(\d{1,9}[.)]|[*\-+])[ \t\n\r\f]")
-    _parse_info = ("", False, 0)
 
-    def __init__(self) -> None:
-        self.bullet, self.ordered, self.start = self._parse_info
+    class ParseInfo(NamedTuple):
+        bullet: str
+        ordered: bool
+        start: int
+
+    def __init__(self, info: List.ParseInfo) -> None:
+        self.bullet, self.ordered, self.start = info
         self.tight = True
 
     @classmethod
     def match(cls, source: Source) -> bool:
         m = source.expect_re(cls.pattern)
         if not m:
             return False
         bullet, ordered, start = m.group(1), False, 1
         if bullet[:-1].isdigit():
             ordered = True
             start = int(bullet[:-1])
-        cls._parse_info = (bullet, ordered, start)
+        source.context.list_info = cls.ParseInfo(bullet, ordered, start)
         return m is not None
 
     @classmethod
     def parse(cls, source: Source) -> List:
-        state = cls()
+        state = cls(source.context.list_info)
         children = []
         tight = True
         has_blank_line = False
+        parser = source.parser
         with source.under_state(state):
             while not source.exhausted:
-                if parser.block_elements["ListItem"].match(source):  # type: ignore
-                    el = parser.block_elements["ListItem"].parse(source)  # type: ignore
+                if parser.block_elements["ListItem"].match(source):
+                    el = parser.block_elements["ListItem"].parse(source)
                     if not isinstance(el, BlockElement):
-                        el = parser.block_elements["ListItem"](el)  # type: ignore
+                        el = cast("type[ListItem]", parser.block_elements["ListItem"])(
+                            el
+                        )
                     children.append(el)
                     source.anchor()
                     if has_blank_line:
                         tight = False
                 elif BlankLine.match(source):
                     BlankLine.parse(source)
                     has_blank_line = True
@@ -497,21 +507,25 @@
         state.tight = tight
         return state
 
 
 class ListItem(BlockElement):
     """List item element. It can only be created by List.parse"""
 
-    _parse_info = (0, "", 0)
     virtual = True
     _tight = False
     pattern = re.compile(r" {,3}(\d{1,9}[.)]|[*\-+])[ \t\n\r\f]")
 
-    def __init__(self) -> None:
-        indent, bullet, mid = self._parse_info
+    class ParseInfo(NamedTuple):
+        indent: int
+        bullet: str
+        mid: int
+
+    def __init__(self, info: ListItem.ParseInfo) -> None:
+        indent, bullet, mid = info
         self._prefix = " " * indent + re.escape(bullet) + " " * mid
         self._second_prefix = " " * (len(bullet) + indent + (mid or 1))
 
     @classmethod
     def parse_leading(cls, line: str, prefix_pos: int) -> tuple[int, str, int, str]:
         stripped_line = line[prefix_pos:].expandtabs(4).lstrip()
         indent = len(line) - prefix_pos - len(stripped_line)
@@ -519,67 +533,67 @@
         mid = len(spaces)
         if mid > 4:
             mid = 1
         return indent, bullet, mid, tail
 
     @classmethod
     def match(cls, source: Source) -> bool:
-        if parser.block_elements["ThematicBreak"].match(source):  # type: ignore
+        if source.parser.block_elements["ThematicBreak"].match(source):
             return False
         if not source.expect_re(cls.pattern):
             return False
         next_line = cast(str, source.next_line(False)).expandtabs(4)
         prefix_pos = 0
         m = re.match(source.prefix, next_line)
         if m is not None:
             prefix_pos = m.end()
-        indent, bullet, mid, _ = cls.parse_leading(next_line.rstrip(), prefix_pos)  # type: ignore
+        indent, bullet, mid, _ = cls.parse_leading(next_line.rstrip(), prefix_pos)
         parent = source.state
         assert isinstance(parent, List)
         if (
             parent.ordered
             and not bullet[:-1].isdigit()
             or bullet[-1] != parent.bullet[-1]
         ):
             return False
         if not parent.ordered and bullet != parent.bullet:
             return False
-        cls._parse_info = (indent, bullet, mid)
+        source.context.list_item_info = cls.ParseInfo(indent, bullet, mid)
         return True
 
     @classmethod
     def parse(cls, source: Source) -> ListItem:
-        state = cls()
+        state = cls(source.context.list_item_info)
         state.children = []
         with source.under_state(state):
-            if not source.next_line().strip():  # type: ignore
+            if not source.next_line().strip():  # type: ignore[union-attr]
                 source.consume()
-                if not source.next_line() or not source.next_line().strip():  # type: ignore
+                if not source.next_line() or not source.next_line().strip():  # type: ignore[union-attr]
                     return state
-            state.children = parser.parse(source)  # type: ignore
+            state.children = source.parser.parse_source(source)
         if isinstance(state.children[-1], BlankLine):
             # Remove the last blank line from list item
-            blankline = state.children.pop()
+            blankline = cast(BlankLine, state.children.pop())
             if state.children:
                 source.pos = blankline._anchor
         return state
 
 
 class LinkRefDef(BlockElement):
     """Link reference definition:
     [label]: destination "title"
     """
 
     pattern = re.compile(r" {,3}(\[[\s\S]*?)(?=\n\n|\Z)", flags=re.M)
-    _parse_info = (
-        inline_parser._EMPTY_GROUP,
-        inline_parser._EMPTY_GROUP,
-        inline_parser._EMPTY_GROUP,
-        -1,
-    )
+
+    class ParseInfo(NamedTuple):
+        link_label: inline_parser.Group
+        link_dest: inline_parser.Group
+        link_title: inline_parser.Group
+        end: int
 
     @classmethod
     def match(cls, source: Source) -> bool:
         m = source.expect_re(cls.pattern)
         if not m:
             return False
         text = source._buffer
@@ -603,22 +617,21 @@
         if text[i:end].strip():
             if link_title.text and "\n" in text[link_dest.end : link_title.start]:
                 link_title = inline_parser._EMPTY_GROUP
                 end = find_next(text, "\n", link_dest.end) + 1
             else:
                 # There is content after the link title
                 return False
-        cls._parse_info = (link_label, link_dest, link_title, end)
+        source.context.linkref_info = cls.ParseInfo(
+            link_label, link_dest, link_title, end
+        )
         return True
 
     @classmethod
     def parse(cls, source: Source) -> LinkRefDef:
-        label, dest, title, pos = cls._parse_info
+        label, dest, title, pos = source.context.linkref_info
         normalized_label = normalize_label(label.text[1:-1])
-        assert isinstance(source.root, Document)
-        if normalized_label not in source.root.link_ref_defs:
-            source.root.link_ref_defs[normalized_label] = (dest.text, title.text)
+        link_ref_defs = source.root.link_ref_defs
+        if normalized_label not in link_ref_defs:
+            link_ref_defs[normalized_label] = (dest.text, title.text)
         source.pos = pos
         return cls()
-
-
-parser = None
```

### Comparing `marko-1.3.1/marko/cli.py` & `marko-2.0.0/marko/cli.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.1/marko/element.py` & `marko-2.0.0/marko/element.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.1/marko/ext/codehilite.py` & `marko-2.0.0/marko/ext/codehilite.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 import json
 
 from pygments import highlight
 from pygments.formatters import html
 from pygments.lexers import get_lexer_by_name, guess_lexer
 from pygments.util import ClassNotFound
 
+from marko.helpers import MarkoExtension
+
 
 def _parse_extras(line):
     if not line:
         return {}
     extras = {}
     for token in line.split(","):
         k, has_eq, v = token.partition("=")
@@ -40,28 +42,24 @@
 
 
 class CodeHiliteRendererMixin:
     options = {}  # type: dict
 
     def render_fenced_code(self, element):
         code = element.children[0].children
-        options = CodeHiliteRendererMixin.options.copy()
-        options.update(_parse_extras(getattr(element, "extra", None)))
+        options = {**self.options, **_parse_extras(getattr(element, "extra", None))}
         if element.lang:
             try:
                 lexer = get_lexer_by_name(element.lang, stripall=True)
             except ClassNotFound:
                 lexer = guess_lexer(code)
         else:
             lexer = guess_lexer(code)
         formatter = html.HtmlFormatter(**options)
         return highlight(code, lexer, formatter)
 
 
-class CodeHilite:
-    def __init__(self, **options):
-        CodeHiliteRendererMixin.options = options
-        self.renderer_mixins = [CodeHiliteRendererMixin]
-
-
 def make_extension(**options):
-    return CodeHilite(**options)
+    mixin_cls = type(
+        "CodeHiliteRendererMixin", (CodeHiliteRendererMixin,), {"options": options}
+    )
+    return MarkoExtension(renderer_mixins=[mixin_cls])
```

### Comparing `marko-1.3.1/marko/ext/footnote.py` & `marko-2.0.0/marko/ext/footnote.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,23 +9,25 @@
     from marko import Markdown
 
     text = 'Foo[^1]\\n\\n[^1]: This is a footnote.\\n'
     markdown = Markdown(extensions=['footnote'])
     print(markdown(text))
 
 """
+from __future__ import annotations
+
 import re
 
 from marko import block, helpers, inline
 
 
 class Document(block.Document):
-    def __init__(self, text):
+    def __init__(self):
+        super().__init__()
         self.footnotes = {}
-        super().__init__(text)
 
 
 class FootnoteDef(block.BlockElement):
     pattern = re.compile(r" {,3}\[\^([^\]]+)\]:[^\n\S]*(?=\S| {4})")
     priority = 6
 
     def __init__(self, match):
@@ -37,31 +39,31 @@
     def match(cls, source):
         return source.expect_re(cls.pattern)
 
     @classmethod
     def parse(cls, source):
         state = cls(source.match)
         with source.under_state(state):
-            state.children = block.parser.parse(source)
+            state.children = source.parser.parse_source(source)
         source.root.footnotes[state.label] = state
         return state
 
 
 class FootnoteRef(inline.InlineElement):
     pattern = re.compile(r"\[\^([^\]]+)\]")
     priority = 6
 
     def __init__(self, match):
         self.label = helpers.normalize_label(match.group(1))
 
     @classmethod
-    def find(cls, text):
-        for match in super().find(text):
+    def find(cls, text, *, source):
+        for match in super().find(text, source=source):
             label = helpers.normalize_label(match.group(1))
-            if label in inline._root_node.footnotes:
+            if label in source.root.footnotes:
                 yield match
 
 
 class FootnoteRendererMixin:
     def __init__(self):
         super().__init__()
         self.footnotes = []
@@ -98,14 +100,12 @@
             return text
         children = "".join(self._render_footnote_def(item) for item in items)
         footnotes = f'<div class="footnotes">\n<ol>\n{children}</ol>\n</div>\n'
         self.footnotes = []
         return text + footnotes
 
 
-class Footnote:
-    elements = [Document, FootnoteDef, FootnoteRef]
-    renderer_mixins = [FootnoteRendererMixin]
-
-
 def make_extension():
-    return Footnote()
+    return helpers.MarkoExtension(
+        elements=[Document, FootnoteDef, FootnoteRef],
+        renderer_mixins=[FootnoteRendererMixin],
+    )
```

### Comparing `marko-1.3.1/marko/ext/gfm/__init__.py` & `marko-2.0.0/marko/ext/gfm/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     from marko.ext.gfm import gfm
     print(gfm(text))
 
 """
 import re
 
 from marko import Markdown
+from marko.helpers import MarkoExtension
 
 from . import elements
 
 
 class GFMRendererMixin:
     tagfilter = re.compile(
         r"<(title|texarea|style|xmp|iframe|noembed|noframes|script|plaintext)",
@@ -46,15 +47,15 @@
     def render_strikethrough(self, element):
         return "<del>{}</del>".format(self.render_children(element))
 
     def render_inline_html(self, element):
         return self.tagfilter.sub(r"&lt;\1", element.children)
 
     def render_html_block(self, element):
-        return self.tagfilter_no_open.sub(r"\1&lt;\2", element.children)
+        return self.tagfilter_no_open.sub(r"\1&lt;\2", element.body)
 
     def render_table(self, element):
         header, body = element.children[0], element.children[1:]
         theader = "<thead>\n{}</thead>".format(self.render(header))
         tbody = ""
         if body:
             tbody = "\n<tbody>\n{}</tbody>".format(
@@ -74,27 +75,27 @@
             tag=tag, children=self.render_children(element), align=align
         )
 
     def render_url(self, element):
         return self.render_link(element)
 
 
-class GFM:
-    elements = [
+GFM = MarkoExtension(
+    elements=[
         elements.Paragraph,
         elements.ListItem,
         elements.InlineHTML,
         elements.Strikethrough,
         elements.Url,
         elements.Table,
         elements.TableRow,
         elements.TableCell,
-    ]
-    renderer_mixins = [GFMRendererMixin]
+    ],
+    renderer_mixins=[GFMRendererMixin],
+)
 
 
-gfm = Markdown()
-gfm.use(GFM)
+gfm = Markdown(extensions=[GFM])
 
 
 def make_extension():
-    return GFM()
+    return GFM
```

### Comparing `marko-1.3.1/marko/ext/gfm/elements.py` & `marko-2.0.0/marko/ext/gfm/elements.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 class Paragraph(block.Paragraph):
     _task_list_item_pattern = re.compile(r"(\[[\sxX]\])\s+\S")
     override = True
 
     def __init__(self, lines):
         super().__init__(lines)
-        m = self._task_list_item_pattern.match(self.children)
+        m = self._task_list_item_pattern.match(self.inline_body)
         if m:
             self.checked = m.group(1)[1:-1].lower() == "x"
-            self.children = self.children[m.end(1) :]
+            self.inline_body = self.inline_body[m.end(1) :]
 
 
 class InlineHTML(inline.InlineHTML):
     pattern = re.compile(
         r"(<%s(?:%s)* */?>"  # open tag
         r"|</%s *>"  # closing tag
         r"|<!--(?:>|->|[\s\S]*?-->)"  # HTML comment
@@ -78,15 +78,15 @@
 
     def __init__(self, match):
         super().__init__(match)
         if self.www_pattern.match(self.dest):
             self.dest = "http://" + self.dest
 
     @classmethod
-    def find(cls, text):
+    def find(cls, text, *, source):
         for match in itertools.chain(
             cls.www_pattern.finditer(text), cls.bare_pattern.finditer(text)
         ):
             domain = match.group(2)
             if domain:
                 parts = domain.split(".")
                 if len(parts) < 2 or any("_" in p for p in parts[-2:]):
@@ -152,15 +152,15 @@
                 if stripped_d[0] == ":" and stripped_d[-1] == ":":
                     th.align = "center"
                 elif stripped_d[0] == ":":
                     th.align = "left"
                 elif stripped_d[-1] == ":":
                     th.align = "right"
             while not source.exhausted:
-                for e in block.parser._build_block_element_list():
+                for e in source.parser._build_block_element_list():
                     if issubclass(e, (Table, block.Paragraph)):
                         continue
                     if e.match(source):
                         break
                 else:
                     if TableRow.match(source):
                         rv.children.append(TableRow(TableRow.parse(source)))
@@ -213,13 +213,12 @@
         return cells
 
 
 class TableCell(block.BlockElement):
     """A table cell element."""
 
     virtual = True
-    inline_children = True
 
     def __init__(self, text):
-        self.children = text.strip().replace("\\|", "|")
+        self.inline_body = text.strip().replace("\\|", "|")
         self.header = False
         self.align = None
```

### Comparing `marko-1.3.1/marko/ext/latex_renderer.py` & `marko-2.0.0/marko/ext/latex_renderer.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 LaTeX renderer
 """
 from __future__ import annotations
 
 import logging
 from typing import Iterable
 
-from marko import Renderer
+from marko.helpers import MarkoExtension
+from marko.renderer import Renderer
 
 _logger = logging.getLogger(__name__)
 
 
-class LatexRenderer(Renderer):
+class LatexRendererMixin:
     """Render the parsed Markdown to LaTeX format."""
 
     _packages: set[str]
 
     def __init__(self):
         super().__init__()
         self._packages = set()
@@ -156,7 +157,15 @@
 
         return "".join(specials.get(s, s) for s in text)
 
     @staticmethod
     def _environment(env_name: str, content: str, options: Iterable[str] = ()) -> str:
         options_str = f"[{','.join(options)}]" if options else ""
         return f"\\begin{{{env_name}}}{options_str}\n{content}\\end{{{env_name}}}\n"
+
+
+class LatexRenderer(LatexRendererMixin, Renderer):
+    """Render the parsed Markdown to LaTeX format."""
+
+
+def make_extension():
+    return MarkoExtension(renderer_mixins=[LatexRendererMixin])
```

### Comparing `marko-1.3.1/marko/ext/pangu.py` & `marko-2.0.0/marko/ext/pangu.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     from marko import Markdown
 
     markdown = Markdown(extensions=['pangu'])
     print(markdown(text))
 """
 import re
 
+from marko.helpers import MarkoExtension
+
 CJK_RE = (
     r"\u2e80-\u2eff\u2f00-\u2fdf\u3040-\u309f\u30a0-\u30ff\u3100-\u312f"
     r"\u3200-\u32ff\u3400-\u4dbf\u4e00-\u9fff\uf900-\ufaff"
 )
 LATIN_RE = r"a-zA-Z0-9"
 PANGU_RE = re.compile(
     r"((?<=[{cjk}])(?=[{latin}])|(?<=[{latin}])(?=[{cjk}]))".format(
@@ -32,13 +34,9 @@
 
 class PanguRendererMixin:
     def render_raw_text(self, element):
         rv = super().render_raw_text(element)
         return PANGU_RE.sub('<span class="pangu"></span>', rv)
 
 
-class Pangu:
-    renderer_mixins = [PanguRendererMixin]
-
-
 def make_extension():
-    return Pangu()
+    return MarkoExtension(renderer_mixins=[PanguRendererMixin])
```

### Comparing `marko-1.3.1/marko/ext/toc.py` & `marko-2.0.0/marko/ext/toc.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,31 +4,33 @@
 
 Renders the TOC(Table Of Content) for a markdown document.
 This requires to install `toc` extras::
 
     pip install marko[toc]
 
 Arguments:
-* openning: the openning tag, defaults to <ul>
-* closing: the closing tag, defaults to </ul>
-* item_format: the toc item format, defaults to '<li><a href="#{slug}">{text}</a></li>'
+    * openning: the openning tag, defaults to <ul>
+    * closing: the closing tag, defaults to </ul>
+    * item_format: the toc item format, defaults to '<li><a href="#{slug}">{text}</a></li>'
 
 Usage::
 
     from marko import Markdown
 
     markdown = Markdown(extensions=['toc'])
 
     print(markdown(text))
     print(markdown.renderer.render_toc())
 
 """
 import re
 
-from slugify import slugify  # type: ignore
+from slugify import slugify
+
+from marko.helpers import MarkoExtension  # type: ignore
 
 
 class TocRendererMixin:
     openning = "<ul>"
     closing = "</ul>"
     item_format = '<li><a href="#{slug}">{text}</a></li>'
 
@@ -45,42 +47,39 @@
         for level, slug, text in self.headings:
             if first_level is not None and level >= first_level + maxdepth:
                 continue
 
             if first_level is None:
                 first_level = level
                 last_level = level
-                rv.append(TocRendererMixin.openning + "\n")
+                rv.append(self.openning + "\n")
 
             if last_level == level - 1:
-                rv.append(TocRendererMixin.openning + "\n")
+                rv.append(self.openning + "\n")
                 last_level = level
             while last_level > level:
-                rv.append(TocRendererMixin.closing + "\n")
+                rv.append(self.closing + "\n")
                 last_level -= 1
             # last_level == level
-            rv.append(TocRendererMixin.item_format.format(slug=slug, text=text) + "\n")
+            rv.append(self.item_format.format(slug=slug, text=text) + "\n")
         for _ in range(first_level, last_level + 1):
-            rv.append(TocRendererMixin.closing + "\n")
+            rv.append(self.closing + "\n")
 
         return "".join(rv)
 
     def render_heading(self, element):
         children = self.render_children(element)
         slug = slugify(re.sub(r"<.+?>", "", children))
         self.headings.append((int(element.level), slug, children))
         return '<h{0} id="{1}">{2}</h{0}>\n'.format(element.level, slug, children)
 
 
-class Toc:
-    def __init__(self, openning=None, closing=None, item_format=None):
-        if openning:
-            TocRendererMixin.openning = openning
-        if closing:
-            TocRendererMixin.closing = closing
-        if item_format:
-            TocRendererMixin.item_format = item_format
-        self.renderer_mixins = [TocRendererMixin]
-
-
 def make_extension(openning=None, closing=None, item_format=None):
-    return Toc(openning, closing, item_format)
+    options = {}
+    if openning:
+        options["openning"] = openning
+    if closing:
+        options["closing"] = closing
+    if item_format:
+        options["item_format"] = item_format
+    renderer_mixins = [type("TocRendererMixin", (TocRendererMixin,), options)]
+    return MarkoExtension(renderer_mixins=renderer_mixins)
```

### Comparing `marko-1.3.1/marko/html_renderer.py` & `marko-2.0.0/marko/html_renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             lang, html.escape(element.children[0].children)  # type: ignore
         )
 
     def render_code_block(self, element: block.CodeBlock) -> str:
         return self.render_fenced_code(cast("block.FencedCode", element))
 
     def render_html_block(self, element: block.HTMLBlock) -> str:
-        return element.children  # type: ignore
+        return element.body
 
     def render_thematic_break(self, element: block.ThematicBreak) -> str:
         return "<hr />\n"
 
     def render_heading(self, element: block.Heading) -> str:
         return "<h{level}>{children}</h{level}>\n".format(
             level=element.level, children=self.render_children(element)
@@ -80,15 +80,15 @@
     def render_emphasis(self, element: inline.Emphasis) -> str:
         return f"<em>{self.render_children(element)}</em>"
 
     def render_strong_emphasis(self, element: inline.StrongEmphasis) -> str:
         return f"<strong>{self.render_children(element)}</strong>"
 
     def render_inline_html(self, element: inline.InlineHTML) -> str:
-        return self.render_html_block(cast("block.HTMLBlock", element))
+        return cast(str, element.children)
 
     def render_plain_text(self, element: Any) -> str:
         if isinstance(element.children, str):
             return self.escape_html(element.children)
         return self.render_children(element)
 
     def render_link(self, element: inline.Link) -> str:
```

### Comparing `marko-1.3.1/marko/inline.py` & `marko-2.0.0/marko/inline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 Inline(span) level elements
 """
 from __future__ import annotations
 
 import re
-from typing import TYPE_CHECKING, Iterator, Match, Pattern, Sequence
+from typing import TYPE_CHECKING, Iterator, Pattern, Sequence
 
-from . import inline_parser, patterns
+from . import patterns
 from .element import Element
 
 if TYPE_CHECKING:
     from .inline_parser import _Match
+    from .source import Source
 
 __all__ = (
     "LineBreak",
     "Literal",
-    "LinkOrEmph",
     "InlineHTML",
     "CodeSpan",
     "Emphasis",
     "StrongEmphasis",
     "Link",
     "Image",
     "AutoLink",
@@ -49,34 +49,35 @@
 
     def __init__(self, match: _Match) -> None:
         """Parses the matched object into an element"""
         if not self.parse_children:
             self.children = match.group(self.parse_group)
 
     @classmethod
-    def find(cls, text: str) -> Iterator[Match]:
+    def find(cls, text: str, *, source: Source) -> Iterator[_Match]:
         """This method should return an iterable containing matches of this element."""
         if isinstance(cls.pattern, str):
             cls.pattern = re.compile(cls.pattern)
         return cls.pattern.finditer(text)
 
 
 class Literal(InlineElement):
     """Literal escapes need to be parsed at the first."""
 
     priority = 7
     pattern = re.compile(r'\\([!"#\$%&\'()*+,\-./:;<=>?@\[\\\]^_`{|}~])')
 
     @classmethod
     def strip_backslash(cls, text: str) -> str:
-        return cls.pattern.sub(r"\1", text)
+        return cls.pattern.sub(r"\1", text)  # type: ignore[unio]
 
 
 class LineBreak(InlineElement):
     """Line breaks:
+
     Soft: '\n'
     Hard: '  \n'
     """
 
     priority = 2
     pattern = r"( *|\\)\n(?!\Z)"
 
@@ -94,29 +95,14 @@
         r"|<\?[\s\S]*?\?>"  # processing instruction
         r"|<![A-Z]+ +[\s\S]*?>"  # declaration
         r"|<!\[CDATA\[[\s\S]*?\]\]>)"  # CDATA section
         % (patterns.tag_name, patterns.attribute, patterns.tag_name)
     )
 
 
-class LinkOrEmph(InlineElement):
-    """This is a special element, whose parsing is done specially.
-    And it produces Link or Emphasis elements.
-    """
-
-    parse_children = True
-
-    def __new__(cls, match: _Match) -> LinkOrEmph:
-        return parser.inline_elements[match.etype](match)  # type: ignore
-
-    @classmethod
-    def find(cls, text: str) -> Iterator[Match]:
-        return inline_parser.find_links_or_emphs(text, _root_node)  # type: ignore
-
-
 class StrongEmphasis(InlineElement):
     """Strong emphasis: **sample text**"""
 
     virtual = True
     parse_children = True
 
 
@@ -193,12 +179,7 @@
     virtual = True
     if TYPE_CHECKING:
         children: str
 
     def __init__(self, match: str, escape: bool = True) -> None:
         self.children = match
         self.escape = escape
-
-
-# backrefs to avoid cylic  import
-parser = None
-_root_node = None
```

### Comparing `marko-1.3.1/marko/inline_parser.py` & `marko-2.0.0/marko/inline_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,66 @@
 """
 Parse inline elements
 """
 from __future__ import annotations
 
-import collections
 import re
-from typing import TYPE_CHECKING, Match, Type, Union
+from typing import TYPE_CHECKING, Match, NamedTuple, Union
 
 from . import patterns
 from .helpers import find_next, is_paired, normalize_label
+from .inline import InlineElement
 
 if TYPE_CHECKING:
-    from .block import Document
-    from .inline import InlineElement
+    from .source import Source
 
-    ElementType = Type[InlineElement]
     _Match = Union[Match[str], "MatchObj"]
 
-Group = collections.namedtuple("Group", "start end text")
+    ElementType = type[InlineElement]
+
+
+class Group(NamedTuple):
+    start: int
+    end: int
+    text: str | None
+
+
 _EMPTY_GROUP = Group(-1, -1, None)
 WHITESPACE = " \n\t"
 ASCII_CONTROL = "".join(chr(i) for i in range(0, 32)) + chr(127)
 
 
 class ParseError(ValueError):
     """Raised when parsing fails."""
 
 
 def parse(
-    text: str, elements: list[ElementType], fallback: ElementType
+    text: str, elements: list[ElementType], fallback: ElementType, source: Source
 ) -> list[InlineElement]:
     """Parse given text and produce a list of inline elements.
 
     :param text: the text to be parsed.
     :param elements: the element types to be included in parsing
     :param fallback: fallback class when no other element type is matched.
     """
-    # this is a raw list of elements that may contain overlaps.
+
+    class LinkOrEmph(InlineElement):
+        parse_children = True
+
+        def __new__(cls, match: _Match) -> InlineElement:  # type: ignore
+            assert isinstance(match, MatchObj)
+            return source.parser.inline_elements[match.etype](match)
+
+    # A raw list of elements that may contain overlaps.
     tokens: list[Token] = []
+    for m in find_links_or_emphs(text, source.root.link_ref_defs):
+        tokens.append(Token(LinkOrEmph, m, text, fallback))
+
     for etype in elements:
-        for match in etype.find(text):
+        for match in etype.find(text, source=source):
             tokens.append(Token(etype, match, text, fallback))
     tokens.sort()
     tokens = _resolve_overlap(tokens)
     return make_elements(tokens, text, fallback=fallback)
 
 
 def _resolve_overlap(tokens: list[Token]) -> list[Token]:
@@ -154,19 +171,21 @@
             self.__class__.__name__, self.etype.__name__, self.start, self.end
         )
 
     def __lt__(self, o: Token) -> bool:
         return self.start < o.start
 
 
-def find_links_or_emphs(text: str, root_node: Document) -> list[MatchObj]:
+def find_links_or_emphs(
+    text: str, link_ref_defs: dict[str, tuple[str, str]]
+) -> list[MatchObj]:
     """Fink links/images or emphasis from text.
 
     :param text: the original text.
-    :param root_node: a reference to the root node of the AST.
+    :param link_ref_defs: a mapping of link ref definitions.
     :returns: an iterable of match object.
     """
     delimiters_re = re.compile(r"(?:!?\[|\*+|_+)")
     i = 0
     delimiters: list[Delimiter] = []
     escape = False
     matches: list[MatchObj] = []
@@ -178,15 +197,15 @@
             i += 1
         elif text[i] == "\\":
             escape = True
             i += 1
         elif code_pattern.match(text, i):
             i = code_pattern.match(text, i).end()  # type: ignore
         elif text[i] == "]":
-            node = look_for_image_or_link(text, delimiters, i, root_node, matches)
+            node = look_for_image_or_link(text, delimiters, i, link_ref_defs, matches)
             if node:
                 i = node.end()
                 matches.append(node)
             else:
                 i += 1
         else:
             m = delimiters_re.match(text, i)
@@ -199,28 +218,29 @@
     return matches
 
 
 def look_for_image_or_link(
     text: str,
     delimiters: list[Delimiter],
     close: int,
-    root_node: Document,
+    link_ref_defs: dict[str, tuple[str, str]],
     matches: list[MatchObj],
 ) -> MatchObj | None:
     for i, d in list(enumerate(delimiters))[::-1]:
         if d.content not in ("[", "!["):
             continue
         if not d.active:
             break  # break to remove the delimiter and return None
         if not _is_legal_link_text(text[d.end : close]):
             break
         link_text = Group(d.end, close, text[d.end : close])
+        assert link_text.text is not None
         etype = "Image" if d.content == "![" else "Link"
         match = _expect_inline_link(text, close + 1) or _expect_reference_link(
-            text, close + 1, link_text[2], root_node
+            text, close + 1, link_text.text, link_ref_defs
         )
         if not match:  # not a link
             break
         rv = MatchObj(etype, text, d.start, match[2], link_text, match[0], match[1])
         process_emphasis(text, delimiters, i, matches)
         if etype == "Link":
             for d in delimiters[:i]:
@@ -277,14 +297,15 @@
         if right_bracket < 0:
             raise ParseError()
         i = right_bracket + 1
         link_dest = Group(start, i, link_text[start:i])
     else:
         escaped = False
         pairs = 0
+        i = 0
         for i, c in enumerate(link_text[start:], start):
             if escaped:
                 escaped = False
             elif c == "\\":
                 escaped = True
             elif c in WHITESPACE:
                 break
@@ -344,33 +365,36 @@
     end = _parse_link_separator(text, end)
     if end >= len(text) or text[end] != ")":
         return None
     return link_dest, link_title, end + 1
 
 
 def _expect_reference_link(
-    text: str, start: int, link_text: str, root_node: Document
+    text: str, start: int, link_text: str, link_ref_defs: dict[str, tuple[str, str]]
 ) -> tuple[Group, Group, int] | None:
     link_label = _parse_link_label(text, start)
     label = link_text
     if link_label is not None:
+        assert link_label.text is not None
         label = link_label.text[1:-1] or link_text
     elif text[start : start + 2] == "[]":
         link_label = Group(start, start + 2, "[]")
-    result = _get_reference_link(label, root_node)
+    result = _get_reference_link(label, link_ref_defs)
     if not result:
         return None
     link_dest = Group(start, start, result[0])
     link_title = Group(start, start, result[1])
     return (link_dest, link_title, link_label.end if link_label else start)
 
 
-def _get_reference_link(link_label: str, root_node: Document) -> tuple[str, str] | None:
+def _get_reference_link(
+    link_label: str, link_ref_defs: dict[str, tuple[str, str]]
+) -> tuple[str, str] | None:
     normalized_label = normalize_label(link_label)
-    return root_node.link_ref_defs.get(normalized_label, None)
+    return link_ref_defs.get(normalized_label)
 
 
 def process_emphasis(
     text: str,
     delimiters: list[Delimiter],
     stack_bottom: int | None,
     matches: list[MatchObj],
```

### Comparing `marko-1.3.1/marko/md_renderer.py` & `marko-2.0.0/marko/md_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         lines = [self._prefix + indent + lines[0]] + [
             self._second_prefix + indent + line for line in lines[1:]
         ]
         self._prefix = self._second_prefix
         return "\n".join(lines) + "\n"
 
     def render_html_block(self, element: block.HTMLBlock) -> str:
-        result = self._prefix + element.children + "\n"
+        result = self._prefix + element.body + "\n"  # type: ignore[attr-defined]
         self._prefix = self._second_prefix
         return result
 
     def render_thematic_break(self, element: block.ThematicBreak) -> str:
         result = self._prefix + "* * *\n"
         self._prefix = self._second_prefix
         return result
```

### Comparing `marko-1.3.1/marko/parser.py` & `marko-2.0.0/marko/parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Base parser
 """
 from __future__ import annotations
 
 import itertools
-from typing import TYPE_CHECKING, Type
+from typing import TYPE_CHECKING, Type, cast
 
-from .helpers import Source
+from .source import Source
 
 
 class Parser:
     r"""
     All elements defined in CommonMark's spec are included in the parser
     by default.
 
@@ -20,17 +20,14 @@
 
     :param \*extras: extra elements to be included in parsing process.
     """
 
     def __init__(self) -> None:
         self.block_elements: dict[str, BlockElementType] = {}
         self.inline_elements: dict[str, InlineElementType] = {}
-        # Create references in block and inline modules to avoid cyclic import.
-        block.parser = self  # type: ignore
-        inline.parser = self  # type: ignore
 
         for el in itertools.chain(
             (getattr(block, name) for name in block.__all__),
             (getattr(inline, name) for name in inline.__all__),
         ):
             self.add_element(el)
 
@@ -50,56 +47,73 @@
         else:
             raise TypeError(
                 "The element should be a subclass of either `BlockElement` or "
                 "`InlineElement`."
             )
         dest[element.get_type()] = element
 
-    def parse(
-        self, source_or_text: Source | str
-    ) -> list[block.BlockElement] | block.BlockElement:
+    def parse(self, text: str) -> block.Document:
         """Do the actual parsing and returns an AST or parsed element.
 
         :param source_or_text: the text or source object.
             Based on the type, it will do following:
             - text: returns the parsed Document element.
             - source: parse the source and returns the parsed children as a list.
         """
-        if isinstance(source_or_text, str):
-            return self.block_elements["Document"](source_or_text)  # type: ignore
+        source = Source(text)
+        source.parser = self
+        doc = cast(block.Document, self.block_elements["Document"]())
+        with source.under_state(doc):
+            doc.children = self.parse_source(source)
+            self.parse_inline(doc, source)
+        return doc
+
+    def parse_source(self, source: Source) -> list[block.BlockElement]:
         element_list = self._build_block_element_list()
         ast: list[block.BlockElement] = []
-        assert isinstance(source_or_text, Source)
-        while not source_or_text.exhausted:
+        while not source.exhausted:
             for ele_type in element_list:
-                if ele_type.match(source_or_text):
-                    result = ele_type.parse(source_or_text)
+                if ele_type.match(source):
+                    result = ele_type.parse(source)
                     if not hasattr(result, "priority"):
                         # In some cases ``parse()`` won't return the element, but
                         # instead some information to create one, which will be passed
                         # to ``__init__()``.
                         result = ele_type(result)  # type: ignore
                     ast.append(result)
                     break
             else:
                 # Quit the current parsing and go back to the last level.
                 break
         return ast
 
-    def parse_inline(self, text: str) -> list[inline.InlineElement]:
+    def parse_inline(self, element: block.BlockElement, source: Source) -> None:
+        """Inline parsing is postponed so that all link references
+        are seen before that.
+        """
+        if element.inline_body:
+            element.children = self._parse_inline(element.inline_body, source)
+            # clear the inline body to avoid parsing it again.
+            element.inline_body = ""
+        else:
+            for child in element.children:
+                if isinstance(child, block.BlockElement):
+                    self.parse_inline(child, source)
+
+    def _parse_inline(self, text: str, source: Source) -> list[inline.InlineElement]:
         """Parses text into inline elements.
         RawText is not considered in parsing but created as a wrapper of holes
         that don't match any other elements.
 
         :param text: the text to be parsed.
         :returns: a list of inline elements.
         """
         element_list = self._build_inline_element_list()
         return inline_parser.parse(
-            text, element_list, fallback=self.inline_elements["RawText"]
+            text, element_list, fallback=self.inline_elements["RawText"], source=source
         )
 
     def _build_block_element_list(self) -> list[BlockElementType]:
         """Return a list of block elements, ordered from highest priority to lowest."""
         return sorted(
             (e for e in self.block_elements.values() if not e.virtual),
             key=lambda e: e.priority,
```

### Comparing `marko-1.3.1/marko/patterns.py` & `marko-2.0.0/marko/patterns.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.1/marko/renderer.py` & `marko-2.0.0/marko/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import TYPE_CHECKING, Any, Callable, TypeVar
 
 if TYPE_CHECKING:
     from .block import Document
     from .element import Element
 
 _T = TypeVar("_T", bound="Renderer")
+_charref_bak = html._charref  # type: ignore[attr-defined]
 
 
 class Renderer:
     """The base class of renderers.
 
     A custom renderer should subclass this class and include your own render functions.
 
@@ -41,20 +42,19 @@
     )
 
     def __init__(self) -> None:
         self.root_node: Document | None = None
 
     def __enter__(self: _T) -> _T:
         """Provide a context so that root_node can be reset after render."""
-        self._charref_bak = html._charref  # type: ignore[attr-defined]
         html._charref = self._charref  # type: ignore[attr-defined]
         return self
 
     def __exit__(self, *args: Any) -> None:
-        html._charref = self._charref_bak  # type: ignore[attr-defined]
+        html._charref = _charref_bak  # type: ignore[attr-defined]
 
     def render(self, element: Element) -> Any:
         """Renders the given element to string.
 
         :param element: a element to be rendered.
         :returns: the output string or any values.
         """
```

### Comparing `marko-1.3.1/pyproject.toml` & `marko-2.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
-    "pdm-pep517",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [project]
 authors = [
     { name = "Frost Ming", email = "mianghong@gmail.com" },
 ]
 dynamic = []
 requires-python = ">=3.7"
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "1.3.1"
+version = "2.0.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/frostming/marko"
 Documentation = "https://marko-py.readthedocs.io"
@@ -41,26 +41,44 @@
 codehilite = [
     "pygments",
 ]
 
 [project.scripts]
 marko = "marko.cli:main"
 
+[tool.pdm]
+plugins = [
+    "pdm-autoexport",
+]
+
 [tool.pdm.version]
-from = "marko/__init__.py"
+source = "file"
+path = "marko/__init__.py"
 
 [tool.pdm.dev-dependencies]
 benchmark = [
     "commonmark>=0.9",
     "markdown>=3.3",
     "markdown-it-py>=2.0; python_version >= '3.7'",
     "mistune>=2.0",
     "mistletoe>=0.7",
 ]
 dev = [
     "pytest",
     "pytest-cov",
     "mypy>=0.950",
 ]
+doc = [
+    "marko[toc]",
+    "sphinx>=5.3.0",
+    "shibuya>=2023.6.8",
+]
+
+[[tool.pdm.autoexport]]
+filename = "docs/reqs.txt"
+groups = [
+    "doc",
+]
+without-hashes = true
 
 [tool.isort]
 profile = "black"
```

### Comparing `marko-1.3.1/tests/__init__.py` & `marko-2.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.1/tests/benchmark.py` & `marko-2.0.0/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.1/tests/normalize.py` & `marko-2.0.0/tests/normalize.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.1/tests/samples/jquery.md` & `marko-2.0.0/tests/samples/jquery.md`

 * *Files identical despite different names*

### Comparing `marko-1.3.1/tests/samples/syntax.md` & `marko-2.0.0/tests/samples/syntax.md`

 * *Files identical despite different names*

### Comparing `marko-1.3.1/tests/spec/commonmark.txt` & `marko-2.0.0/tests/spec/commonmark.txt`

 * *Files identical despite different names*

### Comparing `marko-1.3.1/tests/spec/gfm.txt` & `marko-2.0.0/tests/spec/gfm.txt`

 * *Files identical despite different names*

### Comparing `marko-1.3.1/tests/test_basic.py` & `marko-2.0.0/tests/test_basic.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,62 +62,57 @@
         assert hasattr(markdown.renderer, "render_footnote_def")
 
     def test_extension_override(self):
         class MyRendererMixin:
             def render_paragraph(self, element):
                 return "foo bar"
 
-        class MyExtension:
-            renderer_mixins = [MyRendererMixin]
+        my_extension = marko.MarkoExtension(renderer_mixins=[MyRendererMixin])
 
-        markdown = marko.Markdown(extensions=["gfm", MyExtension])
+        markdown = marko.Markdown(extensions=["gfm", my_extension])
         out = markdown.convert("hello world\n")
         assert out == "foo bar"
 
     def test_extension_override_element(self):
         class MyHeading(block.Heading):
             override = True
 
-        class MyExtension:
-            elements = [MyHeading]
+        my_extension = marko.MarkoExtension(elements=[MyHeading])
 
-        markdown = marko.Markdown(extensions=[MyExtension])
+        markdown = marko.Markdown(extensions=[my_extension])
         markdown._setup_extensions()
         assert markdown.parser.block_elements["Heading"] is MyHeading
         assert markdown.parser.block_elements["Heading"].get_type() == "Heading"
 
     def test_extension_override_non_base_element(self):
         class MyHeading(block.BlockElement):
             override = True
 
-        class MyExtension:
-            elements = [MyHeading]
+        my_extension = marko.MarkoExtension(elements=[MyHeading])
 
-        markdown = marko.Markdown(extensions=[MyExtension])
+        markdown = marko.Markdown(extensions=[my_extension])
         markdown._setup_extensions()
         assert markdown.parser.block_elements["MyHeading"] is MyHeading
         assert markdown.parser.block_elements["MyHeading"].get_type() == "MyHeading"
 
     def test_extension_with_illegal_element(self):
-        class MyExtension:
-            elements = [object]
+        my_extension = marko.MarkoExtension(elements=[object])  # type: ignore
 
-        markdown = marko.Markdown(extensions=[MyExtension])
+        markdown = marko.Markdown(extensions=[my_extension])
         with pytest.raises(TypeError, match="The element should be a subclass of"):
             markdown.convert("hello world\n")
 
     def test_no_delegate_render_methods(self):
         class RendererMixin:
             def render_paragraph(self, element):
                 return "ohohohohohoh"
 
-        class Extension:
-            renderer_mixins = [RendererMixin]
+        my_extension = marko.MarkoExtension(renderer_mixins=[RendererMixin])
 
-        markdown = marko.Markdown(renderer=ASTRenderer, extensions=[Extension])
+        markdown = marko.Markdown(renderer=ASTRenderer, extensions=[my_extension])
         res = markdown.convert("Hello world")
         paragraph = res["children"][0]
         assert isinstance(paragraph, dict)
         assert paragraph["element"] == "paragraph"
 
         raw_text = paragraph["children"][0]
         assert raw_text["children"] == "Hello world"
```

### Comparing `marko-1.3.1/tests/test_ext.py` & `marko-2.0.0/tests/test_ext.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         content = "# Foo\n#### Foobar\n"
         self.markdown(content)
         toc = self.markdown.renderer.render_toc()
         assert '<li><a href="#foo">Foo</a></li>' in toc
         assert '<li><a href="#foobar">Foobar</a></li>' not in toc
 
     def test_render_toc_replace_tags(self):
-        from marko.ext.toc import Toc
+        from marko.ext.toc import make_extension as Toc
 
         markdown = Markdown(extensions=[Toc("<div>", "</div>")])
         content = "#### Foobar\n"
         markdown(content)
         toc = markdown.renderer.render_toc()
         assert "<div>\n" in toc
         assert "</div>\n" in toc
@@ -82,16 +82,16 @@
         assert '<div class="highlight">' in self.markdown(content)
 
     def test_render_code_block(self):
         content = '    print("hello")\n'
         assert '<div class="highlight">' in self.markdown(content)
 
     def test_codehilite_options(self):
-        from marko.ext.codehilite import CodeHilite
+        from marko.ext.codehilite import make_extension
 
-        markdown = Markdown(extensions=[CodeHilite(linenos="table")])
+        markdown = Markdown(extensions=[make_extension(linenos="table")])
         content = '```python\nprint("hello")\n```'
         assert '<table class="highlighttable">' in markdown(content)
 
     def test_render_code_block_with_extra(self):
         content = '```python filename="test.py"\nprint("hello")\n```'
         assert '<span class="filename">test.py</span>' in self.markdown(content)
```

### Comparing `marko-1.3.1/tests/test_helpers.py` & `marko-2.0.0/tests/test_helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 
+import marko.source
 from marko import helpers
 
 
 @pytest.mark.parametrize(
     "raw_string",
     [
         "(hello(to)world)",
@@ -27,15 +28,15 @@
     ],
 )
 def test_is_not_paired(raw_string):
     assert not helpers.is_paired(raw_string)
 
 
 def test_source_no_state():
-    source = helpers.Source("hello world")
+    source = marko.source.Source("hello world")
 
     with pytest.raises(RuntimeError, match="Need to push a state first"):
         source.root
 
     with pytest.raises(RuntimeError, match="Need to push a state first"):
         source.state
```

### Comparing `marko-1.3.1/tests/test_latex.py` & `marko-2.0.0/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.1/tests/test_spec.py` & `marko-2.0.0/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `marko-1.3.1/PKG-INFO` & `marko-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: marko
-Version: 1.3.1
+Version: 2.0.0
 Summary: A markdown parser with high extensibility.
+Home-page: https://github.com/frostming/marko
+Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
-Author-email: Frost Ming <mianghong@gmail.com>
-Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: codehilite
-Provides-Extra: toc
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Homepage, https://github.com/frostming/marko
 Project-URL: Documentation, https://marko-py.readthedocs.io
-Project-URL: homepage, https://github.com/frostming/marko
+Requires-Python: >=3.7
+Provides-Extra: toc
+Provides-Extra: codehilite
+Requires-Dist: python-slugify; extra == "toc"
+Requires-Dist: pygments; extra == "codehilite"
 Description-Content-Type: text/markdown
 
 # 𝓜𝓪𝓻𝓴𝓸
 
 > A markdown parser with high extensibility.
 
 [![PyPI](https://img.shields.io/pypi/v/marko.svg?logo=python&logoColor=white)](https://pypi.org/project/marko/)
@@ -29,26 +32,23 @@
 [![Documentation Status](https://img.shields.io/readthedocs/marko-py.svg?logo=readthedocs)](https://marko-py.readthedocs.io/en/latest/?badge=latest)
 [![CommonMark Spec](https://img.shields.io/badge/CommonMark-0.30-blue.svg)][spec]
 
 ![Build Status](https://github.com/frostming/marko/workflows/Tests/badge.svg)
 [![codecov](https://codecov.io/gh/frostming/marko/branch/master/graph/badge.svg)](https://codecov.io/gh/frostming/marko)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/b785f5b3fa7c4d93a02372d31b3f73b1)](https://www.codacy.com/app/frostming/marko?utm_source=github.com&utm_medium=referral&utm_content=frostming/marko&utm_campaign=Badge_Grade)
 
-Marko is a markdown parser written in pure Python that complies with [CommonMark's spec v0.30][spec].
-It is designed to be highly extensible, see [Extensions](#extensions) for details.
+Marko is a pure Python markdown parser that adheres to the specifications of [CommonMark's spec v0.30][spec]. It has been designed with high extensibility in mind, as detailed in the [Extensions](#extensions) section.
 
 Marko requires Python 3.7 or higher.
 
 ## Why Marko
 
-Among all implementations of Python's markdown parser, it is a common issue that user can't easily extend it to add his own features. Furthermore, [Python-Markdown][pymd] and [mistune][mistune] don't comply with CommonMark's spec. It is a good reason for me to develop a new markdown parser.
+Of all the Python markdown parsers available, a common issue is the difficulty for users to add their own features. Additionally, both [Python-Markdown][pymd] and [mistune][mistune] do not comply with CommonMark specifications. This has prompted me to develop a new markdown parser.
 
-Respecting that Marko complies with CommonMark's spec at the same time, which is a super complicated spec, Marko's performance will be affected. However, using a parser
-which doesn't comply with the CommonMark spec may give you unexpected rendered results from time to time.
-A benchmark result shows that Marko is 3 times slower than [Python-Markdown][pymd], but a bit faster than [Commonmark-py][cmpy], much slower than [mistune][mistune]. If performance is a bigger concern to you than spec compliance, you'd better choose another parser.
+Marko's compliance with the complex CommonMark specification can impact its performance. However, using a parser that does not adhere to this spec may result in unexpected rendering outcomes. According to benchmark results, Marko is three times slower than Python-Markdown but slightly faster than Commonmark-py and significantly slower than mistune. If prioritizing performance over spec compliance is crucial for you, it would be best to opt for another parser.
 
 [spec]: https://spec.commonmark.org/0.30/
 [pymd]: https://github.com/waylan/Python-Markdown
 [mistune]: https://github.com/lepture/mistune
 [cmpy]: https://github.com/rtfd/CommonMark-py
 
 ## Use Marko
@@ -71,21 +71,21 @@
 
 ## Extensions
 
 It is super easy to use an extension:
 
 ```python
 from marko import Markdown
-from marko.ext.footnote import Footnote
+from marko.ext.footnote import make_extension
 # Add footnote extension
-markdown = Markdown(extensions=[Footnote])
+markdown = Markdown(extensions=[make_extension()])
 # Or you can just:
 markdown = Markdown(extensions=['footnote'])
 # Alternatively you can register an extension later
-markdown.use(Footnote)
+markdown.use(make_extension())
 ```
 
 An example of using an extension with the command-line version of Marko:
 
 ```
 $ cat this_has_footnote.txt | marko -e footnote > hi_world.html
 ```
@@ -99,8 +99,7 @@
 write your own extension.
 
 ## License
 
 Marko is released under [MIT License](LICENSE)
 
 ## [Change Log](CHANGELOG.md)
-
```

