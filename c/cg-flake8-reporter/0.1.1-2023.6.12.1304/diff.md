# Comparing `tmp/cg_flake8_reporter-0.1.1.tar.gz` & `tmp/cg_flake8_reporter-2023.6.12.1304.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg_flake8_reporter-0.1.1.tar", max compression
+gzip compressed data, was "cg_flake8_reporter-2023.6.12.1304.tar", max compression
```

## Comparing `cg_flake8_reporter-0.1.1.tar` & `cg_flake8_reporter-2023.6.12.1304.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2362 2023-05-31 13:11:46.818733 cg_flake8_reporter-0.1.1/README.md
--rw-r--r--   0        0        0      159 2023-05-31 13:19:44.972710 cg_flake8_reporter-0.1.1/cg_flake8_reporter/__init__.py
--rw-r--r--   0        0        0     6466 2023-05-31 13:11:46.818939 cg_flake8_reporter-0.1.1/cg_flake8_reporter/plugin.py
--rw-r--r--   0        0        0     1860 2023-05-31 13:20:06.815755 cg_flake8_reporter-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 cg_flake8_reporter-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2398 2023-06-12 13:04:21.013890 cg_flake8_reporter-2023.6.12.1304/README.md
+-rw-r--r--   0        0        0      136 2023-06-12 13:04:21.013890 cg_flake8_reporter-2023.6.12.1304/cg_flake8_reporter/__init__.py
+-rw-r--r--   0        0        0     5958 2023-06-12 13:04:21.013890 cg_flake8_reporter-2023.6.12.1304/cg_flake8_reporter/plugin.py
+-rw-r--r--   0        0        0     1729 2023-06-12 13:04:47.806075 cg_flake8_reporter-2023.6.12.1304/pyproject.toml
+-rw-r--r--   0        0        0     2783 1970-01-01 00:00:00.000000 cg_flake8_reporter-2023.6.12.1304/PKG-INFO
```

### Comparing `cg_flake8_reporter-0.1.1/README.md` & `cg_flake8_reporter-2023.6.12.1304/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# cg-pytest-reporter
+# cg-flake8-reporter
 
 A Flae8 reporter plugin for CodeGrade AutoTest v2.
 
 This plugin writes messages to CodeGrade AutoTest v2's structured output channel.
 For each violation Flake8 reports, a `comments` message is written as described
 in CodeGrade's documentation. When Flake8 finishes its analysis, a final message
 is written with the amount of points that were achieved in the code quality run.
@@ -10,19 +10,19 @@
 ## Configuration
 
 In order to use the custom reporter, make sure you have installed both Flake8
 and this package:
 
 ```bash
 python3 -m pip install flake8==6.0.0
-python3 -m pip install cg_flake8_reporter
+python3 -m pip install cg-flake8-reporter
 ```
 
-This reporter is registered with Flake8 as `jsonfd`, to use it run flake with
-the option `--format=jsonfd`.
+This reporter is registered with Flake8 as `cg-flake8-reporter`, to use it run
+flake with the option `--format=cg-flake8-reporter`.
 
 The custom reporter adds a few new options to Flake8: `cg-points-deducted`,
 `cg-flake8-fd` and `cg-base-path`.
 
 ### cg-points-deducted
 
 The `cg-points-deducted` option makes it possible to configure the amount of
@@ -58,12 +58,12 @@
 
 ## Usage
 
 To run Flake8 with the custom reporter:
 
 ```bash
 python3 -m flake8 \
-    --format=jsonfd \
+    --format=cg-flake8-reporter \
     --cg-points-deducted='info:1,warning:3,error:5' \
     --cg-flake8-fd=1 \
     ./
 ```
```

### Comparing `cg_flake8_reporter-0.1.1/cg_flake8_reporter/plugin.py` & `cg_flake8_reporter-2023.6.12.1304/cg_flake8_reporter/plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,30 +33,26 @@
     Also calculates a score based on severity of errors/warnings.
     """
     def __init__(self, options: argparse.Namespace) -> None:
         """
         Initialize buffer for comments, score, and points deducted for each severity level.
         """
         super().__init__(options)
-        self._buffer: t.Mapping[str,
-                                t.Any] = {"tag": "comments", "comments": {}}
+        self._buffer: t.MutableMapping[str, t.Any] = {
+            "tag": "comments", "comments": {}
+        }
         self._score = Fraction(1, 1)
         self._buffer_size = 0
         self._points_deducted = {
             'info': Fraction(0, 1),
             'warning': Fraction(0, 1),
             'error': Fraction(0, 1),
         }
         # pylint: disable=consider-using-with
-        try:
-            self._file = open(options.cg_flake8_fd, 'wb', buffering=0)
-        except OSError as e:
-            raise IOError(
-                f'Could not open file descriptor {options.cg_flake8_fd}'
-            ) from e
+        self._file = open(options.cg_flake8_fd, 'wb', buffering=0)
 
         self._base_path = Path(options.cg_base_path)
 
         if options.cg_points_deducted:
             self._points_deducted = {
                 severity: Fraction(int(points), 100)
                 for severity, points in (
@@ -100,15 +96,15 @@
             default='/',
             help="""
 The base path of the reported files. Files that are not children of this path
 will not be reported.
             """
         )
 
-    def format(self, error: flake8.violation.Violation):
+    def format(self, error: flake8.violation.Violation) -> None:
         """
         Format the error/warning and add to buffer.
         Also update the score based on error severity.
         """
         try:
             abs_path = os.path.abspath(error.filename)
             relative_path = Path(abs_path).relative_to(self._base_path)
@@ -116,15 +112,15 @@
             return
 
         code = error.code
         if code.startswith('E') or code.startswith('F'):
             severity = 'error'
         elif code.startswith('W'):
             severity = 'warning'
-        elif code.startswith('C') or code.startswith('N8'):  # pragma: no cover
+        elif code.startswith('C') or code.startswith('N8'):
             severity = 'info'
 
         if severity in self._points_deducted:
             self._score = max(
                 self._score - self._points_deducted[severity], Fraction(0)
             )
 
@@ -132,60 +128,48 @@
             "code": error.code,
             "severity": severity,
             "loc": {
                 "start": {
                     "line": error.line_number,
                     "column": error.column_number,
                 },
-                "end": {
-                    "line": error.line_number,
-                    "column": error.column_number,
-                },
+                "end": {"line": error.line_number, },
             },
             "msg": error.text,
         }
 
+        added_size = len(json_dumps(err_item))
+
+        if self._buffer_size + added_size >= MESSAGE_SIZE_LIMIT:
+            self.flush()
+
         file_comments = self._buffer["comments"].get(str(relative_path))
         if file_comments is None:
             file_comments = {
                 "filename": str(relative_path),
                 "origin": "Flake8",
                 "items": [],
             }
-            self._buffer["comments"][str(relative_path)] = file_comments
+            added_size += len(json_dumps(file_comments))
 
         file_comments["items"].append(err_item)
-        self._buffer_size += len(json_dumps(err_item))
-
-        if self._buffer_size >= MESSAGE_SIZE_LIMIT:
-            self.flush()
+        self._buffer["comments"][str(relative_path)] = file_comments
+        self._buffer_size += added_size
 
-    def flush(self):
+    def flush(self) -> None:
         """
         Write the comments to file descriptor and clear the buffer.
         """
         self._buffer["comments"] = list(self._buffer["comments"].values())
         data = json_dumps(self._buffer) + '\n'
 
-        try:
-            self._file.write(data.encode('utf8'))
-        except OSError as e:
-            raise IOError(
-                f'Could not write comments to file descriptor {self._file.fileno()}'
-            ) from e
-        finally:
-            self._buffer = {"tag": "comments", "comments": {}}
-            self._buffer_size = 0
+        self._file.write(data.encode('utf8'))
+        self._buffer = {"tag": "comments", "comments": {}}
+        self._buffer_size = len(json_dumps(self._buffer))
 
-    def stop(self):
+    def stop(self) -> None:
         """
         At the end, flush the remaining comments and write the score.
         """
         self.flush()
         data = json_dumps({"tag": "points", "points": str(self._score)})
-
-        try:
-            self._file.write(data.encode('utf8'))
-        except OSError as e:
-            raise IOError(
-                f'Could not write score to file descriptor {self._file.fileno()}'
-            ) from e
+        self._file.write(data.encode('utf8'))
```

### Comparing `cg_flake8_reporter-0.1.1/pyproject.toml` & `cg_flake8_reporter-2023.6.12.1304/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 [tool.poetry]
 name = "cg-flake8-reporter"
-version = "0.1.1"
+version = "2023.06.12.1304"
 description = ""
 authors = ["CodeGrade <info@codegrade.com>"]
 readme = "README.md"
 packages = [{ include = "cg_flake8_reporter" }]
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
+python = "^3.10"
 "flake8" = ">=6.0.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.2.0"
 pylint = "^2.17.4"
 yapf = "^0.33.0"
 isort = "^5.12.0"
 pytest = ">=7.0.0"
 pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.pytest.ini_options]
-# This should be the default value, but Pytest did not find the test classes
-# without this rule...
-python_classes = "Test*"
-
 [tool.yapf]
 based_on_style = "pep8"
 coalesce_brackets = true
 dedent_closing_brackets = true
 indent_dictionary_value = true
 spaces_around_power_operator = true
 space_between_ending_comma_and_closing_bracket = true
@@ -66,8 +61,8 @@
 ignore-imports = true
 bad-functions = "apply,reduce,print"
 max-public-methods = 25
 const-rgx = "_?(([A-Z_][A-Z0-9_]*)|(__.*__))$"
 class-const-naming-style = "any"
 
 [tool.poetry.plugins."flake8.report"]
-jsonfd = "cg_flake8_reporter:CustomFormatter"
+cg-flake8-reporter = "cg_flake8_reporter:CustomFormatter"
```

### Comparing `cg_flake8_reporter-0.1.1/PKG-INFO` & `cg_flake8_reporter-2023.6.12.1304/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: cg-flake8-reporter
-Version: 0.1.1
+Version: 2023.6.12.1304
 Summary: 
 Author: CodeGrade
 Author-email: info@codegrade.com
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: flake8 (>=6.0.0)
 Description-Content-Type: text/markdown
 
-# cg-pytest-reporter
+# cg-flake8-reporter
 
 A Flae8 reporter plugin for CodeGrade AutoTest v2.
 
 This plugin writes messages to CodeGrade AutoTest v2's structured output channel.
 For each violation Flake8 reports, a `comments` message is written as described
 in CodeGrade's documentation. When Flake8 finishes its analysis, a final message
 is written with the amount of points that were achieved in the code quality run.
@@ -24,19 +23,19 @@
 ## Configuration
 
 In order to use the custom reporter, make sure you have installed both Flake8
 and this package:
 
 ```bash
 python3 -m pip install flake8==6.0.0
-python3 -m pip install cg_flake8_reporter
+python3 -m pip install cg-flake8-reporter
 ```
 
-This reporter is registered with Flake8 as `jsonfd`, to use it run flake with
-the option `--format=jsonfd`.
+This reporter is registered with Flake8 as `cg-flake8-reporter`, to use it run
+flake with the option `--format=cg-flake8-reporter`.
 
 The custom reporter adds a few new options to Flake8: `cg-points-deducted`,
 `cg-flake8-fd` and `cg-base-path`.
 
 ### cg-points-deducted
 
 The `cg-points-deducted` option makes it possible to configure the amount of
@@ -72,13 +71,13 @@
 
 ## Usage
 
 To run Flake8 with the custom reporter:
 
 ```bash
 python3 -m flake8 \
-    --format=jsonfd \
+    --format=cg-flake8-reporter \
     --cg-points-deducted='info:1,warning:3,error:5' \
     --cg-flake8-fd=1 \
     ./
 ```
```

