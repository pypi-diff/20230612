# Comparing `tmp/jira2branch-0.2.0.tar.gz` & `tmp/jira2branch-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jira2branch-0.2.0.tar", max compression
+gzip compressed data, was "jira2branch-0.2.1.tar", max compression
```

## Comparing `jira2branch-0.2.0.tar` & `jira2branch-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-05-19 17:01:56.796560 jira2branch-0.2.0/LICENSE
--rw-r--r--   0        0        0     1638 2023-05-24 15:25:44.402088 jira2branch-0.2.0/README.md
--rw-r--r--   0        0        0       75 2023-05-19 17:00:08.394276 jira2branch-0.2.0/jira2branch/__init__.py
--rw-r--r--   0        0        0    20610 2023-06-07 14:24:28.539445 jira2branch-0.2.0/jira2branch/__main__.py
--rw-r--r--   0        0        0        0 2023-05-19 17:00:08.394276 jira2branch-0.2.0/jira2branch/tests/__init__.py
--rw-r--r--   0        0        0     1483 2023-05-19 17:00:08.394276 jira2branch-0.2.0/jira2branch/tests/test_main.py
--rw-r--r--   0        0        0      655 2023-06-07 14:25:38.869526 jira2branch-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 jira2branch-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-19 17:01:56.796560 jira2branch-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1993 2023-06-12 14:36:00.717511 jira2branch-0.2.1/README.md
+-rw-r--r--   0        0        0       75 2023-05-19 17:00:08.394276 jira2branch-0.2.1/jira2branch/__init__.py
+-rw-r--r--   0        0        0    20610 2023-06-12 14:31:07.673993 jira2branch-0.2.1/jira2branch/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-19 17:00:08.394276 jira2branch-0.2.1/jira2branch/tests/__init__.py
+-rw-r--r--   0        0        0     1483 2023-05-19 17:00:08.394276 jira2branch-0.2.1/jira2branch/tests/test_main.py
+-rw-r--r--   0        0        0      655 2023-06-12 14:36:24.930860 jira2branch-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 jira2branch-0.2.1/PKG-INFO
```

### Comparing `jira2branch-0.2.0/LICENSE` & `jira2branch-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jira2branch-0.2.0/README.md` & `jira2branch-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,20 @@
   tracking remote branch
 
 Options:
   -n, --name-only      Generates the branch name and prints it, no actual
                        branch will be created (default is False)
   -p, --push           Push newly created branch to remote (default is False)
   -t, --target PATH    Target repository (default is current directory)
-  -r, --merge-request  Create merge request. Requires --push. (default is
-                       False)
+  -r, --merge-request  Create merge request. Requires --push. (default is False)
+  -c, --confirm        Request confirmation before creating the merge request (default is False)
+  -d --dry-run         Dry run. Prints out the MR payload in JSON format but does not invoke the API 
+  
+  --preview (experimental) This toggles live preview ON when editing a merge request description. Requires vim being set as $EDITOR with markdown-preview.vim plugin installed
+
   --help               Show this message and exit.
 ```
 
 - Branch naming format is as follows:
   - {CONVENTIONAL_COMMIT_PREFIX}/{ISSUE_ID}_{ISSUE_TITLE}
 
 ## Requirements
```

### Comparing `jira2branch-0.2.0/jira2branch/__main__.py` & `jira2branch-0.2.1/jira2branch/__main__.py`

 * *Files identical despite different names*

### Comparing `jira2branch-0.2.0/jira2branch/tests/test_main.py` & `jira2branch-0.2.1/jira2branch/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `jira2branch-0.2.0/pyproject.toml` & `jira2branch-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jira2branch"
-version = "0.2.0"
+version = "0.2.1"
 description = "Takes a JIRA issue and creates a git branch"
 authors = ["Tiago Pereira <tiago@tiagoafpereira.net>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python :: 3",
```

### Comparing `jira2branch-0.2.0/PKG-INFO` & `jira2branch-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira2branch
-Version: 0.2.0
+Version: 0.2.1
 Summary: Takes a JIRA issue and creates a git branch
 License: MIT
 Author: Tiago Pereira
 Author-email: tiago@tiagoafpereira.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -30,16 +30,20 @@
   tracking remote branch
 
 Options:
   -n, --name-only      Generates the branch name and prints it, no actual
                        branch will be created (default is False)
   -p, --push           Push newly created branch to remote (default is False)
   -t, --target PATH    Target repository (default is current directory)
-  -r, --merge-request  Create merge request. Requires --push. (default is
-                       False)
+  -r, --merge-request  Create merge request. Requires --push. (default is False)
+  -c, --confirm        Request confirmation before creating the merge request (default is False)
+  -d --dry-run         Dry run. Prints out the MR payload in JSON format but does not invoke the API 
+  
+  --preview (experimental) This toggles live preview ON when editing a merge request description. Requires vim being set as $EDITOR with markdown-preview.vim plugin installed
+
   --help               Show this message and exit.
 ```
 
 - Branch naming format is as follows:
   - {CONVENTIONAL_COMMIT_PREFIX}/{ISSUE_ID}_{ISSUE_TITLE}
 
 ## Requirements
```

