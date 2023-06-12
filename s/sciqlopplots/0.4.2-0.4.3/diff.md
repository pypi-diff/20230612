# Comparing `tmp/sciqlopplots-0.4.2-cp39-cp39-win_amd64.whl.zip` & `tmp/sciqlopplots-0.4.3-cp39-cp39-manylinux_2_28_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,8 @@
-Zip file size: 2684612 bytes, number of entries: 7
-?rw-rw-r--  2.0 fat     3120 b- stor 23-Jun-07 21:27 sciqlopplots-0.4.2.dist-info/METADATA
-?rw-rw-r--  2.0 fat       83 b- stor 23-Jun-07 21:27 sciqlopplots-0.4.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1585 b- stor 23-Jun-07 21:18 sciqlopplots-0.4.2.dist-info/COPYING
--rw-rw-rw-  2.0 fat  2675712 b- stor 23-Jun-07 21:27 SciQLopPlots/SciQLopPlotsBindings.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2232 b- stor 23-Jun-07 21:27 SciQLopPlots/SciQLopPlotsBindings.cp39-win_amd64.lib
--rw-rw-rw-  2.0 fat      171 b- stor 23-Jun-07 21:18 SciQLopPlots/__init__.py
-?rw-rw-r--  2.0 fat      615 b- stor 23-Jun-07 21:27 sciqlopplots-0.4.2.dist-info/RECORD
-7 files, 2683518 bytes uncompressed, 2683518 bytes compressed:  0.0%
+Zip file size: 5257532 bytes, number of entries: 6
+?rw-rw-r--  2.0 unx     3120 b- stor 23-Jun-12 09:27 sciqlopplots-0.4.3.dist-info/METADATA
+?rw-rw-r--  2.0 unx       86 b- stor 23-Jun-12 09:27 sciqlopplots-0.4.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1552 b- stor 23-Jun-12 09:20 sciqlopplots-0.4.3.dist-info/COPYING
+-rwxr-xr-x  2.0 unx  5251152 b- stor 23-Jun-12 09:27 SciQLopPlots/SciQLopPlotsBindings.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      166 b- stor 23-Jun-12 09:20 SciQLopPlots/__init__.py
+?rw-rw-r--  2.0 unx      518 b- stor 23-Jun-12 09:27 sciqlopplots-0.4.3.dist-info/RECORD
+6 files, 5256594 bytes uncompressed, 5256594 bytes compressed:  0.0%
```

## zipnote {}

```diff
@@ -1,22 +1,19 @@
-Filename: sciqlopplots-0.4.2.dist-info/METADATA
+Filename: sciqlopplots-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: sciqlopplots-0.4.2.dist-info/WHEEL
+Filename: sciqlopplots-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: sciqlopplots-0.4.2.dist-info/COPYING
+Filename: sciqlopplots-0.4.3.dist-info/COPYING
 Comment: 
 
-Filename: SciQLopPlots/SciQLopPlotsBindings.cp39-win_amd64.pyd
-Comment: 
-
-Filename: SciQLopPlots/SciQLopPlotsBindings.cp39-win_amd64.lib
+Filename: SciQLopPlots/SciQLopPlotsBindings.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
 Filename: SciQLopPlots/__init__.py
 Comment: 
 
-Filename: sciqlopplots-0.4.2.dist-info/RECORD
+Filename: sciqlopplots-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## SciQLopPlots/__init__.py

```diff
@@ -1,5 +1,5 @@
-from PySide6 import QtCore, QtGui, QtWidgets
-from .SciQLopPlotsBindings import *
-from .SciQLopPlotsBindings import _QCustomPlot as QCustomPlot
-
-__version__ = '0.4.2'
+from PySide6 import QtCore, QtGui, QtWidgets
+from .SciQLopPlotsBindings import *
+from .SciQLopPlotsBindings import _QCustomPlot as QCustomPlot
+
+__version__ = '0.4.3'
```

## Comparing `sciqlopplots-0.4.2.dist-info/METADATA` & `sciqlopplots-0.4.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciqlopplots
-Version: 0.4.2
+Version: 0.4.3
 Summary: SciQLop plot API based on QCustomPlot
 Home-page: https://github.com/SciQLop/SciQLopPlots
 Author-Email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 License: GNU GENERAL PUBLIC LICENSE
                               Version 3, 29 June 2007
         
             An easy to use ISTP loader package.
```

## Comparing `sciqlopplots-0.4.2.dist-info/COPYING` & `sciqlopplots-0.4.3.dist-info/COPYING`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-GNU GENERAL PUBLIC LICENSE
-                      Version 3, 29 June 2007
-
-    An easy to use ISTP loader package.
-    Copyright (C) 2022  Alexis Jeandet
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
-
+GNU GENERAL PUBLIC LICENSE
+                      Version 3, 29 June 2007
+
+    An easy to use ISTP loader package.
+    Copyright (C) 2022  Alexis Jeandet
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<http://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+
```

