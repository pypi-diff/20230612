# Comparing `tmp/jupyterlab_genv-0.2.0.tar.gz` & `tmp/jupyterlab_genv-0.3.0.tar.gz`

## Comparing `jupyterlab_genv-0.2.0.tar` & `jupyterlab_genv-0.3.0.tar`

### file list

```diff
@@ -1,53 +1,52 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/.eslintrc.js
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/.stylelintrc
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/MANIFEST.in
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/TODO.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/Test.ipynb
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/install.json
--rw-r--r--   0        0        0   328793 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/package-lock.json
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/tsconfig.json
--rw-r--r--   0        0        0   258893 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/yarn.lock
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyter-config/nb-config/jupyterlab_genv.json
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyter-config/server-config/jupyterlab_genv.json
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/__init__.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/__main__.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/_version.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/genv_provisioner.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/handlers.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/genv/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/genv/control.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/genv/devices.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/genv/envs.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/genv/installation.py
--rw-r--r--   0        0        0    20565 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/build_log.json
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/package.json
--rw-r--r--   0        0        0    18782 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/lib_index_js.ff60ebd71c9a48ac429f.js
--rw-r--r--   0        0        0    16241 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/lib_index_js.ff60ebd71c9a48ac429f.js.map
--rw-r--r--   0        0        0    28617 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/remoteEntry.620874b13a1cfcb8a98e.js
--rw-r--r--   0        0        0    27387 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/remoteEntry.620874b13a1cfcb8a98e.js.map
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/style.js
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/style_index_js.584bbd372a8c350b76d6.js
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/style_index_js.584bbd372a8c350b76d6.js.map
--rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f136769aaa598352c213.js
--rw-r--r--   0        0        0    13793 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f136769aaa598352c213.js.map
--rw-r--r--   0        0        0   844987 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/resources/readme/activate.gif
--rw-r--r--   0        0        0  1589295 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/resources/readme/attach.gif
--rw-r--r--   0        0        0    40559 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/resources/readme/commands.gif
--rw-r--r--   0        0        0  1278811 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/resources/readme/overview.gif
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/src/dialogs.tsx
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/src/handler.ts
--rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/src/index.tsx
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/style/index.js
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/.gitignore
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/LICENSE
--rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/README.md
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    11808 2020-02-02 00:00:00.000000 jupyterlab_genv-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/.eslintrc.js
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/.stylelintrc
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/MANIFEST.in
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/TODO.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/Test.ipynb
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/install.json
+-rw-r--r--   0        0        0   328793 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/package-lock.json
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/tsconfig.json
+-rw-r--r--   0        0        0   258893 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/yarn.lock
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyter-config/nb-config/jupyterlab_genv.json
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyter-config/server-config/jupyterlab_genv.json
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/__init__.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/__main__.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/_version.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/genv_provisioner.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/handlers.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/genv/__init__.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/genv/control.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/genv/devices.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/genv/envs.py
+-rw-r--r--   0        0        0    20565 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/build_log.json
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/package.json
+-rw-r--r--   0        0        0    18782 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/static/lib_index_js.ff60ebd71c9a48ac429f.js
+-rw-r--r--   0        0        0    16241 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/static/lib_index_js.ff60ebd71c9a48ac429f.js.map
+-rw-r--r--   0        0        0    28617 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/static/remoteEntry.620874b13a1cfcb8a98e.js
+-rw-r--r--   0        0        0    27387 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/static/remoteEntry.620874b13a1cfcb8a98e.js.map
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/static/style.js
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/static/style_index_js.584bbd372a8c350b76d6.js
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/static/style_index_js.584bbd372a8c350b76d6.js.map
+-rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f136769aaa598352c213.js
+-rw-r--r--   0        0        0    13793 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f136769aaa598352c213.js.map
+-rw-r--r--   0        0        0   844987 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/resources/readme/activate.gif
+-rw-r--r--   0        0        0  1589295 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/resources/readme/attach.gif
+-rw-r--r--   0        0        0    40559 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/resources/readme/commands.gif
+-rw-r--r--   0        0        0  1278811 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/resources/readme/overview.gif
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/src/dialogs.tsx
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/src/handler.ts
+-rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/src/index.tsx
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/style/index.js
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/LICENSE
+-rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/README.md
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 jupyterlab_genv-0.3.0/PKG-INFO
```

### Comparing `jupyterlab_genv-0.2.0/.eslintrc.js` & `jupyterlab_genv-0.3.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/CHANGELOG.md` & `jupyterlab_genv-0.3.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.3.0] - 2023-06-12
+
+### Changed
+
+- Using Genv 1.0.0 APIs.
+
 ## [0.2.0] - 2023-04-30
 
 ### Changed
 
-- Using updated command `genv-devices find`.
+- Using renamed command `genv-devices find`.
 
 ## [0.1.2] - 2022-12-11
 
 ### Changed
 
 - Initializing spawned terminals using `eval "$(genv init -)"`.
```

### Comparing `jupyterlab_genv-0.2.0/TODO.md` & `jupyterlab_genv-0.3.0/TODO.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/Test.ipynb` & `jupyterlab_genv-0.3.0/Test.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/package-lock.json` & `jupyterlab_genv-0.3.0/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'version'": "'0.3.0'"}*

```diff
@@ -8077,9 +8077,9 @@
             "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
             "version": "0.1.0"
         }
     },
     "lockfileVersion": 1,
     "name": "jupyterlab_genv",
     "requires": true,
-    "version": "0.2.0"
+    "version": "0.3.0"
 }
```

### Comparing `jupyterlab_genv-0.2.0/package.json` & `jupyterlab_genv-0.3.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.3.0'"}*

```diff
@@ -108,9 +108,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.3.0"
 }
```

### Comparing `jupyterlab_genv-0.2.0/tsconfig.json` & `jupyterlab_genv-0.3.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/yarn.lock` & `jupyterlab_genv-0.3.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/jupyterlab_genv/__init__.py` & `jupyterlab_genv-0.3.0/jupyterlab_genv/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/jupyterlab_genv/__main__.py` & `jupyterlab_genv-0.3.0/jupyterlab_genv/__main__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/jupyterlab_genv/genv_provisioner.py` & `jupyterlab_genv-0.3.0/jupyterlab_genv/genv_provisioner.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/jupyterlab_genv/handlers.py` & `jupyterlab_genv-0.3.0/jupyterlab_genv/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/jupyterlab_genv/genv/devices.py` & `jupyterlab_genv-0.3.0/jupyterlab_genv/genv/devices.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, List
 
 from . import control
 
 async def _exec(command: str) -> str:
-    return await control.exec(f'exec devices {command}')
+    return await control.exec(f'devices {command}')
 
 async def ps() -> Dict:
     stdout = await _exec("ps --format csv --no-header --timestamp")
     lines = [line for line in stdout.splitlines() if len(line)]
 
     infos = []
```

### Comparing `jupyterlab_genv-0.2.0/jupyterlab_genv/genv/envs.py` & `jupyterlab_genv-0.3.0/jupyterlab_genv/genv/envs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from typing import Dict, List
 
 from . import control
 
 async def _exec(command: str) -> str:
-    return await control.exec(f'exec envs {command}')
+    return await control.exec(f'envs {command}')
 
 async def activate(eid: str, kernel_id: str) -> None:
     await _exec(f'activate --eid {eid} --uid {os.getuid()} --kernel-id {kernel_id}')
 
 async def find(kernel_id: str) -> str:
     return await _exec(f'find --kernel-id {kernel_id}')
```

### Comparing `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/build_log.json` & `jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/build_log.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/package.json` & `jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/lib_index_js.ff60ebd71c9a48ac429f.js` & `jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/static/lib_index_js.ff60ebd71c9a48ac429f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/lib_index_js.ff60ebd71c9a48ac429f.js.map` & `jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/static/lib_index_js.ff60ebd71c9a48ac429f.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/remoteEntry.620874b13a1cfcb8a98e.js` & `jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/static/remoteEntry.620874b13a1cfcb8a98e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/remoteEntry.620874b13a1cfcb8a98e.js.map` & `jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/static/remoteEntry.620874b13a1cfcb8a98e.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/style_index_js.584bbd372a8c350b76d6.js` & `jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/static/style_index_js.584bbd372a8c350b76d6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/style_index_js.584bbd372a8c350b76d6.js.map` & `jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/static/style_index_js.584bbd372a8c350b76d6.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f136769aaa598352c213.js` & `jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f136769aaa598352c213.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/jupyterlab_genv/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f136769aaa598352c213.js.map` & `jupyterlab_genv-0.3.0/jupyterlab_genv/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f136769aaa598352c213.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/resources/readme/activate.gif` & `jupyterlab_genv-0.3.0/resources/readme/activate.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/resources/readme/attach.gif` & `jupyterlab_genv-0.3.0/resources/readme/attach.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/resources/readme/commands.gif` & `jupyterlab_genv-0.3.0/resources/readme/commands.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/resources/readme/overview.gif` & `jupyterlab_genv-0.3.0/resources/readme/overview.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/src/dialogs.tsx` & `jupyterlab_genv-0.3.0/src/dialogs.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/src/handler.ts` & `jupyterlab_genv-0.3.0/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/src/index.tsx` & `jupyterlab_genv-0.3.0/src/index.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/.gitignore` & `jupyterlab_genv-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/LICENSE` & `jupyterlab_genv-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/README.md` & `jupyterlab_genv-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_genv-0.2.0/pyproject.toml` & `jupyterlab_genv-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling>=1.3.1", "jupyterlab~=3.1"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyterlab_genv"
-version = "0.2.0"
+version = "0.3.0"
 description = "A JupyterLab extension for managing GPU environments using genv."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 authors = [
     { name = "Raz Rotenberg", email = "raz.rotenberg@gmail.com" },
 ]
@@ -24,14 +24,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
+    "genv",
     "jupyter_server>=1.6,<2"
 ]
 
 [project.optional-dependencies]
 test = [
 ]
 
@@ -77,15 +78,15 @@
 file = [
     { src = "pyproject.toml", version_template = "version = \"{major}.{minor}.{patch}{channel}{release}\"" },
     { src = "jupyterlab_genv/_version.py" },
     { src = "package.json" },
 ]
 
 [tool.tbump.version]
-current = "0.2.0"
+current = "0.3.0"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [project.entry-points."jupyter_client.kernel_provisioners"]
```

### Comparing `jupyterlab_genv-0.2.0/PKG-INFO` & `jupyterlab_genv-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_genv
-Version: 0.2.0
+Version: 0.3.0
 Summary: A JupyterLab extension for managing GPU environments using genv.
 Project-URL: Homepage, https://github.com/run-ai/jupyterlab_genv
 Author-email: Raz Rotenberg <raz.rotenberg@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Raz Rotenberg
         All rights reserved.
@@ -44,14 +44,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
+Requires-Dist: genv
 Requires-Dist: jupyter-server<2,>=1.6
 Provides-Extra: test
 Description-Content-Type: text/markdown
 
 # GPU Environment Management for JupyterLab [![Join the community at https://join.slack.com/t/genvcommunity/shared_invite/zt-1i70tphdc-DmFgK5yr3HFI8Txx1yFXBw](https://img.shields.io/badge/Slack-genv-ff007f?logo=slack)](https://join.slack.com/t/genvcommunity/shared_invite/zt-1i70tphdc-DmFgK5yr3HFI8Txx1yFXBw) [![Join the chat at https://gitter.im/run-ai-genv/community](https://badges.gitter.im/run-ai-genv/community.svg)](https://gitter.im/run-ai-genv/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 [![Github Actions Status](https://github.com/run-ai/jupyterlab_genv/workflows/Build/badge.svg)](https://github.com/run-ai/jupyterlab_genv/actions/workflows/build.yml)
```

