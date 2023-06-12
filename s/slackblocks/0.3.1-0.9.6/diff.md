# Comparing `tmp/slackblocks-0.3.1.tar.gz` & `tmp/slackblocks-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slackblocks-0.3.1.tar", max compression
+gzip compressed data, was "slackblocks-0.9.6.tar", max compression
```

## Comparing `slackblocks-0.3.1.tar` & `slackblocks-0.9.6.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0     1526 2023-03-24 03:11:58.711082 slackblocks-0.3.1/LICENSE
--rw-r--r--   0        0        0     2443 2023-03-24 03:11:58.711082 slackblocks-0.3.1/README.md
--rw-r--r--   0        0        0     1025 2023-03-24 03:11:58.715082 slackblocks-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      359 2023-03-24 03:11:58.715082 slackblocks-0.3.1/slackblocks/__init__.py
--rw-r--r--   0        0        0     2412 2023-03-24 03:11:58.715082 slackblocks-0.3.1/slackblocks/attachments.py
--rw-r--r--   0        0        0     6701 2023-03-24 03:11:58.715082 slackblocks-0.3.1/slackblocks/blocks.py
--rw-r--r--   0        0        0     5514 2023-03-24 03:11:58.715082 slackblocks-0.3.1/slackblocks/elements.py
--rw-r--r--   0        0        0      131 2023-03-24 03:11:58.715082 slackblocks-0.3.1/slackblocks/errors.py
--rw-r--r--   0        0        0     3392 2023-03-24 03:11:58.715082 slackblocks-0.3.1/slackblocks/messages.py
--rw-r--r--   0        0        0     1937 2023-03-24 03:11:58.715082 slackblocks-0.3.1/slackblocks/modals.py
--rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 slackblocks-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-06-12 15:43:52.399738 slackblocks-0.9.6/LICENSE
+-rw-r--r--   0        0        0     2400 2023-06-12 15:43:52.399738 slackblocks-0.9.6/README.md
+-rw-r--r--   0        0        0     1384 2023-06-12 15:43:52.399738 slackblocks-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0     1115 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/__init__.py
+-rw-r--r--   0        0        0     2743 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/attachments.py
+-rw-r--r--   0        0        0     6922 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/blocks.py
+-rw-r--r--   0        0        0    40245 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/elements.py
+-rw-r--r--   0        0        0      131 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/errors.py
+-rw-r--r--   0        0        0     3456 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/messages.py
+-rw-r--r--   0        0        0      671 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/modals.py
+-rw-r--r--   0        0        0    11977 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/objects.py
+-rw-r--r--   0        0        0     2815 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/utils.py
+-rw-r--r--   0        0        0     3886 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/views.py
+-rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 slackblocks-0.9.6/setup.py
+-rw-r--r--   0        0        0     3630 1970-01-01 00:00:00.000000 slackblocks-0.9.6/PKG-INFO
```

### Comparing `slackblocks-0.3.1/LICENSE` & `slackblocks-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `slackblocks-0.3.1/README.md` & `slackblocks-0.9.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 ![Python Versions](https://img.shields.io/pypi/pyversions/slackblocks)
 ![PyPI](https://img.shields.io/pypi/v/slackblocks?color=yellow&label=PyPI&logo=python&logoColor=white)
 [![Downloads](https://pepy.tech/badge/slackblocks)](https://pepy.tech/project/slackblocks)
 [![Build Status](https://github.com/nicklambourne/slackblocks/actions/workflows/unit-tests.yml/badge.svg?branch=master)](https://github.com/nicklambourne/slackblocks/actions)
 
 ## What is it?
 
-`slackblocks` is a Python API for building messages in the fancy new Slack Block Kit API.
+`slackblocks` is a Python API for building messages in the fancy Slack Block Kit API.
 
-It was created by [Nicholas Lambourne](https://github.com/nicklambourne) for the [UQCS Slack Bot](https://github.com/UQComputingSociety/uqcsbot) because he hates writing JSON.
-
-N.B: This is still WIP software and some of the more tricky interactive Block elements have yet to be implemented.
+It was created by [Nicholas Lambourne](https://github.com/nicklambourne) for the [UQCS Slack Bot](https://github.com/UQComputingSociety/uqcsbot) because he hates writing JSON, naturally this project has subsequently involved writing more JSON than if he'd done the original task by hand.
 
 ## Requirements
-`slackblocks` requires Python >= 3.6.
+`slackblocks` requires Python >= 3.7.
 
 As of version 0.1.0 it has no dependencies outside the Python standard library.
 
 ## Installation
 
 ```bash
 pip install slackblocks
@@ -44,16 +42,15 @@
     "mrkdwn": true,
     "blocks": [
         {
             "type": "section",
             "block_id": "992ceb6b-9ad4-496b-b8e6-1bd8a632e8b3",
             "text": {
                 "type": "mrkdwn",
-                "text": "Hello, world!",
-                "verbatim": false
+                "text": "Hello, world!"
             }
         }
     ]
 }
 ```
 Which can be sent as payload to the Slack message API HTTP endpoints.
```

### Comparing `slackblocks-0.3.1/pyproject.toml` & `slackblocks-0.9.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 [tool.poetry]
 name = "slackblocks"
-version = "0.3.1"
+version = "0.9.6"
 description = "Python wrapper for the Slack Blocks API"
-authors = ["Nicholas Lambourne <dev@ndl.im>"]
+authors = [
+    "Nicholas Lambourne <dev@ndl.im>",
+]
+maintainers = [
+    "Nicholas Lambourne <dev@ndl.im>",
+]
+homepage = "https://github.com/nicklambourne/slackblocks"
+repository = "https://github.com/nicklambourne/slackblocks"
 license = "BSD-3-Clause"
 readme = "README.md"
+keywords = [
+    "slackblocks", 
+    "slack", 
+    "messaging", 
+    "message generation", 
+    "slack blocks", 
+    "blocks",
+]
 classifiers=[
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Typing :: Typed",
     "Topic :: Communications :: Chat"
 ]
 exclude = ["test/**", "docs/**"]
 
 [tool.poetry.dependencies]
-python = "^3.7.0"
+python = ">=3.7.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 twine = "^4.0.2"
 wheel = "^0.40.0"
 slackclient = "^2.9.4" 
 black = "^23.1.0"
```

### Comparing `slackblocks-0.3.1/slackblocks/attachments.py` & `slackblocks-0.9.6/slackblocks/attachments.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,19 @@
+"""
+Secondary (less important) content can be attached using the deprecated
+attachments API.
+See: https://api.slack.com/reference/messaging/attachments
+"""
 from enum import Enum
 from json import dumps
 from typing import Any, Dict, List, Optional, Union
-from .blocks import Block
-from .errors import InvalidUsageError
+
+from slackblocks.blocks import Block
+from slackblocks.errors import InvalidUsageError
+from slackblocks.utils import coerce_to_list, is_hex
 
 
 class Color(Enum):
     """
     Color utility class for use with the Slack secondary attachments API.
     """
 
@@ -17,14 +24,17 @@
     BLUE = "#0000ff"
     YELLOW = "#ffff00"
     GREEN = "#00ff00"
     ORANGE = "#ff8800"
     PURPLE = "#8800ff"
     BLACK = "#000000"
 
+    def __repr__(self) -> str:
+        return f"<slackblocks Color {self.name}: {self.value}>"
+
 
 class Field:
     """
     Field text objects for use with Slack's secondary attachment API.
     """
 
     def __init__(
@@ -52,32 +62,29 @@
     Secondary content can be attached to messages to include lower priority content
      - content that doesn't necessarily need to be seen to appreciate the intent of
     the message, but perhaps adds further context or additional information.
     """
 
     def __init__(
         self,
-        blocks: Optional[Union[List[Block], Block]] = None,
+        blocks: Optional[Union[Block, List[Block]]] = None,
         color: Optional[Union[str, Color]] = None,
     ):
-        if isinstance(blocks, List):
-            self.blocks = blocks
-        elif isinstance(blocks, Block):
-            self.blocks = [
-                blocks,
-            ]
-        else:
-            self.blocks = None
+        self.blocks = coerce_to_list(blocks, Block, allow_none=True)
         if type(color) is Color:
             self.color = color.value
         elif type(color) is str:
-            if len(color) == 7 and color.startswith("#"):
+            if len(color) == 7 and color.startswith("#") and is_hex(color[1:]):
                 self.color = color
+            elif len(color) == 6 and is_hex(color):
+                self.color = f"#{color}"
             else:
-                raise InvalidUsageError("Color must be a valid hex code (e.g. #ffffff)")
+                raise InvalidUsageError(
+                    "Color must be a valid hex code (e.g. `#ffffff`)"
+                )
         else:
             self.color = None
 
     def _resolve(self) -> Dict[str, Any]:
         attachment = dict()
         if self.blocks:
             attachment["blocks"] = [block._resolve() for block in self.blocks]
```

### Comparing `slackblocks-0.3.1/slackblocks/blocks.py` & `slackblocks-0.9.6/slackblocks/blocks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,28 @@
-from abc import abstractmethod, ABC
+"""
+Blocks are a series of components that can be combined to create rich and
+interactive messages.
+See: https://api.slack.com/reference/block-kit/blocks?ref=bk
+"""
+from abc import ABC, abstractmethod
 from enum import Enum
 from json import dumps
 from typing import Any, Dict, List, Optional, Union
 from uuid import uuid4
-from .elements import Element, ElementType, Text, TextType
-from .errors import InvalidUsageError
+
+from slackblocks.elements import Element, ElementType
+from slackblocks.errors import InvalidUsageError
+from slackblocks.objects import (
+    CompositionObject,
+    CompositionObjectType,
+    Text,
+    TextLike,
+    TextType,
+)
+from slackblocks.utils import coerce_to_list
 
 
 class BlockType(Enum):
     """
     Convenience class for identifying the different types of blocks available
     in the Slack Blocks API and their programmatic names.
     """
@@ -42,152 +56,79 @@
     def _resolve(self) -> Dict[str, any]:
         pass
 
     def __repr__(self) -> str:
         return dumps(self._resolve(), indent=4)
 
 
-class SectionBlock(Block):
-    """
-    A section is one of the most flexible blocks available -
-    it can be used as a simple text block, in combination with text fields,
-    or side-by-side with any of the available block elements.
-    """
-
-    def __init__(
-        self,
-        text: Optional[Union[str, Text]] = None,
-        block_id: Optional[str] = None,
-        fields: Optional[List[Text]] = None,
-        accessory: Optional[Element] = None,
-    ):
-        super().__init__(type_=BlockType.SECTION, block_id=block_id)
-        if text:
-            if type(text) is Text:
-                self.text = text
-            else:
-                self.text = Text(text)
-        else:
-            self.text = text
-        self.fields = fields
-        self.accessory = accessory
-
-    def _resolve(self) -> Dict[str, Any]:
-        section = self._attributes()
-        if self.text:
-            section["text"] = self.text._resolve()
-        if self.fields:
-            section["fields"] = [field._resolve() for field in self.fields]
-        if self.accessory:
-            section["accessory"] = self.accessory._resolve()
-        return section
-
-
-class DividerBlock(Block):
-    """
-    A content divider, like an <hr>, to split up different blocks inside of
-    a message. The divider block is nice and neat, requiring only a type.
-    """
-
-    def __init__(self, block_id: Optional[str] = None):
-        super().__init__(type_=BlockType.DIVIDER, block_id=block_id)
-
-    def _resolve(self):
-        return self._attributes()
-
-
-class ImageBlock(Block):
-    """
-    A simple image block, designed to make those cat photos really pop.
-    """
-
-    def __init__(
-        self,
-        image_url: str,
-        alt_text: Optional[str] = "",
-        title: Optional[Union[Text, str]] = None,
-        block_id: Optional[str] = None,
-    ):
-        super().__init__(type_=BlockType.IMAGE, block_id=block_id)
-        self.image_url = image_url
-        self.alt_text = alt_text
-        if title and type(title) is Text:
-            if title.text_type == TextType.MARKDOWN:
-                self.title = Text(
-                    text=title.text,
-                    type_=TextType.PLAINTEXT,
-                    emoji=title.emoji,
-                    verbatim=title.verbatim,
-                )
-            else:
-                self.title = title
-        elif title:
-            self.title = Text(text=title, type_=TextType.PLAINTEXT)
-        else:
-            self.title = Text(text=" ", type_=TextType.PLAINTEXT)
-
-    def _resolve(self) -> Dict[str, Any]:
-        image = self._attributes()
-        image["image_url"] = self.image_url
-        image["alt_text"] = self.alt_text
-        if self.title:
-            image["title"] = self.title._resolve()
-        return image
-
-
 class ActionsBlock(Block):
     """
     A block that is used to hold interactive elements.
     """
 
     def __init__(
-        self, elements: Optional[List[Element]] = None, block_id: Optional[str] = None
+        self,
+        elements: Optional[List[Union[Element, CompositionObject]]] = None,
+        block_id: Optional[str] = None,
     ):
         super().__init__(type_=BlockType.ACTIONS, block_id=block_id)
-        if isinstance(elements, Element):
-            self.elements = [
-                elements,
-            ]
-        elif isinstance(elements, list) and all(
-            [isinstance(el, Element) for el in elements]
-        ):
-            self.elements = elements
+        self.elements = coerce_to_list(
+            elements, (Element, CompositionObject), allow_none=True, max_size=25
+        )
 
     def _resolve(self):
         actions = self._attributes()
         actions["elements"] = [element._resolve() for element in self.elements]
         return actions
 
 
 class ContextBlock(Block):
     """
     Displays message context, which can include both images and text.
     """
 
     def __init__(
-        self, elements: Optional[List[Element]] = None, block_id: Optional[str] = None
+        self,
+        elements: Optional[List[Union[Element, CompositionObjectType]]] = None,
+        block_id: Optional[str] = None,
     ):
         super().__init__(type_=BlockType.CONTEXT, block_id=block_id)
         self.elements = []
         for element in elements:
-            if element.type == ElementType.TEXT or element.type == ElementType.IMAGE:
+            if (
+                element.type == CompositionObjectType.TEXT
+                or element.type == ElementType.IMAGE
+            ):
                 self.elements.append(element)
             else:
                 raise InvalidUsageError(
-                    "Context blocks can only hold image and text elements"
+                    f"Context blocks can only hold image and text elements, not {element.type}"
                 )
         if len(self.elements) > 10:
             raise InvalidUsageError("Context blocks can hold a maximum of ten elements")
 
     def _resolve(self) -> Dict[str, any]:
         context = self._attributes()
         context["elements"] = [element._resolve() for element in self.elements]
         return context
 
 
+class DividerBlock(Block):
+    """
+    A content divider, like an <hr>, to split up different blocks inside of
+    a message. The divider block is nice and neat, requiring only a type.
+    """
+
+    def __init__(self, block_id: Optional[str] = None):
+        super().__init__(type_=BlockType.DIVIDER, block_id=block_id)
+
+    def _resolve(self):
+        return self._attributes()
+
+
 class FileBlock(Block):
     """
     Displays a remote file.
     """
 
     def __init__(self, external_id: str, source: str, block_id: Optional[str]):
         super().__init__(type_=BlockType.FILE, block_id=block_id)
@@ -213,7 +154,76 @@
         else:
             self.text = Text(text, type_=TextType.PLAINTEXT, verbatim=False)
 
     def _resolve(self) -> Dict[str, any]:
         header = self._attributes()
         header["text"] = self.text._resolve()
         return header
+
+
+class ImageBlock(Block):
+    """
+    A simple image block, designed to make those cat photos really pop.
+    """
+
+    def __init__(
+        self,
+        image_url: str,
+        alt_text: Optional[str] = "",
+        title: Optional[Union[Text, str]] = None,
+        block_id: Optional[str] = None,
+    ):
+        super().__init__(type_=BlockType.IMAGE, block_id=block_id)
+        self.image_url = image_url
+        self.alt_text = alt_text
+        if title and type(title) is Text:
+            if title.text_type == TextType.MARKDOWN:
+                self.title = Text(
+                    text=title.text,
+                    type_=TextType.PLAINTEXT,
+                    emoji=title.emoji,
+                    verbatim=title.verbatim,
+                )
+            else:
+                self.title = title
+        elif title:
+            self.title = Text(text=title, type_=TextType.PLAINTEXT)
+        else:
+            self.title = Text(text=" ", type_=TextType.PLAINTEXT)
+
+    def _resolve(self) -> Dict[str, Any]:
+        image = self._attributes()
+        image["image_url"] = self.image_url
+        image["alt_text"] = self.alt_text
+        if self.title:
+            image["title"] = self.title._resolve()
+        return image
+
+
+class SectionBlock(Block):
+    """
+    A section is one of the most flexible blocks available -
+    it can be used as a simple text block, in combination with text fields,
+    or side-by-side with any of the available block elements.
+    """
+
+    def __init__(
+        self,
+        text: Optional[TextLike] = None,
+        block_id: Optional[str] = None,
+        fields: Optional[List[Text]] = None,
+        accessory: Optional[Element] = None,
+    ):
+        super().__init__(type_=BlockType.SECTION, block_id=block_id)
+        self.text = Text.to_text(text)
+        self.fields = fields
+        self.accessory = accessory
+
+    def _resolve(self) -> Dict[str, Any]:
+        section = self._attributes()
+        if self.text:
+            section["text"] = self.text._resolve()
+        if self.fields:
+            section["fields"] = [field._resolve() for field in self.fields]
+        if self.accessory:
+            section["accessory"] = self.accessory._resolve()
+        return section
```

### Comparing `slackblocks-0.3.1/slackblocks/messages.py` & `slackblocks-0.9.6/slackblocks/messages.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
+"""
+Messages are the core unit of Slack messaging functionality. They can be
+built out using blocks, elements and objects.
+See: https://api.slack.com/messaging
+"""
 from json import dumps
 from typing import Any, Dict, List, Optional, Union
+
+from slackblocks.utils import coerce_to_list
+
 from .attachments import Attachment
 from .blocks import Block
 
 
 class BaseMessage:
     """
     Abstract class for shared functionality between Messages and
-    Acknowledgement responses.
+    MessageResponses.
     """
 
     def __init__(
         self,
         channel: Optional[str] = None,
         text: Optional[str] = "",
         blocks: Optional[Union[List[Block], Block]] = None,
         attachments: Optional[List[Attachment]] = None,
         thread_ts: Optional[str] = None,
         mrkdwn: bool = True,
     ):
-        if isinstance(blocks, List):
-            self.blocks = blocks
-        elif isinstance(blocks, Block):
-            self.blocks = [
-                blocks,
-            ]
-        else:
-            self.blocks = None
+        self.blocks = coerce_to_list(blocks, class_=Block, allow_none=True)
         self.channel = channel
         self.text = text
         self.attachments = attachments or []
         self.thread_ts = thread_ts
         self.mrkdwn = mrkdwn
 
     def _resolve(self) -> Dict[str, Any]:
@@ -59,15 +60,15 @@
     def __repr__(self) -> str:
         return self.json()
 
     def __getitem__(self, item):
         return self._resolve()[item]
 
     def keys(self) -> Dict[str, Any]:
-        return self._resolve()
+        return self._resolve().keys()
 
 
 class Message(BaseMessage):
     """
     A Slack message object that can be converted to a JSON string for use with
     the Slack message API.
     """
```

### Comparing `slackblocks-0.3.1/PKG-INFO` & `slackblocks-0.9.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 Metadata-Version: 2.1
 Name: slackblocks
-Version: 0.3.1
+Version: 0.9.6
 Summary: Python wrapper for the Slack Blocks API
+Home-page: https://github.com/nicklambourne/slackblocks
 License: BSD-3-Clause
+Keywords: slackblocks,slack,messaging,message generation,slack blocks,blocks
 Author: Nicholas Lambourne
 Author-email: dev@ndl.im
-Requires-Python: >=3.7.0,<4.0.0
+Maintainer: Nicholas Lambourne
+Maintainer-email: dev@ndl.im
+Requires-Python: >=3.7.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Communications :: Chat
 Classifier: Typing :: Typed
+Project-URL: Repository, https://github.com/nicklambourne/slackblocks
 Description-Content-Type: text/markdown
 
 # slackblocks <img src="https://github.com/nicklambourne/slackblocks/raw/master/docs/img/sb.png" align="right" width="250px"/>
 
 ![PyPI - License](https://img.shields.io/pypi/l/slackblocks)
 ![Python Versions](https://img.shields.io/pypi/pyversions/slackblocks)
 ![PyPI](https://img.shields.io/pypi/v/slackblocks?color=yellow&label=PyPI&logo=python&logoColor=white)
 [![Downloads](https://pepy.tech/badge/slackblocks)](https://pepy.tech/project/slackblocks)
 [![Build Status](https://github.com/nicklambourne/slackblocks/actions/workflows/unit-tests.yml/badge.svg?branch=master)](https://github.com/nicklambourne/slackblocks/actions)
 
 ## What is it?
 
-`slackblocks` is a Python API for building messages in the fancy new Slack Block Kit API.
-
-It was created by [Nicholas Lambourne](https://github.com/nicklambourne) for the [UQCS Slack Bot](https://github.com/UQComputingSociety/uqcsbot) because he hates writing JSON.
+`slackblocks` is a Python API for building messages in the fancy Slack Block Kit API.
 
-N.B: This is still WIP software and some of the more tricky interactive Block elements have yet to be implemented.
+It was created by [Nicholas Lambourne](https://github.com/nicklambourne) for the [UQCS Slack Bot](https://github.com/UQComputingSociety/uqcsbot) because he hates writing JSON, naturally this project has subsequently involved writing more JSON than if he'd done the original task by hand.
 
 ## Requirements
-`slackblocks` requires Python >= 3.6.
+`slackblocks` requires Python >= 3.7.
 
 As of version 0.1.0 it has no dependencies outside the Python standard library.
 
 ## Installation
 
 ```bash
 pip install slackblocks
@@ -68,16 +72,15 @@
     "mrkdwn": true,
     "blocks": [
         {
             "type": "section",
             "block_id": "992ceb6b-9ad4-496b-b8e6-1bd8a632e8b3",
             "text": {
                 "type": "mrkdwn",
-                "text": "Hello, world!",
-                "verbatim": false
+                "text": "Hello, world!"
             }
         }
     ]
 }
 ```
 Which can be sent as payload to the Slack message API HTTP endpoints.
```

