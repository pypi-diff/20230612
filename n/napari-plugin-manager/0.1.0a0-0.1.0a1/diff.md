# Comparing `tmp/napari-plugin-manager-0.1.0a0.tar.gz` & `tmp/napari-plugin-manager-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-plugin-manager-0.1.0a0.tar", last modified: Thu May 11 11:42:58 2023, max compression
+gzip compressed data, was "napari-plugin-manager-0.1.0a1.tar", last modified: Mon Jun 12 09:06:56 2023, max compression
```

## Comparing `napari-plugin-manager-0.1.0a0.tar` & `napari-plugin-manager-0.1.0a1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jrodriguez   (501) staff       (20)        0 2023-05-11 11:42:58.432117 napari-plugin-manager-0.1.0a0/
-drwxr-xr-x   0 jrodriguez   (501) staff       (20)        0 2023-05-11 11:42:58.424381 napari-plugin-manager-0.1.0a0/.github/
-drwxr-xr-x   0 jrodriguez   (501) staff       (20)        0 2023-05-11 11:42:58.426157 napari-plugin-manager-0.1.0a0/.github/workflows/
--rw-r--r--   0 jrodriguez   (501) staff       (20)     3600 2023-05-11 11:41:03.000000 napari-plugin-manager-0.1.0a0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 jrodriguez   (501) staff       (20)      998 2023-04-25 10:45:36.000000 napari-plugin-manager-0.1.0a0/.gitignore
--rw-r--r--   0 jrodriguez   (501) staff       (20)      686 2023-04-25 10:45:36.000000 napari-plugin-manager-0.1.0a0/.pre-commit-config.yaml
--rw-r--r--   0 jrodriguez   (501) staff       (20)     1506 2023-04-25 10:45:36.000000 napari-plugin-manager-0.1.0a0/LICENSE
--rw-r--r--   0 jrodriguez   (501) staff       (20)     4652 2023-05-11 11:42:58.431717 napari-plugin-manager-0.1.0a0/PKG-INFO
--rw-r--r--   0 jrodriguez   (501) staff       (20)     1580 2023-05-11 11:41:03.000000 napari-plugin-manager-0.1.0a0/README.md
-drwxr-xr-x   0 jrodriguez   (501) staff       (20)        0 2023-05-11 11:42:58.427299 napari-plugin-manager-0.1.0a0/napari_plugin_manager/
--rw-r--r--   0 jrodriguez   (501) staff       (20)        0 2023-04-25 10:45:36.000000 napari-plugin-manager-0.1.0a0/napari_plugin_manager/__init__.py
-drwxr-xr-x   0 jrodriguez   (501) staff       (20)        0 2023-05-11 11:42:58.430402 napari-plugin-manager-0.1.0a0/napari_plugin_manager/_tests/
--rw-r--r--   0 jrodriguez   (501) staff       (20)        0 2023-04-25 10:45:36.000000 napari-plugin-manager-0.1.0a0/napari_plugin_manager/_tests/__init__.py
--rw-r--r--   0 jrodriguez   (501) staff       (20)      812 2023-05-11 11:41:03.000000 napari-plugin-manager-0.1.0a0/napari_plugin_manager/_tests/conftest.py
--rw-r--r--   0 jrodriguez   (501) staff       (20)     6781 2023-04-25 10:45:36.000000 napari-plugin-manager-0.1.0a0/napari_plugin_manager/_tests/test_installer_process.py
--rw-r--r--   0 jrodriguez   (501) staff       (20)    11644 2023-05-11 11:41:03.000000 napari-plugin-manager-0.1.0a0/napari_plugin_manager/_tests/test_qt_plugin_dialog.py
--rw-r--r--   0 jrodriguez   (501) staff       (20)      162 2023-05-11 11:42:58.000000 napari-plugin-manager-0.1.0a0/napari_plugin_manager/_version.py
--rw-r--r--   0 jrodriguez   (501) staff       (20)    18674 2023-04-25 10:45:36.000000 napari-plugin-manager-0.1.0a0/napari_plugin_manager/qt_package_installer.py
--rw-r--r--   0 jrodriguez   (501) staff       (20)    39782 2023-04-26 17:00:33.000000 napari-plugin-manager-0.1.0a0/napari_plugin_manager/qt_plugin_dialog.py
-drwxr-xr-x   0 jrodriguez   (501) staff       (20)        0 2023-05-11 11:42:58.429334 napari-plugin-manager-0.1.0a0/napari_plugin_manager.egg-info/
--rw-r--r--   0 jrodriguez   (501) staff       (20)     4652 2023-05-11 11:42:58.000000 napari-plugin-manager-0.1.0a0/napari_plugin_manager.egg-info/PKG-INFO
--rw-r--r--   0 jrodriguez   (501) staff       (20)      684 2023-05-11 11:42:58.000000 napari-plugin-manager-0.1.0a0/napari_plugin_manager.egg-info/SOURCES.txt
--rw-r--r--   0 jrodriguez   (501) staff       (20)        1 2023-05-11 11:42:58.000000 napari-plugin-manager-0.1.0a0/napari_plugin_manager.egg-info/dependency_links.txt
--rw-r--r--   0 jrodriguez   (501) staff       (20)       79 2023-05-11 11:42:58.000000 napari-plugin-manager-0.1.0a0/napari_plugin_manager.egg-info/requires.txt
--rw-r--r--   0 jrodriguez   (501) staff       (20)       22 2023-05-11 11:42:58.000000 napari-plugin-manager-0.1.0a0/napari_plugin_manager.egg-info/top_level.txt
--rw-r--r--   0 jrodriguez   (501) staff       (20)     5041 2023-05-11 11:41:03.000000 napari-plugin-manager-0.1.0a0/pyproject.toml
--rw-r--r--   0 jrodriguez   (501) staff       (20)       38 2023-05-11 11:42:58.432214 napari-plugin-manager-0.1.0a0/setup.cfg
--rw-r--r--   0 jrodriguez   (501) staff       (20)     1032 2023-05-11 11:41:03.000000 napari-plugin-manager-0.1.0a0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:06:56.535792 napari-plugin-manager-0.1.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:06:56.531792 napari-plugin-manager-0.1.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:06:56.531792 napari-plugin-manager-0.1.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-12 09:06:56.535792 napari-plugin-manager-0.1.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:06:56.531792 napari-plugin-manager-0.1.0a1/napari_plugin_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:06:56.535792 napari-plugin-manager-0.1.0a1/napari_plugin_manager/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager/_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager/_tests/test_installer_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager/_tests/test_qt_plugin_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 09:06:56.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18125 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager/qt_package_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39782 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager/qt_plugin_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:06:56.531792 napari-plugin-manager-0.1.0a1/napari_plugin_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-12 09:06:56.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-12 09:06:56.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:06:56.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-12 09:06:56.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 09:06:56.000000 napari-plugin-manager-0.1.0a1/napari_plugin_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 09:06:56.535792 napari-plugin-manager-0.1.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-12 09:06:45.000000 napari-plugin-manager-0.1.0a1/tox.ini
```

### Comparing `napari-plugin-manager-0.1.0a0/.github/workflows/test_and_deploy.yml` & `napari-plugin-manager-0.1.0a1/.github/workflows/test_and_deploy.yml`

 * *Files 21% similar despite different names*

```diff
@@ -83,25 +83,25 @@
   deploy:
     # this will run when you have tagged a commit, starting with "v*"
     # and requires that you have put your twine API key in your
     # github secrets (see readme for details)
     needs: [test]
     runs-on: ubuntu-latest
     if: contains(github.ref, 'tags')
+    permissions:
+      id-token: write
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install -U setuptools twine build
-      - name: Build and publish
-        env:
-          TWINE_USERNAME: __token__
-          TWINE_PASSWORD: ${{ secrets.TWINE_API_KEY }}
+          pip install -U setuptools build
+      - name: Build
         run: |
           git tag
           python -m build
-          twine upload dist/*
+      - name: Publish package distributions to PyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `napari-plugin-manager-0.1.0a0/.gitignore` & `napari-plugin-manager-0.1.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a0/.pre-commit-config.yaml` & `napari-plugin-manager-0.1.0a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a0/LICENSE` & `napari-plugin-manager-0.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a0/PKG-INFO` & `napari-plugin-manager-0.1.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-plugin-manager
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Install plugins for napari, in napari.
 Author-email: napari team <napari-steering-council@googlegroups.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2018, Napari
         All rights reserved.
```

### Comparing `napari-plugin-manager-0.1.0a0/README.md` & `napari-plugin-manager-0.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a0/napari_plugin_manager/_tests/conftest.py` & `napari-plugin-manager-0.1.0a1/napari_plugin_manager/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a0/napari_plugin_manager/_tests/test_installer_process.py` & `napari-plugin-manager-0.1.0a1/napari_plugin_manager/_tests/test_installer_process.py`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a0/napari_plugin_manager/_tests/test_qt_plugin_dialog.py` & `napari-plugin-manager-0.1.0a1/napari_plugin_manager/_tests/test_qt_plugin_dialog.py`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a0/napari_plugin_manager/qt_package_installer.py` & `napari-plugin-manager-0.1.0a1/napari_plugin_manager/qt_package_installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 from tempfile import gettempdir, mkstemp
 from typing import Deque, Optional, Sequence, Tuple
 
 from napari._version import version as _napari_version
 from napari._version import version_tuple as _napari_version_tuple
 from napari.plugins import plugin_manager
 from napari.plugins.npe2api import _user_agent
-from napari.utils._appdirs import user_plugin_dir, user_site_packages
-from napari.utils.misc import StringEnum, running_as_bundled_app
+from napari.utils.misc import StringEnum
 from napari.utils.translations import trans
 from npe2 import PluginManager
 from qtpy.QtCore import QObject, QProcess, QProcessEnvironment, Signal
 from qtpy.QtWidgets import QTextEdit
 
 JobId = int
 log = getLogger(__name__)
@@ -81,15 +80,15 @@
         raise NotImplementedError
 
     @staticmethod
     def constraints() -> Sequence[str]:
         """
         Version constraints to limit unwanted changes in installation.
         """
-        return [f"napari=={_napari_version}"]
+        return [f"napari=={_napari_version}", "pydantic<2"]
 
     @classmethod
     def available(cls) -> bool:
         """
         Check if the tool is available by performing a little test
         """
         raise NotImplementedError
@@ -123,36 +122,21 @@
             args += ['uninstall', '-y']
         else:
             raise ValueError(f"Action '{self.action}' not supported!")
         if 10 <= log.getEffectiveLevel() < 30:  # DEBUG level
             args.append('-vvv')
         if self.prefix is not None:
             args.extend(['--prefix', str(self.prefix)])
-        elif running_as_bundled_app(
-            check_conda=False
-        ) and sys.platform.startswith('linux'):
-            args += [
-                '--no-warn-script-location',
-                '--prefix',
-                user_plugin_dir(),
-            ]
         return (*args, *self.pkgs)
 
     def environment(
         self, env: QProcessEnvironment = None
     ) -> QProcessEnvironment:
         if env is None:
             env = QProcessEnvironment.systemEnvironment()
-        combined_paths = os.pathsep.join(
-            [
-                user_site_packages(),
-                env.systemEnvironment().value("PYTHONPATH"),
-            ]
-        )
-        env.insert("PYTHONPATH", combined_paths)
         env.insert("PIP_USER_AGENT_USER_DATA", _user_agent())
         return env
 
     @classmethod
     @lru_cache(maxsize=0)
     def _constraints_file(cls) -> str:
         _, path = mkstemp("-napari-constraints.txt", text=True)
@@ -226,15 +210,15 @@
         # in the remote index, only locally; to work around this bug
         # we will have to pin to e.g. 0.4.* instead of 0.4.17.* for now
         version_lower = _napari_version.lower()
         is_dev = "rc" in version_lower or "dev" in version_lower
         pin_level = 2 if is_dev else 3
         version = ".".join([str(x) for x in _napari_version_tuple[:pin_level]])
 
-        return [f"napari={version}"]
+        return [f"napari={version}", "pydantic<2.0a0"]
 
     def _add_constraints_to_env(
         self, env: QProcessEnvironment
     ) -> QProcessEnvironment:
         PINNED = 'CONDA_PINNED_PACKAGES'
         constraints = self.constraints()
         if env.contains(PINNED):
```

### Comparing `napari-plugin-manager-0.1.0a0/napari_plugin_manager/qt_plugin_dialog.py` & `napari-plugin-manager-0.1.0a1/napari_plugin_manager/qt_plugin_dialog.py`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a0/napari_plugin_manager.egg-info/PKG-INFO` & `napari-plugin-manager-0.1.0a1/napari_plugin_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-plugin-manager
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Install plugins for napari, in napari.
 Author-email: napari team <napari-steering-council@googlegroups.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2018, Napari
         All rights reserved.
```

### Comparing `napari-plugin-manager-0.1.0a0/napari_plugin_manager.egg-info/SOURCES.txt` & `napari-plugin-manager-0.1.0a1/napari_plugin_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a0/pyproject.toml` & `napari-plugin-manager-0.1.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-plugin-manager-0.1.0a0/tox.ini` & `napari-plugin-manager-0.1.0a1/tox.ini`

 * *Files identical despite different names*

