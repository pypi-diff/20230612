# Comparing `tmp/le-utils-0.1.9.tar.gz` & `tmp/le-utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\le-utils-0.1.9.tar", last modified: Fri Mar 23 23:22:45 2018, max compression
+gzip compressed data, was "dist/le-utils-0.2.0.tar", last modified: Mon Jun 12 04:14:36 2023, max compression
```

## Comparing `le-utils-0.1.9.tar` & `le-utils-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,44 @@
-drwxrwxrwx   0        0        0        0 2018-03-23 23:22:45.000000 le-utils-0.1.9/
-drwxrwxrwx   0        0        0        0 2018-03-23 23:22:45.000000 le-utils-0.1.9/le_utils/
-drwxrwxrwx   0        0        0        0 2018-03-23 23:22:45.000000 le-utils-0.1.9/le_utils/constants/
--rw-rw-rw-   0        0        0      717 2018-03-14 22:13:23.000000 le-utils-0.1.9/le_utils/constants/content_kinds.py
--rw-rw-rw-   0        0        0     1505 2017-05-17 01:00:02.000000 le-utils-0.1.9/le_utils/constants/exercises.py
--rw-rw-rw-   0        0        0     1437 2018-03-14 22:13:23.000000 le-utils-0.1.9/le_utils/constants/file_formats.py
--rw-rw-rw-   0        0        0      918 2018-03-14 22:13:23.000000 le-utils-0.1.9/le_utils/constants/file_types.py
--rw-rw-rw-   0        0        0     2342 2018-03-14 22:13:23.000000 le-utils-0.1.9/le_utils/constants/format_presets.py
--rw-rw-rw-   0        0        0     8668 2018-03-14 23:05:58.000000 le-utils-0.1.9/le_utils/constants/languages.py
--rw-rw-rw-   0        0        0      694 2017-04-11 03:05:56.000000 le-utils-0.1.9/le_utils/constants/licenses.py
--rw-rw-rw-   0        0        0      177 2018-03-23 23:22:07.000000 le-utils-0.1.9/le_utils/constants/roles.py
--rw-rw-rw-   0        0        0        0 2017-04-11 03:04:18.000000 le-utils-0.1.9/le_utils/constants/__init__.py
--rw-rw-rw-   0        0        0     6394 2017-07-27 19:05:38.000000 le-utils-0.1.9/le_utils/humanhash.py
--rw-rw-rw-   0        0        0     3872 2017-08-21 16:52:11.000000 le-utils-0.1.9/le_utils/proquint.py
-drwxrwxrwx   0        0        0        0 2018-03-23 23:22:45.000000 le-utils-0.1.9/le_utils/resources/
--rw-rw-rw-   0        0        0    18894 2018-03-14 22:13:23.000000 le-utils-0.1.9/le_utils/resources/languagelookup.json
--rw-rw-rw-   0        0        0        0 2017-04-11 03:04:18.000000 le-utils-0.1.9/le_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2018-03-23 23:22:45.000000 le-utils-0.1.9/le_utils.egg-info/
--rw-rw-rw-   0        0        0        1 2018-03-23 23:22:44.000000 le-utils-0.1.9/le_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     6451 2018-03-23 23:22:44.000000 le-utils-0.1.9/le_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       19 2018-03-23 23:22:44.000000 le-utils-0.1.9/le_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0      609 2018-03-23 23:22:45.000000 le-utils-0.1.9/le_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2018-03-23 23:22:44.000000 le-utils-0.1.9/le_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1102 2018-03-14 22:13:23.000000 le-utils-0.1.9/LICENSE.txt
--rw-rw-rw-   0        0        0       29 2017-04-11 03:04:18.000000 le-utils-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     6451 2018-03-23 23:22:45.000000 le-utils-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     4865 2018-03-14 22:13:23.000000 le-utils-0.1.9/README.md
--rw-rw-rw-   0        0        0      108 2018-03-23 23:22:45.000000 le-utils-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1114 2018-03-23 23:22:23.000000 le-utils-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 04:14:36.000000 le-utils-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-12 04:14:19.000000 le-utils-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-06-12 04:14:19.000000 le-utils-0.2.0/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     7165 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/humanhash.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils/constants/
+-rw-r--r--   0 runner    (1001) docker     (122)     4532 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/format_presets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/file_formats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/modalities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/content_kinds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9300 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/languages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/exercises.py
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/completion_criteria.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils/constants/labels/
+-rw-r--r--   0 runner    (1001) docker     (122)     5735 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/labels/subjects.py
+-rw-r--r--   0 runner    (1001) docker     (122)      873 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/labels/levels.py
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/labels/learning_activities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/labels/accessibility_categories.py
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/labels/needs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/labels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/labels/resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1750 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/mastery_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)     8183 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/resources/presetlookup.json
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/resources/kindlookup.json
+-rw-r--r--   0 runner    (1001) docker     (122)    21338 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/resources/languagelookup.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/resources/licenselookup.json
+-rw-r--r--   0 runner    (1001) docker     (122)      710 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/resources/formatlookup.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2851 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/proquint.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12733 2023-06-12 04:14:36.000000 le-utils-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-12 04:14:36.000000 le-utils-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-06-12 04:14:19.000000 le-utils-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    12733 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1163 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    10228 2023-06-12 04:14:19.000000 le-utils-0.2.0/README.md
```

### Comparing `le-utils-0.1.9/le_utils/constants/exercises.py` & `le-utils-0.2.0/le_utils/constants/exercises.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,46 @@
-# coding=utf-8
-
-from gettext import gettext as _
-
-""" Mastery Models """
-DO_ALL = "do_all"
-NUM_CORRECT_IN_A_ROW_10 = "num_correct_in_a_row_10"
-NUM_CORRECT_IN_A_ROW_2 = "num_correct_in_a_row_2"
-NUM_CORRECT_IN_A_ROW_3 = "num_correct_in_a_row_3"
-NUM_CORRECT_IN_A_ROW_5 = "num_correct_in_a_row_5"
-SKILL_CHECK = "skill_check"
-M_OF_N = "m_of_n"
-
-MASTERY_MODELS = (
-    (DO_ALL, _("Do all")),
-    (NUM_CORRECT_IN_A_ROW_2, _("2 in a row")),
-    (NUM_CORRECT_IN_A_ROW_10, _("10 in a row")),
-    (NUM_CORRECT_IN_A_ROW_3, _("3 in a row")),
-    (NUM_CORRECT_IN_A_ROW_5, _("5 in a row")),
-    (SKILL_CHECK, _("Skill check")),
-    (M_OF_N, _("M out of N")),
-)
-
-IMG_PLACEHOLDER = "{☣ LOCALPATH}"
-IMG_FORMAT = "${" + IMG_PLACEHOLDER + "}/{0}"
-IMG_REGEX = r'\$\{☣ LOCALPATH\}\/(.+)'
-
-CONTENT_STORAGE_PLACEHOLDER = "{☣ CONTENTSTORAGE}"
-CONTENT_STORAGE_FORMAT = "${" + CONTENT_STORAGE_PLACEHOLDER + "}/{0}"
-CONTENT_STORAGE_REGEX = r'\(\$\{☣ CONTENTSTORAGE\}\/(.+)\)'
-
-GRAPHIE_DELIMITER = '$$$GRAPHIE_BREAK$$$'
-
-""" Question Types """
-INPUT_QUESTION = "input_question"
-MULTIPLE_SELECTION = "multiple_selection"
-SINGLE_SELECTION = "single_selection"
-FREE_RESPONSE = "free_response"
-PERSEUS_QUESTION = "perseus_question"
-
-question_choices = (
-    (INPUT_QUESTION, _("Input Question")),
-    (MULTIPLE_SELECTION, _("Multiple Selection")),
-    (SINGLE_SELECTION, _("Single Selection")),
-    (FREE_RESPONSE, _("Free Response")),
-    (PERSEUS_QUESTION, _("Perseus Question")),
-)
+# coding=utf-8
+""" Mastery Models """
+DO_ALL = "do_all"
+NUM_CORRECT_IN_A_ROW_10 = "num_correct_in_a_row_10"
+NUM_CORRECT_IN_A_ROW_2 = "num_correct_in_a_row_2"
+NUM_CORRECT_IN_A_ROW_3 = "num_correct_in_a_row_3"
+NUM_CORRECT_IN_A_ROW_5 = "num_correct_in_a_row_5"
+SKILL_CHECK = "skill_check"
+M_OF_N = "m_of_n"
+QUIZ = "quiz"
+
+MASTERY_MODELS = (
+    (DO_ALL, "Do all"),
+    (NUM_CORRECT_IN_A_ROW_2, "2 in a row"),
+    (NUM_CORRECT_IN_A_ROW_10, "10 in a row"),
+    (NUM_CORRECT_IN_A_ROW_3, "3 in a row"),
+    (NUM_CORRECT_IN_A_ROW_5, "5 in a row"),
+    (SKILL_CHECK, "Skill check"),
+    (M_OF_N, "M out of N"),
+    (QUIZ, "Quiz"),
+)
+
+IMG_PLACEHOLDER = "{☣ LOCALPATH}"
+IMG_FORMAT = "${" + IMG_PLACEHOLDER + "}/{0}"
+IMG_REGEX = r"\$\{☣ LOCALPATH\}\/(.+)"
+
+CONTENT_STORAGE_PLACEHOLDER = "{☣ CONTENTSTORAGE}"
+CONTENT_STORAGE_FORMAT = "${" + CONTENT_STORAGE_PLACEHOLDER + "}/{0}"
+CONTENT_STORAGE_REGEX = r"\(\$\{☣ CONTENTSTORAGE\}\/(.+)\)"
+
+GRAPHIE_DELIMITER = "$$$GRAPHIE_BREAK$$$"
+
+""" Question Types """
+INPUT_QUESTION = "input_question"
+MULTIPLE_SELECTION = "multiple_selection"
+SINGLE_SELECTION = "single_selection"
+FREE_RESPONSE = "free_response"
+PERSEUS_QUESTION = "perseus_question"
+
+question_choices = (
+    (INPUT_QUESTION, "Input Question"),
+    (MULTIPLE_SELECTION, "Multiple Selection"),
+    (SINGLE_SELECTION, "Single Selection"),
+    (FREE_RESPONSE, "Free Response"),
+    (PERSEUS_QUESTION, "Perseus Question"),
+)
```

### Comparing `le-utils-0.1.9/LICENSE.txt` & `le-utils-0.2.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-The MIT License (MIT)
-
-Copyright (c) 2018 Learning Equality
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2018 Learning Equality
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

