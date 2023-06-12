# Comparing `tmp/hyfi-0.4.0.tar.gz` & `tmp/hyfi-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.4.0.tar", max compression
+gzip compressed data, was "hyfi-0.5.0.tar", max compression
```

## Comparing `hyfi-0.4.0.tar` & `hyfi-0.5.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1071 2023-05-06 04:23:10.578319 hyfi-0.4.0/LICENSE
--rw-r--r--   0        0        0     1632 2023-05-06 04:23:10.578319 hyfi-0.4.0/README.md
--rw-r--r--   0        0        0     4212 2023-05-06 04:23:37.290506 hyfi-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2708 2023-05-06 04:23:10.578319 hyfi-0.4.0/src/hyfi/__cli__.py
--rw-r--r--   0        0        0      331 2023-05-06 04:23:10.578319 hyfi-0.4.0/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-05-06 04:23:37.230506 hyfi-0.4.0/src/hyfi/_version.py
--rw-r--r--   0        0        0        0 2023-05-06 04:23:10.578319 hyfi-0.4.0/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-05-06 04:23:37.230506 hyfi-0.4.0/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-05-06 04:23:10.578319 hyfi-0.4.0/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       83 2023-05-06 04:23:10.578319 hyfi-0.4.0/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      167 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/conf/cmd/cpcfg.yaml
--rw-r--r--   0        0        0      320 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      552 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      807 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      293 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       21 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/config/__init__.py
--rw-r--r--   0        0        0    14151 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/config/batch.py
--rw-r--r--   0        0        0    19859 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/env.py
--rw-r--r--   0        0        0    12903 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/hydra.py
--rw-r--r--   0        0        0        0 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/image/__init__.py
--rw-r--r--   0        0        0     8474 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/image/collage.py
--rw-r--r--   0        0        0     4341 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/image/motion.py
--rw-r--r--   0        0        0     2556 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/image/plot.py
--rw-r--r--   0        0        0     3358 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/image/utils.py
--rw-r--r--   0        0        0        0 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/io/__init__.py
--rw-r--r--   0        0        0     7152 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/io/cached_path.py
--rw-r--r--   0        0        0    12802 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/io/file.py
--rw-r--r--   0        0        0    26828 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/main.py
--rw-r--r--   0        0        0        0 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/py.typed
--rw-r--r--   0        0        0        0 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0      111 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/batch/__init__.py
--rw-r--r--   0        0        0     2934 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/batch/apply.py
--rw-r--r--   0        0        0     2046 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/batch/apply_batch.py
--rw-r--r--   0        0        0    17469 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/batch/batcher.py
--rw-r--r--   0        0        0     1206 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/cached_path/__init__.py
--rw-r--r--   0        0        0    14396 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/cached_path/cache_file.py
--rw-r--r--   0        0        0     1110 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/cached_path/common.py
--rw-r--r--   0        0        0     1923 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/cached_path/file_lock.py
--rw-r--r--   0        0        0     3440 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/cached_path/meta.py
--rw-r--r--   0        0        0     3326 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/cached_path/progress.py
--rw-r--r--   0        0        0     1460 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2999 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1244 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/cached_path/testing.py
--rw-r--r--   0        0        0     4834 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/cached_path/version.py
--rw-r--r--   0        0        0     6131 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/copier.py
--rw-r--r--   0        0        0     2281 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/env.py
--rw-r--r--   0        0        0    10202 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1046 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3726 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     5234 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     1074 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    10003 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     2123 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/pipe.py
--rw-r--r--   0        0        0     5481 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/tools.py
--rw-r--r--   0        0        0      154 2023-05-06 04:23:10.582319 hyfi-0.4.0/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 hyfi-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-12 08:47:30.230064 hyfi-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1632 2023-06-12 08:47:30.230064 hyfi-0.5.0/README.md
+-rw-r--r--   0        0        0     4515 2023-06-12 08:47:58.534763 hyfi-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3596 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0      331 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-12 08:47:58.450761 hyfi-0.5.0/src/hyfi/_version.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-12 08:47:58.450761 hyfi-0.5.0/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      167 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/cmd/cpcfg.yaml
+-rw-r--r--   0        0        0      320 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      552 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      701 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      293 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      717 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      496 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/path/__default__.yaml
+-rw-r--r--   0        0        0     1518 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      669 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       21 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/config/__init__.py
+-rw-r--r--   0        0        0    13966 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/config/batch.py
+-rw-r--r--   0        0        0    24289 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/env.py
+-rw-r--r--   0        0        0    12839 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/hydra.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/image/__init__.py
+-rw-r--r--   0        0        0     8383 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/image/collage.py
+-rw-r--r--   0        0        0     4318 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/image/motion.py
+-rw-r--r--   0        0        0     2494 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/image/plot.py
+-rw-r--r--   0        0        0     3313 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/image/utils.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/io/__init__.py
+-rw-r--r--   0        0        0     7015 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/io/cached_path.py
+-rw-r--r--   0        0        0    12468 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/io/file.py
+-rw-r--r--   0        0        0    28486 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/main.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/batch/__init__.py
+-rw-r--r--   0        0        0     2885 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/batch/apply.py
+-rw-r--r--   0        0        0     1997 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/batch/apply_batch.py
+-rw-r--r--   0        0        0    16580 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/batch/batcher.py
+-rw-r--r--   0        0        0     1206 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/common.py
+-rw-r--r--   0        0        0     1923 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3440 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1244 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/version.py
+-rw-r--r--   0        0        0     6131 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/copier.py
+-rw-r--r--   0        0        0     5603 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0     9920 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1064 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3595 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     4129 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     1986 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0     9760 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     2022 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/pipe.py
+-rw-r--r--   0        0        0     5466 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/tools.py
+-rw-r--r--   0        0        0      154 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 hyfi-0.5.0/PKG-INFO
```

### Comparing `hyfi-0.4.0/LICENSE` & `hyfi-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.4.0/README.md` & `hyfi-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-0.4.0/pyproject.toml` & `hyfi-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.4.0"
+version = "0.5.0"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
@@ -38,17 +38,28 @@
 optional = true
 
 [tool.poetry.group.ipython.dependencies]
 # A list of all of the optional dependencies, some of which are included in the
 # below `extras`. They can be opted into by apps.
 ipython = "<=8.12.0"
 ipython-autotime = "^0.3.1"
+ipywidgets = "^8.0.6"
 
 [tool.poetry.extras]
-ipython = ["ipython", "ipython-autotime"]
+ipython = ["ipython", "ipython-autotime", "ipywidgets"]
+
+[tool.poetry.group.mkdocs]
+optional = true
+
+[tool.poetry.group.mkdocs.dependencies]
+mkdocs-material = "^9.1.15"
+markdown-include = "^0.8.1"
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
+mkdocs-material-extensions = ">=1.1"
+pymdown-extensions = ">=9.9.1"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `hyfi-0.4.0/src/hyfi/__cli__.py` & `hyfi-0.5.0/src/hyfi/__cli__.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,52 +12,76 @@
 
 
 __config_path__ = "conf"
 __config_name__ = "config"
 
 
 def cmd(**args):
-    """Run the command defined in the config file"""
+    """
+    Run the command defined in the config file
+    Args
+        args : dict Arguments to pass to HyFI.
+    """
     HyFI.run(args)
 
 
 def about(**args):
-    """Print the about information"""
+    """
+    Print the about information for Hyfi.
+    This is a wrapper around _about which takes a HyfiConfig as an argument
+    """
     cfg = HyfiConfig(**args)
     _about(cfg)
 
 
 def run_copy(**args):
-    """Copy all config files in the config directory to the current working directory"""
+    """
+    Copy all config files to the current working directory.
+    This is a wrapper around HyfiConfig to allow us to pass arguments to it.
+    """
     cfg = HyfiConfig(**args)
     cfg = HyFI.to_dict(cfg.copier)
     with Copier(**cfg) as worker:
         worker.run_copy()
 
 
 def cli_main(cfg: DictConfig) -> None:
-    """Main function for the command line interface"""
-    hyfi = HyfiConfig(**cfg)
+    """
+    Main function for the command line interface.
+    Initializes Hydra and instantiates the class.
+    Prints the configuration to standard out if verbose is set to True
+
+    Args:
+        cfg: Configuration dictionary to be used for instantiation
+
+    Returns:
+        None if everything went fine otherwise an error is raised to indicate the reason for the failure ( s )
+    """
+    hyfi = HyfiConfig(**cfg)  # type: ignore
     verbose = hyfi.verbose
     app_name = hyfi.about.name
     print_config = hyfi.print_config
     print_resolved_config = hyfi.print_resolved_config
 
+    # Print out the command line interface for the application.
     if verbose:
-        print("## Command Line Interface for %s ##" % app_name)
+        print(f"## Command Line Interface for {app_name} ##")
     HyFI.initialize(cfg)
 
+    # Print the configuration to the console.
     if print_config:
+        # Prints the configuration to the console.
         if print_resolved_config:
             logger.info("## hydra configuration resolved ##")
             HyFI.pprint(cfg)
         else:
             logger.info("## hydra configuration ##")
             print(HyFI.to_yaml(cfg))
 
+    # Prints out the working directory and original working directory.
     if verbose:
         logger.info(f"Hydra working directory : {os.getcwd()}")
         logger.info(f"Orig working directory  : {hydra.utils.get_original_cwd()}")
 
     HyFI.instantiate(cfg)
 
     HyFI.terminate()
@@ -65,27 +89,31 @@
 
 def hydra_main(
     config_path: Optional[str] = __config_path__,
     config_name: Optional[str] = __config_name__,
 ) -> None:
     """
     Main function for the command line interface of Hydra
-    :param config_path: The config path, a directory where Hydra will search for
+
+    Args:
+        config_path: The config path, a directory where Hydra will search for
                         config files. This path is added to Hydra's searchpath.
                         Relative paths are interpreted relative to the declaring python
                         file. Alternatively, you can use the prefix `pkg://` to specify
                         a python package to add to the searchpath.
                         If config_path is None no directory is added to the Config search path.
-    :param config_name: The name of the config (usually the file name without the .yaml extension)
+        config_name: The name of the config (usually the file name without the .yaml extension)
     """
+    # Returns the path to the config file.
     if config_path is None:
         config_path = __about__.config_path
     hydra.main(
         config_path=config_path,
         config_name=config_name,
         version_base=__hydra_version_base__,
     )(cli_main)()
 
 
+# Run the command line interface
 if __name__ == "__main__":
     """Run the command line interface"""
     hydra_main()
```

### Comparing `hyfi-0.4.0/src/hyfi/conf/copier/conf.yaml` & `hyfi-0.5.0/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.4.0/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.5.0/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.4.0/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.5.0/src/hyfi/conf/mode/__init__.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 logging_level: ${oc.env:HYFI_LOG_LEVEL,WARNING}
 
 hydra:
   job:
     name: ${project.project_name}
     chdir: true
   run:
-    dir: ${project.path.logs}/hydra/${hydra.job.name}/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
+    dir: ${project.path.project_logs}/hydra/${hydra.job.name}/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
   sweep:
-    dir: ${project.path.logs}/hydra/${hydra.job.name}/multiruns/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
+    dir: ${project.path.project_logs}/hydra/${hydra.job.name}/multiruns/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
     subdir: ${hydra.job.num}
   verbose: false
   job_logging:
     handlers:
       console:
         level: ${hydra.job_logging.root.level}
       file:
```

### Comparing `hyfi-0.4.0/src/hyfi/config/batch.py` & `hyfi-0.5.0/src/hyfi/config/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 from ..utils.lib import ensure_import_module
 
 logger = getLogger(__name__)
 
 
 class PathConfig(BaseModel):
     task_name: str = "default-task"
-    root: str = None
-    batch_name: str = None
-    verbose: bool = False
+    task_root: str = ""
+    batch_name: str = ""
 
     class Config:
         extra = "ignore"
 
     def __init__(self, **data: Any):
         if not data:
             data = _compose("path=__batch__")
@@ -28,15 +27,15 @@
                 "There are no arguments to initilize a config, using default config."
             )
         super().__init__(**data)
 
     @property
     def root_dir(self):
         # return as an absolute path
-        return Path(self.root).absolute()
+        return Path(self.task_root).absolute()
 
     @property
     def output_dir(self):
         return self.root_dir / "outputs"
 
     @property
     def batch_dir(self):
@@ -95,18 +94,15 @@
             )
         super().__init__(**data)
         self.init_batch_num()
 
     def init_batch_num(self):
         if self.batch_num is None:
             num_files = len(list(self.config_dir.glob(self.config_filepattern)))
-            if self.resume_latest:
-                self.batch_num = num_files - 1
-            else:
-                self.batch_num = num_files
+            self.batch_num = num_files - 1 if self.resume_latest else num_files
         if self.verbose:
             logger.info(
                 f"Init batch - Batch name: {self.batch_name}, Batch num: {self.batch_num}"
             )
 
     @validator("seed")
     def _validate_seed(cls, v, values):
@@ -116,18 +112,15 @@
             if values.get("verbose"):
                 logger.info(f"Setting seed to {seed}")
             return seed
         return v
 
     @validator("output_extention")
     def _validate_output_extention(cls, v):
-        if v:
-            return v.strip(".")
-        else:
-            return ""
+        return v.strip(".") if v else ""
 
     @property
     def batch_dir(self):
         batch_dir = self.output_dir / self.batch_name
         batch_dir.mkdir(parents=True, exist_ok=True)
         return batch_dir
 
@@ -277,15 +270,15 @@
 
     @property
     def log_dir(self):
         return self.project.path.log_dir
 
     @property
     def cache_dir(self):
-        cache_dir = Path(self.project.path.cache)
+        cache_dir = Path(self.project.path.global_cache)
         if cache_dir is None:
             cache_dir = self.output_dir / ".cache"
             cache_dir.mkdir(parents=True, exist_ok=True)
         return Path(cache_dir)
 
     @property
     def library_dir(self):
@@ -427,35 +420,31 @@
             self._config_ = config
         logger.info(f"Saving config to {self.batch.config_filepath}")
         cfg = _to_dict(self.config)
         if exclude is None:
             exclude = self.__config__.exclude
 
         if include:
-            args = {}
             if isinstance(include, str):
                 include = [include]
-            for key in include:
-                args[key] = cfg[key]
+            args = {key: cfg[key] for key in include}
         else:
             args = cfg
             if exclude:
                 if isinstance(exclude, str):
                     exclude = [exclude]
                 for key in exclude:
                     args.pop(key, None)
         _save(args, self.batch.config_filepath)
         self.save_settings(exclude=exclude)
         return self.batch.config_filename
 
     def save_settings(self, exclude=None, exclude_none=True):
         def dumper(obj):
-            if isinstance(obj, DictConfig):
-                return _to_dict(obj)
-            return str(obj)
+            return _to_dict(obj) if isinstance(obj, DictConfig) else str(obj)
 
         if exclude is None:
             exclude = self.__config__.exclude
         config = self.dict(exclude=exclude, exclude_none=exclude_none)
         if self.verbose:
             logger.info(f"Saving config to {self.batch.config_jsonpath}")
         _save_json(config, self.batch.config_jsonpath, default=dumper)
```

### Comparing `hyfi-0.4.0/src/hyfi/env.py` & `hyfi-0.5.0/src/hyfi/env.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import os
+from enum import Enum
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import hydra
 from omegaconf import DictConfig, ListConfig, OmegaConf, SCMode
 from pydantic import BaseModel, BaseSettings, SecretStr, root_validator, validator
 from pydantic.env_settings import SettingsSourceCallable
 
 from .utils.batch import batcher
-from .utils.env import load_dotenv
+from .utils.env import _check_and_set_value, expand_posix_vars, load_dotenv
 from .utils.logging import getLogger, setLogger
 from .utils.notebook import is_notebook, load_extentions, set_matplotlib_formats
 
 logger = getLogger(__name__)
 
 __hydra_version_base__ = "1.2"
 
+DictKeyType = Union[str, bytes, int, Enum, float, bool]
+
 
 def __version__():
     """Returns the version of HyFI"""
     from ._version import __version__
 
     return __version__
 
@@ -40,30 +43,30 @@
         throw_on_resolution_failure=throw_on_resolution_failure,
         throw_on_missing=throw_on_missing,
     )
 
 
 def _to_dict(
     cfg: Any,
-):
+) -> Any:
     if isinstance(cfg, dict):
         cfg = _to_config(cfg)
     if isinstance(cfg, (DictConfig, ListConfig)):
         return OmegaConf.to_container(
             cfg,
             resolve=True,
             throw_on_missing=False,
             structured_config_mode=SCMode.DICT,
         )
     return cfg
 
 
 def _to_config(
     cfg: Any,
-):
+) -> Union[DictConfig, ListConfig]:
     return OmegaConf.create(cfg)
 
 
 class AboutConfig(BaseModel):
     """About Configuration"""
 
     __package_name__: str = "hyfi"
@@ -125,46 +128,46 @@
 
     def __init__(
         self,
         config_name: str = "__init__",
         **data: Any,
     ):
         if not data:
-            data = _compose(
-                f"joblib={config_name}", config_module=__about__.config_module
-            )
             logger.debug(
                 "There are no arguments to initilize a config, using default config."
             )
+            data = _compose(
+                f"joblib={config_name}", config_module=__about__.config_module
+            )  # type: ignore
         super().__init__(config_name=config_name, **data)
 
     def init_backend(
         self,
     ):
         """Initialize the backend for joblib"""
-        backend = self.distributed_framework.backend
-
         if self.distributed_framework.initialize:
             backend_handle = None
-            if backend == "ray":
-                import ray
-
-                ray_cfg = {"num_cpus": self.distributed_framework.num_workers}
-                logger.info(f"initializing ray with {ray_cfg}")
-                ray.init(**ray_cfg)
-                backend_handle = ray
+            backend = self.distributed_framework.backend
 
-            elif backend == "dask":
-                from dask.distributed import Client
+            if backend == "dask":
+                from dask.distributed import Client  # type: ignore
 
                 dask_cfg = {"n_workers": self.distributed_framework.num_workers}
                 logger.info(f"initializing dask client with {dask_cfg}")
                 client = Client(**dask_cfg)
                 logger.debug(client)
 
+            elif backend == "ray":
+                import ray  # type: ignore
+
+                ray_cfg = {"num_cpus": self.distributed_framework.num_workers}
+                logger.info(f"initializing ray with {ray_cfg}")
+                ray.init(**ray_cfg)
+                backend_handle = ray
+
             batcher.batcher_instance = batcher.Batcher(
                 backend_handle=backend_handle, **self.batcher.dict()
             )
             logger.info(f"initialized batcher with {batcher.batcher_instance}")
         self.__initilized__ = True
 
     def stop_backend(self):
@@ -173,112 +176,156 @@
         if batcher.batcher_instance:
             logger.info("stopping batcher")
             del batcher.batcher_instance
 
         logger.info("stopping distributed framework")
         if self.distributed_framework.initialize:
             if backend == "ray":
-                import ray
+                try:
+                    import ray  # type: ignore
+
+                    if ray.is_initialized():
+                        ray.shutdown()
+                        logger.info("shutting down ray")
+                except ImportError:
+                    logger.warning("ray is not installed")
+
+            elif backend == "dask":
+                try:
+                    from dask.distributed import Client  # type: ignore
 
-                if ray.is_initialized():
-                    ray.shutdown()
-                    logger.info("shutting down ray")
-
-            # elif modin_engine == 'dask':
-            #     from dask.distributed import Client
-
-            #     if Client.initialized():
-            #         client.close()
-            #         log.info(f'shutting down dask client')
+                    if Client.initialized():
+                        Client.close()
+                        logger.info("shutting down dask client")
+                except ImportError:
+                    logger.warning("dask is not installed")
 
 
 class PathConfig(BaseModel):
     config_name: str = "__init__"
-    dotenv_path: str = None
-    workspace: str = None
-    project: str = "hyfi-default"
-    data: str = None
-    home: str = None
-    hyfi: str = None
-    resources: str = None
-    runtime: str = None
-    archive: str = None
-    corpus: str = None
-    datasets: str = None
-    logs: str = None
-    models: str = None
-    outputs: str = None
-    cache: str = None
-    tmp: str = None
-    library: str = None
-    verbose: bool = False
+    # internal paths for hyfi
+    home: str = ""
+    hyfi: str = ""
+    resources: str = ""
+    runtime: str = ""
+    # global paths
+    global_workspace_root: str = ""
+    global_data_root: str = ""
+    global_archive: str = ""
+    global_datasets: str = ""
+    global_models: str = ""
+    global_modules: str = ""
+    global_library: str = ""
+    global_cache: str = ""
+    global_tmp: str = ""
+    # project specific paths
+    project_root: str = ""
+    project_data_root: str = ""
+    project_archive: str = ""
+    project_datasets: str = ""
+    project_models: str = ""
+    project_modules: str = ""
+    project_outputs: str = ""
+    project_logs: str = ""
+    project_library: str = ""
+    project_cache: str = ""
+    project_tmp: str = ""
 
     class Config:
         extra = "allow"
         arbitrary_types_allowed = True
 
     def __init__(
         self,
         config_name: str = "__init__",
         **data: Any,
     ):
+        """
+        Initialize the config. This is the base implementation of __init__. You can override this in your own subclass if you want to customize the initilization of a config by passing a keyword argument ` data `.
+
+        Args:
+                config_name: The name of the config to initialize
+                data: The data to initialize
+        """
+        # Initialize the config module.
         if not data:
-            data = _compose(
-                f"path={config_name}", config_module=__about__.config_module
-            )
             logger.debug(
-                "There are no arguments to initilize a config, using default config."
+                "There are no arguments to initilize a config, using default config %s",
+                config_name,
             )
+            data = _compose(
+                f"path={config_name}", config_module=__about__.config_module
+            )  # type: ignore
         super().__init__(config_name=config_name, **data)
 
     @property
     def log_dir(self):
-        Path(self.logs).mkdir(parents=True, exist_ok=True)
-        return Path(self.logs).absolute()
+        """
+        Create and return the path to the log directory. This is a convenience method for use in unit tests that want to ensure that the log directory exists and is accessible to the user.
+
+
+        Returns:
+                absolute path to the log directory for the project ( including parent directories
+        """
+        Path(self.project_logs).mkdir(parents=True, exist_ok=True)
+        return Path(self.project_logs).absolute()
 
     @property
     def cache_dir(self):
-        Path(self.cache).mkdir(parents=True, exist_ok=True)
-        return Path(self.cache).absolute()
+        """
+        Create and return the directory where cache files are stored. This is useful for debugging and to ensure that we don't accidentally delete the cache files when there are too many files in the cache.
+
+
+        Returns:
+                absolute path to the cache directory for this test run
+        """
+        Path(self.global_cache).mkdir(parents=True, exist_ok=True)
+        return Path(self.global_cache).absolute()
 
 
 class DotEnvConfig(BaseSettings):
     """Environment variables for HyFI"""
 
+    config_name: str = "__init__"
+
+    DOTENV_FILENAME: Optional[str] = ".env"
+    DOTENV_DIR: Optional[str] = ""
+    DOTENV_PATH: Optional[str] = ""
     # Internal
-    HYFI_WORKSPACE_ROOT: Optional[str]
-    HYFI_PROJECT_NAME: Optional[str]
-    HYFI_TASK_NAME: Optional[str]
-    HYFI_PROJECT_ROOT: Optional[str]
-    HYFI_DATA_ROOT: Optional[str]
-    HYFI_RESOURCE_DIR: Optional[str]
-    HYFI_LOG_LEVEL: Optional[str]
-    HYFI_VERBOSE: Optional[Union[bool, str, int]]
-    NUM_WORKERS: Optional[int]
-    CACHED_PATH_CACHE_ROOT: Optional[str]
+    HYFI_RESOURCE_DIR: Optional[str] = ""
+    HYFI_GLOBAL_WORKSPACE_ROOT: Optional[str] = ""
+    HYFI_GLOBAL_DATA_ROOT: Optional[str] = ""
+    HYFI_PROJECT_NAME: Optional[str] = ""
+    HYFI_TASK_NAME: Optional[str] = ""
+    HYFI_PROJECT_ROOT: Optional[str] = ""
+    HYFI_PROJECT_DATA_ROOT: Optional[str] = ""
+    HYFI_LOG_LEVEL: Optional[str] = "WARNING"
+    HYFI_VERBOSE: Optional[Union[bool, str, int]] = False
+    NUM_WORKERS: Optional[int] = 1
+    CACHED_PATH_CACHE_ROOT: Optional[str] = ""
     # For other packages
-    CUDA_DEVICE_ORDER: Optional[str]
-    CUDA_VISIBLE_DEVICES: Optional[str]
-    WANDB_PROJECT: Optional[str]
-    WANDB_DISABLED: Optional[str]
-    WANDB_DIR: Optional[str]
-    WANDB_NOTEBOOK_NAME: Optional[str]
-    WANDB_SILENT: Optional[Union[bool, str]]
-    LABEL_STUDIO_SERVER: Optional[str]
+    CUDA_DEVICE_ORDER: Optional[str] = "PCI_BUS_ID"
+    CUDA_VISIBLE_DEVICES: Optional[str] = ""
+    WANDB_PROJECT: Optional[str] = ""
+    WANDB_DISABLED: Optional[str] = ""
+    WANDB_DIR: Optional[str] = ""
+    WANDB_NOTEBOOK_NAME: Optional[str] = ""
+    WANDB_SILENT: Optional[Union[bool, str]] = False
+    LABEL_STUDIO_SERVER: Optional[str] = ""
     KMP_DUPLICATE_LIB_OK: Optional[str] = "True"
-    TOKENIZERS_PARALLELISM: Optional[bool] = False
+    TOKENIZERS_PARALLELISM: Optional[Union[bool, str]] = False
     # API Keys and Tokens
-    WANDB_API_KEY: Optional[SecretStr]
-    HUGGING_FACE_HUB_TOKEN: Optional[SecretStr]
-    OPENAI_API_KEY: Optional[SecretStr]
-    ECOS_API_KEY: Optional[SecretStr]
-    FRED_API_KEY: Optional[SecretStr]
-    NASDAQ_API_KEY: Optional[SecretStr]
-    HF_USER_ACCESS_TOKEN: Optional[SecretStr]
-    LABEL_STUDIO_USER_TOKEN: Optional[SecretStr]
+    WANDB_API_KEY: Optional[SecretStr] = None
+    HUGGING_FACE_HUB_TOKEN: Optional[SecretStr] = None
+    OPENAI_API_KEY: Optional[SecretStr] = None
+    ECOS_API_KEY: Optional[SecretStr] = None
+    FRED_API_KEY: Optional[SecretStr] = None
+    NASDAQ_API_KEY: Optional[SecretStr] = None
+    HF_USER_ACCESS_TOKEN: Optional[SecretStr] = None
+    LABEL_STUDIO_USER_TOKEN: Optional[SecretStr] = None
 
     class Config:
         env_prefix = ""
         env_nested_delimiter = "__"
         case_sentive = False
         env_file = ".env"
         env_file_encoding = "utf-8"
@@ -293,118 +340,153 @@
             file_secret_settings: SettingsSourceCallable,
         ) -> Tuple[SettingsSourceCallable, ...]:
             load_dotenv()
             return env_settings, file_secret_settings, init_settings
 
     @root_validator()
     def _check_and_set_values(cls, values):
-        workspace = values.get("HYFI_WORKSPACE_ROOT")
-        project = values.get("HYFI_PROJECT_NAME")
-        if workspace is not None and project is not None:
-            project_dir = os.path.join(workspace, "projects", project)
-            values["HYFI_PROJECT_ROOT"] = project_dir
+        global_workspace_root = values.get("HYFI_GLOBAL_WORKSPACE_ROOT")
+        global_data_root = values.get("HYFI_GLOBAL_DATA_ROOT")
+        if global_workspace_root and not global_data_root:
+            global_data_root = os.path.join(global_workspace_root, "data")
+            values["HYFI_GLOBAL_DATA_ROOT"] = global_data_root
+        project_name = values.get("HYFI_PROJECT_NAME")
+        project_root = values.get("HYFI_PROJECT_ROOT")
+        dotenv_dir = values.get("DOTENV_DIR")
+        if not project_root:
+            if global_workspace_root and project_name:
+                project_root = os.path.join(
+                    global_workspace_root, "projects", project_name
+                )
+                values["HYFI_PROJECT_ROOT"] = project_root
+            elif dotenv_dir and Path(dotenv_dir).is_dir():
+                project_root = dotenv_dir
+                values["HYFI_PROJECT_ROOT"] = project_root
+        project_data_root = values.get("HYFI_PROJECT_DATA_ROOT")
+        if project_root and not project_data_root:
+            project_data_root = os.path.join(project_root, "workspace")
+            values["HYFI_PROJECT_DATA_ROOT"] = project_data_root
+
         for k, v in values.items():
             if v is not None:
                 old_value = os.getenv(k.upper())
                 if old_value is None or old_value != str(v):
                     os.environ[k.upper()] = str(v)
                     logger.debug(f"Set environment variable {k.upper()}={v}")
         return values
 
 
 class ProjectConfig(BaseModel):
     """Project Config"""
 
     config_name: str = "__init__"
     project_name: str = "hyfi-project"
-    task_name: str = None
-    workspace_root: str = None
-    project_root: str = None
-    description: str = None
+    task_name: str = ""
+    project_description: str = ""
+    project_root: str = ""
+    project_data_root: str = ""
+    global_workspace_root: str = ""
+    global_data_root: str = ""
     use_huggingface_hub: bool = False
     use_wandb: bool = False
-    verbose: bool = False
+    verbose: Union[bool, int] = False
     # Config Classes
-    dotenv: DotEnvConfig = None
-    joblib: JobLibConfig = None
-    path: PathConfig = None
+    dotenv: DotEnvConfig = None  # type: ignore
+    joblib: JobLibConfig = None  # type: ignore
+    path: PathConfig = None  # type: ignore
 
     class Config:
         extra = "allow"
         arbitrary_types_allowed = True
 
     def __init__(
         self,
         config_name: str = "__init__",
         **data: Any,
     ):
         if not data:
-            data = _compose(
-                f"project={config_name}", config_module=__about__.config_module
-            )
             logger.debug(
                 "There are no arguments to initilize a config, using default config."
             )
+            data = _compose(
+                f"project={config_name}", config_module=__about__.config_module
+            )  # type: ignore
         super().__init__(config_name=config_name, **data)
 
     @validator("project_name", allow_reuse=True)
     def _validate_project_name(cls, v):
         if v is None:
             raise ValueError("Project name must be specified.")
         return v
 
     @property
-    def workspace_dir(self):
-        return Path(self.path.workspace)
+    def environ(self):
+        return os.environ
 
     @property
-    def project_dir(self):
-        return Path(self.path.project)
+    def project_data_dir(self):
+        if self.path is None:
+            raise ValueError("Path object not initialized")
+        _p = Path(self.path.project_data_root)
+        _p.mkdir(parents=True, exist_ok=True)
+        return _p.absolute()
 
     @property
-    def version(self):
-        return __about__.version
+    def project_dir(self):
+        if self.path is None:
+            raise ValueError("Path object not initialized")
+        _p = Path(self.path.project_root)
+        _p.mkdir(parents=True, exist_ok=True)
+        return _p.absolute()
 
     def init_project(self):
         self.dotenv = DotEnvConfig()
         if self.path is None:
             self.path = PathConfig()
         if self.joblib is None:
             self.joblib = JobLibConfig()
 
         if self.dotenv.HYFI_VERBOSE is not None:
-            self.verbose = self.dotenv.HYFI_VERBOSE
-        self.dotenv.HYFI_DATA_ROOT = str(self.path.data)
+            self.verbose = int(self.dotenv.HYFI_VERBOSE)
+        self.dotenv.HYFI_GLOBAL_WORKSPACE_ROOT = str(self.path.global_workspace_root)
+        self.dotenv.HYFI_GLOBAL_DATA_ROOT = str(self.path.global_data_root)
         self.dotenv.CACHED_PATH_CACHE_ROOT = str(self.path.cache_dir / "cached_path")
-        wandb_dir = str(self.path.log_dir)
-        self.dotenv.WANDB_DIR = wandb_dir
+        self.init_wandb()
+        if self.use_huggingface_hub:
+            self.init_huggingface_hub()
+
+    def init_wandb(self):
+        if self.path is None:
+            raise ValueError("Path object not initialized")
+        if self.dotenv is None:
+            raise ValueError("DotEnv object not initialized")
+
+        self.dotenv.WANDB_DIR = str(self.path.log_dir)
         project_name = self.project_name.replace("/", "-").replace("\\", "-")
         self.dotenv.WANDB_PROJECT = project_name
         task_name = self.task_name.replace("/", "-").replace("\\", "-")
         notebook_name = self.path.log_dir / f"{task_name}-nb"
         notebook_name.mkdir(parents=True, exist_ok=True)
         self.dotenv.WANDB_NOTEBOOK_NAME = str(notebook_name)
         self.dotenv.WANDB_SILENT = str(not self.verbose)
         if self.use_wandb:
             try:
-                import wandb
+                import wandb  # type: ignore
 
                 wandb.init(project=self.project_name)
             except ImportError:
                 logger.warning(
                     "wandb is not installed, please install it to use wandb."
                 )
-        if self.use_huggingface_hub:
-            self.init_huggingface_hub()
 
     def init_huggingface_hub(self):
         """Initialize huggingface_hub"""
         try:
-            from huggingface_hub import notebook_login
-            from huggingface_hub.hf_api import HfFolder
+            from huggingface_hub import notebook_login  # type: ignore
+            from huggingface_hub.hf_api import HfFolder  # type: ignore
         except ImportError:
             logger.warning(
                 "huggingface_hub is not installed, please install it to use huggingface_hub."
             )
             return
 
         self.dotenv = DotEnvConfig()
@@ -421,42 +503,32 @@
             else:
                 logger.info(
                     "huggingface_hub.notebook_login() is only available in notebook,"
                     "set HUGGING_FACE_HUB_TOKEN manually"
                 )
 
 
-def _check_and_set_value(key, value):
-    """Check and set value to environment variable"""
-    env_key = key.upper()
-    if value is not None:
-        old_value = os.getenv(env_key, "")
-        if str(old_value).lower() != str(value).lower():
-            os.environ[env_key] = str(value)
-            logger.debug("Set environment variable %s=%s", env_key, str(value))
-    return value
-
-
 class HyfiConfig(BaseModel):
     """HyFI config primary class"""
 
     hyfi_config_path: str = __about__.config_path
     hyfi_config_module: str = __about__.config_module
-    hyfi_user_config_path: str = None
+    hyfi_user_config_path: str = ""
 
     debug_mode: bool = False
     print_config: bool = False
     print_resolved_config: bool = False
     verbose: bool = False
     logging_level: str = "WARNING"
 
-    hydra: DictConfig = None
+    hydra: Optional[DictConfig] = None
 
     about: AboutConfig = AboutConfig()
-    project: ProjectConfig = None
+    project: Optional[ProjectConfig] = None
+    copier: Optional[DictConfig] = None
 
     __version__: str = __version__()
     __initilized__: bool = False
 
     class Config:
         arbitrary_types_allowed = True
         underscore_attrs_are_private = True
@@ -487,42 +559,50 @@
 
     def __init__(self, **data: Any):
         super().__init__(**data)
         # self.about = __about__
 
     def init_workspace(
         self,
-        workspace=None,
-        project=None,
-        task=None,
-        log_level=None,
-        autotime=True,
-        retina=True,
-        verbose=None,
+        project_name: str = "",
+        task_name: str = "",
+        project_root: str = "",
+        project_data_root: str = "",
+        global_workspace_root: str = "",
+        global_data_root: str = "",
+        log_level: str = "",
+        autotime: bool = True,
+        retina: bool = True,
+        verbose: Union[bool, int] = False,
         **kwargs,
     ):
-        """Initialize project in notebook"""
         envs = DotEnvConfig(HYFI_VERBOSE=verbose)
-        if isinstance(workspace, str):
-            envs.HYFI_WORKSPACE_ROOT = workspace
-        if isinstance(project, str):
-            envs.HYFI_PROJECT_NAME = project
-        if isinstance(task, str):
-            envs.HYFI_TASK_NAME = task
-        if isinstance(log_level, str):
+        if project_name:
+            envs.HYFI_PROJECT_NAME = expand_posix_vars(project_name)
+        if task_name:
+            envs.HYFI_TASK_NAME = expand_posix_vars(task_name)
+        if project_root:
+            envs.HYFI_PROJECT_ROOT = expand_posix_vars(project_root)
+        if project_data_root:
+            envs.HYFI_PROJECT_DATA_ROOT = expand_posix_vars(project_data_root)
+        if global_workspace_root:
+            envs.HYFI_GLOBAL_WORKSPACE_ROOT = expand_posix_vars(global_workspace_root)
+        if global_data_root:
+            envs.HYFI_GLOBAL_DATA_ROOT = expand_posix_vars(global_data_root)
+        if log_level:
             envs.HYFI_LOG_LEVEL = log_level
             setLogger(log_level)
             logger.setLevel(log_level)
         if autotime:
             load_extentions(exts=["autotime"])
         if retina:
             set_matplotlib_formats("retina")
         self.initialize()
 
-    def initialize(self, config: Union[DictConfig, Dict] = None):
+    def initialize(self, config: Union[DictConfig, Dict, None] = None):
         """Initialize hyfi config"""
         if self.__initilized__:
             return
         if config is None:
             config = _compose(
                 overrides=["+project=__init__"], config_module=__about__.config_module
             )
@@ -531,72 +611,75 @@
         if "project" not in config:
             logger.warning(
                 "No project config found, skip project config initialization."
             )
             return
         self.project = ProjectConfig(**config["project"])
         self.project.init_project()
-        self.project.joblib.init_backend()
+        if self.project.joblib:
+            self.project.joblib.init_backend()
         self.__initilized__ = True
 
     def terminate(self):
         """Terminate hyfi config"""
         if not self.__initilized__:
             return
-        if self.project is not None:
+        if self.project and self.project.joblib:
             self.project.joblib.stop_backend()
         self.__initilized__ = False
 
     def __repr__(self):
         return f"HyFIConfig(project={self.project})"
 
     def __str__(self):
         return self.__repr__()
 
     @property
     def app_version(self):
-        return self.about.app_version
+        return self.about.version
 
 
 __global_config__ = HyfiConfig()
 
 
 class Dummy:
     def __call__(self, *args, **kwargs):
         return Dummy()
 
 
 def _compose(
-    config_group: str = None,
-    overrides: List[str] = [],
+    config_group: Union[str, None] = None,
+    overrides: Union[List[str], None] = None,
     *,
     return_as_dict: bool = False,
     throw_on_resolution_failure: bool = True,
     throw_on_missing: bool = False,
-    config_name: str = None,
-    config_module: str = None,
+    config_name: Union[str, None] = None,
+    config_module: Union[str, None] = None,
     verbose: bool = False,
-) -> Union[DictConfig, Dict]:
+) -> Union[DictConfig, Dict]:  # sourcery skip: low-code-quality
     """
     Compose your configuration from config groups and overrides (overrides=["override_name"])
 
     :param overrides: List of overrides to apply
     :param config_group: Config group name to select ('config_group=name')
     :param return_as_dict: Return the composed config as a dict
     :param throw_on_resolution_failure: Throw if resolution fails
     :param throw_on_missing: Throw if a config is missing
     :param config_name: Name of the config to compose
     :param verbose: Print the composed config
 
     :return: The composed config
     """
+    if overrides is None:
+        overrides = []
     config_module = config_module or __global_config__.hyfi_config_module
     # if verbose:
     logger.info("config_module: %s", config_module)
-    is_initialized = hydra.core.global_hydra.GlobalHydra.instance().is_initialized()
+    is_initialized = hydra.core.global_hydra.GlobalHydra.instance().is_initialized()  # type: ignore
     if config_group:
         _task = config_group.split("=")
         if len(_task) == 2:
             key, value = _task
         else:
             key = _task[0]
             value = "default"
@@ -615,22 +698,20 @@
         cfg = _select(
             cfg,
             key=key,
             default=None,
             throw_on_missing=False,
             throw_on_resolution_failure=False,
         )
-        if cfg is not None:
-            overide = config_group
-        else:
-            overide = f"+{config_group}"
-        if overrides:
-            overrides.append(overide)
-        else:
-            overrides = [overide]
+        override = config_group if cfg is not None else f"+{config_group}"
+        if isinstance(override, str):
+            if overrides:
+                overrides.append(override)
+            else:
+                overrides = [override]
     # if verbose:
     logger.info(f"compose config with overrides: {overrides}")
     if is_initialized:
         if verbose:
             logger.info("Hydra is already initialized")
         cfg = hydra.compose(config_name=config_name, overrides=overrides)
     else:
@@ -644,10 +725,8 @@
             cfg,
             key=key,
             default=None,
             throw_on_missing=throw_on_missing,
             throw_on_resolution_failure=throw_on_resolution_failure,
         )
     logger.debug("Composed config: %s", OmegaConf.to_yaml(cfg))
-    if return_as_dict and isinstance(cfg, DictConfig):
-        return _to_dict(cfg)
-    return cfg
+    return _to_dict(cfg) if return_as_dict and isinstance(cfg, DictConfig) else cfg
```

### Comparing `hyfi-0.4.0/src/hyfi/hydra.py` & `hyfi-0.5.0/src/hyfi/hydra.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,39 +74,41 @@
 
 
 def _load(file_: Union[str, Path, IO[Any]]) -> Union[DictConfig, ListConfig]:
     return OmegaConf.load(file_)
 
 
 def _save(config: Any, f: Union[str, Path, IO[Any]], resolve: bool = False) -> None:
-    os.makedirs(os.path.dirname(f), exist_ok=True)
+    os.makedirs(os.path.dirname(str(f)), exist_ok=True)
     OmegaConf.save(config, f, resolve=resolve)
 
 
 def _save_json(
     json_dict: dict,
     f: Union[str, Path, IO[Any]],
     indent=4,
     ensure_ascii=False,
     default=None,
     **kwargs,
 ):
+    f = str(f)
     os.makedirs(os.path.dirname(f), exist_ok=True)
     with open(f, "w") as f:
         json.dump(
             json_dict,
             f,
             indent=indent,
             ensure_ascii=ensure_ascii,
             default=default,
             **kwargs,
         )
 
 
 def _load_json(f: Union[str, Path, IO[Any]], **kwargs) -> dict:
+    f = str(f)
     with open(f, "r") as f:
         return json.load(f, **kwargs)
 
 
 def _update(_dict, _overrides):
     import collections.abc
 
@@ -167,15 +169,15 @@
         _config_ = [_config_]
     for _cfg_ in _config_:
         cfg = _select(config, _cfg_)
         _instantiate(cfg)
 
 
 def _partial(
-    config: Any = None, config_group: str = None, *args: Any, **kwargs: Any
+    config: Any = None, config_group: Union[str, None] = None, *args: Any, **kwargs: Any
 ) -> Any:
     if config is None and config_group is None:
         logger.warning("No config specified")
         return None
     elif config_group is not None:
         config = _compose(config_group=config_group)
     kwargs[SpecialKeys.PARTIAL] = True
@@ -298,18 +300,15 @@
     _functions_ = cfg[SpecialKeys.FUNC]
     fn = _partial(_functions_[_name_])
     if _name_ in cfg:
         _parms = cfg[_name_]
         _parms = {**_parms, **parms}
     else:
         _parms = parms
-    if SpecialKeys.EXEC in _parms:
-        _exec_ = _parms.pop(SpecialKeys.EXEC)
-    else:
-        _exec_ = True
+    _exec_ = _parms.pop(SpecialKeys.EXEC) if SpecialKeys.EXEC in _parms else True
     if _exec_:
         if callable(fn):
             if return_function:
                 logger.info(f"Returning function {fn}")
                 return fn
             logger.info(f"Executing function {fn} with parms {_parms}")
             return fn(**_parms)
@@ -335,15 +334,15 @@
 
 OmegaConf.register_new_resolver("__hyfi_path__", __hyfi_path__)
 OmegaConf.register_new_resolver("__search_package_path__", __search_package_path__)
 OmegaConf.register_new_resolver("__home_path__", __home_path__)
 OmegaConf.register_new_resolver("today", today)
 OmegaConf.register_new_resolver("to_datetime", strptime)
 OmegaConf.register_new_resolver("iif", lambda cond, t, f: t if cond else f)
-OmegaConf.register_new_resolver("alt", lambda val, alt: val if val else alt)
+OmegaConf.register_new_resolver("alt", lambda val, alt: val or alt)
 OmegaConf.register_new_resolver("randint", random.randint, use_cache=True)
 OmegaConf.register_new_resolver("get_method", hydra.utils.get_method)
 OmegaConf.register_new_resolver("get_original_cwd", getcwd)
 OmegaConf.register_new_resolver("exists", exists)
 OmegaConf.register_new_resolver("join_path", join_path)
 OmegaConf.register_new_resolver("mkdir", mkdir)
 OmegaConf.register_new_resolver("dirname", os.path.dirname)
@@ -388,15 +387,11 @@
     return _to_dict(value)
 
 
 def _ensure_kwargs(_kwargs, _fn):
     from inspect import getfullargspec as getargspec
 
     if callable(_fn):
-        kwargs = {}
         args = getargspec(_fn).args
         logger.info(f"args of {_fn}: {args}")
-        for k, v in _kwargs.items():
-            if k in args:
-                kwargs[k] = v
-        return kwargs
+        return {k: v for k, v in _kwargs.items() if k in args}
     return _kwargs
```

### Comparing `hyfi-0.4.0/src/hyfi/image/collage.py` & `hyfi-0.5.0/src/hyfi/image/collage.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     """
 
     if not isinstance(images_or_uris, list):
         images_or_uris = [images_or_uris]
     images_or_uris = [
         uri if isinstance(uri, Image.Image) else str(uri) for uri in images_or_uris
     ]
-    if len(images_or_uris) < 1:
+    if not images_or_uris:
         log.info("No images provided")
         return None
 
     if max_images is not None:
         max_images = min(max_images, len(images_or_uris))
     else:
         max_images = len(images_or_uris)
@@ -143,20 +143,20 @@
     ax = plt.gca()
     plt.grid(False)
     if xlabel is None and ylabel is None:
         plt.axis("off")
     if title is not None:
         title = "\n".join(
             sum(
-                [
+                (
                     textwrap.wrap(
                         t, width=int(collage.width / 15 * 12 / title_fontsize)
                     )
                     for t in title.split("\n")
-                ],
+                ),
                 [],
             )
         )
         ax.set_title(title, fontsize=title_fontsize, color=fg_fontcolor)
     if xlabel is not None:
         # plt.xlabel(xlabel, fontdict={"fontsize": xlabel_fontsize})
         ax.set_xlabel(xlabel, fontsize=xlabel_fontsize, color=fg_fontcolor)
@@ -275,15 +275,12 @@
 def gallery(array, ncols=7):
     """
     Create a gallery of images from a numpy array.
     """
     nindex, height, width, intensity = array.shape
     nrows = nindex // ncols
     assert nindex == nrows * ncols
-    # want result.shape = (height*nrows, width*ncols, intensity)
-    result = (
+    return (
         array.reshape(nrows, ncols, height, width, intensity)
         .swapaxes(1, 2)
         .reshape(height * nrows, width * ncols, intensity)
     )
-
-    return result
```

### Comparing `hyfi-0.4.0/src/hyfi/image/motion.py` & `hyfi-0.5.0/src/hyfi/image/motion.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,15 @@
         if image_filepaths is None:
             image_filepaths = sorted(
                 get_filepaths(filename_patterns, base_dir=base_dir)
             )
         if not image_filepaths:
             logger.warning("no images found")
             return
-        frames = [Image.open(image) for image in image_filepaths]
-        if len(frames) > 0:
+        if frames := [Image.open(image) for image in image_filepaths]:
             frame_one = frames[0]
             frame_one.save(
                 output_filepath,
                 format="GIF",
                 append_images=frames,
                 save_all=True,
                 duration=duration,
```

### Comparing `hyfi-0.4.0/src/hyfi/image/plot.py` & `hyfi-0.5.0/src/hyfi/image/plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,18 +28,15 @@
             fontname = fontname or "NanumGothic.ttf"
             if fontname.lower().startswith("nanum"):
                 fontpath = os.path.join("/usr/share/fonts/truetype/nanum/", fontname)
             else:
                 fontpath = os.path.join("/usr/share/fonts/truetype/", fontname)
         if fontpath and not Path(fontpath).is_file():
             paths = find_font_file(fontname)
-            if len(paths) > 0:
-                fontpath = paths[0]
-            else:
-                fontpath = None
+            fontpath = paths[0] if len(paths) > 0 else None
         if verbose:
             logger.info(f"Font path: {fontpath}")
 
     if fontpath is None or not Path(fontpath).is_file():
         fontname = None
         fontpath = None
         logger.warning(f"Font file does not exist at {fontpath}")
@@ -53,23 +50,23 @@
     else:
         font_manager.fontManager.addfont(fontpath)
         fontname = font_manager.FontProperties(fname=fontpath).get_name()
 
         if set_font_for_matplot and fontname:
             rc("font", family=fontname)
             plt.rcParams["axes.unicode_minus"] = False
-            font_family = plt.rcParams["font.family"]
             if verbose:
+                font_family = plt.rcParams["font.family"]
                 logger.info(f"font family: {font_family}")
         if verbose:
             logger.info(f"font name: {fontname}")
     return fontname, fontpath
 
 
 def find_font_file(query):
     """Find font file by query string"""
-    matches = list(
+    return list(
         filter(
-            lambda path: query in os.path.basename(path), font_manager.findSystemFonts()
+            lambda path: query in os.path.basename(path),
+            font_manager.findSystemFonts(),
         )
     )
-    return matches
```

### Comparing `hyfi-0.4.0/src/hyfi/image/utils.py` & `hyfi-0.5.0/src/hyfi/image/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,12 +107,8 @@
 
     return imgs
 
 
 def get_image_font(fontname=None, fontsize=12):
     """Get font for PIL image."""
     fontname, fontpath = get_plot_font(set_font_for_matplot=False, fontname=fontname)
-    if fontpath:
-        font = ImageFont.truetype(fontpath, fontsize)
-    else:
-        font = None
-    return font
+    return ImageFont.truetype(fontpath, fontsize) if fontpath else None
```

### Comparing `hyfi-0.4.0/src/hyfi/io/cached_path.py` & `hyfi-0.5.0/src/hyfi/io/cached_path.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,17 +35,15 @@
     Returns:
         str: Path to the cached file or its parent directory, depending on the 'return_parent_dir' parameter.
     """
     if url_or_filename is None:
         return None
     if verbose:
         logger.info(
-            "caching path: {}, extract_archive: {}, force_extract: {}, cache_dir: {}".format(
-                url_or_filename, extract_archive, force_extract, cache_dir
-            )
+            f"caching path: {url_or_filename}, extract_archive: {extract_archive}, force_extract: {force_extract}, cache_dir: {cache_dir}"
         )
 
     try:
         if url_or_filename.startswith("gd://"):
             _path = cached_gdown(
                 url_or_filename,
                 verbose=verbose,
@@ -78,19 +76,15 @@
             _parent_dir = Path(_path).parent
         elif Path(_path).is_dir():
             _parent_dir = Path(_path)
         else:
             logger.warning(f"Unknown path: {_path}")
             return None
 
-        if return_parent_dir:
-            return _parent_dir.as_posix()
-        else:
-            return _path
-
+        return _parent_dir.as_posix() if return_parent_dir else _path
     except Exception as e:
         logger.error(e)
         return None
 
 
 def cached_gdown(
     url, verbose=False, extract_archive=None, force_extract=False, cache_dir=None
@@ -144,20 +138,19 @@
             path=cache_path.as_posix(),
             quiet=not verbose,
         )
 
         if extract_archive:
             extraction_path, files = extractall(cache_path, force_extract=force_extract)
 
-            if fname and files:
-                for f in files:
-                    if f.endswith(fname):
-                        return f
-            else:
+            if not fname or not files:
                 return extraction_path
+            for f in files:
+                if f.endswith(fname):
+                    return f
         return cache_path
 
     else:
         logger.warning(f"Unknown url: {url}")
         return None
 
 
@@ -184,22 +177,20 @@
         opener, mode = tarfile.open, "r"
     elif path.endswith(".tar.gz") or path.endswith(".tgz"):
         opener, mode = tarfile.open, "r:gz"
     elif path.endswith(".tar.bz2") or path.endswith(".tbz"):
         opener, mode = tarfile.open, "r:bz2"
     else:
         logger.warning(
-            "Could not extract '%s' as no appropriate " "extractor is found" % path
+            f"Could not extract '{path}' as no appropriate extractor is found"
         )
         return path, None
 
     def namelist(f):
-        if isinstance(f, ZipFile):
-            return f.namelist()
-        return [m.path for m in f.members]
+        return f.namelist() if isinstance(f, ZipFile) else [m.path for m in f.members]
 
     def filelist(f):
         files = []
         for fname in namelist(f):
             fname = os.path.join(to, fname)
             files.append(fname)
         return files
```

### Comparing `hyfi-0.4.0/src/hyfi/io/file.py` & `hyfi-0.5.0/src/hyfi/io/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,18 +70,15 @@
         if os.path.exists(filepath):
             if Path(filepath).is_file():
                 filepaths.append(filepath)
         else:
             if os.path.dirname(file) != "":
                 _dir = os.path.dirname(file)
                 file = os.path.basename(file)
-                if base_dir:
-                    base_dir = os.path.join(base_dir, _dir)
-                else:
-                    base_dir = _dir
+                base_dir = os.path.join(base_dir, _dir) if base_dir else _dir
             filepaths += glob_re(file, base_dir, recursive=recursive)
     filepaths = [fp for fp in filepaths if Path(fp).is_file()]
     if verbose:
         logger.info(f"Processing [{len(filepaths)}] files from {filename_patterns}")
 
     return filepaths
 
@@ -145,24 +142,18 @@
             df_each = data[df_name]
             if isinstance(columns, list):
                 _columns = [c for c in columns if c in df_each.columns]
                 df_each = df_each[_columns]
             if add_key_as_name:
                 df_each[name_column] = df_name
             dfs.append(df_each)
-        if len(dfs) > 0:
-            return pd.concat(dfs, ignore_index=ignore_index)
-        else:
-            return None
+        return pd.concat(dfs, ignore_index=ignore_index) if dfs else None
     elif isinstance(data, list):
         logger.info(f"Concatenating {len(data)} dataframes")
-        if len(data) > 0:
-            return pd.concat(data, ignore_index=ignore_index)
-        else:
-            return None
+        return pd.concat(data, ignore_index=ignore_index) if len(data) > 0 else None
     else:
         logger.warning("Warning: data is not a dict")
         return data
 
 
 def load_data(filename, base_dir=None, filetype=None, verbose=False, **kwargs):
     """Load data from a file or a list of files"""
@@ -224,19 +215,15 @@
         filepath = filename
     else:
         fileinfo = os.path.splitext(filename)
         filename = fileinfo[0]
         filetype = fileinfo[1] if len(fileinfo) > 1 else filetype
         filetype = "." + filetype.replace(".", "")
         filename = f"{filename}{filetype}"
-        if base_dir is not None:
-            filepath = os.path.join(base_dir, filename)
-        else:
-            filepath = filename
-
+        filepath = filename if base_dir is None else os.path.join(base_dir, filename)
         if not os.path.exists(filepath):
             logger.warning(f"File {filepath} does not exist")
             return None
     if verbose:
         logger.info(f"Loading data from {filepath}")
     with elapsed_timer(format_time=True) as elapsed:
         if "csv" in filetype or "tsv" in filetype:
@@ -253,15 +240,15 @@
             data = pd.read_parquet(filepath, engine=engine)
         else:
             raise ValueError("filetype must be .csv or .parquet")
         if isinstance(columns, list):
             columns = [c for c in columns if c in data.columns]
             data = data[columns]
         if verbose:
-            logger.info(" >> elapsed time to load data: {}".format(elapsed()))
+            logger.info(f" >> elapsed time to load data: {elapsed()}")
     return data
 
 
 def save_data(
     data: Union[pd.DataFrame, dict],
     filename: str,
     base_dir: str = None,
@@ -277,18 +264,15 @@
     filename = fileinfo[0]
     filetype = fileinfo[1] if len(fileinfo) > 1 else filetype
     filetype = "." + filetype.replace(".", "")
     if suffix is not None:
         filename = f"{filename}-{suffix}{filetype}"
     else:
         filename = f"{filename}{filetype}"
-    if base_dir is not None:
-        filepath = os.path.join(base_dir, filename)
-    else:
-        filepath = filename
+    filepath = filename if base_dir is None else os.path.join(base_dir, filename)
     base_dir = os.path.dirname(filepath)
     filename = os.path.basename(filepath)
     os.makedirs(base_dir, exist_ok=True)
 
     if isinstance(data, dict):
         for k, v in data.items():
             save_data(
@@ -313,15 +297,15 @@
             elif "parquet" in filetype:
                 compression = kwargs.get("compression", "gzip")
                 engine = kwargs.get("engine", "pyarrow")
                 data.to_parquet(filepath, compression=compression, engine=engine)
             else:
                 raise ValueError("filetype must be .csv or .parquet")
             if verbose:
-                logger.info(" >> elapsed time to save data: {}".format(elapsed()))
+                logger.info(f" >> elapsed time to save data: {elapsed()}")
     else:
         raise ValueError(f"Unsupported data type: {type(data)}")
 
 
 def read(uri, mode="rb", encoding=None, head=None, **kwargs) -> bytes:
     """Read data from a file or url"""
     uri = str(uri)
@@ -357,18 +341,15 @@
     """Check if path is a directory"""
     _path = os.path.join(a, *p)
     return Path(_path).is_dir()
 
 
 def check_path(_path: str, alt_path: str = None) -> str:
     """Check if path exists, return alt_path if not"""
-    if os.path.exists(_path):
-        return _path
-    else:
-        return alt_path
+    return _path if os.path.exists(_path) else alt_path
 
 
 def mkdir(_path: str) -> str:
     """Create directory if it does not exist"""
     if _path is None:
         return None
     Path(_path).mkdir(parents=True, exist_ok=True)
@@ -381,14 +362,11 @@
         return False
     _path = os.path.join(a, *p)
     return os.path.exists(_path)
 
 
 def join_path(a, *p) -> str:
     """Join path components intelligently."""
-    if p and p[0] is not None:
-        p = [str(_p) for _p in p]
-        if a is None:
-            return os.path.join(*p)
-        return os.path.join(a, *p)
-    else:
+    if not p or p[0] is None:
         return a
+    p = [str(_p) for _p in p]
+    return os.path.join(*p) if a is None else os.path.join(a, *p)
```

### Comparing `hyfi-0.4.0/src/hyfi/main.py` & `hyfi-0.5.0/src/hyfi/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,26 +32,25 @@
     _to_dict,
     _to_yaml,
     _update,
     _viewsource,
 )
 from .io.cached_path import cached_path
 from .io.file import exists, is_dir, is_file, join_path, mkdir
-from .utils.env import get_osenv, load_dotenv, set_osenv
+from .utils.env import expand_posix_vars, get_osenv, load_dotenv, set_osenv
 from .utils.func import (
     dict_product,
     dict_to_dataframe,
     records_to_dataframe,
     to_dateparm,
     to_datetime,
     to_numeric,
 )
 from .utils.google import mount_google_drive
 from .utils.gpu import nvidia_smi, set_cuda
-from .utils.lib import dependencies
 from .utils.logging import getLogger, setLogger
 from .utils.notebook import (
     clear_output,
     cprint,
     create_button,
     create_dropdown,
     create_floatslider,
@@ -97,40 +96,69 @@
     @staticmethod
     def about() -> None:
         """Print the about information"""
         cfg = __global_config__
         _about(cfg)
 
     @staticmethod
-    def initialize(config: Union[DictConfig, Dict] = None):
+    def initialize(config: Union[DictConfig, Dict] = None):  # type: ignore
         """Initialize the global config"""
         __global_config__.initialize(config)
 
     @staticmethod
     def terminate():
         """Terminate the global config"""
         __global_config__.terminate()
 
     @staticmethod
     def envs() -> DotEnvConfig:
         """Return the current environments"""
-        return DotEnvConfig()
+        return DotEnvConfig()  # type: ignore
+
+    @staticmethod
+    def expand_posix_vars(posix_expr: str, context: dict = None) -> str:  # type: ignore
+        """
+        Expand POSIX variables in a string.
+
+        Args:
+            posix_expr (str): The string containing POSIX variables to be expanded.
+            context (dict, optional): A dictionary containing additional variables to be used in the expansion.
+                Defaults to None.
+
+        Returns:
+            str: The expanded string.
+
+        Examples:
+            >>> expand_posix_vars("$HOME")
+            '/home/user'
+            >>> expand_posix_vars("$HOME/$USER", {"USER": "testuser"})
+            '/home/user/testuser'
+
+        """
+        return expand_posix_vars(posix_expr, context=context)
+
+    @staticmethod
+    def environ(key: str = "", default: Union[str, None] = None) -> Any:
+        """Get the value of an environment variable or return the default value"""
+        return get_osenv(key, default=default)
 
     @staticmethod
     def compose(
-        config_group: str = None,
-        overrides: List[str] = [],
+        config_group: Union[str, None] = None,
+        overrides: Union[List[str], None] = None,
         *,
         return_as_dict: bool = False,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
-        config_name: str = None,
-        config_module: str = None,
+        config_name: Union[str, None] = None,
+        config_module: Union[str, None] = None,
         verbose: bool = False,
     ) -> Union[DictConfig, Dict]:
+        if overrides is None:
+            overrides = []
         return _compose(
             config_group=config_group,
             overrides=overrides,
             return_as_dict=return_as_dict,
             throw_on_resolution_failure=throw_on_resolution_failure,
             throw_on_missing=throw_on_missing,
             config_name=config_name,
@@ -188,15 +216,18 @@
             throw_on_missing=throw_on_missing,
             enum_to_str=enum_to_str,
             structured_config_mode=structured_config_mode,
         )
 
     @staticmethod
     def partial(
-        config: Any = None, config_group: str = None, *args: Any, **kwargs: Any
+        config: Any = None,
+        config_group: Union[str, None] = None,
+        *args: Any,
+        **kwargs: Any,
     ) -> Any:
         return _partial(config=config, config_group=config_group, *args, **kwargs)
 
     @staticmethod
     def instantiate(config: Any, *args: Any, **kwargs: Any) -> Any:
         return _instantiate(config, *args, **kwargs)
 
@@ -280,15 +311,15 @@
     @staticmethod
     def run(config: Any, **kwargs: Any) -> Any:
         _run(config, **kwargs)
 
     @staticmethod
     def load_dotenv(
         override: bool = False,
-        dotenv_dir: str = None,
+        dotenv_dir: str = "",
         dotenv_filename: str = ".env",
         verbose: bool = False,
     ) -> None:
         load_dotenv(
             override=override,
             dotenv_filename=dotenv_filename,
             dotenv_dir=dotenv_dir,
@@ -395,18 +426,14 @@
         )
 
     @staticmethod
     def pipe(data=None, cfg=None):
         return _pipe(data, cfg)
 
     @staticmethod
-    def dependencies(_key=None, path=None):
-        return dependencies(_key, path)
-
-    @staticmethod
     def ensure_list(value):
         return _ensure_list(value)
 
     @staticmethod
     def to_dateparm(_date, _format="%Y-%m-%d"):
         return to_dateparm(_date, _format)
 
@@ -494,24 +521,23 @@
             return _instantiate(
                 kwargs,
                 filename=filename,
                 base_dir=base_dir,
                 verbose=verbose,
                 filetype=filetype,
             )
-        else:
-            if filename is None:
-                raise ValueError("filename must be specified")
-            return load_data(
-                filename,
-                base_dir=base_dir,
-                verbose=verbose,
-                filetype=filetype,
-                **kwargs,
-            )
+        if filename is None:
+            raise ValueError("filename must be specified")
+        return load_data(
+            filename,
+            base_dir=base_dir,
+            verbose=verbose,
+            filetype=filetype,
+            **kwargs,
+        )
 
     @staticmethod
     def get_filepaths(
         filename_patterns=None, base_dir=None, recursive=True, verbose=True, **kwargs
     ):
         from .io.file import get_filepaths
 
@@ -669,22 +695,22 @@
 
     @staticmethod
     def set_cuda(device=0):
         return set_cuda(device)
 
     @staticmethod
     def mount_google_drive(
-        workspace=None,
-        project=None,
-        mountpoint="/content/drive",
-        force_remount=False,
-        timeout_ms=120000,
+        project_root: str = "",
+        project_name: str = "",
+        mountpoint: str = "/content/drive",
+        force_remount: bool = False,
+        timeout_ms: int = 120000,
     ):
         return mount_google_drive(
-            workspace, project, mountpoint, force_remount, timeout_ms
+            project_root, project_name, mountpoint, force_remount, timeout_ms
         )
 
     @staticmethod
     def getsource(obj):
         return _getsource(obj)
 
     @staticmethod
@@ -808,22 +834,18 @@
     def records_to_dataframe(
         data, index=None, exclude=None, columns=None, coerce_float=False, nrows=None
     ):
         return records_to_dataframe(data, index, exclude, columns, coerce_float, nrows)
 
     @staticmethod
     def create_dropdown(
-        options,
-        value,
-        description,
-        disabled=False,
-        style={"description_width": "initial"},
-        layout=None,
-        **kwargs,
+        options, value, description, disabled=False, style=None, layout=None, **kwargs
     ):
+        if style is None:
+            style = {"description_width": "initial"}
         return create_dropdown(
             options,
             value,
             description,
             disabled,
             style,
             layout,
@@ -832,18 +854,20 @@
 
     @staticmethod
     def create_textarea(
         value,
         description,
         placeholder="",
         disabled=False,
-        style={"description_width": "initial"},
+        style=None,
         layout=None,
         **kwargs,
     ):
+        if style is None:
+            style = {"description_width": "initial"}
         return create_textarea(
             value,
             description,
             placeholder,
             disabled,
             style,
             layout,
@@ -858,18 +882,20 @@
 
     @staticmethod
     def create_radiobutton(
         options,
         description,
         value=None,
         disabled=False,
-        style={"description_width": "initial"},
+        style=None,
         layout=None,
         **kwargs,
     ):
+        if style is None:
+            style = {"description_width": "initial"}
         return create_radiobutton(
             options,
             description,
             value,
             disabled,
             style,
             layout,
@@ -894,18 +920,20 @@
         value=None,
         description="",
         disabled=False,
         continuous_update=False,
         orientation="horizontal",
         readout=True,
         readout_format=".1f",
-        style={"description_width": "initial"},
+        style=None,
         layout=None,
         **kwargs,
     ):
+        if style is None:
+            style = {"description_width": "initial"}
         return create_floatslider(
             min,
             max,
             step,
             value,
             description,
             disabled,
@@ -954,34 +982,43 @@
             crop_box,
             mode,
             **kwargs,
         )
 
     @staticmethod
     def init_workspace(
-        workspace=None,
-        project=None,
-        task=None,
-        log_level=None,
-        autotime=True,
-        retina=True,
-        verbose=None,
+        project_name: str = "",
+        task_name: str = "",
+        project_root: str = "",
+        project_data_root: str = "",
+        global_workspace_root: str = "",
+        global_data_root: str = "",
+        log_level: str = "",
+        autotime: bool = True,
+        retina: bool = True,
+        verbose: Union[bool, int] = False,
         **kwargs,
     ) -> ProjectConfig:
         __global_config__.init_workspace(
-            workspace=workspace,
-            project=project,
-            task=task,
+            project_name=project_name,
+            task_name=task_name,
+            project_root=project_root,
+            project_data_root=project_data_root,
+            global_workspace_root=global_workspace_root,
+            global_data_root=global_data_root,
             log_level=log_level,
             autotime=autotime,
             retina=retina,
             verbose=verbose,
             **kwargs,
         )
-        return __global_config__.project
+        if __global_config__.project:
+            return __global_config__.project
+        else:
+            raise ValueError("Project not initialized.")
 
     @staticmethod
     def scale_image(
         image,
         max_width: int = None,
         max_height: int = None,
         max_pixels: int = None,
@@ -1025,13 +1062,13 @@
         dst = str(dst)
         shutil.copyfile(src, dst, follow_symlinks=follow_symlinks)
         logger.info(f"copied {src} to {dst}")
 
     @staticmethod
     def gpu_usage(all=False, attrList=None, useOldCode=False):
         try:
-            from GPUtil import showUtilization
+            from GPUtil import showUtilization  # type: ignore
         except ImportError:
             logger.error("GPUtil is not installed. To install, run: pip install GPUtil")
             return
 
         return showUtilization(all, attrList, useOldCode)
```

### Comparing `hyfi-0.4.0/src/hyfi/utils/batch/apply.py` & `hyfi-0.5.0/src/hyfi/utils/batch/apply.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,18 +53,15 @@
         batcher=None,
         args=[],
         kwargs={},
         cache=None,
         vectorize=None,
         description="batch_apply",
     ):
-        if batcher is None:
-            self.batcher = Batcher()
-        else:
-            self.batcher = batcher
+        self.batcher = Batcher() if batcher is None else batcher
         self.function = function
         self.args = [args]
         self.kwargs = [kwargs]
         self.cache = [cache]
         self.vectorize = [vectorize]
         self.description = description
```

### Comparing `hyfi-0.4.0/src/hyfi/utils/batch/apply_batch.py` & `hyfi-0.5.0/src/hyfi/utils/batch/apply_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,15 @@
 
 
 class ApplyBatch(object):
     # Applies a function to the entire minibatch. Use this for example on Pandas dataframes, to avoid per-row overhead.
     # Function needs to be applicable to the array/list of values!
     # If not, modify/wrap the function to process a list, or use Apply
     def __init__(self, function, batcher=None, args=[], kwargs={}):
-        if batcher is None:
-            self.batcher = Batcher()
-        else:
-            self.batcher = batcher
+        self.batcher = Batcher() if batcher is None else batcher
         self.function = function
         self.args = [args]
         self.kwargs = [kwargs]
 
     def fit(self, data, input_split=False):
         return self
```

### Comparing `hyfi-0.4.0/src/hyfi/utils/batch/batcher.py` & `hyfi-0.5.0/src/hyfi/utils/batch/batcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         data_split: list
                 List of minibatches, each entry is a list-like object representing the data subset in a batch.
         """
         if minibatch_size is None:
             minibatch_size = self.minibatch_size
         if backend is None:
             backend = self.backend
-        if isinstance(data, list) or isinstance(data, tuple) or isinstance(data, dict):
+        if isinstance(data, (list, tuple, dict)):
             len_data = len(data)
         else:
             len_data = data.shape[0]
         if backend == "spark":
             return self.list2indexedrdd(data, minibatch_size)
         if isinstance(data, pd.DataFrame):
             data = [
@@ -170,15 +170,15 @@
         Returns
         -------
         (anonymous): sparse matrix | pd.DataFrame | list
                 Single complete list-like data merged from given batches
         """
         if isinstance(data[0], ssp.csr_matrix):
             return ssp.vstack(data)
-        if isinstance(data[0], pd.DataFrame) or isinstance(data[0], pd.Series):
+        if isinstance(data[0], (pd.DataFrame, pd.Series)):
             return pd.concat(data)
         return [item for sublist in data for item in sublist]
 
     def process_batches(
         self,
         task,
         data,
@@ -269,46 +269,20 @@
             task_num_cpus = self.task_num_cpus
         if task_num_gpus is None:
             task_num_gpus = self.task_num_gpus
         if verbose is None:
             verbose = self.verbose
         if verbose > 1:
             logger.info(
-                "%s %s %s %s %s %s %s %s %s %s %s %s %s %s"
-                % (
-                    " backend:",
-                    backend,
-                    " minibatch_size:",
-                    self.minibatch_size,
-                    " procs:",
-                    procs,
-                    " input_split:",
-                    input_split,
-                    " merge_output:",
-                    merge_output,
-                    " len(data):",
-                    len(data),
-                    "len(args):",
-                    len(args),
-                )
+                f" backend: {backend}  minibatch_size: {self.minibatch_size}  procs: {procs}  input_split: {input_split}  merge_output: {merge_output}  len(data): {len(data)} len(args): {len(args)}"
             )
 
         if verbose > 10:
             logger.info(
-                "%s %s %s %s %s %s %s %s"
-                % (
-                    " len(data):",
-                    len(data),
-                    "len(args):",
-                    len(args),
-                    "[type(x) for x in data]:",
-                    [type(x) for x in data],
-                    "[type(x) for x in args]:",
-                    [type(x) for x in args],
-                )
+                f" len(data): {len(data)} len(args): {len(args)} [type(x) for x in data]: {[type(x) for x in data]} [type(x) for x in args]: {[type(x) for x in args]}"
             )
 
         if not (input_split):
             if backend == "spark":
                 paral_params = self.split_batches(data, minibatch_size, backend="spark")
             else:
                 paral_params = [
@@ -408,24 +382,15 @@
             #   jobs = [self.backend_handle.submit(task, (x,), (), ()) for x in paral_params]
             # 	results = [x() for x in jobs]
 
         if merge_output:
             return self.merge_batches(self.collect_batches(results, backend=backend))
         if verbose > 2:
             logger.info(
-                "%s %s %s %s %s %s %s"
-                % (
-                    " Task:",
-                    task,
-                    " backend:",
-                    backend,
-                    " backend_handle:",
-                    backend_handle,
-                    " completed",
-                )
+                f" Task: {task}  backend: {backend}  backend_handle: {backend_handle}  completed"
             )
         return results
 
     def shuffle_batch(self, texts, labels=None, seed=None):
         """Shuffle a list of samples, as well as the labels if specified
 
         Parameters
@@ -455,15 +420,15 @@
         texts = [texts[x] for x in index_shuf]
         if labels is None:
             return texts
         labels = [labels[x] for x in index_shuf]
         return texts, labels
 
     def __getstate__(self):
-        return dict((k, v) for (k, v) in self.__dict__.items())
+        return dict(self.__dict__.items())
 
     def __setstate__(self, params):
         for key in params:
             setattr(self, key, params[key])
 
 
 batcher_instance: Batcher
```

### Comparing `hyfi-0.4.0/src/hyfi/utils/cached_path/__init__.py` & `hyfi-0.5.0/src/hyfi/utils/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.4.0/src/hyfi/utils/cached_path/_cached_path.py` & `hyfi-0.5.0/src/hyfi/utils/cached_path/_cached_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         file_path, etag = get_from_cache(
             url_or_filename, cache_dir, quiet=quiet, progress=progress
         )
 
         if extract_archive and (is_zipfile(file_path) or tarfile.is_tarfile(file_path)):
             # This is the path the file should be extracted to.
             # For example ~/.cached_path/cache/234234.21341 -> ~/.cached_path/cache/234234.21341-extracted
-            extraction_path = file_path.parent / (file_path.name + "-extracted")
+            extraction_path = file_path.parent / f"{file_path.name}-extracted"
 
     else:
         orig_url_or_filename = url_or_filename
         url_or_filename = Path(url_or_filename).expanduser()
         cache_dir = Path(cache_dir if cache_dir else get_cache_dir()).expanduser()
         cache_dir.mkdir(parents=True, exist_ok=True)
 
@@ -303,16 +303,15 @@
         # target resource, if it exists. We'll only throw an exception if we
         # haven't cached the resource at all yet.
         logger.warning(
             "Connection error occurred while trying to fetch ETag for %s. "
             "Will attempt to use latest cached version of resource",
             url,
         )
-        latest_cached = find_latest_cached(url, cache_dir)
-        if latest_cached:
+        if latest_cached := find_latest_cached(url, cache_dir):
             logger.info(
                 "ETag request failed with recoverable error, using latest cached "
                 "version of %s: %s",
                 url,
                 latest_cached,
             )
             meta = Meta.from_path(_meta_file_path(latest_cached))
```

### Comparing `hyfi-0.4.0/src/hyfi/utils/cached_path/cache_file.py` & `hyfi-0.5.0/src/hyfi/utils/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.4.0/src/hyfi/utils/cached_path/common.py` & `hyfi-0.5.0/src/hyfi/utils/cached_path/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """
 
 
 def _split_cloud_path(url: str, provider: str) -> Tuple[str, str]:
     """Split a full s3 path into the bucket name and path."""
     parsed = urlparse(url)
     if not parsed.netloc or not parsed.path:
-        raise ValueError("bad {} path {}".format(provider, url))
+        raise ValueError(f"bad {provider} path {url}")
     bucket_name = parsed.netloc
     provider_path = parsed.path
     # Remove '/' at beginning of path.
     if provider_path.startswith("/"):
         provider_path = provider_path[1:]
     return bucket_name, provider_path
```

### Comparing `hyfi-0.4.0/src/hyfi/utils/cached_path/file_lock.py` & `hyfi-0.5.0/src/hyfi/utils/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.4.0/src/hyfi/utils/cached_path/meta.py` & `hyfi-0.5.0/src/hyfi/utils/cached_path/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             creation_time=time.time(),
             size=cls.get_resource_size(cached_path),
             etag=etag,
             extraction_dir=extraction_dir,
         )
 
     def to_file(self) -> None:
-        with open(self.cached_path + ".json", "w") as meta_file:
+        with open(f"{self.cached_path}.json", "w") as meta_file:
             json.dump(asdict(self), meta_file)
 
     @classmethod
     def from_path(cls, path: PathOrStr) -> "Meta":
         path = str(path)
         with open(path) as meta_file:
             data = json.load(meta_file)
```

### Comparing `hyfi-0.4.0/src/hyfi/utils/cached_path/progress.py` & `hyfi-0.5.0/src/hyfi/utils/cached_path/progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,17 +99,15 @@
         self.progress.advance(self.task_id, n)
         return n
 
     def writelines(self, lines):
         return self.handle.writelines(lines)
 
     def seek(self, offset: int, whence: int = 0) -> int:
-        pos = self.handle.seek(offset, whence)
-        #  self.progress.update(self.task_id, completed=pos)
-        return pos
+        return self.handle.seek(offset, whence)
 
     def tell(self) -> int:
         return self.handle.tell()
 
     @property
     def raw(self):
         return self.handle.raw
```

### Comparing `hyfi-0.4.0/src/hyfi/utils/cached_path/schemes/__init__.py` & `hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 __all__ = ["HttpClient", "SchemeClient", "hf_get_from_cache"]
 
 try:
     from .beaker import BeakerClient
 
     __all__.append("BeakerClient")
-except (ImportError, ModuleNotFoundError):
+except ImportError:
     BeakerClient = None
 
 
 _SCHEME_TO_CLIENT = {}
 
 
 def add_scheme_client(client: Type[SchemeClient]) -> None:
```

### Comparing `hyfi-0.4.0/src/hyfi/utils/cached_path/schemes/beaker.py` & `hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.4.0/src/hyfi/utils/cached_path/schemes/hf.py` & `hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.4.0/src/hyfi/utils/cached_path/schemes/http.py` & `hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,17 +48,15 @@
             try:
                 with session_with_backoff() as session:
                     response = session.head(self.resource, allow_redirects=True)
             except MaxRetryError as e:
                 raise RecoverableServerError(e.reason)
             self.validate_response(response)
             self._head_response = response
-            return self._head_response
-        else:
-            return self._head_response
+        return self._head_response
 
     def get_etag(self) -> Optional[str]:
         return self.head_response.headers.get("ETag")
 
     def get_size(self) -> Optional[int]:
         content_length = self.head_response.headers.get("Content-Length")
         return None if content_length is None else int(content_length)
```

### Comparing `hyfi-0.4.0/src/hyfi/utils/cached_path/schemes/scheme_client.py` & `hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.4.0/src/hyfi/utils/cached_path/testing.py` & `hyfi-0.5.0/src/hyfi/utils/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.4.0/src/hyfi/utils/cached_path/util.py` & `hyfi-0.5.0/src/hyfi/utils/cached_path/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     resource_bytes = str(resource).encode("utf-8")
     resource_hash = sha256(resource_bytes)
     filename = resource_hash.hexdigest()
 
     if etag:
         etag_bytes = etag.encode("utf-8")
         etag_hash = sha256(etag_bytes)
-        filename += "." + etag_hash.hexdigest()
+        filename += f".{etag_hash.hexdigest()}"
 
     return filename
 
 
 def filename_to_url(
     filename: str, cache_dir: Optional[PathOrStr] = None
 ) -> Tuple[str, Optional[str]]:
@@ -37,19 +37,19 @@
     Raises :exc:`FileNotFoundError` if ``filename`` or its stored metadata do not exist.
 
     This is essentially the inverse of :func:`resource_to_filename()`.
     """
     cache_dir = cache_dir if cache_dir else get_cache_dir()
     cache_path = os.path.join(cache_dir, filename)
     if not os.path.exists(cache_path):
-        raise FileNotFoundError("file {} not found".format(cache_path))
+        raise FileNotFoundError(f"file {cache_path} not found")
 
-    meta_path = cache_path + ".json"
+    meta_path = f"{cache_path}.json"
     if not os.path.exists(meta_path):
-        raise FileNotFoundError("file {} not found".format(meta_path))
+        raise FileNotFoundError(f"file {meta_path} not found")
 
     metadata = Meta.from_path(meta_path)
     return metadata.resource, metadata.etag
 
 
 def find_latest_cached(
     url: str, cache_dir: Optional[PathOrStr] = None
@@ -64,17 +64,15 @@
         print(path, path.suffix, path.name)
         if path.suffix in {".json", ".lock"} or path.name.endswith("-extracted"):
             continue
         mtime = path.stat().st_mtime
         candidates.append((path, mtime))
     # Sort candidates by modification time, newest first.
     candidates.sort(key=lambda x: x[1], reverse=True)
-    if candidates:
-        return candidates[0][0]
-    return None
+    return candidates[0][0] if candidates else None
 
 
 def check_tarfile(tar_file: tarfile.TarFile):
     """Tar files can contain files outside of the extraction directory, or symlinks that point
     outside the extraction directory. We also don't want any block devices fifos, or other
     weird file types extracted. This checks for those issues and throws an exception if there
     is a problem."""
@@ -127,12 +125,12 @@
 
     url_or_filename = os.path.expanduser(str(url_or_filename))
     parsed = urlparse(url_or_filename)
     return parsed.scheme in get_supported_schemes() or os.path.exists(url_or_filename)
 
 
 def _lock_file_path(cache_path: Path) -> Path:
-    return cache_path.parent / (cache_path.name + ".lock")
+    return cache_path.parent / f"{cache_path.name}.lock"
 
 
 def _meta_file_path(cache_path: Path) -> Path:
-    return cache_path.parent / (cache_path.name + ".json")
+    return cache_path.parent / f"{cache_path.name}.json"
```

### Comparing `hyfi-0.4.0/src/hyfi/utils/copier.py` & `hyfi-0.5.0/src/hyfi/utils/copier.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.4.0/src/hyfi/utils/func.py` & `hyfi-0.5.0/src/hyfi/utils/func.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,18 +58,15 @@
 def get_offset_ranges(count, num_workers):
     """Get offset ranges for parallel processing"""
     assert count > num_workers
     step_sz = int(count / num_workers)
     offset_ranges = [0]
     pv_cnt = 1
     for i in range(num_workers):
-        if i == num_workers - 1:
-            pv_cnt = count
-        else:
-            pv_cnt = pv_cnt + step_sz
+        pv_cnt = count if i == num_workers - 1 else pv_cnt + step_sz
         offset_ranges.append(pv_cnt)
     return offset_ranges
 
 
 @contextmanager
 def change_directory(directory):
     """Change directory and change back to original directory"""
@@ -77,19 +74,19 @@
 
     fancy_print(f" Change directory to {directory}")
     os.chdir(directory)
     try:
         yield
 
     except Exception as e:
-        fancy_print(" Exception: {}".format(e))
+        fancy_print(f" Exception: {e}")
         raise e
 
     finally:
-        fancy_print(" Change directory back to {}".format(original))
+        fancy_print(f" Change directory back to {original}")
         os.chdir(original)
 
 
 def fancy_print(*args, color=None, bold=False, **kwargs):
     """Print with color and bold"""
     if bold:
         print("\033[1m", end="")
@@ -170,17 +167,15 @@
 def len_bytes(x):
     """Return the length of a string in bytes"""
     return utf8len(x)
 
 
 def len_words(x):
     """Return the number of words in a string"""
-    if isinstance(x, str):
-        return len(x.split())
-    return 0
+    return len(x.split()) if isinstance(x, str) else 0
 
 
 def len_sents(x, sep):
     """Return the number of sentences in a string"""
     sep = str(sep).encode("utf-8").decode("unicode-escape")
     return len(re.sub(r"(\r?\n|\r){1,}", sep, x).split(sep))
 
@@ -211,19 +206,15 @@
 
 
 def get_modified_time(path):
     """Return the modification time of a file"""
     if not os.path.exists(path):
         return None
     modTimesinceEpoc = os.path.getmtime(path)
-    # Convert seconds since epoch to readable timestamp
-    modificationTime = time.strftime(
-        "%Y-%m-%d %H:%M:%S", time.localtime(modTimesinceEpoc)
-    )
-    return modificationTime
+    return time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(modTimesinceEpoc))
 
 
 def today(_format="%Y-%m-%d"):
     """Return today's date"""
     from datetime import datetime
 
     if _format is None:
@@ -232,18 +223,15 @@
         return datetime.today().strftime(_format)
 
 
 def now(_format="%Y-%m-%d %H:%M:%S"):
     """Return current date and time"""
     from datetime import datetime
 
-    if _format is None:
-        return datetime.now()
-    else:
-        return datetime.now().strftime(_format)
+    return datetime.now() if _format is None else datetime.now().strftime(_format)
 
 
 def strptime(
     _date_str: str,
     _format: str = "%Y-%m-%d",
 ):
     """Return a datetime object from a string"""
@@ -288,27 +276,23 @@
 
 def to_numeric(data, _columns=None, errors="coerce", downcast=None, **kwargs):
     """Convert a string, int, or float object to a float object"""
     import pandas as pd
 
     if isinstance(data, str):
         return float(data)
-    elif isinstance(data, int):
-        return data
-    elif isinstance(data, float):
+    elif isinstance(data, (int, float)) or not isinstance(data, pd.DataFrame):
         return data
-    elif isinstance(data, pd.DataFrame):
+    else:
         if _columns:
             if isinstance(_columns, str):
                 _columns = [_columns]
             for _col in _columns:
                 data[_col] = pd.to_numeric(data[_col], errors=errors, downcast=downcast)
         return data
-    else:
-        return data
 
 
 def human_readable_type_name(t: Type) -> str:
     """
     Generates a useful-for-humans label for a type.
     For builtin types, it's just the class name (eg "str" or "int").
     For other types, it includes the module (eg "pathlib.Path").
@@ -316,15 +300,15 @@
     module = t.__module__
     if module == "builtins":
         return t.__qualname__
     elif module.split(".")[0] == "hyfi":
         module = "hyfi"
 
     try:
-        return module + "." + t.__qualname__
+        return f"{module}.{t.__qualname__}"
     except AttributeError:
         return str(t)
 
 
 def readable_types_list(type_list: List[Type]) -> str:
     """Generates a useful-for-humans label for a list of types."""
     return ", ".join(human_readable_type_name(t) for t in type_list)
```

### Comparing `hyfi-0.4.0/src/hyfi/utils/gpu.py` & `hyfi-0.5.0/src/hyfi/utils/gpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,27 +45,25 @@
     @staticmethod
     def get_gpus():
         return GPUtil.getGPUs()
 
     @staticmethod
     def get_gpu_info():
         gpus = GPUtil.getGPUs()
-        gpu_info = []
-        for gpu in gpus:
-            gpu_info.append(
-                {
-                    "id": gpu.id,
-                    "name": gpu.name,
-                    "load": gpu.load,
-                    "memory_used": gpu.memoryUsed,
-                    "memory_total": gpu.memoryTotal,
-                    "temperature": gpu.temperature,
-                }
-            )
-        return gpu_info
+        return [
+            {
+                "id": gpu.id,
+                "name": gpu.name,
+                "load": gpu.load,
+                "memory_used": gpu.memoryUsed,
+                "memory_total": gpu.memoryTotal,
+                "temperature": gpu.temperature,
+            }
+            for gpu in gpus
+        ]
 
     @staticmethod
     def get_first_available(
         order="first",
         maxLoad=0.5,
         maxMemory=0.5,
         attempts=1,
@@ -98,18 +96,17 @@
             pass
 
 
 def nvidia_smi():
     """Run nvidia-smi and return the output as a string"""
     import subprocess
 
-    nvidiasmi_output = subprocess.run(
+    return subprocess.run(
         ["nvidia-smi", "-L"], stdout=subprocess.PIPE
     ).stdout.decode("utf-8")
-    return nvidiasmi_output
 
 
 def is_cuda_available():
     """Check if cuda is available"""
     try:
         import torch
```

### Comparing `hyfi-0.4.0/src/hyfi/utils/notebook.py` & `hyfi-0.5.0/src/hyfi/utils/notebook.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,18 @@
 
 def is_notebook():
     """Check if the code is running in a notebook."""
     try:
         get_ipython
     except NameError:
         return False
-    shell_type = get_ipython().__class__.__name__
+    # pylint: disable=undefined-variable
+    shell_type = get_ipython().__class__.__name__  # noqa
     # logger.info(f"shell type: {shell_type}")
-    if shell_type == "ZMQInteractiveShell":
-        return True  # Jupyter notebook or qtconsole
-    elif shell_type == "Shell":
-        return True  # Google colab
-    elif shell_type == "TerminalInteractiveShell":
-        return False  # Terminal running IPython
-    else:
-        return False  # Other type
+    return shell_type in ["ZMQInteractiveShell", "Shell"]
 
 
 def is_colab():
     """Check if the code is running in Google Colab."""
     is_colab = "google.colab" in sys.modules
     if is_colab:
         logger.info("Google Colab detected.")
@@ -40,18 +34,15 @@
     """Get the display object for the current environment."""
     try:
         from ipywidgets import Output
     except ImportError:
         logger.info("ipywidgets not installed.")
         return None
 
-    if is_notebook():
-        return Output()
-    else:
-        return None
+    return Output() if is_notebook() else None
 
 
 def clear_output(wait=False):
     """Clear the output of the current notebook."""
     from IPython import display
 
     if is_notebook():
@@ -193,109 +184,99 @@
     from IPython.display import HTML as html_print
     from IPython.display import display
 
     display(html_print(" ".join([colored_str(ti, color=ci) for ti, ci in str_tuples])))
 
 
 def create_dropdown(
-    options,
-    value,
-    description,
-    disabled=False,
-    style={"description_width": "initial"},
-    layout=None,
-    **kwargs,
+    options, value, description, disabled=False, style=None, layout=None, **kwargs
 ):
     """Create a dropdown widget."""
+    if style is None:
+        style = {"description_width": "initial"}
     import ipywidgets as widgets
 
     layout = (
         widgets.Layout(width="auto") if layout is None else widgets.Layout(**layout)
     )
-    dropdown = widgets.Dropdown(
+    return widgets.Dropdown(
         options=options,
         value=value,
         description=description,
         disabled=disabled,
         style=style,
         layout=layout,
         **kwargs,
     )
-    return dropdown
 
 
 def create_textarea(
     value,
     description,
     placeholder="",
     disabled=False,
-    style={"description_width": "initial"},
+    style=None,
     layout=None,
     **kwargs,
 ):
     """Create a textarea widget."""
+    if style is None:
+        style = {"description_width": "initial"}
     import ipywidgets as widgets
 
     layout = (
         widgets.Layout(width="auto") if layout is None else widgets.Layout(**layout)
     )
-    textarea = widgets.Textarea(
+    return widgets.Textarea(
         value=value,
         placeholder=placeholder,
         description=description,
         disabled=disabled,
         style=style,
         layout=layout,
         **kwargs,
     )
-    return textarea
 
 
 def create_button(description, button_style="", icon="check", layout=None, **kwargs):
     """Create a button widget."""
     import ipywidgets as widgets
 
     layout = (
         widgets.Layout(width="auto") if layout is None else widgets.Layout(**layout)
     )
-    button = widgets.Button(
+    return widgets.Button(
         description=description,
         button_style=button_style,
         icon=icon,
         layout=layout,
         **kwargs,
     )
-    return button
 
 
 def create_radiobutton(
-    options,
-    description,
-    value=None,
-    disabled=False,
-    style={"description_width": "initial"},
-    layout=None,
-    **kwargs,
+    options, description, value=None, disabled=False, style=None, layout=None, **kwargs
 ):
     """Create a radiobutton widget."""
+    if style is None:
+        style = {"description_width": "initial"}
     import ipywidgets as widgets
 
     layout = (
         widgets.Layout(width="auto") if layout is None else widgets.Layout(**layout)
     )
-    radiobutton = widgets.RadioButtons(
+    return widgets.RadioButtons(
         options=options,
         value=value,
         description=description,
         disabled=disabled,
         style=style,
         layout=layout,
         **kwargs,
     )
-    return radiobutton
 
 
 def create_image(
     filename=None,
     format=None,
     width=None,
     height=None,
@@ -306,84 +287,87 @@
 
     # from urllib.request import urlopen
 
     if filename is None:
         url = "https://assets.entelecheia.cc/img/placeholder.png"
         # img = urlopen(url).read()
         img = read(url)
-        format = "png"
+        _format = "png"
     else:
         img = read(filename)
-        format = format or filename.split(".")[-1]
-    image = widgets.Image(
+        _format = format or filename.split(".")[-1]
+    return widgets.Image(
         value=img,
-        format=format,
+        format=_format,
         width=width,
         height=height,
         **kwargs,
     )
-    return image
 
 
 def create_floatslider(
     min=0.0,
     max=1.0,
     step=0.1,
     value=None,
     description="",
     disabled=False,
     continuous_update=False,
     orientation="horizontal",
     readout=True,
     readout_format=".1f",
-    style={"description_width": "initial"},
+    style=None,
     layout=None,
     **kwargs,
 ):
     """Create a float slider widget."""
+    if style is None:
+        style = {"description_width": "initial"}
     import ipywidgets as widgets
 
     layout = (
         widgets.Layout(width="auto") if layout is None else widgets.Layout(**layout)
     )
-    slider = widgets.FloatSlider(
+    return widgets.FloatSlider(
         min=min,
         max=max,
         step=step,
         value=value,
         description=description,
         disabled=disabled,
         continuous_update=continuous_update,
         orientation=orientation,
         readout=readout,
         readout_format=readout_format,
         style=style,
         layout=layout,
         **kwargs,
     )
-    return slider
 
 
-def load_extentions(exts=["autotime"]):
+def load_extentions(exts=None):
     """Load extentions."""
-    if is_notebook():
-        from IPython import get_ipython
+    if exts is None:
+        exts = ["autotime"]
+    if not is_notebook():
+        return
+    from IPython import get_ipython
 
-        ip = get_ipython()
-        try:
-            loaded = ip.extension_manager.loaded
-            for ext in exts:
-                if ext not in loaded:
-                    ip.extentension_manager.load_extension(ext)
-        except AttributeError:
-            for ext in exts:
-                try:
-                    ip.magic("load_ext {}".format(ext))
-                except ModuleNotFoundError:
-                    logger.info("Extension %s not found. Install it first.", ext)
+    ip = get_ipython()
+    try:
+        loaded = ip.extension_manager.loaded
+        for ext in exts:
+            if ext not in loaded:
+                ip.extentension_manager.load_extension(ext)
+    except AttributeError:
+        for ext in exts:
+            try:
+                ip.magic(f"load_ext {ext}")
+            except ModuleNotFoundError:
+                logger.info("Extension %s not found. Install it first.", ext)
 
 
 def set_matplotlib_formats(*formats, **kwargs):
     """Set matplotlib formats."""
     if is_notebook():
         from IPython.display import set_matplotlib_formats
```

### Comparing `hyfi-0.4.0/src/hyfi/utils/pipe.py` & `hyfi-0.5.0/src/hyfi/utils/pipe.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,18 +35,15 @@
     use_batcher=True,
     minibatch_size=None,
     num_workers=None,
     **kwargs,
 ):
     batcher_instance = batcher.batcher_instance
     if use_batcher and batcher_instance is not None:
-        if batcher_instance is not None:
-            batcher_minibatch_size = batcher_instance.minibatch_size
-        else:
-            batcher_minibatch_size = 1000
+        batcher_minibatch_size = batcher_instance.minibatch_size
         if minibatch_size is None:
             minibatch_size = batcher_minibatch_size
         if num_workers is not None:
             batcher_instance.procs = int(num_workers)
         if batcher_instance.procs > 1:
             batcher_instance.minibatch_size = min(
                 int(len(series) / batcher_instance.procs) + 1, minibatch_size
```

### Comparing `hyfi-0.4.0/src/hyfi/utils/tools.py` & `hyfi-0.5.0/src/hyfi/utils/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,17 +104,15 @@
 def force_str_end(original_str: str, end: str = "\n") -> str:
     """Make sure a `original_str` ends with `end`.
 
     Params:
         original_str: String that you want to ensure ending.
         end: String that must exist at the end of `original_str`
     """
-    if not original_str.endswith(end):
-        return original_str + end
-    return original_str
+    return original_str + end if not original_str.endswith(end) else original_str
 
 
 def handle_remove_readonly(
     func: Callable, path: str, exc: Tuple[BaseException, OSError, TracebackType]
 ) -> None:
     """Handle errors when trying to remove read-only files through `shutil.rmtree`.
```

### Comparing `hyfi-0.4.0/PKG-INFO` & `hyfi-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.4.0
+Version: 0.5.0
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

