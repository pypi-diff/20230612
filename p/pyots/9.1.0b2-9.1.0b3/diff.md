# Comparing `tmp/pyots-9.1.0b2.tar.gz` & `tmp/pyots-9.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyots-9.1.0b2.tar", last modified: Fri Jun  2 03:22:21 2023, max compression
+gzip compressed data, was "pyots-9.1.0b3.tar", last modified: Mon Jun 12 19:22:12 2023, max compression
```

## Comparing `pyots-9.1.0b2.tar` & `pyots-9.1.0b3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.330149 pyots-9.1.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 03:19:16.000000 pyots-9.1.0b2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.326149 pyots-9.1.0b2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.326149 pyots-9.1.0b2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-02 03:19:16.000000 pyots-9.1.0b2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-02 03:19:16.000000 pyots-9.1.0b2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.326149 pyots-9.1.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-02 03:19:16.000000 pyots-9.1.0b2/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-02 03:19:16.000000 pyots-9.1.0b2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-02 03:19:16.000000 pyots-9.1.0b2/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-02 03:19:16.000000 pyots-9.1.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-02 03:19:16.000000 pyots-9.1.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-02 03:22:21.330149 pyots-9.1.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-02 03:19:16.000000 pyots-9.1.0b2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2403 2023-06-02 03:19:16.000000 pyots-9.1.0b2/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-02 03:19:16.000000 pyots-9.1.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 03:19:16.000000 pyots-9.1.0b2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-02 03:22:21.330149 pyots-9.1.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-06-02 03:19:16.000000 pyots-9.1.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.326149 pyots-9.1.0b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.326149 pyots-9.1.0b2/src/_pyots/
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-02 03:19:16.000000 pyots-9.1.0b2/src/_pyots/bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-02 03:19:16.000000 pyots-9.1.0b2/src/_pyots/pyots-context.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.326149 pyots-9.1.0b2/src/pyots/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-02 03:19:16.000000 pyots-9.1.0b2/src/pyots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.326149 pyots-9.1.0b2/src/pyots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-02 03:22:21.000000 pyots-9.1.0b2/src/pyots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-02 03:22:21.000000 pyots-9.1.0b2/src/pyots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 03:22:21.000000 pyots-9.1.0b2/src/pyots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 03:22:21.000000 pyots-9.1.0b2/src/pyots.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 03:22:21.000000 pyots-9.1.0b2/src/pyots.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.330149 pyots-9.1.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-02 03:19:16.000000 pyots-9.1.0b2/tests/test_compare_ots_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-02 03:19:16.000000 pyots-9.1.0b2/tests/test_ots_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.134186 pyots-9.1.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-12 19:18:42.000000 pyots-9.1.0b3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.130186 pyots-9.1.0b3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.130186 pyots-9.1.0b3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-12 19:18:42.000000 pyots-9.1.0b3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-12 19:18:42.000000 pyots-9.1.0b3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.130186 pyots-9.1.0b3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-12 19:18:42.000000 pyots-9.1.0b3/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-12 19:18:42.000000 pyots-9.1.0b3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-12 19:18:42.000000 pyots-9.1.0b3/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-12 19:18:42.000000 pyots-9.1.0b3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-12 19:18:42.000000 pyots-9.1.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-12 19:22:12.134186 pyots-9.1.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-12 19:18:42.000000 pyots-9.1.0b3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2403 2023-06-12 19:18:42.000000 pyots-9.1.0b3/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-12 19:18:42.000000 pyots-9.1.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-12 19:18:42.000000 pyots-9.1.0b3/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-12 19:18:42.000000 pyots-9.1.0b3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-12 19:22:12.134186 pyots-9.1.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-06-12 19:18:42.000000 pyots-9.1.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.130186 pyots-9.1.0b3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.130186 pyots-9.1.0b3/src/_pyots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-12 19:18:42.000000 pyots-9.1.0b3/src/_pyots/bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-12 19:18:42.000000 pyots-9.1.0b3/src/_pyots/pyots-context.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.130186 pyots-9.1.0b3/src/pyots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-12 19:18:42.000000 pyots-9.1.0b3/src/pyots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.134186 pyots-9.1.0b3/src/pyots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-12 19:22:11.000000 pyots-9.1.0b3/src/pyots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-12 19:22:12.000000 pyots-9.1.0b3/src/pyots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:22:11.000000 pyots-9.1.0b3/src/pyots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:22:11.000000 pyots-9.1.0b3/src/pyots.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 19:22:11.000000 pyots-9.1.0b3/src/pyots.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.134186 pyots-9.1.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-12 19:18:42.000000 pyots-9.1.0b3/tests/test_compare_ots_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-12 19:18:42.000000 pyots-9.1.0b3/tests/test_ots_suite.py
```

### Comparing `pyots-9.1.0b2/.github/ISSUE_TEMPLATE/bug_report.md` & `pyots-9.1.0b3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b2/.github/ISSUE_TEMPLATE/feature_request.md` & `pyots-9.1.0b3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b2/.github/workflows/codeql.yml` & `pyots-9.1.0b3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b2/.github/workflows/release.yml` & `pyots-9.1.0b3/.github/workflows/release.yml`

 * *Files 11% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     - name: Install Python 3.9
       uses: actions/setup-python@v4
       with:
         python-version: '3.9'
 
     - name: Build wheel
-      uses: pypa/cibuildwheel@v2.13.0
+      uses: pypa/cibuildwheel@v2.13.1
       with:
         output-dir: dist
       env:
         CIBW_BUILD: "cp38-* cp39-* cp310-* cp311-*"
         CIBW_ARCHS_MACOS: x86_64 arm64
         CIBW_ENVIRONMENT_MACOS: "CFLAGS='-arch arm64 -arch x86_64' CXXFLAGS='-arch arm64 -arch x86_64' LDFLAGS='-arch arm64 -arch x86_64'"
         CIBW_ARCHS_LINUX: x86_64
@@ -62,14 +62,16 @@
         if-no-files-found: error
         retention-days: 30
 
   publish_release:
     name: Publish Release
     needs: build_wheels
     runs-on: ubuntu-latest
+    permissions:
+      contents: write  # Required by 'action-gh-release'
 
     steps:
 
     - name: Get date & flat tag
       id: date_tag
       run: |
         export DATE=$(TZ=US/Pacific date +'%Y-%m-%d')
@@ -90,13 +92,11 @@
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.pypi_password }}
 
     - name: Create GitHub Release
       uses: softprops/action-gh-release@v1
-      env:
-        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
         body: '${{ steps.date_tag.outputs.VERSION }} released ${{ steps.date_tag.outputs.TODAY }} - [Upstream OTS v${{ steps.date_tag.outputs.VERSION }} Release Notes](https://github.com/khaledhosny/ots/releases/tag/v${{ steps.date_tag.outputs.VERSION }})'
         prerelease: true
         files: ./dist/*
```

### Comparing `pyots-9.1.0b2/.github/workflows/run_tests.yml` & `pyots-9.1.0b3/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b2/.gitignore` & `pyots-9.1.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b2/LICENSE` & `pyots-9.1.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b2/PKG-INFO` & `pyots-9.1.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyots
-Version: 9.1.0b2
+Version: 9.1.0b3
 Summary: Python wrapper for ot-sanitizer
 Home-page: https://github.com/adobe-type-tools/pyots
 Author: Adobe Type team & friends
 Author-email: afdko@adobe.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyots (PYthon OT Sanitizer)
 
 [![Run Tests](https://github.com/adobe-type-tools/pyots/actions/workflows/run_tests.yml/badge.svg)](https://github.com/adobe-type-tools/pyots/actions/workflows/run_tests.yml) [![Build Python Wheels](https://github.com/adobe-type-tools/pyots/actions/workflows/release.yml/badge.svg)](https://github.com/adobe-type-tools/pyots/actions/workflows/release.yml)
```

### Comparing `pyots-9.1.0b2/README.md` & `pyots-9.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b2/build.py` & `pyots-9.1.0b3/build.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b2/setup.py` & `pyots-9.1.0b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,13 +295,13 @@
     description='Python wrapper for ot-sanitizer',
     ext_modules=[pyots_mod],
     long_description_content_type='text/markdown',
     long_description=long_description,
     name='pyots',
     packages=find_packages('src'),
     package_dir={'': 'src'},
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     url='https://github.com/adobe-type-tools/pyots',
     use_scm_version=True,
     setup_requires=['setuptools_scm'],
     zip_safe=False,
 )
```

### Comparing `pyots-9.1.0b2/src/_pyots/bindings.cpp` & `pyots-9.1.0b3/src/_pyots/bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b2/src/_pyots/pyots-context.h` & `pyots-9.1.0b3/src/_pyots/pyots-context.h`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b2/src/pyots/__init__.py` & `pyots-9.1.0b3/src/pyots/__init__.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b2/src/pyots.egg-info/PKG-INFO` & `pyots-9.1.0b3/src/pyots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyots
-Version: 9.1.0b2
+Version: 9.1.0b3
 Summary: Python wrapper for ot-sanitizer
 Home-page: https://github.com/adobe-type-tools/pyots
 Author: Adobe Type team & friends
 Author-email: afdko@adobe.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyots (PYthon OT Sanitizer)
 
 [![Run Tests](https://github.com/adobe-type-tools/pyots/actions/workflows/run_tests.yml/badge.svg)](https://github.com/adobe-type-tools/pyots/actions/workflows/run_tests.yml) [![Build Python Wheels](https://github.com/adobe-type-tools/pyots/actions/workflows/release.yml/badge.svg)](https://github.com/adobe-type-tools/pyots/actions/workflows/release.yml)
```

### Comparing `pyots-9.1.0b2/src/pyots.egg-info/SOURCES.txt` & `pyots-9.1.0b3/src/pyots.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .flake8
 .gitignore
 LICENSE
 README.md
 build.py
 pyproject.toml
+renovate.json
 requirements.txt
 setup.cfg
 setup.py
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/codeql.yml
 .github/workflows/release.yml
```

### Comparing `pyots-9.1.0b2/tests/test_compare_ots_python.py` & `pyots-9.1.0b3/tests/test_compare_ots_python.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b2/tests/test_ots_suite.py` & `pyots-9.1.0b3/tests/test_ots_suite.py`

 * *Files identical despite different names*

