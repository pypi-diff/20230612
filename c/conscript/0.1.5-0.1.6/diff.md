# Comparing `tmp/conscript-0.1.5.tar.gz` & `tmp/conscript-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conscript-0.1.5.tar", last modified: Thu Oct 20 17:19:35 2022, max compression
+gzip compressed data, was "conscript-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `conscript-0.1.5.tar` & `conscript-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2158 2022-10-20 17:19:17.611557 conscript-0.1.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1975 2022-10-20 17:19:17.611557 conscript-0.1.5/.github/workflows/release.yml
--rw-r--r--   0        0        0       48 2022-10-20 17:19:17.611557 conscript-0.1.5/.gitignore
--rw-r--r--   0        0        0      670 2022-10-20 17:19:17.611557 conscript-0.1.5/CHANGES.md
--rw-r--r--   0        0        0    11323 2022-10-20 17:19:17.611557 conscript-0.1.5/LICENSE
--rw-r--r--   0        0        0     4659 2022-10-20 17:19:17.611557 conscript-0.1.5/README.md
--rw-r--r--   0        0        0     1482 2022-10-20 17:19:17.611557 conscript-0.1.5/RELEASE.md
--rw-r--r--   0        0        0      270 2022-10-20 17:19:17.611557 conscript-0.1.5/conscript/__init__.py
--rw-r--r--   0        0        0     3503 2022-10-20 17:19:17.611557 conscript-0.1.5/conscript/main.py
--rw-r--r--   0        0        0      111 2022-10-20 17:19:17.611557 conscript-0.1.5/mypy.ini
--rw-r--r--   0        0        0     1556 2022-10-20 17:19:17.611557 conscript-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1368 2022-10-20 17:19:17.611557 conscript-0.1.5/scripts/changelog.py
--rw-r--r--   0        0        0     3184 2022-10-20 17:19:17.611557 conscript-0.1.5/tests/conftest.py
--rw-r--r--   0        0        0     4998 2022-10-20 17:19:17.611557 conscript-0.1.5/tests/test_main.py
--rw-r--r--   0        0        0     1728 2022-10-20 17:19:17.611557 conscript-0.1.5/tox.ini
--rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 conscript-0.1.5/setup.py
--rw-r--r--   0        0        0     6018 1970-01-01 00:00:00.000000 conscript-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2010 2023-06-12 16:28:23.906760 conscript-0.1.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2081 2023-06-12 16:28:23.906760 conscript-0.1.6/.github/workflows/release.yml
+-rw-r--r--   0        0        0       48 2023-06-12 16:28:23.906760 conscript-0.1.6/.gitignore
+-rw-r--r--   0        0        0      670 2023-06-12 16:28:23.906760 conscript-0.1.6/CHANGES.md
+-rw-r--r--   0        0        0    11323 2023-06-12 16:28:23.906760 conscript-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4659 2023-06-12 16:28:23.906760 conscript-0.1.6/README.md
+-rw-r--r--   0        0        0     1482 2023-06-12 16:28:23.906760 conscript-0.1.6/RELEASE.md
+-rw-r--r--   0        0        0      270 2023-06-12 16:28:23.906760 conscript-0.1.6/conscript/__init__.py
+-rw-r--r--   0        0        0     3503 2023-06-12 16:28:23.906760 conscript-0.1.6/conscript/main.py
+-rw-r--r--   0        0        0      111 2023-06-12 16:28:23.906760 conscript-0.1.6/mypy.ini
+-rw-r--r--   0        0        0     1600 2023-06-12 16:28:23.906760 conscript-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1368 2023-06-12 16:28:23.906760 conscript-0.1.6/scripts/changelog.py
+-rw-r--r--   0        0        0     3825 2023-06-12 16:28:23.906760 conscript-0.1.6/tests/conftest.py
+-rw-r--r--   0        0        0     5126 2023-06-12 16:28:23.906760 conscript-0.1.6/tests/test_main.py
+-rw-r--r--   0        0        0     1848 2023-06-12 16:28:23.906760 conscript-0.1.6/tox.ini
+-rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 conscript-0.1.6/setup.py
+-rw-r--r--   0        0        0     6069 1970-01-01 00:00:00.000000 conscript-0.1.6/PKG-INFO
```

### Comparing `conscript-0.1.5/.github/workflows/ci.yml` & `conscript-0.1.6/.github/workflows/ci.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 name: CI
 on: [push, pull_request]
 jobs:
   org-check:
     name: Check GitHub Organization
     if: ${{ github.repository_owner == 'jsirois' }}
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     steps:
       - name: Noop
         run: "true"
   checks:
     name: TOXENV=${{ matrix.tox-env }}
     needs: org-check
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     strategy:
       matrix:
         include:
           - check-name: Lint
             python-version: 3.9
             tox-env: lint
           - check-name: Types
@@ -34,28 +34,24 @@
           tox-env: ${{ matrix.tox-env }}
   unit-tests:
     name: (${{ matrix.os }}) TOXENV=py${{ matrix.python-version[0] }}${{ matrix.python-version[1] }}
     needs: org-check
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: [[2, 7], [3, 5], [3, 6], [3, 7], [3, 8], [3, 9], [3, 10], [3, 11, "0-beta.3"]]
-        os: [ubuntu-20.04, macos-10.15]
+        python-version: [[2, 7], [3, 7], [3, 8], [3, 9], [3, 10], [3, 11], [3, 12, "0-beta.2"]]
+        os: [ubuntu-22.04, macos-12]
         exclude:
-          - os: macos-10.15
-            python-version: [3, 5]
-          - os: macos-10.15
-            python-version: [3, 6]
-          - os: macos-10.15
+          - os: macos-12
             python-version: [3, 7]
-          - os: macos-10.15
+          - os: macos-12
             python-version: [3, 8]
-          - os: macos-10.15
+          - os: macos-12
             python-version: [3, 9]
-          - os: macos-10.15
+          - os: macos-12
             python-version: [3, 10]
     steps:
       - name: Checkout
         uses: actions/checkout@v3
       - name: Setup Python ${{ join(matrix.python-version, '.') }}
         uses: actions/setup-python@v4
         with:
```

### Comparing `conscript-0.1.5/.github/workflows/release.yml` & `conscript-0.1.6/.github/workflows/release.yml`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     inputs:
       tag:
         description: The tag to manually run a deploy for.
         required: true
 jobs:
   org_check:
     if: ${{ github.repository_owner == 'jsirois' }}
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     steps:
       - name: Noop
         run: "true"
   determine-tag:
     name: Determine the release tag to operate against.
     needs: org_check
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     outputs:
       release-tag: ${{ steps.determine-tag.outputs.release-tag }}
       release-version: ${{ steps.determine-tag.outputs.release-version }}
     steps:
       - name: Determine Tag
         id: determine-tag
         run: |
@@ -37,25 +37,30 @@
           else
             echo "::error::Release tag '${RELEASE_TAG}' must match 'v\d+.\d+.\d+'."
             exit 1
           fi
   pypi:
     name: Publish sdist and wheel to PyPI
     needs: [org_check, determine-tag]
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     environment: Release
+    permissions:
+      id-token: write
     steps:
       - name: Checkout ${{ needs.determine-tag.outputs.release-tag }}
         uses: actions/checkout@v3
         with:
           ref: ${{ needs.determine-tag.outputs.release-tag }}
       - name: Setup Python 3.9
         uses: actions/setup-python@v4
         with:
           python-version: 3.9
-      - name: Publish ${{ needs.determine-tag.outputs.release-tag }}
+      - name: Package ${{ needs.determine-tag.outputs.release-tag }}
         uses: pantsbuild/actions/run-tox@e63d2d0e3c339bdffbe5e51e7c39550e3bc527bb
-        env:
-          FLIT_USERNAME: ${{ secrets.PYPI_USERNAME }}
-          FLIT_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
         with:
-          tox-env: publish
+          tox-env: package
+      - name: Publish ${{ needs.determine-tag.outputs.release-tag }}
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          print-hash: true
+          verbose: true
+
```

### Comparing `conscript-0.1.5/CHANGES.md` & `conscript-0.1.6/CHANGES.md`

 * *Files identical despite different names*

### Comparing `conscript-0.1.5/LICENSE` & `conscript-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `conscript-0.1.5/README.md` & `conscript-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `conscript-0.1.5/RELEASE.md` & `conscript-0.1.6/RELEASE.md`

 * *Files identical despite different names*

### Comparing `conscript-0.1.5/conscript/main.py` & `conscript-0.1.6/conscript/main.py`

 * *Files identical despite different names*

### Comparing `conscript-0.1.5/pyproject.toml` & `conscript-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,18 @@
   "Programming Language :: Python :: 3.5",
   "Programming Language :: Python :: 3.6",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Utilities",
 ]
-requires-python = ">=2.7,<3.12,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*"
+requires-python = ">=2.7,<3.13,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*"
 requires = [
   "setuptools; python_version <= '3.5'",
   "importlib-metadata; python_version == '3.6' or python_version == '3.7'",
 ]
 
 [tool.flit.scripts]
 conscript = "conscript.main:main"
```

### Comparing `conscript-0.1.5/scripts/changelog.py` & `conscript-0.1.6/scripts/changelog.py`

 * *Files identical despite different names*

### Comparing `conscript-0.1.5/tests/conftest.py` & `conscript-0.1.6/tests/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -43,15 +43,34 @@
         )
         args = [sys.executable, "-m", "pex", project_root_dir]
         args.extend(requirements)
         args.extend(["-c", "conscript", "-o", pex])
         subprocess.check_call(args)
         return pex
 
-    return create_conscript_pex
+    def create_conscript_zipapp(requirements):
+        # type: (Iterable[str]) -> str
+        pyz = os.path.join(
+            str(
+                tmpdir_factory.mktemp(
+                    hashlib.sha1(json.dumps(sorted(list(requirements))).encode("utf8")).hexdigest()
+                )
+            ),
+            "conscript.pyz",
+        )
+        args = [sys.executable, "-m", "shiv", project_root_dir]
+        args.extend(requirements)
+        args.extend(["-c", "conscript", "-o", pyz])
+        subprocess.check_call(args)
+        return pyz
+
+    if sys.version_info[:2] <= (3, 11):
+        return create_conscript_pex
+    else:
+        return create_conscript_zipapp
 
 
 @pytest.fixture(scope="session")
 def create_project(tmpdir_factory):
     # type: (Any) -> CreateProject
 
     def create_project(
```

### Comparing `conscript-0.1.5/tests/test_main.py` & `conscript-0.1.6/tests/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,22 +90,22 @@
               -h, --help     show this help message and exit
               -V, --version  show program's version number and exit
             """
         ).format(options_header=OPTIONS_HEADER, argv0=os.path.basename(foo_bar_conscript))
         == get_output(args=[foo_bar_conscript, "foo", "-h"])
     )
 
-    assert (
-        "usage: {argv0} [-h] [PROGRAM]\n"
-        "{argv0}: error: argument PROGRAM: invalid choice: 'baz' (choose from {programs})\n"
-    ).format(
-        argv0=os.path.basename(foo_bar_conscript),
-        programs=", ".join("'{}'".format(program) for program in EXPECTED_PROGRAMS),
-    ) == get_output(
-        args=[foo_bar_conscript, "baz"], expected_returncode=2
+    assert get_output(args=[foo_bar_conscript, "baz"], expected_returncode=2).startswith(
+        (
+            "usage: {argv0} [-h] [PROGRAM]\n"
+            "{argv0}: error: argument PROGRAM: invalid choice: 'baz' (choose from {programs}"
+        ).format(
+            argv0=os.path.basename(foo_bar_conscript),
+            programs=", ".join("'{}'".format(program) for program in EXPECTED_PROGRAMS),
+        )
     )
 
 
 def test_busybox(foo_bar_conscript):
     # type: (str) -> Any
     basedir = os.path.dirname(foo_bar_conscript)
 
@@ -115,38 +115,43 @@
 
     bar_symlink = os.path.join(basedir, "bar")
     os.symlink(foo_bar_conscript, bar_symlink)
     assert_version(args=[bar_symlink], expected_version=BAR_VERSION)
 
     non_program_symlink = os.path.join(basedir, "baz")
     os.symlink(foo_bar_conscript, non_program_symlink)
+
+    output = get_output(args=[non_program_symlink, "-h"])
     # N.B.: We insert a string of '*' and later replace these with spaces to work around `dedent`
     # stripping away significant whitespace indentation performed by the help formatter.
-    assert (
+    assert output.startswith(
         dedent(
             """\
             usage: baz [-h] [PROGRAM]
 
             A baz busy box.
 
             positional arguments:
               PROGRAM     The program to execute.
             **************
                           The following programs are available:
                           + {programs}
+            """
+        )
+        .replace("*", " ")
+        .format(programs="\n              + ".join(EXPECTED_PROGRAMS))
+    )
+    assert output.endswith(
+        dedent(
+            """\
 
             {options_header}:
               -h, --help  Show this help message and exit.
             """
-        )
-        .replace("*", " ")
-        .format(
-            programs="\n              + ".join(EXPECTED_PROGRAMS), options_header=OPTIONS_HEADER
-        )
-        == get_output(args=[non_program_symlink, "-h"])
+        ).format(options_header=OPTIONS_HEADER)
     )
 
 
 def test_repl(foo_bar_conscript):
     # type: (str) -> Any
     process = subprocess.Popen(
         args=[foo_bar_conscript],
```

### Comparing `conscript-0.1.5/tox.ini` & `conscript-0.1.6/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -9,18 +9,22 @@
   typecheck
   py27
   py35
   py36
   py37
   py38
   py39
+  py310
+  py311
+  py312
 
 [testenv]
 deps =
-  pex==2.1.90
+  pex==2.1.137; python_version < "3.12"
+  shiv==1.0.3; python_version >= "3.6"
   pytest==4.6.11; python_version < "3.6"
   pytest==6.2.5; python_version >= "3.6"
 commands =
   pytest {posargs:-vvs}
 
 [_fmt_and_lint]
 basepython = python3
@@ -61,14 +65,15 @@
   mypy --python-version 3.5 .
   mypy --python-version 3.6 .
   mypy --python-version 3.7 .
   mypy --python-version 3.8 .
   mypy --python-version 3.9 .
   mypy --python-version 3.10 .
   mypy --python-version 3.11 .
+  mypy --python-version 3.12 .
 
 [_flit]
 basepython = python3
 deps =
   flit==3.2.0
   Pygments==2.9.0
```

### Comparing `conscript-0.1.5/setup.py` & `conscript-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 {":python_version <= '3.5'": ['setuptools'],
  ":python_version == '3.6' or python_version == '3.7'": ['importlib-metadata']}
 
 entry_points = \
 {'console_scripts': ['conscript = conscript.main:main']}
 
 setup(name='conscript',
-      version='0.1.5',
+      version='0.1.6',
       description='Conscript console scripts in your own Swiss Army Knife.',
       author='John Sirois',
       author_email='john.sirois@gmail.com',
       url='https://github.com/jsirois/conscript',
       packages=packages,
       package_data=package_data,
       extras_require=extras_require,
       entry_points=entry_points,
-      python_requires='>=2.7,<3.12,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*',
+      python_requires='>=2.7,<3.13,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*',
      )
```

### Comparing `conscript-0.1.5/PKG-INFO` & `conscript-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: conscript
-Version: 0.1.5
+Version: 0.1.6
 Summary: Conscript console scripts in your own Swiss Army Knife.
 Home-page: https://github.com/jsirois/conscript
 Author: John Sirois
 Author-email: john.sirois@gmail.com
-Requires-Python: >=2.7,<3.12,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=2.7,<3.13,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Requires-Dist: setuptools; python_version <= '3.5'
 Requires-Dist: importlib-metadata; python_version == '3.6' or python_version == '3.7'
 Project-URL: Changelog, https://github.com/jsirois/conscript/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/jsirois/conscript/blob/main/README.md
 
 # Conscript: console scripts in your own Swiss Army Knife.
```

