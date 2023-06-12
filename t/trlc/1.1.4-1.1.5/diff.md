# Comparing `tmp/trlc-1.1.4.tar.gz` & `tmp/trlc-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trlc-1.1.4.tar", last modified: Tue May  9 09:56:34 2023, max compression
+gzip compressed data, was "trlc-1.1.5.tar", last modified: Mon Jun 12 13:03:47 2023, max compression
```

## Comparing `trlc-1.1.4.tar` & `trlc-1.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:56:34.656125 trlc-1.1.4/
--rw-r--r--   0 florian   (1000) florian   (1000)    35149 2022-12-05 12:42:52.000000 trlc-1.1.4/LICENSE
--rw-r--r--   0 florian   (1000) florian   (1000)     2965 2023-05-09 09:56:34.656125 trlc-1.1.4/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1875 2023-03-01 10:58:12.000000 trlc-1.1.4/README.md
--rw-r--r--   0 florian   (1000) florian   (1000)      103 2023-05-09 09:56:34.656125 trlc-1.1.4/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2135 2023-02-21 07:05:56.000000 trlc-1.1.4/setup.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:56:34.652125 trlc-1.1.4/trlc/
--rw-r--r--   0 florian   (1000) florian   (1000)      815 2022-12-05 12:42:52.000000 trlc-1.1.4/trlc/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    96878 2023-05-08 15:02:21.000000 trlc-1.1.4/trlc/ast.py
--rw-r--r--   0 florian   (1000) florian   (1000)     7223 2023-05-09 09:56:21.000000 trlc-1.1.4/trlc/errors.py
--rw-r--r--   0 florian   (1000) florian   (1000)    15766 2023-05-09 09:56:21.000000 trlc-1.1.4/trlc/lexer.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2475 2023-04-28 09:15:42.000000 trlc-1.1.4/trlc/lint.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1266 2023-03-23 13:32:34.000000 trlc-1.1.4/trlc/math.py
--rw-r--r--   0 florian   (1000) florian   (1000)     3351 2023-03-23 13:32:34.000000 trlc-1.1.4/trlc/nested.py
--rw-r--r--   0 florian   (1000) florian   (1000)    59273 2023-05-09 09:56:21.000000 trlc-1.1.4/trlc/parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)    16319 2023-04-28 09:15:42.000000 trlc-1.1.4/trlc/trlc.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1004 2023-05-09 09:56:30.000000 trlc-1.1.4/trlc/version.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:56:34.656125 trlc-1.1.4/trlc.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     2965 2023-05-09 09:56:34.000000 trlc-1.1.4/trlc.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      322 2023-05-09 09:56:34.000000 trlc-1.1.4/trlc.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-09 09:56:34.000000 trlc-1.1.4/trlc.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       40 2023-05-09 09:56:34.000000 trlc-1.1.4/trlc.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        5 2023-05-09 09:56:34.000000 trlc-1.1.4/trlc.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-12 13:03:47.965439 trlc-1.1.5/
+-rw-r--r--   0 florian   (1000) florian   (1000)    35149 2022-12-05 12:42:52.000000 trlc-1.1.5/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)     3224 2023-06-12 13:03:47.965439 trlc-1.1.5/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     2075 2023-06-12 13:00:29.000000 trlc-1.1.5/README.md
+-rw-r--r--   0 florian   (1000) florian   (1000)      103 2023-06-12 13:03:47.965439 trlc-1.1.5/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2135 2023-02-21 07:05:56.000000 trlc-1.1.5/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-12 13:03:47.965439 trlc-1.1.5/trlc/
+-rw-r--r--   0 florian   (1000) florian   (1000)      815 2022-12-05 12:42:52.000000 trlc-1.1.5/trlc/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)   100290 2023-06-12 13:00:29.000000 trlc-1.1.5/trlc/ast.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     7549 2023-06-12 13:00:29.000000 trlc-1.1.5/trlc/errors.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    19208 2023-06-12 13:00:29.000000 trlc-1.1.5/trlc/lexer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     5478 2023-06-12 13:00:29.000000 trlc-1.1.5/trlc/lint.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1266 2023-03-23 13:32:34.000000 trlc-1.1.5/trlc/math.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     3351 2023-03-23 13:32:34.000000 trlc-1.1.5/trlc/nested.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    59079 2023-06-12 13:00:29.000000 trlc-1.1.5/trlc/parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    16542 2023-06-12 13:00:29.000000 trlc-1.1.5/trlc/trlc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1004 2023-06-12 13:03:41.000000 trlc-1.1.5/trlc/version.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-12 13:03:47.965439 trlc-1.1.5/trlc.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     3224 2023-06-12 13:03:47.000000 trlc-1.1.5/trlc.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      322 2023-06-12 13:03:47.000000 trlc-1.1.5/trlc.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-12 13:03:47.000000 trlc-1.1.5/trlc.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       40 2023-06-12 13:03:47.000000 trlc-1.1.5/trlc.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        5 2023-06-12 13:03:47.000000 trlc-1.1.5/trlc.egg-info/top_level.txt
```

### Comparing `trlc-1.1.4/LICENSE` & `trlc-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `trlc-1.1.4/PKG-INFO` & `trlc-1.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trlc
-Version: 1.1.4
+Version: 1.1.5
 Summary: Treat Requirements Like Code
 Home-page: https://github.com/bmw-software-engineering/trlc
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/trlc/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/trlc/
@@ -23,15 +23,15 @@
 TRLC is a domain-specific language developed at BMW for writing (and
 linking) requirements with meta-data.
 
 The repository contains:
 
 * The [language reference
   manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
-  for TRLC.
+  for TRLC. [Previous versions](https://github.com/bmw-software-engineering/trlc/blob/main/docs/LRM.md) are also available.
 
 * A pure Python reference implementation of TRLC.
 
 The implementation is not very fast, but designed to be pedantically
 correct in following the language definition.  Eventually it will also
 contain a powerful linter to find issues with types and check
 rules.
@@ -46,22 +46,29 @@
 * The API can be used to write other tools based on TRLC (for example
   a tool to render the requirements in HTML, a tool to diff
   requirements or perform an impact analysis, or a tool to perform
   software traceability, etc.)
 
 ## Documentation
 
+### For users
+
 * [Tutorial](https://github.com/bmw-software-engineering/trlc/blob/main/TUTORIAL.md) (read this as a first introduction)
 * [Release Notes](https://github.com/bmw-software-engineering/trlc/blob/main/CHANGELOG.md) (read this to find out whats new)
-* [Python API Documentation](https://bmw-software-engineering.github.io/trlc/)
-  (user guide for using the API)
 * [Language Reference Manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
   (for language lawyers)
 * [License](https://github.com/bmw-software-engineering/trlc/blob/main/LICENSE)
 
+### For developers
+
+* [Python API Documentation](https://bmw-software-engineering.github.io/trlc/)
+  (API reference)
+* [AST Hierarchy](https://bmw-software-engineering.github.io/trlc/ast_hierarchy.svg)
+  (overview over all classes in the AST)
+
 ## Dependencies
 
 ### Run-time
 * Python3 >= 3.7
 
 ### Development tools
 * GNU Make
```

### Comparing `trlc-1.1.4/README.md` & `trlc-1.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 TRLC is a domain-specific language developed at BMW for writing (and
 linking) requirements with meta-data.
 
 The repository contains:
 
 * The [language reference
   manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
-  for TRLC.
+  for TRLC. [Previous versions](docs/LRM.md) are also available.
 
 * A pure Python reference implementation of TRLC.
 
 The implementation is not very fast, but designed to be pedantically
 correct in following the language definition.  Eventually it will also
 contain a powerful linter to find issues with types and check
 rules.
@@ -25,22 +25,29 @@
 * The API can be used to write other tools based on TRLC (for example
   a tool to render the requirements in HTML, a tool to diff
   requirements or perform an impact analysis, or a tool to perform
   software traceability, etc.)
 
 ## Documentation
 
+### For users
+
 * [Tutorial](TUTORIAL.md) (read this as a first introduction)
 * [Release Notes](CHANGELOG.md) (read this to find out whats new)
-* [Python API Documentation](https://bmw-software-engineering.github.io/trlc/)
-  (user guide for using the API)
 * [Language Reference Manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
   (for language lawyers)
 * [License](LICENSE)
 
+### For developers
+
+* [Python API Documentation](https://bmw-software-engineering.github.io/trlc/)
+  (API reference)
+* [AST Hierarchy](https://bmw-software-engineering.github.io/trlc/ast_hierarchy.svg)
+  (overview over all classes in the AST)
+
 ## Dependencies
 
 ### Run-time
 * Python3 >= 3.7
 
 ### Development tools
 * GNU Make
```

### Comparing `trlc-1.1.4/setup.py` & `trlc-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.4/trlc/__init__.py` & `trlc-1.1.5/trlc/__init__.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.4/trlc/ast.py` & `trlc-1.1.5/trlc/ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,100 @@
                Builtin_Function startswith
 
         """
         assert isinstance(indent, int) and indent >= 0
         assert False, "dump not implemented for %s" % self.__class__.__name__
 
 
+class Check_Block(Node):
+    """Node representing check blocks
+
+    Semantically this has no meaning, but it's nice to have some kind
+    of similar representation to how it's in the file.
+
+    :attribute n_typ: composite type for which the checks apply
+    :type: Composite_Type
+
+    :attribute checks: list of checks
+    :type: list[Check]
+
+    """
+    def __init__(self, location, n_typ):
+        super().__init__(location)
+        assert isinstance(n_typ, Composite_Type)
+        self.n_typ  = n_typ
+        self.checks = []
+
+    def add_check(self, n_check):
+        assert isinstance(n_check, Check)
+        self.checks.append(n_check)
+
+
+class Compilation_Unit(Node):
+    """Special node to represent the concrete file structure
+
+    :attribute package: the main package this file declares or contributes to
+    :type: Package
+
+    :attribute imports: package imported by this file
+    :type: list[Package]
+
+    :attribute items: list of
+    :type: list[Node]
+
+    """
+    def __init__(self, file_name):
+        super().__init__(Location(file_name))
+        self.package       = None
+        self.imports       = None
+        self.raw_imports   = []
+        self.items         = []
+
+    def set_package(self, pkg):
+        assert isinstance(pkg, Package)
+        self.package = pkg
+
+    def add_import(self, mh, t_import):
+        assert isinstance(mh, Message_Handler)
+        assert isinstance(t_import, Token)
+        assert t_import.kind == "IDENTIFIER"
+
+        if t_import.value == self.package.name:
+            mh.error(t_import.location,
+                     "package %s cannot import itself" % self.package.name)
+
+        # Skip duplicates
+        for t_previous in self.raw_imports:
+            if t_previous.value == t_import.value:
+                mh.warning(t_import.location,
+                           "duplicate import of package %s" % t_import.value)
+                return
+
+        self.raw_imports.append(t_import)
+
+    def resolve_imports(self, mh, stab):
+        assert isinstance(mh, Message_Handler)
+        assert isinstance(stab, Symbol_Table)
+        self.imports = set()
+        for t_import in self.raw_imports:
+            self.imports.add(stab.lookup(mh, t_import, Package))
+
+    def is_visible(self, n_pkg):
+        assert self.imports is not None
+        assert isinstance(n_pkg, Package)
+        return n_pkg == self.package or n_pkg in self.imports
+
+    def add_item(self, node):
+        assert isinstance(node, (Concrete_Type,
+                                 Check_Block,
+                                 Record_Object)), \
+            "trying to add %s to a compilation unit" % node.__class__.__name__
+        self.items.append(node)
+
+
 class Check(Node):
     """User defined check
 
     This represent a single user-defined check inside a check block::
 
       checks T {
           a /= null implies a > 5, warning "potato", a
@@ -1901,27 +1987,41 @@
 
       foo Integer [5 .. *]
                   ^
 
     :attribute lower_bound: minimum number of elements
     :type: int
 
+    :attribute loc_lower: text location of the lower bound indicator
+    :type: Location
+
     :attribute upper_bound: maximum number of elements (or None)
     :type: int
 
+    :attribute loc_upper: text location of the upper bound indicator
+    :type: Location
+
     :attribute element_type: type of the array elements
     :type: Type
 
     """
-    def __init__(self, location, element_type, lower_bound, upper_bound):
+    def __init__(self,
+                 location,
+                 element_type,
+                 loc_lower,
+                 lower_bound,
+                 loc_upper,
+                 upper_bound):
         assert isinstance(element_type, Type) or element_type is None
         assert isinstance(lower_bound, int)
         assert lower_bound >= 0
         assert upper_bound is None or isinstance(upper_bound, int)
         assert upper_bound is None or upper_bound >= 0
+        assert isinstance(loc_lower, Location)
+        assert isinstance(loc_upper, Location)
 
         if element_type is None:
             name = "universal array"
         elif upper_bound is None:
             if lower_bound == 0:
                 name = "array of %s" % element_type.name
             else:
@@ -1932,15 +2032,17 @@
                                        element_type.name)
         else:
             name = "array of %u to %u %s" % (lower_bound,
                                              upper_bound,
                                              element_type.name)
         super().__init__(name, location)
         self.lower_bound  = lower_bound
+        self.loc_lower    = loc_lower
         self.upper_bound  = upper_bound
+        self.loc_upper    = loc_upper
         self.element_type = element_type
 
     def perform_type_checks(self, mh, value):
         assert isinstance(mh, Message_Handler)
         if isinstance(value, Array_Aggregate):
             return all(self.element_type.perform_type_checks(mh, v)
                        for v in value.value)
@@ -1986,27 +2088,33 @@
     """Packages.
 
     A package is declared when it is first encountered (in either a
     rsl or trlc file). A package contains all symbols declared in it,
     both types and record objects. A package is not associated with
     just a single file, it can be spread over multiple files.
 
+    :attribute declared_late: indicates if this package is declared in a \
+      trlc file
+    :type: bool
+
     :attribute symbols: symbol table of the package
     :type: Symbol_Table
 
     """
-    def __init__(self, name, location, builtin_stab):
+    def __init__(self, name, location, builtin_stab, declared_late):
         super().__init__(name, location)
         assert isinstance(builtin_stab, Symbol_Table)
+        assert isinstance(declared_late, bool)
         self.symbols = Symbol_Table()
         self.symbols.make_visible(builtin_stab)
-        self.declared_late = False
+        self.declared_late = declared_late
 
     def dump(self, indent=0):  # pragma: no cover
         self.write_indent(indent, "Package %s" % self.name)
+        self.write_indent(indent + 1, "Declared_Late: %s" % self.declared_late)
         self.symbols.dump(indent + 1, omit_heading=True)
 
 
 class Composite_Type(Concrete_Type):
     """Abstract base for record and tuple types, as they share some
        functionality.
```

### Comparing `trlc-1.1.4/trlc/errors.py` & `trlc-1.1.5/trlc/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 #
 # TRLC - Treat Requirements Like Code
-# Copyright (C) 2022 Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
+# Copyright (C) 2022-2023 Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 #
 # This file is part of the TRLC Python Reference Implementation.
 #
 # TRLC is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -14,15 +14,14 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
 # or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public
 # License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with TRLC. If not, see <https://www.gnu.org/licenses/>.
 
-import os.path
 import sys
 
 
 class Location:
     """Reference to a source or virtual location
 
     Any message raised by the :class:`Message_Handler` will be
@@ -227,14 +226,25 @@
             kind = "check warning"
         else:
             kind = "warning"
 
         self.warnings += 1
         self.emit(location, kind, message, fatal=False)
 
+    def check(self, location, message, check):
+        assert isinstance(location, Location)
+        assert isinstance(message, str)
+        assert isinstance(check, str)
+
+        self.warnings += 1
+        self.emit(location,
+                  "warning",
+                  "%s [%s]" % (message, check),
+                  fatal=False)
+
     def ice_loc(self, location, message):  # pragma: no cover
         assert isinstance(location, Location)
         assert isinstance(message, str)
 
         self.errors += 1
         self.emit(location, "ICE", message, fatal=False)
         sys.exit(1)
```

### Comparing `trlc-1.1.4/trlc/lexer.py` & `trlc-1.1.5/trlc/lexer.py`

 * *Files 14% similar despite different names*

```diff
@@ -415,30 +415,102 @@
                                          start_col  = start_col,
                                          start_pos  = start_pos,
                                          end_pos    = self.lexpos),
                         "unterminated triple-quoted string")
 
         elif self.is_numeric(self.cc):
             kind = "INTEGER"
-            while self.nc and self.is_numeric(self.nc):
-                self.advance()
 
-            if self.nc == "." and self.nnc != ".":
-                kind = "DECIMAL"
+            if self.cc == "0" and self.nc == "b":
+                digits_allowed   = "01"
+                digits_forbidden = "23456789abcdefABCDEF"
+                int_base         = 2
+                require_digit    = True
+                decimal_allowed  = False
+                self.advance()
+            elif self.cc == "0" and self.nc == "x":
+                digits_allowed   = "0123456789abcdefABCDEF"
+                digits_forbidden = ""
+                int_base         = 16
+                require_digit    = True
+                decimal_allowed  = False
                 self.advance()
-                if not self.nc or not self.is_numeric(self.nc):
+            else:
+                digits_allowed   = "0123456789"
+                digits_forbidden = "abcdefABCDEF"
+                int_base         = 10
+                require_digit    = False
+                decimal_allowed  = True
+
+            while self.nc:
+                if self.nc in digits_allowed:
+                    self.advance()
+                    require_digit = False
+
+                elif self.nc in digits_forbidden:
                     self.mh.lex_error(
                         Source_Reference(lexer      = self,
                                          start_line = start_line,
                                          start_col  = start_col,
-                                         start_pos  = start_pos,
-                                         end_pos    = self.lexpos),
-                        "unfinished decimal number")
-                while self.nc and self.is_numeric(self.nc):
+                                         start_pos  = self.lexpos + 1,
+                                         end_pos    = self.lexpos + 1),
+                        "%s is not a valid base %u digit" % (self.nc,
+                                                             int_base))
+
+                elif require_digit:
+                    self.mh.lex_error(
+                        Source_Reference(lexer      = self,
+                                         start_line = start_line,
+                                         start_col  = start_col,
+                                         start_pos  = self.lexpos + 1,
+                                         end_pos    = self.lexpos + 1),
+                        "base %u digit is required here" % int_base)
+
+                elif self.nc == "_":
                     self.advance()
+                    require_digit = True
+
+                elif self.nc == "." and self.nnc == ".":
+                    # This is a range token, so that one can't be part
+                    # of our number anymore
+                    break
+
+                elif self.nc == ".":
+                    self.advance()
+                    if not decimal_allowed:
+                        if int_base == 10:
+                            msg = "decimal point is not allowed here"
+                        else:
+                            msg = ("base %u integer may not contain a"
+                                   " decimal point" % int_base)
+                        self.mh.lex_error(
+                            Source_Reference(lexer      = self,
+                                             start_line = start_line,
+                                             start_col  = start_col,
+                                             start_pos  = self.lexpos,
+                                             end_pos    = self.lexpos),
+                            msg)
+                    decimal_allowed   = False
+                    require_digit     = True
+                    kind              = "DECIMAL"
+
+                else:  # pragma: no cover
+                    # This is actually a false
+                    # alarm, this line is covered (it's the only
+                    # normal way to exit this loop.
+                    break
+
+            if require_digit:
+                self.mh.lex_error(
+                    Source_Reference(lexer      = self,
+                                     start_line = start_line,
+                                     start_col  = start_col,
+                                     start_pos  = start_pos,
+                                     end_pos    = self.lexpos),
+                    "unfinished base %u integer" % int_base)
 
         else:
             self.mh.lex_error(self.current_location(),
                               "unexpected character '%s'" % self.cc)
 
         sref = Source_Reference(lexer      = self,
                                 start_line = start_line,
@@ -465,18 +537,24 @@
             if value.startswith('"'):
                 value = value[1:-1]
                 value = value.replace('\\"', '"')
             else:
                 value = triple_quoted_string_value(value)
 
         elif kind == "INTEGER":
-            value = int(sref.text())
+            base_text = sref.text().replace("_", "")
+            if int_base == 10:
+                value = int(base_text)
+            elif int_base == 2:
+                value = int(base_text[2:], base=2)
+            else:
+                value = int(base_text[2:], base=16)
 
         elif kind == "DECIMAL":
-            value = Fraction(sref.text())
+            value = Fraction(sref.text().replace("_", ""))
 
         elif kind == "COMMENT":
             value = sref.text()
             if value.startswith("//"):
                 value = value[2:].strip()
             else:
                 value = value[2:]
```

### Comparing `trlc-1.1.4/trlc/math.py` & `trlc-1.1.5/trlc/math.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.4/trlc/nested.py` & `trlc-1.1.5/trlc/nested.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.4/trlc/parser.py` & `trlc-1.1.5/trlc/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,23 +238,22 @@
         self.match("REFLIST_IDENTIFIER")
         if self.peek("REFLIST_DOT"):
             package = self.parent.stab.lookup_direct(
                 mh                = self.mh,
                 name              = self.ct.value,
                 error_location    = self.ct.location,
                 required_subclass = ast.Package)
-            if package != self.parent.pkg and \
-               package.name not in self.parent.imports:
+            if not self.parent.cu.is_visible(package):
                 self.mh.error(self.ct.location,
                               "package must be imported before use")
 
             self.match("REFLIST_DOT")
             self.match("REFLIST_IDENTIFIER")
         else:
-            package = self.parent.pkg
+            package = self.parent.cu.package
 
         ref = ast.Record_Reference(location = self.ct.location,
                                    name     = self.ct.value,
                                    typ      = None,
                                    package  = package)
         self.references.append(ref)
 
@@ -277,18 +276,15 @@
         else:
             super().__init__(mh, TRLC_Lexer(mh, file_name),
                              eoc_name  = "end-of-file",
                              token_map = Token.KIND,
                              keywords  = TRLC_Lexer.KEYWORDS)
         self.lint_mode = lint_mode
         self.stab      = stab
-        self.pkg       = None
-        self.raw_deps  = []
-        self.deps      = []
-        self.imports   = set()
+        self.cu        = ast.Compilation_Unit(file_name)
 
         self.builtin_bool    = stab.table["Boolean"]
         self.builtin_int     = stab.table["Integer"]
         self.builtin_decimal = stab.table["Decimal"]
         self.builtin_str     = stab.table["String"]
         self.builtin_mstr    = stab.table["Markup_String"]
 
@@ -315,51 +311,56 @@
         assert isinstance(match_ident, bool)
 
         if match_ident:
             self.match("IDENTIFIER")
         sym = scope.lookup(self.mh, self.ct)
 
         if isinstance(sym, ast.Package):
-            if sym != self.pkg and sym.name not in self.imports:
+            if not self.cu.is_visible(sym):
                 self.mh.error(self.ct.location,
                               "package must be imported before use")
             self.match("DOT")
             self.match("IDENTIFIER")
             return sym.symbols.lookup(self.mh, self.ct, required_subclass)
         else:
+            # Easiest way to generate the correct error message
             return scope.lookup(self.mh, self.ct, required_subclass)
 
     def parse_type_declaration(self):
         if self.peek_kw("enum"):
-            self.parse_enum_declaration()
+            n_item = self.parse_enum_declaration()
         elif self.peek_kw("tuple"):
-            self.parse_tuple_declaration()
+            n_item = self.parse_tuple_declaration()
         else:
-            self.parse_record_declaration()
+            n_item = self.parse_record_declaration()
+        assert isinstance(n_item, ast.Concrete_Type)
+        return n_item
 
     def parse_enum_declaration(self):
         self.match_kw("enum")
         name, description = self.parse_described_name()
 
         enum = ast.Enumeration_Type(name        = name.value,
                                     description = description,
                                     location    = name.location,
-                                    package     = self.pkg)
-        self.pkg.symbols.register(self.mh, enum)
+                                    package     = self.cu.package)
+        self.cu.package.symbols.register(self.mh, enum)
 
         self.match("C_BRA")
         while not self.peek("C_KET"):
             name, description = self.parse_described_name()
             lit = ast.Enumeration_Literal_Spec(name        = name.value,
                                                description = description,
                                                location    = name.location,
                                                enum        = enum)
             enum.literals.register(self.mh, lit)
         self.match("C_KET")
 
+        return enum
+
     def parse_tuple_field(self,
                           n_tuple,
                           optional_allowed,
                           optional_reason,
                           optional_required):
         assert isinstance(n_tuple, ast.Tuple_Type)
         assert isinstance(optional_allowed, bool)
@@ -392,15 +393,15 @@
     def parse_tuple_declaration(self):
         self.match_kw("tuple")
         name, description = self.parse_described_name()
 
         n_tuple = ast.Tuple_Type(name        = name.value,
                                  description = description,
                                  location    = name.location,
-                                 package     = self.pkg)
+                                 package     = self.cu.package)
 
         self.match("C_BRA")
 
         n_field = self.parse_tuple_field(
             n_tuple,
             optional_allowed  = False,
             optional_reason   = "first field may not be optional",
@@ -435,15 +436,17 @@
                 optional_required = optional_required)
             n_tuple.components.register(self.mh, n_field)
             optional_required |= n_field.optional
 
         self.match("C_KET")
 
         # Late registration to avoid recursion in tuples
-        self.pkg.symbols.register(self.mh, n_tuple)
+        self.cu.package.symbols.register(self.mh, n_tuple)
+
+        return n_tuple
 
     def parse_record_component(self, n_record):
         assert isinstance(n_record, ast.Record_Type)
 
         c_name, c_descr = self.parse_described_name()
         if self.peek_kw("optional"):
             self.match_kw("optional")
@@ -453,47 +456,34 @@
         c_typ = self.parse_qualified_name(self.default_scope,
                                           ast.Type)
 
         if self.peek("S_BRA"):
             self.match("S_BRA")
             self.match("INTEGER")
             a_lo = self.ct.value
+            loc_lo = self.ct.location
             self.match("RANGE")
             a_loc = self.ct.location
             if self.peek("INTEGER"):
                 self.match("INTEGER")
                 a_hi = self.ct.value
-                if a_lo > a_hi:
-                    self.mh.error(self.ct.location,
-                                  "upper bound must be at least %u" % a_lo,
-                                  fatal = False)
-                elif a_hi == 0:
-                    self.mh.error(self.ct.location,
-                                  "this array makes no sense",
-                                  fatal = False)
-                elif a_hi == 1 and a_lo == 1:
-                    self.mh.warning(a_loc,
-                                    "array of fixed size 1 "
-                                    "should not be an array")
-                elif a_hi == 1 and a_lo == 0:
-                    self.mh.warning(a_loc,
-                                    "consider making this array an"
-                                    " optional %s" % c_typ.name)
-
             elif self.peek("OPERATOR") and self.nt.value == "*":
                 self.match("OPERATOR")
                 a_hi = None
             else:
                 self.mh.error(self.nt.location,
                               "expected INTEGER or * for upper bound")
+            loc_hi = self.ct.location
             self.match("S_KET")
             c_typ = ast.Array_Type(location     = a_loc,
                                    element_type = c_typ,
                                    lower_bound  = a_lo,
-                                   upper_bound  = a_hi)
+                                   upper_bound  = a_hi,
+                                   loc_lower    = loc_lo,
+                                   loc_upper    = loc_hi)
 
         return ast.Composite_Component(name        = c_name.value,
                                        description = c_descr,
                                        location    = c_name.location,
                                        member_of   = n_record,
                                        n_typ       = c_typ,
                                        optional    = c_optional)
@@ -520,24 +510,25 @@
                                                     ast.Record_Type)
         else:
             root_record = None
 
         if self.lint_mode and \
            root_record and root_record.is_final and \
            not is_final:
-            self.mh.warning(name.location,
-                            "consider clarifying that this record is final")
+            self.mh.check(name.location,
+                          "consider clarifying that this record is final",
+                          "clarify_final")
 
         record = ast.Record_Type(name        = name.value,
                                  description = description,
                                  location    = name.location,
-                                 package     = self.pkg,
+                                 package     = self.cu.package,
                                  n_parent    = root_record,
                                  is_abstract = is_abstract)
-        self.pkg.symbols.register(self.mh, record)
+        self.cu.package.symbols.register(self.mh, record)
 
         self.match("C_BRA")
         while not self.peek("C_KET"):
             if self.peek_kw("freeze"):
                 self.match_kw("freeze")
                 self.match("IDENTIFIER")
                 n_comp = record.components.lookup(self.mh,
@@ -566,14 +557,16 @@
 
         self.match("C_KET")
 
         # Finally mark record final if applicable
         if is_final:
             record.is_final = True
 
+        return record
+
     def parse_expression(self, scope):
         assert isinstance(scope, ast.Scope)
 
         n_lhs = self.parse_relation(scope)
 
         if self.peek_kw("and"):
             while self.peek_kw("and"):
@@ -729,18 +722,19 @@
             t_unary = None
 
         n_lhs = self.parse_term(scope)
         if t_unary:
             if self.lint_mode and \
                isinstance(n_lhs, ast.Binary_Expression) and \
                not has_explicit_brackets:
-                self.mh.warning(t_unary.location,
-                                "expression means -(%s), place explicit "
-                                "brackets to clarify intent" %
-                                n_lhs.to_string())
+                self.mh.check(t_unary.location,
+                              "expression means -(%s), place explicit "
+                              "brackets to clarify intent" %
+                              n_lhs.to_string(),
+                              "unary_minus_precedence")
             n_lhs = ast.Unary_Expression(
                 mh        = self.mh,
                 location  = t_unary.location,
                 typ       = n_lhs.typ,
                 operator  = un_add_map[t_unary.value],
                 n_operand = n_lhs)
 
@@ -944,18 +938,19 @@
         assert isinstance(n_name, (ast.Builtin_Function,
                                    ast.Builtin_Numeric_Type))
         assert isinstance(t_name, Token)
 
         # Lint: complain about old functions
         if isinstance(n_name, ast.Builtin_Function) and \
            self.lint_mode and n_name.deprecated:
-            self.mh.warning(
+            self.mh.check(
                 t_name.location,
-                "deprecated feature, please use function %s instead" %
-                n_name.name.replace("trlc:", ""))
+                "please use function %s instead" %
+                n_name.name.replace("trlc:", ""),
+                "deprecated_feature")
 
         # Parse the arguments.
         parameters = []
         self.match("BRA")
         while not self.peek("KET"):
             parameters.append(self.parse_expression(scope))
             if self.peek("COMMA"):
@@ -1170,18 +1165,22 @@
                     n_rhs    = n_index)
 
         return n_name
 
     def parse_check_block(self):
         self.match_kw("checks")
         self.match("IDENTIFIER")
-        n_ctype = self.pkg.symbols.lookup(self.mh, self.ct, ast.Composite_Type)
+        n_ctype = self.cu.package.symbols.lookup(self.mh,
+                                                 self.ct,
+                                                 ast.Composite_Type)
+        n_check_block = ast.Check_Block(location = self.ct.location,
+                                        n_typ    = n_ctype)
         scope = ast.Scope()
         scope.push(self.stab)
-        scope.push(self.pkg.symbols)
+        scope.push(self.cu.package.symbols)
         scope.push(n_ctype.components)
         self.match("C_BRA")
         while not self.peek("C_KET"):
             c_expr = self.parse_expression(scope)
 
             self.match("COMMA")
             if self.peek("KEYWORD"):
@@ -1207,19 +1206,22 @@
 
             n_check = ast.Check(n_type    = n_ctype,
                                 n_expr    = c_expr,
                                 n_anchor  = c_anchor,
                                 severity  = c_sev,
                                 t_message = t_msg)
             n_ctype.add_check(n_check)
+            n_check_block.add_check(n_check)
 
             assert scope.size() == 3
 
         self.match("C_KET")
 
+        return n_check_block
+
     def parse_section_declaration(self):
         self.match_kw("section")
         self.match("STRING")
         if self.section:
             sec = ast.Section(name     = self.ct.value,
                               location = self.ct.location,
                               parent   = self.section[-1])
@@ -1327,35 +1329,29 @@
         elif isinstance(typ, ast.Record_Type):
             self.match("IDENTIFIER")
             t_name = self.ct
             if self.peek("DOT"):
                 self.match("DOT")
                 self.match("IDENTIFIER")
                 the_pkg = self.stab.lookup(self.mh, t_name, ast.Package)
-                if the_pkg != self.pkg and the_pkg.name not in self.imports:
+                if not self.cu.is_visible(the_pkg):
                     self.mh.error(self.ct.location,
                                   "package must be imported before use")
                 t_name = self.ct
             else:
-                the_pkg = self.pkg
+                the_pkg = self.cu.package
 
             rv = ast.Record_Reference(location = t_name.location,
                                       name     = t_name.value,
                                       typ      = typ,
                                       package  = the_pkg)
+
+            # We can do an early lookup if the target is known
             if the_pkg.symbols.contains(t_name.value):
-                rv.target = the_pkg.symbols.lookup(self.mh,
-                                                   t_name,
-                                                   ast.Record_Object)
-                if not rv.target.n_typ.is_subclass_of(typ):
-                    self.mh.error(t_name.location,
-                                  "incorrect type, expected %s but %s is %s" %
-                                  (typ.name,
-                                   rv.name,
-                                   rv.target.n_typ.name))
+                rv.resolve_references(self.mh)
 
             return rv
 
         elif isinstance(typ, ast.Tuple_Type) and typ.has_separators():
             rv = ast.Tuple_Aggregate(self.nt.location, typ)
 
             next_is_optional = False
@@ -1422,16 +1418,16 @@
 
         self.match("IDENTIFIER")
         obj = ast.Record_Object(
             name      = self.ct.value,
             location  = self.ct.location,
             n_typ     = r_typ,
             section   = self.section[-1] if self.section else None,
-            n_package = self.pkg)
-        self.pkg.symbols.register(self.mh, obj)
+            n_package = self.cu.package)
+        self.cu.package.symbols.register(self.mh, obj)
 
         self.match("C_BRA")
         while not self.peek("C_KET"):
             self.match("IDENTIFIER")
             comp = r_typ.components.lookup(self.mh,
                                            self.ct,
                                            ast.Composite_Component)
@@ -1455,80 +1451,86 @@
                         (comp.name,
                          self.mh.cross_file_reference(comp.location)))
                 else:
                     obj.assign(comp, ast.Implicit_Null(obj, comp))
 
         self.match("C_KET")
 
+        return obj
+
     def parse_trlc_entry(self):
         if self.peek_kw("section"):
             self.parse_section_declaration()
         else:
-            self.parse_record_object_declaration()
+            self.cu.add_item(self.parse_record_object_declaration())
+
+    def parse_preamble(self, kind):
+        assert kind in ("rsl", "check", "trlc")
 
-    def parse_rsl_header(self):
+        # First, parse package indication, declaring the package if
+        # needed
         self.match_kw("package")
         self.match("IDENTIFIER")
 
-        self.pkg = ast.Package(self.ct.value,
-                               self.ct.location,
-                               self.stab)
-        self.stab.register(self.mh, self.pkg)
-        self.default_scope.push(self.pkg.symbols)
-
-        while self.peek_kw("import"):
-            self.match_kw("import")
-            self.match("IDENTIFIER")
-            self.raw_deps.append(self.ct)
-            self.imports.add(self.ct.value)
+        if kind == "rsl":
+            declare_package = True
+        elif kind == "check":
+            declare_package = False
+        else:
+            declare_package = not self.stab.contains(self.ct.value)
+
+        if declare_package:
+            pkg = ast.Package(name          = self.ct.value,
+                              location      = self.ct.location,
+                              builtin_stab  = self.stab,
+                              declared_late = kind == "trlc")
+            self.stab.register(self.mh, pkg)
+        else:
+            pkg = self.stab.lookup(self.mh, self.ct, ast.Package)
+            if pkg.declared_late and kind == "trlc":
+                self.mh.warning(
+                    self.ct.location,
+                    "duplicate late declaration of package %s,"
+                    " previous declaration in %s;"
+                    " consider adding an rsl file declaring the"
+                    " package" %
+                    (pkg.name,
+                     self.mh.cross_file_reference(pkg.location)))
+
+        self.cu.set_package(pkg)
+        self.default_scope.push(self.cu.package.symbols)
+
+        # Second, parse import list (but don't resolve names yet)
+        if kind != "check":
+            while self.peek_kw("import"):
+                self.match_kw("import")
+                self.match("IDENTIFIER")
+                self.cu.add_import(self.mh, self.ct)
 
     def parse_rsl_file(self):
-        assert self.pkg is not None
+        assert self.cu.package is not None
 
         while not self.peek_eof():
             if self.peek_kw("checks"):
-                self.parse_check_block()
+                self.cu.add_item(self.parse_check_block())
             else:
-                self.parse_type_declaration()
+                self.cu.add_item(self.parse_type_declaration())
 
         self.match_eof()
 
     def parse_check_file(self):
-        self.match_kw("package")
-        self.match("IDENTIFIER")
-
-        self.pkg = self.stab.lookup(self.mh, self.ct, ast.Package)
-        self.default_scope.push(self.pkg.symbols)
+        self.parse_preamble("check")
+        self.cu.resolve_imports(self.mh, self.stab)
 
         while not self.peek_eof():
-            self.parse_check_block()
+            self.cu.add_item(self.parse_check_block())
 
         self.match_eof()
 
     def parse_trlc_file(self):
-        self.match_kw("package")
-        self.match("IDENTIFIER")
-
-        if self.stab.contains(self.ct.value):
-            self.pkg = self.stab.lookup(self.mh, self.ct, ast.Package)
-        else:
-            self.pkg = ast.Package(self.ct.value,
-                                   self.ct.location,
-                                   self.stab)
-            self.pkg.declared_late = True
-            self.stab.register(self.mh, self.pkg)
-        self.default_scope.push(self.pkg.symbols)
-
-        while self.peek_kw("import"):
-            self.match_kw("import")
-            self.match("IDENTIFIER")
-            pkg = self.stab.lookup(self.mh, self.ct, ast.Package)
-            if pkg.declared_late:
-                self.mh.error(self.ct.location,
-                              "package must be declared in rsl file to be"
-                              " importable")
-            self.imports.add(pkg.name)
+        assert self.cu.package is not None
+        self.cu.resolve_imports(self.mh, self.stab)
 
         while self.peek_kw("section") or self.peek("IDENTIFIER"):
             self.parse_trlc_entry()
 
         self.match_eof()
```

### Comparing `trlc-1.1.4/trlc/trlc.py` & `trlc-1.1.5/trlc/trlc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 #
 # TRLC - Treat Requirements Like Code
-# Copyright (C) 2022 Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
+# Copyright (C) 2022-2023 Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 #
 # This file is part of the TRLC Python Reference Implementation.
 #
 # TRLC is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -175,22 +175,22 @@
     def register_rsl_file(self, file_name):
         assert os.path.isfile(file_name)
         assert file_name not in self.rsl_files
 
         self.update_common_root(file_name)
 
         self.rsl_files[file_name] = self.create_parser(file_name)
-        self.rsl_files[file_name].parse_rsl_header()
+        self.rsl_files[file_name].parse_preamble("rsl")
 
         self.register_package(
-            package_name = self.rsl_files[file_name].pkg.name,
+            package_name = self.rsl_files[file_name].cu.package.name,
             file_name    = file_name)
-        for import_name in self.rsl_files[file_name].raw_deps:
+        for import_name in self.rsl_files[file_name].cu.raw_imports:
             self.register_dependency(
-                package_name = self.rsl_files[file_name].pkg.name,
+                package_name = self.rsl_files[file_name].cu.package.name,
                 import_name  = import_name.value)
 
     def register_check_file(self, file_name):
         assert os.path.isfile(file_name)
         assert file_name not in self.check_files
 
         self.update_common_root(file_name)
@@ -202,18 +202,15 @@
 
         self.update_common_root(file_name)
         self.trlc_files[file_name] = self.create_parser(file_name)
 
     def parse_rsl_files(self):
         # First, check that each package import is known
         for parser in self.rsl_files.values():
-            for t_import in parser.raw_deps:
-                parser.deps.append(parser.stab.lookup(self.mh,
-                                                      t_import,
-                                                      ast.Package))
+            parser.cu.resolve_imports(self.mh, self.stab)
 
         # Second, parse packages that have no unparsed
         # dependencies. Keep doing it until we parse everything or
         # until we have reached a fix point (in which case we have a
         # cycle in our dependencies).
         processed_packages = set()
         while self.packages:
@@ -252,19 +249,32 @@
                 self.check_files[name].parse_check_file()
             except TRLC_Error:
                 ok = False
         return ok
 
     def parse_trlc_files(self):
         ok = True
+
+        # First, pre-parse the file_preamble of all files to discover
+        # all late packages
+        for name in sorted(self.trlc_files):
+            try:
+                self.trlc_files[name].parse_preamble("trlc")
+            except TRLC_Error:
+                ok = False
+        if not ok:
+            return False
+
+        # Then actually parse
         for name in sorted(self.trlc_files):
             try:
                 self.trlc_files[name].parse_trlc_file()
             except TRLC_Error:
                 ok = False
+
         return ok
 
     def resolve_record_references(self):
         ok = True
         for package in self.stab.values(ast.Package):
             for obj in package.symbols.values(ast.Record_Object):
                 try:
@@ -444,22 +454,22 @@
             summary += " no issues"
 
         print(summary)
 
         if options.show_file_list and ok:
             for filename in sorted(sm.rsl_files):
                 print("> Model %s (Package %s)" %
-                      (filename, sm.rsl_files[filename].pkg.name))
+                      (filename, sm.rsl_files[filename].cu.package.name))
             for filename in sorted(sm.check_files):
                 print("> Checks %s (Package %s)" %
-                      (filename, sm.check_files[filename].pkg.name))
+                      (filename, sm.check_files[filename].cu.package.name))
             if not options.lint:
                 for filename in sorted(sm.trlc_files):
                     print("> Requirements %s (Package %s)" %
-                          (filename, sm.trlc_files[filename].pkg.name))
+                          (filename, sm.trlc_files[filename].cu.package.name))
 
     if ok:
         return 0
     else:
         return 1
```

### Comparing `trlc-1.1.4/trlc/version.py` & `trlc-1.1.5/trlc/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
 # or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public
 # License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with TRLC. If not, see <https://www.gnu.org/licenses/>.
 
-VERSION_TUPLE = (1, 1, 4)
+VERSION_TUPLE = (1, 1, 5)
 VERSION_SUFFIX = ""
 
 TRLC_VERSION = ("%u.%u.%u" % VERSION_TUPLE) + \
     ("-%s" % VERSION_SUFFIX if VERSION_SUFFIX else "")
 
 FULL_NAME = "TRLC %s" % TRLC_VERSION
```

### Comparing `trlc-1.1.4/trlc.egg-info/PKG-INFO` & `trlc-1.1.5/trlc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trlc
-Version: 1.1.4
+Version: 1.1.5
 Summary: Treat Requirements Like Code
 Home-page: https://github.com/bmw-software-engineering/trlc
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/trlc/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/trlc/
@@ -23,15 +23,15 @@
 TRLC is a domain-specific language developed at BMW for writing (and
 linking) requirements with meta-data.
 
 The repository contains:
 
 * The [language reference
   manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
-  for TRLC.
+  for TRLC. [Previous versions](https://github.com/bmw-software-engineering/trlc/blob/main/docs/LRM.md) are also available.
 
 * A pure Python reference implementation of TRLC.
 
 The implementation is not very fast, but designed to be pedantically
 correct in following the language definition.  Eventually it will also
 contain a powerful linter to find issues with types and check
 rules.
@@ -46,22 +46,29 @@
 * The API can be used to write other tools based on TRLC (for example
   a tool to render the requirements in HTML, a tool to diff
   requirements or perform an impact analysis, or a tool to perform
   software traceability, etc.)
 
 ## Documentation
 
+### For users
+
 * [Tutorial](https://github.com/bmw-software-engineering/trlc/blob/main/TUTORIAL.md) (read this as a first introduction)
 * [Release Notes](https://github.com/bmw-software-engineering/trlc/blob/main/CHANGELOG.md) (read this to find out whats new)
-* [Python API Documentation](https://bmw-software-engineering.github.io/trlc/)
-  (user guide for using the API)
 * [Language Reference Manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
   (for language lawyers)
 * [License](https://github.com/bmw-software-engineering/trlc/blob/main/LICENSE)
 
+### For developers
+
+* [Python API Documentation](https://bmw-software-engineering.github.io/trlc/)
+  (API reference)
+* [AST Hierarchy](https://bmw-software-engineering.github.io/trlc/ast_hierarchy.svg)
+  (overview over all classes in the AST)
+
 ## Dependencies
 
 ### Run-time
 * Python3 >= 3.7
 
 ### Development tools
 * GNU Make
```

