# Comparing `tmp/guitk-0.4.1.tar.gz` & `tmp/guitk-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guitk-0.4.1.tar", max compression
+gzip compressed data, was "guitk-0.4.2.tar", max compression
```

## Comparing `guitk-0.4.1.tar` & `guitk-0.4.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1070 2021-03-08 04:36:45.000000 guitk-0.4.1/LICENSE
--rw-r--r--   0        0        0     9589 2023-06-05 13:48:02.322455 guitk-0.4.1/README.md
--rw-r--r--   0        0        0     2820 2023-06-05 13:57:04.928578 guitk-0.4.1/guitk/__init__.py
--rw-r--r--   0        0        0    12161 2023-06-05 13:44:42.707599 guitk-0.4.1/guitk/__main__.py
--rw-r--r--   0        0        0     1968 2023-06-05 13:44:42.707839 guitk-0.4.1/guitk/_debug.py
--rw-r--r--   0        0        0     2430 2023-06-05 13:44:42.708070 guitk-0.4.1/guitk/_on.py
--rw-r--r--   0        0        0    10707 2023-06-05 13:44:42.708422 guitk-0.4.1/guitk/basewidget.py
--rw-r--r--   0        0        0      294 2023-06-05 13:44:42.708769 guitk-0.4.1/guitk/constants.py
--rw-r--r--   0        0        0    24190 2023-06-05 13:44:42.709103 guitk-0.4.1/guitk/containers.py
--rw-r--r--   0        0        0     1306 2023-06-05 13:44:42.709339 guitk-0.4.1/guitk/debugwindow.py
--rw-r--r--   0        0        0     2437 2023-06-05 13:44:42.709558 guitk-0.4.1/guitk/events.py
--rw-r--r--   0        0        0    22563 2023-06-05 13:44:42.709859 guitk-0.4.1/guitk/frame.py
--rw-r--r--   0        0        0     4723 2023-06-05 13:44:42.710063 guitk-0.4.1/guitk/image.py
--rw-r--r--   0        0        0     5510 2023-06-05 13:44:42.710655 guitk-0.4.1/guitk/layout.py
--rw-r--r--   0        0        0     3448 2023-06-05 13:44:42.710932 guitk-0.4.1/guitk/menu.py
--rw-r--r--   0        0        0     2873 2023-06-05 13:44:42.711259 guitk-0.4.1/guitk/redirect.py
--rw-r--r--   0        0        0     1618 2023-06-05 13:44:42.711438 guitk-0.4.1/guitk/spacer.py
--rw-r--r--   0        0        0    11449 2023-06-05 13:44:42.711640 guitk-0.4.1/guitk/tk_text.py
--rw-r--r--   0        0        0     2523 2023-06-05 13:44:42.712010 guitk-0.4.1/guitk/tkroot.py
--rw-r--r--   0        0        0     8686 2023-06-05 13:44:42.712276 guitk-0.4.1/guitk/tooltips.py
--rw-r--r--   0        0        0    13189 2023-06-05 13:44:42.712537 guitk-0.4.1/guitk/ttk_button.py
--rw-r--r--   0        0        0     5088 2023-06-05 13:44:42.712731 guitk-0.4.1/guitk/ttk_checkbutton.py
--rw-r--r--   0        0        0     5717 2023-06-05 13:44:42.713001 guitk-0.4.1/guitk/ttk_combobox.py
--rw-r--r--   0        0        0    10384 2023-06-05 13:44:42.713197 guitk-0.4.1/guitk/ttk_entry.py
--rw-r--r--   0        0        0     7596 2023-06-05 13:44:42.713434 guitk-0.4.1/guitk/ttk_label.py
--rw-r--r--   0        0        0     8873 2023-06-05 13:44:42.713652 guitk-0.4.1/guitk/ttk_notebook.py
--rw-r--r--   0        0        0     8883 2023-06-05 13:44:42.714581 guitk-0.4.1/guitk/ttk_panedwindow.py
--rw-r--r--   0        0        0     4898 2023-06-05 13:44:42.714718 guitk-0.4.1/guitk/ttk_progressbar.py
--rw-r--r--   0        0        0     6148 2023-06-05 13:44:42.714850 guitk-0.4.1/guitk/ttk_radiobutton.py
--rw-r--r--   0        0        0     7161 2023-06-05 13:44:42.714992 guitk-0.4.1/guitk/ttk_scale.py
--rw-r--r--   0        0        0     2943 2023-06-05 13:44:42.715116 guitk-0.4.1/guitk/ttk_separator.py
--rw-r--r--   0        0        0     7801 2023-06-05 13:44:42.715319 guitk-0.4.1/guitk/ttk_spinbox.py
--rw-r--r--   0        0        0    12619 2023-06-05 13:44:42.715472 guitk-0.4.1/guitk/ttk_treeview.py
--rw-r--r--   0        0        0      771 2023-06-05 13:44:42.715589 guitk-0.4.1/guitk/types.py
--rw-r--r--   0        0        0     2527 2023-06-05 13:44:42.715787 guitk-0.4.1/guitk/utils.py
--rw-r--r--   0        0        0     9333 2023-06-05 13:44:42.716003 guitk-0.4.1/guitk/widget.py
--rw-r--r--   0        0        0    18725 2023-06-05 13:44:42.716457 guitk-0.4.1/guitk/window.py
--rw-r--r--   0        0        0      769 2023-06-05 13:57:04.928888 guitk-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    10421 1970-01-01 00:00:00.000000 guitk-0.4.1/setup.py
--rw-r--r--   0        0        0    10161 1970-01-01 00:00:00.000000 guitk-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2021-03-08 04:36:45.000000 guitk-0.4.2/LICENSE
+-rw-r--r--   0        0        0    10040 2023-06-12 13:30:09.123098 guitk-0.4.2/README.md
+-rw-r--r--   0        0        0     2880 2023-06-12 13:30:09.124344 guitk-0.4.2/guitk/__init__.py
+-rw-r--r--   0        0        0    12161 2023-06-05 13:44:42.707599 guitk-0.4.2/guitk/__main__.py
+-rw-r--r--   0        0        0     1968 2023-06-05 13:44:42.707839 guitk-0.4.2/guitk/_debug.py
+-rw-r--r--   0        0        0     2430 2023-06-05 13:44:42.708070 guitk-0.4.2/guitk/_on.py
+-rw-r--r--   0        0        0    10707 2023-06-05 13:44:42.708422 guitk-0.4.2/guitk/basewidget.py
+-rw-r--r--   0        0        0      317 2023-06-12 13:27:03.430985 guitk-0.4.2/guitk/constants.py
+-rw-r--r--   0        0        0    24190 2023-06-05 13:44:42.709103 guitk-0.4.2/guitk/containers.py
+-rw-r--r--   0        0        0     1306 2023-06-05 13:44:42.709339 guitk-0.4.2/guitk/debugwindow.py
+-rw-r--r--   0        0        0     2437 2023-06-11 15:11:10.947825 guitk-0.4.2/guitk/events.py
+-rw-r--r--   0        0        0    22563 2023-06-05 13:44:42.709859 guitk-0.4.2/guitk/frame.py
+-rw-r--r--   0        0        0     4723 2023-06-05 13:44:42.710063 guitk-0.4.2/guitk/image.py
+-rw-r--r--   0        0        0     5510 2023-06-05 13:44:42.710655 guitk-0.4.2/guitk/layout.py
+-rw-r--r--   0        0        0    17405 2023-06-12 13:27:03.431329 guitk-0.4.2/guitk/menu.py
+-rw-r--r--   0        0        0     2873 2023-06-05 13:44:42.711259 guitk-0.4.2/guitk/redirect.py
+-rw-r--r--   0        0        0     1618 2023-06-05 13:44:42.711438 guitk-0.4.2/guitk/spacer.py
+-rw-r--r--   0        0        0    11449 2023-06-05 13:44:42.711640 guitk-0.4.2/guitk/tk_text.py
+-rw-r--r--   0        0        0     2523 2023-06-05 13:44:42.712010 guitk-0.4.2/guitk/tkroot.py
+-rw-r--r--   0        0        0     8686 2023-06-05 13:44:42.712276 guitk-0.4.2/guitk/tooltips.py
+-rw-r--r--   0        0        0    13189 2023-06-11 02:55:57.103304 guitk-0.4.2/guitk/ttk_button.py
+-rw-r--r--   0        0        0     5088 2023-06-05 13:44:42.712731 guitk-0.4.2/guitk/ttk_checkbutton.py
+-rw-r--r--   0        0        0     5717 2023-06-05 13:44:42.713001 guitk-0.4.2/guitk/ttk_combobox.py
+-rw-r--r--   0        0        0    10384 2023-06-05 13:44:42.713197 guitk-0.4.2/guitk/ttk_entry.py
+-rw-r--r--   0        0        0     7596 2023-06-05 13:44:42.713434 guitk-0.4.2/guitk/ttk_label.py
+-rw-r--r--   0        0        0     8873 2023-06-05 13:44:42.713652 guitk-0.4.2/guitk/ttk_notebook.py
+-rw-r--r--   0        0        0     8883 2023-06-05 13:44:42.714581 guitk-0.4.2/guitk/ttk_panedwindow.py
+-rw-r--r--   0        0        0     4898 2023-06-05 13:44:42.714718 guitk-0.4.2/guitk/ttk_progressbar.py
+-rw-r--r--   0        0        0     6148 2023-06-05 13:44:42.714850 guitk-0.4.2/guitk/ttk_radiobutton.py
+-rw-r--r--   0        0        0     7161 2023-06-05 13:44:42.714992 guitk-0.4.2/guitk/ttk_scale.py
+-rw-r--r--   0        0        0     2943 2023-06-05 13:44:42.715116 guitk-0.4.2/guitk/ttk_separator.py
+-rw-r--r--   0        0        0     7801 2023-06-05 13:44:42.715319 guitk-0.4.2/guitk/ttk_spinbox.py
+-rw-r--r--   0        0        0    12619 2023-06-05 13:44:42.715472 guitk-0.4.2/guitk/ttk_treeview.py
+-rw-r--r--   0        0        0      771 2023-06-05 13:44:42.715589 guitk-0.4.2/guitk/types.py
+-rw-r--r--   0        0        0     2527 2023-06-05 13:44:42.715787 guitk-0.4.2/guitk/utils.py
+-rw-r--r--   0        0        0     9333 2023-06-05 13:44:42.716003 guitk-0.4.2/guitk/widget.py
+-rw-r--r--   0        0        0    19055 2023-06-12 13:27:03.431732 guitk-0.4.2/guitk/window.py
+-rw-r--r--   0        0        0      804 2023-06-12 13:30:09.124615 guitk-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    10884 1970-01-01 00:00:00.000000 guitk-0.4.2/setup.py
+-rw-r--r--   0        0        0    10612 1970-01-01 00:00:00.000000 guitk-0.4.2/PKG-INFO
```

### Comparing `guitk-0.4.1/LICENSE` & `guitk-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/README.md` & `guitk-0.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,26 @@
 
 GUITk allows you to build complete GUI applications with a few lines of code. GUITk makes it easy to layout your GUI elements and respond to events using a declarative syntax. Because GUITk is built on top of tkinter, you can access the underlying tkinter API if you need to but for many use cases, you can build your GUI without needing to know much about tkinter.
 
 GUITk apps are built by subclasses the `guitk.Window` class. Your GUI elements are layed out using a `guitk.HLayout` (horizontal layout) or `guitk.VLayout` (vertical layout) object which takes care of placing all widgets in the window using a declarative syntax. This is much simpler than using the underlying tkinter [grid manager](https://tkdocs.com/shipman/grid.html) or [pack](https://dafarry.github.io/tkinterbook/pack.htm) geometry managers.
 
 GUITk is in alpha stage but is in constant development so check back frequently if this interests you or open an issue to start a conversation about what pain points this project could help you solve!
 
+Documentation is available at [GUITk](https://rhettbull.github.io/guitk/).
+
 ## Code Example
 
-### Simple VLayout
+### Simple HLayout
 
-![hello.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/hello.py.png "Hello World example")
+<!--[[[cog
+import os
+os.system("python3 utils/screenshot.py examples/hello.py HelloWindow docs/images/hello.py.png --overwrite")
+]]]-->
+<!--[[[end]]]-->
+![hello.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/docs/images/hello.py.png "Hello World example")
 
 ```python
 """Simple Hello World example using guitk """
 
 import guitk as ui
 
 
@@ -52,22 +59,26 @@
 
 ## Motivation
 
 The goal of GUITk is to make it very easy to create simple and attractive GUI apps with python. It borrows ideas from several other libraries include [PySimpleGUI](https://www.pysimplegui.org/en/latest/), [SwiftUI](https://developer.apple.com/documentation/swiftui), [textual](https://github.com/Textualize/textual), and [applepy](https://github.com/eduardohleite/applepy). GUITk builds on [tkinter](https://docs.python.org/3/library/tkinter.html) which ships with the Python standard library and works across many platforms. tkinter is a mature and powerful GUI framework but requires a fair bit of boiler plate and understanding of the underlying framework to use effectively. GUITk attempts to simplify this by providing a higher level interface to tkinter while still allowing you to access the underlying tkinter API if you need to.
 
 Though you can build simple apps without knowing much about tkinter, GUITk is not intended to fully abstract away the tkinter interface. A basic understanding of tkinter will be helpful when building with GUITk. I highly recommend Mark Roseman's excellent [Modern Tkinter for Busy Python Developers](https://tkdocs.com/book.html) book as a starting point.
 
-
 ## Installation
 
 * `python3 -m pip install guitk`
 
 ## Anatomy of a guitk program
 
-![hello2.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/hello2.py.png "Hello World example")
+<!--[[[cog
+import os
+os.system("python3 utils/screenshot.py examples/hello2.py HelloWorld docs/images/hello2.py.png --overwrite")
+]]]-->
+<!--[[[end]]]-->
+![hello2.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/docs/images/hello2.py.png "Hello World example")
 
 ```python
 """Hello World example using guitk """
 
 import guitk as ui
 
 
@@ -155,15 +166,15 @@
     # instantiate your Window class and run it
     name = HelloWorld().run()
     print(f"Hello {name}")
 ```
 
 ## Documentation
 
-Not much documentation at this point.  Take a look at the [examples](https://github.com/RhetTbull/guitk/tree/main/examples) directory for a number of self-documenting examples on use of various widgets.
+Not much documentation at this point but there's a start [here](https://rhettbull.github.io/guitk/).  Take a look at the [examples](https://github.com/RhetTbull/guitk/tree/main/examples) directory for a number of self-documenting examples on use of various widgets.
 
 ## Testing
 
 There are currently no automated tests as I haven't figured out how to do these with tkinter. I am working on adding tests and there are several tests that run with `pytest` in the `tests` directory.  These are not automated and require user interaction.
 
 You can also run `python3 -m guitk` which opens a window with examples of all the widgets. I find this useful for quick testing of layout and widget behavior.
 
@@ -182,16 +193,16 @@
 * [x] Radiobutton
 * [x] Text
 * [x] ScrolledText
 * [x] Treeview
 * [x] Listbox
 * [x] Combobox
 * [x] Spinner
-* [ ] Other widgets
-* [ ] Menus
+* [x] Other widgets
+* [x] Menus
 * [x] Tooltips
 * [ ] Documentation
 * [x] Add docstrings
 * [x] Add type hints to public API
 * [ ] Tests
 
 ## License
```

### Comparing `guitk-0.4.1/guitk/__init__.py` & `guitk-0.4.2/guitk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .basewidget import BaseWidget
 from .containers import HGrid, HStack, VGrid, VStack
 from .debugwindow import DebugWindow
 from .events import Event, EventCommand, EventType
 from .frame import Frame, LabelFrame
 from .image import Image
 from .layout import HLayout, VLayout
-from .menu import Command, Menu
+from .menu import Command, Menu, MenuBar, MenuSeparator
 from .spacer import HSpacer, VSpacer
 from .tk_text import Output, Text
 from .tkroot import *
 from .ttk_button import BrowseDirectoryButton, BrowseFileButton, Button
 from .ttk_checkbutton import Checkbutton, CheckButton
 from .ttk_combobox import Combobox, ComboBox
 from .ttk_entry import Entry, LabelEntry
@@ -45,15 +45,15 @@
 from .ttk_scale import Scale
 from .ttk_separator import HSeparator, VSeparator
 from .ttk_spinbox import Spinbox, SpinBox
 from .ttk_treeview import Listbox, ListBox, Treeview, TreeView
 from .widget import Widget, widget_class_factory
 from .window import Window
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 __author__ = "Rhet Turnbull"
 
 __all__ = [
     "BaseWidget",
     "BrowseDirectoryButton",
     "BrowseFileButton",
     "Button",
@@ -81,14 +81,16 @@
     "LabelEntry",
     "LabelFrame",
     "LinkLabel",
     "Linklabel",
     "ListBox",
     "Listbox",
     "Menu",
+    "MenuBar",
+    "MenuSeparator",
     "NoteBook",
     "Notebook",
     "Output",
     "PROGRESS_DETERMINATE",
     "PROGRESS_INDETERMINATE",
     "PanedWindow",
     "Panedwindow",
```

### Comparing `guitk-0.4.1/guitk/__main__.py` & `guitk-0.4.2/guitk/__main__.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/_debug.py` & `guitk-0.4.2/guitk/_debug.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/_on.py` & `guitk-0.4.2/guitk/_on.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/basewidget.py` & `guitk-0.4.2/guitk/basewidget.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/containers.py` & `guitk-0.4.2/guitk/containers.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/debugwindow.py` & `guitk-0.4.2/guitk/debugwindow.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/events.py` & `guitk-0.4.2/guitk/events.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/frame.py` & `guitk-0.4.2/guitk/frame.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/image.py` & `guitk-0.4.2/guitk/image.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/layout.py` & `guitk-0.4.2/guitk/layout.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/redirect.py` & `guitk-0.4.2/guitk/redirect.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/spacer.py` & `guitk-0.4.2/guitk/spacer.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/tk_text.py` & `guitk-0.4.2/guitk/tk_text.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/tkroot.py` & `guitk-0.4.2/guitk/tkroot.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/tooltips.py` & `guitk-0.4.2/guitk/tooltips.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/ttk_button.py` & `guitk-0.4.2/guitk/ttk_button.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/ttk_checkbutton.py` & `guitk-0.4.2/guitk/ttk_checkbutton.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/ttk_combobox.py` & `guitk-0.4.2/guitk/ttk_combobox.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/ttk_entry.py` & `guitk-0.4.2/guitk/ttk_entry.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/ttk_label.py` & `guitk-0.4.2/guitk/ttk_label.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/ttk_notebook.py` & `guitk-0.4.2/guitk/ttk_notebook.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/ttk_panedwindow.py` & `guitk-0.4.2/guitk/ttk_panedwindow.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/ttk_progressbar.py` & `guitk-0.4.2/guitk/ttk_progressbar.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/ttk_radiobutton.py` & `guitk-0.4.2/guitk/ttk_radiobutton.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/ttk_scale.py` & `guitk-0.4.2/guitk/ttk_scale.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/ttk_separator.py` & `guitk-0.4.2/guitk/ttk_separator.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/ttk_spinbox.py` & `guitk-0.4.2/guitk/ttk_spinbox.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/ttk_treeview.py` & `guitk-0.4.2/guitk/ttk_treeview.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/types.py` & `guitk-0.4.2/guitk/types.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/utils.py` & `guitk-0.4.2/guitk/utils.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/widget.py` & `guitk-0.4.2/guitk/widget.py`

 * *Files identical despite different names*

### Comparing `guitk-0.4.1/guitk/window.py` & `guitk-0.4.2/guitk/window.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 from tkinter import ttk
 from typing import TYPE_CHECKING, Any, Hashable
 
 from guitk.tkroot import _TKRoot
 
 from ._debug import debug, debug_watch
 from .basewidget import BaseWidget
-from .constants import DEFAULT_PADX, DEFAULT_PADY
+from .constants import DEFAULT_PADX, DEFAULT_PADY, MENU_MARKER
 from .events import Event, EventCommand, EventType
 from .frame import _LayoutMixin
 from .layout import push_parent
-from .menu import Command, Menu
+from .menu import Command, Menu, MenuBar
 from .ttk_label import Label
 from .types import PadType, SizeType, TooltipType
 
 
 class _WindowBaseClass:
     # only needed to keep typing happy
     pass
@@ -181,15 +181,15 @@
     def _config(self):
         self.title = "My Window"
         """Title to display in the window's title bar """
 
         self.layout = []
         """Every class that inherits from Window must define it's own layout """
 
-        self.menu = {}
+        self.menu: MenuBar | None = None
         """ Optionally provide a menu """
 
         self.padx = DEFAULT_PADX
         self.pady = DEFAULT_PADY
         """Default padding around widgets """
 
         self.theme = None
@@ -390,42 +390,46 @@
         pass
 
     def _forget_widget(self, widget: BaseWidget):
         """Remove widget from the window's bookkeeping but don't destroy it"""
         self._widget_by_key.pop(widget.key, None)
         self._widgets.remove(widget)
 
-    def _add_menus(self, menu: Menu, menu_items, path=None):
-        path = f"MENU:{menu._label}" if path is None else path
-        for m in menu_items:
-            if type(m) == dict:
-                # submenu
-                for subm in m:
-                    subm._create_widget(menu._menu, self)
-                    subpath = f"{path}|{subm._label}"
-                    self._add_menus(subm, m[subm], subpath)
-            elif isinstance(m, Command):
-                command_path = f"{path}|{m._label}"
-                m._create_widget(menu._menu, self, command_path)
+    def _add_menus(self, menu: Menu, path: str | None = None):
+        """Add menus to the window recursively
 
-    def _build_menu(self):
-        if type(self.menu) != dict:
-            raise ValueError("self.menu must be a dict")
+        Args:
+            menu (Menu): the Menu object to add
+            path (str, optional): the path to the menu item which is used as the key
+        """
+        path = f"{MENU_MARKER}{menu._label}" if path is None else path
+        for m in menu:
+            subpath = f"{path}|{m._label}"
+            m._create_widget(menu._menu, self, subpath)
+            self._widgets.append(m)
+            self._widget_by_key[m.key] = m
+            if isinstance(m, Menu):
+                self._add_menus(m, subpath)
 
+    def _build_menu(self):
+        """Build the menu bar"""
         if self._root_menu is None:
             # create the root menu
             self.root.option_add("*tearOff", tk.FALSE)
             self._root_menu = tk.Menu(self.root)
             self.window["menu"] = self._root_menu
 
         for m in self.menu:
             if not isinstance(m, Menu):
-                raise ValueError("self.menu keys must be Menu objects")
-            m._create_widget(self._root_menu, self)
-            self._add_menus(m, self.menu[m])
+                raise ValueError("self.menu items must be Menu objects")
+            path = f"{MENU_MARKER}{m._label}"
+            m._create_widget(self._root_menu, self, path)
+            self._widgets.append(m)
+            self._widget_by_key[m.key] = m
+            self._add_menus(m, path)
 
     @debug_watch
     def _destroy(self):
         """Destroy the window and all child windows and perform cleanup"""
         if self._destroyed:
             # HACK: avoid multiple calls to _destroy which can occur if
             # the user handles the Quit event themselves
@@ -480,23 +484,29 @@
     def _handle_event(self, event: Event):
         """Handle events for this window"""
         # only handle events if widget has events=True; Window objects always get events
         if isinstance(event.widget, (BaseWidget, Window)) and not event.widget.events:
             return
 
         # filter events for this window
-        if event.id == self._id:
-            # handle custom commands
-            self._handle_commands(event)
-
-            self.handle_event(event)
-
-            # if deleting the window, call _destroy after handle_event has had a chance to handle it
-            if event.event_type == EventType.Quit:
-                self._destroy()
+        if event.id != self._id:
+            return
+
+        # swallow MenuCommand events if the menu is disabled
+        # if event.event_type == EventType.MenuCommand and not self.menu.enabled:
+
+        # handle custom commands
+        self._handle_commands(event)
+
+        # call subclass handle_event
+        self.handle_event(event)
+
+        # if deleting the window, call _destroy after handle_event has had a chance to handle it
+        if event.event_type == EventType.Quit:
+            self._destroy()
 
     @debug_watch
     def _handle_commands(self, event):
         """Handle commands bound to widgets in the window"""
         for command in self._commands:
             if (
                 (command.widget is None or command.widget == event.widget)
```

### Comparing `guitk-0.4.1/pyproject.toml` & `guitk-0.4.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "guitk"
-version = "0.4.1"
+version = "0.4.2"
 description = "Python GUI Toolkit for Tk (guitk): simplify the layout and construction of tkinter graphical user interfaces in python."
 authors = ["Rhet Turnbull <rturnbull+git@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -16,14 +16,16 @@
 mkdocstrings-python = "^0.8.3"
 bump2version = "^1.0.1"
 markdownpp = "^1.5.1"
 ruff = "^0.0.265"
 mypy = "^1.3.0"
 pytest-cov = "^4.1.0"
 pillow = "^9.5.0"
+cogapp = "^3.3.0"
+doit = "^0.36.0"
 
 [tool.ruff]
 target-version = "py39"
 line-length = 125
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `guitk-0.4.1/setup.py` & `guitk-0.4.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['guitk']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'guitk',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': 'Python GUI Toolkit for Tk (guitk): simplify the layout and construction of tkinter graphical user interfaces in python.',
-    'long_description': '<!--* DO NOT EDIT README.md, instead edit README.mdpp and process with MarkdownPP using build_readme.sh -->\n\n# Python GUI Toolkit for TK (GUITk)\n\n## Synopsis\n\nGUITk is a declarative framework for building nice-looking, cross-platform GUIs with [tkinter](https://docs.python.org/3/library/tkinter.html) inspired by [SwiftUI](https://developer.apple.com/documentation/swiftui).\n\nGUITk allows you to build complete GUI applications with a few lines of code. GUITk makes it easy to layout your GUI elements and respond to events using a declarative syntax. Because GUITk is built on top of tkinter, you can access the underlying tkinter API if you need to but for many use cases, you can build your GUI without needing to know much about tkinter.\n\nGUITk apps are built by subclasses the `guitk.Window` class. Your GUI elements are layed out using a `guitk.HLayout` (horizontal layout) or `guitk.VLayout` (vertical layout) object which takes care of placing all widgets in the window using a declarative syntax. This is much simpler than using the underlying tkinter [grid manager](https://tkdocs.com/shipman/grid.html) or [pack](https://dafarry.github.io/tkinterbook/pack.htm) geometry managers.\n\nGUITk is in alpha stage but is in constant development so check back frequently if this interests you or open an issue to start a conversation about what pain points this project could help you solve!\n\n## Code Example\n\n### Simple VLayout\n\n![hello.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/hello.py.png "Hello World example")\n\n```python\n"""Simple Hello World example using guitk """\n\nimport guitk as ui\n\n\n# subclass guitk.Window as the starting point for your app\'s main window\nclass HelloWindow(ui.Window):\n    def config(self):\n        """Configure the window"""\n\n        # set the window title\n        self.title = "Hello, World"\n\n        # define a layout for the window\n        # the layout manager will automatically add widgets to the window\n        with ui.HLayout():\n            ui.Label("What\'s your name?")\n            ui.Entry(key="name", focus=True)\n            ui.Button("Ok")\n\n    @ui.on(key="Ok")\n    def on_ok(self, event: ui.Event):\n        """Handle the Ok button click"""\n        print("Hello, ", self.get("name").value)\n\n\n# run your event loop\nif __name__ == "__main__":\n    HelloWindow().run()\n```\n\n## Motivation\n\nThe goal of GUITk is to make it very easy to create simple and attractive GUI apps with python. It borrows ideas from several other libraries include [PySimpleGUI](https://www.pysimplegui.org/en/latest/), [SwiftUI](https://developer.apple.com/documentation/swiftui), [textual](https://github.com/Textualize/textual), and [applepy](https://github.com/eduardohleite/applepy). GUITk builds on [tkinter](https://docs.python.org/3/library/tkinter.html) which ships with the Python standard library and works across many platforms. tkinter is a mature and powerful GUI framework but requires a fair bit of boiler plate and understanding of the underlying framework to use effectively. GUITk attempts to simplify this by providing a higher level interface to tkinter while still allowing you to access the underlying tkinter API if you need to.\n\nThough you can build simple apps without knowing much about tkinter, GUITk is not intended to fully abstract away the tkinter interface. A basic understanding of tkinter will be helpful when building with GUITk. I highly recommend Mark Roseman\'s excellent [Modern Tkinter for Busy Python Developers](https://tkdocs.com/book.html) book as a starting point.\n\n\n## Installation\n\n* `python3 -m pip install guitk`\n\n## Anatomy of a guitk program\n\n![hello2.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/hello2.py.png "Hello World example")\n\n```python\n"""Hello World example using guitk """\n\nimport guitk as ui\n\n\nclass HelloWorld(ui.Window):\n    # subclass guitk.Window as the starting point for your app\'s main window\n    def config(self):\n        # Your Window class needs to define a config() method that describes the layout, title, etc for your app\n        # config() is called by the Window class when the Window is being created\n\n        # Title for the window\n        self.title = "Hello, World"\n\n        # optionally set size as a tuple of (width, height)\n        self.size = (320, 240)\n\n        # you can also use self.geometry for consistency with tkinter\n        # self.geometry = "320x240"\n\n        # Define the window\'s contents\n        # guitk.Label corresponds to a tkinter.ttk.Label, etc.\n        # optionally provide a unique key to each element to easily reference the element later\n        # use a HLayout or VLayout class to define the layout of the window\n        # HLayout arranges widgets horizontally, VLayout arranges widgets vertically\n        with ui.VLayout():\n            # use a VLayout to stack the widgets vertically\n            # standard tkinter layout options such as sticky and weight are supported\n            ui.Label("What\'s your name?", sticky="ew", anchor="center", weightx=1)\n            # most widgets emit events; Entry has events turned off by default so enable with events=True\n            # each widget can be assigned a key, which should be unique, to easily reference the widget later\n            # set focus=True so the Entry box has focus when the window is displayed\n            ui.Entry(key="entry_name", events=True, focus=True, weightx=1, sticky="ew")\n            ui.Label("", width=40, key="output")\n            with ui.HStack():\n                # align these two buttons in a horizontal row using HStack\n                ui.Button("Ok")\n                ui.Button("Quit")\n\n    # Every Window class has 3 special methods that can be overridden to provide custom behavior\n    # you do not need to provide any of these methods if you do not need to customize the default behavior\n    # (the default behavior is to do nothing)\n    # These special methods are: setup(), teardown(), and handle_event()\n\n    def setup(self):\n        """Perform any initialization needed before the Window is displayed"""\n        # your setup() method is called by the Window class after config() just before the Window is displayed\n        # use this to initialize any internal state you need\n        # you do not need to provide a setup() method if no initialization is needed\n        print("setup")\n\n    def teardown(self):\n        """Perform any cleanup needed before destroying the window"""\n        # your teardown() method is called by the Window class after the Window is closed\n        # use this to clean up before the Window is destroyed\n        # you do not need to provide a teardown() method if no cleanup is needed\n        print("teardown")\n\n    def handle_event(self, event: ui.Event):\n        """handle_event() is called by the Window class when an event occurs"""\n        # you do not need to provide a handle_event() method if you prefer to use\n        # the @on decorator to bind functions to events (see below)\n        # handle_event() is a useful place to put code that needs to run for every event\n        # or for use during debugging\n        print(f"handle_event: {event}")\n\n    @ui.on(key="Quit")\n    def on_quit(self):\n        # return the value of the Entry box\n        self.quit(self["entry_name"].value)\n\n    @ui.on(key="Ok")\n    @ui.on(event_type=ui.EventType.EntryReturn)\n    def on_ok(self):\n        # User pressed the OK button or the Return key inside the Entry box\n        # the @on decorator can be used to bind a function to an event\n        # @on can be repeated to bind the function to multiple events\n        # set the output Label to the value of the Entry box\n        # individual widgets can be accessed by their key; the window object acts as a dictionary of widgets\n        greeting = f"Hello {self[\'entry_name\'].value}! Thanks for trying guitk."\n\n        # if you prefer, you can use get() instead of the dictionary syntax\n        self.get("output").value = greeting\n\n\nif __name__ == "__main__":\n    # instantiate your Window class and run it\n    name = HelloWorld().run()\n    print(f"Hello {name}")\n```\n\n## Documentation\n\nNot much documentation at this point.  Take a look at the [examples](https://github.com/RhetTbull/guitk/tree/main/examples) directory for a number of self-documenting examples on use of various widgets.\n\n## Testing\n\nThere are currently no automated tests as I haven\'t figured out how to do these with tkinter. I am working on adding tests and there are several tests that run with `pytest` in the `tests` directory.  These are not automated and require user interaction.\n\nYou can also run `python3 -m guitk` which opens a window with examples of all the widgets. I find this useful for quick testing of layout and widget behavior.\n\n## Contributors\n\nContributions welcome! If this project interests you, open an Issue or send a PR!\n\n## TODO\n\n* [x] Basic prototype\n* [x] Frame\n* [x] Label\n* [x] Entry\n* [x] Button\n* [x] Checkbutton\n* [x] Radiobutton\n* [x] Text\n* [x] ScrolledText\n* [x] Treeview\n* [x] Listbox\n* [x] Combobox\n* [x] Spinner\n* [ ] Other widgets\n* [ ] Menus\n* [x] Tooltips\n* [ ] Documentation\n* [x] Add docstrings\n* [x] Add type hints to public API\n* [ ] Tests\n\n## License\n\nLicensed under the MIT License.\n\n## See Also\n\n* [Textual](https://github.com/Textualize/textual) - An amazing Python framework for building user interfaces in the terminal.\n* [PySimpleGUI](https://www.PySimpleGUI.org) - A Python GUI Framework.\n* [applepy](https://github.com/eduardohleite/applepy) - A declarative GUI framework for developing native macOS applications in Python 3.\n',
+    'long_description': '<!--* DO NOT EDIT README.md, instead edit README.mdpp and process with MarkdownPP using build_readme.sh -->\n\n# Python GUI Toolkit for TK (GUITk)\n\n## Synopsis\n\nGUITk is a declarative framework for building nice-looking, cross-platform GUIs with [tkinter](https://docs.python.org/3/library/tkinter.html) inspired by [SwiftUI](https://developer.apple.com/documentation/swiftui).\n\nGUITk allows you to build complete GUI applications with a few lines of code. GUITk makes it easy to layout your GUI elements and respond to events using a declarative syntax. Because GUITk is built on top of tkinter, you can access the underlying tkinter API if you need to but for many use cases, you can build your GUI without needing to know much about tkinter.\n\nGUITk apps are built by subclasses the `guitk.Window` class. Your GUI elements are layed out using a `guitk.HLayout` (horizontal layout) or `guitk.VLayout` (vertical layout) object which takes care of placing all widgets in the window using a declarative syntax. This is much simpler than using the underlying tkinter [grid manager](https://tkdocs.com/shipman/grid.html) or [pack](https://dafarry.github.io/tkinterbook/pack.htm) geometry managers.\n\nGUITk is in alpha stage but is in constant development so check back frequently if this interests you or open an issue to start a conversation about what pain points this project could help you solve!\n\nDocumentation is available at [GUITk](https://rhettbull.github.io/guitk/).\n\n## Code Example\n\n### Simple HLayout\n\n<!--[[[cog\nimport os\nos.system("python3 utils/screenshot.py examples/hello.py HelloWindow docs/images/hello.py.png --overwrite")\n]]]-->\n<!--[[[end]]]-->\n![hello.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/docs/images/hello.py.png "Hello World example")\n\n```python\n"""Simple Hello World example using guitk """\n\nimport guitk as ui\n\n\n# subclass guitk.Window as the starting point for your app\'s main window\nclass HelloWindow(ui.Window):\n    def config(self):\n        """Configure the window"""\n\n        # set the window title\n        self.title = "Hello, World"\n\n        # define a layout for the window\n        # the layout manager will automatically add widgets to the window\n        with ui.HLayout():\n            ui.Label("What\'s your name?")\n            ui.Entry(key="name", focus=True)\n            ui.Button("Ok")\n\n    @ui.on(key="Ok")\n    def on_ok(self, event: ui.Event):\n        """Handle the Ok button click"""\n        print("Hello, ", self.get("name").value)\n\n\n# run your event loop\nif __name__ == "__main__":\n    HelloWindow().run()\n```\n\n## Motivation\n\nThe goal of GUITk is to make it very easy to create simple and attractive GUI apps with python. It borrows ideas from several other libraries include [PySimpleGUI](https://www.pysimplegui.org/en/latest/), [SwiftUI](https://developer.apple.com/documentation/swiftui), [textual](https://github.com/Textualize/textual), and [applepy](https://github.com/eduardohleite/applepy). GUITk builds on [tkinter](https://docs.python.org/3/library/tkinter.html) which ships with the Python standard library and works across many platforms. tkinter is a mature and powerful GUI framework but requires a fair bit of boiler plate and understanding of the underlying framework to use effectively. GUITk attempts to simplify this by providing a higher level interface to tkinter while still allowing you to access the underlying tkinter API if you need to.\n\nThough you can build simple apps without knowing much about tkinter, GUITk is not intended to fully abstract away the tkinter interface. A basic understanding of tkinter will be helpful when building with GUITk. I highly recommend Mark Roseman\'s excellent [Modern Tkinter for Busy Python Developers](https://tkdocs.com/book.html) book as a starting point.\n\n## Installation\n\n* `python3 -m pip install guitk`\n\n## Anatomy of a guitk program\n\n<!--[[[cog\nimport os\nos.system("python3 utils/screenshot.py examples/hello2.py HelloWorld docs/images/hello2.py.png --overwrite")\n]]]-->\n<!--[[[end]]]-->\n![hello2.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/docs/images/hello2.py.png "Hello World example")\n\n```python\n"""Hello World example using guitk """\n\nimport guitk as ui\n\n\nclass HelloWorld(ui.Window):\n    # subclass guitk.Window as the starting point for your app\'s main window\n    def config(self):\n        # Your Window class needs to define a config() method that describes the layout, title, etc for your app\n        # config() is called by the Window class when the Window is being created\n\n        # Title for the window\n        self.title = "Hello, World"\n\n        # optionally set size as a tuple of (width, height)\n        self.size = (320, 240)\n\n        # you can also use self.geometry for consistency with tkinter\n        # self.geometry = "320x240"\n\n        # Define the window\'s contents\n        # guitk.Label corresponds to a tkinter.ttk.Label, etc.\n        # optionally provide a unique key to each element to easily reference the element later\n        # use a HLayout or VLayout class to define the layout of the window\n        # HLayout arranges widgets horizontally, VLayout arranges widgets vertically\n        with ui.VLayout():\n            # use a VLayout to stack the widgets vertically\n            # standard tkinter layout options such as sticky and weight are supported\n            ui.Label("What\'s your name?", sticky="ew", anchor="center", weightx=1)\n            # most widgets emit events; Entry has events turned off by default so enable with events=True\n            # each widget can be assigned a key, which should be unique, to easily reference the widget later\n            # set focus=True so the Entry box has focus when the window is displayed\n            ui.Entry(key="entry_name", events=True, focus=True, weightx=1, sticky="ew")\n            ui.Label("", width=40, key="output")\n            with ui.HStack():\n                # align these two buttons in a horizontal row using HStack\n                ui.Button("Ok")\n                ui.Button("Quit")\n\n    # Every Window class has 3 special methods that can be overridden to provide custom behavior\n    # you do not need to provide any of these methods if you do not need to customize the default behavior\n    # (the default behavior is to do nothing)\n    # These special methods are: setup(), teardown(), and handle_event()\n\n    def setup(self):\n        """Perform any initialization needed before the Window is displayed"""\n        # your setup() method is called by the Window class after config() just before the Window is displayed\n        # use this to initialize any internal state you need\n        # you do not need to provide a setup() method if no initialization is needed\n        print("setup")\n\n    def teardown(self):\n        """Perform any cleanup needed before destroying the window"""\n        # your teardown() method is called by the Window class after the Window is closed\n        # use this to clean up before the Window is destroyed\n        # you do not need to provide a teardown() method if no cleanup is needed\n        print("teardown")\n\n    def handle_event(self, event: ui.Event):\n        """handle_event() is called by the Window class when an event occurs"""\n        # you do not need to provide a handle_event() method if you prefer to use\n        # the @on decorator to bind functions to events (see below)\n        # handle_event() is a useful place to put code that needs to run for every event\n        # or for use during debugging\n        print(f"handle_event: {event}")\n\n    @ui.on(key="Quit")\n    def on_quit(self):\n        # return the value of the Entry box\n        self.quit(self["entry_name"].value)\n\n    @ui.on(key="Ok")\n    @ui.on(event_type=ui.EventType.EntryReturn)\n    def on_ok(self):\n        # User pressed the OK button or the Return key inside the Entry box\n        # the @on decorator can be used to bind a function to an event\n        # @on can be repeated to bind the function to multiple events\n        # set the output Label to the value of the Entry box\n        # individual widgets can be accessed by their key; the window object acts as a dictionary of widgets\n        greeting = f"Hello {self[\'entry_name\'].value}! Thanks for trying guitk."\n\n        # if you prefer, you can use get() instead of the dictionary syntax\n        self.get("output").value = greeting\n\n\nif __name__ == "__main__":\n    # instantiate your Window class and run it\n    name = HelloWorld().run()\n    print(f"Hello {name}")\n```\n\n## Documentation\n\nNot much documentation at this point but there\'s a start [here](https://rhettbull.github.io/guitk/).  Take a look at the [examples](https://github.com/RhetTbull/guitk/tree/main/examples) directory for a number of self-documenting examples on use of various widgets.\n\n## Testing\n\nThere are currently no automated tests as I haven\'t figured out how to do these with tkinter. I am working on adding tests and there are several tests that run with `pytest` in the `tests` directory.  These are not automated and require user interaction.\n\nYou can also run `python3 -m guitk` which opens a window with examples of all the widgets. I find this useful for quick testing of layout and widget behavior.\n\n## Contributors\n\nContributions welcome! If this project interests you, open an Issue or send a PR!\n\n## TODO\n\n* [x] Basic prototype\n* [x] Frame\n* [x] Label\n* [x] Entry\n* [x] Button\n* [x] Checkbutton\n* [x] Radiobutton\n* [x] Text\n* [x] ScrolledText\n* [x] Treeview\n* [x] Listbox\n* [x] Combobox\n* [x] Spinner\n* [x] Other widgets\n* [x] Menus\n* [x] Tooltips\n* [ ] Documentation\n* [x] Add docstrings\n* [x] Add type hints to public API\n* [ ] Tests\n\n## License\n\nLicensed under the MIT License.\n\n## See Also\n\n* [Textual](https://github.com/Textualize/textual) - An amazing Python framework for building user interfaces in the terminal.\n* [PySimpleGUI](https://www.PySimpleGUI.org) - A Python GUI Framework.\n* [applepy](https://github.com/eduardohleite/applepy) - A declarative GUI framework for developing native macOS applications in Python 3.\n',
     'author': 'Rhet Turnbull',
     'author_email': 'rturnbull+git@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `guitk-0.4.1/PKG-INFO` & `guitk-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guitk
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python GUI Toolkit for Tk (guitk): simplify the layout and construction of tkinter graphical user interfaces in python.
 License: MIT
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,19 +23,26 @@
 
 GUITk allows you to build complete GUI applications with a few lines of code. GUITk makes it easy to layout your GUI elements and respond to events using a declarative syntax. Because GUITk is built on top of tkinter, you can access the underlying tkinter API if you need to but for many use cases, you can build your GUI without needing to know much about tkinter.
 
 GUITk apps are built by subclasses the `guitk.Window` class. Your GUI elements are layed out using a `guitk.HLayout` (horizontal layout) or `guitk.VLayout` (vertical layout) object which takes care of placing all widgets in the window using a declarative syntax. This is much simpler than using the underlying tkinter [grid manager](https://tkdocs.com/shipman/grid.html) or [pack](https://dafarry.github.io/tkinterbook/pack.htm) geometry managers.
 
 GUITk is in alpha stage but is in constant development so check back frequently if this interests you or open an issue to start a conversation about what pain points this project could help you solve!
 
+Documentation is available at [GUITk](https://rhettbull.github.io/guitk/).
+
 ## Code Example
 
-### Simple VLayout
+### Simple HLayout
 
-![hello.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/hello.py.png "Hello World example")
+<!--[[[cog
+import os
+os.system("python3 utils/screenshot.py examples/hello.py HelloWindow docs/images/hello.py.png --overwrite")
+]]]-->
+<!--[[[end]]]-->
+![hello.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/docs/images/hello.py.png "Hello World example")
 
 ```python
 """Simple Hello World example using guitk """
 
 import guitk as ui
 
 
@@ -67,22 +74,26 @@
 
 ## Motivation
 
 The goal of GUITk is to make it very easy to create simple and attractive GUI apps with python. It borrows ideas from several other libraries include [PySimpleGUI](https://www.pysimplegui.org/en/latest/), [SwiftUI](https://developer.apple.com/documentation/swiftui), [textual](https://github.com/Textualize/textual), and [applepy](https://github.com/eduardohleite/applepy). GUITk builds on [tkinter](https://docs.python.org/3/library/tkinter.html) which ships with the Python standard library and works across many platforms. tkinter is a mature and powerful GUI framework but requires a fair bit of boiler plate and understanding of the underlying framework to use effectively. GUITk attempts to simplify this by providing a higher level interface to tkinter while still allowing you to access the underlying tkinter API if you need to.
 
 Though you can build simple apps without knowing much about tkinter, GUITk is not intended to fully abstract away the tkinter interface. A basic understanding of tkinter will be helpful when building with GUITk. I highly recommend Mark Roseman's excellent [Modern Tkinter for Busy Python Developers](https://tkdocs.com/book.html) book as a starting point.
 
-
 ## Installation
 
 * `python3 -m pip install guitk`
 
 ## Anatomy of a guitk program
 
-![hello2.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/examples/hello2.py.png "Hello World example")
+<!--[[[cog
+import os
+os.system("python3 utils/screenshot.py examples/hello2.py HelloWorld docs/images/hello2.py.png --overwrite")
+]]]-->
+<!--[[[end]]]-->
+![hello2.py example](https://raw.githubusercontent.com/RhetTbull/guitk/main/docs/images/hello2.py.png "Hello World example")
 
 ```python
 """Hello World example using guitk """
 
 import guitk as ui
 
 
@@ -170,15 +181,15 @@
     # instantiate your Window class and run it
     name = HelloWorld().run()
     print(f"Hello {name}")
 ```
 
 ## Documentation
 
-Not much documentation at this point.  Take a look at the [examples](https://github.com/RhetTbull/guitk/tree/main/examples) directory for a number of self-documenting examples on use of various widgets.
+Not much documentation at this point but there's a start [here](https://rhettbull.github.io/guitk/).  Take a look at the [examples](https://github.com/RhetTbull/guitk/tree/main/examples) directory for a number of self-documenting examples on use of various widgets.
 
 ## Testing
 
 There are currently no automated tests as I haven't figured out how to do these with tkinter. I am working on adding tests and there are several tests that run with `pytest` in the `tests` directory.  These are not automated and require user interaction.
 
 You can also run `python3 -m guitk` which opens a window with examples of all the widgets. I find this useful for quick testing of layout and widget behavior.
 
@@ -197,16 +208,16 @@
 * [x] Radiobutton
 * [x] Text
 * [x] ScrolledText
 * [x] Treeview
 * [x] Listbox
 * [x] Combobox
 * [x] Spinner
-* [ ] Other widgets
-* [ ] Menus
+* [x] Other widgets
+* [x] Menus
 * [x] Tooltips
 * [ ] Documentation
 * [x] Add docstrings
 * [x] Add type hints to public API
 * [ ] Tests
 
 ## License
```

