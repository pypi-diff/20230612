# Comparing `tmp/getise-1.0.0.tar.gz` & `tmp/getise-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getise-1.0.0.tar", max compression
+gzip compressed data, was "getise-1.0.1.tar", max compression
```

## Comparing `getise-1.0.0.tar` & `getise-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1322 2023-06-12 09:32:56.957731 getise-1.0.0/LICENSE
--rw-r--r--   0        0        0      253 2023-06-12 12:57:14.032517 getise-1.0.0/README.md
--rw-r--r--   0        0        0      686 2023-06-12 12:57:14.033452 getise-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      262 2023-06-12 10:34:31.881384 getise-1.0.0/src/getise/__init__.py
--rw-r--r--   0        0        0     9547 2023-06-12 12:57:14.033933 getise-1.0.0/src/getise/cli.py
--rw-r--r--   0        0        0      996 1970-01-01 00:00:00.000000 getise-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1322 2023-06-12 09:32:56.957731 getise-1.0.1/LICENSE
+-rw-r--r--   0        0        0      253 2023-06-12 12:57:14.032517 getise-1.0.1/README.md
+-rw-r--r--   0        0        0      686 2023-06-12 13:02:06.520497 getise-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      262 2023-06-12 13:01:38.005412 getise-1.0.1/src/getise/__init__.py
+-rw-r--r--   0        0        0     9618 2023-06-12 13:02:05.135560 getise-1.0.1/src/getise/cli.py
+-rw-r--r--   0        0        0      996 1970-01-01 00:00:00.000000 getise-1.0.1/PKG-INFO
```

### Comparing `getise-1.0.0/LICENSE` & `getise-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `getise-1.0.0/pyproject.toml` & `getise-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getise"
-version = "1.0.0"
+version = "1.0.1"
 description = "Get networks from Cisco ISE"
 authors = ["Rob Woodward <rob@emailplus.org>"]
 
 license = "BSD-2-Clause"
 readme = "README.md"
 repository = "https://github.com/robwdwd/getise"
 include = ["README.md", "LICENSE"]
```

### Comparing `getise-1.0.0/src/getise/cli.py` & `getise-1.0.1/src/getise/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,14 +283,15 @@
     #
     git_repo = Repo(cfg["git"]["basedir"])
 
     # Pull in updates from the repository to make sure we are
     # up-to-date with everything.
     #
     origin = git_repo.remotes["origin"]
+    secondary = git_repo.remotes["secondary"]
     origin.pull()
 
     # Close and flush all the files
     #
     for open_file in gitseedfiles:
         gitseedfiles[open_file]["handle"].flush()
         gitseedfiles[open_file]["handle"].close()
@@ -321,14 +322,15 @@
         git_repo.index.add([gitseedfiles[git_file]["file_relative"]])
 
     # If we have changed files then stage and push them.
     #
     if git_repo.is_dirty():
         git_repo.index.commit("Get ISE Devices automated commit")
         origin.push()
+        secondary.push()
 
     ise_session.close()
 
     # Clean up the logging.
     #
     rejectfile.flush()
     dumpfile.flush()
```

### Comparing `getise-1.0.0/PKG-INFO` & `getise-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getise
-Version: 1.0.0
+Version: 1.0.1
 Summary: Get networks from Cisco ISE
 Home-page: https://github.com/robwdwd/getise
 License: BSD-2-Clause
 Author: Rob Woodward
 Author-email: rob@emailplus.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

