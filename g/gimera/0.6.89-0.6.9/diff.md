# Comparing `tmp/gimera-0.6.89.tar.gz` & `tmp/gimera-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimera-0.6.89.tar", last modified: Mon Jun 12 21:15:24 2023, max compression
+gzip compressed data, was "gimera-0.6.9.tar", last modified: Fri Jul  8 21:48:00 2022, max compression
```

## Comparing `gimera-0.6.89.tar` & `gimera-0.6.9.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:15:24.851783 gimera-0.6.89/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-12 21:14:37.000000 gimera-0.6.89/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-12 21:15:24.851783 gimera-0.6.89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-12 21:14:37.000000 gimera-0.6.89/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:15:24.847782 gimera-0.6.89/gimera/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-12 21:14:37.000000 gimera-0.6.89/gimera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-12 21:14:37.000000 gimera-0.6.89/gimera/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-12 21:14:37.000000 gimera-0.6.89/gimera/consts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    38290 2023-06-12 21:14:37.000000 gimera-0.6.89/gimera/gimera.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-12 21:14:37.000000 gimera-0.6.89/gimera/gitcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-12 21:14:37.000000 gimera-0.6.89/gimera/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-12 21:14:37.000000 gimera-0.6.89/gimera/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:15:24.851783 gimera-0.6.89/gimera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-12 21:15:24.000000 gimera-0.6.89/gimera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-12 21:15:24.000000 gimera-0.6.89/gimera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:15:24.000000 gimera-0.6.89/gimera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-12 21:15:24.000000 gimera-0.6.89/gimera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-12 21:15:24.000000 gimera-0.6.89/gimera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 21:15:24.000000 gimera-0.6.89/gimera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-12 21:15:24.851783 gimera-0.6.89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-12 21:14:37.000000 gimera-0.6.89/setup.py
+drwxr-xr-x   0 marcwimmer   (501) staff       (20)        0 2022-07-08 21:48:00.943252 gimera-0.6.9/
+-rw-r--r--   0 marcwimmer   (501) staff       (20)     1068 2021-07-26 15:49:47.000000 gimera-0.6.9/LICENSE.txt
+-rw-r--r--   0 marcwimmer   (501) staff       (20)     2317 2022-07-08 21:48:00.943340 gimera-0.6.9/PKG-INFO
+-rw-r--r--   0 marcwimmer   (501) staff       (20)     1978 2022-07-05 06:37:51.000000 gimera-0.6.9/README.md
+drwxr-xr-x   0 marcwimmer   (501) staff       (20)        0 2022-07-08 21:48:00.923126 gimera-0.6.9/gimera/
+-rw-r--r--   0 marcwimmer   (501) staff       (20)      112 2022-07-05 17:42:31.000000 gimera-0.6.9/gimera/__init__.py
+-rwxr-xr-x   0 marcwimmer   (501) staff       (20)    23463 2022-07-08 21:47:57.000000 gimera-0.6.9/gimera/gimera.py
+-rw-r--r--   0 marcwimmer   (501) staff       (20)     4029 2022-07-08 13:35:42.000000 gimera-0.6.9/gimera/gitcommands.py
+-rw-r--r--   0 marcwimmer   (501) staff       (20)     8956 2022-07-08 13:35:42.000000 gimera-0.6.9/gimera/repo.py
+-rw-r--r--   0 marcwimmer   (501) staff       (20)     1138 2022-07-08 13:35:42.000000 gimera-0.6.9/gimera/tools.py
+drwxr-xr-x   0 marcwimmer   (501) staff       (20)        0 2022-07-08 21:48:00.943026 gimera-0.6.9/gimera.egg-info/
+-rw-r--r--   0 marcwimmer   (501) staff       (20)     2317 2022-07-08 21:48:00.000000 gimera-0.6.9/gimera.egg-info/PKG-INFO
+-rw-r--r--   0 marcwimmer   (501) staff       (20)      311 2022-07-08 21:48:00.000000 gimera-0.6.9/gimera.egg-info/SOURCES.txt
+-rw-r--r--   0 marcwimmer   (501) staff       (20)        1 2022-07-08 21:48:00.000000 gimera-0.6.9/gimera.egg-info/dependency_links.txt
+-rw-r--r--   0 marcwimmer   (501) staff       (20)       45 2022-07-08 21:48:00.000000 gimera-0.6.9/gimera.egg-info/entry_points.txt
+-rw-r--r--   0 marcwimmer   (501) staff       (20)       29 2022-07-08 21:48:00.000000 gimera-0.6.9/gimera.egg-info/requires.txt
+-rw-r--r--   0 marcwimmer   (501) staff       (20)        7 2022-07-08 21:48:00.000000 gimera-0.6.9/gimera.egg-info/top_level.txt
+-rw-r--r--   0 marcwimmer   (501) staff       (20)      396 2022-07-08 21:48:00.947265 gimera-0.6.9/setup.cfg
+-rw-r--r--   0 marcwimmer   (501) staff       (20)     3834 2022-07-08 13:35:42.000000 gimera-0.6.9/setup.py
```

### Comparing `gimera-0.6.89/LICENSE.txt` & `gimera-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gimera-0.6.89/README.md` & `gimera-0.6.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: gimera
+Version: 0.6.9
+Summary: Handling git submodules and patches per yml
+Home-page: https://github.com/marcwimmer/gimera
+Author: Marc-Christian Wimmer
+Author-email: marc@itewimmer.de
+License: MIT
+Platform: UNKNOWN
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
 # Welcome to GIMERA
 
 Advanced handling of submodules by integrating them or handling as submodules as you know
 but provide auto merge functions of hotfixes from other repositories or inside.
 
 Rule of thumb:
 
@@ -11,51 +25,41 @@
 During run of gimera commits are done for example after pulling submodules or updating
 local paths.
 
 
 ## How to install:
 
 ```bash
-pipx install gimera
-gimera completion  (Follow instructions)
+pip install gimera
 ```
 
 
 
 ## How to use:
 
 Put gimera.yml into your root folder of your project:
 
 ```yaml
-common:
-  vars:
-    VERSION: '15.0'
 repos:
     # make ordinary git submodule:
     - url: "https://github.com/foo/bar"
-      branch: branch1_${VERSION}
+      branch: branch1
       path: roles/sub1
       patches: []
       type: submodule
 
-      # default True
-      enabled: True
-
 
     # instead of submodule put the content directly in the repository;
     # apply patches from local git repository
     - url: "https://github.com/foo/bar"
       branch: branch1
       path: roles2/sub1
       patches:
           - 'roles2/sub1_patches'
       type: integrated
-      ignored_patchfiles:
-        - file1.patch
-        - roles2/sub1_patches/file1.patch
 
     # apply patches from another remote repository
     #
     - url: "https://github.com/foo/bar"
       branch: branch1
       path: roles2/sub1
       remotes:
@@ -83,98 +87,33 @@
 
 ```bash
 gimera apply
 ```
 
 Then a patch file is created as suggestion in roles2/sub1_patches which you may commit and push.
 
-### Re-Edit patch file:
-
-```bash
-gimera edit-patch file1.patch file2.patch
-```
-
-  * by this, you can combine several patch files into one again
-
-
 ## How to fetch only one or more repo:
 
 ```bash
 gimera apply repo_path repo_path2 repo_path3`
 ```
 ## How to fetch latest versions:
 
 ```bash
 gimera apply --update
 ```
 
 Latest versions are pulled and patches are applied.
 
-## Force Integrated or Submodule mode for repo and subrepositories
-
-Use Case: you have an integrated repository. Now you want to turn it into submodule,
-to easily commit and push changes. Then you do:
-
-```bash
-gimera apply <path> -S
-```
-
-Now although it is configured as integrated, it is now a submodule.
-
-After that you can go back to default settings or force integrated mode.
-You should call update to pull the latest version.
-
-```bash
-gimera apply <path> -I --update
-```
-
-## Recursive setup
-
-If you have your tools in git submodules and depending where you add your modules
-specific patches have to be applied, you can use the following structure. A concrete
-use case is for example odoo and using sub modules.
-
-So instead of creating a branch for 13.0 / 14.0 / 15.0 / 16.0 you just create the
-main branch and working on version 14.0 for example. Then you create patch dirs
-for each version.
-
-In the submodule:
-```yaml
-gimera.yml
-
-common:
-  patches:
-    - patches/${VERSION}
-
-```
-
-The main gimera which integrates the submodule should be:
-```yaml
-common:
-  vars:
-    VERSION: 15.0
-repos:
-  type: integrated
-  url: .....
-  path: sub1
-```
-
-After that a recursive gimera is required.
-```
-gimera apply -r
-```
-
-# Demo Videos
-
-## Edit existing patch file and update it
-
 
 ## Contributors
   * Michael Tietz (mtietz@mt-software.de)
   * Walter Saltzmann
 
 
 ## install directly
 
 ```bash
 pip install git+https://github.com/marcwimmer/gimera
-```
+```
+
+
```

### Comparing `gimera-0.6.89/gimera/gitcommands.py` & `gimera-0.6.9/gimera/gitcommands.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,30 +4,26 @@
 
 
 class GitCommands(object):
     def __init__(self, path=None):
         self.path = Path(path or os.getcwd())
 
     @property
-    def configdir(self):
-        from .repo import Repo
+    def resolved_git_dir(self):
+        #if .git is a path pointing to the real dir
+        import pudb;pudb.set_trace()
 
-        stop_at = Repo(self.path).root_repo
-        here = self.path
-        while True:
-            default = here / ".git"
-            if default.exists() and default.is_dir():
-                return default
-            if default.is_file():
-                path = default.read_text().strip().split("gitdir:")[1].strip()
-                return (here / path).resolve()
-
-            if here == stop_at:
-                break
-            here = here.parent
+    @property
+    def configdir(self):
+        default = self.path / '.git'
+        if default.exists() and default.is_dir():
+            return default
+        if default.is_file():
+            path = default.read_text().strip().split("gitdir:")[1].strip()
+            return (self.path / path).resolve()
         raise Exception("Config dir not found")
 
     def X(self, *params, allow_error=False):
         return X(*params, output=False, cwd=self.path, allow_error=allow_error)
 
     def out(self, *params, allow_error=False):
         return X(*params, output=True, cwd=self.path, allow_error=allow_error)
@@ -46,16 +42,15 @@
             #          M  asdsad
             #         ??  asasdasd
             modifier = line[:2]
             path = line.strip().split(" ", 1)[1]
             if path.startswith(".."):
                 continue
             path = Path(path.strip())
-            parent_path = getattr(self, "parent_path", None)
-            if parent_path:
+            if parent_path := getattr(self, "parent_path", None):
                 path = parent_path / path
             else:
                 path = self.path / path
             if safe_relative_to(path, self.path):
                 yield modifier, path
 
     @property
@@ -134,8 +129,8 @@
         self.X("git", "commit", "-am", msg)
 
     @property
     def hex(self):
         return self.out("git", "log", "-n", "1", "--pretty=%H")
 
     def checkout(self, ref, force=False):
-        self.X("git", "checkout", "-f" if force else None, ref)
+        self.X("git", "checkout", "-f" if force else None, ref)
```

### Comparing `gimera-0.6.89/gimera/repo.py` & `gimera-0.6.9/gimera/repo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import subprocess
-import click
 import shutil
 from .gitcommands import GitCommands
 from pathlib import Path
-from .tools import yieldlist, X, safe_relative_to, _raise_error, rmtree
-from .consts import gitcmd as git
+from .tools import yieldlist, X, safe_relative_to, _raise_error
 
 
 class Repo(GitCommands):
     def __init__(self, path):
         self.path = Path(path)
         self.working_dir = Path(path)
 
@@ -29,51 +27,17 @@
         for i in path.parts:
             if (path / ".git").is_dir():
                 return Repo(path)
             path = path.parent
         else:
             return None
 
-    @property
-    def _git_path(self):
-        return self.path / ".git"
-
-    def ls_files_states(self, params):
-        """
-        e.g. ls_files_states("-dmosk" )
-        """
-        if "-t" not in params:
-            params += ["-t"]
-
-        def extract(line):
-            if "\t" in line:
-                return line.split("\t")[-1]
-            return line[2:]
-
-        files = list(
-            map(
-                lambda line: Path(extract(line)),
-                self.out(*(["git", "ls-files"] + params)).splitlines(),
-            )
-        )
-        return files
-
     def force_remove_submodule(self, path):
         # https://github.com/jeremysears/scripts/blob/master/bin/git-submodule-rewrite
         self.please_no_staged_files()
-
-        # if there are dirty files, then abort to not destroy data
-        dirty_files = self.ls_files_states(["-dmok"])
-        dirty_files = list(
-            filter(
-                lambda file: not file.is_dir()
-                and safe_relative_to(self.path / file, self.path / path),
-                dirty_files,
-            )
-        )
         fullpath = self.path / path
         if fullpath.exists():
             self.X(
                 "git",
                 "config",
                 "-f",
                 ".gitmodules",
@@ -101,41 +65,43 @@
 
         subrepo = Repo(self.path / path)
         self.X("rm", "-rf", path)
         if fullpath.exists():
             self.X("git", "add", "-A", path)
         if self.lsfiles(fullpath.relative_to(self.path)):
             self.X("git", "add", "-A", path)
-        if (self.path / ".gitmodules") in self.all_dirty_files:
+        if (self.path / '.gitmodules') in self.all_dirty_files:
             self.X("git", "add", "-A", ".gitmodules")
 
         if self.staged_files:
             self.X("git", "commit", "-m", f"removed submodule {path}")
         self.X("rm", "-rf", f".git/modules/{subrepo.rel_path_to_root_repo}")
 
     @property
     def next_module_root(self):
         if not self.path.exists():
             return None
 
         p = self.path
         for i in range(len(p.parts)):
-            if (p / ".git").exists():
+            if (p / ".gitmodules").exists():
+                return p
+            if (p / ".git").is_dir():
                 return p
             p = p.parent
         return self.path
 
     @yieldlist
     def get_submodules(self):
-        submodules = self.out("git", "submodule", "status").splitlines()
+        submodules = self.out("git", "submodule--helper", "list").splitlines()
         for line in submodules:
-            splitted = line.strip().split(" ")
-            yield Submodule(self.next_module_root / splitted[1], self.next_module_root)
+            splitted = line.strip().split("\t", 3)
+            yield Submodule(self.next_module_root / splitted[-1], self.next_module_root)
 
-    def _fix_to_remove_subdirectories(self, config):
+    def _fix_to_remove_subdirectories(self):
         # https://stackoverflow.com/questions/4185365/no-submodule-mapping-found-in-gitmodule-for-a-path-thats-not-a-submodule
         # commands may block
         # git submodule--helper works and shows something
         # git submodule says: fatal: no submodule mapping found in .gitmodules
         # there is special folder with id 16000 then, then must be removed with git rm
         # then; not tested, because then it suddenly worked
         lines = [
@@ -144,22 +110,14 @@
             if x.strip().startswith("160000")
         ]
         # 160000 5e8add9536e584f73ea25d4cf51577832d480e90 0       addons_robot
         for line in lines:
             linepath = line.split("\t", 1)[1]
             path = self.path / linepath
             if path.exists():
-                from .gimera import REPO_TYPE_SUB
-
-                if not [
-                    x
-                    for x in config.repos
-                    if x.path == path and x.ttype == REPO_TYPE_SUB
-                ]:
-                    continue
                 self.please_no_staged_files()
                 # if .gitmodules is dirty then commit that first, otherwise:
                 # fatal: please stage your changes to .gitmodules or stash them to proceed
                 if (self.path / ".gitmodules") in self.all_dirty_files:
                     self.X("git", "add", ".gitmodules")
                     self.X(
                         "git",
@@ -187,47 +145,23 @@
 
     def remove_remote(self, remote):
         self.X("git", "remote", "rm", remote and remote.name or None)
 
     def add_remote(self, repo):
         self.X("git", "remote", "add", repo.name, repo.url)
 
-    def pull(self, remote=None, ref=None, repo_yml=None):
-        """
-        The git reset hard way was necessary in a live repository; local files
-        had to be overridden that stand in the way
-
-        This was too weak:
+    def pull(self, remote=None, ref=None):
         self.X("git", "pull", "--no-edit", remote and remote.name or None, ref)
 
-
-        "params remote": remote object
-
-        """
-        if repo_yml:
-            assert not remote
-            assert not ref
-            remote = "origin"
-            ref = repo_yml.branch
-
-        if remote and not isinstance(remote, str):
-            remote = remote.name
-
-        if not remote and not ref:
-            raise Exception("Requires remote and ref or yaml configuration.")
-
-        self.X("git", "pull", "--no-edit", "--no-rebase", remote, ref)
-
     def full_clean(self):
         self.X("git", "checkout", "-f")
         self.X("git", "clean", "-xdff")
 
     def please_no_staged_files(self):
-        staged = self.staged_files
-        if not staged:
+        if not (staged := self.staged_files):
             return
         _raise_error(
             "For the operation there mustnt be " f"any staged files like {staged}"
         )
 
     @property
     @yieldlist
@@ -274,85 +208,25 @@
             self.X("git", "clean", "-fd", self.path / check)
             if not safe_relative_to(check, dont_go_beyond):
                 break
             if not check.exists():
                 check = check.parent
                 continue
             if not list(check.iterdir()):
-                rmtree(check)
+                shutil.rmtree(check)
             check = check.parent
             if not safe_relative_to(check, self.path):
                 break
 
     def lsfiles(self, path):
         files = list(
             map(lambda x: Path(x), self.out("git", "ls-files", path).splitlines())
         )
         return files
 
-    def commit_dir_if_dirty(self, rel_path, commit_msg):
-        # commit updated directories
-        if any(
-            map(
-                lambda filepath: safe_relative_to(filepath, self.path / rel_path),
-                self.all_dirty_files,
-            )
-        ):
-            self.X("git", "add", rel_path)
-            # if there are no staged files, it can be, that below that, there is a
-            # submodule which changed files; then after git add it is not added
-            if self.staged_files:
-                self.X(
-                    "git",
-                    "commit",
-                    "-m",
-                    commit_msg,
-                )
-
-    def submodule_add(self, branch, url, rel_path):
-        commands = git + [
-            "submodule",
-            "add",
-            "--force",
-            "-b",
-            str(branch),
-            url,
-            rel_path,
-        ]
-        try:
-            self.out(*commands)
-        except subprocess.CalledProcessError:
-            self._remove_internal_submodule_clone(self.rel_path_to_root_repo / rel_path)
-            if (self.path / rel_path).exists():
-                rmtree(self.path / rel_path)
-            self.out(*commands)
-
-    def _remove_internal_submodule_clone(self, rel_path_to_root):
-        repo = self.root_repo
-        root = repo.path / ".git" / "modules"
-        parts = list(rel_path_to_root.parts)
-        while parts:
-            part = parts.pop(0)
-            if not parts:
-                # kill
-                next_path = root / part
-                if next_path.exists():
-                    rmtree(next_path)
-                else:
-                    _raise_error(
-                        f"Could not delete submodule {part} in {root} - not found"
-                    )
-
-            else:
-                next_path = root / part / "modules"
-                if next_path.exists():
-                    root = next_path
-                else:
-                    _raise_error(f"Could not find submodule in .git for {part}")
-
 
 class Remote(object):
     def __init__(self, repo, name, url):
         self.repo = repo
         self.name = name
         self.url = url
```

