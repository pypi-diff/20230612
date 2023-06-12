# Comparing `tmp/git-sim-0.3.1.tar.gz` & `tmp/git-sim-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-sim-0.3.1.tar", last modified: Tue Jun  6 18:46:27 2023, max compression
+gzip compressed data, was "git-sim-0.3.2.tar", last modified: Mon Jun 12 02:56:59 2023, max compression
```

## Comparing `git-sim-0.3.1.tar` & `git-sim-0.3.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 18:46:27.922754 git-sim-0.3.1/
--rw-rw-rw-   0        0        0    18431 2023-03-09 07:57:29.000000 git-sim-0.3.1/LICENSE
--rw-rw-rw-   0        0        0       26 2023-03-09 07:57:17.000000 git-sim-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0    25490 2023-06-06 18:46:27.922754 git-sim-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    24683 2023-06-06 18:44:43.000000 git-sim-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 18:46:27.914290 git-sim-0.3.1/git_sim/
--rw-rw-rw-   0        0        0       23 2023-06-06 18:44:43.000000 git-sim-0.3.1/git_sim/__init__.py
--rw-rw-rw-   0        0        0     8333 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/__main__.py
--rw-rw-rw-   0        0        0     2852 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/add.py
--rw-rw-rw-   0        0        0     3680 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/animations.py
--rw-rw-rw-   0        0        0     1511 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/branch.py
--rw-rw-rw-   0        0        0     4415 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/checkout.py
--rw-rw-rw-   0        0        0     2302 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/cherrypick.py
--rw-rw-rw-   0        0        0     3921 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/clean.py
--rw-rw-rw-   0        0        0     2974 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/clone.py
--rw-rw-rw-   0        0        0     8586 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/commands.py
--rw-rw-rw-   0        0        0     3175 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/commit.py
--rw-rw-rw-   0        0        0      572 2023-04-21 21:10:02.000000 git-sim-0.3.1/git_sim/enums.py
--rw-rw-rw-   0        0        0     2842 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/fetch.py
--rw-rw-rw-   0        0        0    46330 2023-06-06 18:44:43.000000 git-sim-0.3.1/git_sim/git_sim_base_command.py
--rw-rw-rw-   0        0        0     1415 2023-06-06 18:37:54.000000 git-sim-0.3.1/git_sim/log.py
--rw-rw-rw-   0        0        0    63319 2023-03-09 07:57:17.000000 git-sim-0.3.1/git_sim/logo.png
--rw-rw-rw-   0        0        0     7251 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/merge.py
--rw-rw-rw-   0        0        0     2937 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/mv.py
--rw-rw-rw-   0        0        0     3844 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/pull.py
--rw-rw-rw-   0        0        0     7226 2023-04-21 21:10:02.000000 git-sim-0.3.1/git_sim/push.py
--rw-rw-rw-   0        0        0     6057 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/rebase.py
--rw-rw-rw-   0        0        0     5042 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/reset.py
--rw-rw-rw-   0        0        0     2467 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/restore.py
--rw-rw-rw-   0        0        0     5607 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/revert.py
--rw-rw-rw-   0        0        0     4541 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/rm.py
--rw-rw-rw-   0        0        0     1380 2023-04-21 20:23:21.000000 git-sim-0.3.1/git_sim/settings.py
--rw-rw-rw-   0        0        0     6505 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/stash.py
--rw-rw-rw-   0        0        0      829 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/status.py
--rw-rw-rw-   0        0        0     4413 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/switch.py
--rw-rw-rw-   0        0        0     1469 2023-04-21 20:10:26.000000 git-sim-0.3.1/git_sim/tag.py
-drwxrwxrwx   0        0        0        0 2023-06-06 18:46:27.921754 git-sim-0.3.1/git_sim.egg-info/
--rw-rw-rw-   0        0        0    25490 2023-06-06 18:46:27.000000 git-sim-0.3.1/git_sim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      770 2023-06-06 18:46:27.000000 git-sim-0.3.1/git_sim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 18:46:27.000000 git-sim-0.3.1/git_sim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-06-06 18:46:27.000000 git-sim-0.3.1/git_sim.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2023-06-06 18:46:27.000000 git-sim-0.3.1/git_sim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-06 18:46:27.000000 git-sim-0.3.1/git_sim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 18:46:27.922754 git-sim-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1468 2023-04-21 20:23:21.000000 git-sim-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:56:59.256162 git-sim-0.3.2/
+-rw-rw-rw-   0        0        0    18431 2023-03-09 07:57:29.000000 git-sim-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-03-09 07:57:17.000000 git-sim-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    25490 2023-06-12 02:56:59.256162 git-sim-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    24683 2023-06-12 02:56:27.000000 git-sim-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 02:56:59.249657 git-sim-0.3.2/git_sim/
+-rw-rw-rw-   0        0        0       23 2023-06-12 02:56:27.000000 git-sim-0.3.2/git_sim/__init__.py
+-rw-rw-rw-   0        0        0     8333 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/__main__.py
+-rw-rw-rw-   0        0        0     2852 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/add.py
+-rw-rw-rw-   0        0        0     3680 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/animations.py
+-rw-rw-rw-   0        0        0     1511 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/branch.py
+-rw-rw-rw-   0        0        0     4415 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/checkout.py
+-rw-rw-rw-   0        0        0     2302 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/cherrypick.py
+-rw-rw-rw-   0        0        0     3921 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/clean.py
+-rw-rw-rw-   0        0        0     2974 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/clone.py
+-rw-rw-rw-   0        0        0     8586 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/commands.py
+-rw-rw-rw-   0        0        0     3175 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/commit.py
+-rw-rw-rw-   0        0        0      572 2023-04-21 21:10:02.000000 git-sim-0.3.2/git_sim/enums.py
+-rw-rw-rw-   0        0        0     2842 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/fetch.py
+-rw-rw-rw-   0        0        0    46330 2023-06-12 02:56:27.000000 git-sim-0.3.2/git_sim/git_sim_base_command.py
+-rw-rw-rw-   0        0        0     1415 2023-06-06 18:37:54.000000 git-sim-0.3.2/git_sim/log.py
+-rw-rw-rw-   0        0        0    63319 2023-03-09 07:57:17.000000 git-sim-0.3.2/git_sim/logo.png
+-rw-rw-rw-   0        0        0     7258 2023-06-12 02:56:27.000000 git-sim-0.3.2/git_sim/merge.py
+-rw-rw-rw-   0        0        0     2937 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/mv.py
+-rw-rw-rw-   0        0        0     3844 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/pull.py
+-rw-rw-rw-   0        0        0     7226 2023-04-21 21:10:02.000000 git-sim-0.3.2/git_sim/push.py
+-rw-rw-rw-   0        0        0     6057 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/rebase.py
+-rw-rw-rw-   0        0        0     5042 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/reset.py
+-rw-rw-rw-   0        0        0     2467 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/restore.py
+-rw-rw-rw-   0        0        0     5607 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/revert.py
+-rw-rw-rw-   0        0        0     4541 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/rm.py
+-rw-rw-rw-   0        0        0     1380 2023-04-21 20:23:21.000000 git-sim-0.3.2/git_sim/settings.py
+-rw-rw-rw-   0        0        0     6505 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/stash.py
+-rw-rw-rw-   0        0        0      829 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/status.py
+-rw-rw-rw-   0        0        0     4413 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/switch.py
+-rw-rw-rw-   0        0        0     1469 2023-04-21 20:10:26.000000 git-sim-0.3.2/git_sim/tag.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:56:59.254657 git-sim-0.3.2/git_sim.egg-info/
+-rw-rw-rw-   0        0        0    25490 2023-06-12 02:56:59.000000 git-sim-0.3.2/git_sim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      770 2023-06-12 02:56:59.000000 git-sim-0.3.2/git_sim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 02:56:59.000000 git-sim-0.3.2/git_sim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-06-12 02:56:59.000000 git-sim-0.3.2/git_sim.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       64 2023-06-12 02:56:59.000000 git-sim-0.3.2/git_sim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 02:56:59.000000 git-sim-0.3.2/git_sim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 02:56:59.256162 git-sim-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1468 2023-04-21 20:23:21.000000 git-sim-0.3.2/setup.py
```

### Comparing `git-sim-0.3.1/LICENSE` & `git-sim-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/PKG-INFO` & `git-sim-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-sim
-Version: 0.3.1
+Version: 0.3.2
 Summary: Simulate Git commands on your own repos by generating an image (default) or video visualization depicting the command's behavior.
 Home-page: https://initialcommit.com/tools/git-sim
 Author: Jacob Stopak
 Author-email: jacob@initialcommit.io
 Project-URL: Homepage, https://initialcommit.com/tools/git-sim
 Project-URL: Source, https://github.com/initialcommit-com/git-sim
 Keywords: git sim simulation simulate git-simulate git-simulation git-sim manim animation gitanimation image video dryrun dry-run
```

### Comparing `git-sim-0.3.1/README.md` & `git-sim-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/__main__.py` & `git-sim-0.3.2/git_sim/__main__.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/add.py` & `git-sim-0.3.2/git_sim/add.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/animations.py` & `git-sim-0.3.2/git_sim/animations.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/branch.py` & `git-sim-0.3.2/git_sim/branch.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/checkout.py` & `git-sim-0.3.2/git_sim/checkout.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/cherrypick.py` & `git-sim-0.3.2/git_sim/cherrypick.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/clean.py` & `git-sim-0.3.2/git_sim/clean.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/clone.py` & `git-sim-0.3.2/git_sim/clone.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/commands.py` & `git-sim-0.3.2/git_sim/commands.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/commit.py` & `git-sim-0.3.2/git_sim/commit.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/enums.py` & `git-sim-0.3.2/git_sim/enums.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/fetch.py` & `git-sim-0.3.2/git_sim/fetch.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/git_sim_base_command.py` & `git-sim-0.3.2/git_sim/git_sim_base_command.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/log.py` & `git-sim-0.3.2/git_sim/log.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/logo.png` & `git-sim-0.3.2/git_sim/logo.png`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/merge.py` & `git-sim-0.3.2/git_sim/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             )
             sys.exit(1)
 
         self.show_intro()
         head_commit = self.get_commit()
         branch_commit = self.get_commit(self.branch)
 
-        if not self.is_remote_tracking_branch(self.branch):
+        if self.branch not in self.get_remote_tracking_branches():
             if self.branch in self.repo.git.branch("--contains", head_commit.hexsha):
                 self.ff = True
         else:
             if self.branch in self.repo.git.branch(
                 "-r", "--contains", head_commit.hexsha
             ):
                 self.ff = True
```

### Comparing `git-sim-0.3.1/git_sim/mv.py` & `git-sim-0.3.2/git_sim/mv.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/pull.py` & `git-sim-0.3.2/git_sim/pull.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/push.py` & `git-sim-0.3.2/git_sim/push.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/rebase.py` & `git-sim-0.3.2/git_sim/rebase.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/reset.py` & `git-sim-0.3.2/git_sim/reset.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/restore.py` & `git-sim-0.3.2/git_sim/restore.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/revert.py` & `git-sim-0.3.2/git_sim/revert.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/rm.py` & `git-sim-0.3.2/git_sim/rm.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/settings.py` & `git-sim-0.3.2/git_sim/settings.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/stash.py` & `git-sim-0.3.2/git_sim/stash.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/status.py` & `git-sim-0.3.2/git_sim/status.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/switch.py` & `git-sim-0.3.2/git_sim/switch.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim/tag.py` & `git-sim-0.3.2/git_sim/tag.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/git_sim.egg-info/PKG-INFO` & `git-sim-0.3.2/git_sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-sim
-Version: 0.3.1
+Version: 0.3.2
 Summary: Simulate Git commands on your own repos by generating an image (default) or video visualization depicting the command's behavior.
 Home-page: https://initialcommit.com/tools/git-sim
 Author: Jacob Stopak
 Author-email: jacob@initialcommit.io
 Project-URL: Homepage, https://initialcommit.com/tools/git-sim
 Project-URL: Source, https://github.com/initialcommit-com/git-sim
 Keywords: git sim simulation simulate git-simulate git-simulation git-sim manim animation gitanimation image video dryrun dry-run
```

### Comparing `git-sim-0.3.1/git_sim.egg-info/SOURCES.txt` & `git-sim-0.3.2/git_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git-sim-0.3.1/setup.py` & `git-sim-0.3.2/setup.py`

 * *Files identical despite different names*

