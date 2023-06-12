# Comparing `tmp/encode_utils_cli-0.0.4a1.tar.gz` & `tmp/encode_utils_cli-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encode_utils_cli-0.0.4a1.tar", max compression
+gzip compressed data, was "encode_utils_cli-1.0.0a1.tar", max compression
```

## Comparing `encode_utils_cli-0.0.4a1.tar` & `encode_utils_cli-1.0.0a1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/LICENSE
--rw-r--r--   0        0        0      828 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/README.md
--rw-r--r--   0        0        0     2599 2023-05-05 09:18:11.132545 encode_utils_cli-0.0.4a1/pyproject.toml
--rw-r--r--   0        0        0       70 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/__init__.py
--rw-r--r--   0        0        0      177 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/__main__.py
--rw-r--r--   0        0        0      970 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/_cli.py
--rw-r--r--   0        0        0     2087 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/chapt2bmqpyml.py
--rw-r--r--   0        0        0      666 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/frames_denum.py
--rwxr-xr-x   0        0        0     1209 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/mpls2chap.py
--rw-r--r--   0        0        0      427 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/num_frames.py
--rw-r--r--   0        0        0     1163 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/re_chapters.py
--rwxr-xr-x   0        0        0     1042 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/re_titles.py
--rwxr-xr-x   0        0        0      966 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/screens2bm.py
--rw-r--r--   0        0        0       35 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/__init__.py
--rw-r--r--   0        0        0     2012 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/load_mpls.py
--rw-r--r--   0        0        0      312 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/source.py
--rw-r--r--   0        0        0      672 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/timeconv.py
--rw-r--r--   0        0        0     2203 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/vs_screens.py
--rwxr-xr-x   0        0        0      758 2023-05-05 09:17:55.672742 encode_utils_cli-0.0.4a1/src/encode_utils_cli/zones_validator.py
--rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 encode_utils_cli-0.0.4a1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/LICENSE
+-rw-r--r--   0        0        0      809 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/README.md
+-rw-r--r--   0        0        0     2603 2023-06-12 16:13:29.698697 encode_utils_cli-1.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/__init__.py
+-rw-r--r--   0        0        0      177 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/__main__.py
+-rw-r--r--   0        0        0      931 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/_cli.py
+-rw-r--r--   0        0        0     2087 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/chapt2bmqpyml.py
+-rw-r--r--   0        0        0      666 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/frames_denum.py
+-rwxr-xr-x   0        0        0     1164 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/mpls2chap.py
+-rw-r--r--   0        0        0      427 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/num_frames.py
+-rw-r--r--   0        0        0     1163 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/re_chapters.py
+-rwxr-xr-x   0        0        0     1042 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/re_titles.py
+-rwxr-xr-x   0        0        0      966 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/screens2bm.py
+-rw-r--r--   0        0        0       35 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/util/__init__.py
+-rw-r--r--   0        0        0     2012 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/util/load_mpls.py
+-rw-r--r--   0        0        0      312 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/util/source.py
+-rw-r--r--   0        0        0      672 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/util/timeconv.py
+-rw-r--r--   0        0        0     2203 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/vs_screens.py
+-rwxr-xr-x   0        0        0      758 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/zones_validator.py
+-rw-r--r--   0        0        0     1755 1970-01-01 00:00:00.000000 encode_utils_cli-1.0.0a1/PKG-INFO
```

### Comparing `encode_utils_cli-0.0.4a1/LICENSE` & `encode_utils_cli-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4a1/README.md` & `encode_utils_cli-1.0.0a1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # encode-utils-cli
 
 > Encode utils collection
 
 [![PyPI version](https://img.shields.io/pypi/v/encode-utils-cli)](https://pypi.org/project/encode-utils-cli)
-[![CI/CD](https://github.com/DeadNews/encode-utils-cli/actions/workflows/python-vs-app.yml/badge.svg)](https://github.com/DeadNews/encode-utils-cli/actions/workflows/python-vs-app.yml)
+[![Main](https://github.com/DeadNews/encode-utils-cli/actions/workflows/main.yml/badge.svg)](https://github.com/DeadNews/encode-utils-cli/actions/workflows/main.yml)
 [![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/encode-utils-cli/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/encode-utils-cli/main)
 [![codecov](https://codecov.io/gh/DeadNews/encode-utils-cli/branch/main/graph/badge.svg?token=OCZDZIYPMC)](https://codecov.io/gh/DeadNews/encode-utils-cli)
 
 ## Installation
 
 ```sh
 pip install encode-utils-cli
```

### Comparing `encode_utils_cli-0.0.4a1/pyproject.toml` & `encode_utils_cli-1.0.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "encode-utils-cli"
-version = "0.0.4-alpha.1"
+version = "1.0.0-alpha.1"
 description = "Encode utils collection"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/encode-utils-cli"
 repository = "https://github.com/DeadNews/encode-utils-cli"
 keywords = ["cli", "encode", "vapoursynth", "mpls"]
@@ -26,34 +26,34 @@
 vapoursynth = ">=60"
 click = "^8.1.3"
 pyperclip = "^1.8.2"
 pyyaml = "^6.0"
 schema = "^0.7.5"
 tomli = "^2.0.1"
 
-[tool.poetry.group.ci.dependencies]
+[tool.poetry.group.lint.dependencies]
 black = "^23.3.0"
-mypy = "^1.2.0"
+mypy = "^1.3.0"
 poethepoet = "^0.20.0"
-ruff = "^0.0.264"
+ruff = "^0.0.272"
 types-pyyaml = "^6.0.12.9"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.3.1"
-pytest-cov = "^4.0.0"
+pytest = "^7.3.2"
+pytest-cov = "^4.1.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.3"
 mkdocs-click = "^0.8.0"
 
 [tool.poe.tasks]
 ruff = "ruff check ."
 black = "black --check ."
 mypy = "mypy ."
-ci.sequence = ["ruff", "black", "mypy"]
+lint.sequence = ["ruff", "black", "mypy"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.black]
```

### Comparing `encode_utils_cli-0.0.4a1/src/encode_utils_cli/_cli.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from encode_utils_cli.re_chapters import re_chapters
 from encode_utils_cli.re_titles import re_titles
 from encode_utils_cli.screens2bm import screens2bm
 from encode_utils_cli.vs_screens import vs_screens
 from encode_utils_cli.zones_validator import zones_validator
 
 
-@click.group(context_settings={"show_default": True, "help_option_names": ["-h", "--help"]})
+@click.group(context_settings={"show_default": True})
 @click.version_option()
 def cli() -> None:
     """Entrypoint for cli."""
 
 
 cli.add_command(chapt2bmqpyml)
 cli.add_command(frames_denum)
```

### Comparing `encode_utils_cli-0.0.4a1/src/encode_utils_cli/chapt2bmqpyml.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/chapt2bmqpyml.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4a1/src/encode_utils_cli/frames_denum.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/frames_denum.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4a1/src/encode_utils_cli/mpls2chap.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/mpls2chap.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,11 +37,7 @@
         startpos = ep.times[0]
         chapters = [
             f"CHAPTER{index:02d}={seconds2ts((time - startpos) / 45000.0)}\n"
             f"CHAPTER{index:02d}NAME="
             for index, time in enumerate(ep.times)
         ]
         Path(f"{out_dir}/e{number}.txt").write_text("\n".join(chapters))
-
-
-if __name__ == "__main__":
-    mpls2chap()
```

### Comparing `encode_utils_cli-0.0.4a1/src/encode_utils_cli/re_chapters.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/re_chapters.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4a1/src/encode_utils_cli/re_titles.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/re_titles.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4a1/src/encode_utils_cli/screens2bm.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/screens2bm.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/load_mpls.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/util/load_mpls.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4a1/src/encode_utils_cli/util/timeconv.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/util/timeconv.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4a1/src/encode_utils_cli/vs_screens.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/vs_screens.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4a1/src/encode_utils_cli/zones_validator.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/zones_validator.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-0.0.4a1/PKG-INFO` & `encode_utils_cli-1.0.0a1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encode-utils-cli
-Version: 0.0.4a1
+Version: 1.0.0a1
 Summary: Encode utils collection
 Home-page: https://github.com/DeadNews/encode-utils-cli
 License: MIT
 Keywords: cli,encode,vapoursynth,mpls
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.10,<4.0
@@ -25,15 +25,15 @@
 Description-Content-Type: text/markdown
 
 # encode-utils-cli
 
 > Encode utils collection
 
 [![PyPI version](https://img.shields.io/pypi/v/encode-utils-cli)](https://pypi.org/project/encode-utils-cli)
-[![CI/CD](https://github.com/DeadNews/encode-utils-cli/actions/workflows/python-vs-app.yml/badge.svg)](https://github.com/DeadNews/encode-utils-cli/actions/workflows/python-vs-app.yml)
+[![Main](https://github.com/DeadNews/encode-utils-cli/actions/workflows/main.yml/badge.svg)](https://github.com/DeadNews/encode-utils-cli/actions/workflows/main.yml)
 [![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/encode-utils-cli/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/encode-utils-cli/main)
 [![codecov](https://codecov.io/gh/DeadNews/encode-utils-cli/branch/main/graph/badge.svg?token=OCZDZIYPMC)](https://codecov.io/gh/DeadNews/encode-utils-cli)
 
 ## Installation
 
 ```sh
 pip install encode-utils-cli
```

