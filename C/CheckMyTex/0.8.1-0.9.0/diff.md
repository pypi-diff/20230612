# Comparing `tmp/CheckMyTex-0.8.1.tar.gz` & `tmp/CheckMyTex-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CheckMyTex-0.8.1.tar", last modified: Sat Aug 13 17:15:59 2022, max compression
+gzip compressed data, was "CheckMyTex-0.9.0.tar", last modified: Tue Aug 16 15:53:03 2022, max compression
```

## Comparing `CheckMyTex-0.8.1.tar` & `CheckMyTex-0.9.0.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:15:59.303561 CheckMyTex-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:15:59.303561 CheckMyTex-0.8.1/CheckMyTex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10334 2022-08-13 17:15:59.000000 CheckMyTex-0.8.1/CheckMyTex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-08-13 17:15:59.000000 CheckMyTex-0.8.1/CheckMyTex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-13 17:15:59.000000 CheckMyTex-0.8.1/CheckMyTex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-08-13 17:15:59.000000 CheckMyTex-0.8.1/CheckMyTex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-13 17:15:59.000000 CheckMyTex-0.8.1/CheckMyTex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-13 17:15:59.000000 CheckMyTex-0.8.1/CheckMyTex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-13 17:15:59.000000 CheckMyTex-0.8.1/CheckMyTex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10334 2022-08-13 17:15:59.303561 CheckMyTex-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9811 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:15:59.303561 CheckMyTex-0.8.1/checkmytex/
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/analyze.py
--rw-r--r--   0 runner    (1001) docker     (121)     3120 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/analyzed_document.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:15:59.303561 CheckMyTex-0.8.1/checkmytex/cli/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/cli/arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2734 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/cli/file_printer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/cli/highlighted_output.py
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/cli/overview.py
--rw-r--r--   0 runner    (1001) docker     (121)     5062 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/cli/problem_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     3360 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/document_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:15:59.303561 CheckMyTex-0.8.1/checkmytex/filtering/
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/filtering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3794 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/filtering/authors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3205 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/filtering/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2933 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/filtering/math_mode.py
--rw-r--r--   0 runner    (1001) docker     (121)     3451 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/filtering/whitelist.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:15:59.303561 CheckMyTex-0.8.1/checkmytex/finding/
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/finding/abstract_checker.py
--rw-r--r--   0 runner    (1001) docker     (121)     2832 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/finding/chktex.py
--rw-r--r--   0 runner    (1001) docker     (121)     1983 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/finding/cleveref.py
--rw-r--r--   0 runner    (1001) docker     (121)     4199 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/finding/languagetool.py
--rw-r--r--   0 runner    (1001) docker     (121)     1808 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/finding/nphard.py
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/finding/problem.py
--rw-r--r--   0 runner    (1001) docker     (121)     3975 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/finding/proselint.py
--rw-r--r--   0 runner    (1001) docker     (121)     2184 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/finding/siunitx.py
--rw-r--r--   0 runner    (1001) docker     (121)     5156 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/finding/spellcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:15:59.303561 CheckMyTex-0.8.1/checkmytex/latex_document/
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/latex_document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/latex_document/indexed_string.py
--rw-r--r--   0 runner    (1001) docker     (121)     7849 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/latex_document/latex_document.py
--rw-r--r--   0 runner    (1001) docker     (121)     2013 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/latex_document/origin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3063 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/latex_document/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:15:59.303561 CheckMyTex-0.8.1/checkmytex/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/utils/choice.py
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/checkmytex/utils/editor.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-13 17:15:59.303561 CheckMyTex-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-08-13 17:15:56.000000 CheckMyTex-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 15:53:03.431392 CheckMyTex-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 15:53:03.427391 CheckMyTex-0.9.0/CheckMyTex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10606 2022-08-16 15:53:03.000000 CheckMyTex-0.9.0/CheckMyTex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1438 2022-08-16 15:53:03.000000 CheckMyTex-0.9.0/CheckMyTex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 15:53:03.000000 CheckMyTex-0.9.0/CheckMyTex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-08-16 15:53:03.000000 CheckMyTex-0.9.0/CheckMyTex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 15:53:03.000000 CheckMyTex-0.9.0/CheckMyTex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-16 15:53:03.000000 CheckMyTex-0.9.0/CheckMyTex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-16 15:53:03.000000 CheckMyTex-0.9.0/CheckMyTex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    10606 2022-08-16 15:53:03.431392 CheckMyTex-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10083 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 15:53:03.427391 CheckMyTex-0.9.0/checkmytex/
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3297 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/analyzed_document.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 15:53:03.427391 CheckMyTex-0.9.0/checkmytex/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      969 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/cli/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3003 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/cli/file_printer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/cli/highlighted_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)      812 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/cli/overview.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4904 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/cli/problem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3326 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/document_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 15:53:03.427391 CheckMyTex-0.9.0/checkmytex/filtering/
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/filtering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3835 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/filtering/authors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3323 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/filtering/filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2949 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/filtering/math_mode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3451 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/filtering/whitelist.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 15:53:03.427391 CheckMyTex-0.9.0/checkmytex/finding/
+-rw-r--r--   0 runner    (1001) docker     (121)      398 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/finding/abstract_checker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2843 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/finding/chktex.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/finding/cleveref.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4264 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/finding/languagetool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1849 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/finding/nphard.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/finding/problem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3986 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/finding/proselint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2195 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/finding/siunitx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5178 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/finding/spellcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 15:53:03.431392 CheckMyTex-0.9.0/checkmytex/latex_document/
+-rw-r--r--   0 runner    (1001) docker     (121)      659 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/latex_document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/latex_document/detex.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4724 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/latex_document/indexed_string.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5237 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/latex_document/latex_document.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2870 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/latex_document/origin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4354 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/latex_document/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2955 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/latex_document/source.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 15:53:03.431392 CheckMyTex-0.9.0/checkmytex/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/utils/choice.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/checkmytex/utils/editor.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-16 15:53:03.431392 CheckMyTex-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-08-16 15:52:56.000000 CheckMyTex-0.9.0/setup.py
```

### Comparing `CheckMyTex-0.8.1/CheckMyTex.egg-info/PKG-INFO` & `CheckMyTex-0.9.0/CheckMyTex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheckMyTex
-Version: 0.8.1
+Version: 0.9.0
 Summary: A simple tool for checking complex LaTeX documents, e.g., dissertations.
 Home-page: https://github.com/d-krupke/checkmytex
 Author: Dominik Krupke
 Author-email: krupke@ibr.cs.tu-bs.de
 License: MIT
 Keywords: LaTeX
 Platform: UNKNOWN
@@ -123,14 +123,20 @@
 
 This tool will have problems with some areas of you document. You can exclude these areas by adding lines with
 `%%PAUSE-CHECKING` and `%%CONTINUE-CHECKING`. This may be easier than whitelisting all the problems.
 
 The time to check a 300-page dissertation is around a few seconds. A better spell checking would be available but
 drastically increase the runtime.
 
+If you want to process the output with another tool, you can export the result as json
+using:
+```bash
+checkmytex --json analysis.json main.tex
+```
+
 ## Extending CheckMyTex
 
 ### Finding problems in the LaTeX document
 
 CheckMyTex already comes with a set of very useful tools and rules to find potential problems.
 
 ```python
@@ -151,19 +157,20 @@
 import typing
 
 
 class NoOld(Checker):
     def check(self, document: LatexDocument) -> typing.Iterable[Problem]:
         source = document.get_source()
         for match in re.finditer(r"\\old\{", source):
-            origin = document.get_origin_of_source(match.start(), match.end())
+            origin = document.get_simplified_origin_of_source(match.start(), match.end())
             context = document.get_source_context(origin)
             long_id = f"NO_OLD:{context}"
             yield Problem(origin, "Please do not use \\old{! (it confuses highlighting)",
-                          context=context, long_id=long_id, tool="CustomNoOld", rule="NO_OLD")
+                          context=context, long_id=long_id, tool="CustomNoOld",
+                          rule="NO_OLD")
 ```
 
 This is all!
 Now you can add this rule to the `DocumentAnalyzer` with `add_checker`.
 You may want to copy the main.py and build yourself a custom version that directly includes this rule.
 
 ### Filtering patterns of false positives
@@ -202,15 +209,16 @@
         expr = r"\\begin\{align\}.*?\\end\{align\}"
         source = document.get_source()
         for match in re.finditer(expr, source, re.MULTILINE | re.DOTALL):
             self._ranges.append((match.start(), match.end()))
 
     def filter(self, problems: typing.Iterable[Problem]) -> typing.Iterable[Problem]:
         for p in problems:
-            if any(r[0] <= p.origin.begin.spos < r[1] for r in self._ranges):
+            s_span = p.origin.get_source_span()
+            if any(r[0] <= s_span[0] < r[1] for r in self._ranges):
                 continue  # problem starts within a previous found range of an align-environment
             yield p
 ```
 
 We can add this filter similar to a checker to the `DocumentAnalyzer`.
 
 ## Other Languages
@@ -226,11 +234,12 @@
 
 - Reduce double-whitespace matches. They do not matter in LaTeX. Maybe clean the detexed file instead of just disabling
   the corresponding rules?
 - More configuration options. Currently, the best option is to simply build your own [main.py](./checkmytex/__main__.py)
 
 ## Changes
 
+- 0.9.0: Fundamental refactoring and JSON-ouput.
 - 0.8.1: Fixing problem with text manipulated by commands. All found errors now should only span a single line. Solution is ugly and should be improved. For now, it is working.
   .
```

### Comparing `CheckMyTex-0.8.1/CheckMyTex.egg-info/SOURCES.txt` & `CheckMyTex-0.9.0/CheckMyTex.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 checkmytex/finding/languagetool.py
 checkmytex/finding/nphard.py
 checkmytex/finding/problem.py
 checkmytex/finding/proselint.py
 checkmytex/finding/siunitx.py
 checkmytex/finding/spellcheck.py
 checkmytex/latex_document/__init__.py
+checkmytex/latex_document/detex.py
 checkmytex/latex_document/indexed_string.py
 checkmytex/latex_document/latex_document.py
 checkmytex/latex_document/origin.py
 checkmytex/latex_document/parser.py
+checkmytex/latex_document/source.py
 checkmytex/utils/__init__.py
 checkmytex/utils/choice.py
 checkmytex/utils/editor.py
```

### Comparing `CheckMyTex-0.8.1/LICENSE` & `CheckMyTex-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CheckMyTex-0.8.1/PKG-INFO` & `CheckMyTex-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheckMyTex
-Version: 0.8.1
+Version: 0.9.0
 Summary: A simple tool for checking complex LaTeX documents, e.g., dissertations.
 Home-page: https://github.com/d-krupke/checkmytex
 Author: Dominik Krupke
 Author-email: krupke@ibr.cs.tu-bs.de
 License: MIT
 Keywords: LaTeX
 Platform: UNKNOWN
@@ -123,14 +123,20 @@
 
 This tool will have problems with some areas of you document. You can exclude these areas by adding lines with
 `%%PAUSE-CHECKING` and `%%CONTINUE-CHECKING`. This may be easier than whitelisting all the problems.
 
 The time to check a 300-page dissertation is around a few seconds. A better spell checking would be available but
 drastically increase the runtime.
 
+If you want to process the output with another tool, you can export the result as json
+using:
+```bash
+checkmytex --json analysis.json main.tex
+```
+
 ## Extending CheckMyTex
 
 ### Finding problems in the LaTeX document
 
 CheckMyTex already comes with a set of very useful tools and rules to find potential problems.
 
 ```python
@@ -151,19 +157,20 @@
 import typing
 
 
 class NoOld(Checker):
     def check(self, document: LatexDocument) -> typing.Iterable[Problem]:
         source = document.get_source()
         for match in re.finditer(r"\\old\{", source):
-            origin = document.get_origin_of_source(match.start(), match.end())
+            origin = document.get_simplified_origin_of_source(match.start(), match.end())
             context = document.get_source_context(origin)
             long_id = f"NO_OLD:{context}"
             yield Problem(origin, "Please do not use \\old{! (it confuses highlighting)",
-                          context=context, long_id=long_id, tool="CustomNoOld", rule="NO_OLD")
+                          context=context, long_id=long_id, tool="CustomNoOld",
+                          rule="NO_OLD")
 ```
 
 This is all!
 Now you can add this rule to the `DocumentAnalyzer` with `add_checker`.
 You may want to copy the main.py and build yourself a custom version that directly includes this rule.
 
 ### Filtering patterns of false positives
@@ -202,15 +209,16 @@
         expr = r"\\begin\{align\}.*?\\end\{align\}"
         source = document.get_source()
         for match in re.finditer(expr, source, re.MULTILINE | re.DOTALL):
             self._ranges.append((match.start(), match.end()))
 
     def filter(self, problems: typing.Iterable[Problem]) -> typing.Iterable[Problem]:
         for p in problems:
-            if any(r[0] <= p.origin.begin.spos < r[1] for r in self._ranges):
+            s_span = p.origin.get_source_span()
+            if any(r[0] <= s_span[0] < r[1] for r in self._ranges):
                 continue  # problem starts within a previous found range of an align-environment
             yield p
 ```
 
 We can add this filter similar to a checker to the `DocumentAnalyzer`.
 
 ## Other Languages
@@ -226,11 +234,12 @@
 
 - Reduce double-whitespace matches. They do not matter in LaTeX. Maybe clean the detexed file instead of just disabling
   the corresponding rules?
 - More configuration options. Currently, the best option is to simply build your own [main.py](./checkmytex/__main__.py)
 
 ## Changes
 
+- 0.9.0: Fundamental refactoring and JSON-ouput.
 - 0.8.1: Fixing problem with text manipulated by commands. All found errors now should only span a single line. Solution is ugly and should be improved. For now, it is working.
   .
```

### Comparing `CheckMyTex-0.8.1/README.md` & `CheckMyTex-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -106,14 +106,20 @@
 
 This tool will have problems with some areas of you document. You can exclude these areas by adding lines with
 `%%PAUSE-CHECKING` and `%%CONTINUE-CHECKING`. This may be easier than whitelisting all the problems.
 
 The time to check a 300-page dissertation is around a few seconds. A better spell checking would be available but
 drastically increase the runtime.
 
+If you want to process the output with another tool, you can export the result as json
+using:
+```bash
+checkmytex --json analysis.json main.tex
+```
+
 ## Extending CheckMyTex
 
 ### Finding problems in the LaTeX document
 
 CheckMyTex already comes with a set of very useful tools and rules to find potential problems.
 
 ```python
@@ -134,19 +140,20 @@
 import typing
 
 
 class NoOld(Checker):
     def check(self, document: LatexDocument) -> typing.Iterable[Problem]:
         source = document.get_source()
         for match in re.finditer(r"\\old\{", source):
-            origin = document.get_origin_of_source(match.start(), match.end())
+            origin = document.get_simplified_origin_of_source(match.start(), match.end())
             context = document.get_source_context(origin)
             long_id = f"NO_OLD:{context}"
             yield Problem(origin, "Please do not use \\old{! (it confuses highlighting)",
-                          context=context, long_id=long_id, tool="CustomNoOld", rule="NO_OLD")
+                          context=context, long_id=long_id, tool="CustomNoOld",
+                          rule="NO_OLD")
 ```
 
 This is all!
 Now you can add this rule to the `DocumentAnalyzer` with `add_checker`.
 You may want to copy the main.py and build yourself a custom version that directly includes this rule.
 
 ### Filtering patterns of false positives
@@ -185,15 +192,16 @@
         expr = r"\\begin\{align\}.*?\\end\{align\}"
         source = document.get_source()
         for match in re.finditer(expr, source, re.MULTILINE | re.DOTALL):
             self._ranges.append((match.start(), match.end()))
 
     def filter(self, problems: typing.Iterable[Problem]) -> typing.Iterable[Problem]:
         for p in problems:
-            if any(r[0] <= p.origin.begin.spos < r[1] for r in self._ranges):
+            s_span = p.origin.get_source_span()
+            if any(r[0] <= s_span[0] < r[1] for r in self._ranges):
                 continue  # problem starts within a previous found range of an align-environment
             yield p
 ```
 
 We can add this filter similar to a checker to the `DocumentAnalyzer`.
 
 ## Other Languages
@@ -209,9 +217,10 @@
 
 - Reduce double-whitespace matches. They do not matter in LaTeX. Maybe clean the detexed file instead of just disabling
   the corresponding rules?
 - More configuration options. Currently, the best option is to simply build your own [main.py](./checkmytex/__main__.py)
 
 ## Changes
 
+- 0.9.0: Fundamental refactoring and JSON-ouput.
 - 0.8.1: Fixing problem with text manipulated by commands. All found errors now should only span a single line. Solution is ugly and should be improved. For now, it is working.
   .
```

### Comparing `CheckMyTex-0.8.1/checkmytex/__main__.py` & `CheckMyTex-0.9.0/checkmytex/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 A main file to execute CheckMyTex with CLI.
 """
+import json
+
 from checkmytex.cli import InteractiveCli, log, parse_arguments
 from checkmytex.document_analyzer import DocumentAnalyzer
 from checkmytex.filtering import (
     IgnoreIncludegraphics,
     IgnoreLikelyAuthorNames,
     IgnoreRefs,
     IgnoreRepeatedWords,
@@ -21,34 +23,39 @@
     """
     A main function, such that it can also be called with different entry
     points
     :return: None
     """
     args = parse_arguments(log)
     whitelist = Whitelist(args.whitelist)
-    log("Parsing LaTeX project...")
+    log_ = log
+    log_("Parsing LaTeX project...")
     try:
         parser = LatexParser()
         latex_document = parser.parse(args.path[0])
-        engine = DocumentAnalyzer(log=log)
+        engine = DocumentAnalyzer(log=log_)
+        engine.log = log_
         engine.setup_default()
         # Add filter
         engine.add_filter(whitelist)
         engine.add_filter(IgnoreIncludegraphics())
         engine.add_filter(IgnoreRefs())
         engine.add_filter(IgnoreRepeatedWords(["problem", "problems"]))
         engine.add_filter(IgnoreLikelyAuthorNames())
         engine.add_filter(IgnoreWordsFromBibliography())
         engine.add_filter(IgnoreSpellingWithMath())
         engine.add_filter(
             MathMode({"SPELLING": None, "languagetool": None, "Proselint": None})
         )
 
         analyzed_document = engine.analyze(latex_document)
-
+        if args.json:
+            with open(args.json, "w") as f:
+                json.dump(analyzed_document.serialize(), f)
+            return
         InteractiveCli(analyzed_document, whitelist, just_print=args.print)
     except KeyError as key_error:
         print("Error:", str(key_error))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `CheckMyTex-0.8.1/checkmytex/analyzed_document.py` & `CheckMyTex-0.9.0/checkmytex/analyzed_document.py`

 * *Files 15% similar despite different names*

```diff
@@ -65,29 +65,34 @@
     def get_problems(
         self, file: typing.Optional[str] = None, line: typing.Optional[int] = None
     ) -> typing.List[Problem]:
         """
         Returns problems. Can be for a specific file and even line.
         """
         if file:
-            problems = [p for p in self.problems if p.origin.file == file]
+            problems = [p for p in self.problems if p.origin.get_file() == file]
             if line:
-                problems = [
-                    p
-                    for p in problems
-                    if p.origin.begin.row <= line <= p.origin.end.row
-                ]
+                problems = [p for p in problems if p.origin.get_file_line() == line]
             return problems
         return self.problems
 
+    def get_orphaned_problems(self):
+        return [p for p in self.problems if not p.origin]
+
     def list_files(self) -> typing.Iterable[str]:
         """
         List all files of the document.
         """
         for file_path in self.document.files():
             yield file_path
 
     def get_file_content(self, file_name: str) -> str:
         """
         Returns the content of a specific file in the document.
         """
         return self.document.get_file_content(file_name)
+
+    def serialize(self):
+        return {
+            "document": self.document.serialize(),
+            "problems": [p.serialize() for p in self.problems]
+        }
```

### Comparing `CheckMyTex-0.8.1/checkmytex/cli/arguments.py` & `CheckMyTex-0.9.0/checkmytex/cli/arguments.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     :return: The parsed arguments.
     """
     parser = argparse.ArgumentParser(
         description="CheckMyTex: A simple tool for checking your LaTeX."
     )
 
     parser.add_argument("-w", help="Path to whitelist", type=str)
+    parser.add_argument("--json", type=str, help="Write result as json to file.")
     parser.add_argument("--print", action="store_true", help="Just print the output")
     parser.add_argument("path", nargs=1, help="Path to main.tex")
     args = parser.parse_args()
     if not args.path:
         parser.print_help()
         sys.exit(1)
     if args.w:
```

### Comparing `CheckMyTex-0.8.1/checkmytex/cli/cli.py` & `CheckMyTex-0.9.0/checkmytex/cli/cli.py`

 * *Files identical despite different names*

### Comparing `CheckMyTex-0.8.1/checkmytex/cli/file_printer.py` & `CheckMyTex-0.9.0/checkmytex/cli/file_printer.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,41 +23,51 @@
 
     def _enumerate_relevant_lines(self, lines, problems):
         for i, line_content in enumerate(lines):
             if self._shorten is None:
                 yield i, line_content
 
             def in_range(problem):
-                begin = problem.origin.begin.row - self._shorten
-                end = problem.origin.end.row + self._shorten
+                begin = problem.origin.begin.file.position.line - self._shorten
+                end = problem.origin.end.file.position.line + self._shorten
                 return begin <= i < end
 
             if any(in_range(p) for p in problems):
                 yield i, line_content
 
     def _print_line(self, file_name, line_number, line):
         problems = self._analyzed_document.get_problems(file_name, line_number)
 
         def span(p):
-            a = p.origin.begin.col if p.origin.begin.row == line_number else 0
-            b = p.origin.end.col if p.origin.end.row == line_number else len(line)
+            a = (
+                p.origin.begin.file.position.line_offset
+                if p.origin.begin.file.position.line == line_number
+                else 0
+            )
+            b = (
+                p.origin.end.file.position.line_offset
+                if p.origin.end.file.position.line == line_number
+                else len(line)
+            )
             return a, b
 
         highlighted_line = add_highlights(line, (span(p) for p in problems))
         print(
             f"{ColorCodes.BLACK_ON_WHITE}{line_number}:{ColorCodes.ENDC}",
             highlighted_line,
         )
 
     def _print_problem(self, p: Problem):
         print(f" >>> {ColorCodes.WARNING}{p.message}{ColorCodes.ENDC} ({p.tool})")
 
     def _handle_line_problems(self, f, i):
         line_problems = self._analyzed_document.get_problems(f, line=i)
-        line_problems = [p for p in line_problems if p.origin.end.row == i]
+        line_problems = [
+            p for p in line_problems if p.origin.end.file.position.line == i
+        ]
         for p in line_problems:
             self._print_problem(p)
             self._problem_handler(p)
 
     def print(self, file_path: str):
         source = self._analyzed_document.get_file_content(file_path)
         lines = source.split("\n")
```

### Comparing `CheckMyTex-0.8.1/checkmytex/cli/highlighted_output.py` & `CheckMyTex-0.9.0/checkmytex/cli/highlighted_output.py`

 * *Files identical despite different names*

### Comparing `CheckMyTex-0.8.1/checkmytex/cli/overview.py` & `CheckMyTex-0.9.0/checkmytex/cli/overview.py`

 * *Files identical despite different names*

### Comparing `CheckMyTex-0.8.1/checkmytex/cli/problem_handler.py` & `CheckMyTex-0.9.0/checkmytex/cli/problem_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,80 +35,79 @@
         self.analyzed_document.mark_as_false_positive(problem)
         return True
 
     def _ignore_all(self, problem):
         self.analyzed_document.remove_with_rule(problem.rule)
         return True
 
-    def _edit(self, problem):
-        f = problem.origin.file
-        line = problem.origin.begin.row
+    def _edit(self, problem: Problem):
+        f = problem.origin.get_file()
+        line = problem.origin.get_file_line()
         self.editor.open(file=f, line=line)
         return True
 
     def _next_file(self, problem):
-        self._skip_file = problem.origin.file
+        self._skip_file = problem.origin.get_file()
         return True
 
     def _look_up(self, problem):
         webbrowser.open(problem.look_up_url)
         return False
 
     def _print_details(self, problem: Problem):
         print("Message:", problem.message)
         print("Tool:", problem.tool)
         print("Rule:", problem.rule)
         print("Context:", problem.context.replace("\n", " "))
         o = problem.origin
         n = 40
-        if o.begin.tpos is not None and o.end.tpos is not None:
+        t_span = o.get_text_span()
+        if t_span:
             text = self.analyzed_document.document.get_text()
-            begin = max(0, o.begin.tpos - n)
-            end = min(len(text), o.end.tpos + n)
+            begin = max(0, t_span[0] - n)
+            end = min(len(text), t_span[1] + n)
             print_detail(
-                "Text: " + text[begin : o.begin.tpos],
-                text[o.begin.tpos : o.end.tpos],
-                text[o.end.tpos : end],
+                "Text: " + text[begin : t_span[0]],
+                text[t_span[0] : t_span[1]],
+                text[t_span[1] : end],
             )
-        if None not in (o.begin.spos, o.end.spos):
+        s_span = o.get_source_span()
+        if s_span:
             source = self.analyzed_document.document.get_source()
-            begin = max(0, o.begin.spos - n)
-            end = min(len(source), o.end.spos + n)
+            s_span = o.get_source_span()
+            begin = max(0, s_span[0] - n)
+            end = min(len(source),s_span[1] + n)
             print_detail(
-                "Source: " + source[begin : o.begin.spos],
-                source[o.begin.spos : o.end.spos],
-                source[o.end.spos : end],
+                "Source: " + source[begin : s_span[0]],
+                source[s_span[0] : s_span[1]],
+                source[s_span[1] : end],
             )
         print("Position:", problem.origin)
         return False
 
     def find(self, problem: Problem):
         log("Use this find-utility to compare with other occurrences.")
         pattern = input("Find pattern (regex):")
         if pattern:
             log("Searching in text...")
             for origin in self.analyzed_document.document.find_in_text(pattern):
                 print(origin)
-                for l in range(origin.begin.row, origin.end.row + 1):
-                    source = self.analyzed_document.get_file_content(origin.file).split(
-                        "\n"
-                    )
-                    print_simple_line(l, source[l])
+                l = origin.get_source_line()
+                source = self.analyzed_document.document.get_source(l)
+                print_simple_line(l, source)
             log("Searching in source...")
             for origin in self.analyzed_document.document.find_in_source(pattern):
                 print(origin)
-                for l in range(origin.begin.row, origin.end.row + 1):
-                    source = self.analyzed_document.get_file_content(origin.file).split(
-                        "\n"
-                    )
-                    print_simple_line(l, source[l])
+                l = origin.get_source_line()
+                source = self.analyzed_document.document.get_source(l)
+                print_simple_line(l, source)
         return False
 
     def __call__(self, problem: Problem):
-        if problem.origin.file == self._skip_file:
+        if problem.origin.get_file() == self._skip_file:
             return
         prompt = OptionPrompt()
         prompt.add_option(
             "s", "[s]kip", lambda p: True, help_="Skip to the next problem."
         )
         prompt.add_option(
             "S", "[S]kip all", self._skip_all, help_="Skip all similar problems."
```

### Comparing `CheckMyTex-0.8.1/checkmytex/document_analyzer.py` & `CheckMyTex-0.9.0/checkmytex/document_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,10 +98,9 @@
             try:
                 for problem in checker.check(latex_document):
                     yield problem
             except AssertionError as ae:
                 raise ae
             except Exception as e:
                 logging.getLogger("CheckMyTex").error(
-                    f"Exception using {checker}: {e}. {type(e)}"
+                    f"Exception using {checker}: {e}."
                 )
-                raise e
```

### Comparing `CheckMyTex-0.8.1/checkmytex/filtering/authors.py` & `CheckMyTex-0.9.0/checkmytex/filtering/authors.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,30 +32,30 @@
                 self._name_elements.update(name.split("-"))
         self._name_elements.add("et")
         self._name_elements.add("al")
 
     def filter(self, problems: typing.Iterable[Problem]) -> typing.Iterable[Problem]:
         for problem in problems:
             if problem.rule == "SPELLING":
-                begin = problem.origin.begin.tpos
-                end = problem.origin.end.tpos
+                begin = problem.origin.begin.text.index
+                end = problem.origin.end.text.index
                 misspelled_word = self._text[begin:end].strip()
                 if misspelled_word in self._name_elements:
                     continue
             yield problem
 
 
 def _find_bibtex_paths(document: LatexDocument):
     regex = r"\\((addbibresource)|(bibliography))\{(?P<path>[^}]+)\}"
     paths = set()
     for match in re.finditer(regex, document.get_source()):
         bib_file = match.group("path")
-        in_file = document.get_origin_of_source(
+        in_file = document.get_simplified_origin_of_source(
             match.start("path"), match.end("path")
-        ).file
+        ).get_file()
         path = os.path.join(os.path.dirname(in_file), bib_file)
         if os.path.isfile(path):
             paths.add(path)
         elif os.path.isfile(path + ".bib"):
             paths.add(path + ".bib")
     return paths
 
@@ -98,13 +98,13 @@
         self._text = document.get_text()
         bibtex = self._collect_bibtexs(document)
         self._extract_words_from_bibtex(bibtex)
 
     def filter(self, problems: typing.Iterable[Problem]) -> typing.Iterable[Problem]:
         for problem in problems:
             if problem.rule == "SPELLING":
-                begin = problem.origin.begin.tpos
-                end = problem.origin.end.tpos
+                begin = problem.origin.begin.text.index
+                end = problem.origin.end.text.index
                 misspelled_word = self._text[begin:end].strip()
                 if misspelled_word in self.word_list:
                     continue
             yield problem
```

### Comparing `CheckMyTex-0.8.1/checkmytex/filtering/filter.py` & `CheckMyTex-0.9.0/checkmytex/filtering/filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,16 +29,16 @@
         expr = r"\\includegraphics(\[[^\]]*\])?\{(?P<path>[^\}]+)\}"
         for match in re.finditer(expr, document.get_source()):
             r = (match.start("path"), match.end("path"))
             self._ranges.append(r)
 
     def filter(self, problems: typing.Iterable[Problem]) -> typing.Iterable[Problem]:
         for problem in problems:
-            begin = problem.origin.begin.spos
-            end = problem.origin.end.spos
+            begin = problem.origin.begin.source.index
+            end = problem.origin.end.source.index
             if not any(r[0] <= begin <= end <= r[1] for r in self._ranges):
                 yield problem
 
 
 class IgnoreRefs(Filter):
     def __init__(self):
         self._ranges = []
@@ -47,16 +47,16 @@
         expr = r"\\(([Cc]?ref)|(fullcite)|(f?ref((ch)|(sec))))\{(?P<ref>[^\}]+)\}"
         for match in re.finditer(expr, document.get_source()):
             span = (match.start("ref"), match.end("ref"))
             self._ranges.append(span)
 
     def filter(self, problems: typing.Iterable[Problem]) -> typing.Iterable[Problem]:
         for problem in problems:
-            begin = problem.origin.begin.spos
-            end = problem.origin.end.spos
+            begin = problem.origin.begin.source.index
+            end = problem.origin.end.source.index
             if not any(r[0] <= begin <= end <= r[1] for r in self._ranges):
                 yield problem
 
 
 class IgnoreRepeatedWords(Filter):
     def __init__(self, words: typing.List[str]):
         self.words = words
@@ -66,15 +66,17 @@
         self.document = document
 
     def filter(self, problems: typing.Iterable[Problem]) -> typing.Iterable[Problem]:
         assert self.document, "Prepare has been called."
         for problem in problems:
             if problem.rule == "EN_REPEATEDWORDS_PROBLEM":
                 text = self.document.get_file_content(problem.origin.file)
-                section = text[problem.origin.begin.pos : problem.origin.end.pos]
+                section = text[
+                    problem.origin.begin.file.position.index : problem.origin.end.file.position.index
+                ]
                 if section.strip().lower() in self.words:
                     continue
             yield problem
 
 
 class IgnoreSpellingWithMath(Filter):
     def __init__(self):
@@ -82,13 +84,13 @@
 
     def prepare(self, document: LatexDocument):
         self.document = document
 
     def filter(self, problems: typing.Iterable[Problem]) -> typing.Iterable[Problem]:
         for problem in problems:
             if problem.rule == "SPELLING":
-                begin = problem.origin.begin.spos
-                end = problem.origin.end.spos
+                begin = problem.origin.begin.source.index
+                end = problem.origin.end.source.index
                 source_of_word = self.document.get_source()[begin:end]
                 if "\\" in source_of_word or "$" in source_of_word:
                     continue
             yield problem
```

### Comparing `CheckMyTex-0.8.1/checkmytex/filtering/math_mode.py` & `CheckMyTex-0.9.0/checkmytex/filtering/math_mode.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,16 +71,16 @@
                 if not rules or problem.rule in rules:
                     return True
         return False
 
     def _problem_applies(self, problem):
         if not self._problem_fits_rule(problem):
             return False
-        begin = problem.origin.begin.spos
-        end = problem.origin.end.spos
+        begin = problem.origin.begin.source.index
+        end = problem.origin.end.source.index
         if not any(r[0] <= begin <= end <= r[1] for r in self.ranges):
             return False
         return True
 
     def filter(self, problems: typing.Iterable[Problem]) -> typing.Iterable[Problem]:
         for problem in problems:
             if not self._problem_applies(problem):
```

### Comparing `CheckMyTex-0.8.1/checkmytex/filtering/whitelist.py` & `CheckMyTex-0.9.0/checkmytex/filtering/whitelist.py`

 * *Files identical despite different names*

### Comparing `CheckMyTex-0.8.1/checkmytex/finding/abstract_checker.py` & `CheckMyTex-0.9.0/checkmytex/finding/abstract_checker.py`

 * *Files identical despite different names*

### Comparing `CheckMyTex-0.8.1/checkmytex/finding/chktex.py` & `CheckMyTex-0.9.0/checkmytex/finding/chktex.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     message = match.group("message")
     message_type = match.group("type")
     context_before = match.group("context_before")
     text = match.group("text")
     context_after = match.group("context_after")
     begin = (row - 1, col - 1)
     end = (row - 1, col + max(len(text), 1) - 1)
-    origin = document.get_origin_of_source(begin, end)
+    origin = document.get_simplified_origin_of_source(begin, end)
 
     longid = message + "|" + context_before + text + context_after
     return Problem(
         origin=origin,
         tool="chktex",
         long_id=longid,
         context=context_before + text + context_after,
```

### Comparing `CheckMyTex-0.8.1/checkmytex/finding/cleveref.py` & `CheckMyTex-0.9.0/checkmytex/finding/cleveref.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,16 +15,18 @@
     A checker module for finding raw \\ref. Better use \\cref.
     """
 
     def check(self, document: LatexDocument) -> typing.Iterable[Problem]:
         self.log("Checking for cleveref usage...")
         # \ref instead of smarter \cref
         for match in re.finditer(r"\\ref\{[^\}]+\}", document.get_source()):
-            origin = document.get_origin_of_source(match.start(), match.end())
-            context = document.get_source_context(origin)
+            origin = document.get_simplified_origin_of_source(
+                match.start(), match.end()
+            )
+            context = match.string
             message = (
                 "Prefer using cleveref's \\cref or \\Cref instead of native \\ref."
             )
             rule = "CREF"
             yield Problem(
                 origin,
                 context=context,
@@ -33,18 +35,18 @@
                 tool="CleverrefCheck",
                 rule=rule,
                 look_up_url="https://ctan.org/pkg/cleveref?lang=en",
             )
         # \cref instead of \Cref at beginning of sentence
         expr = r"\.\s*(?P<cref>\\cref\{[^\}]+\})"  # ". \cref{xxx}"
         for match in re.finditer(expr, document.get_source()):
-            origin = document.get_origin_of_source(
+            origin = document.get_simplified_origin_of_source(
                 match.start("cref"), match.end("cref")
             )
-            context = document.get_source_context(origin)
+            context = match.string
             message = "Use \\Cref instead of \\cref at the beginning of a sentence."
             rule = "CREF-CAPTION"
             yield Problem(
                 origin,
                 context=context,
                 message=message,
                 long_id=rule + "|" + context,
```

### Comparing `CheckMyTex-0.8.1/checkmytex/finding/languagetool.py` & `CheckMyTex-0.9.0/checkmytex/finding/languagetool.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         )
         data = json.loads(result)
         for problem in data["matches"]:
             try:
                 look_up_url = problem["rule"]["urls"][0]["value"]
             except KeyError:
                 look_up_url = None
-            origin = document.get_origin_of_text(
+            origin = document.get_simplified_origin_of_text(
                 problem["offset"], problem["offset"] + problem["length"]
             )
             # using source context because the detexed context is too unstable with math
             context = document.get_source_context(origin)
             # the rule 'a/an' results in many false positives before math or commands.
             if self._is_an_before_math(problem, origin, document):
                 continue
@@ -68,27 +68,29 @@
         """
         'A' before math or a command will frequently lead to false positives.
         """
         if problem["rule"]["id"] != "EN_A_VS_AN":
             return False
         source = document.get_source()
         context = source[
-            origin.end.spos : max(len(source), origin.end.spos + 10)
+            origin.end.source.index : max(len(source), origin.end.source.index + 10)
         ].strip()
         if context and context[0] in ("\\", "$"):
             return True
         return False
 
     def _is_uppercase_letter_after_backslash(
         self, problem, origin: Origin, document: LatexDocument
     ) -> bool:
         if problem["rule"]["id"] != "UPPERCASE_SENTENCE_START":
             return False
         source = document.get_source()
-        context = source[max(0, origin.begin.spos - 10) : origin.begin.spos].strip()
+        context = source[
+            max(0, origin.begin.source.index - 10) : origin.begin.source.index
+        ].strip()
         if context and context[-1] == "\\":
             return True
         return False
 
     def is_available(self) -> bool:
         return bool(shutil.which("languagetool"))
```

### Comparing `CheckMyTex-0.8.1/checkmytex/finding/nphard.py` & `CheckMyTex-0.9.0/checkmytex/finding/nphard.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,17 @@
             if "\\NP" in cmd:  # $\NP$ and \NP can be mixed with no problem
                 variants_np.add("\\NP")
                 continue  # do not create a warning for usage of \\NP
             variants_np.add(cmd)
             if len(variants_np) <= 1:
                 continue
 
-            origin = document.get_origin_of_source(match.start(), match.end())
+            origin = document.get_simplified_origin_of_source(
+                match.start(), match.end()
+            )
             context = document.get_source_context(origin)
             message = "Non-uniform 'NP'. Maybe use the 'complexity'-package?"
             rule = "UNIFORM-NP"
             yield Problem(
                 origin,
                 context=context,
                 message=message,
```

### Comparing `CheckMyTex-0.8.1/checkmytex/finding/problem.py` & `CheckMyTex-0.9.0/checkmytex/finding/problem.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 
     def __eq__(self, other):
         return other.short_id == self.short_id
 
     def __hash__(self):
         return hash(self.short_id)
 
-    def to_json(self) -> dict:
+    def serialize(self) -> dict:
         return {
             "id": self.short_id,
             "tool": self.tool,
             "message": self.message,
             "context": self.context,
             "rule": self.rule,
-            "origin": self.origin,
+            "origin": self.origin.serialize() if self.origin else None,
             "url": self.look_up_url,
         }
```

### Comparing `CheckMyTex-0.8.1/checkmytex/finding/proselint.py` & `CheckMyTex-0.9.0/checkmytex/finding/proselint.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     def check(self, document: LatexDocument) -> typing.Iterable[Problem]:
         self.log("Running proselint...")
         text = document.get_text()
         suggestions = proselint.tools.lint(text, config=_proselint_config)
         for suggestion in suggestions:
             rule = suggestion[0]
             message = suggestion[1]
-            origin = document.get_origin_of_text(
+            origin = document.get_simplified_origin_of_text(
                 suggestion[4], suggestion[4] + suggestion[6]
             )
             context = document.get_source_context(origin)
             severity = suggestion[7]
             replacements = suggestion[8]
             yield Problem(
                 origin,
```

### Comparing `CheckMyTex-0.8.1/checkmytex/finding/siunitx.py` & `CheckMyTex-0.9.0/checkmytex/finding/siunitx.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         for match in self.regex.finditer(source):
             num = match.group("number").strip()
             if len(num) == 1 or (len(num) == 2 and num[1] in (".", ",")):
                 # Don't complain about small numbers.
                 continue
             if _looks_like_year(num):  # many false positives.
                 continue
-            origin = document.get_origin_of_source(
+            origin = document.get_simplified_origin_of_source(
                 match.start("number"), match.end("number")
             )
             message = (
                 "Use siunitx to get nice and uniform numbers "
                 "(\\num{} at least for >=10 000)"
                 " and units (\\SI{}{} for all sizes)."
             )
```

### Comparing `CheckMyTex-0.8.1/checkmytex/finding/spellcheck.py` & `CheckMyTex-0.9.0/checkmytex/finding/spellcheck.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         for match in word_regex.finditer(text):
             word = match.group("word").strip()
             if word[-1] in ":,.!?)":
                 word = word[:-1]
             if not is_word.fullmatch(word):
                 continue
             begin = match.start("word")
-            origin = document.get_origin_of_text(begin, begin + len(word))
+            origin = document.get_simplified_origin_of_text(begin, begin + len(word))
             if word not in word_occurrences:
                 word_occurrences[word] = []
             word_occurrences[word].append(origin)
         return word_occurrences
 
     def check(self, document: LatexDocument) -> typing.Iterable[Problem]:
         self.log("Running spellchecking...")
@@ -108,15 +108,15 @@
                     yield p
 
     def _create_word_problems(self, word, begin, document, text):
         word_elements = word.split("-")
         for word_element in word_elements:
             if len(word_element) < 2 or not self.spell.unknown([word_element]):
                 continue
-            origin = document.get_origin_of_text(begin, begin + len(word))
+            origin = document.get_simplified_origin_of_text(begin, begin + len(word))
             candidates = [
                 c for c in self.spell.candidates(word_element) if c != word_element
             ]
             context = text[max(0, begin - 20) : min(len(text), begin + len(word) + 20)]
             url = f"https://www.google.com/search?q={urllib.parse.quote(word)}"
             msg = f"Spelling '{word}'. Candidates: {candidates}."
             yield Problem(
```

### Comparing `CheckMyTex-0.8.1/checkmytex/latex_document/__init__.py` & `CheckMyTex-0.9.0/checkmytex/latex_document/__init__.py`

 * *Files identical despite different names*

### Comparing `CheckMyTex-0.8.1/checkmytex/latex_document/origin.py` & `CheckMyTex-0.9.0/checkmytex/latex_document/origin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,93 @@
 import typing
 
+from checkmytex.latex_document.indexed_string import TextPosition
+from checkmytex.latex_document.source import FilePosition
 
-class Origin:
+
+class OriginPointer:
     """
-    The origin of a part of the parse latex document.
+    A position in a text file.
     """
 
-    class Position:
-        """
-        A position in a text file.
-        """
-
-        def __init__(
+    def __init__(
             self,
-            pos: int,
-            row: int,
-            col: int,
-            spos: int,
-            tpos: typing.Optional[int] = None,
-        ):
-            self.pos = pos  # position in the file. Starting at zero.
-            self.row = row  # row or line in the file. Starting at zero.
-            self.col = col  # column in the line. Starting at zero.
-            self.spos = spos  # position in the source string
-            self.tpos = tpos  # position in the text string
-
-        def __eq__(self, other):
-            if not isinstance(other, Origin.Position):
-                raise ValueError("Can only compare positions.")
-            return (
-                self.pos == other.pos
-                and self.row == other.row
-                and self.col == other.col
-            )
-
-        def __lt__(self, other):
-            if not isinstance(other, Origin.Position):
-                raise ValueError("Can only compare positions.")
-            return self.pos < other.pos
+            file: FilePosition,
+            source: TextPosition,
+            text: typing.Optional[TextPosition] = None,
+    ):
+        self.file = file  # position in file
+        self.source = source  # position in flat source
+        self.text = text  # position in detexed text
+
+    def __eq__(self, other):
+        if not isinstance(other, OriginPointer):
+            raise ValueError("Can only compare positions.")
+        return self.file == other.file
+
+    def __lt__(self, other):
+        if not isinstance(other, OriginPointer):
+            raise ValueError("Can only compare positions.")
+        return self.source < other.source
+
+    def __repr__(self):
+        return f"FILE:{self.file}|SOURCE:{self.source}|text::{self.text}"
+
+    def serialize(self) -> typing.Dict:
+        return {"file": self.file.serialize(),
+                "source": self.source.serialize(),
+                "text": self.text.serialize() if self.text else None}
+
+
+class Origin:
+    """
+    The origin of a part of the parse latex document.
+    """
 
     def __lt__(self, other):
         return (self.begin, self.end) < (other.begin, other.end)
 
-    def __init__(self, file: str, begin: Position, end: Position):
-        self.file: str = file
-        self.begin: Origin.Position = begin
-        self.end: Origin.Position = end
-        assert begin != end, "This would be empty"
+    def __init__(self, begin: OriginPointer, end: OriginPointer):
+        assert begin.file.path == end.file.path
+        self.begin: OriginPointer = begin
+        self.end: OriginPointer = end
+        assert begin < end, "This would be empty"
+
+    def get_file(self):
+        return self.begin.file.path
+
+    def get_text_span(self) -> typing.Optional[typing.Tuple[int, int]]:
+        if self.begin.text is None:
+            return None
+        return self.begin.text.index, self.end.text.index
+
+    def get_source_span(self) -> typing.Tuple[int, int]:
+        return self.begin.source.index, self.end.source.index
+
+    def get_file_span(self) -> typing.Tuple[int, int]:
+        return self.begin.file.position.index, self.end.file.position.index
+
+    def get_text_line(self) -> int:
+        return self.begin.text.line
+
+    def get_source_line(self) -> int:
+        return self.begin.source.line
+
+    def get_file_line(self) -> int:
+        return self.begin.file.position.line
 
     def __repr__(self):
-        return (
-            f"{self.file}"
-            f"[{self.begin.pos}:{self.begin.row}:{self.begin.col}"
-            f"-{self.end.pos}:{self.end.row}:{self.end.col}]"
-        )
+        return f"{self.get_file()}" f"[{self.begin.file.position}-{self.end.file.position}]"
 
     def __eq__(self, other):
         if not isinstance(other, Origin):
             raise ValueError("Can only compare origins.")
         return (
-            self.file == other.file
-            and self.begin == other.begin
-            and self.end == other.end
+                self.begin == other.begin
+                and self.end == other.end
         )
+
+    def serialize(self) -> typing.Dict:
+        return {
+            "begin": self.begin.serialize(),
+            "end": self.end.serialize()
+        }
```

### Comparing `CheckMyTex-0.8.1/checkmytex/utils/choice.py` & `CheckMyTex-0.9.0/checkmytex/utils/choice.py`

 * *Files identical despite different names*

### Comparing `CheckMyTex-0.8.1/checkmytex/utils/editor.py` & `CheckMyTex-0.9.0/checkmytex/utils/editor.py`

 * *Files identical despite different names*

### Comparing `CheckMyTex-0.8.1/setup.py` & `CheckMyTex-0.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
     with open("README.md") as file:
         return file.read()
 
 
 setup(
     name="CheckMyTex",
-    version="0.8.1",
+    version="0.9.0",
     description="A simple tool for checking complex LaTeX documents, e.g., dissertations.",
     long_description=readme(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

