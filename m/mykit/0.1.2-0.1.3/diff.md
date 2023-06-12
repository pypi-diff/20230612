# Comparing `tmp/mykit-0.1.2.tar.gz` & `tmp/mykit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mykit-0.1.2.tar", last modified: Mon Jun 12 12:16:32 2023, max compression
+gzip compressed data, was "mykit-0.1.3.tar", last modified: Mon Jun 12 14:22:06 2023, max compression
```

## Comparing `mykit-0.1.2.tar` & `mykit-0.1.3.tar`

### file list

```diff
@@ -1,47 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.890277 mykit-0.1.2/
--rw-rw-rw-   0        0        0     1097 2023-04-10 22:01:23.000000 mykit-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     4701 2023-06-12 12:16:32.886274 mykit-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4197 2023-06-12 12:12:50.000000 mykit-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.648218 mykit-0.1.2/mykit/
--rw-rw-rw-   0        0        0      134 2023-06-12 12:04:04.000000 mykit-0.1.2/mykit/__init__.py
--rw-rw-rw-   0        0        0      326 2023-05-27 14:47:02.000000 mykit-0.1.2/mykit/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.793257 mykit-0.1.2/mykit/kit/
--rw-rw-rw-   0        0        0     3655 2023-06-11 17:23:45.000000 mykit-0.1.2/mykit/kit/color.py
--rw-rw-rw-   0        0        0     5809 2023-06-12 11:57:08.000000 mykit-0.1.2/mykit/kit/ffmpeg.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.804262 mykit-0.1.2/mykit/kit/graph/
--rw-rw-rw-   0        0        0    16521 2023-06-12 12:03:05.000000 mykit-0.1.2/mykit/kit/graph/graph2d.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.487175 mykit-0.1.2/mykit/kit/gui/
-drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.827263 mykit-0.1.2/mykit/kit/gui/button/
--rw-rw-rw-   0        0        0     7403 2023-05-13 04:57:02.000000 mykit-0.1.2/mykit/kit/gui/button/__init__.py
--rw-rw-rw-   0        0        0    11489 2023-05-20 15:47:14.000000 mykit-0.1.2/mykit/kit/gui/button/v2.py
--rw-rw-rw-   0        0        0    13441 2023-05-27 15:38:04.000000 mykit-0.1.2/mykit/kit/gui/button/v3.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.840271 mykit-0.1.2/mykit/kit/gui/label/
--rw-rw-rw-   0        0        0     6076 2023-05-12 14:09:30.000000 mykit-0.1.2/mykit/kit/gui/label/__init__.py
--rw-rw-rw-   0        0        0     9542 2023-05-27 15:38:15.000000 mykit-0.1.2/mykit/kit/gui/label/v2.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.846276 mykit-0.1.2/mykit/kit/gui/shape/
--rw-rw-rw-   0        0        0     4224 2023-05-13 04:59:18.000000 mykit-0.1.2/mykit/kit/gui/shape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.861268 mykit-0.1.2/mykit/kit/gui/slider/
--rw-rw-rw-   0        0        0    20347 2023-05-18 07:01:02.000000 mykit-0.1.2/mykit/kit/gui/slider/__init__.py
--rw-rw-rw-   0        0        0    28699 2023-05-27 18:19:56.000000 mykit-0.1.2/mykit/kit/gui/slider/v2.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.867270 mykit-0.1.2/mykit/kit/keycrate/
--rw-rw-rw-   0        0        0     6467 2023-05-18 13:56:54.000000 mykit-0.1.2/mykit/kit/keycrate/__init__.py
--rw-rw-rw-   0        0        0     2741 2023-06-12 12:12:05.000000 mykit-0.1.2/mykit/kit/math.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.502184 mykit-0.1.2/mykit/kit/neuralnet/
-drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.875275 mykit-0.1.2/mykit/kit/neuralnet/dense/
--rw-rw-rw-   0        0        0     7317 2023-05-15 21:04:54.000000 mykit-0.1.2/mykit/kit/neuralnet/dense/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.878272 mykit-0.1.2/mykit/kit/neuralnet/genetic/
--rw-rw-rw-   0        0        0    15106 2023-05-27 08:37:35.000000 mykit-0.1.2/mykit/kit/neuralnet/genetic/__init__.py
--rw-rw-rw-   0        0        0     3039 2023-05-06 18:30:49.000000 mykit-0.1.2/mykit/kit/noise.py
--rw-rw-rw-   0        0        0     4253 2023-05-18 13:55:09.000000 mykit-0.1.2/mykit/kit/path.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.882273 mykit-0.1.2/mykit/kit/quick_visual/
--rw-rw-rw-   0        0        0      838 2023-05-06 12:20:28.000000 mykit-0.1.2/mykit/kit/quick_visual/plot2d.py
--rw-rw-rw-   0        0        0      403 2023-06-11 18:43:02.000000 mykit-0.1.2/mykit/kit/text.py
--rw-rw-rw-   0        0        0     2453 2023-06-12 11:34:47.000000 mykit-0.1.2/mykit/kit/time.py
--rw-rw-rw-   0        0        0     3156 2023-05-18 13:20:09.000000 mykit-0.1.2/mykit/kit/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:16:32.727238 mykit-0.1.2/mykit.egg-info/
--rw-rw-rw-   0        0        0     4701 2023-06-12 12:16:32.000000 mykit-0.1.2/mykit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      739 2023-06-12 12:16:32.000000 mykit-0.1.2/mykit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 12:16:32.000000 mykit-0.1.2/mykit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-12 12:16:32.000000 mykit-0.1.2/mykit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      582 2023-06-12 12:03:36.000000 mykit-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 12:16:32.891279 mykit-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.258652 mykit-0.1.3/
+-rw-rw-rw-   0        0        0     1097 2023-04-10 22:01:23.000000 mykit-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3832 2023-06-12 14:22:06.255653 mykit-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1984 2023-06-12 14:07:52.000000 mykit-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.005598 mykit-0.1.3/mykit/
+-rw-rw-rw-   0        0        0      204 2023-06-12 13:37:25.000000 mykit-0.1.3/mykit/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-12 13:35:43.000000 mykit-0.1.3/mykit/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.182640 mykit-0.1.3/mykit/app/
+-rw-rw-rw-   0        0        0     4152 2023-06-12 13:55:45.000000 mykit-0.1.3/mykit/app/arrow.py
+-rw-rw-rw-   0        0        0    12892 2023-06-12 14:04:51.000000 mykit-0.1.3/mykit/app/button.py
+-rw-rw-rw-   0        0        0     9010 2023-06-12 14:04:57.000000 mykit-0.1.3/mykit/app/label.py
+-rw-rw-rw-   0        0        0    28006 2023-06-12 14:05:24.000000 mykit-0.1.3/mykit/app/slider.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.220646 mykit-0.1.3/mykit/kit/
+-rw-rw-rw-   0        0        0     2965 2023-06-12 13:39:03.000000 mykit-0.1.3/mykit/kit/color.py
+-rw-rw-rw-   0        0        0     5809 2023-06-12 11:57:08.000000 mykit-0.1.3/mykit/kit/ffmpeg.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.225647 mykit-0.1.3/mykit/kit/graph/
+-rw-rw-rw-   0        0        0    16521 2023-06-12 12:03:05.000000 mykit-0.1.3/mykit/kit/graph/graph2d.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.233650 mykit-0.1.3/mykit/kit/keycrate/
+-rw-rw-rw-   0        0        0     6473 2023-06-12 14:01:25.000000 mykit-0.1.3/mykit/kit/keycrate/__init__.py
+-rw-rw-rw-   0        0        0     2741 2023-06-12 12:12:05.000000 mykit-0.1.3/mykit/kit/math.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.244653 mykit-0.1.3/mykit/kit/neuralnet/
+-rw-rw-rw-   0        0        0     7320 2023-06-12 14:05:32.000000 mykit-0.1.3/mykit/kit/neuralnet/dense.py
+-rw-rw-rw-   0        0        0    15109 2023-06-12 14:05:43.000000 mykit-0.1.3/mykit/kit/neuralnet/genetic.py
+-rw-rw-rw-   0        0        0     3039 2023-05-06 18:30:49.000000 mykit-0.1.3/mykit/kit/noise.py
+-rw-rw-rw-   0        0        0     4253 2023-05-18 13:55:09.000000 mykit-0.1.3/mykit/kit/path.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.252652 mykit-0.1.3/mykit/kit/quick_visual/
+-rw-rw-rw-   0        0        0      841 2023-06-12 14:06:19.000000 mykit-0.1.3/mykit/kit/quick_visual/plot2d.py
+-rw-rw-rw-   0        0        0      403 2023-06-11 18:43:02.000000 mykit-0.1.3/mykit/kit/text.py
+-rw-rw-rw-   0        0        0     2453 2023-06-12 11:34:47.000000 mykit-0.1.3/mykit/kit/time.py
+-rw-rw-rw-   0        0        0     3156 2023-05-18 13:20:09.000000 mykit-0.1.3/mykit/kit/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:22:06.070614 mykit-0.1.3/mykit.egg-info/
+-rw-rw-rw-   0        0        0     3832 2023-06-12 14:22:05.000000 mykit-0.1.3/mykit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2023-06-12 14:22:05.000000 mykit-0.1.3/mykit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 14:22:05.000000 mykit-0.1.3/mykit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 14:22:05.000000 mykit-0.1.3/mykit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      688 2023-06-12 14:19:03.000000 mykit-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 14:22:06.259653 mykit-0.1.3/setup.cfg
```

### Comparing `mykit-0.1.2/LICENSE` & `mykit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-0.1.2/mykit/kit/color.py` & `mykit-0.1.3/mykit/kit/color.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,54 +32,27 @@
     b = int(b1 + (b2 - b1)*x)
 
     ## convert interpolated RGB values to hexadecimal color string
     interpolated_color = f'#{r:02x}{g:02x}{b:02x}'
     return interpolated_color
 
 
-def get_gray(lum: int = 128, alpha: float = 1.0, /) -> str:
-    """
-    Return grayscale color in hexadecimal.
-
-    ---
-
-    ## Params
-    - `lum`: luminance, interval: [0, 255].
-    - `alpha`: opacity, interval: [0, 1].
-
-    ## Demo
-    >>> get_gray(255, 1)
-    '#ffffff'
-    >>> get_gray(255, 0)
-    '#000000'
-    >>> get_gray(128, 1)
-    '#808080'
-
-    ## Docs
-    - This function has been deprecated; use `getgray` instead.
-    """
-    lum_prime = round(lum*alpha)
-    return f'#{lum_prime:02x}{lum_prime:02x}{lum_prime:02x}'
-
 def getgray(alpha: float, /, max_lum: int = 255) -> str:
     """
     Returns a hexadecimal color value representing a grayscale shade based on the given alpha and maximum luminance.
 
     ---
 
     ## Params
     - `alpha`: A grayscale shade intensity value in the range [0, 1].
     - `max_lum`: Maximum luminance value for grayscale in the range [0, 255].
 
     ## Demo
     >>> getgray(0.5)
     '#808080'
-
-    ## Docs
-    - This function is the next version of `get_gray` (optimized, better variable names, and improved argument order).
     """
     a = f'{round(max_lum*alpha):02x}'
     return f'#{a}{a}{a}'
 
 
 def rgb_to_hex(r: int, g: int, b: int, /) -> str:
     return f'#{r:02x}{g:02x}{b:02x}'
```

### Comparing `mykit-0.1.2/mykit/kit/ffmpeg.py` & `mykit-0.1.3/mykit/kit/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.2/mykit/kit/graph/graph2d.py` & `mykit-0.1.3/mykit/kit/graph/graph2d.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.2/mykit/kit/gui/button/v2.py` & `mykit-0.1.3/mykit/app/button.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,32 @@
 import random as _random
 import tkinter as _tk
 import typing as _typing
 
 
 class Button:
-    """
-    The next version of `carbon.gui.button.Button`.
-
-    ## What's new
-    - Arguments reordering, default value changes
-    - Added colors (button color, border color, label color) parameters
-    - Added height (button's height) parameters
-    - Param `id` and `label` are now optional
-    """
 
     page: _tk.Canvas = None
     @staticmethod
     def set_page(page: _tk.Canvas, /) -> None:
         Button.page = page
 
     buttons: dict[str, 'Button'] = {}
     button_tags: dict[str, list['Button']] = {}
 
     def __init__(
         self,
-        x: int,
-        y: int,
-        fn: _typing.Callable[[], None],
-        
+        x: int = 0,
+        y: int = 0,
+        fn: _typing.Callable[[], None] | None = None,
         label: str = '',
-
+        label_font: str | tuple[str, int] = 'Verdana 8',
         anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'] = 'nw',
-
         width: int = 100,
         height: int = 18,
-        
         locked: bool = False,
         visible: bool = True,
 
         color_btn_normal: str = '#464646',
         color_btn_hover: str = '#5a5a5a',
         color_btn_press: str = '#6e6e6e',
         color_btn_locked: str = '#282828',
@@ -48,52 +36,49 @@
         color_lbl_locked: str = '#050505',
 
         id: str | None = None,
         tags: str | list[str] | None = None,
     ) -> None:
         """
         ## Params
-        - `x` and `y` is the position of the `anchor`
+        - `x` and `y` is the position of the `anchor` (not the center of the button)
         - `color_btn_normal`: button's color
         - `color_bd_normal`: button's border color
         - `color_lbl_normal`: button's label color
         """
 
+        ## make sure the page has already been set
+        if Button.page is None:
+            raise AssertionError('It seems you forgot to do `Button.set_page(page)`.')
+
         self.x = x
         self.y = y
         self.fn = fn
-
-        ## below isn't necessary because will be checked at `self._anchoring()`  (delete below code soon)
-        # if anchor.lower() not in ['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']:
-        #     raise ValueError(f'Invalid anchor value: {repr(anchor)}')
-        # self.anchor = anchor.lower()
-        self.anchor = anchor
-
         self.label = label
-        
+        self.label_font = label_font
+        self.anchor = anchor
         self.width = width
         self.height = height
-
         self.locked = locked
         self.visible = visible
 
         self.color_btn_normal = color_btn_normal
         self.color_btn_hover = color_btn_hover
         self.color_btn_press = color_btn_press
         self.color_btn_locked = color_btn_locked
         self.color_bd_normal = color_bd_normal
         self.color_bd_locked = color_bd_locked
         self.color_lbl_normal = color_lbl_normal
         self.color_lbl_locked = color_lbl_locked
 
         ## self.id ensures that we can modify a specific instance without affecting the others
         if id is None:
-            self.id = str(_random.randint(-10000, 10000))
+            self.id = str(_random.randint(0, 100_000))
             while self.id in Button.buttons:
-                self.id = str(_random.randint(-10000, 10000))
+                self.id = str(_random.randint(0, 100_000))
         else:
             self.id = id
             if self.id in Button.buttons:
                 raise ValueError(f'The id {repr(id)} is duplicated.')
         Button.buttons[self.id] = self
 
         ## <tags>
@@ -107,60 +92,25 @@
                 if tag in Button.button_tags:
                     Button.button_tags[tag].append(self)
                 else:
                     Button.button_tags[tag] = [self]
         ## </tags>
 
 
-        ## preprocess
-        self._anchoring()
-
-
         ## runtime
+
         self.default_label = label
         self.pressed = False
         self.hovered = False
 
 
         ## init
+
         self._redraw()
 
-    def _anchoring(self):
-        
-        self.anchor = self.anchor.lower()
-        
-        if self.anchor == 'center':
-            self.ctr_x = self.x
-            self.ctr_y = self.y
-        elif self.anchor == 'n':
-            self.ctr_x = self.x
-            self.ctr_y = self.y + self.height/2
-        elif self.anchor == 'ne':
-            self.ctr_x = self.x - self.width/2
-            self.ctr_y = self.y + self.height/2
-        elif self.anchor == 'e':
-            self.ctr_x = self.x - self.width/2
-            self.ctr_y = self.y
-        elif self.anchor == 'se':
-            self.ctr_x = self.x - self.width/2
-            self.ctr_y = self.y - self.height/2
-        elif self.anchor == 's':
-            self.ctr_x = self.x
-            self.ctr_y = self.y - self.height/2
-        elif self.anchor == 'sw':
-            self.ctr_x = self.x + self.width/2
-            self.ctr_y = self.y - self.height/2
-        elif self.anchor == 'w':
-            self.ctr_x = self.x + self.width/2
-            self.ctr_y = self.y
-        elif self.anchor == 'nw':
-            self.ctr_x = self.x + self.width/2
-            self.ctr_y = self.y + self.height/2
-        else:
-            raise ValueError(f'Unexpected anchor value: {repr(self.anchor)}')
 
     def _redraw(self):
 
         if self.locked:
             color_btn = self.color_btn_locked
             color_bd = self.color_bd_locked
             color_lbl = self.color_lbl_locked
@@ -177,105 +127,114 @@
             color_bd = self.color_bd_normal
             color_lbl = self.color_lbl_normal
 
         Button.page.delete(f'Button_{self.id}')
 
         if self.visible:
 
+            ## This overhead will be executed each time this function is called.
+            ## It may be inefficient, but it makes the code cleaner.
+            X, Y = self.get_anchor_loc('center')  # the center of the button
+
             Button.page.create_rectangle(
-                self.ctr_x - self.width/2, self.ctr_y - self.height/2,
-                self.ctr_x + self.width/2, self.ctr_y + self.height/2,
+                X - self.width/2, Y - self.height/2,
+                X + self.width/2, Y + self.height/2,
                 fill=color_btn, width=1, outline=color_bd,
                 tags=f'Button_{self.id}'
             )
             Button.page.create_text(
-                self.ctr_x, self.ctr_y,
-                text=self.label, font='Arial 9',
+                X, Y,
+                text=self.label, font=self.label_font,
                 fill=color_lbl,
                 tags=f'Button_{self.id}'
             )
 
-    def hover(self):
+
+    def _hover(self):
+
+        w2 = self.width/2
+        h2 = self.height/2
         
-        mousex = Button.page.winfo_pointerx()
-        mousey = Button.page.winfo_pointery()
+        x = Button.page.winfo_pointerx()
+        y = Button.page.winfo_pointery()
+
+        X, Y = self.get_anchor_loc('center')
+
+        ## `True` if the mouse cursor is inside the button
+        inside = (X-w2 <= x <= X+w2) and (Y-h2 <= y <= Y+h2)
 
-        if (
-            (self.ctr_x-self.width/2 <= mousex <= self.ctr_x+self.width/2)
-            and
-            (self.ctr_y-self.height/2 <= mousey <= self.ctr_y+self.height/2)
-            and
-            (not self.locked)
-            and
-            (self.visible)
-            and
-            (not self.hovered)
-        ):
+        if inside and (not self.locked) and self.visible and (not self.hovered):
             self.hovered = True
-            self._redraw()
-        elif (
-            (self.hovered)
-            and
-            (not ((self.ctr_x-self.width/2 <= mousex <= self.ctr_x+self.width/2) and (self.ctr_y-self.height/2 <= mousey <= self.ctr_y+self.height/2)))
-        ):
+            self._redraw()  # just redraw once here
+
+        elif self.hovered and (not inside):
             self.hovered = False
-            self._redraw()
+            self._redraw()  # just redraw once here
+
+        ## reminder: don't put it right here because it will redraw regardless of the hovered state
+        # self._redraw()
+
+    @staticmethod
+    def hover_listener():
+        for button in Button.buttons.values():
+            button._hover()
+
 
     def press(self):
         
-        mousex = Button.page.winfo_pointerx()
-        mousey = Button.page.winfo_pointery()
+        x = Button.page.winfo_pointerx()
+        y = Button.page.winfo_pointery()
 
-        if (
-            (self.ctr_x-self.width/2 <= mousex <= self.ctr_x+self.width/2)
-            and
-            (self.ctr_y-self.height/2 <= mousey <= self.ctr_y+self.height/2)
-            and
-            (not self.locked)
-            and
-            (self.visible)
-        ):
-            self.pressed = True
-            self._redraw()
+        X, Y = self.get_anchor_loc('center')
+        w2 = self.width/2
+        h2 = self.height/2
+        inside = (X-w2 <= x <= X+w2) and (Y-h2 <= y <= Y+h2)
 
-    def release(self):
-        if self.pressed:
-            self.pressed = False
+        if inside and (not self.locked) and self.visible:
+            self.pressed = True
             self._redraw()
-            self.fn()
-
-    @staticmethod
-    def hover_listener():
-        for button in Button.buttons.values():
-            button.hover()
 
     @staticmethod
     def press_listener():
         for button in Button.buttons.values():
             button.press()
 
+
+    def release(self):
+        if self.pressed:
+            self.pressed = False
+            self._redraw()            
+            if self.fn is not None:
+                self.fn()
+
     @staticmethod
     def release_listener():
         for button in list(Button.buttons.values()):
             button.release()
 
+
     def set_lock(self, locked: bool, /):
         if self.locked is not locked:
             self.locked = locked
             self._redraw()
     
     @staticmethod
     def set_lock_by_id(id: str, locked: bool, /):
         Button.buttons[id].set_lock(locked)
 
     @staticmethod
     def set_lock_by_tag(tag: str, locked: bool, /):
         for button in Button.button_tags[tag]:
             button.set_lock(locked)
 
+    @staticmethod
+    def set_lock_all(locked: bool, /):
+        for button in Button.buttons.values():
+            button.set_lock(locked)
+
 
     def set_visibility(self, visible: bool, /):
         if self.visible is not visible:
             self.visible = visible
             self._redraw()
 
     @staticmethod
@@ -290,15 +249,18 @@
     @staticmethod
     def set_visibility_all(visible: bool, /):
         for button in Button.buttons.values():
             button.set_visibility(visible)
 
 
     def set_label(self, label: str | None, /):
-        """if `None` -> default label."""
+        """
+        If `label = None`, the default label (the one assigned
+        when the instance was created) will be used.
+        """
 
         if label is None:
             label = self.default_label
 
         if self.label != label:
             self.label = label
             self._redraw()
@@ -313,60 +275,153 @@
             self.fn = fn
 
     @staticmethod
     def set_fn_by_id(id: str, fn: _typing.Callable[[], None], /):
         Button.buttons[id].set_fn(fn)
 
 
-    def move(self, x: int, y: int, /, anchor: str | None = None) -> None:
-        """move the button (using the default anchor if `anchor=None`)"""
-        
+    def get_anchor_loc(
+        self,
+        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'],
+        /
+    ) -> tuple[int, int]:
+        """To get the button's center coordinate, use `anchor='center'`"""
+
+        W = self.width
+        H = self.height
+
+        ## get the coordinates for the center (X, Y)
+        if self.anchor == 'center':
+            X = self.x
+            Y = self.y
+        elif self.anchor == 'n':
+            X = self.x
+            Y = self.y + H/2
+        elif self.anchor == 'ne':
+            X = self.x - W/2
+            Y = self.y + H/2
+        elif self.anchor == 'e':
+            X = self.x - W/2
+            Y = self.y
+        elif self.anchor == 'se':
+            X = self.x - W/2
+            Y = self.y - H/2
+        elif self.anchor == 's':
+            X = self.x
+            Y = self.y - H/2
+        elif self.anchor == 'sw':
+            X = self.x + W/2
+            Y = self.y - H/2
+        elif self.anchor == 'w':
+            X = self.x + W/2
+            Y = self.y
+        elif self.anchor == 'nw':
+            X = self.x + W/2
+            Y = self.y + H/2
+
+        ## returning the requested anchor location
+        if anchor == 'center':
+            return (X, Y)
+        elif anchor == 'n':
+            return (X, Y-H/2)
+        elif anchor == 'ne':
+            return (X+W/2, Y-H/2)
+        elif anchor == 'e':
+            return (X+W/2, Y)
+        elif anchor == 'se':
+            return (X+W/2, Y+H/2)
+        elif anchor == 's':
+            return (X, Y+H/2)
+        elif anchor == 'sw':
+            return (X-W/2, Y+H/2)
+        elif anchor == 'w':
+            return (X-W/2, Y)
+        elif anchor == 'nw':
+            return (X-W/2, Y-H/2)
+        else:
+            raise ValueError(f'Invalid anchor value: {repr(anchor)}')
+
+    @staticmethod
+    def get_anchor_loc_by_id(
+        id: str,
+        anchor: _typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw'],
+        /
+    ) -> tuple[int, int]:
+        return Button.buttons[id].get_anchor_loc(anchor)
+
+
+    def move(
+        self,
+        x: int,
+        y: int,
+        /,
+        anchor: _typing.Optional[_typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
+    ) -> None:
+        """If `anchor = None`, the current anchor will be used."""
         self.x = x
         self.y = y
-        
         if anchor is not None:
             self.anchor = anchor
-
-        self._anchoring()
         self._redraw()
 
     @staticmethod
-    def move_by_id(id: str, x: int, y: int, /) -> None:
-        Button.buttons[id].move(x, y)
+    def move_by_id(
+        id: str,
+        x: int,
+        y: int,
+        /,
+        anchor: _typing.Optional[_typing.Literal['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']] = None
+    ) -> None:
+        Button.buttons[id].move(x, y, anchor)
+
+
+    def align(
+        self,
+        target: 'Button',
+        anchor: str = 'nw',
+        target_anchor: str = 'ne',
+        xgap: float = 15,
+        ygap: float = 0
+    ) -> 'Button':
+        """
+        Valid options for `anchor` and `target_anchor` are `['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']`.
+        """
+
+        ## getting the target anchor location
+        x, y = target.get_anchor_loc(target_anchor)
+
+        ## shifting
+        x += xgap
+        y += ygap
+
+        ## moving the label
+        self.move(x, y, anchor)
+
+        ## return the instance so that this method can also be used when
+        ## creating the instance, like `btn_2 = Button().align(btn_1)`.
+        return self
 
 
     def destroy(self) -> None:
         Button.buttons.pop(self.id)
         
         if self.tags is not None:
             for tag in self.tags:
                 Button.button_tags[tag].remove(self)
                 if Button.button_tags[tag] == []:
                     Button.button_tags.pop(tag)
 
         Button.page.delete(f'Button_{self.id}')
+    
+    @staticmethod
+    def destroy_by_id(id: str, /) -> None:
+        Button.buttons[id].destroy()
 
     @staticmethod
     def destroy_by_tag(tag: str, /) -> None:
-
-        if tag not in Button.button_tags:
-            return
-
         for button in list(Button.button_tags[tag]):
             button.destroy()
 
     @staticmethod
     def destroy_all() -> None:
         for button in list(Button.buttons.values()):
             button.destroy()
-    
-
-    def get_bounding_box(self) -> tuple[float, float, float, float]:
-        tl_x = self.ctr_x - self.width/2
-        tl_y = self.ctr_y - self.height/2
-        dr_x = self.ctr_x + self.width/2
-        dr_y = self.ctr_y + self.height/2
-        return [tl_x, tl_y, dr_x, dr_y]
-
-    @staticmethod
-    def get_bounding_box_by_id(id: str, /) -> tuple[float, float, float, float]:
-        return Button.buttons[id].get_bounding_box()
```

### Comparing `mykit-0.1.2/mykit/kit/gui/label/v2.py` & `mykit-0.1.3/mykit/app/label.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,13 @@
 import random as _random
 import tkinter as _tk
 import typing as _typing
 
 
 class Label:
-    """
-    The next version of `carbon.gui.label.Label`
-
-    ---
-
-    ## New:
-    - param `id` is now optional
-    - Default font set to Verdana
-    - Params `x` and `y` are now optional since the position can be adjusted using the `align` method for better positioning
-    - new methods: `get_anchor_loc`, `align`
-    """
 
     labels: dict[str, 'Label'] = {}
     label_tags: dict[str, list['Label']] = {}
 
     def __init__(
         self,
         x: int = 0,
@@ -252,18 +241,14 @@
         anchor: str = 'nw',
         target_anchor: str = 'ne',
         xgap: float = 15,
         ygap: float = 0
     ) -> 'Label':
         """
         Valid options for `anchor` and `target_anchor` are `['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']`.
-
-        NOTE: if you want to align with other widgets like `carbon.gui.button`
-              or `carbon.gui.slider`, make sure their version supports the
-              `get_anchor_loc` method
         """
 
         ## getting the target anchor location
         x, y = target.get_anchor_loc(target_anchor)
 
         ## shifting
         x += xgap
```

### Comparing `mykit-0.1.2/mykit/kit/gui/shape/__init__.py` & `mykit-0.1.3/mykit/app/arrow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import math as _math
 import random as _random
 import tkinter as _tk
 
-from carbon.math import (
+from mykit.kit.math import (
     get_angle as _get_angle,
-    rotate_coordinate as _rotate_coordinate
+    rotate as _rotate
 )
 
 
-class _Shape:
+class Arrow:
 
     page: _tk.Canvas = None
     @staticmethod
     def set_page(page: _tk.Canvas, /) -> None:
-        _Shape.page = page
-
-
-class Arrow(_Shape):
+        Arrow.page = page
 
     arrows: dict[str, 'Arrow'] = {}
     arrow_tags: dict[str, list['Arrow']] = {}
 
     def __init__(
         self,
         from_x: int, from_y: int,
@@ -75,41 +72,41 @@
         ## </tags>
 
         ## init
         self._redraw()
 
     def _redraw(self):
 
-        _Shape.page.delete(f'Arrow_{self.id}')
+        Arrow.page.delete(f'Arrow_{self.id}')
 
         if self.visible:
-            _Shape.page.create_line(
+            Arrow.page.create_line(
                 self.from_x, self.from_y,
                 self.to_x, self.to_y,
                 fill=self.color, width=self.width_rod, tags=f'Arrow_{self.id}'
             )
 
             ## <creating the tip>
             ## for `angle`: remember to flip the y-sign because tkinter's y-positive direction towards the bottom
             angle = _get_angle(self.from_x, -self.from_y, self.to_x, -self.to_y)
             
             tipx = self.tip_len*_math.sin(self.tip_angle*_math.pi/180)
             tipy = self.tip_len*_math.cos(self.tip_angle*_math.pi/180)
             
             ## Remember `tip_left` and `tip_right` with y-positive towards the top,
             ## as they transformed under normal Cartesian coordinates.
-            tip_left = _rotate_coordinate(-tipx, -tipy, 0, 0, angle)
-            tip_right = _rotate_coordinate(tipx, -tipy, 0, 0, angle)
+            tip_left = _rotate(-tipx, -tipy, 0, 0, angle)
+            tip_right = _rotate(tipx, -tipy, 0, 0, angle)
 
             ## Revert to the tkinter coordinate scheme, where y-positive is oriented downwards.
             tip_left = (self.to_x+tip_left[0], self.to_y-tip_left[1])
             tip_right = (self.to_x+tip_right[0], self.to_y-tip_right[1])
 
             tip_points = [tip_left, (self.to_x, self.to_y), tip_right]
-            _Shape.page.create_line(tip_points, fill=self.color, width=self.width_tip, tags=f'Arrow_{self.id}')
+            Arrow.page.create_line(tip_points, fill=self.color, width=self.width_tip, tags=f'Arrow_{self.id}')
             ## </creating the tip>
 
 
     def set_visibility(self, visible: bool, /):
         if visible != self.visible:
             self.visible = visible
             self._redraw()
```

### Comparing `mykit-0.1.2/mykit/kit/gui/slider/v2.py` & `mykit-0.1.3/mykit/app/slider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,15 @@
 import random as _random
 import tkinter as _tk
 import typing as _typing
 
-from carbon.utils import minmax_normalization as _norm
+from mykit.kit.utils import minmax_normalization as _norm
 
 
 class _Slider:
-    """
-    The next version of `carbon.gui.slider`
-
-    ---
-
-    ## New
-    - The page-focus mechanism is no longer used in order to reduce complexity
-    - Now the colors can be customized through arguments
-    - The slider dimension can be adjusted
-    - Params `id`, `x`, `y`, `min`, `max`, `step`, and `init` are now optional
-    - Added a `tolerance` parameter to determine how closely the cursor needs
-      to be to the slider's step values for it to move to a new value
-    """
 
     page: _tk.Canvas = None
     @staticmethod
     def set_page(page: _tk.Canvas, /):
         _Slider.page = page
 
     sliders: dict[str, '_Slider'] = {}
@@ -374,18 +361,14 @@
         anchor: str = 'nw',
         target_anchor: str = 'ne',
         xgap: float = 15,
         ygap: float = 0
     ) -> '_Slider':
         """
         Valid options for `anchor` and `target_anchor` are `['center', 'n', 'ne', 'e', 'se', 's', 'sw', 'w', 'nw']`.
-
-        NOTE: if you want to align with other widgets like `carbon.gui.label`
-              or `carbon.gui.button`, make sure their version supports the
-              `get_anchor_loc` method
         """
 
         ## getting the target anchor location
         x, y = target.get_anchor_loc(target_anchor)
 
         ## shifting
         x += xgap
```

### Comparing `mykit-0.1.2/mykit/kit/keycrate/__init__.py` & `mykit-0.1.3/mykit/kit/keycrate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re as _re
 import typing as _typing
 
-from carbon.path import open_file as _open_file
-from carbon.utils import is_valid_var_name as _is_valid_var_name
+from mykit.kit.path import open_file as _open_file
+from mykit.kit.utils import is_valid_var_name as _is_valid_var_name
 
 
 class KeyCrate:
     """
     Using a .txt file (which is easy to open, read, and modify)
     to store key-value pairs, aiming to keep it simple and fast.
     """
```

### Comparing `mykit-0.1.2/mykit/kit/math.py` & `mykit-0.1.3/mykit/kit/math.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.2/mykit/kit/neuralnet/dense/__init__.py` & `mykit-0.1.3/mykit/kit/neuralnet/dense.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as _np
 import random as _random
 import typing as _typing
 
-from carbon.math import relu as _ReLU
+from mykit.kit.math import relu as _ReLU
 
 
 class DenseNN:
     """Also known as fully connected neural networks"""
 
     def __init__(
         self,
```

### Comparing `mykit-0.1.2/mykit/kit/neuralnet/genetic/__init__.py` & `mykit-0.1.3/mykit/kit/neuralnet/genetic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import random as _random
 import numpy as _np
 import typing as _typing
 
-from carbon.neuralnet.dense import DenseNN as _DenseNN
+from mykit.kit.neuralnet.dense import DenseNN as _DenseNN
 
 
 class GeneticNN:
 
     def __init__(
         self,
         layer_sizes: list[int],
```

### Comparing `mykit-0.1.2/mykit/kit/noise.py` & `mykit-0.1.3/mykit/kit/noise.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.2/mykit/kit/path.py` & `mykit-0.1.3/mykit/kit/path.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.2/mykit/kit/quick_visual/plot2d.py` & `mykit-0.1.3/mykit/kit/quick_visual/plot2d.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tkinter as _tk
 from typing import Optional as _Optional
 
-from carbon.graph.graph2d import graph2d as _graph2d
+from mykit.kit.graph.graph2d import graph2d as _graph2d
 
 
 def plot2d(
     points: list[tuple[float, float]],
     xspan = 0.80,
     yspan = 0.65,
     graph2d_cfg: dict = {}
```

### Comparing `mykit-0.1.2/mykit/kit/time.py` & `mykit-0.1.3/mykit/kit/time.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.2/mykit/kit/utils.py` & `mykit-0.1.3/mykit/kit/utils.py`

 * *Files identical despite different names*

### Comparing `mykit-0.1.2/pyproject.toml` & `mykit-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
+
 [project]
 name = "mykit"
-version = "0.1.2"
+version = "0.1.3"
+description = "Python utility library"
 authors = [
-  { name="Nicholas Valentinus", email="nvfastplease@gmail.com" },
+  {name = "Nicholas Valentinus", email = "nvfastplease@gmail.com"},
 ]
-description = "Python utility library"
 readme = "README.md"
+license = {file = "LICENSE"}
 requires-python = ">=3.7"
 classifiers = [
+    "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+keywords = ["python", "toolkit", "mykit"]
+
 
 [project.urls]
-"Homepage" = "https://github.com/nvfp/mykit"
-"Bug Tracker" = "https://github.com/nvfp/mykit/issues"
+repo = "https://github.com/nvfp/mykit"
+tracker = "https://github.com/nvfp/mykit/issues"
```

