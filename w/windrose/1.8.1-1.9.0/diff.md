# Comparing `tmp/windrose-1.8.1.tar.gz` & `tmp/windrose-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windrose-1.8.1.tar", last modified: Wed Dec 21 00:07:17 2022, max compression
+gzip compressed data, was "windrose-1.9.0.tar", last modified: Mon Jun 12 17:45:59 2023, max compression
```

## Comparing `windrose-1.8.1.tar` & `windrose-1.9.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-12-21 00:07:17.545029 windrose-1.8.1/
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-12-21 00:07:17.541029 windrose-1.8.1/.binder/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      156 2022-09-21 16:10:09.000000 windrose-1.8.1/.binder/environment.yml
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-12-21 00:07:17.541029 windrose-1.8.1/.github/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      310 2022-12-21 00:06:43.000000 windrose-1.8.1/.github/dependabot.yml
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-12-21 00:07:17.545029 windrose-1.8.1/.github/workflows/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1249 2022-12-21 00:06:43.000000 windrose-1.8.1/.github/workflows/deploy-docs.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1036 2022-12-21 00:06:43.000000 windrose-1.8.1/.github/workflows/pypi.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1030 2022-12-21 00:06:43.000000 windrose-1.8.1/.github/workflows/tests.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     4250 2022-09-21 16:10:09.000000 windrose-1.8.1/CHANGELOG.md
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     3215 2022-09-21 11:55:12.000000 windrose-1.8.1/CODE_OF_CONDUCT.md
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2339 2022-09-21 16:10:09.000000 windrose-1.8.1/CONTRIBUTING.md
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1498 2022-09-21 16:10:09.000000 windrose-1.8.1/CONTRIBUTORS.md
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       74 2022-09-21 16:10:09.000000 windrose-1.8.1/LICENCE.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1481 2022-09-21 16:10:09.000000 windrose-1.8.1/LICENCE_BSD-3-Clause.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    21391 2022-09-21 16:10:09.000000 windrose-1.8.1/LICENCE_CECILL-B.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      277 2022-09-21 16:10:09.000000 windrose-1.8.1/MANIFEST.in
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     4989 2022-12-21 00:07:17.545029 windrose-1.8.1/PKG-INFO
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     3954 2022-09-26 13:15:26.000000 windrose-1.8.1/README.md
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      375 2022-09-21 16:10:09.000000 windrose-1.8.1/pyproject.toml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1261 2022-09-21 16:10:09.000000 windrose-1.8.1/release-procedure.md
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      282 2022-09-21 16:10:09.000000 windrose-1.8.1/requirements-dev.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       41 2022-12-21 00:06:43.000000 windrose-1.8.1/requirements.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1511 2022-12-21 00:07:17.545029 windrose-1.8.1/setup.cfg
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      419 2022-09-21 16:10:09.000000 windrose-1.8.1/setup.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-12-21 00:07:17.545029 windrose-1.8.1/windrose/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      897 2022-09-21 16:10:09.000000 windrose-1.8.1/windrose/__init__.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    34243 2022-12-21 00:06:43.000000 windrose-1.8.1/windrose/windrose.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-12-21 00:07:17.545029 windrose-1.8.1/windrose.egg-info/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      414 2022-12-21 00:07:17.000000 windrose-1.8.1/windrose.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:45:59.025693 windrose-1.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:45:59.025693 windrose-1.9.0/.binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-12 17:45:45.000000 windrose-1.9.0/.binder/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:45:59.025693 windrose-1.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-12 17:45:45.000000 windrose-1.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:45:59.025693 windrose-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-12 17:45:45.000000 windrose-1.9.0/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-12 17:45:45.000000 windrose-1.9.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-12 17:45:45.000000 windrose-1.9.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-12 17:45:45.000000 windrose-1.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-12 17:45:45.000000 windrose-1.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-12 17:45:45.000000 windrose-1.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-12 17:45:45.000000 windrose-1.9.0/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-12 17:45:45.000000 windrose-1.9.0/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-12 17:45:45.000000 windrose-1.9.0/LICENCE_BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21391 2023-06-12 17:45:45.000000 windrose-1.9.0/LICENCE_CECILL-B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-12 17:45:45.000000 windrose-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-12 17:45:59.025693 windrose-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-12 17:45:45.000000 windrose-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-12 17:45:45.000000 windrose-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-12 17:45:45.000000 windrose-1.9.0/release-procedure.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 17:45:45.000000 windrose-1.9.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 17:45:45.000000 windrose-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-12 17:45:59.029693 windrose-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-12 17:45:45.000000 windrose-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:45:59.025693 windrose-1.9.0/windrose/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-12 17:45:45.000000 windrose-1.9.0/windrose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:45:59.025693 windrose-1.9.0/windrose/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-12 17:45:58.000000 windrose-1.9.0/windrose/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    34263 2023-06-12 17:45:45.000000 windrose-1.9.0/windrose/windrose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:45:59.025693 windrose-1.9.0/windrose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-12 17:45:59.000000 windrose-1.9.0/windrose.egg-info/SOURCES.txt
```

### Comparing `windrose-1.8.1/.github/workflows/deploy-docs.yml` & `windrose-1.9.0/.github/workflows/deploy-docs.yml`

 * *Files 11% similar despite different names*

```diff
@@ -15,36 +15,39 @@
 
     steps:
     - name: checkout
       uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
-    - name: Setup Mamba
-      uses: mamba-org/provision-with-micromamba@v14
+    - name: Setup Micromamba
+      uses: mamba-org/setup-micromamba@v1
       with:
-        environment-file: false
+        environment-name: TEST
+        init-shell: bash
+        create-args: >-
+          python=3 pip
+          --file requirements.txt
+          --file requirements-dev.txt
+          --channel conda-forge
 
-    - name: Build environment
+    - name: Install windrose
       shell: bash -l {0}
-      run: >
-        micromamba create --name TEST python=3 --file requirements.txt --file requirements-dev.txt --channel conda-forge
-        && micromamba activate TEST
-        && python -m pip install -e . --no-deps --force-reinstall
+      run: |
+        python -m pip install -e . --no-deps --force-reinstall
 
     - name: Build documentation
       shell: bash -l {0}
       run: |
         set -e
-        micromamba activate TEST
         jupyter nbconvert --to notebook --execute notebooks/usage.ipynb --output=usage-output.ipynb
         mv notebooks/*output.ipynb docs/
         pushd docs
         make clean html linkcheck
         popd
 
     - name: Deploy
-      if: github.event_name == 'release' || github.event_name == 'push'
-      uses: peaceiris/actions-gh-pages@v3.9.0
+      if: success() && github.event_name == 'release'
+      uses: peaceiris/actions-gh-pages@v3
       with:
         github_token: ${{ secrets.GITHUB_TOKEN }}
         publish_dir: docs/_build/html
```

### Comparing `windrose-1.8.1/.github/workflows/pypi.yml` & `windrose-1.9.0/.github/workflows/pypi.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 name: Publish to PyPI
 
-on: ["push", "pull_request"]
+on:
+  pull_request:
+  push:
+    branches:
+      - main
+  release:
+    types:
+      - published
 
 defaults:
   run:
     shell: bash
 
 jobs:
   packages:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.x
+        python-version: "3.x"
 
     - name: Get tags
       run: git fetch --depth=1 origin +refs/tags/*:refs/tags/*
 
     - name: Install build tools
       run: |
-        python -m pip install --upgrade pip wheel setuptools setuptools_scm build twine check-manifest
+        python -m pip install --upgrade pip build
 
     - name: Build binary wheel
       run: python -m build --sdist --wheel . --outdir dist
 
     - name: CheckFiles
       run: >
-        check-manifest
+        python -m pip install --upgrade check-manifest
+        && check-manifest
         && ls dist
 
     - name: Test wheels
-      run: |
-        cd dist && python -m pip install windrose*.whl
-        python -m twine check *
+      run: >
+        python -m pip install --upgrade pip twine
+        && cd dist && python -m pip install windrose*.whl
+        && python -m twine check *
 
     - name: Publish a Python distribution to PyPI
-      if: ${{ github.event_name == 'release' }}
-      uses: pypa/gh-action-pypi-publish@v1.6.4
+      if: success() && github.event_name == 'release'
+      uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_PASSWORD }}
```

### Comparing `windrose-1.8.1/.github/workflows/tests.yml` & `windrose-1.9.0/.github/workflows/tests.yml`

 * *Files 12% similar despite different names*

```diff
@@ -13,25 +13,28 @@
         python-version: ["3.8", "3.9", "3.10", "3.11"]
         os: [windows-latest, ubuntu-latest, macos-latest]
       fail-fast: false
 
     steps:
     - uses: actions/checkout@v3
 
-    - name: Setup
-      uses: mamba-org/provision-with-micromamba@v14
+    - name: Setup Micromamba for Python ${{ matrix.python-version }}
+      uses: mamba-org/setup-micromamba@v1
       with:
-        environment-file: false
+        environment-name: TEST
+        init-shell: bash
+        create-args: >-
+          python=${{ matrix.python-version }} pip
+          --file requirements.txt
+          --file requirements-dev.txt
+          --channel conda-forge
 
-    - name: Python ${{ matrix.python-version }}
+    - name: Install windrose
       shell: bash -l {0}
-      run: >
-        micromamba create --name TEST python=${{ matrix.python-version }} --file requirements.txt --file requirements-dev.txt --channel conda-forge
-        && micromamba activate TEST
-        && python -m pip install -e . --no-deps --force-reinstall
+      run: |
+        python -m pip install -e . --no-deps --force-reinstall
 
     - name: Tests
       shell: bash -l {0}
       run: |
-        micromamba activate TEST
         pytest -s -rxs -vv -Werror tests/ --mpl --mpl-generate-summary=html \
         --mpl-results-path="windrose_test_output-${{ matrix.os }}-${{ matrix.python-version }}"
```

### Comparing `windrose-1.8.1/CHANGELOG.md` & `windrose-1.9.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `windrose-1.8.1/CODE_OF_CONDUCT.md` & `windrose-1.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `windrose-1.8.1/CONTRIBUTING.md` & `windrose-1.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `windrose-1.8.1/CONTRIBUTORS.md` & `windrose-1.9.0/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `windrose-1.8.1/LICENCE_BSD-3-Clause.txt` & `windrose-1.9.0/LICENCE_BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `windrose-1.8.1/LICENCE_CECILL-B.txt` & `windrose-1.9.0/LICENCE_CECILL-B.txt`

 * *Files identical despite different names*

### Comparing `windrose-1.8.1/PKG-INFO` & `windrose-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windrose
-Version: 1.8.1
+Version: 1.9.0
 Summary: Python Matplotlib, Numpy library to manage wind data, draw windrose (also known as a polar rose plot)
 Home-page: https://github.com/python-windrose/windrose
 Author: Lionel Roubeyrie
 Author-email: s.celles@gmail.co
 Maintainer: Sebastien Celles
 License: BCeCILL-B OR BSD-3-Clause
 Project-URL: Documentation, https://python-windrose.github.io/windrose
@@ -55,20 +55,21 @@
 
 ### Requirements
 
 - matplotlib http://matplotlib.org/
 - numpy http://www.numpy.org/
 - and naturally python https://www.python.org/ :-P
 
-Option libraries:
+Optional libraries:
 
 - Pandas http://pandas.pydata.org/ (to feed plot functions easily)
 - Scipy http://www.scipy.org/ (to fit data with Weibull distribution)
 - ffmpeg https://www.ffmpeg.org/ (to output video)
 - click http://click.pocoo.org/ (for command line interface tools)
+- seaborn https://seaborn.pydata.org/ (for easy subplots)
 
 ### Install latest release version via pip
 
 A package is available and can be downloaded from PyPi and installed using:
 
 ```bash
 $ pip install windrose
@@ -102,8 +103,8 @@
 ### Contributing
 
 If you discover issues, have ideas for improvements or new features, please report them.
 [CONTRIBUTING.md](https://github.com/python-windrose/windrose/blob/master/CONTRIBUTING.md) explains
 how to contribute to this project.
 
 ### List of contributors and/or notable users
-https://github.com/python-windrose/windrose/blob/master/CONTRIBUTORS.md
+https://github.com/python-windrose/windrose/blob/main/CONTRIBUTORS.md
```

### Comparing `windrose-1.8.1/README.md` & `windrose-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,21 @@
 
 ### Requirements
 
 - matplotlib http://matplotlib.org/
 - numpy http://www.numpy.org/
 - and naturally python https://www.python.org/ :-P
 
-Option libraries:
+Optional libraries:
 
 - Pandas http://pandas.pydata.org/ (to feed plot functions easily)
 - Scipy http://www.scipy.org/ (to fit data with Weibull distribution)
 - ffmpeg https://www.ffmpeg.org/ (to output video)
 - click http://click.pocoo.org/ (for command line interface tools)
+- seaborn https://seaborn.pydata.org/ (for easy subplots)
 
 ### Install latest release version via pip
 
 A package is available and can be downloaded from PyPi and installed using:
 
 ```bash
 $ pip install windrose
@@ -78,8 +79,8 @@
 ### Contributing
 
 If you discover issues, have ideas for improvements or new features, please report them.
 [CONTRIBUTING.md](https://github.com/python-windrose/windrose/blob/master/CONTRIBUTING.md) explains
 how to contribute to this project.
 
 ### List of contributors and/or notable users
-https://github.com/python-windrose/windrose/blob/master/CONTRIBUTORS.md
+https://github.com/python-windrose/windrose/blob/main/CONTRIBUTORS.md
```

### Comparing `windrose-1.8.1/release-procedure.md` & `windrose-1.9.0/release-procedure.md`

 * *Files identical despite different names*

### Comparing `windrose-1.8.1/setup.cfg` & `windrose-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `windrose-1.8.1/windrose/windrose.py` & `windrose-1.9.0/windrose/windrose.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 from numpy.lib.twodim_base import histogram2d
 
 ZBASE = -1000  # The starting zorder for all drawing, negative to have the grid on
 VAR_DEFAULT = "speed"
 DIR_DEFAULT = "direction"
 FIGSIZE_DEFAULT = (8, 8)
 DPI_DEFAULT = 80
-CALM_CIRCLE_COLOR = "red"
-CALM_CIRCLE_ALPHA = 0.4
 DEFAULT_THETA_LABELS = ["E", "N-E", "N", "N-W", "W", "S-W", "S", "S-E"]
 
 
 def _copy_docstring(source):
     """
 
     Copy the docstring from another function.
@@ -123,32 +121,32 @@
                     figsize=figsize,
                     dpi=DPI_DEFAULT,
                     facecolor="w",
                     edgecolor="w",
                 )
             if rect is None:
                 rect = [0.1, 0.1, 0.8, 0.8]
-            ax = WindroseAxes(fig, rect, rmax=rmax, *args, **kwargs)
+            ax = WindroseAxes(fig, rect, *args, **kwargs)
             fig.add_axes(ax)
             return ax
         else:
             return ax
 
     def clear(self):
         """
         Clear the current axes
         """
         PolarAxes.clear(self)
 
         self.theta_angles = np.arange(0, 360, 45)
         self.set_thetagrids(angles=self.theta_angles, labels=self.theta_labels)
 
-        self._info = {"dir": list(), "bins": list(), "table": list()}
+        self._info = {"dir": [], "bins": [], "table": []}
 
-        self.patches_list = list()
+        self.patches_list = []
 
         self.calm_count = None
 
     def _colors(self, cmap, n):
         """
         Returns a list of n colors based on the colormap cmap
 
@@ -219,33 +217,37 @@
             the border between the axes and legend edge
         kwarg
             Every other kwarg argument supported by
             :obj:`matplotlib.pyplot.legend`
         """
 
         def get_handles():
-            handles = list()
+            handles = []
             for p in self.patches_list:
                 if isinstance(p, mpl.patches.Polygon) or isinstance(
-                    p, mpl.patches.Rectangle
+                    p,
+                    mpl.patches.Rectangle,
                 ):
                     color = p.get_facecolor()
                 elif isinstance(p, mpl.lines.Line2D):
                     color = p.get_color()
                 else:
                     raise AttributeError("Can't handle patches")
                 handles.append(
                     mpl.patches.Rectangle(
-                        (0, 0), 0.2, 0.2, facecolor=color, edgecolor="black"
-                    )
+                        (0, 0),
+                        0.2,
+                        0.2,
+                        facecolor=color,
+                        edgecolor="black",
+                    ),
                 )
             return handles
 
         def get_labels(decimal_places=1, units=None):
-
             digits = np.copy(self._info["bins"]).tolist()
             if not digits:
                 return ""
             digits[-1] = digits[-2]
             digits = [f"{label:.{decimal_places}f}" for label in digits]
             fmt = "[{} : {}"
             if locale.getlocale()[0] in ["fr_FR"]:
@@ -301,47 +303,64 @@
         mean_values :
         frequency :
         calm_limit : float, default None
         kwarg
             Any argument accepted by :obj:`matplotlib.pyplot.plot`.
         """
 
+        normed = kwargs.pop("normed", False)
+        blowto = kwargs.pop("blowto", False)
+
+        # Calm condition, mask data if needed
+        calm_limit = kwargs.pop("calm_limit", None)
+        total = len(var)
+        if calm_limit is not None:
+            mask = var > calm_limit
+            self.calm_count = len(var) - np.count_nonzero(mask)
+            if normed:
+                self.calm_count = self.calm_count * 100 / len(var)
+            var = var[mask]
+            direction = direction[mask]
+
         # if weibull factors are entered overwrite direction and var
         if "weibull_factors" in kwargs or "mean_values" in kwargs:
             if "weibull_factors" in kwargs and "mean_values" in kwargs:
                 raise TypeError("cannot specify both weibull_factors and mean_values")
             statistic_type = "unset"
             if "weibull_factors" in kwargs:
                 statistic_type = "weibull"
                 val = kwargs.pop("weibull_factors")
             elif "mean_values" in kwargs:
                 statistic_type = "mean"
                 val = kwargs.pop("mean_values")
             if val:
                 if "frequency" not in kwargs:
                     raise TypeError(
-                        "specify 'frequency' argument for statistical input"
+                        "specify 'frequency' argument for statistical input",
                     )
                 windFrequencies = kwargs.pop("frequency")
                 if len(windFrequencies) != len(direction) or len(direction) != len(var):
                     if len(windFrequencies) != len(direction):
                         raise TypeError("len(frequency) != len(direction)")
                     elif len(direction) != len(var):
                         raise TypeError("len(frequency) != len(direction)")
                 windSpeeds = []
                 windDirections = []
                 for dbin in range(len(direction)):
                     for _ in range(int(windFrequencies[dbin] * 10000)):
                         if statistic_type == "weibull":
                             windSpeeds.append(
-                                random.weibullvariate(var[dbin][0], var[dbin][1])
+                                random.weibullvariate(var[dbin][0], var[dbin][1]),
                             )
                         elif statistic_type == "mean":
                             windSpeeds.append(
-                                random.weibullvariate(var[dbin] * 2 / np.sqrt(np.pi), 2)
+                                random.weibullvariate(
+                                    var[dbin] * 2 / np.sqrt(np.pi),
+                                    2,
+                                ),
                             )
                         windDirections.append(direction[dbin])
                 var, direction = windSpeeds, windDirections
 
         # self.clear()
         kwargs.pop("zorder", None)
 
@@ -372,49 +391,31 @@
             if cmap is None:
                 cmap = plt.get_cmap()
             colors = self._colors(cmap, nbins)
 
         # Building the angles list
         angles = np.arange(0, -2 * np.pi, -2 * np.pi / nsector) + np.pi / 2
 
-        normed = kwargs.pop("normed", False)
-        blowto = kwargs.pop("blowto", False)
-
-        # Calm condition
-        calm_limit = kwargs.pop("calm_limit", None)
-        if calm_limit is not None:
-            mask = var > calm_limit
-            self.calm_count = len(var) - np.count_nonzero(mask)
-            if normed:
-                self.calm_count = self.calm_count * 100 / len(var)
-            var = var[mask]
-            direction = direction[mask]
-
         # Set the global information dictionary
         self._info["dir"], self._info["bins"], self._info["table"] = histogram(
-            direction, var, bins, nsector, normed, blowto
+            direction,
+            var,
+            bins,
+            nsector,
+            normed,
+            blowto,
+            total,
         )
 
         return bins, nbins, nsector, colors, angles, kwargs
 
     def _calm_circle(self):
-        """
-        Draw the calm centered circle
-        and return the initial offset for plots methods
-        """
+        """Draw the calm centered circle"""
         if self.calm_count and self.calm_count > 0:
-            circle = mpl.patches.Circle(
-                (0.0, 0.0),
-                self.calm_count,
-                transform=self.transData._b,
-                color=CALM_CIRCLE_COLOR,
-                alpha=CALM_CIRCLE_ALPHA,
-            )
-            self.add_artist(circle)
-        return self.calm_count or 0
+            self.set_rorigin(-(np.sqrt(self.calm_count / np.pi)))
 
     def contour(self, direction, var, **kwargs):
         """
         Plot a windrose in linear mode. For each var bins, a line will be
         draw on the axes, a segment between each sector (center to center).
         Each line can be formatted (color, width, ...) like with standard plot
         pylab command.
@@ -424,17 +425,17 @@
         direction : 1D array
             directions the wind blows from, North centred
         var : 1D array
             values of the variable to compute. Typically the wind speeds.
 
         Other Parameters
         ----------------
-        sector : integer, optional
+        nsector : integer, optional
             number of sectors used to compute the windrose table. If not set,
-            nsectors=16, then each sector will be 360/16=22.5°, and the
+            nsector=16, then each sector will be 360/16=22.5°, and the
             resulting computed table will be aligned with the cardinals points.
         bins : 1D array or integer, optional
             number of bins, or a sequence of bins variable. If not set, bins=6,
             then bins=linspace(min(var), max(var), 6)
         blowto : bool, optional
             If True, the windrose will be pi rotated, to show where the wind
             blow to (useful for pollutant rose).
@@ -460,23 +461,25 @@
 
         # closing lines
         angles = np.hstack((angles, angles[-1] - 2 * np.pi / nsector))
         vals = np.hstack(
             (
                 self._info["table"],
                 np.reshape(
-                    self._info["table"][:, 0], (self._info["table"].shape[0], 1)
+                    self._info["table"][:, 0],
+                    (self._info["table"].shape[0], 1),
                 ),
-            )
+            ),
         )
 
-        offset = self._calm_circle()
+        self._calm_circle()
+        origin = 0
         for i in range(nbins):
-            val = vals[i, :] + offset
-            offset += vals[i, :]
+            val = vals[i, :] + origin
+            origin += vals[i, :]
             zorder = ZBASE + nbins - i
             patch = self.plot(angles, val, color=colors[i], zorder=zorder, **kwargs)
             self.patches_list.extend(patch)
         self._update()
 
     def contourf(self, direction, var, **kwargs):
         """
@@ -492,15 +495,15 @@
         var : 1D array
             values of the variable to compute. Typically the wind speeds
 
         Other Parameters
         ----------------
         nsector: integer, optional
             number of sectors used to compute the windrose table. If not set,
-            nsectors=16, then each sector will be 360/16=22.5°, and the
+            nsector=16, then each sector will be 360/16=22.5°, and the
             resulting computed table will be aligned with the cardinals points.
         bins : 1D array or integer, optional
             number of bins, or a sequence of bins variable. If not set, bins=6,
             then bins=linspace(min(`var`), max(`var`), 6)
         blowto : bool, optional
             If True, the windrose will be pi rotated, to show where the wind
             blow to (useful for pollutant rose).
@@ -528,22 +531,24 @@
 
         # closing lines
         angles = np.hstack((angles, angles[-1] - 2 * np.pi / nsector))
         vals = np.hstack(
             (
                 self._info["table"],
                 np.reshape(
-                    self._info["table"][:, 0], (self._info["table"].shape[0], 1)
+                    self._info["table"][:, 0],
+                    (self._info["table"].shape[0], 1),
                 ),
-            )
+            ),
         )
-        offset = self._calm_circle()
+        self._calm_circle()
+        origin = 0
         for i in range(nbins):
-            val = vals[i, :] + offset
-            offset += vals[i, :]
+            val = vals[i, :] + origin
+            origin += vals[i, :]
             zorder = ZBASE + nbins - i
             patch = self.fill(
                 np.append(angles, 0),
                 np.append(val, 0),
                 facecolor=colors[i],
                 edgecolor=colors[i],
                 zorder=zorder,
@@ -564,15 +569,15 @@
         var : 1D array
             values of the variable to compute. Typically the wind speeds.
 
         Other Parameters
         ----------------
         nsector : integer, optional
             number of sectors used to compute the windrose table. If not set,
-            nsectors=16, then each sector will be 360/16=22.5°, and the
+            nsector=16, then each sector will be 360/16=22.5°, and the
             resulting computed table will be aligned with the cardinals points.
         bins : 1D array or integer, optional
             number of bins, or a sequence of bins variable. If not set, bins=6
             between min(`var`) and max(`var`).
         blowto : bool, optional.
             if True, the windrose will be pi rotated, to show where the wind
             blow to (useful for pollutant rose).
@@ -606,25 +611,25 @@
                 raise ValueError("edgecolor must be a string color")
         opening = kwargs.pop("opening", None)
         if opening is None:
             opening = 0.8
         dtheta = 2 * np.pi / nsector
         opening = dtheta * opening
 
-        offs = self._calm_circle()
+        self._calm_circle()
 
         for j in range(nsector):
-            offset = offs
+            origin = 0
             for i in range(nbins):
                 if i > 0:
-                    offset += self._info["table"][i - 1, j]
+                    origin += self._info["table"][i - 1, j]
                 val = self._info["table"][i, j]
                 zorder = ZBASE + nbins - i
                 patch = mpl.patches.Rectangle(
-                    (angles[j] - opening / 2, offset),
+                    (angles[j] - opening / 2, origin),
                     opening,
                     val,
                     facecolor=colors[i],
                     edgecolor=edgecolor,
                     zorder=zorder,
                     **kwargs,
                 )
@@ -645,15 +650,15 @@
         var : 1D array
             values of the variable to compute. Typically the wind speeds
 
         Other Parameters
         ----------------
         nsector: integer, optional
             number of sectors used to compute the windrose table. If not set,
-            nsectors=16, then each sector will be 360/16=22.5°, and the
+            nsector=16, then each sector will be 360/16=22.5°, and the
             resulting computed table will be aligned with the cardinals points.
         bins : 1D array or integer, optional
             number of bins, or a sequence of bins variable. If not set, bins=6
             between min(`var`) and max(`var`).
         blowto : bool, optional
             If True, the windrose will be pi rotated, to show where the wind
             blow to (useful for pollutant rose).
@@ -680,25 +685,25 @@
         kwargs.pop("facecolor", None)
         edgecolor = kwargs.pop("edgecolor", None)
         if edgecolor is not None:
             if not isinstance(edgecolor, str):
                 raise ValueError("edgecolor must be a string color")
         opening = np.linspace(0.0, np.pi / 16, nbins)
 
-        offs = self._calm_circle()
+        self._calm_circle()
 
         for j in range(nsector):
-            offset = offs
+            origin = 0
             for i in range(nbins):
                 if i > 0:
-                    offset += self._info["table"][i - 1, j]
+                    origin += self._info["table"][i - 1, j]
                 val = self._info["table"][i, j]
                 zorder = ZBASE + nbins - i
                 patch = mpl.patches.Rectangle(
-                    (angles[j] - opening[i] / 2, offset),
+                    (angles[j] - opening[i] / 2, origin),
                     opening[i],
                     val,
                     facecolor=colors[i],
                     edgecolor=edgecolor,
                     zorder=zorder,
                     **kwargs,
                 )
@@ -751,15 +756,15 @@
         self.bar(center, hist, align="center", width=width, color=bar_color)
         params = scipy.stats.exponweib.fit(var, floc=0, f0=1)
         x = np.linspace(0, bins[-1], Nx)
         self.plot(x, scipy.stats.exponweib.pdf(x, *params), color=plot_color)
         return (self, params)
 
 
-def histogram(direction, var, bins, nsector, normed=False, blowto=False):
+def histogram(direction, var, bins, nsector, normed=False, blowto=False, total=0):
     """
     Returns an array where, for each sector of wind
     (centred on the north), we have the number of time the wind comes with a
     particular var (speed, pollutant concentration, ...).
 
     Parameters
     ----------
@@ -801,15 +806,15 @@
 
     table = histogram2d(x=var, y=direction, bins=[var_bins, dir_bins], density=False)[0]
     # add the last value to the first to have the table of North winds
     table[:, 0] = table[:, 0] + table[:, -1]
     # and remove the last col
     table = table[:, :-1]
     if normed:
-        table = table * 100 / table.sum()
+        table = table * 100 / total
 
     return dir_edges, var_bins, table
 
 
 @_copy_docstring(WindroseAxes.contour)
 def wrcontour(direction, var, ax=None, rmax=None, figsize=FIGSIZE_DEFAULT, **kwargs):
     """
@@ -965,15 +970,17 @@
     rmax=None,
     ax=None,
     **kwargs,
 ):
     """Plot windrose from a pandas DataFrame."""
     var = df[var_name].values
     direction = df[direction_name].values
-    return plot_windrose_np(direction, var, by=by, rmax=rmax, ax=ax, **kwargs)
+    return plot_windrose_np(
+        direction, var, kind=kind, by=by, rmax=rmax, ax=ax, **kwargs
+    )
 
 
 def plot_windrose_np(
     direction,
     var,
     kind="contour",
     clean_flag=True,
@@ -997,9 +1004,9 @@
         ax = f_plot(direction=direction, var=var, rmax=rmax, ax=ax, **kwargs)
         if kind not in ["pdf"]:
             ax.set_legend()
         return ax
     else:
         raise NotImplementedError(
             "'by' keyword not supported for now "
-            "https://github.com/scls19fr/windrose/issues/10"
+            "https://github.com/scls19fr/windrose/issues/10",
         )
```

