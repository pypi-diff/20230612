# Comparing `tmp/idf_build_apps-1.0.0rc0.tar.gz` & `tmp/idf_build_apps-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf_build_apps-1.0.0rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "idf_build_apps-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `idf_build_apps-1.0.0rc0.tar` & `idf_build_apps-1.0.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      351 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.editorconfig
--rw-r--r--   0        0        0      123 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.git-blame-ignore-revs
--rw-r--r--   0        0        0       25 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.gitattributes
--rw-r--r--   0        0        0      253 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.github/workflows/check-pre-commit.yml
--rw-r--r--   0        0        0      675 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.github/workflows/issue_comment.yml
--rw-r--r--   0        0        0      620 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.github/workflows/new_issues.yml
--rw-r--r--   0        0        0      796 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.github/workflows/new_prs.yml
--rw-r--r--   0        0        0      438 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      521 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.github/workflows/test-build-docs.yml
--rw-r--r--   0        0        0     3685 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.github/workflows/test-build-idf-apps.yml
--rw-r--r--   0        0        0     3076 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.gitignore
--rw-r--r--   0        0        0     1077 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      383 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/.readthedocs.yml
--rw-r--r--   0        0        0     5128 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/CHANGELOG.md
--rw-r--r--   0        0        0     1834 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/LICENSE
--rw-r--r--   0        0        0     3843 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/README.md
--rw-r--r--   0        0        0       33 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/docs/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0      634 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/docs/Makefile
--rw-r--r--   0        0        0     6947 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/docs/_static/espressif-logo.svg
--rw-r--r--   0        0        0      942 2023-05-24 02:57:14.729606 idf_build_apps-1.0.0rc0/docs/_static/theme_overrides.css
--rw-r--r--   0        0        0      119 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/docs/_templates/layout.html
--rw-r--r--   0        0        0      490 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/docs/api.rst
--rw-r--r--   0        0        0     1449 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/docs/conf.py
--rw-r--r--   0        0        0     2652 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/docs/config_file.md
--rw-r--r--   0        0        0    10368 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/docs/find_build.md
--rw-r--r--   0        0        0      474 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/docs/index.rst
--rw-r--r--   0        0        0     5648 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/docs/manifest.md
--rw-r--r--   0        0        0      485 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/__init__.py
--rw-r--r--   0        0        0      182 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/__main__.py
--rw-r--r--   0        0        0    26619 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/app.py
--rw-r--r--   0        0        0     2794 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/config.py
--rw-r--r--   0        0        0     2187 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/constants.py
--rw-r--r--   0        0        0     6087 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/finder.py
--rw-r--r--   0        0        0     2220 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/log.py
--rw-r--r--   0        0        0    30651 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/main.py
--rw-r--r--   0        0        0      133 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/manifest/__init__.py
--rw-r--r--   0        0        0     6321 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/manifest/if_parser.py
--rw-r--r--   0        0        0     5956 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/manifest/manifest.py
--rw-r--r--   0        0        0     3423 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/manifest/soc_header.py
--rw-r--r--   0        0        0     6577 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/idf_build_apps/utils.py
--rw-r--r--   0        0        0      101 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/license_header.txt
--rw-r--r--   0        0        0     1874 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0     1221 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/tests/conftest.py
--rw-r--r--   0        0        0     3347 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/tests/test_build.py
--rw-r--r--   0        0        0    16010 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/tests/test_finder.py
--rw-r--r--   0        0        0      995 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/tests/test_manifest.py
--rw-r--r--   0        0        0     2394 2023-05-24 02:57:14.733606 idf_build_apps-1.0.0rc0/tests/test_utils.py
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 idf_build_apps-1.0.0rc0/setup.py
--rw-r--r--   0        0        0     5498 1970-01-01 00:00:00.000000 idf_build_apps-1.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0      351 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.editorconfig
+-rw-r--r--   0        0        0      123 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.git-blame-ignore-revs
+-rw-r--r--   0        0        0       25 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.gitattributes
+-rw-r--r--   0        0        0      253 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.github/workflows/check-pre-commit.yml
+-rw-r--r--   0        0        0      675 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.github/workflows/issue_comment.yml
+-rw-r--r--   0        0        0      620 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.github/workflows/new_issues.yml
+-rw-r--r--   0        0        0      796 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.github/workflows/new_prs.yml
+-rw-r--r--   0        0        0      438 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      521 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.github/workflows/test-build-docs.yml
+-rw-r--r--   0        0        0     3767 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.github/workflows/test-build-idf-apps.yml
+-rw-r--r--   0        0        0     3076 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1077 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      383 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.readthedocs.yml
+-rw-r--r--   0        0        0     5204 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1882 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3843 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/README.md
+-rw-r--r--   0        0        0       33 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0      634 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0     6947 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/_static/espressif-logo.svg
+-rw-r--r--   0        0        0      942 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0      119 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/_templates/layout.html
+-rw-r--r--   0        0        0      490 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/api.rst
+-rw-r--r--   0        0        0     1449 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/conf.py
+-rw-r--r--   0        0        0     2652 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/config_file.md
+-rw-r--r--   0        0        0    10473 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/find_build.md
+-rw-r--r--   0        0        0      474 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/index.rst
+-rw-r--r--   0        0        0     5717 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/manifest.md
+-rw-r--r--   0        0        0      481 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/__init__.py
+-rw-r--r--   0        0        0      182 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/__main__.py
+-rw-r--r--   0        0        0    26619 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/app.py
+-rw-r--r--   0        0        0     2794 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/config.py
+-rw-r--r--   0        0        0     2187 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/constants.py
+-rw-r--r--   0        0        0     6328 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/finder.py
+-rw-r--r--   0        0        0     2220 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/log.py
+-rw-r--r--   0        0        0    30607 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/main.py
+-rw-r--r--   0        0        0      133 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/manifest/__init__.py
+-rw-r--r--   0        0        0     6321 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/manifest/if_parser.py
+-rw-r--r--   0        0        0     5956 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/manifest/manifest.py
+-rw-r--r--   0        0        0     3423 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/manifest/soc_header.py
+-rw-r--r--   0        0        0     6748 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/utils.py
+-rw-r--r--   0        0        0      101 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/license_header.txt
+-rw-r--r--   0        0        0     1911 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1221 2023-06-12 08:52:33.082932 idf_build_apps-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0     3347 2023-06-12 08:52:33.082932 idf_build_apps-1.0.1/tests/test_build.py
+-rw-r--r--   0        0        0    16908 2023-06-12 08:52:33.082932 idf_build_apps-1.0.1/tests/test_finder.py
+-rw-r--r--   0        0        0      995 2023-06-12 08:52:33.082932 idf_build_apps-1.0.1/tests/test_manifest.py
+-rw-r--r--   0        0        0     3710 2023-06-12 08:52:33.082932 idf_build_apps-1.0.1/tests/test_utils.py
+-rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 idf_build_apps-1.0.1/setup.py
+-rw-r--r--   0        0        0     5540 1970-01-01 00:00:00.000000 idf_build_apps-1.0.1/PKG-INFO
```

### Comparing `idf_build_apps-1.0.0rc0/.github/workflows/issue_comment.yml` & `idf_build_apps-1.0.1/.github/workflows/issue_comment.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/.github/workflows/new_issues.yml` & `idf_build_apps-1.0.1/.github/workflows/new_issues.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/.github/workflows/new_prs.yml` & `idf_build_apps-1.0.1/.github/workflows/new_prs.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/.github/workflows/test-build-docs.yml` & `idf_build_apps-1.0.1/.github/workflows/test-build-docs.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/.github/workflows/test-build-idf-apps.yml` & `idf_build_apps-1.0.1/.github/workflows/test-build-idf-apps.yml`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         with:
           name: wheel
       - name: Build the Apps
         run: |
           export PYENV_ROOT="$HOME/.pyenv" && export PATH="$PYENV_ROOT/bin:$PATH" && eval "$(pyenv init --path)"
           pyenv global ${{ matrix.python-version }}
           rm $(which python3)
+          echo "urllib3<1.25,>=1.21.1" >> $IDF_PATH/requirements.txt
           bash $IDF_PATH/install.sh
           . $IDF_PATH/export.sh
           pip install idf_build_apps-*-py2.py3-none-any.whl
           python -m idf_build_apps build -vv -t esp32 \
             -p $IDF_PATH/examples/get-started/hello_world \
             --size-file size_info.json \
             --ignore-warning-str \
@@ -72,15 +73,15 @@
               "Support for Python 2 is deprecated"
 
   build-apps-on-idf-env:
     if: ${{ github.ref == 'refs/heads/main' }}
     needs: build-python-packages
     strategy:
       matrix:
-        idf-branch: [ release-v4.3, release-v4.4, release-v5.0]
+        idf-branch: [release-v4.3, release-v4.4, release-v5.0, release-v5.1]
     runs-on: ubuntu-latest
     container:
       image: espressif/idf:${{ matrix.idf-branch }}
     steps:
       - name: Download wheel
         uses: actions/download-artifact@v3
         with:
```

### Comparing `idf_build_apps-1.0.0rc0/.gitignore` & `idf_build_apps-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/.pre-commit-config.yaml` & `idf_build_apps-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/CHANGELOG.md` & `idf_build_apps-1.0.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
-## [Unreleased - 1.0.0]
+## [1.0.1] (2023-06-12)
+
+## Fixed
+
+- glob patterns are matched recursively
+
+## [1.0.0] (2023-05-25)
 
 ## Added
 
 - Support keyword `depends_filepatterns` in the manifest file
 - Support expanding environment variables in the manifest files
 
 ## BREAKING CHANGES
@@ -126,15 +132,15 @@
 - wrong log level on "Loading manifest file: ...". Set from `INFO` to `DEBUG`
 - wrong log level on "Building app \[ID\]: ...". Set from `DEBUG` to `INFO`
 
 ## [0.3.1] (2023-02-20)
 
 ### Fixed
 
-- Ralative path defined in the manifest files depend on the current work path
+- Relative path defined in the manifest files depend on the current work path
 
   Added `manifest_rootpath` argument in `find_apps()`. Will use this value instead as the root folder for calculating absolute path
 
 ## [0.3.0] (2023-01-10)
 
 ### Added
```

### Comparing `idf_build_apps-1.0.0rc0/CONTRIBUTING.md` & `idf_build_apps-1.0.1/CONTRIBUTING.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 Please use python 3.7+ for developing, but keep in mind that we need to support all ESP-IDF release versions.
 
 | ESP-IDF Version | Supported Python Versions |
 |-----------------|---------------------------|
 | 4.1             | 2.7, 3.4+                 |
 | 4.2             | 2.7, 3.4+                 |
-| 4.3             | 3.6+                      |
-| 4.4             | 3.6+                      |
+| 4.3             | 2.7, 3.4+                 |
+| 4.4             | 2.7, 3.4+                 |
 | 5.0             | 3.7+                      |
+| 5.1             | 3.7+                      |
 | master          | 3.7+                      |
 
 ## Setup the Dev Environment
 
 1. Create virtual environment
 
     ```shell
```

### Comparing `idf_build_apps-1.0.0rc0/LICENSE` & `idf_build_apps-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/README.md` & `idf_build_apps-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/docs/Makefile` & `idf_build_apps-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/docs/_static/espressif-logo.svg` & `idf_build_apps-1.0.1/docs/_static/espressif-logo.svg`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/docs/_static/theme_overrides.css` & `idf_build_apps-1.0.1/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/docs/conf.py` & `idf_build_apps-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/docs/config_file.md` & `idf_build_apps-1.0.1/docs/config_file.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/docs/find_build.md` & `idf_build_apps-1.0.1/docs/find_build.md`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     kconfig -- be overriden by --> sdkconfig -- be overriden by --> sdkconfig_target
 
     subgraph "which would only be applied when building with the corresponding target"
     sdkconfig_target
     end
 ```
 
+(config-rules)=
 ### Config Rules
 
 Config rule represents the sdkconfig file pattern and the config name. The syntax is simple: `[FILE_PATTERN]=[CONFIG_NAME]`.
 
 - `FILE_PATTERN`: Name of the sdkconfig file, optionally with a single wildcard (`*`) character.
 - `CONFIG_NAME`: Name of the corresponding build configuration, or None if the value of wildcard is to be used.
 
@@ -92,45 +93,46 @@
       -
    *  - ``sdkconfig.ci.*=``
       -  - ``foo``
          - ``bar``
       - The wildcard matches two files. Build two apps based on each sdkconfig file.
       -  - ``sdkconfig.ci.foo``
          - ``sdkconfig.ci.bar``
+```
 
-.. note::
-
-   For each config rule, only one wildcard is supported.
+```{note}
+For each config rule, only one wildcard is supported.
 ```
 
 ### Placeholders for Work Directory and Build Directory
 
 Here we defined two new terms of directories, work directory and build directory.
 
 #### Work Directory
 
 Work directory is the directory where the build actually happens. `idf-build-apps` would first copy the whole project to the work directory, then start the real build process. The benefit of specifying work directory is that you could keep your local build directory and `sdkconfig` file untouched.
 
 By default, `idf-build-apps` would use the project directory as the work directory.
 
 #### Build Directory
 
-Build directory is the directory where the binary files output would be generated. If it is set to a relative path, the full path would be calculated based on the work directory. If it is a absolute path, it would override the work directory settings.
+Build directory is the directory where the binary files output would be generated. If it is set to a relative path, the full path would be calculated based on the work directory. If it is an absolute path, it would override the work directory settings.
 
 By default, `idf-build-apps` would follow what ESP-IDF does, use `build` as the build directory.
 
 #### Placeholders
 
 Placeholders are a set of symbols, which could be used when setting work directory and build directory. The placeholders would be replaced while building as follows:
 
 - `@t`: Would be replaced by the target chip type.
 - `@w`: Would be replaced by the wildcard if exists, otherwise would be replaced by the config name.
 - `@n`: Would be replaced by the project name.
 - `@f`: Would be replaced by the escaped project path (replaced "/" to "_").
 - `@i`: Would be replaced by the build index. (only available in `build` command)
+- `@p`: Would be replaced by the parallel build index. (default to `1`, only available in `build` command)
 
 For example,
 
 ```shell
 idf-build-apps find -p . --recursive --target esp32 --config "sdkconfig.ci.*=" --build-dir build_@t_@w
 ```
 
@@ -156,19 +158,16 @@
 (cmake) App ./test-2, target esp32, sdkconfig (default), build in /tmp/build/test-2_esp32
 ```
 
 ## Build Apps
 
 Building apps is a process that build all the applications that are collected by the "finding apps" process.
 
-```{eval-rst}
-
-.. note::
-
-   Almost all CLI options that ``find`` supported are also supported in ``build`` command. You may call ``idf-build-apps find -h`` or ``idf-build-apps build -h`` for all possible CLI options.
+```{note}
+Almost all CLI options that ``find`` supported are also supported in ``build`` command. You may call ``idf-build-apps find -h`` or ``idf-build-apps build -h`` for all possible CLI options.
 ```
 
 ### Tips on `build` CLI Options
 
 #### Check Build Warnings
 
 You may use `--check-warnings` to enable this check. If any warning is captured while the building process, the exit code would turn to a non-zero value. Besides, `idf-build-apps` provides CLI options `--ignore-warnings-str` and `--ignore-warnings-file` to let you bypass some false alarms.
```

### Comparing `idf_build_apps-1.0.0rc0/docs/manifest.md` & `idf_build_apps-1.0.1/docs/manifest.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 - Capitalized Words
   - Variables start with `SOC_`. The value would be parsed from `IDF_PATH/components/soc/[TARGET]/include/soc/*_caps.h`
   - `IDF_TARGET`
   - `IDF_VERSION_MAJOR`
   - `IDF_VERSION_MINOR`
   - `IDF_VERSION_PATCH`
   - `INCLUDE_DEFAULT` (The default value of officially supported targets is 1, otherwise is 0)
+  - `CONFIG_NAME` (config name defined in [](project:#config-rules))
   - environment variables, default to `0` if not set
 - String, must be double-quoted. e.g., `"esp32"`, `"12345"`
 - Integer, support decimal and hex. e.g., `1`, `0xAB`
 - List of strings or integers, or both types at the same time. e.g., `["esp32", 1]`
 
 ### Operators
 
@@ -134,15 +135,15 @@
 One app will be built when:
 
 - The app itself is modified (`.md` files are excluded)
 - Any of the specified `depends_components` in the corresponding manifest file are modified
 - Files that matches any of the specified `depends_filepatterns` in the corresponding manifest file are modified
 - Any of the `build_components` are modified. `build_components` are defined in the `project_description.json`, which is generated by running `idf.py reconfigure` or `idf.py build`
 
-For example, this is an app `exmaple/foo`, which depends on `comp1`, `comp2`, `comp3` and all files under `common_header_files`:
+For example, this is an app `example/foo`, which depends on `comp1`, `comp2`, `comp3` and all files under `common_header_files`:
 
 ```yaml
 examples/foo:
   depends_components:
     - comp1
     - comp2
     - comp3
```

### Comparing `idf_build_apps-1.0.0rc0/idf_build_apps/app.py` & `idf_build_apps-1.0.1/idf_build_apps/app.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/idf_build_apps/config.py` & `idf_build_apps-1.0.1/idf_build_apps/config.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/idf_build_apps/constants.py` & `idf_build_apps-1.0.1/idf_build_apps/constants.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/idf_build_apps/finder.py` & `idf_build_apps-1.0.1/idf_build_apps/finder.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .app import (
     App,
     BuildOrNot,
     CMakeApp,
 )
 from .utils import (
     config_rules_from_str,
+    to_absolute_path,
     to_list,
 )
 
 
 def _get_apps_from_path(
     path,  # type: str
     target,  # type: str
@@ -161,23 +162,26 @@
         if exclude_list:
             LOGGER.warning('--exclude option is ignored when used without --recursive')
 
         return _get_apps_from_path(path, target, build_system, **kwargs)
 
     # The remaining part is for recursive == True
     apps = []
+    # handle the exclude list, since the config file might use linux style, but run in windows
+    exclude_list = [to_absolute_path(p) for p in exclude_list]
     for root, dirs, _ in os.walk(path):
         LOGGER.debug('Entering %s', root)
-        if root in exclude_list:
+        root_path = to_absolute_path(root)
+        if root_path in exclude_list:
             LOGGER.debug('=> Skipping %s (excluded)', root)
             del dirs[:]
             continue
 
-        if root.endswith('managed_components'):  # idf-component-manager
-            LOGGER.debug('=> Skipping %s (managed components)', root)
+        if root_path.parts[-1] == 'managed_components':  # idf-component-manager
+            LOGGER.debug('=> Skipping %s (managed components)', root_path)
             del dirs[:]
             continue
 
         _found_apps = _get_apps_from_path(root, target, build_system, **kwargs)
         if _found_apps:  # root has at least one app
             LOGGER.debug('=> Stop iteration sub dirs of %s since it has apps', root)
             del dirs[:]
```

### Comparing `idf_build_apps-1.0.0rc0/idf_build_apps/log.py` & `idf_build_apps-1.0.1/idf_build_apps/log.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/idf_build_apps/main.py` & `idf_build_apps-1.0.1/idf_build_apps/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,19 +494,15 @@
         '--build-system', default='cmake', choices=['cmake'], help='filter apps by given build system'
     )
     common_args.add_argument(
         '--recursive',
         action='store_true',
         help='Look for apps in the specified paths recursively',
     )
-    common_args.add_argument(
-        '--exclude',
-        nargs='+',
-        help='Ignore specified directory (if --recursive is given)',
-    )
+    common_args.add_argument('--exclude', nargs='+', help='Ignore specified path (if --recursive is given)')
     common_args.add_argument(
         '--work-dir',
         help='If set, the app is first copied into the specified directory, and then built. '
         'If not set, the work directory is the directory of the app. Can expand placeholders',
     )
     common_args.add_argument(
         '--build-dir',
@@ -584,18 +580,17 @@
         'specified modified files.',
     )
     common_args.add_argument(
         '-if',
         '--ignore-app-dependencies-filepatterns',
         nargs='*',
         default=None,
-        help='space-separated list which specifies the file patterns used for ignoring the component dependencies. '
-        'The `depends_components` and `depends_filepatterns` set in the manifest files will be ignored when any of '
-        'the specified file patterns matches any of the modified files. Must be used together with '
-        '--modified-files',
+        help='space-separated list which specifies the file patterns used for ignoring checking the app dependencies. '
+        'The `depends_components` and `depends_filepatterns` set in the manifest files will be ignored when any of the '
+        'specified file patterns matches any of the modified files. Must be used together with --modified-files',
     )
 
     common_args.add_argument(
         '--no-color',
         action='store_true',
         help='enable colored output by default on UNIX-like systems. enable this flag to make the logs uncolored.',
     )
```

### Comparing `idf_build_apps-1.0.0rc0/idf_build_apps/manifest/if_parser.py` & `idf_build_apps-1.0.1/idf_build_apps/manifest/if_parser.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/idf_build_apps/manifest/manifest.py` & `idf_build_apps-1.0.1/idf_build_apps/manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/idf_build_apps/manifest/soc_header.py` & `idf_build_apps-1.0.1/idf_build_apps/manifest/soc_header.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/idf_build_apps/utils.py` & `idf_build_apps-1.0.1/idf_build_apps/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,20 @@
 
 try:
     import typing as t
 except ImportError:
     pass
 
 
+if sys.version_info < (3, 5):
+    import glob2 as glob
+else:
+    import glob
+
+
 class ConfigRule:
     def __init__(self, file_name, config_name):  # type: (str, str) -> None
         """
         ConfigRule represents the sdkconfig file and the config name.
 
         For example:
             - filename='', config_name='default' — represents the default app configuration, and gives it a name
@@ -209,18 +215,21 @@
 
 
 def files_matches_patterns(
     files,  # type: list[str] | str
     patterns,  # type: list[str] | str
     rootpath=None,  # type: str
 ):  # type: (...) -> bool
-    # can't match a absolute pattern with a relative path
+    # can't match an absolute pattern with a relative path
     # change all to absolute paths
     files = [to_absolute_path(f, rootpath) for f in to_list(files)]
     patterns = [to_absolute_path(p, rootpath) for p in to_list(patterns)]
 
+    matched_paths = set()
+    for pat in patterns:
+        matched_paths.update(glob.glob(str(pat), recursive=True))
+
     for f in files:
-        for p in patterns:
-            if f.match(str(p)):
-                return True
+        if str(f) in matched_paths:
+            return True
 
     return False
```

### Comparing `idf_build_apps-1.0.0rc0/pyproject.toml` & `idf_build_apps-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 
 dependencies = [
     "pathlib; python_version < '3.4'",
+    "glob2; python_version < '3.5'",
     "pyparsing",
     "pyyaml",
     "packaging",
     "toml; python_version < '3.11'",
 ]
 
 [project.optional-dependencies]
```

### Comparing `idf_build_apps-1.0.0rc0/tests/conftest.py` & `idf_build_apps-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/tests/test_build.py` & `idf_build_apps-1.0.1/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/tests/test_finder.py` & `idf_build_apps-1.0.1/tests/test_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import logging
 import os
+import tempfile
 from pathlib import (
     Path,
 )
 
 import pytest
 from conftest import (
     create_project,
@@ -181,17 +182,16 @@
             assert filtered_apps == apps
         else:
             assert not filtered_apps
 
     @pytest.mark.parametrize(
         'modified_components, modified_files, could_find_apps',
         [
-            ([], '/foo', True),
             ([], str(IDF_PATH / 'examples' / 'README.md'), False),
-            (None, [str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md')], True),
+            (None, [str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md')], False),
             (
                 [],
                 [
                     str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.md'),
                     str(IDF_PATH / 'examples' / 'get-started' / 'hello_world' / 'a.c'),
                 ],
                 True,
@@ -204,15 +204,14 @@
         assert apps
 
         yaml_file = tmp_path / 'test.yml'
         yaml_file.write_text(
             f'''
 {test_dir}:
     depends_filepatterns:
-        - /foo
         - examples/get-started/hello_world/**
         - examples/foo/**
 ''',
             encoding='utf8',
         )
 
         filtered_apps = find_apps(
@@ -465,7 +464,36 @@
             str(tmp_path / 'test1'),
             'esp32',
             config_rules_str=['sdkconfig.ci=default', 'sdkconfig.ci.*='],
             manifest_files=yaml_file,
         )
         assert len(apps) == 3
         monkeypatch.delenv('TEST_ENV_VAR')
+
+
+@pytest.mark.parametrize(
+    'exclude_list, apps_count',
+    [
+        (['test1'], 3),  # not excluded
+        (['folder1/test2'], 2),
+        (['folder1'], 1),
+        (['folder2/test2'], 2),
+    ],
+)
+def test_find_apps_with_exclude(tmp_path, exclude_list, apps_count):
+    (tmp_path / 'folder1').mkdir()
+    (tmp_path / 'folder2').mkdir()
+
+    create_project('test1', tmp_path / 'folder1')
+    create_project('test2', tmp_path / 'folder1')
+    create_project('test2', tmp_path / 'folder2')
+
+    os.chdir(tmp_path)
+    apps = find_apps(str(tmp_path), 'esp32', recursive=True, exclude_list=exclude_list)
+    assert len(apps) == apps_count
+
+    # or with absolute_path
+    exclude_list = [os.path.abspath(x) for x in exclude_list]
+    tmp_path = os.path.abspath(tmp_path)
+    os.chdir(tempfile.tempdir)
+    apps = find_apps(str(tmp_path), 'esp32', recursive=True, exclude_list=exclude_list)
+    assert len(apps) == apps_count
```

### Comparing `idf_build_apps-1.0.0rc0/tests/test_manifest.py` & `idf_build_apps-1.0.1/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.0rc0/setup.py` & `idf_build_apps-1.0.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 
 install_requires = \
 ['pyparsing', 'pyyaml', 'packaging']
 
 extras_require = \
 {":python_version < '3.11'": ['toml'],
  ":python_version < '3.4'": ['pathlib'],
+ ":python_version < '3.5'": ['glob2'],
  'doc': ['sphinx',
          'sphinx-rtd-theme',
          'sphinx_copybutton',
          'myst-parser',
          'sphinxcontrib-mermaid'],
  'test': ['pytest', 'pytest-cov']}
 
 entry_points = \
 {'console_scripts': ['idf-build-apps = idf_build_apps:main.main']}
 
 setup(name='idf-build-apps',
-      version='1.0.0rc0',
+      version='1.0.1',
       description='Tools for building ESP-IDF related apps.',
       author=None,
       author_email='Fu Hanxi <fuhanxi@espressif.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `idf_build_apps-1.0.0rc0/PKG-INFO` & `idf_build_apps-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-build-apps
-Version: 1.0.0rc0
+Version: 1.0.1
 Summary: Tools for building ESP-IDF related apps.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pathlib; python_version < '3.4'
+Requires-Dist: glob2; python_version < '3.5'
 Requires-Dist: pyparsing
 Requires-Dist: pyyaml
 Requires-Dist: packaging
 Requires-Dist: toml; python_version < '3.11'
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinx-rtd-theme ; extra == "doc"
 Requires-Dist: sphinx_copybutton ; extra == "doc"
```

