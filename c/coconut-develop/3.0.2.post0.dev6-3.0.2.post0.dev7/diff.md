# Comparing `tmp/coconut-develop-3.0.2.post0.dev6.tar.gz` & `tmp/coconut-develop-3.0.2.post0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coconut-develop-3.0.2.post0.dev6.tar", last modified: Sat Jun 10 04:37:22 2023, max compression
+gzip compressed data, was "dist/coconut-develop-3.0.2.post0.dev7.tar", last modified: Sun Jun 11 23:51:34 2023, max compression
```

## Comparing `coconut-develop-3.0.2.post0.dev6.tar` & `coconut-develop-3.0.2.post0.dev7.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/
--rw-r--r--   0 runner    (1001) docker     (122)    13803 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)   199678 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/DOCS.md
--rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/FAQ.md
--rw-r--r--   0 runner    (1001) docker     (122)    65131 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/HELP.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6940 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/__coconut__/
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/__coconut__/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    42392 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/__coconut__/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/__coconut__/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/_coconut/
--rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/_coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4759 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/_coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/_coconut/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/
--rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/__coconut__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/__coconut__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13505 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/_pyparsing.py
--rw-r--r--   0 runner    (1001) docker     (122)     9278 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/api.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/command/
--rw-r--r--   0 runner    (1001) docker     (122)      778 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     8489 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/command/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    44611 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/command/command.py
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/command/command.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/command/mypy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/command/resources/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/command/resources/zcoconut.pth
--rw-r--r--   0 runner    (1001) docker     (122)    23531 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/command/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/command/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   196410 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    93111 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/compiler/grammar.py
--rw-r--r--   0 runner    (1001) docker     (122)    34976 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/compiler/header.py
--rw-r--r--   0 runner    (1001) docker     (122)    58872 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/compiler/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/compiler/templates/
--rw-r--r--   0 runner    (1001) docker     (122)   102260 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/compiler/templates/header.py_template
--rw-r--r--   0 runner    (1001) docker     (122)    48882 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/compiler/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    36611 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/convenience.py
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/convenience.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/highlighter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/icoconut/
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/icoconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/icoconut/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/icoconut/coconut/
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/icoconut/coconut/kernel.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/icoconut/coconut_py/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/icoconut/coconut_py/kernel.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/icoconut/coconut_py2/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/icoconut/coconut_py2/kernel.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/icoconut/coconut_py3/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/icoconut/coconut_py3/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/icoconut/embed.py
--rw-r--r--   0 runner    (1001) docker     (122)    10729 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/icoconut/root.py
--rw-r--r--   0 runner    (1001) docker     (122)     8406 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/integrations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/main.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    11623 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/requirements.py
--rw-r--r--   0 runner    (1001) docker     (122)    15522 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/root.py
--rw-r--r--   0 runner    (1001) docker     (122)    19564 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4577 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/constants_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    30399 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/agnostic/
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/agnostic/__init__.coco
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/agnostic/main.coco
--rw-r--r--   0 runner    (1001) docker     (122)    63255 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/agnostic/primary.coco
--rw-r--r--   0 runner    (1001) docker     (122)     5219 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/agnostic/specific.coco
--rw-r--r--   0 runner    (1001) docker     (122)    42163 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/agnostic/suite.coco
--rw-r--r--   0 runner    (1001) docker     (122)    15411 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/agnostic/tutorial.coco
--rw-r--r--   0 runner    (1001) docker     (122)    46282 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/agnostic/util.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/non_strict/
--rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/target_2/
--rw-r--r--   0 runner    (1001) docker     (122)      356 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/target_2/py2_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/target_3/
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/target_3/py3_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/target_35/
--rw-r--r--   0 runner    (1001) docker     (122)     2751 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/target_35/py35_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/target_36/
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/target_36/py36_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/target_38/
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/target_38/py38_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/target_sys/
--rw-r--r--   0 runner    (1001) docker     (122)     5206 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
--rw-r--r--   0 runner    (1001) docker     (122)    22378 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/extras.coco
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/runnable.coco
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/tests/src/runner.coco
--rw-r--r--   0 runner    (1001) docker     (122)    11530 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/coconut/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut_develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/coconut_develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-10 04:37:22.000000 coconut-develop-3.0.2.post0.dev6/xontrib/
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-06-10 03:36:25.000000 coconut-develop-3.0.2.post0.dev6/xontrib/coconut.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)    13803 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/xontrib/coconut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/_coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)     4759 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/_coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/_coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/_coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7601 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut_develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut_develop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    65131 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/HELP.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/FAQ.md
+-rw-r--r--   0 runner    (1001) docker     (122)   199842 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/DOCS.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13505 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/_pyparsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/convenience.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/__coconut__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15522 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/root.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/api.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/coconut_py3/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/coconut_py3/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10742 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/root.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/coconut_py/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/coconut_py/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/embed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/coconut_py2/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/coconut_py2/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-06-11 23:51:33.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/coconut/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/__coconut__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/
+-rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/mypy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44611 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8489 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/command.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/watch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/resources/zcoconut.pth
+-rw-r--r--   0 runner    (1001) docker     (122)    23531 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11623 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9278 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     8406 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19564 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)    35187 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/header.py
+-rw-r--r--   0 runner    (1001) docker     (122)    93362 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58872 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)   196410 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)   102260 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/templates/header.py_template
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48882 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36611 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11530 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4577 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/constants_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/runner.coco
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/runnable.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_35/
+-rw-r--r--   0 runner    (1001) docker     (122)     2751 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_35/py35_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_38/
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_38/py38_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_2/
+-rw-r--r--   0 runner    (1001) docker     (122)      356 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_2/py2_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_36/
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_36/py36_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_sys/
+-rw-r--r--   0 runner    (1001) docker     (122)     5206 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/non_strict/
+-rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_3/py3_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (122)    42163 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/suite.coco
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/__init__.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    46282 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/util.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    63255 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/primary.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    15411 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/tutorial.coco
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/main.coco
+-rw-r--r--   0 runner    (1001) docker     (122)     5219 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/specific.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    22378 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/extras.coco
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30524 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/__coconut__/
+-rw-r--r--   0 runner    (1001) docker     (122)    42392 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/__coconut__/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/__coconut__/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/__coconut__/__init__.py
```

### Comparing `coconut-develop-3.0.2.post0.dev6/CONTRIBUTING.md` & `coconut-develop-3.0.2.post0.dev7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/DOCS.md` & `coconut-develop-3.0.2.post0.dev7/DOCS.md`

 * *Files 0% similar despite different names*

```diff
@@ -6572,5909 +6572,5920 @@
 00019ab0: 6963 6974 2066 756e 6374 696f 6e20 6170  icit function ap
 00019ac0: 706c 6963 6174 696f 6e20 616e 6420 636f  plication and co
 00019ad0: 6566 6669 6369 656e 7420 7379 6e74 6178  efficient syntax
 00019ae0: 2e20 546f 2075 7365 2060 6177 6169 7460  . To use `await`
 00019af0: 2c20 7369 6d70 6c79 2070 6172 656e 7468  , simply parenth
 00019b00: 6573 697a 6520 7468 6520 6578 7072 6573  esize the expres
 00019b10: 7369 6f6e 2c20 6173 2069 6e20 6061 7761  sion, as in `awa
-00019b20: 6974 2028 6620 7829 602e 0a0a 2323 2323  it (f x)`...####
-00019b30: 2320 4578 616d 706c 6573 0a0a 2a2a 436f  # Examples..**Co
-00019b40: 636f 6e75 743a 2a2a 0a60 6060 636f 636f  conut:**.```coco
-00019b50: 6e75 740a 6465 6620 6628 782c 2079 2920  nut.def f(x, y) 
-00019b60: 3d20 2878 2c20 7929 0a70 7269 6e74 2866  = (x, y).print(f
-00019b70: 2035 2031 3029 0a60 6060 0a0a 6060 6063   5 10).```..```c
-00019b80: 6f63 6f6e 7574 0a64 6566 2070 3128 7829  oconut.def p1(x)
-00019b90: 203d 2078 202b 2031 0a70 7269 6e74 203c   = x + 1.print <
-00019ba0: 7c20 7031 2035 0a60 6060 0a0a 6060 6063  | p1 5.```..```c
-00019bb0: 6f63 6f6e 7574 0a71 7561 6420 3d20 3520  oconut.quad = 5 
-00019bc0: 782a 2a32 202b 2033 2078 202b 2031 0a60  x**2 + 3 x + 1.`
-00019bd0: 6060 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a  ``..**Python:**.
-00019be0: 6060 6063 6f63 6f6e 7574 5f70 7974 686f  ```coconut_pytho
-00019bf0: 6e0a 6465 6620 6628 782c 2079 293a 2072  n.def f(x, y): r
-00019c00: 6574 7572 6e20 2878 2c20 7929 0a70 7269  eturn (x, y).pri
-00019c10: 6e74 2866 2831 3030 2c20 352b 3629 290a  nt(f(100, 5+6)).
-00019c20: 6060 600a 0a60 6060 636f 636f 6e75 745f  ```..```coconut_
-00019c30: 7079 7468 6f6e 0a64 6566 2070 3128 7829  python.def p1(x)
-00019c40: 3a20 7265 7475 726e 2078 202b 2031 0a70  : return x + 1.p
-00019c50: 7269 6e74 2870 3128 3529 290a 6060 600a  rint(p1(5)).```.
-00019c60: 0a60 6060 636f 636f 6e75 745f 7079 7468  .```coconut_pyth
-00019c70: 6f6e 0a71 7561 6420 3d20 3520 2a20 782a  on.quad = 5 * x*
-00019c80: 2a32 202b 2033 202a 2078 202b 2031 0a60  *2 + 3 * x + 1.`
-00019c90: 6060 0a0a 2323 2320 4b65 7977 6f72 6420  ``..### Keyword 
-00019ca0: 4172 6775 6d65 6e74 204e 616d 6520 456c  Argument Name El
-00019cb0: 6973 696f 6e0a 0a57 6865 6e20 7061 7373  ision..When pass
-00019cc0: 696e 6720 696e 206c 6f6e 6720 7661 7269  ing in long vari
-00019cd0: 6162 6c65 206e 616d 6573 2061 7320 6b65  able names as ke
-00019ce0: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
-00019cf0: 6f66 2074 6865 2073 616d 6520 6e61 6d65  of the same name
-00019d00: 2c20 436f 636f 6e75 7420 7375 7070 6f72  , Coconut suppor
-00019d10: 7473 2074 6865 2073 796e 7461 780a 6060  ts the syntax.``
-00019d20: 600a 6628 2e2e 2e3d 6c6f 6e67 5f76 6172  `.f(...=long_var
-00019d30: 6961 626c 655f 6e61 6d65 290a 6060 600a  iable_name).```.
-00019d40: 6173 2061 2073 686f 7274 6861 6e64 2066  as a shorthand f
-00019d50: 6f72 0a60 6060 0a66 286c 6f6e 675f 7661  or.```.f(long_va
-00019d60: 7269 6162 6c65 5f6e 616d 653d 6c6f 6e67  riable_name=long
-00019d70: 5f76 6172 6961 626c 655f 6e61 6d65 290a  _variable_name).
-00019d80: 6060 600a 0a53 7563 6820 7379 6e74 6178  ```..Such syntax
-00019d90: 2069 7320 616c 736f 2073 7570 706f 7274   is also support
-00019da0: 6564 2069 6e20 5b70 6172 7469 616c 2061  ed in [partial a
-00019db0: 7070 6c69 6361 7469 6f6e 5d28 2370 6172  pplication](#par
-00019dc0: 7469 616c 2d61 7070 6c69 6361 7469 6f6e  tial-application
-00019dd0: 2920 616e 6420 5b61 6e6f 6e79 6d6f 7573  ) and [anonymous
-00019de0: 2060 6e61 6d65 6474 7570 6c65 6073 5d28   `namedtuple`s](
-00019df0: 2361 6e6f 6e79 6d6f 7573 2d6e 616d 6564  #anonymous-named
-00019e00: 7475 706c 6573 292e 0a0a 2323 2323 2320  tuples)...##### 
-00019e10: 4578 616d 706c 650a 0a2a 2a43 6f63 6f6e  Example..**Cocon
-00019e20: 7574 3a2a 2a0a 6060 6063 6f63 6f6e 7574  ut:**.```coconut
-00019e30: 0a72 6561 6c6c 795f 6c6f 6e67 5f76 6172  .really_long_var
-00019e40: 6961 626c 655f 6e61 6d65 5f31 203d 2067  iable_name_1 = g
-00019e50: 6574 5f31 2829 0a72 6561 6c6c 795f 6c6f  et_1().really_lo
-00019e60: 6e67 5f76 6172 6961 626c 655f 6e61 6d65  ng_variable_name
-00019e70: 5f32 203d 2067 6574 5f32 2829 0a6d 6169  _2 = get_2().mai
-00019e80: 6e5f 6675 6e63 280a 2020 2020 2e2e 2e3d  n_func(.    ...=
-00019e90: 7265 616c 6c79 5f6c 6f6e 675f 7661 7269  really_long_vari
-00019ea0: 6162 6c65 5f6e 616d 655f 312c 0a20 2020  able_name_1,.   
-00019eb0: 202e 2e2e 3d72 6561 6c6c 795f 6c6f 6e67   ...=really_long
-00019ec0: 5f76 6172 6961 626c 655f 6e61 6d65 5f32  _variable_name_2
-00019ed0: 2c0a 290a 6060 600a 0a2a 2a50 7974 686f  ,.).```..**Pytho
-00019ee0: 6e3a 2a2a 0a60 6060 636f 636f 6e75 745f  n:**.```coconut_
-00019ef0: 7079 7468 6f6e 0a72 6561 6c6c 795f 6c6f  python.really_lo
-00019f00: 6e67 5f76 6172 6961 626c 655f 6e61 6d65  ng_variable_name
-00019f10: 5f31 203d 2067 6574 5f31 2829 0a72 6561  _1 = get_1().rea
-00019f20: 6c6c 795f 6c6f 6e67 5f76 6172 6961 626c  lly_long_variabl
-00019f30: 655f 6e61 6d65 5f32 203d 2067 6574 5f32  e_name_2 = get_2
-00019f40: 2829 0a6d 6169 6e5f 6675 6e63 280a 2020  ().main_func(.  
-00019f50: 2020 7265 616c 6c79 5f6c 6f6e 675f 7661    really_long_va
-00019f60: 7269 6162 6c65 5f6e 616d 655f 313d 7265  riable_name_1=re
-00019f70: 616c 6c79 5f6c 6f6e 675f 7661 7269 6162  ally_long_variab
-00019f80: 6c65 5f6e 616d 655f 312c 0a20 2020 2072  le_name_1,.    r
-00019f90: 6561 6c6c 795f 6c6f 6e67 5f76 6172 6961  eally_long_varia
-00019fa0: 626c 655f 6e61 6d65 5f32 3d72 6561 6c6c  ble_name_2=reall
-00019fb0: 795f 6c6f 6e67 5f76 6172 6961 626c 655f  y_long_variable_
-00019fc0: 6e61 6d65 5f32 2c0a 290a 6060 600a 0a23  name_2,.).```..#
-00019fd0: 2323 2041 6e6f 6e79 6d6f 7573 204e 616d  ## Anonymous Nam
-00019fe0: 6564 7475 706c 6573 0a0a 436f 636f 6e75  edtuples..Coconu
-00019ff0: 7420 7375 7070 6f72 7473 2061 6e6f 6e79  t supports anony
-0001a000: 6d6f 7573 205b 606e 616d 6564 7475 706c  mous [`namedtupl
-0001a010: 6560 5d28 6874 7470 733a 2f2f 646f 6373  e`](https://docs
-0001a020: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
-0001a030: 6272 6172 792f 636f 6c6c 6563 7469 6f6e  brary/collection
-0001a040: 732e 6874 6d6c 2363 6f6c 6c65 6374 696f  s.html#collectio
-0001a050: 6e73 2e6e 616d 6564 7475 706c 6529 206c  ns.namedtuple) l
-0001a060: 6974 6572 616c 732c 2073 7563 6820 7468  iterals, such th
-0001a070: 6174 2060 2861 3d31 2c20 623d 3229 6020  at `(a=1, b=2)` 
-0001a080: 6361 6e20 6265 2075 7365 6420 6a75 7374  can be used just
-0001a090: 2061 7320 6028 312c 2032 2960 2c20 6275   as `(1, 2)`, bu
-0001a0a0: 7420 7769 7468 2061 6464 6564 206e 616d  t with added nam
-0001a0b0: 6573 2e20 416e 6f6e 796d 6f75 7320 606e  es. Anonymous `n
-0001a0c0: 616d 6564 7475 706c 6560 7320 6172 6520  amedtuple`s are 
-0001a0d0: 616c 7761 7973 2070 6963 6b6c 6561 626c  always pickleabl
-0001a0e0: 652e 0a0a 5468 6520 7379 6e74 6178 2066  e...The syntax f
-0001a0f0: 6f72 2061 6e6f 6e79 6d6f 7573 206e 616d  or anonymous nam
-0001a100: 6564 7475 706c 6520 6c69 7465 7261 6c73  edtuple literals
-0001a110: 2069 733a 0a60 6060 636f 636f 6e75 740a   is:.```coconut.
-0001a120: 283c 6e61 6d65 3e20 5b3a 203c 7479 7065  (<name> [: <type
-0001a130: 3e5d 203d 203c 7661 6c75 653e 2c20 2e2e  >] = <value>, ..
-0001a140: 2e29 0a60 6060 0a77 6865 7265 2c20 6966  .).```.where, if
-0001a150: 2060 3c74 7970 653e 6020 6973 2067 6976   `<type>` is giv
-0001a160: 656e 2066 6f72 2061 6e79 2066 6965 6c64  en for any field
-0001a170: 2c20 5b60 7479 7069 6e67 2e4e 616d 6564  , [`typing.Named
-0001a180: 5475 706c 6560 5d28 6874 7470 733a 2f2f  Tuple`](https://
-0001a190: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
-0001a1a0: 332f 6c69 6272 6172 792f 7479 7069 6e67  3/library/typing
-0001a1b0: 2e68 746d 6c23 7479 7069 6e67 2e4e 616d  .html#typing.Nam
-0001a1c0: 6564 5475 706c 6529 2069 7320 7573 6564  edTuple) is used
-0001a1d0: 2069 6e73 7465 6164 206f 6620 6063 6f6c   instead of `col
-0001a1e0: 6c65 6374 696f 6e73 2e6e 616d 6564 7475  lections.namedtu
-0001a1f0: 706c 6560 2e0a 0a41 6e6f 6e79 6d6f 7573  ple`...Anonymous
-0001a200: 2060 6e61 6d65 6474 7570 6c65 6073 2061   `namedtuple`s a
-0001a210: 6c73 6f20 7375 7070 6f72 7420 5b6b 6579  lso support [key
-0001a220: 776f 7264 2061 7267 756d 656e 7420 6e61  word argument na
-0001a230: 6d65 2065 6c69 7369 6f6e 5d28 236b 6579  me elision](#key
-0001a240: 776f 7264 2d61 7267 756d 656e 742d 6e61  word-argument-na
-0001a250: 6d65 2d65 6c69 7369 6f6e 292e 0a0a 2323  me-elision)...##
-0001a260: 2323 2320 605f 6e61 6d65 6474 7570 6c65  ### `_namedtuple
-0001a270: 5f6f 6660 0a0a 4f6e 2050 7974 686f 6e20  _of`..On Python 
-0001a280: 7665 7273 696f 6e73 2060 3e3d 332e 3660  versions `>=3.6`
-0001a290: 2c20 605f 6e61 6d65 6474 7570 6c65 5f6f  , `_namedtuple_o
-0001a2a0: 6660 2069 7320 7072 6f76 6964 6564 2061  f` is provided a
-0001a2b0: 7320 6120 6275 696c 742d 696e 2074 6861  s a built-in tha
-0001a2c0: 7420 6361 6e20 6d69 6d69 6320 7468 6520  t can mimic the 
-0001a2d0: 6265 6861 7669 6f72 206f 6620 616e 6f6e  behavior of anon
-0001a2e0: 796d 6f75 7320 6e61 6d65 6474 7570 6c65  ymous namedtuple
-0001a2f0: 206c 6974 6572 616c 7320 7375 6368 2074   literals such t
-0001a300: 6861 7420 605f 6e61 6d65 6474 7570 6c65  hat `_namedtuple
-0001a310: 5f6f 6628 613d 312c 2062 3d32 2960 2069  _of(a=1, b=2)` i
-0001a320: 7320 6571 7569 7661 6c65 6e74 2074 6f20  s equivalent to 
-0001a330: 6028 613d 312c 2062 3d32 2960 2e20 5369  `(a=1, b=2)`. Si
-0001a340: 6e63 6520 605f 6e61 6d65 6474 7570 6c65  nce `_namedtuple
-0001a350: 5f6f 6660 2069 7320 6f6e 6c79 2061 7661  _of` is only ava
-0001a360: 696c 6162 6c65 206f 6e20 5079 7468 6f6e  ilable on Python
-0001a370: 2033 2e36 2061 6e64 2061 626f 7665 2c20   3.6 and above, 
-0001a380: 686f 7765 7665 722c 2069 7420 6973 2067  however, it is g
-0001a390: 656e 6572 616c 6c79 2072 6563 6f6d 6d65  enerally recomme
-0001a3a0: 6e64 6564 2074 6f20 7573 6520 616e 6f6e  nded to use anon
-0001a3b0: 796d 6f75 7320 6e61 6d65 6474 7570 6c65  ymous namedtuple
-0001a3c0: 206c 6974 6572 616c 7320 696e 7374 6561   literals instea
-0001a3d0: 642c 2061 7320 7468 6579 2077 6f72 6b20  d, as they work 
-0001a3e0: 6f6e 2061 6e79 2050 7974 686f 6e20 7665  on any Python ve
-0001a3f0: 7273 696f 6e2e 0a0a 5f60 5f6e 616d 6564  rsion..._`_named
-0001a400: 7475 706c 655f 6f66 6020 6973 206a 7573  tuple_of` is jus
-0001a410: 7420 7072 6f76 6964 6564 2074 6f20 6769  t provided to gi
-0001a420: 7665 206e 616d 6564 7475 706c 6520 6c69  ve namedtuple li
-0001a430: 7465 7261 6c73 2061 2072 6570 7265 7365  terals a represe
-0001a440: 6e74 6174 696f 6e20 7468 6174 2063 6f72  ntation that cor
-0001a450: 7265 7370 6f6e 6473 2074 6f20 616e 2065  responds to an e
-0001a460: 7870 7265 7373 696f 6e20 7468 6174 2063  xpression that c
-0001a470: 616e 2062 6520 7573 6564 2074 6f20 7265  an be used to re
-0001a480: 6372 6561 7465 2074 6865 6d2e 5f0a 0a23  create them._..#
-0001a490: 2323 2323 2045 7861 6d70 6c65 0a0a 2a2a  #### Example..**
-0001a4a0: 436f 636f 6e75 743a 2a2a 0a60 6060 636f  Coconut:**.```co
-0001a4b0: 636f 6e75 740a 7573 6572 7320 3d20 5b0a  conut.users = [.
-0001a4c0: 2020 2020 2869 643d 312c 206e 616d 653d      (id=1, name=
-0001a4d0: 2241 6c69 6365 2229 2c0a 2020 2020 2869  "Alice"),.    (i
-0001a4e0: 643d 322c 206e 616d 653d 2242 6f62 2229  d=2, name="Bob")
-0001a4f0: 2c0a 5d0a 6060 600a 0a2a 2a50 7974 686f  ,.].```..**Pytho
-0001a500: 6e3a 2a2a 0a60 6060 636f 636f 6e75 745f  n:**.```coconut_
-0001a510: 7079 7468 6f6e 0a66 726f 6d20 636f 6c6c  python.from coll
-0001a520: 6563 7469 6f6e 7320 696d 706f 7274 206e  ections import n
-0001a530: 616d 6564 7475 706c 650a 0a75 7365 7273  amedtuple..users
-0001a540: 203d 205b 0a20 2020 206e 616d 6564 7475   = [.    namedtu
-0001a550: 706c 6528 225f 222c 2022 6964 2c20 6e61  ple("_", "id, na
-0001a560: 6d65 2229 2831 2c20 2241 6c69 6365 2229  me")(1, "Alice")
-0001a570: 2c0a 2020 2020 6e61 6d65 6474 7570 6c65  ,.    namedtuple
-0001a580: 2822 5f22 2c20 2269 642c 206e 616d 6522  ("_", "id, name"
-0001a590: 2928 322c 2022 426f 6222 292c 0a5d 0a60  )(2, "Bob"),.].`
-0001a5a0: 6060 0a0a 2323 2320 5365 7420 4c69 7465  ``..### Set Lite
-0001a5b0: 7261 6c73 0a0a 436f 636f 6e75 7420 616c  rals..Coconut al
-0001a5c0: 6c6f 7773 2061 6e20 6f70 7469 6f6e 616c  lows an optional
-0001a5d0: 2060 7360 2074 6f20 6265 2070 7265 7065   `s` to be prepe
-0001a5e0: 6e64 6564 2069 6e20 6672 6f6e 7420 6f66  nded in front of
-0001a5f0: 2050 7974 686f 6e20 7365 7420 6c69 7465   Python set lite
-0001a600: 7261 6c73 2e20 5768 696c 6520 696e 206d  rals. While in m
-0001a610: 6f73 7420 6361 7365 7320 7468 6973 2064  ost cases this d
-0001a620: 6f65 7320 6e6f 7468 696e 672c 2069 6e20  oes nothing, in 
-0001a630: 7468 6520 6361 7365 206f 6620 7468 6520  the case of the 
-0001a640: 656d 7074 7920 7365 7420 6974 206c 6574  empty set it let
-0001a650: 7320 436f 636f 6e75 7420 6b6e 6f77 2074  s Coconut know t
-0001a660: 6861 7420 6974 2069 7320 616e 2065 6d70  hat it is an emp
-0001a670: 7479 2073 6574 2061 6e64 206e 6f74 2061  ty set and not a
-0001a680: 6e20 656d 7074 7920 6469 6374 696f 6e61  n empty dictiona
-0001a690: 7279 2e20 5365 7420 6c69 7465 7261 6c73  ry. Set literals
-0001a6a0: 2061 6c73 6f20 7375 7070 6f72 7420 756e   also support un
-0001a6b0: 7061 636b 696e 6720 7379 6e74 6178 2028  packing syntax (
-0001a6c0: 652e 672e 2060 737b 2a78 737d 6029 2e0a  e.g. `s{*xs}`)..
-0001a6d0: 0a41 6464 6974 696f 6e61 6c6c 792c 2043  .Additionally, C
-0001a6e0: 6f63 6f6e 7574 2061 6c73 6f20 7375 7070  oconut also supp
-0001a6f0: 6f72 7473 2072 6570 6c61 6369 6e67 2074  orts replacing t
-0001a700: 6865 2060 7360 2077 6974 6820 616e 2060  he `s` with an `
-0001a710: 6660 2074 6f20 6765 6e65 7261 7465 2061  f` to generate a
-0001a720: 2060 6672 6f7a 656e 7365 7460 206f 7220   `frozenset` or 
-0001a730: 616e 2060 6d60 2074 6f20 6765 6e65 7261  an `m` to genera
-0001a740: 7465 2061 2043 6f63 6f6e 7574 205b 606d  te a Coconut [`m
-0001a750: 756c 7469 7365 7460 5d28 236d 756c 7469  ultiset`](#multi
-0001a760: 7365 7429 2e0a 0a23 2323 2323 2045 7861  set)...##### Exa
-0001a770: 6d70 6c65 0a0a 2a2a 436f 636f 6e75 743a  mple..**Coconut:
-0001a780: 2a2a 0a60 6060 636f 636f 6e75 740a 656d  **.```coconut.em
-0001a790: 7074 795f 6672 6f7a 656e 5f73 6574 203d  pty_frozen_set =
-0001a7a0: 2066 7b7d 0a60 6060 0a0a 2a2a 5079 7468   f{}.```..**Pyth
-0001a7b0: 6f6e 3a2a 2a0a 6060 6063 6f63 6f6e 7574  on:**.```coconut
-0001a7c0: 5f70 7974 686f 6e0a 656d 7074 795f 6672  _python.empty_fr
-0001a7d0: 6f7a 656e 5f73 6574 203d 2066 726f 7a65  ozen_set = froze
-0001a7e0: 6e73 6574 2829 0a60 6060 0a0a 2323 2320  nset().```..### 
-0001a7f0: 496d 6167 696e 6172 7920 4c69 7465 7261  Imaginary Litera
-0001a800: 6c73 0a0a 496e 2061 6464 6974 696f 6e20  ls..In addition 
-0001a810: 746f 2050 7974 686f 6e27 7320 603c 6e75  to Python's `<nu
-0001a820: 6d3e 6a60 206f 7220 603c 6e75 6d3e 4a60  m>j` or `<num>J`
-0001a830: 206e 6f74 6174 696f 6e20 666f 7220 696d   notation for im
-0001a840: 6167 696e 6172 7920 6c69 7465 7261 6c73  aginary literals
-0001a850: 2c20 436f 636f 6e75 7420 616c 736f 2073  , Coconut also s
-0001a860: 7570 706f 7274 7320 603c 6e75 6d3e 6960  upports `<num>i`
-0001a870: 206f 7220 603c 6e75 6d3e 4960 2c20 746f   or `<num>I`, to
-0001a880: 206d 616b 6520 696d 6167 696e 6172 7920   make imaginary 
-0001a890: 6c69 7465 7261 6c73 206d 6f72 6520 7265  literals more re
-0001a8a0: 6164 6162 6c65 2069 6620 7573 6564 2069  adable if used i
-0001a8b0: 6e20 6120 6d61 7468 656d 6174 6963 616c  n a mathematical
-0001a8c0: 2063 6f6e 7465 7874 2e0a 0a23 2323 2323   context...#####
-0001a8d0: 2050 7974 686f 6e20 446f 6373 0a0a 496d   Python Docs..Im
-0001a8e0: 6167 696e 6172 7920 6c69 7465 7261 6c73  aginary literals
-0001a8f0: 2061 7265 2064 6573 6372 6962 6564 2062   are described b
-0001a900: 7920 7468 6520 666f 6c6c 6f77 696e 6720  y the following 
-0001a910: 6c65 7869 6361 6c20 6465 6669 6e69 7469  lexical definiti
-0001a920: 6f6e 733a 0a60 6060 636f 636f 6e75 740a  ons:.```coconut.
-0001a930: 696d 6167 6e75 6d62 6572 203a 3a3d 2028  imagnumber ::= (
-0001a940: 666c 6f61 746e 756d 6265 7220 7c20 696e  floatnumber | in
-0001a950: 7470 6172 7429 2028 226a 2220 7c20 224a  tpart) ("j" | "J
-0001a960: 2220 7c20 2269 2220 7c20 2249 2229 0a60  " | "i" | "I").`
-0001a970: 6060 0a41 6e20 696d 6167 696e 6172 7920  ``.An imaginary 
-0001a980: 6c69 7465 7261 6c20 7969 656c 6473 2061  literal yields a
-0001a990: 2063 6f6d 706c 6578 206e 756d 6265 7220   complex number 
-0001a9a0: 7769 7468 2061 2072 6561 6c20 7061 7274  with a real part
-0001a9b0: 206f 6620 302e 302e 2043 6f6d 706c 6578   of 0.0. Complex
-0001a9c0: 206e 756d 6265 7273 2061 7265 2072 6570   numbers are rep
-0001a9d0: 7265 7365 6e74 6564 2061 7320 6120 7061  resented as a pa
-0001a9e0: 6972 206f 6620 666c 6f61 7469 6e67 2070  ir of floating p
-0001a9f0: 6f69 6e74 206e 756d 6265 7273 2061 6e64  oint numbers and
-0001aa00: 2068 6176 6520 7468 6520 7361 6d65 2072   have the same r
-0001aa10: 6573 7472 6963 7469 6f6e 7320 6f6e 2074  estrictions on t
-0001aa20: 6865 6972 2072 616e 6765 2e20 546f 2063  heir range. To c
-0001aa30: 7265 6174 6520 6120 636f 6d70 6c65 7820  reate a complex 
-0001aa40: 6e75 6d62 6572 2077 6974 6820 6120 6e6f  number with a no
-0001aa50: 6e7a 6572 6f20 7265 616c 2070 6172 742c  nzero real part,
-0001aa60: 2061 6464 2061 2066 6c6f 6174 696e 6720   add a floating 
-0001aa70: 706f 696e 7420 6e75 6d62 6572 2074 6f20  point number to 
-0001aa80: 6974 2c20 652e 672e 2c20 6028 332b 3469  it, e.g., `(3+4i
-0001aa90: 2960 2e20 536f 6d65 2065 7861 6d70 6c65  )`. Some example
-0001aaa0: 7320 6f66 2069 6d61 6769 6e61 7279 206c  s of imaginary l
-0001aab0: 6974 6572 616c 733a 0a60 6060 636f 636f  iterals:.```coco
-0001aac0: 6e75 740a 332e 3134 6920 2020 3130 2e69  nut.3.14i   10.i
-0001aad0: 2020 2020 3130 6920 2020 2020 2e30 3031      10i     .001
-0001aae0: 6920 2020 3165 3130 3069 2020 332e 3134  i   1e100i  3.14
-0001aaf0: 652d 3130 690a 6060 600a 0a23 2323 2323  e-10i.```..#####
-0001ab00: 2045 7861 6d70 6c65 0a0a 2a2a 436f 636f   Example..**Coco
-0001ab10: 6e75 743a 2a2a 0a60 6060 636f 636f 6e75  nut:**.```coconu
-0001ab20: 740a 3320 2b20 3469 207c 3e20 6162 7320  t.3 + 4i |> abs 
-0001ab30: 7c3e 2070 7269 6e74 0a60 6060 0a0a 2a2a  |> print.```..**
-0001ab40: 5079 7468 6f6e 3a2a 2a0a 6060 6063 6f63  Python:**.```coc
-0001ab50: 6f6e 7574 5f70 7974 686f 6e0a 7072 696e  onut_python.prin
-0001ab60: 7428 6162 7328 3320 2b20 346a 2929 0a60  t(abs(3 + 4j)).`
-0001ab70: 6060 0a0a 2323 2320 416c 7465 726e 6174  ``..### Alternat
-0001ab80: 6976 6520 5465 726e 6172 7920 4f70 6572  ive Ternary Oper
-0001ab90: 6174 6f72 0a0a 5079 7468 6f6e 2073 7570  ator..Python sup
-0001aba0: 706f 7274 7320 7468 6520 7465 726e 6172  ports the ternar
-0001abb0: 7920 6f70 6572 6174 6f72 2073 796e 7461  y operator synta
-0001abc0: 780a 6060 6063 6f63 6f6e 7574 5f70 7974  x.```coconut_pyt
-0001abd0: 686f 6e0a 7265 7375 6c74 203d 2069 665f  hon.result = if_
-0001abe0: 7472 7565 2069 6620 636f 6e64 6974 696f  true if conditio
-0001abf0: 6e20 656c 7365 2069 665f 6661 6c73 650a  n else if_false.
-0001ac00: 6060 600a 7768 6963 682c 2073 696e 6365  ```.which, since
-0001ac10: 2043 6f63 6f6e 7574 2069 7320 6120 7375   Coconut is a su
-0001ac20: 7065 7273 6574 206f 6620 5079 7468 6f6e  perset of Python
-0001ac30: 2c20 436f 636f 6e75 7420 616c 736f 2073  , Coconut also s
-0001ac40: 7570 706f 7274 732e 0a0a 486f 7765 7665  upports...Howeve
-0001ac50: 722c 2043 6f63 6f6e 7574 2061 6c73 6f20  r, Coconut also 
-0001ac60: 7072 6f76 6964 6573 2061 6e20 616c 7465  provides an alte
-0001ac70: 726e 6174 6976 6520 7379 6e74 6178 2074  rnative syntax t
-0001ac80: 6861 7420 7573 6573 2074 6865 206d 6f72  hat uses the mor
-0001ac90: 6520 636f 6e76 656e 7469 6f6e 616c 2061  e conventional a
-0001aca0: 7267 756d 656e 7420 6f72 6465 7269 6e67  rgument ordering
-0001acb0: 2061 730a 6060 600a 7265 7375 6c74 203d   as.```.result =
-0001acc0: 2069 6620 636f 6e64 6974 696f 6e20 7468   if condition th
-0001acd0: 656e 2069 665f 7472 7565 2065 6c73 6520  en if_true else 
-0001ace0: 6966 5f66 616c 7365 0a60 6060 0a6d 616b  if_false.```.mak
-0001acf0: 696e 6720 7573 6520 6f66 2074 6865 2043  ing use of the C
-0001ad00: 6f63 6f6e 7574 2d73 7065 6369 6669 6320  oconut-specific 
-0001ad10: 6074 6865 6e60 206b 6579 776f 7264 2028  `then` keyword (
-0001ad20: 5b74 686f 7567 6820 436f 636f 6e75 7420  [though Coconut 
-0001ad30: 7374 696c 6c20 616c 6c6f 7773 2060 7468  still allows `th
-0001ad40: 656e 6020 6173 2061 2076 6172 6961 626c  en` as a variabl
-0001ad50: 6520 6e61 6d65 5d28 2368 616e 646c 696e  e name](#handlin
-0001ad60: 672d 6b65 7977 6f72 642d 7661 7269 6162  g-keyword-variab
-0001ad70: 6c65 2d6e 616d 652d 6f76 6572 6c61 7029  le-name-overlap)
-0001ad80: 292e 0a0a 2323 2323 2320 4578 616d 706c  )...##### Exampl
-0001ad90: 650a 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a  e..**Coconut:**.
-0001ada0: 6060 6063 6f63 6f6e 7574 0a76 616c 7565  ```coconut.value
-0001adb0: 203d 2028 0a20 2020 2069 6620 7368 6f75   = (.    if shou
-0001adc0: 6c64 5f75 7365 5f61 2829 2074 6865 6e20  ld_use_a() then 
-0001add0: 610a 2020 2020 656c 7365 2069 6620 7368  a.    else if sh
-0001ade0: 6f75 6c64 5f75 7365 5f62 2829 2074 6865  ould_use_b() the
-0001adf0: 6e20 620a 2020 2020 656c 7365 2069 6620  n b.    else if 
-0001ae00: 7368 6f75 6c64 5f75 7365 5f63 2829 2074  should_use_c() t
-0001ae10: 6865 6e20 630a 2020 2020 656c 7365 2066  hen c.    else f
-0001ae20: 616c 6c62 6163 6b0a 290a 6060 600a 0a2a  allback.).```..*
-0001ae30: 2a50 7974 686f 6e3a 2a2a 0a60 6060 636f  *Python:**.```co
-0001ae40: 636f 6e75 745f 7079 7468 6f6e 0a76 616c  conut_python.val
-0001ae50: 7565 203d 2028 0a20 2020 2061 2069 6620  ue = (.    a if 
-0001ae60: 7368 6f75 6c64 5f75 7365 5f61 2829 2065  should_use_a() e
-0001ae70: 6c73 650a 2020 2020 6220 6966 2073 686f  lse.    b if sho
-0001ae80: 756c 645f 7573 655f 6228 2920 656c 7365  uld_use_b() else
-0001ae90: 0a20 2020 2063 2069 6620 7368 6f75 6c64  .    c if should
-0001aea0: 5f75 7365 5f63 2829 2065 6c73 650a 2020  _use_c() else.  
-0001aeb0: 2020 6661 6c6c 6261 636b 0a29 0a60 6060    fallback.).```
-0001aec0: 0a0a 2323 2046 756e 6374 696f 6e20 4465  ..## Function De
-0001aed0: 6669 6e69 7469 6f6e 0a0a 6060 607b 636f  finition..```{co
-0001aee0: 6e74 656e 7473 7d0a 2d2d 2d0a 6c6f 6361  ntents}.---.loca
-0001aef0: 6c3a 0a64 6570 7468 3a20 310a 2d2d 2d0a  l:.depth: 1.---.
-0001af00: 6060 600a 0a23 2323 2054 6169 6c20 4361  ```..### Tail Ca
-0001af10: 6c6c 204f 7074 696d 697a 6174 696f 6e0a  ll Optimization.
-0001af20: 0a43 6f63 6f6e 7574 2077 696c 6c20 7065  .Coconut will pe
-0001af30: 7266 6f72 6d20 6175 746f 6d61 7469 6320  rform automatic 
-0001af40: 5b74 6169 6c20 6361 6c6c 5d28 6874 7470  [tail call](http
-0001af50: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
-0001af60: 2e6f 7267 2f77 696b 692f 5461 696c 5f63  .org/wiki/Tail_c
-0001af70: 616c 6c29 206f 7074 696d 697a 6174 696f  all) optimizatio
-0001af80: 6e20 616e 6420 7461 696c 2072 6563 7572  n and tail recur
-0001af90: 7369 6f6e 2065 6c69 6d69 6e61 7469 6f6e  sion elimination
-0001afa0: 206f 6e20 616e 7920 6675 6e63 7469 6f6e   on any function
-0001afb0: 2074 6861 7420 6d65 6574 7320 7468 6520   that meets the 
-0001afc0: 666f 6c6c 6f77 696e 6720 6372 6974 6572  following criter
-0001afd0: 6961 3a0a 0a31 2e20 6974 206d 7573 7420  ia:..1. it must 
-0001afe0: 6469 7265 6374 6c79 2072 6574 7572 6e20  directly return 
-0001aff0: 2875 7369 6e67 2065 6974 6865 7220 6072  (using either `r
-0001b000: 6574 7572 6e60 206f 7220 5b61 7373 6967  eturn` or [assig
-0001b010: 6e6d 656e 7420 6675 6e63 7469 6f6e 206e  nment function n
-0001b020: 6f74 6174 696f 6e5d 2823 6173 7369 676e  otation](#assign
-0001b030: 6d65 6e74 2d66 756e 6374 696f 6e73 2929  ment-functions))
-0001b040: 2061 2063 616c 6c20 746f 2069 7473 656c   a call to itsel
-0001b050: 6620 2874 6169 6c20 7265 6375 7273 696f  f (tail recursio
-0001b060: 6e20 656c 696d 696e 6174 696f 6e2c 2074  n elimination, t
-0001b070: 6865 206d 6f73 7420 706f 7765 7266 756c  he most powerful
-0001b080: 206f 7074 696d 697a 6174 696f 6e29 206f   optimization) o
-0001b090: 7220 616e 6f74 6865 7220 6675 6e63 7469  r another functi
-0001b0a0: 6f6e 2028 7461 696c 2063 616c 6c20 6f70  on (tail call op
-0001b0b0: 7469 6d69 7a61 7469 6f6e 292c 0a32 2e20  timization),.2. 
-0001b0c0: 6974 206d 7573 7420 6e6f 7420 6265 2061  it must not be a
-0001b0d0: 2067 656e 6572 6174 6f72 2028 7573 6573   generator (uses
-0001b0e0: 2060 7969 656c 6460 2920 6f72 2061 6e20   `yield`) or an 
-0001b0f0: 6173 796e 6368 726f 6e6f 7573 2066 756e  asynchronous fun
-0001b100: 6374 696f 6e20 2875 7365 7320 6061 7379  ction (uses `asy
-0001b110: 6e63 6029 2e0a 0a54 6169 6c20 6361 6c6c  nc`)...Tail call
-0001b120: 206f 7074 696d 697a 6174 696f 6e20 2874   optimization (t
-0001b130: 686f 7567 6820 6e6f 7420 7461 696c 2072  hough not tail r
-0001b140: 6563 7572 7369 6f6e 2065 6c69 6d69 6e61  ecursion elimina
-0001b150: 7469 6f6e 2920 7769 6c6c 2077 6f72 6b20  tion) will work 
-0001b160: 6576 656e 2066 6f72 2031 2920 6d75 7475  even for 1) mutu
-0001b170: 616c 2072 6563 7572 7369 6f6e 2061 6e64  al recursion and
-0001b180: 2032 2920 7061 7474 6572 6e2d 6d61 7463   2) pattern-matc
-0001b190: 6869 6e67 2066 756e 6374 696f 6e73 2073  hing functions s
-0001b1a0: 706c 6974 2061 6372 6f73 7320 6d75 6c74  plit across mult
-0001b1b0: 6970 6c65 2064 6566 696e 6974 696f 6e73  iple definitions
-0001b1c0: 2075 7369 6e67 205b 6061 6464 7061 7474   using [`addpatt
-0001b1d0: 6572 6e60 5d28 2361 6464 7061 7474 6572  ern`](#addpatter
-0001b1e0: 6e29 2e0a 0a49 6620 796f 7520 6172 6520  n)...If you are 
-0001b1f0: 656e 636f 756e 7465 7269 6e67 2061 2060  encountering a `
-0001b200: 5275 6e74 696d 6545 7272 6f72 6020 6475  RuntimeError` du
-0001b210: 6520 746f 206d 6178 696d 756d 2072 6563  e to maximum rec
-0001b220: 7572 7369 6f6e 2064 6570 7468 2c20 6974  ursion depth, it
-0001b230: 2069 7320 6869 6768 6c79 2072 6563 6f6d   is highly recom
-0001b240: 6d65 6e64 6564 2074 6861 7420 796f 7520  mended that you 
-0001b250: 7265 7772 6974 6520 796f 7572 2066 756e  rewrite your fun
-0001b260: 6374 696f 6e20 746f 206d 6565 7420 6569  ction to meet ei
-0001b270: 7468 6572 2074 6865 2063 7269 7465 7269  ther the criteri
-0001b280: 6120 6162 6f76 6520 666f 7220 7461 696c  a above for tail
-0001b290: 2063 616c 6c20 6f70 7469 6d69 7a61 7469   call optimizati
-0001b2a0: 6f6e 2c20 6f72 2074 6865 2063 6f72 7265  on, or the corre
-0001b2b0: 7370 6f6e 6469 6e67 2063 7269 7465 7269  sponding criteri
-0001b2c0: 6120 666f 7220 5b60 7265 6375 7273 6976  a for [`recursiv
-0001b2d0: 655f 6974 6572 6174 6f72 605d 2823 7265  e_iterator`](#re
-0001b2e0: 6375 7273 6976 652d 6974 6572 6174 6f72  cursive-iterator
-0001b2f0: 292c 2065 6974 6865 7220 6f66 2077 6869  ), either of whi
-0001b300: 6368 2073 686f 756c 6420 7072 6576 656e  ch should preven
-0001b310: 7420 7375 6368 2065 7272 6f72 732e 0a0a  t such errors...
-0001b320: 2323 2323 2320 4578 616d 706c 650a 0a2a  ##### Example..*
-0001b330: 2a43 6f63 6f6e 7574 3a2a 2a0a 6060 6063  *Coconut:**.```c
-0001b340: 6f63 6f6e 7574 0a23 2075 6e6c 696b 6520  oconut.# unlike 
-0001b350: 696e 2050 7974 686f 6e2c 2074 6869 7320  in Python, this 
-0001b360: 6675 6e63 7469 6f6e 2077 696c 6c20 6e65  function will ne
-0001b370: 7665 7220 6869 7420 6120 6d61 7869 6d75  ver hit a maximu
-0001b380: 6d20 7265 6375 7273 696f 6e20 6465 7074  m recursion dept
-0001b390: 6820 6572 726f 720a 6465 6620 6661 6374  h error.def fact
-0001b3a0: 6f72 6961 6c28 6e2c 2061 6363 3d31 293a  orial(n, acc=1):
-0001b3b0: 0a20 2020 206d 6174 6368 206e 3a0a 2020  .    match n:.  
-0001b3c0: 2020 2020 2020 6361 7365 2030 3a0a 2020        case 0:.  
-0001b3d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001b3e0: 2061 6363 0a20 2020 2020 2020 2063 6173   acc.        cas
-0001b3f0: 6520 696e 7428 2920 6966 206e 203e 2030  e int() if n > 0
-0001b400: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0001b410: 7475 726e 2066 6163 746f 7269 616c 286e  turn factorial(n
-0001b420: 2d31 2c20 6163 632a 6e29 0a60 6060 0a5f  -1, acc*n).```._
-0001b430: 5368 6f77 6361 7365 7320 7461 696c 2072  Showcases tail r
-0001b440: 6563 7572 7369 6f6e 2065 6c69 6d69 6e61  ecursion elimina
-0001b450: 7469 6f6e 2e5f 0a0a 6060 6063 6f63 6f6e  tion._..```cocon
-0001b460: 7574 0a23 2075 6e6c 696b 6520 696e 2050  ut.# unlike in P
-0001b470: 7974 686f 6e2c 206e 6569 7468 6572 206f  ython, neither o
-0001b480: 6620 7468 6573 6520 6675 6e63 7469 6f6e  f these function
-0001b490: 7320 7769 6c6c 2065 7665 7220 6869 7420  s will ever hit 
-0001b4a0: 6120 6d61 7869 6d75 6d20 7265 6375 7273  a maximum recurs
-0001b4b0: 696f 6e20 6465 7074 6820 6572 726f 720a  ion depth error.
-0001b4c0: 6465 6620 6973 5f65 7665 6e28 3029 203d  def is_even(0) =
-0001b4d0: 2054 7275 650a 6164 6470 6174 7465 726e   True.addpattern
-0001b4e0: 2064 6566 2069 735f 6576 656e 286e 2060   def is_even(n `
-0001b4f0: 6973 696e 7374 616e 6365 6020 696e 7420  isinstance` int 
-0001b500: 6966 206e 203e 2030 2920 3d20 6973 5f6f  if n > 0) = is_o
-0001b510: 6464 286e 2d31 290a 0a64 6566 2069 735f  dd(n-1)..def is_
-0001b520: 6f64 6428 3029 203d 2046 616c 7365 0a61  odd(0) = False.a
-0001b530: 6464 7061 7474 6572 6e20 6465 6620 6973  ddpattern def is
-0001b540: 5f6f 6464 286e 2060 6973 696e 7374 616e  _odd(n `isinstan
-0001b550: 6365 6020 696e 7420 6966 206e 203e 2030  ce` int if n > 0
-0001b560: 2920 3d20 6973 5f65 7665 6e28 6e2d 3129  ) = is_even(n-1)
-0001b570: 0a60 6060 0a5f 5368 6f77 6361 7365 7320  .```._Showcases 
-0001b580: 7461 696c 2063 616c 6c20 6f70 7469 6d69  tail call optimi
-0001b590: 7a61 7469 6f6e 2e5f 0a0a 2a2a 5079 7468  zation._..**Pyth
-0001b5a0: 6f6e 3a2a 2a0a 5f43 616e 2774 2062 6520  on:**._Can't be 
-0001b5b0: 646f 6e65 2077 6974 686f 7574 2072 6577  done without rew
-0001b5c0: 7269 7469 6e67 2074 6865 2066 756e 6374  riting the funct
-0001b5d0: 696f 6e28 7329 2e5f 0a0a 2323 2323 2060  ion(s)._..#### `
-0001b5e0: 2d2d 6e6f 2d74 636f 6020 666c 6167 0a0a  --no-tco` flag..
-0001b5f0: 5461 696c 2063 616c 6c20 6f70 7469 6d69  Tail call optimi
-0001b600: 7a61 7469 6f6e 2077 696c 6c20 6265 2074  zation will be t
-0001b610: 7572 6e65 6420 6f66 6620 6966 2079 6f75  urned off if you
-0001b620: 2070 6173 7320 7468 6520 602d 2d6e 6f2d   pass the `--no-
-0001b630: 7463 6f60 2063 6f6d 6d61 6e64 2d6c 696e  tco` command-lin
-0001b640: 6520 6f70 7469 6f6e 2c20 7768 6963 6820  e option, which 
-0001b650: 6973 2075 7365 6675 6c20 6966 2079 6f75  is useful if you
-0001b660: 2061 7265 2068 6176 696e 6720 7472 6f75   are having trou
-0001b670: 626c 6520 7265 6164 696e 6720 796f 7572  ble reading your
-0001b680: 2074 7261 6365 6261 636b 7320 616e 642f   tracebacks and/
-0001b690: 6f72 206e 6565 6420 6d61 7869 6d75 6d20  or need maximum 
-0001b6a0: 7065 7266 6f72 6d61 6e63 652e 0a0a 602d  performance...`-
-0001b6b0: 2d6e 6f2d 7463 6f60 2064 6f65 7320 6e6f  -no-tco` does no
-0001b6c0: 7420 6469 7361 626c 6520 7461 696c 2072  t disable tail r
-0001b6d0: 6563 7572 7369 6f6e 2065 6c69 6d69 6e61  ecursion elimina
-0001b6e0: 7469 6f6e 2e0a 5468 6973 2069 7320 6265  tion..This is be
-0001b6f0: 6361 7573 6520 7461 696c 2072 6563 7572  cause tail recur
-0001b700: 7369 6f6e 2065 6c69 6d69 6e61 7469 6f6e  sion elimination
-0001b710: 2069 7320 7573 7561 6c6c 7920 6661 7374   is usually fast
-0001b720: 6572 2074 6861 6e20 646f 696e 6720 6e6f  er than doing no
-0001b730: 7468 696e 672c 2077 6869 6c65 206f 7468  thing, while oth
-0001b740: 6572 2074 7970 6573 206f 6620 7461 696c  er types of tail
-0001b750: 2063 616c 6c20 6f70 7469 6d69 7a61 7469   call optimizati
-0001b760: 6f6e 2061 7265 2075 7375 616c 6c79 2073  on are usually s
-0001b770: 6c6f 7765 7220 7468 616e 2064 6f69 6e67  lower than doing
-0001b780: 206e 6f74 6869 6e67 2e0a 5461 696c 2072   nothing..Tail r
-0001b790: 6563 7572 7369 6f6e 2065 6c69 6d69 6e61  ecursion elimina
-0001b7a0: 7469 6f6e 2072 6573 756c 7473 2069 6e20  tion results in 
-0001b7b0: 6120 6269 6720 7065 7266 6f72 6d61 6e63  a big performanc
-0001b7c0: 6520 7769 6e20 6265 6361 7573 6520 5079  e win because Py
-0001b7d0: 7468 6f6e 2068 6173 2061 2066 6169 726c  thon has a fairl
-0001b7e0: 7920 6c61 7267 6520 6675 6e63 7469 6f6e  y large function
-0001b7f0: 2063 616c 6c20 6f76 6572 6865 6164 2e20   call overhead. 
-0001b800: 4279 2075 6e77 696e 6469 6e67 2061 2072  By unwinding a r
-0001b810: 6563 7572 7369 7665 2066 756e 6374 696f  ecursive functio
-0001b820: 6e2c 2066 6172 2066 6577 6572 2066 756e  n, far fewer fun
-0001b830: 6374 696f 6e20 6361 6c6c 7320 6e65 6564  ction calls need
-0001b840: 2074 6f20 6265 206d 6164 652e 0a57 6865   to be made..Whe
-0001b850: 6e20 7468 6520 602d 2d6e 6f2d 7463 6f60  n the `--no-tco`
-0001b860: 2066 6c61 6720 6973 2064 6973 6162 6c65   flag is disable
-0001b870: 642c 2043 6f63 6f6e 7574 2077 696c 6c20  d, Coconut will 
-0001b880: 6174 7465 6d70 7420 746f 2064 6f20 616c  attempt to do al
-0001b890: 6c20 7479 7065 7320 6f66 2074 6169 6c20  l types of tail 
-0001b8a0: 6361 6c6c 206f 7074 696d 697a 6174 696f  call optimizatio
-0001b8b0: 6e73 2c20 6861 6e64 6c69 6e67 206e 6f6e  ns, handling non
-0001b8c0: 2d72 6563 7572 7369 7665 2074 6169 6c20  -recursive tail 
-0001b8d0: 6361 6c6c 732c 2073 706c 6974 2070 6174  calls, split pat
-0001b8e0: 7465 726e 2d6d 6174 6368 696e 6720 6675  tern-matching fu
-0001b8f0: 6e63 7469 6f6e 732c 206d 7574 7561 6c20  nctions, mutual 
-0001b900: 7265 6375 7273 696f 6e2c 2061 6e64 2074  recursion, and t
-0001b910: 6169 6c20 7265 6375 7273 696f 6e2e 2057  ail recursion. W
-0001b920: 6865 6e20 7468 6520 602d 2d6e 6f2d 7463  hen the `--no-tc
-0001b930: 6f60 2066 6c61 6720 6973 2065 6e61 626c  o` flag is enabl
-0001b940: 6564 2c20 436f 636f 6e75 7420 7769 6c6c  ed, Coconut will
-0001b950: 206e 6f20 6c6f 6e67 6572 2070 6572 666f   no longer perfo
-0001b960: 726d 2061 6e79 2074 6169 6c20 6361 6c6c  rm any tail call
-0001b970: 206f 7074 696d 697a 6174 696f 6e73 206f   optimizations o
-0001b980: 7468 6572 2074 6861 6e20 7461 696c 2072  ther than tail r
-0001b990: 6563 7572 7369 6f6e 2065 6c69 6d69 6e61  ecursion elimina
-0001b9a0: 7469 6f6e 2e0a 0a23 2323 2320 5461 696c  tion...#### Tail
-0001b9b0: 2052 6563 7572 7369 6f6e 2045 6c69 6d69   Recursion Elimi
-0001b9c0: 6e61 7469 6f6e 2061 6e64 2050 7974 686f  nation and Pytho
-0001b9d0: 6e20 6c61 6d62 6461 730a 0a43 6f63 6f6e  n lambdas..Cocon
-0001b9e0: 7574 2064 6f65 7320 6e6f 7420 7065 7266  ut does not perf
-0001b9f0: 6f72 6d20 7461 696c 2072 6563 7572 7369  orm tail recursi
-0001ba00: 6f6e 2065 6c69 6d69 6e61 7469 6f6e 2069  on elimination i
-0001ba10: 6e20 6675 6e63 7469 6f6e 7320 7468 6174  n functions that
-0001ba20: 2075 7469 6c69 7a65 206c 616d 6264 6173   utilize lambdas
-0001ba30: 206f 7220 696e 6e65 7220 6675 6e63 7469   or inner functi
-0001ba40: 6f6e 732e 2054 6869 7320 6973 2062 6563  ons. This is bec
-0001ba50: 6175 7365 206f 6620 7468 6520 7761 7920  ause of the way 
-0001ba60: 7468 6174 2050 7974 686f 6e20 6861 6e64  that Python hand
-0001ba70: 6c65 7320 6c61 6d62 6461 732e 0a0a 4561  les lambdas...Ea
-0001ba80: 6368 206c 616d 6264 6120 7374 6f72 6573  ch lambda stores
-0001ba90: 2061 2070 6f69 6e74 6572 2074 6f20 7468   a pointer to th
-0001baa0: 6520 6e61 6d65 7370 6163 6520 656e 636c  e namespace encl
-0001bab0: 6f73 696e 6720 6974 2c20 7261 7468 6572  osing it, rather
-0001bac0: 2074 6861 6e20 6120 636f 7079 206f 6620   than a copy of 
-0001bad0: 7468 6520 6e61 6d65 7370 6163 652e 2054  the namespace. T
-0001bae0: 6875 732c 2069 6620 7468 6520 436f 636f  hus, if the Coco
-0001baf0: 6e75 7420 636f 6d70 696c 6572 2074 7269  nut compiler tri
-0001bb00: 6573 2074 6f20 7265 6379 636c 6520 616e  es to recycle an
-0001bb10: 7974 6869 6e67 2069 6e20 7468 6520 6e61  ything in the na
-0001bb20: 6d65 7370 6163 6520 7468 6174 2070 726f  mespace that pro
-0001bb30: 6475 6365 6420 7468 6520 6c61 6d62 6461  duced the lambda
-0001bb40: 2c20 7768 6963 6820 6e65 6564 7320 746f  , which needs to
-0001bb50: 2062 6520 646f 6e65 2066 6f72 2054 5245   be done for TRE
-0001bb60: 2c20 7468 6520 6c61 6d62 6461 2063 616e  , the lambda can
-0001bb70: 2062 6520 6368 616e 6765 6420 7265 7472   be changed retr
-0001bb80: 6f61 6374 6976 656c 792e 0a0a 4120 7369  oactively...A si
-0001bb90: 6d70 6c65 2065 7861 6d70 6c65 2064 656d  mple example dem
-0001bba0: 6f6e 7374 7261 7469 6e67 2074 6869 7320  onstrating this 
-0001bbb0: 6265 6861 7669 6f72 2069 6e20 5079 7468  behavior in Pyth
-0001bbc0: 6f6e 3a0a 0a60 6060 7079 7468 6f6e 0a78  on:..```python.x
-0001bbd0: 203d 2031 0a66 6f6f 203d 206c 616d 6264   = 1.foo = lambd
-0001bbe0: 613a 2078 0a70 7269 6e74 2866 6f6f 2829  a: x.print(foo()
-0001bbf0: 2920 2023 2031 0a78 203d 2032 2020 2020  )  # 1.x = 2    
-0001bc00: 2020 2020 2023 2044 6972 6563 746c 7920       # Directly 
-0001bc10: 616c 7465 7220 7468 6520 7661 6c75 6573  alter the values
-0001bc20: 2069 6e20 7468 6520 6e61 6d65 7370 6163   in the namespac
-0001bc30: 6520 656e 636c 6f73 696e 6720 666f 6f0a  e enclosing foo.
-0001bc40: 7072 696e 7428 666f 6f28 2929 2020 2320  print(foo())  # 
-0001bc50: 3220 2821 290a 6060 600a 0a42 6563 6175  2 (!).```..Becau
-0001bc60: 7365 2074 6869 7320 636f 756c 6420 6861  se this could ha
-0001bc70: 7665 2075 6e69 6e74 656e 6465 6420 616e  ve unintended an
-0001bc80: 6420 706f 7465 6e74 6961 6c6c 7920 6461  d potentially da
-0001bc90: 6d61 6769 6e67 2063 6f6e 7365 7175 656e  maging consequen
-0001bca0: 6365 732c 2043 6f63 6f6e 7574 206f 7074  ces, Coconut opt
-0001bcb0: 7320 746f 206e 6f74 2070 6572 666f 726d  s to not perform
-0001bcc0: 2054 5245 206f 6e20 616e 7920 6675 6e63   TRE on any func
-0001bcd0: 7469 6f6e 2077 6974 6820 6120 6c61 6d62  tion with a lamb
-0001bce0: 6461 206f 7220 696e 6e65 7220 6675 6e63  da or inner func
-0001bcf0: 7469 6f6e 2e0a 0a23 2323 2041 7373 6967  tion...### Assig
-0001bd00: 6e6d 656e 7420 4675 6e63 7469 6f6e 730a  nment Functions.
-0001bd10: 0a43 6f63 6f6e 7574 2061 6c6c 6f77 7320  .Coconut allows 
-0001bd20: 666f 7220 6173 7369 676e 6d65 6e74 2066  for assignment f
-0001bd30: 756e 6374 696f 6e20 6465 6669 6e69 7469  unction definiti
-0001bd40: 6f6e 2074 6861 7420 6175 746f 6d61 7469  on that automati
-0001bd50: 6361 6c6c 7920 7265 7475 726e 7320 7468  cally returns th
-0001bd60: 6520 6c61 7374 206c 696e 6520 6f66 2074  e last line of t
-0001bd70: 6865 2066 756e 6374 696f 6e20 626f 6479  he function body
-0001bd80: 2e20 416e 2061 7373 6967 6e6d 656e 7420  . An assignment 
-0001bd90: 6675 6e63 7469 6f6e 2069 7320 636f 6e73  function is cons
-0001bda0: 7472 7563 7465 6420 6279 2073 7562 7374  tructed by subst
-0001bdb0: 6974 7574 696e 6720 603d 6020 666f 7220  ituting `=` for 
-0001bdc0: 603a 6020 6166 7465 7220 7468 6520 6675  `:` after the fu
-0001bdd0: 6e63 7469 6f6e 2064 6566 696e 6974 696f  nction definitio
-0001bde0: 6e20 6c69 6e65 2e20 5468 7573 2c20 7468  n line. Thus, th
-0001bdf0: 6520 7379 6e74 6178 2066 6f72 2061 7373  e syntax for ass
-0001be00: 6967 6e6d 656e 7420 6675 6e63 7469 6f6e  ignment function
-0001be10: 2064 6566 696e 6974 696f 6e20 6973 2065   definition is e
-0001be20: 6974 6865 720a 6060 6063 6f63 6f6e 7574  ither.```coconut
-0001be30: 0a5b 6173 796e 635d 2064 6566 203c 6e61  .[async] def <na
-0001be40: 6d65 3e28 3c61 7267 733e 2920 3d20 3c65  me>(<args>) = <e
-0001be50: 7870 723e 0a60 6060 0a66 6f72 206f 6e65  xpr>.```.for one
-0001be60: 2d6c 696e 6572 7320 6f72 0a60 6060 636f  -liners or.```co
-0001be70: 636f 6e75 740a 5b61 7379 6e63 5d20 6465  conut.[async] de
-0001be80: 6620 3c6e 616d 653e 283c 6172 6773 3e29  f <name>(<args>)
-0001be90: 203d 0a20 2020 203c 7374 6d74 733e 0a20   =.    <stmts>. 
-0001bea0: 2020 203c 6578 7072 3e0a 6060 600a 666f     <expr>.```.fo
-0001beb0: 7220 6675 6c6c 2066 756e 6374 696f 6e73  r full functions
-0001bec0: 2c20 7768 6572 6520 603c 6e61 6d65 3e60  , where `<name>`
-0001bed0: 2069 7320 7468 6520 6e61 6d65 206f 6620   is the name of 
-0001bee0: 7468 6520 6675 6e63 7469 6f6e 2c20 603c  the function, `<
-0001bef0: 6172 6773 3e60 2061 7265 2074 6865 2066  args>` are the f
-0001bf00: 756e 6374 696f 6e73 2061 7267 756d 656e  unctions argumen
-0001bf10: 7473 2c20 603c 7374 6d74 733e 6020 6172  ts, `<stmts>` ar
-0001bf20: 6520 616e 7920 7374 6174 656d 656e 7473  e any statements
-0001bf30: 2074 6861 7420 7468 6520 6675 6e63 7469   that the functi
-0001bf40: 6f6e 2073 686f 756c 6420 6578 6563 7574  on should execut
-0001bf50: 652c 2061 6e64 2060 3c65 7870 723e 6020  e, and `<expr>` 
-0001bf60: 6973 2074 6865 2076 616c 7565 2074 6861  is the value tha
-0001bf70: 7420 7468 6520 6675 6e63 7469 6f6e 2073  t the function s
-0001bf80: 686f 756c 6420 7265 7475 726e 2e0a 0a5f  hould return..._
-0001bf90: 4e6f 7465 3a20 4173 7369 676e 6d65 6e74  Note: Assignment
-0001bfa0: 2066 756e 6374 696f 6e20 6465 6669 6e69   function defini
-0001bfb0: 7469 6f6e 2063 616e 2062 6520 636f 6d62  tion can be comb
-0001bfc0: 696e 6564 2077 6974 6820 696e 6669 7820  ined with infix 
-0001bfd0: 616e 642f 6f72 2070 6174 7465 726e 2d6d  and/or pattern-m
-0001bfe0: 6174 6368 696e 6720 6675 6e63 7469 6f6e  atching function
-0001bff0: 2064 6566 696e 6974 696f 6e2e 5f0a 0a23   definition._..#
-0001c000: 2323 2323 2052 6174 696f 6e61 6c65 0a0a  #### Rationale..
-0001c010: 436f 636f 6e75 7427 7320 4173 7369 676e  Coconut's Assign
-0001c020: 6d65 6e74 2066 756e 6374 696f 6e20 6465  ment function de
-0001c030: 6669 6e69 7469 6f6e 2069 7320 6173 2065  finition is as e
-0001c040: 6173 7920 746f 2077 7269 7465 2061 7320  asy to write as 
-0001c050: 6173 7369 676e 6d65 6e74 2074 6f20 6120  assignment to a 
-0001c060: 6c61 6d62 6461 2c20 6275 7420 7769 6c6c  lambda, but will
-0001c070: 2061 7070 6561 7220 6e61 6d65 6420 696e   appear named in
-0001c080: 2074 7261 6365 6261 636b 732c 2061 7320   tracebacks, as 
-0001c090: 6974 2063 6f6d 7069 6c65 7320 746f 206e  it compiles to n
-0001c0a0: 6f72 6d61 6c20 5079 7468 6f6e 2066 756e  ormal Python fun
-0001c0b0: 6374 696f 6e20 6465 6669 6e69 7469 6f6e  ction definition
-0001c0c0: 2e0a 0a23 2323 2323 2045 7861 6d70 6c65  ...##### Example
-0001c0d0: 0a0a 2a2a 436f 636f 6e75 743a 2a2a 0a60  ..**Coconut:**.`
-0001c0e0: 6060 636f 636f 6e75 740a 6465 6620 6269  ``coconut.def bi
-0001c0f0: 6e65 7870 2878 2920 3d20 322a 2a78 0a35  nexp(x) = 2**x.5
-0001c100: 207c 3e20 6269 6e65 7870 207c 3e20 7072   |> binexp |> pr
-0001c110: 696e 740a 6060 600a 0a2a 2a50 7974 686f  int.```..**Pytho
-0001c120: 6e3a 2a2a 0a60 6060 636f 636f 6e75 745f  n:**.```coconut_
-0001c130: 7079 7468 6f6e 0a64 6566 2062 696e 6578  python.def binex
-0001c140: 7028 7829 3a20 7265 7475 726e 2032 2a2a  p(x): return 2**
-0001c150: 780a 7072 696e 7428 6269 6e65 7870 2835  x.print(binexp(5
-0001c160: 2929 0a60 6060 0a0a 2323 2320 5061 7474  )).```..### Patt
-0001c170: 6572 6e2d 4d61 7463 6869 6e67 2046 756e  ern-Matching Fun
-0001c180: 6374 696f 6e73 0a0a 436f 636f 6e75 7420  ctions..Coconut 
-0001c190: 7061 7474 6572 6e2d 6d61 7463 6869 6e67  pattern-matching
-0001c1a0: 2066 756e 6374 696f 6e73 2061 7265 206a   functions are j
-0001c1b0: 7573 7420 6e6f 726d 616c 2066 756e 6374  ust normal funct
-0001c1c0: 696f 6e73 2c20 6578 6365 7074 2077 6865  ions, except whe
-0001c1d0: 7265 2074 6865 2061 7267 756d 656e 7473  re the arguments
-0001c1e0: 2061 7265 2070 6174 7465 726e 7320 746f   are patterns to
-0001c1f0: 2062 6520 6d61 7463 6865 6420 6167 6169   be matched agai
-0001c200: 6e73 7420 696e 7374 6561 6420 6f66 2076  nst instead of v
-0001c210: 6172 6961 626c 6573 2074 6f20 6265 2061  ariables to be a
-0001c220: 7373 6967 6e65 6420 746f 2e20 5468 6520  ssigned to. The 
-0001c230: 7379 6e74 6178 2066 6f72 2070 6174 7465  syntax for patte
-0001c240: 726e 2d6d 6174 6368 696e 6720 6675 6e63  rn-matching func
-0001c250: 7469 6f6e 2064 6566 696e 6974 696f 6e20  tion definition 
-0001c260: 6973 0a60 6060 636f 636f 6e75 740a 5b6d  is.```coconut.[m
-0001c270: 6174 6368 5d20 6465 6620 3c6e 616d 653e  atch] def <name>
-0001c280: 283c 6172 673e 2c20 3c61 7267 3e2c 202e  (<arg>, <arg>, .
-0001c290: 2e2e 205b 6966 203c 636f 6e64 3e5d 2920  .. [if <cond>]) 
-0001c2a0: 5b2d 3e20 3c72 6574 7572 6e5f 7479 7065  [-> <return_type
-0001c2b0: 3e5d 3a0a 2020 2020 3c62 6f64 793e 0a60  >]:.    <body>.`
-0001c2c0: 6060 0a77 6865 7265 2060 3c61 7267 3e60  ``.where `<arg>`
-0001c2d0: 2069 7320 6465 6669 6e65 6420 6173 0a60   is defined as.`
-0001c2e0: 6060 636f 636f 6e75 740a 5b2a 7c2a 2a5d  ``coconut.[*|**]
-0001c2f0: 203c 7061 7474 6572 6e3e 205b 3d20 3c64   <pattern> [= <d
-0001c300: 6566 6175 6c74 3e5d 0a60 6060 0a77 6865  efault>].```.whe
-0001c310: 7265 2060 3c6e 616d 653e 6020 6973 2074  re `<name>` is t
-0001c320: 6865 206e 616d 6520 6f66 2074 6865 2066  he name of the f
-0001c330: 756e 6374 696f 6e2c 2060 3c63 6f6e 643e  unction, `<cond>
-0001c340: 6020 6973 2061 6e20 6f70 7469 6f6e 616c  ` is an optional
-0001c350: 2061 6464 6974 696f 6e61 6c20 6368 6563   additional chec
-0001c360: 6b2c 2060 3c62 6f64 793e 6020 6973 2074  k, `<body>` is t
-0001c370: 6865 2062 6f64 7920 6f66 2074 6865 2066  he body of the f
-0001c380: 756e 6374 696f 6e2c 2060 3c70 6174 7465  unction, `<patte
-0001c390: 726e 3e60 2069 7320 6465 6669 6e65 6420  rn>` is defined 
-0001c3a0: 6279 2043 6f63 6f6e 7574 2773 205b 606d  by Coconut's [`m
-0001c3b0: 6174 6368 6020 7374 6174 656d 656e 745d  atch` statement]
-0001c3c0: 2823 6d61 7463 6829 2c20 603c 6465 6661  (#match), `<defa
-0001c3d0: 756c 743e 6020 6973 2074 6865 206f 7074  ult>` is the opt
-0001c3e0: 696f 6e61 6c20 6465 6661 756c 7420 6966  ional default if
-0001c3f0: 206e 6f20 6172 6775 6d65 6e74 2069 7320   no argument is 
-0001c400: 7061 7373 6564 2c20 616e 6420 603c 7265  passed, and `<re
-0001c410: 7475 726e 5f74 7970 653e 6020 6973 2074  turn_type>` is t
-0001c420: 6865 206f 7074 696f 6e61 6c20 7265 7475  he optional retu
-0001c430: 726e 2074 7970 6520 616e 6e6f 7461 7469  rn type annotati
-0001c440: 6f6e 2028 6e6f 7465 2074 6861 7420 6172  on (note that ar
-0001c450: 6775 6d65 6e74 2074 7970 6520 616e 6e6f  gument type anno
-0001c460: 7461 7469 6f6e 7320 6172 6520 6e6f 7420  tations are not 
-0001c470: 7375 7070 6f72 7465 6420 666f 7220 7061  supported for pa
-0001c480: 7474 6572 6e2d 6d61 7463 6869 6e67 2066  ttern-matching f
-0001c490: 756e 6374 696f 6e73 292e 2054 6865 2060  unctions). The `
-0001c4a0: 6d61 7463 6860 206b 6579 776f 7264 2061  match` keyword a
-0001c4b0: 7420 7468 6520 6265 6769 6e6e 696e 6720  t the beginning 
-0001c4c0: 6973 206f 7074 696f 6e61 6c2c 2062 7574  is optional, but
-0001c4d0: 2069 7320 736f 6d65 7469 6d65 7320 6e65   is sometimes ne
-0001c4e0: 6365 7373 6172 7920 746f 2064 6973 616d  cessary to disam
-0001c4f0: 6269 6775 6174 6520 7061 7474 6572 6e2d  biguate pattern-
-0001c500: 6d61 7463 6869 6e67 2066 756e 6374 696f  matching functio
-0001c510: 6e20 6465 6669 6e69 7469 6f6e 2066 726f  n definition fro
-0001c520: 6d20 6e6f 726d 616c 2066 756e 6374 696f  m normal functio
-0001c530: 6e20 6465 6669 6e69 7469 6f6e 2c20 7369  n definition, si
-0001c540: 6e63 6520 5079 7468 6f6e 2066 756e 6374  nce Python funct
-0001c550: 696f 6e20 6465 6669 6e69 7469 6f6e 2077  ion definition w
-0001c560: 696c 6c20 616c 7761 7973 2074 616b 6520  ill always take 
-0001c570: 7072 6563 6564 656e 6365 2e20 4e6f 7465  precedence. Note
-0001c580: 2074 6861 7420 7468 6520 6061 7379 6e63   that the `async
-0001c590: 6020 616e 6420 606d 6174 6368 6020 6b65  ` and `match` ke
-0001c5a0: 7977 6f72 6473 2063 616e 2062 6520 696e  ywords can be in
-0001c5b0: 2061 6e79 206f 7264 6572 2e0a 0a49 6620   any order...If 
-0001c5c0: 603c 7061 7474 6572 6e3e 6020 6861 7320  `<pattern>` has 
-0001c5d0: 6120 7661 7269 6162 6c65 206e 616d 6520  a variable name 
-0001c5e0: 2865 6974 6865 7220 6469 7265 6374 6c79  (either directly
-0001c5f0: 206f 7220 7769 7468 2060 6173 6029 2c20   or with `as`), 
-0001c600: 7468 6520 7265 7375 6c74 696e 6720 7061  the resulting pa
-0001c610: 7474 6572 6e2d 6d61 7463 6869 6e67 2066  ttern-matching f
-0001c620: 756e 6374 696f 6e20 7769 6c6c 2073 7570  unction will sup
-0001c630: 706f 7274 206b 6579 776f 7264 2061 7267  port keyword arg
-0001c640: 756d 656e 7473 2075 7369 6e67 2074 6861  uments using tha
-0001c650: 7420 7661 7269 6162 6c65 206e 616d 652e  t variable name.
-0001c660: 0a0a 496e 2061 6464 6974 696f 6e20 746f  ..In addition to
-0001c670: 2073 7570 706f 7274 696e 6720 7061 7474   supporting patt
-0001c680: 6572 6e2d 6d61 7463 6869 6e67 2069 6e20  ern-matching in 
-0001c690: 7468 6569 7220 6172 6775 6d65 6e74 732c  their arguments,
-0001c6a0: 2070 6174 7465 726e 2d6d 6174 6368 696e   pattern-matchin
-0001c6b0: 6720 6675 6e63 7469 6f6e 2064 6566 696e  g function defin
-0001c6c0: 6974 696f 6e73 2061 6c73 6f20 6861 7665  itions also have
-0001c6d0: 2061 2063 6f75 706c 6520 6f66 206e 6f74   a couple of not
-0001c6e0: 6162 6c65 2064 6966 6665 7265 6e63 6573  able differences
-0001c6f0: 2063 6f6d 7061 7265 6420 746f 2050 7974   compared to Pyt
-0001c700: 686f 6e20 6675 6e63 7469 6f6e 732e 2053  hon functions. S
-0001c710: 7065 6369 6669 6361 6c6c 793a 0a2d 2049  pecifically:.- I
-0001c720: 6620 7061 7474 6572 6e2d 6d61 7463 6869  f pattern-matchi
-0001c730: 6e67 2066 756e 6374 696f 6e20 6465 6669  ng function defi
-0001c740: 6e69 7469 6f6e 2066 6169 6c73 2c20 6974  nition fails, it
-0001c750: 2077 696c 6c20 7261 6973 6520 6120 5b60   will raise a [`
-0001c760: 4d61 7463 6845 7272 6f72 605d 2823 6d61  MatchError`](#ma
-0001c770: 7463 6865 7272 6f72 2920 286a 7573 7420  tcherror) (just 
-0001c780: 6c69 6b65 205b 6465 7374 7275 6374 7572  like [destructur
-0001c790: 696e 6720 6173 7369 676e 6d65 6e74 5d28  ing assignment](
-0001c7a0: 2364 6573 7472 7563 7475 7269 6e67 2d61  #destructuring-a
-0001c7b0: 7373 6967 6e6d 656e 7429 2920 696e 7374  ssignment)) inst
-0001c7c0: 6561 6420 6f66 2061 2060 5479 7065 4572  ead of a `TypeEr
-0001c7d0: 726f 7260 2e0a 2d20 416c 6c20 6465 6661  ror`..- All defa
-0001c7e0: 756c 7473 2069 6e20 7061 7474 6572 6e2d  ults in pattern-
-0001c7f0: 6d61 7463 6869 6e67 2066 756e 6374 696f  matching functio
-0001c800: 6e20 6465 6669 6e69 7469 6f6e 2061 7265  n definition are
-0001c810: 206c 6174 652d 626f 756e 6420 7261 7468   late-bound rath
-0001c820: 6572 2074 6861 6e20 6561 726c 792d 626f  er than early-bo
-0001c830: 756e 642e 2054 6875 732c 2060 6d61 7463  und. Thus, `matc
-0001c840: 6820 6465 6620 6628 7873 3d5b 5d29 203d  h def f(xs=[]) =
-0001c850: 2078 7360 2077 696c 6c20 696e 7374 616e   xs` will instan
-0001c860: 7469 6174 6520 6120 6e65 7720 6c69 7374  tiate a new list
-0001c870: 2066 6f72 2065 6163 6820 6361 6c6c 2077   for each call w
-0001c880: 6865 7265 2060 7873 6020 6973 206e 6f74  here `xs` is not
-0001c890: 2067 6976 656e 2c20 756e 6c69 6b65 2060   given, unlike `
-0001c8a0: 6465 6620 6628 7873 3d5b 5d29 203d 2078  def f(xs=[]) = x
-0001c8b0: 7360 2c20 7768 6963 6820 7769 6c6c 2075  s`, which will u
-0001c8c0: 7365 2074 6865 2073 616d 6520 6c69 7374  se the same list
-0001c8d0: 2066 6f72 2061 6c6c 2063 616c 6c73 2077   for all calls w
-0001c8e0: 6865 7265 2060 7873 6020 6973 2075 6e73  here `xs` is uns
-0001c8f0: 7065 6369 6669 6564 2e0a 0a50 6174 7465  pecified...Patte
-0001c900: 726e 2d6d 6174 6368 696e 6720 6675 6e63  rn-matching func
-0001c910: 7469 6f6e 2064 6566 696e 6974 696f 6e20  tion definition 
-0001c920: 6361 6e20 616c 736f 2062 6520 636f 6d62  can also be comb
-0001c930: 696e 6564 2077 6974 6820 6061 7379 6e63  ined with `async
-0001c940: 6020 6675 6e63 7469 6f6e 732c 205b 6063  ` functions, [`c
-0001c950: 6f70 7963 6c6f 7375 7265 6020 6675 6e63  opyclosure` func
-0001c960: 7469 6f6e 735d 2823 636f 7079 636c 6f73  tions](#copyclos
-0001c970: 7572 652d 6675 6e63 7469 6f6e 7329 2c20  ure-functions), 
-0001c980: 5b60 7969 656c 6460 2066 756e 6374 696f  [`yield` functio
-0001c990: 6e73 5d28 2365 7870 6c69 6369 742d 6765  ns](#explicit-ge
-0001c9a0: 6e65 7261 746f 7273 292c 205b 696e 6669  nerators), [infi
-0001c9b0: 7820 6675 6e63 7469 6f6e 2064 6566 696e  x function defin
-0001c9c0: 6974 696f 6e5d 2823 696e 6669 782d 6675  ition](#infix-fu
-0001c9d0: 6e63 7469 6f6e 7329 2c20 616e 6420 5b61  nctions), and [a
-0001c9e0: 7373 6967 6e6d 656e 7420 6675 6e63 7469  ssignment functi
-0001c9f0: 6f6e 2073 796e 7461 785d 2823 6173 7369  on syntax](#assi
-0001ca00: 676e 6d65 6e74 2d66 756e 6374 696f 6e73  gnment-functions
-0001ca10: 292e 2054 6865 2076 6172 696f 7573 206b  ). The various k
-0001ca20: 6579 776f 7264 7320 696e 2066 726f 6e74  eywords in front
-0001ca30: 206f 6620 7468 6520 6064 6566 6020 6361   of the `def` ca
-0001ca40: 6e20 6265 2070 7574 2069 6e20 616e 7920  n be put in any 
-0001ca50: 6f72 6465 722e 0a0a 2323 2323 2320 4578  order...##### Ex
-0001ca60: 616d 706c 650a 0a2a 2a43 6f63 6f6e 7574  ample..**Coconut
-0001ca70: 3a2a 2a0a 6060 6063 6f63 6f6e 7574 0a64  :**.```coconut.d
-0001ca80: 6566 206c 6173 745f 7477 6f28 5f20 2b20  ef last_two(_ + 
-0001ca90: 5b61 2c20 625d 293a 0a20 2020 2072 6574  [a, b]):.    ret
-0001caa0: 7572 6e20 612c 2062 0a64 6566 2078 7964  urn a, b.def xyd
-0001cab0: 6963 745f 746f 5f78 7974 7570 6c65 287b  ict_to_xytuple({
-0001cac0: 2278 223a 2078 2060 6973 696e 7374 616e  "x": x `isinstan
-0001cad0: 6365 6020 696e 742c 2022 7922 3a20 7920  ce` int, "y": y 
-0001cae0: 6069 7369 6e73 7461 6e63 6560 2069 6e74  `isinstance` int
-0001caf0: 7d29 3a0a 2020 2020 7265 7475 726e 2078  }):.    return x
-0001cb00: 2c20 790a 0a72 616e 6765 2835 2920 7c3e  , y..range(5) |>
-0001cb10: 206c 6173 745f 7477 6f20 7c3e 2070 7269   last_two |> pri
-0001cb20: 6e74 0a7b 2278 223a 312c 2022 7922 3a32  nt.{"x":1, "y":2
-0001cb30: 7d20 7c3e 2078 7964 6963 745f 746f 5f78  } |> xydict_to_x
-0001cb40: 7974 7570 6c65 207c 3e20 7072 696e 740a  ytuple |> print.
-0001cb50: 6060 600a 0a2a 2a50 7974 686f 6e3a 2a2a  ```..**Python:**
-0001cb60: 0a5f 4361 6e27 7420 6265 2064 6f6e 6520  ._Can't be done 
-0001cb70: 7769 7468 6f75 7420 6120 6c6f 6e67 2073  without a long s
-0001cb80: 6572 6965 7320 6f66 2063 6865 636b 7320  eries of checks 
-0001cb90: 6174 2074 6865 2074 6f70 206f 6620 7468  at the top of th
-0001cba0: 6520 6675 6e63 7469 6f6e 2e20 5365 6520  e function. See 
-0001cbb0: 7468 6520 636f 6d70 696c 6564 2063 6f64  the compiled cod
-0001cbc0: 6520 666f 7220 7468 6520 5079 7468 6f6e  e for the Python
-0001cbd0: 2073 796e 7461 782e 5f0a 0a23 2323 2060   syntax._..### `
-0001cbe0: 6164 6470 6174 7465 726e 6020 4675 6e63  addpattern` Func
-0001cbf0: 7469 6f6e 730a 0a43 6f63 6f6e 7574 2070  tions..Coconut p
-0001cc00: 726f 7669 6465 7320 7468 6520 6061 6464  rovides the `add
-0001cc10: 7061 7474 6572 6e20 6465 6660 2073 796e  pattern def` syn
-0001cc20: 7461 7820 6173 2061 2073 686f 7274 6375  tax as a shortcu
-0001cc30: 7420 666f 7220 7468 6520 6675 6c6c 0a60  t for the full.`
-0001cc40: 6060 636f 636f 6e75 740a 4061 6464 7061  ``coconut.@addpa
-0001cc50: 7474 6572 6e28 6675 6e63 290a 6d61 7463  ttern(func).matc
-0001cc60: 6820 6465 6620 6675 6e63 282e 2e2e 293a  h def func(...):
-0001cc70: 0a20 202e 2e2e 0a60 6060 0a73 796e 7461  .  ....```.synta
-0001cc80: 7820 7573 696e 6720 7468 6520 5b60 6164  x using the [`ad
-0001cc90: 6470 6174 7465 726e 605d 2823 6164 6470  dpattern`](#addp
-0001cca0: 6174 7465 726e 2920 6465 636f 7261 746f  attern) decorato
-0001ccb0: 722e 0a0a 4164 6469 7469 6f6e 616c 6c79  r...Additionally
-0001ccc0: 2c20 6061 6464 7061 7474 6572 6e20 6465  , `addpattern de
-0001ccd0: 6660 2077 696c 6c20 6163 7420 6a75 7374  f` will act just
-0001cce0: 206c 696b 6520 6120 6e6f 726d 616c 205b   like a normal [
-0001ccf0: 606d 6174 6368 2064 6566 605d 2823 7061  `match def`](#pa
-0001cd00: 7474 6572 6e2d 6d61 7463 6869 6e67 2d66  ttern-matching-f
-0001cd10: 756e 6374 696f 6e73 2920 6966 2074 6865  unctions) if the
-0001cd20: 2066 756e 6374 696f 6e20 6861 7320 6e6f   function has no
-0001cd30: 7420 7072 6576 696f 7573 6c79 2062 6565  t previously bee
-0001cd40: 6e20 6465 6669 6e65 642c 2061 6c6c 6f77  n defined, allow
-0001cd50: 696e 6720 666f 7220 6061 6464 7061 7474  ing for `addpatt
-0001cd60: 6572 6e20 6465 6660 2074 6f20 6265 2075  ern def` to be u
-0001cd70: 7365 6420 666f 7220 6561 6368 2063 6173  sed for each cas
-0001cd80: 6520 7261 7468 6572 2074 6861 6e20 7265  e rather than re
-0001cd90: 7175 6972 696e 6720 606d 6174 6368 2064  quiring `match d
-0001cda0: 6566 6020 666f 7220 7468 6520 6669 7273  ef` for the firs
-0001cdb0: 7420 6361 7365 2061 6e64 2060 6164 6470  t case and `addp
-0001cdc0: 6174 7465 726e 2064 6566 6020 666f 7220  attern def` for 
-0001cdd0: 6675 7475 7265 2063 6173 6573 2e0a 0a49  future cases...I
-0001cde0: 6620 796f 7520 7761 6e74 2074 6f20 7075  f you want to pu
-0001cdf0: 7420 6120 6465 636f 7261 746f 7220 6f6e  t a decorator on
-0001ce00: 2061 6e20 6061 6464 7061 7474 6572 6e20   an `addpattern 
-0001ce10: 6465 6660 2066 756e 6374 696f 6e2c 206d  def` function, m
-0001ce20: 616b 6520 7375 7265 2074 6f20 7075 7420  ake sure to put 
-0001ce30: 6974 206f 6e20 7468 6520 5f6c 6173 745f  it on the _last_
-0001ce40: 2070 6174 7465 726e 2066 756e 6374 696f   pattern functio
-0001ce50: 6e2e 0a0a 2323 2323 2320 4578 616d 706c  n...##### Exampl
-0001ce60: 650a 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a  e..**Coconut:**.
-0001ce70: 6060 6063 6f63 6f6e 7574 0a61 6464 7061  ```coconut.addpa
-0001ce80: 7474 6572 6e20 6465 6620 6661 6374 6f72  ttern def factor
-0001ce90: 6961 6c28 3029 203d 2031 0a61 6464 7061  ial(0) = 1.addpa
-0001cea0: 7474 6572 6e20 6465 6620 6661 6374 6f72  ttern def factor
-0001ceb0: 6961 6c28 6e29 203d 206e 202a 2066 6163  ial(n) = n * fac
-0001cec0: 746f 7269 616c 286e 202d 2031 290a 6060  torial(n - 1).``
-0001ced0: 600a 0a2a 2a50 7974 686f 6e3a 2a2a 0a5f  `..**Python:**._
-0001cee0: 4361 6e27 7420 6265 2064 6f6e 6520 7769  Can't be done wi
-0001cef0: 7468 6f75 7420 6120 636f 6d70 6c69 6361  thout a complica
-0001cf00: 7465 6420 6465 636f 7261 746f 7220 6465  ted decorator de
-0001cf10: 6669 6e69 7469 6f6e 2061 6e64 2061 206c  finition and a l
-0001cf20: 6f6e 6720 7365 7269 6573 206f 6620 6368  ong series of ch
-0001cf30: 6563 6b73 2066 6f72 2065 6163 6820 7061  ecks for each pa
-0001cf40: 7474 6572 6e2d 6d61 7463 6869 6e67 2e20  ttern-matching. 
-0001cf50: 5365 6520 7468 6520 636f 6d70 696c 6564  See the compiled
-0001cf60: 2063 6f64 6520 666f 7220 7468 6520 5079   code for the Py
-0001cf70: 7468 6f6e 2073 796e 7461 782e 5f0a 0a23  thon syntax._..#
-0001cf80: 2323 2060 636f 7079 636c 6f73 7572 6560  ## `copyclosure`
-0001cf90: 2046 756e 6374 696f 6e73 0a0a 436f 636f   Functions..Coco
-0001cfa0: 6e75 7420 7375 7070 6f72 7473 2074 6865  nut supports the
-0001cfb0: 2073 796e 7461 780a 6060 600a 636f 7079   syntax.```.copy
-0001cfc0: 636c 6f73 7572 6520 6465 6620 3c6e 616d  closure def <nam
-0001cfd0: 653e 283c 6172 6773 3e29 3a0a 2020 2020  e>(<args>):.    
-0001cfe0: 3c62 6f64 793e 0a60 6060 0a74 6f20 6465  <body>.```.to de
-0001cff0: 6669 6e65 2061 2066 756e 6374 696f 6e20  fine a function 
-0001d000: 7468 6174 2075 7365 7320 6173 2069 7473  that uses as its
-0001d010: 2063 6c6f 7375 7265 2061 2073 6861 6c6c   closure a shall
-0001d020: 6f77 2063 6f70 7920 6f66 2069 7473 2065  ow copy of its e
-0001d030: 6e63 6c6f 7369 6e67 2073 636f 7065 7320  nclosing scopes 
-0001d040: 6174 2074 6865 2074 696d 6520 7468 6174  at the time that
-0001d050: 2074 6865 2066 756e 6374 696f 6e20 6973   the function is
-0001d060: 2064 6566 696e 6564 2c20 7261 7468 6572   defined, rather
-0001d070: 2074 6861 6e20 6120 7265 6665 7265 6e63   than a referenc
-0001d080: 6520 746f 2074 686f 7365 2073 636f 7065  e to those scope
-0001d090: 7320 2861 7320 7769 7468 206e 6f72 6d61  s (as with norma
-0001d0a0: 6c20 5079 7468 6f6e 2066 756e 6374 696f  l Python functio
-0001d0b0: 6e73 292e 0a0a 466f 7220 6578 616d 706c  ns)...For exampl
-0001d0c0: 652c 6069 6e0a 6060 6063 6f63 6f6e 7574  e,`in.```coconut
-0001d0d0: 0a64 6566 206f 7574 6572 5f66 756e 6328  .def outer_func(
-0001d0e0: 293a 0a20 2020 2066 756e 6373 203d 205b  ):.    funcs = [
-0001d0f0: 5d0a 2020 2020 666f 7220 7820 696e 2072  ].    for x in r
-0001d100: 616e 6765 2831 3029 3a0a 2020 2020 2020  ange(10):.      
-0001d110: 2020 636f 7079 636c 6f73 7572 6520 6465    copyclosure de
-0001d120: 6620 696e 6e65 725f 6675 6e63 2829 3a0a  f inner_func():.
-0001d130: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001d140: 726e 2078 0a20 2020 2020 2020 2066 756e  rn x.        fun
-0001d150: 6373 2e61 7070 656e 6428 696e 6e65 725f  cs.append(inner_
-0001d160: 6675 6e63 290a 2020 2020 7265 7475 726e  func).    return
-0001d170: 2066 756e 6373 0a60 6060 0a74 6865 2072   funcs.```.the r
-0001d180: 6573 756c 7469 6e67 2060 696e 6e65 725f  esulting `inner_
-0001d190: 6675 6e63 6073 2077 696c 6c20 6561 6368  func`s will each
-0001d1a0: 2072 6574 7572 6e20 6120 5f64 6966 6665   return a _diffe
-0001d1b0: 7265 6e74 5f20 6078 6020 7661 6c75 6520  rent_ `x` value 
-0001d1c0: 7261 7468 6572 2074 6861 6e20 616c 6c20  rather than all 
-0001d1d0: 7468 6520 7361 6d65 2060 7860 2076 616c  the same `x` val
-0001d1e0: 7565 2c20 7369 6e63 6520 7468 6579 206c  ue, since they l
-0001d1f0: 6f6f 6b20 6174 2077 6861 7420 6078 6020  ook at what `x` 
-0001d200: 7761 7320 626f 756e 6420 746f 2061 7420  was bound to at 
-0001d210: 6675 6e63 7469 6f6e 2064 6566 696e 6974  function definit
-0001d220: 696f 6e20 7469 6d65 2072 6174 6865 7220  ion time rather 
-0001d230: 7468 616e 2064 7572 696e 6720 6675 6e63  than during func
-0001d240: 7469 6f6e 2065 7865 6375 7469 6f6e 2e0a  tion execution..
-0001d250: 0a60 636f 7079 636c 6f73 7572 6560 2066  .`copyclosure` f
-0001d260: 756e 6374 696f 6e73 2063 616e 2061 6c73  unctions can als
-0001d270: 6f20 6265 2063 6f6d 6269 6e65 6420 7769  o be combined wi
-0001d280: 7468 2060 6173 796e 6360 2066 756e 6374  th `async` funct
-0001d290: 696f 6e73 2c20 5b60 7969 656c 6460 2066  ions, [`yield` f
-0001d2a0: 756e 6374 696f 6e73 5d28 2365 7870 6c69  unctions](#expli
-0001d2b0: 6369 742d 6765 6e65 7261 746f 7273 292c  cit-generators),
-0001d2c0: 205b 7061 7474 6572 6e2d 6d61 7463 6869   [pattern-matchi
-0001d2d0: 6e67 2066 756e 6374 696f 6e73 5d28 2370  ng functions](#p
-0001d2e0: 6174 7465 726e 2d6d 6174 6368 696e 672d  attern-matching-
-0001d2f0: 6675 6e63 7469 6f6e 7329 2c20 5b69 6e66  functions), [inf
-0001d300: 6978 2066 756e 6374 696f 6e20 6465 6669  ix function defi
-0001d310: 6e69 7469 6f6e 5d28 2369 6e66 6978 2d66  nition](#infix-f
-0001d320: 756e 6374 696f 6e73 292c 2061 6e64 205b  unctions), and [
-0001d330: 6173 7369 676e 6d65 6e74 2066 756e 6374  assignment funct
-0001d340: 696f 6e20 7379 6e74 6178 5d28 2361 7373  ion syntax](#ass
-0001d350: 6967 6e6d 656e 742d 6675 6e63 7469 6f6e  ignment-function
-0001d360: 7329 2e20 5468 6520 7661 7269 6f75 7320  s). The various 
-0001d370: 6b65 7977 6f72 6473 2069 6e20 6672 6f6e  keywords in fron
-0001d380: 7420 6f66 2074 6865 2060 6465 6660 2063  t of the `def` c
-0001d390: 616e 2062 6520 7075 7420 696e 2061 6e79  an be put in any
-0001d3a0: 206f 7264 6572 2e0a 0a49 6620 6067 6c6f   order...If `glo
-0001d3b0: 6261 6c60 206f 7220 606e 6f6e 6c6f 6361  bal` or `nonloca
-0001d3c0: 6c60 2061 7265 2075 7365 6420 696e 2061  l` are used in a
-0001d3d0: 2060 636f 7079 636c 6f73 7572 6560 2066   `copyclosure` f
-0001d3e0: 756e 6374 696f 6e2c 2074 6865 7920 7769  unction, they wi
-0001d3f0: 6c6c 206e 6f74 2062 6520 6162 6c65 2074  ll not be able t
-0001d400: 6f20 6d6f 6469 6679 2076 6172 6961 626c  o modify variabl
-0001d410: 6573 2069 6e20 656e 636c 6f73 696e 6720  es in enclosing 
-0001d420: 7363 6f70 6573 2e20 486f 7765 7665 722c  scopes. However,
-0001d430: 2074 6865 7920 7769 6c6c 2061 6c6c 6f77   they will allow
-0001d440: 2073 7461 7465 2074 6f20 6265 2070 7265   state to be pre
-0001d450: 7365 7276 6564 2061 6363 726f 7373 206d  served accross m
-0001d460: 756c 7469 706c 6520 6361 6c6c 7320 746f  ultiple calls to
-0001d470: 2074 6865 2060 636f 7079 636c 6f73 7572   the `copyclosur
-0001d480: 6560 2066 756e 6374 696f 6e2e 0a0a 2323  e` function...##
-0001d490: 2323 2320 4578 616d 706c 650a 0a2a 2a43  ### Example..**C
-0001d4a0: 6f63 6f6e 7574 3a2a 2a0a 6060 6063 6f63  oconut:**.```coc
-0001d4b0: 6f6e 7574 0a64 6566 206f 7574 6572 5f66  onut.def outer_f
-0001d4c0: 756e 6328 293a 0a20 2020 2066 756e 6373  unc():.    funcs
-0001d4d0: 203d 205b 5d0a 2020 2020 666f 7220 7820   = [].    for x 
-0001d4e0: 696e 2072 616e 6765 2831 3029 3a0a 2020  in range(10):.  
-0001d4f0: 2020 2020 2020 636f 7079 636c 6f73 7572        copyclosur
-0001d500: 6520 6465 6620 696e 6e65 725f 6675 6e63  e def inner_func
-0001d510: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0001d520: 7265 7475 726e 2078 0a20 2020 2020 2020  return x.       
-0001d530: 2066 756e 6373 2e61 7070 656e 6428 696e   funcs.append(in
-0001d540: 6e65 725f 6675 6e63 290a 2020 2020 7265  ner_func).    re
-0001d550: 7475 726e 2066 756e 6373 0a60 6060 0a0a  turn funcs.```..
-0001d560: 2a2a 5079 7468 6f6e 3a2a 2a0a 6060 6063  **Python:**.```c
-0001d570: 6f63 6f6e 7574 5f70 7974 686f 6e0a 6672  oconut_python.fr
-0001d580: 6f6d 2066 756e 6374 6f6f 6c73 2069 6d70  om functools imp
-0001d590: 6f72 7420 7061 7274 6961 6c0a 0a64 6566  ort partial..def
-0001d5a0: 206f 7574 6572 5f66 756e 6328 293a 0a20   outer_func():. 
-0001d5b0: 2020 2066 756e 6373 203d 205b 5d0a 2020     funcs = [].  
-0001d5c0: 2020 666f 7220 7820 696e 2072 616e 6765    for x in range
-0001d5d0: 2831 3029 3a0a 2020 2020 2020 2020 6465  (10):.        de
-0001d5e0: 6620 696e 6e65 725f 6675 6e63 285f 7829  f inner_func(_x)
-0001d5f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0001d600: 7475 726e 205f 780a 2020 2020 2020 2020  turn _x.        
-0001d610: 6675 6e63 732e 6170 7065 6e64 2870 6172  funcs.append(par
-0001d620: 7469 616c 2869 6e6e 6572 5f66 756e 632c  tial(inner_func,
-0001d630: 2078 2929 0a20 2020 2072 6574 7572 6e20   x)).    return 
-0001d640: 6675 6e63 730a 6060 600a 0a23 2323 2045  funcs.```..### E
-0001d650: 7870 6c69 6369 7420 4765 6e65 7261 746f  xplicit Generato
-0001d660: 7273 0a0a 436f 636f 6e75 7420 7375 7070  rs..Coconut supp
-0001d670: 6f72 7473 2074 6865 2073 796e 7461 780a  orts the syntax.
-0001d680: 6060 600a 7969 656c 6420 6465 6620 3c6e  ```.yield def <n
-0001d690: 616d 653e 283c 6172 6773 3e29 3a0a 2020  ame>(<args>):.  
-0001d6a0: 2020 3c62 6f64 793e 0a60 6060 0a74 6f20    <body>.```.to 
-0001d6b0: 6465 6e6f 7465 2074 6861 7420 796f 7520  denote that you 
-0001d6c0: 6172 6520 6578 706c 6963 6974 6c79 2064  are explicitly d
-0001d6d0: 6566 696e 696e 6720 6120 6765 6e65 7261  efining a genera
-0001d6e0: 746f 7220 6675 6e63 7469 6f6e 2e20 5468  tor function. Th
-0001d6f0: 6973 2069 7320 7573 6566 756c 2074 6f20  is is useful to 
-0001d700: 656e 7375 7265 2074 6861 742c 2065 7665  ensure that, eve
-0001d710: 6e20 6966 2061 6c6c 2074 6865 2060 7969  n if all the `yi
-0001d720: 656c 6460 7320 696e 2079 6f75 7220 6675  eld`s in your fu
-0001d730: 6e63 7469 6f6e 2061 7265 2072 656d 6f76  nction are remov
-0001d740: 6564 2c20 6974 276c 6c20 616c 7761 7973  ed, it'll always
-0001d750: 2062 6520 6120 6765 6e65 7261 746f 7220   be a generator 
-0001d760: 6675 6e63 7469 6f6e 2e0a 0a45 7870 6c69  function...Expli
-0001d770: 6369 7420 6765 6e65 7261 746f 7220 6675  cit generator fu
-0001d780: 6e63 7469 6f6e 7320 6361 6e20 616c 736f  nctions can also
-0001d790: 2062 6520 636f 6d62 696e 6564 2077 6974   be combined wit
-0001d7a0: 6820 6061 7379 6e63 6020 6675 6e63 7469  h `async` functi
-0001d7b0: 6f6e 732c 205b 6063 6f70 7963 6c6f 7375  ons, [`copyclosu
-0001d7c0: 7265 6020 6675 6e63 7469 6f6e 735d 2823  re` functions](#
-0001d7d0: 636f 7079 636c 6f73 7572 652d 6675 6e63  copyclosure-func
-0001d7e0: 7469 6f6e 7329 2c20 5b70 6174 7465 726e  tions), [pattern
-0001d7f0: 2d6d 6174 6368 696e 6720 6675 6e63 7469  -matching functi
-0001d800: 6f6e 735d 2823 7061 7474 6572 6e2d 6d61  ons](#pattern-ma
-0001d810: 7463 6869 6e67 2d66 756e 6374 696f 6e73  tching-functions
-0001d820: 292c 205b 696e 6669 7820 6675 6e63 7469  ), [infix functi
-0001d830: 6f6e 2064 6566 696e 6974 696f 6e5d 2823  on definition](#
-0001d840: 696e 6669 782d 6675 6e63 7469 6f6e 7329  infix-functions)
-0001d850: 2c20 616e 6420 5b61 7373 6967 6e6d 656e  , and [assignmen
-0001d860: 7420 6675 6e63 7469 6f6e 2073 796e 7461  t function synta
-0001d870: 785d 2823 6173 7369 676e 6d65 6e74 2d66  x](#assignment-f
-0001d880: 756e 6374 696f 6e73 2920 2874 686f 7567  unctions) (thoug
-0001d890: 6820 6e6f 7465 2074 6861 7420 6173 7369  h note that assi
-0001d8a0: 676e 6d65 6e74 2066 756e 6374 696f 6e20  gnment function 
-0001d8b0: 7379 6e74 6178 2068 6572 6520 6372 6561  syntax here crea
-0001d8c0: 7465 7320 6120 6765 6e65 7261 746f 7220  tes a generator 
-0001d8d0: 7265 7475 726e 292e 2054 6865 2076 6172  return). The var
-0001d8e0: 696f 7573 206b 6579 776f 7264 7320 696e  ious keywords in
-0001d8f0: 2066 726f 6e74 206f 6620 7468 6520 6064   front of the `d
-0001d900: 6566 6020 6361 6e20 6265 2070 7574 2069  ef` can be put i
-0001d910: 6e20 616e 7920 6f72 6465 722e 0a0a 2323  n any order...##
-0001d920: 2323 2320 4578 616d 706c 650a 0a2a 2a43  ### Example..**C
-0001d930: 6f63 6f6e 7574 3a2a 2a0a 6060 6063 6f63  oconut:**.```coc
-0001d940: 6f6e 7574 0a79 6965 6c64 2064 6566 2065  onut.yield def e
-0001d950: 6d70 7479 5f69 7428 293a 2070 6173 730a  mpty_it(): pass.
-0001d960: 6060 600a 0a2a 2a50 7974 686f 6e3a 2a2a  ```..**Python:**
-0001d970: 0a60 6060 636f 636f 6e75 745f 7079 7468  .```coconut_pyth
-0001d980: 6f6e 0a64 6566 2065 6d70 7479 5f69 7428  on.def empty_it(
-0001d990: 293a 0a20 2020 2069 6620 4661 6c73 653a  ):.    if False:
-0001d9a0: 0a20 2020 2020 2020 2079 6965 6c64 0a60  .        yield.`
-0001d9b0: 6060 0a0a 2323 2320 446f 7474 6564 2046  ``..### Dotted F
-0001d9c0: 756e 6374 696f 6e20 4465 6669 6e69 7469  unction Definiti
-0001d9d0: 6f6e 0a0a 436f 636f 6e75 7420 616c 6c6f  on..Coconut allo
-0001d9e0: 7773 2066 6f72 2066 756e 6374 696f 6e20  ws for function 
-0001d9f0: 6465 6669 6e69 7469 6f6e 2075 7369 6e67  definition using
-0001da00: 2061 2064 6f74 7465 6420 6e61 6d65 2074   a dotted name t
-0001da10: 6f20 6173 7369 676e 2061 2066 756e 6374  o assign a funct
-0001da20: 696f 6e20 6173 2061 206d 6574 686f 6420  ion as a method 
-0001da30: 6f66 2061 6e20 6f62 6a65 6374 2061 7320  of an object as 
-0001da40: 7370 6563 6966 6965 6420 696e 205b 5045  specified in [PE
-0001da50: 5020 3534 325d 2868 7474 7073 3a2f 2f77  P 542](https://w
-0001da60: 7777 2e70 7974 686f 6e2e 6f72 672f 6465  ww.python.org/de
-0001da70: 762f 7065 7073 2f70 6570 2d30 3534 322f  v/peps/pep-0542/
-0001da80: 292e 2044 6f74 7465 6420 6675 6e63 7469  ). Dotted functi
-0001da90: 6f6e 2064 6566 696e 6974 696f 6e20 6361  on definition ca
-0001daa0: 6e20 6265 2063 6f6d 6269 6e65 6420 7769  n be combined wi
-0001dab0: 7468 2061 6c6c 206f 7468 6572 2074 7970  th all other typ
-0001dac0: 6573 206f 6620 6675 6e63 7469 6f6e 2064  es of function d
-0001dad0: 6566 696e 6974 696f 6e20 6162 6f76 652e  efinition above.
-0001dae0: 0a0a 2323 2323 2320 4578 616d 706c 650a  ..##### Example.
-0001daf0: 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a 6060  .**Coconut:**.``
-0001db00: 6063 6f63 6f6e 7574 0a64 6566 204d 7943  `coconut.def MyC
-0001db10: 6c61 7373 2e6d 795f 6d65 7468 6f64 2873  lass.my_method(s
-0001db20: 656c 6629 3a0a 2020 2020 2e2e 2e0a 6060  elf):.    ....``
-0001db30: 600a 0a2a 2a50 7974 686f 6e3a 2a2a 0a60  `..**Python:**.`
-0001db40: 6060 636f 636f 6e75 745f 7079 7468 6f6e  ``coconut_python
-0001db50: 0a64 6566 206d 795f 6d65 7468 6f64 2873  .def my_method(s
-0001db60: 656c 6629 3a0a 2020 2020 2e2e 2e0a 4d79  elf):.    ....My
-0001db70: 436c 6173 732e 6d79 5f6d 6574 686f 6420  Class.my_method 
-0001db80: 3d20 6d79 5f6d 6574 686f 640a 6060 600a  = my_method.```.
-0001db90: 0a23 2320 5374 6174 656d 656e 7473 0a0a  .## Statements..
-0001dba0: 6060 607b 636f 6e74 656e 7473 7d0a 2d2d  ```{contents}.--
-0001dbb0: 2d0a 6c6f 6361 6c3a 0a64 6570 7468 3a20  -.local:.depth: 
-0001dbc0: 310a 2d2d 2d0a 6060 600a 0a23 2323 2044  1.---.```..### D
-0001dbd0: 6573 7472 7563 7475 7269 6e67 2041 7373  estructuring Ass
-0001dbe0: 6967 6e6d 656e 740a 0a43 6f63 6f6e 7574  ignment..Coconut
-0001dbf0: 2073 7570 706f 7274 7320 7369 676e 6966   supports signif
-0001dc00: 6963 616e 746c 7920 656e 6861 6e63 6564  icantly enhanced
-0001dc10: 2064 6573 7472 7563 7475 7269 6e67 2061   destructuring a
-0001dc20: 7373 6967 6e6d 656e 742c 2073 696d 696c  ssignment, simil
-0001dc30: 6172 2074 6f20 5079 7468 6f6e 2773 2074  ar to Python's t
-0001dc40: 7570 6c65 2f6c 6973 7420 6465 7374 7275  uple/list destru
-0001dc50: 6374 7572 696e 672c 2062 7574 206d 7563  cturing, but muc
-0001dc60: 6820 6d6f 7265 2070 6f77 6572 6675 6c2e  h more powerful.
-0001dc70: 2054 6865 2073 796e 7461 7820 666f 7220   The syntax for 
-0001dc80: 436f 636f 6e75 7427 7320 6465 7374 7275  Coconut's destru
-0001dc90: 6374 7572 696e 6720 6173 7369 676e 6d65  cturing assignme
-0001dca0: 6e74 2069 730a 6060 6063 6f63 6f6e 7574  nt is.```coconut
-0001dcb0: 0a5b 6d61 7463 685d 203c 7061 7474 6572  .[match] <patter
-0001dcc0: 6e3e 203d 203c 7661 6c75 653e 0a60 6060  n> = <value>.```
-0001dcd0: 0a77 6865 7265 2060 3c76 616c 7565 3e60  .where `<value>`
-0001dce0: 2069 7320 616e 7920 6578 7072 6573 7369   is any expressi
-0001dcf0: 6f6e 2061 6e64 2060 3c70 6174 7465 726e  on and `<pattern
-0001dd00: 3e60 2069 7320 6465 6669 6e65 6420 6279  >` is defined by
-0001dd10: 2043 6f63 6f6e 7574 2773 205b 606d 6174   Coconut's [`mat
-0001dd20: 6368 6020 7374 6174 656d 656e 745d 2823  ch` statement](#
-0001dd30: 6d61 7463 6829 2e20 5468 6520 606d 6174  match). The `mat
-0001dd40: 6368 6020 6b65 7977 6f72 6420 6174 2074  ch` keyword at t
-0001dd50: 6865 2062 6567 696e 6e69 6e67 2069 7320  he beginning is 
-0001dd60: 6f70 7469 6f6e 616c 2c20 6275 7420 6973  optional, but is
-0001dd70: 2073 6f6d 6574 696d 6573 206e 6563 6573   sometimes neces
-0001dd80: 7361 7279 2074 6f20 6469 7361 6d62 6967  sary to disambig
-0001dd90: 7561 7465 2064 6573 7472 7563 7475 7269  uate destructuri
-0001dda0: 6e67 2061 7373 6967 6e6d 656e 7420 6672  ng assignment fr
-0001ddb0: 6f6d 206e 6f72 6d61 6c20 6173 7369 676e  om normal assign
-0001ddc0: 6d65 6e74 2c20 7768 6963 6820 7769 6c6c  ment, which will
-0001ddd0: 2061 6c77 6179 7320 7461 6b65 2070 7265   always take pre
-0001dde0: 6365 6465 6e63 652e 2043 6f63 6f6e 7574  cedence. Coconut
-0001ddf0: 2773 2064 6573 7472 7563 7475 7269 6e67  's destructuring
-0001de00: 2061 7373 6967 6e6d 656e 7420 6973 2065   assignment is e
-0001de10: 7175 6976 616c 656e 7420 746f 2061 206d  quivalent to a m
-0001de20: 6174 6368 2073 7461 7465 6d65 6e74 2074  atch statement t
-0001de30: 6861 7420 666f 6c6c 6f77 7320 7468 6520  hat follows the 
-0001de40: 7379 6e74 6178 3a0a 6060 6063 6f63 6f6e  syntax:.```cocon
-0001de50: 7574 0a6d 6174 6368 203c 7061 7474 6572  ut.match <patter
-0001de60: 6e3e 2069 6e20 3c76 616c 7565 3e3a 0a20  n> in <value>:. 
-0001de70: 2020 2070 6173 730a 656c 7365 3a0a 2020     pass.else:.  
-0001de80: 2020 6572 7220 3d20 4d61 7463 6845 7272    err = MatchErr
-0001de90: 6f72 283c 6572 726f 7220 6d65 7373 6167  or(<error messag
-0001dea0: 653e 290a 2020 2020 6572 722e 7061 7474  e>).    err.patt
-0001deb0: 6572 6e20 3d20 223c 7061 7474 6572 6e3e  ern = "<pattern>
-0001dec0: 220a 2020 2020 6572 722e 7661 6c75 6520  ".    err.value 
-0001ded0: 3d20 3c76 616c 7565 3e0a 2020 2020 7261  = <value>.    ra
-0001dee0: 6973 6520 6572 720a 6060 600a 4966 2061  ise err.```.If a
-0001def0: 2064 6573 7472 7563 7475 7269 6e67 2061   destructuring a
-0001df00: 7373 6967 6e6d 656e 7420 7374 6174 656d  ssignment statem
-0001df10: 656e 7420 6661 696c 732c 2074 6865 6e20  ent fails, then 
-0001df20: 696e 7374 6561 6420 6f66 2063 6f6e 7469  instead of conti
-0001df30: 6e75 696e 6720 6f6e 2061 7320 6966 2061  nuing on as if a
-0001df40: 2060 6d61 7463 6860 2062 6c6f 636b 2068   `match` block h
-0001df50: 6164 2066 6169 6c65 642c 2061 205b 604d  ad failed, a [`M
-0001df60: 6174 6368 4572 726f 7260 5d28 236d 6174  atchError`](#mat
-0001df70: 6368 6572 726f 7229 206f 626a 6563 7420  cherror) object 
-0001df80: 7769 6c6c 2062 6520 7261 6973 6564 2064  will be raised d
-0001df90: 6573 6372 6962 696e 6720 7468 6520 6661  escribing the fa
-0001dfa0: 696c 7572 652e 0a0a 2323 2323 2320 4578  ilure...##### Ex
-0001dfb0: 616d 706c 650a 0a2a 2a43 6f63 6f6e 7574  ample..**Coconut
-0001dfc0: 3a2a 2a0a 6060 6063 6f63 6f6e 7574 0a5f  :**.```coconut._
-0001dfd0: 202b 205b 612c 2062 5d20 3d20 5b30 2c20   + [a, b] = [0, 
-0001dfe0: 312c 2032 2c20 335d 0a70 7269 6e74 2861  1, 2, 3].print(a
-0001dff0: 2c20 6229 0a60 6060 0a0a 2a2a 5079 7468  , b).```..**Pyth
-0001e000: 6f6e 3a2a 2a0a 5f43 616e 2774 2062 6520  on:**._Can't be 
-0001e010: 646f 6e65 2077 6974 686f 7574 2061 206c  done without a l
-0001e020: 6f6e 6720 7365 7269 6573 206f 6620 6368  ong series of ch
-0001e030: 6563 6b73 2069 6e20 706c 6163 6520 6f66  ecks in place of
-0001e040: 2074 6865 2064 6573 7472 7563 7475 7269   the destructuri
-0001e050: 6e67 2061 7373 6967 6e6d 656e 7420 7374  ng assignment st
-0001e060: 6174 656d 656e 742e 2053 6565 2074 6865  atement. See the
-0001e070: 2063 6f6d 7069 6c65 6420 636f 6465 2066   compiled code f
-0001e080: 6f72 2074 6865 2050 7974 686f 6e20 7379  or the Python sy
-0001e090: 6e74 6178 2e5f 0a0a 2323 2320 5479 7065  ntax._..### Type
-0001e0a0: 2050 6172 616d 6574 6572 2053 796e 7461   Parameter Synta
-0001e0b0: 780a 0a43 6f63 6f6e 7574 2066 756c 6c79  x..Coconut fully
-0001e0c0: 2073 7570 706f 7274 7320 5b50 7974 686f   supports [Pytho
-0001e0d0: 6e20 332e 3132 2050 4550 2036 3935 5d28  n 3.12 PEP 695](
-0001e0e0: 6874 7470 733a 2f2f 7065 7073 2e70 7974  https://peps.pyt
-0001e0f0: 686f 6e2e 6f72 672f 7065 702d 3036 3935  hon.org/pep-0695
-0001e100: 2f29 2074 7970 6520 7061 7261 6d65 7465  /) type paramete
-0001e110: 7220 7379 6e74 6178 206f 6e20 616c 6c20  r syntax on all 
-0001e120: 5079 7468 6f6e 2076 6572 7369 6f6e 732e  Python versions.
-0001e130: 0a0a 5468 6174 2069 6e63 6c75 6465 7320  ..That includes 
-0001e140: 7479 7065 2070 6172 616d 6574 6572 7320  type parameters 
-0001e150: 666f 7220 636c 6173 7365 732c 205b 6064  for classes, [`d
-0001e160: 6174 6160 2074 7970 6573 5d28 2364 6174  ata` types](#dat
-0001e170: 6129 2c20 616e 6420 5b61 6c6c 2074 7970  a), and [all typ
-0001e180: 6573 206f 6620 6675 6e63 7469 6f6e 2064  es of function d
-0001e190: 6566 696e 6974 696f 6e5d 2823 6675 6e63  efinition](#func
-0001e1a0: 7469 6f6e 2d64 6566 696e 6974 696f 6e29  tion-definition)
-0001e1b0: 2e20 466f 7220 6469 6666 6572 656e 7420  . For different 
-0001e1c0: 7479 7065 7320 6f66 2066 756e 6374 696f  types of functio
-0001e1d0: 6e20 6465 6669 6e69 7469 6f6e 2c20 7468  n definition, th
-0001e1e0: 6520 7479 7065 2070 6172 616d 6574 6572  e type parameter
-0001e1f0: 7320 616c 7761 7973 2063 6f6d 6520 696e  s always come in
-0001e200: 2062 7261 636b 6574 7320 7269 6768 7420   brackets right 
-0001e210: 6166 7465 7220 7468 6520 6675 6e63 7469  after the functi
-0001e220: 6f6e 206e 616d 652e 2043 6f63 6f6e 7574  on name. Coconut
-0001e230: 2773 205b 656e 6861 6e63 6564 2074 7970  's [enhanced typ
-0001e240: 6520 616e 6e6f 7461 7469 6f6e 2073 796e  e annotation syn
-0001e250: 7461 785d 2823 656e 6861 6e63 6564 2d74  tax](#enhanced-t
-0001e260: 7970 652d 616e 6e6f 7461 7469 6f6e 2920  ype-annotation) 
-0001e270: 6973 2073 7570 706f 7274 6564 2066 6f72  is supported for
-0001e280: 2061 6c6c 2074 7970 6520 7061 7261 6d65   all type parame
-0001e290: 7465 7220 626f 756e 6473 2e0a 0a5f 5761  ter bounds..._Wa
-0001e2a0: 726e 696e 673a 2075 6e74 696c 2060 6d79  rning: until `my
-0001e2b0: 7079 6020 6164 6473 2073 7570 706f 7274  py` adds support
-0001e2c0: 2066 6f72 2060 696e 6665 725f 7661 7269   for `infer_vari
-0001e2d0: 616e 6365 3d54 7275 6560 2069 6e20 6054  ance=True` in `T
-0001e2e0: 7970 6556 6172 602c 2060 5479 7065 5661  ypeVar`, `TypeVa
-0001e2f0: 7260 7320 6372 6561 7465 6420 7468 6973  r`s created this
-0001e300: 2077 6179 2077 696c 6c20 616c 7761 7973   way will always
-0001e310: 2062 6520 696e 7661 7269 616e 742e 5f0a   be invariant._.
-0001e320: 0a41 6464 6974 696f 6e61 6c6c 792c 2043  .Additionally, C
-0001e330: 6f63 6f6e 7574 2073 7570 706f 7274 7320  oconut supports 
-0001e340: 7468 6520 616c 7465 726e 6174 6976 6520  the alternative 
-0001e350: 626f 756e 6473 2073 796e 7461 7820 6f66  bounds syntax of
-0001e360: 2060 7479 7065 204e 6577 5479 7065 5b54   `type NewType[T
-0001e370: 203c 3a20 626f 756e 645d 203d 202e 2e2e   <: bound] = ...
-0001e380: 6020 7261 7468 6572 2074 6861 6e20 6074  ` rather than `t
-0001e390: 7970 6520 4e65 7754 7970 655b 543a 2062  ype NewType[T: b
-0001e3a0: 6f75 6e64 5d20 3d20 2e2e 2e60 2c20 746f  ound] = ...`, to
-0001e3b0: 206d 616b 6520 6974 206d 6f72 6520 636c   make it more cl
-0001e3c0: 6561 7220 7468 6174 2069 7420 6973 2061  ear that it is a
-0001e3d0: 6e20 7570 7065 7220 626f 756e 6420 7261  n upper bound ra
-0001e3e0: 7468 6572 2074 6861 6e20 6120 7479 7065  ther than a type
-0001e3f0: 2e20 496e 2060 2d2d 7374 7269 6374 6020  . In `--strict` 
-0001e400: 6d6f 6465 2c20 603c 3a60 2069 7320 7265  mode, `<:` is re
-0001e410: 7175 6972 6564 206f 7665 7220 603a 6020  quired over `:` 
-0001e420: 666f 7220 616c 6c20 7479 7065 2070 6172  for all type par
-0001e430: 616d 6574 6572 2062 6f75 6e64 732e 205f  ameter bounds. _
-0001e440: 4445 5052 4543 4154 4544 3a20 603c 3d60  DEPRECATED: `<=`
-0001e450: 2063 616e 2061 6c73 6f20 6265 2075 7365   can also be use
-0001e460: 6420 6173 2061 6e20 616c 7465 726e 6174  d as an alternat
-0001e470: 6976 6520 746f 2060 3c3a 602e 5f0a 0a4e  ive to `<:`._..N
-0001e480: 6f74 6520 7468 6174 2074 6865 2060 3c3a  ote that the `<:
-0001e490: 6020 7379 6e74 6178 2073 686f 756c 6420  ` syntax should 
-0001e4a0: 6f6e 6c79 2062 6520 7573 6564 2066 6f72  only be used for
-0001e4b0: 205b 7479 7065 2062 6f75 6e64 735d 2868   [type bounds](h
-0001e4c0: 7474 7073 3a2f 2f70 6570 732e 7079 7468  ttps://peps.pyth
-0001e4d0: 6f6e 2e6f 7267 2f70 6570 2d30 3639 352f  on.org/pep-0695/
-0001e4e0: 2375 7070 6572 2d62 6f75 6e64 2d73 7065  #upper-bound-spe
-0001e4f0: 6369 6669 6361 7469 6f6e 292c 206e 6f74  cification), not
-0001e500: 205b 7479 7065 2063 6f6e 7374 7261 696e   [type constrain
-0001e510: 7473 5d28 6874 7470 733a 2f2f 7065 7073  ts](https://peps
-0001e520: 2e70 7974 686f 6e2e 6f72 672f 7065 702d  .python.org/pep-
-0001e530: 3036 3935 2f23 636f 6e73 7472 6169 6e65  0695/#constraine
-0001e540: 642d 7479 7065 2d73 7065 6369 6669 6361  d-type-specifica
-0001e550: 7469 6f6e 29e2 8094 666f 7220 7479 7065  tion)...for type
-0001e560: 2063 6f6e 7374 7261 696e 7473 2c20 436f   constraints, Co
-0001e570: 636f 6e75 7420 7374 796c 6520 7072 6566  conut style pref
-0001e580: 6572 7320 7468 6520 7661 6e69 6c6c 6120  ers the vanilla 
-0001e590: 5079 7468 6f6e 2060 3a60 2073 796e 7461  Python `:` synta
-0001e5a0: 782c 2077 6869 6368 2068 656c 7073 2074  x, which helps t
-0001e5b0: 6f20 6469 7361 6d62 6967 7561 7465 2062  o disambiguate b
-0001e5c0: 6574 7765 656e 2074 6865 2074 776f 2063  etween the two c
-0001e5d0: 6173 6573 2c20 6173 2074 6865 7920 6172  ases, as they ar
-0001e5e0: 6520 6675 6e63 7469 6f6e 616c 6c79 2064  e functionally d
-0001e5f0: 6966 6665 7265 6e74 2062 7574 206f 7468  ifferent but oth
-0001e600: 6572 7769 7365 2068 6172 6420 746f 2074  erwise hard to t
-0001e610: 656c 6c20 6170 6172 7420 6174 2061 2067  ell apart at a g
-0001e620: 6c61 6e63 652e 2054 6869 7320 6973 2065  lance. This is e
-0001e630: 6e66 6f72 6365 6420 696e 2060 2d2d 7374  nforced in `--st
-0001e640: 7269 6374 6020 6d6f 6465 2e0a 0a5f 4e6f  rict` mode..._No
-0001e650: 7465 2074 6861 742c 2062 7920 6465 6661  te that, by defa
-0001e660: 756c 742c 2061 6c6c 2074 7970 6520 6465  ult, all type de
-0001e670: 636c 6172 6174 696f 6e73 2061 7265 2077  clarations are w
-0001e680: 7261 7070 6564 2069 6e20 7374 7269 6e67  rapped in string
-0001e690: 7320 746f 2065 6e61 626c 6520 666f 7277  s to enable forw
-0001e6a0: 6172 6420 7265 6665 7265 6e63 6573 2061  ard references a
-0001e6b0: 6e64 2069 6d70 726f 7665 2072 756e 7469  nd improve runti
-0001e6c0: 6d65 2070 6572 666f 726d 616e 6365 2e20  me performance. 
-0001e6d0: 4966 2079 6f75 2064 6f6e 2774 2077 616e  If you don't wan
-0001e6e0: 7420 7468 6174 e280 9465 2e67 2e20 6265  t that...e.g. be
-0001e6f0: 6361 7573 6520 796f 7520 7761 6e74 2074  cause you want t
-0001e700: 6f20 7573 6520 7479 7065 2061 6e6e 6f74  o use type annot
-0001e710: 6174 696f 6e73 2061 7420 7275 6e74 696d  ations at runtim
-0001e720: 65e2 8094 7369 6d70 6c79 2070 6173 7320  e...simply pass 
-0001e730: 7468 6520 602d 2d6e 6f2d 7772 6170 2d74  the `--no-wrap-t
-0001e740: 7970 6573 6020 666c 6167 2e5f 0a0a 2323  ypes` flag._..##
-0001e750: 2323 2320 5045 5020 3639 3520 446f 6373  ### PEP 695 Docs
-0001e760: 0a0a 4465 6669 6e69 6e67 2061 2067 656e  ..Defining a gen
-0001e770: 6572 6963 2063 6c61 7373 2070 7269 6f72  eric class prior
-0001e780: 2074 6f20 7468 6973 2050 4550 206c 6f6f   to this PEP loo
-0001e790: 6b73 2073 6f6d 6574 6869 6e67 206c 696b  ks something lik
-0001e7a0: 6520 7468 6973 2e0a 0a60 6060 636f 636f  e this...```coco
-0001e7b0: 6e75 745f 7079 7468 6f6e 0a66 726f 6d20  nut_python.from 
-0001e7c0: 7479 7069 6e67 2069 6d70 6f72 7420 4765  typing import Ge
-0001e7d0: 6e65 7269 632c 2054 7970 6556 6172 0a0a  neric, TypeVar..
-0001e7e0: 5f54 5f63 6f20 3d20 5479 7065 5661 7228  _T_co = TypeVar(
-0001e7f0: 225f 545f 636f 222c 2063 6f76 6172 6961  "_T_co", covaria
-0001e800: 6e74 3d54 7275 652c 2062 6f75 6e64 3d73  nt=True, bound=s
-0001e810: 7472 290a 0a63 6c61 7373 2043 6c61 7373  tr)..class Class
-0001e820: 4128 4765 6e65 7269 635b 5f54 5f63 6f5d  A(Generic[_T_co]
-0001e830: 293a 0a20 2020 2064 6566 206d 6574 686f  ):.    def metho
-0001e840: 6431 2873 656c 6629 202d 3e20 5f54 5f63  d1(self) -> _T_c
-0001e850: 6f3a 0a20 2020 2020 2020 202e 2e2e 0a60  o:.        ....`
-0001e860: 6060 0a0a 5769 7468 2074 6865 206e 6577  ``..With the new
-0001e870: 2073 796e 7461 782c 2069 7420 6c6f 6f6b   syntax, it look
-0001e880: 7320 6c69 6b65 2074 6869 732e 0a0a 6060  s like this...``
-0001e890: 6063 6f63 6f6e 7574 0a63 6c61 7373 2043  `coconut.class C
-0001e8a0: 6c61 7373 415b 543a 2073 7472 5d3a 0a20  lassA[T: str]:. 
-0001e8b0: 2020 2064 6566 206d 6574 686f 6431 2873     def method1(s
-0001e8c0: 656c 6629 202d 3e20 543a 0a20 2020 2020  elf) -> T:.     
-0001e8d0: 2020 202e 2e2e 0a60 6060 0a0a 4865 7265     ....```..Here
-0001e8e0: 2069 7320 616e 2065 7861 6d70 6c65 206f   is an example o
-0001e8f0: 6620 6120 6765 6e65 7269 6320 6675 6e63  f a generic func
-0001e900: 7469 6f6e 2074 6f64 6179 2e0a 0a60 6060  tion today...```
-0001e910: 636f 636f 6e75 745f 7079 7468 6f6e 0a66  coconut_python.f
-0001e920: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-0001e930: 7420 5479 7065 5661 720a 0a5f 5420 3d20  t TypeVar.._T = 
-0001e940: 5479 7065 5661 7228 225f 5422 290a 0a64  TypeVar("_T")..d
-0001e950: 6566 2066 756e 6328 613a 205f 542c 2062  ef func(a: _T, b
-0001e960: 3a20 5f54 2920 2d3e 205f 543a 0a20 2020  : _T) -> _T:.   
-0001e970: 202e 2e2e 0a60 6060 0a0a 416e 6420 7468   ....```..And th
-0001e980: 6520 6e65 7720 7379 6e74 6178 2e0a 0a60  e new syntax...`
-0001e990: 6060 636f 636f 6e75 740a 6465 6620 6675  ``coconut.def fu
-0001e9a0: 6e63 5b54 5d28 613a 2054 2c20 623a 2054  nc[T](a: T, b: T
-0001e9b0: 2920 2d3e 2054 3a0a 2020 2020 2e2e 2e0a  ) -> T:.    ....
-0001e9c0: 6060 600a 0a48 6572 6520 6973 2061 6e20  ```..Here is an 
-0001e9d0: 6578 616d 706c 6520 6f66 2061 2067 656e  example of a gen
-0001e9e0: 6572 6963 2074 7970 6520 616c 6961 7320  eric type alias 
-0001e9f0: 746f 6461 792e 0a0a 6060 6063 6f63 6f6e  today...```cocon
-0001ea00: 7574 5f70 7974 686f 6e0a 6672 6f6d 2074  ut_python.from t
-0001ea10: 7970 696e 6720 696d 706f 7274 2054 7970  yping import Typ
-0001ea20: 6541 6c69 6173 0a0a 5f54 203d 2054 7970  eAlias.._T = Typ
-0001ea30: 6556 6172 2822 5f54 2229 0a0a 4c69 7374  eVar("_T")..List
-0001ea40: 4f72 5365 743a 2054 7970 6541 6c69 6173  OrSet: TypeAlias
-0001ea50: 203d 206c 6973 745b 5f54 5d20 7c20 7365   = list[_T] | se
-0001ea60: 745b 5f54 5d0a 6060 600a 0a41 6e64 2077  t[_T].```..And w
-0001ea70: 6974 6820 7468 6520 6e65 7720 7379 6e74  ith the new synt
-0001ea80: 6178 2e0a 0a60 6060 636f 636f 6e75 740a  ax...```coconut.
-0001ea90: 7479 7065 204c 6973 744f 7253 6574 5b54  type ListOrSet[T
-0001eaa0: 5d20 3d20 6c69 7374 5b54 5d20 7c20 7365  ] = list[T] | se
-0001eab0: 745b 545d 0a60 6060 0a0a 0a23 2323 2323  t[T].```...#####
-0001eac0: 2045 7861 6d70 6c65 0a0a 2a2a 436f 636f   Example..**Coco
-0001ead0: 6e75 743a 2a2a 0a60 6060 636f 636f 6e75  nut:**.```coconu
-0001eae0: 740a 6461 7461 2044 5b54 5d28 783a 2054  t.data D[T](x: T
-0001eaf0: 2c20 793a 2054 290a 0a64 6566 206d 795f  , y: T)..def my_
-0001eb00: 6964 656e 745b 545d 2878 3a20 5429 202d  ident[T](x: T) -
-0001eb10: 3e20 5420 3d20 780a 6060 600a 0a2a 2a50  > T = x.```..**P
-0001eb20: 7974 686f 6e3a 2a2a 0a5f 4361 6e27 7420  ython:**._Can't 
-0001eb30: 6265 2064 6f6e 6520 7769 7468 6f75 7420  be done without 
-0001eb40: 6120 636f 6d70 6c65 7820 6465 6669 6e69  a complex defini
-0001eb50: 7469 6f6e 2066 6f72 2074 6865 2064 6174  tion for the dat
-0001eb60: 6120 7479 7065 2e20 5365 6520 7468 6520  a type. See the 
-0001eb70: 636f 6d70 696c 6564 2063 6f64 6520 666f  compiled code fo
-0001eb80: 7220 7468 6520 5079 7468 6f6e 2073 796e  r the Python syn
-0001eb90: 7461 782e 5f0a 0a23 2323 2049 6d70 6c69  tax._..### Impli
-0001eba0: 6369 7420 6070 6173 7360 0a0a 436f 636f  cit `pass`..Coco
-0001ebb0: 6e75 7420 7375 7070 6f72 7473 2074 6865  nut supports the
-0001ebc0: 2073 696d 706c 6520 6063 6c61 7373 206e   simple `class n
-0001ebd0: 616d 6528 6261 7365 2960 2061 6e64 2060  ame(base)` and `
-0001ebe0: 6461 7461 206e 616d 6528 6172 6773 2960  data name(args)`
-0001ebf0: 2061 7320 616c 6961 7365 7320 666f 7220   as aliases for 
-0001ec00: 6063 6c61 7373 206e 616d 6528 6261 7365  `class name(base
-0001ec10: 293a 2070 6173 7360 2061 6e64 2060 6461  ): pass` and `da
-0001ec20: 7461 206e 616d 6528 6172 6773 293a 2070  ta name(args): p
-0001ec30: 6173 7360 2e0a 0a23 2323 2323 2045 7861  ass`...##### Exa
-0001ec40: 6d70 6c65 0a0a 2a2a 436f 636f 6e75 743a  mple..**Coconut:
-0001ec50: 2a2a 0a60 6060 636f 636f 6e75 740a 636c  **.```coconut.cl
-0001ec60: 6173 7320 5472 6565 0a64 6174 6120 456d  ass Tree.data Em
-0001ec70: 7074 7920 6672 6f6d 2054 7265 650a 6461  pty from Tree.da
-0001ec80: 7461 204c 6561 6628 6974 656d 2920 6672  ta Leaf(item) fr
-0001ec90: 6f6d 2054 7265 650a 6461 7461 204e 6f64  om Tree.data Nod
-0001eca0: 6528 6c65 6674 2c20 7269 6768 7429 2066  e(left, right) f
-0001ecb0: 726f 6d20 5472 6565 0a60 6060 0a0a 2a2a  rom Tree.```..**
-0001ecc0: 5079 7468 6f6e 3a2a 2a0a 5f43 616e 2774  Python:**._Can't
-0001ecd0: 2062 6520 646f 6e65 2077 6974 686f 7574   be done without
-0001ece0: 2061 2073 6572 6965 7320 6f66 206d 6574   a series of met
-0001ecf0: 686f 6420 6465 6669 6e69 7469 6f6e 7320  hod definitions 
-0001ed00: 666f 7220 6561 6368 2064 6174 6120 7479  for each data ty
-0001ed10: 7065 2e20 5365 6520 7468 6520 636f 6d70  pe. See the comp
-0001ed20: 696c 6564 2063 6f64 6520 666f 7220 7468  iled code for th
-0001ed30: 6520 5079 7468 6f6e 2073 796e 7461 782e  e Python syntax.
-0001ed40: 5f0a 0a23 2323 2044 6563 6f72 6174 6f72  _..### Decorator
-0001ed50: 730a 0a55 6e6c 696b 6520 5079 7468 6f6e  s..Unlike Python
-0001ed60: 2c20 7768 6963 6820 6f6e 6c79 2073 7570  , which only sup
-0001ed70: 706f 7274 7320 6120 7369 6e67 6c65 2076  ports a single v
-0001ed80: 6172 6961 626c 6520 6f72 2066 756e 6374  ariable or funct
-0001ed90: 696f 6e20 6361 6c6c 2069 6e20 6120 6465  ion call in a de
-0001eda0: 636f 7261 746f 722c 2043 6f63 6f6e 7574  corator, Coconut
-0001edb0: 2073 7570 706f 7274 7320 616e 7920 6578   supports any ex
-0001edc0: 7072 6573 7369 6f6e 2061 7320 696e 205b  pression as in [
-0001edd0: 5045 5020 3631 345d 2868 7474 7073 3a2f  PEP 614](https:/
-0001ede0: 2f77 7777 2e70 7974 686f 6e2e 6f72 672f  /www.python.org/
-0001edf0: 6465 762f 7065 7073 2f70 6570 2d30 3631  dev/peps/pep-061
-0001ee00: 342f 292e 0a0a 2323 2323 2320 4578 616d  4/)...##### Exam
-0001ee10: 706c 650a 0a2a 2a43 6f63 6f6e 7574 3a2a  ple..**Coconut:*
-0001ee20: 2a0a 6060 6063 6f63 6f6e 7574 0a40 2077  *.```coconut.@ w
-0001ee30: 7261 7070 6572 3120 2e2e 2077 7261 7070  rapper1 .. wrapp
-0001ee40: 6572 3224 2861 7267 290a 6465 6620 6675  er2$(arg).def fu
-0001ee50: 6e63 2878 2920 3d20 782a 2a32 0a60 6060  nc(x) = x**2.```
-0001ee60: 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a 6060  ..**Python:**.``
-0001ee70: 6063 6f63 6f6e 7574 5f70 7974 686f 6e0a  `coconut_python.
-0001ee80: 6465 6620 7772 6170 7065 7228 6675 6e63  def wrapper(func
-0001ee90: 293a 0a20 2020 2072 6574 7572 6e20 7772  ):.    return wr
-0001eea0: 6170 7065 7231 2877 7261 7070 6572 3228  apper1(wrapper2(
-0001eeb0: 6172 672c 2066 756e 6329 290a 4077 7261  arg, func)).@wra
-0001eec0: 7070 6572 0a64 6566 2066 756e 6328 7829  pper.def func(x)
-0001eed0: 3a0a 2020 2020 7265 7475 726e 2078 2a2a  :.    return x**
-0001eee0: 320a 6060 600a 0a23 2323 2053 7461 7465  2.```..### State
-0001eef0: 6d65 6e74 204e 6573 7469 6e67 0a0a 436f  ment Nesting..Co
-0001ef00: 636f 6e75 7420 7375 7070 6f72 7473 2074  conut supports t
-0001ef10: 6865 206e 6573 7469 6e67 206f 6620 636f  he nesting of co
-0001ef20: 6d70 6f75 6e64 2073 7461 7465 6d65 6e74  mpound statement
-0001ef30: 7320 6f6e 2074 6865 2073 616d 6520 6c69  s on the same li
-0001ef40: 6e65 2e20 5468 6973 2061 6c6c 6f77 7320  ne. This allows 
-0001ef50: 7468 6520 6d69 7869 6e67 206f 6620 606d  the mixing of `m
-0001ef60: 6174 6368 6020 616e 6420 6069 6660 2073  atch` and `if` s
-0001ef70: 7461 7465 6d65 6e74 7320 746f 6765 7468  tatements togeth
-0001ef80: 6572 2c20 6173 2077 656c 6c20 6173 2063  er, as well as c
-0001ef90: 6f6d 706f 756e 6420 6074 7279 6020 7374  ompound `try` st
-0001efa0: 6174 656d 656e 7473 2e0a 0a23 2323 2323  atements...#####
-0001efb0: 2045 7861 6d70 6c65 0a0a 2a2a 436f 636f   Example..**Coco
-0001efc0: 6e75 743a 2a2a 0a60 6060 636f 636f 6e75  nut:**.```coconu
-0001efd0: 740a 6966 2069 6e76 616c 6964 2869 6e70  t.if invalid(inp
-0001efe0: 7574 5f6c 6973 7429 3a0a 2020 2020 7261  ut_list):.    ra
-0001eff0: 6973 6520 4578 6365 7074 696f 6e28 290a  ise Exception().
-0001f000: 656c 7365 3a20 6d61 7463 6820 5b68 6561  else: match [hea
-0001f010: 645d 202b 2074 6169 6c20 696e 2069 6e70  d] + tail in inp
-0001f020: 7574 5f6c 6973 743a 0a20 2020 2070 7269  ut_list:.    pri
-0001f030: 6e74 2868 6561 642c 2074 6169 6c29 0a65  nt(head, tail).e
-0001f040: 6c73 653a 0a20 2020 2070 7269 6e74 2869  lse:.    print(i
-0001f050: 6e70 7574 5f6c 6973 7429 0a60 6060 0a0a  nput_list).```..
-0001f060: 2a2a 5079 7468 6f6e 3a2a 2a0a 6060 6063  **Python:**.```c
-0001f070: 6f63 6f6e 7574 5f70 7974 686f 6e0a 6672  oconut_python.fr
-0001f080: 6f6d 2063 6f6c 6c65 6374 696f 6e73 2e61  om collections.a
-0001f090: 6263 2069 6d70 6f72 7420 5365 7175 656e  bc import Sequen
-0001f0a0: 6365 0a69 6620 696e 7661 6c69 6428 696e  ce.if invalid(in
-0001f0b0: 7075 745f 6c69 7374 293a 0a20 2020 2072  put_list):.    r
-0001f0c0: 6169 7365 2045 7863 6570 7469 6f6e 2829  aise Exception()
-0001f0d0: 0a65 6c69 6620 6973 696e 7374 616e 6365  .elif isinstance
-0001f0e0: 2869 6e70 7574 5f6c 6973 742c 2053 6571  (input_list, Seq
-0001f0f0: 7565 6e63 6529 2061 6e64 206c 656e 2869  uence) and len(i
-0001f100: 6e70 7574 5f6c 6973 7429 203e 3d20 313a  nput_list) >= 1:
-0001f110: 0a20 2020 2068 6561 642c 2074 6169 6c20  .    head, tail 
-0001f120: 3d20 696e 7075 746c 6973 745b 305d 2c20  = inputlist[0], 
-0001f130: 696e 7075 746c 6973 745b 313a 5d0a 2020  inputlist[1:].  
-0001f140: 2020 7072 696e 7428 6865 6164 2c20 7461    print(head, ta
-0001f150: 696c 290a 656c 7365 3a0a 2020 2020 7072  il).else:.    pr
-0001f160: 696e 7428 696e 7075 745f 6c69 7374 290a  int(input_list).
-0001f170: 6060 600a 0a23 2323 2060 6578 6365 7074  ```..### `except
-0001f180: 6020 5374 6174 656d 656e 7473 0a0a 5079  ` Statements..Py
-0001f190: 7468 6f6e 2033 2072 6571 7569 7265 7320  thon 3 requires 
-0001f1a0: 7468 6174 2069 6620 6d75 6c74 6970 6c65  that if multiple
-0001f1b0: 2065 7863 6570 7469 6f6e 7320 6172 6520   exceptions are 
-0001f1c0: 746f 2062 6520 6361 7567 6874 2c20 7468  to be caught, th
-0001f1d0: 6579 206d 7573 7420 6265 2070 6c61 6365  ey must be place
-0001f1e0: 6420 696e 7369 6465 206f 6620 7061 7265  d inside of pare
-0001f1f0: 6e74 6865 7365 732c 2073 6f20 6173 2074  ntheses, so as t
-0001f200: 6f20 6469 7361 6c6c 6f77 2050 7974 686f  o disallow Pytho
-0001f210: 6e20 3227 7320 7573 6520 6f66 2061 2063  n 2's use of a c
-0001f220: 6f6d 6d61 2069 6e73 7465 6164 206f 6620  omma instead of 
-0001f230: 6061 7360 2e20 436f 636f 6e75 7420 616c  `as`. Coconut al
-0001f240: 6c6f 7773 2063 6f6d 6d61 7320 696e 2065  lows commas in e
-0001f250: 7863 6570 7420 7374 6174 656d 656e 7473  xcept statements
-0001f260: 2074 6f20 7472 616e 736c 6174 6520 746f   to translate to
-0001f270: 2063 6174 6368 696e 6720 6d75 6c74 6970   catching multip
-0001f280: 6c65 2065 7863 6570 7469 6f6e 7320 7769  le exceptions wi
-0001f290: 7468 6f75 7420 7468 6520 6e65 6564 2066  thout the need f
-0001f2a0: 6f72 2070 6172 656e 7468 6573 6573 2c20  or parentheses, 
-0001f2b0: 7369 6e63 652c 2061 7320 696e 2050 7974  since, as in Pyt
-0001f2c0: 686f 6e20 332c 2060 6173 6020 6973 2061  hon 3, `as` is a
-0001f2d0: 6c77 6179 7320 7265 7175 6972 6564 2074  lways required t
-0001f2e0: 6f20 6269 6e64 2074 6865 2065 7863 6570  o bind the excep
-0001f2f0: 7469 6f6e 2074 6f20 6120 6e61 6d65 2e0a  tion to a name..
-0001f300: 0a23 2323 2323 2045 7861 6d70 6c65 0a0a  .##### Example..
-0001f310: 2a2a 436f 636f 6e75 743a 2a2a 0a60 6060  **Coconut:**.```
-0001f320: 636f 636f 6e75 740a 7472 793a 0a20 2020  coconut.try:.   
-0001f330: 2075 6e73 6166 655f 6675 6e63 2861 7267   unsafe_func(arg
-0001f340: 290a 6578 6365 7074 2053 796e 7461 7845  ).except SyntaxE
-0001f350: 7272 6f72 2c20 5661 6c75 6545 7272 6f72  rror, ValueError
-0001f360: 2061 7320 6572 723a 0a20 2020 2068 616e   as err:.    han
-0001f370: 646c 6528 6572 7229 0a60 6060 0a0a 2a2a  dle(err).```..**
-0001f380: 5079 7468 6f6e 3a2a 2a0a 6060 6063 6f63  Python:**.```coc
-0001f390: 6f6e 7574 5f70 7974 686f 6e0a 7472 793a  onut_python.try:
-0001f3a0: 0a20 2020 2075 6e73 6166 655f 6675 6e63  .    unsafe_func
-0001f3b0: 2861 7267 290a 6578 6365 7074 2028 5379  (arg).except (Sy
-0001f3c0: 6e74 6178 4572 726f 722c 2056 616c 7565  ntaxError, Value
-0001f3d0: 4572 726f 7229 2061 7320 6572 723a 0a20  Error) as err:. 
-0001f3e0: 2020 2068 616e 646c 6528 6572 7229 0a60     handle(err).`
-0001f3f0: 6060 0a0a 2323 2320 496e 2d6c 696e 6520  ``..### In-line 
-0001f400: 6067 6c6f 6261 6c60 2041 6e64 2060 6e6f  `global` And `no
-0001f410: 6e6c 6f63 616c 6020 4173 7369 676e 6d65  nlocal` Assignme
-0001f420: 6e74 0a0a 436f 636f 6e75 7420 616c 6c6f  nt..Coconut allo
-0001f430: 7773 2066 6f72 2060 676c 6f62 616c 6020  ws for `global` 
-0001f440: 6f72 2060 6e6f 6e6c 6f63 616c 6020 746f  or `nonlocal` to
-0001f450: 2070 7265 6365 6465 2061 7373 6967 6e6d   precede assignm
-0001f460: 656e 7420 746f 2061 206c 6973 7420 6f66  ent to a list of
-0001f470: 2076 6172 6961 626c 6573 206f 7220 2861   variables or (a
-0001f480: 7567 6d65 6e74 6564 2920 6173 7369 676e  ugmented) assign
-0001f490: 6d65 6e74 2074 6f20 6120 7661 7269 6162  ment to a variab
-0001f4a0: 6c65 2074 6f20 6d61 6b65 2074 6861 7420  le to make that 
-0001f4b0: 6173 7369 676e 6d65 6e74 2060 676c 6f62  assignment `glob
-0001f4c0: 616c 6020 6f72 2060 6e6f 6e6c 6f63 616c  al` or `nonlocal
-0001f4d0: 602c 2072 6573 7065 6374 6976 656c 792e  `, respectively.
-0001f4e0: 0a0a 2323 2323 2320 4578 616d 706c 650a  ..##### Example.
-0001f4f0: 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a 6060  .**Coconut:**.``
-0001f500: 6063 6f63 6f6e 7574 0a67 6c6f 6261 6c20  `coconut.global 
-0001f510: 7374 6174 655f 612c 2073 7461 7465 5f62  state_a, state_b
-0001f520: 203d 2031 302c 2031 3030 0a67 6c6f 6261   = 10, 100.globa
-0001f530: 6c20 7374 6174 655f 6320 2b3d 2031 0a60  l state_c += 1.`
-0001f540: 6060 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a  ``..**Python:**.
-0001f550: 6060 6063 6f63 6f6e 7574 5f70 7974 686f  ```coconut_pytho
-0001f560: 6e0a 676c 6f62 616c 2073 7461 7465 5f61  n.global state_a
-0001f570: 2c20 7374 6174 655f 623b 2073 7461 7465  , state_b; state
-0001f580: 5f61 2c20 7374 6174 655f 6220 3d20 3130  _a, state_b = 10
-0001f590: 2c20 3130 300a 676c 6f62 616c 2073 7461  , 100.global sta
-0001f5a0: 7465 5f63 3b20 7374 6174 655f 6320 2b3d  te_c; state_c +=
-0001f5b0: 2031 0a60 6060 0a0a 2323 2320 436f 6465   1.```..### Code
-0001f5c0: 2050 6173 7374 6872 6f75 6768 0a0a 436f   Passthrough..Co
-0001f5d0: 636f 6e75 7420 7375 7070 6f72 7473 2074  conut supports t
-0001f5e0: 6865 2061 6269 6c69 7479 2074 6f20 7061  he ability to pa
-0001f5f0: 7373 2061 7262 6974 7261 7279 2063 6f64  ss arbitrary cod
-0001f600: 6520 7468 726f 7567 6820 7468 6520 636f  e through the co
-0001f610: 6d70 696c 6572 2077 6974 686f 7574 2062  mpiler without b
-0001f620: 6569 6e67 2074 6f75 6368 6564 2c20 666f  eing touched, fo
-0001f630: 7220 636f 6d70 6174 6962 696c 6974 7920  r compatibility 
-0001f640: 7769 7468 206f 7468 6572 2076 6172 6961  with other varia
-0001f650: 6e74 7320 6f66 2050 7974 686f 6e2c 2073  nts of Python, s
-0001f660: 7563 6820 6173 205b 4379 7468 6f6e 5d28  uch as [Cython](
-0001f670: 6874 7470 3a2f 2f63 7974 686f 6e2e 6f72  http://cython.or
-0001f680: 672f 2920 6f72 205b 4d79 7468 6f6e 5d28  g/) or [Mython](
-0001f690: 6874 7470 3a2f 2f6d 7974 686f 6e2e 6f72  http://mython.or
-0001f6a0: 672f 292e 2041 6e79 7468 696e 6720 706c  g/). Anything pl
-0001f6b0: 6163 6564 2062 6574 7765 656e 2060 5c28  aced between `\(
-0001f6c0: 6020 616e 6420 7468 6520 636f 7272 6573  ` and the corres
-0001f6d0: 706f 6e64 696e 6720 636c 6f73 6520 7061  ponding close pa
-0001f6e0: 7265 6e74 6865 7369 7320 7769 6c6c 2062  renthesis will b
-0001f6f0: 6520 7061 7373 6564 2074 6872 6f75 6768  e passed through
-0001f700: 2c20 6173 2077 656c 6c20 6173 2061 6e79  , as well as any
-0001f710: 206c 696e 6520 7374 6172 7469 6e67 2077   line starting w
-0001f720: 6974 6820 605c 5c60 2c20 7768 6963 6820  ith `\\`, which 
-0001f730: 7769 6c6c 2068 6176 6520 7468 6520 6164  will have the ad
-0001f740: 6469 7469 6f6e 616c 2065 6666 6563 7420  ditional effect 
-0001f750: 6f66 2061 6c6c 6f77 696e 6720 696e 6465  of allowing inde
-0001f760: 6e74 6174 696f 6e20 756e 6465 7220 6974  ntation under it
-0001f770: 2e0a 0a23 2323 2323 2045 7861 6d70 6c65  ...##### Example
-0001f780: 0a0a 2a2a 436f 636f 6e75 743a 2a2a 0a60  ..**Coconut:**.`
-0001f790: 6060 636f 636f 6e75 740a 5c5c 6364 6566  ``coconut.\\cdef
-0001f7a0: 2066 2878 293a 0a20 2020 2072 6574 7572   f(x):.    retur
-0001f7b0: 6e20 7820 7c3e 2067 0a60 6060 0a0a 2a2a  n x |> g.```..**
-0001f7c0: 5079 7468 6f6e 3a2a 2a0a 6060 6063 6f63  Python:**.```coc
-0001f7d0: 6f6e 7574 5f70 7974 686f 6e0a 6364 6566  onut_python.cdef
-0001f7e0: 2066 2878 293a 0a20 2020 2072 6574 7572   f(x):.    retur
-0001f7f0: 6e20 6728 7829 0a60 6060 0a0a 2323 2320  n g(x).```..### 
-0001f800: 456e 6861 6e63 6564 2050 6172 656e 7468  Enhanced Parenth
-0001f810: 6574 6963 616c 2043 6f6e 7469 6e75 6174  etical Continuat
-0001f820: 696f 6e0a 0a53 696e 6365 2043 6f63 6f6e  ion..Since Cocon
-0001f830: 7574 2073 796e 7461 7820 6973 2061 2073  ut syntax is a s
-0001f840: 7570 6572 7365 7420 6f66 2050 7974 686f  uperset of Pytho
-0001f850: 6e20 3320 7379 6e74 6178 2c20 436f 636f  n 3 syntax, Coco
-0001f860: 6e75 7420 7375 7070 6f72 7473 2074 6865  nut supports the
-0001f870: 2073 616d 6520 6c69 6e65 2063 6f6e 7469   same line conti
-0001f880: 6e75 6174 696f 6e20 7379 6e74 6178 2061  nuation syntax a
-0001f890: 7320 5079 7468 6f6e 2e20 5468 6174 206d  s Python. That m
-0001f8a0: 6561 6e73 2062 6f74 6820 6261 636b 736c  eans both backsl
-0001f8b0: 6173 6820 6c69 6e65 2063 6f6e 7469 6e75  ash line continu
-0001f8c0: 6174 696f 6e20 616e 6420 696d 706c 6965  ation and implie
-0001f8d0: 6420 6c69 6e65 2063 6f6e 7469 6e75 6174  d line continuat
-0001f8e0: 696f 6e20 696e 7369 6465 206f 6620 7061  ion inside of pa
-0001f8f0: 7265 6e74 6865 7365 732c 2062 7261 636b  rentheses, brack
-0001f900: 6574 732c 206f 7220 6272 6163 6573 2077  ets, or braces w
-0001f910: 696c 6c20 616c 6c20 776f 726b 2e0a 0a49  ill all work...I
-0001f920: 6e20 5079 7468 6f6e 2c20 686f 7765 7665  n Python, howeve
-0001f930: 722c 2074 6865 7265 2061 7265 2073 6f6d  r, there are som
-0001f940: 6520 6361 7365 7320 2873 7563 6820 6173  e cases (such as
-0001f950: 206d 756c 7469 706c 6520 6077 6974 6860   multiple `with`
-0001f960: 2073 7461 7465 6d65 6e74 7329 2077 6865   statements) whe
-0001f970: 7265 206f 6e6c 7920 6261 636b 736c 6173  re only backslas
-0001f980: 6820 636f 6e74 696e 7561 7469 6f6e 2c20  h continuation, 
-0001f990: 616e 6420 6e6f 7420 7061 7265 6e74 6865  and not parenthe
-0001f9a0: 7469 6361 6c20 636f 6e74 696e 7561 7469  tical continuati
-0001f9b0: 6f6e 2c20 6973 2073 7570 706f 7274 6564  on, is supported
-0001f9c0: 2e20 436f 636f 6e75 7420 6164 6473 2073  . Coconut adds s
-0001f9d0: 7570 706f 7274 2066 6f72 2070 6172 656e  upport for paren
-0001f9e0: 7468 6574 6963 616c 2063 6f6e 7469 6e75  thetical continu
-0001f9f0: 6174 696f 6e20 696e 2061 6c6c 2074 6865  ation in all the
-0001fa00: 7365 2063 6173 6573 2e20 5468 6973 2061  se cases. This a
-0001fa10: 6c73 6f20 696e 636c 7564 6573 2073 7570  lso includes sup
-0001fa20: 706f 7274 2061 7320 7065 7220 5b50 4550  port as per [PEP
-0001fa30: 2036 3739 5d28 6874 7470 733a 2f2f 7065   679](https://pe
-0001fa40: 7073 2e70 7974 686f 6e2e 6f72 672f 7065  ps.python.org/pe
-0001fa50: 702d 3036 3739 2920 666f 7220 7061 7265  p-0679) for pare
-0001fa60: 6e74 6865 7369 7a65 6420 6061 7373 6572  nthesized `asser
-0001fa70: 7460 2073 7461 7465 6d65 6e74 732e 0a0a  t` statements...
-0001fa80: 5375 7070 6f72 7469 6e67 2070 6172 656e  Supporting paren
-0001fa90: 7468 6574 6963 616c 2063 6f6e 7469 6e75  thetical continu
-0001faa0: 6174 696f 6e20 6576 6572 7977 6865 7265  ation everywhere
-0001fab0: 2061 6c6c 6f77 7320 7468 6520 5b50 4550   allows the [PEP
-0001fac0: 2038 5d28 6874 7470 733a 2f2f 7777 772e   8](https://www.
-0001fad0: 7079 7468 6f6e 2e6f 7267 2f64 6576 2f70  python.org/dev/p
-0001fae0: 6570 732f 7065 702d 3030 3038 2f29 2063  eps/pep-0008/) c
-0001faf0: 6f6e 7665 6e74 696f 6e2c 2077 6869 6368  onvention, which
-0001fb00: 2061 766f 6964 7320 6261 636b 736c 6173   avoids backslas
-0001fb10: 6820 636f 6e74 696e 7561 7469 6f6e 2069  h continuation i
-0001fb20: 6e20 6661 766f 7220 6f66 2069 6d70 6c69  n favor of impli
-0001fb30: 6564 2070 6172 656e 7468 6574 6963 616c  ed parenthetical
-0001fb40: 2063 6f6e 7469 6e75 6174 696f 6e2c 2074   continuation, t
-0001fb50: 6f20 616c 7761 7973 2062 6520 706f 7373  o always be poss
-0001fb60: 6962 6c65 2074 6f20 666f 6c6c 6f77 2e20  ible to follow. 
-0001fb70: 4672 6f6d 2050 4550 2038 3a0a 0a3e 2054  From PEP 8:..> T
-0001fb80: 6865 2070 7265 6665 7272 6564 2077 6179  he preferred way
-0001fb90: 206f 6620 7772 6170 7069 6e67 206c 6f6e   of wrapping lon
-0001fba0: 6720 6c69 6e65 7320 6973 2062 7920 7573  g lines is by us
-0001fbb0: 696e 6720 5079 7468 6f6e 2773 2069 6d70  ing Python's imp
-0001fbc0: 6c69 6564 206c 696e 6520 636f 6e74 696e  lied line contin
-0001fbd0: 7561 7469 6f6e 2069 6e73 6964 6520 7061  uation inside pa
-0001fbe0: 7265 6e74 6865 7365 732c 2062 7261 636b  rentheses, brack
-0001fbf0: 6574 7320 616e 6420 6272 6163 6573 2e20  ets and braces. 
-0001fc00: 4c6f 6e67 206c 696e 6573 2063 616e 2062  Long lines can b
-0001fc10: 6520 6272 6f6b 656e 206f 7665 7220 6d75  e broken over mu
-0001fc20: 6c74 6970 6c65 206c 696e 6573 2062 7920  ltiple lines by 
-0001fc30: 7772 6170 7069 6e67 2065 7870 7265 7373  wrapping express
-0001fc40: 696f 6e73 2069 6e20 7061 7265 6e74 6865  ions in parenthe
-0001fc50: 7365 732e 2054 6865 7365 2073 686f 756c  ses. These shoul
-0001fc60: 6420 6265 2075 7365 6420 696e 2070 7265  d be used in pre
-0001fc70: 6665 7265 6e63 6520 746f 2075 7369 6e67  ference to using
-0001fc80: 2061 2062 6163 6b73 6c61 7368 2066 6f72   a backslash for
-0001fc90: 206c 696e 6520 636f 6e74 696e 7561 7469   line continuati
-0001fca0: 6f6e 2e0a 0a5f 4e6f 7465 3a20 5061 7373  on..._Note: Pass
-0001fcb0: 696e 6720 602d 2d73 7472 6963 7460 2077  ing `--strict` w
-0001fcc0: 696c 6c20 656e 666f 7263 6520 7468 6520  ill enforce the 
-0001fcd0: 5045 5020 3820 636f 6e76 656e 7469 6f6e  PEP 8 convention
-0001fce0: 2062 7920 6469 7361 6c6c 6f77 696e 6720   by disallowing 
-0001fcf0: 6261 636b 736c 6173 6820 636f 6e74 696e  backslash contin
-0001fd00: 7561 7469 6f6e 732e 5f0a 0a23 2323 2323  uations._..#####
-0001fd10: 2045 7861 6d70 6c65 0a0a 2a2a 436f 636f   Example..**Coco
-0001fd20: 6e75 743a 2a2a 0a60 6060 636f 636f 6e75  nut:**.```coconu
-0001fd30: 740a 7769 7468 2028 6f70 656e 2827 2f70  t.with (open('/p
-0001fd40: 6174 682f 746f 2f73 6f6d 652f 6669 6c65  ath/to/some/file
-0001fd50: 2f79 6f75 2f77 616e 742f 746f 2f72 6561  /you/want/to/rea
-0001fd60: 6427 2920 6173 2066 696c 655f 312c 0a20  d') as file_1,. 
-0001fd70: 2020 2020 206f 7065 6e28 272f 7061 7468       open('/path
-0001fd80: 2f74 6f2f 736f 6d65 2f66 696c 652f 6265  /to/some/file/be
-0001fd90: 696e 672f 7772 6974 7465 6e27 2c20 2777  ing/written', 'w
-0001fda0: 2729 2061 7320 6669 6c65 5f32 293a 0a20  ') as file_2):. 
-0001fdb0: 2020 2066 696c 655f 322e 7772 6974 6528     file_2.write(
-0001fdc0: 6669 6c65 5f31 2e72 6561 6428 2929 0a60  file_1.read()).`
-0001fdd0: 6060 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a  ``..**Python:**.
-0001fde0: 6060 6063 6f63 6f6e 7574 5f70 7974 686f  ```coconut_pytho
-0001fdf0: 6e0a 2320 7370 6c69 7420 696e 746f 2074  n.# split into t
-0001fe00: 776f 2077 6974 6820 7374 6174 656d 656e  wo with statemen
-0001fe10: 7473 2066 6f72 2050 7974 686f 6e20 322e  ts for Python 2.
-0001fe20: 3620 636f 6d70 6174 6962 696c 6974 790a  6 compatibility.
-0001fe30: 7769 7468 206f 7065 6e28 272f 7061 7468  with open('/path
-0001fe40: 2f74 6f2f 736f 6d65 2f66 696c 652f 796f  /to/some/file/yo
-0001fe50: 752f 7761 6e74 2f74 6f2f 7265 6164 2729  u/want/to/read')
-0001fe60: 2061 7320 6669 6c65 5f31 3a0a 2020 2020   as file_1:.    
-0001fe70: 7769 7468 206f 7065 6e28 272f 7061 7468  with open('/path
-0001fe80: 2f74 6f2f 736f 6d65 2f66 696c 652f 6265  /to/some/file/be
-0001fe90: 696e 672f 7772 6974 7465 6e27 2c20 2777  ing/written', 'w
-0001fea0: 2729 2061 7320 6669 6c65 5f32 3a0a 2020  ') as file_2:.  
-0001feb0: 2020 2020 2020 6669 6c65 5f32 2e77 7269        file_2.wri
-0001fec0: 7465 2866 696c 655f 312e 7265 6164 2829  te(file_1.read()
-0001fed0: 290a 6060 600a 0a23 2323 2041 7373 6967  ).```..### Assig
-0001fee0: 6e6d 656e 7420 4578 7072 6573 7369 6f6e  nment Expression
-0001fef0: 2043 6861 696e 696e 670a 0a55 6e6c 696b   Chaining..Unlik
-0001ff00: 6520 5079 7468 6f6e 2c20 436f 636f 6e75  e Python, Coconu
-0001ff10: 7420 616c 6c6f 7773 2061 7373 6967 6e6d  t allows assignm
-0001ff20: 656e 7420 6578 7072 6573 7369 6f6e 7320  ent expressions 
-0001ff30: 746f 2062 6520 6368 6169 6e65 642c 2061  to be chained, a
-0001ff40: 7320 696e 2060 6120 3a3d 2062 203a 3d20  s in `a := b := 
-0001ff50: 6360 2e20 4e6f 7465 2c20 686f 7765 7665  c`. Note, howeve
-0001ff60: 722c 2074 6861 7420 6173 7369 676e 6d65  r, that assignme
-0001ff70: 6e74 2065 7870 7265 7373 696f 6e73 2069  nt expressions i
-0001ff80: 6e20 6765 6e65 7261 6c20 6172 6520 6375  n general are cu
-0001ff90: 7272 656e 746c 7920 6f6e 6c79 2073 7570  rrently only sup
-0001ffa0: 706f 7274 6564 206f 6e20 602d 2d74 6172  ported on `--tar
-0001ffb0: 6765 7420 332e 3860 206f 7220 6869 6768  get 3.8` or high
-0001ffc0: 6572 2e0a 0a23 2323 2323 2045 7861 6d70  er...##### Examp
-0001ffd0: 6c65 0a0a 2a2a 436f 636f 6e75 743a 2a2a  le..**Coconut:**
-0001ffe0: 0a60 6060 636f 636f 6e75 740a 2861 203a  .```coconut.(a :
-0001fff0: 3d20 6220 3a3d 2031 290a 6060 600a 0a2a  = b := 1).```..*
-00020000: 2a50 7974 686f 6e3a 2a2a 0a60 6060 636f  *Python:**.```co
-00020010: 636f 6e75 745f 7079 7468 6f6e 0a28 6120  conut_python.(a 
-00020020: 3a3d 2028 6220 3a3d 2031 2929 0a60 6060  := (b := 1)).```
-00020030: 0a0a 2323 2042 7569 6c74 2d49 6e73 0a0a  ..## Built-Ins..
-00020040: 6060 607b 636f 6e74 656e 7473 7d0a 2d2d  ```{contents}.--
-00020050: 2d0a 6c6f 6361 6c3a 0a64 6570 7468 3a20  -.local:.depth: 
-00020060: 320a 2d2d 2d0a 6060 600a 0a23 2323 2042  2.---.```..### B
-00020070: 7569 6c74 2d49 6e20 4675 6e63 7469 6f6e  uilt-In Function
-00020080: 2044 6563 6f72 6174 6f72 730a 0a60 6060   Decorators..```
-00020090: 7b63 6f6e 7465 6e74 737d 0a2d 2d2d 0a6c  {contents}.---.l
-000200a0: 6f63 616c 3a0a 6465 7074 683a 2031 0a2d  ocal:.depth: 1.-
-000200b0: 2d2d 0a60 6060 0a0a 2323 2323 2060 6164  --.```..#### `ad
-000200c0: 6470 6174 7465 726e 600a 0a2a 2a61 6464  dpattern`..**add
-000200d0: 7061 7474 6572 6e2a 2a28 5f62 6173 655c  pattern**(_base\
-000200e0: 5f66 756e 635f 2c20 2a5f 6164 645c 5f66  _func_, *_add\_f
-000200f0: 756e 6373 5f2c 205f 616c 6c6f 775c 5f61  uncs_, _allow\_a
-00020100: 6e79 5c5f 6675 6e63 5f3d 6046 616c 7365  ny\_func_=`False
-00020110: 6029 0a0a 5461 6b65 7320 6f6e 6520 6172  `)..Takes one ar
-00020120: 6775 6d65 6e74 2074 6861 7420 6973 2061  gument that is a
-00020130: 205b 7061 7474 6572 6e2d 6d61 7463 6869   [pattern-matchi
-00020140: 6e67 2066 756e 6374 696f 6e5d 2823 7061  ng function](#pa
-00020150: 7474 6572 6e2d 6d61 7463 6869 6e67 2d66  ttern-matching-f
-00020160: 756e 6374 696f 6e73 292c 2061 6e64 2072  unctions), and r
-00020170: 6574 7572 6e73 2061 2064 6563 6f72 6174  eturns a decorat
-00020180: 6f72 2074 6861 7420 6164 6473 2074 6865  or that adds the
-00020190: 2070 6174 7465 726e 7320 696e 2074 6865   patterns in the
-000201a0: 2065 7869 7374 696e 6720 6675 6e63 7469   existing functi
-000201b0: 6f6e 2074 6f20 7468 6520 6e65 7720 6675  on to the new fu
-000201c0: 6e63 7469 6f6e 2062 6569 6e67 2064 6563  nction being dec
-000201d0: 6f72 6174 6564 2c20 7768 6572 6520 7468  orated, where th
-000201e0: 6520 6578 6973 7469 6e67 2070 6174 7465  e existing patte
-000201f0: 726e 7320 6172 6520 6368 6563 6b65 6420  rns are checked 
-00020200: 6669 7273 742c 2074 6865 6e20 7468 6520  first, then the 
-00020210: 6e65 772e 2060 6164 6470 6174 7465 726e  new. `addpattern
-00020220: 6020 616c 736f 2073 7570 706f 7274 7320  ` also supports 
-00020230: 6120 7368 6f72 7463 7574 2073 796e 7461  a shortcut synta
-00020240: 7820 7768 6572 6520 7468 6520 6e65 7720  x where the new 
-00020250: 7061 7474 6572 6e73 2063 616e 2062 6520  patterns can be 
-00020260: 7061 7373 6564 2069 6e20 6469 7265 6374  passed in direct
-00020270: 6c79 2e0a 0a52 6f75 6768 6c79 2065 7175  ly...Roughly equ
-00020280: 6976 616c 656e 7420 746f 3a0a 6060 600a  ivalent to:.```.
-00020290: 6465 6620 5f70 6174 7465 726e 5f61 6464  def _pattern_add
-000202a0: 6572 2862 6173 655f 6675 6e63 2c20 6164  er(base_func, ad
-000202b0: 645f 6675 6e63 293a 0a20 2020 2064 6566  d_func):.    def
-000202c0: 2061 6464 5f70 6174 7465 726e 5f66 756e   add_pattern_fun
-000202d0: 6328 2a61 7267 732c 202a 2a6b 7761 7267  c(*args, **kwarg
-000202e0: 7329 3a0a 2020 2020 2020 2020 7472 793a  s):.        try:
-000202f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00020300: 7572 6e20 6261 7365 5f66 756e 6328 2a61  urn base_func(*a
-00020310: 7267 732c 202a 2a6b 7761 7267 7329 0a20  rgs, **kwargs). 
-00020320: 2020 2020 2020 2065 7863 6570 7420 4d61         except Ma
-00020330: 7463 6845 7272 6f72 3a0a 2020 2020 2020  tchError:.      
-00020340: 2020 2020 2020 7265 7475 726e 2061 6464        return add
-00020350: 5f66 756e 6328 2a61 7267 732c 202a 2a6b  _func(*args, **k
-00020360: 7761 7267 7329 0a20 2020 2072 6574 7572  wargs).    retur
-00020370: 6e20 6164 645f 7061 7474 6572 6e5f 6675  n add_pattern_fu
-00020380: 6e63 0a64 6566 2061 6464 7061 7474 6572  nc.def addpatter
-00020390: 6e28 6261 7365 5f66 756e 632c 202a 6164  n(base_func, *ad
-000203a0: 645f 6675 6e63 732c 2061 6c6c 6f77 5f61  d_funcs, allow_a
-000203b0: 6e79 5f66 756e 633d 4661 6c73 6529 3a0a  ny_func=False):.
-000203c0: 2020 2020 2222 2244 6563 6f72 6174 6f72      """Decorator
-000203d0: 2074 6f20 6164 6420 6120 6e65 7720 6361   to add a new ca
-000203e0: 7365 2074 6f20 6120 7061 7474 6572 6e2d  se to a pattern-
-000203f0: 6d61 7463 6869 6e67 2066 756e 6374 696f  matching functio
-00020400: 6e20 2877 6865 7265 2074 6865 206e 6577  n (where the new
-00020410: 2063 6173 6520 6973 2063 6865 636b 6564   case is checked
-00020420: 206c 6173 7429 2e0a 0a20 2020 2050 6173   last)...    Pas
-00020430: 7320 616c 6c6f 775f 616e 795f 6675 6e63  s allow_any_func
-00020440: 3d54 7275 6520 746f 2061 6c6c 6f77 2061  =True to allow a
-00020450: 6e79 206f 626a 6563 7420 6173 2074 6865  ny object as the
-00020460: 2062 6173 655f 6675 6e63 2072 6174 6865   base_func rathe
-00020470: 7220 7468 616e 206a 7573 7420 7061 7474  r than just patt
-00020480: 6572 6e2d 6d61 7463 6869 6e67 2066 756e  ern-matching fun
-00020490: 6374 696f 6e73 2e0a 2020 2020 4966 2061  ctions..    If a
-000204a0: 6464 5f66 756e 6320 6973 2070 6173 7365  dd_func is passe
-000204b0: 642c 2061 6464 7061 7474 6572 6e28 6261  d, addpattern(ba
-000204c0: 7365 5f66 756e 632c 2061 6464 5f66 756e  se_func, add_fun
-000204d0: 6329 2069 7320 6571 7569 7661 6c65 6e74  c) is equivalent
-000204e0: 2074 6f20 6164 6470 6174 7465 726e 2862   to addpattern(b
-000204f0: 6173 655f 6675 6e63 2928 6164 645f 6675  ase_func)(add_fu
-00020500: 6e63 292e 0a20 2020 2022 2222 0a20 2020  nc)..    """.   
-00020510: 2069 6620 6e6f 7420 6164 645f 6675 6e63   if not add_func
-00020520: 733a 0a20 2020 2020 2020 2072 6574 7572  s:.        retur
-00020530: 6e20 6164 6470 6174 7465 726e 2428 6261  n addpattern$(ba
-00020540: 7365 5f66 756e 6329 0a20 2020 2066 6f72  se_func).    for
-00020550: 2061 6464 5f66 756e 6320 696e 2061 6464   add_func in add
-00020560: 5f66 756e 6373 3a0a 2020 2020 2020 2020  _funcs:.        
-00020570: 6261 7365 5f66 756e 6320 3d20 7061 7474  base_func = patt
-00020580: 6572 6e5f 6164 6465 7228 6261 7365 5f66  ern_adder(base_f
-00020590: 756e 632c 2061 6464 5f66 756e 6329 0a20  unc, add_func). 
-000205a0: 2020 2072 6574 7572 6e20 6261 7365 5f66     return base_f
-000205b0: 756e 630a 6060 600a 0a49 6620 796f 7520  unc.```..If you 
-000205c0: 7761 6e74 2074 6f20 6769 7665 2061 6e20  want to give an 
-000205d0: 6061 6464 7061 7474 6572 6e60 2066 756e  `addpattern` fun
-000205e0: 6374 696f 6e20 6120 646f 6373 7472 696e  ction a docstrin
-000205f0: 672c 206d 616b 6520 7375 7265 2074 6f20  g, make sure to 
-00020600: 7075 7420 6974 206f 6e20 7468 6520 5f6c  put it on the _l
-00020610: 6173 745f 2066 756e 6374 696f 6e2e 0a0a  ast_ function...
-00020620: 4e6f 7465 2074 6861 7420 7468 6520 6675  Note that the fu
-00020630: 6e63 7469 6f6e 2074 616b 656e 2062 7920  nction taken by 
-00020640: 6061 6464 7061 7474 6572 6e60 206d 7573  `addpattern` mus
-00020650: 7420 6265 2061 2070 6174 7465 726e 2d6d  t be a pattern-m
-00020660: 6174 6368 696e 6720 6675 6e63 7469 6f6e  atching function
-00020670: 2e20 4966 2060 6164 6470 6174 7465 726e  . If `addpattern
-00020680: 6020 7265 6365 6976 6573 2061 206e 6f6e  ` receives a non
-00020690: 2070 6174 7465 726e 2d6d 6174 6368 696e   pattern-matchin
-000206a0: 6720 6675 6e63 7469 6f6e 2c20 7468 6520  g function, the 
-000206b0: 6675 6e63 7469 6f6e 2077 6974 6820 6e6f  function with no
-000206c0: 7420 7261 6973 6520 604d 6174 6368 4572  t raise `MatchEr
-000206d0: 726f 7260 2c20 616e 6420 6061 6464 7061  ror`, and `addpa
-000206e0: 7474 6572 6e60 2077 6f6e 2774 2062 6520  ttern` won't be 
-000206f0: 6162 6c65 2074 6f20 6465 7465 6374 2074  able to detect t
-00020700: 6865 2066 6169 6c65 6420 6d61 7463 682e  he failed match.
-00020710: 2054 6875 732c 2069 6620 6120 6c61 7465   Thus, if a late
-00020720: 7220 6675 6e63 7469 6f6e 2077 6173 206d  r function was m
-00020730: 6561 6e74 2074 6f20 6265 2063 616c 6c65  eant to be calle
-00020740: 642c 2060 6164 6470 6174 7465 726e 6020  d, `addpattern` 
-00020750: 7769 6c6c 206e 6f74 206b 6e6f 7720 7468  will not know th
-00020760: 6174 2074 6865 2066 6972 7374 206d 6174  at the first mat
-00020770: 6368 2066 6169 6c65 6420 616e 6420 7468  ch failed and th
-00020780: 6520 636f 7272 6563 7420 7061 7468 2077  e correct path w
-00020790: 696c 6c20 6e65 7665 7220 6265 2072 6561  ill never be rea
-000207a0: 6368 6564 2e0a 0a46 6f72 2065 7861 6d70  ched...For examp
-000207b0: 6c65 2c20 7468 6520 666f 6c6c 6f77 696e  le, the followin
-000207c0: 6720 636f 6465 2072 6169 7365 7320 6120  g code raises a 
-000207d0: 6054 7970 6545 7272 6f72 603a 0a60 6060  `TypeError`:.```
-000207e0: 636f 636f 6e75 740a 6465 6620 7072 696e  coconut.def prin
-000207f0: 745f 7479 7065 2829 3a0a 2020 2020 7072  t_type():.    pr
-00020800: 696e 7428 2252 6563 6569 7665 6420 6e6f  int("Received no
-00020810: 2061 7267 756d 656e 7473 2e22 290a 0a40   arguments.")..@
-00020820: 6164 6470 6174 7465 726e 2870 7269 6e74  addpattern(print
-00020830: 5f74 7970 6529 0a64 6566 2070 7269 6e74  _type).def print
-00020840: 5f74 7970 6528 696e 7428 2929 3a0a 2020  _type(int()):.  
-00020850: 2020 7072 696e 7428 2252 6563 6569 7665    print("Receive
-00020860: 6420 616e 2069 6e74 2e22 290a 0a70 7269  d an int.")..pri
-00020870: 6e74 5f74 7970 6528 2920 2023 2061 7070  nt_type()  # app
-00020880: 6561 7273 2074 6f20 776f 726b 0a70 7269  ears to work.pri
-00020890: 6e74 5f74 7970 6528 3129 2023 2054 7970  nt_type(1) # Typ
-000208a0: 6545 7272 6f72 3a20 7072 696e 745f 7479  eError: print_ty
-000208b0: 7065 2829 2074 616b 6573 2030 2070 6f73  pe() takes 0 pos
-000208c0: 6974 696f 6e61 6c20 6172 6775 6d65 6e74  itional argument
-000208d0: 7320 6275 7420 3120 7761 7320 6769 7665  s but 1 was give
-000208e0: 6e0a 6060 600a 0a54 6869 7320 6361 6e20  n.```..This can 
-000208f0: 6265 2066 6978 6564 2062 7920 7573 696e  be fixed by usin
-00020900: 6720 6569 7468 6572 2074 6865 2060 6d61  g either the `ma
-00020910: 7463 6860 206f 7220 6061 6464 7061 7474  tch` or `addpatt
-00020920: 6572 6e60 206b 6579 776f 7264 2e20 466f  ern` keyword. Fo
-00020930: 7220 6578 616d 706c 653a 0a60 6060 636f  r example:.```co
-00020940: 636f 6e75 740a 6d61 7463 6820 6465 6620  conut.match def 
-00020950: 7072 696e 745f 7479 7065 2829 3a0a 2020  print_type():.  
-00020960: 2020 7072 696e 7428 2252 6563 6569 7665    print("Receive
-00020970: 6420 6e6f 2061 7267 756d 656e 7473 2e22  d no arguments."
-00020980: 290a 0a61 6464 7061 7474 6572 6e20 6465  )..addpattern de
-00020990: 6620 7072 696e 745f 7479 7065 2869 6e74  f print_type(int
-000209a0: 2829 293a 0a20 2020 2070 7269 6e74 2822  ()):.    print("
-000209b0: 5265 6365 6976 6564 2061 6e20 696e 742e  Received an int.
-000209c0: 2229 0a0a 7072 696e 745f 7479 7065 2831  ")..print_type(1
-000209d0: 2920 2023 2057 6f72 6b73 2061 7320 6578  )  # Works as ex
-000209e0: 7065 6374 6564 0a70 7269 6e74 5f74 7970  pected.print_typ
-000209f0: 6528 2254 6869 7320 6973 2061 2073 7472  e("This is a str
-00020a00: 696e 672e 2229 2023 2052 6169 7365 7320  ing.") # Raises 
-00020a10: 4d61 7463 6845 7272 6f72 0a60 6060 0a0a  MatchError.```..
-00020a20: 5468 6520 6c61 7374 2063 6173 6520 696e  The last case in
-00020a30: 2061 6e20 6061 6464 7061 7474 6572 6e60   an `addpattern`
-00020a40: 2066 756e 6374 696f 6e2c 2068 6f77 6576   function, howev
-00020a50: 6572 2c20 646f 6573 6e27 7420 6861 7665  er, doesn't have
-00020a60: 2074 6f20 6265 2061 2070 6174 7465 726e   to be a pattern
-00020a70: 2d6d 6174 6368 696e 6720 6675 6e63 7469  -matching functi
-00020a80: 6f6e 2069 6620 6974 2069 7320 696e 7465  on if it is inte
-00020a90: 6e64 6564 2074 6f20 6361 7463 6820 616c  nded to catch al
-00020aa0: 6c20 7265 6d61 696e 696e 6720 6361 7365  l remaining case
-00020ab0: 732e 0a0a 546f 2063 6174 6368 2074 6869  s...To catch thi
-00020ac0: 7320 6d69 7374 616b 652c 2060 6164 6470  s mistake, `addp
-00020ad0: 6174 7465 726e 6020 7769 6c6c 2065 6d69  attern` will emi
-00020ae0: 7420 6120 7761 726e 696e 6720 6966 2070  t a warning if p
-00020af0: 6173 7365 6420 7768 6174 2069 7420 6265  assed what it be
-00020b00: 6c69 6576 6573 2074 6f20 6265 2061 206e  lieves to be a n
-00020b10: 6f6e 2d70 6174 7465 726e 2d6d 6174 6368  on-pattern-match
-00020b20: 696e 6720 6675 6e63 7469 6f6e 2e20 486f  ing function. Ho
-00020b30: 7765 7665 722c 2074 6869 7320 7761 726e  wever, this warn
-00020b40: 696e 6720 6361 6e20 736f 6d65 7469 6d65  ing can sometime
-00020b50: 7320 6265 2065 7272 6f6e 656f 7573 2069  s be erroneous i
-00020b60: 6620 7468 6520 6f72 6967 696e 616c 2070  f the original p
-00020b70: 6174 7465 726e 2d6d 6174 6368 696e 6720  attern-matching 
-00020b80: 6675 6e63 7469 6f6e 2068 6173 2062 6565  function has bee
-00020b90: 6e20 7772 6170 7065 6420 696e 2073 6f6d  n wrapped in som
-00020ba0: 6520 7761 792c 2069 6e20 7768 6963 6820  e way, in which 
-00020bb0: 6361 7365 2079 6f75 2063 616e 2070 6173  case you can pas
-00020bc0: 7320 6061 6c6c 6f77 5f61 6e79 5f66 756e  s `allow_any_fun
-00020bd0: 633d 5472 7565 6020 746f 2064 6973 6d69  c=True` to dismi
-00020be0: 7373 2074 6865 2077 6172 6e69 6e67 2e0a  ss the warning..
-00020bf0: 0a23 2323 2323 2045 7861 6d70 6c65 0a0a  .##### Example..
-00020c00: 2a2a 436f 636f 6e75 743a 2a2a 0a60 6060  **Coconut:**.```
-00020c10: 636f 636f 6e75 740a 6465 6620 6661 6374  coconut.def fact
-00020c20: 6f72 6961 6c28 3029 203d 2031 0a0a 4061  orial(0) = 1..@a
-00020c30: 6464 7061 7474 6572 6e28 6661 6374 6f72  ddpattern(factor
-00020c40: 6961 6c29 0a64 6566 2066 6163 746f 7269  ial).def factori
-00020c50: 616c 286e 2920 3d20 6e20 2a20 6661 6374  al(n) = n * fact
-00020c60: 6f72 6961 6c28 6e20 2d20 3129 0a60 6060  orial(n - 1).```
-00020c70: 0a5f 5369 6d70 6c65 2065 7861 6d70 6c65  ._Simple example
-00020c80: 206f 6620 6164 6469 6e67 2061 206e 6577   of adding a new
-00020c90: 2070 6174 7465 726e 2074 6f20 6120 7061   pattern to a pa
-00020ca0: 7474 6572 6e2d 6d61 7463 6869 6e67 2066  ttern-matching f
-00020cb0: 756e 6374 696f 6e2e 5f0a 0a60 6060 636f  unction._..```co
-00020cc0: 636f 6e75 740a 225b 415d 2c20 5b42 5d22  conut."[A], [B]"
-00020cd0: 207c 3e20 7769 6e64 6f77 736f 6624 2833   |> windowsof$(3
-00020ce0: 2920 7c3e 206d 6170 2428 6164 6470 6174  ) |> map$(addpat
-00020cf0: 7465 726e 280a 2020 2020 2864 6566 2028  tern(.    (def (
-00020d00: 2822 5b22 2c22 4122 2c22 5d22 2929 202d  ("[","A","]")) -
-00020d10: 3e20 2241 2229 2c0a 2020 2020 2864 6566  > "A"),.    (def
-00020d20: 2028 2822 5b22 2c22 4222 2c22 5d22 2929   (("[","B","]"))
-00020d30: 202d 3e20 2242 2229 2c0a 2020 2020 2864   -> "B"),.    (d
-00020d40: 6566 2028 285f 2c5f 2c5f 2929 202d 3e20  ef ((_,_,_)) -> 
-00020d50: 4e6f 6e65 292c 0a29 2920 7c3e 2066 696c  None),.)) |> fil
-00020d60: 7465 7224 2828 2e69 7320 4e6f 6e65 2920  ter$((.is None) 
-00020d70: 2e2e 3e20 286e 6f74 2929 207c 3e20 6c69  ..> (not)) |> li
-00020d80: 7374 207c 3e20 7072 696e 740a 6060 600a  st |> print.```.
-00020d90: 5f41 6e20 6578 616d 706c 6520 6f66 2061  _An example of a
-00020da0: 2063 6173 6520 7768 6572 6520 7573 696e   case where usin
-00020db0: 6720 7468 6520 6061 6464 7061 7474 6572  g the `addpatter
-00020dc0: 6e60 2066 756e 6374 696f 6e20 6973 206e  n` function is n
-00020dd0: 6563 6573 7361 7279 206f 7665 7220 7468  ecessary over th
-00020de0: 6520 5b60 6164 6470 6174 7465 726e 6020  e [`addpattern` 
-00020df0: 6b65 7977 6f72 645d 2823 6164 6470 6174  keyword](#addpat
-00020e00: 7465 726e 2d66 756e 6374 696f 6e73 2920  tern-functions) 
-00020e10: 6475 6520 746f 2074 6865 2075 7365 206f  due to the use o
-00020e20: 6620 696e 2d6c 696e 6520 7061 7474 6572  f in-line patter
-00020e30: 6e2d 6d61 7463 6869 6e67 205b 7374 6174  n-matching [stat
-00020e40: 656d 656e 7420 6c61 6d62 6461 735d 2823  ement lambdas](#
-00020e50: 7374 6174 656d 656e 742d 6c61 6d62 6461  statement-lambda
-00020e60: 7329 2e5f 0a0a 2a2a 5079 7468 6f6e 3a2a  s)._..**Python:*
-00020e70: 2a0a 5f43 616e 2774 2062 6520 646f 6e65  *._Can't be done
-00020e80: 2077 6974 686f 7574 2061 2063 6f6d 706c   without a compl
-00020e90: 6963 6174 6564 2064 6563 6f72 6174 6f72  icated decorator
-00020ea0: 2064 6566 696e 6974 696f 6e20 616e 6420   definition and 
-00020eb0: 6120 6c6f 6e67 2073 6572 6965 7320 6f66  a long series of
-00020ec0: 2063 6865 636b 7320 666f 7220 6561 6368   checks for each
-00020ed0: 2070 6174 7465 726e 2d6d 6174 6368 696e   pattern-matchin
-00020ee0: 672e 2053 6565 2074 6865 2063 6f6d 7069  g. See the compi
-00020ef0: 6c65 6420 636f 6465 2066 6f72 2074 6865  led code for the
-00020f00: 2050 7974 686f 6e20 7379 6e74 6178 2e5f   Python syntax._
-00020f10: 0a0a 2323 2323 2320 6070 7265 7061 7474  ..##### `prepatt
-00020f20: 6572 6e60 0a0a 2a2a 4445 5052 4543 4154  ern`..**DEPRECAT
-00020f30: 4544 3a2a 2a20 436f 636f 6e75 7420 616c  ED:** Coconut al
-00020f40: 736f 2068 6173 2061 2060 7072 6570 6174  so has a `prepat
-00020f50: 7465 726e 6020 6275 696c 742d 696e 2c20  tern` built-in, 
-00020f60: 7768 6963 6820 6164 6473 2070 6174 7465  which adds patte
-00020f70: 726e 7320 696e 2074 6865 206f 7070 6f73  rns in the oppos
-00020f80: 6974 6520 6f72 6465 7220 6f66 2060 6164  ite order of `ad
-00020f90: 6470 6174 7465 726e 603b 2060 7072 6570  dpattern`; `prep
-00020fa0: 6174 7465 726e 6020 6973 2064 6566 696e  attern` is defin
-00020fb0: 6564 2061 733a 0a0a 6060 6063 6f63 6f6e  ed as:..```cocon
-00020fc0: 7574 5f70 7974 686f 6e0a 6465 6620 7072  ut_python.def pr
-00020fd0: 6570 6174 7465 726e 2862 6173 655f 6675  epattern(base_fu
-00020fe0: 6e63 293a 0a20 2020 2022 2222 4465 636f  nc):.    """Deco
-00020ff0: 7261 746f 7220 746f 2061 6464 2061 206e  rator to add a n
-00021000: 6577 2063 6173 6520 746f 2061 2070 6174  ew case to a pat
-00021010: 7465 726e 2d6d 6174 6368 696e 6720 6675  tern-matching fu
-00021020: 6e63 7469 6f6e 2c0a 2020 2020 7768 6572  nction,.    wher
-00021030: 6520 7468 6520 6e65 7720 6361 7365 2069  e the new case i
-00021040: 7320 6368 6563 6b65 6420 6669 7273 742e  s checked first.
-00021050: 2222 220a 2020 2020 6465 6620 7061 7474  """.    def patt
-00021060: 6572 6e5f 7072 6570 656e 6465 7228 6675  ern_prepender(fu
-00021070: 6e63 293a 0a20 2020 2020 2020 2072 6574  nc):.        ret
-00021080: 7572 6e20 6164 6470 6174 7465 726e 2866  urn addpattern(f
-00021090: 756e 6329 2862 6173 655f 6675 6e63 290a  unc)(base_func).
-000210a0: 2020 2020 7265 7475 726e 2070 6174 7465      return patte
-000210b0: 726e 5f70 7265 7065 6e64 6572 0a60 6060  rn_prepender.```
-000210c0: 0a5f 4e6f 7465 3a20 5061 7373 696e 6720  ._Note: Passing 
-000210d0: 602d 2d73 7472 6963 7460 2064 6973 6162  `--strict` disab
-000210e0: 6c65 7320 6465 7072 6563 6174 6564 2066  les deprecated f
-000210f0: 6561 7475 7265 732e 5f0a 0a23 2323 2320  eatures._..#### 
-00021100: 606d 656d 6f69 7a65 600a 0a2a 2a6d 656d  `memoize`..**mem
-00021110: 6f69 7a65 2a2a 285f 6d61 7873 697a 655f  oize**(_maxsize_
-00021120: 3d60 4e6f 6e65 602c 205f 7479 7065 645f  =`None`, _typed_
-00021130: 3d60 4661 6c73 6560 290a 0a2a 2a6d 656d  =`False`)..**mem
-00021140: 6f69 7a65 2a2a 285f 7573 6572 5c5f 6675  oize**(_user\_fu
-00021150: 6e63 7469 6f6e 5f29 0a0a 436f 636f 6e75  nction_)..Coconu
-00021160: 7420 7072 6f76 6964 6573 2060 6675 6e63  t provides `func
-00021170: 746f 6f6c 732e 6c72 755f 6361 6368 6560  tools.lru_cache`
-00021180: 2061 7320 6120 6275 696c 742d 696e 2075   as a built-in u
-00021190: 6e64 6572 2074 6865 206e 616d 6520 606d  nder the name `m
-000211a0: 656d 6f69 7a65 6020 7769 7468 2074 6865  emoize` with the
-000211b0: 206d 6f64 6966 6963 6174 696f 6e20 7468   modification th
-000211c0: 6174 2074 6865 205f 6d61 7873 697a 655f  at the _maxsize_
-000211d0: 2070 6172 616d 6574 6572 2069 7320 7365   parameter is se
-000211e0: 7420 746f 2060 4e6f 6e65 6020 6279 2064  t to `None` by d
-000211f0: 6566 6175 6c74 2e20 606d 656d 6f69 7a65  efault. `memoize
-00021200: 6020 6d61 6b65 7320 7468 6520 7573 6520  ` makes the use 
-00021210: 6361 7365 206f 6620 6f70 7469 6d69 7a69  case of optimizi
-00021220: 6e67 2072 6563 7572 7369 7665 2066 756e  ng recursive fun
-00021230: 6374 696f 6e73 2065 6173 6965 722c 2061  ctions easier, a
-00021240: 7320 6120 5f6d 6178 7369 7a65 5f20 6f66  s a _maxsize_ of
-00021250: 2060 4e6f 6e65 6020 6973 2075 7375 616c   `None` is usual
-00021260: 6c79 2077 6861 7420 6973 2064 6573 6972  ly what is desir
-00021270: 6564 2069 6e20 7468 6174 2063 6173 652e  ed in that case.
-00021280: 0a0a 5573 6520 6f66 2060 6d65 6d6f 697a  ..Use of `memoiz
-00021290: 6560 2072 6571 7569 7265 7320 6066 756e  e` requires `fun
-000212a0: 6374 6f6f 6c73 2e6c 7275 5f63 6163 6865  ctools.lru_cache
-000212b0: 602c 2077 6869 6368 2065 7869 7374 7320  `, which exists 
-000212c0: 696e 2074 6865 2050 7974 686f 6e20 3320  in the Python 3 
-000212d0: 7374 616e 6461 7264 206c 6962 7261 7279  standard library
-000212e0: 2c20 6275 7420 756e 6465 7220 5079 7468  , but under Pyth
-000212f0: 6f6e 2032 2077 696c 6c20 7265 7175 6972  on 2 will requir
-00021300: 6520 6070 6970 2069 6e73 7461 6c6c 2062  e `pip install b
-00021310: 6163 6b70 6f72 7473 2e66 756e 6374 6f6f  ackports.functoo
-00021320: 6c73 5f6c 7275 5f63 6163 6865 6020 746f  ls_lru_cache` to
-00021330: 2066 756e 6374 696f 6e2e 2041 6464 6974   function. Addit
-00021340: 696f 6e61 6c6c 792c 2069 6620 6f6e 2050  ionally, if on P
-00021350: 7974 686f 6e20 3220 616e 6420 6062 6163  ython 2 and `bac
-00021360: 6b70 6f72 7473 2e66 756e 6374 6f6f 6c73  kports.functools
-00021370: 5f6c 7275 5f63 6163 6865 6020 6973 2070  _lru_cache` is p
-00021380: 7265 7365 6e74 2c20 436f 636f 6e75 7420  resent, Coconut 
-00021390: 7769 6c6c 2070 6174 6368 2060 6675 6e63  will patch `func
-000213a0: 746f 6f6c 7360 2073 7563 6820 7468 6174  tools` such that
-000213b0: 2060 6675 6e63 746f 6f6c 732e 6c72 755f   `functools.lru_
-000213c0: 6361 6368 6520 3d20 6261 636b 706f 7274  cache = backport
-000213d0: 732e 6675 6e63 746f 6f6c 735f 6c72 755f  s.functools_lru_
-000213e0: 6361 6368 652e 6c72 755f 6361 6368 6560  cache.lru_cache`
-000213f0: 2e0a 0a23 2323 2323 2050 7974 686f 6e20  ...##### Python 
-00021400: 446f 6373 0a0a 402a 2a6d 656d 6f69 7a65  Docs..@**memoize
-00021410: 2a2a 285f 7573 6572 5c5f 6675 6e63 7469  **(_user\_functi
-00021420: 6f6e 5f29 0a0a 402a 2a6d 656d 6f69 7a65  on_)..@**memoize
-00021430: 2a2a 285f 6d61 7873 697a 653d 4e6f 6e65  **(_maxsize=None
-00021440: 2c20 7479 7065 643d 4661 6c73 655f 290a  , typed=False_).
-00021450: 0a44 6563 6f72 6174 6f72 2074 6f20 7772  .Decorator to wr
-00021460: 6170 2061 2066 756e 6374 696f 6e20 7769  ap a function wi
-00021470: 7468 2061 206d 656d 6f69 7a69 6e67 2063  th a memoizing c
-00021480: 616c 6c61 626c 6520 7468 6174 2073 6176  allable that sav
-00021490: 6573 2075 7020 746f 2074 6865 205f 6d61  es up to the _ma
-000214a0: 7873 697a 655f 206d 6f73 7420 7265 6365  xsize_ most rece
-000214b0: 6e74 2063 616c 6c73 2e20 4974 2063 616e  nt calls. It can
-000214c0: 2073 6176 6520 7469 6d65 2077 6865 6e20   save time when 
-000214d0: 616e 2065 7870 656e 7369 7665 206f 7220  an expensive or 
-000214e0: 492f 4f20 626f 756e 6420 6675 6e63 7469  I/O bound functi
-000214f0: 6f6e 2069 7320 7065 7269 6f64 6963 616c  on is periodical
-00021500: 6c79 2063 616c 6c65 6420 7769 7468 2074  ly called with t
-00021510: 6865 2073 616d 6520 6172 6775 6d65 6e74  he same argument
-00021520: 732e 0a0a 5369 6e63 6520 6120 6469 6374  s...Since a dict
-00021530: 696f 6e61 7279 2069 7320 7573 6564 2074  ionary is used t
-00021540: 6f20 6361 6368 6520 7265 7375 6c74 732c  o cache results,
-00021550: 2074 6865 2070 6f73 6974 696f 6e61 6c20   the positional 
-00021560: 616e 6420 6b65 7977 6f72 6420 6172 6775  and keyword argu
-00021570: 6d65 6e74 7320 746f 2074 6865 2066 756e  ments to the fun
-00021580: 6374 696f 6e20 6d75 7374 2062 6520 6861  ction must be ha
-00021590: 7368 6162 6c65 2e0a 0a44 6973 7469 6e63  shable...Distinc
-000215a0: 7420 6172 6775 6d65 6e74 2070 6174 7465  t argument patte
-000215b0: 726e 7320 6d61 7920 6265 2063 6f6e 7369  rns may be consi
-000215c0: 6465 7265 6420 746f 2062 6520 6469 7374  dered to be dist
-000215d0: 696e 6374 2063 616c 6c73 2077 6974 6820  inct calls with 
-000215e0: 7365 7061 7261 7465 2063 6163 6865 2065  separate cache e
-000215f0: 6e74 7269 6573 2e20 466f 7220 6578 616d  ntries. For exam
-00021600: 706c 652c 2060 6628 613d 312c 2062 3d32  ple, `f(a=1, b=2
-00021610: 2960 2061 6e64 2060 6628 623d 322c 2061  )` and `f(b=2, a
-00021620: 3d31 2960 2064 6966 6665 7220 696e 2074  =1)` differ in t
-00021630: 6865 6972 206b 6579 776f 7264 2061 7267  heir keyword arg
-00021640: 756d 656e 7420 6f72 6465 7220 616e 6420  ument order and 
-00021650: 6d61 7920 6861 7665 2074 776f 2073 6570  may have two sep
-00021660: 6172 6174 6520 6361 6368 6520 656e 7472  arate cache entr
-00021670: 6965 732e 0a0a 4966 205f 7573 6572 5c5f  ies...If _user\_
-00021680: 6675 6e63 7469 6f6e 5f20 6973 2073 7065  function_ is spe
-00021690: 6369 6669 6564 2c20 6974 206d 7573 7420  cified, it must 
-000216a0: 6265 2061 2063 616c 6c61 626c 652e 2054  be a callable. T
-000216b0: 6869 7320 616c 6c6f 7773 2074 6865 205f  his allows the _
-000216c0: 6d65 6d6f 697a 655f 2064 6563 6f72 6174  memoize_ decorat
-000216d0: 6f72 2074 6f20 6265 2061 7070 6c69 6564  or to be applied
-000216e0: 2064 6972 6563 746c 7920 746f 2061 2075   directly to a u
-000216f0: 7365 7220 6675 6e63 7469 6f6e 2c20 6c65  ser function, le
-00021700: 6176 696e 6720 7468 6520 6d61 7873 697a  aving the maxsiz
-00021710: 6520 6174 2069 7473 2064 6566 6175 6c74  e at its default
-00021720: 2076 616c 7565 206f 6620 604e 6f6e 6560   value of `None`
-00021730: 3a0a 6060 6063 6f63 6f6e 7574 5f70 7974  :.```coconut_pyt
-00021740: 686f 6e0a 406d 656d 6f69 7a65 0a64 6566  hon.@memoize.def
-00021750: 2063 6f75 6e74 5f76 6f77 656c 7328 7365   count_vowels(se
-00021760: 6e74 656e 6365 293a 0a20 2020 2072 6574  ntence):.    ret
-00021770: 7572 6e20 7375 6d28 7365 6e74 656e 6365  urn sum(sentence
-00021780: 2e63 6f75 6e74 2876 6f77 656c 2920 666f  .count(vowel) fo
-00021790: 7220 766f 7765 6c20 696e 2027 4145 494f  r vowel in 'AEIO
-000217a0: 5561 6569 6f75 2729 0a60 6060 0a0a 4966  Uaeiou').```..If
-000217b0: 205f 6d61 7873 697a 655f 2069 7320 7365   _maxsize_ is se
-000217c0: 7420 746f 2060 4e6f 6e65 602c 2074 6865  t to `None`, the
-000217d0: 204c 5255 2066 6561 7475 7265 2069 7320   LRU feature is 
-000217e0: 6469 7361 626c 6564 2061 6e64 2074 6865  disabled and the
-000217f0: 2063 6163 6865 2063 616e 2067 726f 7720   cache can grow 
-00021800: 7769 7468 6f75 7420 626f 756e 642e 0a0a  without bound...
-00021810: 4966 205f 7479 7065 645f 2069 7320 7365  If _typed_ is se
-00021820: 7420 746f 2074 7275 652c 2066 756e 6374  t to true, funct
-00021830: 696f 6e20 6172 6775 6d65 6e74 7320 6f66  ion arguments of
-00021840: 2064 6966 6665 7265 6e74 2074 7970 6573   different types
-00021850: 2077 696c 6c20 6265 2063 6163 6865 6420   will be cached 
-00021860: 7365 7061 7261 7465 6c79 2e20 4966 2074  separately. If t
-00021870: 7970 6564 2069 7320 6661 6c73 652c 2074  yped is false, t
-00021880: 6865 2069 6d70 6c65 6d65 6e74 6174 696f  he implementatio
-00021890: 6e20 7769 6c6c 2075 7375 616c 6c79 2072  n will usually r
-000218a0: 6567 6172 6420 7468 656d 2061 7320 6571  egard them as eq
-000218b0: 7569 7661 6c65 6e74 2063 616c 6c73 2061  uivalent calls a
-000218c0: 6e64 206f 6e6c 7920 6361 6368 6520 6120  nd only cache a 
-000218d0: 7369 6e67 6c65 2072 6573 756c 742e 2028  single result. (
-000218e0: 536f 6d65 2074 7970 6573 2073 7563 6820  Some types such 
-000218f0: 6173 2073 7472 2061 6e64 2069 6e74 206d  as str and int m
-00021900: 6179 2062 6520 6361 6368 6564 2073 6570  ay be cached sep
-00021910: 6172 6174 656c 7920 6576 656e 2077 6865  arately even whe
-00021920: 6e20 7479 7065 6420 6973 2066 616c 7365  n typed is false
-00021930: 2e29 0a0a 4e6f 7465 2c20 7479 7065 2073  .)..Note, type s
-00021940: 7065 6369 6669 6369 7479 2061 7070 6c69  pecificity appli
-00021950: 6573 206f 6e6c 7920 746f 2074 6865 2066  es only to the f
-00021960: 756e 6374 696f 6ee2 8099 7320 696d 6d65  unction...s imme
-00021970: 6469 6174 6520 6172 6775 6d65 6e74 7320  diate arguments 
-00021980: 7261 7468 6572 2074 6861 6e20 7468 6569  rather than thei
-00021990: 7220 636f 6e74 656e 7473 2e20 5468 6520  r contents. The 
-000219a0: 7363 616c 6172 2061 7267 756d 656e 7473  scalar arguments
-000219b0: 2c20 6044 6563 696d 616c 2834 3229 6020  , `Decimal(42)` 
-000219c0: 616e 6420 6046 7261 6374 696f 6e28 3432  and `Fraction(42
-000219d0: 2960 2061 7265 2062 6520 7472 6561 7465  )` are be treate
-000219e0: 6420 6173 2064 6973 7469 6e63 7420 6361  d as distinct ca
-000219f0: 6c6c 7320 7769 7468 2064 6973 7469 6e63  lls with distinc
-00021a00: 7420 7265 7375 6c74 732e 2049 6e20 636f  t results. In co
-00021a10: 6e74 7261 7374 2c20 7468 6520 7475 706c  ntrast, the tupl
-00021a20: 6520 6172 6775 6d65 6e74 7320 6028 2761  e arguments `('a
-00021a30: 6e73 7765 7227 2c20 4465 6369 6d61 6c28  nswer', Decimal(
-00021a40: 3432 2929 6020 616e 6420 6028 2761 6e73  42))` and `('ans
-00021a50: 7765 7227 2c20 4672 6163 7469 6f6e 2834  wer', Fraction(4
-00021a60: 3229 2960 2061 7265 2074 7265 6174 6564  2))` are treated
-00021a70: 2061 7320 6571 7569 7661 6c65 6e74 2e0a   as equivalent..
-00021a80: 0a54 6865 2064 6563 6f72 6174 6f72 2061  .The decorator a
-00021a90: 6c73 6f20 7072 6f76 6964 6573 2061 2060  lso provides a `
-00021aa0: 6361 6368 655f 636c 6561 7228 2960 2066  cache_clear()` f
-00021ab0: 756e 6374 696f 6e20 666f 7220 636c 6561  unction for clea
-00021ac0: 7269 6e67 206f 7220 696e 7661 6c69 6461  ring or invalida
-00021ad0: 7469 6e67 2074 6865 2063 6163 6865 2e0a  ting the cache..
-00021ae0: 0a54 6865 206f 7269 6769 6e61 6c20 756e  .The original un
-00021af0: 6465 726c 7969 6e67 2066 756e 6374 696f  derlying functio
-00021b00: 6e20 6973 2061 6363 6573 7369 626c 6520  n is accessible 
-00021b10: 7468 726f 7567 6820 7468 6520 605f 5f77  through the `__w
-00021b20: 7261 7070 6564 5f5f 6020 6174 7472 6962  rapped__` attrib
-00021b30: 7574 652e 2054 6869 7320 6973 2075 7365  ute. This is use
-00021b40: 6675 6c20 666f 7220 696e 7472 6f73 7065  ful for introspe
-00021b50: 6374 696f 6e2c 2066 6f72 2062 7970 6173  ction, for bypas
-00021b60: 7369 6e67 2074 6865 2063 6163 6865 2c20  sing the cache, 
-00021b70: 6f72 2066 6f72 2072 6577 7261 7070 696e  or for rewrappin
-00021b80: 6720 7468 6520 6675 6e63 7469 6f6e 2077  g the function w
-00021b90: 6974 6820 6120 6469 6666 6572 656e 7420  ith a different 
-00021ba0: 6361 6368 652e 0a0a 5468 6520 6361 6368  cache...The cach
-00021bb0: 6520 6b65 6570 7320 7265 6665 7265 6e63  e keeps referenc
-00021bc0: 6573 2074 6f20 7468 6520 6172 6775 6d65  es to the argume
-00021bd0: 6e74 7320 616e 6420 7265 7475 726e 2076  nts and return v
-00021be0: 616c 7565 7320 756e 7469 6c20 7468 6579  alues until they
-00021bf0: 2061 6765 206f 7574 206f 6620 7468 6520   age out of the 
-00021c00: 6361 6368 6520 6f72 2075 6e74 696c 2074  cache or until t
-00021c10: 6865 2063 6163 6865 2069 7320 636c 6561  he cache is clea
-00021c20: 7265 642e 0a0a 4966 2061 206d 6574 686f  red...If a metho
-00021c30: 6420 6973 2063 6163 6865 642c 2074 6865  d is cached, the
-00021c40: 2060 7365 6c66 6020 696e 7374 616e 6365   `self` instance
-00021c50: 2061 7267 756d 656e 7420 6973 2069 6e63   argument is inc
-00021c60: 6c75 6465 6420 696e 2074 6865 2063 6163  luded in the cac
-00021c70: 6865 2e20 5365 6520 5b48 6f77 2064 6f20  he. See [How do 
-00021c80: 4920 6361 6368 6520 6d65 7468 6f64 2063  I cache method c
-00021c90: 616c 6c73 3f5d 2868 7474 7073 3a2f 2f64  alls?](https://d
-00021ca0: 6f63 732e 7079 7468 6f6e 2e6f 7267 2f33  ocs.python.org/3
-00021cb0: 2f66 6171 2f70 726f 6772 616d 6d69 6e67  /faq/programming
-00021cc0: 2e68 746d 6c23 6661 712d 6361 6368 652d  .html#faq-cache-
-00021cd0: 6d65 7468 6f64 2d63 616c 6c73 290a 0a41  method-calls)..A
-00021ce0: 6e20 5b4c 5255 2028 6c65 6173 7420 7265  n [LRU (least re
-00021cf0: 6365 6e74 6c79 2075 7365 6429 2063 6163  cently used) cac
-00021d00: 6865 5d28 6874 7470 733a 2f2f 656e 2e77  he](https://en.w
-00021d10: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
-00021d20: 692f 4361 6368 655f 7265 706c 6163 656d  i/Cache_replacem
-00021d30: 656e 745f 706f 6c69 6369 6573 234c 6561  ent_policies#Lea
-00021d40: 7374 5f72 6563 656e 746c 795f 7573 6564  st_recently_used
-00021d50: 5f28 4c52 5529 2920 776f 726b 7320 6265  _(LRU)) works be
-00021d60: 7374 2077 6865 6e20 7468 6520 6d6f 7374  st when the most
-00021d70: 2072 6563 656e 7420 6361 6c6c 7320 6172   recent calls ar
-00021d80: 6520 7468 6520 6265 7374 2070 7265 6469  e the best predi
-00021d90: 6374 6f72 7320 6f66 2075 7063 6f6d 696e  ctors of upcomin
-00021da0: 6720 6361 6c6c 7320 2866 6f72 2065 7861  g calls (for exa
-00021db0: 6d70 6c65 2c20 7468 6520 6d6f 7374 2070  mple, the most p
-00021dc0: 6f70 756c 6172 2061 7274 6963 6c65 7320  opular articles 
-00021dd0: 6f6e 2061 206e 6577 7320 7365 7276 6572  on a news server
-00021de0: 2074 656e 6420 746f 2063 6861 6e67 6520   tend to change 
-00021df0: 6561 6368 2064 6179 292e 2054 6865 2063  each day). The c
-00021e00: 6163 6865 e280 9973 2073 697a 6520 6c69  ache...s size li
-00021e10: 6d69 7420 6173 7375 7265 7320 7468 6174  mit assures that
-00021e20: 2074 6865 2063 6163 6865 2064 6f65 7320   the cache does 
-00021e30: 6e6f 7420 6772 6f77 2077 6974 686f 7574  not grow without
-00021e40: 2062 6f75 6e64 206f 6e20 6c6f 6e67 2d72   bound on long-r
-00021e50: 756e 6e69 6e67 2070 726f 6365 7373 6573  unning processes
-00021e60: 2073 7563 6820 6173 2077 6562 2073 6572   such as web ser
-00021e70: 7665 7273 2e0a 0a49 6e20 6765 6e65 7261  vers...In genera
-00021e80: 6c2c 2074 6865 204c 5255 2063 6163 6865  l, the LRU cache
-00021e90: 2073 686f 756c 6420 6f6e 6c79 2062 6520   should only be 
-00021ea0: 7573 6564 2077 6865 6e20 796f 7520 7761  used when you wa
-00021eb0: 6e74 2074 6f20 7265 7573 6520 7072 6576  nt to reuse prev
-00021ec0: 696f 7573 6c79 2063 6f6d 7075 7465 6420  iously computed 
-00021ed0: 7661 6c75 6573 2e20 4163 636f 7264 696e  values. Accordin
-00021ee0: 676c 792c 2069 7420 646f 6573 6ee2 8099  gly, it doesn...
-00021ef0: 7420 6d61 6b65 2073 656e 7365 2074 6f20  t make sense to 
-00021f00: 6361 6368 6520 6675 6e63 7469 6f6e 7320  cache functions 
-00021f10: 7769 7468 2073 6964 652d 6566 6665 6374  with side-effect
-00021f20: 732c 2066 756e 6374 696f 6e73 2074 6861  s, functions tha
-00021f30: 7420 6e65 6564 2074 6f20 6372 6561 7465  t need to create
-00021f40: 2064 6973 7469 6e63 7420 6d75 7461 626c   distinct mutabl
-00021f50: 6520 6f62 6a65 6374 7320 6f6e 2065 6163  e objects on eac
-00021f60: 6820 6361 6c6c 2c20 6f72 2069 6d70 7572  h call, or impur
-00021f70: 6520 6675 6e63 7469 6f6e 7320 7375 6368  e functions such
-00021f80: 2061 7320 7469 6d65 2829 206f 7220 7261   as time() or ra
-00021f90: 6e64 6f6d 2829 2e0a 0a45 7861 6d70 6c65  ndom()...Example
-00021fa0: 206f 6620 6566 6669 6369 656e 746c 7920   of efficiently 
-00021fb0: 636f 6d70 7574 696e 6720 4669 626f 6e61  computing Fibona
-00021fc0: 6363 6920 6e75 6d62 6572 7320 7573 696e  cci numbers usin
-00021fd0: 6720 6120 6361 6368 6520 746f 2069 6d70  g a cache to imp
-00021fe0: 6c65 6d65 6e74 2061 2064 796e 616d 6963  lement a dynamic
-00021ff0: 2070 726f 6772 616d 6d69 6e67 2074 6563   programming tec
-00022000: 686e 6971 7565 3a0a 6060 6063 6f63 6f6e  hnique:.```cocon
-00022010: 7574 5f70 7963 6f6e 0a40 6d65 6d6f 697a  ut_pycon.@memoiz
-00022020: 650a 6465 6620 6669 6228 6e29 3a0a 2020  e.def fib(n):.  
-00022030: 2020 6966 206e 203c 2032 3a0a 2020 2020    if n < 2:.    
-00022040: 2020 2020 7265 7475 726e 206e 0a20 2020      return n.   
-00022050: 2072 6574 7572 6e20 6669 6228 6e2d 3129   return fib(n-1)
-00022060: 202b 2066 6962 286e 2d32 290a 0a3e 3e3e   + fib(n-2)..>>>
-00022070: 205b 6669 6228 6e29 2066 6f72 206e 2069   [fib(n) for n i
-00022080: 6e20 7261 6e67 6528 3136 295d 0a5b 302c  n range(16)].[0,
-00022090: 2031 2c20 312c 2032 2c20 332c 2035 2c20   1, 1, 2, 3, 5, 
-000220a0: 382c 2031 332c 2032 312c 2033 342c 2035  8, 13, 21, 34, 5
-000220b0: 352c 2038 392c 2031 3434 2c20 3233 332c  5, 89, 144, 233,
-000220c0: 2033 3737 2c20 3631 305d 0a0a 3e3e 3e20   377, 610]..>>> 
-000220d0: 6669 622e 6361 6368 655f 696e 666f 2829  fib.cache_info()
-000220e0: 0a43 6163 6865 496e 666f 2868 6974 733d  .CacheInfo(hits=
-000220f0: 3238 2c20 6d69 7373 6573 3d31 362c 206d  28, misses=16, m
-00022100: 6178 7369 7a65 3d4e 6f6e 652c 2063 7572  axsize=None, cur
-00022110: 7273 697a 653d 3136 290a 6060 600a 0a23  rsize=16).```..#
-00022120: 2323 2323 2045 7861 6d70 6c65 0a0a 2a2a  #### Example..**
-00022130: 436f 636f 6e75 743a 2a2a 0a60 6060 636f  Coconut:**.```co
-00022140: 636f 6e75 740a 6465 6620 6669 6228 6e20  conut.def fib(n 
-00022150: 6966 206e 203c 2032 2920 3d20 6e0a 0a40  if n < 2) = n..@
-00022160: 6d65 6d6f 697a 650a 4061 6464 7061 7474  memoize.@addpatt
-00022170: 6572 6e28 6669 6229 0a64 6566 2066 6962  ern(fib).def fib
-00022180: 286e 2920 3d20 6669 6228 6e2d 3129 202b  (n) = fib(n-1) +
-00022190: 2066 6962 286e 2d32 290a 6060 600a 0a2a   fib(n-2).```..*
-000221a0: 2a50 7974 686f 6e3a 2a2a 0a60 6060 636f  *Python:**.```co
-000221b0: 636f 6e75 745f 7079 7468 6f6e 0a74 7279  conut_python.try
-000221c0: 3a0a 2020 2020 6672 6f6d 2066 756e 6374  :.    from funct
-000221d0: 6f6f 6c73 2069 6d70 6f72 7420 6c72 755f  ools import lru_
-000221e0: 6361 6368 650a 6578 6365 7074 2049 6d70  cache.except Imp
-000221f0: 6f72 7445 7272 6f72 3a0a 2020 2020 6672  ortError:.    fr
-00022200: 6f6d 2062 6163 6b70 6f72 7473 2e66 756e  om backports.fun
-00022210: 6374 6f6f 6c73 5f6c 7275 5f63 6163 6865  ctools_lru_cache
-00022220: 2069 6d70 6f72 7420 6c72 755f 6361 6368   import lru_cach
-00022230: 650a 406c 7275 5f63 6163 6865 286d 6178  e.@lru_cache(max
-00022240: 7369 7a65 3d4e 6f6e 6529 0a64 6566 2066  size=None).def f
-00022250: 6962 286e 293a 0a20 2020 2069 6620 6e20  ib(n):.    if n 
-00022260: 3c20 323a 0a20 2020 2020 2020 2072 6574  < 2:.        ret
-00022270: 7572 6e20 6e0a 2020 2020 7265 7475 726e  urn n.    return
-00022280: 2066 6962 286e 2d31 2920 2b20 6669 6228   fib(n-1) + fib(
-00022290: 6e2d 3229 0a60 6060 0a0a 2323 2323 2060  n-2).```..#### `
-000222a0: 6f76 6572 7269 6465 600a 0a2a 2a6f 7665  override`..**ove
-000222b0: 7272 6964 652a 2a28 5f66 756e 635f 290a  rride**(_func_).
-000222c0: 0a43 6f63 6f6e 7574 2070 726f 7669 6465  .Coconut provide
-000222d0: 7320 7468 6520 6040 6f76 6572 7269 6465  s the `@override
-000222e0: 6020 6465 636f 7261 746f 7220 746f 2061  ` decorator to a
-000222f0: 6c6c 6f77 2064 6563 6c61 7269 6e67 2061  llow declaring a
-00022300: 206d 6574 686f 6420 6465 6669 6e69 7469   method definiti
-00022310: 6f6e 2069 6e20 6120 7375 6263 6c61 7373  on in a subclass
-00022320: 2061 7320 616e 206f 7665 7272 6964 6520   as an override 
-00022330: 6f66 2073 6f6d 6520 7061 7265 6e74 2063  of some parent c
-00022340: 6c61 7373 206d 6574 686f 642e 2057 6865  lass method. Whe
-00022350: 6e20 6040 6f76 6572 7269 6465 6020 6973  n `@override` is
-00022360: 2075 7365 6420 6f6e 2061 206d 6574 686f   used on a metho
-00022370: 642c 2069 6620 6120 6d65 7468 6f64 206f  d, if a method o
-00022380: 6620 7468 6520 7361 6d65 206e 616d 6520  f the same name 
-00022390: 646f 6573 206e 6f74 2065 7869 7374 206f  does not exist o
-000223a0: 6e20 736f 6d65 2070 6172 656e 7420 636c  n some parent cl
-000223b0: 6173 732c 2074 6865 2063 6c61 7373 2064  ass, the class d
-000223c0: 6566 696e 6974 696f 6e20 7769 6c6c 2072  efinition will r
-000223d0: 6169 7365 2061 2060 5275 6e74 696d 6545  aise a `RuntimeE
-000223e0: 7272 6f72 602e 0a0a 4164 6469 7469 6f6e  rror`...Addition
-000223f0: 616c 6c79 2c20 606f 7665 7272 6964 6560  ally, `override`
-00022400: 2077 696c 6c20 7072 6573 656e 7420 746f   will present to
-00022410: 2074 7970 6520 6368 6563 6b65 7273 2061   type checkers a
-00022420: 7320 5b60 7479 7069 6e67 5f65 7874 656e  s [`typing_exten
-00022430: 7369 6f6e 732e 6f76 6572 7269 6465 605d  sions.override`]
-00022440: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-00022450: 672f 7072 6f6a 6563 742f 7479 7069 6e67  g/project/typing
-00022460: 2d65 7874 656e 7369 6f6e 732f 292e 0a0a  -extensions/)...
-00022470: 2323 2323 2320 4578 616d 706c 650a 0a2a  ##### Example..*
-00022480: 2a43 6f63 6f6e 7574 3a2a 2a0a 6060 6063  *Coconut:**.```c
-00022490: 6f63 6f6e 7574 0a63 6c61 7373 2041 3a0a  oconut.class A:.
-000224a0: 2020 2020 7820 3d20 310a 2020 2020 6465      x = 1.    de
-000224b0: 6620 6628 7365 6c66 2c20 7929 203d 2073  f f(self, y) = s
-000224c0: 656c 662e 7820 2b20 790a 0a63 6c61 7373  elf.x + y..class
-000224d0: 2042 3a0a 2020 2020 406f 7665 7272 6964   B:.    @overrid
-000224e0: 650a 2020 2020 6465 6620 6628 7365 6c66  e.    def f(self
-000224f0: 2c20 7929 203d 2073 656c 662e 7820 2b20  , y) = self.x + 
-00022500: 7920 2b20 310a 6060 600a 0a2a 2a50 7974  y + 1.```..**Pyt
-00022510: 686f 6e3a 2a2a 0a5f 4361 6e27 7420 6265  hon:**._Can't be
-00022520: 2064 6f6e 6520 7769 7468 6f75 7420 6120   done without a 
-00022530: 6c6f 6e67 2064 6563 6f72 6174 6f72 2064  long decorator d
-00022540: 6566 696e 6974 696f 6e2e 2054 6865 2066  efinition. The f
-00022550: 756c 6c20 6465 6669 6e69 7469 6f6e 206f  ull definition o
-00022560: 6620 7468 6520 6465 636f 7261 746f 7220  f the decorator 
-00022570: 696e 2050 7974 686f 6e20 6361 6e20 6265  in Python can be
-00022580: 2066 6f75 6e64 2069 6e20 7468 6520 436f   found in the Co
-00022590: 636f 6e75 7420 6865 6164 6572 2e5f 0a0a  conut header._..
-000225a0: 2323 2323 2060 7265 6375 7273 6976 655f  #### `recursive_
-000225b0: 6974 6572 6174 6f72 600a 0a2a 2a72 6563  iterator`..**rec
-000225c0: 7572 7369 7665 5c5f 6974 6572 6174 6f72  ursive\_iterator
-000225d0: 2a2a 285f 6675 6e63 5f29 0a0a 436f 636f  **(_func_)..Coco
-000225e0: 6e75 7420 7072 6f76 6964 6573 2061 2060  nut provides a `
-000225f0: 7265 6375 7273 6976 655f 6974 6572 6174  recursive_iterat
-00022600: 6f72 6020 6465 636f 7261 746f 7220 7468  or` decorator th
-00022610: 6174 206d 656d 6f69 7a65 7320 616e 7920  at memoizes any 
-00022620: 7374 6174 656c 6573 732c 2072 6563 7572  stateless, recur
-00022630: 7369 7665 2066 756e 6374 696f 6e20 7468  sive function th
-00022640: 6174 2072 6574 7572 6e73 2061 6e20 6974  at returns an it
-00022650: 6572 6174 6f72 2e20 546f 2075 7365 2060  erator. To use `
-00022660: 7265 6375 7273 6976 655f 6974 6572 6174  recursive_iterat
-00022670: 6f72 6020 6f6e 2061 2066 756e 6374 696f  or` on a functio
-00022680: 6e2c 2069 7420 6d75 7374 206d 6565 7420  n, it must meet 
-00022690: 7468 6520 666f 6c6c 6f77 696e 6720 6372  the following cr
-000226a0: 6974 6572 6961 3a0a 0a31 2e20 796f 7572  iteria:..1. your
-000226b0: 2066 756e 6374 696f 6e20 6569 7468 6572   function either
-000226c0: 2061 6c77 6179 7320 6072 6574 7572 6e60   always `return`
-000226d0: 7320 616e 2069 7465 7261 746f 7220 6f72  s an iterator or
-000226e0: 2067 656e 6572 6174 6573 2061 6e20 6974   generates an it
-000226f0: 6572 6174 6f72 2075 7369 6e67 2060 7969  erator using `yi
-00022700: 656c 6460 2c0a 322e 2077 6865 6e20 6361  eld`,.2. when ca
-00022710: 6c6c 6564 206d 756c 7469 706c 6520 7469  lled multiple ti
-00022720: 6d65 7320 7769 7468 2061 7267 756d 656e  mes with argumen
-00022730: 7473 2074 6861 7420 6172 6520 6571 7561  ts that are equa
-00022740: 6c2c 2079 6f75 7220 6675 6e63 7469 6f6e  l, your function
-00022750: 2070 726f 6475 6365 7320 7468 6520 7361   produces the sa
-00022760: 6d65 2069 7465 7261 746f 7220 2879 6f75  me iterator (you
-00022770: 7220 6675 6e63 7469 6f6e 2069 7320 7374  r function is st
-00022780: 6174 656c 6573 7329 2c20 616e 640a 332e  ateless), and.3.
-00022790: 2079 6f75 7220 6675 6e63 7469 6f6e 2067   your function g
-000227a0: 6574 7320 6361 6c6c 6564 2028 7573 7561  ets called (usua
-000227b0: 6c6c 7920 6361 6c6c 7320 6974 7365 6c66  lly calls itself
-000227c0: 2920 6d75 6c74 6970 6c65 2074 696d 6573  ) multiple times
-000227d0: 2077 6974 6820 7468 6520 7361 6d65 2061   with the same a
-000227e0: 7267 756d 656e 7473 2e0a 0a49 6620 796f  rguments...If yo
-000227f0: 7520 6172 6520 656e 636f 756e 7465 7269  u are encounteri
-00022800: 6e67 2061 2060 5275 6e74 696d 6545 7272  ng a `RuntimeErr
-00022810: 6f72 6020 6475 6520 746f 206d 6178 696d  or` due to maxim
-00022820: 756d 2072 6563 7572 7369 6f6e 2064 6570  um recursion dep
-00022830: 7468 2c20 6974 2069 7320 6869 6768 6c79  th, it is highly
-00022840: 2072 6563 6f6d 6d65 6e64 6564 2074 6861   recommended tha
-00022850: 7420 796f 7520 7265 7772 6974 6520 796f  t you rewrite yo
-00022860: 7572 2066 756e 6374 696f 6e20 746f 206d  ur function to m
-00022870: 6565 7420 6569 7468 6572 2074 6865 2063  eet either the c
-00022880: 7269 7465 7269 6120 6162 6f76 6520 666f  riteria above fo
-00022890: 7220 6072 6563 7572 7369 7665 5f69 7465  r `recursive_ite
-000228a0: 7261 746f 7260 2c20 6f72 2074 6865 2063  rator`, or the c
-000228b0: 6f72 7265 7370 6f6e 6469 6e67 2063 7269  orresponding cri
-000228c0: 7465 7269 6120 666f 7220 436f 636f 6e75  teria for Coconu
-000228d0: 7427 7320 5b74 6169 6c20 6361 6c6c 206f  t's [tail call o
-000228e0: 7074 696d 697a 6174 696f 6e5d 2823 7461  ptimization](#ta
-000228f0: 696c 2d63 616c 6c2d 6f70 7469 6d69 7a61  il-call-optimiza
-00022900: 7469 6f6e 292c 2065 6974 6865 7220 6f66  tion), either of
-00022910: 2077 6869 6368 2073 686f 756c 6420 7072   which should pr
-00022920: 6576 656e 7420 7375 6368 2065 7272 6f72  event such error
-00022930: 732e 0a0a 4675 7274 6865 726d 6f72 652c  s...Furthermore,
-00022940: 2060 7265 6375 7273 6976 655f 6974 6572   `recursive_iter
-00022950: 6174 6f72 6020 616c 736f 2061 6c6c 6f77  ator` also allow
-00022960: 7320 7468 6520 7265 736f 6c75 7469 6f6e  s the resolution
-00022970: 206f 6620 6120 5b6e 6173 7479 2073 6567   of a [nasty seg
-00022980: 6d65 6e74 6174 696f 6e20 6661 756c 7420  mentation fault 
-00022990: 696e 2050 7974 686f 6e27 7320 6974 6572  in Python's iter
-000229a0: 6174 6f72 206c 6f67 6963 2074 6861 7420  ator logic that 
-000229b0: 6861 7320 6e65 7665 7220 6265 656e 2066  has never been f
-000229c0: 6978 6564 5d28 6874 7470 3a2f 2f62 7567  ixed](http://bug
-000229d0: 732e 7079 7468 6f6e 2e6f 7267 2f69 7373  s.python.org/iss
-000229e0: 7565 3134 3031 3029 2e20 5370 6563 6966  ue14010). Specif
-000229f0: 6963 616c 6c79 2c20 696e 7374 6561 6420  ically, instead 
-00022a00: 6f66 2077 7269 7469 6e67 0a60 6060 636f  of writing.```co
-00022a10: 636f 6e75 740a 7365 7120 3d20 6765 745f  conut.seq = get_
-00022a20: 656c 656d 2829 203a 3a20 7365 710a 6060  elem() :: seq.``
-00022a30: 600a 7768 6963 6820 7769 6c6c 2063 7261  `.which will cra
-00022a40: 7368 2064 7565 2074 6f20 7468 6520 6166  sh due to the af
-00022a50: 6f72 656d 656e 7469 6f6e 6564 2050 7974  orementioned Pyt
-00022a60: 686f 6e20 6973 7375 652c 2077 7269 7465  hon issue, write
-00022a70: 0a60 6060 636f 636f 6e75 740a 4072 6563  .```coconut.@rec
-00022a80: 7572 7369 7665 5f69 7465 7261 746f 720a  ursive_iterator.
-00022a90: 6465 6620 7365 7128 2920 3d20 6765 745f  def seq() = get_
-00022aa0: 656c 656d 2829 203a 3a20 7365 7128 290a  elem() :: seq().
-00022ab0: 6060 600a 7768 6963 6820 7769 6c6c 2077  ```.which will w
-00022ac0: 6f72 6b20 6a75 7374 2066 696e 652e 0a0a  ork just fine...
-00022ad0: 4f6e 6520 7069 7466 616c 6c20 746f 206b  One pitfall to k
-00022ae0: 6565 7020 696e 206d 696e 6420 776f 726b  eep in mind work
-00022af0: 696e 6720 7769 7468 2060 7265 6375 7273  ing with `recurs
-00022b00: 6976 655f 6974 6572 6174 6f72 6020 6973  ive_iterator` is
-00022b10: 2074 6861 7420 6974 2073 686f 756c 646e   that it shouldn
-00022b20: 2774 2062 6520 7573 6564 2069 6e20 636f  't be used in co
-00022b30: 6e74 6578 7473 2077 6865 7265 2074 6865  ntexts where the
-00022b40: 2066 756e 6374 696f 6e20 6361 6e20 706f   function can po
-00022b50: 7465 6e74 6961 6c6c 7920 6265 2063 616c  tentially be cal
-00022b60: 6c65 6420 6d75 6c74 6970 6c65 2074 696d  led multiple tim
-00022b70: 6573 2077 6974 6820 7468 6520 7361 6d65  es with the same
-00022b80: 2069 7465 7261 746f 7220 6f62 6a65 6374   iterator object
-00022b90: 2061 7320 616e 2069 6e70 7574 2c20 6275   as an input, bu
-00022ba0: 7420 7769 7468 2074 6861 7420 6f62 6a65  t with that obje
-00022bb0: 6374 206e 6f74 2061 6374 7561 6c6c 7920  ct not actually 
-00022bc0: 636f 7272 6573 706f 6e64 696e 6720 746f  corresponding to
-00022bd0: 2074 6865 2073 616d 6520 6974 656d 7320   the same items 
-00022be0: 2865 2e67 2e20 6265 6361 7573 6520 7468  (e.g. because th
-00022bf0: 6520 6669 7273 7420 7469 6d65 2074 6865  e first time the
-00022c00: 206f 626a 6563 7420 6861 736e 2774 2062   object hasn't b
-00022c10: 6565 6e20 6974 6572 6174 6564 206f 7665  een iterated ove
-00022c20: 7220 7965 7420 616e 6420 7468 6520 7365  r yet and the se
-00022c30: 636f 6e64 2074 696d 6520 6974 2068 6173  cond time it has
-00022c40: 2062 6565 6e29 2e0a 0a23 2323 2323 2045   been)...##### E
-00022c50: 7861 6d70 6c65 0a0a 2a2a 436f 636f 6e75  xample..**Coconu
-00022c60: 743a 2a2a 0a60 6060 636f 636f 6e75 740a  t:**.```coconut.
-00022c70: 4072 6563 7572 7369 7665 5f69 7465 7261  @recursive_itera
-00022c80: 746f 720a 6465 6620 6669 6228 2920 3d20  tor.def fib() = 
-00022c90: 2831 2c20 3129 203a 3a20 6d61 7028 282b  (1, 1) :: map((+
-00022ca0: 292c 2066 6962 2829 2c20 6669 6228 2924  ), fib(), fib()$
-00022cb0: 5b31 3a5d 290a 6060 600a 0a2a 2a50 7974  [1:]).```..**Pyt
-00022cc0: 686f 6e3a 2a2a 0a5f 4361 6e27 7420 6265  hon:**._Can't be
-00022cd0: 2064 6f6e 6520 7769 7468 6f75 7420 6120   done without a 
-00022ce0: 6c6f 6e67 2064 6563 6f72 6174 6f72 2064  long decorator d
-00022cf0: 6566 696e 6974 696f 6e2e 2054 6865 2066  efinition. The f
-00022d00: 756c 6c20 6465 6669 6e69 7469 6f6e 206f  ull definition o
-00022d10: 6620 7468 6520 6465 636f 7261 746f 7220  f the decorator 
-00022d20: 696e 2050 7974 686f 6e20 6361 6e20 6265  in Python can be
-00022d30: 2066 6f75 6e64 2069 6e20 7468 6520 436f   found in the Co
-00022d40: 636f 6e75 7420 6865 6164 6572 2e5f 0a0a  conut header._..
-00022d50: 2323 2320 4275 696c 742d 496e 2054 7970  ### Built-In Typ
-00022d60: 6573 0a0a 6060 607b 636f 6e74 656e 7473  es..```{contents
-00022d70: 7d0a 2d2d 2d0a 6c6f 6361 6c3a 0a64 6570  }.---.local:.dep
-00022d80: 7468 3a20 310a 2d2d 2d0a 6060 600a 0a23  th: 1.---.```..#
-00022d90: 2323 2320 606d 756c 7469 7365 7460 0a0a  ### `multiset`..
-00022da0: 2a2a 6d75 6c74 6973 6574 2a2a 285f 6974  **multiset**(_it
-00022db0: 6572 6162 6c65 5f3d 604e 6f6e 6560 2c20  erable_=`None`, 
-00022dc0: 2f2c 202a 2a6b 7764 7329 0a0a 436f 636f  /, **kwds)..Coco
-00022dd0: 6e75 7420 7072 6f76 6964 6573 2060 6d75  nut provides `mu
-00022de0: 6c74 6973 6574 6020 6173 2061 2062 7569  ltiset` as a bui
-00022df0: 6c74 2d69 6e20 7375 6263 6c61 7373 206f  lt-in subclass o
-00022e00: 6620 5b60 636f 6c6c 6563 7469 6f6e 732e  f [`collections.
-00022e10: 436f 756e 7465 7260 5d28 6874 7470 733a  Counter`](https:
-00022e20: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
-00022e30: 672f 332f 6c69 6272 6172 792f 636f 6c6c  g/3/library/coll
-00022e40: 6563 7469 6f6e 732e 6874 6d6c 2363 6f6c  ections.html#col
-00022e50: 6c65 6374 696f 6e73 2e43 6f75 6e74 6572  lections.Counter
-00022e60: 2920 7468 6174 2061 6464 6974 696f 6e61  ) that additiona
-00022e70: 6c6c 7920 696d 706c 656d 656e 7473 2074  lly implements t
-00022e80: 6865 2066 756c 6c20 5b53 6574 2061 6e64  he full [Set and
-00022e90: 204d 7574 6162 6c65 5365 7420 696e 7465   MutableSet inte
-00022ea0: 7266 6163 6573 5d28 6874 7470 733a 2f2f  rfaces](https://
-00022eb0: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
-00022ec0: 332f 6c69 6272 6172 792f 636f 6c6c 6563  3/library/collec
-00022ed0: 7469 6f6e 732e 6162 632e 6874 6d6c 292e  tions.abc.html).
-00022ee0: 0a0a 466f 7220 6561 7369 6c79 2063 6f6e  ..For easily con
-00022ef0: 7374 7275 6374 696e 6720 6d75 6c74 6973  structing multis
-00022f00: 6574 732c 2043 6f63 6f6e 7574 2061 6c73  ets, Coconut als
-00022f10: 6f20 7072 6f76 6964 6573 205b 6d75 6c74  o provides [mult
-00022f20: 6973 6574 206c 6974 6572 616c 735d 2823  iset literals](#
-00022f30: 7365 742d 6c69 7465 7261 6c73 292e 0a0a  set-literals)...
-00022f40: 5468 6520 6e65 7720 6d65 7468 6f64 7320  The new methods 
-00022f50: 7072 6f76 6964 6564 2062 7920 606d 756c  provided by `mul
-00022f60: 7469 7365 7460 206f 6e20 746f 7020 6f66  tiset` on top of
-00022f70: 2060 636f 6c6c 6563 7469 6f6e 732e 436f   `collections.Co
-00022f80: 756e 7465 7260 2061 7265 3a0a 2d20 6d75  unter` are:.- mu
-00022f90: 6c74 6973 6574 2e2a 2a61 6464 2a2a 285f  ltiset.**add**(_
-00022fa0: 6974 656d 5f29 3a20 4164 6420 616e 2065  item_): Add an e
-00022fb0: 6c65 6d65 6e74 2074 6f20 6120 6d75 6c74  lement to a mult
-00022fc0: 6973 6574 2e0a 2d20 6d75 6c74 6973 6574  iset..- multiset
-00022fd0: 2e2a 2a64 6973 6361 7264 2a2a 285f 6974  .**discard**(_it
-00022fe0: 656d 5f29 3a20 5265 6d6f 7665 2061 6e20  em_): Remove an 
-00022ff0: 656c 656d 656e 7420 6672 6f6d 2061 206d  element from a m
-00023000: 756c 7469 7365 7420 6966 2069 7420 6973  ultiset if it is
-00023010: 2061 206d 656d 6265 722e 0a2d 206d 756c   a member..- mul
-00023020: 7469 7365 742e 2a2a 7265 6d6f 7665 2a2a  tiset.**remove**
-00023030: 285f 6974 656d 5f29 3a20 5265 6d6f 7665  (_item_): Remove
-00023040: 2061 6e20 656c 656d 656e 7420 6672 6f6d   an element from
-00023050: 2061 206d 756c 7469 7365 743b 2069 7420   a multiset; it 
-00023060: 6d75 7374 2062 6520 6120 6d65 6d62 6572  must be a member
-00023070: 2e0a 2d20 6d75 6c74 6973 6574 2e2a 2a69  ..- multiset.**i
-00023080: 7364 6973 6a6f 696e 742a 2a28 5f6f 7468  sdisjoint**(_oth
-00023090: 6572 5f29 3a20 5265 7475 726e 2054 7275  er_): Return Tru
-000230a0: 6520 6966 2074 776f 206d 756c 7469 7365  e if two multise
-000230b0: 7473 2068 6176 6520 6120 6e75 6c6c 2069  ts have a null i
-000230c0: 6e74 6572 7365 6374 696f 6e2e 0a2d 206d  ntersection..- m
-000230d0: 756c 7469 7365 742e 2a2a 5c5f 5c5f 786f  ultiset.**\_\_xo
-000230e0: 725c 5f5c 5f2a 2a28 5f6f 7468 6572 5f29  r\_\_**(_other_)
-000230f0: 3a20 5265 7475 726e 2074 6865 2073 796d  : Return the sym
-00023100: 6d65 7472 6963 2064 6966 6665 7265 6e63  metric differenc
-00023110: 6520 6f66 2074 776f 206d 756c 7469 7365  e of two multise
-00023120: 7473 2061 7320 6120 6e65 7720 6d75 6c74  ts as a new mult
-00023130: 6973 6574 2e20 5370 6563 6966 6963 616c  iset. Specifical
-00023140: 6c79 3a20 6061 205e 2062 203d 2028 6120  ly: `a ^ b = (a 
-00023150: 2d20 6229 207c 2028 6220 2d20 6129 600a  - b) | (b - a)`.
-00023160: 2d20 6d75 6c74 6973 6574 2e2a 2a63 6f75  - multiset.**cou
-00023170: 6e74 2a2a 285f 6974 656d 5f29 3a20 5265  nt**(_item_): Re
-00023180: 7475 726e 2074 6865 206e 756d 6265 7220  turn the number 
-00023190: 6f66 2074 696d 6573 2061 6e20 656c 656d  of times an elem
-000231a0: 656e 7420 6f63 6375 7273 2069 6e20 6120  ent occurs in a 
-000231b0: 6d75 6c74 6973 6574 2e20 4571 7569 7661  multiset. Equiva
-000231c0: 6c65 6e74 2074 6f20 606d 756c 7469 7365  lent to `multise
-000231d0: 745b 6974 656d 5d60 2c20 6275 7420 6164  t[item]`, but ad
-000231e0: 6469 7469 6f6e 616c 6c79 2076 6572 6966  ditionally verif
-000231f0: 6965 7320 7468 6520 636f 756e 7420 6973  ies the count is
-00023200: 206e 6f6e 2d6e 6567 6174 6976 652e 0a2d   non-negative..-
-00023210: 206d 756c 7469 7365 742e 2a2a 5c5f 5c5f   multiset.**\_\_
-00023220: 666d 6170 5c5f 5c5f 2a2a 285f 6675 6e63  fmap\_\_**(_func
-00023230: 5f29 3a20 4170 706c 7920 6120 6675 6e63  _): Apply a func
-00023240: 7469 6f6e 2074 6f20 7468 6520 636f 6e74  tion to the cont
-00023250: 656e 7473 206f 6620 7468 6520 6d75 6c74  ents of the mult
-00023260: 6973 6574 2c20 7072 6573 6572 7669 6e67  iset, preserving
-00023270: 2063 6f75 6e74 733b 206d 6167 6963 206d   counts; magic m
-00023280: 6574 686f 6420 666f 7220 5b60 666d 6170  ethod for [`fmap
-00023290: 605d 2823 666d 6170 292e 0a0a 436f 636f  `](#fmap)...Coco
-000232a0: 6e75 7420 616c 736f 2065 6e73 7572 6573  nut also ensures
-000232b0: 2074 6861 7420 606d 756c 7469 7365 7460   that `multiset`
-000232c0: 2073 7570 706f 7274 7320 5b72 6963 6820   supports [rich 
-000232d0: 636f 6d70 6172 6973 6f6e 7320 616e 6420  comparisons and 
-000232e0: 6043 6f75 6e74 6572 2e74 6f74 616c 2829  `Counter.total()
-000232f0: 605d 2868 7474 7073 3a2f 2f64 6f63 732e  `](https://docs.
-00023300: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
-00023310: 7261 7279 2f63 6f6c 6c65 6374 696f 6e73  rary/collections
-00023320: 2e68 746d 6c23 636f 6c6c 6563 7469 6f6e  .html#collection
-00023330: 732e 436f 756e 7465 7229 206f 6e20 616c  s.Counter) on al
-00023340: 6c20 5079 7468 6f6e 2076 6572 7369 6f6e  l Python version
-00023350: 732e 0a0a 2323 2323 2320 4578 616d 706c  s...##### Exampl
-00023360: 650a 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a  e..**Coconut:**.
-00023370: 6060 6063 6f63 6f6e 7574 0a6d 795f 6d75  ```coconut.my_mu
-00023380: 6c74 6973 6574 203d 206d 7b31 2c20 312c  ltiset = m{1, 1,
-00023390: 2032 7d0a 6d79 5f6d 756c 7469 7365 742e   2}.my_multiset.
-000233a0: 6164 6428 3329 0a6d 795f 6d75 6c74 6973  add(3).my_multis
-000233b0: 6574 2e72 656d 6f76 6528 3229 0a70 7269  et.remove(2).pri
-000233c0: 6e74 286d 795f 6d75 6c74 6973 6574 290a  nt(my_multiset).
-000233d0: 6060 600a 0a2a 2a50 7974 686f 6e3a 2a2a  ```..**Python:**
-000233e0: 0a60 6060 636f 636f 6e75 745f 7079 7468  .```coconut_pyth
-000233f0: 6f6e 0a66 726f 6d20 636f 6c6c 6563 7469  on.from collecti
-00023400: 6f6e 7320 696d 706f 7274 2043 6f75 6e74  ons import Count
-00023410: 6572 0a6d 795f 636f 756e 7465 7220 3d20  er.my_counter = 
-00023420: 436f 756e 7465 7228 2831 2c20 312c 2032  Counter((1, 1, 2
-00023430: 2929 0a6d 795f 636f 756e 7465 725b 335d  )).my_counter[3]
-00023440: 202b 3d20 310a 6d79 5f63 6f75 6e74 6572   += 1.my_counter
-00023450: 5b32 5d20 2d3d 2031 0a69 6620 6d79 5f63  [2] -= 1.if my_c
-00023460: 6f75 6e74 6572 5b32 5d20 3c3d 2030 3a0a  ounter[2] <= 0:.
-00023470: 2020 2020 6465 6c20 6d79 5f63 6f75 6e74      del my_count
-00023480: 6572 5b32 5d0a 7072 696e 7428 6d79 5f63  er[2].print(my_c
-00023490: 6f75 6e74 6572 290a 6060 600a 0a23 2323  ounter).```..###
-000234a0: 2320 6045 7870 6563 7465 6460 0a0a 2a2a  # `Expected`..**
-000234b0: 4578 7065 6374 6564 2a2a 285f 7265 7375  Expected**(_resu
-000234c0: 6c74 5f3d 604e 6f6e 6560 2c20 5f65 7272  lt_=`None`, _err
-000234d0: 6f72 5f3d 604e 6f6e 6560 290a 0a43 6f63  or_=`None`)..Coc
-000234e0: 6f6e 7574 2773 2060 4578 7065 6374 6564  onut's `Expected
-000234f0: 6020 6275 696c 742d 696e 2069 7320 6120  ` built-in is a 
-00023500: 436f 636f 6e75 7420 5b60 6461 7461 6020  Coconut [`data` 
-00023510: 7479 7065 5d28 2364 6174 6129 2074 6861  type](#data) tha
-00023520: 7420 7265 7072 6573 656e 7473 2061 2076  t represents a v
-00023530: 616c 7565 2074 6861 7420 6d61 7920 6f72  alue that may or
-00023540: 206d 6179 206e 6f74 2062 6520 616e 2065   may not be an e
-00023550: 7272 6f72 2c20 7369 6d69 6c61 7220 746f  rror, similar to
-00023560: 2048 6173 6b65 6c6c 2773 205b 6045 6974   Haskell's [`Eit
-00023570: 6865 7260 5d28 6874 7470 733a 2f2f 6861  her`](https://ha
-00023580: 636b 6167 652e 6861 736b 656c 6c2e 6f72  ckage.haskell.or
-00023590: 672f 7061 636b 6167 652f 6261 7365 2d34  g/package/base-4
-000235a0: 2e31 372e 302e 302f 646f 6373 2f44 6174  .17.0.0/docs/Dat
-000235b0: 612d 4569 7468 6572 2e68 746d 6c29 2e0a  a-Either.html)..
-000235c0: 0a60 4578 7065 6374 6564 6020 6973 2065  .`Expected` is e
-000235d0: 6666 6563 7469 7665 6c79 2065 7175 6976  ffectively equiv
-000235e0: 616c 656e 7420 746f 2074 6865 2066 6f6c  alent to the fol
-000235f0: 6c6f 7769 6e67 3a0a 6060 6063 6f63 6f6e  lowing:.```cocon
-00023600: 7574 0a64 6174 6120 4578 7065 6374 6564  ut.data Expected
-00023610: 5b54 5d28 7265 7375 6c74 3a20 543f 203d  [T](result: T? =
-00023620: 204e 6f6e 652c 2065 7272 6f72 3a20 4261   None, error: Ba
-00023630: 7365 4578 6365 7074 696f 6e3f 203d 204e  seException? = N
-00023640: 6f6e 6529 3a0a 2020 2020 6465 6620 5f5f  one):.    def __
-00023650: 626f 6f6c 5f5f 2873 656c 6629 202d 3e20  bool__(self) -> 
-00023660: 626f 6f6c 3a0a 2020 2020 2020 2020 7265  bool:.        re
-00023670: 7475 726e 2073 656c 662e 6572 726f 7220  turn self.error 
-00023680: 6973 204e 6f6e 650a 2020 2020 6465 6620  is None.    def 
-00023690: 5f5f 666d 6170 5f5f 5b55 5d28 7365 6c66  __fmap__[U](self
-000236a0: 2c20 6675 6e63 3a20 5420 2d3e 2055 2920  , func: T -> U) 
-000236b0: 2d3e 2045 7870 6563 7465 645b 555d 3a0a  -> Expected[U]:.
-000236c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000236d0: 656c 662e 5f5f 636c 6173 735f 5f28 6675  elf.__class__(fu
-000236e0: 6e63 2873 656c 662e 7265 7375 6c74 2929  nc(self.result))
-000236f0: 2069 6620 7365 6c66 2065 6c73 6520 7365   if self else se
-00023700: 6c66 0a20 2020 2064 6566 2061 6e64 5f74  lf.    def and_t
-00023710: 6865 6e5b 555d 2873 656c 662c 2066 756e  hen[U](self, fun
-00023720: 633a 2054 202d 3e20 4578 7065 6374 6564  c: T -> Expected
-00023730: 5b55 5d29 202d 3e20 4578 7065 6374 6564  [U]) -> Expected
-00023740: 5b55 5d3a 0a20 2020 2020 2020 2022 2222  [U]:.        """
-00023750: 4d61 7073 2061 2054 202d 3e20 4578 7065  Maps a T -> Expe
-00023760: 6374 6564 5b55 5d20 6f76 6572 2061 6e20  cted[U] over an 
-00023770: 4578 7065 6374 6564 5b54 5d20 746f 2070  Expected[T] to p
-00023780: 726f 6475 6365 2061 6e20 4578 7065 6374  roduce an Expect
-00023790: 6564 5b55 5d2e 0a20 2020 2020 2020 2049  ed[U]..        I
-000237a0: 6d70 6c65 6d65 6e74 7320 6120 6d6f 6e61  mplements a mona
-000237b0: 6469 6320 6269 6e64 2e20 4571 7569 7661  dic bind. Equiva
-000237c0: 6c65 6e74 2074 6f20 666d 6170 202e 2e3e  lent to fmap ..>
-000237d0: 202e 6a6f 696e 2829 2e22 2222 0a20 2020   .join().""".   
-000237e0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000237f0: 207c 3e20 666d 6170 2428 6675 6e63 2920   |> fmap$(func) 
-00023800: 7c3e 202e 6a6f 696e 2829 0a20 2020 2064  |> .join().    d
-00023810: 6566 206a 6f69 6e28 7365 6c66 3a20 4578  ef join(self: Ex
-00023820: 7065 6374 6564 5b45 7870 6563 7465 645b  pected[Expected[
-00023830: 545d 5d29 202d 3e20 4578 7065 6374 6564  T]]) -> Expected
-00023840: 5b54 5d3a 0a20 2020 2020 2020 2022 2222  [T]:.        """
-00023850: 4d6f 6e61 6469 6320 6a6f 696e 2e20 436f  Monadic join. Co
-00023860: 6e76 6572 7473 2045 7870 6563 7465 645b  nverts Expected[
-00023870: 4578 7065 6374 6564 5b54 5d5d 2074 6f20  Expected[T]] to 
-00023880: 4578 7065 6374 6564 5b54 5d2e 2222 220a  Expected[T].""".
-00023890: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-000238a0: 656c 663a 0a20 2020 2020 2020 2020 2020  elf:.           
-000238b0: 2072 6574 7572 6e20 7365 6c66 0a20 2020   return self.   
-000238c0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-000238d0: 2e72 6573 756c 7420 6069 7369 6e73 7461  .result `isinsta
-000238e0: 6e63 6560 2045 7870 6563 7465 643a 0a20  nce` Expected:. 
-000238f0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00023900: 2054 7970 6545 7272 6f72 2822 4578 7065   TypeError("Expe
-00023910: 6374 6564 2e6a 6f69 6e28 2920 7265 7175  cted.join() requ
-00023920: 6972 6573 2061 6e20 4578 7065 6374 6564  ires an Expected
-00023930: 5b45 7870 6563 7465 645b 5f5d 5d22 290a  [Expected[_]]").
-00023940: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00023950: 656c 662e 7265 7375 6c74 0a20 2020 2064  elf.result.    d
-00023960: 6566 206d 6170 5f65 7272 6f72 2873 656c  ef map_error(sel
-00023970: 662c 2066 756e 633a 2042 6173 6545 7863  f, func: BaseExc
-00023980: 6570 7469 6f6e 202d 3e20 4261 7365 4578  eption -> BaseEx
-00023990: 6365 7074 696f 6e29 202d 3e20 4578 7065  ception) -> Expe
-000239a0: 6374 6564 5b54 5d3a 0a20 2020 2020 2020  cted[T]:.       
-000239b0: 2022 2222 4d61 7073 2066 756e 6320 6f76   """Maps func ov
-000239c0: 6572 2074 6865 2065 7272 6f72 2069 6620  er the error if 
-000239d0: 6974 2065 7869 7374 732e 2222 220a 2020  it exists.""".  
-000239e0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000239f0: 6620 6966 2073 656c 6620 656c 7365 2073  f if self else s
-00023a00: 656c 662e 5f5f 636c 6173 735f 5f28 6572  elf.__class__(er
-00023a10: 726f 723d 6675 6e63 2873 656c 662e 6572  ror=func(self.er
-00023a20: 726f 7229 290a 2020 2020 6465 6620 6f72  ror)).    def or
-00023a30: 5f65 6c73 655b 555d 2873 656c 662c 2066  _else[U](self, f
-00023a40: 756e 633a 2042 6173 6545 7863 6570 7469  unc: BaseExcepti
-00023a50: 6f6e 202d 3e20 4578 7065 6374 6564 5b55  on -> Expected[U
-00023a60: 5d29 202d 3e20 4578 7065 6374 6564 5b54  ]) -> Expected[T
-00023a70: 207c 2055 5d3a 0a20 2020 2020 2020 2022   | U]:.        "
-00023a80: 2222 5265 7475 726e 2073 656c 6620 6966  ""Return self if
-00023a90: 206e 6f20 6572 726f 722c 206f 7468 6572   no error, other
-00023aa0: 7769 7365 2072 6574 7572 6e20 7468 6520  wise return the 
-00023ab0: 7265 7375 6c74 206f 6620 6576 616c 7561  result of evalua
-00023ac0: 7469 6e67 2066 756e 6320 6f6e 2074 6865  ting func on the
-00023ad0: 2065 7272 6f72 2e22 2222 0a20 2020 2020   error.""".     
-00023ae0: 2020 2072 6574 7572 6e20 7365 6c66 2069     return self i
-00023af0: 6620 7365 6c66 2065 6c73 6520 6675 6e63  f self else func
-00023b00: 2873 656c 662e 6572 726f 7229 0a20 2020  (self.error).   
-00023b10: 2064 6566 2072 6573 756c 745f 6f72 5b55   def result_or[U
-00023b20: 5d28 7365 6c66 2c20 6465 6661 756c 743a  ](self, default:
-00023b30: 2055 2920 2d3e 2054 207c 2055 3a0a 2020   U) -> T | U:.  
-00023b40: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
-00023b50: 7468 6520 7265 7375 6c74 2069 6620 6974  the result if it
-00023b60: 2065 7869 7374 732c 206f 7468 6572 7769   exists, otherwi
-00023b70: 7365 2072 6574 7572 6e20 7468 6520 6465  se return the de
-00023b80: 6661 756c 742e 2222 220a 2020 2020 2020  fault.""".      
-00023b90: 2020 7265 7475 726e 2073 656c 662e 7265    return self.re
-00023ba0: 7375 6c74 2069 6620 7365 6c66 2065 6c73  sult if self els
-00023bb0: 6520 6465 6661 756c 740a 2020 2020 6465  e default.    de
-00023bc0: 6620 7265 7375 6c74 5f6f 725f 656c 7365  f result_or_else
-00023bd0: 5b55 5d28 7365 6c66 2c20 6675 6e63 3a20  [U](self, func: 
-00023be0: 4261 7365 4578 6365 7074 696f 6e20 2d3e  BaseException ->
-00023bf0: 2055 2920 2d3e 2054 207c 2055 3a0a 2020   U) -> T | U:.  
-00023c00: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
-00023c10: 7468 6520 7265 7375 6c74 2069 6620 6974  the result if it
-00023c20: 2065 7869 7374 732c 206f 7468 6572 7769   exists, otherwi
-00023c30: 7365 2072 6574 7572 6e20 7468 6520 7265  se return the re
-00023c40: 7375 6c74 206f 6620 6576 616c 7561 7469  sult of evaluati
-00023c50: 6e67 2066 756e 6320 6f6e 2074 6865 2065  ng func on the e
-00023c60: 7272 6f72 2e22 2222 0a20 2020 2020 2020  rror.""".       
-00023c70: 2072 6574 7572 6e20 7365 6c66 2e72 6573   return self.res
-00023c80: 756c 7420 6966 2073 656c 6620 656c 7365  ult if self else
-00023c90: 2066 756e 6328 7365 6c66 2e65 7272 6f72   func(self.error
-00023ca0: 290a 2020 2020 6465 6620 756e 7772 6170  ).    def unwrap
-00023cb0: 2873 656c 6629 202d 3e20 543a 0a20 2020  (self) -> T:.   
-00023cc0: 2020 2020 2022 2222 556e 7772 6170 2074       """Unwrap t
-00023cd0: 6865 2072 6573 756c 7420 6f72 2072 6169  he result or rai
-00023ce0: 7365 2074 6865 2065 7272 6f72 2e22 2222  se the error."""
-00023cf0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00023d00: 7365 6c66 3a0a 2020 2020 2020 2020 2020  self:.          
-00023d10: 2020 7261 6973 6520 7365 6c66 2e65 7272    raise self.err
-00023d20: 6f72 0a20 2020 2020 2020 2072 6574 7572  or.        retur
-00023d30: 6e20 7365 6c66 2e72 6573 756c 740a 6060  n self.result.``
-00023d40: 600a 0a60 4578 7065 6374 6564 6020 6973  `..`Expected` is
-00023d50: 2070 7269 6d61 7269 6c79 2075 7365 6420   primarily used 
-00023d60: 6173 2074 6865 2072 6574 7572 6e20 7479  as the return ty
-00023d70: 7065 2066 6f72 205b 6073 6166 655f 6361  pe for [`safe_ca
-00023d80: 6c6c 605d 2823 7361 6665 5f63 616c 6c29  ll`](#safe_call)
-00023d90: 2e20 4765 6e65 7261 6c6c 792c 2074 6865  . Generally, the
-00023da0: 2062 6573 7420 7761 7920 746f 2075 7365   best way to use
-00023db0: 2060 4578 7065 6374 6564 6020 6973 2077   `Expected` is w
-00023dc0: 6974 6820 5b60 666d 6170 605d 2823 666d  ith [`fmap`](#fm
-00023dd0: 6170 292c 2077 6869 6368 2077 696c 6c20  ap), which will 
-00023de0: 6170 706c 7920 6120 6675 6e63 7469 6f6e  apply a function
-00023df0: 2074 6f20 7468 6520 7265 7375 6c74 2069   to the result i
-00023e00: 6620 6974 2065 7869 7374 732c 206f 7220  f it exists, or 
-00023e10: 6f74 6865 7277 6973 6520 7265 7461 696e  otherwise retain
-00023e20: 2074 6865 2065 7272 6f72 2e20 4966 2079   the error. If y
-00023e30: 6f75 2077 616e 7420 746f 2073 6571 7565  ou want to seque
-00023e40: 6e63 6520 6d75 6c74 6970 6c65 2060 4578  nce multiple `Ex
-00023e50: 7065 6374 6564 602d 7265 7475 726e 696e  pected`-returnin
-00023e60: 6720 6f70 6572 6174 696f 6e73 2c20 602e  g operations, `.
-00023e70: 616e 645f 7468 656e 6020 7368 6f75 6c64  and_then` should
-00023e80: 2062 6520 7573 6564 2069 6e73 7465 6164   be used instead
-00023e90: 206f 6620 6066 6d61 7060 2e0a 0a54 6f20   of `fmap`...To 
-00023ea0: 6d61 7463 6820 6167 6169 6e73 7420 616e  match against an
-00023eb0: 2060 4578 7065 6374 6564 602c 206a 7573   `Expected`, jus
-00023ec0: 743a 0a60 6060 0a45 7870 6563 7465 6428  t:.```.Expected(
-00023ed0: 7265 7329 203d 2045 7870 6563 7465 6428  res) = Expected(
-00023ee0: 2272 6573 756c 7422 290a 4578 7065 6374  "result").Expect
-00023ef0: 6564 2865 7272 6f72 3d65 7272 2920 3d20  ed(error=err) = 
-00023f00: 4578 7065 6374 6564 2865 7272 6f72 3d54  Expected(error=T
-00023f10: 7970 6545 7272 6f72 2829 290a 6060 600a  ypeError()).```.
-00023f20: 0a23 2323 2323 2045 7861 6d70 6c65 0a0a  .##### Example..
-00023f30: 2a2a 436f 636f 6e75 743a 2a2a 0a60 6060  **Coconut:**.```
-00023f40: 636f 636f 6e75 740a 6465 6620 7472 795f  coconut.def try_
-00023f50: 6469 7669 6465 2878 3a20 666c 6f61 742c  divide(x: float,
-00023f60: 2079 3a20 666c 6f61 7429 202d 3e20 4578   y: float) -> Ex
-00023f70: 7065 6374 6564 5b66 6c6f 6174 5d3a 0a20  pected[float]:. 
-00023f80: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00023f90: 7265 7475 726e 2045 7870 6563 7465 6428  return Expected(
-00023fa0: 7820 2f20 7929 0a20 2020 2065 7863 6570  x / y).    excep
-00023fb0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00023fc0: 7272 3a0a 2020 2020 2020 2020 7265 7475  rr:.        retu
-00023fd0: 726e 2045 7870 6563 7465 6428 6572 726f  rn Expected(erro
-00023fe0: 723d 6572 7229 0a0a 7472 795f 6469 7669  r=err)..try_divi
-00023ff0: 6465 2831 2c20 3229 207c 3e20 666d 6170  de(1, 2) |> fmap
-00024000: 2428 2e2b 3129 207c 3e20 7072 696e 740a  $(.+1) |> print.
-00024010: 7472 795f 6469 7669 6465 2831 2c20 3029  try_divide(1, 0)
-00024020: 207c 3e20 666d 6170 2428 2e2b 3129 207c   |> fmap$(.+1) |
-00024030: 3e20 7072 696e 740a 6060 600a 0a2a 2a50  > print.```..**P
-00024040: 7974 686f 6e3a 2a2a 0a5f 4361 6e27 7420  ython:**._Can't 
-00024050: 6265 2064 6f6e 6520 7769 7468 6f75 7420  be done without 
-00024060: 6120 636f 6d70 6c65 7820 6045 7870 6563  a complex `Expec
-00024070: 7465 6460 2064 6566 696e 6974 696f 6e2e  ted` definition.
-00024080: 2053 6565 2074 6865 2063 6f6d 7069 6c65   See the compile
-00024090: 6420 636f 6465 2066 6f72 2074 6865 2050  d code for the P
-000240a0: 7974 686f 6e20 7379 6e74 6178 2e5f 0a0a  ython syntax._..
-000240b0: 2323 2323 2060 4d61 7463 6845 7272 6f72  #### `MatchError
-000240c0: 600a 0a41 2060 4d61 7463 6845 7272 6f72  `..A `MatchError
-000240d0: 6020 6973 2072 6169 7365 6420 7768 656e  ` is raised when
-000240e0: 2061 205b 6465 7374 7275 6374 7572 696e   a [destructurin
-000240f0: 6720 6173 7369 676e 6d65 6e74 5d28 2364  g assignment](#d
-00024100: 6573 7472 7563 7475 7269 6e67 2d61 7373  estructuring-ass
-00024110: 6967 6e6d 656e 7429 206f 7220 5b70 6174  ignment) or [pat
-00024120: 7465 726e 2d6d 6174 6368 696e 6720 6675  tern-matching fu
-00024130: 6e63 7469 6f6e 5d28 2370 6174 7465 726e  nction](#pattern
-00024140: 2d6d 6174 6368 696e 672d 6675 6e63 7469  -matching-functi
-00024150: 6f6e 7329 2066 6169 6c73 2c20 616e 6420  ons) fails, and 
-00024160: 7468 7573 2060 4d61 7463 6845 7272 6f72  thus `MatchError
-00024170: 6020 6973 2070 726f 7669 6465 6420 6173  ` is provided as
-00024180: 2061 2062 7569 6c74 2d69 6e20 666f 7220   a built-in for 
-00024190: 6361 7463 6869 6e67 2074 686f 7365 2065  catching those e
-000241a0: 7272 6f72 732e 2060 4d61 7463 6845 7272  rrors. `MatchErr
-000241b0: 6f72 6020 6f62 6a65 6374 7320 7375 7070  or` objects supp
-000241c0: 6f72 7420 7468 7265 6520 6174 7472 6962  ort three attrib
-000241d0: 7574 6573 3a20 6070 6174 7465 726e 602c  utes: `pattern`,
-000241e0: 2077 6869 6368 2069 7320 6120 7374 7269   which is a stri
-000241f0: 6e67 2064 6573 6372 6962 696e 6720 7468  ng describing th
-00024200: 6520 6661 696c 6564 2070 6174 7465 726e  e failed pattern
-00024210: 3b20 6076 616c 7565 602c 2077 6869 6368  ; `value`, which
-00024220: 2069 7320 7468 6520 6f62 6a65 6374 2074   is the object t
-00024230: 6861 7420 6661 696c 6564 2074 6f20 6d61  hat failed to ma
-00024240: 7463 6820 7468 6174 2070 6174 7465 726e  tch that pattern
-00024250: 3b20 616e 6420 606d 6573 7361 6765 6020  ; and `message` 
-00024260: 7768 6963 6820 6973 2074 6865 2066 756c  which is the ful
-00024270: 6c20 6572 726f 7220 6d65 7373 6167 652e  l error message.
-00024280: 2054 6f20 6176 6f69 6420 756e 6e65 6365   To avoid unnece
-00024290: 7373 6172 7920 6072 6570 7260 2063 616c  ssary `repr` cal
-000242a0: 6c73 2c20 604d 6174 6368 4572 726f 7260  ls, `MatchError`
-000242b0: 206f 6e6c 7920 636f 6d70 7574 6573 2074   only computes t
-000242c0: 6865 2060 6d65 7373 6167 6560 206f 6e63  he `message` onc
-000242d0: 6520 6974 2069 7320 6163 7475 616c 6c79  e it is actually
-000242e0: 2072 6571 7565 7374 6564 2e0a 0a41 6464   requested...Add
-000242f0: 6974 696f 6e61 6c6c 792c 2069 6620 796f  itionally, if yo
-00024300: 7520 6172 6520 7573 696e 6720 5b76 6965  u are using [vie
-00024310: 7720 7061 7474 6572 6e73 5d28 236d 6174  w patterns](#mat
-00024320: 6368 292c 2079 6f75 206d 6967 6874 206e  ch), you might n
-00024330: 6565 6420 746f 2072 6169 7365 2079 6f75  eed to raise you
-00024340: 7220 6f77 6e20 604d 6174 6368 4572 726f  r own `MatchErro
-00024350: 7260 2028 7468 6f75 6768 2079 6f75 2063  r` (though you c
-00024360: 616e 2061 6c73 6f20 6a75 7374 2075 7365  an also just use
-00024370: 2061 2064 6573 7472 7563 7475 7269 6e67   a destructuring
-00024380: 2061 7373 6967 6e6d 656e 7420 6f72 2070   assignment or p
-00024390: 6174 7465 726e 2d6d 6174 6368 696e 6720  attern-matching 
-000243a0: 6675 6e63 7469 6f6e 2064 6566 696e 6974  function definit
-000243b0: 696f 6e20 746f 2064 6f20 736f 292e 2054  ion to do so). T
-000243c0: 6f20 7261 6973 6520 796f 7572 206f 776e  o raise your own
-000243d0: 2060 4d61 7463 6845 7272 6f72 602c 206a   `MatchError`, j
-000243e0: 7573 7420 6072 6169 7365 204d 6174 6368  ust `raise Match
-000243f0: 4572 726f 7228 7061 7474 6572 6e2c 2076  Error(pattern, v
-00024400: 616c 7565 2960 2028 626f 7468 2061 7267  alue)` (both arg
-00024410: 756d 656e 7473 2061 7265 206f 7074 696f  uments are optio
-00024420: 6e61 6c29 2e0a 0a49 6e20 736f 6d65 2063  nal)...In some c
-00024430: 6173 6573 2077 6865 7265 2074 6865 7265  ases where there
-00024440: 2061 7265 206d 756c 7469 706c 6520 436f   are multiple Co
-00024450: 636f 6e75 7420 7061 636b 6167 6573 2069  conut packages i
-00024460: 6e73 7461 6c6c 6564 2061 7420 7468 6520  nstalled at the 
-00024470: 7361 6d65 2074 696d 652c 2074 6865 7265  same time, there
-00024480: 206d 6179 2062 6520 6d75 6c74 6970 6c65   may be multiple
-00024490: 2060 4d61 7463 6845 7272 6f72 6073 2064   `MatchError`s d
-000244a0: 6566 696e 6564 2069 6e20 6469 6666 6572  efined in differ
-000244b0: 656e 7420 7061 636b 6167 6573 2e20 436f  ent packages. Co
-000244c0: 636f 6e75 7420 6361 6e20 7065 7266 6f72  conut can perfor
-000244d0: 6d20 736f 6d65 206d 6167 6963 2075 6e64  m some magic und
-000244e0: 6572 2074 6865 2068 6f6f 6420 746f 206d  er the hood to m
-000244f0: 616b 6520 7375 7265 2074 6861 7420 616c  ake sure that al
-00024500: 6c20 7468 6573 6520 604d 6174 6368 4572  l these `MatchEr
-00024510: 726f 7260 7320 7769 6c6c 2073 6561 6d6c  ror`s will seaml
-00024520: 6573 736c 7920 696e 7465 726f 7065 7261  essly interopera
-00024530: 7465 2c20 6275 7420 6f6e 6c79 2069 6620  te, but only if 
-00024540: 616c 6c20 7375 6368 2070 6163 6b61 6765  all such package
-00024550: 7320 6172 6520 636f 6d70 696c 6564 2069  s are compiled i
-00024560: 6e20 5b60 2d2d 7061 636b 6167 6560 206d  n [`--package` m
-00024570: 6f64 6520 7261 7468 6572 2074 6861 6e20  ode rather than 
-00024580: 602d 2d73 7461 6e64 616c 6f6e 6560 206d  `--standalone` m
-00024590: 6f64 655d 2823 636f 6d70 696c 6174 696f  ode](#compilatio
-000245a0: 6e2d 6d6f 6465 7329 2e0a 0a23 2323 2047  n-modes)...### G
-000245b0: 656e 6572 6963 2042 7569 6c74 2d49 6e20  eneric Built-In 
-000245c0: 4675 6e63 7469 6f6e 730a 0a60 6060 7b63  Functions..```{c
-000245d0: 6f6e 7465 6e74 737d 0a2d 2d2d 0a6c 6f63  ontents}.---.loc
-000245e0: 616c 3a0a 6465 7074 683a 2031 0a2d 2d2d  al:.depth: 1.---
-000245f0: 0a60 6060 0a0a 2323 2323 2060 6d61 6b65  .```..#### `make
-00024600: 6461 7461 600a 0a2a 2a6d 616b 6564 6174  data`..**makedat
-00024610: 612a 2a28 5f64 6174 615c 5f74 7970 655f  a**(_data\_type_
-00024620: 2c20 2a5f 6172 6773 5f29 0a0a 436f 636f  , *_args_)..Coco
-00024630: 6e75 7420 7072 6f76 6964 6573 2074 6865  nut provides the
-00024640: 2060 6d61 6b65 6461 7461 6020 6675 6e63   `makedata` func
-00024650: 7469 6f6e 2074 6f20 636f 6e73 7472 7563  tion to construc
-00024660: 7420 6120 636f 6e74 6169 6e65 7220 6769  t a container gi
-00024670: 7665 6e20 7468 6520 6465 7369 7265 6420  ven the desired 
-00024680: 7479 7065 2061 6e64 2063 6f6e 7465 6e74  type and content
-00024690: 732e 2054 6869 7320 6973 2070 6172 7469  s. This is parti
-000246a0: 6375 6c61 726c 7920 7573 6566 756c 2077  cularly useful w
-000246b0: 6865 6e20 7772 6974 696e 6720 616c 7465  hen writing alte
-000246c0: 726e 6174 6976 6520 636f 6e73 7472 7563  rnative construc
-000246d0: 746f 7273 2066 6f72 205b 6064 6174 6160  tors for [`data`
-000246e0: 5d28 2364 6174 6129 2074 7970 6573 2062  ](#data) types b
-000246f0: 7920 6f76 6572 7772 6974 696e 6720 605f  y overwriting `_
-00024700: 5f6e 6577 5f5f 602c 2073 696e 6365 2069  _new__`, since i
-00024710: 7420 616c 6c6f 7773 2064 6972 6563 7420  t allows direct 
-00024720: 6163 6365 7373 2074 6f20 7468 6520 6261  access to the ba
-00024730: 7365 2063 6f6e 7374 7275 6374 6f72 206f  se constructor o
-00024740: 6620 7468 6520 6461 7461 2074 7970 6520  f the data type 
-00024750: 6372 6561 7465 6420 7769 7468 2074 6865  created with the
-00024760: 2043 6f63 6f6e 7574 2060 6461 7461 6020   Coconut `data` 
-00024770: 7374 6174 656d 656e 742e 0a0a 606d 616b  statement...`mak
-00024780: 6564 6174 6160 2074 616b 6573 2074 6865  edata` takes the
-00024790: 2064 6174 6120 7479 7065 2074 6f20 636f   data type to co
-000247a0: 6e73 7472 7563 7420 6173 2074 6865 2066  nstruct as the f
-000247b0: 6972 7374 2061 7267 756d 656e 742c 2061  irst argument, a
-000247c0: 6e64 2074 6865 206f 626a 6563 7473 2074  nd the objects t
-000247d0: 6f20 7075 7420 696e 2074 6861 7420 636f  o put in that co
-000247e0: 6e74 6169 6e65 7220 6173 2074 6865 2072  ntainer as the r
-000247f0: 6573 7420 6f66 2074 6865 2061 7267 756d  est of the argum
-00024800: 656e 7473 2e0a 0a60 6d61 6b65 6461 7461  ents...`makedata
-00024810: 6020 6361 6e20 616c 736f 2062 6520 7573  ` can also be us
-00024820: 6564 2074 6f20 6578 7472 6163 7420 7468  ed to extract th
-00024830: 6520 756e 6465 726c 7969 6e67 2063 6f6e  e underlying con
-00024840: 7374 7275 6374 6f72 2066 6f72 205b 606d  structor for [`m
-00024850: 6174 6368 2064 6174 6160 5d28 236d 6174  atch data`](#mat
-00024860: 6368 2d64 6174 6129 2074 7970 6573 2074  ch-data) types t
-00024870: 6861 7420 6279 7061 7373 6573 2074 6865  hat bypasses the
-00024880: 206e 6f72 6d61 6c20 7061 7474 6572 6e2d   normal pattern-
-00024890: 6d61 7463 6869 6e67 2063 6f6e 7374 7275  matching constru
-000248a0: 6374 6f72 2e0a 0a41 6464 6974 696f 6e61  ctor...Additiona
-000248b0: 6c6c 792c 2060 6d61 6b65 6461 7461 6020  lly, `makedata` 
-000248c0: 6361 6e20 616c 736f 2062 6520 6361 6c6c  can also be call
-000248d0: 6564 2077 6974 6820 6e6f 6e2d 6064 6174  ed with non-`dat
-000248e0: 6160 2074 7970 6520 6173 2074 6865 2066  a` type as the f
-000248f0: 6972 7374 2061 7267 756d 656e 742c 2069  irst argument, i
-00024900: 6e20 7768 6963 6820 6361 7365 2069 7420  n which case it 
-00024910: 7769 6c6c 2064 6f20 6974 7320 6265 7374  will do its best
-00024920: 2074 6f20 636f 6e73 7472 7563 7420 7468   to construct th
-00024930: 6520 6769 7665 6e20 7479 7065 206f 6620  e given type of 
-00024940: 6f62 6a65 6374 2077 6974 6820 7468 6520  object with the 
-00024950: 6769 7665 6e20 6172 6775 6d65 6e74 732e  given arguments.
-00024960: 2054 6869 7320 6675 6e63 7469 6f6e 616c   This functional
-00024970: 6974 7920 6973 2075 7365 6420 696e 7465  ity is used inte
-00024980: 726e 616c 6c79 2062 7920 6066 6d61 7060  rnally by `fmap`
-00024990: 2e0a 0a23 2323 2323 2060 6461 7461 6d61  ...##### `datama
-000249a0: 6b65 7260 0a0a 2a2a 4445 5052 4543 4154  ker`..**DEPRECAT
-000249b0: 4544 3a2a 2a20 436f 636f 6e75 7420 616c  ED:** Coconut al
-000249c0: 736f 2068 6173 2061 2060 6461 7461 6d61  so has a `datama
-000249d0: 6b65 7260 2062 7569 6c74 2d69 6e2c 2077  ker` built-in, w
-000249e0: 6869 6368 2070 6172 7469 616c 6c79 2061  hich partially a
-000249f0: 7070 6c69 6573 2060 6d61 6b65 6461 7461  pplies `makedata
-00024a00: 603b 2060 6461 7461 6d61 6b65 7260 2069  `; `datamaker` i
-00024a10: 7320 6465 6669 6e65 6420 6173 3a0a 6060  s defined as:.``
-00024a20: 6063 6f63 6f6e 7574 0a64 6566 2064 6174  `coconut.def dat
-00024a30: 616d 616b 6572 2864 6174 615f 7479 7065  amaker(data_type
-00024a40: 293a 0a20 2020 2022 2222 4765 7420 7468  ):.    """Get th
-00024a50: 6520 6f72 6967 696e 616c 2063 6f6e 7374  e original const
-00024a60: 7275 6374 6f72 206f 6620 7468 6520 6769  ructor of the gi
-00024a70: 7665 6e20 6461 7461 2074 7970 6520 6f72  ven data type or
-00024a80: 2063 6c61 7373 2e22 2222 0a20 2020 2072   class.""".    r
-00024a90: 6574 7572 6e20 6d61 6b65 6461 7461 2428  eturn makedata$(
-00024aa0: 6461 7461 5f74 7970 6529 0a60 6060 0a5f  data_type).```._
-00024ab0: 4e6f 7465 3a20 5061 7373 696e 6720 602d  Note: Passing `-
-00024ac0: 2d73 7472 6963 7460 2064 6973 6162 6c65  -strict` disable
-00024ad0: 7320 6465 7072 6563 6174 6564 2066 6561  s deprecated fea
-00024ae0: 7475 7265 732e 5f0a 0a23 2323 2323 2045  tures._..##### E
-00024af0: 7861 6d70 6c65 0a0a 2a2a 436f 636f 6e75  xample..**Coconu
-00024b00: 743a 2a2a 0a60 6060 636f 636f 6e75 740a  t:**.```coconut.
-00024b10: 6461 7461 2054 7570 6c65 2865 6c65 6d73  data Tuple(elems
-00024b20: 293a 0a20 2020 2064 6566 205f 5f6e 6577  ):.    def __new
-00024b30: 5f5f 2863 6c73 2c20 2a65 6c65 6d73 293a  __(cls, *elems):
-00024b40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00024b50: 656c 656d 7320 7c3e 206d 616b 6564 6174  elems |> makedat
-00024b60: 6124 2863 6c73 290a 6060 600a 0a2a 2a50  a$(cls).```..**P
-00024b70: 7974 686f 6e3a 2a2a 0a5f 4361 6e27 7420  ython:**._Can't 
-00024b80: 6265 2064 6f6e 6520 7769 7468 6f75 7420  be done without 
-00024b90: 6120 7365 7269 6573 206f 6620 6d65 7468  a series of meth
-00024ba0: 6f64 2064 6566 696e 6974 696f 6e73 2066  od definitions f
-00024bb0: 6f72 2065 6163 6820 6461 7461 2074 7970  or each data typ
-00024bc0: 652e 2053 6565 2074 6865 2063 6f6d 7069  e. See the compi
-00024bd0: 6c65 6420 636f 6465 2066 6f72 2074 6865  led code for the
-00024be0: 2050 7974 686f 6e20 7379 6e74 6178 2e5f   Python syntax._
-00024bf0: 0a0a 2323 2323 2060 666d 6170 600a 0a2a  ..#### `fmap`..*
-00024c00: 2a66 6d61 702a 2a28 5f66 756e 635f 2c20  *fmap**(_func_, 
-00024c10: 5f6f 626a 5f29 0a0a 496e 2048 6173 6b65  _obj_)..In Haske
-00024c20: 6c6c 2c20 6066 6d61 7028 6675 6e63 2c20  ll, `fmap(func, 
-00024c30: 6f62 6a29 6020 7461 6b65 7320 6120 6461  obj)` takes a da
-00024c40: 7461 2074 7970 6520 606f 626a 6020 616e  ta type `obj` an
-00024c50: 6420 7265 7475 726e 7320 6120 6e65 7720  d returns a new 
-00024c60: 6461 7461 2074 7970 6520 7769 7468 2060  data type with `
-00024c70: 6675 6e63 6020 6d61 7070 6564 206f 7665  func` mapped ove
-00024c80: 7220 7468 6520 636f 6e74 656e 7473 2e20  r the contents. 
-00024c90: 436f 636f 6e75 7427 7320 6066 6d61 7060  Coconut's `fmap`
-00024ca0: 2066 756e 6374 696f 6e20 646f 6573 2074   function does t
-00024cb0: 6865 2065 7861 6374 2073 616d 6520 7468  he exact same th
-00024cc0: 696e 6720 666f 7220 436f 636f 6e75 7427  ing for Coconut'
-00024cd0: 7320 5b64 6174 6120 7479 7065 735d 2823  s [data types](#
-00024ce0: 6461 7461 292e 0a0a 6066 6d61 7060 2063  data)...`fmap` c
-00024cf0: 616e 2061 6c73 6f20 6265 2075 7365 6420  an also be used 
-00024d00: 6f6e 2074 6865 2062 7569 6c74 2d69 6e20  on the built-in 
-00024d10: 6f62 6a65 6374 7320 6073 7472 602c 2060  objects `str`, `
-00024d20: 6469 6374 602c 2060 6c69 7374 602c 2060  dict`, `list`, `
-00024d30: 7475 706c 6560 2c20 6073 6574 602c 2060  tuple`, `set`, `
-00024d40: 6672 6f7a 656e 7365 7460 2c20 616e 6420  frozenset`, and 
-00024d50: 6064 6963 7460 2061 7320 6120 7661 7269  `dict` as a vari
-00024d60: 616e 7420 6f66 2060 6d61 7060 2074 6861  ant of `map` tha
-00024d70: 7420 7265 7475 726e 7320 6261 636b 2061  t returns back a
-00024d80: 6e20 6f62 6a65 6374 206f 6620 7468 6520  n object of the 
-00024d90: 7361 6d65 2074 7970 652e 0a0a 5468 6520  same type...The 
-00024da0: 6265 6861 7669 6f72 206f 6620 6066 6d61  behavior of `fma
-00024db0: 7060 2066 6f72 2061 2067 6976 656e 206f  p` for a given o
-00024dc0: 626a 6563 7420 6361 6e20 6265 206f 7665  bject can be ove
-00024dd0: 7272 6964 6465 6e20 6279 2064 6566 696e  rridden by defin
-00024de0: 696e 6720 616e 2060 5f5f 666d 6170 5f5f  ing an `__fmap__
-00024df0: 2873 656c 662c 2066 756e 6329 6020 6d61  (self, func)` ma
-00024e00: 6769 6320 6d65 7468 6f64 2074 6861 7420  gic method that 
-00024e10: 7769 6c6c 2062 6520 6361 6c6c 6564 2077  will be called w
-00024e20: 6865 6e65 7665 7220 6066 6d61 7060 2069  henever `fmap` i
-00024e30: 7320 696e 766f 6b65 6420 6f6e 2074 6861  s invoked on tha
-00024e40: 7420 6f62 6a65 6374 2e20 4e6f 7465 2074  t object. Note t
-00024e50: 6861 7420 605f 5f66 6d61 705f 5f60 2069  hat `__fmap__` i
-00024e60: 6d70 6c65 6d65 6e74 6174 696f 6e73 2073  mplementations s
-00024e70: 686f 756c 6420 616c 7761 7973 2073 6174  hould always sat
-00024e80: 6973 6679 2074 6865 205b 4675 6e63 746f  isfy the [Functo
-00024e90: 7220 4c61 7773 5d28 6874 7470 733a 2f2f  r Laws](https://
-00024ea0: 7769 6b69 2e68 6173 6b65 6c6c 2e6f 7267  wiki.haskell.org
-00024eb0: 2f46 756e 6374 6f72 292e 0a0a 466f 7220  /Functor)...For 
-00024ec0: 6064 6963 7460 2c20 6f72 2061 6e79 206f  `dict`, or any o
-00024ed0: 7468 6572 2060 636f 6c6c 6563 7469 6f6e  ther `collection
-00024ee0: 732e 6162 632e 4d61 7070 696e 6760 2c20  s.abc.Mapping`, 
-00024ef0: 6066 6d61 7060 2077 696c 6c20 6d61 7020  `fmap` will map 
-00024f00: 6f76 6572 2074 6865 206d 6170 7069 6e67  over the mapping
-00024f10: 2773 2060 2e69 7465 6d73 2829 6020 696e  's `.items()` in
-00024f20: 7374 6561 6420 6f66 2074 6865 2064 6566  stead of the def
-00024f30: 6175 6c74 2069 7465 7261 7469 6f6e 2074  ault iteration t
-00024f40: 6872 6f75 6768 2069 7473 2060 2e6b 6579  hrough its `.key
-00024f50: 7328 2960 2c20 7769 7468 2074 6865 206e  s()`, with the n
-00024f60: 6577 206d 6170 7069 6e67 2072 6563 6f6e  ew mapping recon
-00024f70: 7374 7275 6374 6564 2066 726f 6d20 7468  structed from th
-00024f80: 6520 6d61 7070 6564 206f 7665 7220 6974  e mapped over it
-00024f90: 656d 732e 205f 4445 5052 4543 4154 4544  ems. _DEPRECATED
-00024fa0: 3a20 6066 6d61 7024 2873 7461 726d 6170  : `fmap$(starmap
-00024fb0: 5f6f 7665 725f 6d61 7070 696e 6773 3d54  _over_mappings=T
-00024fc0: 7275 6529 6020 7769 6c6c 2060 7374 6172  rue)` will `star
-00024fd0: 6d61 7060 206f 7665 7220 7468 6520 602e  map` over the `.
-00024fe0: 6974 656d 7328 2960 2069 6e73 7465 6164  items()` instead
-00024ff0: 206f 6620 606d 6170 6020 6f76 6572 2074   of `map` over t
-00025000: 6865 6d2e 5f0a 0a46 6f72 205b 606e 756d  hem._..For [`num
-00025010: 7079 605d 2823 6e75 6d70 792d 696e 7465  py`](#numpy-inte
-00025020: 6772 6174 696f 6e29 206f 626a 6563 7473  gration) objects
-00025030: 2c20 6066 6d61 7060 2077 696c 6c20 7573  , `fmap` will us
-00025040: 6520 5b60 6e70 2e76 6563 746f 7269 7a65  e [`np.vectorize
-00025050: 605d 2868 7474 7073 3a2f 2f64 6f63 732e  `](https://docs.
-00025060: 7363 6970 792e 6f72 672f 646f 632f 6e75  scipy.org/doc/nu
-00025070: 6d70 792f 7265 6665 7265 6e63 652f 6765  mpy/reference/ge
-00025080: 6e65 7261 7465 642f 6e75 6d70 792e 7665  nerated/numpy.ve
-00025090: 6374 6f72 697a 652e 6874 6d6c 2920 746f  ctorize.html) to
-000250a0: 2070 726f 6475 6365 2074 6865 2072 6573   produce the res
-000250b0: 756c 742e 0a0a 466f 7220 5b60 7061 6e64  ult...For [`pand
-000250c0: 6173 605d 2868 7474 7073 3a2f 2f70 616e  as`](https://pan
-000250d0: 6461 732e 7079 6461 7461 2e6f 7267 2f29  das.pydata.org/)
-000250e0: 206f 626a 6563 7473 2c20 6066 6d61 7060   objects, `fmap`
-000250f0: 2077 696c 6c20 7573 6520 5b60 2e61 7070   will use [`.app
-00025100: 6c79 605d 2868 7474 7073 3a2f 2f70 616e  ly`](https://pan
-00025110: 6461 732e 7079 6461 7461 2e6f 7267 2f64  das.pydata.org/d
-00025120: 6f63 732f 7265 6665 7265 6e63 652f 6170  ocs/reference/ap
-00025130: 692f 7061 6e64 6173 2e44 6174 6146 7261  i/pandas.DataFra
-00025140: 6d65 2e61 7070 6c79 2e68 746d 6c29 2061  me.apply.html) a
-00025150: 6c6f 6e67 2074 6865 206c 6173 7420 6178  long the last ax
-00025160: 6973 2028 736f 2072 6f77 2d77 6973 6520  is (so row-wise 
-00025170: 666f 7220 6044 6174 6146 7261 6d65 6027  for `DataFrame`'
-00025180: 732c 2065 6c65 6d65 6e74 2d77 6973 6520  s, element-wise 
-00025190: 666f 7220 6053 6572 6965 7360 2773 292e  for `Series`'s).
-000251a0: 0a0a 466f 7220 6173 796e 6368 726f 6e6f  ..For asynchrono
-000251b0: 7573 2069 7465 7261 626c 6573 2c20 6066  us iterables, `f
-000251c0: 6d61 7060 2077 696c 6c20 6d61 7020 6173  map` will map as
-000251d0: 796e 6368 726f 6e6f 7573 6c79 2c20 6d61  ynchronously, ma
-000251e0: 6b69 6e67 2060 666d 6170 6020 6571 7569  king `fmap` equi
-000251f0: 7661 6c65 6e74 2069 6e20 7468 6174 2063  valent in that c
-00025200: 6173 6520 746f 0a60 6060 636f 636f 6e75  ase to.```coconu
-00025210: 745f 7079 7468 6f6e 0a61 7379 6e63 2064  t_python.async d
-00025220: 6566 2066 6d61 705f 6f76 6572 5f61 7379  ef fmap_over_asy
-00025230: 6e63 5f69 7465 7273 2866 756e 632c 2061  nc_iters(func, a
-00025240: 7379 6e63 5f69 7465 7229 3a0a 2020 2020  sync_iter):.    
-00025250: 6173 796e 6320 666f 7220 6974 656d 2069  async for item i
-00025260: 6e20 6173 796e 635f 6974 6572 3a0a 2020  n async_iter:.  
-00025270: 2020 2020 2020 7969 656c 6420 6675 6e63        yield func
-00025280: 2869 7465 6d29 0a60 6060 0a73 7563 6820  (item).```.such 
-00025290: 7468 6174 2060 666d 6170 6020 6361 6e20  that `fmap` can 
-000252a0: 6566 6665 6374 6976 656c 7920 6265 2075  effectively be u
-000252b0: 7365 6420 6173 2061 6e20 6173 796e 6320  sed as an async 
-000252c0: 6d61 702e 0a0a 5f44 4550 5245 4341 5445  map..._DEPRECATE
-000252d0: 443a 2060 666d 6170 2866 756e 632c 206f  D: `fmap(func, o
-000252e0: 626a 2c20 6661 6c6c 6261 636b 5f74 6f5f  bj, fallback_to_
-000252f0: 696e 6974 3d54 7275 6529 6020 7769 6c6c  init=True)` will
-00025300: 2066 616c 6c20 6261 636b 2074 6f20 606f   fall back to `o
-00025310: 626a 2e5f 5f63 6c61 7373 5f5f 286d 6170  bj.__class__(map
-00025320: 2866 756e 632c 206f 626a 2929 6020 6966  (func, obj))` if
-00025330: 206e 6f20 6066 6d61 7060 2069 6d70 6c65   no `fmap` imple
-00025340: 6d65 6e74 6174 696f 6e20 6973 2061 7661  mentation is ava
-00025350: 696c 6162 6c65 2072 6174 6865 7220 7468  ilable rather th
-00025360: 616e 2072 6169 7365 2060 5479 7065 4572  an raise `TypeEr
-00025370: 726f 7260 2e5f 0a0a 2323 2323 2320 4578  ror`._..##### Ex
-00025380: 616d 706c 650a 0a2a 2a43 6f63 6f6e 7574  ample..**Coconut
-00025390: 3a2a 2a0a 6060 6063 6f63 6f6e 7574 0a5b  :**.```coconut.[
-000253a0: 312c 2032 2c20 335d 207c 3e20 666d 6170  1, 2, 3] |> fmap
-000253b0: 2428 7820 2d3e 2078 2b31 2920 3d3d 205b  $(x -> x+1) == [
-000253c0: 322c 2033 2c20 345d 0a0a 636c 6173 7320  2, 3, 4]..class 
-000253d0: 4d61 7962 650a 6461 7461 204e 6f74 6869  Maybe.data Nothi
-000253e0: 6e67 2829 2066 726f 6d20 4d61 7962 650a  ng() from Maybe.
-000253f0: 6461 7461 204a 7573 7428 6e29 2066 726f  data Just(n) fro
-00025400: 6d20 4d61 7962 650a 0a4a 7573 7428 3329  m Maybe..Just(3)
-00025410: 207c 3e20 666d 6170 2428 7820 2d3e 2078   |> fmap$(x -> x
-00025420: 2a32 2920 3d3d 204a 7573 7428 3629 0a4e  *2) == Just(6).N
-00025430: 6f74 6869 6e67 2829 207c 3e20 666d 6170  othing() |> fmap
-00025440: 2428 7820 2d3e 2078 2a32 2920 3d3d 204e  $(x -> x*2) == N
-00025450: 6f74 6869 6e67 2829 0a60 6060 0a0a 2a2a  othing().```..**
-00025460: 5079 7468 6f6e 3a2a 2a0a 5f43 616e 2774  Python:**._Can't
-00025470: 2062 6520 646f 6e65 2077 6974 686f 7574   be done without
-00025480: 2061 2073 6572 6965 7320 6f66 206d 6574   a series of met
-00025490: 686f 6420 6465 6669 6e69 7469 6f6e 7320  hod definitions 
-000254a0: 666f 7220 6561 6368 2064 6174 6120 7479  for each data ty
-000254b0: 7065 2e20 5365 6520 7468 6520 636f 6d70  pe. See the comp
-000254c0: 696c 6564 2063 6f64 6520 666f 7220 7468  iled code for th
-000254d0: 6520 5079 7468 6f6e 2073 796e 7461 782e  e Python syntax.
-000254e0: 5f0a 0a0a 2323 2323 2060 6361 6c6c 600a  _...#### `call`.
-000254f0: 0a2a 2a63 616c 6c2a 2a28 5f66 756e 635f  .**call**(_func_
-00025500: 2c20 2f2c 202a 5f61 7267 735f 2c20 5c2a  , /, *_args_, \*
-00025510: 5c2a 5f6b 7761 7267 735f 290a 0a43 6f63  \*_kwargs_)..Coc
-00025520: 6f6e 7574 2773 2060 6361 6c6c 6020 7369  onut's `call` si
-00025530: 6d70 6c79 2069 6d70 6c65 6d65 6e74 7320  mply implements 
-00025540: 6675 6e63 7469 6f6e 2061 7070 6c69 6361  function applica
-00025550: 7469 6f6e 2e20 5468 7573 2c20 6063 616c  tion. Thus, `cal
-00025560: 6c60 2069 7320 6566 6665 6374 6976 656c  l` is effectivel
-00025570: 7920 6571 7569 7661 6c65 6e74 2074 6f0a  y equivalent to.
-00025580: 6060 6063 6f63 6f6e 7574 0a64 6566 2063  ```coconut.def c
-00025590: 616c 6c28 662c 202f 2c20 2a61 7267 732c  all(f, /, *args,
-000255a0: 202a 2a6b 7761 7267 7329 203d 2066 282a   **kwargs) = f(*
-000255b0: 6172 6773 2c20 2a2a 6b77 6172 6773 290a  args, **kwargs).
-000255c0: 6060 600a 0a60 6361 6c6c 6020 6973 2070  ```..`call` is p
-000255d0: 7269 6d61 7269 6c79 2075 7365 6675 6c20  rimarily useful 
-000255e0: 6173 2061 6e20 5b6f 7065 7261 746f 7220  as an [operator 
-000255f0: 6675 6e63 7469 6f6e 5d28 236f 7065 7261  function](#opera
-00025600: 746f 722d 6675 6e63 7469 6f6e 7329 2066  tor-functions) f
-00025610: 6f72 2066 756e 6374 696f 6e20 6170 706c  or function appl
-00025620: 6963 6174 696f 6e20 7768 656e 2077 7269  ication when wri
-00025630: 7469 6e67 2069 6e20 6120 706f 696e 742d  ting in a point-
-00025640: 6672 6565 2073 7479 6c65 2e0a 0a5f 4445  free style..._DE
-00025650: 5052 4543 4154 4544 3a20 606f 6660 2069  PRECATED: `of` i
-00025660: 7320 6176 6169 6c61 626c 6520 6173 2061  s available as a
-00025670: 2064 6570 7265 6361 7465 6420 616c 6961   deprecated alia
-00025680: 7320 666f 7220 6063 616c 6c60 2e20 4e6f  s for `call`. No
-00025690: 7465 2074 6861 7420 6465 7072 6563 6174  te that deprecat
-000256a0: 6564 2066 6561 7475 7265 7320 6172 6520  ed features are 
-000256b0: 6469 7361 626c 6564 2069 6e20 602d 2d73  disabled in `--s
-000256c0: 7472 6963 7460 206d 6f64 652e 5f0a 0a23  trict` mode._..#
-000256d0: 2323 2320 6073 6166 655f 6361 6c6c 600a  ### `safe_call`.
-000256e0: 0a2a 2a73 6166 655f 6361 6c6c 2a2a 285f  .**safe_call**(_
-000256f0: 6675 6e63 5f2c 202f 2c20 2a5f 6172 6773  func_, /, *_args
-00025700: 5f2c 205c 2a5c 2a5f 6b77 6172 6773 5f29  _, \*\*_kwargs_)
-00025710: 0a0a 436f 636f 6e75 7427 7320 6073 6166  ..Coconut's `saf
-00025720: 655f 6361 6c6c 6020 6973 2061 2076 6572  e_call` is a ver
-00025730: 7369 6f6e 206f 6620 5b60 6361 6c6c 605d  sion of [`call`]
-00025740: 2823 6361 6c6c 2920 7468 6174 2063 6174  (#call) that cat
-00025750: 6368 6573 2061 6e79 2060 4578 6365 7074  ches any `Except
-00025760: 696f 6e60 7320 616e 6420 7265 7475 726e  ion`s and return
-00025770: 7320 616e 205b 6045 7870 6563 7465 6460  s an [`Expected`
-00025780: 5d28 2365 7870 6563 7465 6429 2063 6f6e  ](#expected) con
-00025790: 7461 696e 696e 6720 6569 7468 6572 2074  taining either t
-000257a0: 6865 2072 6573 756c 7420 6f72 2074 6865  he result or the
-000257b0: 2065 7272 6f72 2e0a 0a60 7361 6665 5f63   error...`safe_c
-000257c0: 616c 6c60 2069 7320 6566 6665 6374 6976  all` is effectiv
-000257d0: 656c 7920 6571 7569 7661 6c65 6e74 2074  ely equivalent t
-000257e0: 6f3a 0a60 6060 636f 636f 6e75 740a 6465  o:.```coconut.de
-000257f0: 6620 7361 6665 5f63 616c 6c28 662c 202f  f safe_call(f, /
-00025800: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
-00025810: 7329 3a0a 2020 2020 7472 793a 0a20 2020  s):.    try:.   
-00025820: 2020 2020 2072 6574 7572 6e20 4578 7065       return Expe
-00025830: 6374 6564 2866 282a 6172 6773 2c20 2a2a  cted(f(*args, **
-00025840: 6b77 6172 6773 2929 0a20 2020 2065 7863  kwargs)).    exc
-00025850: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00025860: 2065 7272 3a0a 2020 2020 2020 2020 7265   err:.        re
-00025870: 7475 726e 2045 7870 6563 7465 6428 6572  turn Expected(er
-00025880: 726f 723d 6572 7229 0a60 6060 0a0a 2323  ror=err).```..##
-00025890: 2323 2320 4578 616d 706c 650a 0a2a 2a43  ### Example..**C
-000258a0: 6f63 6f6e 7574 3a2a 2a0a 6060 6063 6f63  oconut:**.```coc
-000258b0: 6f6e 7574 0a72 6573 2c20 6572 7220 3d20  onut.res, err = 
-000258c0: 7361 6665 5f63 616c 6c28 2d3e 2031 202f  safe_call(-> 1 /
-000258d0: 2030 2920 7c3e 2066 6d61 7024 282e 2b31   0) |> fmap$(.+1
-000258e0: 290a 6060 600a 0a2a 2a50 7974 686f 6e3a  ).```..**Python:
-000258f0: 2a2a 0a5f 4361 6e27 7420 6265 2064 6f6e  **._Can't be don
-00025900: 6520 7769 7468 6f75 7420 6120 636f 6d70  e without a comp
-00025910: 6c65 7820 6045 7870 6563 7465 6460 2064  lex `Expected` d
-00025920: 6566 696e 6974 696f 6e2e 2053 6565 2074  efinition. See t
-00025930: 6865 2063 6f6d 7069 6c65 6420 636f 6465  he compiled code
-00025940: 2066 6f72 2074 6865 2050 7974 686f 6e20   for the Python 
-00025950: 7379 6e74 6178 2e5f 0a0a 2323 2323 2060  syntax._..#### `
-00025960: 6964 656e 7460 0a0a 2a2a 6964 656e 742a  ident`..**ident*
-00025970: 2a28 5f78 5f2c 202a 2c20 5f73 6964 655c  *(_x_, *, _side\
-00025980: 5f65 6666 6563 745f 3d60 4e6f 6e65 6029  _effect_=`None`)
-00025990: 0a0a 436f 636f 6e75 7427 7320 6069 6465  ..Coconut's `ide
-000259a0: 6e74 6020 6973 2074 6865 2069 6465 6e74  nt` is the ident
-000259b0: 6974 7920 6675 6e63 7469 6f6e 2c20 6765  ity function, ge
-000259c0: 6e65 7261 6c6c 7920 6571 7569 7661 6c65  nerally equivale
-000259d0: 6e74 2074 6f20 6078 202d 3e20 7860 2e0a  nt to `x -> x`..
-000259e0: 0a60 6964 656e 7460 2061 6c73 6f20 6163  .`ident` also ac
-000259f0: 6365 7074 7320 6f6e 6520 6b65 7977 6f72  cepts one keywor
-00025a00: 642d 6f6e 6c79 2061 7267 756d 656e 742c  d-only argument,
-00025a10: 2060 7369 6465 5f65 6666 6563 7460 2c20   `side_effect`, 
-00025a20: 7768 6963 6820 7370 6563 6966 6965 7320  which specifies 
-00025a30: 6120 6675 6e63 7469 6f6e 2074 6f20 6361  a function to ca
-00025a40: 6c6c 206f 6e20 7468 6520 6172 6775 6d65  ll on the argume
-00025a50: 6e74 2062 6566 6f72 6520 6974 2069 7320  nt before it is 
-00025a60: 7265 7475 726e 6564 2e20 5468 7573 2c20  returned. Thus, 
-00025a70: 6069 6465 6e74 6020 6973 2065 6666 6563  `ident` is effec
-00025a80: 7469 7665 6c79 2065 7175 6976 616c 656e  tively equivalen
-00025a90: 7420 746f 3a0a 6060 6063 6f63 6f6e 7574  t to:.```coconut
-00025aa0: 0a64 6566 2069 6465 6e74 2878 2c20 2a2c  .def ident(x, *,
-00025ab0: 2073 6964 655f 6566 6665 6374 3d4e 6f6e   side_effect=Non
-00025ac0: 6529 3a0a 2020 2020 6966 2073 6964 655f  e):.    if side_
-00025ad0: 6566 6665 6374 2069 7320 6e6f 7420 4e6f  effect is not No
-00025ae0: 6e65 3a0a 2020 2020 2020 2020 7369 6465  ne:.        side
-00025af0: 5f65 6666 6563 7428 7829 0a20 2020 2072  _effect(x).    r
-00025b00: 6574 7572 6e20 780a 6060 600a 0a60 6964  eturn x.```..`id
-00025b10: 656e 7460 2069 7320 7072 696d 6172 696c  ent` is primaril
-00025b20: 7920 7573 6566 756c 2077 6865 6e20 7772  y useful when wr
-00025b30: 6974 696e 6720 696e 2061 2070 6f69 6e74  iting in a point
-00025b40: 2d66 7265 6520 7374 796c 6520 2865 2e67  -free style (e.g
-00025b50: 2e20 696e 2063 6f6d 6269 6e61 7469 6f6e  . in combination
-00025b60: 2077 6974 6820 5b60 6c69 6674 605d 2823   with [`lift`](#
-00025b70: 6c69 6674 2929 206f 7220 666f 7220 6465  lift)) or for de
-00025b80: 6275 6767 696e 6720 5b70 6970 6573 5d28  bugging [pipes](
-00025b90: 2370 6970 6573 2920 7768 6572 6520 6069  #pipes) where `i
-00025ba0: 6465 6e74 2428 7369 6465 5f65 6666 6563  dent$(side_effec
-00025bb0: 743d 7072 696e 7429 6020 6361 6e20 6c65  t=print)` can le
-00025bc0: 7420 796f 7520 7365 6520 7768 6174 2069  t you see what i
-00025bd0: 7320 6265 696e 6720 7069 7065 642e 0a0a  s being piped...
-00025be0: 2323 2323 2060 636f 6e73 7460 0a0a 2a2a  #### `const`..**
-00025bf0: 636f 6e73 742a 2a28 5f76 616c 7565 5f29  const**(_value_)
-00025c00: 0a0a 436f 636f 6e75 7427 7320 6063 6f6e  ..Coconut's `con
-00025c10: 7374 6020 7369 6d70 6c79 2063 6f6e 7374  st` simply const
-00025c20: 7275 6374 7320 6120 6675 6e63 7469 6f6e  ructs a function
-00025c30: 2074 6861 742c 2077 6861 7465 7665 7220   that, whatever 
-00025c40: 6974 7320 6172 6775 6d65 6e74 732c 206a  its arguments, j
-00025c50: 7573 7420 7265 7475 726e 7320 7468 6520  ust returns the 
-00025c60: 6769 7665 6e20 7661 6c75 652e 2054 6875  given value. Thu
-00025c70: 732c 2060 636f 6e73 7460 2069 7320 6571  s, `const` is eq
-00025c80: 7569 7661 6c65 6e74 2074 6f20 6120 7069  uivalent to a pi
-00025c90: 636b 6c65 6162 6c65 2076 6572 7369 6f6e  ckleable version
-00025ca0: 206f 660a 6060 6063 6f63 6f6e 7574 0a64   of.```coconut.d
-00025cb0: 6566 2063 6f6e 7374 2876 616c 7565 2920  ef const(value) 
-00025cc0: 3d20 282a 6172 6773 2c20 2a2a 6b77 6172  = (*args, **kwar
-00025cd0: 6773 2920 2d3e 2076 616c 7565 0a60 6060  gs) -> value.```
-00025ce0: 0a0a 6063 6f6e 7374 6020 6973 2070 7269  ..`const` is pri
-00025cf0: 6d61 7269 6c79 2075 7365 6675 6c20 7768  marily useful wh
-00025d00: 656e 2077 7269 7469 6e67 2069 6e20 6120  en writing in a 
-00025d10: 706f 696e 742d 6672 6565 2073 7479 6c65  point-free style
-00025d20: 2028 652e 672e 2069 6e20 636f 6d62 696e   (e.g. in combin
-00025d30: 6174 696f 6e20 7769 7468 205b 606c 6966  ation with [`lif
-00025d40: 7460 5d28 236c 6966 7429 292e 0a0a 2323  t`](#lift))...##
-00025d50: 2323 2060 666c 6970 600a 0a2a 2a66 6c69  ## `flip`..**fli
-00025d60: 702a 2a28 5f66 756e 635f 2c20 5f6e 6172  p**(_func_, _nar
-00025d70: 6773 5f3d 604e 6f6e 6560 290a 0a43 6f63  gs_=`None`)..Coc
-00025d80: 6f6e 7574 2773 2060 666c 6970 2866 2c20  onut's `flip(f, 
-00025d90: 6e61 7267 733d 4e6f 6e65 2960 2069 7320  nargs=None)` is 
-00025da0: 6120 6869 6768 6572 2d6f 7264 6572 2066  a higher-order f
-00025db0: 756e 6374 696f 6e20 7468 6174 2c20 6769  unction that, gi
-00025dc0: 7665 6e20 6120 6675 6e63 7469 6f6e 2060  ven a function `
-00025dd0: 6660 2c20 7265 7475 726e 7320 6120 6e65  f`, returns a ne
-00025de0: 7720 6675 6e63 7469 6f6e 2077 6974 6820  w function with 
-00025df0: 7265 7665 7273 6564 2061 7267 756d 656e  reversed argumen
-00025e00: 7420 6f72 6465 722e 2049 6620 606e 6172  t order. If `nar
-00025e10: 6773 6020 6973 2070 6173 7365 642c 206f  gs` is passed, o
-00025e20: 6e6c 7920 7468 6520 6669 7273 7420 606e  nly the first `n
-00025e30: 6172 6773 6020 6172 6775 6d65 6e74 7320  args` arguments 
-00025e40: 6172 6520 7265 7665 7273 6564 2e0a 0a46  are reversed...F
-00025e50: 6f72 2074 6865 2062 696e 6172 7920 6361  or the binary ca
-00025e60: 7365 2c20 6066 6c69 7060 2077 6f72 6b73  se, `flip` works
-00025e70: 2061 730a 6060 6063 6f63 6f6e 7574 0a66   as.```coconut.f
-00025e80: 6c69 7028 662c 2032 2928 782c 2079 2920  lip(f, 2)(x, y) 
-00025e90: 3d3d 2066 2879 2c20 7829 0a60 6060 0a73  == f(y, x).```.s
-00025ea0: 7563 6820 7468 6174 2060 666c 6970 2428  uch that `flip$(
-00025eb0: 3f2c 2032 2960 2069 6d70 6c65 6d65 6e74  ?, 2)` implement
-00025ec0: 7320 7468 6520 6043 6020 636f 6d62 696e  s the `C` combin
-00025ed0: 6174 6f72 2028 6066 6c69 7060 2069 6e20  ator (`flip` in 
-00025ee0: 4861 736b 656c 6c29 2e0a 0a49 6e20 7468  Haskell)...In th
-00025ef0: 6520 6765 6e65 7261 6c20 6361 7365 2c20  e general case, 
-00025f00: 6066 6c69 7060 2069 7320 6571 7569 7661  `flip` is equiva
-00025f10: 6c65 6e74 2074 6f20 6120 7069 636b 6c65  lent to a pickle
-00025f20: 6162 6c65 2076 6572 7369 6f6e 206f 660a  able version of.
-00025f30: 6060 6063 6f63 6f6e 7574 0a64 6566 2066  ```coconut.def f
-00025f40: 6c69 7028 662c 206e 6172 6773 3d4e 6f6e  lip(f, nargs=Non
-00025f50: 6529 203d 0a20 2020 2028 2a61 7267 732c  e) =.    (*args,
-00025f60: 202a 2a6b 7761 7267 7329 202d 3e20 280a   **kwargs) -> (.
-00025f70: 2020 2020 2020 2020 6628 2a61 7267 735b          f(*args[
-00025f80: 3a3a 2d31 5d2c 202a 2a6b 7761 7267 7329  ::-1], **kwargs)
-00025f90: 2069 6620 6e61 7267 7320 6973 204e 6f6e   if nargs is Non
-00025fa0: 650a 2020 2020 2020 2020 656c 7365 2066  e.        else f
-00025fb0: 282a 2861 7267 735b 6e61 7267 732d 313a  (*(args[nargs-1:
-00025fc0: 3a2d 315d 202b 2061 7267 735b 6e61 7267  :-1] + args[narg
-00025fd0: 733a 5d29 2c20 2a2a 6b77 6172 6773 290a  s:]), **kwargs).
-00025fe0: 2020 2020 290a 6060 600a 0a23 2323 2320      ).```..#### 
-00025ff0: 606c 6966 7460 0a0a 2a2a 6c69 6674 2a2a  `lift`..**lift**
-00026000: 285f 6675 6e63 5f29 0a0a 2a2a 6c69 6674  (_func_)..**lift
-00026010: 2a2a 285f 6675 6e63 5f2c 202a 5f66 756e  **(_func_, *_fun
-00026020: 635c 5f61 7267 735f 2c20 2a2a 5f66 756e  c\_args_, **_fun
-00026030: 635c 5f6b 7761 7267 735f 290a 0a43 6f63  c\_kwargs_)..Coc
-00026040: 6f6e 7574 2773 2060 6c69 6674 6020 6275  onut's `lift` bu
-00026050: 696c 742d 696e 2069 7320 6120 6869 6768  ilt-in is a high
-00026060: 6572 2d6f 7264 6572 2066 756e 6374 696f  er-order functio
-00026070: 6e20 7468 6174 2074 616b 6573 2069 6e20  n that takes in 
-00026080: 6120 6675 6e63 7469 6f6e 2061 6e64 20e2  a function and .
-00026090: 809c 6c69 6674 73e2 809d 2069 7420 7570  ..lifts... it up
-000260a0: 2073 6f20 7468 6174 2061 6c6c 206f 6620   so that all of 
-000260b0: 6974 7320 6172 6775 6d65 6e74 7320 6172  its arguments ar
-000260c0: 6520 6675 6e63 7469 6f6e 732e 0a0a 4173  e functions...As
-000260d0: 2061 2073 696d 706c 6520 6578 616d 706c   a simple exampl
-000260e0: 652c 2066 6f72 2061 2062 696e 6172 7920  e, for a binary 
-000260f0: 6675 6e63 7469 6f6e 2060 6628 782c 2079  function `f(x, y
-00026100: 2960 2061 6e64 2074 776f 2075 6e61 7279  )` and two unary
-00026110: 2066 756e 6374 696f 6e73 2060 6728 7a29   functions `g(z)
-00026120: 6020 616e 6420 6068 287a 2960 2c20 606c  ` and `h(z)`, `l
-00026130: 6966 7460 2077 6f72 6b73 2061 730a 6060  ift` works as.``
-00026140: 6063 6f63 6f6e 7574 0a6c 6966 7428 6629  `coconut.lift(f)
-00026150: 2867 2c20 6829 287a 2920 3d3d 2066 2867  (g, h)(z) == f(g
-00026160: 287a 292c 2068 287a 2929 0a60 6060 0a73  (z), h(z)).```.s
-00026170: 7563 6820 7468 6174 2069 6e20 7468 6973  uch that in this
-00026180: 2063 6173 6520 606c 6966 7460 2069 6d70   case `lift` imp
-00026190: 6c65 6d65 6e74 7320 7468 6520 6053 2760  lements the `S'`
-000261a0: 2063 6f6d 6269 6e61 746f 7220 2860 6c69   combinator (`li
-000261b0: 6674 4132 6020 6f72 2060 6c69 6674 4d32  ftA2` or `liftM2
-000261c0: 6020 696e 2048 6173 6b65 6c6c 292e 0a0a  ` in Haskell)...
-000261d0: 496e 2074 6865 2067 656e 6572 616c 2063  In the general c
-000261e0: 6173 652c 2060 6c69 6674 6020 6973 2065  ase, `lift` is e
-000261f0: 7175 6976 616c 656e 7420 746f 2061 2070  quivalent to a p
-00026200: 6963 6b6c 6561 626c 6520 7665 7273 696f  ickleable versio
-00026210: 6e20 6f66 0a60 6060 636f 636f 6e75 740a  n of.```coconut.
-00026220: 6465 6620 6c69 6674 2866 2920 3d20 280a  def lift(f) = (.
-00026230: 2020 2020 282a 6675 6e63 5f61 7267 732c      (*func_args,
-00026240: 202a 2a66 756e 635f 6b77 6172 6773 2920   **func_kwargs) 
-00026250: 2d3e 0a20 2020 2020 2020 2028 2a61 7267  ->.        (*arg
-00026260: 732c 202a 2a6b 7761 7267 7329 202d 3e0a  s, **kwargs) ->.
-00026270: 2020 2020 2020 2020 2020 2020 6628 0a20              f(. 
-00026280: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-00026290: 2867 282a 6172 6773 2c20 2a2a 6b77 6172  (g(*args, **kwar
-000262a0: 6773 2920 666f 7220 6720 696e 2066 756e  gs) for g in fun
-000262b0: 635f 6172 6773 292c 0a20 2020 2020 2020  c_args),.       
-000262c0: 2020 2020 2020 2020 202a 2a7b 6b3a 2068           **{k: h
-000262d0: 282a 6172 6773 2c20 2a2a 6b77 6172 6773  (*args, **kwargs
-000262e0: 2920 666f 7220 6b2c 2068 2069 6e20 6675  ) for k, h in fu
-000262f0: 6e63 5f6b 7761 7267 732e 6974 656d 7328  nc_kwargs.items(
-00026300: 297d 0a20 2020 2020 2020 2020 2020 2029  )}.            )
-00026310: 0a29 0a60 6060 0a0a 606c 6966 7460 2061  .).```..`lift` a
-00026320: 6c73 6f20 7375 7070 6f72 7473 2061 2073  lso supports a s
-00026330: 686f 7274 6375 7420 666f 726d 2073 7563  hortcut form suc
-00026340: 6820 7468 6174 2060 6c69 6674 2866 2c20  h that `lift(f, 
-00026350: 2a66 756e 635f 6172 6773 2c20 2a2a 6675  *func_args, **fu
-00026360: 6e63 5f6b 7761 7267 7329 6020 6973 2065  nc_kwargs)` is e
-00026370: 7175 6976 616c 656e 7420 746f 2060 6c69  quivalent to `li
-00026380: 6674 2866 2928 2a66 756e 635f 6172 6773  ft(f)(*func_args
-00026390: 2c20 2a2a 6675 6e63 5f6b 7761 7267 7329  , **func_kwargs)
-000263a0: 602e 0a0a 2323 2323 2320 4578 616d 706c  `...##### Exampl
-000263b0: 650a 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a  e..**Coconut:**.
-000263c0: 6060 6063 6f63 6f6e 7574 0a78 735f 616e  ```coconut.xs_an
-000263d0: 645f 7873 7031 203d 2069 6465 6e74 2060  d_xsp1 = ident `
-000263e0: 6c69 6674 287a 6970 2960 206d 6170 2428  lift(zip)` map$(
-000263f0: 2d3e 5f2b 3129 0a6d 696e 5f61 6e64 5f6d  ->_+1).min_and_m
-00026400: 6178 203d 206c 6966 7428 2c29 286d 696e  ax = lift(,)(min
-00026410: 2c20 6d61 7829 0a70 6c75 735f 616e 645f  , max).plus_and_
-00026420: 7469 6d65 7320 3d20 282b 2920 606c 6966  times = (+) `lif
-00026430: 7428 2c29 6020 282a 290a 6060 600a 0a2a  t(,)` (*).```..*
-00026440: 2a50 7974 686f 6e3a 2a2a 0a60 6060 636f  *Python:**.```co
-00026450: 636f 6e75 745f 7079 7468 6f6e 0a64 6566  conut_python.def
-00026460: 2078 735f 616e 645f 7873 7031 2878 7329   xs_and_xsp1(xs)
-00026470: 3a0a 2020 2020 7265 7475 726e 207a 6970  :.    return zip
-00026480: 2878 732c 206d 6170 286c 616d 6264 6120  (xs, map(lambda 
-00026490: 783a 2078 202b 2031 2c20 7873 2929 0a64  x: x + 1, xs)).d
-000264a0: 6566 206d 696e 5f61 6e64 5f6d 6178 2878  ef min_and_max(x
-000264b0: 7329 3a0a 2020 2020 7265 7475 726e 206d  s):.    return m
-000264c0: 696e 2878 7329 2c20 6d61 7828 7873 290a  in(xs), max(xs).
-000264d0: 6465 6620 706c 7573 5f61 6e64 5f74 696d  def plus_and_tim
-000264e0: 6573 2878 2c20 7929 3a0a 2020 2020 7265  es(x, y):.    re
-000264f0: 7475 726e 2078 202b 2079 2c20 7820 2a20  turn x + y, x * 
-00026500: 790a 6060 600a 0a23 2323 2320 6061 6e64  y.```..#### `and
-00026510: 5f74 6865 6e60 2061 6e64 2060 616e 645f  _then` and `and_
-00026520: 7468 656e 5f61 7761 6974 600a 0a43 6f63  then_await`..Coc
-00026530: 6f6e 7574 2070 726f 7669 6465 7320 7468  onut provides th
-00026540: 6520 6061 6e64 5f74 6865 6e60 2061 6e64  e `and_then` and
-00026550: 2060 616e 645f 7468 656e 5f61 7761 6974   `and_then_await
-00026560: 6020 6275 696c 742d 696e 7320 666f 7220  ` built-ins for 
-00026570: 636f 6d70 6f73 696e 6720 6061 7379 6e63  composing `async
-00026580: 6020 6675 6e63 7469 6f6e 732e 2053 7065  ` functions. Spe
-00026590: 6369 6669 6361 6c6c 793a 0a2a 2054 6f20  cifically:.* To 
-000265a0: 666f 7277 6172 6473 2063 6f6d 706f 7365  forwards compose
-000265b0: 2061 6e20 6173 796e 6320 6675 6e63 7469   an async functi
-000265c0: 6f6e 2060 6173 796e 635f 6660 2077 6974  on `async_f` wit
-000265d0: 6820 6120 6e6f 726d 616c 2066 756e 6374  h a normal funct
-000265e0: 696f 6e20 6067 6020 2873 7563 6820 7468  ion `g` (such th
-000265f0: 6174 2060 6760 2069 7320 6361 6c6c 6564  at `g` is called
-00026600: 206f 6e20 7468 6520 7265 7375 6c74 206f   on the result o
-00026610: 6620 6061 7761 6974 6069 6e67 2060 6173  f `await`ing `as
-00026620: 796e 635f 6660 292c 2077 7269 7465 2060  ync_f`), write `
-00026630: 6061 7379 6e63 5f66 2060 616e 645f 7468  `async_f `and_th
-00026640: 656e 6020 6760 602e 0a2a 2054 6f20 666f  en` g``..* To fo
-00026650: 7277 6172 6473 2063 6f6d 706f 7365 2061  rwards compose a
-00026660: 6e20 6173 796e 6320 6675 6e63 7469 6f6e  n async function
-00026670: 2060 6173 796e 635f 6660 2077 6974 6820   `async_f` with 
-00026680: 616e 6f74 6865 7220 6173 796e 6320 6675  another async fu
-00026690: 6e63 7469 6f6e 2060 6173 796e 635f 6760  nction `async_g`
-000266a0: 2028 7375 6368 2074 6861 7420 6061 7379   (such that `asy
-000266b0: 6e63 5f67 6020 6973 2063 616c 6c65 6420  nc_g` is called 
-000266c0: 6f6e 2074 6865 2072 6573 756c 7420 6f66  on the result of
-000266d0: 2060 6177 6169 7460 696e 6720 6061 7379   `await`ing `asy
-000266e0: 6e63 5f66 602c 2061 6e64 2074 6865 6e20  nc_f`, and then 
-000266f0: 6061 7379 6e63 5f67 6020 6973 2069 7473  `async_g` is its
-00026700: 656c 6620 6177 6169 7465 6429 2c20 7772  elf awaited), wr
-00026710: 6974 6520 6060 6173 796e 635f 6620 6061  ite ``async_f `a
-00026720: 6e64 5f74 6865 6e5f 6177 6169 7460 2061  nd_then_await` a
-00026730: 7379 6e63 5f67 6060 2e0a 2a20 546f 2066  sync_g``..* To f
-00026740: 6f72 7761 7264 7320 636f 6d70 6f73 6520  orwards compose 
-00026750: 6120 6e6f 726d 616c 2066 756e 6374 696f  a normal functio
-00026760: 6e20 6066 6020 7769 7468 2061 6e20 6173  n `f` with an as
-00026770: 796e 6320 6675 6e63 7469 6f6e 2060 6173  ync function `as
-00026780: 796e 635f 6760 2028 7375 6368 2074 6861  ync_g` (such tha
-00026790: 7420 6061 7379 6e63 5f67 6020 6973 2063  t `async_g` is c
-000267a0: 616c 6c65 6420 6f6e 2074 6865 2072 6573  alled on the res
-000267b0: 756c 7420 6f66 2060 6660 292c 206a 7573  ult of `f`), jus
-000267c0: 7420 7772 6974 6520 6066 202e 2e3e 2061  t write `f ..> a
-000267d0: 7379 6e63 5f67 602e 0a0a 4e6f 7465 2074  sync_g`...Note t
-000267e0: 6861 7420 616c 6c20 6f66 2074 6865 2061  hat all of the a
-000267f0: 626f 7665 2077 696c 6c20 616c 7761 7973  bove will always
-00026800: 2072 6573 756c 7420 696e 2074 6865 2072   result in the r
-00026810: 6573 756c 7469 6e67 2063 6f6d 706f 7369  esulting composi
-00026820: 7469 6f6e 2062 6569 6e67 2061 6e20 6061  tion being an `a
-00026830: 7379 6e63 6020 6675 6e63 7469 6f6e 2e0a  sync` function..
-00026840: 0a54 6865 2062 7569 6c74 2d69 6e73 2061  .The built-ins a
-00026850: 7265 2065 6666 6563 7469 7665 6c79 2065  re effectively e
-00026860: 7175 6976 616c 656e 7420 746f 3a0a 6060  quivalent to:.``
-00026870: 6063 6f63 6f6e 7574 0a64 6566 2061 6e64  `coconut.def and
-00026880: 5f74 6865 6e5b 2a2a 542c 2055 2c20 565d  _then[**T, U, V]
-00026890: 280a 2020 2020 6669 7273 745f 6173 796e  (.    first_asyn
-000268a0: 635f 6675 6e63 3a20 6173 796e 6320 282a  c_func: async (*
-000268b0: 2a54 2920 2d3e 2055 2c0a 2020 2020 7365  *T) -> U,.    se
-000268c0: 636f 6e64 5f66 756e 633a 2055 202d 3e20  cond_func: U -> 
-000268d0: 562c 0a29 202d 3e20 6173 796e 6320 282a  V,.) -> async (*
-000268e0: 2a54 2920 2d3e 2056 203d 0a20 2020 2061  *T) -> V =.    a
-000268f0: 7379 6e63 2064 6566 2028 2a61 7267 732c  sync def (*args,
-00026900: 202a 2a6b 7761 7267 7329 202d 3e20 280a   **kwargs) -> (.
-00026910: 2020 2020 2020 2020 6669 7273 745f 6173          first_as
-00026920: 796e 635f 6675 6e63 282a 6172 6773 2c20  ync_func(*args, 
-00026930: 2a2a 6b77 6172 6773 290a 2020 2020 2020  **kwargs).      
-00026940: 2020 7c3e 2061 7761 6974 0a20 2020 2020    |> await.     
-00026950: 2020 207c 3e20 7365 636f 6e64 5f66 756e     |> second_fun
-00026960: 630a 2020 2020 290a 0a64 6566 2061 6e64  c.    )..def and
-00026970: 5f74 6865 6e5f 6177 6169 745b 2a2a 542c  _then_await[**T,
-00026980: 2055 2c20 565d 280a 2020 2020 6669 7273   U, V](.    firs
-00026990: 745f 6173 796e 635f 6675 6e63 3a20 6173  t_async_func: as
-000269a0: 796e 6320 282a 2a54 2920 2d3e 2055 2c0a  ync (**T) -> U,.
-000269b0: 2020 2020 7365 636f 6e64 5f61 7379 6e63      second_async
-000269c0: 5f66 756e 633a 2061 7379 6e63 2055 202d  _func: async U -
-000269d0: 3e20 562c 0a29 202d 3e20 6173 796e 6320  > V,.) -> async 
-000269e0: 282a 2a54 2920 2d3e 2056 203d 0a20 2020  (**T) -> V =.   
-000269f0: 2061 7379 6e63 2064 6566 2028 2a61 7267   async def (*arg
-00026a00: 732c 202a 2a6b 7761 7267 7329 202d 3e20  s, **kwargs) -> 
-00026a10: 280a 2020 2020 2020 2020 6669 7273 745f  (.        first_
-00026a20: 6173 796e 635f 6675 6e63 282a 6172 6773  async_func(*args
-00026a30: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
-00026a40: 2020 2020 7c3e 2061 7761 6974 0a20 2020      |> await.   
-00026a50: 2020 2020 207c 3e20 7365 636f 6e64 5f61       |> second_a
-00026a60: 7379 6e63 5f66 756e 630a 2020 2020 2020  sync_func.      
-00026a70: 2020 7c3e 2061 7761 6974 0a20 2020 2029    |> await.    )
-00026a80: 0a60 6060 0a0a 4c69 6b65 206e 6f72 6d61  .```..Like norma
-00026a90: 6c20 5b66 756e 6374 696f 6e20 636f 6d70  l [function comp
-00026aa0: 6f73 6974 696f 6e5d 2823 6675 6e63 7469  osition](#functi
-00026ab0: 6f6e 2d63 6f6d 706f 7369 7469 6f6e 292c  on-composition),
-00026ac0: 2060 616e 645f 7468 656e 6020 616e 6420   `and_then` and 
-00026ad0: 6061 6e64 5f74 6865 6e5f 6177 6169 7460  `and_then_await`
-00026ae0: 2077 696c 6c20 7072 6573 6572 7665 2061   will preserve a
-00026af0: 6c6c 206d 6574 6164 6174 6120 6174 7461  ll metadata atta
-00026b00: 6368 6564 2074 6f20 7468 6520 6669 7273  ched to the firs
-00026b10: 7420 6675 6e63 7469 6f6e 2069 6e20 7468  t function in th
-00026b20: 6520 636f 6d70 6f73 6974 696f 6e2e 0a0a  e composition...
-00026b30: 2323 2323 2320 4578 616d 706c 650a 0a2a  ##### Example..*
-00026b40: 2a43 6f63 6f6e 7574 3a2a 2a0a 6060 6063  *Coconut:**.```c
-00026b50: 6f63 6f6e 7574 0a6c 6f61 645f 616e 645f  oconut.load_and_
-00026b60: 7365 6e64 5f64 6174 6120 3d20 280a 2020  send_data = (.  
-00026b70: 2020 6c6f 6164 5f64 6174 615f 6173 796e    load_data_asyn
-00026b80: 6328 290a 2020 2020 6061 6e64 5f74 6865  c().    `and_the
-00026b90: 6e60 2070 726f 635f 6461 7461 0a20 2020  n` proc_data.   
-00026ba0: 2060 616e 645f 7468 656e 5f61 7761 6974   `and_then_await
-00026bb0: 6020 7365 6e64 5f64 6174 610a 290a 6060  ` send_data.).``
-00026bc0: 600a 0a2a 2a50 7974 686f 6e3a 2a2a 0a60  `..**Python:**.`
-00026bd0: 6060 636f 636f 6e75 745f 7079 7468 6f6e  ``coconut_python
-00026be0: 0a61 7379 6e63 2064 6566 206c 6f61 645f  .async def load_
-00026bf0: 616e 645f 7365 6e64 5f64 6174 6128 293a  and_send_data():
-00026c00: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
-00026c10: 7420 7365 6e64 5f64 6174 6128 7072 6f63  t send_data(proc
-00026c20: 5f64 6174 6128 6177 6169 7420 6c6f 6164  _data(await load
-00026c30: 5f64 6174 615f 6173 796e 6328 2929 290a  _data_async())).
-00026c40: 6060 600a 0a23 2323 2042 7569 6c74 2d49  ```..### Built-I
-00026c50: 6e73 2066 6f72 2057 6f72 6b69 6e67 2077  ns for Working w
-00026c60: 6974 6820 4974 6572 6174 6f72 730a 0a60  ith Iterators..`
-00026c70: 6060 7b63 6f6e 7465 6e74 737d 0a2d 2d2d  ``{contents}.---
-00026c80: 0a6c 6f63 616c 3a0a 6465 7074 683a 2031  .local:.depth: 1
-00026c90: 0a2d 2d2d 0a60 6060 0a0a 2323 2323 2045  .---.```..#### E
-00026ca0: 6e68 616e 6365 6420 4275 696c 742d 496e  nhanced Built-In
-00026cb0: 730a 0a43 6f63 6f6e 7574 2773 2060 6d61  s..Coconut's `ma
-00026cc0: 7060 2c20 607a 6970 602c 2060 6669 6c74  p`, `zip`, `filt
-00026cd0: 6572 602c 2060 7265 7665 7273 6564 602c  er`, `reversed`,
-00026ce0: 2061 6e64 2060 656e 756d 6572 6174 6560   and `enumerate`
-00026cf0: 206f 626a 6563 7473 2061 7265 2065 6e68   objects are enh
-00026d00: 616e 6365 6420 7665 7273 696f 6e73 206f  anced versions o
-00026d10: 6620 7468 6569 7220 5079 7468 6f6e 2065  f their Python e
-00026d20: 7175 6976 616c 656e 7473 2074 6861 7420  quivalents that 
-00026d30: 7375 7070 6f72 743a 0a0a 2d20 6072 6576  support:..- `rev
-00026d40: 6572 7365 6460 0a2d 2060 7265 7072 600a  ersed`.- `repr`.
-00026d50: 2d20 4f70 7469 6d69 7a65 6420 6e6f 726d  - Optimized norm
-00026d60: 616c 2028 616e 6420 6974 6572 6174 6f72  al (and iterator
-00026d70: 2920 696e 6465 7869 6e67 2f73 6c69 6369  ) indexing/slici
-00026d80: 6e67 2028 606d 6170 602c 2060 7a69 7060  ng (`map`, `zip`
-00026d90: 2c20 6072 6576 6572 7365 6460 2c20 616e  , `reversed`, an
-00026da0: 6420 6065 6e75 6d65 7261 7465 6020 6275  d `enumerate` bu
-00026db0: 7420 6e6f 7420 6066 696c 7465 7260 292e  t not `filter`).
-00026dc0: 0a2d 2060 6c65 6e60 2028 616c 6c20 6275  .- `len` (all bu
-00026dd0: 7420 6066 696c 7465 7260 2920 2874 686f  t `filter`) (tho
-00026de0: 7567 6820 6062 6f6f 6c60 2077 696c 6c20  ugh `bool` will 
-00026df0: 7374 696c 6c20 616c 7761 7973 2079 6965  still always yie
-00026e00: 6c64 2060 5472 7565 6029 2e0a 2d20 5468  ld `True`)..- Th
-00026e10: 6520 6162 696c 6974 7920 746f 2062 6520  e ability to be 
-00026e20: 6974 6572 6174 6564 206f 7665 7220 6d75  iterated over mu
-00026e30: 6c74 6970 6c65 2074 696d 6573 2069 6620  ltiple times if 
-00026e40: 7468 6520 756e 6465 726c 7969 6e67 2069  the underlying i
-00026e50: 7465 7261 746f 7273 2063 616e 2062 6520  terators can be 
-00026e60: 6974 6572 6174 6564 206f 7665 7220 6d75  iterated over mu
-00026e70: 6c74 6970 6c65 2074 696d 6573 2e0a 2d20  ltiple times..- 
-00026e80: 5b50 4550 2036 3138 5d28 6874 7470 733a  [PEP 618](https:
-00026e90: 2f2f 7777 772e 7079 7468 6f6e 2e6f 7267  //www.python.org
-00026ea0: 2f64 6576 2f70 6570 732f 7065 702d 3036  /dev/peps/pep-06
-00026eb0: 3138 2920 607a 6970 282e 2e2e 2c20 7374  18) `zip(..., st
-00026ec0: 7269 6374 3d54 7275 6529 6020 7375 7070  rict=True)` supp
-00026ed0: 6f72 7420 6f6e 2061 6c6c 2050 7974 686f  ort on all Pytho
-00026ee0: 6e20 7665 7273 696f 6e73 2e0a 2d20 4164  n versions..- Ad
-00026ef0: 6465 6420 6073 7472 6963 743d 5472 7565  ded `strict=True
-00026f00: 6020 7375 7070 6f72 7420 746f 2060 6d61  ` support to `ma
-00026f10: 7060 2061 7320 7765 6c6c 2028 656e 666f  p` as well (enfo
-00026f20: 7263 6573 2074 6861 7420 6974 6572 6162  rces that iterab
-00026f30: 6c65 7320 6172 6520 7468 6520 7361 6d65  les are the same
-00026f40: 206c 656e 6774 6820 696e 2074 6865 206d   length in the m
-00026f50: 756c 7469 2d69 7465 7261 626c 6520 6361  ulti-iterable ca
-00026f60: 7365 3b20 7573 6573 2060 7a69 7060 2075  se; uses `zip` u
-00026f70: 6e64 6572 2074 6865 2068 6f6f 6420 7375  nder the hood su
-00026f80: 6368 2074 6861 7420 6572 726f 7273 2077  ch that errors w
-00026f90: 696c 6c20 7368 6f77 2075 7020 6173 2060  ill show up as `
-00026fa0: 7a69 7028 2e2e 2e2c 2073 7472 6963 743d  zip(..., strict=
-00026fb0: 5472 7565 2960 2065 7272 6f72 7329 2e0a  True)` errors)..
-00026fc0: 2d20 4164 6465 6420 6174 7472 6962 7574  - Added attribut
-00026fd0: 6573 2077 6869 6368 2073 7562 636c 6173  es which subclas
-00026fe0: 7365 7320 6361 6e20 6d61 6b65 2075 7365  ses can make use
-00026ff0: 206f 6620 746f 2067 6574 2061 7420 7468   of to get at th
-00027000: 6520 6f72 6967 696e 616c 2061 7267 756d  e original argum
-00027010: 656e 7473 2074 6f20 7468 6520 6f62 6a65  ents to the obje
-00027020: 6374 3a0a 2020 2a20 606d 6170 603a 2060  ct:.  * `map`: `
-00027030: 6675 6e63 602c 2060 6974 6572 7360 0a20  func`, `iters`. 
-00027040: 202a 2060 7a69 7060 3a20 6069 7465 7273   * `zip`: `iters
-00027050: 600a 2020 2a20 6066 696c 7465 7260 3a20  `.  * `filter`: 
-00027060: 6066 756e 6360 2c20 6069 7465 7260 0a20  `func`, `iter`. 
-00027070: 202a 2060 7265 7665 7273 6564 603a 2060   * `reversed`: `
-00027080: 6974 6572 600a 2020 2a20 6065 6e75 6d65  iter`.  * `enume
-00027090: 7261 7465 603a 2060 6974 6572 602c 2060  rate`: `iter`, `
-000270a0: 7374 6172 7460 0a0a 2323 2323 2320 496e  start`..##### In
-000270b0: 6465 7869 6e67 2069 6e74 6f20 6f74 6865  dexing into othe
-000270c0: 7220 6275 696c 742d 696e 730a 0a54 686f  r built-ins..Tho
-000270d0: 7567 6820 436f 636f 6e75 7420 7072 6f76  ugh Coconut prov
-000270e0: 6964 6573 2072 616e 646f 6d20 6163 6365  ides random acce
-000270f0: 7373 2069 6e64 6578 696e 672f 736c 6963  ss indexing/slic
-00027100: 696e 6720 746f 2060 7261 6e67 6560 2c20  ing to `range`, 
-00027110: 606d 6170 602c 2060 7a69 7060 2c20 6072  `map`, `zip`, `r
-00027120: 6576 6572 7365 6460 2c20 616e 6420 6065  eversed`, and `e
-00027130: 6e75 6d65 7261 7465 602c 2043 6f63 6f6e  numerate`, Cocon
-00027140: 7574 2063 616e 6e6f 7420 696e 6465 7820  ut cannot index 
-00027150: 696e 746f 2062 7569 6c74 2d69 6e73 206c  into built-ins l
-00027160: 696b 6520 6066 696c 7465 7260 2c20 6074  ike `filter`, `t
-00027170: 616b 6577 6869 6c65 602c 206f 7220 6064  akewhile`, or `d
-00027180: 726f 7077 6869 6c65 6020 6469 7265 6374  ropwhile` direct
-00027190: 6c79 2c20 6173 2074 6865 7265 2069 7320  ly, as there is 
-000271a0: 6e6f 2065 6666 6963 6965 6e74 2077 6179  no efficient way
-000271b0: 2074 6f20 646f 2073 6f2e 0a0a 6060 6063   to do so...```c
-000271c0: 6f63 6f6e 7574 0a72 616e 6765 2831 3029  oconut.range(10)
-000271d0: 207c 3e20 6669 6c74 6572 2428 692d 3e69   |> filter$(i->i
-000271e0: 3e33 2920 7c3e 202e 5b30 5d20 2023 2064  >3) |> .[0]  # d
-000271f0: 6f65 736e 2774 2077 6f72 6b0a 6060 600a  oesn't work.```.
-00027200: 0a49 6e20 6f72 6465 7220 746f 206d 616b  .In order to mak
-00027210: 6520 7468 6973 2077 6f72 6b2c 2079 6f75  e this work, you
-00027220: 2063 616e 2065 7870 6c69 6369 746c 7920   can explicitly 
-00027230: 7573 6520 6974 6572 6174 6f72 2073 6c69  use iterator sli
-00027240: 6369 6e67 2c20 7768 6963 6820 6973 206c  cing, which is l
-00027250: 6573 7320 6566 6669 6369 656e 7420 696e  ess efficient in
-00027260: 2074 6865 2067 656e 6572 616c 2063 6173   the general cas
-00027270: 653a 0a0a 6060 6063 6f63 6f6e 7574 0a72  e:..```coconut.r
-00027280: 616e 6765 2831 3029 207c 3e20 6669 6c74  ange(10) |> filt
-00027290: 6572 2428 692d 3e69 3e33 2920 7c3e 202e  er$(i->i>3) |> .
-000272a0: 245b 305d 2020 2320 776f 726b 730a 6060  $[0]  # works.``
-000272b0: 600a 0a46 6f72 206d 6f72 6520 696e 666f  `..For more info
-000272c0: 726d 6174 696f 6e20 6f6e 2043 6f63 6f6e  rmation on Cocon
-000272d0: 7574 2773 2069 7465 7261 746f 7220 736c  ut's iterator sl
-000272e0: 6963 696e 672c 2073 6565 205b 6865 7265  icing, see [here
-000272f0: 5d28 2369 7465 7261 746f 722d 736c 6963  ](#iterator-slic
-00027300: 696e 6729 2e0a 0a23 2323 2323 2045 7861  ing)...##### Exa
-00027310: 6d70 6c65 730a 0a2a 2a43 6f63 6f6e 7574  mples..**Coconut
-00027320: 3a2a 2a0a 6060 6063 6f63 6f6e 7574 0a6d  :**.```coconut.m
-00027330: 6170 2828 2b29 2c20 7261 6e67 6528 3529  ap((+), range(5)
-00027340: 2c20 7261 6e67 6528 3629 2920 7c3e 206c  , range(6)) |> l
-00027350: 656e 207c 3e20 7072 696e 740a 7261 6e67  en |> print.rang
-00027360: 6528 3130 2920 7c3e 2066 696c 7465 7224  e(10) |> filter$
-00027370: 2828 7829 202d 3e20 7820 3c20 3529 207c  ((x) -> x < 5) |
-00027380: 3e20 7265 7665 7273 6564 207c 3e20 7475  > reversed |> tu
-00027390: 706c 6520 7c3e 2070 7269 6e74 0a60 6060  ple |> print.```
-000273a0: 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a 5f43  ..**Python:**._C
-000273b0: 616e 2774 2062 6520 646f 6e65 2077 6974  an't be done wit
-000273c0: 686f 7574 2064 6566 696e 696e 6720 6120  hout defining a 
-000273d0: 6375 7374 6f6d 2060 6d61 7060 2074 7970  custom `map` typ
-000273e0: 652e 2054 6865 2066 756c 6c20 6465 6669  e. The full defi
-000273f0: 6e69 7469 6f6e 206f 6620 606d 6170 6020  nition of `map` 
-00027400: 6361 6e20 6265 2066 6f75 6e64 2069 6e20  can be found in 
-00027410: 7468 6520 436f 636f 6e75 7420 6865 6164  the Coconut head
-00027420: 6572 2e5f 0a0a 2a2a 436f 636f 6e75 743a  er._..**Coconut:
-00027430: 2a2a 0a60 6060 636f 636f 6e75 740a 7261  **.```coconut.ra
-00027440: 6e67 6528 302c 2031 322c 2032 295b 345d  nge(0, 12, 2)[4]
-00027450: 2020 2320 380a 0a6d 6170 2828 692d 3e69    # 8..map((i->i
-00027460: 2a32 292c 2072 616e 6765 2831 3029 295b  *2), range(10))[
-00027470: 325d 2020 2320 340a 6060 600a 0a2a 2a50  2]  # 4.```..**P
-00027480: 7974 686f 6e3a 2a2a 0a5f 4361 6ee2 8099  ython:**._Can...
-00027490: 7420 6265 2064 6f6e 6520 7175 6963 6b6c  t be done quickl
-000274a0: 7920 7769 7468 6f75 7420 436f 636f 6e75  y without Coconu
-000274b0: 74e2 8099 7320 6974 6572 6162 6c65 2069  t...s iterable i
-000274c0: 6e64 6578 696e 672c 2077 6869 6368 2072  ndexing, which r
-000274d0: 6571 7569 7265 7320 6d61 6e79 2063 6f6d  equires many com
-000274e0: 706c 6963 6174 6564 2070 6965 6365 732e  plicated pieces.
-000274f0: 2054 6865 206e 6563 6573 7361 7279 2064   The necessary d
-00027500: 6566 696e 6974 696f 6e73 2069 6e20 5079  efinitions in Py
-00027510: 7468 6f6e 2063 616e 2062 6520 666f 756e  thon can be foun
-00027520: 6420 696e 2074 6865 2043 6f63 6f6e 7574  d in the Coconut
-00027530: 2068 6561 6465 722e 5f0a 0a23 2323 2320   header._..#### 
-00027540: 6072 6564 7563 6560 0a0a 2a2a 7265 6475  `reduce`..**redu
-00027550: 6365 2a2a 285f 6675 6e63 7469 6f6e 5f2c  ce**(_function_,
-00027560: 205f 6974 6572 6162 6c65 5f5b 2c20 5f69   _iterable_[, _i
-00027570: 6e69 7469 616c 5f5d 2c20 2f29 0a0a 436f  nitial_], /)..Co
-00027580: 636f 6e75 7420 7265 2d69 6e74 726f 6475  conut re-introdu
-00027590: 6365 7320 5079 7468 6f6e 2032 2773 2060  ces Python 2's `
-000275a0: 7265 6475 6365 6020 6275 696c 742d 696e  reduce` built-in
-000275b0: 2c20 7573 696e 6720 7468 6520 6066 756e  , using the `fun
-000275c0: 6374 6f6f 6c73 2e72 6564 7563 6560 2076  ctools.reduce` v
-000275d0: 6572 7369 6f6e 2e0a 0a23 2323 2323 2050  ersion...##### P
-000275e0: 7974 686f 6e20 446f 6373 0a0a 2a2a 7265  ython Docs..**re
-000275f0: 6475 6365 2a2a 285f 6675 6e63 7469 6f6e  duce**(_function
-00027600: 2c20 6974 6572 6162 6c65 5f2a 2a5b 2a2a  , iterable_**[**
-00027610: 5f2c 2069 6e69 7469 616c 5f2a 2a5d 2a2a  _, initial_**]**
-00027620: 290a 0a41 7070 6c79 205f 6675 6e63 7469  )..Apply _functi
-00027630: 6f6e 5f20 6f66 2074 776f 2061 7267 756d  on_ of two argum
-00027640: 656e 7473 2063 756d 756c 6174 6976 656c  ents cumulativel
-00027650: 7920 746f 2074 6865 2069 7465 6d73 206f  y to the items o
-00027660: 6620 5f73 6571 7565 6e63 655f 2c20 6672  f _sequence_, fr
-00027670: 6f6d 206c 6566 7420 746f 2072 6967 6874  om left to right
-00027680: 2c20 736f 2061 7320 746f 2072 6564 7563  , so as to reduc
-00027690: 6520 7468 6520 7365 7175 656e 6365 2074  e the sequence t
-000276a0: 6f20 6120 7369 6e67 6c65 2076 616c 7565  o a single value
-000276b0: 2e20 466f 7220 6578 616d 706c 652c 2060  . For example, `
-000276c0: 7265 6475 6365 2828 782c 2079 2920 2d3e  reduce((x, y) ->
-000276d0: 2078 2b79 2c20 5b31 2c20 322c 2033 2c20   x+y, [1, 2, 3, 
-000276e0: 342c 2035 5d29 6020 6361 6c63 756c 6174  4, 5])` calculat
-000276f0: 6573 2060 2828 2828 312b 3229 2b33 292b  es `((((1+2)+3)+
-00027700: 3429 2b35 2960 2e20 5468 6520 6c65 6674  4)+5)`. The left
-00027710: 2061 7267 756d 656e 742c 205f 785f 2c20   argument, _x_, 
-00027720: 6973 2074 6865 2061 6363 756d 756c 6174  is the accumulat
-00027730: 6564 2076 616c 7565 2061 6e64 2074 6865  ed value and the
-00027740: 2072 6967 6874 2061 7267 756d 656e 742c   right argument,
-00027750: 205f 795f 2c20 6973 2074 6865 2075 7064   _y_, is the upd
-00027760: 6174 6520 7661 6c75 6520 6672 6f6d 2074  ate value from t
-00027770: 6865 205f 7365 7175 656e 6365 5f2e 2049  he _sequence_. I
-00027780: 6620 7468 6520 6f70 7469 6f6e 616c 205f  f the optional _
-00027790: 696e 6974 6961 6c5f 2069 7320 7072 6573  initial_ is pres
-000277a0: 656e 742c 2069 7420 6973 2070 6c61 6365  ent, it is place
-000277b0: 6420 6265 666f 7265 2074 6865 2069 7465  d before the ite
-000277c0: 6d73 206f 6620 7468 6520 7365 7175 656e  ms of the sequen
-000277d0: 6365 2069 6e20 7468 6520 6361 6c63 756c  ce in the calcul
-000277e0: 6174 696f 6e2c 2061 6e64 2073 6572 7665  ation, and serve
-000277f0: 7320 6173 2061 2064 6566 6175 6c74 2077  s as a default w
-00027800: 6865 6e20 7468 6520 7365 7175 656e 6365  hen the sequence
-00027810: 2069 7320 656d 7074 792e 2049 6620 5f69   is empty. If _i
-00027820: 6e69 7469 616c 5f20 6973 206e 6f74 2067  nitial_ is not g
-00027830: 6976 656e 2061 6e64 205f 7365 7175 656e  iven and _sequen
-00027840: 6365 5f20 636f 6e74 6169 6e73 206f 6e6c  ce_ contains onl
-00027850: 7920 6f6e 6520 6974 656d 2c20 7468 6520  y one item, the 
-00027860: 6669 7273 7420 6974 656d 2069 7320 7265  first item is re
-00027870: 7475 726e 6564 2e0a 0a23 2323 2323 2045  turned...##### E
-00027880: 7861 6d70 6c65 0a0a 2a2a 436f 636f 6e75  xample..**Coconu
-00027890: 743a 2a2a 0a60 6060 636f 636f 6e75 740a  t:**.```coconut.
-000278a0: 7072 6f64 7563 7420 3d20 7265 6475 6365  product = reduce
-000278b0: 2428 2a29 0a72 616e 6765 2831 2c20 3130  $(*).range(1, 10
-000278c0: 2920 7c3e 2070 726f 6475 6374 207c 3e20  ) |> product |> 
-000278d0: 7072 696e 740a 6060 600a 0a2a 2a50 7974  print.```..**Pyt
-000278e0: 686f 6e3a 2a2a 0a60 6060 636f 636f 6e75  hon:**.```coconu
-000278f0: 745f 7079 7468 6f6e 0a69 6d70 6f72 7420  t_python.import 
-00027900: 6f70 6572 6174 6f72 0a69 6d70 6f72 7420  operator.import 
-00027910: 6675 6e63 746f 6f6c 730a 7072 6f64 7563  functools.produc
-00027920: 7420 3d20 6675 6e63 746f 6f6c 732e 7061  t = functools.pa
-00027930: 7274 6961 6c28 6675 6e63 746f 6f6c 732e  rtial(functools.
-00027940: 7265 6475 6365 2c20 6f70 6572 6174 6f72  reduce, operator
-00027950: 2e6d 756c 290a 7072 696e 7428 7072 6f64  .mul).print(prod
-00027960: 7563 7428 7261 6e67 6528 312c 2031 3029  uct(range(1, 10)
-00027970: 2929 0a60 6060 0a0a 2323 2323 2060 7265  )).```..#### `re
-00027980: 6974 6572 6162 6c65 600a 0a2a 2a72 6569  iterable`..**rei
-00027990: 7465 7261 626c 652a 2a28 5f69 7465 7261  terable**(_itera
-000279a0: 626c 655f 290a 0a60 7265 6974 6572 6162  ble_)..`reiterab
-000279b0: 6c65 6020 7772 6170 7320 7468 6520 6769  le` wraps the gi
-000279c0: 7665 6e20 6974 6572 6162 6c65 2074 6f20  ven iterable to 
-000279d0: 656e 7375 7265 2074 6861 7420 6576 6572  ensure that ever
-000279e0: 7920 7469 6d65 2074 6865 2060 7265 6974  y time the `reit
-000279f0: 6572 6162 6c65 6020 6973 2069 7465 7261  erable` is itera
-00027a00: 7465 6420 6f76 6572 2c20 6974 2070 726f  ted over, it pro
-00027a10: 6475 6365 7320 7468 6520 7361 6d65 2072  duces the same r
-00027a20: 6573 756c 7473 2e20 4e6f 7465 2074 6861  esults. Note tha
-00027a30: 7420 7468 6520 7265 7375 6c74 206e 6565  t the result nee
-00027a40: 6420 6e6f 7420 6265 2061 2060 7265 6974  d not be a `reit
-00027a50: 6572 6162 6c65 6020 6f62 6a65 6374 2069  erable` object i
-00027a60: 6620 7468 6520 6769 7665 6e20 6974 6572  f the given iter
-00027a70: 6162 6c65 2069 7320 616c 7265 6164 7920  able is already 
-00027a80: 7265 6974 6572 6162 6c65 2e20 6072 6569  reiterable. `rei
-00027a90: 7465 7261 626c 6560 2075 7365 7320 5b60  terable` uses [`
-00027aa0: 7465 6560 5d28 2374 6565 2920 756e 6465  tee`](#tee) unde
-00027ab0: 7220 7468 6520 686f 6f64 2061 6e64 2060  r the hood and `
-00027ac0: 7465 6560 2063 616e 2062 6520 7573 6564  tee` can be used
-00027ad0: 2069 6e20 6974 7320 706c 6163 652c 2074   in its place, t
-00027ae0: 686f 7567 6820 6072 6569 7465 7261 626c  hough `reiterabl
-00027af0: 6560 2069 7320 6765 6e65 7261 6c6c 7920  e` is generally 
-00027b00: 7265 636f 6d6d 656e 6465 6420 6f76 6572  recommended over
-00027b10: 2060 7465 6560 2e0a 0a23 2323 2323 2045   `tee`...##### E
-00027b20: 7861 6d70 6c65 0a0a 2a2a 436f 636f 6e75  xample..**Coconu
-00027b30: 743a 2a2a 0a60 6060 636f 636f 6e75 740a  t:**.```coconut.
-00027b40: 6465 6620 6c69 7374 5f74 7970 6528 7873  def list_type(xs
-00027b50: 293a 0a20 2020 206d 6174 6368 2072 6569  ):.    match rei
-00027b60: 7465 7261 626c 6528 7873 293a 0a20 2020  terable(xs):.   
-00027b70: 2020 2020 2063 6173 6520 5b66 7374 2c20       case [fst, 
-00027b80: 736e 645d 203a 3a20 7461 696c 3a0a 2020  snd] :: tail:.  
-00027b90: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00027ba0: 2022 6174 206c 6561 7374 2032 220a 2020   "at least 2".  
-00027bb0: 2020 2020 2020 6361 7365 205b 6673 745d        case [fst]
-00027bc0: 203a 3a20 7461 696c 3a0a 2020 2020 2020   :: tail:.      
-00027bd0: 2020 2020 2020 7265 7475 726e 2022 6174        return "at
-00027be0: 206c 6561 7374 2031 220a 2020 2020 2020   least 1".      
-00027bf0: 2020 6361 7365 2028 7c20 7c29 3a0a 2020    case (| |):.  
-00027c00: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00027c10: 2022 656d 7074 7922 0a60 6060 0a0a 2a2a   "empty".```..**
-00027c20: 5079 7468 6f6e 3a2a 2a0a 5f43 616e 2774  Python:**._Can't
-00027c30: 2062 6520 646f 6e65 2077 6974 686f 7574   be done without
-00027c40: 2061 206c 6f6e 6720 7365 7269 6573 206f   a long series o
-00027c50: 6620 6368 6563 6b73 2066 6f72 2065 6163  f checks for eac
-00027c60: 6820 606d 6174 6368 6020 7374 6174 656d  h `match` statem
-00027c70: 656e 742e 2053 6565 2074 6865 2063 6f6d  ent. See the com
-00027c80: 7069 6c65 6420 636f 6465 2066 6f72 2074  piled code for t
-00027c90: 6865 2050 7974 686f 6e20 7379 6e74 6178  he Python syntax
-00027ca0: 2e5f 0a0a 2323 2323 2060 7374 6172 6d61  ._..#### `starma
-00027cb0: 7060 0a0a 2a2a 7374 6172 6d61 702a 2a28  p`..**starmap**(
-00027cc0: 5f66 756e 6374 696f 6e5f 2c20 5f69 7465  _function_, _ite
-00027cd0: 7261 626c 655f 290a 0a43 6f63 6f6e 7574  rable_)..Coconut
-00027ce0: 2070 726f 7669 6465 7320 6120 6d6f 6469   provides a modi
-00027cf0: 6669 6564 2076 6572 7369 6f6e 206f 6620  fied version of 
-00027d00: 6069 7465 7274 6f6f 6c73 2e73 7461 726d  `itertools.starm
-00027d10: 6170 6020 7468 6174 2073 7570 706f 7274  ap` that support
-00027d20: 7320 6072 6576 6572 7365 6460 2c20 6072  s `reversed`, `r
-00027d30: 6570 7260 2c20 6f70 7469 6d69 7a65 6420  epr`, optimized 
-00027d40: 6e6f 726d 616c 2028 616e 6420 6974 6572  normal (and iter
-00027d50: 6174 6f72 2920 736c 6963 696e 672c 2060  ator) slicing, `
-00027d60: 6c65 6e60 2c20 616e 6420 6066 756e 6360  len`, and `func`
-00027d70: 2f60 6974 6572 6020 6174 7472 6962 7574  /`iter` attribut
-00027d80: 6573 2e0a 0a23 2323 2323 2050 7974 686f  es...##### Pytho
-00027d90: 6e20 446f 6373 0a0a 2a2a 7374 6172 6d61  n Docs..**starma
-00027da0: 702a 2a28 5f66 756e 6374 696f 6e2c 2069  p**(_function, i
-00027db0: 7465 7261 626c 655f 290a 0a4d 616b 6520  terable_)..Make 
-00027dc0: 616e 2069 7465 7261 746f 7220 7468 6174  an iterator that
-00027dd0: 2063 6f6d 7075 7465 7320 7468 6520 6675   computes the fu
-00027de0: 6e63 7469 6f6e 2075 7369 6e67 2061 7267  nction using arg
-00027df0: 756d 656e 7473 206f 6274 6169 6e65 6420  uments obtained 
-00027e00: 6672 6f6d 2074 6865 2069 7465 7261 626c  from the iterabl
-00027e10: 652e 2055 7365 6420 696e 7374 6561 6420  e. Used instead 
-00027e20: 6f66 2060 6d61 7028 2960 2077 6865 6e20  of `map()` when 
-00027e30: 6172 6775 6d65 6e74 2070 6172 616d 6574  argument paramet
-00027e40: 6572 7320 6172 6520 616c 7265 6164 7920  ers are already 
-00027e50: 6772 6f75 7065 6420 696e 2074 7570 6c65  grouped in tuple
-00027e60: 7320 6672 6f6d 2061 2073 696e 676c 6520  s from a single 
-00027e70: 6974 6572 6162 6c65 2028 7468 6520 6461  iterable (the da
-00027e80: 7461 2068 6173 2062 6565 6e20 2270 7265  ta has been "pre
-00027e90: 2d7a 6970 7065 6422 292e 2054 6865 2064  -zipped"). The d
-00027ea0: 6966 6665 7265 6e63 6520 6265 7477 6565  ifference betwee
-00027eb0: 6e20 606d 6170 2829 6020 616e 6420 6073  n `map()` and `s
-00027ec0: 7461 726d 6170 2829 6020 7061 7261 6c6c  tarmap()` parall
-00027ed0: 656c 7320 7468 6520 6469 7374 696e 6374  els the distinct
-00027ee0: 696f 6e20 6265 7477 6565 6e20 6066 756e  ion between `fun
-00027ef0: 6374 696f 6e28 612c 6229 6020 616e 6420  ction(a,b)` and 
-00027f00: 6066 756e 6374 696f 6e28 2a63 2960 2e20  `function(*c)`. 
-00027f10: 526f 7567 686c 7920 6571 7569 7661 6c65  Roughly equivale
-00027f20: 6e74 2074 6f3a 0a0a 6060 6063 6f63 6f6e  nt to:..```cocon
-00027f30: 7574 5f70 7974 686f 6e0a 6465 6620 7374  ut_python.def st
-00027f40: 6172 6d61 7028 6675 6e63 7469 6f6e 2c20  armap(function, 
-00027f50: 6974 6572 6162 6c65 293a 0a20 2020 2023  iterable):.    #
-00027f60: 2073 7461 726d 6170 2870 6f77 2c20 5b28   starmap(pow, [(
-00027f70: 322c 3529 2c20 2833 2c32 292c 2028 3130  2,5), (3,2), (10
-00027f80: 2c33 295d 2920 2d2d 3e20 3332 2039 2031  ,3)]) --> 32 9 1
-00027f90: 3030 300a 2020 2020 666f 7220 6172 6773  000.    for args
-00027fa0: 2069 6e20 6974 6572 6162 6c65 3a0a 2020   in iterable:.  
-00027fb0: 2020 2020 2020 7969 656c 6420 6675 6e63        yield func
-00027fc0: 7469 6f6e 282a 6172 6773 290a 6060 600a  tion(*args).```.
-00027fd0: 0a23 2323 2323 2045 7861 6d70 6c65 0a0a  .##### Example..
-00027fe0: 2a2a 436f 636f 6e75 743a 2a2a 0a60 6060  **Coconut:**.```
-00027ff0: 636f 636f 6e75 740a 7261 6e67 6528 312c  coconut.range(1,
-00028000: 2035 2920 7c3e 206d 6170 2428 7261 6e67   5) |> map$(rang
-00028010: 6529 207c 3e20 7374 6172 6d61 7024 2870  e) |> starmap$(p
-00028020: 7269 6e74 2920 7c3e 2063 6f6e 7375 6d65  rint) |> consume
-00028030: 0a60 6060 0a0a 2a2a 5079 7468 6f6e 3a2a  .```..**Python:*
-00028040: 2a0a 6060 6063 6f63 6f6e 7574 5f70 7974  *.```coconut_pyt
-00028050: 686f 6e0a 696d 706f 7274 2069 7465 7274  hon.import itert
-00028060: 6f6f 6c73 2c20 636f 6c6c 6563 7469 6f6e  ools, collection
-00028070: 730a 636f 6c6c 6563 7469 6f6e 732e 6465  s.collections.de
-00028080: 7175 6528 6974 6572 746f 6f6c 732e 7374  que(itertools.st
-00028090: 6172 6d61 7028 7072 696e 742c 206d 6170  armap(print, map
-000280a0: 2872 616e 6765 2c20 7261 6e67 6528 312c  (range, range(1,
-000280b0: 2035 2929 292c 206d 6178 6c65 6e3d 3029   5))), maxlen=0)
-000280c0: 0a60 6060 0a0a 2323 2323 2060 7a69 705f  .```..#### `zip_
-000280d0: 6c6f 6e67 6573 7460 0a0a 2a2a 7a69 705c  longest`..**zip\
-000280e0: 5f6c 6f6e 6765 7374 2a2a 282a 5f69 7465  _longest**(*_ite
-000280f0: 7261 626c 6573 5f2c 205f 6669 6c6c 7661  rables_, _fillva
-00028100: 6c75 655f 3d60 4e6f 6e65 6029 0a0a 436f  lue_=`None`)..Co
-00028110: 636f 6e75 7420 7072 6f76 6964 6573 2061  conut provides a
-00028120: 6e20 656e 6861 6e63 6564 2076 6572 7369  n enhanced versi
-00028130: 6f6e 206f 6620 6069 7465 7274 6f6f 6c73  on of `itertools
-00028140: 2e7a 6970 5f6c 6f6e 6765 7374 6020 6173  .zip_longest` as
-00028150: 2061 2062 7569 6c74 2d69 6e20 756e 6465   a built-in unde
-00028160: 7220 7468 6520 6e61 6d65 2060 7a69 705f  r the name `zip_
-00028170: 6c6f 6e67 6573 7460 2e20 607a 6970 5f6c  longest`. `zip_l
-00028180: 6f6e 6765 7374 6020 7375 7070 6f72 7473  ongest` supports
-00028190: 2061 6c6c 2074 6865 2073 616d 6520 6665   all the same fe
-000281a0: 6174 7572 6573 2061 7320 436f 636f 6e75  atures as Coconu
-000281b0: 7427 7320 5b65 6e68 616e 6365 6420 7a69  t's [enhanced zi
-000281c0: 705d 2823 656e 6861 6e63 6564 2d62 7569  p](#enhanced-bui
-000281d0: 6c74 2d69 6e73 2920 6173 2077 656c 6c20  lt-ins) as well 
-000281e0: 6173 2074 6865 2061 6464 6974 696f 6e61  as the additiona
-000281f0: 6c20 6174 7472 6962 7574 6520 6066 696c  l attribute `fil
-00028200: 6c76 616c 7565 602e 0a0a 2323 2323 2320  lvalue`...##### 
-00028210: 5079 7468 6f6e 2044 6f63 730a 0a2a 2a7a  Python Docs..**z
-00028220: 6970 5c5f 6c6f 6e67 6573 742a 2a28 5f5c  ip\_longest**(_\
-00028230: 2a69 7465 7261 626c 6573 2c20 6669 6c6c  *iterables, fill
-00028240: 7661 6c75 653d 4e6f 6e65 5f29 0a0a 4d61  value=None_)..Ma
-00028250: 6b65 2061 6e20 6974 6572 6174 6f72 2074  ke an iterator t
-00028260: 6861 7420 6167 6772 6567 6174 6573 2065  hat aggregates e
-00028270: 6c65 6d65 6e74 7320 6672 6f6d 2065 6163  lements from eac
-00028280: 6820 6f66 2074 6865 2069 7465 7261 626c  h of the iterabl
-00028290: 6573 2e20 4966 2074 6865 2069 7465 7261  es. If the itera
-000282a0: 626c 6573 2061 7265 206f 6620 756e 6576  bles are of unev
-000282b0: 656e 206c 656e 6774 682c 206d 6973 7369  en length, missi
-000282c0: 6e67 2076 616c 7565 7320 6172 6520 6669  ng values are fi
-000282d0: 6c6c 6564 2d69 6e20 7769 7468 205f 6669  lled-in with _fi
-000282e0: 6c6c 7661 6c75 655f 2e20 4974 6572 6174  llvalue_. Iterat
-000282f0: 696f 6e20 636f 6e74 696e 7565 7320 756e  ion continues un
-00028300: 7469 6c20 7468 6520 6c6f 6e67 6573 7420  til the longest 
-00028310: 6974 6572 6162 6c65 2069 7320 6578 6861  iterable is exha
-00028320: 7573 7465 642e 2052 6f75 6768 6c79 2065  usted. Roughly e
-00028330: 7175 6976 616c 656e 7420 746f 3a0a 0a60  quivalent to:..`
-00028340: 6060 636f 636f 6e75 745f 7079 7468 6f6e  ``coconut_python
-00028350: 0a64 6566 207a 6970 5f6c 6f6e 6765 7374  .def zip_longest
-00028360: 282a 6172 6773 2c20 6669 6c6c 7661 6c75  (*args, fillvalu
-00028370: 653d 4e6f 6e65 293a 0a20 2020 2023 207a  e=None):.    # z
-00028380: 6970 5f6c 6f6e 6765 7374 2827 4142 4344  ip_longest('ABCD
-00028390: 272c 2027 7879 272c 2066 696c 6c76 616c  ', 'xy', fillval
-000283a0: 7565 3d27 2d27 2920 2d2d 3e20 4178 2042  ue='-') --> Ax B
-000283b0: 7920 432d 2044 2d0a 2020 2020 6974 6572  y C- D-.    iter
-000283c0: 6174 6f72 7320 3d20 5b69 7465 7228 6974  ators = [iter(it
-000283d0: 2920 666f 7220 6974 2069 6e20 6172 6773  ) for it in args
-000283e0: 5d0a 2020 2020 6e75 6d5f 6163 7469 7665  ].    num_active
-000283f0: 203d 206c 656e 2869 7465 7261 746f 7273   = len(iterators
-00028400: 290a 2020 2020 6966 206e 6f74 206e 756d  ).    if not num
-00028410: 5f61 6374 6976 653a 0a20 2020 2020 2020  _active:.       
-00028420: 2072 6574 7572 6e0a 2020 2020 7768 696c   return.    whil
-00028430: 6520 5472 7565 3a0a 2020 2020 2020 2020  e True:.        
-00028440: 7661 6c75 6573 203d 205b 5d0a 2020 2020  values = [].    
-00028450: 2020 2020 666f 7220 692c 2069 7420 696e      for i, it in
-00028460: 2065 6e75 6d65 7261 7465 2869 7465 7261   enumerate(itera
-00028470: 746f 7273 293a 0a20 2020 2020 2020 2020  tors):.         
-00028480: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00028490: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-000284a0: 6e65 7874 2869 7429 0a20 2020 2020 2020  next(it).       
-000284b0: 2020 2020 2065 7863 6570 7420 5374 6f70       except Stop
-000284c0: 4974 6572 6174 696f 6e3a 0a20 2020 2020  Iteration:.     
-000284d0: 2020 2020 2020 2020 2020 206e 756d 5f61             num_a
-000284e0: 6374 6976 6520 2d3d 2031 0a20 2020 2020  ctive -= 1.     
-000284f0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00028500: 7420 6e75 6d5f 6163 7469 7665 3a0a 2020  t num_active:.  
-00028510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028520: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00028530: 2020 2020 2020 2020 2069 7465 7261 746f           iterato
-00028540: 7273 5b69 5d20 3d20 7265 7065 6174 2866  rs[i] = repeat(f
-00028550: 696c 6c76 616c 7565 290a 2020 2020 2020  illvalue).      
-00028560: 2020 2020 2020 2020 2020 7661 6c75 6520            value 
-00028570: 3d20 6669 6c6c 7661 6c75 650a 2020 2020  = fillvalue.    
-00028580: 2020 2020 2020 2020 7661 6c75 6573 2e61          values.a
-00028590: 7070 656e 6428 7661 6c75 6529 0a20 2020  ppend(value).   
-000285a0: 2020 2020 2079 6965 6c64 2074 7570 6c65       yield tuple
-000285b0: 2876 616c 7565 7329 0a60 6060 0a0a 4966  (values).```..If
-000285c0: 206f 6e65 206f 6620 7468 6520 6974 6572   one of the iter
-000285d0: 6162 6c65 7320 6973 2070 6f74 656e 7469  ables is potenti
-000285e0: 616c 6c79 2069 6e66 696e 6974 652c 2074  ally infinite, t
-000285f0: 6865 6e20 7468 6520 607a 6970 5f6c 6f6e  hen the `zip_lon
-00028600: 6765 7374 2829 6020 6675 6e63 7469 6f6e  gest()` function
-00028610: 2073 686f 756c 6420 6265 2077 7261 7070   should be wrapp
-00028620: 6564 2077 6974 6820 736f 6d65 7468 696e  ed with somethin
-00028630: 6720 7468 6174 206c 696d 6974 7320 7468  g that limits th
-00028640: 6520 6e75 6d62 6572 206f 6620 6361 6c6c  e number of call
-00028650: 7320 2866 6f72 2065 7861 6d70 6c65 2069  s (for example i
-00028660: 7465 7261 746f 7220 736c 6963 696e 6720  terator slicing 
-00028670: 6f72 2060 7461 6b65 7768 696c 6560 292e  or `takewhile`).
-00028680: 2049 6620 6e6f 7420 7370 6563 6966 6965   If not specifie
-00028690: 642c 205f 6669 6c6c 7661 6c75 655f 2064  d, _fillvalue_ d
-000286a0: 6566 6175 6c74 7320 746f 2060 4e6f 6e65  efaults to `None
-000286b0: 602e 0a0a 2323 2323 2320 4578 616d 706c  `...##### Exampl
-000286c0: 650a 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a  e..**Coconut:**.
-000286d0: 6060 6063 6f63 6f6e 7574 0a72 6573 756c  ```coconut.resul
-000286e0: 7420 3d20 7a69 705f 6c6f 6e67 6573 7428  t = zip_longest(
-000286f0: 7261 6e67 6528 3529 2c20 7261 6e67 6528  range(5), range(
-00028700: 3130 2929 0a60 6060 0a0a 2a2a 5079 7468  10)).```..**Pyth
-00028710: 6f6e 3a2a 2a0a 6060 6063 6f63 6f6e 7574  on:**.```coconut
-00028720: 5f70 7974 686f 6e0a 696d 706f 7274 2069  _python.import i
-00028730: 7465 7274 6f6f 6c73 0a72 6573 756c 7420  tertools.result 
-00028740: 3d20 6974 6572 746f 6f6c 732e 7a69 705f  = itertools.zip_
-00028750: 6c6f 6e67 6573 7428 7261 6e67 6528 3529  longest(range(5)
-00028760: 2c20 7261 6e67 6528 3130 2929 0a60 6060  , range(10)).```
-00028770: 0a0a 2323 2323 2060 7461 6b65 7768 696c  ..#### `takewhil
-00028780: 6560 0a0a 2a2a 7461 6b65 7768 696c 652a  e`..**takewhile*
-00028790: 2a28 5f70 7265 6469 6361 7465 5f2c 205f  *(_predicate_, _
-000287a0: 6974 6572 6162 6c65 5f2c 202f 290a 0a43  iterable_, /)..C
-000287b0: 6f63 6f6e 7574 2070 726f 7669 6465 7320  oconut provides 
-000287c0: 6069 7465 7274 6f6f 6c73 2e74 616b 6577  `itertools.takew
-000287d0: 6869 6c65 6020 6173 2061 2062 7569 6c74  hile` as a built
-000287e0: 2d69 6e20 756e 6465 7220 7468 6520 6e61  -in under the na
-000287f0: 6d65 2060 7461 6b65 7768 696c 6560 2e0a  me `takewhile`..
-00028800: 0a23 2323 2323 2050 7974 686f 6e20 446f  .##### Python Do
-00028810: 6373 0a0a 2a2a 7461 6b65 7768 696c 652a  cs..**takewhile*
-00028820: 2a28 5f70 7265 6469 6361 7465 2c20 6974  *(_predicate, it
-00028830: 6572 6162 6c65 5f29 0a0a 4d61 6b65 2061  erable_)..Make a
-00028840: 6e20 6974 6572 6174 6f72 2074 6861 7420  n iterator that 
-00028850: 7265 7475 726e 7320 656c 656d 656e 7473  returns elements
-00028860: 2066 726f 6d20 7468 6520 5f69 7465 7261   from the _itera
-00028870: 626c 655f 2061 7320 6c6f 6e67 2061 7320  ble_ as long as 
-00028880: 7468 6520 5f70 7265 6469 6361 7465 5f20  the _predicate_ 
-00028890: 6973 2074 7275 652e 2045 7175 6976 616c  is true. Equival
-000288a0: 656e 7420 746f 3a0a 6060 6063 6f63 6f6e  ent to:.```cocon
-000288b0: 7574 5f70 7974 686f 6e0a 6465 6620 7461  ut_python.def ta
-000288c0: 6b65 7768 696c 6528 7072 6564 6963 6174  kewhile(predicat
-000288d0: 652c 2069 7465 7261 626c 6529 3a0a 2020  e, iterable):.  
-000288e0: 2020 2320 7461 6b65 7768 696c 6528 6c61    # takewhile(la
-000288f0: 6d62 6461 2078 3a20 783c 352c 205b 312c  mbda x: x<5, [1,
-00028900: 342c 362c 342c 315d 2920 2d2d 3e20 3120  4,6,4,1]) --> 1 
-00028910: 340a 2020 2020 666f 7220 7820 696e 2069  4.    for x in i
-00028920: 7465 7261 626c 653a 0a20 2020 2020 2020  terable:.       
-00028930: 2069 6620 7072 6564 6963 6174 6528 7829   if predicate(x)
-00028940: 3a0a 2020 2020 2020 2020 2020 2020 7969  :.            yi
-00028950: 656c 6420 780a 2020 2020 2020 2020 656c  eld x.        el
-00028960: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00028970: 6272 6561 6b0a 6060 600a 0a23 2323 2323  break.```..#####
-00028980: 2045 7861 6d70 6c65 0a0a 2a2a 436f 636f   Example..**Coco
-00028990: 6e75 743a 2a2a 0a60 6060 636f 636f 6e75  nut:**.```coconu
-000289a0: 740a 6e65 6761 7469 7665 7320 3d20 6e75  t.negatives = nu
-000289b0: 6d69 7465 7220 7c3e 2074 616b 6577 6869  miter |> takewhi
-000289c0: 6c65 2428 7820 2d3e 2078 203c 2030 290a  le$(x -> x < 0).
-000289d0: 6060 600a 0a2a 2a50 7974 686f 6e3a 2a2a  ```..**Python:**
-000289e0: 0a60 6060 636f 636f 6e75 745f 7079 7468  .```coconut_pyth
-000289f0: 6f6e 0a69 6d70 6f72 7420 6974 6572 746f  on.import iterto
-00028a00: 6f6c 730a 6e65 6761 7469 7665 7320 3d20  ols.negatives = 
-00028a10: 6974 6572 746f 6f6c 732e 7461 6b65 7768  itertools.takewh
-00028a20: 696c 6528 6c61 6d62 6461 2078 3a20 7820  ile(lambda x: x 
-00028a30: 3c20 302c 206e 756d 6974 6572 290a 6060  < 0, numiter).``
-00028a40: 600a 0a23 2323 2320 6064 726f 7077 6869  `..#### `dropwhi
-00028a50: 6c65 600a 0a2a 2a64 726f 7077 6869 6c65  le`..**dropwhile
-00028a60: 2a2a 285f 7072 6564 6963 6174 655f 2c20  **(_predicate_, 
-00028a70: 5f69 7465 7261 626c 655f 2c20 2f29 0a0a  _iterable_, /)..
-00028a80: 436f 636f 6e75 7420 7072 6f76 6964 6573  Coconut provides
-00028a90: 2060 6974 6572 746f 6f6c 732e 6472 6f70   `itertools.drop
-00028aa0: 7768 696c 6560 2061 7320 6120 6275 696c  while` as a buil
-00028ab0: 742d 696e 2075 6e64 6572 2074 6865 206e  t-in under the n
-00028ac0: 616d 6520 6064 726f 7077 6869 6c65 602e  ame `dropwhile`.
-00028ad0: 0a0a 2323 2323 2320 5079 7468 6f6e 2044  ..##### Python D
-00028ae0: 6f63 730a 0a2a 2a64 726f 7077 6869 6c65  ocs..**dropwhile
-00028af0: 2a2a 285f 7072 6564 6963 6174 652c 2069  **(_predicate, i
-00028b00: 7465 7261 626c 655f 290a 0a4d 616b 6520  terable_)..Make 
-00028b10: 616e 2069 7465 7261 746f 7220 7468 6174  an iterator that
-00028b20: 2064 726f 7073 2065 6c65 6d65 6e74 7320   drops elements 
-00028b30: 6672 6f6d 2074 6865 205f 6974 6572 6162  from the _iterab
-00028b40: 6c65 5f20 6173 206c 6f6e 6720 6173 2074  le_ as long as t
-00028b50: 6865 205f 7072 6564 6963 6174 655f 2069  he _predicate_ i
-00028b60: 7320 7472 7565 3b20 6166 7465 7277 6172  s true; afterwar
-00028b70: 6473 2c20 7265 7475 726e 7320 6576 6572  ds, returns ever
-00028b80: 7920 656c 656d 656e 742e 204e 6f74 653a  y element. Note:
-00028b90: 2074 6865 2069 7465 7261 746f 7220 646f   the iterator do
-00028ba0: 6573 206e 6f74 2070 726f 6475 6365 2061  es not produce a
-00028bb0: 6e79 206f 7574 7075 7420 756e 7469 6c20  ny output until 
-00028bc0: 7468 6520 7072 6564 6963 6174 6520 6669  the predicate fi
-00028bd0: 7273 7420 6265 636f 6d65 7320 6661 6c73  rst becomes fals
-00028be0: 652c 2073 6f20 6974 206d 6179 2068 6176  e, so it may hav
-00028bf0: 6520 6120 6c65 6e67 7468 7920 7374 6172  e a lengthy star
-00028c00: 742d 7570 2074 696d 652e 2045 7175 6976  t-up time. Equiv
-00028c10: 616c 656e 7420 746f 3a0a 6060 6063 6f63  alent to:.```coc
-00028c20: 6f6e 7574 5f70 7974 686f 6e0a 6465 6620  onut_python.def 
-00028c30: 6472 6f70 7768 696c 6528 7072 6564 6963  dropwhile(predic
-00028c40: 6174 652c 2069 7465 7261 626c 6529 3a0a  ate, iterable):.
-00028c50: 2020 2020 2320 6472 6f70 7768 696c 6528      # dropwhile(
-00028c60: 6c61 6d62 6461 2078 3a20 783c 352c 205b  lambda x: x<5, [
-00028c70: 312c 342c 362c 342c 315d 2920 2d2d 3e20  1,4,6,4,1]) --> 
-00028c80: 3620 3420 310a 2020 2020 6974 6572 6162  6 4 1.    iterab
-00028c90: 6c65 203d 2069 7465 7228 6974 6572 6162  le = iter(iterab
-00028ca0: 6c65 290a 2020 2020 666f 7220 7820 696e  le).    for x in
-00028cb0: 2069 7465 7261 626c 653a 0a20 2020 2020   iterable:.     
-00028cc0: 2020 2069 6620 6e6f 7420 7072 6564 6963     if not predic
-00028cd0: 6174 6528 7829 3a0a 2020 2020 2020 2020  ate(x):.        
-00028ce0: 2020 2020 7969 656c 6420 780a 2020 2020      yield x.    
-00028cf0: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
-00028d00: 2020 666f 7220 7820 696e 2069 7465 7261    for x in itera
-00028d10: 626c 653a 0a20 2020 2020 2020 2079 6965  ble:.        yie
-00028d20: 6c64 2078 0a60 6060 0a0a 2323 2323 2320  ld x.```..##### 
-00028d30: 4578 616d 706c 650a 0a2a 2a43 6f63 6f6e  Example..**Cocon
-00028d40: 7574 3a2a 2a0a 6060 6063 6f63 6f6e 7574  ut:**.```coconut
-00028d50: 0a70 6f73 6974 6976 6573 203d 206e 756d  .positives = num
-00028d60: 6974 6572 207c 3e20 6472 6f70 7768 696c  iter |> dropwhil
-00028d70: 6524 2878 202d 3e20 7820 3c20 3029 0a60  e$(x -> x < 0).`
-00028d80: 6060 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a  ``..**Python:**.
-00028d90: 6060 6063 6f63 6f6e 7574 5f70 7974 686f  ```coconut_pytho
-00028da0: 6e0a 696d 706f 7274 2069 7465 7274 6f6f  n.import itertoo
-00028db0: 6c73 0a70 6f73 6974 6976 6573 203d 2069  ls.positives = i
-00028dc0: 7465 7274 6f6f 6c73 2e64 726f 7077 6869  tertools.dropwhi
-00028dd0: 6c65 286c 616d 6264 6120 783a 2078 203c  le(lambda x: x <
-00028de0: 2030 2c20 6e75 6d69 7465 7229 0a60 6060   0, numiter).```
-00028df0: 0a0a 2323 2323 2060 666c 6174 7465 6e60  ..#### `flatten`
-00028e00: 0a0a 2a2a 666c 6174 7465 6e2a 2a28 5f69  ..**flatten**(_i
-00028e10: 7465 7261 626c 655f 2c20 5f6c 6576 656c  terable_, _level
-00028e20: 735f 3d60 3160 290a 0a43 6f63 6f6e 7574  s_=`1`)..Coconut
-00028e30: 2070 726f 7669 6465 7320 616e 2065 6e68   provides an enh
-00028e40: 616e 6365 6420 7665 7273 696f 6e20 6f66  anced version of
-00028e50: 2060 6974 6572 746f 6f6c 732e 6368 6169   `itertools.chai
-00028e60: 6e2e 6672 6f6d 5f69 7465 7261 626c 6560  n.from_iterable`
-00028e70: 2061 7320 6120 6275 696c 742d 696e 2075   as a built-in u
-00028e80: 6e64 6572 2074 6865 206e 616d 6520 6066  nder the name `f
-00028e90: 6c61 7474 656e 6020 7769 7468 2061 6464  latten` with add
-00028ea0: 6564 2073 7570 706f 7274 2066 6f72 2060  ed support for `
-00028eb0: 7265 7665 7273 6564 602c 2060 7265 7072  reversed`, `repr
-00028ec0: 602c 2060 696e 602c 2060 2e63 6f75 6e74  `, `in`, `.count
-00028ed0: 2829 602c 2060 2e69 6e64 6578 2829 602c  ()`, `.index()`,
-00028ee0: 2061 6e64 2060 666d 6170 602e 0a0a 4279   and `fmap`...By
-00028ef0: 2064 6566 6175 6c74 2c20 6066 6c61 7474   default, `flatt
-00028f00: 656e 6020 6f6e 6c79 2066 6c61 7474 656e  en` only flatten
-00028f10: 7320 7468 6520 746f 7020 6c65 7665 6c20  s the top level 
-00028f20: 6f66 2074 6865 2067 6976 656e 2069 7465  of the given ite
-00028f30: 7261 626c 652f 6172 7261 792e 2049 6620  rable/array. If 
-00028f40: 5f6c 6576 656c 735f 2069 7320 7061 7373  _levels_ is pass
-00028f50: 6564 2c20 686f 7765 7665 722c 2069 7420  ed, however, it 
-00028f60: 6361 6e20 6265 2075 7365 6420 746f 2063  can be used to c
-00028f70: 6f6e 7472 6f6c 2074 6865 206e 756d 6265  ontrol the numbe
-00028f80: 7220 6f66 206c 6576 656c 7320 666c 6174  r of levels flat
-00028f90: 7465 6e65 642c 2077 6974 6820 6030 6020  tened, with `0` 
-00028fa0: 6d65 616e 696e 6720 6e6f 2066 6c61 7474  meaning no flatt
-00028fb0: 656e 696e 6720 616e 6420 604e 6f6e 6560  ening and `None`
-00028fc0: 2066 6c61 7474 656e 696e 6720 6173 206d   flattening as m
-00028fd0: 616e 7920 6974 6572 6162 6c65 7320 6173  any iterables as
-00028fe0: 2061 7265 2066 6f75 6e64 2e20 4e6f 7465   are found. Note
-00028ff0: 2074 6861 7420 6966 205f 6c65 7665 6c73   that if _levels
-00029000: 5f20 6973 2073 6574 2074 6f20 616e 7920  _ is set to any 
-00029010: 6e6f 6e2d 604e 6f6e 6560 2076 616c 7565  non-`None` value
-00029020: 2c20 7468 6520 6669 7273 7420 5f6c 6576  , the first _lev
-00029030: 656c 735f 206c 6576 656c 7320 6d75 7374  els_ levels must
-00029040: 2062 6520 6974 6572 6162 6c65 732c 206f   be iterables, o
-00029050: 7220 656c 7365 2061 6e20 6572 726f 7220  r else an error 
-00029060: 7769 6c6c 2062 6520 7261 6973 6564 2e0a  will be raised..
-00029070: 0a23 2323 2323 2050 7974 686f 6e20 446f  .##### Python Do
-00029080: 6373 0a0a 6368 6169 6e2e 2a2a 6672 6f6d  cs..chain.**from
-00029090: 5f69 7465 7261 626c 652a 2a28 5f69 7465  _iterable**(_ite
-000290a0: 7261 626c 655f 290a 0a41 6c74 6572 6e61  rable_)..Alterna
-000290b0: 7465 2063 6f6e 7374 7275 6374 6f72 2066  te constructor f
-000290c0: 6f72 2060 6368 6169 6e28 2960 2e20 4765  or `chain()`. Ge
-000290d0: 7473 2063 6861 696e 6564 2069 6e70 7574  ts chained input
-000290e0: 7320 6672 6f6d 2061 2073 696e 676c 6520  s from a single 
-000290f0: 6974 6572 6162 6c65 2061 7267 756d 656e  iterable argumen
-00029100: 7420 7468 6174 2069 7320 6576 616c 7561  t that is evalua
-00029110: 7465 6420 6c61 7a69 6c79 2e20 526f 7567  ted lazily. Roug
-00029120: 686c 7920 6571 7569 7661 6c65 6e74 2074  hly equivalent t
-00029130: 6f3a 0a0a 6060 6063 6f63 6f6e 7574 5f70  o:..```coconut_p
-00029140: 7974 686f 6e0a 6465 6620 666c 6174 7465  ython.def flatte
-00029150: 6e28 6974 6572 6162 6c65 7329 3a0a 2020  n(iterables):.  
-00029160: 2020 2320 666c 6174 7465 6e28 5b27 4142    # flatten(['AB
-00029170: 4327 2c20 2744 4546 275d 2920 2d2d 3e20  C', 'DEF']) --> 
-00029180: 4120 4220 4320 4420 4520 460a 2020 2020  A B C D E F.    
-00029190: 666f 7220 6974 2069 6e20 6974 6572 6162  for it in iterab
-000291a0: 6c65 733a 0a20 2020 2020 2020 2066 6f72  les:.        for
-000291b0: 2065 6c65 6d65 6e74 2069 6e20 6974 3a0a   element in it:.
-000291c0: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
-000291d0: 6420 656c 656d 656e 740a 6060 600a 0a23  d element.```..#
-000291e0: 2323 2323 2045 7861 6d70 6c65 0a0a 2a2a  #### Example..**
-000291f0: 436f 636f 6e75 743a 2a2a 0a60 6060 636f  Coconut:**.```co
-00029200: 636f 6e75 740a 6974 6572 5f6f 665f 6974  conut.iter_of_it
-00029210: 6572 7320 3d20 5b5b 312c 2032 5d2c 205b  ers = [[1, 2], [
-00029220: 332c 2034 5d5d 0a66 6c61 745f 6974 203d  3, 4]].flat_it =
-00029230: 2069 7465 725f 6f66 5f69 7465 7273 207c   iter_of_iters |
-00029240: 3e20 666c 6174 7465 6e20 7c3e 206c 6973  > flatten |> lis
-00029250: 740a 6060 600a 0a2a 2a50 7974 686f 6e3a  t.```..**Python:
-00029260: 2a2a 0a60 6060 636f 636f 6e75 745f 7079  **.```coconut_py
-00029270: 7468 6f6e 0a66 726f 6d20 6974 6572 746f  thon.from iterto
-00029280: 6f6c 7320 696d 706f 7274 2063 6861 696e  ols import chain
-00029290: 0a69 7465 725f 6f66 5f69 7465 7273 203d  .iter_of_iters =
-000292a0: 205b 5b31 2c20 325d 2c20 5b33 2c20 345d   [[1, 2], [3, 4]
-000292b0: 5d0a 666c 6174 5f69 7420 3d20 6974 6572  ].flat_it = iter
-000292c0: 5f6f 665f 6974 6572 7320 7c3e 2063 6861  _of_iters |> cha
-000292d0: 696e 2e66 726f 6d5f 6974 6572 6162 6c65  in.from_iterable
-000292e0: 207c 3e20 6c69 7374 0a60 6060 0a0a 2323   |> list.```..##
-000292f0: 2323 2060 7363 616e 600a 0a2a 2a73 6361  ## `scan`..**sca
-00029300: 6e2a 2a28 5f66 756e 6374 696f 6e5f 2c20  n**(_function_, 
-00029310: 5f69 7465 7261 626c 655f 5b2c 205f 696e  _iterable_[, _in
-00029320: 6974 6961 6c5f 5d29 0a0a 436f 636f 6e75  itial_])..Coconu
-00029330: 7420 7072 6f76 6964 6573 2061 206d 6f64  t provides a mod
-00029340: 6966 6965 6420 7665 7273 696f 6e20 6f66  ified version of
-00029350: 2060 6974 6572 746f 6f6c 732e 6163 6375   `itertools.accu
-00029360: 6d75 6c61 7465 6020 7769 7468 206f 7070  mulate` with opp
-00029370: 6f73 6974 6520 6172 6775 6d65 6e74 206f  osite argument o
-00029380: 7264 6572 2061 7320 6073 6361 6e60 2074  rder as `scan` t
-00029390: 6861 7420 616c 736f 2073 7570 706f 7274  hat also support
-000293a0: 7320 6072 6570 7260 2c20 606c 656e 602c  s `repr`, `len`,
-000293b0: 2061 6e64 2060 6675 6e63 602f 6069 7465   and `func`/`ite
-000293c0: 7260 2f60 696e 6974 6961 6c60 2061 7474  r`/`initial` att
-000293d0: 7269 6275 7465 732e 2060 7363 616e 6020  ributes. `scan` 
-000293e0: 776f 726b 7320 6578 6163 746c 7920 6c69  works exactly li
-000293f0: 6b65 205b 6072 6564 7563 6560 5d28 2372  ke [`reduce`](#r
-00029400: 6564 7563 6529 2c20 6578 6365 7074 2074  educe), except t
-00029410: 6861 7420 696e 7374 6561 6420 6f66 206f  hat instead of o
-00029420: 6e6c 7920 7265 7475 726e 696e 6720 7468  nly returning th
-00029430: 6520 6c61 7374 2061 6363 756d 756c 6174  e last accumulat
-00029440: 6564 2076 616c 7565 2c20 6974 2072 6574  ed value, it ret
-00029450: 7572 6e73 2061 6e20 6974 6572 6174 6f72  urns an iterator
-00029460: 206f 6620 616c 6c20 7468 6520 696e 7465   of all the inte
-00029470: 726d 6564 6961 7465 2076 616c 7565 732e  rmediate values.
-00029480: 0a0a 2323 2323 2320 5079 7468 6f6e 2044  ..##### Python D
-00029490: 6f63 730a 0a2a 2a73 6361 6e2a 2a28 5f66  ocs..**scan**(_f
-000294a0: 756e 6374 696f 6e2c 2069 7465 7261 626c  unction, iterabl
-000294b0: 655f 2a2a 5b2a 2a5f 2c20 696e 6974 6961  e_**[**_, initia
-000294c0: 6c5f 2a2a 5d2a 2a29 0a0a 4d61 6b65 2061  l_**]**)..Make a
-000294d0: 6e20 6974 6572 6174 6f72 2074 6861 7420  n iterator that 
-000294e0: 7265 7475 726e 7320 6163 6375 6d75 6c61  returns accumula
-000294f0: 7465 6420 7265 7375 6c74 7320 6f66 2073  ted results of s
-00029500: 6f6d 6520 6675 6e63 7469 6f6e 206f 6620  ome function of 
-00029510: 7477 6f20 6172 6775 6d65 6e74 732e 2045  two arguments. E
-00029520: 6c65 6d65 6e74 7320 6f66 2074 6865 2069  lements of the i
-00029530: 6e70 7574 2069 7465 7261 626c 6520 6d61  nput iterable ma
-00029540: 7920 6265 2061 6e79 2074 7970 6520 7468  y be any type th
-00029550: 6174 2063 616e 2062 6520 6163 6365 7074  at can be accept
-00029560: 6564 2061 7320 6172 6775 6d65 6e74 7320  ed as arguments 
-00029570: 746f 205f 6675 6e63 7469 6f6e 5f2e 2028  to _function_. (
-00029580: 466f 7220 6578 616d 706c 652c 2077 6974  For example, wit
-00029590: 6820 7468 6520 6f70 6572 6174 696f 6e20  h the operation 
-000295a0: 6f66 2061 6464 6974 696f 6e2c 2065 6c65  of addition, ele
-000295b0: 6d65 6e74 7320 6d61 7920 6265 2061 6e79  ments may be any
-000295c0: 2061 6464 6162 6c65 2074 7970 6520 696e   addable type in
-000295d0: 636c 7564 696e 6720 4465 6369 6d61 6c20  cluding Decimal 
-000295e0: 6f72 2046 7261 6374 696f 6e2e 2920 4966  or Fraction.) If
-000295f0: 2074 6865 2069 6e70 7574 2069 7465 7261   the input itera
-00029600: 626c 6520 6973 2065 6d70 7479 2c20 7468  ble is empty, th
-00029610: 6520 6f75 7470 7574 2069 7465 7261 626c  e output iterabl
-00029620: 6520 7769 6c6c 2061 6c73 6f20 6265 2065  e will also be e
-00029630: 6d70 7479 2e0a 0a49 6620 6e6f 205f 696e  mpty...If no _in
-00029640: 6974 6961 6c5f 2069 7320 6769 7665 6e2c  itial_ is given,
-00029650: 2072 6f75 6768 6c79 2065 7175 6976 616c   roughly equival
-00029660: 656e 7420 746f 3a0a 6060 6063 6f63 6f6e  ent to:.```cocon
-00029670: 7574 5f70 7974 686f 6e0a 6465 6620 7363  ut_python.def sc
-00029680: 616e 2866 756e 6374 696f 6e2c 2069 7465  an(function, ite
-00029690: 7261 626c 6529 3a0a 2020 2020 2752 6574  rable):.    'Ret
-000296a0: 7572 6e20 7275 6e6e 696e 6720 746f 7461  urn running tota
-000296b0: 6c73 270a 2020 2020 2320 7363 616e 286f  ls'.    # scan(o
-000296c0: 7065 7261 746f 722e 6164 642c 205b 312c  perator.add, [1,
-000296d0: 322c 332c 342c 355d 2920 2d2d 3e20 3120  2,3,4,5]) --> 1 
-000296e0: 3320 3620 3130 2031 350a 2020 2020 2320  3 6 10 15.    # 
-000296f0: 7363 616e 286f 7065 7261 746f 722e 6d75  scan(operator.mu
-00029700: 6c2c 205b 312c 322c 332c 342c 355d 2920  l, [1,2,3,4,5]) 
-00029710: 2d2d 3e20 3120 3220 3620 3234 2031 3230  --> 1 2 6 24 120
-00029720: 0a20 2020 2069 7420 3d20 6974 6572 2869  .    it = iter(i
-00029730: 7465 7261 626c 6529 0a20 2020 2074 7279  terable).    try
-00029740: 3a0a 2020 2020 2020 2020 746f 7461 6c20  :.        total 
-00029750: 3d20 6e65 7874 2869 7429 0a20 2020 2065  = next(it).    e
-00029760: 7863 6570 7420 5374 6f70 4974 6572 6174  xcept StopIterat
-00029770: 696f 6e3a 0a20 2020 2020 2020 2072 6574  ion:.        ret
-00029780: 7572 6e0a 2020 2020 7969 656c 6420 746f  urn.    yield to
-00029790: 7461 6c0a 2020 2020 666f 7220 656c 656d  tal.    for elem
-000297a0: 656e 7420 696e 2069 743a 0a20 2020 2020  ent in it:.     
-000297b0: 2020 2074 6f74 616c 203d 2066 756e 6374     total = funct
-000297c0: 696f 6e28 746f 7461 6c2c 2065 6c65 6d65  ion(total, eleme
-000297d0: 6e74 290a 2020 2020 2020 2020 7969 656c  nt).        yiel
-000297e0: 6420 746f 7461 6c0a 6060 600a 0a23 2323  d total.```..###
-000297f0: 2323 2045 7861 6d70 6c65 0a0a 2a2a 436f  ## Example..**Co
-00029800: 636f 6e75 743a 2a2a 0a60 6060 636f 636f  conut:**.```coco
-00029810: 6e75 740a 696e 7075 745f 6461 7461 203d  nut.input_data =
-00029820: 205b 332c 2034 2c20 362c 2032 2c20 312c   [3, 4, 6, 2, 1,
-00029830: 2039 2c20 302c 2037 2c20 352c 2038 5d0a   9, 0, 7, 5, 8].
-00029840: 7275 6e6e 696e 675f 6d61 7820 3d20 696e  running_max = in
-00029850: 7075 745f 6461 7461 207c 3e20 7363 616e  put_data |> scan
-00029860: 2428 6d61 7829 207c 3e20 6c69 7374 0a60  $(max) |> list.`
-00029870: 6060 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a  ``..**Python:**.
-00029880: 6060 6063 6f63 6f6e 7574 5f70 7974 686f  ```coconut_pytho
-00029890: 6e0a 696e 7075 745f 6461 7461 203d 205b  n.input_data = [
-000298a0: 332c 2034 2c20 362c 2032 2c20 312c 2039  3, 4, 6, 2, 1, 9
-000298b0: 2c20 302c 2037 2c20 352c 2038 5d0a 7275  , 0, 7, 5, 8].ru
-000298c0: 6e6e 696e 675f 6d61 7820 3d20 5b5d 0a6d  nning_max = [].m
-000298d0: 6178 5f73 6f5f 6661 7220 3d20 696e 7075  ax_so_far = inpu
-000298e0: 745f 6461 7461 5b30 5d0a 666f 7220 7820  t_data[0].for x 
-000298f0: 696e 2069 6e70 7574 5f64 6174 613a 0a20  in input_data:. 
-00029900: 2020 2069 6620 7820 3e20 6d61 785f 736f     if x > max_so
-00029910: 5f66 6172 3a0a 2020 2020 2020 2020 6d61  _far:.        ma
-00029920: 785f 736f 5f66 6172 203d 2078 0a20 2020  x_so_far = x.   
-00029930: 2072 756e 6e69 6e67 5f6d 6178 2e61 7070   running_max.app
-00029940: 656e 6428 7829 0a60 6060 0a0a 2323 2323  end(x).```..####
-00029950: 2060 636f 756e 7460 0a0a 2a2a 636f 756e   `count`..**coun
-00029960: 742a 2a28 5f73 7461 7274 5f3d 6030 602c  t**(_start_=`0`,
-00029970: 205f 7374 6570 5f3d 6031 6029 0a0a 436f   _step_=`1`)..Co
-00029980: 636f 6e75 7420 7072 6f76 6964 6573 2061  conut provides a
-00029990: 206d 6f64 6966 6965 6420 7665 7273 696f   modified versio
-000299a0: 6e20 6f66 2060 6974 6572 746f 6f6c 732e  n of `itertools.
-000299b0: 636f 756e 7460 2074 6861 7420 7375 7070  count` that supp
-000299c0: 6f72 7473 2060 696e 602c 206e 6f72 6d61  orts `in`, norma
-000299d0: 6c20 736c 6963 696e 672c 206f 7074 696d  l slicing, optim
-000299e0: 697a 6564 2069 7465 7261 746f 7220 736c  ized iterator sl
-000299f0: 6963 696e 672c 2074 6865 2073 7461 6e64  icing, the stand
-00029a00: 6172 6420 6063 6f75 6e74 6020 616e 6420  ard `count` and 
-00029a10: 6069 6e64 6578 6020 7365 7175 656e 6365  `index` sequence
-00029a20: 206d 6574 686f 6473 2c20 6072 6570 7260   methods, `repr`
-00029a30: 2c20 616e 6420 6073 7461 7274 602f 6073  , and `start`/`s
-00029a40: 7465 7060 2061 7474 7269 6275 7465 7320  tep` attributes 
-00029a50: 6173 2061 2062 7569 6c74 2d69 6e20 756e  as a built-in un
-00029a60: 6465 7220 7468 6520 6e61 6d65 2060 636f  der the name `co
-00029a70: 756e 7460 2e0a 0a41 6464 6974 696f 6e61  unt`...Additiona
-00029a80: 6c6c 792c 2069 6620 7468 6520 5f73 7465  lly, if the _ste
-00029a90: 705f 2070 6172 616d 6574 6572 2069 7320  p_ parameter is 
-00029aa0: 7365 7420 746f 2060 4e6f 6e65 602c 2060  set to `None`, `
-00029ab0: 636f 756e 7460 2077 696c 6c20 6265 6861  count` will beha
-00029ac0: 7665 206c 696b 6520 6069 7465 7274 6f6f  ve like `itertoo
-00029ad0: 6c73 2e72 6570 6561 7460 2069 6e73 7465  ls.repeat` inste
-00029ae0: 6164 2e0a 0a23 2323 2323 2050 7974 686f  ad...##### Pytho
-00029af0: 6e20 446f 6373 0a0a 2a2a 636f 756e 742a  n Docs..**count*
-00029b00: 2a28 5f73 7461 7274 3d30 2c20 7374 6570  *(_start=0, step
-00029b10: 3d31 5f29 0a0a 4d61 6b65 2061 6e20 6974  =1_)..Make an it
-00029b20: 6572 6174 6f72 2074 6861 7420 7265 7475  erator that retu
-00029b30: 726e 7320 6576 656e 6c79 2073 7061 6365  rns evenly space
-00029b40: 6420 7661 6c75 6573 2073 7461 7274 696e  d values startin
-00029b50: 6720 7769 7468 206e 756d 6265 7220 5f73  g with number _s
-00029b60: 7461 7274 5f2e 204f 6674 656e 2075 7365  tart_. Often use
-00029b70: 6420 6173 2061 6e20 6172 6775 6d65 6e74  d as an argument
-00029b80: 2074 6f20 606d 6170 2829 6020 746f 2067   to `map()` to g
-00029b90: 656e 6572 6174 6520 636f 6e73 6563 7574  enerate consecut
-00029ba0: 6976 6520 6461 7461 2070 6f69 6e74 732e  ive data points.
-00029bb0: 2041 6c73 6f2c 2075 7365 6420 7769 7468   Also, used with
-00029bc0: 2060 7a69 7028 2960 2074 6f20 6164 6420   `zip()` to add 
-00029bd0: 7365 7175 656e 6365 206e 756d 6265 7273  sequence numbers
-00029be0: 2e20 526f 7567 686c 7920 6571 7569 7661  . Roughly equiva
-00029bf0: 6c65 6e74 2074 6f3a 0a60 6060 636f 636f  lent to:.```coco
-00029c00: 6e75 745f 7079 7468 6f6e 0a64 6566 2063  nut_python.def c
-00029c10: 6f75 6e74 2873 7461 7274 3d30 2c20 7374  ount(start=0, st
-00029c20: 6570 3d31 293a 0a20 2020 2023 2063 6f75  ep=1):.    # cou
-00029c30: 6e74 2831 3029 202d 2d3e 2031 3020 3131  nt(10) --> 10 11
-00029c40: 2031 3220 3133 2031 3420 2e2e 2e0a 2020   12 13 14 ....  
-00029c50: 2020 2320 636f 756e 7428 322e 352c 2030    # count(2.5, 0
-00029c60: 2e35 2920 2d3e 2032 2e35 2033 2e30 2033  .5) -> 2.5 3.0 3
-00029c70: 2e35 202e 2e2e 0a20 2020 206e 203d 2073  .5 ....    n = s
-00029c80: 7461 7274 0a20 2020 2077 6869 6c65 2054  tart.    while T
-00029c90: 7275 653a 0a20 2020 2020 2020 2079 6965  rue:.        yie
-00029ca0: 6c64 206e 0a20 2020 2020 2020 2069 6620  ld n.        if 
-00029cb0: 7374 6570 3a0a 2020 2020 2020 2020 2020  step:.          
-00029cc0: 6e20 2b3d 2073 7465 700a 6060 600a 0a23  n += step.```..#
-00029cd0: 2323 2323 2045 7861 6d70 6c65 0a0a 2a2a  #### Example..**
-00029ce0: 436f 636f 6e75 743a 2a2a 0a60 6060 636f  Coconut:**.```co
-00029cf0: 636f 6e75 740a 636f 756e 7428 2924 5b31  conut.count()$[1
-00029d00: 302a 2a31 3030 5d20 7c3e 2070 7269 6e74  0**100] |> print
-00029d10: 0a60 6060 0a0a 2a2a 5079 7468 6f6e 3a2a  .```..**Python:*
-00029d20: 2a0a 5f43 616e 2774 2062 6520 646f 6e65  *._Can't be done
-00029d30: 2071 7569 636b 6c79 2077 6974 686f 7574   quickly without
-00029d40: 2043 6f63 6f6e 7574 2773 2069 7465 7261   Coconut's itera
-00029d50: 746f 7220 736c 6963 696e 672c 2077 6869  tor slicing, whi
-00029d60: 6368 2072 6571 7569 7265 7320 6d61 6e79  ch requires many
-00029d70: 2063 6f6d 706c 6963 6174 6564 2070 6965   complicated pie
-00029d80: 6365 732e 2054 6865 206e 6563 6573 7361  ces. The necessa
-00029d90: 7279 2064 6566 696e 6974 696f 6e73 2069  ry definitions i
-00029da0: 6e20 5079 7468 6f6e 2063 616e 2062 6520  n Python can be 
-00029db0: 666f 756e 6420 696e 2074 6865 2043 6f63  found in the Coc
-00029dc0: 6f6e 7574 2068 6561 6465 722e 5f0a 0a23  onut header._..#
-00029dd0: 2323 2320 6063 7963 6c65 600a 0a2a 2a63  ### `cycle`..**c
-00029de0: 7963 6c65 2a2a 285f 6974 6572 6162 6c65  ycle**(_iterable
-00029df0: 5f2c 205f 7469 6d65 735f 3d60 4e6f 6e65  _, _times_=`None
-00029e00: 6029 0a0a 436f 636f 6e75 7427 7320 6063  `)..Coconut's `c
-00029e10: 7963 6c65 6020 6973 2061 206d 6f64 6966  ycle` is a modif
-00029e20: 6965 6420 7665 7273 696f 6e20 6f66 2060  ied version of `
-00029e30: 6974 6572 746f 6f6c 732e 6379 636c 6560  itertools.cycle`
-00029e40: 2077 6974 6820 6120 6074 696d 6573 6020   with a `times` 
-00029e50: 7061 7261 6d65 7465 7220 7468 6174 2063  parameter that c
-00029e60: 6f6e 7472 6f6c 7320 7468 6520 6e75 6d62  ontrols the numb
-00029e70: 6572 206f 6620 7469 6d65 7320 746f 2063  er of times to c
-00029e80: 7963 6c65 2074 6872 6f75 6768 205f 6974  ycle through _it
-00029e90: 6572 6162 6c65 5f20 6265 666f 7265 2073  erable_ before s
-00029ea0: 746f 7070 696e 672e 2060 6379 636c 6560  topping. `cycle`
-00029eb0: 2061 6c73 6f20 7375 7070 6f72 7473 2060   also supports `
-00029ec0: 696e 602c 2073 6c69 6369 6e67 2c20 606c  in`, slicing, `l
-00029ed0: 656e 602c 2060 7265 7665 7273 6564 602c  en`, `reversed`,
-00029ee0: 2060 2e63 6f75 6e74 2829 602c 2060 2e69   `.count()`, `.i
-00029ef0: 6e64 6578 2829 602c 2061 6e64 2060 7265  ndex()`, and `re
-00029f00: 7072 602e 0a0a 2323 2323 2320 5079 7468  pr`...##### Pyth
-00029f10: 6f6e 2044 6f63 730a 0a2a 2a63 7963 6c65  on Docs..**cycle
-00029f20: 2a2a 285f 6974 6572 6162 6c65 5f29 0a0a  **(_iterable_)..
-00029f30: 4d61 6b65 2061 6e20 6974 6572 6174 6f72  Make an iterator
-00029f40: 2072 6574 7572 6e69 6e67 2065 6c65 6d65   returning eleme
-00029f50: 6e74 7320 6672 6f6d 2074 6865 2069 7465  nts from the ite
-00029f60: 7261 626c 6520 616e 6420 7361 7669 6e67  rable and saving
-00029f70: 2061 2063 6f70 7920 6f66 2065 6163 682e   a copy of each.
-00029f80: 2057 6865 6e20 7468 6520 6974 6572 6162   When the iterab
-00029f90: 6c65 2069 7320 6578 6861 7573 7465 642c  le is exhausted,
-00029fa0: 2072 6574 7572 6e20 656c 656d 656e 7473   return elements
-00029fb0: 2066 726f 6d20 7468 6520 7361 7665 6420   from the saved 
-00029fc0: 636f 7079 2e20 5265 7065 6174 7320 696e  copy. Repeats in
-00029fd0: 6465 6669 6e69 7465 6c79 2e20 526f 7567  definitely. Roug
-00029fe0: 686c 7920 6571 7569 7661 6c65 6e74 2074  hly equivalent t
-00029ff0: 6f3a 0a0a 6060 6063 6f63 6f6e 7574 5f70  o:..```coconut_p
-0002a000: 7974 686f 6e0a 6465 6620 6379 636c 6528  ython.def cycle(
-0002a010: 6974 6572 6162 6c65 293a 0a20 2020 2023  iterable):.    #
-0002a020: 2063 7963 6c65 2827 4142 4344 2729 202d   cycle('ABCD') -
-0002a030: 2d3e 2041 2042 2043 2044 2041 2042 2043  -> A B C D A B C
-0002a040: 2044 2041 2042 2043 2044 202e 2e2e 0a20   D A B C D .... 
-0002a050: 2020 2073 6176 6564 203d 205b 5d0a 2020     saved = [].  
-0002a060: 2020 666f 7220 656c 656d 656e 7420 696e    for element in
-0002a070: 2069 7465 7261 626c 653a 0a20 2020 2020   iterable:.     
-0002a080: 2020 2079 6965 6c64 2065 6c65 6d65 6e74     yield element
-0002a090: 0a20 2020 2020 2020 2073 6176 6564 2e61  .        saved.a
-0002a0a0: 7070 656e 6428 656c 656d 656e 7429 0a20  ppend(element). 
-0002a0b0: 2020 2077 6869 6c65 2073 6176 6564 3a0a     while saved:.
-0002a0c0: 2020 2020 2020 2020 666f 7220 656c 656d          for elem
-0002a0d0: 656e 7420 696e 2073 6176 6564 3a0a 2020  ent in saved:.  
-0002a0e0: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
-0002a0f0: 6420 656c 656d 656e 740a 6060 600a 0a4e  d element.```..N
-0002a100: 6f74 652c 2074 6869 7320 6d65 6d62 6572  ote, this member
-0002a110: 206f 6620 7468 6520 746f 6f6c 6b69 7420   of the toolkit 
-0002a120: 6d61 7920 7265 7175 6972 6520 7369 676e  may require sign
-0002a130: 6966 6963 616e 7420 6175 7869 6c69 6172  ificant auxiliar
-0002a140: 7920 7374 6f72 6167 6520 2864 6570 656e  y storage (depen
-0002a150: 6469 6e67 206f 6e20 7468 6520 6c65 6e67  ding on the leng
-0002a160: 7468 206f 6620 7468 6520 6974 6572 6162  th of the iterab
-0002a170: 6c65 292e 0a0a 2323 2323 2320 4578 616d  le)...##### Exam
-0002a180: 706c 650a 0a2a 2a43 6f63 6f6e 7574 3a2a  ple..**Coconut:*
-0002a190: 2a0a 6060 6063 6f63 6f6e 7574 0a63 7963  *.```coconut.cyc
-0002a1a0: 6c65 2872 616e 6765 2832 292c 2032 2920  le(range(2), 2) 
-0002a1b0: 7c3e 206c 6973 7420 7c3e 2070 7269 6e74  |> list |> print
-0002a1c0: 0a60 6060 0a0a 2a2a 5079 7468 6f6e 3a2a  .```..**Python:*
-0002a1d0: 2a0a 6060 6063 6f63 6f6e 7574 5f70 7974  *.```coconut_pyt
-0002a1e0: 686f 6e0a 6672 6f6d 2069 7465 7274 6f6f  hon.from itertoo
-0002a1f0: 6c73 2069 6d70 6f72 7420 6379 636c 652c  ls import cycle,
-0002a200: 2069 736c 6963 650a 7072 696e 7428 6c69   islice.print(li
-0002a210: 7374 2869 736c 6963 6528 6379 636c 6528  st(islice(cycle(
-0002a220: 7261 6e67 6528 3229 292c 2034 2929 290a  range(2)), 4))).
-0002a230: 6060 600a 0a23 2323 2320 6063 6172 7465  ```..#### `carte
-0002a240: 7369 616e 5f70 726f 6475 6374 600a 0a2a  sian_product`..*
-0002a250: 2a63 6172 7465 7369 616e 5c5f 7072 6f64  *cartesian\_prod
-0002a260: 7563 742a 2a28 2a5f 6974 6572 6162 6c65  uct**(*_iterable
-0002a270: 735f 2c20 5f72 6570 6561 745f 3d60 3160  s_, _repeat_=`1`
-0002a280: 290a 0a43 6f63 6f6e 7574 2070 726f 7669  )..Coconut provi
-0002a290: 6465 7320 616e 2065 6e68 616e 6365 6420  des an enhanced 
-0002a2a0: 7665 7273 696f 6e20 6f66 2060 6974 6572  version of `iter
-0002a2b0: 746f 6f6c 732e 7072 6f64 7563 7460 2061  tools.product` a
-0002a2c0: 7320 6120 6275 696c 742d 696e 2075 6e64  s a built-in und
-0002a2d0: 6572 2074 6865 206e 616d 6520 6063 6172  er the name `car
-0002a2e0: 7465 7369 616e 5f70 726f 6475 6374 6020  tesian_product` 
-0002a2f0: 7769 7468 2061 6464 6564 2073 7570 706f  with added suppo
-0002a300: 7274 2066 6f72 2060 6c65 6e60 2c20 6072  rt for `len`, `r
-0002a310: 6570 7260 2c20 6069 6e60 2c20 602e 636f  epr`, `in`, `.co
-0002a320: 756e 7428 2960 2c20 616e 6420 6066 6d61  unt()`, and `fma
-0002a330: 7060 2e0a 0a41 6464 6974 696f 6e61 6c6c  p`...Additionall
-0002a340: 792c 2060 6361 7274 6573 6961 6e5f 7072  y, `cartesian_pr
-0002a350: 6f64 7563 7460 2069 6e63 6c75 6465 7320  oduct` includes 
-0002a360: 7370 6563 6961 6c20 7375 7070 6f72 7420  special support 
-0002a370: 666f 7220 5b60 6e75 6d70 7960 5d28 236e  for [`numpy`](#n
-0002a380: 756d 7079 2d69 6e74 6567 7261 7469 6f6e  umpy-integration
-0002a390: 2920 6f62 6a65 6374 732c 2069 6e20 7768  ) objects, in wh
-0002a3a0: 6963 6820 6361 7365 2061 206d 756c 7469  ich case a multi
-0002a3b0: 6469 6d65 6e73 696f 6e61 6c20 6172 7261  dimensional arra
-0002a3c0: 7920 6973 2072 6574 7572 6e65 6420 696e  y is returned in
-0002a3d0: 7374 6561 6420 6f66 2061 6e20 6974 6572  stead of an iter
-0002a3e0: 6174 6f72 2e0a 0a23 2323 2323 2050 7974  ator...##### Pyt
-0002a3f0: 686f 6e20 446f 6373 0a0a 2a2a 6361 7274  hon Docs..**cart
-0002a400: 6573 6961 6e5c 5f70 726f 6475 6374 2a2a  esian\_product**
-0002a410: 285f 5c2a 6974 6572 6162 6c65 732c 2072  (_\*iterables, r
-0002a420: 6570 6561 743d 315f 290a 0a43 6172 7465  epeat=1_)..Carte
-0002a430: 7369 616e 2070 726f 6475 6374 206f 6620  sian product of 
-0002a440: 696e 7075 7420 6974 6572 6162 6c65 732e  input iterables.
-0002a450: 0a0a 526f 7567 686c 7920 6571 7569 7661  ..Roughly equiva
-0002a460: 6c65 6e74 2074 6f20 6e65 7374 6564 2066  lent to nested f
-0002a470: 6f72 2d6c 6f6f 7073 2069 6e20 6120 6765  or-loops in a ge
-0002a480: 6e65 7261 746f 7220 6578 7072 6573 7369  nerator expressi
-0002a490: 6f6e 2e20 466f 7220 6578 616d 706c 652c  on. For example,
-0002a4a0: 2060 6361 7274 6573 6961 6e5f 7072 6f64   `cartesian_prod
-0002a4b0: 7563 7428 412c 2042 2960 2072 6574 7572  uct(A, B)` retur
-0002a4c0: 6e73 2074 6865 2073 616d 6520 6173 2060  ns the same as `
-0002a4d0: 2828 782c 7929 2066 6f72 2078 2069 6e20  ((x,y) for x in 
-0002a4e0: 4120 666f 7220 7920 696e 2042 2960 2e0a  A for y in B)`..
-0002a4f0: 0a54 6865 206e 6573 7465 6420 6c6f 6f70  .The nested loop
-0002a500: 7320 6379 636c 6520 6c69 6b65 2061 6e20  s cycle like an 
-0002a510: 6f64 6f6d 6574 6572 2077 6974 6820 7468  odometer with th
-0002a520: 6520 7269 6768 746d 6f73 7420 656c 656d  e rightmost elem
-0002a530: 656e 7420 6164 7661 6e63 696e 6720 6f6e  ent advancing on
-0002a540: 2065 7665 7279 2069 7465 7261 7469 6f6e   every iteration
-0002a550: 2e20 5468 6973 2070 6174 7465 726e 2063  . This pattern c
-0002a560: 7265 6174 6573 2061 206c 6578 6963 6f67  reates a lexicog
-0002a570: 7261 7068 6963 206f 7264 6572 696e 6720  raphic ordering 
-0002a580: 736f 2074 6861 7420 6966 2074 6865 2069  so that if the i
-0002a590: 6e70 7574 e280 9973 2069 7465 7261 626c  nput...s iterabl
-0002a5a0: 6573 2061 7265 2073 6f72 7465 642c 2074  es are sorted, t
-0002a5b0: 6865 2070 726f 6475 6374 2074 7570 6c65  he product tuple
-0002a5c0: 7320 6172 6520 656d 6974 7465 6420 696e  s are emitted in
-0002a5d0: 2073 6f72 7465 6420 6f72 6465 722e 0a0a   sorted order...
-0002a5e0: 546f 2063 6f6d 7075 7465 2074 6865 2070  To compute the p
-0002a5f0: 726f 6475 6374 206f 6620 616e 2069 7465  roduct of an ite
-0002a600: 7261 626c 6520 7769 7468 2069 7473 656c  rable with itsel
-0002a610: 662c 2073 7065 6369 6679 2074 6865 206e  f, specify the n
-0002a620: 756d 6265 7220 6f66 2072 6570 6574 6974  umber of repetit
-0002a630: 696f 6e73 2077 6974 6820 7468 6520 6f70  ions with the op
-0002a640: 7469 6f6e 616c 2072 6570 6561 7420 6b65  tional repeat ke
-0002a650: 7977 6f72 6420 6172 6775 6d65 6e74 2e20  yword argument. 
-0002a660: 466f 7220 6578 616d 706c 652c 2060 7072  For example, `pr
-0002a670: 6f64 7563 7428 412c 2072 6570 6561 743d  oduct(A, repeat=
-0002a680: 3429 6020 6d65 616e 7320 7468 6520 7361  4)` means the sa
-0002a690: 6d65 2061 7320 6063 6172 7465 7369 616e  me as `cartesian
-0002a6a0: 5f70 726f 6475 6374 2841 2c20 412c 2041  _product(A, A, A
-0002a6b0: 2c20 4129 602e 0a0a 5468 6973 2066 756e  , A)`...This fun
-0002a6c0: 6374 696f 6e20 6973 2072 6f75 6768 6c79  ction is roughly
-0002a6d0: 2065 7175 6976 616c 656e 7420 746f 2074   equivalent to t
-0002a6e0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f64  he following cod
-0002a6f0: 652c 2065 7863 6570 7420 7468 6174 2074  e, except that t
-0002a700: 6865 2061 6374 7561 6c20 696d 706c 656d  he actual implem
-0002a710: 656e 7461 7469 6f6e 2064 6f65 7320 6e6f  entation does no
-0002a720: 7420 6275 696c 6420 7570 2069 6e74 6572  t build up inter
-0002a730: 6d65 6469 6174 6520 7265 7375 6c74 7320  mediate results 
-0002a740: 696e 206d 656d 6f72 793a 0a0a 6060 6063  in memory:..```c
-0002a750: 6f63 6f6e 7574 5f70 7974 686f 6e0a 6465  oconut_python.de
-0002a760: 6620 6361 7274 6573 6961 6e5f 7072 6f64  f cartesian_prod
-0002a770: 7563 7428 2a61 7267 732c 2072 6570 6561  uct(*args, repea
-0002a780: 743d 3129 3a0a 2020 2020 2320 7072 6f64  t=1):.    # prod
-0002a790: 7563 7428 2741 4243 4427 2c20 2778 7927  uct('ABCD', 'xy'
-0002a7a0: 2920 2d2d 3e20 4178 2041 7920 4278 2042  ) --> Ax Ay Bx B
-0002a7b0: 7920 4378 2043 7920 4478 2044 790a 2020  y Cx Cy Dx Dy.  
-0002a7c0: 2020 2320 7072 6f64 7563 7428 7261 6e67    # product(rang
-0002a7d0: 6528 3229 2c20 7265 7065 6174 3d33 2920  e(2), repeat=3) 
-0002a7e0: 2d2d 3e20 3030 3020 3030 3120 3031 3020  --> 000 001 010 
-0002a7f0: 3031 3120 3130 3020 3130 3120 3131 3020  011 100 101 110 
-0002a800: 3131 310a 2020 2020 706f 6f6c 7320 3d20  111.    pools = 
-0002a810: 5b74 7570 6c65 2870 6f6f 6c29 2066 6f72  [tuple(pool) for
-0002a820: 2070 6f6f 6c20 696e 2061 7267 735d 202a   pool in args] *
-0002a830: 2072 6570 6561 740a 2020 2020 7265 7375   repeat.    resu
-0002a840: 6c74 203d 205b 5b5d 5d0a 2020 2020 666f  lt = [[]].    fo
-0002a850: 7220 706f 6f6c 2069 6e20 706f 6f6c 733a  r pool in pools:
-0002a860: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0002a870: 3d20 5b78 2b5b 795d 2066 6f72 2078 2069  = [x+[y] for x i
-0002a880: 6e20 7265 7375 6c74 2066 6f72 2079 2069  n result for y i
-0002a890: 6e20 706f 6f6c 5d0a 2020 2020 666f 7220  n pool].    for 
-0002a8a0: 7072 6f64 2069 6e20 7265 7375 6c74 3a0a  prod in result:.
-0002a8b0: 2020 2020 2020 2020 7969 656c 6420 7475          yield tu
-0002a8c0: 706c 6528 7072 6f64 290a 6060 600a 0a42  ple(prod).```..B
-0002a8d0: 6566 6f72 6520 6063 6172 7465 7369 616e  efore `cartesian
-0002a8e0: 5f70 726f 6475 6374 2829 6020 7275 6e73  _product()` runs
-0002a8f0: 2c20 6974 2063 6f6d 706c 6574 656c 7920  , it completely 
-0002a900: 636f 6e73 756d 6573 2074 6865 2069 6e70  consumes the inp
-0002a910: 7574 2069 7465 7261 626c 6573 2c20 6b65  ut iterables, ke
-0002a920: 6570 696e 6720 706f 6f6c 7320 6f66 2076  eping pools of v
-0002a930: 616c 7565 7320 696e 206d 656d 6f72 7920  alues in memory 
-0002a940: 746f 2067 656e 6572 6174 6520 7468 6520  to generate the 
-0002a950: 7072 6f64 7563 7473 2e20 4163 636f 7264  products. Accord
-0002a960: 696e 676c 792c 2069 7420 6973 206f 6e6c  ingly, it is onl
-0002a970: 7920 7573 6566 756c 2077 6974 6820 6669  y useful with fi
-0002a980: 6e69 7465 2069 6e70 7574 732e 0a0a 2323  nite inputs...##
-0002a990: 2323 2320 4578 616d 706c 650a 0a2a 2a43  ### Example..**C
-0002a9a0: 6f63 6f6e 7574 3a2a 2a0a 6060 6063 6f63  oconut:**.```coc
-0002a9b0: 6f6e 7574 0a76 203d 205b 312c 2032 5d0a  onut.v = [1, 2].
-0002a9c0: 6173 7365 7274 2063 6172 7465 7369 616e  assert cartesian
-0002a9d0: 5f70 726f 6475 6374 2876 2c20 7629 207c  _product(v, v) |
-0002a9e0: 3e20 6c69 7374 203d 3d20 5b28 312c 2031  > list == [(1, 1
-0002a9f0: 292c 2028 312c 2032 292c 2028 322c 2031  ), (1, 2), (2, 1
-0002aa00: 292c 2028 322c 2032 295d 0a60 6060 0a0a  ), (2, 2)].```..
-0002aa10: 2a2a 5079 7468 6f6e 3a2a 2a0a 6060 6063  **Python:**.```c
-0002aa20: 6f63 6f6e 7574 5f70 7974 686f 6e0a 6672  oconut_python.fr
-0002aa30: 6f6d 2069 7465 7274 6f6f 6c73 2069 6d70  om itertools imp
-0002aa40: 6f72 7420 7072 6f64 7563 740a 7620 3d20  ort product.v = 
-0002aa50: 5b31 2c20 325d 0a61 7373 6572 7420 6c69  [1, 2].assert li
-0002aa60: 7374 2870 726f 6475 6374 2876 2c20 7629  st(product(v, v)
-0002aa70: 2920 3d3d 205b 2831 2c20 3129 2c20 2831  ) == [(1, 1), (1
-0002aa80: 2c20 3229 2c20 2832 2c20 3129 2c20 2832  , 2), (2, 1), (2
-0002aa90: 2c20 3229 5d0a 6060 600a 0a23 2323 2320  , 2)].```..#### 
-0002aaa0: 606d 756c 7469 5f65 6e75 6d65 7261 7465  `multi_enumerate
-0002aab0: 600a 0a2a 2a6d 756c 7469 5c5f 656e 756d  `..**multi\_enum
-0002aac0: 6572 6174 652a 2a28 5f69 7465 7261 626c  erate**(_iterabl
-0002aad0: 655f 290a 0a43 6f63 6f6e 7574 2773 2060  e_)..Coconut's `
-0002aae0: 6d75 6c74 695f 656e 756d 6572 6174 6560  multi_enumerate`
-0002aaf0: 2065 6e75 6d65 7261 7465 7320 7468 726f   enumerates thro
-0002ab00: 7567 6820 616e 2069 7465 7261 626c 6520  ugh an iterable 
-0002ab10: 6f66 2069 7465 7261 626c 6573 2e20 606d  of iterables. `m
-0002ab20: 756c 7469 5f65 6e75 6d65 7261 7465 6020  ulti_enumerate` 
-0002ab30: 776f 726b 7320 6c69 6b65 2065 6e75 6d65  works like enume
-0002ab40: 7261 7465 2c20 6275 7420 696e 6465 7865  rate, but indexe
-0002ab50: 7320 7468 726f 7567 6820 696e 6e65 7220  s through inner 
-0002ab60: 6974 6572 6162 6c65 7320 616e 6420 7072  iterables and pr
-0002ab70: 6f64 7563 6573 2061 2074 7570 6c65 2069  oduces a tuple i
-0002ab80: 6e64 6578 2072 6570 7265 7365 6e74 696e  ndex representin
-0002ab90: 6720 7468 6520 696e 6465 7820 696e 2065  g the index in e
-0002aba0: 6163 6820 696e 6e65 7220 6974 6572 6162  ach inner iterab
-0002abb0: 6c65 2e20 5375 7070 6f72 7473 2069 6e64  le. Supports ind
-0002abc0: 6578 696e 672e 0a0a 466f 7220 5b60 6e75  exing...For [`nu
-0002abd0: 6d70 7960 5d28 236e 756d 7079 2d69 6e74  mpy`](#numpy-int
-0002abe0: 6567 7261 7469 6f6e 2920 6f62 6a65 6374  egration) object
-0002abf0: 732c 2075 7365 7320 5b60 6e70 2e6e 6469  s, uses [`np.ndi
-0002ac00: 7465 7260 5d28 6874 7470 733a 2f2f 6e75  ter`](https://nu
-0002ac10: 6d70 792e 6f72 672f 646f 632f 7374 6162  mpy.org/doc/stab
-0002ac20: 6c65 2f72 6566 6572 656e 6365 2f67 656e  le/reference/gen
-0002ac30: 6572 6174 6564 2f6e 756d 7079 2e6e 6469  erated/numpy.ndi
-0002ac40: 7465 722e 6874 6d6c 2920 756e 6465 7220  ter.html) under 
-0002ac50: 7468 6520 686f 6f64 2e20 416c 736f 2073  the hood. Also s
-0002ac60: 7570 706f 7274 7320 606c 656e 6020 666f  upports `len` fo
-0002ac70: 7220 5b60 6e75 6d70 7960 5d28 236e 756d  r [`numpy`](#num
-0002ac80: 7079 2d69 6e74 6567 7261 7469 6f6e 2920  py-integration) 
-0002ac90: 6172 7261 7973 2e0a 0a23 2323 2323 2045  arrays...##### E
-0002aca0: 7861 6d70 6c65 0a0a 2a2a 436f 636f 6e75  xample..**Coconu
-0002acb0: 743a 2a2a 0a60 6060 636f 636f 6e75 745f  t:**.```coconut_
-0002acc0: 7079 636f 6e0a 3e3e 3e20 5b31 2c20 323b  pycon.>>> [1, 2;
-0002acd0: 3b20 332c 2034 5d20 7c3e 206d 756c 7469  ; 3, 4] |> multi
-0002ace0: 5f65 6e75 6d65 7261 7465 207c 3e20 6c69  _enumerate |> li
-0002acf0: 7374 0a5b 2828 302c 2030 292c 2031 292c  st.[((0, 0), 1),
-0002ad00: 2028 2830 2c20 3129 2c20 3229 2c20 2828   ((0, 1), 2), ((
-0002ad10: 312c 2030 292c 2033 292c 2028 2831 2c20  1, 0), 3), ((1, 
-0002ad20: 3129 2c20 3429 5d0a 6060 600a 0a2a 2a50  1), 4)].```..**P
-0002ad30: 7974 686f 6e3a 2a2a 0a60 6060 636f 636f  ython:**.```coco
-0002ad40: 6e75 745f 7079 7468 6f6e 0a61 7272 6179  nut_python.array
-0002ad50: 203d 205b 5b31 2c20 325d 2c20 5b33 2c20   = [[1, 2], [3, 
-0002ad60: 345d 5d0a 656e 756d 6572 6174 6564 5f61  4]].enumerated_a
-0002ad70: 7272 6179 203d 205b 5d0a 666f 7220 6920  rray = [].for i 
-0002ad80: 696e 2072 616e 6765 286c 656e 2861 7272  in range(len(arr
-0002ad90: 6179 2929 3a0a 2020 2020 666f 7220 6a20  ay)):.    for j 
-0002ada0: 696e 2072 616e 6765 286c 656e 2861 7272  in range(len(arr
-0002adb0: 6179 5b69 5d29 293a 0a20 2020 2020 2020  ay[i])):.       
-0002adc0: 2065 6e75 6d65 7261 7465 645f 6172 7261   enumerated_arra
-0002add0: 792e 6170 7065 6e64 2828 2869 2c20 6a29  y.append(((i, j)
-0002ade0: 2c20 6172 7261 795b 695d 5b6a 5d29 290a  , array[i][j])).
-0002adf0: 6060 600a 0a23 2323 2320 6067 726f 7570  ```..#### `group
-0002ae00: 736f 6660 0a0a 2a2a 6772 6f75 7073 6f66  sof`..**groupsof
-0002ae10: 2a2a 285f 6e5f 2c20 5f69 7465 7261 626c  **(_n_, _iterabl
-0002ae20: 655f 2c20 5f66 696c 6c76 616c 7565 5f3d  e_, _fillvalue_=
-0002ae30: 602e 2e2e 6029 0a0a 436f 636f 6e75 7420  `...`)..Coconut 
-0002ae40: 7072 6f76 6964 6573 2074 6865 2060 6772  provides the `gr
-0002ae50: 6f75 7073 6f66 6020 6275 696c 742d 696e  oupsof` built-in
-0002ae60: 2074 6f20 7370 6c69 7420 616e 2069 7465   to split an ite
-0002ae70: 7261 626c 6520 696e 746f 2067 726f 7570  rable into group
-0002ae80: 7320 6f66 2061 2073 7065 6369 6669 6320  s of a specific 
-0002ae90: 6c65 6e67 7468 2e20 5370 6563 6966 6963  length. Specific
-0002aea0: 616c 6c79 2c20 6067 726f 7570 736f 6628  ally, `groupsof(
-0002aeb0: 6e2c 2069 7465 7261 626c 6529 6020 7769  n, iterable)` wi
-0002aec0: 6c6c 2073 706c 6974 2060 6974 6572 6162  ll split `iterab
-0002aed0: 6c65 6020 696e 746f 2074 7570 6c65 7320  le` into tuples 
-0002aee0: 6f66 206c 656e 6774 6820 606e 602c 2077  of length `n`, w
-0002aef0: 6974 6820 6f6e 6c79 2074 6865 206c 6173  ith only the las
-0002af00: 7420 7475 706c 6520 706f 7465 6e74 6961  t tuple potentia
-0002af10: 6c6c 7920 6f66 2073 697a 6520 603c 206e  lly of size `< n
-0002af20: 6020 6966 2074 6865 206c 656e 6774 6820  ` if the length 
-0002af30: 6f66 2060 6974 6572 6162 6c65 6020 6973  of `iterable` is
-0002af40: 206e 6f74 2064 6976 6973 6962 6c65 2062   not divisible b
-0002af50: 7920 606e 602e 2049 6620 7468 6174 2069  y `n`. If that i
-0002af60: 7320 6e6f 7420 7468 6520 6465 7369 7265  s not the desire
-0002af70: 6420 6265 6861 7669 6f72 2c20 5f66 696c  d behavior, _fil
-0002af80: 6c76 616c 7565 5f20 6361 6e20 6265 2070  lvalue_ can be p
-0002af90: 6173 7365 6420 616e 6420 7769 6c6c 2062  assed and will b
-0002afa0: 6520 7573 6564 2074 6f20 7061 6420 7468  e used to pad th
-0002afb0: 6520 656e 6420 6f66 2074 6865 206c 6173  e end of the las
-0002afc0: 7420 7475 706c 6520 746f 206c 656e 6774  t tuple to lengt
-0002afd0: 6820 606e 602e 0a0a 4164 6469 7469 6f6e  h `n`...Addition
-0002afe0: 616c 6c79 2c20 6067 726f 7570 736f 6660  ally, `groupsof`
-0002aff0: 2073 7570 706f 7274 7320 606c 656e 6020   supports `len` 
-0002b000: 7768 656e 2060 6974 6572 6162 6c65 6020  when `iterable` 
-0002b010: 7375 7070 6f72 7473 2060 6c65 6e60 2e0a  supports `len`..
-0002b020: 0a23 2323 2323 2045 7861 6d70 6c65 0a0a  .##### Example..
-0002b030: 2a2a 436f 636f 6e75 743a 2a2a 0a60 6060  **Coconut:**.```
-0002b040: 636f 636f 6e75 740a 7061 6972 7320 3d20  coconut.pairs = 
-0002b050: 7261 6e67 6528 312c 2031 3129 207c 3e20  range(1, 11) |> 
-0002b060: 6772 6f75 7073 6f66 2428 3229 0a60 6060  groupsof$(2).```
-0002b070: 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a 6060  ..**Python:**.``
-0002b080: 6063 6f63 6f6e 7574 5f70 7974 686f 6e0a  `coconut_python.
-0002b090: 7061 6972 7320 3d20 5b5d 0a67 726f 7570  pairs = [].group
-0002b0a0: 203d 205b 5d0a 666f 7220 6974 656d 2069   = [].for item i
-0002b0b0: 6e20 7261 6e67 6528 312c 2031 3129 3a0a  n range(1, 11):.
-0002b0c0: 2020 2020 6772 6f75 702e 6170 7065 6e64      group.append
-0002b0d0: 2869 7465 6d29 0a20 2020 2069 6620 6c65  (item).    if le
-0002b0e0: 6e28 6772 6f75 7029 203d 3d20 323a 0a20  n(group) == 2:. 
-0002b0f0: 2020 2020 2020 2070 6169 7273 2e61 7070         pairs.app
-0002b100: 656e 6428 7475 706c 6528 6772 6f75 7029  end(tuple(group)
-0002b110: 290a 2020 2020 2020 2020 6772 6f75 7020  ).        group 
-0002b120: 3d20 5b5d 0a69 6620 6772 6f75 703a 0a20  = [].if group:. 
-0002b130: 2020 2070 6169 7273 2e61 7070 656e 6428     pairs.append(
-0002b140: 7475 706c 6528 6772 6f75 7029 290a 6060  tuple(group)).``
-0002b150: 600a 0a23 2323 2320 6077 696e 646f 7773  `..#### `windows
-0002b160: 6f66 600a 0a2a 2a77 696e 646f 7773 6f66  of`..**windowsof
-0002b170: 2a2a 285f 7369 7a65 5f2c 205f 6974 6572  **(_size_, _iter
-0002b180: 6162 6c65 5f2c 205f 6669 6c6c 7661 6c75  able_, _fillvalu
-0002b190: 655f 3d60 2e2e 2e60 2c20 5f73 7465 705f  e_=`...`, _step_
-0002b1a0: 3d60 3160 290a 0a60 7769 6e64 6f77 736f  =`1`)..`windowso
-0002b1b0: 6660 2070 726f 6475 6365 7320 616e 2069  f` produces an i
-0002b1c0: 7465 7261 626c 6520 7468 6174 2065 6666  terable that eff
-0002b1d0: 6563 7469 7665 6c79 206d 696d 6963 7320  ectively mimics 
-0002b1e0: 6120 736c 6964 696e 6720 7769 6e64 6f77  a sliding window
-0002b1f0: 206f 7665 7220 5f69 7465 7261 626c 655f   over _iterable_
-0002b200: 206f 6620 7369 7a65 205f 7369 7a65 5f2e   of size _size_.
-0002b210: 205f 7374 6570 5f20 6465 7465 726d 696e   _step_ determin
-0002b220: 6573 2074 6865 2073 7061 6369 6e67 2062  es the spacing b
-0002b230: 6574 7765 656e 2077 696e 646f 7773 2e0a  etween windows..
-0002b240: 0a49 6620 5f73 697a 655f 2069 7320 6c61  .If _size_ is la
-0002b250: 7267 6572 2074 6861 6e20 5f69 7465 7261  rger than _itera
-0002b260: 626c 655f 2c20 6077 696e 646f 7773 6f66  ble_, `windowsof
-0002b270: 6020 7769 6c6c 2070 726f 6475 6365 2061  ` will produce a
-0002b280: 6e20 656d 7074 7920 6974 6572 6162 6c65  n empty iterable
-0002b290: 2e20 4966 2074 6861 7420 6973 206e 6f74  . If that is not
-0002b2a0: 2074 6865 2064 6573 6972 6564 2062 6568   the desired beh
-0002b2b0: 6176 696f 722c 205f 6669 6c6c 7661 6c75  avior, _fillvalu
-0002b2c0: 655f 2063 616e 2062 6520 7061 7373 6564  e_ can be passed
-0002b2d0: 2061 6e64 2077 696c 6c20 6265 2075 7365   and will be use
-0002b2e0: 6420 696e 2070 6c61 6365 206f 6620 6d69  d in place of mi
-0002b2f0: 7373 696e 6720 7661 6c75 6573 2e20 416c  ssing values. Al
-0002b300: 736f 2c20 6966 205f 6669 6c6c 7661 6c75  so, if _fillvalu
-0002b310: 655f 2069 7320 7061 7373 6564 2061 6e64  e_ is passed and
-0002b320: 2074 6865 206c 656e 6774 6820 6f66 2074   the length of t
-0002b330: 6865 205f 6974 6572 6162 6c65 5f20 6973  he _iterable_ is
-0002b340: 206e 6f74 2064 6976 6973 6962 6c65 2062   not divisible b
-0002b350: 7920 5f73 7465 705f 2c20 5f66 696c 6c76  y _step_, _fillv
-0002b360: 616c 7565 5f20 7769 6c6c 2062 6520 7573  alue_ will be us
-0002b370: 6564 2069 6e20 7468 6174 2063 6173 6520  ed in that case 
-0002b380: 746f 2070 6164 2074 6865 206c 6173 7420  to pad the last 
-0002b390: 7769 6e64 6f77 2061 7320 7765 6c6c 2e20  window as well. 
-0002b3a0: 4e6f 7465 2074 6861 7420 5f66 696c 6c76  Note that _fillv
-0002b3b0: 616c 7565 5f20 7769 6c6c 206f 6e6c 7920  alue_ will only 
-0002b3c0: 6576 6572 2061 7070 6561 7220 696e 2074  ever appear in t
-0002b3d0: 6865 206c 6173 7420 7769 6e64 6f77 2e0a  he last window..
-0002b3e0: 0a41 6464 6974 696f 6e61 6c6c 792c 2060  .Additionally, `
-0002b3f0: 7769 6e64 6f77 736f 6660 2073 7570 706f  windowsof` suppo
-0002b400: 7274 7320 606c 656e 6020 7768 656e 2060  rts `len` when `
-0002b410: 6974 6572 6162 6c65 6020 7375 7070 6f72  iterable` suppor
-0002b420: 7473 2060 6c65 6e60 2e0a 0a23 2323 2323  ts `len`...#####
-0002b430: 2045 7861 6d70 6c65 0a0a 2a2a 436f 636f   Example..**Coco
-0002b440: 6e75 743a 2a2a 0a60 6060 636f 636f 6e75  nut:**.```coconu
-0002b450: 740a 6173 7365 7274 2022 3132 3334 3522  t.assert "12345"
-0002b460: 207c 3e20 7769 6e64 6f77 736f 6624 2833   |> windowsof$(3
-0002b470: 2920 7c3e 206c 6973 7420 3d3d 205b 2822  ) |> list == [("
-0002b480: 3122 2c20 2232 222c 2022 3322 292c 2028  1", "2", "3"), (
-0002b490: 2232 222c 2022 3322 2c20 2234 2229 2c20  "2", "3", "4"), 
-0002b4a0: 2822 3322 2c20 2234 222c 2022 3522 295d  ("3", "4", "5")]
-0002b4b0: 0a60 6060 0a0a 2a2a 5079 7468 6f6e 3a2a  .```..**Python:*
-0002b4c0: 2a0a 5f43 616e 2774 2062 6520 646f 6e65  *._Can't be done
-0002b4d0: 2077 6974 686f 7574 2074 6865 2064 6566   without the def
-0002b4e0: 696e 6974 696f 6e20 6f66 2060 7769 6e64  inition of `wind
-0002b4f0: 6f77 736f 6660 3b20 7365 6520 7468 6520  owsof`; see the 
-0002b500: 636f 6d70 696c 6564 2068 6561 6465 7220  compiled header 
-0002b510: 666f 7220 7468 6520 6675 6c6c 2064 6566  for the full def
-0002b520: 696e 6974 696f 6e2e 5f0a 0a23 2323 2320  inition._..#### 
-0002b530: 6063 6f6c 6c65 6374 6279 600a 0a2a 2a63  `collectby`..**c
-0002b540: 6f6c 6c65 6374 6279 2a2a 285f 6b65 795c  ollectby**(_key\
-0002b550: 5f66 756e 635f 2c20 5f69 7465 7261 626c  _func_, _iterabl
-0002b560: 655f 2c20 5f76 616c 7565 5c5f 6675 6e63  e_, _value\_func
-0002b570: 5f3d 604e 6f6e 6560 2c20 5f72 6564 7563  _=`None`, _reduc
-0002b580: 655c 5f66 756e 635f 3d60 4e6f 6e65 6029  e\_func_=`None`)
-0002b590: 0a0a 6063 6f6c 6c65 6374 6279 286b 6579  ..`collectby(key
-0002b5a0: 5f66 756e 632c 2069 7465 7261 626c 6529  _func, iterable)
-0002b5b0: 6020 636f 6c6c 6563 7473 2074 6865 2069  ` collects the i
-0002b5c0: 7465 6d73 2069 6e20 6069 7465 7261 626c  tems in `iterabl
-0002b5d0: 6560 2069 6e74 6f20 6120 6469 6374 696f  e` into a dictio
-0002b5e0: 6e61 7279 206f 6620 6c69 7374 7320 6b65  nary of lists ke
-0002b5f0: 7965 6420 6279 2060 6b65 795f 6675 6e63  yed by `key_func
-0002b600: 2869 7465 6d29 602e 0a0a 4966 2060 7661  (item)`...If `va
-0002b610: 6c75 655f 6675 6e63 6020 6973 2070 6173  lue_func` is pas
-0002b620: 7365 642c 2060 636f 6c6c 6563 7462 7928  sed, `collectby(
-0002b630: 6b65 795f 6675 6e63 2c20 6974 6572 6162  key_func, iterab
-0002b640: 6c65 2c20 7661 6c75 655f 6675 6e63 3d76  le, value_func=v
-0002b650: 616c 7565 5f66 756e 6329 6020 696e 7374  alue_func)` inst
-0002b660: 6561 6420 636f 6c6c 6563 7473 2076 616c  ead collects val
-0002b670: 7565 5f66 756e 6328 6974 656d 2920 696e  ue_func(item) in
-0002b680: 746f 2065 6163 6820 6c69 7374 2069 6e73  to each list ins
-0002b690: 7465 6164 206f 6620 6974 656d 2e0a 0a49  tead of item...I
-0002b6a0: 6620 6072 6564 7563 655f 6675 6e63 6020  f `reduce_func` 
-0002b6b0: 6973 2070 6173 7365 642c 2060 636f 6c6c  is passed, `coll
-0002b6c0: 6563 7462 7928 6b65 795f 6675 6e63 2c20  ectby(key_func, 
-0002b6d0: 6974 6572 6162 6c65 2c20 7265 6475 6365  iterable, reduce
-0002b6e0: 5f66 756e 633d 7265 6475 6365 5f66 756e  _func=reduce_fun
-0002b6f0: 6329 602c 2069 6e73 7465 6164 206f 6620  c)`, instead of 
-0002b700: 636f 6c6c 6563 7469 6e67 2074 6865 2069  collecting the i
-0002b710: 7465 6d73 2069 6e74 6f20 6c69 7374 732c  tems into lists,
-0002b720: 2072 6564 7563 6573 206f 7665 7220 7468   reduces over th
-0002b730: 6520 6974 656d 7320 6f66 2065 6163 6820  e items of each 
-0002b740: 6b65 7920 7769 7468 2072 6564 7563 655f  key with reduce_
-0002b750: 6675 6e63 2c20 6566 6665 6374 6976 656c  func, effectivel
-0002b760: 7920 696d 706c 656d 656e 7469 6e67 2061  y implementing a
-0002b770: 204d 6170 5265 6475 6365 206f 7065 7261   MapReduce opera
-0002b780: 7469 6f6e 2e0a 0a60 636f 6c6c 6563 7462  tion...`collectb
-0002b790: 7960 2069 7320 6566 6665 6374 6976 656c  y` is effectivel
-0002b7a0: 7920 6571 7569 7661 6c65 6e74 2074 6f3a  y equivalent to:
-0002b7b0: 0a60 6060 636f 636f 6e75 745f 7079 7468  .```coconut_pyth
-0002b7c0: 6f6e 0a66 726f 6d20 636f 6c6c 6563 7469  on.from collecti
-0002b7d0: 6f6e 7320 696d 706f 7274 2064 6566 6175  ons import defau
-0002b7e0: 6c74 6469 6374 0a0a 6465 6620 636f 6c6c  ltdict..def coll
-0002b7f0: 6563 7462 7928 6b65 795f 6675 6e63 2c20  ectby(key_func, 
-0002b800: 6974 6572 6162 6c65 2c20 7661 6c75 655f  iterable, value_
-0002b810: 6675 6e63 3d69 6465 6e74 2c20 7265 6475  func=ident, redu
-0002b820: 6365 5f66 756e 633d 4e6f 6e65 293a 0a20  ce_func=None):. 
-0002b830: 2020 2063 6f6c 6c65 6374 696f 6e20 3d20     collection = 
-0002b840: 6465 6661 756c 7464 6963 7428 6c69 7374  defaultdict(list
-0002b850: 2920 6966 2072 6564 7563 655f 6675 6e63  ) if reduce_func
-0002b860: 2069 7320 4e6f 6e65 2065 6c73 6520 7b7d   is None else {}
-0002b870: 0a20 2020 2066 6f72 2069 7465 6d20 696e  .    for item in
-0002b880: 2069 7465 7261 626c 653a 0a20 2020 2020   iterable:.     
-0002b890: 2020 206b 6579 203d 206b 6579 5f66 756e     key = key_fun
-0002b8a0: 6328 6974 656d 290a 2020 2020 2020 2020  c(item).        
-0002b8b0: 7661 6c75 6520 3d20 7661 6c75 655f 6675  value = value_fu
-0002b8c0: 6e63 2869 7465 6d29 0a20 2020 2020 2020  nc(item).       
-0002b8d0: 2069 6620 7265 6475 6365 5f66 756e 6320   if reduce_func 
-0002b8e0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0002b8f0: 2020 2020 2063 6f6c 6c65 6374 696f 6e5b       collection[
-0002b900: 6b65 795d 2e61 7070 656e 6428 7661 6c75  key].append(valu
-0002b910: 6529 0a20 2020 2020 2020 2065 6c73 653a  e).        else:
-0002b920: 0a20 2020 2020 2020 2020 2020 206f 6c64  .            old
-0002b930: 5f76 616c 7565 203d 2063 6f6c 6c65 6374  _value = collect
-0002b940: 696f 6e2e 6765 7428 6b65 792c 2073 656e  ion.get(key, sen
-0002b950: 7469 6e65 6c29 0a20 2020 2020 2020 2020  tinel).         
-0002b960: 2020 2069 6620 6f6c 645f 7661 6c75 6520     if old_value 
-0002b970: 6973 206e 6f74 2073 656e 7469 6e65 6c3a  is not sentinel:
-0002b980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b990: 2076 616c 7565 203d 2072 6564 7563 655f   value = reduce_
-0002b9a0: 6675 6e63 286f 6c64 5f76 616c 7565 2c20  func(old_value, 
-0002b9b0: 7661 6c75 6529 0a20 2020 2020 2020 2020  value).         
-0002b9c0: 2020 2063 6f6c 6c65 6374 696f 6e5b 6b65     collection[ke
-0002b9d0: 795d 203d 2076 616c 7565 0a20 2020 2072  y] = value.    r
-0002b9e0: 6574 7572 6e20 636f 6c6c 6563 7469 6f6e  eturn collection
-0002b9f0: 0a60 6060 0a0a 6063 6f6c 6c65 6374 6279  .```..`collectby
-0002ba00: 6020 6973 2073 696d 696c 6172 2074 6f20  ` is similar to 
-0002ba10: 5b60 6974 6572 746f 6f6c 732e 6772 6f75  [`itertools.grou
-0002ba20: 7062 7960 5d28 6874 7470 733a 2f2f 646f  pby`](https://do
-0002ba30: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
-0002ba40: 6c69 6272 6172 792f 6974 6572 746f 6f6c  library/itertool
-0002ba50: 732e 6874 6d6c 2369 7465 7274 6f6f 6c73  s.html#itertools
-0002ba60: 2e67 726f 7570 6279 2920 6578 6365 7074  .groupby) except
-0002ba70: 2074 6861 7420 6063 6f6c 6c65 6374 6279   that `collectby
-0002ba80: 6020 6167 6772 6567 6174 6573 2063 6f6d  ` aggregates com
-0002ba90: 6d6f 6e20 656c 656d 656e 7473 2072 6567  mon elements reg
-0002baa0: 6172 646c 6573 7320 6f66 2074 6865 6972  ardless of their
-0002bab0: 206f 7264 6572 2069 6e20 7468 6520 696e   order in the in
-0002bac0: 7075 7420 6974 6572 6162 6c65 2c20 7768  put iterable, wh
-0002bad0: 6572 6561 7320 6067 726f 7570 6279 6020  ereas `groupby` 
-0002bae0: 6f6e 6c79 2061 6767 7265 6761 7465 7320  only aggregates 
-0002baf0: 636f 6d6d 6f6e 2065 6c65 6d65 6e74 7320  common elements 
-0002bb00: 7468 6174 2061 7265 2061 646a 6163 656e  that are adjacen
-0002bb10: 7420 696e 2074 6865 2069 6e70 7574 2069  t in the input i
-0002bb20: 7465 7261 626c 652e 0a0a 2323 2323 2320  terable...##### 
-0002bb30: 4578 616d 706c 650a 0a2a 2a43 6f63 6f6e  Example..**Cocon
-0002bb40: 7574 3a2a 2a0a 6060 6063 6f63 6f6e 7574  ut:**.```coconut
-0002bb50: 0a75 7365 725f 6261 6c61 6e63 6573 203d  .user_balances =
-0002bb60: 2028 0a20 2020 2062 616c 616e 6365 5f64   (.    balance_d
-0002bb70: 6174 610a 2020 2020 7c3e 2063 6f6c 6c65  ata.    |> colle
-0002bb80: 6374 6279 2428 2e75 7365 722c 2076 616c  ctby$(.user, val
-0002bb90: 7565 5f66 756e 633d 2e62 616c 616e 6365  ue_func=.balance
-0002bba0: 2c20 7265 6475 6365 5f66 756e 633d 282b  , reduce_func=(+
-0002bbb0: 2929 0a29 0a60 6060 0a0a 2a2a 5079 7468  )).).```..**Pyth
-0002bbc0: 6f6e 3a2a 2a0a 6060 6063 6f63 6f6e 7574  on:**.```coconut
-0002bbd0: 5f70 7974 686f 6e0a 6672 6f6d 2063 6f6c  _python.from col
-0002bbe0: 6c65 6374 696f 6e73 2069 6d70 6f72 7420  lections import 
-0002bbf0: 6465 6661 756c 7464 6963 740a 0a75 7365  defaultdict..use
-0002bc00: 725f 6261 6c61 6e63 6573 203d 2064 6566  r_balances = def
-0002bc10: 6175 6c74 6469 6374 2869 6e74 290a 666f  aultdict(int).fo
-0002bc20: 7220 6974 656d 2069 6e20 6261 6c61 6e63  r item in balanc
-0002bc30: 655f 6461 7461 3a0a 2020 2020 7573 6572  e_data:.    user
-0002bc40: 5f62 616c 616e 6365 735b 6974 656d 2e75  _balances[item.u
-0002bc50: 7365 725d 202b 3d20 6974 656d 2e62 616c  ser] += item.bal
-0002bc60: 616e 6365 0a60 6060 0a0a 2323 2323 2060  ance.```..#### `
-0002bc70: 616c 6c5f 6571 7561 6c60 0a0a 2a2a 616c  all_equal`..**al
-0002bc80: 6c5c 5f65 7175 616c 2a2a 285f 6974 6572  l\_equal**(_iter
-0002bc90: 6162 6c65 5f29 0a0a 436f 636f 6e75 7427  able_)..Coconut'
-0002bca0: 7320 6061 6c6c 5f65 7175 616c 6020 6275  s `all_equal` bu
-0002bcb0: 696c 742d 696e 2074 616b 6573 2069 6e20  ilt-in takes in 
-0002bcc0: 616e 2069 7465 7261 626c 6520 616e 6420  an iterable and 
-0002bcd0: 6465 7465 726d 696e 6573 2077 6865 7468  determines wheth
-0002bce0: 6572 2061 6c6c 206f 6620 6974 7320 656c  er all of its el
-0002bcf0: 656d 656e 7473 2061 7265 2065 7175 616c  ements are equal
-0002bd00: 2074 6f20 6561 6368 206f 7468 6572 2e20   to each other. 
-0002bd10: 6061 6c6c 5f65 7175 616c 6020 6173 7375  `all_equal` assu
-0002bd20: 6d65 7320 7472 616e 7369 7469 7669 7479  mes transitivity
-0002bd30: 206f 6620 6571 7561 6c69 7479 2061 6e64   of equality and
-0002bd40: 2074 6861 7420 6021 3d60 2069 7320 7468   that `!=` is th
-0002bd50: 6520 6e65 6761 7469 6f6e 206f 6620 603d  e negation of `=
-0002bd60: 3d60 2e20 5370 6563 6961 6c20 7375 7070  =`. Special supp
-0002bd70: 6f72 7420 6973 2070 726f 7669 6465 6420  ort is provided 
-0002bd80: 666f 7220 5b60 6e75 6d70 7960 5d28 236e  for [`numpy`](#n
-0002bd90: 756d 7079 2d69 6e74 6567 7261 7469 6f6e  umpy-integration
-0002bda0: 2920 6f62 6a65 6374 732e 0a0a 2323 2323  ) objects...####
-0002bdb0: 2320 4578 616d 706c 650a 0a2a 2a43 6f63  # Example..**Coc
-0002bdc0: 6f6e 7574 3a2a 2a0a 6060 6063 6f63 6f6e  onut:**.```cocon
-0002bdd0: 7574 0a61 6c6c 5f65 7175 616c 285b 312c  ut.all_equal([1,
-0002bde0: 2031 2c20 315d 290a 616c 6c5f 6571 7561   1, 1]).all_equa
-0002bdf0: 6c28 5b31 2c20 312c 2032 5d29 0a60 6060  l([1, 1, 2]).```
-0002be00: 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a 6060  ..**Python:**.``
-0002be10: 6063 6f63 6f6e 7574 5f70 7974 686f 6e0a  `coconut_python.
-0002be20: 7365 6e74 696e 656c 203d 206f 626a 6563  sentinel = objec
-0002be30: 7428 290a 6465 6620 616c 6c5f 6571 7561  t().def all_equa
-0002be40: 6c28 6974 6572 6162 6c65 293a 0a20 2020  l(iterable):.   
-0002be50: 2066 6972 7374 5f69 7465 6d20 3d20 7365   first_item = se
-0002be60: 6e74 696e 656c 0a20 2020 2066 6f72 2069  ntinel.    for i
-0002be70: 7465 6d20 696e 2069 7465 7261 626c 653a  tem in iterable:
-0002be80: 0a20 2020 2020 2020 2069 6620 6669 7273  .        if firs
-0002be90: 745f 6974 656d 2069 7320 7365 6e74 696e  t_item is sentin
-0002bea0: 656c 3a0a 2020 2020 2020 2020 2020 2020  el:.            
-0002beb0: 6669 7273 745f 6974 656d 203d 2069 7465  first_item = ite
-0002bec0: 6d0a 2020 2020 2020 2020 656c 6966 2066  m.        elif f
-0002bed0: 6972 7374 5f69 7465 6d20 213d 2069 7465  irst_item != ite
-0002bee0: 6d3a 0a20 2020 2020 2020 2020 2020 2072  m:.            r
-0002bef0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-0002bf00: 7265 7475 726e 2054 7275 650a 616c 6c5f  return True.all_
-0002bf10: 6571 7561 6c28 5b31 2c20 312c 2031 5d29  equal([1, 1, 1])
-0002bf20: 0a61 6c6c 5f65 7175 616c 285b 312c 2031  .all_equal([1, 1
-0002bf30: 2c20 325d 290a 6060 600a 0a23 2323 2320  , 2]).```..#### 
-0002bf40: 6070 6172 616c 6c65 6c5f 6d61 7060 0a0a  `parallel_map`..
-0002bf50: 2a2a 7061 7261 6c6c 656c 5c5f 6d61 702a  **parallel\_map*
-0002bf60: 2a28 5f66 756e 6374 696f 6e5f 2c20 2a5f  *(_function_, *_
-0002bf70: 6974 6572 6162 6c65 735f 2c20 2a2c 205f  iterables_, *, _
-0002bf80: 6368 756e 6b73 697a 655f 3d60 3160 2c20  chunksize_=`1`, 
-0002bf90: 5f73 7472 6963 745f 3d60 4661 6c73 6560  _strict_=`False`
-0002bfa0: 290a 0a43 6f63 6f6e 7574 2070 726f 7669  )..Coconut provi
-0002bfb0: 6465 7320 6120 7061 7261 6c6c 656c 2076  des a parallel v
-0002bfc0: 6572 7369 6f6e 206f 6620 606d 6170 6020  ersion of `map` 
-0002bfd0: 756e 6465 7220 7468 6520 6e61 6d65 2060  under the name `
-0002bfe0: 7061 7261 6c6c 656c 5f6d 6170 602e 2060  parallel_map`. `
-0002bff0: 7061 7261 6c6c 656c 5f6d 6170 6020 6d61  parallel_map` ma
-0002c000: 6b65 7320 7573 6520 6f66 206d 756c 7469  kes use of multi
-0002c010: 706c 6520 7072 6f63 6573 7365 732c 2061  ple processes, a
-0002c020: 6e64 2069 7320 7468 6572 6566 6f72 6520  nd is therefore 
-0002c030: 6d75 6368 2066 6173 7465 7220 7468 616e  much faster than
-0002c040: 2060 6d61 7060 2066 6f72 2043 5055 2d62   `map` for CPU-b
-0002c050: 6f75 6e64 2074 6173 6b73 2e20 6070 6172  ound tasks. `par
-0002c060: 616c 6c65 6c5f 6d61 7060 206e 6576 6572  allel_map` never
-0002c070: 206c 6f61 6473 2074 6865 2065 6e74 6972   loads the entir
-0002c080: 6520 696e 7075 7420 6974 6572 6174 6f72  e input iterator
-0002c090: 2069 6e74 6f20 6d65 6d6f 7279 2c20 7468   into memory, th
-0002c0a0: 6f75 6768 2069 7420 646f 6573 2063 6f6e  ough it does con
-0002c0b0: 7375 6d65 2074 6865 2065 6e74 6972 6520  sume the entire 
-0002c0c0: 696e 7075 7420 6974 6572 6174 6f72 2061  input iterator a
-0002c0d0: 7320 736f 6f6e 2061 7320 6120 7369 6e67  s soon as a sing
-0002c0e0: 6c65 206f 7574 7075 7420 6973 2072 6571  le output is req
-0002c0f0: 7565 7374 6564 2e20 4966 2061 6e79 2065  uested. If any e
-0002c100: 7863 6570 7469 6f6e 7320 6172 6520 7261  xceptions are ra
-0002c110: 6973 6564 2069 6e73 6964 6520 6f66 2060  ised inside of `
-0002c120: 7061 7261 6c6c 656c 5f6d 6170 602c 2061  parallel_map`, a
-0002c130: 2074 7261 6365 6261 636b 2077 696c 6c20   traceback will 
-0002c140: 6265 2070 7269 6e74 6564 2061 7320 736f  be printed as so
-0002c150: 6f6e 2061 7320 7468 6579 2061 7265 2065  on as they are e
-0002c160: 6e63 6f75 6e74 6572 6564 2e0a 0a42 6563  ncountered...Bec
-0002c170: 6175 7365 2060 7061 7261 6c6c 656c 5f6d  ause `parallel_m
-0002c180: 6170 6020 7573 6573 206d 756c 7469 706c  ap` uses multipl
-0002c190: 6520 7072 6f63 6573 7365 7320 666f 7220  e processes for 
-0002c1a0: 6974 7320 6578 6563 7574 696f 6e2c 2069  its execution, i
-0002c1b0: 7420 6973 206e 6563 6573 7361 7279 2074  t is necessary t
-0002c1c0: 6861 7420 616c 6c20 6f66 2069 7473 2061  hat all of its a
-0002c1d0: 7267 756d 656e 7473 2062 6520 7069 636b  rguments be pick
-0002c1e0: 6c65 6162 6c65 2e20 4f6e 6c79 206f 626a  leable. Only obj
-0002c1f0: 6563 7473 2064 6566 696e 6564 2061 7420  ects defined at 
-0002c200: 7468 6520 6d6f 6475 6c65 206c 6576 656c  the module level
-0002c210: 2c20 616e 6420 6e6f 7420 6c61 6d62 6461  , and not lambda
-0002c220: 732c 206f 626a 6563 7473 2064 6566 696e  s, objects defin
-0002c230: 6564 2069 6e73 6964 6520 6f66 2061 2066  ed inside of a f
-0002c240: 756e 6374 696f 6e2c 206f 7220 6f62 6a65  unction, or obje
-0002c250: 6374 7320 6465 6669 6e65 6420 696e 7369  cts defined insi
-0002c260: 6465 206f 6620 7468 6520 696e 7465 7270  de of the interp
-0002c270: 7265 7465 722c 2061 7265 2070 6963 6b6c  reter, are pickl
-0002c280: 6561 626c 652e 2046 7572 7468 6572 6d6f  eable. Furthermo
-0002c290: 7265 2c20 6f6e 2057 696e 646f 7773 2c20  re, on Windows, 
-0002c2a0: 6974 2069 7320 6e65 6365 7373 6172 7920  it is necessary 
-0002c2b0: 7468 6174 2061 6c6c 2063 616c 6c73 2074  that all calls t
-0002c2c0: 6f20 6070 6172 616c 6c65 6c5f 6d61 7060  o `parallel_map`
-0002c2d0: 206f 6363 7572 2069 6e73 6964 6520 6f66   occur inside of
-0002c2e0: 2061 6e20 6069 6620 5f5f 6e61 6d65 5f5f   an `if __name__
-0002c2f0: 203d 3d20 225f 5f6d 6169 6e5f 5f22 6020   == "__main__"` 
-0002c300: 6775 6172 642e 0a0a 6070 6172 616c 6c65  guard...`paralle
-0002c310: 6c5f 6d61 7060 2073 7570 706f 7274 7320  l_map` supports 
-0002c320: 6120 6063 6875 6e6b 7369 7a65 6020 6172  a `chunksize` ar
-0002c330: 6775 6d65 6e74 2c20 7768 6963 6820 6465  gument, which de
-0002c340: 7465 726d 696e 6573 2068 6f77 206d 616e  termines how man
-0002c350: 7920 6974 656d 7320 6172 6520 7061 7373  y items are pass
-0002c360: 6564 2074 6f20 6561 6368 2070 726f 6365  ed to each proce
-0002c370: 7373 2061 7420 6120 7469 6d65 2e20 4c61  ss at a time. La
-0002c380: 7267 6572 2076 616c 7565 7320 6f66 205f  rger values of _
-0002c390: 6368 756e 6b73 697a 655f 2061 7265 2072  chunksize_ are r
-0002c3a0: 6563 6f6d 6d65 6e64 6564 2077 6865 6e20  ecommended when 
-0002c3b0: 6465 616c 696e 6720 7769 7468 2076 6572  dealing with ver
-0002c3c0: 7920 6c6f 6e67 2069 7465 7261 626c 6573  y long iterables
-0002c3d0: 2e20 4164 6469 7469 6f6e 616c 6c79 2c20  . Additionally, 
-0002c3e0: 696e 2074 6865 206d 756c 7469 2d69 7465  in the multi-ite
-0002c3f0: 7261 626c 6520 6361 7365 2c20 5f73 7472  rable case, _str
-0002c400: 6963 745f 2063 616e 2062 6520 7365 7420  ict_ can be set 
-0002c410: 746f 2060 5472 7565 6020 746f 2065 6e73  to `True` to ens
-0002c420: 7572 6520 7468 6174 2061 6c6c 2069 7465  ure that all ite
-0002c430: 7261 626c 6573 2061 7265 2074 6865 2073  rables are the s
-0002c440: 616d 6520 6c65 6e67 7468 2e0a 0a49 6620  ame length...If 
-0002c450: 6d75 6c74 6970 6c65 2073 6571 7565 6e74  multiple sequent
-0002c460: 6961 6c20 6361 6c6c 7320 746f 2060 7061  ial calls to `pa
-0002c470: 7261 6c6c 656c 5f6d 6170 6020 6e65 6564  rallel_map` need
-0002c480: 2074 6f20 6265 206d 6164 652c 2069 7420   to be made, it 
-0002c490: 6973 2068 6967 686c 7920 7265 636f 6d6d  is highly recomm
-0002c4a0: 656e 6465 6420 7468 6174 2074 6865 7920  ended that they 
-0002c4b0: 6265 2064 6f6e 6520 696e 7369 6465 206f  be done inside o
-0002c4c0: 6620 6120 6077 6974 6820 7061 7261 6c6c  f a `with parall
-0002c4d0: 656c 5f6d 6170 2e6d 756c 7469 706c 655f  el_map.multiple_
-0002c4e0: 7365 7175 656e 7469 616c 5f63 616c 6c73  sequential_calls
-0002c4f0: 2829 3a60 2062 6c6f 636b 2c20 7768 6963  ():` block, whic
-0002c500: 6820 7769 6c6c 2063 6175 7365 2074 6865  h will cause the
-0002c510: 2064 6966 6665 7265 6e74 2063 616c 6c73   different calls
-0002c520: 2074 6f20 7573 6520 7468 6520 7361 6d65   to use the same
-0002c530: 2070 726f 6365 7373 2070 6f6f 6c20 616e   process pool an
-0002c540: 6420 7265 7375 6c74 2069 6e20 6070 6172  d result in `par
-0002c550: 616c 6c65 6c5f 6d61 7060 2069 6d6d 6564  allel_map` immed
-0002c560: 6961 7465 6c79 2072 6574 7572 6e69 6e67  iately returning
-0002c570: 2061 206c 6973 7420 7261 7468 6572 2074   a list rather t
-0002c580: 6861 6e20 6120 6070 6172 616c 6c65 6c5f  han a `parallel_
-0002c590: 6d61 7060 206f 626a 6563 742e 2049 6620  map` object. If 
-0002c5a0: 6d75 6c74 6970 6c65 2073 6571 7565 6e74  multiple sequent
-0002c5b0: 6961 6c20 6361 6c6c 7320 6172 6520 6e65  ial calls are ne
-0002c5c0: 6365 7373 6172 7920 616e 6420 7468 6520  cessary and the 
-0002c5d0: 6c61 7a69 6e65 7373 206f 6620 7061 7261  laziness of para
-0002c5e0: 6c6c 656c 5f6d 6170 2069 7320 7265 7175  llel_map is requ
-0002c5f0: 6972 6564 2c20 7468 656e 2074 6865 2060  ired, then the `
-0002c600: 7061 7261 6c6c 656c 5f6d 6170 6020 6f62  parallel_map` ob
-0002c610: 6a65 6374 7320 7368 6f75 6c64 2062 6520  jects should be 
-0002c620: 636f 6e73 7472 7563 7465 6420 6265 666f  constructed befo
-0002c630: 7265 2074 6865 2060 6d75 6c74 6970 6c65  re the `multiple
-0002c640: 5f73 6571 7565 6e74 6961 6c5f 6361 6c6c  _sequential_call
-0002c650: 7360 2062 6c6f 636b 2061 6e64 2074 6865  s` block and the
-0002c660: 6e20 6f6e 6c79 2069 7465 7261 7465 6420  n only iterated 
-0002c670: 6f76 6572 206f 6e63 6520 696e 7369 6465  over once inside
-0002c680: 2074 6865 2062 6c6f 636b 2e0a 0a60 7061   the block...`pa
-0002c690: 7261 6c6c 656c 5f6d 6170 2e6d 756c 7469  rallel_map.multi
-0002c6a0: 706c 655f 7365 7175 656e 7469 616c 5f63  ple_sequential_c
-0002c6b0: 616c 6c73 6020 616c 736f 2073 7570 706f  alls` also suppo
-0002c6c0: 7274 7320 6120 606d 6178 5f77 6f72 6b65  rts a `max_worke
-0002c6d0: 7273 6020 6172 6775 6d65 6e74 2074 6f20  rs` argument to 
-0002c6e0: 7365 7420 7468 6520 6e75 6d62 6572 206f  set the number o
-0002c6f0: 6620 7072 6f63 6573 7365 732e 0a0a 2323  f processes...##
-0002c700: 2323 2320 5079 7468 6f6e 2044 6f63 730a  ### Python Docs.
-0002c710: 0a2a 2a70 6172 616c 6c65 6c5f 6d61 702a  .**parallel_map*
-0002c720: 2a28 5f66 756e 632c 205c 2a69 7465 7261  *(_func, \*itera
-0002c730: 626c 6573 5f2c 205f 6368 756e 6b73 697a  bles_, _chunksiz
-0002c740: 655f 3d60 3160 290a 0a45 7175 6976 616c  e_=`1`)..Equival
-0002c750: 656e 7420 746f 2060 6d61 7028 6675 6e63  ent to `map(func
-0002c760: 2c20 2a69 7465 7261 626c 6573 2960 2065  , *iterables)` e
-0002c770: 7863 6570 7420 5f66 756e 635f 2069 7320  xcept _func_ is 
-0002c780: 6578 6563 7574 6564 2061 7379 6e63 6872  executed asynchr
-0002c790: 6f6e 6f75 736c 7920 616e 6420 7365 7665  onously and seve
-0002c7a0: 7261 6c20 6361 6c6c 7320 746f 205f 6675  ral calls to _fu
-0002c7b0: 6e63 5f20 6d61 7920 6265 206d 6164 6520  nc_ may be made 
-0002c7c0: 636f 6e63 7572 7265 6e74 6c79 2e20 4966  concurrently. If
-0002c7d0: 2061 2063 616c 6c20 7261 6973 6573 2061   a call raises a
-0002c7e0: 6e20 6578 6365 7074 696f 6e2c 2074 6865  n exception, the
-0002c7f0: 6e20 7468 6174 2065 7863 6570 7469 6f6e  n that exception
-0002c800: 2077 696c 6c20 6265 2072 6169 7365 6420   will be raised 
-0002c810: 7768 656e 2069 7473 2076 616c 7565 2069  when its value i
-0002c820: 7320 7265 7472 6965 7665 6420 6672 6f6d  s retrieved from
-0002c830: 2074 6865 2069 7465 7261 746f 722e 0a0a   the iterator...
-0002c840: 6070 6172 616c 6c65 6c5f 6d61 7060 2063  `parallel_map` c
-0002c850: 686f 7073 2074 6865 2069 7465 7261 626c  hops the iterabl
-0002c860: 6520 696e 746f 2061 206e 756d 6265 7220  e into a number 
-0002c870: 6f66 2063 6875 6e6b 7320 7768 6963 6820  of chunks which 
-0002c880: 6974 2073 7562 6d69 7473 2074 6f20 7468  it submits to th
-0002c890: 6520 7072 6f63 6573 7320 706f 6f6c 2061  e process pool a
-0002c8a0: 7320 7365 7061 7261 7465 2074 6173 6b73  s separate tasks
-0002c8b0: 2e20 5468 6520 2861 7070 726f 7869 6d61  . The (approxima
-0002c8c0: 7465 2920 7369 7a65 206f 6620 7468 6573  te) size of thes
-0002c8d0: 6520 6368 756e 6b73 2063 616e 2062 6520  e chunks can be 
-0002c8e0: 7370 6563 6966 6965 6420 6279 2073 6574  specified by set
-0002c8f0: 7469 6e67 205f 6368 756e 6b73 697a 655f  ting _chunksize_
-0002c900: 2074 6f20 6120 706f 7369 7469 7665 2069   to a positive i
-0002c910: 6e74 6567 6572 2e20 466f 7220 7665 7279  nteger. For very
-0002c920: 206c 6f6e 6720 6974 6572 6162 6c65 7320   long iterables 
-0002c930: 7573 696e 6720 6120 6c61 7267 6520 7661  using a large va
-0002c940: 6c75 6520 666f 7220 5f63 6875 6e6b 7369  lue for _chunksi
-0002c950: 7a65 5f20 6361 6e20 6d61 6b65 2074 6865  ze_ can make the
-0002c960: 206a 6f62 2063 6f6d 706c 6574 6520 2a2a   job complete **
-0002c970: 6d75 6368 2a2a 2066 6173 7465 7220 7468  much** faster th
-0002c980: 616e 2075 7369 6e67 2074 6865 2064 6566  an using the def
-0002c990: 6175 6c74 2076 616c 7565 206f 6620 6031  ault value of `1
-0002c9a0: 602e 0a0a 2323 2323 2320 4578 616d 706c  `...##### Exampl
-0002c9b0: 650a 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a  e..**Coconut:**.
-0002c9c0: 6060 6063 6f63 6f6e 7574 0a70 6172 616c  ```coconut.paral
-0002c9d0: 6c65 6c5f 6d61 7028 706f 7724 2832 292c  lel_map(pow$(2),
-0002c9e0: 2072 616e 6765 2831 3030 2929 207c 3e20   range(100)) |> 
-0002c9f0: 6c69 7374 207c 3e20 7072 696e 740a 6060  list |> print.``
-0002ca00: 600a 0a2a 2a50 7974 686f 6e3a 2a2a 0a60  `..**Python:**.`
-0002ca10: 6060 636f 636f 6e75 745f 7079 7468 6f6e  ``coconut_python
-0002ca20: 0a69 6d70 6f72 7420 6675 6e63 746f 6f6c  .import functool
-0002ca30: 730a 6672 6f6d 206d 756c 7469 7072 6f63  s.from multiproc
-0002ca40: 6573 7369 6e67 2069 6d70 6f72 7420 506f  essing import Po
-0002ca50: 6f6c 0a77 6974 6820 506f 6f6c 2829 2061  ol.with Pool() a
-0002ca60: 7320 706f 6f6c 3a0a 2020 2020 7072 696e  s pool:.    prin
-0002ca70: 7428 6c69 7374 2870 6f6f 6c2e 696d 6170  t(list(pool.imap
-0002ca80: 2866 756e 6374 6f6f 6c73 2e70 6172 7469  (functools.parti
-0002ca90: 616c 2870 6f77 2c20 3229 2c20 7261 6e67  al(pow, 2), rang
-0002caa0: 6528 3130 3029 2929 290a 6060 600a 0a23  e(100)))).```..#
-0002cab0: 2323 2320 6063 6f6e 6375 7272 656e 745f  ### `concurrent_
-0002cac0: 6d61 7060 0a0a 2a2a 636f 6e63 7572 7265  map`..**concurre
-0002cad0: 6e74 5c5f 6d61 702a 2a28 5f66 756e 6374  nt\_map**(_funct
-0002cae0: 696f 6e5f 2c20 2a5f 6974 6572 6162 6c65  ion_, *_iterable
-0002caf0: 735f 2c20 2a2c 205f 6368 756e 6b73 697a  s_, *, _chunksiz
-0002cb00: 655f 3d60 3160 2c20 5f73 7472 6963 745f  e_=`1`, _strict_
-0002cb10: 3d60 4661 6c73 6560 290a 0a43 6f63 6f6e  =`False`)..Cocon
-0002cb20: 7574 2070 726f 7669 6465 7320 6120 636f  ut provides a co
-0002cb30: 6e63 7572 7265 6e74 2076 6572 7369 6f6e  ncurrent version
-0002cb40: 206f 6620 5b60 7061 7261 6c6c 656c 5f6d   of [`parallel_m
-0002cb50: 6170 605d 2823 7061 7261 6c6c 656c 5f6d  ap`](#parallel_m
-0002cb60: 6170 2920 756e 6465 7220 7468 6520 6e61  ap) under the na
-0002cb70: 6d65 2060 636f 6e63 7572 7265 6e74 5f6d  me `concurrent_m
-0002cb80: 6170 602e 2060 636f 6e63 7572 7265 6e74  ap`. `concurrent
-0002cb90: 5f6d 6170 6020 6265 6861 7665 7320 6964  _map` behaves id
-0002cba0: 656e 7469 6361 6c6c 7920 746f 2060 7061  entically to `pa
-0002cbb0: 7261 6c6c 656c 5f6d 6170 6020 2869 6e63  rallel_map` (inc
-0002cbc0: 6c75 6469 6e67 2073 7570 706f 7274 2066  luding support f
-0002cbd0: 6f72 2060 636f 6e63 7572 7265 6e74 5f6d  or `concurrent_m
-0002cbe0: 6170 2e6d 756c 7469 706c 655f 7365 7175  ap.multiple_sequ
-0002cbf0: 656e 7469 616c 5f63 616c 6c73 6029 2065  ential_calls`) e
-0002cc00: 7863 6570 7420 7468 6174 2069 7420 7573  xcept that it us
-0002cc10: 6573 206d 756c 7469 7468 7265 6164 696e  es multithreadin
-0002cc20: 6720 696e 7374 6561 6420 6f66 206d 756c  g instead of mul
-0002cc30: 7469 7072 6f63 6573 7369 6e67 2c20 616e  tiprocessing, an
-0002cc40: 6420 6973 2074 6865 7265 666f 7265 2070  d is therefore p
-0002cc50: 7269 6d61 7269 6c79 2075 7365 6675 6c20  rimarily useful 
-0002cc60: 6f6e 6c79 2066 6f72 2049 4f2d 626f 756e  only for IO-boun
-0002cc70: 6420 7461 736b 7320 6475 6520 746f 2043  d tasks due to C
-0002cc80: 5079 7468 6f6e 2773 2047 6c6f 6261 6c20  Python's Global 
-0002cc90: 496e 7465 7270 7265 7465 7220 4c6f 636b  Interpreter Lock
-0002cca0: 2e0a 0a23 2323 2323 2050 7974 686f 6e20  ...##### Python 
-0002ccb0: 446f 6373 0a0a 2a2a 636f 6e63 7572 7265  Docs..**concurre
-0002ccc0: 6e74 5f6d 6170 2a2a 285f 6675 6e63 2c20  nt_map**(_func, 
-0002ccd0: 5c2a 6974 6572 6162 6c65 735f 2c20 5f63  \*iterables_, _c
-0002cce0: 6875 6e6b 7369 7a65 5f3d 6031 6029 0a0a  hunksize_=`1`)..
-0002ccf0: 4571 7569 7661 6c65 6e74 2074 6f20 606d  Equivalent to `m
-0002cd00: 6170 2866 756e 632c 202a 6974 6572 6162  ap(func, *iterab
-0002cd10: 6c65 7329 6020 6578 6365 7074 205f 6675  les)` except _fu
-0002cd20: 6e63 5f20 6973 2065 7865 6375 7465 6420  nc_ is executed 
-0002cd30: 6173 796e 6368 726f 6e6f 7573 6c79 2061  asynchronously a
-0002cd40: 6e64 2073 6576 6572 616c 2063 616c 6c73  nd several calls
-0002cd50: 2074 6f20 5f66 756e 635f 206d 6179 2062   to _func_ may b
-0002cd60: 6520 6d61 6465 2063 6f6e 6375 7272 656e  e made concurren
-0002cd70: 746c 792e 2049 6620 6120 6361 6c6c 2072  tly. If a call r
-0002cd80: 6169 7365 7320 616e 2065 7863 6570 7469  aises an excepti
-0002cd90: 6f6e 2c20 7468 656e 2074 6861 7420 6578  on, then that ex
-0002cda0: 6365 7074 696f 6e20 7769 6c6c 2062 6520  ception will be 
-0002cdb0: 7261 6973 6564 2077 6865 6e20 6974 7320  raised when its 
-0002cdc0: 7661 6c75 6520 6973 2072 6574 7269 6576  value is retriev
-0002cdd0: 6564 2066 726f 6d20 7468 6520 6974 6572  ed from the iter
-0002cde0: 6174 6f72 2e0a 0a60 636f 6e63 7572 7265  ator...`concurre
-0002cdf0: 6e74 5f6d 6170 6020 6368 6f70 7320 7468  nt_map` chops th
-0002ce00: 6520 6974 6572 6162 6c65 2069 6e74 6f20  e iterable into 
-0002ce10: 6120 6e75 6d62 6572 206f 6620 6368 756e  a number of chun
-0002ce20: 6b73 2077 6869 6368 2069 7420 7375 626d  ks which it subm
-0002ce30: 6974 7320 746f 2074 6865 2074 6872 6561  its to the threa
-0002ce40: 6420 706f 6f6c 2061 7320 7365 7061 7261  d pool as separa
-0002ce50: 7465 2074 6173 6b73 2e20 5468 6520 2861  te tasks. The (a
-0002ce60: 7070 726f 7869 6d61 7465 2920 7369 7a65  pproximate) size
-0002ce70: 206f 6620 7468 6573 6520 6368 756e 6b73   of these chunks
-0002ce80: 2063 616e 2062 6520 7370 6563 6966 6965   can be specifie
-0002ce90: 6420 6279 2073 6574 7469 6e67 205f 6368  d by setting _ch
-0002cea0: 756e 6b73 697a 655f 2074 6f20 6120 706f  unksize_ to a po
-0002ceb0: 7369 7469 7665 2069 6e74 6567 6572 2e20  sitive integer. 
-0002cec0: 466f 7220 7665 7279 206c 6f6e 6720 6974  For very long it
-0002ced0: 6572 6162 6c65 7320 7573 696e 6720 6120  erables using a 
-0002cee0: 6c61 7267 6520 7661 6c75 6520 666f 7220  large value for 
-0002cef0: 5f63 6875 6e6b 7369 7a65 5f20 6361 6e20  _chunksize_ can 
-0002cf00: 6d61 6b65 2074 6865 206a 6f62 2063 6f6d  make the job com
-0002cf10: 706c 6574 6520 2a2a 6d75 6368 2a2a 2066  plete **much** f
-0002cf20: 6173 7465 7220 7468 616e 2075 7369 6e67  aster than using
-0002cf30: 2074 6865 2064 6566 6175 6c74 2076 616c   the default val
-0002cf40: 7565 206f 6620 6031 602e 0a0a 2323 2323  ue of `1`...####
-0002cf50: 2320 4578 616d 706c 650a 0a2a 2a43 6f63  # Example..**Coc
-0002cf60: 6f6e 7574 3a2a 2a0a 6060 6063 6f63 6f6e  onut:**.```cocon
-0002cf70: 7574 0a63 6f6e 6375 7272 656e 745f 6d61  ut.concurrent_ma
-0002cf80: 7028 6765 745f 6461 7461 5f66 6f72 5f75  p(get_data_for_u
-0002cf90: 7365 722c 2067 6574 5f61 6c6c 5f75 7365  ser, get_all_use
-0002cfa0: 7273 2829 2920 7c3e 206c 6973 7420 7c3e  rs()) |> list |>
-0002cfb0: 2070 7269 6e74 0a60 6060 0a0a 2a2a 5079   print.```..**Py
-0002cfc0: 7468 6f6e 3a2a 2a0a 6060 6063 6f63 6f6e  thon:**.```cocon
-0002cfd0: 7574 5f70 7974 686f 6e0a 696d 706f 7274  ut_python.import
-0002cfe0: 2066 756e 6374 6f6f 6c73 0a69 6d70 6f72   functools.impor
-0002cff0: 7420 636f 6e63 7572 7265 6e74 2e66 7574  t concurrent.fut
-0002d000: 7572 6573 0a77 6974 6820 636f 6e63 7572  ures.with concur
-0002d010: 7265 6e74 2e66 7574 7572 6573 2e54 6872  rent.futures.Thr
-0002d020: 6561 6450 6f6f 6c45 7865 6375 746f 7228  eadPoolExecutor(
-0002d030: 2920 6173 2065 7865 6375 746f 723a 0a20  ) as executor:. 
-0002d040: 2020 2070 7269 6e74 286c 6973 7428 6578     print(list(ex
-0002d050: 6563 7574 6f72 2e6d 6170 2867 6574 5f64  ecutor.map(get_d
-0002d060: 6174 615f 666f 725f 7573 6572 2c20 6765  ata_for_user, ge
-0002d070: 745f 616c 6c5f 7573 6572 7328 2929 2929  t_all_users())))
-0002d080: 0a60 6060 0a0a 2323 2323 2060 7465 6560  .```..#### `tee`
-0002d090: 0a0a 2a2a 7465 652a 2a28 5f69 7465 7261  ..**tee**(_itera
-0002d0a0: 626c 655f 2c20 5f6e 5f3d 6032 6029 0a0a  ble_, _n_=`2`)..
-0002d0b0: 436f 636f 6e75 7420 7072 6f76 6964 6573  Coconut provides
-0002d0c0: 2061 6e20 6f70 7469 6d69 7a65 6420 7665   an optimized ve
-0002d0d0: 7273 696f 6e20 6f66 2060 6974 6572 746f  rsion of `iterto
-0002d0e0: 6f6c 732e 7465 6560 2061 7320 6120 6275  ols.tee` as a bu
-0002d0f0: 696c 742d 696e 2075 6e64 6572 2074 6865  ilt-in under the
-0002d100: 206e 616d 6520 6074 6565 602e 0a0a 5468   name `tee`...Th
-0002d110: 6f75 6768 2060 7465 6560 2069 7320 6e6f  ough `tee` is no
-0002d120: 7420 6465 7072 6563 6174 6564 2c20 5b60  t deprecated, [`
-0002d130: 7265 6974 6572 6162 6c65 605d 2823 7265  reiterable`](#re
-0002d140: 6974 6572 6162 6c65 2920 6973 2067 656e  iterable) is gen
-0002d150: 6572 616c 6c79 2072 6563 6f6d 6d65 6e64  erally recommend
-0002d160: 6564 206f 7665 7220 6074 6565 602e 0a0a  ed over `tee`...
-0002d170: 4375 7374 6f6d 2060 7465 6560 2f60 7265  Custom `tee`/`re
-0002d180: 6974 6572 6162 6c65 6020 696d 706c 656d  iterable` implem
-0002d190: 656e 7461 7469 6f6e 7320 666f 7220 6375  entations for cu
-0002d1a0: 7374 6f6d 205b 436f 6e74 6169 6e65 7273  stom [Containers
-0002d1b0: 2f43 6f6c 6c65 6374 696f 6e73 5d28 6874  /Collections](ht
-0002d1c0: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
-0002d1d0: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
-0002d1e0: 636f 6c6c 6563 7469 6f6e 732e 6162 632e  collections.abc.
-0002d1f0: 6874 6d6c 2920 7368 6f75 6c64 2062 6520  html) should be 
-0002d200: 7075 7420 696e 2074 6865 2060 5f5f 636f  put in the `__co
-0002d210: 7079 5f5f 6020 6d65 7468 6f64 2e20 4e6f  py__` method. No
-0002d220: 7465 2074 6861 7420 616c 6c20 5b53 6571  te that all [Seq
-0002d230: 7565 6e63 6573 2f4d 6170 7069 6e67 732f  uences/Mappings/
-0002d240: 5365 7473 5d28 6874 7470 733a 2f2f 646f  Sets](https://do
-0002d250: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
-0002d260: 6c69 6272 6172 792f 636f 6c6c 6563 7469  library/collecti
-0002d270: 6f6e 732e 6162 632e 6874 6d6c 2920 6172  ons.abc.html) ar
-0002d280: 6520 616c 7761 7973 2061 7373 756d 6564  e always assumed
-0002d290: 2074 6f20 6265 2072 6569 7465 7261 626c   to be reiterabl
-0002d2a0: 6520 6576 656e 2077 6974 686f 7574 2063  e even without c
-0002d2b0: 616c 6c69 6e67 2060 5f5f 636f 7079 5f5f  alling `__copy__
-0002d2c0: 602e 0a0a 2323 2323 2320 5079 7468 6f6e  `...##### Python
-0002d2d0: 2044 6f63 730a 0a2a 2a74 6565 2a2a 285f   Docs..**tee**(_
-0002d2e0: 6974 6572 6162 6c65 2c20 6e3d 325f 290a  iterable, n=2_).
-0002d2f0: 0a52 6574 7572 6e20 5f6e 5f20 696e 6465  .Return _n_ inde
-0002d300: 7065 6e64 656e 7420 6974 6572 6174 6f72  pendent iterator
-0002d310: 7320 6672 6f6d 2061 2073 696e 676c 6520  s from a single 
-0002d320: 6974 6572 6162 6c65 2e20 4571 7569 7661  iterable. Equiva
-0002d330: 6c65 6e74 2074 6f3a 0a60 6060 636f 636f  lent to:.```coco
-0002d340: 6e75 745f 7079 7468 6f6e 0a64 6566 2074  nut_python.def t
-0002d350: 6565 2869 7465 7261 626c 652c 206e 3d32  ee(iterable, n=2
-0002d360: 293a 0a20 2020 2069 7420 3d20 6974 6572  ):.    it = iter
-0002d370: 2869 7465 7261 626c 6529 0a20 2020 2064  (iterable).    d
-0002d380: 6571 7565 7320 3d20 5b63 6f6c 6c65 6374  eques = [collect
-0002d390: 696f 6e73 2e64 6571 7565 2829 2066 6f72  ions.deque() for
-0002d3a0: 2069 2069 6e20 7261 6e67 6528 6e29 5d0a   i in range(n)].
-0002d3b0: 2020 2020 6465 6620 6765 6e28 6d79 6465      def gen(myde
-0002d3c0: 7175 6529 3a0a 2020 2020 2020 2020 7768  que):.        wh
-0002d3d0: 696c 6520 5472 7565 3a0a 2020 2020 2020  ile True:.      
-0002d3e0: 2020 2020 2020 6966 206e 6f74 206d 7964        if not myd
-0002d3f0: 6571 7565 3a20 2020 2020 2020 2020 2020  eque:           
-0002d400: 2020 2320 7768 656e 2074 6865 206c 6f63    # when the loc
-0002d410: 616c 2064 6571 7565 2069 7320 656d 7074  al deque is empt
-0002d420: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-0002d430: 2020 6e65 7776 616c 203d 206e 6578 7428    newval = next(
-0002d440: 6974 2920 2020 2020 2020 2320 6665 7463  it)       # fetc
-0002d450: 6820 6120 6e65 7720 7661 6c75 6520 616e  h a new value an
-0002d460: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-0002d470: 2020 666f 7220 6420 696e 2064 6571 7565    for d in deque
-0002d480: 733a 2020 2020 2020 2020 2320 6c6f 6164  s:        # load
-0002d490: 2069 7420 746f 2061 6c6c 2074 6865 2064   it to all the d
-0002d4a0: 6571 7565 730a 2020 2020 2020 2020 2020  eques.          
-0002d4b0: 2020 2020 2020 2020 2020 642e 6170 7065            d.appe
-0002d4c0: 6e64 286e 6577 7661 6c29 0a20 2020 2020  nd(newval).     
-0002d4d0: 2020 2020 2020 2079 6965 6c64 206d 7964         yield myd
-0002d4e0: 6571 7565 2e70 6f70 6c65 6674 2829 0a20  eque.popleft(). 
-0002d4f0: 2020 2072 6574 7572 6e20 7475 706c 6528     return tuple(
-0002d500: 6765 6e28 6429 2066 6f72 2064 2069 6e20  gen(d) for d in 
-0002d510: 6465 7175 6573 290a 6060 600a 4f6e 6365  deques).```.Once
-0002d520: 2060 7465 6528 2960 2068 6173 206d 6164   `tee()` has mad
-0002d530: 6520 6120 7370 6c69 742c 2074 6865 206f  e a split, the o
-0002d540: 7269 6769 6e61 6c20 5f69 7465 7261 626c  riginal _iterabl
-0002d550: 655f 2073 686f 756c 6420 6e6f 7420 6265  e_ should not be
-0002d560: 2075 7365 6420 616e 7977 6865 7265 2065   used anywhere e
-0002d570: 6c73 653b 206f 7468 6572 7769 7365 2c20  lse; otherwise, 
-0002d580: 7468 6520 5f69 7465 7261 626c 655f 2063  the _iterable_ c
-0002d590: 6f75 6c64 2067 6574 2061 6476 616e 6365  ould get advance
-0002d5a0: 6420 7769 7468 6f75 7420 7468 6520 7465  d without the te
-0002d5b0: 6520 6f62 6a65 6374 7320 6265 696e 6720  e objects being 
-0002d5c0: 696e 666f 726d 6564 2e0a 0a54 6869 7320  informed...This 
-0002d5d0: 6974 6572 746f 6f6c 206d 6179 2072 6571  itertool may req
-0002d5e0: 7569 7265 2073 6967 6e69 6669 6361 6e74  uire significant
-0002d5f0: 2061 7578 696c 6961 7279 2073 746f 7261   auxiliary stora
-0002d600: 6765 2028 6465 7065 6e64 696e 6720 6f6e  ge (depending on
-0002d610: 2068 6f77 206d 7563 6820 7465 6d70 6f72   how much tempor
-0002d620: 6172 7920 6461 7461 206e 6565 6473 2074  ary data needs t
-0002d630: 6f20 6265 2073 746f 7265 6429 2e20 496e  o be stored). In
-0002d640: 2067 656e 6572 616c 2c20 6966 206f 6e65   general, if one
-0002d650: 2069 7465 7261 746f 7220 7573 6573 206d   iterator uses m
-0002d660: 6f73 7420 6f72 2061 6c6c 206f 6620 7468  ost or all of th
-0002d670: 6520 6461 7461 2062 6566 6f72 6520 616e  e data before an
-0002d680: 6f74 6865 7220 6974 6572 6174 6f72 2073  other iterator s
-0002d690: 7461 7274 732c 2069 7420 6973 2066 6173  tarts, it is fas
-0002d6a0: 7465 7220 746f 2075 7365 2060 6c69 7374  ter to use `list
-0002d6b0: 2829 6020 696e 7374 6561 6420 6f66 2060  ()` instead of `
-0002d6c0: 7465 6528 2960 2e0a 0a23 2323 2323 2045  tee()`...##### E
-0002d6d0: 7861 6d70 6c65 0a0a 2a2a 436f 636f 6e75  xample..**Coconu
-0002d6e0: 743a 2a2a 0a60 6060 636f 636f 6e75 740a  t:**.```coconut.
-0002d6f0: 6f72 6967 696e 616c 2c20 7465 6d70 203d  original, temp =
-0002d700: 2074 6565 286f 7269 6769 6e61 6c29 0a73   tee(original).s
-0002d710: 6c69 6365 6420 3d20 7465 6d70 245b 353a  liced = temp$[5:
-0002d720: 5d0a 6060 600a 0a2a 2a50 7974 686f 6e3a  ].```..**Python:
-0002d730: 2a2a 0a60 6060 636f 636f 6e75 745f 7079  **.```coconut_py
-0002d740: 7468 6f6e 0a69 6d70 6f72 7420 6974 6572  thon.import iter
-0002d750: 746f 6f6c 730a 6f72 6967 696e 616c 2c20  tools.original, 
-0002d760: 7465 6d70 203d 2069 7465 7274 6f6f 6c73  temp = itertools
-0002d770: 2e74 6565 286f 7269 6769 6e61 6c29 0a73  .tee(original).s
-0002d780: 6c69 6365 6420 3d20 6974 6572 746f 6f6c  liced = itertool
-0002d790: 732e 6973 6c69 6365 2874 656d 702c 2035  s.islice(temp, 5
-0002d7a0: 2c20 4e6f 6e65 290a 6060 600a 0a23 2323  , None).```..###
-0002d7b0: 2320 6063 6f6e 7375 6d65 600a 0a2a 2a63  # `consume`..**c
-0002d7c0: 6f6e 7375 6d65 2a2a 285f 6974 6572 6162  onsume**(_iterab
-0002d7d0: 6c65 5f2c 205f 6b65 6570 5c5f 6c61 7374  le_, _keep\_last
-0002d7e0: 5f3d 6030 6029 0a0a 436f 636f 6e75 7420  _=`0`)..Coconut 
-0002d7f0: 7072 6f76 6964 6573 2074 6865 2060 636f  provides the `co
-0002d800: 6e73 756d 6560 2066 756e 6374 696f 6e20  nsume` function 
-0002d810: 746f 2065 6666 6963 6965 6e74 6c79 2065  to efficiently e
-0002d820: 7868 6175 7374 2061 6e20 6974 6572 6174  xhaust an iterat
-0002d830: 6f72 2061 6e64 2074 6875 7320 7065 7266  or and thus perf
-0002d840: 6f72 6d20 616e 7920 6c61 7a79 2065 7661  orm any lazy eva
-0002d850: 6c75 6174 696f 6e20 636f 6e74 6169 6e65  luation containe
-0002d860: 6420 7769 7468 696e 2069 742e 2060 636f  d within it. `co
-0002d870: 6e73 756d 6560 2074 616b 6573 206f 6e65  nsume` takes one
-0002d880: 206f 7074 696f 6e61 6c20 6172 6775 6d65   optional argume
-0002d890: 6e74 2c20 606b 6565 705f 6c61 7374 602c  nt, `keep_last`,
-0002d8a0: 2074 6861 7420 6465 6661 756c 7473 2074   that defaults t
-0002d8b0: 6f20 3020 616e 6420 7370 6563 6966 6965  o 0 and specifie
-0002d8c0: 7320 686f 7720 6d61 6e79 2c20 6966 2061  s how many, if a
-0002d8d0: 6e79 2c20 6974 656d 7320 6672 6f6d 2074  ny, items from t
-0002d8e0: 6865 2065 6e64 2074 6f20 7265 7475 726e  he end to return
-0002d8f0: 2061 7320 6120 7365 7175 656e 6365 2028   as a sequence (
-0002d900: 604e 6f6e 6560 2077 696c 6c20 6b65 6570  `None` will keep
-0002d910: 2061 6c6c 2065 6c65 6d65 6e74 7329 2e0a   all elements)..
-0002d920: 0a45 7175 6976 616c 656e 7420 746f 3a0a  .Equivalent to:.
-0002d930: 6060 6063 6f63 6f6e 7574 0a64 6566 2063  ```coconut.def c
-0002d940: 6f6e 7375 6d65 2869 7465 7261 626c 652c  onsume(iterable,
-0002d950: 206b 6565 705f 6c61 7374 3d30 293a 0a20   keep_last=0):. 
-0002d960: 2020 2022 2222 4675 6c6c 7920 6578 6861     """Fully exha
-0002d970: 7573 7420 6974 6572 6162 6c65 2061 6e64  ust iterable and
-0002d980: 2072 6574 7572 6e20 7468 6520 6c61 7374   return the last
-0002d990: 206b 6565 705f 6c61 7374 2065 6c65 6d65   keep_last eleme
-0002d9a0: 6e74 732e 2222 220a 2020 2020 7265 7475  nts.""".    retu
-0002d9b0: 726e 2063 6f6c 6c65 6374 696f 6e73 2e64  rn collections.d
-0002d9c0: 6571 7565 2869 7465 7261 626c 652c 206d  eque(iterable, m
-0002d9d0: 6178 6c65 6e3d 6b65 6570 5f6c 6173 7429  axlen=keep_last)
-0002d9e0: 2020 2320 6661 7374 6573 7420 7761 7920    # fastest way 
-0002d9f0: 746f 2065 7868 6175 7374 2061 6e20 6974  to exhaust an it
-0002da00: 6572 6174 6f72 0a60 6060 0a0a 2323 2323  erator.```..####
-0002da10: 2320 5261 7469 6f6e 616c 650a 0a49 6e20  # Rationale..In 
-0002da20: 7468 6520 7072 6f63 6573 7320 6f66 206c  the process of l
-0002da30: 617a 696c 7920 6170 706c 7969 6e67 206f  azily applying o
-0002da40: 7065 7261 7469 6f6e 7320 746f 2069 7465  perations to ite
-0002da50: 7261 746f 7273 2c20 6576 656e 7475 616c  rators, eventual
-0002da60: 6c79 2061 2070 6f69 6e74 2069 7320 7265  ly a point is re
-0002da70: 6163 6865 6420 7768 6572 6520 6576 616c  ached where eval
-0002da80: 7561 7469 6f6e 206f 6620 7468 6520 6974  uation of the it
-0002da90: 6572 6174 6f72 2069 7320 6e65 6365 7373  erator is necess
-0002daa0: 6172 792e 2054 6f20 646f 2074 6869 7320  ary. To do this 
-0002dab0: 6566 6669 6369 656e 746c 792c 2043 6f63  efficiently, Coc
-0002dac0: 6f6e 7574 2070 726f 7669 6465 7320 7468  onut provides th
-0002dad0: 6520 6063 6f6e 7375 6d65 6020 6675 6e63  e `consume` func
-0002dae0: 7469 6f6e 2c20 7768 6963 6820 7769 6c6c  tion, which will
-0002daf0: 2066 756c 6c79 2065 7868 6175 7374 2074   fully exhaust t
-0002db00: 6865 2069 7465 7261 746f 7220 6769 7665  he iterator give
-0002db10: 6e20 746f 2069 742e 0a0a 2323 2323 2320  n to it...##### 
-0002db20: 4578 616d 706c 650a 0a2a 2a43 6f63 6f6e  Example..**Cocon
-0002db30: 7574 3a2a 2a0a 6060 6063 6f63 6f6e 7574  ut:**.```coconut
-0002db40: 0a72 616e 6765 2831 3029 207c 3e20 6d61  .range(10) |> ma
-0002db50: 7024 2828 7829 202d 3e20 782a 2a32 2920  p$((x) -> x**2) 
-0002db60: 7c3e 206d 6170 2428 7072 696e 7429 207c  |> map$(print) |
-0002db70: 3e20 636f 6e73 756d 650a 6060 600a 0a2a  > consume.```..*
-0002db80: 2a50 7974 686f 6e3a 2a2a 0a60 6060 636f  *Python:**.```co
-0002db90: 636f 6e75 745f 7079 7468 6f6e 0a63 6f6c  conut_python.col
-0002dba0: 6c65 6374 696f 6e73 2e64 6571 7565 286d  lections.deque(m
-0002dbb0: 6170 2870 7269 6e74 2c20 6d61 7028 6c61  ap(print, map(la
-0002dbc0: 6d62 6461 2078 3a20 782a 2a32 2c20 7261  mbda x: x**2, ra
-0002dbd0: 6e67 6528 3130 2929 292c 206d 6178 6c65  nge(10))), maxle
-0002dbe0: 6e3d 3029 0a60 6060 0a0a 2323 2320 5479  n=0).```..### Ty
-0002dbf0: 7069 6e67 2d53 7065 6369 6669 6320 4275  ping-Specific Bu
-0002dc00: 696c 742d 496e 730a 0a60 6060 7b63 6f6e  ilt-Ins..```{con
-0002dc10: 7465 6e74 737d 0a2d 2d2d 0a6c 6f63 616c  tents}.---.local
-0002dc20: 3a0a 6465 7074 683a 2031 0a2d 2d2d 0a60  :.depth: 1.---.`
-0002dc30: 6060 0a0a 2323 2323 2060 5459 5045 5f43  ``..#### `TYPE_C
-0002dc40: 4845 434b 494e 4760 0a0a 5468 6520 6054  HECKING`..The `T
-0002dc50: 5950 455f 4348 4543 4b49 4e47 6020 7661  YPE_CHECKING` va
-0002dc60: 7269 6162 6c65 2069 7320 7365 7420 746f  riable is set to
-0002dc70: 2060 4661 6c73 6560 2061 7420 7275 6e74   `False` at runt
-0002dc80: 696d 6520 616e 6420 6054 7275 6560 2064  ime and `True` d
-0002dc90: 7572 696e 6720 7479 7065 5f63 6865 636b  uring type_check
-0002dca0: 696e 672c 2061 6c6c 6f77 696e 6720 796f  ing, allowing yo
-0002dcb0: 7520 746f 2070 7265 7665 6e74 2079 6f75  u to prevent you
-0002dcc0: 7220 6074 7970 696e 6760 2069 6d70 6f72  r `typing` impor
-0002dcd0: 7473 2061 6e64 2060 5479 7065 5661 7260  ts and `TypeVar`
-0002dce0: 2064 6566 696e 6974 696f 6e73 2066 726f   definitions fro
-0002dcf0: 6d20 6265 696e 6720 6578 6563 7574 6564  m being executed
-0002dd00: 2061 7420 7275 6e74 696d 652e 2042 7920   at runtime. By 
-0002dd10: 7772 6170 7069 6e67 2079 6f75 7220 6074  wrapping your `t
-0002dd20: 7970 696e 6760 2069 6d70 6f72 7473 2069  yping` imports i
-0002dd30: 6e20 616e 2060 6966 2054 5950 455f 4348  n an `if TYPE_CH
-0002dd40: 4543 4b49 4e47 3a60 2062 6c6f 636b 2c20  ECKING:` block, 
-0002dd50: 796f 7520 6361 6e20 6576 656e 2075 7365  you can even use
-0002dd60: 2074 6865 205b 6074 7970 696e 6760 5d28   the [`typing`](
-0002dd70: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
-0002dd80: 686f 6e2e 6f72 672f 332f 6c69 6272 6172  hon.org/3/librar
-0002dd90: 792f 7479 7069 6e67 2e68 746d 6c29 206d  y/typing.html) m
-0002dda0: 6f64 756c 6520 6f6e 2050 7974 686f 6e20  odule on Python 
-0002ddb0: 7665 7273 696f 6e73 2074 6861 7420 646f  versions that do
-0002ddc0: 6e27 7420 6e61 7469 7665 6c79 2073 7570  n't natively sup
-0002ddd0: 706f 7274 2069 742e 2046 7572 7468 6572  port it. Further
-0002dde0: 6d6f 7265 2c20 6054 5950 455f 4348 4543  more, `TYPE_CHEC
-0002ddf0: 4b49 4e47 6020 6361 6e20 616c 736f 2062  KING` can also b
-0002de00: 6520 7573 6564 2074 6f20 6869 6465 2063  e used to hide c
-0002de10: 6f64 6520 7468 6174 2069 7320 6d69 7374  ode that is mist
-0002de20: 7970 6564 2062 7920 6465 6661 756c 742e  yped by default.
-0002de30: 0a0a 2323 2323 2320 5079 7468 6f6e 2044  ..##### Python D
-0002de40: 6f63 730a 0a41 2073 7065 6369 616c 2063  ocs..A special c
-0002de50: 6f6e 7374 616e 7420 7468 6174 2069 7320  onstant that is 
-0002de60: 6173 7375 6d65 6420 746f 2062 6520 6054  assumed to be `T
-0002de70: 7275 6560 2062 7920 3372 6420 7061 7274  rue` by 3rd part
-0002de80: 7920 7374 6174 6963 2074 7970 6520 6368  y static type ch
-0002de90: 6563 6b65 7273 2e20 4974 2069 7320 6046  eckers. It is `F
-0002dea0: 616c 7365 6020 6174 2072 756e 7469 6d65  alse` at runtime
-0002deb0: 2e20 5573 6167 653a 0a60 6060 636f 636f  . Usage:.```coco
-0002dec0: 6e75 745f 7079 7468 6f6e 0a69 6620 5459  nut_python.if TY
-0002ded0: 5045 5f43 4845 434b 494e 473a 0a20 2020  PE_CHECKING:.   
-0002dee0: 2069 6d70 6f72 7420 6578 7065 6e73 6976   import expensiv
-0002def0: 655f 6d6f 640a 0a64 6566 2066 756e 2861  e_mod..def fun(a
-0002df00: 7267 3a20 6578 7065 6e73 6976 655f 6d6f  rg: expensive_mo
-0002df10: 642e 536f 6d65 5479 7065 2920 2d3e 204e  d.SomeType) -> N
-0002df20: 6f6e 653a 0a20 2020 206c 6f63 616c 5f76  one:.    local_v
-0002df30: 6172 3a20 6578 7065 6e73 6976 655f 6d6f  ar: expensive_mo
-0002df40: 642e 416e 6f74 6865 7254 7970 6520 3d20  d.AnotherType = 
-0002df50: 6f74 6865 725f 6675 6e28 290a 6060 600a  other_fun().```.
-0002df60: 0a23 2323 2323 2045 7861 6d70 6c65 730a  .##### Examples.
-0002df70: 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a 6060  .**Coconut:**.``
-0002df80: 6063 6f63 6f6e 7574 0a69 6620 5459 5045  `coconut.if TYPE
-0002df90: 5f43 4845 434b 494e 473a 0a20 2020 2066  _CHECKING:.    f
-0002dfa0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-0002dfb0: 7420 4c69 7374 0a78 3a20 4c69 7374 5b73  t List.x: List[s
-0002dfc0: 7472 5d20 3d20 5b22 6122 2c20 2262 225d  tr] = ["a", "b"]
-0002dfd0: 0a60 6060 0a0a 6060 6063 6f63 6f6e 7574  .```..```coconut
-0002dfe0: 0a69 6620 5459 5045 5f43 4845 434b 494e  .if TYPE_CHECKIN
-0002dff0: 473a 0a20 2020 2064 6566 2066 6163 746f  G:.    def facto
-0002e000: 7269 616c 286e 3a20 696e 7429 202d 3e20  rial(n: int) -> 
-0002e010: 696e 743a 202e 2e2e 0a65 6c73 653a 0a20  int: ....else:. 
-0002e020: 2020 2064 6566 2066 6163 746f 7269 616c     def factorial
-0002e030: 2830 2920 3d20 310a 2020 2020 6164 6470  (0) = 1.    addp
-0002e040: 6174 7465 726e 2064 6566 2066 6163 746f  attern def facto
-0002e050: 7269 616c 286e 2920 3d20 6e20 2a20 6661  rial(n) = n * fa
-0002e060: 6374 6f72 6961 6c28 6e2d 3129 0a60 6060  ctorial(n-1).```
-0002e070: 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a 6060  ..**Python:**.``
-0002e080: 6063 6f63 6f6e 7574 5f70 7974 686f 6e0a  `coconut_python.
-0002e090: 7472 793a 0a20 2020 2066 726f 6d20 7479  try:.    from ty
-0002e0a0: 7069 6e67 2069 6d70 6f72 7420 5459 5045  ping import TYPE
-0002e0b0: 5f43 4845 434b 494e 470a 6578 6365 7074  _CHECKING.except
-0002e0c0: 2049 6d70 6f72 7445 7272 6f72 3a0a 2020   ImportError:.  
-0002e0d0: 2020 5459 5045 5f43 4845 434b 494e 4720    TYPE_CHECKING 
-0002e0e0: 3d20 4661 6c73 650a 0a69 6620 5459 5045  = False..if TYPE
-0002e0f0: 5f43 4845 434b 494e 473a 0a20 2020 2066  _CHECKING:.    f
-0002e100: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-0002e110: 7420 4c69 7374 0a78 3a20 4c69 7374 5b73  t List.x: List[s
-0002e120: 7472 5d20 3d20 5b22 6122 2c20 2262 225d  tr] = ["a", "b"]
-0002e130: 0a60 6060 0a0a 6060 6063 6f63 6f6e 7574  .```..```coconut
-0002e140: 5f70 7974 686f 6e0a 7472 793a 0a20 2020  _python.try:.   
-0002e150: 2066 726f 6d20 7479 7069 6e67 2069 6d70   from typing imp
-0002e160: 6f72 7420 5459 5045 5f43 4845 434b 494e  ort TYPE_CHECKIN
-0002e170: 470a 6578 6365 7074 2049 6d70 6f72 7445  G.except ImportE
-0002e180: 7272 6f72 3a0a 2020 2020 5459 5045 5f43  rror:.    TYPE_C
-0002e190: 4845 434b 494e 4720 3d20 4661 6c73 650a  HECKING = False.
-0002e1a0: 0a69 6620 5459 5045 5f43 4845 434b 494e  .if TYPE_CHECKIN
-0002e1b0: 473a 0a20 2020 2064 6566 2066 6163 746f  G:.    def facto
-0002e1c0: 7269 616c 286e 3a20 696e 7429 202d 3e20  rial(n: int) -> 
-0002e1d0: 696e 743a 202e 2e2e 0a65 6c73 653a 0a20  int: ....else:. 
-0002e1e0: 2020 2064 6566 2066 6163 746f 7269 616c     def factorial
-0002e1f0: 286e 293a 0a20 2020 2020 2020 2069 6620  (n):.        if 
-0002e200: 6e20 3d3d 2030 3a0a 2020 2020 2020 2020  n == 0:.        
-0002e210: 2020 2020 7265 7475 726e 2031 0a20 2020      return 1.   
-0002e220: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0002e230: 2020 2020 2020 2072 6574 7572 6e20 6e20         return n 
-0002e240: 2a20 6661 6374 6f72 6961 6c28 6e2d 3129  * factorial(n-1)
-0002e250: 0a60 6060 0a0a 2323 2323 2060 7265 7665  .```..#### `reve
-0002e260: 616c 5f74 7970 6560 2061 6e64 2060 7265  al_type` and `re
-0002e270: 7665 616c 5f6c 6f63 616c 7360 0a0a 5768  veal_locals`..Wh
-0002e280: 656e 2075 7369 6e67 204d 7950 792c 2060  en using MyPy, `
-0002e290: 7265 7665 616c 5f74 7970 6528 3c65 7870  reveal_type(<exp
-0002e2a0: 723e 2960 2077 696c 6c20 6361 7573 6520  r>)` will cause 
-0002e2b0: 4d79 5079 2074 6f20 7072 696e 7420 7468  MyPy to print th
-0002e2c0: 6520 7479 7065 206f 6620 603c 6578 7072  e type of `<expr
-0002e2d0: 3e60 2061 6e64 2060 7265 7665 616c 5f6c  >` and `reveal_l
-0002e2e0: 6f63 616c 7328 2960 2077 696c 6c20 6361  ocals()` will ca
-0002e2f0: 7573 6520 4d79 5079 2074 6f20 7072 696e  use MyPy to prin
-0002e300: 7420 7468 6520 7479 7065 7320 6f66 2074  t the types of t
-0002e310: 6865 2063 7572 7265 6e74 2060 6c6f 6361  he current `loca
-0002e320: 6c73 2829 602e 2041 7420 7275 6e74 696d  ls()`. At runtim
-0002e330: 652c 2060 7265 7665 616c 5f74 7970 6528  e, `reveal_type(
-0002e340: 7829 6020 6973 2061 6c77 6179 7320 7468  x)` is always th
-0002e350: 6520 6964 656e 7469 7479 2066 756e 6374  e identity funct
-0002e360: 696f 6e20 616e 6420 6072 6576 6561 6c5f  ion and `reveal_
-0002e370: 6c6f 6361 6c73 2829 6020 616c 7761 7973  locals()` always
-0002e380: 2072 6574 7572 6e73 2060 4e6f 6e65 602e   returns `None`.
-0002e390: 2053 6565 205b 7468 6520 4d79 5079 2064   See [the MyPy d
-0002e3a0: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-0002e3b0: 7470 733a 2f2f 6d79 7079 2e72 6561 6474  tps://mypy.readt
-0002e3c0: 6865 646f 6373 2e69 6f2f 656e 2f73 7461  hedocs.io/en/sta
-0002e3d0: 626c 652f 636f 6d6d 6f6e 5f69 7373 7565  ble/common_issue
-0002e3e0: 732e 6874 6d6c 2372 6576 6561 6c2d 7479  s.html#reveal-ty
-0002e3f0: 7065 2920 666f 7220 6d6f 7265 2069 6e66  pe) for more inf
-0002e400: 6f72 6d61 7469 6f6e 2e0a 0a23 2323 2323  ormation...#####
-0002e410: 2045 7861 6d70 6c65 0a0a 2a2a 436f 636f   Example..**Coco
-0002e420: 6e75 743a 2a2a 0a60 6060 636f 636f 6e75  nut:**.```coconu
-0002e430: 745f 7079 636f 6e0a 3e20 636f 636f 6e75  t_pycon.> coconu
-0002e440: 7420 2d2d 6d79 7079 0a43 6f63 6f6e 7574  t --mypy.Coconut
-0002e450: 2049 6e74 6572 7072 6574 6572 2076 582e   Interpreter vX.
-0002e460: 582e 583a 0a28 656e 7465 7220 2765 7869  X.X:.(enter 'exi
-0002e470: 7428 2927 206f 7220 7072 6573 7320 4374  t()' or press Ct
-0002e480: 726c 2d44 2074 6f20 656e 6429 0a3e 3e3e  rl-D to end).>>>
-0002e490: 2072 6576 6561 6c5f 7479 7065 2866 6d61   reveal_type(fma
-0002e4a0: 7029 0a3c 6675 6e63 7469 6f6e 2066 6d61  p).<function fma
-0002e4b0: 7020 6174 2030 7830 3030 3030 3233 3942  p at 0x00000239B
-0002e4c0: 3036 4532 3034 303e 0a3c 7374 7269 6e67  06E2040>.<string
-0002e4d0: 3e3a 3137 3a20 6e6f 7465 3a20 5265 7665  >:17: note: Reve
-0002e4e0: 616c 6564 2074 7970 6520 6973 2027 6465  aled type is 'de
-0002e4f0: 6620 5b5f 542c 205f 555d 2028 6675 6e63  f [_T, _U] (func
-0002e500: 3a20 6465 6620 285f 5460 2d31 2920 2d3e  : def (_T`-1) ->
-0002e510: 205f 5560 2d32 2c20 6f62 6a3a 2074 7970   _U`-2, obj: typ
-0002e520: 696e 672e 4974 6572 6162 6c65 5b5f 5460  ing.Iterable[_T`
-0002e530: 2d31 5d29 202d 3e20 7479 7069 6e67 2e49  -1]) -> typing.I
-0002e540: 7465 7261 626c 655b 5f55 602d 325d 270a  terable[_U`-2]'.
-0002e550: 3e3e 3e0a 6060 600a 0a2a 2a50 7974 686f  >>>.```..**Pytho
-0002e560: 6e2a 2a0a 6060 6063 6f63 6f6e 7574 5f70  n**.```coconut_p
-0002e570: 7974 686f 6e0a 7472 793a 0a20 2020 2066  ython.try:.    f
-0002e580: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-0002e590: 7420 5459 5045 5f43 4845 434b 494e 470a  t TYPE_CHECKING.
-0002e5a0: 6578 6365 7074 2049 6d70 6f72 7445 7272  except ImportErr
-0002e5b0: 6f72 3a0a 2020 2020 5459 5045 5f43 4845  or:.    TYPE_CHE
-0002e5c0: 434b 494e 4720 3d20 4661 6c73 650a 0a69  CKING = False..i
-0002e5d0: 6620 6e6f 7420 5459 5045 5f43 4845 434b  f not TYPE_CHECK
-0002e5e0: 494e 473a 0a20 2020 2064 6566 2072 6576  ING:.    def rev
-0002e5f0: 6561 6c5f 7479 7065 2878 293a 0a20 2020  eal_type(x):.   
-0002e600: 2020 2020 2072 6574 7572 6e20 780a 0a66       return x..f
-0002e610: 726f 6d20 636f 636f 6e75 742e 5f5f 636f  rom coconut.__co
-0002e620: 636f 6e75 745f 5f20 696d 706f 7274 2066  conut__ import f
-0002e630: 6d61 700a 7265 7665 616c 5f74 7970 6528  map.reveal_type(
-0002e640: 666d 6170 290a 6060 600a 0a23 2320 436f  fmap).```..## Co
-0002e650: 636f 6e75 7420 4150 490a 0a60 6060 7b63  conut API..```{c
-0002e660: 6f6e 7465 6e74 737d 0a2d 2d2d 0a6c 6f63  ontents}.---.loc
-0002e670: 616c 3a0a 6465 7074 683a 2032 0a2d 2d2d  al:.depth: 2.---
-0002e680: 0a60 6060 0a0a 2323 2320 6063 6f63 6f6e  .```..### `cocon
-0002e690: 7574 2e65 6d62 6564 600a 0a2a 2a63 6f63  ut.embed`..**coc
-0002e6a0: 6f6e 7574 2e65 6d62 6564 2a2a 285f 6b65  onut.embed**(_ke
-0002e6b0: 726e 656c 5f3d 604e 6f6e 6560 2c20 5f64  rnel_=`None`, _d
-0002e6c0: 6570 7468 5f3d 6030 602c 205c 2a5c 2a5f  epth_=`0`, \*\*_
-0002e6d0: 6b77 6172 6773 5f29 0a0a 4966 205f 6b65  kwargs_)..If _ke
-0002e6e0: 726e 656c 5f3d 6046 616c 7365 6020 2864  rnel_=`False` (d
-0002e6f0: 6566 6175 6c74 292c 2065 6d62 6564 7320  efault), embeds 
-0002e700: 6120 436f 636f 6e75 7420 4a75 7079 7465  a Coconut Jupyte
-0002e710: 7220 636f 6e73 6f6c 6520 696e 6974 6961  r console initia
-0002e720: 6c69 7a65 6420 6672 6f6d 2074 6865 2063  lized from the c
-0002e730: 7572 7265 6e74 206c 6f63 616c 206e 616d  urrent local nam
-0002e740: 6573 7061 6365 2e20 4966 205f 6b65 726e  espace. If _kern
-0002e750: 656c 5f3d 6054 7275 6560 2c20 6c61 756e  el_=`True`, laun
-0002e760: 6368 6573 2061 2043 6f63 6f6e 7574 204a  ches a Coconut J
-0002e770: 7570 7974 6572 206b 6572 6e65 6c20 696e  upyter kernel in
-0002e780: 6974 6961 6c69 7a65 6420 6672 6f6d 2074  itialized from t
-0002e790: 6865 206c 6f63 616c 206e 616d 6573 7061  he local namespa
-0002e7a0: 6365 2074 6861 7420 6361 6e20 7468 656e  ce that can then
-0002e7b0: 2062 6520 6174 7461 6368 6564 2074 6f2e   be attached to.
-0002e7c0: 2054 6865 205f 6465 7074 685f 2069 6e64   The _depth_ ind
-0002e7d0: 6963 6174 6573 2068 6f77 206d 616e 7920  icates how many 
-0002e7e0: 6164 6469 7469 6f6e 616c 2063 616c 6c20  additional call 
-0002e7f0: 6672 616d 6573 2074 6f20 6967 6e6f 7265  frames to ignore
-0002e800: 2e20 5f6b 7761 7267 735f 2061 7265 2061  . _kwargs_ are a
-0002e810: 7320 696e 205b 4950 7974 686f 6e2e 656d  s in [IPython.em
-0002e820: 6265 645d 2868 7474 7073 3a2f 2f69 7079  bed](https://ipy
-0002e830: 7468 6f6e 2e72 6561 6474 6865 646f 6373  thon.readthedocs
-0002e840: 2e69 6f2f 656e 2f73 7461 626c 652f 6170  .io/en/stable/ap
-0002e850: 692f 6765 6e65 7261 7465 642f 4950 7974  i/generated/IPyt
-0002e860: 686f 6e2e 7465 726d 696e 616c 2e65 6d62  hon.terminal.emb
-0002e870: 6564 2e68 746d 6c23 4950 7974 686f 6e2e  ed.html#IPython.
-0002e880: 7465 726d 696e 616c 2e65 6d62 6564 2e65  terminal.embed.e
-0002e890: 6d62 6564 2920 6f72 205b 4950 7974 686f  mbed) or [IPytho
-0002e8a0: 6e2e 656d 6265 645f 6b65 726e 656c 5d28  n.embed_kernel](
-0002e8b0: 6874 7470 733a 2f2f 6970 7974 686f 6e2e  https://ipython.
-0002e8c0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-0002e8d0: 6e2f 7374 6162 6c65 2f61 7069 2f67 656e  n/stable/api/gen
-0002e8e0: 6572 6174 6564 2f49 5079 7468 6f6e 2e68  erated/IPython.h
-0002e8f0: 746d 6c23 4950 7974 686f 6e2e 656d 6265  tml#IPython.embe
-0002e900: 645f 6b65 726e 656c 2920 6261 7365 6420  d_kernel) based 
-0002e910: 6f6e 205f 6b65 726e 656c 5f2e 0a0a 5265  on _kernel_...Re
-0002e920: 636f 6d6d 656e 6465 6420 7573 6167 6520  commended usage 
-0002e930: 6973 2061 7320 6120 6465 6275 6767 696e  is as a debuggin
-0002e940: 6720 746f 6f6c 2c20 7768 6572 6520 7468  g tool, where th
-0002e950: 6520 636f 6465 2060 6672 6f6d 2063 6f63  e code `from coc
-0002e960: 6f6e 7574 2069 6d70 6f72 7420 656d 6265  onut import embe
-0002e970: 643b 2065 6d62 6564 2829 6020 6361 6e20  d; embed()` can 
-0002e980: 6265 2069 6e73 6572 7465 6420 746f 206c  be inserted to l
-0002e990: 6175 6e63 6820 616e 2069 6e74 6572 6163  aunch an interac
-0002e9a0: 7469 7665 2043 6f63 6f6e 7574 2073 6865  tive Coconut she
-0002e9b0: 6c6c 2069 6e69 7469 616c 697a 6564 2066  ll initialized f
-0002e9c0: 726f 6d20 7468 6174 2070 6f69 6e74 2e0a  rom that point..
-0002e9d0: 0a23 2323 2041 7574 6f6d 6174 6963 2043  .### Automatic C
-0002e9e0: 6f6d 7069 6c61 7469 6f6e 0a0a 4966 2079  ompilation..If y
-0002e9f0: 6f75 2064 6f6e 2774 2063 6172 6520 6162  ou don't care ab
-0002ea00: 6f75 7420 7468 6520 6578 6163 7420 636f  out the exact co
-0002ea10: 6d70 696c 6174 696f 6e20 7061 7261 6d65  mpilation parame
-0002ea20: 7465 7273 2079 6f75 2077 616e 7420 746f  ters you want to
-0002ea30: 2075 7365 2c20 6175 746f 6d61 7469 6320   use, automatic 
-0002ea40: 636f 6d70 696c 6174 696f 6e20 6c65 7473  compilation lets
-0002ea50: 2043 6f63 6f6e 7574 2074 616b 6520 6361   Coconut take ca
-0002ea60: 7265 206f 6620 6576 6572 7974 6869 6e67  re of everything
-0002ea70: 2066 6f72 2079 6f75 2e20 4175 746f 6d61   for you. Automa
-0002ea80: 7469 6320 636f 6d70 696c 6174 696f 6e20  tic compilation 
-0002ea90: 6361 6e20 6265 2065 6e61 626c 6564 2065  can be enabled e
-0002eaa0: 6974 6865 7220 6279 2069 6d70 6f72 7469  ither by importi
-0002eab0: 6e67 205b 6063 6f63 6f6e 7574 2e61 7069  ng [`coconut.api
-0002eac0: 605d 2823 636f 636f 6e75 742d 6170 6929  `](#coconut-api)
-0002ead0: 2062 6566 6f72 6520 796f 7520 696d 706f   before you impo
-0002eae0: 7274 2061 6e79 7468 696e 6720 656c 7365  rt anything else
-0002eaf0: 2c20 6f72 2062 7920 7275 6e6e 696e 6720  , or by running 
-0002eb00: 6063 6f63 6f6e 7574 202d 2d73 6974 652d  `coconut --site-
-0002eb10: 696e 7374 616c 6c60 2e20 4f6e 6365 2061  install`. Once a
-0002eb20: 7574 6f6d 6174 6963 2063 6f6d 7069 6c61  utomatic compila
-0002eb30: 7469 6f6e 2069 7320 656e 6162 6c65 642c  tion is enabled,
-0002eb40: 2043 6f63 6f6e 7574 2077 696c 6c20 6368   Coconut will ch
-0002eb50: 6563 6b20 6561 6368 206f 6620 796f 7572  eck each of your
-0002eb60: 2069 6d70 6f72 7473 2074 6f20 7365 6520   imports to see 
-0002eb70: 6966 2079 6f75 2061 7265 2061 7474 656d  if you are attem
-0002eb80: 7074 696e 6720 746f 2069 6d70 6f72 7420  pting to import 
-0002eb90: 6120 602e 636f 636f 6020 6669 6c65 2061  a `.coco` file a
-0002eba0: 6e64 2c20 6966 2073 6f2c 2061 7574 6f6d  nd, if so, autom
-0002ebb0: 6174 6963 616c 6c79 2063 6f6d 7069 6c65  atically compile
-0002ebc0: 2069 7420 666f 7220 796f 752e 204e 6f74   it for you. Not
-0002ebd0: 6520 7468 6174 2c20 666f 7220 436f 636f  e that, for Coco
-0002ebe0: 6e75 7420 746f 206b 6e6f 7720 7768 6174  nut to know what
-0002ebf0: 2066 696c 6520 796f 7520 6172 6520 7472   file you are tr
-0002ec00: 7969 6e67 2074 6f20 696d 706f 7274 2c20  ying to import, 
-0002ec10: 6974 2077 696c 6c20 6e65 6564 2074 6f20  it will need to 
-0002ec20: 6265 2061 6363 6573 7369 626c 6520 7669  be accessible vi
-0002ec30: 6120 6073 7973 2e70 6174 6860 2c20 6a75  a `sys.path`, ju
-0002ec40: 7374 206c 696b 6520 6120 6e6f 726d 616c  st like a normal
-0002ec50: 2069 6d70 6f72 742e 0a0a 4175 746f 6d61   import...Automa
-0002ec60: 7469 6320 636f 6d70 696c 6174 696f 6e20  tic compilation 
-0002ec70: 616c 7761 7973 2063 6f6d 7069 6c65 7320  always compiles 
-0002ec80: 6d6f 6475 6c65 7320 616e 6420 7061 636b  modules and pack
-0002ec90: 6167 6573 2069 6e2d 706c 6163 652c 2061  ages in-place, a
-0002eca0: 6e64 2061 6c77 6179 7320 7573 6573 2060  nd always uses `
-0002ecb0: 2d2d 7461 7267 6574 2073 7973 602e 2041  --target sys`. A
-0002ecc0: 7574 6f6d 6174 6963 2063 6f6d 7069 6c61  utomatic compila
-0002ecd0: 7469 6f6e 2069 7320 616c 7761 7973 2061  tion is always a
-0002ece0: 7661 696c 6162 6c65 2069 6e20 7468 6520  vailable in the 
-0002ecf0: 436f 636f 6e75 7420 696e 7465 7270 7265  Coconut interpre
-0002ed00: 7465 722c 2061 6e64 2c20 6966 2075 7369  ter, and, if usi
-0002ed10: 6e67 2074 6865 2043 6f63 6f6e 7574 2069  ng the Coconut i
-0002ed20: 6e74 6572 7072 6574 6572 2c20 6120 6072  nterpreter, a `r
-0002ed30: 656c 6f61 6460 2062 7569 6c74 2d69 6e20  eload` built-in 
-0002ed40: 6973 2070 726f 7669 6465 6420 746f 2065  is provided to e
-0002ed50: 6173 696c 7920 7265 6c6f 6164 2069 6d70  asily reload imp
-0002ed60: 6f72 7465 6420 6d6f 6475 6c65 732e 2041  orted modules. A
-0002ed70: 6464 6974 696f 6e61 6c6c 792c 2074 6865  dditionally, the
-0002ed80: 2069 6e74 6572 7072 6574 6572 2061 6c77   interpreter alw
-0002ed90: 6179 7320 616c 6c6f 7773 2069 6d70 6f72  ays allows impor
-0002eda0: 7469 6e67 2066 726f 6d20 7468 6520 6375  ting from the cu
-0002edb0: 7272 656e 7420 776f 726b 696e 6720 6469  rrent working di
-0002edc0: 7265 6374 6f72 792c 206c 6574 7469 6e67  rectory, letting
-0002edd0: 2079 6f75 2065 6173 696c 7920 636f 6d70   you easily comp
-0002ede0: 696c 6520 616e 6420 706c 6179 2061 726f  ile and play aro
-0002edf0: 756e 6420 7769 7468 2061 2060 2e63 6f63  und with a `.coc
-0002ee00: 6f60 2066 696c 6520 7369 6d70 6c79 2062  o` file simply b
-0002ee10: 7920 7275 6e6e 696e 6720 7468 6520 436f  y running the Co
-0002ee20: 636f 6e75 7420 696e 7465 7270 7265 7465  conut interprete
-0002ee30: 7220 616e 6420 696d 706f 7274 696e 6720  r and importing 
-0002ee40: 6974 2e0a 0a23 2323 2043 6f63 6f6e 7574  it...### Coconut
-0002ee50: 2045 6e63 6f64 696e 670a 0a57 6869 6c65   Encoding..While
-0002ee60: 2061 7574 6f6d 6174 6963 2063 6f6d 7069   automatic compi
-0002ee70: 6c61 7469 6f6e 2069 7320 7468 6520 7072  lation is the pr
-0002ee80: 6566 6572 7265 6420 6d65 7468 6f64 2066  eferred method f
-0002ee90: 6f72 2064 796e 616d 6963 616c 6c79 2063  or dynamically c
-0002eea0: 6f6d 7069 6c69 6e67 2043 6f63 6f6e 7574  ompiling Coconut
-0002eeb0: 2066 696c 6573 2c20 6173 2069 7420 6361   files, as it ca
-0002eec0: 6368 6573 2074 6865 2063 6f6d 7069 6c65  ches the compile
-0002eed0: 6420 636f 6465 2061 7320 6120 602e 7079  d code as a `.py
-0002eee0: 6020 6669 6c65 2074 6f20 7072 6576 656e  ` file to preven
-0002eef0: 7420 7265 636f 6d70 696c 6174 696f 6e2c  t recompilation,
-0002ef00: 2043 6f63 6f6e 7574 2061 6c73 6f20 7375   Coconut also su
-0002ef10: 7070 6f72 7473 2061 2073 7065 6369 616c  pports a special
-0002ef20: 0a60 6060 636f 636f 6e75 740a 2320 636f  .```coconut.# co
-0002ef30: 6469 6e67 3a20 636f 636f 6e75 740a 6060  ding: coconut.``
-0002ef40: 600a 6465 636c 6172 6174 696f 6e20 7768  `.declaration wh
-0002ef50: 6963 6820 6361 6e20 6265 2061 6464 6564  ich can be added
-0002ef60: 2074 6f20 602e 7079 6020 6669 6c65 7320   to `.py` files 
-0002ef70: 746f 2068 6176 6520 7468 656d 2074 7265  to have them tre
-0002ef80: 6174 6564 2061 7320 436f 636f 6e75 7420  ated as Coconut 
-0002ef90: 6669 6c65 7320 696e 7374 6561 642e 2054  files instead. T
-0002efa0: 6f20 7573 6520 7375 6368 2061 2063 6f64  o use such a cod
-0002efb0: 696e 6720 6465 636c 6172 6174 696f 6e2c  ing declaration,
-0002efc0: 2079 6f75 276c 6c20 6e65 6564 2074 6f20   you'll need to 
-0002efd0: 6569 7468 6572 2072 756e 2060 636f 636f  either run `coco
-0002efe0: 6e75 7420 2d2d 7369 7465 2d69 6e73 7461  nut --site-insta
-0002eff0: 6c6c 6020 6f72 2060 696d 706f 7274 2063  ll` or `import c
-0002f000: 6f63 6f6e 7574 2e61 7069 6020 6174 2073  oconut.api` at s
-0002f010: 6f6d 6520 706f 696e 7420 6265 666f 7265  ome point before
-0002f020: 2079 6f75 2066 6972 7374 2061 7474 656d   you first attem
-0002f030: 7074 2074 6f20 696d 706f 7274 2061 2066  pt to import a f
-0002f040: 696c 6520 7769 7468 2061 2060 2320 636f  ile with a `# co
-0002f050: 6469 6e67 3a20 636f 636f 6e75 7460 2064  ding: coconut` d
-0002f060: 6563 6c61 7261 7469 6f6e 2e20 4c69 6b65  eclaration. Like
-0002f070: 2061 7574 6f6d 6174 6963 2063 6f6d 7069   automatic compi
-0002f080: 6c61 7469 6f6e 2c20 636f 6d70 696c 6174  lation, compilat
-0002f090: 696f 6e20 6973 2061 6c77 6179 7320 646f  ion is always do
-0002f0a0: 6e65 2077 6974 6820 602d 2d74 6172 6765  ne with `--targe
-0002f0b0: 7420 7379 7360 2061 6e64 2069 7320 616c  t sys` and is al
-0002f0c0: 7761 7973 2061 7661 696c 6162 6c65 2066  ways available f
-0002f0d0: 726f 6d20 7468 6520 436f 636f 6e75 7420  rom the Coconut 
-0002f0e0: 696e 7465 7270 7265 7465 722e 0a0a 2323  interpreter...##
-0002f0f0: 2320 6063 6f63 6f6e 7574 2e61 7069 600a  # `coconut.api`.
-0002f100: 0a49 6e20 6164 6469 7469 6f6e 2074 6f20  .In addition to 
-0002f110: 656e 6162 6c69 6e67 2061 7574 6f6d 6174  enabling automat
-0002f120: 6963 2063 6f6d 7069 6c61 7469 6f6e 2c20  ic compilation, 
-0002f130: 6063 6f63 6f6e 7574 2e61 7069 6020 6361  `coconut.api` ca
-0002f140: 6e20 616c 736f 2062 6520 7573 6564 2074  n also be used t
-0002f150: 6f20 6361 6c6c 2074 6865 2043 6f63 6f6e  o call the Cocon
-0002f160: 7574 2063 6f6d 7069 6c65 7220 6672 6f6d  ut compiler from
-0002f170: 2063 6f64 6520 696e 7374 6561 6420 6f66   code instead of
-0002f180: 2066 726f 6d20 7468 6520 636f 6d6d 616e   from the comman
-0002f190: 6420 6c69 6e65 2e20 5365 6520 6265 6c6f  d line. See belo
-0002f1a0: 7720 666f 7220 7370 6563 6966 6963 6174  w for specificat
-0002f1b0: 696f 6e73 206f 6620 7468 6520 6469 6666  ions of the diff
-0002f1c0: 6572 656e 7420 6170 6920 6675 6e63 7469  erent api functi
-0002f1d0: 6f6e 732e 0a0a 5f44 4550 5245 4341 5445  ons..._DEPRECATE
-0002f1e0: 443a 2060 636f 636f 6e75 742e 636f 6e76  D: `coconut.conv
-0002f1f0: 656e 6965 6e63 6560 2069 7320 6120 6465  enience` is a de
-0002f200: 7072 6563 6174 6564 2061 6c69 6173 2066  precated alias f
-0002f210: 6f72 2060 636f 636f 6e75 742e 6170 6960  or `coconut.api`
-0002f220: 2e5f 0a0a 2323 2323 2060 6765 745f 7374  ._..#### `get_st
-0002f230: 6174 6560 0a0a 2a2a 636f 636f 6e75 742e  ate`..**coconut.
-0002f240: 6170 692e 6765 745c 5f73 7461 7465 2a2a  api.get\_state**
-0002f250: 285f 7374 6174 655f 3d60 4e6f 6e65 6029  (_state_=`None`)
-0002f260: 0a0a 4765 7473 2061 2073 7461 7465 206f  ..Gets a state o
-0002f270: 626a 6563 7420 7768 6963 6820 7374 6f72  bject which stor
-0002f280: 6573 2074 6865 2063 7572 7265 6e74 2063  es the current c
-0002f290: 6f6d 7069 6c61 7469 6f6e 2070 6172 616d  ompilation param
-0002f2a0: 6574 6572 732e 2053 7461 7465 206f 626a  eters. State obj
-0002f2b0: 6563 7473 2063 616e 2062 6520 636f 6e66  ects can be conf
-0002f2c0: 6967 7572 6564 2077 6974 6820 5b2a 2a73  igured with [**s
-0002f2d0: 6574 7570 2a2a 5d28 2373 6574 7570 2920  etup**](#setup) 
-0002f2e0: 6f72 205b 2a2a 636d 642a 2a5d 2823 636d  or [**cmd**](#cm
-0002f2f0: 6429 2061 6e64 2074 6865 6e20 7573 6564  d) and then used
-0002f300: 2069 6e20 5b2a 2a70 6172 7365 2a2a 5d28   in [**parse**](
-0002f310: 2370 6172 7365 2920 6f72 205b 2a2a 636f  #parse) or [**co
-0002f320: 636f 6e75 745c 5f65 7661 6c2a 2a5d 2823  conut\_eval**](#
-0002f330: 636f 636f 6e75 745f 6576 616c 292e 0a0a  coconut_eval)...
-0002f340: 4966 205f 7374 6174 655f 2069 7320 604e  If _state_ is `N
-0002f350: 6f6e 6560 2c20 6765 7473 2061 206e 6577  one`, gets a new
-0002f360: 2073 7461 7465 206f 626a 6563 742c 2077   state object, w
-0002f370: 6865 7265 6173 2069 6620 5f73 7461 7465  hereas if _state
-0002f380: 5f20 6973 2060 4661 6c73 6560 2c20 7468  _ is `False`, th
-0002f390: 6520 676c 6f62 616c 2073 7461 7465 206f  e global state o
-0002f3a0: 626a 6563 7420 6973 2072 6574 7572 6e65  bject is returne
-0002f3b0: 642e 0a0a 2323 2323 2060 7061 7273 6560  d...#### `parse`
-0002f3c0: 0a0a 2a2a 636f 636f 6e75 742e 6170 692e  ..**coconut.api.
-0002f3d0: 7061 7273 652a 2a28 5f63 6f64 655f 3d60  parse**(_code_=`
-0002f3e0: 2222 602c 205f 6d6f 6465 5f3d 6022 7379  ""`, _mode_=`"sy
-0002f3f0: 7322 602c 205f 7374 6174 655f 3d60 4661  s"`, _state_=`Fa
-0002f400: 6c73 6560 2c20 5f6b 6565 705c 5f69 6e74  lse`, _keep\_int
-0002f410: 6572 6e61 6c5c 5f73 7461 7465 5f3d 604e  ernal\_state_=`N
-0002f420: 6f6e 6560 290a 0a4c 696b 656c 7920 7468  one`)..Likely th
-0002f430: 6520 6d6f 7374 2075 7365 6675 6c20 6f66  e most useful of
-0002f440: 2074 6865 2061 7069 2066 756e 6374 696f   the api functio
-0002f450: 6e73 2c20 6070 6172 7365 6020 7461 6b65  ns, `parse` take
-0002f460: 7320 436f 636f 6e75 7420 636f 6465 2061  s Coconut code a
-0002f470: 7320 696e 7075 7420 616e 6420 6f75 7470  s input and outp
-0002f480: 7574 7320 7468 6520 6571 7569 7661 6c65  uts the equivale
-0002f490: 6e74 2063 6f6d 7069 6c65 6420 5079 7468  nt compiled Pyth
-0002f4a0: 6f6e 2063 6f64 652e 205f 6d6f 6465 5f20  on code. _mode_ 
-0002f4b0: 6973 2075 7365 6420 746f 2069 6e64 6963  is used to indic
-0002f4c0: 6174 6520 7468 6520 636f 6e74 6578 7420  ate the context 
-0002f4d0: 666f 7220 7468 6520 7061 7273 696e 6720  for the parsing 
-0002f4e0: 616e 6420 5f73 7461 7465 5f20 6973 2074  and _state_ is t
-0002f4f0: 6865 2073 7461 7465 206f 626a 6563 7420  he state object 
-0002f500: 7374 6f72 696e 6720 7468 6520 636f 6d70  storing the comp
-0002f510: 696c 6174 696f 6e20 7061 7261 6d65 7465  ilation paramete
-0002f520: 7273 2074 6f20 7573 6520 6173 206f 6274  rs to use as obt
-0002f530: 6169 6e65 6420 6672 6f6d 205b 2a2a 6765  ained from [**ge
-0002f540: 745f 7374 6174 652a 2a5d 2823 6765 745f  t_state**](#get_
-0002f550: 7374 6174 6529 2028 6966 2060 4661 6c73  state) (if `Fals
-0002f560: 6560 2c20 7573 6573 2074 6865 2067 6c6f  e`, uses the glo
-0002f570: 6261 6c20 7374 6174 6520 6f62 6a65 6374  bal state object
-0002f580: 292e 205f 6b65 6570 5c5f 696e 7465 726e  ). _keep\_intern
-0002f590: 616c 5c5f 7374 6174 655f 2064 6574 6572  al\_state_ deter
-0002f5a0: 6d69 6e65 7320 7768 6574 6865 7220 7468  mines whether th
-0002f5b0: 6520 7374 6174 6520 6f62 6a65 6374 2077  e state object w
-0002f5c0: 696c 6c20 6b65 6570 2069 6e74 6572 6e61  ill keep interna
-0002f5d0: 6c20 7374 6174 6520 2873 7563 6820 6173  l state (such as
-0002f5e0: 2077 6861 7420 5b63 7573 746f 6d20 6f70   what [custom op
-0002f5f0: 6572 6174 6f72 735d 2823 6375 7374 6f6d  erators](#custom
-0002f600: 2d6f 7065 7261 746f 7273 2920 6861 7665  -operators) have
-0002f610: 2062 6565 6e20 6465 636c 6172 6564 29e2   been declared).
-0002f620: 8094 6966 2060 4e6f 6e65 602c 2069 6e74  ..if `None`, int
-0002f630: 6572 6e61 6c20 7374 6174 6520 7769 6c6c  ernal state will
-0002f640: 2062 6520 6b65 7074 2069 6666 2079 6f75   be kept iff you
-0002f650: 2061 7265 206e 6f74 2075 7369 6e67 2074   are not using t
-0002f660: 6865 2067 6c6f 6261 6c20 5f73 7461 7465  he global _state
-0002f670: 5f2e 0a0a 4966 205f 636f 6465 5f20 6973  _...If _code_ is
-0002f680: 206e 6f74 2070 6173 7365 642c 2060 7061   not passed, `pa
-0002f690: 7273 6560 2077 696c 6c20 6f75 7470 7574  rse` will output
-0002f6a0: 206a 7573 7420 7468 6520 6769 7665 6e20   just the given 
-0002f6b0: 5f6d 6f64 655f 2773 2068 6561 6465 722c  _mode_'s header,
-0002f6c0: 2077 6869 6368 2063 616e 2062 6520 6578   which can be ex
-0002f6d0: 6563 7574 6564 2074 6f20 7365 7420 7570  ecuted to set up
-0002f6e0: 2061 6e20 6578 6563 7574 696f 6e20 656e   an execution en
-0002f6f0: 7669 726f 6e6d 656e 7420 696e 2077 6869  vironment in whi
-0002f700: 6368 2066 7574 7572 6520 636f 6465 2063  ch future code c
-0002f710: 616e 2062 6520 7061 7273 6564 2061 6e64  an be parsed and
-0002f720: 2065 7865 6375 7465 6420 7769 7468 6f75   executed withou
-0002f730: 7420 6120 6865 6164 6572 2e0a 0a45 6163  t a header...Eac
-0002f740: 6820 5f6d 6f64 655f 2068 6173 2074 776f  h _mode_ has two
-0002f750: 2063 6f6d 706f 6e65 6e74 733a 2077 6861   components: wha
-0002f760: 7420 7061 7273 6572 2069 7420 7573 6573  t parser it uses
-0002f770: 2c20 616e 6420 7768 6174 2068 6561 6465  , and what heade
-0002f780: 7220 6974 2070 7265 7065 6e64 732e 2054  r it prepends. T
-0002f790: 6865 2070 6172 7365 7220 6465 7465 726d  he parser determ
-0002f7a0: 696e 6573 2077 6861 7420 436f 636f 6e75  ines what Coconu
-0002f7b0: 7420 636f 6465 2069 7320 616c 6c6f 7765  t code is allowe
-0002f7c0: 6420 6173 2069 6e70 7574 2c20 616e 6420  d as input, and 
-0002f7d0: 7468 6520 6865 6164 6572 2064 6574 6572  the header deter
-0002f7e0: 6d69 6e65 7320 686f 7720 7468 6520 636f  mines how the co
-0002f7f0: 6d70 696c 6564 2050 7974 686f 6e20 6361  mpiled Python ca
-0002f800: 6e20 6265 2075 7365 642e 2050 6f73 7369  n be used. Possi
-0002f810: 626c 6520 7661 6c75 6573 206f 6620 5f6d  ble values of _m
-0002f820: 6f64 655f 2061 7265 3a0a 0a2d 2060 2273  ode_ are:..- `"s
-0002f830: 7973 2260 3a20 2874 6865 2064 6566 6175  ys"`: (the defau
-0002f840: 6c74 290a 2020 2020 2b20 7061 7273 6572  lt).    + parser
-0002f850: 3a20 6669 6c65 0a20 2020 2020 2020 202a  : file.        *
-0002f860: 2054 6865 2066 696c 6520 7061 7273 6572   The file parser
-0002f870: 2063 616e 2070 6172 7365 2061 6e79 2043   can parse any C
-0002f880: 6f63 6f6e 7574 2063 6f64 652e 0a20 2020  oconut code..   
-0002f890: 202b 2068 6561 6465 723a 2073 7973 0a20   + header: sys. 
-0002f8a0: 2020 2020 2020 202a 2054 6869 7320 6865         * This he
-0002f8b0: 6164 6572 2069 6d70 6f72 7473 205b 6063  ader imports [`c
-0002f8c0: 6f63 6f6e 7574 2e5f 5f63 6f63 6f6e 7574  oconut.__coconut
-0002f8d0: 5f5f 605d 2823 636f 636f 6e75 742d 636f  __`](#coconut-co
-0002f8e0: 636f 6e75 7429 2074 6f20 6163 6365 7373  conut) to access
-0002f8f0: 2074 6865 206e 6563 6573 7361 7279 2043   the necessary C
-0002f900: 6f63 6f6e 7574 206f 626a 6563 7473 2e0a  oconut objects..
-0002f910: 2d20 6022 6578 6563 2260 3a0a 2020 2020  - `"exec"`:.    
-0002f920: 2b20 7061 7273 6572 3a20 6669 6c65 0a20  + parser: file. 
-0002f930: 2020 202b 2068 6561 6465 723a 2065 7865     + header: exe
-0002f940: 630a 2020 2020 2020 2020 2a20 5768 656e  c.        * When
-0002f950: 2070 6173 7365 6420 746f 2060 6578 6563   passed to `exec
-0002f960: 6020 6174 2074 6865 2067 6c6f 6261 6c20  ` at the global 
-0002f970: 6c65 7665 6c2c 2074 6869 7320 6865 6164  level, this head
-0002f980: 6572 2077 696c 6c20 6372 6561 7465 2061  er will create a
-0002f990: 6c6c 2074 6865 206e 6563 6573 7361 7279  ll the necessary
-0002f9a0: 2043 6f63 6f6e 7574 206f 626a 6563 7473   Coconut objects
-0002f9b0: 2069 7473 656c 6620 696e 7374 6561 6420   itself instead 
-0002f9c0: 6f66 2069 6d70 6f72 7469 6e67 2074 6865  of importing the
-0002f9d0: 6d2e 0a2d 2060 2266 696c 6522 603a 0a20  m..- `"file"`:. 
-0002f9e0: 2020 202b 2070 6172 7365 723a 2066 696c     + parser: fil
-0002f9f0: 650a 2020 2020 2b20 6865 6164 6572 3a20  e.    + header: 
-0002fa00: 6669 6c65 0a20 2020 2020 2020 202a 2054  file.        * T
-0002fa10: 6869 7320 6865 6164 6572 2069 7320 6d65  his header is me
-0002fa20: 616e 7420 746f 2062 6520 7772 6974 7465  ant to be writte
-0002fa30: 6e20 746f 2061 2060 2d2d 7374 616e 6461  n to a `--standa
-0002fa40: 6c6f 6e65 6020 6669 6c65 2061 6e64 2073  lone` file and s
-0002fa50: 686f 756c 6420 6e6f 7420 6265 2070 6173  hould not be pas
-0002fa60: 7365 6420 746f 2060 6578 6563 602e 0a2d  sed to `exec`..-
-0002fa70: 2060 2270 6163 6b61 6765 2260 3a0a 2020   `"package"`:.  
-0002fa80: 2020 2b20 7061 7273 6572 3a20 6669 6c65    + parser: file
-0002fa90: 0a20 2020 202b 2068 6561 6465 723a 2070  .    + header: p
-0002faa0: 6163 6b61 6765 0a20 2020 2020 2020 202a  ackage.        *
-0002fab0: 2054 6869 7320 6865 6164 6572 2069 7320   This header is 
-0002fac0: 6d65 616e 7420 746f 2062 6520 7772 6974  meant to be writ
-0002fad0: 7465 6e20 746f 2061 2060 2d2d 7061 636b  ten to a `--pack
-0002fae0: 6167 6560 2066 696c 6520 616e 6420 7368  age` file and sh
-0002faf0: 6f75 6c64 206e 6f74 2062 6520 7061 7373  ould not be pass
-0002fb00: 6564 2074 6f20 6065 7865 6360 2e0a 2d20  ed to `exec`..- 
-0002fb10: 6022 626c 6f63 6b22 603a 0a20 2020 202b  `"block"`:.    +
-0002fb20: 2070 6172 7365 723a 2066 696c 650a 2020   parser: file.  
-0002fb30: 2020 2b20 6865 6164 6572 3a20 6e6f 6e65    + header: none
-0002fb40: 0a20 2020 2020 2020 202a 204e 6f20 6865  .        * No he
-0002fb50: 6164 6572 2069 7320 696e 636c 7564 6564  ader is included
-0002fb60: 2c20 7468 7573 2074 6869 7320 6361 6e20  , thus this can 
-0002fb70: 6f6e 6c79 2062 6520 7061 7373 6564 2074  only be passed t
-0002fb80: 6f20 6065 7865 6360 2069 6620 636f 6465  o `exec` if code
-0002fb90: 2077 6974 6820 6120 6865 6164 6572 2068   with a header h
-0002fba0: 6173 2061 6c72 6561 6479 2062 6565 6e20  as already been 
-0002fbb0: 6578 6563 7574 6564 2061 7420 7468 6520  executed at the 
-0002fbc0: 676c 6f62 616c 206c 6576 656c 2e0a 2d20  global level..- 
-0002fbd0: 6022 7369 6e67 6c65 2260 3a0a 2020 2020  `"single"`:.    
-0002fbe0: 2b20 7061 7273 6572 3a20 7369 6e67 6c65  + parser: single
-0002fbf0: 0a20 2020 2020 2020 202a 2043 616e 206f  .        * Can o
-0002fc00: 6e6c 7920 7061 7273 6520 6f6e 6520 6c69  nly parse one li
-0002fc10: 6e65 206f 6620 436f 636f 6e75 7420 636f  ne of Coconut co
-0002fc20: 6465 2e0a 2020 2020 2b20 6865 6164 6572  de..    + header
-0002fc30: 3a20 6e6f 6e65 0a2d 2060 2265 7661 6c22  : none.- `"eval"
-0002fc40: 603a 0a20 2020 202b 2070 6172 7365 723a  `:.    + parser:
-0002fc50: 2065 7661 6c0a 2020 2020 2020 2020 2a20   eval.        * 
-0002fc60: 4361 6e20 6f6e 6c79 2070 6172 7365 2061  Can only parse a
-0002fc70: 2043 6f63 6f6e 7574 2065 7870 7265 7373   Coconut express
-0002fc80: 696f 6e2c 206e 6f74 2061 2073 7461 7465  ion, not a state
-0002fc90: 6d65 6e74 2e0a 2020 2020 2b20 6865 6164  ment..    + head
-0002fca0: 6572 3a20 6e6f 6e65 0a2d 2060 226c 656e  er: none.- `"len
-0002fcb0: 6965 6e74 2260 3a0a 2020 2020 2b20 7061  ient"`:.    + pa
-0002fcc0: 7273 6572 3a20 6c65 6e69 656e 740a 2020  rser: lenient.  
-0002fcd0: 2020 2020 2020 2a20 4361 6e20 7061 7273        * Can pars
-0002fce0: 6520 616e 7920 436f 636f 6e75 7420 636f  e any Coconut co
-0002fcf0: 6465 2c20 616c 6c6f 7773 206c 6561 6469  de, allows leadi
-0002fd00: 6e67 2077 6869 7465 7370 6163 652c 2061  ng whitespace, a
-0002fd10: 6e64 2068 6173 206e 6f20 7472 6169 6c69  nd has no traili
-0002fd20: 6e67 206e 6577 6c69 6e65 2e0a 2020 2020  ng newline..    
-0002fd30: 2b20 6865 6164 6572 3a20 6e6f 6e65 0a2d  + header: none.-
-0002fd40: 2060 2278 6f6e 7368 2260 3a0a 2020 2020   `"xonsh"`:.    
-0002fd50: 2b20 7061 7273 6572 3a20 786f 6e73 680a  + parser: xonsh.
-0002fd60: 2020 2020 2020 2020 2a20 5061 7273 6573          * Parses
-0002fd70: 2043 6f63 6f6e 7574 205b 6078 6f6e 7368   Coconut [`xonsh
-0002fd80: 605d 2868 7474 7073 3a2f 2f78 6f6e 2e73  `](https://xon.s
-0002fd90: 6829 2063 6f64 6520 666f 7220 7573 6520  h) code for use 
-0002fda0: 696e 205b 436f 636f 6e75 7427 7320 6078  in [Coconut's `x
-0002fdb0: 6f6e 7368 6020 7375 7070 6f72 745d 2823  onsh` support](#
-0002fdc0: 786f 6e73 682d 7375 7070 6f72 7429 2e0a  xonsh-support)..
+00019b20: 6974 2028 6620 7829 602e 0a0a 5f4e 6f74  it (f x)`..._Not
+00019b30: 653a 2069 6d70 6c69 6369 7420 6675 6e63  e: implicit func
+00019b40: 7469 6f6e 2061 7070 6c69 6361 7469 6f6e  tion application
+00019b50: 2061 6e64 2063 6f65 6666 6963 6965 6e74   and coefficient
+00019b60: 2073 796e 7461 7820 6973 2064 6973 6162   syntax is disab
+00019b70: 6c65 6420 7768 656e 205b 7573 696e 6720  led when [using 
+00019b80: 436f 636f 6e75 7420 696e 2060 786f 6e73  Coconut in `xons
+00019b90: 6860 5d28 2378 6f6e 7368 2d73 7570 706f  h`](#xonsh-suppo
+00019ba0: 7274 2920 6475 6520 746f 2063 6f6e 666c  rt) due to confl
+00019bb0: 6963 7469 6e67 2077 6974 6820 636f 6e73  icting with cons
+00019bc0: 6f6c 6520 636f 6d6d 616e 6473 2e5f 0a0a  ole commands._..
+00019bd0: 2323 2323 2320 4578 616d 706c 6573 0a0a  ##### Examples..
+00019be0: 2a2a 436f 636f 6e75 743a 2a2a 0a60 6060  **Coconut:**.```
+00019bf0: 636f 636f 6e75 740a 6465 6620 6628 782c  coconut.def f(x,
+00019c00: 2079 2920 3d20 2878 2c20 7929 0a70 7269   y) = (x, y).pri
+00019c10: 6e74 2866 2035 2031 3029 0a60 6060 0a0a  nt(f 5 10).```..
+00019c20: 6060 6063 6f63 6f6e 7574 0a64 6566 2070  ```coconut.def p
+00019c30: 3128 7829 203d 2078 202b 2031 0a70 7269  1(x) = x + 1.pri
+00019c40: 6e74 203c 7c20 7031 2035 0a60 6060 0a0a  nt <| p1 5.```..
+00019c50: 6060 6063 6f63 6f6e 7574 0a71 7561 6420  ```coconut.quad 
+00019c60: 3d20 3520 782a 2a32 202b 2033 2078 202b  = 5 x**2 + 3 x +
+00019c70: 2031 0a60 6060 0a0a 2a2a 5079 7468 6f6e   1.```..**Python
+00019c80: 3a2a 2a0a 6060 6063 6f63 6f6e 7574 5f70  :**.```coconut_p
+00019c90: 7974 686f 6e0a 6465 6620 6628 782c 2079  ython.def f(x, y
+00019ca0: 293a 2072 6574 7572 6e20 2878 2c20 7929  ): return (x, y)
+00019cb0: 0a70 7269 6e74 2866 2831 3030 2c20 352b  .print(f(100, 5+
+00019cc0: 3629 290a 6060 600a 0a60 6060 636f 636f  6)).```..```coco
+00019cd0: 6e75 745f 7079 7468 6f6e 0a64 6566 2070  nut_python.def p
+00019ce0: 3128 7829 3a20 7265 7475 726e 2078 202b  1(x): return x +
+00019cf0: 2031 0a70 7269 6e74 2870 3128 3529 290a   1.print(p1(5)).
+00019d00: 6060 600a 0a60 6060 636f 636f 6e75 745f  ```..```coconut_
+00019d10: 7079 7468 6f6e 0a71 7561 6420 3d20 3520  python.quad = 5 
+00019d20: 2a20 782a 2a32 202b 2033 202a 2078 202b  * x**2 + 3 * x +
+00019d30: 2031 0a60 6060 0a0a 2323 2320 4b65 7977   1.```..### Keyw
+00019d40: 6f72 6420 4172 6775 6d65 6e74 204e 616d  ord Argument Nam
+00019d50: 6520 456c 6973 696f 6e0a 0a57 6865 6e20  e Elision..When 
+00019d60: 7061 7373 696e 6720 696e 206c 6f6e 6720  passing in long 
+00019d70: 7661 7269 6162 6c65 206e 616d 6573 2061  variable names a
+00019d80: 7320 6b65 7977 6f72 6420 6172 6775 6d65  s keyword argume
+00019d90: 6e74 7320 6f66 2074 6865 2073 616d 6520  nts of the same 
+00019da0: 6e61 6d65 2c20 436f 636f 6e75 7420 7375  name, Coconut su
+00019db0: 7070 6f72 7473 2074 6865 2073 796e 7461  pports the synta
+00019dc0: 780a 6060 600a 6628 2e2e 2e3d 6c6f 6e67  x.```.f(...=long
+00019dd0: 5f76 6172 6961 626c 655f 6e61 6d65 290a  _variable_name).
+00019de0: 6060 600a 6173 2061 2073 686f 7274 6861  ```.as a shortha
+00019df0: 6e64 2066 6f72 0a60 6060 0a66 286c 6f6e  nd for.```.f(lon
+00019e00: 675f 7661 7269 6162 6c65 5f6e 616d 653d  g_variable_name=
+00019e10: 6c6f 6e67 5f76 6172 6961 626c 655f 6e61  long_variable_na
+00019e20: 6d65 290a 6060 600a 0a53 7563 6820 7379  me).```..Such sy
+00019e30: 6e74 6178 2069 7320 616c 736f 2073 7570  ntax is also sup
+00019e40: 706f 7274 6564 2069 6e20 5b70 6172 7469  ported in [parti
+00019e50: 616c 2061 7070 6c69 6361 7469 6f6e 5d28  al application](
+00019e60: 2370 6172 7469 616c 2d61 7070 6c69 6361  #partial-applica
+00019e70: 7469 6f6e 2920 616e 6420 5b61 6e6f 6e79  tion) and [anony
+00019e80: 6d6f 7573 2060 6e61 6d65 6474 7570 6c65  mous `namedtuple
+00019e90: 6073 5d28 2361 6e6f 6e79 6d6f 7573 2d6e  `s](#anonymous-n
+00019ea0: 616d 6564 7475 706c 6573 292e 0a0a 2323  amedtuples)...##
+00019eb0: 2323 2320 4578 616d 706c 650a 0a2a 2a43  ### Example..**C
+00019ec0: 6f63 6f6e 7574 3a2a 2a0a 6060 6063 6f63  oconut:**.```coc
+00019ed0: 6f6e 7574 0a72 6561 6c6c 795f 6c6f 6e67  onut.really_long
+00019ee0: 5f76 6172 6961 626c 655f 6e61 6d65 5f31  _variable_name_1
+00019ef0: 203d 2067 6574 5f31 2829 0a72 6561 6c6c   = get_1().reall
+00019f00: 795f 6c6f 6e67 5f76 6172 6961 626c 655f  y_long_variable_
+00019f10: 6e61 6d65 5f32 203d 2067 6574 5f32 2829  name_2 = get_2()
+00019f20: 0a6d 6169 6e5f 6675 6e63 280a 2020 2020  .main_func(.    
+00019f30: 2e2e 2e3d 7265 616c 6c79 5f6c 6f6e 675f  ...=really_long_
+00019f40: 7661 7269 6162 6c65 5f6e 616d 655f 312c  variable_name_1,
+00019f50: 0a20 2020 202e 2e2e 3d72 6561 6c6c 795f  .    ...=really_
+00019f60: 6c6f 6e67 5f76 6172 6961 626c 655f 6e61  long_variable_na
+00019f70: 6d65 5f32 2c0a 290a 6060 600a 0a2a 2a50  me_2,.).```..**P
+00019f80: 7974 686f 6e3a 2a2a 0a60 6060 636f 636f  ython:**.```coco
+00019f90: 6e75 745f 7079 7468 6f6e 0a72 6561 6c6c  nut_python.reall
+00019fa0: 795f 6c6f 6e67 5f76 6172 6961 626c 655f  y_long_variable_
+00019fb0: 6e61 6d65 5f31 203d 2067 6574 5f31 2829  name_1 = get_1()
+00019fc0: 0a72 6561 6c6c 795f 6c6f 6e67 5f76 6172  .really_long_var
+00019fd0: 6961 626c 655f 6e61 6d65 5f32 203d 2067  iable_name_2 = g
+00019fe0: 6574 5f32 2829 0a6d 6169 6e5f 6675 6e63  et_2().main_func
+00019ff0: 280a 2020 2020 7265 616c 6c79 5f6c 6f6e  (.    really_lon
+0001a000: 675f 7661 7269 6162 6c65 5f6e 616d 655f  g_variable_name_
+0001a010: 313d 7265 616c 6c79 5f6c 6f6e 675f 7661  1=really_long_va
+0001a020: 7269 6162 6c65 5f6e 616d 655f 312c 0a20  riable_name_1,. 
+0001a030: 2020 2072 6561 6c6c 795f 6c6f 6e67 5f76     really_long_v
+0001a040: 6172 6961 626c 655f 6e61 6d65 5f32 3d72  ariable_name_2=r
+0001a050: 6561 6c6c 795f 6c6f 6e67 5f76 6172 6961  eally_long_varia
+0001a060: 626c 655f 6e61 6d65 5f32 2c0a 290a 6060  ble_name_2,.).``
+0001a070: 600a 0a23 2323 2041 6e6f 6e79 6d6f 7573  `..### Anonymous
+0001a080: 204e 616d 6564 7475 706c 6573 0a0a 436f   Namedtuples..Co
+0001a090: 636f 6e75 7420 7375 7070 6f72 7473 2061  conut supports a
+0001a0a0: 6e6f 6e79 6d6f 7573 205b 606e 616d 6564  nonymous [`named
+0001a0b0: 7475 706c 6560 5d28 6874 7470 733a 2f2f  tuple`](https://
+0001a0c0: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
+0001a0d0: 332f 6c69 6272 6172 792f 636f 6c6c 6563  3/library/collec
+0001a0e0: 7469 6f6e 732e 6874 6d6c 2363 6f6c 6c65  tions.html#colle
+0001a0f0: 6374 696f 6e73 2e6e 616d 6564 7475 706c  ctions.namedtupl
+0001a100: 6529 206c 6974 6572 616c 732c 2073 7563  e) literals, suc
+0001a110: 6820 7468 6174 2060 2861 3d31 2c20 623d  h that `(a=1, b=
+0001a120: 3229 6020 6361 6e20 6265 2075 7365 6420  2)` can be used 
+0001a130: 6a75 7374 2061 7320 6028 312c 2032 2960  just as `(1, 2)`
+0001a140: 2c20 6275 7420 7769 7468 2061 6464 6564  , but with added
+0001a150: 206e 616d 6573 2e20 416e 6f6e 796d 6f75   names. Anonymou
+0001a160: 7320 606e 616d 6564 7475 706c 6560 7320  s `namedtuple`s 
+0001a170: 6172 6520 616c 7761 7973 2070 6963 6b6c  are always pickl
+0001a180: 6561 626c 652e 0a0a 5468 6520 7379 6e74  eable...The synt
+0001a190: 6178 2066 6f72 2061 6e6f 6e79 6d6f 7573  ax for anonymous
+0001a1a0: 206e 616d 6564 7475 706c 6520 6c69 7465   namedtuple lite
+0001a1b0: 7261 6c73 2069 733a 0a60 6060 636f 636f  rals is:.```coco
+0001a1c0: 6e75 740a 283c 6e61 6d65 3e20 5b3a 203c  nut.(<name> [: <
+0001a1d0: 7479 7065 3e5d 203d 203c 7661 6c75 653e  type>] = <value>
+0001a1e0: 2c20 2e2e 2e29 0a60 6060 0a77 6865 7265  , ...).```.where
+0001a1f0: 2c20 6966 2060 3c74 7970 653e 6020 6973  , if `<type>` is
+0001a200: 2067 6976 656e 2066 6f72 2061 6e79 2066   given for any f
+0001a210: 6965 6c64 2c20 5b60 7479 7069 6e67 2e4e  ield, [`typing.N
+0001a220: 616d 6564 5475 706c 6560 5d28 6874 7470  amedTuple`](http
+0001a230: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
+0001a240: 6f72 672f 332f 6c69 6272 6172 792f 7479  org/3/library/ty
+0001a250: 7069 6e67 2e68 746d 6c23 7479 7069 6e67  ping.html#typing
+0001a260: 2e4e 616d 6564 5475 706c 6529 2069 7320  .NamedTuple) is 
+0001a270: 7573 6564 2069 6e73 7465 6164 206f 6620  used instead of 
+0001a280: 6063 6f6c 6c65 6374 696f 6e73 2e6e 616d  `collections.nam
+0001a290: 6564 7475 706c 6560 2e0a 0a41 6e6f 6e79  edtuple`...Anony
+0001a2a0: 6d6f 7573 2060 6e61 6d65 6474 7570 6c65  mous `namedtuple
+0001a2b0: 6073 2061 6c73 6f20 7375 7070 6f72 7420  `s also support 
+0001a2c0: 5b6b 6579 776f 7264 2061 7267 756d 656e  [keyword argumen
+0001a2d0: 7420 6e61 6d65 2065 6c69 7369 6f6e 5d28  t name elision](
+0001a2e0: 236b 6579 776f 7264 2d61 7267 756d 656e  #keyword-argumen
+0001a2f0: 742d 6e61 6d65 2d65 6c69 7369 6f6e 292e  t-name-elision).
+0001a300: 0a0a 2323 2323 2320 605f 6e61 6d65 6474  ..##### `_namedt
+0001a310: 7570 6c65 5f6f 6660 0a0a 4f6e 2050 7974  uple_of`..On Pyt
+0001a320: 686f 6e20 7665 7273 696f 6e73 2060 3e3d  hon versions `>=
+0001a330: 332e 3660 2c20 605f 6e61 6d65 6474 7570  3.6`, `_namedtup
+0001a340: 6c65 5f6f 6660 2069 7320 7072 6f76 6964  le_of` is provid
+0001a350: 6564 2061 7320 6120 6275 696c 742d 696e  ed as a built-in
+0001a360: 2074 6861 7420 6361 6e20 6d69 6d69 6320   that can mimic 
+0001a370: 7468 6520 6265 6861 7669 6f72 206f 6620  the behavior of 
+0001a380: 616e 6f6e 796d 6f75 7320 6e61 6d65 6474  anonymous namedt
+0001a390: 7570 6c65 206c 6974 6572 616c 7320 7375  uple literals su
+0001a3a0: 6368 2074 6861 7420 605f 6e61 6d65 6474  ch that `_namedt
+0001a3b0: 7570 6c65 5f6f 6628 613d 312c 2062 3d32  uple_of(a=1, b=2
+0001a3c0: 2960 2069 7320 6571 7569 7661 6c65 6e74  )` is equivalent
+0001a3d0: 2074 6f20 6028 613d 312c 2062 3d32 2960   to `(a=1, b=2)`
+0001a3e0: 2e20 5369 6e63 6520 605f 6e61 6d65 6474  . Since `_namedt
+0001a3f0: 7570 6c65 5f6f 6660 2069 7320 6f6e 6c79  uple_of` is only
+0001a400: 2061 7661 696c 6162 6c65 206f 6e20 5079   available on Py
+0001a410: 7468 6f6e 2033 2e36 2061 6e64 2061 626f  thon 3.6 and abo
+0001a420: 7665 2c20 686f 7765 7665 722c 2069 7420  ve, however, it 
+0001a430: 6973 2067 656e 6572 616c 6c79 2072 6563  is generally rec
+0001a440: 6f6d 6d65 6e64 6564 2074 6f20 7573 6520  ommended to use 
+0001a450: 616e 6f6e 796d 6f75 7320 6e61 6d65 6474  anonymous namedt
+0001a460: 7570 6c65 206c 6974 6572 616c 7320 696e  uple literals in
+0001a470: 7374 6561 642c 2061 7320 7468 6579 2077  stead, as they w
+0001a480: 6f72 6b20 6f6e 2061 6e79 2050 7974 686f  ork on any Pytho
+0001a490: 6e20 7665 7273 696f 6e2e 0a0a 5f60 5f6e  n version..._`_n
+0001a4a0: 616d 6564 7475 706c 655f 6f66 6020 6973  amedtuple_of` is
+0001a4b0: 206a 7573 7420 7072 6f76 6964 6564 2074   just provided t
+0001a4c0: 6f20 6769 7665 206e 616d 6564 7475 706c  o give namedtupl
+0001a4d0: 6520 6c69 7465 7261 6c73 2061 2072 6570  e literals a rep
+0001a4e0: 7265 7365 6e74 6174 696f 6e20 7468 6174  resentation that
+0001a4f0: 2063 6f72 7265 7370 6f6e 6473 2074 6f20   corresponds to 
+0001a500: 616e 2065 7870 7265 7373 696f 6e20 7468  an expression th
+0001a510: 6174 2063 616e 2062 6520 7573 6564 2074  at can be used t
+0001a520: 6f20 7265 6372 6561 7465 2074 6865 6d2e  o recreate them.
+0001a530: 5f0a 0a23 2323 2323 2045 7861 6d70 6c65  _..##### Example
+0001a540: 0a0a 2a2a 436f 636f 6e75 743a 2a2a 0a60  ..**Coconut:**.`
+0001a550: 6060 636f 636f 6e75 740a 7573 6572 7320  ``coconut.users 
+0001a560: 3d20 5b0a 2020 2020 2869 643d 312c 206e  = [.    (id=1, n
+0001a570: 616d 653d 2241 6c69 6365 2229 2c0a 2020  ame="Alice"),.  
+0001a580: 2020 2869 643d 322c 206e 616d 653d 2242    (id=2, name="B
+0001a590: 6f62 2229 2c0a 5d0a 6060 600a 0a2a 2a50  ob"),.].```..**P
+0001a5a0: 7974 686f 6e3a 2a2a 0a60 6060 636f 636f  ython:**.```coco
+0001a5b0: 6e75 745f 7079 7468 6f6e 0a66 726f 6d20  nut_python.from 
+0001a5c0: 636f 6c6c 6563 7469 6f6e 7320 696d 706f  collections impo
+0001a5d0: 7274 206e 616d 6564 7475 706c 650a 0a75  rt namedtuple..u
+0001a5e0: 7365 7273 203d 205b 0a20 2020 206e 616d  sers = [.    nam
+0001a5f0: 6564 7475 706c 6528 225f 222c 2022 6964  edtuple("_", "id
+0001a600: 2c20 6e61 6d65 2229 2831 2c20 2241 6c69  , name")(1, "Ali
+0001a610: 6365 2229 2c0a 2020 2020 6e61 6d65 6474  ce"),.    namedt
+0001a620: 7570 6c65 2822 5f22 2c20 2269 642c 206e  uple("_", "id, n
+0001a630: 616d 6522 2928 322c 2022 426f 6222 292c  ame")(2, "Bob"),
+0001a640: 0a5d 0a60 6060 0a0a 2323 2320 5365 7420  .].```..### Set 
+0001a650: 4c69 7465 7261 6c73 0a0a 436f 636f 6e75  Literals..Coconu
+0001a660: 7420 616c 6c6f 7773 2061 6e20 6f70 7469  t allows an opti
+0001a670: 6f6e 616c 2060 7360 2074 6f20 6265 2070  onal `s` to be p
+0001a680: 7265 7065 6e64 6564 2069 6e20 6672 6f6e  repended in fron
+0001a690: 7420 6f66 2050 7974 686f 6e20 7365 7420  t of Python set 
+0001a6a0: 6c69 7465 7261 6c73 2e20 5768 696c 6520  literals. While 
+0001a6b0: 696e 206d 6f73 7420 6361 7365 7320 7468  in most cases th
+0001a6c0: 6973 2064 6f65 7320 6e6f 7468 696e 672c  is does nothing,
+0001a6d0: 2069 6e20 7468 6520 6361 7365 206f 6620   in the case of 
+0001a6e0: 7468 6520 656d 7074 7920 7365 7420 6974  the empty set it
+0001a6f0: 206c 6574 7320 436f 636f 6e75 7420 6b6e   lets Coconut kn
+0001a700: 6f77 2074 6861 7420 6974 2069 7320 616e  ow that it is an
+0001a710: 2065 6d70 7479 2073 6574 2061 6e64 206e   empty set and n
+0001a720: 6f74 2061 6e20 656d 7074 7920 6469 6374  ot an empty dict
+0001a730: 696f 6e61 7279 2e20 5365 7420 6c69 7465  ionary. Set lite
+0001a740: 7261 6c73 2061 6c73 6f20 7375 7070 6f72  rals also suppor
+0001a750: 7420 756e 7061 636b 696e 6720 7379 6e74  t unpacking synt
+0001a760: 6178 2028 652e 672e 2060 737b 2a78 737d  ax (e.g. `s{*xs}
+0001a770: 6029 2e0a 0a41 6464 6974 696f 6e61 6c6c  `)...Additionall
+0001a780: 792c 2043 6f63 6f6e 7574 2061 6c73 6f20  y, Coconut also 
+0001a790: 7375 7070 6f72 7473 2072 6570 6c61 6369  supports replaci
+0001a7a0: 6e67 2074 6865 2060 7360 2077 6974 6820  ng the `s` with 
+0001a7b0: 616e 2060 6660 2074 6f20 6765 6e65 7261  an `f` to genera
+0001a7c0: 7465 2061 2060 6672 6f7a 656e 7365 7460  te a `frozenset`
+0001a7d0: 206f 7220 616e 2060 6d60 2074 6f20 6765   or an `m` to ge
+0001a7e0: 6e65 7261 7465 2061 2043 6f63 6f6e 7574  nerate a Coconut
+0001a7f0: 205b 606d 756c 7469 7365 7460 5d28 236d   [`multiset`](#m
+0001a800: 756c 7469 7365 7429 2e0a 0a23 2323 2323  ultiset)...#####
+0001a810: 2045 7861 6d70 6c65 0a0a 2a2a 436f 636f   Example..**Coco
+0001a820: 6e75 743a 2a2a 0a60 6060 636f 636f 6e75  nut:**.```coconu
+0001a830: 740a 656d 7074 795f 6672 6f7a 656e 5f73  t.empty_frozen_s
+0001a840: 6574 203d 2066 7b7d 0a60 6060 0a0a 2a2a  et = f{}.```..**
+0001a850: 5079 7468 6f6e 3a2a 2a0a 6060 6063 6f63  Python:**.```coc
+0001a860: 6f6e 7574 5f70 7974 686f 6e0a 656d 7074  onut_python.empt
+0001a870: 795f 6672 6f7a 656e 5f73 6574 203d 2066  y_frozen_set = f
+0001a880: 726f 7a65 6e73 6574 2829 0a60 6060 0a0a  rozenset().```..
+0001a890: 2323 2320 496d 6167 696e 6172 7920 4c69  ### Imaginary Li
+0001a8a0: 7465 7261 6c73 0a0a 496e 2061 6464 6974  terals..In addit
+0001a8b0: 696f 6e20 746f 2050 7974 686f 6e27 7320  ion to Python's 
+0001a8c0: 603c 6e75 6d3e 6a60 206f 7220 603c 6e75  `<num>j` or `<nu
+0001a8d0: 6d3e 4a60 206e 6f74 6174 696f 6e20 666f  m>J` notation fo
+0001a8e0: 7220 696d 6167 696e 6172 7920 6c69 7465  r imaginary lite
+0001a8f0: 7261 6c73 2c20 436f 636f 6e75 7420 616c  rals, Coconut al
+0001a900: 736f 2073 7570 706f 7274 7320 603c 6e75  so supports `<nu
+0001a910: 6d3e 6960 206f 7220 603c 6e75 6d3e 4960  m>i` or `<num>I`
+0001a920: 2c20 746f 206d 616b 6520 696d 6167 696e  , to make imagin
+0001a930: 6172 7920 6c69 7465 7261 6c73 206d 6f72  ary literals mor
+0001a940: 6520 7265 6164 6162 6c65 2069 6620 7573  e readable if us
+0001a950: 6564 2069 6e20 6120 6d61 7468 656d 6174  ed in a mathemat
+0001a960: 6963 616c 2063 6f6e 7465 7874 2e0a 0a23  ical context...#
+0001a970: 2323 2323 2050 7974 686f 6e20 446f 6373  #### Python Docs
+0001a980: 0a0a 496d 6167 696e 6172 7920 6c69 7465  ..Imaginary lite
+0001a990: 7261 6c73 2061 7265 2064 6573 6372 6962  rals are describ
+0001a9a0: 6564 2062 7920 7468 6520 666f 6c6c 6f77  ed by the follow
+0001a9b0: 696e 6720 6c65 7869 6361 6c20 6465 6669  ing lexical defi
+0001a9c0: 6e69 7469 6f6e 733a 0a60 6060 636f 636f  nitions:.```coco
+0001a9d0: 6e75 740a 696d 6167 6e75 6d62 6572 203a  nut.imagnumber :
+0001a9e0: 3a3d 2028 666c 6f61 746e 756d 6265 7220  := (floatnumber 
+0001a9f0: 7c20 696e 7470 6172 7429 2028 226a 2220  | intpart) ("j" 
+0001aa00: 7c20 224a 2220 7c20 2269 2220 7c20 2249  | "J" | "i" | "I
+0001aa10: 2229 0a60 6060 0a41 6e20 696d 6167 696e  ").```.An imagin
+0001aa20: 6172 7920 6c69 7465 7261 6c20 7969 656c  ary literal yiel
+0001aa30: 6473 2061 2063 6f6d 706c 6578 206e 756d  ds a complex num
+0001aa40: 6265 7220 7769 7468 2061 2072 6561 6c20  ber with a real 
+0001aa50: 7061 7274 206f 6620 302e 302e 2043 6f6d  part of 0.0. Com
+0001aa60: 706c 6578 206e 756d 6265 7273 2061 7265  plex numbers are
+0001aa70: 2072 6570 7265 7365 6e74 6564 2061 7320   represented as 
+0001aa80: 6120 7061 6972 206f 6620 666c 6f61 7469  a pair of floati
+0001aa90: 6e67 2070 6f69 6e74 206e 756d 6265 7273  ng point numbers
+0001aaa0: 2061 6e64 2068 6176 6520 7468 6520 7361   and have the sa
+0001aab0: 6d65 2072 6573 7472 6963 7469 6f6e 7320  me restrictions 
+0001aac0: 6f6e 2074 6865 6972 2072 616e 6765 2e20  on their range. 
+0001aad0: 546f 2063 7265 6174 6520 6120 636f 6d70  To create a comp
+0001aae0: 6c65 7820 6e75 6d62 6572 2077 6974 6820  lex number with 
+0001aaf0: 6120 6e6f 6e7a 6572 6f20 7265 616c 2070  a nonzero real p
+0001ab00: 6172 742c 2061 6464 2061 2066 6c6f 6174  art, add a float
+0001ab10: 696e 6720 706f 696e 7420 6e75 6d62 6572  ing point number
+0001ab20: 2074 6f20 6974 2c20 652e 672e 2c20 6028   to it, e.g., `(
+0001ab30: 332b 3469 2960 2e20 536f 6d65 2065 7861  3+4i)`. Some exa
+0001ab40: 6d70 6c65 7320 6f66 2069 6d61 6769 6e61  mples of imagina
+0001ab50: 7279 206c 6974 6572 616c 733a 0a60 6060  ry literals:.```
+0001ab60: 636f 636f 6e75 740a 332e 3134 6920 2020  coconut.3.14i   
+0001ab70: 3130 2e69 2020 2020 3130 6920 2020 2020  10.i    10i     
+0001ab80: 2e30 3031 6920 2020 3165 3130 3069 2020  .001i   1e100i  
+0001ab90: 332e 3134 652d 3130 690a 6060 600a 0a23  3.14e-10i.```..#
+0001aba0: 2323 2323 2045 7861 6d70 6c65 0a0a 2a2a  #### Example..**
+0001abb0: 436f 636f 6e75 743a 2a2a 0a60 6060 636f  Coconut:**.```co
+0001abc0: 636f 6e75 740a 3320 2b20 3469 207c 3e20  conut.3 + 4i |> 
+0001abd0: 6162 7320 7c3e 2070 7269 6e74 0a60 6060  abs |> print.```
+0001abe0: 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a 6060  ..**Python:**.``
+0001abf0: 6063 6f63 6f6e 7574 5f70 7974 686f 6e0a  `coconut_python.
+0001ac00: 7072 696e 7428 6162 7328 3320 2b20 346a  print(abs(3 + 4j
+0001ac10: 2929 0a60 6060 0a0a 2323 2320 416c 7465  )).```..### Alte
+0001ac20: 726e 6174 6976 6520 5465 726e 6172 7920  rnative Ternary 
+0001ac30: 4f70 6572 6174 6f72 0a0a 5079 7468 6f6e  Operator..Python
+0001ac40: 2073 7570 706f 7274 7320 7468 6520 7465   supports the te
+0001ac50: 726e 6172 7920 6f70 6572 6174 6f72 2073  rnary operator s
+0001ac60: 796e 7461 780a 6060 6063 6f63 6f6e 7574  yntax.```coconut
+0001ac70: 5f70 7974 686f 6e0a 7265 7375 6c74 203d  _python.result =
+0001ac80: 2069 665f 7472 7565 2069 6620 636f 6e64   if_true if cond
+0001ac90: 6974 696f 6e20 656c 7365 2069 665f 6661  ition else if_fa
+0001aca0: 6c73 650a 6060 600a 7768 6963 682c 2073  lse.```.which, s
+0001acb0: 696e 6365 2043 6f63 6f6e 7574 2069 7320  ince Coconut is 
+0001acc0: 6120 7375 7065 7273 6574 206f 6620 5079  a superset of Py
+0001acd0: 7468 6f6e 2c20 436f 636f 6e75 7420 616c  thon, Coconut al
+0001ace0: 736f 2073 7570 706f 7274 732e 0a0a 486f  so supports...Ho
+0001acf0: 7765 7665 722c 2043 6f63 6f6e 7574 2061  wever, Coconut a
+0001ad00: 6c73 6f20 7072 6f76 6964 6573 2061 6e20  lso provides an 
+0001ad10: 616c 7465 726e 6174 6976 6520 7379 6e74  alternative synt
+0001ad20: 6178 2074 6861 7420 7573 6573 2074 6865  ax that uses the
+0001ad30: 206d 6f72 6520 636f 6e76 656e 7469 6f6e   more convention
+0001ad40: 616c 2061 7267 756d 656e 7420 6f72 6465  al argument orde
+0001ad50: 7269 6e67 2061 730a 6060 600a 7265 7375  ring as.```.resu
+0001ad60: 6c74 203d 2069 6620 636f 6e64 6974 696f  lt = if conditio
+0001ad70: 6e20 7468 656e 2069 665f 7472 7565 2065  n then if_true e
+0001ad80: 6c73 6520 6966 5f66 616c 7365 0a60 6060  lse if_false.```
+0001ad90: 0a6d 616b 696e 6720 7573 6520 6f66 2074  .making use of t
+0001ada0: 6865 2043 6f63 6f6e 7574 2d73 7065 6369  he Coconut-speci
+0001adb0: 6669 6320 6074 6865 6e60 206b 6579 776f  fic `then` keywo
+0001adc0: 7264 2028 5b74 686f 7567 6820 436f 636f  rd ([though Coco
+0001add0: 6e75 7420 7374 696c 6c20 616c 6c6f 7773  nut still allows
+0001ade0: 2060 7468 656e 6020 6173 2061 2076 6172   `then` as a var
+0001adf0: 6961 626c 6520 6e61 6d65 5d28 2368 616e  iable name](#han
+0001ae00: 646c 696e 672d 6b65 7977 6f72 642d 7661  dling-keyword-va
+0001ae10: 7269 6162 6c65 2d6e 616d 652d 6f76 6572  riable-name-over
+0001ae20: 6c61 7029 292e 0a0a 2323 2323 2320 4578  lap))...##### Ex
+0001ae30: 616d 706c 650a 0a2a 2a43 6f63 6f6e 7574  ample..**Coconut
+0001ae40: 3a2a 2a0a 6060 6063 6f63 6f6e 7574 0a76  :**.```coconut.v
+0001ae50: 616c 7565 203d 2028 0a20 2020 2069 6620  alue = (.    if 
+0001ae60: 7368 6f75 6c64 5f75 7365 5f61 2829 2074  should_use_a() t
+0001ae70: 6865 6e20 610a 2020 2020 656c 7365 2069  hen a.    else i
+0001ae80: 6620 7368 6f75 6c64 5f75 7365 5f62 2829  f should_use_b()
+0001ae90: 2074 6865 6e20 620a 2020 2020 656c 7365   then b.    else
+0001aea0: 2069 6620 7368 6f75 6c64 5f75 7365 5f63   if should_use_c
+0001aeb0: 2829 2074 6865 6e20 630a 2020 2020 656c  () then c.    el
+0001aec0: 7365 2066 616c 6c62 6163 6b0a 290a 6060  se fallback.).``
+0001aed0: 600a 0a2a 2a50 7974 686f 6e3a 2a2a 0a60  `..**Python:**.`
+0001aee0: 6060 636f 636f 6e75 745f 7079 7468 6f6e  ``coconut_python
+0001aef0: 0a76 616c 7565 203d 2028 0a20 2020 2061  .value = (.    a
+0001af00: 2069 6620 7368 6f75 6c64 5f75 7365 5f61   if should_use_a
+0001af10: 2829 2065 6c73 650a 2020 2020 6220 6966  () else.    b if
+0001af20: 2073 686f 756c 645f 7573 655f 6228 2920   should_use_b() 
+0001af30: 656c 7365 0a20 2020 2063 2069 6620 7368  else.    c if sh
+0001af40: 6f75 6c64 5f75 7365 5f63 2829 2065 6c73  ould_use_c() els
+0001af50: 650a 2020 2020 6661 6c6c 6261 636b 0a29  e.    fallback.)
+0001af60: 0a60 6060 0a0a 2323 2046 756e 6374 696f  .```..## Functio
+0001af70: 6e20 4465 6669 6e69 7469 6f6e 0a0a 6060  n Definition..``
+0001af80: 607b 636f 6e74 656e 7473 7d0a 2d2d 2d0a  `{contents}.---.
+0001af90: 6c6f 6361 6c3a 0a64 6570 7468 3a20 310a  local:.depth: 1.
+0001afa0: 2d2d 2d0a 6060 600a 0a23 2323 2054 6169  ---.```..### Tai
+0001afb0: 6c20 4361 6c6c 204f 7074 696d 697a 6174  l Call Optimizat
+0001afc0: 696f 6e0a 0a43 6f63 6f6e 7574 2077 696c  ion..Coconut wil
+0001afd0: 6c20 7065 7266 6f72 6d20 6175 746f 6d61  l perform automa
+0001afe0: 7469 6320 5b74 6169 6c20 6361 6c6c 5d28  tic [tail call](
+0001aff0: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
+0001b000: 6564 6961 2e6f 7267 2f77 696b 692f 5461  edia.org/wiki/Ta
+0001b010: 696c 5f63 616c 6c29 206f 7074 696d 697a  il_call) optimiz
+0001b020: 6174 696f 6e20 616e 6420 7461 696c 2072  ation and tail r
+0001b030: 6563 7572 7369 6f6e 2065 6c69 6d69 6e61  ecursion elimina
+0001b040: 7469 6f6e 206f 6e20 616e 7920 6675 6e63  tion on any func
+0001b050: 7469 6f6e 2074 6861 7420 6d65 6574 7320  tion that meets 
+0001b060: 7468 6520 666f 6c6c 6f77 696e 6720 6372  the following cr
+0001b070: 6974 6572 6961 3a0a 0a31 2e20 6974 206d  iteria:..1. it m
+0001b080: 7573 7420 6469 7265 6374 6c79 2072 6574  ust directly ret
+0001b090: 7572 6e20 2875 7369 6e67 2065 6974 6865  urn (using eithe
+0001b0a0: 7220 6072 6574 7572 6e60 206f 7220 5b61  r `return` or [a
+0001b0b0: 7373 6967 6e6d 656e 7420 6675 6e63 7469  ssignment functi
+0001b0c0: 6f6e 206e 6f74 6174 696f 6e5d 2823 6173  on notation](#as
+0001b0d0: 7369 676e 6d65 6e74 2d66 756e 6374 696f  signment-functio
+0001b0e0: 6e73 2929 2061 2063 616c 6c20 746f 2069  ns)) a call to i
+0001b0f0: 7473 656c 6620 2874 6169 6c20 7265 6375  tself (tail recu
+0001b100: 7273 696f 6e20 656c 696d 696e 6174 696f  rsion eliminatio
+0001b110: 6e2c 2074 6865 206d 6f73 7420 706f 7765  n, the most powe
+0001b120: 7266 756c 206f 7074 696d 697a 6174 696f  rful optimizatio
+0001b130: 6e29 206f 7220 616e 6f74 6865 7220 6675  n) or another fu
+0001b140: 6e63 7469 6f6e 2028 7461 696c 2063 616c  nction (tail cal
+0001b150: 6c20 6f70 7469 6d69 7a61 7469 6f6e 292c  l optimization),
+0001b160: 0a32 2e20 6974 206d 7573 7420 6e6f 7420  .2. it must not 
+0001b170: 6265 2061 2067 656e 6572 6174 6f72 2028  be a generator (
+0001b180: 7573 6573 2060 7969 656c 6460 2920 6f72  uses `yield`) or
+0001b190: 2061 6e20 6173 796e 6368 726f 6e6f 7573   an asynchronous
+0001b1a0: 2066 756e 6374 696f 6e20 2875 7365 7320   function (uses 
+0001b1b0: 6061 7379 6e63 6029 2e0a 0a54 6169 6c20  `async`)...Tail 
+0001b1c0: 6361 6c6c 206f 7074 696d 697a 6174 696f  call optimizatio
+0001b1d0: 6e20 2874 686f 7567 6820 6e6f 7420 7461  n (though not ta
+0001b1e0: 696c 2072 6563 7572 7369 6f6e 2065 6c69  il recursion eli
+0001b1f0: 6d69 6e61 7469 6f6e 2920 7769 6c6c 2077  mination) will w
+0001b200: 6f72 6b20 6576 656e 2066 6f72 2031 2920  ork even for 1) 
+0001b210: 6d75 7475 616c 2072 6563 7572 7369 6f6e  mutual recursion
+0001b220: 2061 6e64 2032 2920 7061 7474 6572 6e2d   and 2) pattern-
+0001b230: 6d61 7463 6869 6e67 2066 756e 6374 696f  matching functio
+0001b240: 6e73 2073 706c 6974 2061 6372 6f73 7320  ns split across 
+0001b250: 6d75 6c74 6970 6c65 2064 6566 696e 6974  multiple definit
+0001b260: 696f 6e73 2075 7369 6e67 205b 6061 6464  ions using [`add
+0001b270: 7061 7474 6572 6e60 5d28 2361 6464 7061  pattern`](#addpa
+0001b280: 7474 6572 6e29 2e0a 0a49 6620 796f 7520  ttern)...If you 
+0001b290: 6172 6520 656e 636f 756e 7465 7269 6e67  are encountering
+0001b2a0: 2061 2060 5275 6e74 696d 6545 7272 6f72   a `RuntimeError
+0001b2b0: 6020 6475 6520 746f 206d 6178 696d 756d  ` due to maximum
+0001b2c0: 2072 6563 7572 7369 6f6e 2064 6570 7468   recursion depth
+0001b2d0: 2c20 6974 2069 7320 6869 6768 6c79 2072  , it is highly r
+0001b2e0: 6563 6f6d 6d65 6e64 6564 2074 6861 7420  ecommended that 
+0001b2f0: 796f 7520 7265 7772 6974 6520 796f 7572  you rewrite your
+0001b300: 2066 756e 6374 696f 6e20 746f 206d 6565   function to mee
+0001b310: 7420 6569 7468 6572 2074 6865 2063 7269  t either the cri
+0001b320: 7465 7269 6120 6162 6f76 6520 666f 7220  teria above for 
+0001b330: 7461 696c 2063 616c 6c20 6f70 7469 6d69  tail call optimi
+0001b340: 7a61 7469 6f6e 2c20 6f72 2074 6865 2063  zation, or the c
+0001b350: 6f72 7265 7370 6f6e 6469 6e67 2063 7269  orresponding cri
+0001b360: 7465 7269 6120 666f 7220 5b60 7265 6375  teria for [`recu
+0001b370: 7273 6976 655f 6974 6572 6174 6f72 605d  rsive_iterator`]
+0001b380: 2823 7265 6375 7273 6976 652d 6974 6572  (#recursive-iter
+0001b390: 6174 6f72 292c 2065 6974 6865 7220 6f66  ator), either of
+0001b3a0: 2077 6869 6368 2073 686f 756c 6420 7072   which should pr
+0001b3b0: 6576 656e 7420 7375 6368 2065 7272 6f72  event such error
+0001b3c0: 732e 0a0a 2323 2323 2320 4578 616d 706c  s...##### Exampl
+0001b3d0: 650a 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a  e..**Coconut:**.
+0001b3e0: 6060 6063 6f63 6f6e 7574 0a23 2075 6e6c  ```coconut.# unl
+0001b3f0: 696b 6520 696e 2050 7974 686f 6e2c 2074  ike in Python, t
+0001b400: 6869 7320 6675 6e63 7469 6f6e 2077 696c  his function wil
+0001b410: 6c20 6e65 7665 7220 6869 7420 6120 6d61  l never hit a ma
+0001b420: 7869 6d75 6d20 7265 6375 7273 696f 6e20  ximum recursion 
+0001b430: 6465 7074 6820 6572 726f 720a 6465 6620  depth error.def 
+0001b440: 6661 6374 6f72 6961 6c28 6e2c 2061 6363  factorial(n, acc
+0001b450: 3d31 293a 0a20 2020 206d 6174 6368 206e  =1):.    match n
+0001b460: 3a0a 2020 2020 2020 2020 6361 7365 2030  :.        case 0
+0001b470: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0001b480: 7475 726e 2061 6363 0a20 2020 2020 2020  turn acc.       
+0001b490: 2063 6173 6520 696e 7428 2920 6966 206e   case int() if n
+0001b4a0: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
+0001b4b0: 2020 7265 7475 726e 2066 6163 746f 7269    return factori
+0001b4c0: 616c 286e 2d31 2c20 6163 632a 6e29 0a60  al(n-1, acc*n).`
+0001b4d0: 6060 0a5f 5368 6f77 6361 7365 7320 7461  ``._Showcases ta
+0001b4e0: 696c 2072 6563 7572 7369 6f6e 2065 6c69  il recursion eli
+0001b4f0: 6d69 6e61 7469 6f6e 2e5f 0a0a 6060 6063  mination._..```c
+0001b500: 6f63 6f6e 7574 0a23 2075 6e6c 696b 6520  oconut.# unlike 
+0001b510: 696e 2050 7974 686f 6e2c 206e 6569 7468  in Python, neith
+0001b520: 6572 206f 6620 7468 6573 6520 6675 6e63  er of these func
+0001b530: 7469 6f6e 7320 7769 6c6c 2065 7665 7220  tions will ever 
+0001b540: 6869 7420 6120 6d61 7869 6d75 6d20 7265  hit a maximum re
+0001b550: 6375 7273 696f 6e20 6465 7074 6820 6572  cursion depth er
+0001b560: 726f 720a 6465 6620 6973 5f65 7665 6e28  ror.def is_even(
+0001b570: 3029 203d 2054 7275 650a 6164 6470 6174  0) = True.addpat
+0001b580: 7465 726e 2064 6566 2069 735f 6576 656e  tern def is_even
+0001b590: 286e 2060 6973 696e 7374 616e 6365 6020  (n `isinstance` 
+0001b5a0: 696e 7420 6966 206e 203e 2030 2920 3d20  int if n > 0) = 
+0001b5b0: 6973 5f6f 6464 286e 2d31 290a 0a64 6566  is_odd(n-1)..def
+0001b5c0: 2069 735f 6f64 6428 3029 203d 2046 616c   is_odd(0) = Fal
+0001b5d0: 7365 0a61 6464 7061 7474 6572 6e20 6465  se.addpattern de
+0001b5e0: 6620 6973 5f6f 6464 286e 2060 6973 696e  f is_odd(n `isin
+0001b5f0: 7374 616e 6365 6020 696e 7420 6966 206e  stance` int if n
+0001b600: 203e 2030 2920 3d20 6973 5f65 7665 6e28   > 0) = is_even(
+0001b610: 6e2d 3129 0a60 6060 0a5f 5368 6f77 6361  n-1).```._Showca
+0001b620: 7365 7320 7461 696c 2063 616c 6c20 6f70  ses tail call op
+0001b630: 7469 6d69 7a61 7469 6f6e 2e5f 0a0a 2a2a  timization._..**
+0001b640: 5079 7468 6f6e 3a2a 2a0a 5f43 616e 2774  Python:**._Can't
+0001b650: 2062 6520 646f 6e65 2077 6974 686f 7574   be done without
+0001b660: 2072 6577 7269 7469 6e67 2074 6865 2066   rewriting the f
+0001b670: 756e 6374 696f 6e28 7329 2e5f 0a0a 2323  unction(s)._..##
+0001b680: 2323 2060 2d2d 6e6f 2d74 636f 6020 666c  ## `--no-tco` fl
+0001b690: 6167 0a0a 5461 696c 2063 616c 6c20 6f70  ag..Tail call op
+0001b6a0: 7469 6d69 7a61 7469 6f6e 2077 696c 6c20  timization will 
+0001b6b0: 6265 2074 7572 6e65 6420 6f66 6620 6966  be turned off if
+0001b6c0: 2079 6f75 2070 6173 7320 7468 6520 602d   you pass the `-
+0001b6d0: 2d6e 6f2d 7463 6f60 2063 6f6d 6d61 6e64  -no-tco` command
+0001b6e0: 2d6c 696e 6520 6f70 7469 6f6e 2c20 7768  -line option, wh
+0001b6f0: 6963 6820 6973 2075 7365 6675 6c20 6966  ich is useful if
+0001b700: 2079 6f75 2061 7265 2068 6176 696e 6720   you are having 
+0001b710: 7472 6f75 626c 6520 7265 6164 696e 6720  trouble reading 
+0001b720: 796f 7572 2074 7261 6365 6261 636b 7320  your tracebacks 
+0001b730: 616e 642f 6f72 206e 6565 6420 6d61 7869  and/or need maxi
+0001b740: 6d75 6d20 7065 7266 6f72 6d61 6e63 652e  mum performance.
+0001b750: 0a0a 602d 2d6e 6f2d 7463 6f60 2064 6f65  ..`--no-tco` doe
+0001b760: 7320 6e6f 7420 6469 7361 626c 6520 7461  s not disable ta
+0001b770: 696c 2072 6563 7572 7369 6f6e 2065 6c69  il recursion eli
+0001b780: 6d69 6e61 7469 6f6e 2e0a 5468 6973 2069  mination..This i
+0001b790: 7320 6265 6361 7573 6520 7461 696c 2072  s because tail r
+0001b7a0: 6563 7572 7369 6f6e 2065 6c69 6d69 6e61  ecursion elimina
+0001b7b0: 7469 6f6e 2069 7320 7573 7561 6c6c 7920  tion is usually 
+0001b7c0: 6661 7374 6572 2074 6861 6e20 646f 696e  faster than doin
+0001b7d0: 6720 6e6f 7468 696e 672c 2077 6869 6c65  g nothing, while
+0001b7e0: 206f 7468 6572 2074 7970 6573 206f 6620   other types of 
+0001b7f0: 7461 696c 2063 616c 6c20 6f70 7469 6d69  tail call optimi
+0001b800: 7a61 7469 6f6e 2061 7265 2075 7375 616c  zation are usual
+0001b810: 6c79 2073 6c6f 7765 7220 7468 616e 2064  ly slower than d
+0001b820: 6f69 6e67 206e 6f74 6869 6e67 2e0a 5461  oing nothing..Ta
+0001b830: 696c 2072 6563 7572 7369 6f6e 2065 6c69  il recursion eli
+0001b840: 6d69 6e61 7469 6f6e 2072 6573 756c 7473  mination results
+0001b850: 2069 6e20 6120 6269 6720 7065 7266 6f72   in a big perfor
+0001b860: 6d61 6e63 6520 7769 6e20 6265 6361 7573  mance win becaus
+0001b870: 6520 5079 7468 6f6e 2068 6173 2061 2066  e Python has a f
+0001b880: 6169 726c 7920 6c61 7267 6520 6675 6e63  airly large func
+0001b890: 7469 6f6e 2063 616c 6c20 6f76 6572 6865  tion call overhe
+0001b8a0: 6164 2e20 4279 2075 6e77 696e 6469 6e67  ad. By unwinding
+0001b8b0: 2061 2072 6563 7572 7369 7665 2066 756e   a recursive fun
+0001b8c0: 6374 696f 6e2c 2066 6172 2066 6577 6572  ction, far fewer
+0001b8d0: 2066 756e 6374 696f 6e20 6361 6c6c 7320   function calls 
+0001b8e0: 6e65 6564 2074 6f20 6265 206d 6164 652e  need to be made.
+0001b8f0: 0a57 6865 6e20 7468 6520 602d 2d6e 6f2d  .When the `--no-
+0001b900: 7463 6f60 2066 6c61 6720 6973 2064 6973  tco` flag is dis
+0001b910: 6162 6c65 642c 2043 6f63 6f6e 7574 2077  abled, Coconut w
+0001b920: 696c 6c20 6174 7465 6d70 7420 746f 2064  ill attempt to d
+0001b930: 6f20 616c 6c20 7479 7065 7320 6f66 2074  o all types of t
+0001b940: 6169 6c20 6361 6c6c 206f 7074 696d 697a  ail call optimiz
+0001b950: 6174 696f 6e73 2c20 6861 6e64 6c69 6e67  ations, handling
+0001b960: 206e 6f6e 2d72 6563 7572 7369 7665 2074   non-recursive t
+0001b970: 6169 6c20 6361 6c6c 732c 2073 706c 6974  ail calls, split
+0001b980: 2070 6174 7465 726e 2d6d 6174 6368 696e   pattern-matchin
+0001b990: 6720 6675 6e63 7469 6f6e 732c 206d 7574  g functions, mut
+0001b9a0: 7561 6c20 7265 6375 7273 696f 6e2c 2061  ual recursion, a
+0001b9b0: 6e64 2074 6169 6c20 7265 6375 7273 696f  nd tail recursio
+0001b9c0: 6e2e 2057 6865 6e20 7468 6520 602d 2d6e  n. When the `--n
+0001b9d0: 6f2d 7463 6f60 2066 6c61 6720 6973 2065  o-tco` flag is e
+0001b9e0: 6e61 626c 6564 2c20 436f 636f 6e75 7420  nabled, Coconut 
+0001b9f0: 7769 6c6c 206e 6f20 6c6f 6e67 6572 2070  will no longer p
+0001ba00: 6572 666f 726d 2061 6e79 2074 6169 6c20  erform any tail 
+0001ba10: 6361 6c6c 206f 7074 696d 697a 6174 696f  call optimizatio
+0001ba20: 6e73 206f 7468 6572 2074 6861 6e20 7461  ns other than ta
+0001ba30: 696c 2072 6563 7572 7369 6f6e 2065 6c69  il recursion eli
+0001ba40: 6d69 6e61 7469 6f6e 2e0a 0a23 2323 2320  mination...#### 
+0001ba50: 5461 696c 2052 6563 7572 7369 6f6e 2045  Tail Recursion E
+0001ba60: 6c69 6d69 6e61 7469 6f6e 2061 6e64 2050  limination and P
+0001ba70: 7974 686f 6e20 6c61 6d62 6461 730a 0a43  ython lambdas..C
+0001ba80: 6f63 6f6e 7574 2064 6f65 7320 6e6f 7420  oconut does not 
+0001ba90: 7065 7266 6f72 6d20 7461 696c 2072 6563  perform tail rec
+0001baa0: 7572 7369 6f6e 2065 6c69 6d69 6e61 7469  ursion eliminati
+0001bab0: 6f6e 2069 6e20 6675 6e63 7469 6f6e 7320  on in functions 
+0001bac0: 7468 6174 2075 7469 6c69 7a65 206c 616d  that utilize lam
+0001bad0: 6264 6173 206f 7220 696e 6e65 7220 6675  bdas or inner fu
+0001bae0: 6e63 7469 6f6e 732e 2054 6869 7320 6973  nctions. This is
+0001baf0: 2062 6563 6175 7365 206f 6620 7468 6520   because of the 
+0001bb00: 7761 7920 7468 6174 2050 7974 686f 6e20  way that Python 
+0001bb10: 6861 6e64 6c65 7320 6c61 6d62 6461 732e  handles lambdas.
+0001bb20: 0a0a 4561 6368 206c 616d 6264 6120 7374  ..Each lambda st
+0001bb30: 6f72 6573 2061 2070 6f69 6e74 6572 2074  ores a pointer t
+0001bb40: 6f20 7468 6520 6e61 6d65 7370 6163 6520  o the namespace 
+0001bb50: 656e 636c 6f73 696e 6720 6974 2c20 7261  enclosing it, ra
+0001bb60: 7468 6572 2074 6861 6e20 6120 636f 7079  ther than a copy
+0001bb70: 206f 6620 7468 6520 6e61 6d65 7370 6163   of the namespac
+0001bb80: 652e 2054 6875 732c 2069 6620 7468 6520  e. Thus, if the 
+0001bb90: 436f 636f 6e75 7420 636f 6d70 696c 6572  Coconut compiler
+0001bba0: 2074 7269 6573 2074 6f20 7265 6379 636c   tries to recycl
+0001bbb0: 6520 616e 7974 6869 6e67 2069 6e20 7468  e anything in th
+0001bbc0: 6520 6e61 6d65 7370 6163 6520 7468 6174  e namespace that
+0001bbd0: 2070 726f 6475 6365 6420 7468 6520 6c61   produced the la
+0001bbe0: 6d62 6461 2c20 7768 6963 6820 6e65 6564  mbda, which need
+0001bbf0: 7320 746f 2062 6520 646f 6e65 2066 6f72  s to be done for
+0001bc00: 2054 5245 2c20 7468 6520 6c61 6d62 6461   TRE, the lambda
+0001bc10: 2063 616e 2062 6520 6368 616e 6765 6420   can be changed 
+0001bc20: 7265 7472 6f61 6374 6976 656c 792e 0a0a  retroactively...
+0001bc30: 4120 7369 6d70 6c65 2065 7861 6d70 6c65  A simple example
+0001bc40: 2064 656d 6f6e 7374 7261 7469 6e67 2074   demonstrating t
+0001bc50: 6869 7320 6265 6861 7669 6f72 2069 6e20  his behavior in 
+0001bc60: 5079 7468 6f6e 3a0a 0a60 6060 7079 7468  Python:..```pyth
+0001bc70: 6f6e 0a78 203d 2031 0a66 6f6f 203d 206c  on.x = 1.foo = l
+0001bc80: 616d 6264 613a 2078 0a70 7269 6e74 2866  ambda: x.print(f
+0001bc90: 6f6f 2829 2920 2023 2031 0a78 203d 2032  oo())  # 1.x = 2
+0001bca0: 2020 2020 2020 2020 2023 2044 6972 6563           # Direc
+0001bcb0: 746c 7920 616c 7465 7220 7468 6520 7661  tly alter the va
+0001bcc0: 6c75 6573 2069 6e20 7468 6520 6e61 6d65  lues in the name
+0001bcd0: 7370 6163 6520 656e 636c 6f73 696e 6720  space enclosing 
+0001bce0: 666f 6f0a 7072 696e 7428 666f 6f28 2929  foo.print(foo())
+0001bcf0: 2020 2320 3220 2821 290a 6060 600a 0a42    # 2 (!).```..B
+0001bd00: 6563 6175 7365 2074 6869 7320 636f 756c  ecause this coul
+0001bd10: 6420 6861 7665 2075 6e69 6e74 656e 6465  d have unintende
+0001bd20: 6420 616e 6420 706f 7465 6e74 6961 6c6c  d and potentiall
+0001bd30: 7920 6461 6d61 6769 6e67 2063 6f6e 7365  y damaging conse
+0001bd40: 7175 656e 6365 732c 2043 6f63 6f6e 7574  quences, Coconut
+0001bd50: 206f 7074 7320 746f 206e 6f74 2070 6572   opts to not per
+0001bd60: 666f 726d 2054 5245 206f 6e20 616e 7920  form TRE on any 
+0001bd70: 6675 6e63 7469 6f6e 2077 6974 6820 6120  function with a 
+0001bd80: 6c61 6d62 6461 206f 7220 696e 6e65 7220  lambda or inner 
+0001bd90: 6675 6e63 7469 6f6e 2e0a 0a23 2323 2041  function...### A
+0001bda0: 7373 6967 6e6d 656e 7420 4675 6e63 7469  ssignment Functi
+0001bdb0: 6f6e 730a 0a43 6f63 6f6e 7574 2061 6c6c  ons..Coconut all
+0001bdc0: 6f77 7320 666f 7220 6173 7369 676e 6d65  ows for assignme
+0001bdd0: 6e74 2066 756e 6374 696f 6e20 6465 6669  nt function defi
+0001bde0: 6e69 7469 6f6e 2074 6861 7420 6175 746f  nition that auto
+0001bdf0: 6d61 7469 6361 6c6c 7920 7265 7475 726e  matically return
+0001be00: 7320 7468 6520 6c61 7374 206c 696e 6520  s the last line 
+0001be10: 6f66 2074 6865 2066 756e 6374 696f 6e20  of the function 
+0001be20: 626f 6479 2e20 416e 2061 7373 6967 6e6d  body. An assignm
+0001be30: 656e 7420 6675 6e63 7469 6f6e 2069 7320  ent function is 
+0001be40: 636f 6e73 7472 7563 7465 6420 6279 2073  constructed by s
+0001be50: 7562 7374 6974 7574 696e 6720 603d 6020  ubstituting `=` 
+0001be60: 666f 7220 603a 6020 6166 7465 7220 7468  for `:` after th
+0001be70: 6520 6675 6e63 7469 6f6e 2064 6566 696e  e function defin
+0001be80: 6974 696f 6e20 6c69 6e65 2e20 5468 7573  ition line. Thus
+0001be90: 2c20 7468 6520 7379 6e74 6178 2066 6f72  , the syntax for
+0001bea0: 2061 7373 6967 6e6d 656e 7420 6675 6e63   assignment func
+0001beb0: 7469 6f6e 2064 6566 696e 6974 696f 6e20  tion definition 
+0001bec0: 6973 2065 6974 6865 720a 6060 6063 6f63  is either.```coc
+0001bed0: 6f6e 7574 0a5b 6173 796e 635d 2064 6566  onut.[async] def
+0001bee0: 203c 6e61 6d65 3e28 3c61 7267 733e 2920   <name>(<args>) 
+0001bef0: 3d20 3c65 7870 723e 0a60 6060 0a66 6f72  = <expr>.```.for
+0001bf00: 206f 6e65 2d6c 696e 6572 7320 6f72 0a60   one-liners or.`
+0001bf10: 6060 636f 636f 6e75 740a 5b61 7379 6e63  ``coconut.[async
+0001bf20: 5d20 6465 6620 3c6e 616d 653e 283c 6172  ] def <name>(<ar
+0001bf30: 6773 3e29 203d 0a20 2020 203c 7374 6d74  gs>) =.    <stmt
+0001bf40: 733e 0a20 2020 203c 6578 7072 3e0a 6060  s>.    <expr>.``
+0001bf50: 600a 666f 7220 6675 6c6c 2066 756e 6374  `.for full funct
+0001bf60: 696f 6e73 2c20 7768 6572 6520 603c 6e61  ions, where `<na
+0001bf70: 6d65 3e60 2069 7320 7468 6520 6e61 6d65  me>` is the name
+0001bf80: 206f 6620 7468 6520 6675 6e63 7469 6f6e   of the function
+0001bf90: 2c20 603c 6172 6773 3e60 2061 7265 2074  , `<args>` are t
+0001bfa0: 6865 2066 756e 6374 696f 6e73 2061 7267  he functions arg
+0001bfb0: 756d 656e 7473 2c20 603c 7374 6d74 733e  uments, `<stmts>
+0001bfc0: 6020 6172 6520 616e 7920 7374 6174 656d  ` are any statem
+0001bfd0: 656e 7473 2074 6861 7420 7468 6520 6675  ents that the fu
+0001bfe0: 6e63 7469 6f6e 2073 686f 756c 6420 6578  nction should ex
+0001bff0: 6563 7574 652c 2061 6e64 2060 3c65 7870  ecute, and `<exp
+0001c000: 723e 6020 6973 2074 6865 2076 616c 7565  r>` is the value
+0001c010: 2074 6861 7420 7468 6520 6675 6e63 7469   that the functi
+0001c020: 6f6e 2073 686f 756c 6420 7265 7475 726e  on should return
+0001c030: 2e0a 0a5f 4e6f 7465 3a20 4173 7369 676e  ..._Note: Assign
+0001c040: 6d65 6e74 2066 756e 6374 696f 6e20 6465  ment function de
+0001c050: 6669 6e69 7469 6f6e 2063 616e 2062 6520  finition can be 
+0001c060: 636f 6d62 696e 6564 2077 6974 6820 696e  combined with in
+0001c070: 6669 7820 616e 642f 6f72 2070 6174 7465  fix and/or patte
+0001c080: 726e 2d6d 6174 6368 696e 6720 6675 6e63  rn-matching func
+0001c090: 7469 6f6e 2064 6566 696e 6974 696f 6e2e  tion definition.
+0001c0a0: 5f0a 0a23 2323 2323 2052 6174 696f 6e61  _..##### Rationa
+0001c0b0: 6c65 0a0a 436f 636f 6e75 7427 7320 4173  le..Coconut's As
+0001c0c0: 7369 676e 6d65 6e74 2066 756e 6374 696f  signment functio
+0001c0d0: 6e20 6465 6669 6e69 7469 6f6e 2069 7320  n definition is 
+0001c0e0: 6173 2065 6173 7920 746f 2077 7269 7465  as easy to write
+0001c0f0: 2061 7320 6173 7369 676e 6d65 6e74 2074   as assignment t
+0001c100: 6f20 6120 6c61 6d62 6461 2c20 6275 7420  o a lambda, but 
+0001c110: 7769 6c6c 2061 7070 6561 7220 6e61 6d65  will appear name
+0001c120: 6420 696e 2074 7261 6365 6261 636b 732c  d in tracebacks,
+0001c130: 2061 7320 6974 2063 6f6d 7069 6c65 7320   as it compiles 
+0001c140: 746f 206e 6f72 6d61 6c20 5079 7468 6f6e  to normal Python
+0001c150: 2066 756e 6374 696f 6e20 6465 6669 6e69   function defini
+0001c160: 7469 6f6e 2e0a 0a23 2323 2323 2045 7861  tion...##### Exa
+0001c170: 6d70 6c65 0a0a 2a2a 436f 636f 6e75 743a  mple..**Coconut:
+0001c180: 2a2a 0a60 6060 636f 636f 6e75 740a 6465  **.```coconut.de
+0001c190: 6620 6269 6e65 7870 2878 2920 3d20 322a  f binexp(x) = 2*
+0001c1a0: 2a78 0a35 207c 3e20 6269 6e65 7870 207c  *x.5 |> binexp |
+0001c1b0: 3e20 7072 696e 740a 6060 600a 0a2a 2a50  > print.```..**P
+0001c1c0: 7974 686f 6e3a 2a2a 0a60 6060 636f 636f  ython:**.```coco
+0001c1d0: 6e75 745f 7079 7468 6f6e 0a64 6566 2062  nut_python.def b
+0001c1e0: 696e 6578 7028 7829 3a20 7265 7475 726e  inexp(x): return
+0001c1f0: 2032 2a2a 780a 7072 696e 7428 6269 6e65   2**x.print(bine
+0001c200: 7870 2835 2929 0a60 6060 0a0a 2323 2320  xp(5)).```..### 
+0001c210: 5061 7474 6572 6e2d 4d61 7463 6869 6e67  Pattern-Matching
+0001c220: 2046 756e 6374 696f 6e73 0a0a 436f 636f   Functions..Coco
+0001c230: 6e75 7420 7061 7474 6572 6e2d 6d61 7463  nut pattern-matc
+0001c240: 6869 6e67 2066 756e 6374 696f 6e73 2061  hing functions a
+0001c250: 7265 206a 7573 7420 6e6f 726d 616c 2066  re just normal f
+0001c260: 756e 6374 696f 6e73 2c20 6578 6365 7074  unctions, except
+0001c270: 2077 6865 7265 2074 6865 2061 7267 756d   where the argum
+0001c280: 656e 7473 2061 7265 2070 6174 7465 726e  ents are pattern
+0001c290: 7320 746f 2062 6520 6d61 7463 6865 6420  s to be matched 
+0001c2a0: 6167 6169 6e73 7420 696e 7374 6561 6420  against instead 
+0001c2b0: 6f66 2076 6172 6961 626c 6573 2074 6f20  of variables to 
+0001c2c0: 6265 2061 7373 6967 6e65 6420 746f 2e20  be assigned to. 
+0001c2d0: 5468 6520 7379 6e74 6178 2066 6f72 2070  The syntax for p
+0001c2e0: 6174 7465 726e 2d6d 6174 6368 696e 6720  attern-matching 
+0001c2f0: 6675 6e63 7469 6f6e 2064 6566 696e 6974  function definit
+0001c300: 696f 6e20 6973 0a60 6060 636f 636f 6e75  ion is.```coconu
+0001c310: 740a 5b6d 6174 6368 5d20 6465 6620 3c6e  t.[match] def <n
+0001c320: 616d 653e 283c 6172 673e 2c20 3c61 7267  ame>(<arg>, <arg
+0001c330: 3e2c 202e 2e2e 205b 6966 203c 636f 6e64  >, ... [if <cond
+0001c340: 3e5d 2920 5b2d 3e20 3c72 6574 7572 6e5f  >]) [-> <return_
+0001c350: 7479 7065 3e5d 3a0a 2020 2020 3c62 6f64  type>]:.    <bod
+0001c360: 793e 0a60 6060 0a77 6865 7265 2060 3c61  y>.```.where `<a
+0001c370: 7267 3e60 2069 7320 6465 6669 6e65 6420  rg>` is defined 
+0001c380: 6173 0a60 6060 636f 636f 6e75 740a 5b2a  as.```coconut.[*
+0001c390: 7c2a 2a5d 203c 7061 7474 6572 6e3e 205b  |**] <pattern> [
+0001c3a0: 3d20 3c64 6566 6175 6c74 3e5d 0a60 6060  = <default>].```
+0001c3b0: 0a77 6865 7265 2060 3c6e 616d 653e 6020  .where `<name>` 
+0001c3c0: 6973 2074 6865 206e 616d 6520 6f66 2074  is the name of t
+0001c3d0: 6865 2066 756e 6374 696f 6e2c 2060 3c63  he function, `<c
+0001c3e0: 6f6e 643e 6020 6973 2061 6e20 6f70 7469  ond>` is an opti
+0001c3f0: 6f6e 616c 2061 6464 6974 696f 6e61 6c20  onal additional 
+0001c400: 6368 6563 6b2c 2060 3c62 6f64 793e 6020  check, `<body>` 
+0001c410: 6973 2074 6865 2062 6f64 7920 6f66 2074  is the body of t
+0001c420: 6865 2066 756e 6374 696f 6e2c 2060 3c70  he function, `<p
+0001c430: 6174 7465 726e 3e60 2069 7320 6465 6669  attern>` is defi
+0001c440: 6e65 6420 6279 2043 6f63 6f6e 7574 2773  ned by Coconut's
+0001c450: 205b 606d 6174 6368 6020 7374 6174 656d   [`match` statem
+0001c460: 656e 745d 2823 6d61 7463 6829 2c20 603c  ent](#match), `<
+0001c470: 6465 6661 756c 743e 6020 6973 2074 6865  default>` is the
+0001c480: 206f 7074 696f 6e61 6c20 6465 6661 756c   optional defaul
+0001c490: 7420 6966 206e 6f20 6172 6775 6d65 6e74  t if no argument
+0001c4a0: 2069 7320 7061 7373 6564 2c20 616e 6420   is passed, and 
+0001c4b0: 603c 7265 7475 726e 5f74 7970 653e 6020  `<return_type>` 
+0001c4c0: 6973 2074 6865 206f 7074 696f 6e61 6c20  is the optional 
+0001c4d0: 7265 7475 726e 2074 7970 6520 616e 6e6f  return type anno
+0001c4e0: 7461 7469 6f6e 2028 6e6f 7465 2074 6861  tation (note tha
+0001c4f0: 7420 6172 6775 6d65 6e74 2074 7970 6520  t argument type 
+0001c500: 616e 6e6f 7461 7469 6f6e 7320 6172 6520  annotations are 
+0001c510: 6e6f 7420 7375 7070 6f72 7465 6420 666f  not supported fo
+0001c520: 7220 7061 7474 6572 6e2d 6d61 7463 6869  r pattern-matchi
+0001c530: 6e67 2066 756e 6374 696f 6e73 292e 2054  ng functions). T
+0001c540: 6865 2060 6d61 7463 6860 206b 6579 776f  he `match` keywo
+0001c550: 7264 2061 7420 7468 6520 6265 6769 6e6e  rd at the beginn
+0001c560: 696e 6720 6973 206f 7074 696f 6e61 6c2c  ing is optional,
+0001c570: 2062 7574 2069 7320 736f 6d65 7469 6d65   but is sometime
+0001c580: 7320 6e65 6365 7373 6172 7920 746f 2064  s necessary to d
+0001c590: 6973 616d 6269 6775 6174 6520 7061 7474  isambiguate patt
+0001c5a0: 6572 6e2d 6d61 7463 6869 6e67 2066 756e  ern-matching fun
+0001c5b0: 6374 696f 6e20 6465 6669 6e69 7469 6f6e  ction definition
+0001c5c0: 2066 726f 6d20 6e6f 726d 616c 2066 756e   from normal fun
+0001c5d0: 6374 696f 6e20 6465 6669 6e69 7469 6f6e  ction definition
+0001c5e0: 2c20 7369 6e63 6520 5079 7468 6f6e 2066  , since Python f
+0001c5f0: 756e 6374 696f 6e20 6465 6669 6e69 7469  unction definiti
+0001c600: 6f6e 2077 696c 6c20 616c 7761 7973 2074  on will always t
+0001c610: 616b 6520 7072 6563 6564 656e 6365 2e20  ake precedence. 
+0001c620: 4e6f 7465 2074 6861 7420 7468 6520 6061  Note that the `a
+0001c630: 7379 6e63 6020 616e 6420 606d 6174 6368  sync` and `match
+0001c640: 6020 6b65 7977 6f72 6473 2063 616e 2062  ` keywords can b
+0001c650: 6520 696e 2061 6e79 206f 7264 6572 2e0a  e in any order..
+0001c660: 0a49 6620 603c 7061 7474 6572 6e3e 6020  .If `<pattern>` 
+0001c670: 6861 7320 6120 7661 7269 6162 6c65 206e  has a variable n
+0001c680: 616d 6520 2865 6974 6865 7220 6469 7265  ame (either dire
+0001c690: 6374 6c79 206f 7220 7769 7468 2060 6173  ctly or with `as
+0001c6a0: 6029 2c20 7468 6520 7265 7375 6c74 696e  `), the resultin
+0001c6b0: 6720 7061 7474 6572 6e2d 6d61 7463 6869  g pattern-matchi
+0001c6c0: 6e67 2066 756e 6374 696f 6e20 7769 6c6c  ng function will
+0001c6d0: 2073 7570 706f 7274 206b 6579 776f 7264   support keyword
+0001c6e0: 2061 7267 756d 656e 7473 2075 7369 6e67   arguments using
+0001c6f0: 2074 6861 7420 7661 7269 6162 6c65 206e   that variable n
+0001c700: 616d 652e 0a0a 496e 2061 6464 6974 696f  ame...In additio
+0001c710: 6e20 746f 2073 7570 706f 7274 696e 6720  n to supporting 
+0001c720: 7061 7474 6572 6e2d 6d61 7463 6869 6e67  pattern-matching
+0001c730: 2069 6e20 7468 6569 7220 6172 6775 6d65   in their argume
+0001c740: 6e74 732c 2070 6174 7465 726e 2d6d 6174  nts, pattern-mat
+0001c750: 6368 696e 6720 6675 6e63 7469 6f6e 2064  ching function d
+0001c760: 6566 696e 6974 696f 6e73 2061 6c73 6f20  efinitions also 
+0001c770: 6861 7665 2061 2063 6f75 706c 6520 6f66  have a couple of
+0001c780: 206e 6f74 6162 6c65 2064 6966 6665 7265   notable differe
+0001c790: 6e63 6573 2063 6f6d 7061 7265 6420 746f  nces compared to
+0001c7a0: 2050 7974 686f 6e20 6675 6e63 7469 6f6e   Python function
+0001c7b0: 732e 2053 7065 6369 6669 6361 6c6c 793a  s. Specifically:
+0001c7c0: 0a2d 2049 6620 7061 7474 6572 6e2d 6d61  .- If pattern-ma
+0001c7d0: 7463 6869 6e67 2066 756e 6374 696f 6e20  tching function 
+0001c7e0: 6465 6669 6e69 7469 6f6e 2066 6169 6c73  definition fails
+0001c7f0: 2c20 6974 2077 696c 6c20 7261 6973 6520  , it will raise 
+0001c800: 6120 5b60 4d61 7463 6845 7272 6f72 605d  a [`MatchError`]
+0001c810: 2823 6d61 7463 6865 7272 6f72 2920 286a  (#matcherror) (j
+0001c820: 7573 7420 6c69 6b65 205b 6465 7374 7275  ust like [destru
+0001c830: 6374 7572 696e 6720 6173 7369 676e 6d65  cturing assignme
+0001c840: 6e74 5d28 2364 6573 7472 7563 7475 7269  nt](#destructuri
+0001c850: 6e67 2d61 7373 6967 6e6d 656e 7429 2920  ng-assignment)) 
+0001c860: 696e 7374 6561 6420 6f66 2061 2060 5479  instead of a `Ty
+0001c870: 7065 4572 726f 7260 2e0a 2d20 416c 6c20  peError`..- All 
+0001c880: 6465 6661 756c 7473 2069 6e20 7061 7474  defaults in patt
+0001c890: 6572 6e2d 6d61 7463 6869 6e67 2066 756e  ern-matching fun
+0001c8a0: 6374 696f 6e20 6465 6669 6e69 7469 6f6e  ction definition
+0001c8b0: 2061 7265 206c 6174 652d 626f 756e 6420   are late-bound 
+0001c8c0: 7261 7468 6572 2074 6861 6e20 6561 726c  rather than earl
+0001c8d0: 792d 626f 756e 642e 2054 6875 732c 2060  y-bound. Thus, `
+0001c8e0: 6d61 7463 6820 6465 6620 6628 7873 3d5b  match def f(xs=[
+0001c8f0: 5d29 203d 2078 7360 2077 696c 6c20 696e  ]) = xs` will in
+0001c900: 7374 616e 7469 6174 6520 6120 6e65 7720  stantiate a new 
+0001c910: 6c69 7374 2066 6f72 2065 6163 6820 6361  list for each ca
+0001c920: 6c6c 2077 6865 7265 2060 7873 6020 6973  ll where `xs` is
+0001c930: 206e 6f74 2067 6976 656e 2c20 756e 6c69   not given, unli
+0001c940: 6b65 2060 6465 6620 6628 7873 3d5b 5d29  ke `def f(xs=[])
+0001c950: 203d 2078 7360 2c20 7768 6963 6820 7769   = xs`, which wi
+0001c960: 6c6c 2075 7365 2074 6865 2073 616d 6520  ll use the same 
+0001c970: 6c69 7374 2066 6f72 2061 6c6c 2063 616c  list for all cal
+0001c980: 6c73 2077 6865 7265 2060 7873 6020 6973  ls where `xs` is
+0001c990: 2075 6e73 7065 6369 6669 6564 2e0a 0a50   unspecified...P
+0001c9a0: 6174 7465 726e 2d6d 6174 6368 696e 6720  attern-matching 
+0001c9b0: 6675 6e63 7469 6f6e 2064 6566 696e 6974  function definit
+0001c9c0: 696f 6e20 6361 6e20 616c 736f 2062 6520  ion can also be 
+0001c9d0: 636f 6d62 696e 6564 2077 6974 6820 6061  combined with `a
+0001c9e0: 7379 6e63 6020 6675 6e63 7469 6f6e 732c  sync` functions,
+0001c9f0: 205b 6063 6f70 7963 6c6f 7375 7265 6020   [`copyclosure` 
+0001ca00: 6675 6e63 7469 6f6e 735d 2823 636f 7079  functions](#copy
+0001ca10: 636c 6f73 7572 652d 6675 6e63 7469 6f6e  closure-function
+0001ca20: 7329 2c20 5b60 7969 656c 6460 2066 756e  s), [`yield` fun
+0001ca30: 6374 696f 6e73 5d28 2365 7870 6c69 6369  ctions](#explici
+0001ca40: 742d 6765 6e65 7261 746f 7273 292c 205b  t-generators), [
+0001ca50: 696e 6669 7820 6675 6e63 7469 6f6e 2064  infix function d
+0001ca60: 6566 696e 6974 696f 6e5d 2823 696e 6669  efinition](#infi
+0001ca70: 782d 6675 6e63 7469 6f6e 7329 2c20 616e  x-functions), an
+0001ca80: 6420 5b61 7373 6967 6e6d 656e 7420 6675  d [assignment fu
+0001ca90: 6e63 7469 6f6e 2073 796e 7461 785d 2823  nction syntax](#
+0001caa0: 6173 7369 676e 6d65 6e74 2d66 756e 6374  assignment-funct
+0001cab0: 696f 6e73 292e 2054 6865 2076 6172 696f  ions). The vario
+0001cac0: 7573 206b 6579 776f 7264 7320 696e 2066  us keywords in f
+0001cad0: 726f 6e74 206f 6620 7468 6520 6064 6566  ront of the `def
+0001cae0: 6020 6361 6e20 6265 2070 7574 2069 6e20  ` can be put in 
+0001caf0: 616e 7920 6f72 6465 722e 0a0a 2323 2323  any order...####
+0001cb00: 2320 4578 616d 706c 650a 0a2a 2a43 6f63  # Example..**Coc
+0001cb10: 6f6e 7574 3a2a 2a0a 6060 6063 6f63 6f6e  onut:**.```cocon
+0001cb20: 7574 0a64 6566 206c 6173 745f 7477 6f28  ut.def last_two(
+0001cb30: 5f20 2b20 5b61 2c20 625d 293a 0a20 2020  _ + [a, b]):.   
+0001cb40: 2072 6574 7572 6e20 612c 2062 0a64 6566   return a, b.def
+0001cb50: 2078 7964 6963 745f 746f 5f78 7974 7570   xydict_to_xytup
+0001cb60: 6c65 287b 2278 223a 2078 2060 6973 696e  le({"x": x `isin
+0001cb70: 7374 616e 6365 6020 696e 742c 2022 7922  stance` int, "y"
+0001cb80: 3a20 7920 6069 7369 6e73 7461 6e63 6560  : y `isinstance`
+0001cb90: 2069 6e74 7d29 3a0a 2020 2020 7265 7475   int}):.    retu
+0001cba0: 726e 2078 2c20 790a 0a72 616e 6765 2835  rn x, y..range(5
+0001cbb0: 2920 7c3e 206c 6173 745f 7477 6f20 7c3e  ) |> last_two |>
+0001cbc0: 2070 7269 6e74 0a7b 2278 223a 312c 2022   print.{"x":1, "
+0001cbd0: 7922 3a32 7d20 7c3e 2078 7964 6963 745f  y":2} |> xydict_
+0001cbe0: 746f 5f78 7974 7570 6c65 207c 3e20 7072  to_xytuple |> pr
+0001cbf0: 696e 740a 6060 600a 0a2a 2a50 7974 686f  int.```..**Pytho
+0001cc00: 6e3a 2a2a 0a5f 4361 6e27 7420 6265 2064  n:**._Can't be d
+0001cc10: 6f6e 6520 7769 7468 6f75 7420 6120 6c6f  one without a lo
+0001cc20: 6e67 2073 6572 6965 7320 6f66 2063 6865  ng series of che
+0001cc30: 636b 7320 6174 2074 6865 2074 6f70 206f  cks at the top o
+0001cc40: 6620 7468 6520 6675 6e63 7469 6f6e 2e20  f the function. 
+0001cc50: 5365 6520 7468 6520 636f 6d70 696c 6564  See the compiled
+0001cc60: 2063 6f64 6520 666f 7220 7468 6520 5079   code for the Py
+0001cc70: 7468 6f6e 2073 796e 7461 782e 5f0a 0a23  thon syntax._..#
+0001cc80: 2323 2060 6164 6470 6174 7465 726e 6020  ## `addpattern` 
+0001cc90: 4675 6e63 7469 6f6e 730a 0a43 6f63 6f6e  Functions..Cocon
+0001cca0: 7574 2070 726f 7669 6465 7320 7468 6520  ut provides the 
+0001ccb0: 6061 6464 7061 7474 6572 6e20 6465 6660  `addpattern def`
+0001ccc0: 2073 796e 7461 7820 6173 2061 2073 686f   syntax as a sho
+0001ccd0: 7274 6375 7420 666f 7220 7468 6520 6675  rtcut for the fu
+0001cce0: 6c6c 0a60 6060 636f 636f 6e75 740a 4061  ll.```coconut.@a
+0001ccf0: 6464 7061 7474 6572 6e28 6675 6e63 290a  ddpattern(func).
+0001cd00: 6d61 7463 6820 6465 6620 6675 6e63 282e  match def func(.
+0001cd10: 2e2e 293a 0a20 202e 2e2e 0a60 6060 0a73  ..):.  ....```.s
+0001cd20: 796e 7461 7820 7573 696e 6720 7468 6520  yntax using the 
+0001cd30: 5b60 6164 6470 6174 7465 726e 605d 2823  [`addpattern`](#
+0001cd40: 6164 6470 6174 7465 726e 2920 6465 636f  addpattern) deco
+0001cd50: 7261 746f 722e 0a0a 4164 6469 7469 6f6e  rator...Addition
+0001cd60: 616c 6c79 2c20 6061 6464 7061 7474 6572  ally, `addpatter
+0001cd70: 6e20 6465 6660 2077 696c 6c20 6163 7420  n def` will act 
+0001cd80: 6a75 7374 206c 696b 6520 6120 6e6f 726d  just like a norm
+0001cd90: 616c 205b 606d 6174 6368 2064 6566 605d  al [`match def`]
+0001cda0: 2823 7061 7474 6572 6e2d 6d61 7463 6869  (#pattern-matchi
+0001cdb0: 6e67 2d66 756e 6374 696f 6e73 2920 6966  ng-functions) if
+0001cdc0: 2074 6865 2066 756e 6374 696f 6e20 6861   the function ha
+0001cdd0: 7320 6e6f 7420 7072 6576 696f 7573 6c79  s not previously
+0001cde0: 2062 6565 6e20 6465 6669 6e65 642c 2061   been defined, a
+0001cdf0: 6c6c 6f77 696e 6720 666f 7220 6061 6464  llowing for `add
+0001ce00: 7061 7474 6572 6e20 6465 6660 2074 6f20  pattern def` to 
+0001ce10: 6265 2075 7365 6420 666f 7220 6561 6368  be used for each
+0001ce20: 2063 6173 6520 7261 7468 6572 2074 6861   case rather tha
+0001ce30: 6e20 7265 7175 6972 696e 6720 606d 6174  n requiring `mat
+0001ce40: 6368 2064 6566 6020 666f 7220 7468 6520  ch def` for the 
+0001ce50: 6669 7273 7420 6361 7365 2061 6e64 2060  first case and `
+0001ce60: 6164 6470 6174 7465 726e 2064 6566 6020  addpattern def` 
+0001ce70: 666f 7220 6675 7475 7265 2063 6173 6573  for future cases
+0001ce80: 2e0a 0a49 6620 796f 7520 7761 6e74 2074  ...If you want t
+0001ce90: 6f20 7075 7420 6120 6465 636f 7261 746f  o put a decorato
+0001cea0: 7220 6f6e 2061 6e20 6061 6464 7061 7474  r on an `addpatt
+0001ceb0: 6572 6e20 6465 6660 2066 756e 6374 696f  ern def` functio
+0001cec0: 6e2c 206d 616b 6520 7375 7265 2074 6f20  n, make sure to 
+0001ced0: 7075 7420 6974 206f 6e20 7468 6520 5f6c  put it on the _l
+0001cee0: 6173 745f 2070 6174 7465 726e 2066 756e  ast_ pattern fun
+0001cef0: 6374 696f 6e2e 0a0a 2323 2323 2320 4578  ction...##### Ex
+0001cf00: 616d 706c 650a 0a2a 2a43 6f63 6f6e 7574  ample..**Coconut
+0001cf10: 3a2a 2a0a 6060 6063 6f63 6f6e 7574 0a61  :**.```coconut.a
+0001cf20: 6464 7061 7474 6572 6e20 6465 6620 6661  ddpattern def fa
+0001cf30: 6374 6f72 6961 6c28 3029 203d 2031 0a61  ctorial(0) = 1.a
+0001cf40: 6464 7061 7474 6572 6e20 6465 6620 6661  ddpattern def fa
+0001cf50: 6374 6f72 6961 6c28 6e29 203d 206e 202a  ctorial(n) = n *
+0001cf60: 2066 6163 746f 7269 616c 286e 202d 2031   factorial(n - 1
+0001cf70: 290a 6060 600a 0a2a 2a50 7974 686f 6e3a  ).```..**Python:
+0001cf80: 2a2a 0a5f 4361 6e27 7420 6265 2064 6f6e  **._Can't be don
+0001cf90: 6520 7769 7468 6f75 7420 6120 636f 6d70  e without a comp
+0001cfa0: 6c69 6361 7465 6420 6465 636f 7261 746f  licated decorato
+0001cfb0: 7220 6465 6669 6e69 7469 6f6e 2061 6e64  r definition and
+0001cfc0: 2061 206c 6f6e 6720 7365 7269 6573 206f   a long series o
+0001cfd0: 6620 6368 6563 6b73 2066 6f72 2065 6163  f checks for eac
+0001cfe0: 6820 7061 7474 6572 6e2d 6d61 7463 6869  h pattern-matchi
+0001cff0: 6e67 2e20 5365 6520 7468 6520 636f 6d70  ng. See the comp
+0001d000: 696c 6564 2063 6f64 6520 666f 7220 7468  iled code for th
+0001d010: 6520 5079 7468 6f6e 2073 796e 7461 782e  e Python syntax.
+0001d020: 5f0a 0a23 2323 2060 636f 7079 636c 6f73  _..### `copyclos
+0001d030: 7572 6560 2046 756e 6374 696f 6e73 0a0a  ure` Functions..
+0001d040: 436f 636f 6e75 7420 7375 7070 6f72 7473  Coconut supports
+0001d050: 2074 6865 2073 796e 7461 780a 6060 600a   the syntax.```.
+0001d060: 636f 7079 636c 6f73 7572 6520 6465 6620  copyclosure def 
+0001d070: 3c6e 616d 653e 283c 6172 6773 3e29 3a0a  <name>(<args>):.
+0001d080: 2020 2020 3c62 6f64 793e 0a60 6060 0a74      <body>.```.t
+0001d090: 6f20 6465 6669 6e65 2061 2066 756e 6374  o define a funct
+0001d0a0: 696f 6e20 7468 6174 2075 7365 7320 6173  ion that uses as
+0001d0b0: 2069 7473 2063 6c6f 7375 7265 2061 2073   its closure a s
+0001d0c0: 6861 6c6c 6f77 2063 6f70 7920 6f66 2069  hallow copy of i
+0001d0d0: 7473 2065 6e63 6c6f 7369 6e67 2073 636f  ts enclosing sco
+0001d0e0: 7065 7320 6174 2074 6865 2074 696d 6520  pes at the time 
+0001d0f0: 7468 6174 2074 6865 2066 756e 6374 696f  that the functio
+0001d100: 6e20 6973 2064 6566 696e 6564 2c20 7261  n is defined, ra
+0001d110: 7468 6572 2074 6861 6e20 6120 7265 6665  ther than a refe
+0001d120: 7265 6e63 6520 746f 2074 686f 7365 2073  rence to those s
+0001d130: 636f 7065 7320 2861 7320 7769 7468 206e  copes (as with n
+0001d140: 6f72 6d61 6c20 5079 7468 6f6e 2066 756e  ormal Python fun
+0001d150: 6374 696f 6e73 292e 0a0a 466f 7220 6578  ctions)...For ex
+0001d160: 616d 706c 652c 6069 6e0a 6060 6063 6f63  ample,`in.```coc
+0001d170: 6f6e 7574 0a64 6566 206f 7574 6572 5f66  onut.def outer_f
+0001d180: 756e 6328 293a 0a20 2020 2066 756e 6373  unc():.    funcs
+0001d190: 203d 205b 5d0a 2020 2020 666f 7220 7820   = [].    for x 
+0001d1a0: 696e 2072 616e 6765 2831 3029 3a0a 2020  in range(10):.  
+0001d1b0: 2020 2020 2020 636f 7079 636c 6f73 7572        copyclosur
+0001d1c0: 6520 6465 6620 696e 6e65 725f 6675 6e63  e def inner_func
+0001d1d0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0001d1e0: 7265 7475 726e 2078 0a20 2020 2020 2020  return x.       
+0001d1f0: 2066 756e 6373 2e61 7070 656e 6428 696e   funcs.append(in
+0001d200: 6e65 725f 6675 6e63 290a 2020 2020 7265  ner_func).    re
+0001d210: 7475 726e 2066 756e 6373 0a60 6060 0a74  turn funcs.```.t
+0001d220: 6865 2072 6573 756c 7469 6e67 2060 696e  he resulting `in
+0001d230: 6e65 725f 6675 6e63 6073 2077 696c 6c20  ner_func`s will 
+0001d240: 6561 6368 2072 6574 7572 6e20 6120 5f64  each return a _d
+0001d250: 6966 6665 7265 6e74 5f20 6078 6020 7661  ifferent_ `x` va
+0001d260: 6c75 6520 7261 7468 6572 2074 6861 6e20  lue rather than 
+0001d270: 616c 6c20 7468 6520 7361 6d65 2060 7860  all the same `x`
+0001d280: 2076 616c 7565 2c20 7369 6e63 6520 7468   value, since th
+0001d290: 6579 206c 6f6f 6b20 6174 2077 6861 7420  ey look at what 
+0001d2a0: 6078 6020 7761 7320 626f 756e 6420 746f  `x` was bound to
+0001d2b0: 2061 7420 6675 6e63 7469 6f6e 2064 6566   at function def
+0001d2c0: 696e 6974 696f 6e20 7469 6d65 2072 6174  inition time rat
+0001d2d0: 6865 7220 7468 616e 2064 7572 696e 6720  her than during 
+0001d2e0: 6675 6e63 7469 6f6e 2065 7865 6375 7469  function executi
+0001d2f0: 6f6e 2e0a 0a60 636f 7079 636c 6f73 7572  on...`copyclosur
+0001d300: 6560 2066 756e 6374 696f 6e73 2063 616e  e` functions can
+0001d310: 2061 6c73 6f20 6265 2063 6f6d 6269 6e65   also be combine
+0001d320: 6420 7769 7468 2060 6173 796e 6360 2066  d with `async` f
+0001d330: 756e 6374 696f 6e73 2c20 5b60 7969 656c  unctions, [`yiel
+0001d340: 6460 2066 756e 6374 696f 6e73 5d28 2365  d` functions](#e
+0001d350: 7870 6c69 6369 742d 6765 6e65 7261 746f  xplicit-generato
+0001d360: 7273 292c 205b 7061 7474 6572 6e2d 6d61  rs), [pattern-ma
+0001d370: 7463 6869 6e67 2066 756e 6374 696f 6e73  tching functions
+0001d380: 5d28 2370 6174 7465 726e 2d6d 6174 6368  ](#pattern-match
+0001d390: 696e 672d 6675 6e63 7469 6f6e 7329 2c20  ing-functions), 
+0001d3a0: 5b69 6e66 6978 2066 756e 6374 696f 6e20  [infix function 
+0001d3b0: 6465 6669 6e69 7469 6f6e 5d28 2369 6e66  definition](#inf
+0001d3c0: 6978 2d66 756e 6374 696f 6e73 292c 2061  ix-functions), a
+0001d3d0: 6e64 205b 6173 7369 676e 6d65 6e74 2066  nd [assignment f
+0001d3e0: 756e 6374 696f 6e20 7379 6e74 6178 5d28  unction syntax](
+0001d3f0: 2361 7373 6967 6e6d 656e 742d 6675 6e63  #assignment-func
+0001d400: 7469 6f6e 7329 2e20 5468 6520 7661 7269  tions). The vari
+0001d410: 6f75 7320 6b65 7977 6f72 6473 2069 6e20  ous keywords in 
+0001d420: 6672 6f6e 7420 6f66 2074 6865 2060 6465  front of the `de
+0001d430: 6660 2063 616e 2062 6520 7075 7420 696e  f` can be put in
+0001d440: 2061 6e79 206f 7264 6572 2e0a 0a49 6620   any order...If 
+0001d450: 6067 6c6f 6261 6c60 206f 7220 606e 6f6e  `global` or `non
+0001d460: 6c6f 6361 6c60 2061 7265 2075 7365 6420  local` are used 
+0001d470: 696e 2061 2060 636f 7079 636c 6f73 7572  in a `copyclosur
+0001d480: 6560 2066 756e 6374 696f 6e2c 2074 6865  e` function, the
+0001d490: 7920 7769 6c6c 206e 6f74 2062 6520 6162  y will not be ab
+0001d4a0: 6c65 2074 6f20 6d6f 6469 6679 2076 6172  le to modify var
+0001d4b0: 6961 626c 6573 2069 6e20 656e 636c 6f73  iables in enclos
+0001d4c0: 696e 6720 7363 6f70 6573 2e20 486f 7765  ing scopes. Howe
+0001d4d0: 7665 722c 2074 6865 7920 7769 6c6c 2061  ver, they will a
+0001d4e0: 6c6c 6f77 2073 7461 7465 2074 6f20 6265  llow state to be
+0001d4f0: 2070 7265 7365 7276 6564 2061 6363 726f   preserved accro
+0001d500: 7373 206d 756c 7469 706c 6520 6361 6c6c  ss multiple call
+0001d510: 7320 746f 2074 6865 2060 636f 7079 636c  s to the `copycl
+0001d520: 6f73 7572 6560 2066 756e 6374 696f 6e2e  osure` function.
+0001d530: 0a0a 2323 2323 2320 4578 616d 706c 650a  ..##### Example.
+0001d540: 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a 6060  .**Coconut:**.``
+0001d550: 6063 6f63 6f6e 7574 0a64 6566 206f 7574  `coconut.def out
+0001d560: 6572 5f66 756e 6328 293a 0a20 2020 2066  er_func():.    f
+0001d570: 756e 6373 203d 205b 5d0a 2020 2020 666f  uncs = [].    fo
+0001d580: 7220 7820 696e 2072 616e 6765 2831 3029  r x in range(10)
+0001d590: 3a0a 2020 2020 2020 2020 636f 7079 636c  :.        copycl
+0001d5a0: 6f73 7572 6520 6465 6620 696e 6e65 725f  osure def inner_
+0001d5b0: 6675 6e63 2829 3a0a 2020 2020 2020 2020  func():.        
+0001d5c0: 2020 2020 7265 7475 726e 2078 0a20 2020      return x.   
+0001d5d0: 2020 2020 2066 756e 6373 2e61 7070 656e       funcs.appen
+0001d5e0: 6428 696e 6e65 725f 6675 6e63 290a 2020  d(inner_func).  
+0001d5f0: 2020 7265 7475 726e 2066 756e 6373 0a60    return funcs.`
+0001d600: 6060 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a  ``..**Python:**.
+0001d610: 6060 6063 6f63 6f6e 7574 5f70 7974 686f  ```coconut_pytho
+0001d620: 6e0a 6672 6f6d 2066 756e 6374 6f6f 6c73  n.from functools
+0001d630: 2069 6d70 6f72 7420 7061 7274 6961 6c0a   import partial.
+0001d640: 0a64 6566 206f 7574 6572 5f66 756e 6328  .def outer_func(
+0001d650: 293a 0a20 2020 2066 756e 6373 203d 205b  ):.    funcs = [
+0001d660: 5d0a 2020 2020 666f 7220 7820 696e 2072  ].    for x in r
+0001d670: 616e 6765 2831 3029 3a0a 2020 2020 2020  ange(10):.      
+0001d680: 2020 6465 6620 696e 6e65 725f 6675 6e63    def inner_func
+0001d690: 285f 7829 3a0a 2020 2020 2020 2020 2020  (_x):.          
+0001d6a0: 2020 7265 7475 726e 205f 780a 2020 2020    return _x.    
+0001d6b0: 2020 2020 6675 6e63 732e 6170 7065 6e64      funcs.append
+0001d6c0: 2870 6172 7469 616c 2869 6e6e 6572 5f66  (partial(inner_f
+0001d6d0: 756e 632c 2078 2929 0a20 2020 2072 6574  unc, x)).    ret
+0001d6e0: 7572 6e20 6675 6e63 730a 6060 600a 0a23  urn funcs.```..#
+0001d6f0: 2323 2045 7870 6c69 6369 7420 4765 6e65  ## Explicit Gene
+0001d700: 7261 746f 7273 0a0a 436f 636f 6e75 7420  rators..Coconut 
+0001d710: 7375 7070 6f72 7473 2074 6865 2073 796e  supports the syn
+0001d720: 7461 780a 6060 600a 7969 656c 6420 6465  tax.```.yield de
+0001d730: 6620 3c6e 616d 653e 283c 6172 6773 3e29  f <name>(<args>)
+0001d740: 3a0a 2020 2020 3c62 6f64 793e 0a60 6060  :.    <body>.```
+0001d750: 0a74 6f20 6465 6e6f 7465 2074 6861 7420  .to denote that 
+0001d760: 796f 7520 6172 6520 6578 706c 6963 6974  you are explicit
+0001d770: 6c79 2064 6566 696e 696e 6720 6120 6765  ly defining a ge
+0001d780: 6e65 7261 746f 7220 6675 6e63 7469 6f6e  nerator function
+0001d790: 2e20 5468 6973 2069 7320 7573 6566 756c  . This is useful
+0001d7a0: 2074 6f20 656e 7375 7265 2074 6861 742c   to ensure that,
+0001d7b0: 2065 7665 6e20 6966 2061 6c6c 2074 6865   even if all the
+0001d7c0: 2060 7969 656c 6460 7320 696e 2079 6f75   `yield`s in you
+0001d7d0: 7220 6675 6e63 7469 6f6e 2061 7265 2072  r function are r
+0001d7e0: 656d 6f76 6564 2c20 6974 276c 6c20 616c  emoved, it'll al
+0001d7f0: 7761 7973 2062 6520 6120 6765 6e65 7261  ways be a genera
+0001d800: 746f 7220 6675 6e63 7469 6f6e 2e0a 0a45  tor function...E
+0001d810: 7870 6c69 6369 7420 6765 6e65 7261 746f  xplicit generato
+0001d820: 7220 6675 6e63 7469 6f6e 7320 6361 6e20  r functions can 
+0001d830: 616c 736f 2062 6520 636f 6d62 696e 6564  also be combined
+0001d840: 2077 6974 6820 6061 7379 6e63 6020 6675   with `async` fu
+0001d850: 6e63 7469 6f6e 732c 205b 6063 6f70 7963  nctions, [`copyc
+0001d860: 6c6f 7375 7265 6020 6675 6e63 7469 6f6e  losure` function
+0001d870: 735d 2823 636f 7079 636c 6f73 7572 652d  s](#copyclosure-
+0001d880: 6675 6e63 7469 6f6e 7329 2c20 5b70 6174  functions), [pat
+0001d890: 7465 726e 2d6d 6174 6368 696e 6720 6675  tern-matching fu
+0001d8a0: 6e63 7469 6f6e 735d 2823 7061 7474 6572  nctions](#patter
+0001d8b0: 6e2d 6d61 7463 6869 6e67 2d66 756e 6374  n-matching-funct
+0001d8c0: 696f 6e73 292c 205b 696e 6669 7820 6675  ions), [infix fu
+0001d8d0: 6e63 7469 6f6e 2064 6566 696e 6974 696f  nction definitio
+0001d8e0: 6e5d 2823 696e 6669 782d 6675 6e63 7469  n](#infix-functi
+0001d8f0: 6f6e 7329 2c20 616e 6420 5b61 7373 6967  ons), and [assig
+0001d900: 6e6d 656e 7420 6675 6e63 7469 6f6e 2073  nment function s
+0001d910: 796e 7461 785d 2823 6173 7369 676e 6d65  yntax](#assignme
+0001d920: 6e74 2d66 756e 6374 696f 6e73 2920 2874  nt-functions) (t
+0001d930: 686f 7567 6820 6e6f 7465 2074 6861 7420  hough note that 
+0001d940: 6173 7369 676e 6d65 6e74 2066 756e 6374  assignment funct
+0001d950: 696f 6e20 7379 6e74 6178 2068 6572 6520  ion syntax here 
+0001d960: 6372 6561 7465 7320 6120 6765 6e65 7261  creates a genera
+0001d970: 746f 7220 7265 7475 726e 292e 2054 6865  tor return). The
+0001d980: 2076 6172 696f 7573 206b 6579 776f 7264   various keyword
+0001d990: 7320 696e 2066 726f 6e74 206f 6620 7468  s in front of th
+0001d9a0: 6520 6064 6566 6020 6361 6e20 6265 2070  e `def` can be p
+0001d9b0: 7574 2069 6e20 616e 7920 6f72 6465 722e  ut in any order.
+0001d9c0: 0a0a 2323 2323 2320 4578 616d 706c 650a  ..##### Example.
+0001d9d0: 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a 6060  .**Coconut:**.``
+0001d9e0: 6063 6f63 6f6e 7574 0a79 6965 6c64 2064  `coconut.yield d
+0001d9f0: 6566 2065 6d70 7479 5f69 7428 293a 2070  ef empty_it(): p
+0001da00: 6173 730a 6060 600a 0a2a 2a50 7974 686f  ass.```..**Pytho
+0001da10: 6e3a 2a2a 0a60 6060 636f 636f 6e75 745f  n:**.```coconut_
+0001da20: 7079 7468 6f6e 0a64 6566 2065 6d70 7479  python.def empty
+0001da30: 5f69 7428 293a 0a20 2020 2069 6620 4661  _it():.    if Fa
+0001da40: 6c73 653a 0a20 2020 2020 2020 2079 6965  lse:.        yie
+0001da50: 6c64 0a60 6060 0a0a 2323 2320 446f 7474  ld.```..### Dott
+0001da60: 6564 2046 756e 6374 696f 6e20 4465 6669  ed Function Defi
+0001da70: 6e69 7469 6f6e 0a0a 436f 636f 6e75 7420  nition..Coconut 
+0001da80: 616c 6c6f 7773 2066 6f72 2066 756e 6374  allows for funct
+0001da90: 696f 6e20 6465 6669 6e69 7469 6f6e 2075  ion definition u
+0001daa0: 7369 6e67 2061 2064 6f74 7465 6420 6e61  sing a dotted na
+0001dab0: 6d65 2074 6f20 6173 7369 676e 2061 2066  me to assign a f
+0001dac0: 756e 6374 696f 6e20 6173 2061 206d 6574  unction as a met
+0001dad0: 686f 6420 6f66 2061 6e20 6f62 6a65 6374  hod of an object
+0001dae0: 2061 7320 7370 6563 6966 6965 6420 696e   as specified in
+0001daf0: 205b 5045 5020 3534 325d 2868 7474 7073   [PEP 542](https
+0001db00: 3a2f 2f77 7777 2e70 7974 686f 6e2e 6f72  ://www.python.or
+0001db10: 672f 6465 762f 7065 7073 2f70 6570 2d30  g/dev/peps/pep-0
+0001db20: 3534 322f 292e 2044 6f74 7465 6420 6675  542/). Dotted fu
+0001db30: 6e63 7469 6f6e 2064 6566 696e 6974 696f  nction definitio
+0001db40: 6e20 6361 6e20 6265 2063 6f6d 6269 6e65  n can be combine
+0001db50: 6420 7769 7468 2061 6c6c 206f 7468 6572  d with all other
+0001db60: 2074 7970 6573 206f 6620 6675 6e63 7469   types of functi
+0001db70: 6f6e 2064 6566 696e 6974 696f 6e20 6162  on definition ab
+0001db80: 6f76 652e 0a0a 2323 2323 2320 4578 616d  ove...##### Exam
+0001db90: 706c 650a 0a2a 2a43 6f63 6f6e 7574 3a2a  ple..**Coconut:*
+0001dba0: 2a0a 6060 6063 6f63 6f6e 7574 0a64 6566  *.```coconut.def
+0001dbb0: 204d 7943 6c61 7373 2e6d 795f 6d65 7468   MyClass.my_meth
+0001dbc0: 6f64 2873 656c 6629 3a0a 2020 2020 2e2e  od(self):.    ..
+0001dbd0: 2e0a 6060 600a 0a2a 2a50 7974 686f 6e3a  ..```..**Python:
+0001dbe0: 2a2a 0a60 6060 636f 636f 6e75 745f 7079  **.```coconut_py
+0001dbf0: 7468 6f6e 0a64 6566 206d 795f 6d65 7468  thon.def my_meth
+0001dc00: 6f64 2873 656c 6629 3a0a 2020 2020 2e2e  od(self):.    ..
+0001dc10: 2e0a 4d79 436c 6173 732e 6d79 5f6d 6574  ..MyClass.my_met
+0001dc20: 686f 6420 3d20 6d79 5f6d 6574 686f 640a  hod = my_method.
+0001dc30: 6060 600a 0a23 2320 5374 6174 656d 656e  ```..## Statemen
+0001dc40: 7473 0a0a 6060 607b 636f 6e74 656e 7473  ts..```{contents
+0001dc50: 7d0a 2d2d 2d0a 6c6f 6361 6c3a 0a64 6570  }.---.local:.dep
+0001dc60: 7468 3a20 310a 2d2d 2d0a 6060 600a 0a23  th: 1.---.```..#
+0001dc70: 2323 2044 6573 7472 7563 7475 7269 6e67  ## Destructuring
+0001dc80: 2041 7373 6967 6e6d 656e 740a 0a43 6f63   Assignment..Coc
+0001dc90: 6f6e 7574 2073 7570 706f 7274 7320 7369  onut supports si
+0001dca0: 676e 6966 6963 616e 746c 7920 656e 6861  gnificantly enha
+0001dcb0: 6e63 6564 2064 6573 7472 7563 7475 7269  nced destructuri
+0001dcc0: 6e67 2061 7373 6967 6e6d 656e 742c 2073  ng assignment, s
+0001dcd0: 696d 696c 6172 2074 6f20 5079 7468 6f6e  imilar to Python
+0001dce0: 2773 2074 7570 6c65 2f6c 6973 7420 6465  's tuple/list de
+0001dcf0: 7374 7275 6374 7572 696e 672c 2062 7574  structuring, but
+0001dd00: 206d 7563 6820 6d6f 7265 2070 6f77 6572   much more power
+0001dd10: 6675 6c2e 2054 6865 2073 796e 7461 7820  ful. The syntax 
+0001dd20: 666f 7220 436f 636f 6e75 7427 7320 6465  for Coconut's de
+0001dd30: 7374 7275 6374 7572 696e 6720 6173 7369  structuring assi
+0001dd40: 676e 6d65 6e74 2069 730a 6060 6063 6f63  gnment is.```coc
+0001dd50: 6f6e 7574 0a5b 6d61 7463 685d 203c 7061  onut.[match] <pa
+0001dd60: 7474 6572 6e3e 203d 203c 7661 6c75 653e  ttern> = <value>
+0001dd70: 0a60 6060 0a77 6865 7265 2060 3c76 616c  .```.where `<val
+0001dd80: 7565 3e60 2069 7320 616e 7920 6578 7072  ue>` is any expr
+0001dd90: 6573 7369 6f6e 2061 6e64 2060 3c70 6174  ession and `<pat
+0001dda0: 7465 726e 3e60 2069 7320 6465 6669 6e65  tern>` is define
+0001ddb0: 6420 6279 2043 6f63 6f6e 7574 2773 205b  d by Coconut's [
+0001ddc0: 606d 6174 6368 6020 7374 6174 656d 656e  `match` statemen
+0001ddd0: 745d 2823 6d61 7463 6829 2e20 5468 6520  t](#match). The 
+0001dde0: 606d 6174 6368 6020 6b65 7977 6f72 6420  `match` keyword 
+0001ddf0: 6174 2074 6865 2062 6567 696e 6e69 6e67  at the beginning
+0001de00: 2069 7320 6f70 7469 6f6e 616c 2c20 6275   is optional, bu
+0001de10: 7420 6973 2073 6f6d 6574 696d 6573 206e  t is sometimes n
+0001de20: 6563 6573 7361 7279 2074 6f20 6469 7361  ecessary to disa
+0001de30: 6d62 6967 7561 7465 2064 6573 7472 7563  mbiguate destruc
+0001de40: 7475 7269 6e67 2061 7373 6967 6e6d 656e  turing assignmen
+0001de50: 7420 6672 6f6d 206e 6f72 6d61 6c20 6173  t from normal as
+0001de60: 7369 676e 6d65 6e74 2c20 7768 6963 6820  signment, which 
+0001de70: 7769 6c6c 2061 6c77 6179 7320 7461 6b65  will always take
+0001de80: 2070 7265 6365 6465 6e63 652e 2043 6f63   precedence. Coc
+0001de90: 6f6e 7574 2773 2064 6573 7472 7563 7475  onut's destructu
+0001dea0: 7269 6e67 2061 7373 6967 6e6d 656e 7420  ring assignment 
+0001deb0: 6973 2065 7175 6976 616c 656e 7420 746f  is equivalent to
+0001dec0: 2061 206d 6174 6368 2073 7461 7465 6d65   a match stateme
+0001ded0: 6e74 2074 6861 7420 666f 6c6c 6f77 7320  nt that follows 
+0001dee0: 7468 6520 7379 6e74 6178 3a0a 6060 6063  the syntax:.```c
+0001def0: 6f63 6f6e 7574 0a6d 6174 6368 203c 7061  oconut.match <pa
+0001df00: 7474 6572 6e3e 2069 6e20 3c76 616c 7565  ttern> in <value
+0001df10: 3e3a 0a20 2020 2070 6173 730a 656c 7365  >:.    pass.else
+0001df20: 3a0a 2020 2020 6572 7220 3d20 4d61 7463  :.    err = Matc
+0001df30: 6845 7272 6f72 283c 6572 726f 7220 6d65  hError(<error me
+0001df40: 7373 6167 653e 290a 2020 2020 6572 722e  ssage>).    err.
+0001df50: 7061 7474 6572 6e20 3d20 223c 7061 7474  pattern = "<patt
+0001df60: 6572 6e3e 220a 2020 2020 6572 722e 7661  ern>".    err.va
+0001df70: 6c75 6520 3d20 3c76 616c 7565 3e0a 2020  lue = <value>.  
+0001df80: 2020 7261 6973 6520 6572 720a 6060 600a    raise err.```.
+0001df90: 4966 2061 2064 6573 7472 7563 7475 7269  If a destructuri
+0001dfa0: 6e67 2061 7373 6967 6e6d 656e 7420 7374  ng assignment st
+0001dfb0: 6174 656d 656e 7420 6661 696c 732c 2074  atement fails, t
+0001dfc0: 6865 6e20 696e 7374 6561 6420 6f66 2063  hen instead of c
+0001dfd0: 6f6e 7469 6e75 696e 6720 6f6e 2061 7320  ontinuing on as 
+0001dfe0: 6966 2061 2060 6d61 7463 6860 2062 6c6f  if a `match` blo
+0001dff0: 636b 2068 6164 2066 6169 6c65 642c 2061  ck had failed, a
+0001e000: 205b 604d 6174 6368 4572 726f 7260 5d28   [`MatchError`](
+0001e010: 236d 6174 6368 6572 726f 7229 206f 626a  #matcherror) obj
+0001e020: 6563 7420 7769 6c6c 2062 6520 7261 6973  ect will be rais
+0001e030: 6564 2064 6573 6372 6962 696e 6720 7468  ed describing th
+0001e040: 6520 6661 696c 7572 652e 0a0a 2323 2323  e failure...####
+0001e050: 2320 4578 616d 706c 650a 0a2a 2a43 6f63  # Example..**Coc
+0001e060: 6f6e 7574 3a2a 2a0a 6060 6063 6f63 6f6e  onut:**.```cocon
+0001e070: 7574 0a5f 202b 205b 612c 2062 5d20 3d20  ut._ + [a, b] = 
+0001e080: 5b30 2c20 312c 2032 2c20 335d 0a70 7269  [0, 1, 2, 3].pri
+0001e090: 6e74 2861 2c20 6229 0a60 6060 0a0a 2a2a  nt(a, b).```..**
+0001e0a0: 5079 7468 6f6e 3a2a 2a0a 5f43 616e 2774  Python:**._Can't
+0001e0b0: 2062 6520 646f 6e65 2077 6974 686f 7574   be done without
+0001e0c0: 2061 206c 6f6e 6720 7365 7269 6573 206f   a long series o
+0001e0d0: 6620 6368 6563 6b73 2069 6e20 706c 6163  f checks in plac
+0001e0e0: 6520 6f66 2074 6865 2064 6573 7472 7563  e of the destruc
+0001e0f0: 7475 7269 6e67 2061 7373 6967 6e6d 656e  turing assignmen
+0001e100: 7420 7374 6174 656d 656e 742e 2053 6565  t statement. See
+0001e110: 2074 6865 2063 6f6d 7069 6c65 6420 636f   the compiled co
+0001e120: 6465 2066 6f72 2074 6865 2050 7974 686f  de for the Pytho
+0001e130: 6e20 7379 6e74 6178 2e5f 0a0a 2323 2320  n syntax._..### 
+0001e140: 5479 7065 2050 6172 616d 6574 6572 2053  Type Parameter S
+0001e150: 796e 7461 780a 0a43 6f63 6f6e 7574 2066  yntax..Coconut f
+0001e160: 756c 6c79 2073 7570 706f 7274 7320 5b50  ully supports [P
+0001e170: 7974 686f 6e20 332e 3132 2050 4550 2036  ython 3.12 PEP 6
+0001e180: 3935 5d28 6874 7470 733a 2f2f 7065 7073  95](https://peps
+0001e190: 2e70 7974 686f 6e2e 6f72 672f 7065 702d  .python.org/pep-
+0001e1a0: 3036 3935 2f29 2074 7970 6520 7061 7261  0695/) type para
+0001e1b0: 6d65 7465 7220 7379 6e74 6178 206f 6e20  meter syntax on 
+0001e1c0: 616c 6c20 5079 7468 6f6e 2076 6572 7369  all Python versi
+0001e1d0: 6f6e 732e 0a0a 5468 6174 2069 6e63 6c75  ons...That inclu
+0001e1e0: 6465 7320 7479 7065 2070 6172 616d 6574  des type paramet
+0001e1f0: 6572 7320 666f 7220 636c 6173 7365 732c  ers for classes,
+0001e200: 205b 6064 6174 6160 2074 7970 6573 5d28   [`data` types](
+0001e210: 2364 6174 6129 2c20 616e 6420 5b61 6c6c  #data), and [all
+0001e220: 2074 7970 6573 206f 6620 6675 6e63 7469   types of functi
+0001e230: 6f6e 2064 6566 696e 6974 696f 6e5d 2823  on definition](#
+0001e240: 6675 6e63 7469 6f6e 2d64 6566 696e 6974  function-definit
+0001e250: 696f 6e29 2e20 466f 7220 6469 6666 6572  ion). For differ
+0001e260: 656e 7420 7479 7065 7320 6f66 2066 756e  ent types of fun
+0001e270: 6374 696f 6e20 6465 6669 6e69 7469 6f6e  ction definition
+0001e280: 2c20 7468 6520 7479 7065 2070 6172 616d  , the type param
+0001e290: 6574 6572 7320 616c 7761 7973 2063 6f6d  eters always com
+0001e2a0: 6520 696e 2062 7261 636b 6574 7320 7269  e in brackets ri
+0001e2b0: 6768 7420 6166 7465 7220 7468 6520 6675  ght after the fu
+0001e2c0: 6e63 7469 6f6e 206e 616d 652e 2043 6f63  nction name. Coc
+0001e2d0: 6f6e 7574 2773 205b 656e 6861 6e63 6564  onut's [enhanced
+0001e2e0: 2074 7970 6520 616e 6e6f 7461 7469 6f6e   type annotation
+0001e2f0: 2073 796e 7461 785d 2823 656e 6861 6e63   syntax](#enhanc
+0001e300: 6564 2d74 7970 652d 616e 6e6f 7461 7469  ed-type-annotati
+0001e310: 6f6e 2920 6973 2073 7570 706f 7274 6564  on) is supported
+0001e320: 2066 6f72 2061 6c6c 2074 7970 6520 7061   for all type pa
+0001e330: 7261 6d65 7465 7220 626f 756e 6473 2e0a  rameter bounds..
+0001e340: 0a5f 5761 726e 696e 673a 2075 6e74 696c  ._Warning: until
+0001e350: 2060 6d79 7079 6020 6164 6473 2073 7570   `mypy` adds sup
+0001e360: 706f 7274 2066 6f72 2060 696e 6665 725f  port for `infer_
+0001e370: 7661 7269 616e 6365 3d54 7275 6560 2069  variance=True` i
+0001e380: 6e20 6054 7970 6556 6172 602c 2060 5479  n `TypeVar`, `Ty
+0001e390: 7065 5661 7260 7320 6372 6561 7465 6420  peVar`s created 
+0001e3a0: 7468 6973 2077 6179 2077 696c 6c20 616c  this way will al
+0001e3b0: 7761 7973 2062 6520 696e 7661 7269 616e  ways be invarian
+0001e3c0: 742e 5f0a 0a41 6464 6974 696f 6e61 6c6c  t._..Additionall
+0001e3d0: 792c 2043 6f63 6f6e 7574 2073 7570 706f  y, Coconut suppo
+0001e3e0: 7274 7320 7468 6520 616c 7465 726e 6174  rts the alternat
+0001e3f0: 6976 6520 626f 756e 6473 2073 796e 7461  ive bounds synta
+0001e400: 7820 6f66 2060 7479 7065 204e 6577 5479  x of `type NewTy
+0001e410: 7065 5b54 203c 3a20 626f 756e 645d 203d  pe[T <: bound] =
+0001e420: 202e 2e2e 6020 7261 7468 6572 2074 6861   ...` rather tha
+0001e430: 6e20 6074 7970 6520 4e65 7754 7970 655b  n `type NewType[
+0001e440: 543a 2062 6f75 6e64 5d20 3d20 2e2e 2e60  T: bound] = ...`
+0001e450: 2c20 746f 206d 616b 6520 6974 206d 6f72  , to make it mor
+0001e460: 6520 636c 6561 7220 7468 6174 2069 7420  e clear that it 
+0001e470: 6973 2061 6e20 7570 7065 7220 626f 756e  is an upper boun
+0001e480: 6420 7261 7468 6572 2074 6861 6e20 6120  d rather than a 
+0001e490: 7479 7065 2e20 496e 2060 2d2d 7374 7269  type. In `--stri
+0001e4a0: 6374 6020 6d6f 6465 2c20 603c 3a60 2069  ct` mode, `<:` i
+0001e4b0: 7320 7265 7175 6972 6564 206f 7665 7220  s required over 
+0001e4c0: 603a 6020 666f 7220 616c 6c20 7479 7065  `:` for all type
+0001e4d0: 2070 6172 616d 6574 6572 2062 6f75 6e64   parameter bound
+0001e4e0: 732e 205f 4445 5052 4543 4154 4544 3a20  s. _DEPRECATED: 
+0001e4f0: 603c 3d60 2063 616e 2061 6c73 6f20 6265  `<=` can also be
+0001e500: 2075 7365 6420 6173 2061 6e20 616c 7465   used as an alte
+0001e510: 726e 6174 6976 6520 746f 2060 3c3a 602e  rnative to `<:`.
+0001e520: 5f0a 0a4e 6f74 6520 7468 6174 2074 6865  _..Note that the
+0001e530: 2060 3c3a 6020 7379 6e74 6178 2073 686f   `<:` syntax sho
+0001e540: 756c 6420 6f6e 6c79 2062 6520 7573 6564  uld only be used
+0001e550: 2066 6f72 205b 7479 7065 2062 6f75 6e64   for [type bound
+0001e560: 735d 2868 7474 7073 3a2f 2f70 6570 732e  s](https://peps.
+0001e570: 7079 7468 6f6e 2e6f 7267 2f70 6570 2d30  python.org/pep-0
+0001e580: 3639 352f 2375 7070 6572 2d62 6f75 6e64  695/#upper-bound
+0001e590: 2d73 7065 6369 6669 6361 7469 6f6e 292c  -specification),
+0001e5a0: 206e 6f74 205b 7479 7065 2063 6f6e 7374   not [type const
+0001e5b0: 7261 696e 7473 5d28 6874 7470 733a 2f2f  raints](https://
+0001e5c0: 7065 7073 2e70 7974 686f 6e2e 6f72 672f  peps.python.org/
+0001e5d0: 7065 702d 3036 3935 2f23 636f 6e73 7472  pep-0695/#constr
+0001e5e0: 6169 6e65 642d 7479 7065 2d73 7065 6369  ained-type-speci
+0001e5f0: 6669 6361 7469 6f6e 29e2 8094 666f 7220  fication)...for 
+0001e600: 7479 7065 2063 6f6e 7374 7261 696e 7473  type constraints
+0001e610: 2c20 436f 636f 6e75 7420 7374 796c 6520  , Coconut style 
+0001e620: 7072 6566 6572 7320 7468 6520 7661 6e69  prefers the vani
+0001e630: 6c6c 6120 5079 7468 6f6e 2060 3a60 2073  lla Python `:` s
+0001e640: 796e 7461 782c 2077 6869 6368 2068 656c  yntax, which hel
+0001e650: 7073 2074 6f20 6469 7361 6d62 6967 7561  ps to disambigua
+0001e660: 7465 2062 6574 7765 656e 2074 6865 2074  te between the t
+0001e670: 776f 2063 6173 6573 2c20 6173 2074 6865  wo cases, as the
+0001e680: 7920 6172 6520 6675 6e63 7469 6f6e 616c  y are functional
+0001e690: 6c79 2064 6966 6665 7265 6e74 2062 7574  ly different but
+0001e6a0: 206f 7468 6572 7769 7365 2068 6172 6420   otherwise hard 
+0001e6b0: 746f 2074 656c 6c20 6170 6172 7420 6174  to tell apart at
+0001e6c0: 2061 2067 6c61 6e63 652e 2054 6869 7320   a glance. This 
+0001e6d0: 6973 2065 6e66 6f72 6365 6420 696e 2060  is enforced in `
+0001e6e0: 2d2d 7374 7269 6374 6020 6d6f 6465 2e0a  --strict` mode..
+0001e6f0: 0a5f 4e6f 7465 2074 6861 742c 2062 7920  ._Note that, by 
+0001e700: 6465 6661 756c 742c 2061 6c6c 2074 7970  default, all typ
+0001e710: 6520 6465 636c 6172 6174 696f 6e73 2061  e declarations a
+0001e720: 7265 2077 7261 7070 6564 2069 6e20 7374  re wrapped in st
+0001e730: 7269 6e67 7320 746f 2065 6e61 626c 6520  rings to enable 
+0001e740: 666f 7277 6172 6420 7265 6665 7265 6e63  forward referenc
+0001e750: 6573 2061 6e64 2069 6d70 726f 7665 2072  es and improve r
+0001e760: 756e 7469 6d65 2070 6572 666f 726d 616e  untime performan
+0001e770: 6365 2e20 4966 2079 6f75 2064 6f6e 2774  ce. If you don't
+0001e780: 2077 616e 7420 7468 6174 e280 9465 2e67   want that...e.g
+0001e790: 2e20 6265 6361 7573 6520 796f 7520 7761  . because you wa
+0001e7a0: 6e74 2074 6f20 7573 6520 7479 7065 2061  nt to use type a
+0001e7b0: 6e6e 6f74 6174 696f 6e73 2061 7420 7275  nnotations at ru
+0001e7c0: 6e74 696d 65e2 8094 7369 6d70 6c79 2070  ntime...simply p
+0001e7d0: 6173 7320 7468 6520 602d 2d6e 6f2d 7772  ass the `--no-wr
+0001e7e0: 6170 2d74 7970 6573 6020 666c 6167 2e5f  ap-types` flag._
+0001e7f0: 0a0a 2323 2323 2320 5045 5020 3639 3520  ..##### PEP 695 
+0001e800: 446f 6373 0a0a 4465 6669 6e69 6e67 2061  Docs..Defining a
+0001e810: 2067 656e 6572 6963 2063 6c61 7373 2070   generic class p
+0001e820: 7269 6f72 2074 6f20 7468 6973 2050 4550  rior to this PEP
+0001e830: 206c 6f6f 6b73 2073 6f6d 6574 6869 6e67   looks something
+0001e840: 206c 696b 6520 7468 6973 2e0a 0a60 6060   like this...```
+0001e850: 636f 636f 6e75 745f 7079 7468 6f6e 0a66  coconut_python.f
+0001e860: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+0001e870: 7420 4765 6e65 7269 632c 2054 7970 6556  t Generic, TypeV
+0001e880: 6172 0a0a 5f54 5f63 6f20 3d20 5479 7065  ar.._T_co = Type
+0001e890: 5661 7228 225f 545f 636f 222c 2063 6f76  Var("_T_co", cov
+0001e8a0: 6172 6961 6e74 3d54 7275 652c 2062 6f75  ariant=True, bou
+0001e8b0: 6e64 3d73 7472 290a 0a63 6c61 7373 2043  nd=str)..class C
+0001e8c0: 6c61 7373 4128 4765 6e65 7269 635b 5f54  lassA(Generic[_T
+0001e8d0: 5f63 6f5d 293a 0a20 2020 2064 6566 206d  _co]):.    def m
+0001e8e0: 6574 686f 6431 2873 656c 6629 202d 3e20  ethod1(self) -> 
+0001e8f0: 5f54 5f63 6f3a 0a20 2020 2020 2020 202e  _T_co:.        .
+0001e900: 2e2e 0a60 6060 0a0a 5769 7468 2074 6865  ...```..With the
+0001e910: 206e 6577 2073 796e 7461 782c 2069 7420   new syntax, it 
+0001e920: 6c6f 6f6b 7320 6c69 6b65 2074 6869 732e  looks like this.
+0001e930: 0a0a 6060 6063 6f63 6f6e 7574 0a63 6c61  ..```coconut.cla
+0001e940: 7373 2043 6c61 7373 415b 543a 2073 7472  ss ClassA[T: str
+0001e950: 5d3a 0a20 2020 2064 6566 206d 6574 686f  ]:.    def metho
+0001e960: 6431 2873 656c 6629 202d 3e20 543a 0a20  d1(self) -> T:. 
+0001e970: 2020 2020 2020 202e 2e2e 0a60 6060 0a0a         ....```..
+0001e980: 4865 7265 2069 7320 616e 2065 7861 6d70  Here is an examp
+0001e990: 6c65 206f 6620 6120 6765 6e65 7269 6320  le of a generic 
+0001e9a0: 6675 6e63 7469 6f6e 2074 6f64 6179 2e0a  function today..
+0001e9b0: 0a60 6060 636f 636f 6e75 745f 7079 7468  .```coconut_pyth
+0001e9c0: 6f6e 0a66 726f 6d20 7479 7069 6e67 2069  on.from typing i
+0001e9d0: 6d70 6f72 7420 5479 7065 5661 720a 0a5f  mport TypeVar.._
+0001e9e0: 5420 3d20 5479 7065 5661 7228 225f 5422  T = TypeVar("_T"
+0001e9f0: 290a 0a64 6566 2066 756e 6328 613a 205f  )..def func(a: _
+0001ea00: 542c 2062 3a20 5f54 2920 2d3e 205f 543a  T, b: _T) -> _T:
+0001ea10: 0a20 2020 202e 2e2e 0a60 6060 0a0a 416e  .    ....```..An
+0001ea20: 6420 7468 6520 6e65 7720 7379 6e74 6178  d the new syntax
+0001ea30: 2e0a 0a60 6060 636f 636f 6e75 740a 6465  ...```coconut.de
+0001ea40: 6620 6675 6e63 5b54 5d28 613a 2054 2c20  f func[T](a: T, 
+0001ea50: 623a 2054 2920 2d3e 2054 3a0a 2020 2020  b: T) -> T:.    
+0001ea60: 2e2e 2e0a 6060 600a 0a48 6572 6520 6973  ....```..Here is
+0001ea70: 2061 6e20 6578 616d 706c 6520 6f66 2061   an example of a
+0001ea80: 2067 656e 6572 6963 2074 7970 6520 616c   generic type al
+0001ea90: 6961 7320 746f 6461 792e 0a0a 6060 6063  ias today...```c
+0001eaa0: 6f63 6f6e 7574 5f70 7974 686f 6e0a 6672  oconut_python.fr
+0001eab0: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+0001eac0: 2054 7970 6541 6c69 6173 0a0a 5f54 203d   TypeAlias.._T =
+0001ead0: 2054 7970 6556 6172 2822 5f54 2229 0a0a   TypeVar("_T")..
+0001eae0: 4c69 7374 4f72 5365 743a 2054 7970 6541  ListOrSet: TypeA
+0001eaf0: 6c69 6173 203d 206c 6973 745b 5f54 5d20  lias = list[_T] 
+0001eb00: 7c20 7365 745b 5f54 5d0a 6060 600a 0a41  | set[_T].```..A
+0001eb10: 6e64 2077 6974 6820 7468 6520 6e65 7720  nd with the new 
+0001eb20: 7379 6e74 6178 2e0a 0a60 6060 636f 636f  syntax...```coco
+0001eb30: 6e75 740a 7479 7065 204c 6973 744f 7253  nut.type ListOrS
+0001eb40: 6574 5b54 5d20 3d20 6c69 7374 5b54 5d20  et[T] = list[T] 
+0001eb50: 7c20 7365 745b 545d 0a60 6060 0a0a 0a23  | set[T].```...#
+0001eb60: 2323 2323 2045 7861 6d70 6c65 0a0a 2a2a  #### Example..**
+0001eb70: 436f 636f 6e75 743a 2a2a 0a60 6060 636f  Coconut:**.```co
+0001eb80: 636f 6e75 740a 6461 7461 2044 5b54 5d28  conut.data D[T](
+0001eb90: 783a 2054 2c20 793a 2054 290a 0a64 6566  x: T, y: T)..def
+0001eba0: 206d 795f 6964 656e 745b 545d 2878 3a20   my_ident[T](x: 
+0001ebb0: 5429 202d 3e20 5420 3d20 780a 6060 600a  T) -> T = x.```.
+0001ebc0: 0a2a 2a50 7974 686f 6e3a 2a2a 0a5f 4361  .**Python:**._Ca
+0001ebd0: 6e27 7420 6265 2064 6f6e 6520 7769 7468  n't be done with
+0001ebe0: 6f75 7420 6120 636f 6d70 6c65 7820 6465  out a complex de
+0001ebf0: 6669 6e69 7469 6f6e 2066 6f72 2074 6865  finition for the
+0001ec00: 2064 6174 6120 7479 7065 2e20 5365 6520   data type. See 
+0001ec10: 7468 6520 636f 6d70 696c 6564 2063 6f64  the compiled cod
+0001ec20: 6520 666f 7220 7468 6520 5079 7468 6f6e  e for the Python
+0001ec30: 2073 796e 7461 782e 5f0a 0a23 2323 2049   syntax._..### I
+0001ec40: 6d70 6c69 6369 7420 6070 6173 7360 0a0a  mplicit `pass`..
+0001ec50: 436f 636f 6e75 7420 7375 7070 6f72 7473  Coconut supports
+0001ec60: 2074 6865 2073 696d 706c 6520 6063 6c61   the simple `cla
+0001ec70: 7373 206e 616d 6528 6261 7365 2960 2061  ss name(base)` a
+0001ec80: 6e64 2060 6461 7461 206e 616d 6528 6172  nd `data name(ar
+0001ec90: 6773 2960 2061 7320 616c 6961 7365 7320  gs)` as aliases 
+0001eca0: 666f 7220 6063 6c61 7373 206e 616d 6528  for `class name(
+0001ecb0: 6261 7365 293a 2070 6173 7360 2061 6e64  base): pass` and
+0001ecc0: 2060 6461 7461 206e 616d 6528 6172 6773   `data name(args
+0001ecd0: 293a 2070 6173 7360 2e0a 0a23 2323 2323  ): pass`...#####
+0001ece0: 2045 7861 6d70 6c65 0a0a 2a2a 436f 636f   Example..**Coco
+0001ecf0: 6e75 743a 2a2a 0a60 6060 636f 636f 6e75  nut:**.```coconu
+0001ed00: 740a 636c 6173 7320 5472 6565 0a64 6174  t.class Tree.dat
+0001ed10: 6120 456d 7074 7920 6672 6f6d 2054 7265  a Empty from Tre
+0001ed20: 650a 6461 7461 204c 6561 6628 6974 656d  e.data Leaf(item
+0001ed30: 2920 6672 6f6d 2054 7265 650a 6461 7461  ) from Tree.data
+0001ed40: 204e 6f64 6528 6c65 6674 2c20 7269 6768   Node(left, righ
+0001ed50: 7429 2066 726f 6d20 5472 6565 0a60 6060  t) from Tree.```
+0001ed60: 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a 5f43  ..**Python:**._C
+0001ed70: 616e 2774 2062 6520 646f 6e65 2077 6974  an't be done wit
+0001ed80: 686f 7574 2061 2073 6572 6965 7320 6f66  hout a series of
+0001ed90: 206d 6574 686f 6420 6465 6669 6e69 7469   method definiti
+0001eda0: 6f6e 7320 666f 7220 6561 6368 2064 6174  ons for each dat
+0001edb0: 6120 7479 7065 2e20 5365 6520 7468 6520  a type. See the 
+0001edc0: 636f 6d70 696c 6564 2063 6f64 6520 666f  compiled code fo
+0001edd0: 7220 7468 6520 5079 7468 6f6e 2073 796e  r the Python syn
+0001ede0: 7461 782e 5f0a 0a23 2323 2044 6563 6f72  tax._..### Decor
+0001edf0: 6174 6f72 730a 0a55 6e6c 696b 6520 5079  ators..Unlike Py
+0001ee00: 7468 6f6e 2c20 7768 6963 6820 6f6e 6c79  thon, which only
+0001ee10: 2073 7570 706f 7274 7320 6120 7369 6e67   supports a sing
+0001ee20: 6c65 2076 6172 6961 626c 6520 6f72 2066  le variable or f
+0001ee30: 756e 6374 696f 6e20 6361 6c6c 2069 6e20  unction call in 
+0001ee40: 6120 6465 636f 7261 746f 722c 2043 6f63  a decorator, Coc
+0001ee50: 6f6e 7574 2073 7570 706f 7274 7320 616e  onut supports an
+0001ee60: 7920 6578 7072 6573 7369 6f6e 2061 7320  y expression as 
+0001ee70: 696e 205b 5045 5020 3631 345d 2868 7474  in [PEP 614](htt
+0001ee80: 7073 3a2f 2f77 7777 2e70 7974 686f 6e2e  ps://www.python.
+0001ee90: 6f72 672f 6465 762f 7065 7073 2f70 6570  org/dev/peps/pep
+0001eea0: 2d30 3631 342f 292e 0a0a 2323 2323 2320  -0614/)...##### 
+0001eeb0: 4578 616d 706c 650a 0a2a 2a43 6f63 6f6e  Example..**Cocon
+0001eec0: 7574 3a2a 2a0a 6060 6063 6f63 6f6e 7574  ut:**.```coconut
+0001eed0: 0a40 2077 7261 7070 6572 3120 2e2e 2077  .@ wrapper1 .. w
+0001eee0: 7261 7070 6572 3224 2861 7267 290a 6465  rapper2$(arg).de
+0001eef0: 6620 6675 6e63 2878 2920 3d20 782a 2a32  f func(x) = x**2
+0001ef00: 0a60 6060 0a0a 2a2a 5079 7468 6f6e 3a2a  .```..**Python:*
+0001ef10: 2a0a 6060 6063 6f63 6f6e 7574 5f70 7974  *.```coconut_pyt
+0001ef20: 686f 6e0a 6465 6620 7772 6170 7065 7228  hon.def wrapper(
+0001ef30: 6675 6e63 293a 0a20 2020 2072 6574 7572  func):.    retur
+0001ef40: 6e20 7772 6170 7065 7231 2877 7261 7070  n wrapper1(wrapp
+0001ef50: 6572 3228 6172 672c 2066 756e 6329 290a  er2(arg, func)).
+0001ef60: 4077 7261 7070 6572 0a64 6566 2066 756e  @wrapper.def fun
+0001ef70: 6328 7829 3a0a 2020 2020 7265 7475 726e  c(x):.    return
+0001ef80: 2078 2a2a 320a 6060 600a 0a23 2323 2053   x**2.```..### S
+0001ef90: 7461 7465 6d65 6e74 204e 6573 7469 6e67  tatement Nesting
+0001efa0: 0a0a 436f 636f 6e75 7420 7375 7070 6f72  ..Coconut suppor
+0001efb0: 7473 2074 6865 206e 6573 7469 6e67 206f  ts the nesting o
+0001efc0: 6620 636f 6d70 6f75 6e64 2073 7461 7465  f compound state
+0001efd0: 6d65 6e74 7320 6f6e 2074 6865 2073 616d  ments on the sam
+0001efe0: 6520 6c69 6e65 2e20 5468 6973 2061 6c6c  e line. This all
+0001eff0: 6f77 7320 7468 6520 6d69 7869 6e67 206f  ows the mixing o
+0001f000: 6620 606d 6174 6368 6020 616e 6420 6069  f `match` and `i
+0001f010: 6660 2073 7461 7465 6d65 6e74 7320 746f  f` statements to
+0001f020: 6765 7468 6572 2c20 6173 2077 656c 6c20  gether, as well 
+0001f030: 6173 2063 6f6d 706f 756e 6420 6074 7279  as compound `try
+0001f040: 6020 7374 6174 656d 656e 7473 2e0a 0a23  ` statements...#
+0001f050: 2323 2323 2045 7861 6d70 6c65 0a0a 2a2a  #### Example..**
+0001f060: 436f 636f 6e75 743a 2a2a 0a60 6060 636f  Coconut:**.```co
+0001f070: 636f 6e75 740a 6966 2069 6e76 616c 6964  conut.if invalid
+0001f080: 2869 6e70 7574 5f6c 6973 7429 3a0a 2020  (input_list):.  
+0001f090: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
+0001f0a0: 6e28 290a 656c 7365 3a20 6d61 7463 6820  n().else: match 
+0001f0b0: 5b68 6561 645d 202b 2074 6169 6c20 696e  [head] + tail in
+0001f0c0: 2069 6e70 7574 5f6c 6973 743a 0a20 2020   input_list:.   
+0001f0d0: 2070 7269 6e74 2868 6561 642c 2074 6169   print(head, tai
+0001f0e0: 6c29 0a65 6c73 653a 0a20 2020 2070 7269  l).else:.    pri
+0001f0f0: 6e74 2869 6e70 7574 5f6c 6973 7429 0a60  nt(input_list).`
+0001f100: 6060 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a  ``..**Python:**.
+0001f110: 6060 6063 6f63 6f6e 7574 5f70 7974 686f  ```coconut_pytho
+0001f120: 6e0a 6672 6f6d 2063 6f6c 6c65 6374 696f  n.from collectio
+0001f130: 6e73 2e61 6263 2069 6d70 6f72 7420 5365  ns.abc import Se
+0001f140: 7175 656e 6365 0a69 6620 696e 7661 6c69  quence.if invali
+0001f150: 6428 696e 7075 745f 6c69 7374 293a 0a20  d(input_list):. 
+0001f160: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
+0001f170: 6f6e 2829 0a65 6c69 6620 6973 696e 7374  on().elif isinst
+0001f180: 616e 6365 2869 6e70 7574 5f6c 6973 742c  ance(input_list,
+0001f190: 2053 6571 7565 6e63 6529 2061 6e64 206c   Sequence) and l
+0001f1a0: 656e 2869 6e70 7574 5f6c 6973 7429 203e  en(input_list) >
+0001f1b0: 3d20 313a 0a20 2020 2068 6561 642c 2074  = 1:.    head, t
+0001f1c0: 6169 6c20 3d20 696e 7075 746c 6973 745b  ail = inputlist[
+0001f1d0: 305d 2c20 696e 7075 746c 6973 745b 313a  0], inputlist[1:
+0001f1e0: 5d0a 2020 2020 7072 696e 7428 6865 6164  ].    print(head
+0001f1f0: 2c20 7461 696c 290a 656c 7365 3a0a 2020  , tail).else:.  
+0001f200: 2020 7072 696e 7428 696e 7075 745f 6c69    print(input_li
+0001f210: 7374 290a 6060 600a 0a23 2323 2060 6578  st).```..### `ex
+0001f220: 6365 7074 6020 5374 6174 656d 656e 7473  cept` Statements
+0001f230: 0a0a 5079 7468 6f6e 2033 2072 6571 7569  ..Python 3 requi
+0001f240: 7265 7320 7468 6174 2069 6620 6d75 6c74  res that if mult
+0001f250: 6970 6c65 2065 7863 6570 7469 6f6e 7320  iple exceptions 
+0001f260: 6172 6520 746f 2062 6520 6361 7567 6874  are to be caught
+0001f270: 2c20 7468 6579 206d 7573 7420 6265 2070  , they must be p
+0001f280: 6c61 6365 6420 696e 7369 6465 206f 6620  laced inside of 
+0001f290: 7061 7265 6e74 6865 7365 732c 2073 6f20  parentheses, so 
+0001f2a0: 6173 2074 6f20 6469 7361 6c6c 6f77 2050  as to disallow P
+0001f2b0: 7974 686f 6e20 3227 7320 7573 6520 6f66  ython 2's use of
+0001f2c0: 2061 2063 6f6d 6d61 2069 6e73 7465 6164   a comma instead
+0001f2d0: 206f 6620 6061 7360 2e20 436f 636f 6e75   of `as`. Coconu
+0001f2e0: 7420 616c 6c6f 7773 2063 6f6d 6d61 7320  t allows commas 
+0001f2f0: 696e 2065 7863 6570 7420 7374 6174 656d  in except statem
+0001f300: 656e 7473 2074 6f20 7472 616e 736c 6174  ents to translat
+0001f310: 6520 746f 2063 6174 6368 696e 6720 6d75  e to catching mu
+0001f320: 6c74 6970 6c65 2065 7863 6570 7469 6f6e  ltiple exception
+0001f330: 7320 7769 7468 6f75 7420 7468 6520 6e65  s without the ne
+0001f340: 6564 2066 6f72 2070 6172 656e 7468 6573  ed for parenthes
+0001f350: 6573 2c20 7369 6e63 652c 2061 7320 696e  es, since, as in
+0001f360: 2050 7974 686f 6e20 332c 2060 6173 6020   Python 3, `as` 
+0001f370: 6973 2061 6c77 6179 7320 7265 7175 6972  is always requir
+0001f380: 6564 2074 6f20 6269 6e64 2074 6865 2065  ed to bind the e
+0001f390: 7863 6570 7469 6f6e 2074 6f20 6120 6e61  xception to a na
+0001f3a0: 6d65 2e0a 0a23 2323 2323 2045 7861 6d70  me...##### Examp
+0001f3b0: 6c65 0a0a 2a2a 436f 636f 6e75 743a 2a2a  le..**Coconut:**
+0001f3c0: 0a60 6060 636f 636f 6e75 740a 7472 793a  .```coconut.try:
+0001f3d0: 0a20 2020 2075 6e73 6166 655f 6675 6e63  .    unsafe_func
+0001f3e0: 2861 7267 290a 6578 6365 7074 2053 796e  (arg).except Syn
+0001f3f0: 7461 7845 7272 6f72 2c20 5661 6c75 6545  taxError, ValueE
+0001f400: 7272 6f72 2061 7320 6572 723a 0a20 2020  rror as err:.   
+0001f410: 2068 616e 646c 6528 6572 7229 0a60 6060   handle(err).```
+0001f420: 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a 6060  ..**Python:**.``
+0001f430: 6063 6f63 6f6e 7574 5f70 7974 686f 6e0a  `coconut_python.
+0001f440: 7472 793a 0a20 2020 2075 6e73 6166 655f  try:.    unsafe_
+0001f450: 6675 6e63 2861 7267 290a 6578 6365 7074  func(arg).except
+0001f460: 2028 5379 6e74 6178 4572 726f 722c 2056   (SyntaxError, V
+0001f470: 616c 7565 4572 726f 7229 2061 7320 6572  alueError) as er
+0001f480: 723a 0a20 2020 2068 616e 646c 6528 6572  r:.    handle(er
+0001f490: 7229 0a60 6060 0a0a 2323 2320 496e 2d6c  r).```..### In-l
+0001f4a0: 696e 6520 6067 6c6f 6261 6c60 2041 6e64  ine `global` And
+0001f4b0: 2060 6e6f 6e6c 6f63 616c 6020 4173 7369   `nonlocal` Assi
+0001f4c0: 676e 6d65 6e74 0a0a 436f 636f 6e75 7420  gnment..Coconut 
+0001f4d0: 616c 6c6f 7773 2066 6f72 2060 676c 6f62  allows for `glob
+0001f4e0: 616c 6020 6f72 2060 6e6f 6e6c 6f63 616c  al` or `nonlocal
+0001f4f0: 6020 746f 2070 7265 6365 6465 2061 7373  ` to precede ass
+0001f500: 6967 6e6d 656e 7420 746f 2061 206c 6973  ignment to a lis
+0001f510: 7420 6f66 2076 6172 6961 626c 6573 206f  t of variables o
+0001f520: 7220 2861 7567 6d65 6e74 6564 2920 6173  r (augmented) as
+0001f530: 7369 676e 6d65 6e74 2074 6f20 6120 7661  signment to a va
+0001f540: 7269 6162 6c65 2074 6f20 6d61 6b65 2074  riable to make t
+0001f550: 6861 7420 6173 7369 676e 6d65 6e74 2060  hat assignment `
+0001f560: 676c 6f62 616c 6020 6f72 2060 6e6f 6e6c  global` or `nonl
+0001f570: 6f63 616c 602c 2072 6573 7065 6374 6976  ocal`, respectiv
+0001f580: 656c 792e 0a0a 2323 2323 2320 4578 616d  ely...##### Exam
+0001f590: 706c 650a 0a2a 2a43 6f63 6f6e 7574 3a2a  ple..**Coconut:*
+0001f5a0: 2a0a 6060 6063 6f63 6f6e 7574 0a67 6c6f  *.```coconut.glo
+0001f5b0: 6261 6c20 7374 6174 655f 612c 2073 7461  bal state_a, sta
+0001f5c0: 7465 5f62 203d 2031 302c 2031 3030 0a67  te_b = 10, 100.g
+0001f5d0: 6c6f 6261 6c20 7374 6174 655f 6320 2b3d  lobal state_c +=
+0001f5e0: 2031 0a60 6060 0a0a 2a2a 5079 7468 6f6e   1.```..**Python
+0001f5f0: 3a2a 2a0a 6060 6063 6f63 6f6e 7574 5f70  :**.```coconut_p
+0001f600: 7974 686f 6e0a 676c 6f62 616c 2073 7461  ython.global sta
+0001f610: 7465 5f61 2c20 7374 6174 655f 623b 2073  te_a, state_b; s
+0001f620: 7461 7465 5f61 2c20 7374 6174 655f 6220  tate_a, state_b 
+0001f630: 3d20 3130 2c20 3130 300a 676c 6f62 616c  = 10, 100.global
+0001f640: 2073 7461 7465 5f63 3b20 7374 6174 655f   state_c; state_
+0001f650: 6320 2b3d 2031 0a60 6060 0a0a 2323 2320  c += 1.```..### 
+0001f660: 436f 6465 2050 6173 7374 6872 6f75 6768  Code Passthrough
+0001f670: 0a0a 436f 636f 6e75 7420 7375 7070 6f72  ..Coconut suppor
+0001f680: 7473 2074 6865 2061 6269 6c69 7479 2074  ts the ability t
+0001f690: 6f20 7061 7373 2061 7262 6974 7261 7279  o pass arbitrary
+0001f6a0: 2063 6f64 6520 7468 726f 7567 6820 7468   code through th
+0001f6b0: 6520 636f 6d70 696c 6572 2077 6974 686f  e compiler witho
+0001f6c0: 7574 2062 6569 6e67 2074 6f75 6368 6564  ut being touched
+0001f6d0: 2c20 666f 7220 636f 6d70 6174 6962 696c  , for compatibil
+0001f6e0: 6974 7920 7769 7468 206f 7468 6572 2076  ity with other v
+0001f6f0: 6172 6961 6e74 7320 6f66 2050 7974 686f  ariants of Pytho
+0001f700: 6e2c 2073 7563 6820 6173 205b 4379 7468  n, such as [Cyth
+0001f710: 6f6e 5d28 6874 7470 3a2f 2f63 7974 686f  on](http://cytho
+0001f720: 6e2e 6f72 672f 2920 6f72 205b 4d79 7468  n.org/) or [Myth
+0001f730: 6f6e 5d28 6874 7470 3a2f 2f6d 7974 686f  on](http://mytho
+0001f740: 6e2e 6f72 672f 292e 2041 6e79 7468 696e  n.org/). Anythin
+0001f750: 6720 706c 6163 6564 2062 6574 7765 656e  g placed between
+0001f760: 2060 5c28 6020 616e 6420 7468 6520 636f   `\(` and the co
+0001f770: 7272 6573 706f 6e64 696e 6720 636c 6f73  rresponding clos
+0001f780: 6520 7061 7265 6e74 6865 7369 7320 7769  e parenthesis wi
+0001f790: 6c6c 2062 6520 7061 7373 6564 2074 6872  ll be passed thr
+0001f7a0: 6f75 6768 2c20 6173 2077 656c 6c20 6173  ough, as well as
+0001f7b0: 2061 6e79 206c 696e 6520 7374 6172 7469   any line starti
+0001f7c0: 6e67 2077 6974 6820 605c 5c60 2c20 7768  ng with `\\`, wh
+0001f7d0: 6963 6820 7769 6c6c 2068 6176 6520 7468  ich will have th
+0001f7e0: 6520 6164 6469 7469 6f6e 616c 2065 6666  e additional eff
+0001f7f0: 6563 7420 6f66 2061 6c6c 6f77 696e 6720  ect of allowing 
+0001f800: 696e 6465 6e74 6174 696f 6e20 756e 6465  indentation unde
+0001f810: 7220 6974 2e0a 0a23 2323 2323 2045 7861  r it...##### Exa
+0001f820: 6d70 6c65 0a0a 2a2a 436f 636f 6e75 743a  mple..**Coconut:
+0001f830: 2a2a 0a60 6060 636f 636f 6e75 740a 5c5c  **.```coconut.\\
+0001f840: 6364 6566 2066 2878 293a 0a20 2020 2072  cdef f(x):.    r
+0001f850: 6574 7572 6e20 7820 7c3e 2067 0a60 6060  eturn x |> g.```
+0001f860: 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a 6060  ..**Python:**.``
+0001f870: 6063 6f63 6f6e 7574 5f70 7974 686f 6e0a  `coconut_python.
+0001f880: 6364 6566 2066 2878 293a 0a20 2020 2072  cdef f(x):.    r
+0001f890: 6574 7572 6e20 6728 7829 0a60 6060 0a0a  eturn g(x).```..
+0001f8a0: 2323 2320 456e 6861 6e63 6564 2050 6172  ### Enhanced Par
+0001f8b0: 656e 7468 6574 6963 616c 2043 6f6e 7469  enthetical Conti
+0001f8c0: 6e75 6174 696f 6e0a 0a53 696e 6365 2043  nuation..Since C
+0001f8d0: 6f63 6f6e 7574 2073 796e 7461 7820 6973  oconut syntax is
+0001f8e0: 2061 2073 7570 6572 7365 7420 6f66 2050   a superset of P
+0001f8f0: 7974 686f 6e20 3320 7379 6e74 6178 2c20  ython 3 syntax, 
+0001f900: 436f 636f 6e75 7420 7375 7070 6f72 7473  Coconut supports
+0001f910: 2074 6865 2073 616d 6520 6c69 6e65 2063   the same line c
+0001f920: 6f6e 7469 6e75 6174 696f 6e20 7379 6e74  ontinuation synt
+0001f930: 6178 2061 7320 5079 7468 6f6e 2e20 5468  ax as Python. Th
+0001f940: 6174 206d 6561 6e73 2062 6f74 6820 6261  at means both ba
+0001f950: 636b 736c 6173 6820 6c69 6e65 2063 6f6e  ckslash line con
+0001f960: 7469 6e75 6174 696f 6e20 616e 6420 696d  tinuation and im
+0001f970: 706c 6965 6420 6c69 6e65 2063 6f6e 7469  plied line conti
+0001f980: 6e75 6174 696f 6e20 696e 7369 6465 206f  nuation inside o
+0001f990: 6620 7061 7265 6e74 6865 7365 732c 2062  f parentheses, b
+0001f9a0: 7261 636b 6574 732c 206f 7220 6272 6163  rackets, or brac
+0001f9b0: 6573 2077 696c 6c20 616c 6c20 776f 726b  es will all work
+0001f9c0: 2e0a 0a49 6e20 5079 7468 6f6e 2c20 686f  ...In Python, ho
+0001f9d0: 7765 7665 722c 2074 6865 7265 2061 7265  wever, there are
+0001f9e0: 2073 6f6d 6520 6361 7365 7320 2873 7563   some cases (suc
+0001f9f0: 6820 6173 206d 756c 7469 706c 6520 6077  h as multiple `w
+0001fa00: 6974 6860 2073 7461 7465 6d65 6e74 7329  ith` statements)
+0001fa10: 2077 6865 7265 206f 6e6c 7920 6261 636b   where only back
+0001fa20: 736c 6173 6820 636f 6e74 696e 7561 7469  slash continuati
+0001fa30: 6f6e 2c20 616e 6420 6e6f 7420 7061 7265  on, and not pare
+0001fa40: 6e74 6865 7469 6361 6c20 636f 6e74 696e  nthetical contin
+0001fa50: 7561 7469 6f6e 2c20 6973 2073 7570 706f  uation, is suppo
+0001fa60: 7274 6564 2e20 436f 636f 6e75 7420 6164  rted. Coconut ad
+0001fa70: 6473 2073 7570 706f 7274 2066 6f72 2070  ds support for p
+0001fa80: 6172 656e 7468 6574 6963 616c 2063 6f6e  arenthetical con
+0001fa90: 7469 6e75 6174 696f 6e20 696e 2061 6c6c  tinuation in all
+0001faa0: 2074 6865 7365 2063 6173 6573 2e20 5468   these cases. Th
+0001fab0: 6973 2061 6c73 6f20 696e 636c 7564 6573  is also includes
+0001fac0: 2073 7570 706f 7274 2061 7320 7065 7220   support as per 
+0001fad0: 5b50 4550 2036 3739 5d28 6874 7470 733a  [PEP 679](https:
+0001fae0: 2f2f 7065 7073 2e70 7974 686f 6e2e 6f72  //peps.python.or
+0001faf0: 672f 7065 702d 3036 3739 2920 666f 7220  g/pep-0679) for 
+0001fb00: 7061 7265 6e74 6865 7369 7a65 6420 6061  parenthesized `a
+0001fb10: 7373 6572 7460 2073 7461 7465 6d65 6e74  ssert` statement
+0001fb20: 732e 0a0a 5375 7070 6f72 7469 6e67 2070  s...Supporting p
+0001fb30: 6172 656e 7468 6574 6963 616c 2063 6f6e  arenthetical con
+0001fb40: 7469 6e75 6174 696f 6e20 6576 6572 7977  tinuation everyw
+0001fb50: 6865 7265 2061 6c6c 6f77 7320 7468 6520  here allows the 
+0001fb60: 5b50 4550 2038 5d28 6874 7470 733a 2f2f  [PEP 8](https://
+0001fb70: 7777 772e 7079 7468 6f6e 2e6f 7267 2f64  www.python.org/d
+0001fb80: 6576 2f70 6570 732f 7065 702d 3030 3038  ev/peps/pep-0008
+0001fb90: 2f29 2063 6f6e 7665 6e74 696f 6e2c 2077  /) convention, w
+0001fba0: 6869 6368 2061 766f 6964 7320 6261 636b  hich avoids back
+0001fbb0: 736c 6173 6820 636f 6e74 696e 7561 7469  slash continuati
+0001fbc0: 6f6e 2069 6e20 6661 766f 7220 6f66 2069  on in favor of i
+0001fbd0: 6d70 6c69 6564 2070 6172 656e 7468 6574  mplied parenthet
+0001fbe0: 6963 616c 2063 6f6e 7469 6e75 6174 696f  ical continuatio
+0001fbf0: 6e2c 2074 6f20 616c 7761 7973 2062 6520  n, to always be 
+0001fc00: 706f 7373 6962 6c65 2074 6f20 666f 6c6c  possible to foll
+0001fc10: 6f77 2e20 4672 6f6d 2050 4550 2038 3a0a  ow. From PEP 8:.
+0001fc20: 0a3e 2054 6865 2070 7265 6665 7272 6564  .> The preferred
+0001fc30: 2077 6179 206f 6620 7772 6170 7069 6e67   way of wrapping
+0001fc40: 206c 6f6e 6720 6c69 6e65 7320 6973 2062   long lines is b
+0001fc50: 7920 7573 696e 6720 5079 7468 6f6e 2773  y using Python's
+0001fc60: 2069 6d70 6c69 6564 206c 696e 6520 636f   implied line co
+0001fc70: 6e74 696e 7561 7469 6f6e 2069 6e73 6964  ntinuation insid
+0001fc80: 6520 7061 7265 6e74 6865 7365 732c 2062  e parentheses, b
+0001fc90: 7261 636b 6574 7320 616e 6420 6272 6163  rackets and brac
+0001fca0: 6573 2e20 4c6f 6e67 206c 696e 6573 2063  es. Long lines c
+0001fcb0: 616e 2062 6520 6272 6f6b 656e 206f 7665  an be broken ove
+0001fcc0: 7220 6d75 6c74 6970 6c65 206c 696e 6573  r multiple lines
+0001fcd0: 2062 7920 7772 6170 7069 6e67 2065 7870   by wrapping exp
+0001fce0: 7265 7373 696f 6e73 2069 6e20 7061 7265  ressions in pare
+0001fcf0: 6e74 6865 7365 732e 2054 6865 7365 2073  ntheses. These s
+0001fd00: 686f 756c 6420 6265 2075 7365 6420 696e  hould be used in
+0001fd10: 2070 7265 6665 7265 6e63 6520 746f 2075   preference to u
+0001fd20: 7369 6e67 2061 2062 6163 6b73 6c61 7368  sing a backslash
+0001fd30: 2066 6f72 206c 696e 6520 636f 6e74 696e   for line contin
+0001fd40: 7561 7469 6f6e 2e0a 0a5f 4e6f 7465 3a20  uation..._Note: 
+0001fd50: 5061 7373 696e 6720 602d 2d73 7472 6963  Passing `--stric
+0001fd60: 7460 2077 696c 6c20 656e 666f 7263 6520  t` will enforce 
+0001fd70: 7468 6520 5045 5020 3820 636f 6e76 656e  the PEP 8 conven
+0001fd80: 7469 6f6e 2062 7920 6469 7361 6c6c 6f77  tion by disallow
+0001fd90: 696e 6720 6261 636b 736c 6173 6820 636f  ing backslash co
+0001fda0: 6e74 696e 7561 7469 6f6e 732e 5f0a 0a23  ntinuations._..#
+0001fdb0: 2323 2323 2045 7861 6d70 6c65 0a0a 2a2a  #### Example..**
+0001fdc0: 436f 636f 6e75 743a 2a2a 0a60 6060 636f  Coconut:**.```co
+0001fdd0: 636f 6e75 740a 7769 7468 2028 6f70 656e  conut.with (open
+0001fde0: 2827 2f70 6174 682f 746f 2f73 6f6d 652f  ('/path/to/some/
+0001fdf0: 6669 6c65 2f79 6f75 2f77 616e 742f 746f  file/you/want/to
+0001fe00: 2f72 6561 6427 2920 6173 2066 696c 655f  /read') as file_
+0001fe10: 312c 0a20 2020 2020 206f 7065 6e28 272f  1,.      open('/
+0001fe20: 7061 7468 2f74 6f2f 736f 6d65 2f66 696c  path/to/some/fil
+0001fe30: 652f 6265 696e 672f 7772 6974 7465 6e27  e/being/written'
+0001fe40: 2c20 2777 2729 2061 7320 6669 6c65 5f32  , 'w') as file_2
+0001fe50: 293a 0a20 2020 2066 696c 655f 322e 7772  ):.    file_2.wr
+0001fe60: 6974 6528 6669 6c65 5f31 2e72 6561 6428  ite(file_1.read(
+0001fe70: 2929 0a60 6060 0a0a 2a2a 5079 7468 6f6e  )).```..**Python
+0001fe80: 3a2a 2a0a 6060 6063 6f63 6f6e 7574 5f70  :**.```coconut_p
+0001fe90: 7974 686f 6e0a 2320 7370 6c69 7420 696e  ython.# split in
+0001fea0: 746f 2074 776f 2077 6974 6820 7374 6174  to two with stat
+0001feb0: 656d 656e 7473 2066 6f72 2050 7974 686f  ements for Pytho
+0001fec0: 6e20 322e 3620 636f 6d70 6174 6962 696c  n 2.6 compatibil
+0001fed0: 6974 790a 7769 7468 206f 7065 6e28 272f  ity.with open('/
+0001fee0: 7061 7468 2f74 6f2f 736f 6d65 2f66 696c  path/to/some/fil
+0001fef0: 652f 796f 752f 7761 6e74 2f74 6f2f 7265  e/you/want/to/re
+0001ff00: 6164 2729 2061 7320 6669 6c65 5f31 3a0a  ad') as file_1:.
+0001ff10: 2020 2020 7769 7468 206f 7065 6e28 272f      with open('/
+0001ff20: 7061 7468 2f74 6f2f 736f 6d65 2f66 696c  path/to/some/fil
+0001ff30: 652f 6265 696e 672f 7772 6974 7465 6e27  e/being/written'
+0001ff40: 2c20 2777 2729 2061 7320 6669 6c65 5f32  , 'w') as file_2
+0001ff50: 3a0a 2020 2020 2020 2020 6669 6c65 5f32  :.        file_2
+0001ff60: 2e77 7269 7465 2866 696c 655f 312e 7265  .write(file_1.re
+0001ff70: 6164 2829 290a 6060 600a 0a23 2323 2041  ad()).```..### A
+0001ff80: 7373 6967 6e6d 656e 7420 4578 7072 6573  ssignment Expres
+0001ff90: 7369 6f6e 2043 6861 696e 696e 670a 0a55  sion Chaining..U
+0001ffa0: 6e6c 696b 6520 5079 7468 6f6e 2c20 436f  nlike Python, Co
+0001ffb0: 636f 6e75 7420 616c 6c6f 7773 2061 7373  conut allows ass
+0001ffc0: 6967 6e6d 656e 7420 6578 7072 6573 7369  ignment expressi
+0001ffd0: 6f6e 7320 746f 2062 6520 6368 6169 6e65  ons to be chaine
+0001ffe0: 642c 2061 7320 696e 2060 6120 3a3d 2062  d, as in `a := b
+0001fff0: 203a 3d20 6360 2e20 4e6f 7465 2c20 686f   := c`. Note, ho
+00020000: 7765 7665 722c 2074 6861 7420 6173 7369  wever, that assi
+00020010: 676e 6d65 6e74 2065 7870 7265 7373 696f  gnment expressio
+00020020: 6e73 2069 6e20 6765 6e65 7261 6c20 6172  ns in general ar
+00020030: 6520 6375 7272 656e 746c 7920 6f6e 6c79  e currently only
+00020040: 2073 7570 706f 7274 6564 206f 6e20 602d   supported on `-
+00020050: 2d74 6172 6765 7420 332e 3860 206f 7220  -target 3.8` or 
+00020060: 6869 6768 6572 2e0a 0a23 2323 2323 2045  higher...##### E
+00020070: 7861 6d70 6c65 0a0a 2a2a 436f 636f 6e75  xample..**Coconu
+00020080: 743a 2a2a 0a60 6060 636f 636f 6e75 740a  t:**.```coconut.
+00020090: 2861 203a 3d20 6220 3a3d 2031 290a 6060  (a := b := 1).``
+000200a0: 600a 0a2a 2a50 7974 686f 6e3a 2a2a 0a60  `..**Python:**.`
+000200b0: 6060 636f 636f 6e75 745f 7079 7468 6f6e  ``coconut_python
+000200c0: 0a28 6120 3a3d 2028 6220 3a3d 2031 2929  .(a := (b := 1))
+000200d0: 0a60 6060 0a0a 2323 2042 7569 6c74 2d49  .```..## Built-I
+000200e0: 6e73 0a0a 6060 607b 636f 6e74 656e 7473  ns..```{contents
+000200f0: 7d0a 2d2d 2d0a 6c6f 6361 6c3a 0a64 6570  }.---.local:.dep
+00020100: 7468 3a20 320a 2d2d 2d0a 6060 600a 0a23  th: 2.---.```..#
+00020110: 2323 2042 7569 6c74 2d49 6e20 4675 6e63  ## Built-In Func
+00020120: 7469 6f6e 2044 6563 6f72 6174 6f72 730a  tion Decorators.
+00020130: 0a60 6060 7b63 6f6e 7465 6e74 737d 0a2d  .```{contents}.-
+00020140: 2d2d 0a6c 6f63 616c 3a0a 6465 7074 683a  --.local:.depth:
+00020150: 2031 0a2d 2d2d 0a60 6060 0a0a 2323 2323   1.---.```..####
+00020160: 2060 6164 6470 6174 7465 726e 600a 0a2a   `addpattern`..*
+00020170: 2a61 6464 7061 7474 6572 6e2a 2a28 5f62  *addpattern**(_b
+00020180: 6173 655c 5f66 756e 635f 2c20 2a5f 6164  ase\_func_, *_ad
+00020190: 645c 5f66 756e 6373 5f2c 205f 616c 6c6f  d\_funcs_, _allo
+000201a0: 775c 5f61 6e79 5c5f 6675 6e63 5f3d 6046  w\_any\_func_=`F
+000201b0: 616c 7365 6029 0a0a 5461 6b65 7320 6f6e  alse`)..Takes on
+000201c0: 6520 6172 6775 6d65 6e74 2074 6861 7420  e argument that 
+000201d0: 6973 2061 205b 7061 7474 6572 6e2d 6d61  is a [pattern-ma
+000201e0: 7463 6869 6e67 2066 756e 6374 696f 6e5d  tching function]
+000201f0: 2823 7061 7474 6572 6e2d 6d61 7463 6869  (#pattern-matchi
+00020200: 6e67 2d66 756e 6374 696f 6e73 292c 2061  ng-functions), a
+00020210: 6e64 2072 6574 7572 6e73 2061 2064 6563  nd returns a dec
+00020220: 6f72 6174 6f72 2074 6861 7420 6164 6473  orator that adds
+00020230: 2074 6865 2070 6174 7465 726e 7320 696e   the patterns in
+00020240: 2074 6865 2065 7869 7374 696e 6720 6675   the existing fu
+00020250: 6e63 7469 6f6e 2074 6f20 7468 6520 6e65  nction to the ne
+00020260: 7720 6675 6e63 7469 6f6e 2062 6569 6e67  w function being
+00020270: 2064 6563 6f72 6174 6564 2c20 7768 6572   decorated, wher
+00020280: 6520 7468 6520 6578 6973 7469 6e67 2070  e the existing p
+00020290: 6174 7465 726e 7320 6172 6520 6368 6563  atterns are chec
+000202a0: 6b65 6420 6669 7273 742c 2074 6865 6e20  ked first, then 
+000202b0: 7468 6520 6e65 772e 2060 6164 6470 6174  the new. `addpat
+000202c0: 7465 726e 6020 616c 736f 2073 7570 706f  tern` also suppo
+000202d0: 7274 7320 6120 7368 6f72 7463 7574 2073  rts a shortcut s
+000202e0: 796e 7461 7820 7768 6572 6520 7468 6520  yntax where the 
+000202f0: 6e65 7720 7061 7474 6572 6e73 2063 616e  new patterns can
+00020300: 2062 6520 7061 7373 6564 2069 6e20 6469   be passed in di
+00020310: 7265 6374 6c79 2e0a 0a52 6f75 6768 6c79  rectly...Roughly
+00020320: 2065 7175 6976 616c 656e 7420 746f 3a0a   equivalent to:.
+00020330: 6060 600a 6465 6620 5f70 6174 7465 726e  ```.def _pattern
+00020340: 5f61 6464 6572 2862 6173 655f 6675 6e63  _adder(base_func
+00020350: 2c20 6164 645f 6675 6e63 293a 0a20 2020  , add_func):.   
+00020360: 2064 6566 2061 6464 5f70 6174 7465 726e   def add_pattern
+00020370: 5f66 756e 6328 2a61 7267 732c 202a 2a6b  _func(*args, **k
+00020380: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
+00020390: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+000203a0: 2072 6574 7572 6e20 6261 7365 5f66 756e   return base_fun
+000203b0: 6328 2a61 7267 732c 202a 2a6b 7761 7267  c(*args, **kwarg
+000203c0: 7329 0a20 2020 2020 2020 2065 7863 6570  s).        excep
+000203d0: 7420 4d61 7463 6845 7272 6f72 3a0a 2020  t MatchError:.  
+000203e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000203f0: 2061 6464 5f66 756e 6328 2a61 7267 732c   add_func(*args,
+00020400: 202a 2a6b 7761 7267 7329 0a20 2020 2072   **kwargs).    r
+00020410: 6574 7572 6e20 6164 645f 7061 7474 6572  eturn add_patter
+00020420: 6e5f 6675 6e63 0a64 6566 2061 6464 7061  n_func.def addpa
+00020430: 7474 6572 6e28 6261 7365 5f66 756e 632c  ttern(base_func,
+00020440: 202a 6164 645f 6675 6e63 732c 2061 6c6c   *add_funcs, all
+00020450: 6f77 5f61 6e79 5f66 756e 633d 4661 6c73  ow_any_func=Fals
+00020460: 6529 3a0a 2020 2020 2222 2244 6563 6f72  e):.    """Decor
+00020470: 6174 6f72 2074 6f20 6164 6420 6120 6e65  ator to add a ne
+00020480: 7720 6361 7365 2074 6f20 6120 7061 7474  w case to a patt
+00020490: 6572 6e2d 6d61 7463 6869 6e67 2066 756e  ern-matching fun
+000204a0: 6374 696f 6e20 2877 6865 7265 2074 6865  ction (where the
+000204b0: 206e 6577 2063 6173 6520 6973 2063 6865   new case is che
+000204c0: 636b 6564 206c 6173 7429 2e0a 0a20 2020  cked last)...   
+000204d0: 2050 6173 7320 616c 6c6f 775f 616e 795f   Pass allow_any_
+000204e0: 6675 6e63 3d54 7275 6520 746f 2061 6c6c  func=True to all
+000204f0: 6f77 2061 6e79 206f 626a 6563 7420 6173  ow any object as
+00020500: 2074 6865 2062 6173 655f 6675 6e63 2072   the base_func r
+00020510: 6174 6865 7220 7468 616e 206a 7573 7420  ather than just 
+00020520: 7061 7474 6572 6e2d 6d61 7463 6869 6e67  pattern-matching
+00020530: 2066 756e 6374 696f 6e73 2e0a 2020 2020   functions..    
+00020540: 4966 2061 6464 5f66 756e 6320 6973 2070  If add_func is p
+00020550: 6173 7365 642c 2061 6464 7061 7474 6572  assed, addpatter
+00020560: 6e28 6261 7365 5f66 756e 632c 2061 6464  n(base_func, add
+00020570: 5f66 756e 6329 2069 7320 6571 7569 7661  _func) is equiva
+00020580: 6c65 6e74 2074 6f20 6164 6470 6174 7465  lent to addpatte
+00020590: 726e 2862 6173 655f 6675 6e63 2928 6164  rn(base_func)(ad
+000205a0: 645f 6675 6e63 292e 0a20 2020 2022 2222  d_func)..    """
+000205b0: 0a20 2020 2069 6620 6e6f 7420 6164 645f  .    if not add_
+000205c0: 6675 6e63 733a 0a20 2020 2020 2020 2072  funcs:.        r
+000205d0: 6574 7572 6e20 6164 6470 6174 7465 726e  eturn addpattern
+000205e0: 2428 6261 7365 5f66 756e 6329 0a20 2020  $(base_func).   
+000205f0: 2066 6f72 2061 6464 5f66 756e 6320 696e   for add_func in
+00020600: 2061 6464 5f66 756e 6373 3a0a 2020 2020   add_funcs:.    
+00020610: 2020 2020 6261 7365 5f66 756e 6320 3d20      base_func = 
+00020620: 7061 7474 6572 6e5f 6164 6465 7228 6261  pattern_adder(ba
+00020630: 7365 5f66 756e 632c 2061 6464 5f66 756e  se_func, add_fun
+00020640: 6329 0a20 2020 2072 6574 7572 6e20 6261  c).    return ba
+00020650: 7365 5f66 756e 630a 6060 600a 0a49 6620  se_func.```..If 
+00020660: 796f 7520 7761 6e74 2074 6f20 6769 7665  you want to give
+00020670: 2061 6e20 6061 6464 7061 7474 6572 6e60   an `addpattern`
+00020680: 2066 756e 6374 696f 6e20 6120 646f 6373   function a docs
+00020690: 7472 696e 672c 206d 616b 6520 7375 7265  tring, make sure
+000206a0: 2074 6f20 7075 7420 6974 206f 6e20 7468   to put it on th
+000206b0: 6520 5f6c 6173 745f 2066 756e 6374 696f  e _last_ functio
+000206c0: 6e2e 0a0a 4e6f 7465 2074 6861 7420 7468  n...Note that th
+000206d0: 6520 6675 6e63 7469 6f6e 2074 616b 656e  e function taken
+000206e0: 2062 7920 6061 6464 7061 7474 6572 6e60   by `addpattern`
+000206f0: 206d 7573 7420 6265 2061 2070 6174 7465   must be a patte
+00020700: 726e 2d6d 6174 6368 696e 6720 6675 6e63  rn-matching func
+00020710: 7469 6f6e 2e20 4966 2060 6164 6470 6174  tion. If `addpat
+00020720: 7465 726e 6020 7265 6365 6976 6573 2061  tern` receives a
+00020730: 206e 6f6e 2070 6174 7465 726e 2d6d 6174   non pattern-mat
+00020740: 6368 696e 6720 6675 6e63 7469 6f6e 2c20  ching function, 
+00020750: 7468 6520 6675 6e63 7469 6f6e 2077 6974  the function wit
+00020760: 6820 6e6f 7420 7261 6973 6520 604d 6174  h not raise `Mat
+00020770: 6368 4572 726f 7260 2c20 616e 6420 6061  chError`, and `a
+00020780: 6464 7061 7474 6572 6e60 2077 6f6e 2774  ddpattern` won't
+00020790: 2062 6520 6162 6c65 2074 6f20 6465 7465   be able to dete
+000207a0: 6374 2074 6865 2066 6169 6c65 6420 6d61  ct the failed ma
+000207b0: 7463 682e 2054 6875 732c 2069 6620 6120  tch. Thus, if a 
+000207c0: 6c61 7465 7220 6675 6e63 7469 6f6e 2077  later function w
+000207d0: 6173 206d 6561 6e74 2074 6f20 6265 2063  as meant to be c
+000207e0: 616c 6c65 642c 2060 6164 6470 6174 7465  alled, `addpatte
+000207f0: 726e 6020 7769 6c6c 206e 6f74 206b 6e6f  rn` will not kno
+00020800: 7720 7468 6174 2074 6865 2066 6972 7374  w that the first
+00020810: 206d 6174 6368 2066 6169 6c65 6420 616e   match failed an
+00020820: 6420 7468 6520 636f 7272 6563 7420 7061  d the correct pa
+00020830: 7468 2077 696c 6c20 6e65 7665 7220 6265  th will never be
+00020840: 2072 6561 6368 6564 2e0a 0a46 6f72 2065   reached...For e
+00020850: 7861 6d70 6c65 2c20 7468 6520 666f 6c6c  xample, the foll
+00020860: 6f77 696e 6720 636f 6465 2072 6169 7365  owing code raise
+00020870: 7320 6120 6054 7970 6545 7272 6f72 603a  s a `TypeError`:
+00020880: 0a60 6060 636f 636f 6e75 740a 6465 6620  .```coconut.def 
+00020890: 7072 696e 745f 7479 7065 2829 3a0a 2020  print_type():.  
+000208a0: 2020 7072 696e 7428 2252 6563 6569 7665    print("Receive
+000208b0: 6420 6e6f 2061 7267 756d 656e 7473 2e22  d no arguments."
+000208c0: 290a 0a40 6164 6470 6174 7465 726e 2870  )..@addpattern(p
+000208d0: 7269 6e74 5f74 7970 6529 0a64 6566 2070  rint_type).def p
+000208e0: 7269 6e74 5f74 7970 6528 696e 7428 2929  rint_type(int())
+000208f0: 3a0a 2020 2020 7072 696e 7428 2252 6563  :.    print("Rec
+00020900: 6569 7665 6420 616e 2069 6e74 2e22 290a  eived an int.").
+00020910: 0a70 7269 6e74 5f74 7970 6528 2920 2023  .print_type()  #
+00020920: 2061 7070 6561 7273 2074 6f20 776f 726b   appears to work
+00020930: 0a70 7269 6e74 5f74 7970 6528 3129 2023  .print_type(1) #
+00020940: 2054 7970 6545 7272 6f72 3a20 7072 696e   TypeError: prin
+00020950: 745f 7479 7065 2829 2074 616b 6573 2030  t_type() takes 0
+00020960: 2070 6f73 6974 696f 6e61 6c20 6172 6775   positional argu
+00020970: 6d65 6e74 7320 6275 7420 3120 7761 7320  ments but 1 was 
+00020980: 6769 7665 6e0a 6060 600a 0a54 6869 7320  given.```..This 
+00020990: 6361 6e20 6265 2066 6978 6564 2062 7920  can be fixed by 
+000209a0: 7573 696e 6720 6569 7468 6572 2074 6865  using either the
+000209b0: 2060 6d61 7463 6860 206f 7220 6061 6464   `match` or `add
+000209c0: 7061 7474 6572 6e60 206b 6579 776f 7264  pattern` keyword
+000209d0: 2e20 466f 7220 6578 616d 706c 653a 0a60  . For example:.`
+000209e0: 6060 636f 636f 6e75 740a 6d61 7463 6820  ``coconut.match 
+000209f0: 6465 6620 7072 696e 745f 7479 7065 2829  def print_type()
+00020a00: 3a0a 2020 2020 7072 696e 7428 2252 6563  :.    print("Rec
+00020a10: 6569 7665 6420 6e6f 2061 7267 756d 656e  eived no argumen
+00020a20: 7473 2e22 290a 0a61 6464 7061 7474 6572  ts.")..addpatter
+00020a30: 6e20 6465 6620 7072 696e 745f 7479 7065  n def print_type
+00020a40: 2869 6e74 2829 293a 0a20 2020 2070 7269  (int()):.    pri
+00020a50: 6e74 2822 5265 6365 6976 6564 2061 6e20  nt("Received an 
+00020a60: 696e 742e 2229 0a0a 7072 696e 745f 7479  int.")..print_ty
+00020a70: 7065 2831 2920 2023 2057 6f72 6b73 2061  pe(1)  # Works a
+00020a80: 7320 6578 7065 6374 6564 0a70 7269 6e74  s expected.print
+00020a90: 5f74 7970 6528 2254 6869 7320 6973 2061  _type("This is a
+00020aa0: 2073 7472 696e 672e 2229 2023 2052 6169   string.") # Rai
+00020ab0: 7365 7320 4d61 7463 6845 7272 6f72 0a60  ses MatchError.`
+00020ac0: 6060 0a0a 5468 6520 6c61 7374 2063 6173  ``..The last cas
+00020ad0: 6520 696e 2061 6e20 6061 6464 7061 7474  e in an `addpatt
+00020ae0: 6572 6e60 2066 756e 6374 696f 6e2c 2068  ern` function, h
+00020af0: 6f77 6576 6572 2c20 646f 6573 6e27 7420  owever, doesn't 
+00020b00: 6861 7665 2074 6f20 6265 2061 2070 6174  have to be a pat
+00020b10: 7465 726e 2d6d 6174 6368 696e 6720 6675  tern-matching fu
+00020b20: 6e63 7469 6f6e 2069 6620 6974 2069 7320  nction if it is 
+00020b30: 696e 7465 6e64 6564 2074 6f20 6361 7463  intended to catc
+00020b40: 6820 616c 6c20 7265 6d61 696e 696e 6720  h all remaining 
+00020b50: 6361 7365 732e 0a0a 546f 2063 6174 6368  cases...To catch
+00020b60: 2074 6869 7320 6d69 7374 616b 652c 2060   this mistake, `
+00020b70: 6164 6470 6174 7465 726e 6020 7769 6c6c  addpattern` will
+00020b80: 2065 6d69 7420 6120 7761 726e 696e 6720   emit a warning 
+00020b90: 6966 2070 6173 7365 6420 7768 6174 2069  if passed what i
+00020ba0: 7420 6265 6c69 6576 6573 2074 6f20 6265  t believes to be
+00020bb0: 2061 206e 6f6e 2d70 6174 7465 726e 2d6d   a non-pattern-m
+00020bc0: 6174 6368 696e 6720 6675 6e63 7469 6f6e  atching function
+00020bd0: 2e20 486f 7765 7665 722c 2074 6869 7320  . However, this 
+00020be0: 7761 726e 696e 6720 6361 6e20 736f 6d65  warning can some
+00020bf0: 7469 6d65 7320 6265 2065 7272 6f6e 656f  times be erroneo
+00020c00: 7573 2069 6620 7468 6520 6f72 6967 696e  us if the origin
+00020c10: 616c 2070 6174 7465 726e 2d6d 6174 6368  al pattern-match
+00020c20: 696e 6720 6675 6e63 7469 6f6e 2068 6173  ing function has
+00020c30: 2062 6565 6e20 7772 6170 7065 6420 696e   been wrapped in
+00020c40: 2073 6f6d 6520 7761 792c 2069 6e20 7768   some way, in wh
+00020c50: 6963 6820 6361 7365 2079 6f75 2063 616e  ich case you can
+00020c60: 2070 6173 7320 6061 6c6c 6f77 5f61 6e79   pass `allow_any
+00020c70: 5f66 756e 633d 5472 7565 6020 746f 2064  _func=True` to d
+00020c80: 6973 6d69 7373 2074 6865 2077 6172 6e69  ismiss the warni
+00020c90: 6e67 2e0a 0a23 2323 2323 2045 7861 6d70  ng...##### Examp
+00020ca0: 6c65 0a0a 2a2a 436f 636f 6e75 743a 2a2a  le..**Coconut:**
+00020cb0: 0a60 6060 636f 636f 6e75 740a 6465 6620  .```coconut.def 
+00020cc0: 6661 6374 6f72 6961 6c28 3029 203d 2031  factorial(0) = 1
+00020cd0: 0a0a 4061 6464 7061 7474 6572 6e28 6661  ..@addpattern(fa
+00020ce0: 6374 6f72 6961 6c29 0a64 6566 2066 6163  ctorial).def fac
+00020cf0: 746f 7269 616c 286e 2920 3d20 6e20 2a20  torial(n) = n * 
+00020d00: 6661 6374 6f72 6961 6c28 6e20 2d20 3129  factorial(n - 1)
+00020d10: 0a60 6060 0a5f 5369 6d70 6c65 2065 7861  .```._Simple exa
+00020d20: 6d70 6c65 206f 6620 6164 6469 6e67 2061  mple of adding a
+00020d30: 206e 6577 2070 6174 7465 726e 2074 6f20   new pattern to 
+00020d40: 6120 7061 7474 6572 6e2d 6d61 7463 6869  a pattern-matchi
+00020d50: 6e67 2066 756e 6374 696f 6e2e 5f0a 0a60  ng function._..`
+00020d60: 6060 636f 636f 6e75 740a 225b 415d 2c20  ``coconut."[A], 
+00020d70: 5b42 5d22 207c 3e20 7769 6e64 6f77 736f  [B]" |> windowso
+00020d80: 6624 2833 2920 7c3e 206d 6170 2428 6164  f$(3) |> map$(ad
+00020d90: 6470 6174 7465 726e 280a 2020 2020 2864  dpattern(.    (d
+00020da0: 6566 2028 2822 5b22 2c22 4122 2c22 5d22  ef (("[","A","]"
+00020db0: 2929 202d 3e20 2241 2229 2c0a 2020 2020  )) -> "A"),.    
+00020dc0: 2864 6566 2028 2822 5b22 2c22 4222 2c22  (def (("[","B","
+00020dd0: 5d22 2929 202d 3e20 2242 2229 2c0a 2020  ]")) -> "B"),.  
+00020de0: 2020 2864 6566 2028 285f 2c5f 2c5f 2929    (def ((_,_,_))
+00020df0: 202d 3e20 4e6f 6e65 292c 0a29 2920 7c3e   -> None),.)) |>
+00020e00: 2066 696c 7465 7224 2828 2e69 7320 4e6f   filter$((.is No
+00020e10: 6e65 2920 2e2e 3e20 286e 6f74 2929 207c  ne) ..> (not)) |
+00020e20: 3e20 6c69 7374 207c 3e20 7072 696e 740a  > list |> print.
+00020e30: 6060 600a 5f41 6e20 6578 616d 706c 6520  ```._An example 
+00020e40: 6f66 2061 2063 6173 6520 7768 6572 6520  of a case where 
+00020e50: 7573 696e 6720 7468 6520 6061 6464 7061  using the `addpa
+00020e60: 7474 6572 6e60 2066 756e 6374 696f 6e20  ttern` function 
+00020e70: 6973 206e 6563 6573 7361 7279 206f 7665  is necessary ove
+00020e80: 7220 7468 6520 5b60 6164 6470 6174 7465  r the [`addpatte
+00020e90: 726e 6020 6b65 7977 6f72 645d 2823 6164  rn` keyword](#ad
+00020ea0: 6470 6174 7465 726e 2d66 756e 6374 696f  dpattern-functio
+00020eb0: 6e73 2920 6475 6520 746f 2074 6865 2075  ns) due to the u
+00020ec0: 7365 206f 6620 696e 2d6c 696e 6520 7061  se of in-line pa
+00020ed0: 7474 6572 6e2d 6d61 7463 6869 6e67 205b  ttern-matching [
+00020ee0: 7374 6174 656d 656e 7420 6c61 6d62 6461  statement lambda
+00020ef0: 735d 2823 7374 6174 656d 656e 742d 6c61  s](#statement-la
+00020f00: 6d62 6461 7329 2e5f 0a0a 2a2a 5079 7468  mbdas)._..**Pyth
+00020f10: 6f6e 3a2a 2a0a 5f43 616e 2774 2062 6520  on:**._Can't be 
+00020f20: 646f 6e65 2077 6974 686f 7574 2061 2063  done without a c
+00020f30: 6f6d 706c 6963 6174 6564 2064 6563 6f72  omplicated decor
+00020f40: 6174 6f72 2064 6566 696e 6974 696f 6e20  ator definition 
+00020f50: 616e 6420 6120 6c6f 6e67 2073 6572 6965  and a long serie
+00020f60: 7320 6f66 2063 6865 636b 7320 666f 7220  s of checks for 
+00020f70: 6561 6368 2070 6174 7465 726e 2d6d 6174  each pattern-mat
+00020f80: 6368 696e 672e 2053 6565 2074 6865 2063  ching. See the c
+00020f90: 6f6d 7069 6c65 6420 636f 6465 2066 6f72  ompiled code for
+00020fa0: 2074 6865 2050 7974 686f 6e20 7379 6e74   the Python synt
+00020fb0: 6178 2e5f 0a0a 2323 2323 2320 6070 7265  ax._..##### `pre
+00020fc0: 7061 7474 6572 6e60 0a0a 2a2a 4445 5052  pattern`..**DEPR
+00020fd0: 4543 4154 4544 3a2a 2a20 436f 636f 6e75  ECATED:** Coconu
+00020fe0: 7420 616c 736f 2068 6173 2061 2060 7072  t also has a `pr
+00020ff0: 6570 6174 7465 726e 6020 6275 696c 742d  epattern` built-
+00021000: 696e 2c20 7768 6963 6820 6164 6473 2070  in, which adds p
+00021010: 6174 7465 726e 7320 696e 2074 6865 206f  atterns in the o
+00021020: 7070 6f73 6974 6520 6f72 6465 7220 6f66  pposite order of
+00021030: 2060 6164 6470 6174 7465 726e 603b 2060   `addpattern`; `
+00021040: 7072 6570 6174 7465 726e 6020 6973 2064  prepattern` is d
+00021050: 6566 696e 6564 2061 733a 0a0a 6060 6063  efined as:..```c
+00021060: 6f63 6f6e 7574 5f70 7974 686f 6e0a 6465  oconut_python.de
+00021070: 6620 7072 6570 6174 7465 726e 2862 6173  f prepattern(bas
+00021080: 655f 6675 6e63 293a 0a20 2020 2022 2222  e_func):.    """
+00021090: 4465 636f 7261 746f 7220 746f 2061 6464  Decorator to add
+000210a0: 2061 206e 6577 2063 6173 6520 746f 2061   a new case to a
+000210b0: 2070 6174 7465 726e 2d6d 6174 6368 696e   pattern-matchin
+000210c0: 6720 6675 6e63 7469 6f6e 2c0a 2020 2020  g function,.    
+000210d0: 7768 6572 6520 7468 6520 6e65 7720 6361  where the new ca
+000210e0: 7365 2069 7320 6368 6563 6b65 6420 6669  se is checked fi
+000210f0: 7273 742e 2222 220a 2020 2020 6465 6620  rst.""".    def 
+00021100: 7061 7474 6572 6e5f 7072 6570 656e 6465  pattern_prepende
+00021110: 7228 6675 6e63 293a 0a20 2020 2020 2020  r(func):.       
+00021120: 2072 6574 7572 6e20 6164 6470 6174 7465   return addpatte
+00021130: 726e 2866 756e 6329 2862 6173 655f 6675  rn(func)(base_fu
+00021140: 6e63 290a 2020 2020 7265 7475 726e 2070  nc).    return p
+00021150: 6174 7465 726e 5f70 7265 7065 6e64 6572  attern_prepender
+00021160: 0a60 6060 0a5f 4e6f 7465 3a20 5061 7373  .```._Note: Pass
+00021170: 696e 6720 602d 2d73 7472 6963 7460 2064  ing `--strict` d
+00021180: 6973 6162 6c65 7320 6465 7072 6563 6174  isables deprecat
+00021190: 6564 2066 6561 7475 7265 732e 5f0a 0a23  ed features._..#
+000211a0: 2323 2320 606d 656d 6f69 7a65 600a 0a2a  ### `memoize`..*
+000211b0: 2a6d 656d 6f69 7a65 2a2a 285f 6d61 7873  *memoize**(_maxs
+000211c0: 697a 655f 3d60 4e6f 6e65 602c 205f 7479  ize_=`None`, _ty
+000211d0: 7065 645f 3d60 4661 6c73 6560 290a 0a2a  ped_=`False`)..*
+000211e0: 2a6d 656d 6f69 7a65 2a2a 285f 7573 6572  *memoize**(_user
+000211f0: 5c5f 6675 6e63 7469 6f6e 5f29 0a0a 436f  \_function_)..Co
+00021200: 636f 6e75 7420 7072 6f76 6964 6573 2060  conut provides `
+00021210: 6675 6e63 746f 6f6c 732e 6c72 755f 6361  functools.lru_ca
+00021220: 6368 6560 2061 7320 6120 6275 696c 742d  che` as a built-
+00021230: 696e 2075 6e64 6572 2074 6865 206e 616d  in under the nam
+00021240: 6520 606d 656d 6f69 7a65 6020 7769 7468  e `memoize` with
+00021250: 2074 6865 206d 6f64 6966 6963 6174 696f   the modificatio
+00021260: 6e20 7468 6174 2074 6865 205f 6d61 7873  n that the _maxs
+00021270: 697a 655f 2070 6172 616d 6574 6572 2069  ize_ parameter i
+00021280: 7320 7365 7420 746f 2060 4e6f 6e65 6020  s set to `None` 
+00021290: 6279 2064 6566 6175 6c74 2e20 606d 656d  by default. `mem
+000212a0: 6f69 7a65 6020 6d61 6b65 7320 7468 6520  oize` makes the 
+000212b0: 7573 6520 6361 7365 206f 6620 6f70 7469  use case of opti
+000212c0: 6d69 7a69 6e67 2072 6563 7572 7369 7665  mizing recursive
+000212d0: 2066 756e 6374 696f 6e73 2065 6173 6965   functions easie
+000212e0: 722c 2061 7320 6120 5f6d 6178 7369 7a65  r, as a _maxsize
+000212f0: 5f20 6f66 2060 4e6f 6e65 6020 6973 2075  _ of `None` is u
+00021300: 7375 616c 6c79 2077 6861 7420 6973 2064  sually what is d
+00021310: 6573 6972 6564 2069 6e20 7468 6174 2063  esired in that c
+00021320: 6173 652e 0a0a 5573 6520 6f66 2060 6d65  ase...Use of `me
+00021330: 6d6f 697a 6560 2072 6571 7569 7265 7320  moize` requires 
+00021340: 6066 756e 6374 6f6f 6c73 2e6c 7275 5f63  `functools.lru_c
+00021350: 6163 6865 602c 2077 6869 6368 2065 7869  ache`, which exi
+00021360: 7374 7320 696e 2074 6865 2050 7974 686f  sts in the Pytho
+00021370: 6e20 3320 7374 616e 6461 7264 206c 6962  n 3 standard lib
+00021380: 7261 7279 2c20 6275 7420 756e 6465 7220  rary, but under 
+00021390: 5079 7468 6f6e 2032 2077 696c 6c20 7265  Python 2 will re
+000213a0: 7175 6972 6520 6070 6970 2069 6e73 7461  quire `pip insta
+000213b0: 6c6c 2062 6163 6b70 6f72 7473 2e66 756e  ll backports.fun
+000213c0: 6374 6f6f 6c73 5f6c 7275 5f63 6163 6865  ctools_lru_cache
+000213d0: 6020 746f 2066 756e 6374 696f 6e2e 2041  ` to function. A
+000213e0: 6464 6974 696f 6e61 6c6c 792c 2069 6620  dditionally, if 
+000213f0: 6f6e 2050 7974 686f 6e20 3220 616e 6420  on Python 2 and 
+00021400: 6062 6163 6b70 6f72 7473 2e66 756e 6374  `backports.funct
+00021410: 6f6f 6c73 5f6c 7275 5f63 6163 6865 6020  ools_lru_cache` 
+00021420: 6973 2070 7265 7365 6e74 2c20 436f 636f  is present, Coco
+00021430: 6e75 7420 7769 6c6c 2070 6174 6368 2060  nut will patch `
+00021440: 6675 6e63 746f 6f6c 7360 2073 7563 6820  functools` such 
+00021450: 7468 6174 2060 6675 6e63 746f 6f6c 732e  that `functools.
+00021460: 6c72 755f 6361 6368 6520 3d20 6261 636b  lru_cache = back
+00021470: 706f 7274 732e 6675 6e63 746f 6f6c 735f  ports.functools_
+00021480: 6c72 755f 6361 6368 652e 6c72 755f 6361  lru_cache.lru_ca
+00021490: 6368 6560 2e0a 0a23 2323 2323 2050 7974  che`...##### Pyt
+000214a0: 686f 6e20 446f 6373 0a0a 402a 2a6d 656d  hon Docs..@**mem
+000214b0: 6f69 7a65 2a2a 285f 7573 6572 5c5f 6675  oize**(_user\_fu
+000214c0: 6e63 7469 6f6e 5f29 0a0a 402a 2a6d 656d  nction_)..@**mem
+000214d0: 6f69 7a65 2a2a 285f 6d61 7873 697a 653d  oize**(_maxsize=
+000214e0: 4e6f 6e65 2c20 7479 7065 643d 4661 6c73  None, typed=Fals
+000214f0: 655f 290a 0a44 6563 6f72 6174 6f72 2074  e_)..Decorator t
+00021500: 6f20 7772 6170 2061 2066 756e 6374 696f  o wrap a functio
+00021510: 6e20 7769 7468 2061 206d 656d 6f69 7a69  n with a memoizi
+00021520: 6e67 2063 616c 6c61 626c 6520 7468 6174  ng callable that
+00021530: 2073 6176 6573 2075 7020 746f 2074 6865   saves up to the
+00021540: 205f 6d61 7873 697a 655f 206d 6f73 7420   _maxsize_ most 
+00021550: 7265 6365 6e74 2063 616c 6c73 2e20 4974  recent calls. It
+00021560: 2063 616e 2073 6176 6520 7469 6d65 2077   can save time w
+00021570: 6865 6e20 616e 2065 7870 656e 7369 7665  hen an expensive
+00021580: 206f 7220 492f 4f20 626f 756e 6420 6675   or I/O bound fu
+00021590: 6e63 7469 6f6e 2069 7320 7065 7269 6f64  nction is period
+000215a0: 6963 616c 6c79 2063 616c 6c65 6420 7769  ically called wi
+000215b0: 7468 2074 6865 2073 616d 6520 6172 6775  th the same argu
+000215c0: 6d65 6e74 732e 0a0a 5369 6e63 6520 6120  ments...Since a 
+000215d0: 6469 6374 696f 6e61 7279 2069 7320 7573  dictionary is us
+000215e0: 6564 2074 6f20 6361 6368 6520 7265 7375  ed to cache resu
+000215f0: 6c74 732c 2074 6865 2070 6f73 6974 696f  lts, the positio
+00021600: 6e61 6c20 616e 6420 6b65 7977 6f72 6420  nal and keyword 
+00021610: 6172 6775 6d65 6e74 7320 746f 2074 6865  arguments to the
+00021620: 2066 756e 6374 696f 6e20 6d75 7374 2062   function must b
+00021630: 6520 6861 7368 6162 6c65 2e0a 0a44 6973  e hashable...Dis
+00021640: 7469 6e63 7420 6172 6775 6d65 6e74 2070  tinct argument p
+00021650: 6174 7465 726e 7320 6d61 7920 6265 2063  atterns may be c
+00021660: 6f6e 7369 6465 7265 6420 746f 2062 6520  onsidered to be 
+00021670: 6469 7374 696e 6374 2063 616c 6c73 2077  distinct calls w
+00021680: 6974 6820 7365 7061 7261 7465 2063 6163  ith separate cac
+00021690: 6865 2065 6e74 7269 6573 2e20 466f 7220  he entries. For 
+000216a0: 6578 616d 706c 652c 2060 6628 613d 312c  example, `f(a=1,
+000216b0: 2062 3d32 2960 2061 6e64 2060 6628 623d   b=2)` and `f(b=
+000216c0: 322c 2061 3d31 2960 2064 6966 6665 7220  2, a=1)` differ 
+000216d0: 696e 2074 6865 6972 206b 6579 776f 7264  in their keyword
+000216e0: 2061 7267 756d 656e 7420 6f72 6465 7220   argument order 
+000216f0: 616e 6420 6d61 7920 6861 7665 2074 776f  and may have two
+00021700: 2073 6570 6172 6174 6520 6361 6368 6520   separate cache 
+00021710: 656e 7472 6965 732e 0a0a 4966 205f 7573  entries...If _us
+00021720: 6572 5c5f 6675 6e63 7469 6f6e 5f20 6973  er\_function_ is
+00021730: 2073 7065 6369 6669 6564 2c20 6974 206d   specified, it m
+00021740: 7573 7420 6265 2061 2063 616c 6c61 626c  ust be a callabl
+00021750: 652e 2054 6869 7320 616c 6c6f 7773 2074  e. This allows t
+00021760: 6865 205f 6d65 6d6f 697a 655f 2064 6563  he _memoize_ dec
+00021770: 6f72 6174 6f72 2074 6f20 6265 2061 7070  orator to be app
+00021780: 6c69 6564 2064 6972 6563 746c 7920 746f  lied directly to
+00021790: 2061 2075 7365 7220 6675 6e63 7469 6f6e   a user function
+000217a0: 2c20 6c65 6176 696e 6720 7468 6520 6d61  , leaving the ma
+000217b0: 7873 697a 6520 6174 2069 7473 2064 6566  xsize at its def
+000217c0: 6175 6c74 2076 616c 7565 206f 6620 604e  ault value of `N
+000217d0: 6f6e 6560 3a0a 6060 6063 6f63 6f6e 7574  one`:.```coconut
+000217e0: 5f70 7974 686f 6e0a 406d 656d 6f69 7a65  _python.@memoize
+000217f0: 0a64 6566 2063 6f75 6e74 5f76 6f77 656c  .def count_vowel
+00021800: 7328 7365 6e74 656e 6365 293a 0a20 2020  s(sentence):.   
+00021810: 2072 6574 7572 6e20 7375 6d28 7365 6e74   return sum(sent
+00021820: 656e 6365 2e63 6f75 6e74 2876 6f77 656c  ence.count(vowel
+00021830: 2920 666f 7220 766f 7765 6c20 696e 2027  ) for vowel in '
+00021840: 4145 494f 5561 6569 6f75 2729 0a60 6060  AEIOUaeiou').```
+00021850: 0a0a 4966 205f 6d61 7873 697a 655f 2069  ..If _maxsize_ i
+00021860: 7320 7365 7420 746f 2060 4e6f 6e65 602c  s set to `None`,
+00021870: 2074 6865 204c 5255 2066 6561 7475 7265   the LRU feature
+00021880: 2069 7320 6469 7361 626c 6564 2061 6e64   is disabled and
+00021890: 2074 6865 2063 6163 6865 2063 616e 2067   the cache can g
+000218a0: 726f 7720 7769 7468 6f75 7420 626f 756e  row without boun
+000218b0: 642e 0a0a 4966 205f 7479 7065 645f 2069  d...If _typed_ i
+000218c0: 7320 7365 7420 746f 2074 7275 652c 2066  s set to true, f
+000218d0: 756e 6374 696f 6e20 6172 6775 6d65 6e74  unction argument
+000218e0: 7320 6f66 2064 6966 6665 7265 6e74 2074  s of different t
+000218f0: 7970 6573 2077 696c 6c20 6265 2063 6163  ypes will be cac
+00021900: 6865 6420 7365 7061 7261 7465 6c79 2e20  hed separately. 
+00021910: 4966 2074 7970 6564 2069 7320 6661 6c73  If typed is fals
+00021920: 652c 2074 6865 2069 6d70 6c65 6d65 6e74  e, the implement
+00021930: 6174 696f 6e20 7769 6c6c 2075 7375 616c  ation will usual
+00021940: 6c79 2072 6567 6172 6420 7468 656d 2061  ly regard them a
+00021950: 7320 6571 7569 7661 6c65 6e74 2063 616c  s equivalent cal
+00021960: 6c73 2061 6e64 206f 6e6c 7920 6361 6368  ls and only cach
+00021970: 6520 6120 7369 6e67 6c65 2072 6573 756c  e a single resul
+00021980: 742e 2028 536f 6d65 2074 7970 6573 2073  t. (Some types s
+00021990: 7563 6820 6173 2073 7472 2061 6e64 2069  uch as str and i
+000219a0: 6e74 206d 6179 2062 6520 6361 6368 6564  nt may be cached
+000219b0: 2073 6570 6172 6174 656c 7920 6576 656e   separately even
+000219c0: 2077 6865 6e20 7479 7065 6420 6973 2066   when typed is f
+000219d0: 616c 7365 2e29 0a0a 4e6f 7465 2c20 7479  alse.)..Note, ty
+000219e0: 7065 2073 7065 6369 6669 6369 7479 2061  pe specificity a
+000219f0: 7070 6c69 6573 206f 6e6c 7920 746f 2074  pplies only to t
+00021a00: 6865 2066 756e 6374 696f 6ee2 8099 7320  he function...s 
+00021a10: 696d 6d65 6469 6174 6520 6172 6775 6d65  immediate argume
+00021a20: 6e74 7320 7261 7468 6572 2074 6861 6e20  nts rather than 
+00021a30: 7468 6569 7220 636f 6e74 656e 7473 2e20  their contents. 
+00021a40: 5468 6520 7363 616c 6172 2061 7267 756d  The scalar argum
+00021a50: 656e 7473 2c20 6044 6563 696d 616c 2834  ents, `Decimal(4
+00021a60: 3229 6020 616e 6420 6046 7261 6374 696f  2)` and `Fractio
+00021a70: 6e28 3432 2960 2061 7265 2062 6520 7472  n(42)` are be tr
+00021a80: 6561 7465 6420 6173 2064 6973 7469 6e63  eated as distinc
+00021a90: 7420 6361 6c6c 7320 7769 7468 2064 6973  t calls with dis
+00021aa0: 7469 6e63 7420 7265 7375 6c74 732e 2049  tinct results. I
+00021ab0: 6e20 636f 6e74 7261 7374 2c20 7468 6520  n contrast, the 
+00021ac0: 7475 706c 6520 6172 6775 6d65 6e74 7320  tuple arguments 
+00021ad0: 6028 2761 6e73 7765 7227 2c20 4465 6369  `('answer', Deci
+00021ae0: 6d61 6c28 3432 2929 6020 616e 6420 6028  mal(42))` and `(
+00021af0: 2761 6e73 7765 7227 2c20 4672 6163 7469  'answer', Fracti
+00021b00: 6f6e 2834 3229 2960 2061 7265 2074 7265  on(42))` are tre
+00021b10: 6174 6564 2061 7320 6571 7569 7661 6c65  ated as equivale
+00021b20: 6e74 2e0a 0a54 6865 2064 6563 6f72 6174  nt...The decorat
+00021b30: 6f72 2061 6c73 6f20 7072 6f76 6964 6573  or also provides
+00021b40: 2061 2060 6361 6368 655f 636c 6561 7228   a `cache_clear(
+00021b50: 2960 2066 756e 6374 696f 6e20 666f 7220  )` function for 
+00021b60: 636c 6561 7269 6e67 206f 7220 696e 7661  clearing or inva
+00021b70: 6c69 6461 7469 6e67 2074 6865 2063 6163  lidating the cac
+00021b80: 6865 2e0a 0a54 6865 206f 7269 6769 6e61  he...The origina
+00021b90: 6c20 756e 6465 726c 7969 6e67 2066 756e  l underlying fun
+00021ba0: 6374 696f 6e20 6973 2061 6363 6573 7369  ction is accessi
+00021bb0: 626c 6520 7468 726f 7567 6820 7468 6520  ble through the 
+00021bc0: 605f 5f77 7261 7070 6564 5f5f 6020 6174  `__wrapped__` at
+00021bd0: 7472 6962 7574 652e 2054 6869 7320 6973  tribute. This is
+00021be0: 2075 7365 6675 6c20 666f 7220 696e 7472   useful for intr
+00021bf0: 6f73 7065 6374 696f 6e2c 2066 6f72 2062  ospection, for b
+00021c00: 7970 6173 7369 6e67 2074 6865 2063 6163  ypassing the cac
+00021c10: 6865 2c20 6f72 2066 6f72 2072 6577 7261  he, or for rewra
+00021c20: 7070 696e 6720 7468 6520 6675 6e63 7469  pping the functi
+00021c30: 6f6e 2077 6974 6820 6120 6469 6666 6572  on with a differ
+00021c40: 656e 7420 6361 6368 652e 0a0a 5468 6520  ent cache...The 
+00021c50: 6361 6368 6520 6b65 6570 7320 7265 6665  cache keeps refe
+00021c60: 7265 6e63 6573 2074 6f20 7468 6520 6172  rences to the ar
+00021c70: 6775 6d65 6e74 7320 616e 6420 7265 7475  guments and retu
+00021c80: 726e 2076 616c 7565 7320 756e 7469 6c20  rn values until 
+00021c90: 7468 6579 2061 6765 206f 7574 206f 6620  they age out of 
+00021ca0: 7468 6520 6361 6368 6520 6f72 2075 6e74  the cache or unt
+00021cb0: 696c 2074 6865 2063 6163 6865 2069 7320  il the cache is 
+00021cc0: 636c 6561 7265 642e 0a0a 4966 2061 206d  cleared...If a m
+00021cd0: 6574 686f 6420 6973 2063 6163 6865 642c  ethod is cached,
+00021ce0: 2074 6865 2060 7365 6c66 6020 696e 7374   the `self` inst
+00021cf0: 616e 6365 2061 7267 756d 656e 7420 6973  ance argument is
+00021d00: 2069 6e63 6c75 6465 6420 696e 2074 6865   included in the
+00021d10: 2063 6163 6865 2e20 5365 6520 5b48 6f77   cache. See [How
+00021d20: 2064 6f20 4920 6361 6368 6520 6d65 7468   do I cache meth
+00021d30: 6f64 2063 616c 6c73 3f5d 2868 7474 7073  od calls?](https
+00021d40: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
+00021d50: 7267 2f33 2f66 6171 2f70 726f 6772 616d  rg/3/faq/program
+00021d60: 6d69 6e67 2e68 746d 6c23 6661 712d 6361  ming.html#faq-ca
+00021d70: 6368 652d 6d65 7468 6f64 2d63 616c 6c73  che-method-calls
+00021d80: 290a 0a41 6e20 5b4c 5255 2028 6c65 6173  )..An [LRU (leas
+00021d90: 7420 7265 6365 6e74 6c79 2075 7365 6429  t recently used)
+00021da0: 2063 6163 6865 5d28 6874 7470 733a 2f2f   cache](https://
+00021db0: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
+00021dc0: 2f77 696b 692f 4361 6368 655f 7265 706c  /wiki/Cache_repl
+00021dd0: 6163 656d 656e 745f 706f 6c69 6369 6573  acement_policies
+00021de0: 234c 6561 7374 5f72 6563 656e 746c 795f  #Least_recently_
+00021df0: 7573 6564 5f28 4c52 5529 2920 776f 726b  used_(LRU)) work
+00021e00: 7320 6265 7374 2077 6865 6e20 7468 6520  s best when the 
+00021e10: 6d6f 7374 2072 6563 656e 7420 6361 6c6c  most recent call
+00021e20: 7320 6172 6520 7468 6520 6265 7374 2070  s are the best p
+00021e30: 7265 6469 6374 6f72 7320 6f66 2075 7063  redictors of upc
+00021e40: 6f6d 696e 6720 6361 6c6c 7320 2866 6f72  oming calls (for
+00021e50: 2065 7861 6d70 6c65 2c20 7468 6520 6d6f   example, the mo
+00021e60: 7374 2070 6f70 756c 6172 2061 7274 6963  st popular artic
+00021e70: 6c65 7320 6f6e 2061 206e 6577 7320 7365  les on a news se
+00021e80: 7276 6572 2074 656e 6420 746f 2063 6861  rver tend to cha
+00021e90: 6e67 6520 6561 6368 2064 6179 292e 2054  nge each day). T
+00021ea0: 6865 2063 6163 6865 e280 9973 2073 697a  he cache...s siz
+00021eb0: 6520 6c69 6d69 7420 6173 7375 7265 7320  e limit assures 
+00021ec0: 7468 6174 2074 6865 2063 6163 6865 2064  that the cache d
+00021ed0: 6f65 7320 6e6f 7420 6772 6f77 2077 6974  oes not grow wit
+00021ee0: 686f 7574 2062 6f75 6e64 206f 6e20 6c6f  hout bound on lo
+00021ef0: 6e67 2d72 756e 6e69 6e67 2070 726f 6365  ng-running proce
+00021f00: 7373 6573 2073 7563 6820 6173 2077 6562  sses such as web
+00021f10: 2073 6572 7665 7273 2e0a 0a49 6e20 6765   servers...In ge
+00021f20: 6e65 7261 6c2c 2074 6865 204c 5255 2063  neral, the LRU c
+00021f30: 6163 6865 2073 686f 756c 6420 6f6e 6c79  ache should only
+00021f40: 2062 6520 7573 6564 2077 6865 6e20 796f   be used when yo
+00021f50: 7520 7761 6e74 2074 6f20 7265 7573 6520  u want to reuse 
+00021f60: 7072 6576 696f 7573 6c79 2063 6f6d 7075  previously compu
+00021f70: 7465 6420 7661 6c75 6573 2e20 4163 636f  ted values. Acco
+00021f80: 7264 696e 676c 792c 2069 7420 646f 6573  rdingly, it does
+00021f90: 6ee2 8099 7420 6d61 6b65 2073 656e 7365  n...t make sense
+00021fa0: 2074 6f20 6361 6368 6520 6675 6e63 7469   to cache functi
+00021fb0: 6f6e 7320 7769 7468 2073 6964 652d 6566  ons with side-ef
+00021fc0: 6665 6374 732c 2066 756e 6374 696f 6e73  fects, functions
+00021fd0: 2074 6861 7420 6e65 6564 2074 6f20 6372   that need to cr
+00021fe0: 6561 7465 2064 6973 7469 6e63 7420 6d75  eate distinct mu
+00021ff0: 7461 626c 6520 6f62 6a65 6374 7320 6f6e  table objects on
+00022000: 2065 6163 6820 6361 6c6c 2c20 6f72 2069   each call, or i
+00022010: 6d70 7572 6520 6675 6e63 7469 6f6e 7320  mpure functions 
+00022020: 7375 6368 2061 7320 7469 6d65 2829 206f  such as time() o
+00022030: 7220 7261 6e64 6f6d 2829 2e0a 0a45 7861  r random()...Exa
+00022040: 6d70 6c65 206f 6620 6566 6669 6369 656e  mple of efficien
+00022050: 746c 7920 636f 6d70 7574 696e 6720 4669  tly computing Fi
+00022060: 626f 6e61 6363 6920 6e75 6d62 6572 7320  bonacci numbers 
+00022070: 7573 696e 6720 6120 6361 6368 6520 746f  using a cache to
+00022080: 2069 6d70 6c65 6d65 6e74 2061 2064 796e   implement a dyn
+00022090: 616d 6963 2070 726f 6772 616d 6d69 6e67  amic programming
+000220a0: 2074 6563 686e 6971 7565 3a0a 6060 6063   technique:.```c
+000220b0: 6f63 6f6e 7574 5f70 7963 6f6e 0a40 6d65  oconut_pycon.@me
+000220c0: 6d6f 697a 650a 6465 6620 6669 6228 6e29  moize.def fib(n)
+000220d0: 3a0a 2020 2020 6966 206e 203c 2032 3a0a  :.    if n < 2:.
+000220e0: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+000220f0: 0a20 2020 2072 6574 7572 6e20 6669 6228  .    return fib(
+00022100: 6e2d 3129 202b 2066 6962 286e 2d32 290a  n-1) + fib(n-2).
+00022110: 0a3e 3e3e 205b 6669 6228 6e29 2066 6f72  .>>> [fib(n) for
+00022120: 206e 2069 6e20 7261 6e67 6528 3136 295d   n in range(16)]
+00022130: 0a5b 302c 2031 2c20 312c 2032 2c20 332c  .[0, 1, 1, 2, 3,
+00022140: 2035 2c20 382c 2031 332c 2032 312c 2033   5, 8, 13, 21, 3
+00022150: 342c 2035 352c 2038 392c 2031 3434 2c20  4, 55, 89, 144, 
+00022160: 3233 332c 2033 3737 2c20 3631 305d 0a0a  233, 377, 610]..
+00022170: 3e3e 3e20 6669 622e 6361 6368 655f 696e  >>> fib.cache_in
+00022180: 666f 2829 0a43 6163 6865 496e 666f 2868  fo().CacheInfo(h
+00022190: 6974 733d 3238 2c20 6d69 7373 6573 3d31  its=28, misses=1
+000221a0: 362c 206d 6178 7369 7a65 3d4e 6f6e 652c  6, maxsize=None,
+000221b0: 2063 7572 7273 697a 653d 3136 290a 6060   currsize=16).``
+000221c0: 600a 0a23 2323 2323 2045 7861 6d70 6c65  `..##### Example
+000221d0: 0a0a 2a2a 436f 636f 6e75 743a 2a2a 0a60  ..**Coconut:**.`
+000221e0: 6060 636f 636f 6e75 740a 6465 6620 6669  ``coconut.def fi
+000221f0: 6228 6e20 6966 206e 203c 2032 2920 3d20  b(n if n < 2) = 
+00022200: 6e0a 0a40 6d65 6d6f 697a 650a 4061 6464  n..@memoize.@add
+00022210: 7061 7474 6572 6e28 6669 6229 0a64 6566  pattern(fib).def
+00022220: 2066 6962 286e 2920 3d20 6669 6228 6e2d   fib(n) = fib(n-
+00022230: 3129 202b 2066 6962 286e 2d32 290a 6060  1) + fib(n-2).``
+00022240: 600a 0a2a 2a50 7974 686f 6e3a 2a2a 0a60  `..**Python:**.`
+00022250: 6060 636f 636f 6e75 745f 7079 7468 6f6e  ``coconut_python
+00022260: 0a74 7279 3a0a 2020 2020 6672 6f6d 2066  .try:.    from f
+00022270: 756e 6374 6f6f 6c73 2069 6d70 6f72 7420  unctools import 
+00022280: 6c72 755f 6361 6368 650a 6578 6365 7074  lru_cache.except
+00022290: 2049 6d70 6f72 7445 7272 6f72 3a0a 2020   ImportError:.  
+000222a0: 2020 6672 6f6d 2062 6163 6b70 6f72 7473    from backports
+000222b0: 2e66 756e 6374 6f6f 6c73 5f6c 7275 5f63  .functools_lru_c
+000222c0: 6163 6865 2069 6d70 6f72 7420 6c72 755f  ache import lru_
+000222d0: 6361 6368 650a 406c 7275 5f63 6163 6865  cache.@lru_cache
+000222e0: 286d 6178 7369 7a65 3d4e 6f6e 6529 0a64  (maxsize=None).d
+000222f0: 6566 2066 6962 286e 293a 0a20 2020 2069  ef fib(n):.    i
+00022300: 6620 6e20 3c20 323a 0a20 2020 2020 2020  f n < 2:.       
+00022310: 2072 6574 7572 6e20 6e0a 2020 2020 7265   return n.    re
+00022320: 7475 726e 2066 6962 286e 2d31 2920 2b20  turn fib(n-1) + 
+00022330: 6669 6228 6e2d 3229 0a60 6060 0a0a 2323  fib(n-2).```..##
+00022340: 2323 2060 6f76 6572 7269 6465 600a 0a2a  ## `override`..*
+00022350: 2a6f 7665 7272 6964 652a 2a28 5f66 756e  *override**(_fun
+00022360: 635f 290a 0a43 6f63 6f6e 7574 2070 726f  c_)..Coconut pro
+00022370: 7669 6465 7320 7468 6520 6040 6f76 6572  vides the `@over
+00022380: 7269 6465 6020 6465 636f 7261 746f 7220  ride` decorator 
+00022390: 746f 2061 6c6c 6f77 2064 6563 6c61 7269  to allow declari
+000223a0: 6e67 2061 206d 6574 686f 6420 6465 6669  ng a method defi
+000223b0: 6e69 7469 6f6e 2069 6e20 6120 7375 6263  nition in a subc
+000223c0: 6c61 7373 2061 7320 616e 206f 7665 7272  lass as an overr
+000223d0: 6964 6520 6f66 2073 6f6d 6520 7061 7265  ide of some pare
+000223e0: 6e74 2063 6c61 7373 206d 6574 686f 642e  nt class method.
+000223f0: 2057 6865 6e20 6040 6f76 6572 7269 6465   When `@override
+00022400: 6020 6973 2075 7365 6420 6f6e 2061 206d  ` is used on a m
+00022410: 6574 686f 642c 2069 6620 6120 6d65 7468  ethod, if a meth
+00022420: 6f64 206f 6620 7468 6520 7361 6d65 206e  od of the same n
+00022430: 616d 6520 646f 6573 206e 6f74 2065 7869  ame does not exi
+00022440: 7374 206f 6e20 736f 6d65 2070 6172 656e  st on some paren
+00022450: 7420 636c 6173 732c 2074 6865 2063 6c61  t class, the cla
+00022460: 7373 2064 6566 696e 6974 696f 6e20 7769  ss definition wi
+00022470: 6c6c 2072 6169 7365 2061 2060 5275 6e74  ll raise a `Runt
+00022480: 696d 6545 7272 6f72 602e 0a0a 4164 6469  imeError`...Addi
+00022490: 7469 6f6e 616c 6c79 2c20 606f 7665 7272  tionally, `overr
+000224a0: 6964 6560 2077 696c 6c20 7072 6573 656e  ide` will presen
+000224b0: 7420 746f 2074 7970 6520 6368 6563 6b65  t to type checke
+000224c0: 7273 2061 7320 5b60 7479 7069 6e67 5f65  rs as [`typing_e
+000224d0: 7874 656e 7369 6f6e 732e 6f76 6572 7269  xtensions.overri
+000224e0: 6465 605d 2868 7474 7073 3a2f 2f70 7970  de`](https://pyp
+000224f0: 692e 6f72 672f 7072 6f6a 6563 742f 7479  i.org/project/ty
+00022500: 7069 6e67 2d65 7874 656e 7369 6f6e 732f  ping-extensions/
+00022510: 292e 0a0a 2323 2323 2320 4578 616d 706c  )...##### Exampl
+00022520: 650a 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a  e..**Coconut:**.
+00022530: 6060 6063 6f63 6f6e 7574 0a63 6c61 7373  ```coconut.class
+00022540: 2041 3a0a 2020 2020 7820 3d20 310a 2020   A:.    x = 1.  
+00022550: 2020 6465 6620 6628 7365 6c66 2c20 7929    def f(self, y)
+00022560: 203d 2073 656c 662e 7820 2b20 790a 0a63   = self.x + y..c
+00022570: 6c61 7373 2042 3a0a 2020 2020 406f 7665  lass B:.    @ove
+00022580: 7272 6964 650a 2020 2020 6465 6620 6628  rride.    def f(
+00022590: 7365 6c66 2c20 7929 203d 2073 656c 662e  self, y) = self.
+000225a0: 7820 2b20 7920 2b20 310a 6060 600a 0a2a  x + y + 1.```..*
+000225b0: 2a50 7974 686f 6e3a 2a2a 0a5f 4361 6e27  *Python:**._Can'
+000225c0: 7420 6265 2064 6f6e 6520 7769 7468 6f75  t be done withou
+000225d0: 7420 6120 6c6f 6e67 2064 6563 6f72 6174  t a long decorat
+000225e0: 6f72 2064 6566 696e 6974 696f 6e2e 2054  or definition. T
+000225f0: 6865 2066 756c 6c20 6465 6669 6e69 7469  he full definiti
+00022600: 6f6e 206f 6620 7468 6520 6465 636f 7261  on of the decora
+00022610: 746f 7220 696e 2050 7974 686f 6e20 6361  tor in Python ca
+00022620: 6e20 6265 2066 6f75 6e64 2069 6e20 7468  n be found in th
+00022630: 6520 436f 636f 6e75 7420 6865 6164 6572  e Coconut header
+00022640: 2e5f 0a0a 2323 2323 2060 7265 6375 7273  ._..#### `recurs
+00022650: 6976 655f 6974 6572 6174 6f72 600a 0a2a  ive_iterator`..*
+00022660: 2a72 6563 7572 7369 7665 5c5f 6974 6572  *recursive\_iter
+00022670: 6174 6f72 2a2a 285f 6675 6e63 5f29 0a0a  ator**(_func_)..
+00022680: 436f 636f 6e75 7420 7072 6f76 6964 6573  Coconut provides
+00022690: 2061 2060 7265 6375 7273 6976 655f 6974   a `recursive_it
+000226a0: 6572 6174 6f72 6020 6465 636f 7261 746f  erator` decorato
+000226b0: 7220 7468 6174 206d 656d 6f69 7a65 7320  r that memoizes 
+000226c0: 616e 7920 7374 6174 656c 6573 732c 2072  any stateless, r
+000226d0: 6563 7572 7369 7665 2066 756e 6374 696f  ecursive functio
+000226e0: 6e20 7468 6174 2072 6574 7572 6e73 2061  n that returns a
+000226f0: 6e20 6974 6572 6174 6f72 2e20 546f 2075  n iterator. To u
+00022700: 7365 2060 7265 6375 7273 6976 655f 6974  se `recursive_it
+00022710: 6572 6174 6f72 6020 6f6e 2061 2066 756e  erator` on a fun
+00022720: 6374 696f 6e2c 2069 7420 6d75 7374 206d  ction, it must m
+00022730: 6565 7420 7468 6520 666f 6c6c 6f77 696e  eet the followin
+00022740: 6720 6372 6974 6572 6961 3a0a 0a31 2e20  g criteria:..1. 
+00022750: 796f 7572 2066 756e 6374 696f 6e20 6569  your function ei
+00022760: 7468 6572 2061 6c77 6179 7320 6072 6574  ther always `ret
+00022770: 7572 6e60 7320 616e 2069 7465 7261 746f  urn`s an iterato
+00022780: 7220 6f72 2067 656e 6572 6174 6573 2061  r or generates a
+00022790: 6e20 6974 6572 6174 6f72 2075 7369 6e67  n iterator using
+000227a0: 2060 7969 656c 6460 2c0a 322e 2077 6865   `yield`,.2. whe
+000227b0: 6e20 6361 6c6c 6564 206d 756c 7469 706c  n called multipl
+000227c0: 6520 7469 6d65 7320 7769 7468 2061 7267  e times with arg
+000227d0: 756d 656e 7473 2074 6861 7420 6172 6520  uments that are 
+000227e0: 6571 7561 6c2c 2079 6f75 7220 6675 6e63  equal, your func
+000227f0: 7469 6f6e 2070 726f 6475 6365 7320 7468  tion produces th
+00022800: 6520 7361 6d65 2069 7465 7261 746f 7220  e same iterator 
+00022810: 2879 6f75 7220 6675 6e63 7469 6f6e 2069  (your function i
+00022820: 7320 7374 6174 656c 6573 7329 2c20 616e  s stateless), an
+00022830: 640a 332e 2079 6f75 7220 6675 6e63 7469  d.3. your functi
+00022840: 6f6e 2067 6574 7320 6361 6c6c 6564 2028  on gets called (
+00022850: 7573 7561 6c6c 7920 6361 6c6c 7320 6974  usually calls it
+00022860: 7365 6c66 2920 6d75 6c74 6970 6c65 2074  self) multiple t
+00022870: 696d 6573 2077 6974 6820 7468 6520 7361  imes with the sa
+00022880: 6d65 2061 7267 756d 656e 7473 2e0a 0a49  me arguments...I
+00022890: 6620 796f 7520 6172 6520 656e 636f 756e  f you are encoun
+000228a0: 7465 7269 6e67 2061 2060 5275 6e74 696d  tering a `Runtim
+000228b0: 6545 7272 6f72 6020 6475 6520 746f 206d  eError` due to m
+000228c0: 6178 696d 756d 2072 6563 7572 7369 6f6e  aximum recursion
+000228d0: 2064 6570 7468 2c20 6974 2069 7320 6869   depth, it is hi
+000228e0: 6768 6c79 2072 6563 6f6d 6d65 6e64 6564  ghly recommended
+000228f0: 2074 6861 7420 796f 7520 7265 7772 6974   that you rewrit
+00022900: 6520 796f 7572 2066 756e 6374 696f 6e20  e your function 
+00022910: 746f 206d 6565 7420 6569 7468 6572 2074  to meet either t
+00022920: 6865 2063 7269 7465 7269 6120 6162 6f76  he criteria abov
+00022930: 6520 666f 7220 6072 6563 7572 7369 7665  e for `recursive
+00022940: 5f69 7465 7261 746f 7260 2c20 6f72 2074  _iterator`, or t
+00022950: 6865 2063 6f72 7265 7370 6f6e 6469 6e67  he corresponding
+00022960: 2063 7269 7465 7269 6120 666f 7220 436f   criteria for Co
+00022970: 636f 6e75 7427 7320 5b74 6169 6c20 6361  conut's [tail ca
+00022980: 6c6c 206f 7074 696d 697a 6174 696f 6e5d  ll optimization]
+00022990: 2823 7461 696c 2d63 616c 6c2d 6f70 7469  (#tail-call-opti
+000229a0: 6d69 7a61 7469 6f6e 292c 2065 6974 6865  mization), eithe
+000229b0: 7220 6f66 2077 6869 6368 2073 686f 756c  r of which shoul
+000229c0: 6420 7072 6576 656e 7420 7375 6368 2065  d prevent such e
+000229d0: 7272 6f72 732e 0a0a 4675 7274 6865 726d  rrors...Furtherm
+000229e0: 6f72 652c 2060 7265 6375 7273 6976 655f  ore, `recursive_
+000229f0: 6974 6572 6174 6f72 6020 616c 736f 2061  iterator` also a
+00022a00: 6c6c 6f77 7320 7468 6520 7265 736f 6c75  llows the resolu
+00022a10: 7469 6f6e 206f 6620 6120 5b6e 6173 7479  tion of a [nasty
+00022a20: 2073 6567 6d65 6e74 6174 696f 6e20 6661   segmentation fa
+00022a30: 756c 7420 696e 2050 7974 686f 6e27 7320  ult in Python's 
+00022a40: 6974 6572 6174 6f72 206c 6f67 6963 2074  iterator logic t
+00022a50: 6861 7420 6861 7320 6e65 7665 7220 6265  hat has never be
+00022a60: 656e 2066 6978 6564 5d28 6874 7470 3a2f  en fixed](http:/
+00022a70: 2f62 7567 732e 7079 7468 6f6e 2e6f 7267  /bugs.python.org
+00022a80: 2f69 7373 7565 3134 3031 3029 2e20 5370  /issue14010). Sp
+00022a90: 6563 6966 6963 616c 6c79 2c20 696e 7374  ecifically, inst
+00022aa0: 6561 6420 6f66 2077 7269 7469 6e67 0a60  ead of writing.`
+00022ab0: 6060 636f 636f 6e75 740a 7365 7120 3d20  ``coconut.seq = 
+00022ac0: 6765 745f 656c 656d 2829 203a 3a20 7365  get_elem() :: se
+00022ad0: 710a 6060 600a 7768 6963 6820 7769 6c6c  q.```.which will
+00022ae0: 2063 7261 7368 2064 7565 2074 6f20 7468   crash due to th
+00022af0: 6520 6166 6f72 656d 656e 7469 6f6e 6564  e aforementioned
+00022b00: 2050 7974 686f 6e20 6973 7375 652c 2077   Python issue, w
+00022b10: 7269 7465 0a60 6060 636f 636f 6e75 740a  rite.```coconut.
+00022b20: 4072 6563 7572 7369 7665 5f69 7465 7261  @recursive_itera
+00022b30: 746f 720a 6465 6620 7365 7128 2920 3d20  tor.def seq() = 
+00022b40: 6765 745f 656c 656d 2829 203a 3a20 7365  get_elem() :: se
+00022b50: 7128 290a 6060 600a 7768 6963 6820 7769  q().```.which wi
+00022b60: 6c6c 2077 6f72 6b20 6a75 7374 2066 696e  ll work just fin
+00022b70: 652e 0a0a 4f6e 6520 7069 7466 616c 6c20  e...One pitfall 
+00022b80: 746f 206b 6565 7020 696e 206d 696e 6420  to keep in mind 
+00022b90: 776f 726b 696e 6720 7769 7468 2060 7265  working with `re
+00022ba0: 6375 7273 6976 655f 6974 6572 6174 6f72  cursive_iterator
+00022bb0: 6020 6973 2074 6861 7420 6974 2073 686f  ` is that it sho
+00022bc0: 756c 646e 2774 2062 6520 7573 6564 2069  uldn't be used i
+00022bd0: 6e20 636f 6e74 6578 7473 2077 6865 7265  n contexts where
+00022be0: 2074 6865 2066 756e 6374 696f 6e20 6361   the function ca
+00022bf0: 6e20 706f 7465 6e74 6961 6c6c 7920 6265  n potentially be
+00022c00: 2063 616c 6c65 6420 6d75 6c74 6970 6c65   called multiple
+00022c10: 2074 696d 6573 2077 6974 6820 7468 6520   times with the 
+00022c20: 7361 6d65 2069 7465 7261 746f 7220 6f62  same iterator ob
+00022c30: 6a65 6374 2061 7320 616e 2069 6e70 7574  ject as an input
+00022c40: 2c20 6275 7420 7769 7468 2074 6861 7420  , but with that 
+00022c50: 6f62 6a65 6374 206e 6f74 2061 6374 7561  object not actua
+00022c60: 6c6c 7920 636f 7272 6573 706f 6e64 696e  lly correspondin
+00022c70: 6720 746f 2074 6865 2073 616d 6520 6974  g to the same it
+00022c80: 656d 7320 2865 2e67 2e20 6265 6361 7573  ems (e.g. becaus
+00022c90: 6520 7468 6520 6669 7273 7420 7469 6d65  e the first time
+00022ca0: 2074 6865 206f 626a 6563 7420 6861 736e   the object hasn
+00022cb0: 2774 2062 6565 6e20 6974 6572 6174 6564  't been iterated
+00022cc0: 206f 7665 7220 7965 7420 616e 6420 7468   over yet and th
+00022cd0: 6520 7365 636f 6e64 2074 696d 6520 6974  e second time it
+00022ce0: 2068 6173 2062 6565 6e29 2e0a 0a23 2323   has been)...###
+00022cf0: 2323 2045 7861 6d70 6c65 0a0a 2a2a 436f  ## Example..**Co
+00022d00: 636f 6e75 743a 2a2a 0a60 6060 636f 636f  conut:**.```coco
+00022d10: 6e75 740a 4072 6563 7572 7369 7665 5f69  nut.@recursive_i
+00022d20: 7465 7261 746f 720a 6465 6620 6669 6228  terator.def fib(
+00022d30: 2920 3d20 2831 2c20 3129 203a 3a20 6d61  ) = (1, 1) :: ma
+00022d40: 7028 282b 292c 2066 6962 2829 2c20 6669  p((+), fib(), fi
+00022d50: 6228 2924 5b31 3a5d 290a 6060 600a 0a2a  b()$[1:]).```..*
+00022d60: 2a50 7974 686f 6e3a 2a2a 0a5f 4361 6e27  *Python:**._Can'
+00022d70: 7420 6265 2064 6f6e 6520 7769 7468 6f75  t be done withou
+00022d80: 7420 6120 6c6f 6e67 2064 6563 6f72 6174  t a long decorat
+00022d90: 6f72 2064 6566 696e 6974 696f 6e2e 2054  or definition. T
+00022da0: 6865 2066 756c 6c20 6465 6669 6e69 7469  he full definiti
+00022db0: 6f6e 206f 6620 7468 6520 6465 636f 7261  on of the decora
+00022dc0: 746f 7220 696e 2050 7974 686f 6e20 6361  tor in Python ca
+00022dd0: 6e20 6265 2066 6f75 6e64 2069 6e20 7468  n be found in th
+00022de0: 6520 436f 636f 6e75 7420 6865 6164 6572  e Coconut header
+00022df0: 2e5f 0a0a 2323 2320 4275 696c 742d 496e  ._..### Built-In
+00022e00: 2054 7970 6573 0a0a 6060 607b 636f 6e74   Types..```{cont
+00022e10: 656e 7473 7d0a 2d2d 2d0a 6c6f 6361 6c3a  ents}.---.local:
+00022e20: 0a64 6570 7468 3a20 310a 2d2d 2d0a 6060  .depth: 1.---.``
+00022e30: 600a 0a23 2323 2320 606d 756c 7469 7365  `..#### `multise
+00022e40: 7460 0a0a 2a2a 6d75 6c74 6973 6574 2a2a  t`..**multiset**
+00022e50: 285f 6974 6572 6162 6c65 5f3d 604e 6f6e  (_iterable_=`Non
+00022e60: 6560 2c20 2f2c 202a 2a6b 7764 7329 0a0a  e`, /, **kwds)..
+00022e70: 436f 636f 6e75 7420 7072 6f76 6964 6573  Coconut provides
+00022e80: 2060 6d75 6c74 6973 6574 6020 6173 2061   `multiset` as a
+00022e90: 2062 7569 6c74 2d69 6e20 7375 6263 6c61   built-in subcla
+00022ea0: 7373 206f 6620 5b60 636f 6c6c 6563 7469  ss of [`collecti
+00022eb0: 6f6e 732e 436f 756e 7465 7260 5d28 6874  ons.Counter`](ht
+00022ec0: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
+00022ed0: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
+00022ee0: 636f 6c6c 6563 7469 6f6e 732e 6874 6d6c  collections.html
+00022ef0: 2363 6f6c 6c65 6374 696f 6e73 2e43 6f75  #collections.Cou
+00022f00: 6e74 6572 2920 7468 6174 2061 6464 6974  nter) that addit
+00022f10: 696f 6e61 6c6c 7920 696d 706c 656d 656e  ionally implemen
+00022f20: 7473 2074 6865 2066 756c 6c20 5b53 6574  ts the full [Set
+00022f30: 2061 6e64 204d 7574 6162 6c65 5365 7420   and MutableSet 
+00022f40: 696e 7465 7266 6163 6573 5d28 6874 7470  interfaces](http
+00022f50: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
+00022f60: 6f72 672f 332f 6c69 6272 6172 792f 636f  org/3/library/co
+00022f70: 6c6c 6563 7469 6f6e 732e 6162 632e 6874  llections.abc.ht
+00022f80: 6d6c 292e 0a0a 466f 7220 6561 7369 6c79  ml)...For easily
+00022f90: 2063 6f6e 7374 7275 6374 696e 6720 6d75   constructing mu
+00022fa0: 6c74 6973 6574 732c 2043 6f63 6f6e 7574  ltisets, Coconut
+00022fb0: 2061 6c73 6f20 7072 6f76 6964 6573 205b   also provides [
+00022fc0: 6d75 6c74 6973 6574 206c 6974 6572 616c  multiset literal
+00022fd0: 735d 2823 7365 742d 6c69 7465 7261 6c73  s](#set-literals
+00022fe0: 292e 0a0a 5468 6520 6e65 7720 6d65 7468  )...The new meth
+00022ff0: 6f64 7320 7072 6f76 6964 6564 2062 7920  ods provided by 
+00023000: 606d 756c 7469 7365 7460 206f 6e20 746f  `multiset` on to
+00023010: 7020 6f66 2060 636f 6c6c 6563 7469 6f6e  p of `collection
+00023020: 732e 436f 756e 7465 7260 2061 7265 3a0a  s.Counter` are:.
+00023030: 2d20 6d75 6c74 6973 6574 2e2a 2a61 6464  - multiset.**add
+00023040: 2a2a 285f 6974 656d 5f29 3a20 4164 6420  **(_item_): Add 
+00023050: 616e 2065 6c65 6d65 6e74 2074 6f20 6120  an element to a 
+00023060: 6d75 6c74 6973 6574 2e0a 2d20 6d75 6c74  multiset..- mult
+00023070: 6973 6574 2e2a 2a64 6973 6361 7264 2a2a  iset.**discard**
+00023080: 285f 6974 656d 5f29 3a20 5265 6d6f 7665  (_item_): Remove
+00023090: 2061 6e20 656c 656d 656e 7420 6672 6f6d   an element from
+000230a0: 2061 206d 756c 7469 7365 7420 6966 2069   a multiset if i
+000230b0: 7420 6973 2061 206d 656d 6265 722e 0a2d  t is a member..-
+000230c0: 206d 756c 7469 7365 742e 2a2a 7265 6d6f   multiset.**remo
+000230d0: 7665 2a2a 285f 6974 656d 5f29 3a20 5265  ve**(_item_): Re
+000230e0: 6d6f 7665 2061 6e20 656c 656d 656e 7420  move an element 
+000230f0: 6672 6f6d 2061 206d 756c 7469 7365 743b  from a multiset;
+00023100: 2069 7420 6d75 7374 2062 6520 6120 6d65   it must be a me
+00023110: 6d62 6572 2e0a 2d20 6d75 6c74 6973 6574  mber..- multiset
+00023120: 2e2a 2a69 7364 6973 6a6f 696e 742a 2a28  .**isdisjoint**(
+00023130: 5f6f 7468 6572 5f29 3a20 5265 7475 726e  _other_): Return
+00023140: 2054 7275 6520 6966 2074 776f 206d 756c   True if two mul
+00023150: 7469 7365 7473 2068 6176 6520 6120 6e75  tisets have a nu
+00023160: 6c6c 2069 6e74 6572 7365 6374 696f 6e2e  ll intersection.
+00023170: 0a2d 206d 756c 7469 7365 742e 2a2a 5c5f  .- multiset.**\_
+00023180: 5c5f 786f 725c 5f5c 5f2a 2a28 5f6f 7468  \_xor\_\_**(_oth
+00023190: 6572 5f29 3a20 5265 7475 726e 2074 6865  er_): Return the
+000231a0: 2073 796d 6d65 7472 6963 2064 6966 6665   symmetric diffe
+000231b0: 7265 6e63 6520 6f66 2074 776f 206d 756c  rence of two mul
+000231c0: 7469 7365 7473 2061 7320 6120 6e65 7720  tisets as a new 
+000231d0: 6d75 6c74 6973 6574 2e20 5370 6563 6966  multiset. Specif
+000231e0: 6963 616c 6c79 3a20 6061 205e 2062 203d  ically: `a ^ b =
+000231f0: 2028 6120 2d20 6229 207c 2028 6220 2d20   (a - b) | (b - 
+00023200: 6129 600a 2d20 6d75 6c74 6973 6574 2e2a  a)`.- multiset.*
+00023210: 2a63 6f75 6e74 2a2a 285f 6974 656d 5f29  *count**(_item_)
+00023220: 3a20 5265 7475 726e 2074 6865 206e 756d  : Return the num
+00023230: 6265 7220 6f66 2074 696d 6573 2061 6e20  ber of times an 
+00023240: 656c 656d 656e 7420 6f63 6375 7273 2069  element occurs i
+00023250: 6e20 6120 6d75 6c74 6973 6574 2e20 4571  n a multiset. Eq
+00023260: 7569 7661 6c65 6e74 2074 6f20 606d 756c  uivalent to `mul
+00023270: 7469 7365 745b 6974 656d 5d60 2c20 6275  tiset[item]`, bu
+00023280: 7420 6164 6469 7469 6f6e 616c 6c79 2076  t additionally v
+00023290: 6572 6966 6965 7320 7468 6520 636f 756e  erifies the coun
+000232a0: 7420 6973 206e 6f6e 2d6e 6567 6174 6976  t is non-negativ
+000232b0: 652e 0a2d 206d 756c 7469 7365 742e 2a2a  e..- multiset.**
+000232c0: 5c5f 5c5f 666d 6170 5c5f 5c5f 2a2a 285f  \_\_fmap\_\_**(_
+000232d0: 6675 6e63 5f29 3a20 4170 706c 7920 6120  func_): Apply a 
+000232e0: 6675 6e63 7469 6f6e 2074 6f20 7468 6520  function to the 
+000232f0: 636f 6e74 656e 7473 206f 6620 7468 6520  contents of the 
+00023300: 6d75 6c74 6973 6574 2c20 7072 6573 6572  multiset, preser
+00023310: 7669 6e67 2063 6f75 6e74 733b 206d 6167  ving counts; mag
+00023320: 6963 206d 6574 686f 6420 666f 7220 5b60  ic method for [`
+00023330: 666d 6170 605d 2823 666d 6170 292e 0a0a  fmap`](#fmap)...
+00023340: 436f 636f 6e75 7420 616c 736f 2065 6e73  Coconut also ens
+00023350: 7572 6573 2074 6861 7420 606d 756c 7469  ures that `multi
+00023360: 7365 7460 2073 7570 706f 7274 7320 5b72  set` supports [r
+00023370: 6963 6820 636f 6d70 6172 6973 6f6e 7320  ich comparisons 
+00023380: 616e 6420 6043 6f75 6e74 6572 2e74 6f74  and `Counter.tot
+00023390: 616c 2829 605d 2868 7474 7073 3a2f 2f64  al()`](https://d
+000233a0: 6f63 732e 7079 7468 6f6e 2e6f 7267 2f33  ocs.python.org/3
+000233b0: 2f6c 6962 7261 7279 2f63 6f6c 6c65 6374  /library/collect
+000233c0: 696f 6e73 2e68 746d 6c23 636f 6c6c 6563  ions.html#collec
+000233d0: 7469 6f6e 732e 436f 756e 7465 7229 206f  tions.Counter) o
+000233e0: 6e20 616c 6c20 5079 7468 6f6e 2076 6572  n all Python ver
+000233f0: 7369 6f6e 732e 0a0a 2323 2323 2320 4578  sions...##### Ex
+00023400: 616d 706c 650a 0a2a 2a43 6f63 6f6e 7574  ample..**Coconut
+00023410: 3a2a 2a0a 6060 6063 6f63 6f6e 7574 0a6d  :**.```coconut.m
+00023420: 795f 6d75 6c74 6973 6574 203d 206d 7b31  y_multiset = m{1
+00023430: 2c20 312c 2032 7d0a 6d79 5f6d 756c 7469  , 1, 2}.my_multi
+00023440: 7365 742e 6164 6428 3329 0a6d 795f 6d75  set.add(3).my_mu
+00023450: 6c74 6973 6574 2e72 656d 6f76 6528 3229  ltiset.remove(2)
+00023460: 0a70 7269 6e74 286d 795f 6d75 6c74 6973  .print(my_multis
+00023470: 6574 290a 6060 600a 0a2a 2a50 7974 686f  et).```..**Pytho
+00023480: 6e3a 2a2a 0a60 6060 636f 636f 6e75 745f  n:**.```coconut_
+00023490: 7079 7468 6f6e 0a66 726f 6d20 636f 6c6c  python.from coll
+000234a0: 6563 7469 6f6e 7320 696d 706f 7274 2043  ections import C
+000234b0: 6f75 6e74 6572 0a6d 795f 636f 756e 7465  ounter.my_counte
+000234c0: 7220 3d20 436f 756e 7465 7228 2831 2c20  r = Counter((1, 
+000234d0: 312c 2032 2929 0a6d 795f 636f 756e 7465  1, 2)).my_counte
+000234e0: 725b 335d 202b 3d20 310a 6d79 5f63 6f75  r[3] += 1.my_cou
+000234f0: 6e74 6572 5b32 5d20 2d3d 2031 0a69 6620  nter[2] -= 1.if 
+00023500: 6d79 5f63 6f75 6e74 6572 5b32 5d20 3c3d  my_counter[2] <=
+00023510: 2030 3a0a 2020 2020 6465 6c20 6d79 5f63   0:.    del my_c
+00023520: 6f75 6e74 6572 5b32 5d0a 7072 696e 7428  ounter[2].print(
+00023530: 6d79 5f63 6f75 6e74 6572 290a 6060 600a  my_counter).```.
+00023540: 0a23 2323 2320 6045 7870 6563 7465 6460  .#### `Expected`
+00023550: 0a0a 2a2a 4578 7065 6374 6564 2a2a 285f  ..**Expected**(_
+00023560: 7265 7375 6c74 5f3d 604e 6f6e 6560 2c20  result_=`None`, 
+00023570: 5f65 7272 6f72 5f3d 604e 6f6e 6560 290a  _error_=`None`).
+00023580: 0a43 6f63 6f6e 7574 2773 2060 4578 7065  .Coconut's `Expe
+00023590: 6374 6564 6020 6275 696c 742d 696e 2069  cted` built-in i
+000235a0: 7320 6120 436f 636f 6e75 7420 5b60 6461  s a Coconut [`da
+000235b0: 7461 6020 7479 7065 5d28 2364 6174 6129  ta` type](#data)
+000235c0: 2074 6861 7420 7265 7072 6573 656e 7473   that represents
+000235d0: 2061 2076 616c 7565 2074 6861 7420 6d61   a value that ma
+000235e0: 7920 6f72 206d 6179 206e 6f74 2062 6520  y or may not be 
+000235f0: 616e 2065 7272 6f72 2c20 7369 6d69 6c61  an error, simila
+00023600: 7220 746f 2048 6173 6b65 6c6c 2773 205b  r to Haskell's [
+00023610: 6045 6974 6865 7260 5d28 6874 7470 733a  `Either`](https:
+00023620: 2f2f 6861 636b 6167 652e 6861 736b 656c  //hackage.haskel
+00023630: 6c2e 6f72 672f 7061 636b 6167 652f 6261  l.org/package/ba
+00023640: 7365 2d34 2e31 372e 302e 302f 646f 6373  se-4.17.0.0/docs
+00023650: 2f44 6174 612d 4569 7468 6572 2e68 746d  /Data-Either.htm
+00023660: 6c29 2e0a 0a60 4578 7065 6374 6564 6020  l)...`Expected` 
+00023670: 6973 2065 6666 6563 7469 7665 6c79 2065  is effectively e
+00023680: 7175 6976 616c 656e 7420 746f 2074 6865  quivalent to the
+00023690: 2066 6f6c 6c6f 7769 6e67 3a0a 6060 6063   following:.```c
+000236a0: 6f63 6f6e 7574 0a64 6174 6120 4578 7065  oconut.data Expe
+000236b0: 6374 6564 5b54 5d28 7265 7375 6c74 3a20  cted[T](result: 
+000236c0: 543f 203d 204e 6f6e 652c 2065 7272 6f72  T? = None, error
+000236d0: 3a20 4261 7365 4578 6365 7074 696f 6e3f  : BaseException?
+000236e0: 203d 204e 6f6e 6529 3a0a 2020 2020 6465   = None):.    de
+000236f0: 6620 5f5f 626f 6f6c 5f5f 2873 656c 6629  f __bool__(self)
+00023700: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+00023710: 2020 7265 7475 726e 2073 656c 662e 6572    return self.er
+00023720: 726f 7220 6973 204e 6f6e 650a 2020 2020  ror is None.    
+00023730: 6465 6620 5f5f 666d 6170 5f5f 5b55 5d28  def __fmap__[U](
+00023740: 7365 6c66 2c20 6675 6e63 3a20 5420 2d3e  self, func: T ->
+00023750: 2055 2920 2d3e 2045 7870 6563 7465 645b   U) -> Expected[
+00023760: 555d 3a0a 2020 2020 2020 2020 7265 7475  U]:.        retu
+00023770: 726e 2073 656c 662e 5f5f 636c 6173 735f  rn self.__class_
+00023780: 5f28 6675 6e63 2873 656c 662e 7265 7375  _(func(self.resu
+00023790: 6c74 2929 2069 6620 7365 6c66 2065 6c73  lt)) if self els
+000237a0: 6520 7365 6c66 0a20 2020 2064 6566 2061  e self.    def a
+000237b0: 6e64 5f74 6865 6e5b 555d 2873 656c 662c  nd_then[U](self,
+000237c0: 2066 756e 633a 2054 202d 3e20 4578 7065   func: T -> Expe
+000237d0: 6374 6564 5b55 5d29 202d 3e20 4578 7065  cted[U]) -> Expe
+000237e0: 6374 6564 5b55 5d3a 0a20 2020 2020 2020  cted[U]:.       
+000237f0: 2022 2222 4d61 7073 2061 2054 202d 3e20   """Maps a T -> 
+00023800: 4578 7065 6374 6564 5b55 5d20 6f76 6572  Expected[U] over
+00023810: 2061 6e20 4578 7065 6374 6564 5b54 5d20   an Expected[T] 
+00023820: 746f 2070 726f 6475 6365 2061 6e20 4578  to produce an Ex
+00023830: 7065 6374 6564 5b55 5d2e 0a20 2020 2020  pected[U]..     
+00023840: 2020 2049 6d70 6c65 6d65 6e74 7320 6120     Implements a 
+00023850: 6d6f 6e61 6469 6320 6269 6e64 2e20 4571  monadic bind. Eq
+00023860: 7569 7661 6c65 6e74 2074 6f20 666d 6170  uivalent to fmap
+00023870: 202e 2e3e 202e 6a6f 696e 2829 2e22 2222   ..> .join()."""
+00023880: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00023890: 7365 6c66 207c 3e20 666d 6170 2428 6675  self |> fmap$(fu
+000238a0: 6e63 2920 7c3e 202e 6a6f 696e 2829 0a20  nc) |> .join(). 
+000238b0: 2020 2064 6566 206a 6f69 6e28 7365 6c66     def join(self
+000238c0: 3a20 4578 7065 6374 6564 5b45 7870 6563  : Expected[Expec
+000238d0: 7465 645b 545d 5d29 202d 3e20 4578 7065  ted[T]]) -> Expe
+000238e0: 6374 6564 5b54 5d3a 0a20 2020 2020 2020  cted[T]:.       
+000238f0: 2022 2222 4d6f 6e61 6469 6320 6a6f 696e   """Monadic join
+00023900: 2e20 436f 6e76 6572 7473 2045 7870 6563  . Converts Expec
+00023910: 7465 645b 4578 7065 6374 6564 5b54 5d5d  ted[Expected[T]]
+00023920: 2074 6f20 4578 7065 6374 6564 5b54 5d2e   to Expected[T].
+00023930: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
+00023940: 6f74 2073 656c 663a 0a20 2020 2020 2020  ot self:.       
+00023950: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00023960: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00023970: 7365 6c66 2e72 6573 756c 7420 6069 7369  self.result `isi
+00023980: 6e73 7461 6e63 6560 2045 7870 6563 7465  nstance` Expecte
+00023990: 643a 0a20 2020 2020 2020 2020 2020 2072  d:.            r
+000239a0: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
+000239b0: 4578 7065 6374 6564 2e6a 6f69 6e28 2920  Expected.join() 
+000239c0: 7265 7175 6972 6573 2061 6e20 4578 7065  requires an Expe
+000239d0: 6374 6564 5b45 7870 6563 7465 645b 5f5d  cted[Expected[_]
+000239e0: 5d22 290a 2020 2020 2020 2020 7265 7475  ]").        retu
+000239f0: 726e 2073 656c 662e 7265 7375 6c74 0a20  rn self.result. 
+00023a00: 2020 2064 6566 206d 6170 5f65 7272 6f72     def map_error
+00023a10: 2873 656c 662c 2066 756e 633a 2042 6173  (self, func: Bas
+00023a20: 6545 7863 6570 7469 6f6e 202d 3e20 4261  eException -> Ba
+00023a30: 7365 4578 6365 7074 696f 6e29 202d 3e20  seException) -> 
+00023a40: 4578 7065 6374 6564 5b54 5d3a 0a20 2020  Expected[T]:.   
+00023a50: 2020 2020 2022 2222 4d61 7073 2066 756e       """Maps fun
+00023a60: 6320 6f76 6572 2074 6865 2065 7272 6f72  c over the error
+00023a70: 2069 6620 6974 2065 7869 7374 732e 2222   if it exists.""
+00023a80: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+00023a90: 2073 656c 6620 6966 2073 656c 6620 656c   self if self el
+00023aa0: 7365 2073 656c 662e 5f5f 636c 6173 735f  se self.__class_
+00023ab0: 5f28 6572 726f 723d 6675 6e63 2873 656c  _(error=func(sel
+00023ac0: 662e 6572 726f 7229 290a 2020 2020 6465  f.error)).    de
+00023ad0: 6620 6f72 5f65 6c73 655b 555d 2873 656c  f or_else[U](sel
+00023ae0: 662c 2066 756e 633a 2042 6173 6545 7863  f, func: BaseExc
+00023af0: 6570 7469 6f6e 202d 3e20 4578 7065 6374  eption -> Expect
+00023b00: 6564 5b55 5d29 202d 3e20 4578 7065 6374  ed[U]) -> Expect
+00023b10: 6564 5b54 207c 2055 5d3a 0a20 2020 2020  ed[T | U]:.     
+00023b20: 2020 2022 2222 5265 7475 726e 2073 656c     """Return sel
+00023b30: 6620 6966 206e 6f20 6572 726f 722c 206f  f if no error, o
+00023b40: 7468 6572 7769 7365 2072 6574 7572 6e20  therwise return 
+00023b50: 7468 6520 7265 7375 6c74 206f 6620 6576  the result of ev
+00023b60: 616c 7561 7469 6e67 2066 756e 6320 6f6e  aluating func on
+00023b70: 2074 6865 2065 7272 6f72 2e22 2222 0a20   the error.""". 
+00023b80: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00023b90: 6c66 2069 6620 7365 6c66 2065 6c73 6520  lf if self else 
+00023ba0: 6675 6e63 2873 656c 662e 6572 726f 7229  func(self.error)
+00023bb0: 0a20 2020 2064 6566 2072 6573 756c 745f  .    def result_
+00023bc0: 6f72 5b55 5d28 7365 6c66 2c20 6465 6661  or[U](self, defa
+00023bd0: 756c 743a 2055 2920 2d3e 2054 207c 2055  ult: U) -> T | U
+00023be0: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
+00023bf0: 7572 6e20 7468 6520 7265 7375 6c74 2069  urn the result i
+00023c00: 6620 6974 2065 7869 7374 732c 206f 7468  f it exists, oth
+00023c10: 6572 7769 7365 2072 6574 7572 6e20 7468  erwise return th
+00023c20: 6520 6465 6661 756c 742e 2222 220a 2020  e default.""".  
+00023c30: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00023c40: 662e 7265 7375 6c74 2069 6620 7365 6c66  f.result if self
+00023c50: 2065 6c73 6520 6465 6661 756c 740a 2020   else default.  
+00023c60: 2020 6465 6620 7265 7375 6c74 5f6f 725f    def result_or_
+00023c70: 656c 7365 5b55 5d28 7365 6c66 2c20 6675  else[U](self, fu
+00023c80: 6e63 3a20 4261 7365 4578 6365 7074 696f  nc: BaseExceptio
+00023c90: 6e20 2d3e 2055 2920 2d3e 2054 207c 2055  n -> U) -> T | U
+00023ca0: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
+00023cb0: 7572 6e20 7468 6520 7265 7375 6c74 2069  urn the result i
+00023cc0: 6620 6974 2065 7869 7374 732c 206f 7468  f it exists, oth
+00023cd0: 6572 7769 7365 2072 6574 7572 6e20 7468  erwise return th
+00023ce0: 6520 7265 7375 6c74 206f 6620 6576 616c  e result of eval
+00023cf0: 7561 7469 6e67 2066 756e 6320 6f6e 2074  uating func on t
+00023d00: 6865 2065 7272 6f72 2e22 2222 0a20 2020  he error.""".   
+00023d10: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00023d20: 2e72 6573 756c 7420 6966 2073 656c 6620  .result if self 
+00023d30: 656c 7365 2066 756e 6328 7365 6c66 2e65  else func(self.e
+00023d40: 7272 6f72 290a 2020 2020 6465 6620 756e  rror).    def un
+00023d50: 7772 6170 2873 656c 6629 202d 3e20 543a  wrap(self) -> T:
+00023d60: 0a20 2020 2020 2020 2022 2222 556e 7772  .        """Unwr
+00023d70: 6170 2074 6865 2072 6573 756c 7420 6f72  ap the result or
+00023d80: 2072 6169 7365 2074 6865 2065 7272 6f72   raise the error
+00023d90: 2e22 2222 0a20 2020 2020 2020 2069 6620  .""".        if 
+00023da0: 6e6f 7420 7365 6c66 3a0a 2020 2020 2020  not self:.      
+00023db0: 2020 2020 2020 7261 6973 6520 7365 6c66        raise self
+00023dc0: 2e65 7272 6f72 0a20 2020 2020 2020 2072  .error.        r
+00023dd0: 6574 7572 6e20 7365 6c66 2e72 6573 756c  eturn self.resul
+00023de0: 740a 6060 600a 0a60 4578 7065 6374 6564  t.```..`Expected
+00023df0: 6020 6973 2070 7269 6d61 7269 6c79 2075  ` is primarily u
+00023e00: 7365 6420 6173 2074 6865 2072 6574 7572  sed as the retur
+00023e10: 6e20 7479 7065 2066 6f72 205b 6073 6166  n type for [`saf
+00023e20: 655f 6361 6c6c 605d 2823 7361 6665 5f63  e_call`](#safe_c
+00023e30: 616c 6c29 2e20 4765 6e65 7261 6c6c 792c  all). Generally,
+00023e40: 2074 6865 2062 6573 7420 7761 7920 746f   the best way to
+00023e50: 2075 7365 2060 4578 7065 6374 6564 6020   use `Expected` 
+00023e60: 6973 2077 6974 6820 5b60 666d 6170 605d  is with [`fmap`]
+00023e70: 2823 666d 6170 292c 2077 6869 6368 2077  (#fmap), which w
+00023e80: 696c 6c20 6170 706c 7920 6120 6675 6e63  ill apply a func
+00023e90: 7469 6f6e 2074 6f20 7468 6520 7265 7375  tion to the resu
+00023ea0: 6c74 2069 6620 6974 2065 7869 7374 732c  lt if it exists,
+00023eb0: 206f 7220 6f74 6865 7277 6973 6520 7265   or otherwise re
+00023ec0: 7461 696e 2074 6865 2065 7272 6f72 2e20  tain the error. 
+00023ed0: 4966 2079 6f75 2077 616e 7420 746f 2073  If you want to s
+00023ee0: 6571 7565 6e63 6520 6d75 6c74 6970 6c65  equence multiple
+00023ef0: 2060 4578 7065 6374 6564 602d 7265 7475   `Expected`-retu
+00023f00: 726e 696e 6720 6f70 6572 6174 696f 6e73  rning operations
+00023f10: 2c20 602e 616e 645f 7468 656e 6020 7368  , `.and_then` sh
+00023f20: 6f75 6c64 2062 6520 7573 6564 2069 6e73  ould be used ins
+00023f30: 7465 6164 206f 6620 6066 6d61 7060 2e0a  tead of `fmap`..
+00023f40: 0a54 6f20 6d61 7463 6820 6167 6169 6e73  .To match agains
+00023f50: 7420 616e 2060 4578 7065 6374 6564 602c  t an `Expected`,
+00023f60: 206a 7573 743a 0a60 6060 0a45 7870 6563   just:.```.Expec
+00023f70: 7465 6428 7265 7329 203d 2045 7870 6563  ted(res) = Expec
+00023f80: 7465 6428 2272 6573 756c 7422 290a 4578  ted("result").Ex
+00023f90: 7065 6374 6564 2865 7272 6f72 3d65 7272  pected(error=err
+00023fa0: 2920 3d20 4578 7065 6374 6564 2865 7272  ) = Expected(err
+00023fb0: 6f72 3d54 7970 6545 7272 6f72 2829 290a  or=TypeError()).
+00023fc0: 6060 600a 0a23 2323 2323 2045 7861 6d70  ```..##### Examp
+00023fd0: 6c65 0a0a 2a2a 436f 636f 6e75 743a 2a2a  le..**Coconut:**
+00023fe0: 0a60 6060 636f 636f 6e75 740a 6465 6620  .```coconut.def 
+00023ff0: 7472 795f 6469 7669 6465 2878 3a20 666c  try_divide(x: fl
+00024000: 6f61 742c 2079 3a20 666c 6f61 7429 202d  oat, y: float) -
+00024010: 3e20 4578 7065 6374 6564 5b66 6c6f 6174  > Expected[float
+00024020: 5d3a 0a20 2020 2074 7279 3a0a 2020 2020  ]:.    try:.    
+00024030: 2020 2020 7265 7475 726e 2045 7870 6563      return Expec
+00024040: 7465 6428 7820 2f20 7929 0a20 2020 2065  ted(x / y).    e
+00024050: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+00024060: 6173 2065 7272 3a0a 2020 2020 2020 2020  as err:.        
+00024070: 7265 7475 726e 2045 7870 6563 7465 6428  return Expected(
+00024080: 6572 726f 723d 6572 7229 0a0a 7472 795f  error=err)..try_
+00024090: 6469 7669 6465 2831 2c20 3229 207c 3e20  divide(1, 2) |> 
+000240a0: 666d 6170 2428 2e2b 3129 207c 3e20 7072  fmap$(.+1) |> pr
+000240b0: 696e 740a 7472 795f 6469 7669 6465 2831  int.try_divide(1
+000240c0: 2c20 3029 207c 3e20 666d 6170 2428 2e2b  , 0) |> fmap$(.+
+000240d0: 3129 207c 3e20 7072 696e 740a 6060 600a  1) |> print.```.
+000240e0: 0a2a 2a50 7974 686f 6e3a 2a2a 0a5f 4361  .**Python:**._Ca
+000240f0: 6e27 7420 6265 2064 6f6e 6520 7769 7468  n't be done with
+00024100: 6f75 7420 6120 636f 6d70 6c65 7820 6045  out a complex `E
+00024110: 7870 6563 7465 6460 2064 6566 696e 6974  xpected` definit
+00024120: 696f 6e2e 2053 6565 2074 6865 2063 6f6d  ion. See the com
+00024130: 7069 6c65 6420 636f 6465 2066 6f72 2074  piled code for t
+00024140: 6865 2050 7974 686f 6e20 7379 6e74 6178  he Python syntax
+00024150: 2e5f 0a0a 2323 2323 2060 4d61 7463 6845  ._..#### `MatchE
+00024160: 7272 6f72 600a 0a41 2060 4d61 7463 6845  rror`..A `MatchE
+00024170: 7272 6f72 6020 6973 2072 6169 7365 6420  rror` is raised 
+00024180: 7768 656e 2061 205b 6465 7374 7275 6374  when a [destruct
+00024190: 7572 696e 6720 6173 7369 676e 6d65 6e74  uring assignment
+000241a0: 5d28 2364 6573 7472 7563 7475 7269 6e67  ](#destructuring
+000241b0: 2d61 7373 6967 6e6d 656e 7429 206f 7220  -assignment) or 
+000241c0: 5b70 6174 7465 726e 2d6d 6174 6368 696e  [pattern-matchin
+000241d0: 6720 6675 6e63 7469 6f6e 5d28 2370 6174  g function](#pat
+000241e0: 7465 726e 2d6d 6174 6368 696e 672d 6675  tern-matching-fu
+000241f0: 6e63 7469 6f6e 7329 2066 6169 6c73 2c20  nctions) fails, 
+00024200: 616e 6420 7468 7573 2060 4d61 7463 6845  and thus `MatchE
+00024210: 7272 6f72 6020 6973 2070 726f 7669 6465  rror` is provide
+00024220: 6420 6173 2061 2062 7569 6c74 2d69 6e20  d as a built-in 
+00024230: 666f 7220 6361 7463 6869 6e67 2074 686f  for catching tho
+00024240: 7365 2065 7272 6f72 732e 2060 4d61 7463  se errors. `Matc
+00024250: 6845 7272 6f72 6020 6f62 6a65 6374 7320  hError` objects 
+00024260: 7375 7070 6f72 7420 7468 7265 6520 6174  support three at
+00024270: 7472 6962 7574 6573 3a20 6070 6174 7465  tributes: `patte
+00024280: 726e 602c 2077 6869 6368 2069 7320 6120  rn`, which is a 
+00024290: 7374 7269 6e67 2064 6573 6372 6962 696e  string describin
+000242a0: 6720 7468 6520 6661 696c 6564 2070 6174  g the failed pat
+000242b0: 7465 726e 3b20 6076 616c 7565 602c 2077  tern; `value`, w
+000242c0: 6869 6368 2069 7320 7468 6520 6f62 6a65  hich is the obje
+000242d0: 6374 2074 6861 7420 6661 696c 6564 2074  ct that failed t
+000242e0: 6f20 6d61 7463 6820 7468 6174 2070 6174  o match that pat
+000242f0: 7465 726e 3b20 616e 6420 606d 6573 7361  tern; and `messa
+00024300: 6765 6020 7768 6963 6820 6973 2074 6865  ge` which is the
+00024310: 2066 756c 6c20 6572 726f 7220 6d65 7373   full error mess
+00024320: 6167 652e 2054 6f20 6176 6f69 6420 756e  age. To avoid un
+00024330: 6e65 6365 7373 6172 7920 6072 6570 7260  necessary `repr`
+00024340: 2063 616c 6c73 2c20 604d 6174 6368 4572   calls, `MatchEr
+00024350: 726f 7260 206f 6e6c 7920 636f 6d70 7574  ror` only comput
+00024360: 6573 2074 6865 2060 6d65 7373 6167 6560  es the `message`
+00024370: 206f 6e63 6520 6974 2069 7320 6163 7475   once it is actu
+00024380: 616c 6c79 2072 6571 7565 7374 6564 2e0a  ally requested..
+00024390: 0a41 6464 6974 696f 6e61 6c6c 792c 2069  .Additionally, i
+000243a0: 6620 796f 7520 6172 6520 7573 696e 6720  f you are using 
+000243b0: 5b76 6965 7720 7061 7474 6572 6e73 5d28  [view patterns](
+000243c0: 236d 6174 6368 292c 2079 6f75 206d 6967  #match), you mig
+000243d0: 6874 206e 6565 6420 746f 2072 6169 7365  ht need to raise
+000243e0: 2079 6f75 7220 6f77 6e20 604d 6174 6368   your own `Match
+000243f0: 4572 726f 7260 2028 7468 6f75 6768 2079  Error` (though y
+00024400: 6f75 2063 616e 2061 6c73 6f20 6a75 7374  ou can also just
+00024410: 2075 7365 2061 2064 6573 7472 7563 7475   use a destructu
+00024420: 7269 6e67 2061 7373 6967 6e6d 656e 7420  ring assignment 
+00024430: 6f72 2070 6174 7465 726e 2d6d 6174 6368  or pattern-match
+00024440: 696e 6720 6675 6e63 7469 6f6e 2064 6566  ing function def
+00024450: 696e 6974 696f 6e20 746f 2064 6f20 736f  inition to do so
+00024460: 292e 2054 6f20 7261 6973 6520 796f 7572  ). To raise your
+00024470: 206f 776e 2060 4d61 7463 6845 7272 6f72   own `MatchError
+00024480: 602c 206a 7573 7420 6072 6169 7365 204d  `, just `raise M
+00024490: 6174 6368 4572 726f 7228 7061 7474 6572  atchError(patter
+000244a0: 6e2c 2076 616c 7565 2960 2028 626f 7468  n, value)` (both
+000244b0: 2061 7267 756d 656e 7473 2061 7265 206f   arguments are o
+000244c0: 7074 696f 6e61 6c29 2e0a 0a49 6e20 736f  ptional)...In so
+000244d0: 6d65 2063 6173 6573 2077 6865 7265 2074  me cases where t
+000244e0: 6865 7265 2061 7265 206d 756c 7469 706c  here are multipl
+000244f0: 6520 436f 636f 6e75 7420 7061 636b 6167  e Coconut packag
+00024500: 6573 2069 6e73 7461 6c6c 6564 2061 7420  es installed at 
+00024510: 7468 6520 7361 6d65 2074 696d 652c 2074  the same time, t
+00024520: 6865 7265 206d 6179 2062 6520 6d75 6c74  here may be mult
+00024530: 6970 6c65 2060 4d61 7463 6845 7272 6f72  iple `MatchError
+00024540: 6073 2064 6566 696e 6564 2069 6e20 6469  `s defined in di
+00024550: 6666 6572 656e 7420 7061 636b 6167 6573  fferent packages
+00024560: 2e20 436f 636f 6e75 7420 6361 6e20 7065  . Coconut can pe
+00024570: 7266 6f72 6d20 736f 6d65 206d 6167 6963  rform some magic
+00024580: 2075 6e64 6572 2074 6865 2068 6f6f 6420   under the hood 
+00024590: 746f 206d 616b 6520 7375 7265 2074 6861  to make sure tha
+000245a0: 7420 616c 6c20 7468 6573 6520 604d 6174  t all these `Mat
+000245b0: 6368 4572 726f 7260 7320 7769 6c6c 2073  chError`s will s
+000245c0: 6561 6d6c 6573 736c 7920 696e 7465 726f  eamlessly intero
+000245d0: 7065 7261 7465 2c20 6275 7420 6f6e 6c79  perate, but only
+000245e0: 2069 6620 616c 6c20 7375 6368 2070 6163   if all such pac
+000245f0: 6b61 6765 7320 6172 6520 636f 6d70 696c  kages are compil
+00024600: 6564 2069 6e20 5b60 2d2d 7061 636b 6167  ed in [`--packag
+00024610: 6560 206d 6f64 6520 7261 7468 6572 2074  e` mode rather t
+00024620: 6861 6e20 602d 2d73 7461 6e64 616c 6f6e  han `--standalon
+00024630: 6560 206d 6f64 655d 2823 636f 6d70 696c  e` mode](#compil
+00024640: 6174 696f 6e2d 6d6f 6465 7329 2e0a 0a23  ation-modes)...#
+00024650: 2323 2047 656e 6572 6963 2042 7569 6c74  ## Generic Built
+00024660: 2d49 6e20 4675 6e63 7469 6f6e 730a 0a60  -In Functions..`
+00024670: 6060 7b63 6f6e 7465 6e74 737d 0a2d 2d2d  ``{contents}.---
+00024680: 0a6c 6f63 616c 3a0a 6465 7074 683a 2031  .local:.depth: 1
+00024690: 0a2d 2d2d 0a60 6060 0a0a 2323 2323 2060  .---.```..#### `
+000246a0: 6d61 6b65 6461 7461 600a 0a2a 2a6d 616b  makedata`..**mak
+000246b0: 6564 6174 612a 2a28 5f64 6174 615c 5f74  edata**(_data\_t
+000246c0: 7970 655f 2c20 2a5f 6172 6773 5f29 0a0a  ype_, *_args_)..
+000246d0: 436f 636f 6e75 7420 7072 6f76 6964 6573  Coconut provides
+000246e0: 2074 6865 2060 6d61 6b65 6461 7461 6020   the `makedata` 
+000246f0: 6675 6e63 7469 6f6e 2074 6f20 636f 6e73  function to cons
+00024700: 7472 7563 7420 6120 636f 6e74 6169 6e65  truct a containe
+00024710: 7220 6769 7665 6e20 7468 6520 6465 7369  r given the desi
+00024720: 7265 6420 7479 7065 2061 6e64 2063 6f6e  red type and con
+00024730: 7465 6e74 732e 2054 6869 7320 6973 2070  tents. This is p
+00024740: 6172 7469 6375 6c61 726c 7920 7573 6566  articularly usef
+00024750: 756c 2077 6865 6e20 7772 6974 696e 6720  ul when writing 
+00024760: 616c 7465 726e 6174 6976 6520 636f 6e73  alternative cons
+00024770: 7472 7563 746f 7273 2066 6f72 205b 6064  tructors for [`d
+00024780: 6174 6160 5d28 2364 6174 6129 2074 7970  ata`](#data) typ
+00024790: 6573 2062 7920 6f76 6572 7772 6974 696e  es by overwritin
+000247a0: 6720 605f 5f6e 6577 5f5f 602c 2073 696e  g `__new__`, sin
+000247b0: 6365 2069 7420 616c 6c6f 7773 2064 6972  ce it allows dir
+000247c0: 6563 7420 6163 6365 7373 2074 6f20 7468  ect access to th
+000247d0: 6520 6261 7365 2063 6f6e 7374 7275 6374  e base construct
+000247e0: 6f72 206f 6620 7468 6520 6461 7461 2074  or of the data t
+000247f0: 7970 6520 6372 6561 7465 6420 7769 7468  ype created with
+00024800: 2074 6865 2043 6f63 6f6e 7574 2060 6461   the Coconut `da
+00024810: 7461 6020 7374 6174 656d 656e 742e 0a0a  ta` statement...
+00024820: 606d 616b 6564 6174 6160 2074 616b 6573  `makedata` takes
+00024830: 2074 6865 2064 6174 6120 7479 7065 2074   the data type t
+00024840: 6f20 636f 6e73 7472 7563 7420 6173 2074  o construct as t
+00024850: 6865 2066 6972 7374 2061 7267 756d 656e  he first argumen
+00024860: 742c 2061 6e64 2074 6865 206f 626a 6563  t, and the objec
+00024870: 7473 2074 6f20 7075 7420 696e 2074 6861  ts to put in tha
+00024880: 7420 636f 6e74 6169 6e65 7220 6173 2074  t container as t
+00024890: 6865 2072 6573 7420 6f66 2074 6865 2061  he rest of the a
+000248a0: 7267 756d 656e 7473 2e0a 0a60 6d61 6b65  rguments...`make
+000248b0: 6461 7461 6020 6361 6e20 616c 736f 2062  data` can also b
+000248c0: 6520 7573 6564 2074 6f20 6578 7472 6163  e used to extrac
+000248d0: 7420 7468 6520 756e 6465 726c 7969 6e67  t the underlying
+000248e0: 2063 6f6e 7374 7275 6374 6f72 2066 6f72   constructor for
+000248f0: 205b 606d 6174 6368 2064 6174 6160 5d28   [`match data`](
+00024900: 236d 6174 6368 2d64 6174 6129 2074 7970  #match-data) typ
+00024910: 6573 2074 6861 7420 6279 7061 7373 6573  es that bypasses
+00024920: 2074 6865 206e 6f72 6d61 6c20 7061 7474   the normal patt
+00024930: 6572 6e2d 6d61 7463 6869 6e67 2063 6f6e  ern-matching con
+00024940: 7374 7275 6374 6f72 2e0a 0a41 6464 6974  structor...Addit
+00024950: 696f 6e61 6c6c 792c 2060 6d61 6b65 6461  ionally, `makeda
+00024960: 7461 6020 6361 6e20 616c 736f 2062 6520  ta` can also be 
+00024970: 6361 6c6c 6564 2077 6974 6820 6e6f 6e2d  called with non-
+00024980: 6064 6174 6160 2074 7970 6520 6173 2074  `data` type as t
+00024990: 6865 2066 6972 7374 2061 7267 756d 656e  he first argumen
+000249a0: 742c 2069 6e20 7768 6963 6820 6361 7365  t, in which case
+000249b0: 2069 7420 7769 6c6c 2064 6f20 6974 7320   it will do its 
+000249c0: 6265 7374 2074 6f20 636f 6e73 7472 7563  best to construc
+000249d0: 7420 7468 6520 6769 7665 6e20 7479 7065  t the given type
+000249e0: 206f 6620 6f62 6a65 6374 2077 6974 6820   of object with 
+000249f0: 7468 6520 6769 7665 6e20 6172 6775 6d65  the given argume
+00024a00: 6e74 732e 2054 6869 7320 6675 6e63 7469  nts. This functi
+00024a10: 6f6e 616c 6974 7920 6973 2075 7365 6420  onality is used 
+00024a20: 696e 7465 726e 616c 6c79 2062 7920 6066  internally by `f
+00024a30: 6d61 7060 2e0a 0a23 2323 2323 2060 6461  map`...##### `da
+00024a40: 7461 6d61 6b65 7260 0a0a 2a2a 4445 5052  tamaker`..**DEPR
+00024a50: 4543 4154 4544 3a2a 2a20 436f 636f 6e75  ECATED:** Coconu
+00024a60: 7420 616c 736f 2068 6173 2061 2060 6461  t also has a `da
+00024a70: 7461 6d61 6b65 7260 2062 7569 6c74 2d69  tamaker` built-i
+00024a80: 6e2c 2077 6869 6368 2070 6172 7469 616c  n, which partial
+00024a90: 6c79 2061 7070 6c69 6573 2060 6d61 6b65  ly applies `make
+00024aa0: 6461 7461 603b 2060 6461 7461 6d61 6b65  data`; `datamake
+00024ab0: 7260 2069 7320 6465 6669 6e65 6420 6173  r` is defined as
+00024ac0: 3a0a 6060 6063 6f63 6f6e 7574 0a64 6566  :.```coconut.def
+00024ad0: 2064 6174 616d 616b 6572 2864 6174 615f   datamaker(data_
+00024ae0: 7479 7065 293a 0a20 2020 2022 2222 4765  type):.    """Ge
+00024af0: 7420 7468 6520 6f72 6967 696e 616c 2063  t the original c
+00024b00: 6f6e 7374 7275 6374 6f72 206f 6620 7468  onstructor of th
+00024b10: 6520 6769 7665 6e20 6461 7461 2074 7970  e given data typ
+00024b20: 6520 6f72 2063 6c61 7373 2e22 2222 0a20  e or class.""". 
+00024b30: 2020 2072 6574 7572 6e20 6d61 6b65 6461     return makeda
+00024b40: 7461 2428 6461 7461 5f74 7970 6529 0a60  ta$(data_type).`
+00024b50: 6060 0a5f 4e6f 7465 3a20 5061 7373 696e  ``._Note: Passin
+00024b60: 6720 602d 2d73 7472 6963 7460 2064 6973  g `--strict` dis
+00024b70: 6162 6c65 7320 6465 7072 6563 6174 6564  ables deprecated
+00024b80: 2066 6561 7475 7265 732e 5f0a 0a23 2323   features._..###
+00024b90: 2323 2045 7861 6d70 6c65 0a0a 2a2a 436f  ## Example..**Co
+00024ba0: 636f 6e75 743a 2a2a 0a60 6060 636f 636f  conut:**.```coco
+00024bb0: 6e75 740a 6461 7461 2054 7570 6c65 2865  nut.data Tuple(e
+00024bc0: 6c65 6d73 293a 0a20 2020 2064 6566 205f  lems):.    def _
+00024bd0: 5f6e 6577 5f5f 2863 6c73 2c20 2a65 6c65  _new__(cls, *ele
+00024be0: 6d73 293a 0a20 2020 2020 2020 2072 6574  ms):.        ret
+00024bf0: 7572 6e20 656c 656d 7320 7c3e 206d 616b  urn elems |> mak
+00024c00: 6564 6174 6124 2863 6c73 290a 6060 600a  edata$(cls).```.
+00024c10: 0a2a 2a50 7974 686f 6e3a 2a2a 0a5f 4361  .**Python:**._Ca
+00024c20: 6e27 7420 6265 2064 6f6e 6520 7769 7468  n't be done with
+00024c30: 6f75 7420 6120 7365 7269 6573 206f 6620  out a series of 
+00024c40: 6d65 7468 6f64 2064 6566 696e 6974 696f  method definitio
+00024c50: 6e73 2066 6f72 2065 6163 6820 6461 7461  ns for each data
+00024c60: 2074 7970 652e 2053 6565 2074 6865 2063   type. See the c
+00024c70: 6f6d 7069 6c65 6420 636f 6465 2066 6f72  ompiled code for
+00024c80: 2074 6865 2050 7974 686f 6e20 7379 6e74   the Python synt
+00024c90: 6178 2e5f 0a0a 2323 2323 2060 666d 6170  ax._..#### `fmap
+00024ca0: 600a 0a2a 2a66 6d61 702a 2a28 5f66 756e  `..**fmap**(_fun
+00024cb0: 635f 2c20 5f6f 626a 5f29 0a0a 496e 2048  c_, _obj_)..In H
+00024cc0: 6173 6b65 6c6c 2c20 6066 6d61 7028 6675  askell, `fmap(fu
+00024cd0: 6e63 2c20 6f62 6a29 6020 7461 6b65 7320  nc, obj)` takes 
+00024ce0: 6120 6461 7461 2074 7970 6520 606f 626a  a data type `obj
+00024cf0: 6020 616e 6420 7265 7475 726e 7320 6120  ` and returns a 
+00024d00: 6e65 7720 6461 7461 2074 7970 6520 7769  new data type wi
+00024d10: 7468 2060 6675 6e63 6020 6d61 7070 6564  th `func` mapped
+00024d20: 206f 7665 7220 7468 6520 636f 6e74 656e   over the conten
+00024d30: 7473 2e20 436f 636f 6e75 7427 7320 6066  ts. Coconut's `f
+00024d40: 6d61 7060 2066 756e 6374 696f 6e20 646f  map` function do
+00024d50: 6573 2074 6865 2065 7861 6374 2073 616d  es the exact sam
+00024d60: 6520 7468 696e 6720 666f 7220 436f 636f  e thing for Coco
+00024d70: 6e75 7427 7320 5b64 6174 6120 7479 7065  nut's [data type
+00024d80: 735d 2823 6461 7461 292e 0a0a 6066 6d61  s](#data)...`fma
+00024d90: 7060 2063 616e 2061 6c73 6f20 6265 2075  p` can also be u
+00024da0: 7365 6420 6f6e 2074 6865 2062 7569 6c74  sed on the built
+00024db0: 2d69 6e20 6f62 6a65 6374 7320 6073 7472  -in objects `str
+00024dc0: 602c 2060 6469 6374 602c 2060 6c69 7374  `, `dict`, `list
+00024dd0: 602c 2060 7475 706c 6560 2c20 6073 6574  `, `tuple`, `set
+00024de0: 602c 2060 6672 6f7a 656e 7365 7460 2c20  `, `frozenset`, 
+00024df0: 616e 6420 6064 6963 7460 2061 7320 6120  and `dict` as a 
+00024e00: 7661 7269 616e 7420 6f66 2060 6d61 7060  variant of `map`
+00024e10: 2074 6861 7420 7265 7475 726e 7320 6261   that returns ba
+00024e20: 636b 2061 6e20 6f62 6a65 6374 206f 6620  ck an object of 
+00024e30: 7468 6520 7361 6d65 2074 7970 652e 0a0a  the same type...
+00024e40: 5468 6520 6265 6861 7669 6f72 206f 6620  The behavior of 
+00024e50: 6066 6d61 7060 2066 6f72 2061 2067 6976  `fmap` for a giv
+00024e60: 656e 206f 626a 6563 7420 6361 6e20 6265  en object can be
+00024e70: 206f 7665 7272 6964 6465 6e20 6279 2064   overridden by d
+00024e80: 6566 696e 696e 6720 616e 2060 5f5f 666d  efining an `__fm
+00024e90: 6170 5f5f 2873 656c 662c 2066 756e 6329  ap__(self, func)
+00024ea0: 6020 6d61 6769 6320 6d65 7468 6f64 2074  ` magic method t
+00024eb0: 6861 7420 7769 6c6c 2062 6520 6361 6c6c  hat will be call
+00024ec0: 6564 2077 6865 6e65 7665 7220 6066 6d61  ed whenever `fma
+00024ed0: 7060 2069 7320 696e 766f 6b65 6420 6f6e  p` is invoked on
+00024ee0: 2074 6861 7420 6f62 6a65 6374 2e20 4e6f   that object. No
+00024ef0: 7465 2074 6861 7420 605f 5f66 6d61 705f  te that `__fmap_
+00024f00: 5f60 2069 6d70 6c65 6d65 6e74 6174 696f  _` implementatio
+00024f10: 6e73 2073 686f 756c 6420 616c 7761 7973  ns should always
+00024f20: 2073 6174 6973 6679 2074 6865 205b 4675   satisfy the [Fu
+00024f30: 6e63 746f 7220 4c61 7773 5d28 6874 7470  nctor Laws](http
+00024f40: 733a 2f2f 7769 6b69 2e68 6173 6b65 6c6c  s://wiki.haskell
+00024f50: 2e6f 7267 2f46 756e 6374 6f72 292e 0a0a  .org/Functor)...
+00024f60: 466f 7220 6064 6963 7460 2c20 6f72 2061  For `dict`, or a
+00024f70: 6e79 206f 7468 6572 2060 636f 6c6c 6563  ny other `collec
+00024f80: 7469 6f6e 732e 6162 632e 4d61 7070 696e  tions.abc.Mappin
+00024f90: 6760 2c20 6066 6d61 7060 2077 696c 6c20  g`, `fmap` will 
+00024fa0: 6d61 7020 6f76 6572 2074 6865 206d 6170  map over the map
+00024fb0: 7069 6e67 2773 2060 2e69 7465 6d73 2829  ping's `.items()
+00024fc0: 6020 696e 7374 6561 6420 6f66 2074 6865  ` instead of the
+00024fd0: 2064 6566 6175 6c74 2069 7465 7261 7469   default iterati
+00024fe0: 6f6e 2074 6872 6f75 6768 2069 7473 2060  on through its `
+00024ff0: 2e6b 6579 7328 2960 2c20 7769 7468 2074  .keys()`, with t
+00025000: 6865 206e 6577 206d 6170 7069 6e67 2072  he new mapping r
+00025010: 6563 6f6e 7374 7275 6374 6564 2066 726f  econstructed fro
+00025020: 6d20 7468 6520 6d61 7070 6564 206f 7665  m the mapped ove
+00025030: 7220 6974 656d 732e 205f 4445 5052 4543  r items. _DEPREC
+00025040: 4154 4544 3a20 6066 6d61 7024 2873 7461  ATED: `fmap$(sta
+00025050: 726d 6170 5f6f 7665 725f 6d61 7070 696e  rmap_over_mappin
+00025060: 6773 3d54 7275 6529 6020 7769 6c6c 2060  gs=True)` will `
+00025070: 7374 6172 6d61 7060 206f 7665 7220 7468  starmap` over th
+00025080: 6520 602e 6974 656d 7328 2960 2069 6e73  e `.items()` ins
+00025090: 7465 6164 206f 6620 606d 6170 6020 6f76  tead of `map` ov
+000250a0: 6572 2074 6865 6d2e 5f0a 0a46 6f72 205b  er them._..For [
+000250b0: 606e 756d 7079 605d 2823 6e75 6d70 792d  `numpy`](#numpy-
+000250c0: 696e 7465 6772 6174 696f 6e29 206f 626a  integration) obj
+000250d0: 6563 7473 2c20 6066 6d61 7060 2077 696c  ects, `fmap` wil
+000250e0: 6c20 7573 6520 5b60 6e70 2e76 6563 746f  l use [`np.vecto
+000250f0: 7269 7a65 605d 2868 7474 7073 3a2f 2f64  rize`](https://d
+00025100: 6f63 732e 7363 6970 792e 6f72 672f 646f  ocs.scipy.org/do
+00025110: 632f 6e75 6d70 792f 7265 6665 7265 6e63  c/numpy/referenc
+00025120: 652f 6765 6e65 7261 7465 642f 6e75 6d70  e/generated/nump
+00025130: 792e 7665 6374 6f72 697a 652e 6874 6d6c  y.vectorize.html
+00025140: 2920 746f 2070 726f 6475 6365 2074 6865  ) to produce the
+00025150: 2072 6573 756c 742e 0a0a 466f 7220 5b60   result...For [`
+00025160: 7061 6e64 6173 605d 2868 7474 7073 3a2f  pandas`](https:/
+00025170: 2f70 616e 6461 732e 7079 6461 7461 2e6f  /pandas.pydata.o
+00025180: 7267 2f29 206f 626a 6563 7473 2c20 6066  rg/) objects, `f
+00025190: 6d61 7060 2077 696c 6c20 7573 6520 5b60  map` will use [`
+000251a0: 2e61 7070 6c79 605d 2868 7474 7073 3a2f  .apply`](https:/
+000251b0: 2f70 616e 6461 732e 7079 6461 7461 2e6f  /pandas.pydata.o
+000251c0: 7267 2f64 6f63 732f 7265 6665 7265 6e63  rg/docs/referenc
+000251d0: 652f 6170 692f 7061 6e64 6173 2e44 6174  e/api/pandas.Dat
+000251e0: 6146 7261 6d65 2e61 7070 6c79 2e68 746d  aFrame.apply.htm
+000251f0: 6c29 2061 6c6f 6e67 2074 6865 206c 6173  l) along the las
+00025200: 7420 6178 6973 2028 736f 2072 6f77 2d77  t axis (so row-w
+00025210: 6973 6520 666f 7220 6044 6174 6146 7261  ise for `DataFra
+00025220: 6d65 6027 732c 2065 6c65 6d65 6e74 2d77  me`'s, element-w
+00025230: 6973 6520 666f 7220 6053 6572 6965 7360  ise for `Series`
+00025240: 2773 292e 0a0a 466f 7220 6173 796e 6368  's)...For asynch
+00025250: 726f 6e6f 7573 2069 7465 7261 626c 6573  ronous iterables
+00025260: 2c20 6066 6d61 7060 2077 696c 6c20 6d61  , `fmap` will ma
+00025270: 7020 6173 796e 6368 726f 6e6f 7573 6c79  p asynchronously
+00025280: 2c20 6d61 6b69 6e67 2060 666d 6170 6020  , making `fmap` 
+00025290: 6571 7569 7661 6c65 6e74 2069 6e20 7468  equivalent in th
+000252a0: 6174 2063 6173 6520 746f 0a60 6060 636f  at case to.```co
+000252b0: 636f 6e75 745f 7079 7468 6f6e 0a61 7379  conut_python.asy
+000252c0: 6e63 2064 6566 2066 6d61 705f 6f76 6572  nc def fmap_over
+000252d0: 5f61 7379 6e63 5f69 7465 7273 2866 756e  _async_iters(fun
+000252e0: 632c 2061 7379 6e63 5f69 7465 7229 3a0a  c, async_iter):.
+000252f0: 2020 2020 6173 796e 6320 666f 7220 6974      async for it
+00025300: 656d 2069 6e20 6173 796e 635f 6974 6572  em in async_iter
+00025310: 3a0a 2020 2020 2020 2020 7969 656c 6420  :.        yield 
+00025320: 6675 6e63 2869 7465 6d29 0a60 6060 0a73  func(item).```.s
+00025330: 7563 6820 7468 6174 2060 666d 6170 6020  uch that `fmap` 
+00025340: 6361 6e20 6566 6665 6374 6976 656c 7920  can effectively 
+00025350: 6265 2075 7365 6420 6173 2061 6e20 6173  be used as an as
+00025360: 796e 6320 6d61 702e 0a0a 5f44 4550 5245  ync map..._DEPRE
+00025370: 4341 5445 443a 2060 666d 6170 2866 756e  CATED: `fmap(fun
+00025380: 632c 206f 626a 2c20 6661 6c6c 6261 636b  c, obj, fallback
+00025390: 5f74 6f5f 696e 6974 3d54 7275 6529 6020  _to_init=True)` 
+000253a0: 7769 6c6c 2066 616c 6c20 6261 636b 2074  will fall back t
+000253b0: 6f20 606f 626a 2e5f 5f63 6c61 7373 5f5f  o `obj.__class__
+000253c0: 286d 6170 2866 756e 632c 206f 626a 2929  (map(func, obj))
+000253d0: 6020 6966 206e 6f20 6066 6d61 7060 2069  ` if no `fmap` i
+000253e0: 6d70 6c65 6d65 6e74 6174 696f 6e20 6973  mplementation is
+000253f0: 2061 7661 696c 6162 6c65 2072 6174 6865   available rathe
+00025400: 7220 7468 616e 2072 6169 7365 2060 5479  r than raise `Ty
+00025410: 7065 4572 726f 7260 2e5f 0a0a 2323 2323  peError`._..####
+00025420: 2320 4578 616d 706c 650a 0a2a 2a43 6f63  # Example..**Coc
+00025430: 6f6e 7574 3a2a 2a0a 6060 6063 6f63 6f6e  onut:**.```cocon
+00025440: 7574 0a5b 312c 2032 2c20 335d 207c 3e20  ut.[1, 2, 3] |> 
+00025450: 666d 6170 2428 7820 2d3e 2078 2b31 2920  fmap$(x -> x+1) 
+00025460: 3d3d 205b 322c 2033 2c20 345d 0a0a 636c  == [2, 3, 4]..cl
+00025470: 6173 7320 4d61 7962 650a 6461 7461 204e  ass Maybe.data N
+00025480: 6f74 6869 6e67 2829 2066 726f 6d20 4d61  othing() from Ma
+00025490: 7962 650a 6461 7461 204a 7573 7428 6e29  ybe.data Just(n)
+000254a0: 2066 726f 6d20 4d61 7962 650a 0a4a 7573   from Maybe..Jus
+000254b0: 7428 3329 207c 3e20 666d 6170 2428 7820  t(3) |> fmap$(x 
+000254c0: 2d3e 2078 2a32 2920 3d3d 204a 7573 7428  -> x*2) == Just(
+000254d0: 3629 0a4e 6f74 6869 6e67 2829 207c 3e20  6).Nothing() |> 
+000254e0: 666d 6170 2428 7820 2d3e 2078 2a32 2920  fmap$(x -> x*2) 
+000254f0: 3d3d 204e 6f74 6869 6e67 2829 0a60 6060  == Nothing().```
+00025500: 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a 5f43  ..**Python:**._C
+00025510: 616e 2774 2062 6520 646f 6e65 2077 6974  an't be done wit
+00025520: 686f 7574 2061 2073 6572 6965 7320 6f66  hout a series of
+00025530: 206d 6574 686f 6420 6465 6669 6e69 7469   method definiti
+00025540: 6f6e 7320 666f 7220 6561 6368 2064 6174  ons for each dat
+00025550: 6120 7479 7065 2e20 5365 6520 7468 6520  a type. See the 
+00025560: 636f 6d70 696c 6564 2063 6f64 6520 666f  compiled code fo
+00025570: 7220 7468 6520 5079 7468 6f6e 2073 796e  r the Python syn
+00025580: 7461 782e 5f0a 0a0a 2323 2323 2060 6361  tax._...#### `ca
+00025590: 6c6c 600a 0a2a 2a63 616c 6c2a 2a28 5f66  ll`..**call**(_f
+000255a0: 756e 635f 2c20 2f2c 202a 5f61 7267 735f  unc_, /, *_args_
+000255b0: 2c20 5c2a 5c2a 5f6b 7761 7267 735f 290a  , \*\*_kwargs_).
+000255c0: 0a43 6f63 6f6e 7574 2773 2060 6361 6c6c  .Coconut's `call
+000255d0: 6020 7369 6d70 6c79 2069 6d70 6c65 6d65  ` simply impleme
+000255e0: 6e74 7320 6675 6e63 7469 6f6e 2061 7070  nts function app
+000255f0: 6c69 6361 7469 6f6e 2e20 5468 7573 2c20  lication. Thus, 
+00025600: 6063 616c 6c60 2069 7320 6566 6665 6374  `call` is effect
+00025610: 6976 656c 7920 6571 7569 7661 6c65 6e74  ively equivalent
+00025620: 2074 6f0a 6060 6063 6f63 6f6e 7574 0a64   to.```coconut.d
+00025630: 6566 2063 616c 6c28 662c 202f 2c20 2a61  ef call(f, /, *a
+00025640: 7267 732c 202a 2a6b 7761 7267 7329 203d  rgs, **kwargs) =
+00025650: 2066 282a 6172 6773 2c20 2a2a 6b77 6172   f(*args, **kwar
+00025660: 6773 290a 6060 600a 0a60 6361 6c6c 6020  gs).```..`call` 
+00025670: 6973 2070 7269 6d61 7269 6c79 2075 7365  is primarily use
+00025680: 6675 6c20 6173 2061 6e20 5b6f 7065 7261  ful as an [opera
+00025690: 746f 7220 6675 6e63 7469 6f6e 5d28 236f  tor function](#o
+000256a0: 7065 7261 746f 722d 6675 6e63 7469 6f6e  perator-function
+000256b0: 7329 2066 6f72 2066 756e 6374 696f 6e20  s) for function 
+000256c0: 6170 706c 6963 6174 696f 6e20 7768 656e  application when
+000256d0: 2077 7269 7469 6e67 2069 6e20 6120 706f   writing in a po
+000256e0: 696e 742d 6672 6565 2073 7479 6c65 2e0a  int-free style..
+000256f0: 0a5f 4445 5052 4543 4154 4544 3a20 606f  ._DEPRECATED: `o
+00025700: 6660 2069 7320 6176 6169 6c61 626c 6520  f` is available 
+00025710: 6173 2061 2064 6570 7265 6361 7465 6420  as a deprecated 
+00025720: 616c 6961 7320 666f 7220 6063 616c 6c60  alias for `call`
+00025730: 2e20 4e6f 7465 2074 6861 7420 6465 7072  . Note that depr
+00025740: 6563 6174 6564 2066 6561 7475 7265 7320  ecated features 
+00025750: 6172 6520 6469 7361 626c 6564 2069 6e20  are disabled in 
+00025760: 602d 2d73 7472 6963 7460 206d 6f64 652e  `--strict` mode.
+00025770: 5f0a 0a23 2323 2320 6073 6166 655f 6361  _..#### `safe_ca
+00025780: 6c6c 600a 0a2a 2a73 6166 655f 6361 6c6c  ll`..**safe_call
+00025790: 2a2a 285f 6675 6e63 5f2c 202f 2c20 2a5f  **(_func_, /, *_
+000257a0: 6172 6773 5f2c 205c 2a5c 2a5f 6b77 6172  args_, \*\*_kwar
+000257b0: 6773 5f29 0a0a 436f 636f 6e75 7427 7320  gs_)..Coconut's 
+000257c0: 6073 6166 655f 6361 6c6c 6020 6973 2061  `safe_call` is a
+000257d0: 2076 6572 7369 6f6e 206f 6620 5b60 6361   version of [`ca
+000257e0: 6c6c 605d 2823 6361 6c6c 2920 7468 6174  ll`](#call) that
+000257f0: 2063 6174 6368 6573 2061 6e79 2060 4578   catches any `Ex
+00025800: 6365 7074 696f 6e60 7320 616e 6420 7265  ception`s and re
+00025810: 7475 726e 7320 616e 205b 6045 7870 6563  turns an [`Expec
+00025820: 7465 6460 5d28 2365 7870 6563 7465 6429  ted`](#expected)
+00025830: 2063 6f6e 7461 696e 696e 6720 6569 7468   containing eith
+00025840: 6572 2074 6865 2072 6573 756c 7420 6f72  er the result or
+00025850: 2074 6865 2065 7272 6f72 2e0a 0a60 7361   the error...`sa
+00025860: 6665 5f63 616c 6c60 2069 7320 6566 6665  fe_call` is effe
+00025870: 6374 6976 656c 7920 6571 7569 7661 6c65  ctively equivale
+00025880: 6e74 2074 6f3a 0a60 6060 636f 636f 6e75  nt to:.```coconu
+00025890: 740a 6465 6620 7361 6665 5f63 616c 6c28  t.def safe_call(
+000258a0: 662c 202f 2c20 2a61 7267 732c 202a 2a6b  f, /, *args, **k
+000258b0: 7761 7267 7329 3a0a 2020 2020 7472 793a  wargs):.    try:
+000258c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000258d0: 4578 7065 6374 6564 2866 282a 6172 6773  Expected(f(*args
+000258e0: 2c20 2a2a 6b77 6172 6773 2929 0a20 2020  , **kwargs)).   
+000258f0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00025900: 6e20 6173 2065 7272 3a0a 2020 2020 2020  n as err:.      
+00025910: 2020 7265 7475 726e 2045 7870 6563 7465    return Expecte
+00025920: 6428 6572 726f 723d 6572 7229 0a60 6060  d(error=err).```
+00025930: 0a0a 2323 2323 2320 4578 616d 706c 650a  ..##### Example.
+00025940: 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a 6060  .**Coconut:**.``
+00025950: 6063 6f63 6f6e 7574 0a72 6573 2c20 6572  `coconut.res, er
+00025960: 7220 3d20 7361 6665 5f63 616c 6c28 2d3e  r = safe_call(->
+00025970: 2031 202f 2030 2920 7c3e 2066 6d61 7024   1 / 0) |> fmap$
+00025980: 282e 2b31 290a 6060 600a 0a2a 2a50 7974  (.+1).```..**Pyt
+00025990: 686f 6e3a 2a2a 0a5f 4361 6e27 7420 6265  hon:**._Can't be
+000259a0: 2064 6f6e 6520 7769 7468 6f75 7420 6120   done without a 
+000259b0: 636f 6d70 6c65 7820 6045 7870 6563 7465  complex `Expecte
+000259c0: 6460 2064 6566 696e 6974 696f 6e2e 2053  d` definition. S
+000259d0: 6565 2074 6865 2063 6f6d 7069 6c65 6420  ee the compiled 
+000259e0: 636f 6465 2066 6f72 2074 6865 2050 7974  code for the Pyt
+000259f0: 686f 6e20 7379 6e74 6178 2e5f 0a0a 2323  hon syntax._..##
+00025a00: 2323 2060 6964 656e 7460 0a0a 2a2a 6964  ## `ident`..**id
+00025a10: 656e 742a 2a28 5f78 5f2c 202a 2c20 5f73  ent**(_x_, *, _s
+00025a20: 6964 655c 5f65 6666 6563 745f 3d60 4e6f  ide\_effect_=`No
+00025a30: 6e65 6029 0a0a 436f 636f 6e75 7427 7320  ne`)..Coconut's 
+00025a40: 6069 6465 6e74 6020 6973 2074 6865 2069  `ident` is the i
+00025a50: 6465 6e74 6974 7920 6675 6e63 7469 6f6e  dentity function
+00025a60: 2c20 6765 6e65 7261 6c6c 7920 6571 7569  , generally equi
+00025a70: 7661 6c65 6e74 2074 6f20 6078 202d 3e20  valent to `x -> 
+00025a80: 7860 2e0a 0a60 6964 656e 7460 2061 6c73  x`...`ident` als
+00025a90: 6f20 6163 6365 7074 7320 6f6e 6520 6b65  o accepts one ke
+00025aa0: 7977 6f72 642d 6f6e 6c79 2061 7267 756d  yword-only argum
+00025ab0: 656e 742c 2060 7369 6465 5f65 6666 6563  ent, `side_effec
+00025ac0: 7460 2c20 7768 6963 6820 7370 6563 6966  t`, which specif
+00025ad0: 6965 7320 6120 6675 6e63 7469 6f6e 2074  ies a function t
+00025ae0: 6f20 6361 6c6c 206f 6e20 7468 6520 6172  o call on the ar
+00025af0: 6775 6d65 6e74 2062 6566 6f72 6520 6974  gument before it
+00025b00: 2069 7320 7265 7475 726e 6564 2e20 5468   is returned. Th
+00025b10: 7573 2c20 6069 6465 6e74 6020 6973 2065  us, `ident` is e
+00025b20: 6666 6563 7469 7665 6c79 2065 7175 6976  ffectively equiv
+00025b30: 616c 656e 7420 746f 3a0a 6060 6063 6f63  alent to:.```coc
+00025b40: 6f6e 7574 0a64 6566 2069 6465 6e74 2878  onut.def ident(x
+00025b50: 2c20 2a2c 2073 6964 655f 6566 6665 6374  , *, side_effect
+00025b60: 3d4e 6f6e 6529 3a0a 2020 2020 6966 2073  =None):.    if s
+00025b70: 6964 655f 6566 6665 6374 2069 7320 6e6f  ide_effect is no
+00025b80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00025b90: 7369 6465 5f65 6666 6563 7428 7829 0a20  side_effect(x). 
+00025ba0: 2020 2072 6574 7572 6e20 780a 6060 600a     return x.```.
+00025bb0: 0a60 6964 656e 7460 2069 7320 7072 696d  .`ident` is prim
+00025bc0: 6172 696c 7920 7573 6566 756c 2077 6865  arily useful whe
+00025bd0: 6e20 7772 6974 696e 6720 696e 2061 2070  n writing in a p
+00025be0: 6f69 6e74 2d66 7265 6520 7374 796c 6520  oint-free style 
+00025bf0: 2865 2e67 2e20 696e 2063 6f6d 6269 6e61  (e.g. in combina
+00025c00: 7469 6f6e 2077 6974 6820 5b60 6c69 6674  tion with [`lift
+00025c10: 605d 2823 6c69 6674 2929 206f 7220 666f  `](#lift)) or fo
+00025c20: 7220 6465 6275 6767 696e 6720 5b70 6970  r debugging [pip
+00025c30: 6573 5d28 2370 6970 6573 2920 7768 6572  es](#pipes) wher
+00025c40: 6520 6069 6465 6e74 2428 7369 6465 5f65  e `ident$(side_e
+00025c50: 6666 6563 743d 7072 696e 7429 6020 6361  ffect=print)` ca
+00025c60: 6e20 6c65 7420 796f 7520 7365 6520 7768  n let you see wh
+00025c70: 6174 2069 7320 6265 696e 6720 7069 7065  at is being pipe
+00025c80: 642e 0a0a 2323 2323 2060 636f 6e73 7460  d...#### `const`
+00025c90: 0a0a 2a2a 636f 6e73 742a 2a28 5f76 616c  ..**const**(_val
+00025ca0: 7565 5f29 0a0a 436f 636f 6e75 7427 7320  ue_)..Coconut's 
+00025cb0: 6063 6f6e 7374 6020 7369 6d70 6c79 2063  `const` simply c
+00025cc0: 6f6e 7374 7275 6374 7320 6120 6675 6e63  onstructs a func
+00025cd0: 7469 6f6e 2074 6861 742c 2077 6861 7465  tion that, whate
+00025ce0: 7665 7220 6974 7320 6172 6775 6d65 6e74  ver its argument
+00025cf0: 732c 206a 7573 7420 7265 7475 726e 7320  s, just returns 
+00025d00: 7468 6520 6769 7665 6e20 7661 6c75 652e  the given value.
+00025d10: 2054 6875 732c 2060 636f 6e73 7460 2069   Thus, `const` i
+00025d20: 7320 6571 7569 7661 6c65 6e74 2074 6f20  s equivalent to 
+00025d30: 6120 7069 636b 6c65 6162 6c65 2076 6572  a pickleable ver
+00025d40: 7369 6f6e 206f 660a 6060 6063 6f63 6f6e  sion of.```cocon
+00025d50: 7574 0a64 6566 2063 6f6e 7374 2876 616c  ut.def const(val
+00025d60: 7565 2920 3d20 282a 6172 6773 2c20 2a2a  ue) = (*args, **
+00025d70: 6b77 6172 6773 2920 2d3e 2076 616c 7565  kwargs) -> value
+00025d80: 0a60 6060 0a0a 6063 6f6e 7374 6020 6973  .```..`const` is
+00025d90: 2070 7269 6d61 7269 6c79 2075 7365 6675   primarily usefu
+00025da0: 6c20 7768 656e 2077 7269 7469 6e67 2069  l when writing i
+00025db0: 6e20 6120 706f 696e 742d 6672 6565 2073  n a point-free s
+00025dc0: 7479 6c65 2028 652e 672e 2069 6e20 636f  tyle (e.g. in co
+00025dd0: 6d62 696e 6174 696f 6e20 7769 7468 205b  mbination with [
+00025de0: 606c 6966 7460 5d28 236c 6966 7429 292e  `lift`](#lift)).
+00025df0: 0a0a 2323 2323 2060 666c 6970 600a 0a2a  ..#### `flip`..*
+00025e00: 2a66 6c69 702a 2a28 5f66 756e 635f 2c20  *flip**(_func_, 
+00025e10: 5f6e 6172 6773 5f3d 604e 6f6e 6560 290a  _nargs_=`None`).
+00025e20: 0a43 6f63 6f6e 7574 2773 2060 666c 6970  .Coconut's `flip
+00025e30: 2866 2c20 6e61 7267 733d 4e6f 6e65 2960  (f, nargs=None)`
+00025e40: 2069 7320 6120 6869 6768 6572 2d6f 7264   is a higher-ord
+00025e50: 6572 2066 756e 6374 696f 6e20 7468 6174  er function that
+00025e60: 2c20 6769 7665 6e20 6120 6675 6e63 7469  , given a functi
+00025e70: 6f6e 2060 6660 2c20 7265 7475 726e 7320  on `f`, returns 
+00025e80: 6120 6e65 7720 6675 6e63 7469 6f6e 2077  a new function w
+00025e90: 6974 6820 7265 7665 7273 6564 2061 7267  ith reversed arg
+00025ea0: 756d 656e 7420 6f72 6465 722e 2049 6620  ument order. If 
+00025eb0: 606e 6172 6773 6020 6973 2070 6173 7365  `nargs` is passe
+00025ec0: 642c 206f 6e6c 7920 7468 6520 6669 7273  d, only the firs
+00025ed0: 7420 606e 6172 6773 6020 6172 6775 6d65  t `nargs` argume
+00025ee0: 6e74 7320 6172 6520 7265 7665 7273 6564  nts are reversed
+00025ef0: 2e0a 0a46 6f72 2074 6865 2062 696e 6172  ...For the binar
+00025f00: 7920 6361 7365 2c20 6066 6c69 7060 2077  y case, `flip` w
+00025f10: 6f72 6b73 2061 730a 6060 6063 6f63 6f6e  orks as.```cocon
+00025f20: 7574 0a66 6c69 7028 662c 2032 2928 782c  ut.flip(f, 2)(x,
+00025f30: 2079 2920 3d3d 2066 2879 2c20 7829 0a60   y) == f(y, x).`
+00025f40: 6060 0a73 7563 6820 7468 6174 2060 666c  ``.such that `fl
+00025f50: 6970 2428 3f2c 2032 2960 2069 6d70 6c65  ip$(?, 2)` imple
+00025f60: 6d65 6e74 7320 7468 6520 6043 6020 636f  ments the `C` co
+00025f70: 6d62 696e 6174 6f72 2028 6066 6c69 7060  mbinator (`flip`
+00025f80: 2069 6e20 4861 736b 656c 6c29 2e0a 0a49   in Haskell)...I
+00025f90: 6e20 7468 6520 6765 6e65 7261 6c20 6361  n the general ca
+00025fa0: 7365 2c20 6066 6c69 7060 2069 7320 6571  se, `flip` is eq
+00025fb0: 7569 7661 6c65 6e74 2074 6f20 6120 7069  uivalent to a pi
+00025fc0: 636b 6c65 6162 6c65 2076 6572 7369 6f6e  ckleable version
+00025fd0: 206f 660a 6060 6063 6f63 6f6e 7574 0a64   of.```coconut.d
+00025fe0: 6566 2066 6c69 7028 662c 206e 6172 6773  ef flip(f, nargs
+00025ff0: 3d4e 6f6e 6529 203d 0a20 2020 2028 2a61  =None) =.    (*a
+00026000: 7267 732c 202a 2a6b 7761 7267 7329 202d  rgs, **kwargs) -
+00026010: 3e20 280a 2020 2020 2020 2020 6628 2a61  > (.        f(*a
+00026020: 7267 735b 3a3a 2d31 5d2c 202a 2a6b 7761  rgs[::-1], **kwa
+00026030: 7267 7329 2069 6620 6e61 7267 7320 6973  rgs) if nargs is
+00026040: 204e 6f6e 650a 2020 2020 2020 2020 656c   None.        el
+00026050: 7365 2066 282a 2861 7267 735b 6e61 7267  se f(*(args[narg
+00026060: 732d 313a 3a2d 315d 202b 2061 7267 735b  s-1::-1] + args[
+00026070: 6e61 7267 733a 5d29 2c20 2a2a 6b77 6172  nargs:]), **kwar
+00026080: 6773 290a 2020 2020 290a 6060 600a 0a23  gs).    ).```..#
+00026090: 2323 2320 606c 6966 7460 0a0a 2a2a 6c69  ### `lift`..**li
+000260a0: 6674 2a2a 285f 6675 6e63 5f29 0a0a 2a2a  ft**(_func_)..**
+000260b0: 6c69 6674 2a2a 285f 6675 6e63 5f2c 202a  lift**(_func_, *
+000260c0: 5f66 756e 635c 5f61 7267 735f 2c20 2a2a  _func\_args_, **
+000260d0: 5f66 756e 635c 5f6b 7761 7267 735f 290a  _func\_kwargs_).
+000260e0: 0a43 6f63 6f6e 7574 2773 2060 6c69 6674  .Coconut's `lift
+000260f0: 6020 6275 696c 742d 696e 2069 7320 6120  ` built-in is a 
+00026100: 6869 6768 6572 2d6f 7264 6572 2066 756e  higher-order fun
+00026110: 6374 696f 6e20 7468 6174 2074 616b 6573  ction that takes
+00026120: 2069 6e20 6120 6675 6e63 7469 6f6e 2061   in a function a
+00026130: 6e64 20e2 809c 6c69 6674 73e2 809d 2069  nd ...lifts... i
+00026140: 7420 7570 2073 6f20 7468 6174 2061 6c6c  t up so that all
+00026150: 206f 6620 6974 7320 6172 6775 6d65 6e74   of its argument
+00026160: 7320 6172 6520 6675 6e63 7469 6f6e 732e  s are functions.
+00026170: 0a0a 4173 2061 2073 696d 706c 6520 6578  ..As a simple ex
+00026180: 616d 706c 652c 2066 6f72 2061 2062 696e  ample, for a bin
+00026190: 6172 7920 6675 6e63 7469 6f6e 2060 6628  ary function `f(
+000261a0: 782c 2079 2960 2061 6e64 2074 776f 2075  x, y)` and two u
+000261b0: 6e61 7279 2066 756e 6374 696f 6e73 2060  nary functions `
+000261c0: 6728 7a29 6020 616e 6420 6068 287a 2960  g(z)` and `h(z)`
+000261d0: 2c20 606c 6966 7460 2077 6f72 6b73 2061  , `lift` works a
+000261e0: 730a 6060 6063 6f63 6f6e 7574 0a6c 6966  s.```coconut.lif
+000261f0: 7428 6629 2867 2c20 6829 287a 2920 3d3d  t(f)(g, h)(z) ==
+00026200: 2066 2867 287a 292c 2068 287a 2929 0a60   f(g(z), h(z)).`
+00026210: 6060 0a73 7563 6820 7468 6174 2069 6e20  ``.such that in 
+00026220: 7468 6973 2063 6173 6520 606c 6966 7460  this case `lift`
+00026230: 2069 6d70 6c65 6d65 6e74 7320 7468 6520   implements the 
+00026240: 6053 2760 2063 6f6d 6269 6e61 746f 7220  `S'` combinator 
+00026250: 2860 6c69 6674 4132 6020 6f72 2060 6c69  (`liftA2` or `li
+00026260: 6674 4d32 6020 696e 2048 6173 6b65 6c6c  ftM2` in Haskell
+00026270: 292e 0a0a 496e 2074 6865 2067 656e 6572  )...In the gener
+00026280: 616c 2063 6173 652c 2060 6c69 6674 6020  al case, `lift` 
+00026290: 6973 2065 7175 6976 616c 656e 7420 746f  is equivalent to
+000262a0: 2061 2070 6963 6b6c 6561 626c 6520 7665   a pickleable ve
+000262b0: 7273 696f 6e20 6f66 0a60 6060 636f 636f  rsion of.```coco
+000262c0: 6e75 740a 6465 6620 6c69 6674 2866 2920  nut.def lift(f) 
+000262d0: 3d20 280a 2020 2020 282a 6675 6e63 5f61  = (.    (*func_a
+000262e0: 7267 732c 202a 2a66 756e 635f 6b77 6172  rgs, **func_kwar
+000262f0: 6773 2920 2d3e 0a20 2020 2020 2020 2028  gs) ->.        (
+00026300: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+00026310: 202d 3e0a 2020 2020 2020 2020 2020 2020   ->.            
+00026320: 6628 0a20 2020 2020 2020 2020 2020 2020  f(.             
+00026330: 2020 202a 2867 282a 6172 6773 2c20 2a2a     *(g(*args, **
+00026340: 6b77 6172 6773 2920 666f 7220 6720 696e  kwargs) for g in
+00026350: 2066 756e 635f 6172 6773 292c 0a20 2020   func_args),.   
+00026360: 2020 2020 2020 2020 2020 2020 202a 2a7b               **{
+00026370: 6b3a 2068 282a 6172 6773 2c20 2a2a 6b77  k: h(*args, **kw
+00026380: 6172 6773 2920 666f 7220 6b2c 2068 2069  args) for k, h i
+00026390: 6e20 6675 6e63 5f6b 7761 7267 732e 6974  n func_kwargs.it
+000263a0: 656d 7328 297d 0a20 2020 2020 2020 2020  ems()}.         
+000263b0: 2020 2029 0a29 0a60 6060 0a0a 606c 6966     ).).```..`lif
+000263c0: 7460 2061 6c73 6f20 7375 7070 6f72 7473  t` also supports
+000263d0: 2061 2073 686f 7274 6375 7420 666f 726d   a shortcut form
+000263e0: 2073 7563 6820 7468 6174 2060 6c69 6674   such that `lift
+000263f0: 2866 2c20 2a66 756e 635f 6172 6773 2c20  (f, *func_args, 
+00026400: 2a2a 6675 6e63 5f6b 7761 7267 7329 6020  **func_kwargs)` 
+00026410: 6973 2065 7175 6976 616c 656e 7420 746f  is equivalent to
+00026420: 2060 6c69 6674 2866 2928 2a66 756e 635f   `lift(f)(*func_
+00026430: 6172 6773 2c20 2a2a 6675 6e63 5f6b 7761  args, **func_kwa
+00026440: 7267 7329 602e 0a0a 2323 2323 2320 4578  rgs)`...##### Ex
+00026450: 616d 706c 650a 0a2a 2a43 6f63 6f6e 7574  ample..**Coconut
+00026460: 3a2a 2a0a 6060 6063 6f63 6f6e 7574 0a78  :**.```coconut.x
+00026470: 735f 616e 645f 7873 7031 203d 2069 6465  s_and_xsp1 = ide
+00026480: 6e74 2060 6c69 6674 287a 6970 2960 206d  nt `lift(zip)` m
+00026490: 6170 2428 2d3e 5f2b 3129 0a6d 696e 5f61  ap$(->_+1).min_a
+000264a0: 6e64 5f6d 6178 203d 206c 6966 7428 2c29  nd_max = lift(,)
+000264b0: 286d 696e 2c20 6d61 7829 0a70 6c75 735f  (min, max).plus_
+000264c0: 616e 645f 7469 6d65 7320 3d20 282b 2920  and_times = (+) 
+000264d0: 606c 6966 7428 2c29 6020 282a 290a 6060  `lift(,)` (*).``
+000264e0: 600a 0a2a 2a50 7974 686f 6e3a 2a2a 0a60  `..**Python:**.`
+000264f0: 6060 636f 636f 6e75 745f 7079 7468 6f6e  ``coconut_python
+00026500: 0a64 6566 2078 735f 616e 645f 7873 7031  .def xs_and_xsp1
+00026510: 2878 7329 3a0a 2020 2020 7265 7475 726e  (xs):.    return
+00026520: 207a 6970 2878 732c 206d 6170 286c 616d   zip(xs, map(lam
+00026530: 6264 6120 783a 2078 202b 2031 2c20 7873  bda x: x + 1, xs
+00026540: 2929 0a64 6566 206d 696e 5f61 6e64 5f6d  )).def min_and_m
+00026550: 6178 2878 7329 3a0a 2020 2020 7265 7475  ax(xs):.    retu
+00026560: 726e 206d 696e 2878 7329 2c20 6d61 7828  rn min(xs), max(
+00026570: 7873 290a 6465 6620 706c 7573 5f61 6e64  xs).def plus_and
+00026580: 5f74 696d 6573 2878 2c20 7929 3a0a 2020  _times(x, y):.  
+00026590: 2020 7265 7475 726e 2078 202b 2079 2c20    return x + y, 
+000265a0: 7820 2a20 790a 6060 600a 0a23 2323 2320  x * y.```..#### 
+000265b0: 6061 6e64 5f74 6865 6e60 2061 6e64 2060  `and_then` and `
+000265c0: 616e 645f 7468 656e 5f61 7761 6974 600a  and_then_await`.
+000265d0: 0a43 6f63 6f6e 7574 2070 726f 7669 6465  .Coconut provide
+000265e0: 7320 7468 6520 6061 6e64 5f74 6865 6e60  s the `and_then`
+000265f0: 2061 6e64 2060 616e 645f 7468 656e 5f61   and `and_then_a
+00026600: 7761 6974 6020 6275 696c 742d 696e 7320  wait` built-ins 
+00026610: 666f 7220 636f 6d70 6f73 696e 6720 6061  for composing `a
+00026620: 7379 6e63 6020 6675 6e63 7469 6f6e 732e  sync` functions.
+00026630: 2053 7065 6369 6669 6361 6c6c 793a 0a2a   Specifically:.*
+00026640: 2054 6f20 666f 7277 6172 6473 2063 6f6d   To forwards com
+00026650: 706f 7365 2061 6e20 6173 796e 6320 6675  pose an async fu
+00026660: 6e63 7469 6f6e 2060 6173 796e 635f 6660  nction `async_f`
+00026670: 2077 6974 6820 6120 6e6f 726d 616c 2066   with a normal f
+00026680: 756e 6374 696f 6e20 6067 6020 2873 7563  unction `g` (suc
+00026690: 6820 7468 6174 2060 6760 2069 7320 6361  h that `g` is ca
+000266a0: 6c6c 6564 206f 6e20 7468 6520 7265 7375  lled on the resu
+000266b0: 6c74 206f 6620 6061 7761 6974 6069 6e67  lt of `await`ing
+000266c0: 2060 6173 796e 635f 6660 292c 2077 7269   `async_f`), wri
+000266d0: 7465 2060 6061 7379 6e63 5f66 2060 616e  te ``async_f `an
+000266e0: 645f 7468 656e 6020 6760 602e 0a2a 2054  d_then` g``..* T
+000266f0: 6f20 666f 7277 6172 6473 2063 6f6d 706f  o forwards compo
+00026700: 7365 2061 6e20 6173 796e 6320 6675 6e63  se an async func
+00026710: 7469 6f6e 2060 6173 796e 635f 6660 2077  tion `async_f` w
+00026720: 6974 6820 616e 6f74 6865 7220 6173 796e  ith another asyn
+00026730: 6320 6675 6e63 7469 6f6e 2060 6173 796e  c function `asyn
+00026740: 635f 6760 2028 7375 6368 2074 6861 7420  c_g` (such that 
+00026750: 6061 7379 6e63 5f67 6020 6973 2063 616c  `async_g` is cal
+00026760: 6c65 6420 6f6e 2074 6865 2072 6573 756c  led on the resul
+00026770: 7420 6f66 2060 6177 6169 7460 696e 6720  t of `await`ing 
+00026780: 6061 7379 6e63 5f66 602c 2061 6e64 2074  `async_f`, and t
+00026790: 6865 6e20 6061 7379 6e63 5f67 6020 6973  hen `async_g` is
+000267a0: 2069 7473 656c 6620 6177 6169 7465 6429   itself awaited)
+000267b0: 2c20 7772 6974 6520 6060 6173 796e 635f  , write ``async_
+000267c0: 6620 6061 6e64 5f74 6865 6e5f 6177 6169  f `and_then_awai
+000267d0: 7460 2061 7379 6e63 5f67 6060 2e0a 2a20  t` async_g``..* 
+000267e0: 546f 2066 6f72 7761 7264 7320 636f 6d70  To forwards comp
+000267f0: 6f73 6520 6120 6e6f 726d 616c 2066 756e  ose a normal fun
+00026800: 6374 696f 6e20 6066 6020 7769 7468 2061  ction `f` with a
+00026810: 6e20 6173 796e 6320 6675 6e63 7469 6f6e  n async function
+00026820: 2060 6173 796e 635f 6760 2028 7375 6368   `async_g` (such
+00026830: 2074 6861 7420 6061 7379 6e63 5f67 6020   that `async_g` 
+00026840: 6973 2063 616c 6c65 6420 6f6e 2074 6865  is called on the
+00026850: 2072 6573 756c 7420 6f66 2060 6660 292c   result of `f`),
+00026860: 206a 7573 7420 7772 6974 6520 6066 202e   just write `f .
+00026870: 2e3e 2061 7379 6e63 5f67 602e 0a0a 4e6f  .> async_g`...No
+00026880: 7465 2074 6861 7420 616c 6c20 6f66 2074  te that all of t
+00026890: 6865 2061 626f 7665 2077 696c 6c20 616c  he above will al
+000268a0: 7761 7973 2072 6573 756c 7420 696e 2074  ways result in t
+000268b0: 6865 2072 6573 756c 7469 6e67 2063 6f6d  he resulting com
+000268c0: 706f 7369 7469 6f6e 2062 6569 6e67 2061  position being a
+000268d0: 6e20 6061 7379 6e63 6020 6675 6e63 7469  n `async` functi
+000268e0: 6f6e 2e0a 0a54 6865 2062 7569 6c74 2d69  on...The built-i
+000268f0: 6e73 2061 7265 2065 6666 6563 7469 7665  ns are effective
+00026900: 6c79 2065 7175 6976 616c 656e 7420 746f  ly equivalent to
+00026910: 3a0a 6060 6063 6f63 6f6e 7574 0a64 6566  :.```coconut.def
+00026920: 2061 6e64 5f74 6865 6e5b 2a2a 542c 2055   and_then[**T, U
+00026930: 2c20 565d 280a 2020 2020 6669 7273 745f  , V](.    first_
+00026940: 6173 796e 635f 6675 6e63 3a20 6173 796e  async_func: asyn
+00026950: 6320 282a 2a54 2920 2d3e 2055 2c0a 2020  c (**T) -> U,.  
+00026960: 2020 7365 636f 6e64 5f66 756e 633a 2055    second_func: U
+00026970: 202d 3e20 562c 0a29 202d 3e20 6173 796e   -> V,.) -> asyn
+00026980: 6320 282a 2a54 2920 2d3e 2056 203d 0a20  c (**T) -> V =. 
+00026990: 2020 2061 7379 6e63 2064 6566 2028 2a61     async def (*a
+000269a0: 7267 732c 202a 2a6b 7761 7267 7329 202d  rgs, **kwargs) -
+000269b0: 3e20 280a 2020 2020 2020 2020 6669 7273  > (.        firs
+000269c0: 745f 6173 796e 635f 6675 6e63 282a 6172  t_async_func(*ar
+000269d0: 6773 2c20 2a2a 6b77 6172 6773 290a 2020  gs, **kwargs).  
+000269e0: 2020 2020 2020 7c3e 2061 7761 6974 0a20        |> await. 
+000269f0: 2020 2020 2020 207c 3e20 7365 636f 6e64         |> second
+00026a00: 5f66 756e 630a 2020 2020 290a 0a64 6566  _func.    )..def
+00026a10: 2061 6e64 5f74 6865 6e5f 6177 6169 745b   and_then_await[
+00026a20: 2a2a 542c 2055 2c20 565d 280a 2020 2020  **T, U, V](.    
+00026a30: 6669 7273 745f 6173 796e 635f 6675 6e63  first_async_func
+00026a40: 3a20 6173 796e 6320 282a 2a54 2920 2d3e  : async (**T) ->
+00026a50: 2055 2c0a 2020 2020 7365 636f 6e64 5f61   U,.    second_a
+00026a60: 7379 6e63 5f66 756e 633a 2061 7379 6e63  sync_func: async
+00026a70: 2055 202d 3e20 562c 0a29 202d 3e20 6173   U -> V,.) -> as
+00026a80: 796e 6320 282a 2a54 2920 2d3e 2056 203d  ync (**T) -> V =
+00026a90: 0a20 2020 2061 7379 6e63 2064 6566 2028  .    async def (
+00026aa0: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+00026ab0: 202d 3e20 280a 2020 2020 2020 2020 6669   -> (.        fi
+00026ac0: 7273 745f 6173 796e 635f 6675 6e63 282a  rst_async_func(*
+00026ad0: 6172 6773 2c20 2a2a 6b77 6172 6773 290a  args, **kwargs).
+00026ae0: 2020 2020 2020 2020 7c3e 2061 7761 6974          |> await
+00026af0: 0a20 2020 2020 2020 207c 3e20 7365 636f  .        |> seco
+00026b00: 6e64 5f61 7379 6e63 5f66 756e 630a 2020  nd_async_func.  
+00026b10: 2020 2020 2020 7c3e 2061 7761 6974 0a20        |> await. 
+00026b20: 2020 2029 0a60 6060 0a0a 4c69 6b65 206e     ).```..Like n
+00026b30: 6f72 6d61 6c20 5b66 756e 6374 696f 6e20  ormal [function 
+00026b40: 636f 6d70 6f73 6974 696f 6e5d 2823 6675  composition](#fu
+00026b50: 6e63 7469 6f6e 2d63 6f6d 706f 7369 7469  nction-compositi
+00026b60: 6f6e 292c 2060 616e 645f 7468 656e 6020  on), `and_then` 
+00026b70: 616e 6420 6061 6e64 5f74 6865 6e5f 6177  and `and_then_aw
+00026b80: 6169 7460 2077 696c 6c20 7072 6573 6572  ait` will preser
+00026b90: 7665 2061 6c6c 206d 6574 6164 6174 6120  ve all metadata 
+00026ba0: 6174 7461 6368 6564 2074 6f20 7468 6520  attached to the 
+00026bb0: 6669 7273 7420 6675 6e63 7469 6f6e 2069  first function i
+00026bc0: 6e20 7468 6520 636f 6d70 6f73 6974 696f  n the compositio
+00026bd0: 6e2e 0a0a 2323 2323 2320 4578 616d 706c  n...##### Exampl
+00026be0: 650a 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a  e..**Coconut:**.
+00026bf0: 6060 6063 6f63 6f6e 7574 0a6c 6f61 645f  ```coconut.load_
+00026c00: 616e 645f 7365 6e64 5f64 6174 6120 3d20  and_send_data = 
+00026c10: 280a 2020 2020 6c6f 6164 5f64 6174 615f  (.    load_data_
+00026c20: 6173 796e 6328 290a 2020 2020 6061 6e64  async().    `and
+00026c30: 5f74 6865 6e60 2070 726f 635f 6461 7461  _then` proc_data
+00026c40: 0a20 2020 2060 616e 645f 7468 656e 5f61  .    `and_then_a
+00026c50: 7761 6974 6020 7365 6e64 5f64 6174 610a  wait` send_data.
+00026c60: 290a 6060 600a 0a2a 2a50 7974 686f 6e3a  ).```..**Python:
+00026c70: 2a2a 0a60 6060 636f 636f 6e75 745f 7079  **.```coconut_py
+00026c80: 7468 6f6e 0a61 7379 6e63 2064 6566 206c  thon.async def l
+00026c90: 6f61 645f 616e 645f 7365 6e64 5f64 6174  oad_and_send_dat
+00026ca0: 6128 293a 0a20 2020 2072 6574 7572 6e20  a():.    return 
+00026cb0: 6177 6169 7420 7365 6e64 5f64 6174 6128  await send_data(
+00026cc0: 7072 6f63 5f64 6174 6128 6177 6169 7420  proc_data(await 
+00026cd0: 6c6f 6164 5f64 6174 615f 6173 796e 6328  load_data_async(
+00026ce0: 2929 290a 6060 600a 0a23 2323 2042 7569  ))).```..### Bui
+00026cf0: 6c74 2d49 6e73 2066 6f72 2057 6f72 6b69  lt-Ins for Worki
+00026d00: 6e67 2077 6974 6820 4974 6572 6174 6f72  ng with Iterator
+00026d10: 730a 0a60 6060 7b63 6f6e 7465 6e74 737d  s..```{contents}
+00026d20: 0a2d 2d2d 0a6c 6f63 616c 3a0a 6465 7074  .---.local:.dept
+00026d30: 683a 2031 0a2d 2d2d 0a60 6060 0a0a 2323  h: 1.---.```..##
+00026d40: 2323 2045 6e68 616e 6365 6420 4275 696c  ## Enhanced Buil
+00026d50: 742d 496e 730a 0a43 6f63 6f6e 7574 2773  t-Ins..Coconut's
+00026d60: 2060 6d61 7060 2c20 607a 6970 602c 2060   `map`, `zip`, `
+00026d70: 6669 6c74 6572 602c 2060 7265 7665 7273  filter`, `revers
+00026d80: 6564 602c 2061 6e64 2060 656e 756d 6572  ed`, and `enumer
+00026d90: 6174 6560 206f 626a 6563 7473 2061 7265  ate` objects are
+00026da0: 2065 6e68 616e 6365 6420 7665 7273 696f   enhanced versio
+00026db0: 6e73 206f 6620 7468 6569 7220 5079 7468  ns of their Pyth
+00026dc0: 6f6e 2065 7175 6976 616c 656e 7473 2074  on equivalents t
+00026dd0: 6861 7420 7375 7070 6f72 743a 0a0a 2d20  hat support:..- 
+00026de0: 6072 6576 6572 7365 6460 0a2d 2060 7265  `reversed`.- `re
+00026df0: 7072 600a 2d20 4f70 7469 6d69 7a65 6420  pr`.- Optimized 
+00026e00: 6e6f 726d 616c 2028 616e 6420 6974 6572  normal (and iter
+00026e10: 6174 6f72 2920 696e 6465 7869 6e67 2f73  ator) indexing/s
+00026e20: 6c69 6369 6e67 2028 606d 6170 602c 2060  licing (`map`, `
+00026e30: 7a69 7060 2c20 6072 6576 6572 7365 6460  zip`, `reversed`
+00026e40: 2c20 616e 6420 6065 6e75 6d65 7261 7465  , and `enumerate
+00026e50: 6020 6275 7420 6e6f 7420 6066 696c 7465  ` but not `filte
+00026e60: 7260 292e 0a2d 2060 6c65 6e60 2028 616c  r`)..- `len` (al
+00026e70: 6c20 6275 7420 6066 696c 7465 7260 2920  l but `filter`) 
+00026e80: 2874 686f 7567 6820 6062 6f6f 6c60 2077  (though `bool` w
+00026e90: 696c 6c20 7374 696c 6c20 616c 7761 7973  ill still always
+00026ea0: 2079 6965 6c64 2060 5472 7565 6029 2e0a   yield `True`)..
+00026eb0: 2d20 5468 6520 6162 696c 6974 7920 746f  - The ability to
+00026ec0: 2062 6520 6974 6572 6174 6564 206f 7665   be iterated ove
+00026ed0: 7220 6d75 6c74 6970 6c65 2074 696d 6573  r multiple times
+00026ee0: 2069 6620 7468 6520 756e 6465 726c 7969   if the underlyi
+00026ef0: 6e67 2069 7465 7261 746f 7273 2063 616e  ng iterators can
+00026f00: 2062 6520 6974 6572 6174 6564 206f 7665   be iterated ove
+00026f10: 7220 6d75 6c74 6970 6c65 2074 696d 6573  r multiple times
+00026f20: 2e0a 2d20 5b50 4550 2036 3138 5d28 6874  ..- [PEP 618](ht
+00026f30: 7470 733a 2f2f 7777 772e 7079 7468 6f6e  tps://www.python
+00026f40: 2e6f 7267 2f64 6576 2f70 6570 732f 7065  .org/dev/peps/pe
+00026f50: 702d 3036 3138 2920 607a 6970 282e 2e2e  p-0618) `zip(...
+00026f60: 2c20 7374 7269 6374 3d54 7275 6529 6020  , strict=True)` 
+00026f70: 7375 7070 6f72 7420 6f6e 2061 6c6c 2050  support on all P
+00026f80: 7974 686f 6e20 7665 7273 696f 6e73 2e0a  ython versions..
+00026f90: 2d20 4164 6465 6420 6073 7472 6963 743d  - Added `strict=
+00026fa0: 5472 7565 6020 7375 7070 6f72 7420 746f  True` support to
+00026fb0: 2060 6d61 7060 2061 7320 7765 6c6c 2028   `map` as well (
+00026fc0: 656e 666f 7263 6573 2074 6861 7420 6974  enforces that it
+00026fd0: 6572 6162 6c65 7320 6172 6520 7468 6520  erables are the 
+00026fe0: 7361 6d65 206c 656e 6774 6820 696e 2074  same length in t
+00026ff0: 6865 206d 756c 7469 2d69 7465 7261 626c  he multi-iterabl
+00027000: 6520 6361 7365 3b20 7573 6573 2060 7a69  e case; uses `zi
+00027010: 7060 2075 6e64 6572 2074 6865 2068 6f6f  p` under the hoo
+00027020: 6420 7375 6368 2074 6861 7420 6572 726f  d such that erro
+00027030: 7273 2077 696c 6c20 7368 6f77 2075 7020  rs will show up 
+00027040: 6173 2060 7a69 7028 2e2e 2e2c 2073 7472  as `zip(..., str
+00027050: 6963 743d 5472 7565 2960 2065 7272 6f72  ict=True)` error
+00027060: 7329 2e0a 2d20 4164 6465 6420 6174 7472  s)..- Added attr
+00027070: 6962 7574 6573 2077 6869 6368 2073 7562  ibutes which sub
+00027080: 636c 6173 7365 7320 6361 6e20 6d61 6b65  classes can make
+00027090: 2075 7365 206f 6620 746f 2067 6574 2061   use of to get a
+000270a0: 7420 7468 6520 6f72 6967 696e 616c 2061  t the original a
+000270b0: 7267 756d 656e 7473 2074 6f20 7468 6520  rguments to the 
+000270c0: 6f62 6a65 6374 3a0a 2020 2a20 606d 6170  object:.  * `map
+000270d0: 603a 2060 6675 6e63 602c 2060 6974 6572  `: `func`, `iter
+000270e0: 7360 0a20 202a 2060 7a69 7060 3a20 6069  s`.  * `zip`: `i
+000270f0: 7465 7273 600a 2020 2a20 6066 696c 7465  ters`.  * `filte
+00027100: 7260 3a20 6066 756e 6360 2c20 6069 7465  r`: `func`, `ite
+00027110: 7260 0a20 202a 2060 7265 7665 7273 6564  r`.  * `reversed
+00027120: 603a 2060 6974 6572 600a 2020 2a20 6065  `: `iter`.  * `e
+00027130: 6e75 6d65 7261 7465 603a 2060 6974 6572  numerate`: `iter
+00027140: 602c 2060 7374 6172 7460 0a0a 2323 2323  `, `start`..####
+00027150: 2320 496e 6465 7869 6e67 2069 6e74 6f20  # Indexing into 
+00027160: 6f74 6865 7220 6275 696c 742d 696e 730a  other built-ins.
+00027170: 0a54 686f 7567 6820 436f 636f 6e75 7420  .Though Coconut 
+00027180: 7072 6f76 6964 6573 2072 616e 646f 6d20  provides random 
+00027190: 6163 6365 7373 2069 6e64 6578 696e 672f  access indexing/
+000271a0: 736c 6963 696e 6720 746f 2060 7261 6e67  slicing to `rang
+000271b0: 6560 2c20 606d 6170 602c 2060 7a69 7060  e`, `map`, `zip`
+000271c0: 2c20 6072 6576 6572 7365 6460 2c20 616e  , `reversed`, an
+000271d0: 6420 6065 6e75 6d65 7261 7465 602c 2043  d `enumerate`, C
+000271e0: 6f63 6f6e 7574 2063 616e 6e6f 7420 696e  oconut cannot in
+000271f0: 6465 7820 696e 746f 2062 7569 6c74 2d69  dex into built-i
+00027200: 6e73 206c 696b 6520 6066 696c 7465 7260  ns like `filter`
+00027210: 2c20 6074 616b 6577 6869 6c65 602c 206f  , `takewhile`, o
+00027220: 7220 6064 726f 7077 6869 6c65 6020 6469  r `dropwhile` di
+00027230: 7265 6374 6c79 2c20 6173 2074 6865 7265  rectly, as there
+00027240: 2069 7320 6e6f 2065 6666 6963 6965 6e74   is no efficient
+00027250: 2077 6179 2074 6f20 646f 2073 6f2e 0a0a   way to do so...
+00027260: 6060 6063 6f63 6f6e 7574 0a72 616e 6765  ```coconut.range
+00027270: 2831 3029 207c 3e20 6669 6c74 6572 2428  (10) |> filter$(
+00027280: 692d 3e69 3e33 2920 7c3e 202e 5b30 5d20  i->i>3) |> .[0] 
+00027290: 2023 2064 6f65 736e 2774 2077 6f72 6b0a   # doesn't work.
+000272a0: 6060 600a 0a49 6e20 6f72 6465 7220 746f  ```..In order to
+000272b0: 206d 616b 6520 7468 6973 2077 6f72 6b2c   make this work,
+000272c0: 2079 6f75 2063 616e 2065 7870 6c69 6369   you can explici
+000272d0: 746c 7920 7573 6520 6974 6572 6174 6f72  tly use iterator
+000272e0: 2073 6c69 6369 6e67 2c20 7768 6963 6820   slicing, which 
+000272f0: 6973 206c 6573 7320 6566 6669 6369 656e  is less efficien
+00027300: 7420 696e 2074 6865 2067 656e 6572 616c  t in the general
+00027310: 2063 6173 653a 0a0a 6060 6063 6f63 6f6e   case:..```cocon
+00027320: 7574 0a72 616e 6765 2831 3029 207c 3e20  ut.range(10) |> 
+00027330: 6669 6c74 6572 2428 692d 3e69 3e33 2920  filter$(i->i>3) 
+00027340: 7c3e 202e 245b 305d 2020 2320 776f 726b  |> .$[0]  # work
+00027350: 730a 6060 600a 0a46 6f72 206d 6f72 6520  s.```..For more 
+00027360: 696e 666f 726d 6174 696f 6e20 6f6e 2043  information on C
+00027370: 6f63 6f6e 7574 2773 2069 7465 7261 746f  oconut's iterato
+00027380: 7220 736c 6963 696e 672c 2073 6565 205b  r slicing, see [
+00027390: 6865 7265 5d28 2369 7465 7261 746f 722d  here](#iterator-
+000273a0: 736c 6963 696e 6729 2e0a 0a23 2323 2323  slicing)...#####
+000273b0: 2045 7861 6d70 6c65 730a 0a2a 2a43 6f63   Examples..**Coc
+000273c0: 6f6e 7574 3a2a 2a0a 6060 6063 6f63 6f6e  onut:**.```cocon
+000273d0: 7574 0a6d 6170 2828 2b29 2c20 7261 6e67  ut.map((+), rang
+000273e0: 6528 3529 2c20 7261 6e67 6528 3629 2920  e(5), range(6)) 
+000273f0: 7c3e 206c 656e 207c 3e20 7072 696e 740a  |> len |> print.
+00027400: 7261 6e67 6528 3130 2920 7c3e 2066 696c  range(10) |> fil
+00027410: 7465 7224 2828 7829 202d 3e20 7820 3c20  ter$((x) -> x < 
+00027420: 3529 207c 3e20 7265 7665 7273 6564 207c  5) |> reversed |
+00027430: 3e20 7475 706c 6520 7c3e 2070 7269 6e74  > tuple |> print
+00027440: 0a60 6060 0a0a 2a2a 5079 7468 6f6e 3a2a  .```..**Python:*
+00027450: 2a0a 5f43 616e 2774 2062 6520 646f 6e65  *._Can't be done
+00027460: 2077 6974 686f 7574 2064 6566 696e 696e   without definin
+00027470: 6720 6120 6375 7374 6f6d 2060 6d61 7060  g a custom `map`
+00027480: 2074 7970 652e 2054 6865 2066 756c 6c20   type. The full 
+00027490: 6465 6669 6e69 7469 6f6e 206f 6620 606d  definition of `m
+000274a0: 6170 6020 6361 6e20 6265 2066 6f75 6e64  ap` can be found
+000274b0: 2069 6e20 7468 6520 436f 636f 6e75 7420   in the Coconut 
+000274c0: 6865 6164 6572 2e5f 0a0a 2a2a 436f 636f  header._..**Coco
+000274d0: 6e75 743a 2a2a 0a60 6060 636f 636f 6e75  nut:**.```coconu
+000274e0: 740a 7261 6e67 6528 302c 2031 322c 2032  t.range(0, 12, 2
+000274f0: 295b 345d 2020 2320 380a 0a6d 6170 2828  )[4]  # 8..map((
+00027500: 692d 3e69 2a32 292c 2072 616e 6765 2831  i->i*2), range(1
+00027510: 3029 295b 325d 2020 2320 340a 6060 600a  0))[2]  # 4.```.
+00027520: 0a2a 2a50 7974 686f 6e3a 2a2a 0a5f 4361  .**Python:**._Ca
+00027530: 6ee2 8099 7420 6265 2064 6f6e 6520 7175  n...t be done qu
+00027540: 6963 6b6c 7920 7769 7468 6f75 7420 436f  ickly without Co
+00027550: 636f 6e75 74e2 8099 7320 6974 6572 6162  conut...s iterab
+00027560: 6c65 2069 6e64 6578 696e 672c 2077 6869  le indexing, whi
+00027570: 6368 2072 6571 7569 7265 7320 6d61 6e79  ch requires many
+00027580: 2063 6f6d 706c 6963 6174 6564 2070 6965   complicated pie
+00027590: 6365 732e 2054 6865 206e 6563 6573 7361  ces. The necessa
+000275a0: 7279 2064 6566 696e 6974 696f 6e73 2069  ry definitions i
+000275b0: 6e20 5079 7468 6f6e 2063 616e 2062 6520  n Python can be 
+000275c0: 666f 756e 6420 696e 2074 6865 2043 6f63  found in the Coc
+000275d0: 6f6e 7574 2068 6561 6465 722e 5f0a 0a23  onut header._..#
+000275e0: 2323 2320 6072 6564 7563 6560 0a0a 2a2a  ### `reduce`..**
+000275f0: 7265 6475 6365 2a2a 285f 6675 6e63 7469  reduce**(_functi
+00027600: 6f6e 5f2c 205f 6974 6572 6162 6c65 5f5b  on_, _iterable_[
+00027610: 2c20 5f69 6e69 7469 616c 5f5d 2c20 2f29  , _initial_], /)
+00027620: 0a0a 436f 636f 6e75 7420 7265 2d69 6e74  ..Coconut re-int
+00027630: 726f 6475 6365 7320 5079 7468 6f6e 2032  roduces Python 2
+00027640: 2773 2060 7265 6475 6365 6020 6275 696c  's `reduce` buil
+00027650: 742d 696e 2c20 7573 696e 6720 7468 6520  t-in, using the 
+00027660: 6066 756e 6374 6f6f 6c73 2e72 6564 7563  `functools.reduc
+00027670: 6560 2076 6572 7369 6f6e 2e0a 0a23 2323  e` version...###
+00027680: 2323 2050 7974 686f 6e20 446f 6373 0a0a  ## Python Docs..
+00027690: 2a2a 7265 6475 6365 2a2a 285f 6675 6e63  **reduce**(_func
+000276a0: 7469 6f6e 2c20 6974 6572 6162 6c65 5f2a  tion, iterable_*
+000276b0: 2a5b 2a2a 5f2c 2069 6e69 7469 616c 5f2a  *[**_, initial_*
+000276c0: 2a5d 2a2a 290a 0a41 7070 6c79 205f 6675  *]**)..Apply _fu
+000276d0: 6e63 7469 6f6e 5f20 6f66 2074 776f 2061  nction_ of two a
+000276e0: 7267 756d 656e 7473 2063 756d 756c 6174  rguments cumulat
+000276f0: 6976 656c 7920 746f 2074 6865 2069 7465  ively to the ite
+00027700: 6d73 206f 6620 5f73 6571 7565 6e63 655f  ms of _sequence_
+00027710: 2c20 6672 6f6d 206c 6566 7420 746f 2072  , from left to r
+00027720: 6967 6874 2c20 736f 2061 7320 746f 2072  ight, so as to r
+00027730: 6564 7563 6520 7468 6520 7365 7175 656e  educe the sequen
+00027740: 6365 2074 6f20 6120 7369 6e67 6c65 2076  ce to a single v
+00027750: 616c 7565 2e20 466f 7220 6578 616d 706c  alue. For exampl
+00027760: 652c 2060 7265 6475 6365 2828 782c 2079  e, `reduce((x, y
+00027770: 2920 2d3e 2078 2b79 2c20 5b31 2c20 322c  ) -> x+y, [1, 2,
+00027780: 2033 2c20 342c 2035 5d29 6020 6361 6c63   3, 4, 5])` calc
+00027790: 756c 6174 6573 2060 2828 2828 312b 3229  ulates `((((1+2)
+000277a0: 2b33 292b 3429 2b35 2960 2e20 5468 6520  +3)+4)+5)`. The 
+000277b0: 6c65 6674 2061 7267 756d 656e 742c 205f  left argument, _
+000277c0: 785f 2c20 6973 2074 6865 2061 6363 756d  x_, is the accum
+000277d0: 756c 6174 6564 2076 616c 7565 2061 6e64  ulated value and
+000277e0: 2074 6865 2072 6967 6874 2061 7267 756d   the right argum
+000277f0: 656e 742c 205f 795f 2c20 6973 2074 6865  ent, _y_, is the
+00027800: 2075 7064 6174 6520 7661 6c75 6520 6672   update value fr
+00027810: 6f6d 2074 6865 205f 7365 7175 656e 6365  om the _sequence
+00027820: 5f2e 2049 6620 7468 6520 6f70 7469 6f6e  _. If the option
+00027830: 616c 205f 696e 6974 6961 6c5f 2069 7320  al _initial_ is 
+00027840: 7072 6573 656e 742c 2069 7420 6973 2070  present, it is p
+00027850: 6c61 6365 6420 6265 666f 7265 2074 6865  laced before the
+00027860: 2069 7465 6d73 206f 6620 7468 6520 7365   items of the se
+00027870: 7175 656e 6365 2069 6e20 7468 6520 6361  quence in the ca
+00027880: 6c63 756c 6174 696f 6e2c 2061 6e64 2073  lculation, and s
+00027890: 6572 7665 7320 6173 2061 2064 6566 6175  erves as a defau
+000278a0: 6c74 2077 6865 6e20 7468 6520 7365 7175  lt when the sequ
+000278b0: 656e 6365 2069 7320 656d 7074 792e 2049  ence is empty. I
+000278c0: 6620 5f69 6e69 7469 616c 5f20 6973 206e  f _initial_ is n
+000278d0: 6f74 2067 6976 656e 2061 6e64 205f 7365  ot given and _se
+000278e0: 7175 656e 6365 5f20 636f 6e74 6169 6e73  quence_ contains
+000278f0: 206f 6e6c 7920 6f6e 6520 6974 656d 2c20   only one item, 
+00027900: 7468 6520 6669 7273 7420 6974 656d 2069  the first item i
+00027910: 7320 7265 7475 726e 6564 2e0a 0a23 2323  s returned...###
+00027920: 2323 2045 7861 6d70 6c65 0a0a 2a2a 436f  ## Example..**Co
+00027930: 636f 6e75 743a 2a2a 0a60 6060 636f 636f  conut:**.```coco
+00027940: 6e75 740a 7072 6f64 7563 7420 3d20 7265  nut.product = re
+00027950: 6475 6365 2428 2a29 0a72 616e 6765 2831  duce$(*).range(1
+00027960: 2c20 3130 2920 7c3e 2070 726f 6475 6374  , 10) |> product
+00027970: 207c 3e20 7072 696e 740a 6060 600a 0a2a   |> print.```..*
+00027980: 2a50 7974 686f 6e3a 2a2a 0a60 6060 636f  *Python:**.```co
+00027990: 636f 6e75 745f 7079 7468 6f6e 0a69 6d70  conut_python.imp
+000279a0: 6f72 7420 6f70 6572 6174 6f72 0a69 6d70  ort operator.imp
+000279b0: 6f72 7420 6675 6e63 746f 6f6c 730a 7072  ort functools.pr
+000279c0: 6f64 7563 7420 3d20 6675 6e63 746f 6f6c  oduct = functool
+000279d0: 732e 7061 7274 6961 6c28 6675 6e63 746f  s.partial(functo
+000279e0: 6f6c 732e 7265 6475 6365 2c20 6f70 6572  ols.reduce, oper
+000279f0: 6174 6f72 2e6d 756c 290a 7072 696e 7428  ator.mul).print(
+00027a00: 7072 6f64 7563 7428 7261 6e67 6528 312c  product(range(1,
+00027a10: 2031 3029 2929 0a60 6060 0a0a 2323 2323   10))).```..####
+00027a20: 2060 7265 6974 6572 6162 6c65 600a 0a2a   `reiterable`..*
+00027a30: 2a72 6569 7465 7261 626c 652a 2a28 5f69  *reiterable**(_i
+00027a40: 7465 7261 626c 655f 290a 0a60 7265 6974  terable_)..`reit
+00027a50: 6572 6162 6c65 6020 7772 6170 7320 7468  erable` wraps th
+00027a60: 6520 6769 7665 6e20 6974 6572 6162 6c65  e given iterable
+00027a70: 2074 6f20 656e 7375 7265 2074 6861 7420   to ensure that 
+00027a80: 6576 6572 7920 7469 6d65 2074 6865 2060  every time the `
+00027a90: 7265 6974 6572 6162 6c65 6020 6973 2069  reiterable` is i
+00027aa0: 7465 7261 7465 6420 6f76 6572 2c20 6974  terated over, it
+00027ab0: 2070 726f 6475 6365 7320 7468 6520 7361   produces the sa
+00027ac0: 6d65 2072 6573 756c 7473 2e20 4e6f 7465  me results. Note
+00027ad0: 2074 6861 7420 7468 6520 7265 7375 6c74   that the result
+00027ae0: 206e 6565 6420 6e6f 7420 6265 2061 2060   need not be a `
+00027af0: 7265 6974 6572 6162 6c65 6020 6f62 6a65  reiterable` obje
+00027b00: 6374 2069 6620 7468 6520 6769 7665 6e20  ct if the given 
+00027b10: 6974 6572 6162 6c65 2069 7320 616c 7265  iterable is alre
+00027b20: 6164 7920 7265 6974 6572 6162 6c65 2e20  ady reiterable. 
+00027b30: 6072 6569 7465 7261 626c 6560 2075 7365  `reiterable` use
+00027b40: 7320 5b60 7465 6560 5d28 2374 6565 2920  s [`tee`](#tee) 
+00027b50: 756e 6465 7220 7468 6520 686f 6f64 2061  under the hood a
+00027b60: 6e64 2060 7465 6560 2063 616e 2062 6520  nd `tee` can be 
+00027b70: 7573 6564 2069 6e20 6974 7320 706c 6163  used in its plac
+00027b80: 652c 2074 686f 7567 6820 6072 6569 7465  e, though `reite
+00027b90: 7261 626c 6560 2069 7320 6765 6e65 7261  rable` is genera
+00027ba0: 6c6c 7920 7265 636f 6d6d 656e 6465 6420  lly recommended 
+00027bb0: 6f76 6572 2060 7465 6560 2e0a 0a23 2323  over `tee`...###
+00027bc0: 2323 2045 7861 6d70 6c65 0a0a 2a2a 436f  ## Example..**Co
+00027bd0: 636f 6e75 743a 2a2a 0a60 6060 636f 636f  conut:**.```coco
+00027be0: 6e75 740a 6465 6620 6c69 7374 5f74 7970  nut.def list_typ
+00027bf0: 6528 7873 293a 0a20 2020 206d 6174 6368  e(xs):.    match
+00027c00: 2072 6569 7465 7261 626c 6528 7873 293a   reiterable(xs):
+00027c10: 0a20 2020 2020 2020 2063 6173 6520 5b66  .        case [f
+00027c20: 7374 2c20 736e 645d 203a 3a20 7461 696c  st, snd] :: tail
+00027c30: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00027c40: 7475 726e 2022 6174 206c 6561 7374 2032  turn "at least 2
+00027c50: 220a 2020 2020 2020 2020 6361 7365 205b  ".        case [
+00027c60: 6673 745d 203a 3a20 7461 696c 3a0a 2020  fst] :: tail:.  
+00027c70: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00027c80: 2022 6174 206c 6561 7374 2031 220a 2020   "at least 1".  
+00027c90: 2020 2020 2020 6361 7365 2028 7c20 7c29        case (| |)
+00027ca0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00027cb0: 7475 726e 2022 656d 7074 7922 0a60 6060  turn "empty".```
+00027cc0: 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a 5f43  ..**Python:**._C
+00027cd0: 616e 2774 2062 6520 646f 6e65 2077 6974  an't be done wit
+00027ce0: 686f 7574 2061 206c 6f6e 6720 7365 7269  hout a long seri
+00027cf0: 6573 206f 6620 6368 6563 6b73 2066 6f72  es of checks for
+00027d00: 2065 6163 6820 606d 6174 6368 6020 7374   each `match` st
+00027d10: 6174 656d 656e 742e 2053 6565 2074 6865  atement. See the
+00027d20: 2063 6f6d 7069 6c65 6420 636f 6465 2066   compiled code f
+00027d30: 6f72 2074 6865 2050 7974 686f 6e20 7379  or the Python sy
+00027d40: 6e74 6178 2e5f 0a0a 2323 2323 2060 7374  ntax._..#### `st
+00027d50: 6172 6d61 7060 0a0a 2a2a 7374 6172 6d61  armap`..**starma
+00027d60: 702a 2a28 5f66 756e 6374 696f 6e5f 2c20  p**(_function_, 
+00027d70: 5f69 7465 7261 626c 655f 290a 0a43 6f63  _iterable_)..Coc
+00027d80: 6f6e 7574 2070 726f 7669 6465 7320 6120  onut provides a 
+00027d90: 6d6f 6469 6669 6564 2076 6572 7369 6f6e  modified version
+00027da0: 206f 6620 6069 7465 7274 6f6f 6c73 2e73   of `itertools.s
+00027db0: 7461 726d 6170 6020 7468 6174 2073 7570  tarmap` that sup
+00027dc0: 706f 7274 7320 6072 6576 6572 7365 6460  ports `reversed`
+00027dd0: 2c20 6072 6570 7260 2c20 6f70 7469 6d69  , `repr`, optimi
+00027de0: 7a65 6420 6e6f 726d 616c 2028 616e 6420  zed normal (and 
+00027df0: 6974 6572 6174 6f72 2920 736c 6963 696e  iterator) slicin
+00027e00: 672c 2060 6c65 6e60 2c20 616e 6420 6066  g, `len`, and `f
+00027e10: 756e 6360 2f60 6974 6572 6020 6174 7472  unc`/`iter` attr
+00027e20: 6962 7574 6573 2e0a 0a23 2323 2323 2050  ibutes...##### P
+00027e30: 7974 686f 6e20 446f 6373 0a0a 2a2a 7374  ython Docs..**st
+00027e40: 6172 6d61 702a 2a28 5f66 756e 6374 696f  armap**(_functio
+00027e50: 6e2c 2069 7465 7261 626c 655f 290a 0a4d  n, iterable_)..M
+00027e60: 616b 6520 616e 2069 7465 7261 746f 7220  ake an iterator 
+00027e70: 7468 6174 2063 6f6d 7075 7465 7320 7468  that computes th
+00027e80: 6520 6675 6e63 7469 6f6e 2075 7369 6e67  e function using
+00027e90: 2061 7267 756d 656e 7473 206f 6274 6169   arguments obtai
+00027ea0: 6e65 6420 6672 6f6d 2074 6865 2069 7465  ned from the ite
+00027eb0: 7261 626c 652e 2055 7365 6420 696e 7374  rable. Used inst
+00027ec0: 6561 6420 6f66 2060 6d61 7028 2960 2077  ead of `map()` w
+00027ed0: 6865 6e20 6172 6775 6d65 6e74 2070 6172  hen argument par
+00027ee0: 616d 6574 6572 7320 6172 6520 616c 7265  ameters are alre
+00027ef0: 6164 7920 6772 6f75 7065 6420 696e 2074  ady grouped in t
+00027f00: 7570 6c65 7320 6672 6f6d 2061 2073 696e  uples from a sin
+00027f10: 676c 6520 6974 6572 6162 6c65 2028 7468  gle iterable (th
+00027f20: 6520 6461 7461 2068 6173 2062 6565 6e20  e data has been 
+00027f30: 2270 7265 2d7a 6970 7065 6422 292e 2054  "pre-zipped"). T
+00027f40: 6865 2064 6966 6665 7265 6e63 6520 6265  he difference be
+00027f50: 7477 6565 6e20 606d 6170 2829 6020 616e  tween `map()` an
+00027f60: 6420 6073 7461 726d 6170 2829 6020 7061  d `starmap()` pa
+00027f70: 7261 6c6c 656c 7320 7468 6520 6469 7374  rallels the dist
+00027f80: 696e 6374 696f 6e20 6265 7477 6565 6e20  inction between 
+00027f90: 6066 756e 6374 696f 6e28 612c 6229 6020  `function(a,b)` 
+00027fa0: 616e 6420 6066 756e 6374 696f 6e28 2a63  and `function(*c
+00027fb0: 2960 2e20 526f 7567 686c 7920 6571 7569  )`. Roughly equi
+00027fc0: 7661 6c65 6e74 2074 6f3a 0a0a 6060 6063  valent to:..```c
+00027fd0: 6f63 6f6e 7574 5f70 7974 686f 6e0a 6465  oconut_python.de
+00027fe0: 6620 7374 6172 6d61 7028 6675 6e63 7469  f starmap(functi
+00027ff0: 6f6e 2c20 6974 6572 6162 6c65 293a 0a20  on, iterable):. 
+00028000: 2020 2023 2073 7461 726d 6170 2870 6f77     # starmap(pow
+00028010: 2c20 5b28 322c 3529 2c20 2833 2c32 292c  , [(2,5), (3,2),
+00028020: 2028 3130 2c33 295d 2920 2d2d 3e20 3332   (10,3)]) --> 32
+00028030: 2039 2031 3030 300a 2020 2020 666f 7220   9 1000.    for 
+00028040: 6172 6773 2069 6e20 6974 6572 6162 6c65  args in iterable
+00028050: 3a0a 2020 2020 2020 2020 7969 656c 6420  :.        yield 
+00028060: 6675 6e63 7469 6f6e 282a 6172 6773 290a  function(*args).
+00028070: 6060 600a 0a23 2323 2323 2045 7861 6d70  ```..##### Examp
+00028080: 6c65 0a0a 2a2a 436f 636f 6e75 743a 2a2a  le..**Coconut:**
+00028090: 0a60 6060 636f 636f 6e75 740a 7261 6e67  .```coconut.rang
+000280a0: 6528 312c 2035 2920 7c3e 206d 6170 2428  e(1, 5) |> map$(
+000280b0: 7261 6e67 6529 207c 3e20 7374 6172 6d61  range) |> starma
+000280c0: 7024 2870 7269 6e74 2920 7c3e 2063 6f6e  p$(print) |> con
+000280d0: 7375 6d65 0a60 6060 0a0a 2a2a 5079 7468  sume.```..**Pyth
+000280e0: 6f6e 3a2a 2a0a 6060 6063 6f63 6f6e 7574  on:**.```coconut
+000280f0: 5f70 7974 686f 6e0a 696d 706f 7274 2069  _python.import i
+00028100: 7465 7274 6f6f 6c73 2c20 636f 6c6c 6563  tertools, collec
+00028110: 7469 6f6e 730a 636f 6c6c 6563 7469 6f6e  tions.collection
+00028120: 732e 6465 7175 6528 6974 6572 746f 6f6c  s.deque(itertool
+00028130: 732e 7374 6172 6d61 7028 7072 696e 742c  s.starmap(print,
+00028140: 206d 6170 2872 616e 6765 2c20 7261 6e67   map(range, rang
+00028150: 6528 312c 2035 2929 292c 206d 6178 6c65  e(1, 5))), maxle
+00028160: 6e3d 3029 0a60 6060 0a0a 2323 2323 2060  n=0).```..#### `
+00028170: 7a69 705f 6c6f 6e67 6573 7460 0a0a 2a2a  zip_longest`..**
+00028180: 7a69 705c 5f6c 6f6e 6765 7374 2a2a 282a  zip\_longest**(*
+00028190: 5f69 7465 7261 626c 6573 5f2c 205f 6669  _iterables_, _fi
+000281a0: 6c6c 7661 6c75 655f 3d60 4e6f 6e65 6029  llvalue_=`None`)
+000281b0: 0a0a 436f 636f 6e75 7420 7072 6f76 6964  ..Coconut provid
+000281c0: 6573 2061 6e20 656e 6861 6e63 6564 2076  es an enhanced v
+000281d0: 6572 7369 6f6e 206f 6620 6069 7465 7274  ersion of `itert
+000281e0: 6f6f 6c73 2e7a 6970 5f6c 6f6e 6765 7374  ools.zip_longest
+000281f0: 6020 6173 2061 2062 7569 6c74 2d69 6e20  ` as a built-in 
+00028200: 756e 6465 7220 7468 6520 6e61 6d65 2060  under the name `
+00028210: 7a69 705f 6c6f 6e67 6573 7460 2e20 607a  zip_longest`. `z
+00028220: 6970 5f6c 6f6e 6765 7374 6020 7375 7070  ip_longest` supp
+00028230: 6f72 7473 2061 6c6c 2074 6865 2073 616d  orts all the sam
+00028240: 6520 6665 6174 7572 6573 2061 7320 436f  e features as Co
+00028250: 636f 6e75 7427 7320 5b65 6e68 616e 6365  conut's [enhance
+00028260: 6420 7a69 705d 2823 656e 6861 6e63 6564  d zip](#enhanced
+00028270: 2d62 7569 6c74 2d69 6e73 2920 6173 2077  -built-ins) as w
+00028280: 656c 6c20 6173 2074 6865 2061 6464 6974  ell as the addit
+00028290: 696f 6e61 6c20 6174 7472 6962 7574 6520  ional attribute 
+000282a0: 6066 696c 6c76 616c 7565 602e 0a0a 2323  `fillvalue`...##
+000282b0: 2323 2320 5079 7468 6f6e 2044 6f63 730a  ### Python Docs.
+000282c0: 0a2a 2a7a 6970 5c5f 6c6f 6e67 6573 742a  .**zip\_longest*
+000282d0: 2a28 5f5c 2a69 7465 7261 626c 6573 2c20  *(_\*iterables, 
+000282e0: 6669 6c6c 7661 6c75 653d 4e6f 6e65 5f29  fillvalue=None_)
+000282f0: 0a0a 4d61 6b65 2061 6e20 6974 6572 6174  ..Make an iterat
+00028300: 6f72 2074 6861 7420 6167 6772 6567 6174  or that aggregat
+00028310: 6573 2065 6c65 6d65 6e74 7320 6672 6f6d  es elements from
+00028320: 2065 6163 6820 6f66 2074 6865 2069 7465   each of the ite
+00028330: 7261 626c 6573 2e20 4966 2074 6865 2069  rables. If the i
+00028340: 7465 7261 626c 6573 2061 7265 206f 6620  terables are of 
+00028350: 756e 6576 656e 206c 656e 6774 682c 206d  uneven length, m
+00028360: 6973 7369 6e67 2076 616c 7565 7320 6172  issing values ar
+00028370: 6520 6669 6c6c 6564 2d69 6e20 7769 7468  e filled-in with
+00028380: 205f 6669 6c6c 7661 6c75 655f 2e20 4974   _fillvalue_. It
+00028390: 6572 6174 696f 6e20 636f 6e74 696e 7565  eration continue
+000283a0: 7320 756e 7469 6c20 7468 6520 6c6f 6e67  s until the long
+000283b0: 6573 7420 6974 6572 6162 6c65 2069 7320  est iterable is 
+000283c0: 6578 6861 7573 7465 642e 2052 6f75 6768  exhausted. Rough
+000283d0: 6c79 2065 7175 6976 616c 656e 7420 746f  ly equivalent to
+000283e0: 3a0a 0a60 6060 636f 636f 6e75 745f 7079  :..```coconut_py
+000283f0: 7468 6f6e 0a64 6566 207a 6970 5f6c 6f6e  thon.def zip_lon
+00028400: 6765 7374 282a 6172 6773 2c20 6669 6c6c  gest(*args, fill
+00028410: 7661 6c75 653d 4e6f 6e65 293a 0a20 2020  value=None):.   
+00028420: 2023 207a 6970 5f6c 6f6e 6765 7374 2827   # zip_longest('
+00028430: 4142 4344 272c 2027 7879 272c 2066 696c  ABCD', 'xy', fil
+00028440: 6c76 616c 7565 3d27 2d27 2920 2d2d 3e20  lvalue='-') --> 
+00028450: 4178 2042 7920 432d 2044 2d0a 2020 2020  Ax By C- D-.    
+00028460: 6974 6572 6174 6f72 7320 3d20 5b69 7465  iterators = [ite
+00028470: 7228 6974 2920 666f 7220 6974 2069 6e20  r(it) for it in 
+00028480: 6172 6773 5d0a 2020 2020 6e75 6d5f 6163  args].    num_ac
+00028490: 7469 7665 203d 206c 656e 2869 7465 7261  tive = len(itera
+000284a0: 746f 7273 290a 2020 2020 6966 206e 6f74  tors).    if not
+000284b0: 206e 756d 5f61 6374 6976 653a 0a20 2020   num_active:.   
+000284c0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+000284d0: 7768 696c 6520 5472 7565 3a0a 2020 2020  while True:.    
+000284e0: 2020 2020 7661 6c75 6573 203d 205b 5d0a      values = [].
+000284f0: 2020 2020 2020 2020 666f 7220 692c 2069          for i, i
+00028500: 7420 696e 2065 6e75 6d65 7261 7465 2869  t in enumerate(i
+00028510: 7465 7261 746f 7273 293a 0a20 2020 2020  terators):.     
+00028520: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00028530: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00028540: 6520 3d20 6e65 7874 2869 7429 0a20 2020  e = next(it).   
+00028550: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+00028560: 5374 6f70 4974 6572 6174 696f 6e3a 0a20  StopIteration:. 
+00028570: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00028580: 756d 5f61 6374 6976 6520 2d3d 2031 0a20  um_active -= 1. 
+00028590: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000285a0: 6620 6e6f 7420 6e75 6d5f 6163 7469 7665  f not num_active
+000285b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000285c0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+000285d0: 2020 2020 2020 2020 2020 2020 2069 7465               ite
+000285e0: 7261 746f 7273 5b69 5d20 3d20 7265 7065  rators[i] = repe
+000285f0: 6174 2866 696c 6c76 616c 7565 290a 2020  at(fillvalue).  
+00028600: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00028610: 6c75 6520 3d20 6669 6c6c 7661 6c75 650a  lue = fillvalue.
+00028620: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00028630: 6573 2e61 7070 656e 6428 7661 6c75 6529  es.append(value)
+00028640: 0a20 2020 2020 2020 2079 6965 6c64 2074  .        yield t
+00028650: 7570 6c65 2876 616c 7565 7329 0a60 6060  uple(values).```
+00028660: 0a0a 4966 206f 6e65 206f 6620 7468 6520  ..If one of the 
+00028670: 6974 6572 6162 6c65 7320 6973 2070 6f74  iterables is pot
+00028680: 656e 7469 616c 6c79 2069 6e66 696e 6974  entially infinit
+00028690: 652c 2074 6865 6e20 7468 6520 607a 6970  e, then the `zip
+000286a0: 5f6c 6f6e 6765 7374 2829 6020 6675 6e63  _longest()` func
+000286b0: 7469 6f6e 2073 686f 756c 6420 6265 2077  tion should be w
+000286c0: 7261 7070 6564 2077 6974 6820 736f 6d65  rapped with some
+000286d0: 7468 696e 6720 7468 6174 206c 696d 6974  thing that limit
+000286e0: 7320 7468 6520 6e75 6d62 6572 206f 6620  s the number of 
+000286f0: 6361 6c6c 7320 2866 6f72 2065 7861 6d70  calls (for examp
+00028700: 6c65 2069 7465 7261 746f 7220 736c 6963  le iterator slic
+00028710: 696e 6720 6f72 2060 7461 6b65 7768 696c  ing or `takewhil
+00028720: 6560 292e 2049 6620 6e6f 7420 7370 6563  e`). If not spec
+00028730: 6966 6965 642c 205f 6669 6c6c 7661 6c75  ified, _fillvalu
+00028740: 655f 2064 6566 6175 6c74 7320 746f 2060  e_ defaults to `
+00028750: 4e6f 6e65 602e 0a0a 2323 2323 2320 4578  None`...##### Ex
+00028760: 616d 706c 650a 0a2a 2a43 6f63 6f6e 7574  ample..**Coconut
+00028770: 3a2a 2a0a 6060 6063 6f63 6f6e 7574 0a72  :**.```coconut.r
+00028780: 6573 756c 7420 3d20 7a69 705f 6c6f 6e67  esult = zip_long
+00028790: 6573 7428 7261 6e67 6528 3529 2c20 7261  est(range(5), ra
+000287a0: 6e67 6528 3130 2929 0a60 6060 0a0a 2a2a  nge(10)).```..**
+000287b0: 5079 7468 6f6e 3a2a 2a0a 6060 6063 6f63  Python:**.```coc
+000287c0: 6f6e 7574 5f70 7974 686f 6e0a 696d 706f  onut_python.impo
+000287d0: 7274 2069 7465 7274 6f6f 6c73 0a72 6573  rt itertools.res
+000287e0: 756c 7420 3d20 6974 6572 746f 6f6c 732e  ult = itertools.
+000287f0: 7a69 705f 6c6f 6e67 6573 7428 7261 6e67  zip_longest(rang
+00028800: 6528 3529 2c20 7261 6e67 6528 3130 2929  e(5), range(10))
+00028810: 0a60 6060 0a0a 2323 2323 2060 7461 6b65  .```..#### `take
+00028820: 7768 696c 6560 0a0a 2a2a 7461 6b65 7768  while`..**takewh
+00028830: 696c 652a 2a28 5f70 7265 6469 6361 7465  ile**(_predicate
+00028840: 5f2c 205f 6974 6572 6162 6c65 5f2c 202f  _, _iterable_, /
+00028850: 290a 0a43 6f63 6f6e 7574 2070 726f 7669  )..Coconut provi
+00028860: 6465 7320 6069 7465 7274 6f6f 6c73 2e74  des `itertools.t
+00028870: 616b 6577 6869 6c65 6020 6173 2061 2062  akewhile` as a b
+00028880: 7569 6c74 2d69 6e20 756e 6465 7220 7468  uilt-in under th
+00028890: 6520 6e61 6d65 2060 7461 6b65 7768 696c  e name `takewhil
+000288a0: 6560 2e0a 0a23 2323 2323 2050 7974 686f  e`...##### Pytho
+000288b0: 6e20 446f 6373 0a0a 2a2a 7461 6b65 7768  n Docs..**takewh
+000288c0: 696c 652a 2a28 5f70 7265 6469 6361 7465  ile**(_predicate
+000288d0: 2c20 6974 6572 6162 6c65 5f29 0a0a 4d61  , iterable_)..Ma
+000288e0: 6b65 2061 6e20 6974 6572 6174 6f72 2074  ke an iterator t
+000288f0: 6861 7420 7265 7475 726e 7320 656c 656d  hat returns elem
+00028900: 656e 7473 2066 726f 6d20 7468 6520 5f69  ents from the _i
+00028910: 7465 7261 626c 655f 2061 7320 6c6f 6e67  terable_ as long
+00028920: 2061 7320 7468 6520 5f70 7265 6469 6361   as the _predica
+00028930: 7465 5f20 6973 2074 7275 652e 2045 7175  te_ is true. Equ
+00028940: 6976 616c 656e 7420 746f 3a0a 6060 6063  ivalent to:.```c
+00028950: 6f63 6f6e 7574 5f70 7974 686f 6e0a 6465  oconut_python.de
+00028960: 6620 7461 6b65 7768 696c 6528 7072 6564  f takewhile(pred
+00028970: 6963 6174 652c 2069 7465 7261 626c 6529  icate, iterable)
+00028980: 3a0a 2020 2020 2320 7461 6b65 7768 696c  :.    # takewhil
+00028990: 6528 6c61 6d62 6461 2078 3a20 783c 352c  e(lambda x: x<5,
+000289a0: 205b 312c 342c 362c 342c 315d 2920 2d2d   [1,4,6,4,1]) --
+000289b0: 3e20 3120 340a 2020 2020 666f 7220 7820  > 1 4.    for x 
+000289c0: 696e 2069 7465 7261 626c 653a 0a20 2020  in iterable:.   
+000289d0: 2020 2020 2069 6620 7072 6564 6963 6174       if predicat
+000289e0: 6528 7829 3a0a 2020 2020 2020 2020 2020  e(x):.          
+000289f0: 2020 7969 656c 6420 780a 2020 2020 2020    yield x.      
+00028a00: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00028a10: 2020 2020 6272 6561 6b0a 6060 600a 0a23      break.```..#
+00028a20: 2323 2323 2045 7861 6d70 6c65 0a0a 2a2a  #### Example..**
+00028a30: 436f 636f 6e75 743a 2a2a 0a60 6060 636f  Coconut:**.```co
+00028a40: 636f 6e75 740a 6e65 6761 7469 7665 7320  conut.negatives 
+00028a50: 3d20 6e75 6d69 7465 7220 7c3e 2074 616b  = numiter |> tak
+00028a60: 6577 6869 6c65 2428 7820 2d3e 2078 203c  ewhile$(x -> x <
+00028a70: 2030 290a 6060 600a 0a2a 2a50 7974 686f   0).```..**Pytho
+00028a80: 6e3a 2a2a 0a60 6060 636f 636f 6e75 745f  n:**.```coconut_
+00028a90: 7079 7468 6f6e 0a69 6d70 6f72 7420 6974  python.import it
+00028aa0: 6572 746f 6f6c 730a 6e65 6761 7469 7665  ertools.negative
+00028ab0: 7320 3d20 6974 6572 746f 6f6c 732e 7461  s = itertools.ta
+00028ac0: 6b65 7768 696c 6528 6c61 6d62 6461 2078  kewhile(lambda x
+00028ad0: 3a20 7820 3c20 302c 206e 756d 6974 6572  : x < 0, numiter
+00028ae0: 290a 6060 600a 0a23 2323 2320 6064 726f  ).```..#### `dro
+00028af0: 7077 6869 6c65 600a 0a2a 2a64 726f 7077  pwhile`..**dropw
+00028b00: 6869 6c65 2a2a 285f 7072 6564 6963 6174  hile**(_predicat
+00028b10: 655f 2c20 5f69 7465 7261 626c 655f 2c20  e_, _iterable_, 
+00028b20: 2f29 0a0a 436f 636f 6e75 7420 7072 6f76  /)..Coconut prov
+00028b30: 6964 6573 2060 6974 6572 746f 6f6c 732e  ides `itertools.
+00028b40: 6472 6f70 7768 696c 6560 2061 7320 6120  dropwhile` as a 
+00028b50: 6275 696c 742d 696e 2075 6e64 6572 2074  built-in under t
+00028b60: 6865 206e 616d 6520 6064 726f 7077 6869  he name `dropwhi
+00028b70: 6c65 602e 0a0a 2323 2323 2320 5079 7468  le`...##### Pyth
+00028b80: 6f6e 2044 6f63 730a 0a2a 2a64 726f 7077  on Docs..**dropw
+00028b90: 6869 6c65 2a2a 285f 7072 6564 6963 6174  hile**(_predicat
+00028ba0: 652c 2069 7465 7261 626c 655f 290a 0a4d  e, iterable_)..M
+00028bb0: 616b 6520 616e 2069 7465 7261 746f 7220  ake an iterator 
+00028bc0: 7468 6174 2064 726f 7073 2065 6c65 6d65  that drops eleme
+00028bd0: 6e74 7320 6672 6f6d 2074 6865 205f 6974  nts from the _it
+00028be0: 6572 6162 6c65 5f20 6173 206c 6f6e 6720  erable_ as long 
+00028bf0: 6173 2074 6865 205f 7072 6564 6963 6174  as the _predicat
+00028c00: 655f 2069 7320 7472 7565 3b20 6166 7465  e_ is true; afte
+00028c10: 7277 6172 6473 2c20 7265 7475 726e 7320  rwards, returns 
+00028c20: 6576 6572 7920 656c 656d 656e 742e 204e  every element. N
+00028c30: 6f74 653a 2074 6865 2069 7465 7261 746f  ote: the iterato
+00028c40: 7220 646f 6573 206e 6f74 2070 726f 6475  r does not produ
+00028c50: 6365 2061 6e79 206f 7574 7075 7420 756e  ce any output un
+00028c60: 7469 6c20 7468 6520 7072 6564 6963 6174  til the predicat
+00028c70: 6520 6669 7273 7420 6265 636f 6d65 7320  e first becomes 
+00028c80: 6661 6c73 652c 2073 6f20 6974 206d 6179  false, so it may
+00028c90: 2068 6176 6520 6120 6c65 6e67 7468 7920   have a lengthy 
+00028ca0: 7374 6172 742d 7570 2074 696d 652e 2045  start-up time. E
+00028cb0: 7175 6976 616c 656e 7420 746f 3a0a 6060  quivalent to:.``
+00028cc0: 6063 6f63 6f6e 7574 5f70 7974 686f 6e0a  `coconut_python.
+00028cd0: 6465 6620 6472 6f70 7768 696c 6528 7072  def dropwhile(pr
+00028ce0: 6564 6963 6174 652c 2069 7465 7261 626c  edicate, iterabl
+00028cf0: 6529 3a0a 2020 2020 2320 6472 6f70 7768  e):.    # dropwh
+00028d00: 696c 6528 6c61 6d62 6461 2078 3a20 783c  ile(lambda x: x<
+00028d10: 352c 205b 312c 342c 362c 342c 315d 2920  5, [1,4,6,4,1]) 
+00028d20: 2d2d 3e20 3620 3420 310a 2020 2020 6974  --> 6 4 1.    it
+00028d30: 6572 6162 6c65 203d 2069 7465 7228 6974  erable = iter(it
+00028d40: 6572 6162 6c65 290a 2020 2020 666f 7220  erable).    for 
+00028d50: 7820 696e 2069 7465 7261 626c 653a 0a20  x in iterable:. 
+00028d60: 2020 2020 2020 2069 6620 6e6f 7420 7072         if not pr
+00028d70: 6564 6963 6174 6528 7829 3a0a 2020 2020  edicate(x):.    
+00028d80: 2020 2020 2020 2020 7969 656c 6420 780a          yield x.
+00028d90: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00028da0: 6b0a 2020 2020 666f 7220 7820 696e 2069  k.    for x in i
+00028db0: 7465 7261 626c 653a 0a20 2020 2020 2020  terable:.       
+00028dc0: 2079 6965 6c64 2078 0a60 6060 0a0a 2323   yield x.```..##
+00028dd0: 2323 2320 4578 616d 706c 650a 0a2a 2a43  ### Example..**C
+00028de0: 6f63 6f6e 7574 3a2a 2a0a 6060 6063 6f63  oconut:**.```coc
+00028df0: 6f6e 7574 0a70 6f73 6974 6976 6573 203d  onut.positives =
+00028e00: 206e 756d 6974 6572 207c 3e20 6472 6f70   numiter |> drop
+00028e10: 7768 696c 6524 2878 202d 3e20 7820 3c20  while$(x -> x < 
+00028e20: 3029 0a60 6060 0a0a 2a2a 5079 7468 6f6e  0).```..**Python
+00028e30: 3a2a 2a0a 6060 6063 6f63 6f6e 7574 5f70  :**.```coconut_p
+00028e40: 7974 686f 6e0a 696d 706f 7274 2069 7465  ython.import ite
+00028e50: 7274 6f6f 6c73 0a70 6f73 6974 6976 6573  rtools.positives
+00028e60: 203d 2069 7465 7274 6f6f 6c73 2e64 726f   = itertools.dro
+00028e70: 7077 6869 6c65 286c 616d 6264 6120 783a  pwhile(lambda x:
+00028e80: 2078 203c 2030 2c20 6e75 6d69 7465 7229   x < 0, numiter)
+00028e90: 0a60 6060 0a0a 2323 2323 2060 666c 6174  .```..#### `flat
+00028ea0: 7465 6e60 0a0a 2a2a 666c 6174 7465 6e2a  ten`..**flatten*
+00028eb0: 2a28 5f69 7465 7261 626c 655f 2c20 5f6c  *(_iterable_, _l
+00028ec0: 6576 656c 735f 3d60 3160 290a 0a43 6f63  evels_=`1`)..Coc
+00028ed0: 6f6e 7574 2070 726f 7669 6465 7320 616e  onut provides an
+00028ee0: 2065 6e68 616e 6365 6420 7665 7273 696f   enhanced versio
+00028ef0: 6e20 6f66 2060 6974 6572 746f 6f6c 732e  n of `itertools.
+00028f00: 6368 6169 6e2e 6672 6f6d 5f69 7465 7261  chain.from_itera
+00028f10: 626c 6560 2061 7320 6120 6275 696c 742d  ble` as a built-
+00028f20: 696e 2075 6e64 6572 2074 6865 206e 616d  in under the nam
+00028f30: 6520 6066 6c61 7474 656e 6020 7769 7468  e `flatten` with
+00028f40: 2061 6464 6564 2073 7570 706f 7274 2066   added support f
+00028f50: 6f72 2060 7265 7665 7273 6564 602c 2060  or `reversed`, `
+00028f60: 7265 7072 602c 2060 696e 602c 2060 2e63  repr`, `in`, `.c
+00028f70: 6f75 6e74 2829 602c 2060 2e69 6e64 6578  ount()`, `.index
+00028f80: 2829 602c 2061 6e64 2060 666d 6170 602e  ()`, and `fmap`.
+00028f90: 0a0a 4279 2064 6566 6175 6c74 2c20 6066  ..By default, `f
+00028fa0: 6c61 7474 656e 6020 6f6e 6c79 2066 6c61  latten` only fla
+00028fb0: 7474 656e 7320 7468 6520 746f 7020 6c65  ttens the top le
+00028fc0: 7665 6c20 6f66 2074 6865 2067 6976 656e  vel of the given
+00028fd0: 2069 7465 7261 626c 652f 6172 7261 792e   iterable/array.
+00028fe0: 2049 6620 5f6c 6576 656c 735f 2069 7320   If _levels_ is 
+00028ff0: 7061 7373 6564 2c20 686f 7765 7665 722c  passed, however,
+00029000: 2069 7420 6361 6e20 6265 2075 7365 6420   it can be used 
+00029010: 746f 2063 6f6e 7472 6f6c 2074 6865 206e  to control the n
+00029020: 756d 6265 7220 6f66 206c 6576 656c 7320  umber of levels 
+00029030: 666c 6174 7465 6e65 642c 2077 6974 6820  flattened, with 
+00029040: 6030 6020 6d65 616e 696e 6720 6e6f 2066  `0` meaning no f
+00029050: 6c61 7474 656e 696e 6720 616e 6420 604e  lattening and `N
+00029060: 6f6e 6560 2066 6c61 7474 656e 696e 6720  one` flattening 
+00029070: 6173 206d 616e 7920 6974 6572 6162 6c65  as many iterable
+00029080: 7320 6173 2061 7265 2066 6f75 6e64 2e20  s as are found. 
+00029090: 4e6f 7465 2074 6861 7420 6966 205f 6c65  Note that if _le
+000290a0: 7665 6c73 5f20 6973 2073 6574 2074 6f20  vels_ is set to 
+000290b0: 616e 7920 6e6f 6e2d 604e 6f6e 6560 2076  any non-`None` v
+000290c0: 616c 7565 2c20 7468 6520 6669 7273 7420  alue, the first 
+000290d0: 5f6c 6576 656c 735f 206c 6576 656c 7320  _levels_ levels 
+000290e0: 6d75 7374 2062 6520 6974 6572 6162 6c65  must be iterable
+000290f0: 732c 206f 7220 656c 7365 2061 6e20 6572  s, or else an er
+00029100: 726f 7220 7769 6c6c 2062 6520 7261 6973  ror will be rais
+00029110: 6564 2e0a 0a23 2323 2323 2050 7974 686f  ed...##### Pytho
+00029120: 6e20 446f 6373 0a0a 6368 6169 6e2e 2a2a  n Docs..chain.**
+00029130: 6672 6f6d 5f69 7465 7261 626c 652a 2a28  from_iterable**(
+00029140: 5f69 7465 7261 626c 655f 290a 0a41 6c74  _iterable_)..Alt
+00029150: 6572 6e61 7465 2063 6f6e 7374 7275 6374  ernate construct
+00029160: 6f72 2066 6f72 2060 6368 6169 6e28 2960  or for `chain()`
+00029170: 2e20 4765 7473 2063 6861 696e 6564 2069  . Gets chained i
+00029180: 6e70 7574 7320 6672 6f6d 2061 2073 696e  nputs from a sin
+00029190: 676c 6520 6974 6572 6162 6c65 2061 7267  gle iterable arg
+000291a0: 756d 656e 7420 7468 6174 2069 7320 6576  ument that is ev
+000291b0: 616c 7561 7465 6420 6c61 7a69 6c79 2e20  aluated lazily. 
+000291c0: 526f 7567 686c 7920 6571 7569 7661 6c65  Roughly equivale
+000291d0: 6e74 2074 6f3a 0a0a 6060 6063 6f63 6f6e  nt to:..```cocon
+000291e0: 7574 5f70 7974 686f 6e0a 6465 6620 666c  ut_python.def fl
+000291f0: 6174 7465 6e28 6974 6572 6162 6c65 7329  atten(iterables)
+00029200: 3a0a 2020 2020 2320 666c 6174 7465 6e28  :.    # flatten(
+00029210: 5b27 4142 4327 2c20 2744 4546 275d 2920  ['ABC', 'DEF']) 
+00029220: 2d2d 3e20 4120 4220 4320 4420 4520 460a  --> A B C D E F.
+00029230: 2020 2020 666f 7220 6974 2069 6e20 6974      for it in it
+00029240: 6572 6162 6c65 733a 0a20 2020 2020 2020  erables:.       
+00029250: 2066 6f72 2065 6c65 6d65 6e74 2069 6e20   for element in 
+00029260: 6974 3a0a 2020 2020 2020 2020 2020 2020  it:.            
+00029270: 7969 656c 6420 656c 656d 656e 740a 6060  yield element.``
+00029280: 600a 0a23 2323 2323 2045 7861 6d70 6c65  `..##### Example
+00029290: 0a0a 2a2a 436f 636f 6e75 743a 2a2a 0a60  ..**Coconut:**.`
+000292a0: 6060 636f 636f 6e75 740a 6974 6572 5f6f  ``coconut.iter_o
+000292b0: 665f 6974 6572 7320 3d20 5b5b 312c 2032  f_iters = [[1, 2
+000292c0: 5d2c 205b 332c 2034 5d5d 0a66 6c61 745f  ], [3, 4]].flat_
+000292d0: 6974 203d 2069 7465 725f 6f66 5f69 7465  it = iter_of_ite
+000292e0: 7273 207c 3e20 666c 6174 7465 6e20 7c3e  rs |> flatten |>
+000292f0: 206c 6973 740a 6060 600a 0a2a 2a50 7974   list.```..**Pyt
+00029300: 686f 6e3a 2a2a 0a60 6060 636f 636f 6e75  hon:**.```coconu
+00029310: 745f 7079 7468 6f6e 0a66 726f 6d20 6974  t_python.from it
+00029320: 6572 746f 6f6c 7320 696d 706f 7274 2063  ertools import c
+00029330: 6861 696e 0a69 7465 725f 6f66 5f69 7465  hain.iter_of_ite
+00029340: 7273 203d 205b 5b31 2c20 325d 2c20 5b33  rs = [[1, 2], [3
+00029350: 2c20 345d 5d0a 666c 6174 5f69 7420 3d20  , 4]].flat_it = 
+00029360: 6974 6572 5f6f 665f 6974 6572 7320 7c3e  iter_of_iters |>
+00029370: 2063 6861 696e 2e66 726f 6d5f 6974 6572   chain.from_iter
+00029380: 6162 6c65 207c 3e20 6c69 7374 0a60 6060  able |> list.```
+00029390: 0a0a 2323 2323 2060 7363 616e 600a 0a2a  ..#### `scan`..*
+000293a0: 2a73 6361 6e2a 2a28 5f66 756e 6374 696f  *scan**(_functio
+000293b0: 6e5f 2c20 5f69 7465 7261 626c 655f 5b2c  n_, _iterable_[,
+000293c0: 205f 696e 6974 6961 6c5f 5d29 0a0a 436f   _initial_])..Co
+000293d0: 636f 6e75 7420 7072 6f76 6964 6573 2061  conut provides a
+000293e0: 206d 6f64 6966 6965 6420 7665 7273 696f   modified versio
+000293f0: 6e20 6f66 2060 6974 6572 746f 6f6c 732e  n of `itertools.
+00029400: 6163 6375 6d75 6c61 7465 6020 7769 7468  accumulate` with
+00029410: 206f 7070 6f73 6974 6520 6172 6775 6d65   opposite argume
+00029420: 6e74 206f 7264 6572 2061 7320 6073 6361  nt order as `sca
+00029430: 6e60 2074 6861 7420 616c 736f 2073 7570  n` that also sup
+00029440: 706f 7274 7320 6072 6570 7260 2c20 606c  ports `repr`, `l
+00029450: 656e 602c 2061 6e64 2060 6675 6e63 602f  en`, and `func`/
+00029460: 6069 7465 7260 2f60 696e 6974 6961 6c60  `iter`/`initial`
+00029470: 2061 7474 7269 6275 7465 732e 2060 7363   attributes. `sc
+00029480: 616e 6020 776f 726b 7320 6578 6163 746c  an` works exactl
+00029490: 7920 6c69 6b65 205b 6072 6564 7563 6560  y like [`reduce`
+000294a0: 5d28 2372 6564 7563 6529 2c20 6578 6365  ](#reduce), exce
+000294b0: 7074 2074 6861 7420 696e 7374 6561 6420  pt that instead 
+000294c0: 6f66 206f 6e6c 7920 7265 7475 726e 696e  of only returnin
+000294d0: 6720 7468 6520 6c61 7374 2061 6363 756d  g the last accum
+000294e0: 756c 6174 6564 2076 616c 7565 2c20 6974  ulated value, it
+000294f0: 2072 6574 7572 6e73 2061 6e20 6974 6572   returns an iter
+00029500: 6174 6f72 206f 6620 616c 6c20 7468 6520  ator of all the 
+00029510: 696e 7465 726d 6564 6961 7465 2076 616c  intermediate val
+00029520: 7565 732e 0a0a 2323 2323 2320 5079 7468  ues...##### Pyth
+00029530: 6f6e 2044 6f63 730a 0a2a 2a73 6361 6e2a  on Docs..**scan*
+00029540: 2a28 5f66 756e 6374 696f 6e2c 2069 7465  *(_function, ite
+00029550: 7261 626c 655f 2a2a 5b2a 2a5f 2c20 696e  rable_**[**_, in
+00029560: 6974 6961 6c5f 2a2a 5d2a 2a29 0a0a 4d61  itial_**]**)..Ma
+00029570: 6b65 2061 6e20 6974 6572 6174 6f72 2074  ke an iterator t
+00029580: 6861 7420 7265 7475 726e 7320 6163 6375  hat returns accu
+00029590: 6d75 6c61 7465 6420 7265 7375 6c74 7320  mulated results 
+000295a0: 6f66 2073 6f6d 6520 6675 6e63 7469 6f6e  of some function
+000295b0: 206f 6620 7477 6f20 6172 6775 6d65 6e74   of two argument
+000295c0: 732e 2045 6c65 6d65 6e74 7320 6f66 2074  s. Elements of t
+000295d0: 6865 2069 6e70 7574 2069 7465 7261 626c  he input iterabl
+000295e0: 6520 6d61 7920 6265 2061 6e79 2074 7970  e may be any typ
+000295f0: 6520 7468 6174 2063 616e 2062 6520 6163  e that can be ac
+00029600: 6365 7074 6564 2061 7320 6172 6775 6d65  cepted as argume
+00029610: 6e74 7320 746f 205f 6675 6e63 7469 6f6e  nts to _function
+00029620: 5f2e 2028 466f 7220 6578 616d 706c 652c  _. (For example,
+00029630: 2077 6974 6820 7468 6520 6f70 6572 6174   with the operat
+00029640: 696f 6e20 6f66 2061 6464 6974 696f 6e2c  ion of addition,
+00029650: 2065 6c65 6d65 6e74 7320 6d61 7920 6265   elements may be
+00029660: 2061 6e79 2061 6464 6162 6c65 2074 7970   any addable typ
+00029670: 6520 696e 636c 7564 696e 6720 4465 6369  e including Deci
+00029680: 6d61 6c20 6f72 2046 7261 6374 696f 6e2e  mal or Fraction.
+00029690: 2920 4966 2074 6865 2069 6e70 7574 2069  ) If the input i
+000296a0: 7465 7261 626c 6520 6973 2065 6d70 7479  terable is empty
+000296b0: 2c20 7468 6520 6f75 7470 7574 2069 7465  , the output ite
+000296c0: 7261 626c 6520 7769 6c6c 2061 6c73 6f20  rable will also 
+000296d0: 6265 2065 6d70 7479 2e0a 0a49 6620 6e6f  be empty...If no
+000296e0: 205f 696e 6974 6961 6c5f 2069 7320 6769   _initial_ is gi
+000296f0: 7665 6e2c 2072 6f75 6768 6c79 2065 7175  ven, roughly equ
+00029700: 6976 616c 656e 7420 746f 3a0a 6060 6063  ivalent to:.```c
+00029710: 6f63 6f6e 7574 5f70 7974 686f 6e0a 6465  oconut_python.de
+00029720: 6620 7363 616e 2866 756e 6374 696f 6e2c  f scan(function,
+00029730: 2069 7465 7261 626c 6529 3a0a 2020 2020   iterable):.    
+00029740: 2752 6574 7572 6e20 7275 6e6e 696e 6720  'Return running 
+00029750: 746f 7461 6c73 270a 2020 2020 2320 7363  totals'.    # sc
+00029760: 616e 286f 7065 7261 746f 722e 6164 642c  an(operator.add,
+00029770: 205b 312c 322c 332c 342c 355d 2920 2d2d   [1,2,3,4,5]) --
+00029780: 3e20 3120 3320 3620 3130 2031 350a 2020  > 1 3 6 10 15.  
+00029790: 2020 2320 7363 616e 286f 7065 7261 746f    # scan(operato
+000297a0: 722e 6d75 6c2c 205b 312c 322c 332c 342c  r.mul, [1,2,3,4,
+000297b0: 355d 2920 2d2d 3e20 3120 3220 3620 3234  5]) --> 1 2 6 24
+000297c0: 2031 3230 0a20 2020 2069 7420 3d20 6974   120.    it = it
+000297d0: 6572 2869 7465 7261 626c 6529 0a20 2020  er(iterable).   
+000297e0: 2074 7279 3a0a 2020 2020 2020 2020 746f   try:.        to
+000297f0: 7461 6c20 3d20 6e65 7874 2869 7429 0a20  tal = next(it). 
+00029800: 2020 2065 7863 6570 7420 5374 6f70 4974     except StopIt
+00029810: 6572 6174 696f 6e3a 0a20 2020 2020 2020  eration:.       
+00029820: 2072 6574 7572 6e0a 2020 2020 7969 656c   return.    yiel
+00029830: 6420 746f 7461 6c0a 2020 2020 666f 7220  d total.    for 
+00029840: 656c 656d 656e 7420 696e 2069 743a 0a20  element in it:. 
+00029850: 2020 2020 2020 2074 6f74 616c 203d 2066         total = f
+00029860: 756e 6374 696f 6e28 746f 7461 6c2c 2065  unction(total, e
+00029870: 6c65 6d65 6e74 290a 2020 2020 2020 2020  lement).        
+00029880: 7969 656c 6420 746f 7461 6c0a 6060 600a  yield total.```.
+00029890: 0a23 2323 2323 2045 7861 6d70 6c65 0a0a  .##### Example..
+000298a0: 2a2a 436f 636f 6e75 743a 2a2a 0a60 6060  **Coconut:**.```
+000298b0: 636f 636f 6e75 740a 696e 7075 745f 6461  coconut.input_da
+000298c0: 7461 203d 205b 332c 2034 2c20 362c 2032  ta = [3, 4, 6, 2
+000298d0: 2c20 312c 2039 2c20 302c 2037 2c20 352c  , 1, 9, 0, 7, 5,
+000298e0: 2038 5d0a 7275 6e6e 696e 675f 6d61 7820   8].running_max 
+000298f0: 3d20 696e 7075 745f 6461 7461 207c 3e20  = input_data |> 
+00029900: 7363 616e 2428 6d61 7829 207c 3e20 6c69  scan$(max) |> li
+00029910: 7374 0a60 6060 0a0a 2a2a 5079 7468 6f6e  st.```..**Python
+00029920: 3a2a 2a0a 6060 6063 6f63 6f6e 7574 5f70  :**.```coconut_p
+00029930: 7974 686f 6e0a 696e 7075 745f 6461 7461  ython.input_data
+00029940: 203d 205b 332c 2034 2c20 362c 2032 2c20   = [3, 4, 6, 2, 
+00029950: 312c 2039 2c20 302c 2037 2c20 352c 2038  1, 9, 0, 7, 5, 8
+00029960: 5d0a 7275 6e6e 696e 675f 6d61 7820 3d20  ].running_max = 
+00029970: 5b5d 0a6d 6178 5f73 6f5f 6661 7220 3d20  [].max_so_far = 
+00029980: 696e 7075 745f 6461 7461 5b30 5d0a 666f  input_data[0].fo
+00029990: 7220 7820 696e 2069 6e70 7574 5f64 6174  r x in input_dat
+000299a0: 613a 0a20 2020 2069 6620 7820 3e20 6d61  a:.    if x > ma
+000299b0: 785f 736f 5f66 6172 3a0a 2020 2020 2020  x_so_far:.      
+000299c0: 2020 6d61 785f 736f 5f66 6172 203d 2078    max_so_far = x
+000299d0: 0a20 2020 2072 756e 6e69 6e67 5f6d 6178  .    running_max
+000299e0: 2e61 7070 656e 6428 7829 0a60 6060 0a0a  .append(x).```..
+000299f0: 2323 2323 2060 636f 756e 7460 0a0a 2a2a  #### `count`..**
+00029a00: 636f 756e 742a 2a28 5f73 7461 7274 5f3d  count**(_start_=
+00029a10: 6030 602c 205f 7374 6570 5f3d 6031 6029  `0`, _step_=`1`)
+00029a20: 0a0a 436f 636f 6e75 7420 7072 6f76 6964  ..Coconut provid
+00029a30: 6573 2061 206d 6f64 6966 6965 6420 7665  es a modified ve
+00029a40: 7273 696f 6e20 6f66 2060 6974 6572 746f  rsion of `iterto
+00029a50: 6f6c 732e 636f 756e 7460 2074 6861 7420  ols.count` that 
+00029a60: 7375 7070 6f72 7473 2060 696e 602c 206e  supports `in`, n
+00029a70: 6f72 6d61 6c20 736c 6963 696e 672c 206f  ormal slicing, o
+00029a80: 7074 696d 697a 6564 2069 7465 7261 746f  ptimized iterato
+00029a90: 7220 736c 6963 696e 672c 2074 6865 2073  r slicing, the s
+00029aa0: 7461 6e64 6172 6420 6063 6f75 6e74 6020  tandard `count` 
+00029ab0: 616e 6420 6069 6e64 6578 6020 7365 7175  and `index` sequ
+00029ac0: 656e 6365 206d 6574 686f 6473 2c20 6072  ence methods, `r
+00029ad0: 6570 7260 2c20 616e 6420 6073 7461 7274  epr`, and `start
+00029ae0: 602f 6073 7465 7060 2061 7474 7269 6275  `/`step` attribu
+00029af0: 7465 7320 6173 2061 2062 7569 6c74 2d69  tes as a built-i
+00029b00: 6e20 756e 6465 7220 7468 6520 6e61 6d65  n under the name
+00029b10: 2060 636f 756e 7460 2e0a 0a41 6464 6974   `count`...Addit
+00029b20: 696f 6e61 6c6c 792c 2069 6620 7468 6520  ionally, if the 
+00029b30: 5f73 7465 705f 2070 6172 616d 6574 6572  _step_ parameter
+00029b40: 2069 7320 7365 7420 746f 2060 4e6f 6e65   is set to `None
+00029b50: 602c 2060 636f 756e 7460 2077 696c 6c20  `, `count` will 
+00029b60: 6265 6861 7665 206c 696b 6520 6069 7465  behave like `ite
+00029b70: 7274 6f6f 6c73 2e72 6570 6561 7460 2069  rtools.repeat` i
+00029b80: 6e73 7465 6164 2e0a 0a23 2323 2323 2050  nstead...##### P
+00029b90: 7974 686f 6e20 446f 6373 0a0a 2a2a 636f  ython Docs..**co
+00029ba0: 756e 742a 2a28 5f73 7461 7274 3d30 2c20  unt**(_start=0, 
+00029bb0: 7374 6570 3d31 5f29 0a0a 4d61 6b65 2061  step=1_)..Make a
+00029bc0: 6e20 6974 6572 6174 6f72 2074 6861 7420  n iterator that 
+00029bd0: 7265 7475 726e 7320 6576 656e 6c79 2073  returns evenly s
+00029be0: 7061 6365 6420 7661 6c75 6573 2073 7461  paced values sta
+00029bf0: 7274 696e 6720 7769 7468 206e 756d 6265  rting with numbe
+00029c00: 7220 5f73 7461 7274 5f2e 204f 6674 656e  r _start_. Often
+00029c10: 2075 7365 6420 6173 2061 6e20 6172 6775   used as an argu
+00029c20: 6d65 6e74 2074 6f20 606d 6170 2829 6020  ment to `map()` 
+00029c30: 746f 2067 656e 6572 6174 6520 636f 6e73  to generate cons
+00029c40: 6563 7574 6976 6520 6461 7461 2070 6f69  ecutive data poi
+00029c50: 6e74 732e 2041 6c73 6f2c 2075 7365 6420  nts. Also, used 
+00029c60: 7769 7468 2060 7a69 7028 2960 2074 6f20  with `zip()` to 
+00029c70: 6164 6420 7365 7175 656e 6365 206e 756d  add sequence num
+00029c80: 6265 7273 2e20 526f 7567 686c 7920 6571  bers. Roughly eq
+00029c90: 7569 7661 6c65 6e74 2074 6f3a 0a60 6060  uivalent to:.```
+00029ca0: 636f 636f 6e75 745f 7079 7468 6f6e 0a64  coconut_python.d
+00029cb0: 6566 2063 6f75 6e74 2873 7461 7274 3d30  ef count(start=0
+00029cc0: 2c20 7374 6570 3d31 293a 0a20 2020 2023  , step=1):.    #
+00029cd0: 2063 6f75 6e74 2831 3029 202d 2d3e 2031   count(10) --> 1
+00029ce0: 3020 3131 2031 3220 3133 2031 3420 2e2e  0 11 12 13 14 ..
+00029cf0: 2e0a 2020 2020 2320 636f 756e 7428 322e  ..    # count(2.
+00029d00: 352c 2030 2e35 2920 2d3e 2032 2e35 2033  5, 0.5) -> 2.5 3
+00029d10: 2e30 2033 2e35 202e 2e2e 0a20 2020 206e  .0 3.5 ....    n
+00029d20: 203d 2073 7461 7274 0a20 2020 2077 6869   = start.    whi
+00029d30: 6c65 2054 7275 653a 0a20 2020 2020 2020  le True:.       
+00029d40: 2079 6965 6c64 206e 0a20 2020 2020 2020   yield n.       
+00029d50: 2069 6620 7374 6570 3a0a 2020 2020 2020   if step:.      
+00029d60: 2020 2020 6e20 2b3d 2073 7465 700a 6060      n += step.``
+00029d70: 600a 0a23 2323 2323 2045 7861 6d70 6c65  `..##### Example
+00029d80: 0a0a 2a2a 436f 636f 6e75 743a 2a2a 0a60  ..**Coconut:**.`
+00029d90: 6060 636f 636f 6e75 740a 636f 756e 7428  ``coconut.count(
+00029da0: 2924 5b31 302a 2a31 3030 5d20 7c3e 2070  )$[10**100] |> p
+00029db0: 7269 6e74 0a60 6060 0a0a 2a2a 5079 7468  rint.```..**Pyth
+00029dc0: 6f6e 3a2a 2a0a 5f43 616e 2774 2062 6520  on:**._Can't be 
+00029dd0: 646f 6e65 2071 7569 636b 6c79 2077 6974  done quickly wit
+00029de0: 686f 7574 2043 6f63 6f6e 7574 2773 2069  hout Coconut's i
+00029df0: 7465 7261 746f 7220 736c 6963 696e 672c  terator slicing,
+00029e00: 2077 6869 6368 2072 6571 7569 7265 7320   which requires 
+00029e10: 6d61 6e79 2063 6f6d 706c 6963 6174 6564  many complicated
+00029e20: 2070 6965 6365 732e 2054 6865 206e 6563   pieces. The nec
+00029e30: 6573 7361 7279 2064 6566 696e 6974 696f  essary definitio
+00029e40: 6e73 2069 6e20 5079 7468 6f6e 2063 616e  ns in Python can
+00029e50: 2062 6520 666f 756e 6420 696e 2074 6865   be found in the
+00029e60: 2043 6f63 6f6e 7574 2068 6561 6465 722e   Coconut header.
+00029e70: 5f0a 0a23 2323 2320 6063 7963 6c65 600a  _..#### `cycle`.
+00029e80: 0a2a 2a63 7963 6c65 2a2a 285f 6974 6572  .**cycle**(_iter
+00029e90: 6162 6c65 5f2c 205f 7469 6d65 735f 3d60  able_, _times_=`
+00029ea0: 4e6f 6e65 6029 0a0a 436f 636f 6e75 7427  None`)..Coconut'
+00029eb0: 7320 6063 7963 6c65 6020 6973 2061 206d  s `cycle` is a m
+00029ec0: 6f64 6966 6965 6420 7665 7273 696f 6e20  odified version 
+00029ed0: 6f66 2060 6974 6572 746f 6f6c 732e 6379  of `itertools.cy
+00029ee0: 636c 6560 2077 6974 6820 6120 6074 696d  cle` with a `tim
+00029ef0: 6573 6020 7061 7261 6d65 7465 7220 7468  es` parameter th
+00029f00: 6174 2063 6f6e 7472 6f6c 7320 7468 6520  at controls the 
+00029f10: 6e75 6d62 6572 206f 6620 7469 6d65 7320  number of times 
+00029f20: 746f 2063 7963 6c65 2074 6872 6f75 6768  to cycle through
+00029f30: 205f 6974 6572 6162 6c65 5f20 6265 666f   _iterable_ befo
+00029f40: 7265 2073 746f 7070 696e 672e 2060 6379  re stopping. `cy
+00029f50: 636c 6560 2061 6c73 6f20 7375 7070 6f72  cle` also suppor
+00029f60: 7473 2060 696e 602c 2073 6c69 6369 6e67  ts `in`, slicing
+00029f70: 2c20 606c 656e 602c 2060 7265 7665 7273  , `len`, `revers
+00029f80: 6564 602c 2060 2e63 6f75 6e74 2829 602c  ed`, `.count()`,
+00029f90: 2060 2e69 6e64 6578 2829 602c 2061 6e64   `.index()`, and
+00029fa0: 2060 7265 7072 602e 0a0a 2323 2323 2320   `repr`...##### 
+00029fb0: 5079 7468 6f6e 2044 6f63 730a 0a2a 2a63  Python Docs..**c
+00029fc0: 7963 6c65 2a2a 285f 6974 6572 6162 6c65  ycle**(_iterable
+00029fd0: 5f29 0a0a 4d61 6b65 2061 6e20 6974 6572  _)..Make an iter
+00029fe0: 6174 6f72 2072 6574 7572 6e69 6e67 2065  ator returning e
+00029ff0: 6c65 6d65 6e74 7320 6672 6f6d 2074 6865  lements from the
+0002a000: 2069 7465 7261 626c 6520 616e 6420 7361   iterable and sa
+0002a010: 7669 6e67 2061 2063 6f70 7920 6f66 2065  ving a copy of e
+0002a020: 6163 682e 2057 6865 6e20 7468 6520 6974  ach. When the it
+0002a030: 6572 6162 6c65 2069 7320 6578 6861 7573  erable is exhaus
+0002a040: 7465 642c 2072 6574 7572 6e20 656c 656d  ted, return elem
+0002a050: 656e 7473 2066 726f 6d20 7468 6520 7361  ents from the sa
+0002a060: 7665 6420 636f 7079 2e20 5265 7065 6174  ved copy. Repeat
+0002a070: 7320 696e 6465 6669 6e69 7465 6c79 2e20  s indefinitely. 
+0002a080: 526f 7567 686c 7920 6571 7569 7661 6c65  Roughly equivale
+0002a090: 6e74 2074 6f3a 0a0a 6060 6063 6f63 6f6e  nt to:..```cocon
+0002a0a0: 7574 5f70 7974 686f 6e0a 6465 6620 6379  ut_python.def cy
+0002a0b0: 636c 6528 6974 6572 6162 6c65 293a 0a20  cle(iterable):. 
+0002a0c0: 2020 2023 2063 7963 6c65 2827 4142 4344     # cycle('ABCD
+0002a0d0: 2729 202d 2d3e 2041 2042 2043 2044 2041  ') --> A B C D A
+0002a0e0: 2042 2043 2044 2041 2042 2043 2044 202e   B C D A B C D .
+0002a0f0: 2e2e 0a20 2020 2073 6176 6564 203d 205b  ...    saved = [
+0002a100: 5d0a 2020 2020 666f 7220 656c 656d 656e  ].    for elemen
+0002a110: 7420 696e 2069 7465 7261 626c 653a 0a20  t in iterable:. 
+0002a120: 2020 2020 2020 2079 6965 6c64 2065 6c65         yield ele
+0002a130: 6d65 6e74 0a20 2020 2020 2020 2073 6176  ment.        sav
+0002a140: 6564 2e61 7070 656e 6428 656c 656d 656e  ed.append(elemen
+0002a150: 7429 0a20 2020 2077 6869 6c65 2073 6176  t).    while sav
+0002a160: 6564 3a0a 2020 2020 2020 2020 666f 7220  ed:.        for 
+0002a170: 656c 656d 656e 7420 696e 2073 6176 6564  element in saved
+0002a180: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002a190: 7969 656c 6420 656c 656d 656e 740a 6060  yield element.``
+0002a1a0: 600a 0a4e 6f74 652c 2074 6869 7320 6d65  `..Note, this me
+0002a1b0: 6d62 6572 206f 6620 7468 6520 746f 6f6c  mber of the tool
+0002a1c0: 6b69 7420 6d61 7920 7265 7175 6972 6520  kit may require 
+0002a1d0: 7369 676e 6966 6963 616e 7420 6175 7869  significant auxi
+0002a1e0: 6c69 6172 7920 7374 6f72 6167 6520 2864  liary storage (d
+0002a1f0: 6570 656e 6469 6e67 206f 6e20 7468 6520  epending on the 
+0002a200: 6c65 6e67 7468 206f 6620 7468 6520 6974  length of the it
+0002a210: 6572 6162 6c65 292e 0a0a 2323 2323 2320  erable)...##### 
+0002a220: 4578 616d 706c 650a 0a2a 2a43 6f63 6f6e  Example..**Cocon
+0002a230: 7574 3a2a 2a0a 6060 6063 6f63 6f6e 7574  ut:**.```coconut
+0002a240: 0a63 7963 6c65 2872 616e 6765 2832 292c  .cycle(range(2),
+0002a250: 2032 2920 7c3e 206c 6973 7420 7c3e 2070   2) |> list |> p
+0002a260: 7269 6e74 0a60 6060 0a0a 2a2a 5079 7468  rint.```..**Pyth
+0002a270: 6f6e 3a2a 2a0a 6060 6063 6f63 6f6e 7574  on:**.```coconut
+0002a280: 5f70 7974 686f 6e0a 6672 6f6d 2069 7465  _python.from ite
+0002a290: 7274 6f6f 6c73 2069 6d70 6f72 7420 6379  rtools import cy
+0002a2a0: 636c 652c 2069 736c 6963 650a 7072 696e  cle, islice.prin
+0002a2b0: 7428 6c69 7374 2869 736c 6963 6528 6379  t(list(islice(cy
+0002a2c0: 636c 6528 7261 6e67 6528 3229 292c 2034  cle(range(2)), 4
+0002a2d0: 2929 290a 6060 600a 0a23 2323 2320 6063  ))).```..#### `c
+0002a2e0: 6172 7465 7369 616e 5f70 726f 6475 6374  artesian_product
+0002a2f0: 600a 0a2a 2a63 6172 7465 7369 616e 5c5f  `..**cartesian\_
+0002a300: 7072 6f64 7563 742a 2a28 2a5f 6974 6572  product**(*_iter
+0002a310: 6162 6c65 735f 2c20 5f72 6570 6561 745f  ables_, _repeat_
+0002a320: 3d60 3160 290a 0a43 6f63 6f6e 7574 2070  =`1`)..Coconut p
+0002a330: 726f 7669 6465 7320 616e 2065 6e68 616e  rovides an enhan
+0002a340: 6365 6420 7665 7273 696f 6e20 6f66 2060  ced version of `
+0002a350: 6974 6572 746f 6f6c 732e 7072 6f64 7563  itertools.produc
+0002a360: 7460 2061 7320 6120 6275 696c 742d 696e  t` as a built-in
+0002a370: 2075 6e64 6572 2074 6865 206e 616d 6520   under the name 
+0002a380: 6063 6172 7465 7369 616e 5f70 726f 6475  `cartesian_produ
+0002a390: 6374 6020 7769 7468 2061 6464 6564 2073  ct` with added s
+0002a3a0: 7570 706f 7274 2066 6f72 2060 6c65 6e60  upport for `len`
+0002a3b0: 2c20 6072 6570 7260 2c20 6069 6e60 2c20  , `repr`, `in`, 
+0002a3c0: 602e 636f 756e 7428 2960 2c20 616e 6420  `.count()`, and 
+0002a3d0: 6066 6d61 7060 2e0a 0a41 6464 6974 696f  `fmap`...Additio
+0002a3e0: 6e61 6c6c 792c 2060 6361 7274 6573 6961  nally, `cartesia
+0002a3f0: 6e5f 7072 6f64 7563 7460 2069 6e63 6c75  n_product` inclu
+0002a400: 6465 7320 7370 6563 6961 6c20 7375 7070  des special supp
+0002a410: 6f72 7420 666f 7220 5b60 6e75 6d70 7960  ort for [`numpy`
+0002a420: 5d28 236e 756d 7079 2d69 6e74 6567 7261  ](#numpy-integra
+0002a430: 7469 6f6e 2920 6f62 6a65 6374 732c 2069  tion) objects, i
+0002a440: 6e20 7768 6963 6820 6361 7365 2061 206d  n which case a m
+0002a450: 756c 7469 6469 6d65 6e73 696f 6e61 6c20  ultidimensional 
+0002a460: 6172 7261 7920 6973 2072 6574 7572 6e65  array is returne
+0002a470: 6420 696e 7374 6561 6420 6f66 2061 6e20  d instead of an 
+0002a480: 6974 6572 6174 6f72 2e0a 0a23 2323 2323  iterator...#####
+0002a490: 2050 7974 686f 6e20 446f 6373 0a0a 2a2a   Python Docs..**
+0002a4a0: 6361 7274 6573 6961 6e5c 5f70 726f 6475  cartesian\_produ
+0002a4b0: 6374 2a2a 285f 5c2a 6974 6572 6162 6c65  ct**(_\*iterable
+0002a4c0: 732c 2072 6570 6561 743d 315f 290a 0a43  s, repeat=1_)..C
+0002a4d0: 6172 7465 7369 616e 2070 726f 6475 6374  artesian product
+0002a4e0: 206f 6620 696e 7075 7420 6974 6572 6162   of input iterab
+0002a4f0: 6c65 732e 0a0a 526f 7567 686c 7920 6571  les...Roughly eq
+0002a500: 7569 7661 6c65 6e74 2074 6f20 6e65 7374  uivalent to nest
+0002a510: 6564 2066 6f72 2d6c 6f6f 7073 2069 6e20  ed for-loops in 
+0002a520: 6120 6765 6e65 7261 746f 7220 6578 7072  a generator expr
+0002a530: 6573 7369 6f6e 2e20 466f 7220 6578 616d  ession. For exam
+0002a540: 706c 652c 2060 6361 7274 6573 6961 6e5f  ple, `cartesian_
+0002a550: 7072 6f64 7563 7428 412c 2042 2960 2072  product(A, B)` r
+0002a560: 6574 7572 6e73 2074 6865 2073 616d 6520  eturns the same 
+0002a570: 6173 2060 2828 782c 7929 2066 6f72 2078  as `((x,y) for x
+0002a580: 2069 6e20 4120 666f 7220 7920 696e 2042   in A for y in B
+0002a590: 2960 2e0a 0a54 6865 206e 6573 7465 6420  )`...The nested 
+0002a5a0: 6c6f 6f70 7320 6379 636c 6520 6c69 6b65  loops cycle like
+0002a5b0: 2061 6e20 6f64 6f6d 6574 6572 2077 6974   an odometer wit
+0002a5c0: 6820 7468 6520 7269 6768 746d 6f73 7420  h the rightmost 
+0002a5d0: 656c 656d 656e 7420 6164 7661 6e63 696e  element advancin
+0002a5e0: 6720 6f6e 2065 7665 7279 2069 7465 7261  g on every itera
+0002a5f0: 7469 6f6e 2e20 5468 6973 2070 6174 7465  tion. This patte
+0002a600: 726e 2063 7265 6174 6573 2061 206c 6578  rn creates a lex
+0002a610: 6963 6f67 7261 7068 6963 206f 7264 6572  icographic order
+0002a620: 696e 6720 736f 2074 6861 7420 6966 2074  ing so that if t
+0002a630: 6865 2069 6e70 7574 e280 9973 2069 7465  he input...s ite
+0002a640: 7261 626c 6573 2061 7265 2073 6f72 7465  rables are sorte
+0002a650: 642c 2074 6865 2070 726f 6475 6374 2074  d, the product t
+0002a660: 7570 6c65 7320 6172 6520 656d 6974 7465  uples are emitte
+0002a670: 6420 696e 2073 6f72 7465 6420 6f72 6465  d in sorted orde
+0002a680: 722e 0a0a 546f 2063 6f6d 7075 7465 2074  r...To compute t
+0002a690: 6865 2070 726f 6475 6374 206f 6620 616e  he product of an
+0002a6a0: 2069 7465 7261 626c 6520 7769 7468 2069   iterable with i
+0002a6b0: 7473 656c 662c 2073 7065 6369 6679 2074  tself, specify t
+0002a6c0: 6865 206e 756d 6265 7220 6f66 2072 6570  he number of rep
+0002a6d0: 6574 6974 696f 6e73 2077 6974 6820 7468  etitions with th
+0002a6e0: 6520 6f70 7469 6f6e 616c 2072 6570 6561  e optional repea
+0002a6f0: 7420 6b65 7977 6f72 6420 6172 6775 6d65  t keyword argume
+0002a700: 6e74 2e20 466f 7220 6578 616d 706c 652c  nt. For example,
+0002a710: 2060 7072 6f64 7563 7428 412c 2072 6570   `product(A, rep
+0002a720: 6561 743d 3429 6020 6d65 616e 7320 7468  eat=4)` means th
+0002a730: 6520 7361 6d65 2061 7320 6063 6172 7465  e same as `carte
+0002a740: 7369 616e 5f70 726f 6475 6374 2841 2c20  sian_product(A, 
+0002a750: 412c 2041 2c20 4129 602e 0a0a 5468 6973  A, A, A)`...This
+0002a760: 2066 756e 6374 696f 6e20 6973 2072 6f75   function is rou
+0002a770: 6768 6c79 2065 7175 6976 616c 656e 7420  ghly equivalent 
+0002a780: 746f 2074 6865 2066 6f6c 6c6f 7769 6e67  to the following
+0002a790: 2063 6f64 652c 2065 7863 6570 7420 7468   code, except th
+0002a7a0: 6174 2074 6865 2061 6374 7561 6c20 696d  at the actual im
+0002a7b0: 706c 656d 656e 7461 7469 6f6e 2064 6f65  plementation doe
+0002a7c0: 7320 6e6f 7420 6275 696c 6420 7570 2069  s not build up i
+0002a7d0: 6e74 6572 6d65 6469 6174 6520 7265 7375  ntermediate resu
+0002a7e0: 6c74 7320 696e 206d 656d 6f72 793a 0a0a  lts in memory:..
+0002a7f0: 6060 6063 6f63 6f6e 7574 5f70 7974 686f  ```coconut_pytho
+0002a800: 6e0a 6465 6620 6361 7274 6573 6961 6e5f  n.def cartesian_
+0002a810: 7072 6f64 7563 7428 2a61 7267 732c 2072  product(*args, r
+0002a820: 6570 6561 743d 3129 3a0a 2020 2020 2320  epeat=1):.    # 
+0002a830: 7072 6f64 7563 7428 2741 4243 4427 2c20  product('ABCD', 
+0002a840: 2778 7927 2920 2d2d 3e20 4178 2041 7920  'xy') --> Ax Ay 
+0002a850: 4278 2042 7920 4378 2043 7920 4478 2044  Bx By Cx Cy Dx D
+0002a860: 790a 2020 2020 2320 7072 6f64 7563 7428  y.    # product(
+0002a870: 7261 6e67 6528 3229 2c20 7265 7065 6174  range(2), repeat
+0002a880: 3d33 2920 2d2d 3e20 3030 3020 3030 3120  =3) --> 000 001 
+0002a890: 3031 3020 3031 3120 3130 3020 3130 3120  010 011 100 101 
+0002a8a0: 3131 3020 3131 310a 2020 2020 706f 6f6c  110 111.    pool
+0002a8b0: 7320 3d20 5b74 7570 6c65 2870 6f6f 6c29  s = [tuple(pool)
+0002a8c0: 2066 6f72 2070 6f6f 6c20 696e 2061 7267   for pool in arg
+0002a8d0: 735d 202a 2072 6570 6561 740a 2020 2020  s] * repeat.    
+0002a8e0: 7265 7375 6c74 203d 205b 5b5d 5d0a 2020  result = [[]].  
+0002a8f0: 2020 666f 7220 706f 6f6c 2069 6e20 706f    for pool in po
+0002a900: 6f6c 733a 0a20 2020 2020 2020 2072 6573  ols:.        res
+0002a910: 756c 7420 3d20 5b78 2b5b 795d 2066 6f72  ult = [x+[y] for
+0002a920: 2078 2069 6e20 7265 7375 6c74 2066 6f72   x in result for
+0002a930: 2079 2069 6e20 706f 6f6c 5d0a 2020 2020   y in pool].    
+0002a940: 666f 7220 7072 6f64 2069 6e20 7265 7375  for prod in resu
+0002a950: 6c74 3a0a 2020 2020 2020 2020 7969 656c  lt:.        yiel
+0002a960: 6420 7475 706c 6528 7072 6f64 290a 6060  d tuple(prod).``
+0002a970: 600a 0a42 6566 6f72 6520 6063 6172 7465  `..Before `carte
+0002a980: 7369 616e 5f70 726f 6475 6374 2829 6020  sian_product()` 
+0002a990: 7275 6e73 2c20 6974 2063 6f6d 706c 6574  runs, it complet
+0002a9a0: 656c 7920 636f 6e73 756d 6573 2074 6865  ely consumes the
+0002a9b0: 2069 6e70 7574 2069 7465 7261 626c 6573   input iterables
+0002a9c0: 2c20 6b65 6570 696e 6720 706f 6f6c 7320  , keeping pools 
+0002a9d0: 6f66 2076 616c 7565 7320 696e 206d 656d  of values in mem
+0002a9e0: 6f72 7920 746f 2067 656e 6572 6174 6520  ory to generate 
+0002a9f0: 7468 6520 7072 6f64 7563 7473 2e20 4163  the products. Ac
+0002aa00: 636f 7264 696e 676c 792c 2069 7420 6973  cordingly, it is
+0002aa10: 206f 6e6c 7920 7573 6566 756c 2077 6974   only useful wit
+0002aa20: 6820 6669 6e69 7465 2069 6e70 7574 732e  h finite inputs.
+0002aa30: 0a0a 2323 2323 2320 4578 616d 706c 650a  ..##### Example.
+0002aa40: 0a2a 2a43 6f63 6f6e 7574 3a2a 2a0a 6060  .**Coconut:**.``
+0002aa50: 6063 6f63 6f6e 7574 0a76 203d 205b 312c  `coconut.v = [1,
+0002aa60: 2032 5d0a 6173 7365 7274 2063 6172 7465   2].assert carte
+0002aa70: 7369 616e 5f70 726f 6475 6374 2876 2c20  sian_product(v, 
+0002aa80: 7629 207c 3e20 6c69 7374 203d 3d20 5b28  v) |> list == [(
+0002aa90: 312c 2031 292c 2028 312c 2032 292c 2028  1, 1), (1, 2), (
+0002aaa0: 322c 2031 292c 2028 322c 2032 295d 0a60  2, 1), (2, 2)].`
+0002aab0: 6060 0a0a 2a2a 5079 7468 6f6e 3a2a 2a0a  ``..**Python:**.
+0002aac0: 6060 6063 6f63 6f6e 7574 5f70 7974 686f  ```coconut_pytho
+0002aad0: 6e0a 6672 6f6d 2069 7465 7274 6f6f 6c73  n.from itertools
+0002aae0: 2069 6d70 6f72 7420 7072 6f64 7563 740a   import product.
+0002aaf0: 7620 3d20 5b31 2c20 325d 0a61 7373 6572  v = [1, 2].asser
+0002ab00: 7420 6c69 7374 2870 726f 6475 6374 2876  t list(product(v
+0002ab10: 2c20 7629 2920 3d3d 205b 2831 2c20 3129  , v)) == [(1, 1)
+0002ab20: 2c20 2831 2c20 3229 2c20 2832 2c20 3129  , (1, 2), (2, 1)
+0002ab30: 2c20 2832 2c20 3229 5d0a 6060 600a 0a23  , (2, 2)].```..#
+0002ab40: 2323 2320 606d 756c 7469 5f65 6e75 6d65  ### `multi_enume
+0002ab50: 7261 7465 600a 0a2a 2a6d 756c 7469 5c5f  rate`..**multi\_
+0002ab60: 656e 756d 6572 6174 652a 2a28 5f69 7465  enumerate**(_ite
+0002ab70: 7261 626c 655f 290a 0a43 6f63 6f6e 7574  rable_)..Coconut
+0002ab80: 2773 2060 6d75 6c74 695f 656e 756d 6572  's `multi_enumer
+0002ab90: 6174 6560 2065 6e75 6d65 7261 7465 7320  ate` enumerates 
+0002aba0: 7468 726f 7567 6820 616e 2069 7465 7261  through an itera
+0002abb0: 626c 6520 6f66 2069 7465 7261 626c 6573  ble of iterables
+0002abc0: 2e20 606d 756c 7469 5f65 6e75 6d65 7261  . `multi_enumera
+0002abd0: 7465 6020 776f 726b 7320 6c69 6b65 2065  te` works like e
+0002abe0: 6e75 6d65 7261 7465 2c20 6275 7420 696e  numerate, but in
+0002abf0: 6465 7865 7320 7468 726f 7567 6820 696e  dexes through in
+0002ac00: 6e65 7220 6974 6572 6162 6c65 7320 616e  ner iterables an
+0002ac10: 6420 7072 6f64 7563 6573 2061 2074 7570  d produces a tup
+0002ac20: 6c65 2069 6e64 6578 2072 6570 7265 7365  le index represe
+0002ac30: 6e74 696e 6720 7468 6520 696e 6465 7820  nting the index 
+0002ac40: 696e 2065 6163 6820 696e 6e65 7220 6974  in each inner it
+0002ac50: 6572 6162 6c65 2e20 5375 7070 6f72 7473  erable. Supports
+0002ac60: 2069 6e64 6578 696e 672e 0a0a 466f 7220   indexing...For 
+0002ac70: 5b60 6e75 6d70 7960 5d28 236e 756d 7079  [`numpy`](#numpy
+0002ac80: 2d69 6e74 6567 7261 7469 6f6e 2920 6f62  -integration) ob
+0002ac90: 6a65 6374 732c 2075 7365 7320 5b60 6e70  jects, uses [`np
+0002aca0: 2e6e 6469 7465 7260 5d28 6874 7470 733a  .nditer`](https:
+0002acb0: 2f2f 6e75 6d70 792e 6f72 672f 646f 632f  //numpy.org/doc/
+0002acc0: 7374 6162 6c65 2f72 6566 6572 656e 6365  stable/reference
+0002acd0: 2f67 656e 6572 6174 6564 2f6e 756d 7079  /generated/numpy
+0002ace0: 2e6e 6469 7465 722e 6874 6d6c 2920 756e  .nditer.html) un
+0002acf0: 6465 7220 7468 6520 686f 6f64 2e20 416c  der the hood. Al
+0002ad00: 736f 2073 7570 706f 7274 7320 606c 656e  so supports `len
+0002ad10: 6020 666f 7220 5b60 6e75 6d70 7960 5d28  ` for [`numpy`](
+0002ad20: 236e 756d 7079 2d69 6e74 6567 7261 7469  #numpy-integrati
+0002ad30: 6f6e 2920 6172 7261 7973 2e0a 0a23 2323  on) arrays...###
+0002ad40: 2323 2045 7861 6d70 6c65 0a0a 2a2a 436f  ## Example..**Co
+0002ad50: 636f 6e75 743a 2a2a 0a60 6060 636f 636f  conut:**.```coco
+0002ad60: 6e75 745f 7079 636f 6e0a 3e3e 3e20 5b31  nut_pycon.>>> [1
+0002ad70: 2c20 323b 3b20 332c 2034 5d20 7c3e 206d  , 2;; 3, 4] |> m
+0002ad80: 756c 7469 5f65 6e75 6d65 7261 7465 207c  ulti_enumerate |
+0002ad90: 3e20 6c69 7374 0a5b 2828 302c 2030 292c  > list.[((0, 0),
+0002ada0: 2031 292c 2028 2830 2c20 3129 2c20 3229   1), ((0, 1), 2)
+0002adb0: 2c20 2828 312c 2030 292c 2033 292c 2028  , ((1, 0), 3), (
+0002adc0: 2831 2c20 3129 2c20 3429 5d0a 6060 600a  (1, 1), 4)].```.
+0002add0: 0a2a 2a50 7974 686f 6e3a 2a2a 0a60 6060  .**Python:**.```
+0002ade0: 636f 636f 6e75 745f 7079 7468 6f6e 0a61  coconut_python.a
+0002adf0: 7272 6179 203d 205b 5b31 2c20 325d 2c20  rray = [[1, 2], 
+0002ae00: 5b33 2c20 345d 5d0a 656e 756d 6572 6174  [3, 4]].enumerat
+0002ae10: 6564 5f61 7272 6179 203d 205b 5d0a 666f  ed_array = [].fo
+0002ae20: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
+0002ae30: 2861 7272 6179 2929 3a0a 2020 2020 666f  (array)):.    fo
+0002ae40: 7220 6a20 696e 2072 616e 6765 286c 656e  r j in range(len
+0002ae50: 2861 7272 6179 5b69 5d29 293a 0a20 2020  (array[i])):.   
+0002ae60: 2020 2020 2065 6e75 6d65 7261 7465 645f       enumerated_
+0002ae70: 6172 7261 792e 6170 7065 6e64 2828 2869  array.append(((i
+0002ae80: 2c20 6a29 2c20 6172 7261 795b 695d 5b6a  , j), array[i][j
+0002ae90: 5d29 290a 6060 600a 0a23 2323 2320 6067  ])).```..#### `g
+0002aea0: 726f 7570 736f 6660 0a0a 2a2a 6772 6f75  roupsof`..**grou
+0002aeb0: 7073 6f66 2a2a 285f 6e5f 2c20 5f69 7465  psof**(_n_, _ite
+0002aec0: 7261 626c 655f 2c20 5f66 696c 6c76 616c  rable_, _fillval
+0002aed0: 7565 5f3d 602e 2e2e 6029 0a0a 436f 636f  ue_=`...`)..Coco
+0002aee0: 6e75 7420 7072 6f76 6964 6573 2074 6865  nut provides the
+0002aef0: 2060 6772 6f75 7073 6f66 6020 6275 696c   `groupsof` buil
+0002af00: 742d 696e 2074 6f20 7370 6c69 7420 616e  t-in to split an
+0002af10: 2069 7465 7261 626c 6520 696e 746f 2067   iterable into g
+0002af20: 726f 7570 7320 6f66 2061 2073 7065 6369  roups of a speci
+0002af30: 6669 6320 6c65 6e67 7468 2e20 5370 6563  fic length. Spec
+0002af40: 6966 6963 616c 6c79 2c20 6067 726f 7570  ifically, `group
+0002af50: 736f 6628 6e2c 2069 7465 7261 626c 6529  sof(n, iterable)
+0002af60: 6020 7769 6c6c 2073 706c 6974 2060 6974  ` will split `it
+0002af70: 6572 6162 6c65 6020 696e 746f 2074 7570  erable` into tup
+0002af80: 6c65 7320 6f66 206c 656e 6774 6820 606e  les of length `n
+0002af90: 602c 2077 6974 6820 6f6e 6c79 2074 6865  `, with only the
+0002afa0: 206c 6173 7420 7475 706c 6520 706f 7465   last tuple pote
+0002afb0: 6e74 6961 6c6c 7920 6f66 2073 697a 6520  ntially of size 
+0002afc0: 603c 206e 6020 6966 2074 6865 206c 656e  `< n` if the len
+0002afd0: 6774 6820 6f66 2060 6974 6572 6162 6c65  gth of `iterable
+0002afe0: 6020 6973 206e 6f74 2064 6976 6973 6962  ` is not divisib
+0002aff0: 6c65 2062 7920 606e 602e 2049 6620 7468  le by `n`. If th
+0002b000: 6174 2069 7320 6e6f 7420 7468 6520 6465  at is not the de
+0002b010: 7369 7265 6420 6265 6861 7669 6f72 2c20  sired behavior, 
+0002b020: 5f66 696c 6c76 616c 7565 5f20 6361 6e20  _fillvalue_ can 
+0002b030: 6265 2070 6173 7365 6420 616e 6420 7769  be passed and wi
+0002b040: 6c6c 2062 6520 7573 6564 2074 6f20 7061  ll be used to pa
+0002b050: 6420 7468 6520 656e 6420 6f66 2074 6865  d the end of the
+0002b060: 206c 6173 7420 7475 706c 6520 746f 206c   last tuple to l
+0002b070: 656e 6774 6820 606e 602e 0a0a 4164 6469  ength `n`...Addi
+0002b080: 7469 6f6e 616c 6c79 2c20 6067 726f 7570  tionally, `group
+0002b090: 736f 6660 2073 7570 706f 7274 7320 606c  sof` supports `l
+0002b0a0: 656e 6020 7768 656e 2060 6974 6572 6162  en` when `iterab
+0002b0b0: 6c65 6020 7375 7070 6f72 7473 2060 6c65  le` supports `le
+0002b0c0: 6e60 2e0a 0a23 2323 2323 2045 7861 6d70  n`...##### Examp
+0002b0d0: 6c65 0a0a 2a2a 436f 636f 6e75 743a 2a2a  le..**Coconut:**
+0002b0e0: 0a60 6060 636f 636f 6e75 740a 7061 6972  .```coconut.pair
+0002b0f0: 7320 3d20 7261 6e67 6528 312c 2031 3129  s = range(1, 11)
+0002b100: 207c 3e20 6772 6f75 7073 6f66 2428 3229   |> groupsof$(2)
+0002b110: 0a60 6060 0a0a 2a2a 5079 7468 6f6e 3a2a  .```..**Python:*
+0002b120: 2a0a 6060 6063 6f63 6f6e 7574 5f70 7974  *.```coconut_pyt
+0002b130: 686f 6e0a 7061 6972 7320 3d20 5b5d 0a67  hon.pairs = [].g
+0002b140: 726f 7570 203d 205b 5d0a 666f 7220 6974  roup = [].for it
+0002b150: 656d 2069 6e20 7261 6e67 6528 312c 2031  em in range(1, 1
+0002b160: 3129 3a0a 2020 2020 6772 6f75 702e 6170  1):.    group.ap
+0002b170: 7065 6e64 2869 7465 6d29 0a20 2020 2069  pend(item).    i
+0002b180: 6620 6c65 6e28 6772 6f75 7029 203d 3d20  f len(group) == 
+0002b190: 323a 0a20 2020 2020 2020 2070 6169 7273  2:.        pairs
+0002b1a0: 2e61 7070 656e 6428 7475 706c 6528 6772  .append(tuple(gr
+0002b1b0: 6f75 7029 290a 2020 2020 2020 2020 6772  oup)).        gr
+0002b1c0: 6f75 7020 3d20 5b5d 0a69 6620 6772 6f75  oup = [].if grou
+0002b1d0: 703a 0a20 2020 2070 6169 7273 2e61 7070  p:.    pairs.app
+0002b1e0: 656e 6428 7475 706c 6528 6772 6f75 7029  end(tuple(group)
+0002b1f0: 290a 6060 600a 0a23 2323 2320 6077 696e  ).```..#### `win
+0002b200: 646f 7773 6f66 600a 0a2a 2a77 696e 646f  dowsof`..**windo
+0002b210: 7773 6f66 2a2a 285f 7369 7a65 5f2c 205f  wsof**(_size_, _
+0002b220: 6974 6572 6162 6c65 5f2c 205f 6669 6c6c  iterable_, _fill
+0002b230: 7661 6c75 655f 3d60 2e2e 2e60 2c20 5f73  value_=`...`, _s
+0002b240: 7465 705f 3d60 3160 290a 0a60 7769 6e64  tep_=`1`)..`wind
+0002b250: 6f77 736f 6660 2070 726f 6475 6365 7320  owsof` produces 
+0002b260: 616e 2069 7465 7261 626c 6520 7468 6174  an iterable that
+0002b270: 2065 6666 6563 7469 7665 6c79 206d 696d   effectively mim
+0002b280: 6963 7320 6120 736c 6964 696e 6720 7769  ics a sliding wi
+0002b290: 6e64 6f77 206f 7665 7220 5f69 7465 7261  ndow over _itera
+0002b2a0: 626c 655f 206f 6620 7369 7a65 205f 7369  ble_ of size _si
+0002b2b0: 7a65 5f2e 205f 7374 6570 5f20 6465 7465  ze_. _step_ dete
+0002b2c0: 726d 696e 6573 2074 6865 2073 7061 6369  rmines the spaci
+0002b2d0: 6e67 2062 6574 7765 656e 2077 696e 646f  ng between windo
+0002b2e0: 7773 2e0a 0a49 6620 5f73 697a 655f 2069  ws...If _size_ i
+0002b2f0: 7320 6c61 7267 6572 2074 6861 6e20 5f69  s larger than _i
+0002b300: 7465 7261 626c 655f 2c20 6077 696e 646f  terable_, `windo
+0002b310: 7773 6f66 6020 7769 6c6c 2070 726f 6475  wsof` will produ
+0002b320: 6365 2061 6e20 656d 7074 7920 6974 6572  ce an empty iter
+0002b330: 6162 6c65 2e20 4966 2074 6861 7420 6973  able. If that is
+0002b340: 206e 6f74 2074 6865 2064 6573 6972 6564   not the desired
+0002b350: 2062 6568 6176 696f 722c 205f 6669 6c6c   behavior, _fill
+0002b360: 7661 6c75 655f 2063 616e 2062 6520 7061  value_ can be pa
+0002b370: 7373 6564 2061 6e64 2077 696c 6c20 6265  ssed and will be
+0002b380: 2075 7365 6420 696e 2070 6c61 6365 206f   used in place o
+0002b390: 6620 6d69 7373 696e 6720 7661 6c75 6573  f missing values
+0002b3a0: 2e20 416c 736f 2c20 6966 205f 6669 6c6c  . Also, if _fill
+0002b3b0: 7661 6c75 655f 2069 7320 7061 7373 6564  value_ is passed
+0002b3c0: 2061 6e64 2074 6865 206c 656e 6774 6820   and the length 
+0002b3d0: 6f66 2074 6865 205f 6974 6572 6162 6c65  of the _iterable
+0002b3e0: 5f20 6973 206e 6f74 2064 6976 6973 6962  _ is not divisib
+0002b3f0: 6c65 2062 7920 5f73 7465 705f 2c20 5f66  le by _step_, _f
+0002b400: 696c 6c76 616c 7565 5f20 7769 6c6c 2062  illvalue_ will b
+0002b410: 6520 7573 6564 2069 6e20 7468 6174 2063  e used in that c
+0002b420: 6173 6520 746f 2070 6164 2074 6865 206c  ase to pad the l
+0002b430: 6173 7420 7769 6e64 6f77 2061 7320 7765  ast window as we
+0002b440: 6c6c 2e20 4e6f 7465 2074 6861 7420 5f66  ll. Note that _f
+0002b450: 696c 6c76 616c 7565 5f20 7769 6c6c 206f  illvalue_ will o
+0002b460: 6e6c 7920 6576 6572 2061 7070 6561 7220  nly ever appear 
+0002b470: 696e 2074 6865 206c 6173 7420 7769 6e64  in the last wind
+0002b480: 6f77 2e0a 0a41 6464 6974 696f 6e61 6c6c  ow...Additionall
+0002b490: 792c 2060 7769 6e64 6f77 736f 6660 2073  y, `windowsof` s
+0002b4a0: 7570 706f 7274 7320 606c 656e 6020 7768  upports `len` wh
+0002b4b0: 656e 2060 6974 6572 6162 6c65 6020 7375  en `iterable` su
+0002b4c0: 7070 6f72 7473 2060 6c65 6e60 2e0a 0a23  pports `len`...#
+0002b4d0: 2323 2323 2045 7861 6d70 6c65 0a0a 2a2a  #### Example..**
+0002b4e0: 436f 636f 6e75 743a 2a2a 0a60 6060 636f  Coconut:**.```co
+0002b4f0: 636f 6e75 740a 6173 7365 7274 2022 3132  conut.assert "12
+0002b500: 3334 3522 207c 3e20 7769 6e64 6f77 736f  345" |> windowso
+0002b510: 6624 2833 2920 7c3e 206c 6973 7420 3d3d  f$(3) |> list ==
+0002b520: 205b 2822 3122 2c20 2232 222c 2022 3322   [("1", "2", "3"
+0002b530: 292c 2028 2232 222c 2022 3322 2c20 2234  ), ("2", "3", "4
+0002b540: 2229 2c20 2822 3322 2c20 2234 222c 2022  "), ("3", "4", "
+0002b550: 3522 295d 0a60 6060 0a0a 2a2a 5079 7468  5")].```..**Pyth
+0002b560: 6f6e 3a2a 2a0a 5f43 616e 2774 2062 6520  on:**._Can't be 
+0002b570: 646f 6e65 2077 6974 686f 7574 2074 6865  done without the
+0002b580: 2064 6566 696e 6974 696f 6e20 6f66 2060   definition of `
+0002b590: 7769 6e64 6f77 736f 6660 3b20 7365 6520  windowsof`; see 
+0002b5a0: 7468 6520 636f 6d70 696c 6564 2068 6561  the compiled hea
+0002b5b0: 6465 7220 666f 7220 7468 6520 6675 6c6c  der for the full
+0002b5c0: 2064 6566 696e 6974 696f 6e2e 5f0a 0a23   definition._..#
+0002b5d0: 2323 2320 6063 6f6c 6c65 6374 6279 600a  ### `collectby`.
+0002b5e0: 0a2a 2a63 6f6c 6c65 6374 6279 2a2a 285f  .**collectby**(_
+0002b5f0: 6b65 795c 5f66 756e 635f 2c20 5f69 7465  key\_func_, _ite
+0002b600: 7261 626c 655f 2c20 5f76 616c 7565 5c5f  rable_, _value\_
+0002b610: 6675 6e63 5f3d 604e 6f6e 6560 2c20 5f72  func_=`None`, _r
+0002b620: 6564 7563 655c 5f66 756e 635f 3d60 4e6f  educe\_func_=`No
+0002b630: 6e65 6029 0a0a 6063 6f6c 6c65 6374 6279  ne`)..`collectby
+0002b640: 286b 6579 5f66 756e 632c 2069 7465 7261  (key_func, itera
+0002b650: 626c 6529 6020 636f 6c6c 6563 7473 2074  ble)` collects t
+0002b660: 6865 2069 7465 6d73 2069 6e20 6069 7465  he items in `ite
+0002b670: 7261 626c 6560 2069 6e74 6f20 6120 6469  rable` into a di
+0002b680: 6374 696f 6e61 7279 206f 6620 6c69 7374  ctionary of list
+0002b690: 7320 6b65 7965 6420 6279 2060 6b65 795f  s keyed by `key_
+0002b6a0: 6675 6e63 2869 7465 6d29 602e 0a0a 4966  func(item)`...If
+0002b6b0: 2060 7661 6c75 655f 6675 6e63 6020 6973   `value_func` is
+0002b6c0: 2070 6173 7365 642c 2060 636f 6c6c 6563   passed, `collec
+0002b6d0: 7462 7928 6b65 795f 6675 6e63 2c20 6974  tby(key_func, it
+0002b6e0: 6572 6162 6c65 2c20 7661 6c75 655f 6675  erable, value_fu
+0002b6f0: 6e63 3d76 616c 7565 5f66 756e 6329 6020  nc=value_func)` 
+0002b700: 696e 7374 6561 6420 636f 6c6c 6563 7473  instead collects
+0002b710: 2076 616c 7565 5f66 756e 6328 6974 656d   value_func(item
+0002b720: 2920 696e 746f 2065 6163 6820 6c69 7374  ) into each list
+0002b730: 2069 6e73 7465 6164 206f 6620 6974 656d   instead of item
+0002b740: 2e0a 0a49 6620 6072 6564 7563 655f 6675  ...If `reduce_fu
+0002b750: 6e63 6020 6973 2070 6173 7365 642c 2060  nc` is passed, `
+0002b760: 636f 6c6c 6563 7462 7928 6b65 795f 6675  collectby(key_fu
+0002b770: 6e63 2c20 6974 6572 6162 6c65 2c20 7265  nc, iterable, re
+0002b780: 6475 6365 5f66 756e 633d 7265 6475 6365  duce_func=reduce
+0002b790: 5f66 756e 6329 602c 2069 6e73 7465 6164  _func)`, instead
+0002b7a0: 206f 6620 636f 6c6c 6563 7469 6e67 2074   of collecting t
+0002b7b0: 6865 2069 7465 6d73 2069 6e74 6f20 6c69  he items into li
+0002b7c0: 7374 732c 2072 6564 7563 6573 206f 7665  sts, reduces ove
+0002b7d0: 7220 7468 6520 6974 656d 7320 6f66 2065  r the items of e
+0002b7e0: 6163 6820 6b65 7920 7769 7468 2072 6564  ach key with red
+0002b7f0: 7563 655f 6675 6e63 2c20 6566 6665 6374  uce_func, effect
+0002b800: 6976 656c 7920 696d 706c 656d 656e 7469  ively implementi
+0002b810: 6e67 2061 204d 6170 5265 6475 6365 206f  ng a MapReduce o
+0002b820: 7065 7261 7469 6f6e 2e0a 0a60 636f 6c6c  peration...`coll
+0002b830: 6563 7462 7960 2069 7320 6566 6665 6374  ectby` is effect
+0002b840: 6976 656c 7920 6571 7569 7661 6c65 6e74  ively equivalent
+0002b850: 2074 6f3a 0a60 6060 636f 636f 6e75 745f   to:.```coconut_
+0002b860: 7079 7468 6f6e 0a66 726f 6d20 636f 6c6c  python.from coll
+0002b870: 6563 7469 6f6e 7320 696d 706f 7274 2064  ections import d
+0002b880: 6566 6175 6c74 6469 6374 0a0a 6465 6620  efaultdict..def 
+0002b890: 636f 6c6c 6563 7462 7928 6b65 795f 6675  collectby(key_fu
+0002b8a0: 6e63 2c20 6974 6572 6162 6c65 2c20 7661  nc, iterable, va
+0002b8b0: 6c75 655f 6675 6e63 3d69 6465 6e74 2c20  lue_func=ident, 
+0002b8c0: 7265 6475 6365 5f66 756e 633d 4e6f 6e65  reduce_func=None
+0002b8d0: 293a 0a20 2020 2063 6f6c 6c65 6374 696f  ):.    collectio
+0002b8e0: 6e20 3d20 6465 6661 756c 7464 6963 7428  n = defaultdict(
+0002b8f0: 6c69 7374 2920 6966 2072 6564 7563 655f  list) if reduce_
+0002b900: 6675 6e63 2069 7320 4e6f 6e65 2065 6c73  func is None els
+0002b910: 6520 7b7d 0a20 2020 2066 6f72 2069 7465  e {}.    for ite
+0002b920: 6d20 696e 2069 7465 7261 626c 653a 0a20  m in iterable:. 
+0002b930: 2020 2020 2020 206b 6579 203d 206b 6579         key = key
+0002b940: 5f66 756e 6328 6974 656d 290a 2020 2020  _func(item).    
+0002b950: 2020 2020 7661 6c75 6520 3d20 7661 6c75      value = valu
+0002b960: 655f 6675 6e63 2869 7465 6d29 0a20 2020  e_func(item).   
+0002b970: 2020 2020 2069 6620 7265 6475 6365 5f66       if reduce_f
+0002b980: 756e 6320 6973 204e 6f6e 653a 0a20 2020  unc is None:.   
+0002b990: 2020 2020 2020 2020 2063 6f6c 6c65 6374           collect
+0002b9a0: 696f 6e5b 6b65 795d 2e61 7070 656e 6428  ion[key].append(
+0002b9b0: 7661 6c75 6529 0a20 2020 2020 2020 2065  value).        e
+0002b9c0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0002b9d0: 206f 6c64 5f76 616c 7565 203d 2063 6f6c   old_value = col
+0002b9e0: 6c65 6374 696f 6e2e 6765 7428 6b65 792c  lection.get(key,
+0002b9f0: 2073 656e 7469 6e65 6c29 0a20 2020 2020   sentinel).     
+0002ba00: 2020 2020 2020 2069 6620 6f6c 645f 7661         if old_va
+0002ba10: 6c75 6520 6973 206e 6f74 2073 656e 7469  lue is not senti
+0002ba20: 6e65 6c3a 0a20 2020 2020 2020 2020 2020  nel:.           
+0002ba30: 2020 2020 2076 616c 7565 203d 2072 6564       value = red
+0002ba40: 7563 655f 6675 6e63 286f 6c64 5f76 616c  uce_func(old_val
+0002ba50: 7565 2c20 7661 6c75 6529 0a20 2020 2020  ue, value).     
+0002ba60: 2020 2020 2020 2063 6f6c 6c65 6374 696f         collectio
+0002ba70: 6e5b 6b65 795d 203d 2076 616c 7565 0a20  n[key] = value. 
+0002ba80: 2020 2072 6574 7572 6e20 636f 6c6c 6563     return collec
+0002ba90: 7469 6f6e 0a60 6060 0a0a 6063 6f6c 6c65  tion.```..`colle
+0002baa0: 6374 6279 6020 6973 2073 696d 696c 6172  ctby` is similar
+0002bab0: 2074 6f20 5b60 6974 6572 746f 6f6c 732e   to [`itertools.
+0002bac0: 6772 6f75 7062 7960 5d28 6874 7470 733a  groupby`](https:
+0002bad0: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
+0002bae0: 672f 332f 6c69 6272 6172 792f 6974 6572  g/3/library/iter
+0002baf0: 746f 6f6c 732e 6874 6d6c 2369 7465 7274  tools.html#itert
+0002bb00: 6f6f 6c73 2e67 726f 7570 6279 2920 6578  ools.groupby) ex
+0002bb10: 6365 7074 2074 6861 7420 6063 6f6c 6c65  cept that `colle
+0002bb20: 6374 6279 6020 6167 6772 6567 6174 6573  ctby` aggregates
+0002bb30: 2063 6f6d 6d6f 6e20 656c 656d 656e 7473   common elements
+0002bb40: 2072 6567 6172 646c 6573 7320 6f66 2074   regardless of t
+0002bb50: 6865 6972 206f 7264 6572 2069 6e20 7468  heir order in th
+0002bb60: 6520 696e 7075 7420 6974 6572 6162 6c65  e input iterable
+0002bb70: 2c20 7768 6572 6561 7320 6067 726f 7570  , whereas `group
+0002bb80: 6279 6020 6f6e 6c79 2061 6767 7265 6761  by` only aggrega
+0002bb90: 7465 7320 636f 6d6d 6f6e 2065 6c65 6d65  tes common eleme
+0002bba0: 6e74 7320 7468 6174 2061 7265 2061 646a  nts that are adj
+0002bbb0: 6163 656e 7420 696e 2074 6865 2069 6e70  acent in the inp
+0002bbc0: 7574 2069 7465 7261 626c 652e 0a0a 2323  ut iterable...##
+0002bbd0: 2323 2320 4578 616d 706c 650a 0a2a 2a43  ### Example..**C
+0002bbe0: 6f63 6f6e 7574 3a2a 2a0a 6060 6063 6f63  oconut:**.```coc
+0002bbf0: 6f6e 7574 0a75 7365 725f 6261 6c61 6e63  onut.user_balanc
+0002bc00: 6573 203d 2028 0a20 2020 2062 616c 616e  es = (.    balan
+0002bc10: 6365 5f64 6174 610a 2020 2020 7c3e 2063  ce_data.    |> c
+0002bc20: 6f6c 6c65 6374 6279 2428 2e75 7365 722c  ollectby$(.user,
+0002bc30: 2076 616c 7565 5f66 756e 633d 2e62 616c   value_func=.bal
+0002bc40: 616e 6365 2c20 7265 6475 6365 5f66 756e  ance, reduce_fun
+0002bc50: 633d 282b 2929 0a29 0a60 6060 0a0a 2a2a  c=(+)).).```..**
+0002bc60: 5079 7468 6f6e 3a2a 2a0a 6060 6063 6f63  Python:**.```coc
+0002bc70: 6f6e 7574 5f70 7974 686f 6e0a 6672 6f6d  onut_python.from
+0002bc80: 2063 6f6c 6c65 6374 696f 6e73 2069 6d70   collections imp
+0002bc90: 6f72 7420 6465 6661 756c 7464 6963 740a  ort defaultdict.
+0002bca0: 0a75 7365 725f 6261 6c61 6e63 6573 203d  .user_balances =
+0002bcb0: 2064 6566 6175 6c74 6469 6374 2869 6e74   defaultdict(int
+0002bcc0: 290a 666f 7220 6974 656d 2069 6e20 6261  ).for item in ba
+0002bcd0: 6c61 6e63 655f 6461 7461 3a0a 2020 2020  lance_data:.    
+0002bce0: 7573 6572 5f62 616c 616e 6365 735b 6974  user_balances[it
+0002bcf0: 656d 2e75 7365 725d 202b 3d20 6974 656d  em.user] += item
+0002bd00: 2e62 616c 616e 6365 0a60 6060 0a0a 2323  .balance.```..##
+0002bd10: 2323 2060 616c 6c5f 6571 7561 6c60 0a0a  ## `all_equal`..
+0002bd20: 2a2a 616c 6c5c 5f65 7175 616c 2a2a 285f  **all\_equal**(_
+0002bd30: 6974 6572 6162 6c65 5f29 0a0a 436f 636f  iterable_)..Coco
+0002bd40: 6e75 7427 7320 6061 6c6c 5f65 7175 616c  nut's `all_equal
+0002bd50: 6020 6275 696c 742d 696e 2074 616b 6573  ` built-in takes
+0002bd60: 2069 6e20 616e 2069 7465 7261 626c 6520   in an iterable 
+0002bd70: 616e 6420 6465 7465 726d 696e 6573 2077  and determines w
+0002bd80: 6865 7468 6572 2061 6c6c 206f 6620 6974  hether all of it
+0002bd90: 7320 656c 656d 656e 7473 2061 7265 2065  s elements are e
+0002bda0: 7175 616c 2074 6f20 6561 6368 206f 7468  qual to each oth
+0002bdb0: 6572 2e20 6061 6c6c 5f65 7175 616c 6020  er. `all_equal` 
+0002bdc0: 6173 7375 6d65 7320 7472 616e 7369 7469  assumes transiti
+0002bdd0: 7669 7479 206f 6620 6571 7561 6c69 7479  vity of equality
+0002bde0: 2061 6e64 2074 6861 7420 6021 3d60 2069   and that `!=` i
+0002bdf0: 7320 7468 6520 6e65 6761 7469 6f6e 206f  s the negation o
+0002be00: 6620 603d 3d60 2e20 5370 6563 6961 6c20  f `==`. Special 
+0002be10: 7375 7070 6f72 7420 6973 2070 726f 7669  support is provi
+0002be20: 6465 6420 666f 7220 5b60 6e75 6d70 7960  ded for [`numpy`
+0002be30: 5d28 236e 756d 7079 2d69 6e74 6567 7261  ](#numpy-integra
+0002be40: 7469 6f6e 2920 6f62 6a65 6374 732e 0a0a  tion) objects...
+0002be50: 2323 2323 2320 4578 616d 706c 650a 0a2a  ##### Example..*
+0002be60: 2a43 6f63 6f6e 7574 3a2a 2a0a 6060 6063  *Coconut:**.```c
+0002be70: 6f63 6f6e 7574 0a61 6c6c 5f65 7175 616c  oconut.all_equal
+0002be80: 285b 312c 2031 2c20 315d 290a 616c 6c5f  ([1, 1, 1]).all_
+0002be90: 6571 7561 6c28 5b31 2c20 312c 2032 5d29  equal([1, 1, 2])
+0002bea0: 0a60 6060 0a0a 2a2a 5079 7468 6f6e 3a2a  .```..**Python:*
+0002beb0: 2a0a 6060 6063 6f63 6f6e 7574 5f70 7974  *.```coconut_pyt
+0002bec0: 686f 6e0a 7365 6e74 696e 656c 203d 206f  hon.sentinel = o
+0002bed0: 626a 6563 7428 290a 6465 6620 616c 6c5f  bject().def all_
+0002bee0: 6571 7561 6c28 6974 6572 6162 6c65 293a  equal(iterable):
+0002bef0: 0a20 2020 2066 6972 7374 5f69 7465 6d20  .    first_item 
+0002bf00: 3d20 7365 6e74 696e 656c 0a20 2020 2066  = sentinel.    f
+0002bf10: 6f72 2069 7465 6d20 696e 2069 7465 7261  or item in itera
+0002bf20: 626c 653a 0a20 2020 2020 2020 2069 6620  ble:.        if 
+0002bf30: 6669 7273 745f 6974 656d 2069 7320 7365  first_item is se
+0002bf40: 6e74 696e 656c 3a0a 2020 2020 2020 2020  ntinel:.        
+0002bf50: 2020 2020 6669 7273 745f 6974 656d 203d      first_item =
+0002bf60: 2069 7465 6d0a 2020 2020 2020 2020 656c   item.        el
+0002bf70: 6966 2066 6972 7374 5f69 7465 6d20 213d  if first_item !=
+0002bf80: 2069 7465 6d3a 0a20 2020 2020 2020 2020   item:.         
+0002bf90: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+0002bfa0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0002bfb0: 616c 6c5f 6571 7561 6c28 5b31 2c20 312c  all_equal([1, 1,
+0002bfc0: 2031 5d29 0a61 6c6c 5f65 7175 616c 285b   1]).all_equal([
+0002bfd0: 312c 2031 2c20 325d 290a 6060 600a 0a23  1, 1, 2]).```..#
+0002bfe0: 2323 2320 6070 6172 616c 6c65 6c5f 6d61  ### `parallel_ma
+0002bff0: 7060 0a0a 2a2a 7061 7261 6c6c 656c 5c5f  p`..**parallel\_
+0002c000: 6d61 702a 2a28 5f66 756e 6374 696f 6e5f  map**(_function_
+0002c010: 2c20 2a5f 6974 6572 6162 6c65 735f 2c20  , *_iterables_, 
+0002c020: 2a2c 205f 6368 756e 6b73 697a 655f 3d60  *, _chunksize_=`
+0002c030: 3160 2c20 5f73 7472 6963 745f 3d60 4661  1`, _strict_=`Fa
+0002c040: 6c73 6560 290a 0a43 6f63 6f6e 7574 2070  lse`)..Coconut p
+0002c050: 726f 7669 6465 7320 6120 7061 7261 6c6c  rovides a parall
+0002c060: 656c 2076 6572 7369 6f6e 206f 6620 606d  el version of `m
+0002c070: 6170 6020 756e 6465 7220 7468 6520 6e61  ap` under the na
+0002c080: 6d65 2060 7061 7261 6c6c 656c 5f6d 6170  me `parallel_map
+0002c090: 602e 2060 7061 7261 6c6c 656c 5f6d 6170  `. `parallel_map
+0002c0a0: 6020 6d61 6b65 7320 7573 6520 6f66 206d  ` makes use of m
+0002c0b0: 756c 7469 706c 6520 7072 6f63 6573 7365  ultiple processe
+0002c0c0: 732c 2061 6e64 2069 7320 7468 6572 6566  s, and is theref
+0002c0d0: 6f72 6520 6d75 6368 2066 6173 7465 7220  ore much faster 
+0002c0e0: 7468 616e 2060 6d61 7060 2066 6f72 2043  than `map` for C
+0002c0f0: 5055 2d62 6f75 6e64 2074 6173 6b73 2e20  PU-bound tasks. 
+0002c100: 6070 6172 616c 6c65 6c5f 6d61 7060 206e  `parallel_map` n
+0002c110: 6576 6572 206c 6f61 6473 2074 6865 2065  ever loads the e
+0002c120: 6e74 6972 6520 696e 7075 7420 6974 6572  ntire input iter
+0002c130: 6174 6f72 2069 6e74 6f20 6d65 6d6f 7279  ator into memory
+0002c140: 2c20 7468 6f75 6768 2069 7420 646f 6573  , though it does
+0002c150: 2063 6f6e 7375 6d65 2074 6865 2065 6e74   consume the ent
+0002c160: 6972 6520 696e 7075 7420 6974 6572 6174  ire input iterat
+0002c170: 6f72 2061 7320 736f 6f6e 2061 7320 6120  or as soon as a 
+0002c180: 7369 6e67 6c65 206f 7574 7075 7420 6973  single output is
+0002c190: 2072 6571 7565 7374 6564 2e20 4966 2061   requested. If a
+0002c1a0: 6e79 2065 7863 6570 7469 6f6e 7320 6172  ny exceptions ar
+0002c1b0: 6520 7261 6973 6564 2069 6e73 6964 6520  e raised inside 
+0002c1c0: 6f66 2060 7061 7261 6c6c 656c 5f6d 6170  of `parallel_map
+0002c1d0: 602c 2061 2074 7261 6365 6261 636b 2077  `, a traceback w
+0002c1e0: 696c 6c20 6265 2070 7269 6e74 6564 2061  ill be printed a
+0002c1f0: 7320 736f 6f6e 2061 7320 7468 6579 2061  s soon as they a
+0002c200: 7265 2065 6e63 6f75 6e74 6572 6564 2e0a  re encountered..
+0002c210: 0a42 6563 6175 7365 2060 7061 7261 6c6c  .Because `parall
+0002c220: 656c 5f6d 6170 6020 7573 6573 206d 756c  el_map` uses mul
+0002c230: 7469 706c 6520 7072 6f63 6573 7365 7320  tiple processes 
+0002c240: 666f 7220 6974 7320 6578 6563 7574 696f  for its executio
+0002c250: 6e2c 2069 7420 6973 206e 6563 6573 7361  n, it is necessa
+0002c260: 7279 2074 6861 7420 616c 6c20 6f66 2069  ry that all of i
+0002c270: 7473 2061 7267 756d 656e 7473 2062 6520  ts arguments be 
+0002c280: 7069 636b 6c65 6162 6c65 2e20 4f6e 6c79  pickleable. Only
+0002c290: 206f 626a 6563 7473 2064 6566 696e 6564   objects defined
+0002c2a0: 2061 7420 7468 6520 6d6f 6475 6c65 206c   at the module l
+0002c2b0: 6576 656c 2c20 616e 6420 6e6f 7420 6c61  evel, and not la
+0002c2c0: 6d62 6461 732c 206f 626a 6563 7473 2064  mbdas, objects d
+0002c2d0: 6566 696e 6564 2069 6e73 6964 6520 6f66  efined inside of
+0002c2e0: 2061 2066 756e 6374 696f 6e2c 206f 7220   a function, or 
+0002c2f0: 6f62 6a65 6374 7320 6465 6669 6e65 6420  objects defined 
+0002c300: 696e 7369 6465 206f 6620 7468 6520 696e  inside of the in
+0002c310: 7465 7270 7265 7465 722c 2061 7265 2070  terpreter, are p
+0002c320: 6963 6b6c 6561 626c 652e 2046 7572 7468  ickleable. Furth
+0002c330: 6572 6d6f 7265 2c20 6f6e 2057 696e 646f  ermore, on Windo
+0002c340: 7773 2c20 6974 2069 7320 6e65 6365 7373  ws, it is necess
+0002c350: 6172 7920 7468 6174 2061 6c6c 2063 616c  ary that all cal
+0002c360: 6c73 2074 6f20 6070 6172 616c 6c65 6c5f  ls to `parallel_
+0002c370: 6d61 7060 206f 6363 7572 2069 6e73 6964  map` occur insid
+0002c380: 6520 6f66 2061 6e20 6069 6620 5f5f 6e61  e of an `if __na
+0002c390: 6d65 5f5f 203d 3d20 225f 5f6d 6169 6e5f  me__ == "__main_
+0002c3a0: 5f22 6020 6775 6172 642e 0a0a 6070 6172  _"` guard...`par
+0002c3b0: 616c 6c65 6c5f 6d61 7060 2073 7570 706f  allel_map` suppo
+0002c3c0: 7274 7320 6120 6063 6875 6e6b 7369 7a65  rts a `chunksize
+0002c3d0: 6020 6172 6775 6d65 6e74 2c20 7768 6963  ` argument, whic
+0002c3e0: 6820 6465 7465 726d 696e 6573 2068 6f77  h determines how
+0002c3f0: 206d 616e 7920 6974 656d 7320 6172 6520   many items are 
+0002c400: 7061 7373 6564 2074 6f20 6561 6368 2070  passed to each p
+0002c410: 726f 6365 7373 2061 7420 6120 7469 6d65  rocess at a time
+0002c420: 2e20 4c61 7267 6572 2076 616c 7565 7320  . Larger values 
+0002c430: 6f66 205f 6368 756e 6b73 697a 655f 2061  of _chunksize_ a
+0002c440: 7265 2072 6563 6f6d 6d65 6e64 6564 2077  re recommended w
+0002c450: 6865 6e20 6465 616c 696e 6720 7769 7468  hen dealing with
+0002c460: 2076 6572 7920 6c6f 6e67 2069 7465 7261   very long itera
+0002c470: 626c 6573 2e20 4164 6469 7469 6f6e 616c  bles. Additional
+0002c480: 6c79 2c20 696e 2074 6865 206d 756c 7469  ly, in the multi
+0002c490: 2d69 7465 7261 626c 6520 6361 7365 2c20  -iterable case, 
+0002c4a0: 5f73 7472 6963 745f 2063 616e 2062 6520  _strict_ can be 
+0002c4b0: 7365 7420 746f 2060 5472 7565 6020 746f  set to `True` to
+0002c4c0: 2065 6e73 7572 6520 7468 6174 2061 6c6c   ensure that all
+0002c4d0: 2069 7465 7261 626c 6573 2061 7265 2074   iterables are t
+0002c4e0: 6865 2073 616d 6520 6c65 6e67 7468 2e0a  he same length..
+0002c4f0: 0a49 6620 6d75 6c74 6970 6c65 2073 6571  .If multiple seq
+0002c500: 7565 6e74 6961 6c20 6361 6c6c 7320 746f  uential calls to
+0002c510: 2060 7061 7261 6c6c 656c 5f6d 6170 6020   `parallel_map` 
+0002c520: 6e65 6564 2074 6f20 6265 206d 6164 652c  need to be made,
+0002c530: 2069 7420 6973 2068 6967 686c 7920 7265   it is highly re
+0002c540: 636f 6d6d 656e 6465 6420 7468 6174 2074  commended that t
+0002c550: 6865 7920 6265 2064 6f6e 6520 696e 7369  hey be done insi
+0002c560: 6465 206f 6620 6120 6077 6974 6820 7061  de of a `with pa
+0002c570: 7261 6c6c 656c 5f6d 6170 2e6d 756c 7469  rallel_map.multi
+0002c580: 706c 655f 7365 7175 656e 7469 616c 5f63  ple_sequential_c
+0002c590: 616c 6c73 2829 3a60 2062 6c6f 636b 2c20  alls():` block, 
+0002c5a0: 7768 6963 6820 7769 6c6c 2063 6175 7365  which will cause
+0002c5b0: 2074 6865 2064 6966 6665 7265 6e74 2063   the different c
+0002c5c0: 616c 6c73 2074 6f20 7573 6520 7468 6520  alls to use the 
+0002c5d0: 7361 6d65 2070 726f 6365 7373 2070 6f6f  same process poo
+0002c5e0: 6c20 616e 6420 7265 7375 6c74 2069 6e20  l and result in 
+0002c5f0: 6070 6172 616c 6c65 6c5f 6d61 7060 2069  `parallel_map` i
+0002c600: 6d6d 6564 6961 7465 6c79 2072 6574 7572  mmediately retur
+0002c610: 6e69 6e67 2061 206c 6973 7420 7261 7468  ning a list rath
+0002c620: 6572 2074 6861 6e20 6120 6070 6172 616c  er than a `paral
+0002c630: 6c65 6c5f 6d61 7060 206f 626a 6563 742e  lel_map` object.
+0002c640: 2049 6620 6d75 6c74 6970 6c65 2073 6571   If multiple seq
+0002c650: 7565 6e74 6961 6c20 6361 6c6c 7320 6172  uential calls ar
+0002c660: 6520 6e65 6365 7373 6172 7920 616e 6420  e necessary and 
+0002c670: 7468 6520 6c61 7a69 6e65 7373 206f 6620  the laziness of 
+0002c680: 7061 7261 6c6c 656c 5f6d 6170 2069 7320  parallel_map is 
+0002c690: 7265 7175 6972 6564 2c20 7468 656e 2074  required, then t
+0002c6a0: 6865 2060 7061 7261 6c6c 656c 5f6d 6170  he `parallel_map
+0002c6b0: 6020 6f62 6a65 6374 7320 7368 6f75 6c64  ` objects should
+0002c6c0: 2062 6520 636f 6e73 7472 7563 7465 6420   be constructed 
+0002c6d0: 6265 666f 7265 2074 6865 2060 6d75 6c74  before the `mult
+0002c6e0: 6970 6c65 5f73 6571 7565 6e74 6961 6c5f  iple_sequential_
+0002c6f0: 6361 6c6c 7360 2062 6c6f 636b 2061 6e64  calls` block and
+0002c700: 2074 6865 6e20 6f6e 6c79 2069 7465 7261   then only itera
+0002c710: 7465 6420 6f76 6572 206f 6e63 6520 696e  ted over once in
+0002c720: 7369 6465 2074 6865 2062 6c6f 636b 2e0a  side the block..
+0002c730: 0a60 7061 7261 6c6c 656c 5f6d 6170 2e6d  .`parallel_map.m
+0002c740: 756c 7469 706c 655f 7365 7175 656e 7469  ultiple_sequenti
+0002c750: 616c 5f63 616c 6c73 6020 616c 736f 2073  al_calls` also s
+0002c760: 7570 706f 7274 7320 6120 606d 6178 5f77  upports a `max_w
+0002c770: 6f72 6b65 7273 6020 6172 6775 6d65 6e74  orkers` argument
+0002c780: 2074 6f20 7365 7420 7468 6520 6e75 6d62   to set the numb
+0002c790: 6572 206f 6620 7072 6f63 6573 7365 732e  er of processes.
+0002c7a0: 0a0a 2323 2323 2320 5079 7468 6f6e 2044  ..##### Python D
+0002c7b0: 6f63 730a 0a2a 2a70 6172 616c 6c65 6c5f  ocs..**parallel_
+0002c7c0: 6d61 702a 2a28 5f66 756e 632c 205c 2a69  map**(_func, \*i
+0002c7d0: 7465 7261 626c 6573 5f2c 205f 6368 756e  terables_, _chun
+0002c7e0: 6b73 697a 655f 3d60 3160 290a 0a45 7175  ksize_=`1`)..Equ
+0002c7f0: 6976 616c 656e 7420 746f 2060 6d61 7028  ivalent to `map(
+0002c800: 6675 6e63 2c20 2a69 7465 7261 626c 6573  func, *iterables
+0002c810: 2960 2065 7863 6570 7420 5f66 756e 635f  )` except _func_
+0002c820: 2069 7320 6578 6563 7574 6564 2061 7379   is executed asy
+0002c830: 6e63 6872 6f6e 6f75 736c 7920 616e 6420  nchronously and 
+0002c840: 7365 7665 7261 6c20 6361 6c6c 7320 746f  several calls to
+0002c850: 205f 6675 6e63 5f20 6d61 7920 6265 206d   _func_ may be m
+0002c860: 6164 6520 636f 6e63 7572 7265 6e74 6c79  ade concurrently
+0002c870: 2e20 4966 2061 2063 616c 6c20 7261 6973  . If a call rais
+0002c880: 6573 2061 6e20 6578 6365 7074 696f 6e2c  es an exception,
+0002c890: 2074 6865 6e20 7468 6174 2065 7863 6570   then that excep
+0002c8a0: 7469 6f6e 2077 696c 6c20 6265 2072 6169  tion will be rai
+0002c8b0: 7365 6420 7768 656e 2069 7473 2076 616c  sed when its val
+0002c8c0: 7565 2069 7320 7265 7472 6965 7665 6420  ue is retrieved 
+0002c8d0: 6672 6f6d 2074 6865 2069 7465 7261 746f  from the iterato
+0002c8e0: 722e 0a0a 6070 6172 616c 6c65 6c5f 6d61  r...`parallel_ma
+0002c8f0: 7060 2063 686f 7073 2074 6865 2069 7465  p` chops the ite
+0002c900: 7261 626c 6520 696e 746f 2061 206e 756d  rable into a num
+0002c910: 6265 7220 6f66 2063 6875 6e6b 7320 7768  ber of chunks wh
+0002c920: 6963 6820 6974 2073 7562 6d69 7473 2074  ich it submits t
+0002c930: 6f20 7468 6520 7072 6f63 6573 7320 706f  o the process po
+0002c940: 6f6c 2061 7320 7365 7061 7261 7465 2074  ol as separate t
+0002c950: 6173 6b73 2e20 5468 6520 2861 7070 726f  asks. The (appro
+0002c960: 7869 6d61 7465 2920 7369 7a65 206f 6620  ximate) size of 
+0002c970: 7468 6573 6520 6368 756e 6b73 2063 616e  these chunks can
+0002c980: 2062 6520 7370 6563 6966 6965 6420 6279   be specified by
+0002c990: 2073 6574 7469 6e67 205f 6368 756e 6b73   setting _chunks
+0002c9a0: 697a 655f 2074 6f20 6120 706f 7369 7469  ize_ to a positi
+0002c9b0: 7665 2069 6e74 6567 6572 2e20 466f 7220  ve integer. For 
+0002c9c0: 7665 7279 206c 6f6e 6720 6974 6572 6162  very long iterab
+0002c9d0: 6c65 7320 7573 696e 6720 6120 6c61 7267  les using a larg
+0002c9e0: 6520 7661 6c75 6520 666f 7220 5f63 6875  e value for _chu
+0002c9f0: 6e6b 7369 7a65 5f20 6361 6e20 6d61 6b65  nksize_ can make
+0002ca00: 2074 6865 206a 6f62 2063 6f6d 706c 6574   the job complet
+0002ca10: 6520 2a2a 6d75 6368 2a2a 2066 6173 7465  e **much** faste
+0002ca20: 7220 7468 616e 2075 7369 6e67 2074 6865  r than using the
+0002ca30: 2064 6566 6175 6c74 2076 616c 7565 206f   default value o
+0002ca40: 6620 6031 602e 0a0a 2323 2323 2320 4578  f `1`...##### Ex
+0002ca50: 616d 706c 650a 0a2a 2a43 6f63 6f6e 7574  ample..**Coconut
+0002ca60: 3a2a 2a0a 6060 6063 6f63 6f6e 7574 0a70  :**.```coconut.p
+0002ca70: 6172 616c 6c65 6c5f 6d61 7028 706f 7724  arallel_map(pow$
+0002ca80: 2832 292c 2072 616e 6765 2831 3030 2929  (2), range(100))
+0002ca90: 207c 3e20 6c69 7374 207c 3e20 7072 696e   |> list |> prin
+0002caa0: 740a 6060 600a 0a2a 2a50 7974 686f 6e3a  t.```..**Python:
+0002cab0: 2a2a 0a60 6060 636f 636f 6e75 745f 7079  **.```coconut_py
+0002cac0: 7468 6f6e 0a69 6d70 6f72 7420 6675 6e63  thon.import func
+0002cad0: 746f 6f6c 730a 6672 6f6d 206d 756c 7469  tools.from multi
+0002cae0: 7072 6f63 6573 7369 6e67 2069 6d70 6f72  processing impor
+0002caf0: 7420 506f 6f6c 0a77 6974 6820 506f 6f6c  t Pool.with Pool
+0002cb00: 2829 2061 7320 706f 6f6c 3a0a 2020 2020  () as pool:.    
+0002cb10: 7072 696e 7428 6c69 7374 2870 6f6f 6c2e  print(list(pool.
+0002cb20: 696d 6170 2866 756e 6374 6f6f 6c73 2e70  imap(functools.p
+0002cb30: 6172 7469 616c 2870 6f77 2c20 3229 2c20  artial(pow, 2), 
+0002cb40: 7261 6e67 6528 3130 3029 2929 290a 6060  range(100)))).``
+0002cb50: 600a 0a23 2323 2320 6063 6f6e 6375 7272  `..#### `concurr
+0002cb60: 656e 745f 6d61 7060 0a0a 2a2a 636f 6e63  ent_map`..**conc
+0002cb70: 7572 7265 6e74 5c5f 6d61 702a 2a28 5f66  urrent\_map**(_f
+0002cb80: 756e 6374 696f 6e5f 2c20 2a5f 6974 6572  unction_, *_iter
+0002cb90: 6162 6c65 735f 2c20 2a2c 205f 6368 756e  ables_, *, _chun
+0002cba0: 6b73 697a 655f 3d60 3160 2c20 5f73 7472  ksize_=`1`, _str
+0002cbb0: 6963 745f 3d60 4661 6c73 6560 290a 0a43  ict_=`False`)..C
+0002cbc0: 6f63 6f6e 7574 2070 726f 7669 6465 7320  oconut provides 
+0002cbd0: 6120 636f 6e63 7572 7265 6e74 2076 6572  a concurrent ver
+0002cbe0: 7369 6f6e 206f 6620 5b60 7061 7261 6c6c  sion of [`parall
+0002cbf0: 656c 5f6d 6170 605d 2823 7061 7261 6c6c  el_map`](#parall
+0002cc00: 656c 5f6d 6170 2920 756e 6465 7220 7468  el_map) under th
+0002cc10: 6520 6e61 6d65 2060 636f 6e63 7572 7265  e name `concurre
+0002cc20: 6e74 5f6d 6170 602e 2060 636f 6e63 7572  nt_map`. `concur
+0002cc30: 7265 6e74 5f6d 6170 6020 6265 6861 7665  rent_map` behave
+0002cc40: 7320 6964 656e 7469 6361 6c6c 7920 746f  s identically to
+0002cc50: 2060 7061 7261 6c6c 656c 5f6d 6170 6020   `parallel_map` 
+0002cc60: 2869 6e63 6c75 6469 6e67 2073 7570 706f  (including suppo
+0002cc70: 7274 2066 6f72 2060 636f 6e63 7572 7265  rt for `concurre
+0002cc80: 6e74 5f6d 6170 2e6d 756c 7469 706c 655f  nt_map.multiple_
+0002cc90: 7365 7175 656e 7469 616c 5f63 616c 6c73  sequential_calls
+0002cca0: 6029 2065 7863 6570 7420 7468 6174 2069  `) except that i
+0002ccb0: 7420 7573 6573 206d 756c 7469 7468 7265  t uses multithre
+0002ccc0: 6164 696e 6720 696e 7374 6561 6420 6f66  ading instead of
+0002ccd0: 206d 756c 7469 7072 6f63 6573 7369 6e67   multiprocessing
+0002cce0: 2c20 616e 6420 6973 2074 6865 7265 666f  , and is therefo
+0002ccf0: 7265 2070 7269 6d61 7269 6c79 2075 7365  re primarily use
+0002cd00: 6675 6c20 6f6e 6c79 2066 6f72 2049 4f2d  ful only for IO-
+0002cd10: 626f 756e 6420 7461 736b 7320 6475 6520  bound tasks due 
+0002cd20: 746f 2043 5079 7468 6f6e 2773 2047 6c6f  to CPython's Glo
+0002cd30: 6261 6c20 496e 7465 7270 7265 7465 7220  bal Interpreter 
+0002cd40: 4c6f 636b 2e0a 0a23 2323 2323 2050 7974  Lock...##### Pyt
+0002cd50: 686f 6e20 446f 6373 0a0a 2a2a 636f 6e63  hon Docs..**conc
+0002cd60: 7572 7265 6e74 5f6d 6170 2a2a 285f 6675  urrent_map**(_fu
+0002cd70: 6e63 2c20 5c2a 6974 6572 6162 6c65 735f  nc, \*iterables_
+0002cd80: 2c20 5f63 6875 6e6b 7369 7a65 5f3d 6031  , _chunksize_=`1
+0002cd90: 6029 0a0a 4571 7569 7661 6c65 6e74 2074  `)..Equivalent t
+0002cda0: 6f20 606d 6170 2866 756e 632c 202a 6974  o `map(func, *it
+0002cdb0: 6572 6162 6c65 7329 6020 6578 6365 7074  erables)` except
+0002cdc0: 205f 6675 6e63 5f20 6973 2065 7865 6375   _func_ is execu
+0002cdd0: 7465 6420 6173 796e 6368 726f 6e6f 7573  ted asynchronous
+0002cde0: 6c79 2061 6e64 2073 6576 6572 616c 2063  ly and several c
+0002cdf0: 616c 6c73 2074 6f20 5f66 756e 635f 206d  alls to _func_ m
+0002ce00: 6179 2062 6520 6d61 6465 2063 6f6e 6375  ay be made concu
+0002ce10: 7272 656e 746c 792e 2049 6620 6120 6361  rrently. If a ca
+0002ce20: 6c6c 2072 6169 7365 7320 616e 2065 7863  ll raises an exc
+0002ce30: 6570 7469 6f6e 2c20 7468 656e 2074 6861  eption, then tha
+0002ce40: 7420 6578 6365 7074 696f 6e20 7769 6c6c  t exception will
+0002ce50: 2062 6520 7261 6973 6564 2077 6865 6e20   be raised when 
+0002ce60: 6974 7320 7661 6c75 6520 6973 2072 6574  its value is ret
+0002ce70: 7269 6576 6564 2066 726f 6d20 7468 6520  rieved from the 
+0002ce80: 6974 6572 6174 6f72 2e0a 0a60 636f 6e63  iterator...`conc
+0002ce90: 7572 7265 6e74 5f6d 6170 6020 6368 6f70  urrent_map` chop
+0002cea0: 7320 7468 6520 6974 6572 6162 6c65 2069  s the iterable i
+0002ceb0: 6e74 6f20 6120 6e75 6d62 6572 206f 6620  nto a number of 
+0002cec0: 6368 756e 6b73 2077 6869 6368 2069 7420  chunks which it 
+0002ced0: 7375 626d 6974 7320 746f 2074 6865 2074  submits to the t
+0002cee0: 6872 6561 6420 706f 6f6c 2061 7320 7365  hread pool as se
+0002cef0: 7061 7261 7465 2074 6173 6b73 2e20 5468  parate tasks. Th
+0002cf00: 6520 2861 7070 726f 7869 6d61 7465 2920  e (approximate) 
+0002cf10: 7369 7a65 206f 6620 7468 6573 6520 6368  size of these ch
+0002cf20: 756e 6b73 2063 616e 2062 6520 7370 6563  unks can be spec
+0002cf30: 6966 6965 6420 6279 2073 6574 7469 6e67  ified by setting
+0002cf40: 205f 6368 756e 6b73 697a 655f 2074 6f20   _chunksize_ to 
+0002cf50: 6120 706f 7369 7469 7665 2069 6e74 6567  a positive integ
+0002cf60: 6572 2e20 466f 7220 7665 7279 206c 6f6e  er. For very lon
+0002cf70: 6720 6974 6572 6162 6c65 7320 7573 696e  g iterables usin
+0002cf80: 6720 6120 6c61 7267 6520 7661 6c75 6520  g a large value 
+0002cf90: 666f 7220 5f63 6875 6e6b 7369 7a65 5f20  for _chunksize_ 
+0002cfa0: 6361 6e20 6d61 6b65 2074 6865 206a 6f62  can make the job
+0002cfb0: 2063 6f6d 706c 6574 6520 2a2a 6d75 6368   complete **much
+0002cfc0: 2a2a 2066 6173 7465 7220 7468 616e 2075  ** faster than u
+0002cfd0: 7369 6e67 2074 6865 2064 6566 6175 6c74  sing the default
+0002cfe0: 2076 616c 7565 206f 6620 6031 602e 0a0a   value of `1`...
+0002cff0: 2323 2323 2320 4578 616d 706c 650a 0a2a  ##### Example..*
+0002d000: 2a43 6f63 6f6e 7574 3a2a 2a0a 6060 6063  *Coconut:**.```c
+0002d010: 6f63 6f6e 7574 0a63 6f6e 6375 7272 656e  oconut.concurren
+0002d020: 745f 6d61 7028 6765 745f 6461 7461 5f66  t_map(get_data_f
+0002d030: 6f72 5f75 7365 722c 2067 6574 5f61 6c6c  or_user, get_all
+0002d040: 5f75 7365 7273 2829 2920 7c3e 206c 6973  _users()) |> lis
+0002d050: 7420 7c3e 2070 7269 6e74 0a60 6060 0a0a  t |> print.```..
+0002d060: 2a2a 5079 7468 6f6e 3a2a 2a0a 6060 6063  **Python:**.```c
+0002d070: 6f63 6f6e 7574 5f70 7974 686f 6e0a 696d  oconut_python.im
+0002d080: 706f 7274 2066 756e 6374 6f6f 6c73 0a69  port functools.i
+0002d090: 6d70 6f72 7420 636f 6e63 7572 7265 6e74  mport concurrent
+0002d0a0: 2e66 7574 7572 6573 0a77 6974 6820 636f  .futures.with co
+0002d0b0: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
+0002d0c0: 2e54 6872 6561 6450 6f6f 6c45 7865 6375  .ThreadPoolExecu
+0002d0d0: 746f 7228 2920 6173 2065 7865 6375 746f  tor() as executo
+0002d0e0: 723a 0a20 2020 2070 7269 6e74 286c 6973  r:.    print(lis
+0002d0f0: 7428 6578 6563 7574 6f72 2e6d 6170 2867  t(executor.map(g
+0002d100: 6574 5f64 6174 615f 666f 725f 7573 6572  et_data_for_user
+0002d110: 2c20 6765 745f 616c 6c5f 7573 6572 7328  , get_all_users(
+0002d120: 2929 2929 0a60 6060 0a0a 2323 2323 2060  )))).```..#### `
+0002d130: 7465 6560 0a0a 2a2a 7465 652a 2a28 5f69  tee`..**tee**(_i
+0002d140: 7465 7261 626c 655f 2c20 5f6e 5f3d 6032  terable_, _n_=`2
+0002d150: 6029 0a0a 436f 636f 6e75 7420 7072 6f76  `)..Coconut prov
+0002d160: 6964 6573 2061 6e20 6f70 7469 6d69 7a65  ides an optimize
+0002d170: 6420 7665 7273 696f 6e20 6f66 2060 6974  d version of `it
+0002d180: 6572 746f 6f6c 732e 7465 6560 2061 7320  ertools.tee` as 
+0002d190: 6120 6275 696c 742d 696e 2075 6e64 6572  a built-in under
+0002d1a0: 2074 6865 206e 616d 6520 6074 6565 602e   the name `tee`.
+0002d1b0: 0a0a 5468 6f75 6768 2060 7465 6560 2069  ..Though `tee` i
+0002d1c0: 7320 6e6f 7420 6465 7072 6563 6174 6564  s not deprecated
+0002d1d0: 2c20 5b60 7265 6974 6572 6162 6c65 605d  , [`reiterable`]
+0002d1e0: 2823 7265 6974 6572 6162 6c65 2920 6973  (#reiterable) is
+0002d1f0: 2067 656e 6572 616c 6c79 2072 6563 6f6d   generally recom
+0002d200: 6d65 6e64 6564 206f 7665 7220 6074 6565  mended over `tee
+0002d210: 602e 0a0a 4375 7374 6f6d 2060 7465 6560  `...Custom `tee`
+0002d220: 2f60 7265 6974 6572 6162 6c65 6020 696d  /`reiterable` im
+0002d230: 706c 656d 656e 7461 7469 6f6e 7320 666f  plementations fo
+0002d240: 7220 6375 7374 6f6d 205b 436f 6e74 6169  r custom [Contai
+0002d250: 6e65 7273 2f43 6f6c 6c65 6374 696f 6e73  ners/Collections
+0002d260: 5d28 6874 7470 733a 2f2f 646f 6373 2e70  ](https://docs.p
+0002d270: 7974 686f 6e2e 6f72 672f 332f 6c69 6272  ython.org/3/libr
+0002d280: 6172 792f 636f 6c6c 6563 7469 6f6e 732e  ary/collections.
+0002d290: 6162 632e 6874 6d6c 2920 7368 6f75 6c64  abc.html) should
+0002d2a0: 2062 6520 7075 7420 696e 2074 6865 2060   be put in the `
+0002d2b0: 5f5f 636f 7079 5f5f 6020 6d65 7468 6f64  __copy__` method
+0002d2c0: 2e20 4e6f 7465 2074 6861 7420 616c 6c20  . Note that all 
+0002d2d0: 5b53 6571 7565 6e63 6573 2f4d 6170 7069  [Sequences/Mappi
+0002d2e0: 6e67 732f 5365 7473 5d28 6874 7470 733a  ngs/Sets](https:
+0002d2f0: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
+0002d300: 672f 332f 6c69 6272 6172 792f 636f 6c6c  g/3/library/coll
+0002d310: 6563 7469 6f6e 732e 6162 632e 6874 6d6c  ections.abc.html
+0002d320: 2920 6172 6520 616c 7761 7973 2061 7373  ) are always ass
+0002d330: 756d 6564 2074 6f20 6265 2072 6569 7465  umed to be reite
+0002d340: 7261 626c 6520 6576 656e 2077 6974 686f  rable even witho
+0002d350: 7574 2063 616c 6c69 6e67 2060 5f5f 636f  ut calling `__co
+0002d360: 7079 5f5f 602e 0a0a 2323 2323 2320 5079  py__`...##### Py
+0002d370: 7468 6f6e 2044 6f63 730a 0a2a 2a74 6565  thon Docs..**tee
+0002d380: 2a2a 285f 6974 6572 6162 6c65 2c20 6e3d  **(_iterable, n=
+0002d390: 325f 290a 0a52 6574 7572 6e20 5f6e 5f20  2_)..Return _n_ 
+0002d3a0: 696e 6465 7065 6e64 656e 7420 6974 6572  independent iter
+0002d3b0: 6174 6f72 7320 6672 6f6d 2061 2073 696e  ators from a sin
+0002d3c0: 676c 6520 6974 6572 6162 6c65 2e20 4571  gle iterable. Eq
+0002d3d0: 7569 7661 6c65 6e74 2074 6f3a 0a60 6060  uivalent to:.```
+0002d3e0: 636f 636f 6e75 745f 7079 7468 6f6e 0a64  coconut_python.d
+0002d3f0: 6566 2074 6565 2869 7465 7261 626c 652c  ef tee(iterable,
+0002d400: 206e 3d32 293a 0a20 2020 2069 7420 3d20   n=2):.    it = 
+0002d410: 6974 6572 2869 7465 7261 626c 6529 0a20  iter(iterable). 
+0002d420: 2020 2064 6571 7565 7320 3d20 5b63 6f6c     deques = [col
+0002d430: 6c65 6374 696f 6e73 2e64 6571 7565 2829  lections.deque()
+0002d440: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+0002d450: 6e29 5d0a 2020 2020 6465 6620 6765 6e28  n)].    def gen(
+0002d460: 6d79 6465 7175 6529 3a0a 2020 2020 2020  mydeque):.      
+0002d470: 2020 7768 696c 6520 5472 7565 3a0a 2020    while True:.  
+0002d480: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0002d490: 206d 7964 6571 7565 3a20 2020 2020 2020   mydeque:       
+0002d4a0: 2020 2020 2020 2320 7768 656e 2074 6865        # when the
+0002d4b0: 206c 6f63 616c 2064 6571 7565 2069 7320   local deque is 
+0002d4c0: 656d 7074 790a 2020 2020 2020 2020 2020  empty.          
+0002d4d0: 2020 2020 2020 6e65 7776 616c 203d 206e        newval = n
+0002d4e0: 6578 7428 6974 2920 2020 2020 2020 2320  ext(it)       # 
+0002d4f0: 6665 7463 6820 6120 6e65 7720 7661 6c75  fetch a new valu
+0002d500: 6520 616e 640a 2020 2020 2020 2020 2020  e and.          
+0002d510: 2020 2020 2020 666f 7220 6420 696e 2064        for d in d
+0002d520: 6571 7565 733a 2020 2020 2020 2020 2320  eques:        # 
+0002d530: 6c6f 6164 2069 7420 746f 2061 6c6c 2074  load it to all t
+0002d540: 6865 2064 6571 7565 730a 2020 2020 2020  he deques.      
+0002d550: 2020 2020 2020 2020 2020 2020 2020 642e                d.
+0002d560: 6170 7065 6e64 286e 6577 7661 6c29 0a20  append(newval). 
+0002d570: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
+0002d580: 206d 7964 6571 7565 2e70 6f70 6c65 6674   mydeque.popleft
+0002d590: 2829 0a20 2020 2072 6574 7572 6e20 7475  ().    return tu
+0002d5a0: 706c 6528 6765 6e28 6429 2066 6f72 2064  ple(gen(d) for d
+0002d5b0: 2069 6e20 6465 7175 6573 290a 6060 600a   in deques).```.
+0002d5c0: 4f6e 6365 2060 7465 6528 2960 2068 6173  Once `tee()` has
+0002d5d0: 206d 6164 6520 6120 7370 6c69 742c 2074   made a split, t
+0002d5e0: 6865 206f 7269 6769 6e61 6c20 5f69 7465  he original _ite
+0002d5f0: 7261 626c 655f 2073 686f 756c 6420 6e6f  rable_ should no
+0002d600: 7420 6265 2075 7365 6420 616e 7977 6865  t be used anywhe
+0002d610: 7265 2065 6c73 653b 206f 7468 6572 7769  re else; otherwi
+0002d620: 7365 2c20 7468 6520 5f69 7465 7261 626c  se, the _iterabl
+0002d630: 655f 2063 6f75 6c64 2067 6574 2061 6476  e_ could get adv
+0002d640: 616e 6365 6420 7769 7468 6f75 7420 7468  anced without th
+0002d650: 6520 7465 6520 6f62 6a65 6374 7320 6265  e tee objects be
+0002d660: 696e 6720 696e 666f 726d 6564 2e0a 0a54  ing informed...T
+0002d670: 6869 7320 6974 6572 746f 6f6c 206d 6179  his itertool may
+0002d680: 2072 6571 7569 7265 2073 6967 6e69 6669   require signifi
+0002d690: 6361 6e74 2061 7578 696c 6961 7279 2073  cant auxiliary s
+0002d6a0: 746f 7261 6765 2028 6465 7065 6e64 696e  torage (dependin
+0002d6b0: 6720 6f6e 2068 6f77 206d 7563 6820 7465  g on how much te
+0002d6c0: 6d70 6f72 6172 7920 6461 7461 206e 6565  mporary data nee
+0002d6d0: 6473 2074 6f20 6265 2073 746f 7265 6429  ds to be stored)
+0002d6e0: 2e20 496e 2067 656e 6572 616c 2c20 6966  . In general, if
+0002d6f0: 206f 6e65 2069 7465 7261 746f 7220 7573   one iterator us
+0002d700: 6573 206d 6f73 7420 6f72 2061 6c6c 206f  es most or all o
+0002d710: 6620 7468 6520 6461 7461 2062 6566 6f72  f the data befor
+0002d720: 6520 616e 6f74 6865 7220 6974 6572 6174  e another iterat
+0002d730: 6f72 2073 7461 7274 732c 2069 7420 6973  or starts, it is
+0002d740: 2066 6173 7465 7220 746f 2075 7365 2060   faster to use `
+0002d750: 6c69 7374 2829 6020 696e 7374 6561 6420  list()` instead 
+0002d760: 6f66 2060 7465 6528 2960 2e0a 0a23 2323  of `tee()`...###
+0002d770: 2323 2045 7861 6d70 6c65 0a0a 2a2a 436f  ## Example..**Co
+0002d780: 636f 6e75 743a 2a2a 0a60 6060 636f 636f  conut:**.```coco
+0002d790: 6e75 740a 6f72 6967 696e 616c 2c20 7465  nut.original, te
+0002d7a0: 6d70 203d 2074 6565 286f 7269 6769 6e61  mp = tee(origina
+0002d7b0: 6c29 0a73 6c69 6365 6420 3d20 7465 6d70  l).sliced = temp
+0002d7c0: 245b 353a 5d0a 6060 600a 0a2a 2a50 7974  $[5:].```..**Pyt
+0002d7d0: 686f 6e3a 2a2a 0a60 6060 636f 636f 6e75  hon:**.```coconu
+0002d7e0: 745f 7079 7468 6f6e 0a69 6d70 6f72 7420  t_python.import 
+0002d7f0: 6974 6572 746f 6f6c 730a 6f72 6967 696e  itertools.origin
+0002d800: 616c 2c20 7465 6d70 203d 2069 7465 7274  al, temp = itert
+0002d810: 6f6f 6c73 2e74 6565 286f 7269 6769 6e61  ools.tee(origina
+0002d820: 6c29 0a73 6c69 6365 6420 3d20 6974 6572  l).sliced = iter
+0002d830: 746f 6f6c 732e 6973 6c69 6365 2874 656d  tools.islice(tem
+0002d840: 702c 2035 2c20 4e6f 6e65 290a 6060 600a  p, 5, None).```.
+0002d850: 0a23 2323 2320 6063 6f6e 7375 6d65 600a  .#### `consume`.
+0002d860: 0a2a 2a63 6f6e 7375 6d65 2a2a 285f 6974  .**consume**(_it
+0002d870: 6572 6162 6c65 5f2c 205f 6b65 6570 5c5f  erable_, _keep\_
+0002d880: 6c61 7374 5f3d 6030 6029 0a0a 436f 636f  last_=`0`)..Coco
+0002d890: 6e75 7420 7072 6f76 6964 6573 2074 6865  nut provides the
+0002d8a0: 2060 636f 6e73 756d 6560 2066 756e 6374   `consume` funct
+0002d8b0: 696f 6e20 746f 2065 6666 6963 6965 6e74  ion to efficient
+0002d8c0: 6c79 2065 7868 6175 7374 2061 6e20 6974  ly exhaust an it
+0002d8d0: 6572 6174 6f72 2061 6e64 2074 6875 7320  erator and thus 
+0002d8e0: 7065 7266 6f72 6d20 616e 7920 6c61 7a79  perform any lazy
+0002d8f0: 2065 7661 6c75 6174 696f 6e20 636f 6e74   evaluation cont
+0002d900: 6169 6e65 6420 7769 7468 696e 2069 742e  ained within it.
+0002d910: 2060 636f 6e73 756d 6560 2074 616b 6573   `consume` takes
+0002d920: 206f 6e65 206f 7074 696f 6e61 6c20 6172   one optional ar
+0002d930: 6775 6d65 6e74 2c20 606b 6565 705f 6c61  gument, `keep_la
+0002d940: 7374 602c 2074 6861 7420 6465 6661 756c  st`, that defaul
+0002d950: 7473 2074 6f20 3020 616e 6420 7370 6563  ts to 0 and spec
+0002d960: 6966 6965 7320 686f 7720 6d61 6e79 2c20  ifies how many, 
+0002d970: 6966 2061 6e79 2c20 6974 656d 7320 6672  if any, items fr
+0002d980: 6f6d 2074 6865 2065 6e64 2074 6f20 7265  om the end to re
+0002d990: 7475 726e 2061 7320 6120 7365 7175 656e  turn as a sequen
+0002d9a0: 6365 2028 604e 6f6e 6560 2077 696c 6c20  ce (`None` will 
+0002d9b0: 6b65 6570 2061 6c6c 2065 6c65 6d65 6e74  keep all element
+0002d9c0: 7329 2e0a 0a45 7175 6976 616c 656e 7420  s)...Equivalent 
+0002d9d0: 746f 3a0a 6060 6063 6f63 6f6e 7574 0a64  to:.```coconut.d
+0002d9e0: 6566 2063 6f6e 7375 6d65 2869 7465 7261  ef consume(itera
+0002d9f0: 626c 652c 206b 6565 705f 6c61 7374 3d30  ble, keep_last=0
+0002da00: 293a 0a20 2020 2022 2222 4675 6c6c 7920  ):.    """Fully 
+0002da10: 6578 6861 7573 7420 6974 6572 6162 6c65  exhaust iterable
+0002da20: 2061 6e64 2072 6574 7572 6e20 7468 6520   and return the 
+0002da30: 6c61 7374 206b 6565 705f 6c61 7374 2065  last keep_last e
+0002da40: 6c65 6d65 6e74 732e 2222 220a 2020 2020  lements.""".    
+0002da50: 7265 7475 726e 2063 6f6c 6c65 6374 696f  return collectio
+0002da60: 6e73 2e64 6571 7565 2869 7465 7261 626c  ns.deque(iterabl
+0002da70: 652c 206d 6178 6c65 6e3d 6b65 6570 5f6c  e, maxlen=keep_l
+0002da80: 6173 7429 2020 2320 6661 7374 6573 7420  ast)  # fastest 
+0002da90: 7761 7920 746f 2065 7868 6175 7374 2061  way to exhaust a
+0002daa0: 6e20 6974 6572 6174 6f72 0a60 6060 0a0a  n iterator.```..
+0002dab0: 2323 2323 2320 5261 7469 6f6e 616c 650a  ##### Rationale.
+0002dac0: 0a49 6e20 7468 6520 7072 6f63 6573 7320  .In the process 
+0002dad0: 6f66 206c 617a 696c 7920 6170 706c 7969  of lazily applyi
+0002dae0: 6e67 206f 7065 7261 7469 6f6e 7320 746f  ng operations to
+0002daf0: 2069 7465 7261 746f 7273 2c20 6576 656e   iterators, even
+0002db00: 7475 616c 6c79 2061 2070 6f69 6e74 2069  tually a point i
+0002db10: 7320 7265 6163 6865 6420 7768 6572 6520  s reached where 
+0002db20: 6576 616c 7561 7469 6f6e 206f 6620 7468  evaluation of th
+0002db30: 6520 6974 6572 6174 6f72 2069 7320 6e65  e iterator is ne
+0002db40: 6365 7373 6172 792e 2054 6f20 646f 2074  cessary. To do t
+0002db50: 6869 7320 6566 6669 6369 656e 746c 792c  his efficiently,
+0002db60: 2043 6f63 6f6e 7574 2070 726f 7669 6465   Coconut provide
+0002db70: 7320 7468 6520 6063 6f6e 7375 6d65 6020  s the `consume` 
+0002db80: 6675 6e63 7469 6f6e 2c20 7768 6963 6820  function, which 
+0002db90: 7769 6c6c 2066 756c 6c79 2065 7868 6175  will fully exhau
+0002dba0: 7374 2074 6865 2069 7465 7261 746f 7220  st the iterator 
+0002dbb0: 6769 7665 6e20 746f 2069 742e 0a0a 2323  given to it...##
+0002dbc0: 2323 2320 4578 616d 706c 650a 0a2a 2a43  ### Example..**C
+0002dbd0: 6f63 6f6e 7574 3a2a 2a0a 6060 6063 6f63  oconut:**.```coc
+0002dbe0: 6f6e 7574 0a72 616e 6765 2831 3029 207c  onut.range(10) |
+0002dbf0: 3e20 6d61 7024 2828 7829 202d 3e20 782a  > map$((x) -> x*
+0002dc00: 2a32 2920 7c3e 206d 6170 2428 7072 696e  *2) |> map$(prin
+0002dc10: 7429 207c 3e20 636f 6e73 756d 650a 6060  t) |> consume.``
+0002dc20: 600a 0a2a 2a50 7974 686f 6e3a 2a2a 0a60  `..**Python:**.`
+0002dc30: 6060 636f 636f 6e75 745f 7079 7468 6f6e  ``coconut_python
+0002dc40: 0a63 6f6c 6c65 6374 696f 6e73 2e64 6571  .collections.deq
+0002dc50: 7565 286d 6170 2870 7269 6e74 2c20 6d61  ue(map(print, ma
+0002dc60: 7028 6c61 6d62 6461 2078 3a20 782a 2a32  p(lambda x: x**2
+0002dc70: 2c20 7261 6e67 6528 3130 2929 292c 206d  , range(10))), m
+0002dc80: 6178 6c65 6e3d 3029 0a60 6060 0a0a 2323  axlen=0).```..##
+0002dc90: 2320 5479 7069 6e67 2d53 7065 6369 6669  # Typing-Specifi
+0002dca0: 6320 4275 696c 742d 496e 730a 0a60 6060  c Built-Ins..```
+0002dcb0: 7b63 6f6e 7465 6e74 737d 0a2d 2d2d 0a6c  {contents}.---.l
+0002dcc0: 6f63 616c 3a0a 6465 7074 683a 2031 0a2d  ocal:.depth: 1.-
+0002dcd0: 2d2d 0a60 6060 0a0a 2323 2323 2060 5459  --.```..#### `TY
+0002dce0: 5045 5f43 4845 434b 494e 4760 0a0a 5468  PE_CHECKING`..Th
+0002dcf0: 6520 6054 5950 455f 4348 4543 4b49 4e47  e `TYPE_CHECKING
+0002dd00: 6020 7661 7269 6162 6c65 2069 7320 7365  ` variable is se
+0002dd10: 7420 746f 2060 4661 6c73 6560 2061 7420  t to `False` at 
+0002dd20: 7275 6e74 696d 6520 616e 6420 6054 7275  runtime and `Tru
+0002dd30: 6560 2064 7572 696e 6720 7479 7065 5f63  e` during type_c
+0002dd40: 6865 636b 696e 672c 2061 6c6c 6f77 696e  hecking, allowin
+0002dd50: 6720 796f 7520 746f 2070 7265 7665 6e74  g you to prevent
+0002dd60: 2079 6f75 7220 6074 7970 696e 6760 2069   your `typing` i
+0002dd70: 6d70 6f72 7473 2061 6e64 2060 5479 7065  mports and `Type
+0002dd80: 5661 7260 2064 6566 696e 6974 696f 6e73  Var` definitions
+0002dd90: 2066 726f 6d20 6265 696e 6720 6578 6563   from being exec
+0002dda0: 7574 6564 2061 7420 7275 6e74 696d 652e  uted at runtime.
+0002ddb0: 2042 7920 7772 6170 7069 6e67 2079 6f75   By wrapping you
+0002ddc0: 7220 6074 7970 696e 6760 2069 6d70 6f72  r `typing` impor
+0002ddd0: 7473 2069 6e20 616e 2060 6966 2054 5950  ts in an `if TYP
+0002dde0: 455f 4348 4543 4b49 4e47 3a60 2062 6c6f  E_CHECKING:` blo
+0002ddf0: 636b 2c20 796f 7520 6361 6e20 6576 656e  ck, you can even
+0002de00: 2075 7365 2074 6865 205b 6074 7970 696e   use the [`typin
+0002de10: 6760 5d28 6874 7470 733a 2f2f 646f 6373  g`](https://docs
+0002de20: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
+0002de30: 6272 6172 792f 7479 7069 6e67 2e68 746d  brary/typing.htm
+0002de40: 6c29 206d 6f64 756c 6520 6f6e 2050 7974  l) module on Pyt
+0002de50: 686f 6e20 7665 7273 696f 6e73 2074 6861  hon versions tha
+0002de60: 7420 646f 6e27 7420 6e61 7469 7665 6c79  t don't natively
+0002de70: 2073 7570 706f 7274 2069 742e 2046 7572   support it. Fur
+0002de80: 7468 6572 6d6f 7265 2c20 6054 5950 455f  thermore, `TYPE_
+0002de90: 4348 4543 4b49 4e47 6020 6361 6e20 616c  CHECKING` can al
+0002dea0: 736f 2062 6520 7573 6564 2074 6f20 6869  so be used to hi
+0002deb0: 6465 2063 6f64 6520 7468 6174 2069 7320  de code that is 
+0002dec0: 6d69 7374 7970 6564 2062 7920 6465 6661  mistyped by defa
+0002ded0: 756c 742e 0a0a 2323 2323 2320 5079 7468  ult...##### Pyth
+0002dee0: 6f6e 2044 6f63 730a 0a41 2073 7065 6369  on Docs..A speci
+0002def0: 616c 2063 6f6e 7374 616e 7420 7468 6174  al constant that
+0002df00: 2069 7320 6173 7375 6d65 6420 746f 2062   is assumed to b
+0002df10: 6520 6054 7275 6560 2062 7920 3372 6420  e `True` by 3rd 
+0002df20: 7061 7274 7920 7374 6174 6963 2074 7970  party static typ
+0002df30: 6520 6368 6563 6b65 7273 2e20 4974 2069  e checkers. It i
+0002df40: 7320 6046 616c 7365 6020 6174 2072 756e  s `False` at run
+0002df50: 7469 6d65 2e20 5573 6167 653a 0a60 6060  time. Usage:.```
+0002df60: 636f 636f 6e75 745f 7079 7468 6f6e 0a69  coconut_python.i
+0002df70: 6620 5459 5045 5f43 4845 434b 494e 473a  f TYPE_CHECKING:
+0002df80: 0a20 2020 2069 6d70 6f72 7420 6578 7065  .    import expe
+0002df90: 6e73 6976 655f 6d6f 640a 0a64 6566 2066  nsive_mod..def f
+0002dfa0: 756e 2861 7267 3a20 6578 7065 6e73 6976  un(arg: expensiv
+0002dfb0: 655f 6d6f 642e 536f 6d65 5479 7065 2920  e_mod.SomeType) 
+0002dfc0: 2d3e 204e 6f6e 653a 0a20 2020 206c 6f63  -> None:.    loc
+0002dfd0: 616c 5f76 6172 3a20 6578 7065 6e73 6976  al_var: expensiv
+0002dfe0: 655f 6d6f 642e 416e 6f74 6865 7254 7970  e_mod.AnotherTyp
+0002dff0: 6520 3d20 6f74 6865 725f 6675 6e28 290a  e = other_fun().
+0002e000: 6060 600a 0a23 2323 2323 2045 7861 6d70  ```..##### Examp
+0002e010: 6c65 730a 0a2a 2a43 6f63 6f6e 7574 3a2a  les..**Coconut:*
+0002e020: 2a0a 6060 6063 6f63 6f6e 7574 0a69 6620  *.```coconut.if 
+0002e030: 5459 5045 5f43 4845 434b 494e 473a 0a20  TYPE_CHECKING:. 
+0002e040: 2020 2066 726f 6d20 7479 7069 6e67 2069     from typing i
+0002e050: 6d70 6f72 7420 4c69 7374 0a78 3a20 4c69  mport List.x: Li
+0002e060: 7374 5b73 7472 5d20 3d20 5b22 6122 2c20  st[str] = ["a", 
+0002e070: 2262 225d 0a60 6060 0a0a 6060 6063 6f63  "b"].```..```coc
+0002e080: 6f6e 7574 0a69 6620 5459 5045 5f43 4845  onut.if TYPE_CHE
+0002e090: 434b 494e 473a 0a20 2020 2064 6566 2066  CKING:.    def f
+0002e0a0: 6163 746f 7269 616c 286e 3a20 696e 7429  actorial(n: int)
+0002e0b0: 202d 3e20 696e 743a 202e 2e2e 0a65 6c73   -> int: ....els
+0002e0c0: 653a 0a20 2020 2064 6566 2066 6163 746f  e:.    def facto
+0002e0d0: 7269 616c 2830 2920 3d20 310a 2020 2020  rial(0) = 1.    
+0002e0e0: 6164 6470 6174 7465 726e 2064 6566 2066  addpattern def f
+0002e0f0: 6163 746f 7269 616c 286e 2920 3d20 6e20  actorial(n) = n 
+0002e100: 2a20 6661 6374 6f72 6961 6c28 6e2d 3129  * factorial(n-1)
+0002e110: 0a60 6060 0a0a 2a2a 5079 7468 6f6e 3a2a  .```..**Python:*
+0002e120: 2a0a 6060 6063 6f63 6f6e 7574 5f70 7974  *.```coconut_pyt
+0002e130: 686f 6e0a 7472 793a 0a20 2020 2066 726f  hon.try:.    fro
+0002e140: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+0002e150: 5459 5045 5f43 4845 434b 494e 470a 6578  TYPE_CHECKING.ex
+0002e160: 6365 7074 2049 6d70 6f72 7445 7272 6f72  cept ImportError
+0002e170: 3a0a 2020 2020 5459 5045 5f43 4845 434b  :.    TYPE_CHECK
+0002e180: 494e 4720 3d20 4661 6c73 650a 0a69 6620  ING = False..if 
+0002e190: 5459 5045 5f43 4845 434b 494e 473a 0a20  TYPE_CHECKING:. 
+0002e1a0: 2020 2066 726f 6d20 7479 7069 6e67 2069     from typing i
+0002e1b0: 6d70 6f72 7420 4c69 7374 0a78 3a20 4c69  mport List.x: Li
+0002e1c0: 7374 5b73 7472 5d20 3d20 5b22 6122 2c20  st[str] = ["a", 
+0002e1d0: 2262 225d 0a60 6060 0a0a 6060 6063 6f63  "b"].```..```coc
+0002e1e0: 6f6e 7574 5f70 7974 686f 6e0a 7472 793a  onut_python.try:
+0002e1f0: 0a20 2020 2066 726f 6d20 7479 7069 6e67  .    from typing
+0002e200: 2069 6d70 6f72 7420 5459 5045 5f43 4845   import TYPE_CHE
+0002e210: 434b 494e 470a 6578 6365 7074 2049 6d70  CKING.except Imp
+0002e220: 6f72 7445 7272 6f72 3a0a 2020 2020 5459  ortError:.    TY
+0002e230: 5045 5f43 4845 434b 494e 4720 3d20 4661  PE_CHECKING = Fa
+0002e240: 6c73 650a 0a69 6620 5459 5045 5f43 4845  lse..if TYPE_CHE
+0002e250: 434b 494e 473a 0a20 2020 2064 6566 2066  CKING:.    def f
+0002e260: 6163 746f 7269 616c 286e 3a20 696e 7429  actorial(n: int)
+0002e270: 202d 3e20 696e 743a 202e 2e2e 0a65 6c73   -> int: ....els
+0002e280: 653a 0a20 2020 2064 6566 2066 6163 746f  e:.    def facto
+0002e290: 7269 616c 286e 293a 0a20 2020 2020 2020  rial(n):.       
+0002e2a0: 2069 6620 6e20 3d3d 2030 3a0a 2020 2020   if n == 0:.    
+0002e2b0: 2020 2020 2020 2020 7265 7475 726e 2031          return 1
+0002e2c0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0002e2d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0002e2e0: 6e20 6e20 2a20 6661 6374 6f72 6961 6c28  n n * factorial(
+0002e2f0: 6e2d 3129 0a60 6060 0a0a 2323 2323 2060  n-1).```..#### `
+0002e300: 7265 7665 616c 5f74 7970 6560 2061 6e64  reveal_type` and
+0002e310: 2060 7265 7665 616c 5f6c 6f63 616c 7360   `reveal_locals`
+0002e320: 0a0a 5768 656e 2075 7369 6e67 204d 7950  ..When using MyP
+0002e330: 792c 2060 7265 7665 616c 5f74 7970 6528  y, `reveal_type(
+0002e340: 3c65 7870 723e 2960 2077 696c 6c20 6361  <expr>)` will ca
+0002e350: 7573 6520 4d79 5079 2074 6f20 7072 696e  use MyPy to prin
+0002e360: 7420 7468 6520 7479 7065 206f 6620 603c  t the type of `<
+0002e370: 6578 7072 3e60 2061 6e64 2060 7265 7665  expr>` and `reve
+0002e380: 616c 5f6c 6f63 616c 7328 2960 2077 696c  al_locals()` wil
+0002e390: 6c20 6361 7573 6520 4d79 5079 2074 6f20  l cause MyPy to 
+0002e3a0: 7072 696e 7420 7468 6520 7479 7065 7320  print the types 
+0002e3b0: 6f66 2074 6865 2063 7572 7265 6e74 2060  of the current `
+0002e3c0: 6c6f 6361 6c73 2829 602e 2041 7420 7275  locals()`. At ru
+0002e3d0: 6e74 696d 652c 2060 7265 7665 616c 5f74  ntime, `reveal_t
+0002e3e0: 7970 6528 7829 6020 6973 2061 6c77 6179  ype(x)` is alway
+0002e3f0: 7320 7468 6520 6964 656e 7469 7479 2066  s the identity f
+0002e400: 756e 6374 696f 6e20 616e 6420 6072 6576  unction and `rev
+0002e410: 6561 6c5f 6c6f 6361 6c73 2829 6020 616c  eal_locals()` al
+0002e420: 7761 7973 2072 6574 7572 6e73 2060 4e6f  ways returns `No
+0002e430: 6e65 602e 2053 6565 205b 7468 6520 4d79  ne`. See [the My
+0002e440: 5079 2064 6f63 756d 656e 7461 7469 6f6e  Py documentation
+0002e450: 5d28 6874 7470 733a 2f2f 6d79 7079 2e72  ](https://mypy.r
+0002e460: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+0002e470: 2f73 7461 626c 652f 636f 6d6d 6f6e 5f69  /stable/common_i
+0002e480: 7373 7565 732e 6874 6d6c 2372 6576 6561  ssues.html#revea
+0002e490: 6c2d 7479 7065 2920 666f 7220 6d6f 7265  l-type) for more
+0002e4a0: 2069 6e66 6f72 6d61 7469 6f6e 2e0a 0a23   information...#
+0002e4b0: 2323 2323 2045 7861 6d70 6c65 0a0a 2a2a  #### Example..**
+0002e4c0: 436f 636f 6e75 743a 2a2a 0a60 6060 636f  Coconut:**.```co
+0002e4d0: 636f 6e75 745f 7079 636f 6e0a 3e20 636f  conut_pycon.> co
+0002e4e0: 636f 6e75 7420 2d2d 6d79 7079 0a43 6f63  conut --mypy.Coc
+0002e4f0: 6f6e 7574 2049 6e74 6572 7072 6574 6572  onut Interpreter
+0002e500: 2076 582e 582e 583a 0a28 656e 7465 7220   vX.X.X:.(enter 
+0002e510: 2765 7869 7428 2927 206f 7220 7072 6573  'exit()' or pres
+0002e520: 7320 4374 726c 2d44 2074 6f20 656e 6429  s Ctrl-D to end)
+0002e530: 0a3e 3e3e 2072 6576 6561 6c5f 7479 7065  .>>> reveal_type
+0002e540: 2866 6d61 7029 0a3c 6675 6e63 7469 6f6e  (fmap).<function
+0002e550: 2066 6d61 7020 6174 2030 7830 3030 3030   fmap at 0x00000
+0002e560: 3233 3942 3036 4532 3034 303e 0a3c 7374  239B06E2040>.<st
+0002e570: 7269 6e67 3e3a 3137 3a20 6e6f 7465 3a20  ring>:17: note: 
+0002e580: 5265 7665 616c 6564 2074 7970 6520 6973  Revealed type is
+0002e590: 2027 6465 6620 5b5f 542c 205f 555d 2028   'def [_T, _U] (
+0002e5a0: 6675 6e63 3a20 6465 6620 285f 5460 2d31  func: def (_T`-1
+0002e5b0: 2920 2d3e 205f 5560 2d32 2c20 6f62 6a3a  ) -> _U`-2, obj:
+0002e5c0: 2074 7970 696e 672e 4974 6572 6162 6c65   typing.Iterable
+0002e5d0: 5b5f 5460 2d31 5d29 202d 3e20 7479 7069  [_T`-1]) -> typi
+0002e5e0: 6e67 2e49 7465 7261 626c 655b 5f55 602d  ng.Iterable[_U`-
+0002e5f0: 325d 270a 3e3e 3e0a 6060 600a 0a2a 2a50  2]'.>>>.```..**P
+0002e600: 7974 686f 6e2a 2a0a 6060 6063 6f63 6f6e  ython**.```cocon
+0002e610: 7574 5f70 7974 686f 6e0a 7472 793a 0a20  ut_python.try:. 
+0002e620: 2020 2066 726f 6d20 7479 7069 6e67 2069     from typing i
+0002e630: 6d70 6f72 7420 5459 5045 5f43 4845 434b  mport TYPE_CHECK
+0002e640: 494e 470a 6578 6365 7074 2049 6d70 6f72  ING.except Impor
+0002e650: 7445 7272 6f72 3a0a 2020 2020 5459 5045  tError:.    TYPE
+0002e660: 5f43 4845 434b 494e 4720 3d20 4661 6c73  _CHECKING = Fals
+0002e670: 650a 0a69 6620 6e6f 7420 5459 5045 5f43  e..if not TYPE_C
+0002e680: 4845 434b 494e 473a 0a20 2020 2064 6566  HECKING:.    def
+0002e690: 2072 6576 6561 6c5f 7479 7065 2878 293a   reveal_type(x):
+0002e6a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002e6b0: 780a 0a66 726f 6d20 636f 636f 6e75 742e  x..from coconut.
+0002e6c0: 5f5f 636f 636f 6e75 745f 5f20 696d 706f  __coconut__ impo
+0002e6d0: 7274 2066 6d61 700a 7265 7665 616c 5f74  rt fmap.reveal_t
+0002e6e0: 7970 6528 666d 6170 290a 6060 600a 0a23  ype(fmap).```..#
+0002e6f0: 2320 436f 636f 6e75 7420 4150 490a 0a60  # Coconut API..`
+0002e700: 6060 7b63 6f6e 7465 6e74 737d 0a2d 2d2d  ``{contents}.---
+0002e710: 0a6c 6f63 616c 3a0a 6465 7074 683a 2032  .local:.depth: 2
+0002e720: 0a2d 2d2d 0a60 6060 0a0a 2323 2320 6063  .---.```..### `c
+0002e730: 6f63 6f6e 7574 2e65 6d62 6564 600a 0a2a  oconut.embed`..*
+0002e740: 2a63 6f63 6f6e 7574 2e65 6d62 6564 2a2a  *coconut.embed**
+0002e750: 285f 6b65 726e 656c 5f3d 604e 6f6e 6560  (_kernel_=`None`
+0002e760: 2c20 5f64 6570 7468 5f3d 6030 602c 205c  , _depth_=`0`, \
+0002e770: 2a5c 2a5f 6b77 6172 6773 5f29 0a0a 4966  *\*_kwargs_)..If
+0002e780: 205f 6b65 726e 656c 5f3d 6046 616c 7365   _kernel_=`False
+0002e790: 6020 2864 6566 6175 6c74 292c 2065 6d62  ` (default), emb
+0002e7a0: 6564 7320 6120 436f 636f 6e75 7420 4a75  eds a Coconut Ju
+0002e7b0: 7079 7465 7220 636f 6e73 6f6c 6520 696e  pyter console in
+0002e7c0: 6974 6961 6c69 7a65 6420 6672 6f6d 2074  itialized from t
+0002e7d0: 6865 2063 7572 7265 6e74 206c 6f63 616c  he current local
+0002e7e0: 206e 616d 6573 7061 6365 2e20 4966 205f   namespace. If _
+0002e7f0: 6b65 726e 656c 5f3d 6054 7275 6560 2c20  kernel_=`True`, 
+0002e800: 6c61 756e 6368 6573 2061 2043 6f63 6f6e  launches a Cocon
+0002e810: 7574 204a 7570 7974 6572 206b 6572 6e65  ut Jupyter kerne
+0002e820: 6c20 696e 6974 6961 6c69 7a65 6420 6672  l initialized fr
+0002e830: 6f6d 2074 6865 206c 6f63 616c 206e 616d  om the local nam
+0002e840: 6573 7061 6365 2074 6861 7420 6361 6e20  espace that can 
+0002e850: 7468 656e 2062 6520 6174 7461 6368 6564  then be attached
+0002e860: 2074 6f2e 2054 6865 205f 6465 7074 685f   to. The _depth_
+0002e870: 2069 6e64 6963 6174 6573 2068 6f77 206d   indicates how m
+0002e880: 616e 7920 6164 6469 7469 6f6e 616c 2063  any additional c
+0002e890: 616c 6c20 6672 616d 6573 2074 6f20 6967  all frames to ig
+0002e8a0: 6e6f 7265 2e20 5f6b 7761 7267 735f 2061  nore. _kwargs_ a
+0002e8b0: 7265 2061 7320 696e 205b 4950 7974 686f  re as in [IPytho
+0002e8c0: 6e2e 656d 6265 645d 2868 7474 7073 3a2f  n.embed](https:/
+0002e8d0: 2f69 7079 7468 6f6e 2e72 6561 6474 6865  /ipython.readthe
+0002e8e0: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
+0002e8f0: 652f 6170 692f 6765 6e65 7261 7465 642f  e/api/generated/
+0002e900: 4950 7974 686f 6e2e 7465 726d 696e 616c  IPython.terminal
+0002e910: 2e65 6d62 6564 2e68 746d 6c23 4950 7974  .embed.html#IPyt
+0002e920: 686f 6e2e 7465 726d 696e 616c 2e65 6d62  hon.terminal.emb
+0002e930: 6564 2e65 6d62 6564 2920 6f72 205b 4950  ed.embed) or [IP
+0002e940: 7974 686f 6e2e 656d 6265 645f 6b65 726e  ython.embed_kern
+0002e950: 656c 5d28 6874 7470 733a 2f2f 6970 7974  el](https://ipyt
+0002e960: 686f 6e2e 7265 6164 7468 6564 6f63 732e  hon.readthedocs.
+0002e970: 696f 2f65 6e2f 7374 6162 6c65 2f61 7069  io/en/stable/api
+0002e980: 2f67 656e 6572 6174 6564 2f49 5079 7468  /generated/IPyth
+0002e990: 6f6e 2e68 746d 6c23 4950 7974 686f 6e2e  on.html#IPython.
+0002e9a0: 656d 6265 645f 6b65 726e 656c 2920 6261  embed_kernel) ba
+0002e9b0: 7365 6420 6f6e 205f 6b65 726e 656c 5f2e  sed on _kernel_.
+0002e9c0: 0a0a 5265 636f 6d6d 656e 6465 6420 7573  ..Recommended us
+0002e9d0: 6167 6520 6973 2061 7320 6120 6465 6275  age is as a debu
+0002e9e0: 6767 696e 6720 746f 6f6c 2c20 7768 6572  gging tool, wher
+0002e9f0: 6520 7468 6520 636f 6465 2060 6672 6f6d  e the code `from
+0002ea00: 2063 6f63 6f6e 7574 2069 6d70 6f72 7420   coconut import 
+0002ea10: 656d 6265 643b 2065 6d62 6564 2829 6020  embed; embed()` 
+0002ea20: 6361 6e20 6265 2069 6e73 6572 7465 6420  can be inserted 
+0002ea30: 746f 206c 6175 6e63 6820 616e 2069 6e74  to launch an int
+0002ea40: 6572 6163 7469 7665 2043 6f63 6f6e 7574  eractive Coconut
+0002ea50: 2073 6865 6c6c 2069 6e69 7469 616c 697a   shell initializ
+0002ea60: 6564 2066 726f 6d20 7468 6174 2070 6f69  ed from that poi
+0002ea70: 6e74 2e0a 0a23 2323 2041 7574 6f6d 6174  nt...### Automat
+0002ea80: 6963 2043 6f6d 7069 6c61 7469 6f6e 0a0a  ic Compilation..
+0002ea90: 4966 2079 6f75 2064 6f6e 2774 2063 6172  If you don't car
+0002eaa0: 6520 6162 6f75 7420 7468 6520 6578 6163  e about the exac
+0002eab0: 7420 636f 6d70 696c 6174 696f 6e20 7061  t compilation pa
+0002eac0: 7261 6d65 7465 7273 2079 6f75 2077 616e  rameters you wan
+0002ead0: 7420 746f 2075 7365 2c20 6175 746f 6d61  t to use, automa
+0002eae0: 7469 6320 636f 6d70 696c 6174 696f 6e20  tic compilation 
+0002eaf0: 6c65 7473 2043 6f63 6f6e 7574 2074 616b  lets Coconut tak
+0002eb00: 6520 6361 7265 206f 6620 6576 6572 7974  e care of everyt
+0002eb10: 6869 6e67 2066 6f72 2079 6f75 2e20 4175  hing for you. Au
+0002eb20: 746f 6d61 7469 6320 636f 6d70 696c 6174  tomatic compilat
+0002eb30: 696f 6e20 6361 6e20 6265 2065 6e61 626c  ion can be enabl
+0002eb40: 6564 2065 6974 6865 7220 6279 2069 6d70  ed either by imp
+0002eb50: 6f72 7469 6e67 205b 6063 6f63 6f6e 7574  orting [`coconut
+0002eb60: 2e61 7069 605d 2823 636f 636f 6e75 742d  .api`](#coconut-
+0002eb70: 6170 6929 2062 6566 6f72 6520 796f 7520  api) before you 
+0002eb80: 696d 706f 7274 2061 6e79 7468 696e 6720  import anything 
+0002eb90: 656c 7365 2c20 6f72 2062 7920 7275 6e6e  else, or by runn
+0002eba0: 696e 6720 6063 6f63 6f6e 7574 202d 2d73  ing `coconut --s
+0002ebb0: 6974 652d 696e 7374 616c 6c60 2e20 4f6e  ite-install`. On
+0002ebc0: 6365 2061 7574 6f6d 6174 6963 2063 6f6d  ce automatic com
+0002ebd0: 7069 6c61 7469 6f6e 2069 7320 656e 6162  pilation is enab
+0002ebe0: 6c65 642c 2043 6f63 6f6e 7574 2077 696c  led, Coconut wil
+0002ebf0: 6c20 6368 6563 6b20 6561 6368 206f 6620  l check each of 
+0002ec00: 796f 7572 2069 6d70 6f72 7473 2074 6f20  your imports to 
+0002ec10: 7365 6520 6966 2079 6f75 2061 7265 2061  see if you are a
+0002ec20: 7474 656d 7074 696e 6720 746f 2069 6d70  ttempting to imp
+0002ec30: 6f72 7420 6120 602e 636f 636f 6020 6669  ort a `.coco` fi
+0002ec40: 6c65 2061 6e64 2c20 6966 2073 6f2c 2061  le and, if so, a
+0002ec50: 7574 6f6d 6174 6963 616c 6c79 2063 6f6d  utomatically com
+0002ec60: 7069 6c65 2069 7420 666f 7220 796f 752e  pile it for you.
+0002ec70: 204e 6f74 6520 7468 6174 2c20 666f 7220   Note that, for 
+0002ec80: 436f 636f 6e75 7420 746f 206b 6e6f 7720  Coconut to know 
+0002ec90: 7768 6174 2066 696c 6520 796f 7520 6172  what file you ar
+0002eca0: 6520 7472 7969 6e67 2074 6f20 696d 706f  e trying to impo
+0002ecb0: 7274 2c20 6974 2077 696c 6c20 6e65 6564  rt, it will need
+0002ecc0: 2074 6f20 6265 2061 6363 6573 7369 626c   to be accessibl
+0002ecd0: 6520 7669 6120 6073 7973 2e70 6174 6860  e via `sys.path`
+0002ece0: 2c20 6a75 7374 206c 696b 6520 6120 6e6f  , just like a no
+0002ecf0: 726d 616c 2069 6d70 6f72 742e 0a0a 4175  rmal import...Au
+0002ed00: 746f 6d61 7469 6320 636f 6d70 696c 6174  tomatic compilat
+0002ed10: 696f 6e20 616c 7761 7973 2063 6f6d 7069  ion always compi
+0002ed20: 6c65 7320 6d6f 6475 6c65 7320 616e 6420  les modules and 
+0002ed30: 7061 636b 6167 6573 2069 6e2d 706c 6163  packages in-plac
+0002ed40: 652c 2061 6e64 2061 6c77 6179 7320 7573  e, and always us
+0002ed50: 6573 2060 2d2d 7461 7267 6574 2073 7973  es `--target sys
+0002ed60: 602e 2041 7574 6f6d 6174 6963 2063 6f6d  `. Automatic com
+0002ed70: 7069 6c61 7469 6f6e 2069 7320 616c 7761  pilation is alwa
+0002ed80: 7973 2061 7661 696c 6162 6c65 2069 6e20  ys available in 
+0002ed90: 7468 6520 436f 636f 6e75 7420 696e 7465  the Coconut inte
+0002eda0: 7270 7265 7465 722c 2061 6e64 2c20 6966  rpreter, and, if
+0002edb0: 2075 7369 6e67 2074 6865 2043 6f63 6f6e   using the Cocon
+0002edc0: 7574 2069 6e74 6572 7072 6574 6572 2c20  ut interpreter, 
+0002edd0: 6120 6072 656c 6f61 6460 2062 7569 6c74  a `reload` built
+0002ede0: 2d69 6e20 6973 2070 726f 7669 6465 6420  -in is provided 
+0002edf0: 746f 2065 6173 696c 7920 7265 6c6f 6164  to easily reload
+0002ee00: 2069 6d70 6f72 7465 6420 6d6f 6475 6c65   imported module
+0002ee10: 732e 2041 6464 6974 696f 6e61 6c6c 792c  s. Additionally,
+0002ee20: 2074 6865 2069 6e74 6572 7072 6574 6572   the interpreter
+0002ee30: 2061 6c77 6179 7320 616c 6c6f 7773 2069   always allows i
+0002ee40: 6d70 6f72 7469 6e67 2066 726f 6d20 7468  mporting from th
+0002ee50: 6520 6375 7272 656e 7420 776f 726b 696e  e current workin
+0002ee60: 6720 6469 7265 6374 6f72 792c 206c 6574  g directory, let
+0002ee70: 7469 6e67 2079 6f75 2065 6173 696c 7920  ting you easily 
+0002ee80: 636f 6d70 696c 6520 616e 6420 706c 6179  compile and play
+0002ee90: 2061 726f 756e 6420 7769 7468 2061 2060   around with a `
+0002eea0: 2e63 6f63 6f60 2066 696c 6520 7369 6d70  .coco` file simp
+0002eeb0: 6c79 2062 7920 7275 6e6e 696e 6720 7468  ly by running th
+0002eec0: 6520 436f 636f 6e75 7420 696e 7465 7270  e Coconut interp
+0002eed0: 7265 7465 7220 616e 6420 696d 706f 7274  reter and import
+0002eee0: 696e 6720 6974 2e0a 0a23 2323 2043 6f63  ing it...### Coc
+0002eef0: 6f6e 7574 2045 6e63 6f64 696e 670a 0a57  onut Encoding..W
+0002ef00: 6869 6c65 2061 7574 6f6d 6174 6963 2063  hile automatic c
+0002ef10: 6f6d 7069 6c61 7469 6f6e 2069 7320 7468  ompilation is th
+0002ef20: 6520 7072 6566 6572 7265 6420 6d65 7468  e preferred meth
+0002ef30: 6f64 2066 6f72 2064 796e 616d 6963 616c  od for dynamical
+0002ef40: 6c79 2063 6f6d 7069 6c69 6e67 2043 6f63  ly compiling Coc
+0002ef50: 6f6e 7574 2066 696c 6573 2c20 6173 2069  onut files, as i
+0002ef60: 7420 6361 6368 6573 2074 6865 2063 6f6d  t caches the com
+0002ef70: 7069 6c65 6420 636f 6465 2061 7320 6120  piled code as a 
+0002ef80: 602e 7079 6020 6669 6c65 2074 6f20 7072  `.py` file to pr
+0002ef90: 6576 656e 7420 7265 636f 6d70 696c 6174  event recompilat
+0002efa0: 696f 6e2c 2043 6f63 6f6e 7574 2061 6c73  ion, Coconut als
+0002efb0: 6f20 7375 7070 6f72 7473 2061 2073 7065  o supports a spe
+0002efc0: 6369 616c 0a60 6060 636f 636f 6e75 740a  cial.```coconut.
+0002efd0: 2320 636f 6469 6e67 3a20 636f 636f 6e75  # coding: coconu
+0002efe0: 740a 6060 600a 6465 636c 6172 6174 696f  t.```.declaratio
+0002eff0: 6e20 7768 6963 6820 6361 6e20 6265 2061  n which can be a
+0002f000: 6464 6564 2074 6f20 602e 7079 6020 6669  dded to `.py` fi
+0002f010: 6c65 7320 746f 2068 6176 6520 7468 656d  les to have them
+0002f020: 2074 7265 6174 6564 2061 7320 436f 636f   treated as Coco
+0002f030: 6e75 7420 6669 6c65 7320 696e 7374 6561  nut files instea
+0002f040: 642e 2054 6f20 7573 6520 7375 6368 2061  d. To use such a
+0002f050: 2063 6f64 696e 6720 6465 636c 6172 6174   coding declarat
+0002f060: 696f 6e2c 2079 6f75 276c 6c20 6e65 6564  ion, you'll need
+0002f070: 2074 6f20 6569 7468 6572 2072 756e 2060   to either run `
+0002f080: 636f 636f 6e75 7420 2d2d 7369 7465 2d69  coconut --site-i
+0002f090: 6e73 7461 6c6c 6020 6f72 2060 696d 706f  nstall` or `impo
+0002f0a0: 7274 2063 6f63 6f6e 7574 2e61 7069 6020  rt coconut.api` 
+0002f0b0: 6174 2073 6f6d 6520 706f 696e 7420 6265  at some point be
+0002f0c0: 666f 7265 2079 6f75 2066 6972 7374 2061  fore you first a
+0002f0d0: 7474 656d 7074 2074 6f20 696d 706f 7274  ttempt to import
+0002f0e0: 2061 2066 696c 6520 7769 7468 2061 2060   a file with a `
+0002f0f0: 2320 636f 6469 6e67 3a20 636f 636f 6e75  # coding: coconu
+0002f100: 7460 2064 6563 6c61 7261 7469 6f6e 2e20  t` declaration. 
+0002f110: 4c69 6b65 2061 7574 6f6d 6174 6963 2063  Like automatic c
+0002f120: 6f6d 7069 6c61 7469 6f6e 2c20 636f 6d70  ompilation, comp
+0002f130: 696c 6174 696f 6e20 6973 2061 6c77 6179  ilation is alway
+0002f140: 7320 646f 6e65 2077 6974 6820 602d 2d74  s done with `--t
+0002f150: 6172 6765 7420 7379 7360 2061 6e64 2069  arget sys` and i
+0002f160: 7320 616c 7761 7973 2061 7661 696c 6162  s always availab
+0002f170: 6c65 2066 726f 6d20 7468 6520 436f 636f  le from the Coco
+0002f180: 6e75 7420 696e 7465 7270 7265 7465 722e  nut interpreter.
+0002f190: 0a0a 2323 2320 6063 6f63 6f6e 7574 2e61  ..### `coconut.a
+0002f1a0: 7069 600a 0a49 6e20 6164 6469 7469 6f6e  pi`..In addition
+0002f1b0: 2074 6f20 656e 6162 6c69 6e67 2061 7574   to enabling aut
+0002f1c0: 6f6d 6174 6963 2063 6f6d 7069 6c61 7469  omatic compilati
+0002f1d0: 6f6e 2c20 6063 6f63 6f6e 7574 2e61 7069  on, `coconut.api
+0002f1e0: 6020 6361 6e20 616c 736f 2062 6520 7573  ` can also be us
+0002f1f0: 6564 2074 6f20 6361 6c6c 2074 6865 2043  ed to call the C
+0002f200: 6f63 6f6e 7574 2063 6f6d 7069 6c65 7220  oconut compiler 
+0002f210: 6672 6f6d 2063 6f64 6520 696e 7374 6561  from code instea
+0002f220: 6420 6f66 2066 726f 6d20 7468 6520 636f  d of from the co
+0002f230: 6d6d 616e 6420 6c69 6e65 2e20 5365 6520  mmand line. See 
+0002f240: 6265 6c6f 7720 666f 7220 7370 6563 6966  below for specif
+0002f250: 6963 6174 696f 6e73 206f 6620 7468 6520  ications of the 
+0002f260: 6469 6666 6572 656e 7420 6170 6920 6675  different api fu
+0002f270: 6e63 7469 6f6e 732e 0a0a 5f44 4550 5245  nctions..._DEPRE
+0002f280: 4341 5445 443a 2060 636f 636f 6e75 742e  CATED: `coconut.
+0002f290: 636f 6e76 656e 6965 6e63 6560 2069 7320  convenience` is 
+0002f2a0: 6120 6465 7072 6563 6174 6564 2061 6c69  a deprecated ali
+0002f2b0: 6173 2066 6f72 2060 636f 636f 6e75 742e  as for `coconut.
+0002f2c0: 6170 6960 2e5f 0a0a 2323 2323 2060 6765  api`._..#### `ge
+0002f2d0: 745f 7374 6174 6560 0a0a 2a2a 636f 636f  t_state`..**coco
+0002f2e0: 6e75 742e 6170 692e 6765 745c 5f73 7461  nut.api.get\_sta
+0002f2f0: 7465 2a2a 285f 7374 6174 655f 3d60 4e6f  te**(_state_=`No
+0002f300: 6e65 6029 0a0a 4765 7473 2061 2073 7461  ne`)..Gets a sta
+0002f310: 7465 206f 626a 6563 7420 7768 6963 6820  te object which 
+0002f320: 7374 6f72 6573 2074 6865 2063 7572 7265  stores the curre
+0002f330: 6e74 2063 6f6d 7069 6c61 7469 6f6e 2070  nt compilation p
+0002f340: 6172 616d 6574 6572 732e 2053 7461 7465  arameters. State
+0002f350: 206f 626a 6563 7473 2063 616e 2062 6520   objects can be 
+0002f360: 636f 6e66 6967 7572 6564 2077 6974 6820  configured with 
+0002f370: 5b2a 2a73 6574 7570 2a2a 5d28 2373 6574  [**setup**](#set
+0002f380: 7570 2920 6f72 205b 2a2a 636d 642a 2a5d  up) or [**cmd**]
+0002f390: 2823 636d 6429 2061 6e64 2074 6865 6e20  (#cmd) and then 
+0002f3a0: 7573 6564 2069 6e20 5b2a 2a70 6172 7365  used in [**parse
+0002f3b0: 2a2a 5d28 2370 6172 7365 2920 6f72 205b  **](#parse) or [
+0002f3c0: 2a2a 636f 636f 6e75 745c 5f65 7661 6c2a  **coconut\_eval*
+0002f3d0: 2a5d 2823 636f 636f 6e75 745f 6576 616c  *](#coconut_eval
+0002f3e0: 292e 0a0a 4966 205f 7374 6174 655f 2069  )...If _state_ i
+0002f3f0: 7320 604e 6f6e 6560 2c20 6765 7473 2061  s `None`, gets a
+0002f400: 206e 6577 2073 7461 7465 206f 626a 6563   new state objec
+0002f410: 742c 2077 6865 7265 6173 2069 6620 5f73  t, whereas if _s
+0002f420: 7461 7465 5f20 6973 2060 4661 6c73 6560  tate_ is `False`
+0002f430: 2c20 7468 6520 676c 6f62 616c 2073 7461  , the global sta
+0002f440: 7465 206f 626a 6563 7420 6973 2072 6574  te object is ret
+0002f450: 7572 6e65 642e 0a0a 2323 2323 2060 7061  urned...#### `pa
+0002f460: 7273 6560 0a0a 2a2a 636f 636f 6e75 742e  rse`..**coconut.
+0002f470: 6170 692e 7061 7273 652a 2a28 5f63 6f64  api.parse**(_cod
+0002f480: 655f 3d60 2222 602c 205f 6d6f 6465 5f3d  e_=`""`, _mode_=
+0002f490: 6022 7379 7322 602c 205f 7374 6174 655f  `"sys"`, _state_
+0002f4a0: 3d60 4661 6c73 6560 2c20 5f6b 6565 705c  =`False`, _keep\
+0002f4b0: 5f69 6e74 6572 6e61 6c5c 5f73 7461 7465  _internal\_state
+0002f4c0: 5f3d 604e 6f6e 6560 290a 0a4c 696b 656c  _=`None`)..Likel
+0002f4d0: 7920 7468 6520 6d6f 7374 2075 7365 6675  y the most usefu
+0002f4e0: 6c20 6f66 2074 6865 2061 7069 2066 756e  l of the api fun
+0002f4f0: 6374 696f 6e73 2c20 6070 6172 7365 6020  ctions, `parse` 
+0002f500: 7461 6b65 7320 436f 636f 6e75 7420 636f  takes Coconut co
+0002f510: 6465 2061 7320 696e 7075 7420 616e 6420  de as input and 
+0002f520: 6f75 7470 7574 7320 7468 6520 6571 7569  outputs the equi
+0002f530: 7661 6c65 6e74 2063 6f6d 7069 6c65 6420  valent compiled 
+0002f540: 5079 7468 6f6e 2063 6f64 652e 205f 6d6f  Python code. _mo
+0002f550: 6465 5f20 6973 2075 7365 6420 746f 2069  de_ is used to i
+0002f560: 6e64 6963 6174 6520 7468 6520 636f 6e74  ndicate the cont
+0002f570: 6578 7420 666f 7220 7468 6520 7061 7273  ext for the pars
+0002f580: 696e 6720 616e 6420 5f73 7461 7465 5f20  ing and _state_ 
+0002f590: 6973 2074 6865 2073 7461 7465 206f 626a  is the state obj
+0002f5a0: 6563 7420 7374 6f72 696e 6720 7468 6520  ect storing the 
+0002f5b0: 636f 6d70 696c 6174 696f 6e20 7061 7261  compilation para
+0002f5c0: 6d65 7465 7273 2074 6f20 7573 6520 6173  meters to use as
+0002f5d0: 206f 6274 6169 6e65 6420 6672 6f6d 205b   obtained from [
+0002f5e0: 2a2a 6765 745f 7374 6174 652a 2a5d 2823  **get_state**](#
+0002f5f0: 6765 745f 7374 6174 6529 2028 6966 2060  get_state) (if `
+0002f600: 4661 6c73 6560 2c20 7573 6573 2074 6865  False`, uses the
+0002f610: 2067 6c6f 6261 6c20 7374 6174 6520 6f62   global state ob
+0002f620: 6a65 6374 292e 205f 6b65 6570 5c5f 696e  ject). _keep\_in
+0002f630: 7465 726e 616c 5c5f 7374 6174 655f 2064  ternal\_state_ d
+0002f640: 6574 6572 6d69 6e65 7320 7768 6574 6865  etermines whethe
+0002f650: 7220 7468 6520 7374 6174 6520 6f62 6a65  r the state obje
+0002f660: 6374 2077 696c 6c20 6b65 6570 2069 6e74  ct will keep int
+0002f670: 6572 6e61 6c20 7374 6174 6520 2873 7563  ernal state (suc
+0002f680: 6820 6173 2077 6861 7420 5b63 7573 746f  h as what [custo
+0002f690: 6d20 6f70 6572 6174 6f72 735d 2823 6375  m operators](#cu
+0002f6a0: 7374 6f6d 2d6f 7065 7261 746f 7273 2920  stom-operators) 
+0002f6b0: 6861 7665 2062 6565 6e20 6465 636c 6172  have been declar
+0002f6c0: 6564 29e2 8094 6966 2060 4e6f 6e65 602c  ed)...if `None`,
+0002f6d0: 2069 6e74 6572 6e61 6c20 7374 6174 6520   internal state 
+0002f6e0: 7769 6c6c 2062 6520 6b65 7074 2069 6666  will be kept iff
+0002f6f0: 2079 6f75 2061 7265 206e 6f74 2075 7369   you are not usi
+0002f700: 6e67 2074 6865 2067 6c6f 6261 6c20 5f73  ng the global _s
+0002f710: 7461 7465 5f2e 0a0a 4966 205f 636f 6465  tate_...If _code
+0002f720: 5f20 6973 206e 6f74 2070 6173 7365 642c  _ is not passed,
+0002f730: 2060 7061 7273 6560 2077 696c 6c20 6f75   `parse` will ou
+0002f740: 7470 7574 206a 7573 7420 7468 6520 6769  tput just the gi
+0002f750: 7665 6e20 5f6d 6f64 655f 2773 2068 6561  ven _mode_'s hea
+0002f760: 6465 722c 2077 6869 6368 2063 616e 2062  der, which can b
+0002f770: 6520 6578 6563 7574 6564 2074 6f20 7365  e executed to se
+0002f780: 7420 7570 2061 6e20 6578 6563 7574 696f  t up an executio
+0002f790: 6e20 656e 7669 726f 6e6d 656e 7420 696e  n environment in
+0002f7a0: 2077 6869 6368 2066 7574 7572 6520 636f   which future co
+0002f7b0: 6465 2063 616e 2062 6520 7061 7273 6564  de can be parsed
+0002f7c0: 2061 6e64 2065 7865 6375 7465 6420 7769   and executed wi
+0002f7d0: 7468 6f75 7420 6120 6865 6164 6572 2e0a  thout a header..
+0002f7e0: 0a45 6163 6820 5f6d 6f64 655f 2068 6173  .Each _mode_ has
+0002f7f0: 2074 776f 2063 6f6d 706f 6e65 6e74 733a   two components:
+0002f800: 2077 6861 7420 7061 7273 6572 2069 7420   what parser it 
+0002f810: 7573 6573 2c20 616e 6420 7768 6174 2068  uses, and what h
+0002f820: 6561 6465 7220 6974 2070 7265 7065 6e64  eader it prepend
+0002f830: 732e 2054 6865 2070 6172 7365 7220 6465  s. The parser de
+0002f840: 7465 726d 696e 6573 2077 6861 7420 436f  termines what Co
+0002f850: 636f 6e75 7420 636f 6465 2069 7320 616c  conut code is al
+0002f860: 6c6f 7765 6420 6173 2069 6e70 7574 2c20  lowed as input, 
+0002f870: 616e 6420 7468 6520 6865 6164 6572 2064  and the header d
+0002f880: 6574 6572 6d69 6e65 7320 686f 7720 7468  etermines how th
+0002f890: 6520 636f 6d70 696c 6564 2050 7974 686f  e compiled Pytho
+0002f8a0: 6e20 6361 6e20 6265 2075 7365 642e 2050  n can be used. P
+0002f8b0: 6f73 7369 626c 6520 7661 6c75 6573 206f  ossible values o
+0002f8c0: 6620 5f6d 6f64 655f 2061 7265 3a0a 0a2d  f _mode_ are:..-
+0002f8d0: 2060 2273 7973 2260 3a20 2874 6865 2064   `"sys"`: (the d
+0002f8e0: 6566 6175 6c74 290a 2020 2020 2b20 7061  efault).    + pa
+0002f8f0: 7273 6572 3a20 6669 6c65 0a20 2020 2020  rser: file.     
+0002f900: 2020 202a 2054 6865 2066 696c 6520 7061     * The file pa
+0002f910: 7273 6572 2063 616e 2070 6172 7365 2061  rser can parse a
+0002f920: 6e79 2043 6f63 6f6e 7574 2063 6f64 652e  ny Coconut code.
+0002f930: 0a20 2020 202b 2068 6561 6465 723a 2073  .    + header: s
+0002f940: 7973 0a20 2020 2020 2020 202a 2054 6869  ys.        * Thi
+0002f950: 7320 6865 6164 6572 2069 6d70 6f72 7473  s header imports
+0002f960: 205b 6063 6f63 6f6e 7574 2e5f 5f63 6f63   [`coconut.__coc
+0002f970: 6f6e 7574 5f5f 605d 2823 636f 636f 6e75  onut__`](#coconu
+0002f980: 742d 636f 636f 6e75 7429 2074 6f20 6163  t-coconut) to ac
+0002f990: 6365 7373 2074 6865 206e 6563 6573 7361  cess the necessa
+0002f9a0: 7279 2043 6f63 6f6e 7574 206f 626a 6563  ry Coconut objec
+0002f9b0: 7473 2e0a 2d20 6022 6578 6563 2260 3a0a  ts..- `"exec"`:.
+0002f9c0: 2020 2020 2b20 7061 7273 6572 3a20 6669      + parser: fi
+0002f9d0: 6c65 0a20 2020 202b 2068 6561 6465 723a  le.    + header:
+0002f9e0: 2065 7865 630a 2020 2020 2020 2020 2a20   exec.        * 
+0002f9f0: 5768 656e 2070 6173 7365 6420 746f 2060  When passed to `
+0002fa00: 6578 6563 6020 6174 2074 6865 2067 6c6f  exec` at the glo
+0002fa10: 6261 6c20 6c65 7665 6c2c 2074 6869 7320  bal level, this 
+0002fa20: 6865 6164 6572 2077 696c 6c20 6372 6561  header will crea
+0002fa30: 7465 2061 6c6c 2074 6865 206e 6563 6573  te all the neces
+0002fa40: 7361 7279 2043 6f63 6f6e 7574 206f 626a  sary Coconut obj
+0002fa50: 6563 7473 2069 7473 656c 6620 696e 7374  ects itself inst
+0002fa60: 6561 6420 6f66 2069 6d70 6f72 7469 6e67  ead of importing
+0002fa70: 2074 6865 6d2e 0a2d 2060 2266 696c 6522   them..- `"file"
+0002fa80: 603a 0a20 2020 202b 2070 6172 7365 723a  `:.    + parser:
+0002fa90: 2066 696c 650a 2020 2020 2b20 6865 6164   file.    + head
+0002faa0: 6572 3a20 6669 6c65 0a20 2020 2020 2020  er: file.       
+0002fab0: 202a 2054 6869 7320 6865 6164 6572 2069   * This header i
+0002fac0: 7320 6d65 616e 7420 746f 2062 6520 7772  s meant to be wr
+0002fad0: 6974 7465 6e20 746f 2061 2060 2d2d 7374  itten to a `--st
+0002fae0: 616e 6461 6c6f 6e65 6020 6669 6c65 2061  andalone` file a
+0002faf0: 6e64 2073 686f 756c 6420 6e6f 7420 6265  nd should not be
+0002fb00: 2070 6173 7365 6420 746f 2060 6578 6563   passed to `exec
+0002fb10: 602e 0a2d 2060 2270 6163 6b61 6765 2260  `..- `"package"`
+0002fb20: 3a0a 2020 2020 2b20 7061 7273 6572 3a20  :.    + parser: 
+0002fb30: 6669 6c65 0a20 2020 202b 2068 6561 6465  file.    + heade
+0002fb40: 723a 2070 6163 6b61 6765 0a20 2020 2020  r: package.     
+0002fb50: 2020 202a 2054 6869 7320 6865 6164 6572     * This header
+0002fb60: 2069 7320 6d65 616e 7420 746f 2062 6520   is meant to be 
+0002fb70: 7772 6974 7465 6e20 746f 2061 2060 2d2d  written to a `--
+0002fb80: 7061 636b 6167 6560 2066 696c 6520 616e  package` file an
+0002fb90: 6420 7368 6f75 6c64 206e 6f74 2062 6520  d should not be 
+0002fba0: 7061 7373 6564 2074 6f20 6065 7865 6360  passed to `exec`
+0002fbb0: 2e0a 2d20 6022 626c 6f63 6b22 603a 0a20  ..- `"block"`:. 
+0002fbc0: 2020 202b 2070 6172 7365 723a 2066 696c     + parser: fil
+0002fbd0: 650a 2020 2020 2b20 6865 6164 6572 3a20  e.    + header: 
+0002fbe0: 6e6f 6e65 0a20 2020 2020 2020 202a 204e  none.        * N
+0002fbf0: 6f20 6865 6164 6572 2069 7320 696e 636c  o header is incl
+0002fc00: 7564 6564 2c20 7468 7573 2074 6869 7320  uded, thus this 
+0002fc10: 6361 6e20 6f6e 6c79 2062 6520 7061 7373  can only be pass
+0002fc20: 6564 2074 6f20 6065 7865 6360 2069 6620  ed to `exec` if 
+0002fc30: 636f 6465 2077 6974 6820 6120 6865 6164  code with a head
+0002fc40: 6572 2068 6173 2061 6c72 6561 6479 2062  er has already b
+0002fc50: 6565 6e20 6578 6563 7574 6564 2061 7420  een executed at 
+0002fc60: 7468 6520 676c 6f62 616c 206c 6576 656c  the global level
+0002fc70: 2e0a 2d20 6022 7369 6e67 6c65 2260 3a0a  ..- `"single"`:.
+0002fc80: 2020 2020 2b20 7061 7273 6572 3a20 7369      + parser: si
+0002fc90: 6e67 6c65 0a20 2020 2020 2020 202a 2043  ngle.        * C
+0002fca0: 616e 206f 6e6c 7920 7061 7273 6520 6f6e  an only parse on
+0002fcb0: 6520 6c69 6e65 206f 6620 436f 636f 6e75  e line of Coconu
+0002fcc0: 7420 636f 6465 2e0a 2020 2020 2b20 6865  t code..    + he
+0002fcd0: 6164 6572 3a20 6e6f 6e65 0a2d 2060 2265  ader: none.- `"e
+0002fce0: 7661 6c22 603a 0a20 2020 202b 2070 6172  val"`:.    + par
+0002fcf0: 7365 723a 2065 7661 6c0a 2020 2020 2020  ser: eval.      
+0002fd00: 2020 2a20 4361 6e20 6f6e 6c79 2070 6172    * Can only par
+0002fd10: 7365 2061 2043 6f63 6f6e 7574 2065 7870  se a Coconut exp
+0002fd20: 7265 7373 696f 6e2c 206e 6f74 2061 2073  ression, not a s
+0002fd30: 7461 7465 6d65 6e74 2e0a 2020 2020 2b20  tatement..    + 
+0002fd40: 6865 6164 6572 3a20 6e6f 6e65 0a2d 2060  header: none.- `
+0002fd50: 226c 656e 6965 6e74 2260 3a0a 2020 2020  "lenient"`:.    
+0002fd60: 2b20 7061 7273 6572 3a20 6c65 6e69 656e  + parser: lenien
+0002fd70: 740a 2020 2020 2020 2020 2a20 4361 6e20  t.        * Can 
+0002fd80: 7061 7273 6520 616e 7920 436f 636f 6e75  parse any Coconu
+0002fd90: 7420 636f 6465 2c20 616c 6c6f 7773 206c  t code, allows l
+0002fda0: 6561 6469 6e67 2077 6869 7465 7370 6163  eading whitespac
+0002fdb0: 652c 2061 6e64 2068 6173 206e 6f20 7472  e, and has no tr
+0002fdc0: 6169 6c69 6e67 206e 6577 6c69 6e65 2e0a  ailing newline..
 0002fdd0: 2020 2020 2b20 6865 6164 6572 3a20 6e6f      + header: no
-0002fde0: 6e65 0a0a 2323 2323 2320 4578 616d 706c  ne..##### Exampl
-0002fdf0: 650a 0a60 6060 636f 636f 6e75 745f 7079  e..```coconut_py
-0002fe00: 7468 6f6e 0a66 726f 6d20 636f 636f 6e75  thon.from coconu
-0002fe10: 742e 6170 6920 696d 706f 7274 2070 6172  t.api import par
-0002fe20: 7365 0a65 7865 6328 7061 7273 6528 2929  se.exec(parse())
-0002fe30: 0a77 6869 6c65 2054 7275 653a 0a20 2020  .while True:.   
-0002fe40: 2065 7865 6328 7061 7273 6528 696e 7075   exec(parse(inpu
-0002fe50: 7428 292c 206d 6f64 653d 2262 6c6f 636b  t(), mode="block
-0002fe60: 2229 290a 6060 600a 0a23 2323 2320 6073  ")).```..#### `s
-0002fe70: 6574 7570 600a 0a2a 2a63 6f63 6f6e 7574  etup`..**coconut
-0002fe80: 2e61 7069 2e73 6574 7570 2a2a 285f 7461  .api.setup**(_ta
-0002fe90: 7267 6574 5f3d 604e 6f6e 6560 2c20 5f73  rget_=`None`, _s
-0002fea0: 7472 6963 745f 3d60 4661 6c73 6560 2c20  trict_=`False`, 
-0002feb0: 5f6d 696e 6966 795f 3d60 4661 6c73 6560  _minify_=`False`
-0002fec0: 2c20 5f6c 696e 655c 5f6e 756d 6265 7273  , _line\_numbers
-0002fed0: 5f3d 6046 616c 7365 602c 205f 6b65 6570  _=`False`, _keep
-0002fee0: 5c5f 6c69 6e65 735f 3d60 4661 6c73 6560  \_lines_=`False`
-0002fef0: 2c20 5f6e 6f5c 5f74 636f 5f3d 6046 616c  , _no\_tco_=`Fal
-0002ff00: 7365 602c 205f 6e6f 5c5f 7772 6170 5f3d  se`, _no\_wrap_=
-0002ff10: 6046 616c 7365 602c 202a 2c20 5f73 7461  `False`, *, _sta
-0002ff20: 7465 5f3d 6046 616c 7365 6029 0a0a 6073  te_=`False`)..`s
-0002ff30: 6574 7570 6020 6361 6e20 6265 2075 7365  etup` can be use
-0002ff40: 6420 746f 2073 6574 2075 7020 7468 6520  d to set up the 
-0002ff50: 6769 7665 6e20 7374 6174 6520 6f62 6a65  given state obje
-0002ff60: 6374 2077 6974 6820 7468 6520 6769 7665  ct with the give
-0002ff70: 6e20 636f 6d6d 616e 642d 6c69 6e65 2066  n command-line f
-0002ff80: 6c61 6773 2e20 4966 205f 7374 6174 655f  lags. If _state_
-0002ff90: 2069 7320 6046 616c 7365 602c 2074 6865   is `False`, the
-0002ffa0: 2067 6c6f 6261 6c20 7374 6174 6520 6f62   global state ob
-0002ffb0: 6a65 6374 2069 7320 7573 6564 2e0a 0a54  ject is used...T
-0002ffc0: 6865 2070 6f73 7369 626c 6520 7661 6c75  he possible valu
-0002ffd0: 6573 2066 6f72 2065 6163 6820 666c 6167  es for each flag
-0002ffe0: 2061 7267 756d 656e 7420 6172 653a 0a0a   argument are:..
-0002fff0: 2d20 5f74 6172 6765 745f 3a20 604e 6f6e  - _target_: `Non
-00030000: 6560 2028 6465 6661 756c 7429 2c20 6f72  e` (default), or
-00030010: 2061 6e79 205b 616c 6c6f 7761 626c 6520   any [allowable 
-00030020: 7461 7267 6574 5d28 2361 6c6c 6f77 6162  target](#allowab
-00030030: 6c65 2d74 6172 6765 7473 290a 2d20 5f73  le-targets).- _s
-00030040: 7472 6963 745f 3a20 6046 616c 7365 6020  trict_: `False` 
-00030050: 2864 6566 6175 6c74 2920 6f72 2060 5472  (default) or `Tr
-00030060: 7565 600a 2d20 5f6d 696e 6966 795f 3a20  ue`.- _minify_: 
-00030070: 6046 616c 7365 6020 2864 6566 6175 6c74  `False` (default
-00030080: 2920 6f72 2060 5472 7565 600a 2d20 5f6c  ) or `True`.- _l
-00030090: 696e 655c 5f6e 756d 6265 7273 5f3a 2060  ine\_numbers_: `
-000300a0: 4661 6c73 6560 2028 6465 6661 756c 7429  False` (default)
-000300b0: 206f 7220 6054 7275 6560 0a2d 205f 6b65   or `True`.- _ke
-000300c0: 6570 5c5f 6c69 6e65 735f 3a20 6046 616c  ep\_lines_: `Fal
-000300d0: 7365 6020 2864 6566 6175 6c74 2920 6f72  se` (default) or
-000300e0: 2060 5472 7565 600a 2d20 5f6e 6f5c 5f74   `True`.- _no\_t
-000300f0: 636f 5f3a 2060 4661 6c73 6560 2028 6465  co_: `False` (de
-00030100: 6661 756c 7429 206f 7220 6054 7275 6560  fault) or `True`
-00030110: 0a2d 205f 6e6f 5c5f 7772 6170 5f3a 2060  .- _no\_wrap_: `
-00030120: 4661 6c73 6560 2028 6465 6661 756c 7429  False` (default)
-00030130: 206f 7220 6054 7275 6560 0a0a 2323 2323   or `True`..####
-00030140: 2060 636d 6460 0a0a 2a2a 636f 636f 6e75   `cmd`..**coconu
-00030150: 742e 6170 692e 636d 642a 2a28 5f61 7267  t.api.cmd**(_arg
-00030160: 735f 3d60 4e6f 6e65 602c 202a 2c20 5f61  s_=`None`, *, _a
-00030170: 7267 765f 3d60 4e6f 6e65 602c 205f 696e  rgv_=`None`, _in
-00030180: 7465 7261 6374 5f3d 6046 616c 7365 602c  teract_=`False`,
-00030190: 205f 6465 6661 756c 745c 5f74 6172 6765   _default\_targe
-000301a0: 745f 3d60 4e6f 6e65 602c 205f 7374 6174  t_=`None`, _stat
-000301b0: 655f 3d60 4661 6c73 6560 290a 0a45 7865  e_=`False`)..Exe
-000301c0: 6375 7465 7320 7468 6520 6769 7665 6e20  cutes the given 
-000301d0: 5f61 7267 735f 2061 7320 6966 2074 6865  _args_ as if the
-000301e0: 7920 7765 7265 2066 6564 2074 6f20 6063  y were fed to `c
-000301f0: 6f63 6f6e 7574 6020 6f6e 2074 6865 2063  oconut` on the c
-00030200: 6f6d 6d61 6e64 2d6c 696e 652c 2077 6974  ommand-line, wit
-00030210: 6820 7468 6520 6578 6365 7074 696f 6e20  h the exception 
-00030220: 7468 6174 2075 6e6c 6573 7320 5f69 6e74  that unless _int
-00030230: 6572 6163 745f 2069 7320 7472 7565 206f  eract_ is true o
-00030240: 7220 602d 6960 2069 7320 7061 7373 6564  r `-i` is passed
-00030250: 2c20 7468 6520 696e 7465 7270 7265 7465  , the interprete
-00030260: 7220 7769 6c6c 206e 6f74 2062 6520 7374  r will not be st
-00030270: 6172 7465 642e 2041 6464 6974 696f 6e61  arted. Additiona
-00030280: 6c6c 792c 205f 6172 6776 5f20 6361 6e20  lly, _argv_ can 
-00030290: 6265 2075 7365 6420 746f 2070 6173 7320  be used to pass 
-000302a0: 696e 2061 7267 756d 656e 7473 2061 7320  in arguments as 
-000302b0: 696e 2060 2d2d 6172 6776 6020 616e 6420  in `--argv` and 
-000302c0: 5f64 6566 6175 6c74 5c5f 7461 7267 6574  _default\_target
-000302d0: 5f20 6361 6e20 6265 2075 7365 6420 746f  _ can be used to
-000302e0: 2073 6574 2074 6865 2064 6566 6175 6c74   set the default
-000302f0: 2060 2d2d 7461 7267 6574 602e 0a0a 4861   `--target`...Ha
-00030300: 7320 7468 6520 7361 6d65 2065 6666 6563  s the same effec
-00030310: 7420 6f66 2073 6574 7469 6e67 2074 6865  t of setting the
-00030320: 2063 6f6d 6d61 6e64 2d6c 696e 6520 666c   command-line fl
-00030330: 6167 7320 6f6e 2074 6865 2067 6976 656e  ags on the given
-00030340: 205f 7374 6174 655f 206f 626a 6563 7420   _state_ object 
-00030350: 6173 2060 7365 7475 7060 2028 7769 7468  as `setup` (with
-00030360: 2074 6865 2067 6c6f 6261 6c20 6073 7461   the global `sta
-00030370: 7465 6020 6f62 6a65 6374 2075 7365 6420  te` object used 
-00030380: 7768 656e 205f 7374 6174 655f 2069 7320  when _state_ is 
-00030390: 6046 616c 7365 6029 2e0a 0a23 2323 2320  `False`)...#### 
-000303a0: 6063 6f63 6f6e 7574 5f65 7661 6c60 0a0a  `coconut_eval`..
-000303b0: 2a2a 636f 636f 6e75 742e 6170 692e 636f  **coconut.api.co
-000303c0: 636f 6e75 745f 6576 616c 2a2a 285f 6578  conut_eval**(_ex
-000303d0: 7072 6573 7369 6f6e 5f2c 205f 676c 6f62  pression_, _glob
-000303e0: 616c 735f 3d60 4e6f 6e65 602c 205f 6c6f  als_=`None`, _lo
-000303f0: 6361 6c73 5f3d 604e 6f6e 6560 2c20 5f73  cals_=`None`, _s
-00030400: 7461 7465 5f3d 6046 616c 7365 602c 205f  tate_=`False`, _
-00030410: 6b65 6570 5c5f 696e 7465 726e 616c 5c5f  keep\_internal\_
-00030420: 7374 6174 655f 3d60 4e6f 6e65 6029 0a0a  state_=`None`)..
-00030430: 5665 7273 696f 6e20 6f66 205b 6065 7661  Version of [`eva
-00030440: 6c60 5d28 6874 7470 733a 2f2f 646f 6373  l`](https://docs
-00030450: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
-00030460: 6272 6172 792f 6675 6e63 7469 6f6e 732e  brary/functions.
-00030470: 6874 6d6c 2365 7661 6c29 2077 6869 6368  html#eval) which
-00030480: 2063 616e 2065 7661 6c75 6174 6520 436f   can evaluate Co
-00030490: 636f 6e75 7420 636f 6465 2e0a 0a23 2323  conut code...###
-000304a0: 2320 6076 6572 7369 6f6e 600a 0a2a 2a63  # `version`..**c
-000304b0: 6f63 6f6e 7574 2e61 7069 2e76 6572 7369  oconut.api.versi
-000304c0: 6f6e 2a2a 282a 2a5b 2a2a 5f77 6869 6368  on**(**[**_which
-000304d0: 5f2a 2a5d 2a2a 290a 0a52 6574 7269 6576  _**]**)..Retriev
-000304e0: 6573 2061 2073 7472 696e 6720 636f 6e74  es a string cont
-000304f0: 6169 6e69 6e67 2069 6e66 6f72 6d61 7469  aining informati
-00030500: 6f6e 2061 626f 7574 2074 6865 2043 6f63  on about the Coc
-00030510: 6f6e 7574 2076 6572 7369 6f6e 2e20 5468  onut version. Th
-00030520: 6520 6f70 7469 6f6e 616c 2061 7267 756d  e optional argum
-00030530: 656e 7420 5f77 6869 6368 5f20 6973 2074  ent _which_ is t
-00030540: 6865 2074 7970 6520 6f66 2076 6572 7369  he type of versi
-00030550: 6f6e 2069 6e66 6f72 6d61 7469 6f6e 2064  on information d
-00030560: 6573 6972 6564 2e20 506f 7373 6962 6c65  esired. Possible
-00030570: 2076 616c 7565 7320 6f66 205f 7768 6963   values of _whic
-00030580: 685f 2061 7265 3a0a 0a2d 2060 226e 756d  h_ are:..- `"num
-00030590: 2260 3a20 7468 6520 6e75 6d65 7269 6361  "`: the numerica
-000305a0: 6c20 7665 7273 696f 6e20 2874 6865 2064  l version (the d
-000305b0: 6566 6175 6c74 290a 2d20 6022 6e61 6d65  efault).- `"name
-000305c0: 2260 3a20 7468 6520 7665 7273 696f 6e20  "`: the version 
-000305d0: 636f 6465 6e61 6d65 0a2d 2060 2273 7065  codename.- `"spe
-000305e0: 6322 603a 2074 6865 206e 756d 6572 6963  c"`: the numeric
-000305f0: 616c 2076 6572 7369 6f6e 2077 6974 6820  al version with 
-00030600: 7468 6520 636f 6465 6e61 6d65 2061 7474  the codename att
-00030610: 6163 6865 640a 2d20 6022 7461 6722 603a  ached.- `"tag"`:
-00030620: 2074 6865 2076 6572 7369 6f6e 2074 6167   the version tag
-00030630: 2075 7365 6420 696e 2047 6974 4875 6220   used in GitHub 
-00030640: 616e 6420 646f 6375 6d65 6e74 6174 696f  and documentatio
-00030650: 6e20 5552 4c73 0a2d 2060 222d 7622 603a  n URLs.- `"-v"`:
-00030660: 2074 6865 2066 756c 6c20 7374 7269 6e67   the full string
-00030670: 2070 7269 6e74 6564 2062 7920 6063 6f63   printed by `coc
-00030680: 6f6e 7574 202d 7660 0a0a 2323 2323 2060  onut -v`..#### `
-00030690: 6175 746f 5f63 6f6d 7069 6c61 7469 6f6e  auto_compilation
-000306a0: 600a 0a2a 2a63 6f63 6f6e 7574 2e61 7069  `..**coconut.api
-000306b0: 2e61 7574 6f5f 636f 6d70 696c 6174 696f  .auto_compilatio
-000306c0: 6e2a 2a28 5f6f 6e5f 3d60 5472 7565 6029  n**(_on_=`True`)
-000306d0: 0a0a 5475 726e 7320 5b61 7574 6f6d 6174  ..Turns [automat
-000306e0: 6963 2063 6f6d 7069 6c61 7469 6f6e 5d28  ic compilation](
-000306f0: 2361 7574 6f6d 6174 6963 2d63 6f6d 7069  #automatic-compi
-00030700: 6c61 7469 6f6e 2920 6f6e 206f 7220 6f66  lation) on or of
-00030710: 662e 2054 6869 7320 6675 6e63 7469 6f6e  f. This function
-00030720: 2069 7320 6361 6c6c 6564 2061 7574 6f6d   is called autom
-00030730: 6174 6963 616c 6c79 2077 6865 6e20 6063  atically when `c
-00030740: 6f63 6f6e 7574 2e61 7069 6020 6973 2069  oconut.api` is i
-00030750: 6d70 6f72 7465 642e 0a0a 2323 2323 2060  mported...#### `
-00030760: 7573 655f 636f 636f 6e75 745f 6272 6561  use_coconut_brea
-00030770: 6b70 6f69 6e74 600a 0a2a 2a63 6f63 6f6e  kpoint`..**cocon
-00030780: 7574 2e61 7069 2e75 7365 5f63 6f63 6f6e  ut.api.use_cocon
-00030790: 7574 5f62 7265 616b 706f 696e 742a 2a28  ut_breakpoint**(
-000307a0: 5f6f 6e5f 3d60 5472 7565 6029 0a0a 5377  _on_=`True`)..Sw
-000307b0: 6974 6368 6573 2074 6865 205b 6062 7265  itches the [`bre
-000307c0: 616b 706f 696e 7460 2062 7569 6c74 2d69  akpoint` built-i
-000307d0: 6e5d 2868 7474 7073 3a2f 2f77 7777 2e70  n](https://www.p
-000307e0: 7974 686f 6e2e 6f72 672f 6465 762f 7065  ython.org/dev/pe
-000307f0: 7073 2f70 6570 2d30 3535 332f 2920 7768  ps/pep-0553/) wh
-00030800: 6963 6820 436f 636f 6e75 7420 6d61 6b65  ich Coconut make
-00030810: 7320 756e 6976 6572 7361 6c6c 7920 6176  s universally av
-00030820: 6169 6c61 626c 6520 746f 2075 7365 205b  ailable to use [
-00030830: 6063 6f63 6f6e 7574 2e65 6d62 6564 605d  `coconut.embed`]
-00030840: 2823 636f 636f 6e75 742d 656d 6265 6429  (#coconut-embed)
-00030850: 2069 6e73 7465 6164 206f 6620 5b60 7064   instead of [`pd
-00030860: 622e 7365 745f 7472 6163 6560 5d28 6874  b.set_trace`](ht
-00030870: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
-00030880: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
-00030890: 7064 622e 6874 6d6c 2370 6462 2e73 6574  pdb.html#pdb.set
-000308a0: 5f74 7261 6365 2920 286f 7220 756e 646f  _trace) (or undo
-000308b0: 6573 2074 6861 7420 7377 6974 6368 2069  es that switch i
-000308c0: 6620 606f 6e3d 4661 6c73 6560 292e 2054  f `on=False`). T
-000308d0: 6869 7320 6675 6e63 7469 6f6e 2069 7320  his function is 
-000308e0: 6361 6c6c 6564 2061 7574 6f6d 6174 6963  called automatic
-000308f0: 616c 6c79 2077 6865 6e20 6063 6f63 6f6e  ally when `cocon
-00030900: 7574 2e61 7069 6020 6973 2069 6d70 6f72  ut.api` is impor
-00030910: 7465 642e 0a0a 2323 2323 2060 436f 636f  ted...#### `Coco
-00030920: 6e75 7445 7863 6570 7469 6f6e 600a 0a49  nutException`..I
-00030930: 6620 616e 2065 7272 6f72 2069 7320 656e  f an error is en
-00030940: 636f 756e 7465 7265 6420 696e 2061 2061  countered in a a
-00030950: 7069 2066 756e 6374 696f 6e2c 2061 2060  pi function, a `
-00030960: 436f 636f 6e75 7445 7863 6570 7469 6f6e  CoconutException
-00030970: 6020 696e 7374 616e 6365 206d 6179 2062  ` instance may b
-00030980: 6520 7261 6973 6564 2e20 6063 6f63 6f6e  e raised. `cocon
-00030990: 7574 2e61 7069 2e43 6f63 6f6e 7574 4578  ut.api.CoconutEx
-000309a0: 6365 7074 696f 6e60 2069 7320 7072 6f76  ception` is prov
-000309b0: 6964 6564 2074 6f20 616c 6c6f 7720 6361  ided to allow ca
-000309c0: 7463 6869 6e67 2073 7563 6820 6572 726f  tching such erro
-000309d0: 7273 2e0a 0a23 2323 2060 636f 636f 6e75  rs...### `coconu
-000309e0: 742e 5f5f 636f 636f 6e75 745f 5f60 0a0a  t.__coconut__`..
-000309f0: 4974 2069 7320 736f 6d65 7469 6d65 7320  It is sometimes 
-00030a00: 7573 6566 756c 2074 6f20 6265 2061 626c  useful to be abl
-00030a10: 6520 746f 2061 6363 6573 7320 436f 636f  e to access Coco
-00030a20: 6e75 7420 6275 696c 742d 696e 7320 6672  nut built-ins fr
-00030a30: 6f6d 2070 7572 6520 5079 7468 6f6e 2e20  om pure Python. 
-00030a40: 546f 2061 6363 6f6d 706c 6973 6820 7468  To accomplish th
-00030a50: 6973 2c20 436f 636f 6e75 7420 7072 6f76  is, Coconut prov
-00030a60: 6964 6573 2060 636f 636f 6e75 742e 5f5f  ides `coconut.__
-00030a70: 636f 636f 6e75 745f 5f60 2c20 7768 6963  coconut__`, whic
-00030a80: 6820 6265 6861 7665 7320 6578 6163 746c  h behaves exactl
-00030a90: 7920 6c69 6b65 2074 6865 2060 5f5f 636f  y like the `__co
-00030aa0: 636f 6e75 745f 5f2e 7079 6020 6865 6164  conut__.py` head
-00030ab0: 6572 2066 696c 6520 696e 636c 7564 6564  er file included
-00030ac0: 2077 6865 6e20 436f 636f 6e75 7420 6973   when Coconut is
-00030ad0: 2063 6f6d 7069 6c65 6420 696e 2070 6163   compiled in pac
-00030ae0: 6b61 6765 206d 6f64 652e 0a0a 416c 6c20  kage mode...All 
-00030af0: 436f 636f 6e75 7420 6275 696c 742d 696e  Coconut built-in
-00030b00: 7320 6172 6520 6163 6365 7373 6962 6c65  s are accessible
-00030b10: 2066 726f 6d20 6063 6f63 6f6e 7574 2e5f   from `coconut._
-00030b20: 5f63 6f63 6f6e 7574 5f5f 602e 2054 6865  _coconut__`. The
-00030b30: 2072 6563 6f6d 6d65 6e64 6564 2077 6179   recommended way
-00030b40: 2074 6f20 696d 706f 7274 2074 6865 6d20   to import them 
-00030b50: 6973 2074 6f20 7573 6520 6066 726f 6d20  is to use `from 
-00030b60: 636f 636f 6e75 742e 5f5f 636f 636f 6e75  coconut.__coconu
-00030b70: 745f 5f20 696d 706f 7274 6020 616e 6420  t__ import` and 
-00030b80: 696d 706f 7274 2077 6861 7465 7665 7220  import whatever 
-00030b90: 6275 696c 742d 696e 7320 796f 7527 6c6c  built-ins you'll
-00030ba0: 2062 6520 7573 696e 672e 0a0a 2323 2323   be using...####
-00030bb0: 2320 4578 616d 706c 650a 0a60 6060 636f  # Example..```co
-00030bc0: 636f 6e75 745f 7079 7468 6f6e 0a66 726f  conut_python.fro
-00030bd0: 6d20 636f 636f 6e75 742e 5f5f 636f 636f  m coconut.__coco
-00030be0: 6e75 745f 5f20 696d 706f 7274 2070 6172  nut__ import par
-00030bf0: 616c 6c65 6c5f 6d61 700a 6060 600a       allel_map.```.
+0002fde0: 6e65 0a2d 2060 2278 6f6e 7368 2260 3a0a  ne.- `"xonsh"`:.
+0002fdf0: 2020 2020 2b20 7061 7273 6572 3a20 786f      + parser: xo
+0002fe00: 6e73 680a 2020 2020 2020 2020 2a20 5061  nsh.        * Pa
+0002fe10: 7273 6573 2043 6f63 6f6e 7574 205b 6078  rses Coconut [`x
+0002fe20: 6f6e 7368 605d 2868 7474 7073 3a2f 2f78  onsh`](https://x
+0002fe30: 6f6e 2e73 6829 2063 6f64 6520 666f 7220  on.sh) code for 
+0002fe40: 7573 6520 696e 205b 436f 636f 6e75 7427  use in [Coconut'
+0002fe50: 7320 6078 6f6e 7368 6020 7375 7070 6f72  s `xonsh` suppor
+0002fe60: 745d 2823 786f 6e73 682d 7375 7070 6f72  t](#xonsh-suppor
+0002fe70: 7429 2e0a 2020 2020 2b20 6865 6164 6572  t)..    + header
+0002fe80: 3a20 6e6f 6e65 0a0a 2323 2323 2320 4578  : none..##### Ex
+0002fe90: 616d 706c 650a 0a60 6060 636f 636f 6e75  ample..```coconu
+0002fea0: 745f 7079 7468 6f6e 0a66 726f 6d20 636f  t_python.from co
+0002feb0: 636f 6e75 742e 6170 6920 696d 706f 7274  conut.api import
+0002fec0: 2070 6172 7365 0a65 7865 6328 7061 7273   parse.exec(pars
+0002fed0: 6528 2929 0a77 6869 6c65 2054 7275 653a  e()).while True:
+0002fee0: 0a20 2020 2065 7865 6328 7061 7273 6528  .    exec(parse(
+0002fef0: 696e 7075 7428 292c 206d 6f64 653d 2262  input(), mode="b
+0002ff00: 6c6f 636b 2229 290a 6060 600a 0a23 2323  lock")).```..###
+0002ff10: 2320 6073 6574 7570 600a 0a2a 2a63 6f63  # `setup`..**coc
+0002ff20: 6f6e 7574 2e61 7069 2e73 6574 7570 2a2a  onut.api.setup**
+0002ff30: 285f 7461 7267 6574 5f3d 604e 6f6e 6560  (_target_=`None`
+0002ff40: 2c20 5f73 7472 6963 745f 3d60 4661 6c73  , _strict_=`Fals
+0002ff50: 6560 2c20 5f6d 696e 6966 795f 3d60 4661  e`, _minify_=`Fa
+0002ff60: 6c73 6560 2c20 5f6c 696e 655c 5f6e 756d  lse`, _line\_num
+0002ff70: 6265 7273 5f3d 6046 616c 7365 602c 205f  bers_=`False`, _
+0002ff80: 6b65 6570 5c5f 6c69 6e65 735f 3d60 4661  keep\_lines_=`Fa
+0002ff90: 6c73 6560 2c20 5f6e 6f5c 5f74 636f 5f3d  lse`, _no\_tco_=
+0002ffa0: 6046 616c 7365 602c 205f 6e6f 5c5f 7772  `False`, _no\_wr
+0002ffb0: 6170 5f3d 6046 616c 7365 602c 202a 2c20  ap_=`False`, *, 
+0002ffc0: 5f73 7461 7465 5f3d 6046 616c 7365 6029  _state_=`False`)
+0002ffd0: 0a0a 6073 6574 7570 6020 6361 6e20 6265  ..`setup` can be
+0002ffe0: 2075 7365 6420 746f 2073 6574 2075 7020   used to set up 
+0002fff0: 7468 6520 6769 7665 6e20 7374 6174 6520  the given state 
+00030000: 6f62 6a65 6374 2077 6974 6820 7468 6520  object with the 
+00030010: 6769 7665 6e20 636f 6d6d 616e 642d 6c69  given command-li
+00030020: 6e65 2066 6c61 6773 2e20 4966 205f 7374  ne flags. If _st
+00030030: 6174 655f 2069 7320 6046 616c 7365 602c  ate_ is `False`,
+00030040: 2074 6865 2067 6c6f 6261 6c20 7374 6174   the global stat
+00030050: 6520 6f62 6a65 6374 2069 7320 7573 6564  e object is used
+00030060: 2e0a 0a54 6865 2070 6f73 7369 626c 6520  ...The possible 
+00030070: 7661 6c75 6573 2066 6f72 2065 6163 6820  values for each 
+00030080: 666c 6167 2061 7267 756d 656e 7420 6172  flag argument ar
+00030090: 653a 0a0a 2d20 5f74 6172 6765 745f 3a20  e:..- _target_: 
+000300a0: 604e 6f6e 6560 2028 6465 6661 756c 7429  `None` (default)
+000300b0: 2c20 6f72 2061 6e79 205b 616c 6c6f 7761  , or any [allowa
+000300c0: 626c 6520 7461 7267 6574 5d28 2361 6c6c  ble target](#all
+000300d0: 6f77 6162 6c65 2d74 6172 6765 7473 290a  owable-targets).
+000300e0: 2d20 5f73 7472 6963 745f 3a20 6046 616c  - _strict_: `Fal
+000300f0: 7365 6020 2864 6566 6175 6c74 2920 6f72  se` (default) or
+00030100: 2060 5472 7565 600a 2d20 5f6d 696e 6966   `True`.- _minif
+00030110: 795f 3a20 6046 616c 7365 6020 2864 6566  y_: `False` (def
+00030120: 6175 6c74 2920 6f72 2060 5472 7565 600a  ault) or `True`.
+00030130: 2d20 5f6c 696e 655c 5f6e 756d 6265 7273  - _line\_numbers
+00030140: 5f3a 2060 4661 6c73 6560 2028 6465 6661  _: `False` (defa
+00030150: 756c 7429 206f 7220 6054 7275 6560 0a2d  ult) or `True`.-
+00030160: 205f 6b65 6570 5c5f 6c69 6e65 735f 3a20   _keep\_lines_: 
+00030170: 6046 616c 7365 6020 2864 6566 6175 6c74  `False` (default
+00030180: 2920 6f72 2060 5472 7565 600a 2d20 5f6e  ) or `True`.- _n
+00030190: 6f5c 5f74 636f 5f3a 2060 4661 6c73 6560  o\_tco_: `False`
+000301a0: 2028 6465 6661 756c 7429 206f 7220 6054   (default) or `T
+000301b0: 7275 6560 0a2d 205f 6e6f 5c5f 7772 6170  rue`.- _no\_wrap
+000301c0: 5f3a 2060 4661 6c73 6560 2028 6465 6661  _: `False` (defa
+000301d0: 756c 7429 206f 7220 6054 7275 6560 0a0a  ult) or `True`..
+000301e0: 2323 2323 2060 636d 6460 0a0a 2a2a 636f  #### `cmd`..**co
+000301f0: 636f 6e75 742e 6170 692e 636d 642a 2a28  conut.api.cmd**(
+00030200: 5f61 7267 735f 3d60 4e6f 6e65 602c 202a  _args_=`None`, *
+00030210: 2c20 5f61 7267 765f 3d60 4e6f 6e65 602c  , _argv_=`None`,
+00030220: 205f 696e 7465 7261 6374 5f3d 6046 616c   _interact_=`Fal
+00030230: 7365 602c 205f 6465 6661 756c 745c 5f74  se`, _default\_t
+00030240: 6172 6765 745f 3d60 4e6f 6e65 602c 205f  arget_=`None`, _
+00030250: 7374 6174 655f 3d60 4661 6c73 6560 290a  state_=`False`).
+00030260: 0a45 7865 6375 7465 7320 7468 6520 6769  .Executes the gi
+00030270: 7665 6e20 5f61 7267 735f 2061 7320 6966  ven _args_ as if
+00030280: 2074 6865 7920 7765 7265 2066 6564 2074   they were fed t
+00030290: 6f20 6063 6f63 6f6e 7574 6020 6f6e 2074  o `coconut` on t
+000302a0: 6865 2063 6f6d 6d61 6e64 2d6c 696e 652c  he command-line,
+000302b0: 2077 6974 6820 7468 6520 6578 6365 7074   with the except
+000302c0: 696f 6e20 7468 6174 2075 6e6c 6573 7320  ion that unless 
+000302d0: 5f69 6e74 6572 6163 745f 2069 7320 7472  _interact_ is tr
+000302e0: 7565 206f 7220 602d 6960 2069 7320 7061  ue or `-i` is pa
+000302f0: 7373 6564 2c20 7468 6520 696e 7465 7270  ssed, the interp
+00030300: 7265 7465 7220 7769 6c6c 206e 6f74 2062  reter will not b
+00030310: 6520 7374 6172 7465 642e 2041 6464 6974  e started. Addit
+00030320: 696f 6e61 6c6c 792c 205f 6172 6776 5f20  ionally, _argv_ 
+00030330: 6361 6e20 6265 2075 7365 6420 746f 2070  can be used to p
+00030340: 6173 7320 696e 2061 7267 756d 656e 7473  ass in arguments
+00030350: 2061 7320 696e 2060 2d2d 6172 6776 6020   as in `--argv` 
+00030360: 616e 6420 5f64 6566 6175 6c74 5c5f 7461  and _default\_ta
+00030370: 7267 6574 5f20 6361 6e20 6265 2075 7365  rget_ can be use
+00030380: 6420 746f 2073 6574 2074 6865 2064 6566  d to set the def
+00030390: 6175 6c74 2060 2d2d 7461 7267 6574 602e  ault `--target`.
+000303a0: 0a0a 4861 7320 7468 6520 7361 6d65 2065  ..Has the same e
+000303b0: 6666 6563 7420 6f66 2073 6574 7469 6e67  ffect of setting
+000303c0: 2074 6865 2063 6f6d 6d61 6e64 2d6c 696e   the command-lin
+000303d0: 6520 666c 6167 7320 6f6e 2074 6865 2067  e flags on the g
+000303e0: 6976 656e 205f 7374 6174 655f 206f 626a  iven _state_ obj
+000303f0: 6563 7420 6173 2060 7365 7475 7060 2028  ect as `setup` (
+00030400: 7769 7468 2074 6865 2067 6c6f 6261 6c20  with the global 
+00030410: 6073 7461 7465 6020 6f62 6a65 6374 2075  `state` object u
+00030420: 7365 6420 7768 656e 205f 7374 6174 655f  sed when _state_
+00030430: 2069 7320 6046 616c 7365 6029 2e0a 0a23   is `False`)...#
+00030440: 2323 2320 6063 6f63 6f6e 7574 5f65 7661  ### `coconut_eva
+00030450: 6c60 0a0a 2a2a 636f 636f 6e75 742e 6170  l`..**coconut.ap
+00030460: 692e 636f 636f 6e75 745f 6576 616c 2a2a  i.coconut_eval**
+00030470: 285f 6578 7072 6573 7369 6f6e 5f2c 205f  (_expression_, _
+00030480: 676c 6f62 616c 735f 3d60 4e6f 6e65 602c  globals_=`None`,
+00030490: 205f 6c6f 6361 6c73 5f3d 604e 6f6e 6560   _locals_=`None`
+000304a0: 2c20 5f73 7461 7465 5f3d 6046 616c 7365  , _state_=`False
+000304b0: 602c 205f 6b65 6570 5c5f 696e 7465 726e  `, _keep\_intern
+000304c0: 616c 5c5f 7374 6174 655f 3d60 4e6f 6e65  al\_state_=`None
+000304d0: 6029 0a0a 5665 7273 696f 6e20 6f66 205b  `)..Version of [
+000304e0: 6065 7661 6c60 5d28 6874 7470 733a 2f2f  `eval`](https://
+000304f0: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
+00030500: 332f 6c69 6272 6172 792f 6675 6e63 7469  3/library/functi
+00030510: 6f6e 732e 6874 6d6c 2365 7661 6c29 2077  ons.html#eval) w
+00030520: 6869 6368 2063 616e 2065 7661 6c75 6174  hich can evaluat
+00030530: 6520 436f 636f 6e75 7420 636f 6465 2e0a  e Coconut code..
+00030540: 0a23 2323 2320 6076 6572 7369 6f6e 600a  .#### `version`.
+00030550: 0a2a 2a63 6f63 6f6e 7574 2e61 7069 2e76  .**coconut.api.v
+00030560: 6572 7369 6f6e 2a2a 282a 2a5b 2a2a 5f77  ersion**(**[**_w
+00030570: 6869 6368 5f2a 2a5d 2a2a 290a 0a52 6574  hich_**]**)..Ret
+00030580: 7269 6576 6573 2061 2073 7472 696e 6720  rieves a string 
+00030590: 636f 6e74 6169 6e69 6e67 2069 6e66 6f72  containing infor
+000305a0: 6d61 7469 6f6e 2061 626f 7574 2074 6865  mation about the
+000305b0: 2043 6f63 6f6e 7574 2076 6572 7369 6f6e   Coconut version
+000305c0: 2e20 5468 6520 6f70 7469 6f6e 616c 2061  . The optional a
+000305d0: 7267 756d 656e 7420 5f77 6869 6368 5f20  rgument _which_ 
+000305e0: 6973 2074 6865 2074 7970 6520 6f66 2076  is the type of v
+000305f0: 6572 7369 6f6e 2069 6e66 6f72 6d61 7469  ersion informati
+00030600: 6f6e 2064 6573 6972 6564 2e20 506f 7373  on desired. Poss
+00030610: 6962 6c65 2076 616c 7565 7320 6f66 205f  ible values of _
+00030620: 7768 6963 685f 2061 7265 3a0a 0a2d 2060  which_ are:..- `
+00030630: 226e 756d 2260 3a20 7468 6520 6e75 6d65  "num"`: the nume
+00030640: 7269 6361 6c20 7665 7273 696f 6e20 2874  rical version (t
+00030650: 6865 2064 6566 6175 6c74 290a 2d20 6022  he default).- `"
+00030660: 6e61 6d65 2260 3a20 7468 6520 7665 7273  name"`: the vers
+00030670: 696f 6e20 636f 6465 6e61 6d65 0a2d 2060  ion codename.- `
+00030680: 2273 7065 6322 603a 2074 6865 206e 756d  "spec"`: the num
+00030690: 6572 6963 616c 2076 6572 7369 6f6e 2077  erical version w
+000306a0: 6974 6820 7468 6520 636f 6465 6e61 6d65  ith the codename
+000306b0: 2061 7474 6163 6865 640a 2d20 6022 7461   attached.- `"ta
+000306c0: 6722 603a 2074 6865 2076 6572 7369 6f6e  g"`: the version
+000306d0: 2074 6167 2075 7365 6420 696e 2047 6974   tag used in Git
+000306e0: 4875 6220 616e 6420 646f 6375 6d65 6e74  Hub and document
+000306f0: 6174 696f 6e20 5552 4c73 0a2d 2060 222d  ation URLs.- `"-
+00030700: 7622 603a 2074 6865 2066 756c 6c20 7374  v"`: the full st
+00030710: 7269 6e67 2070 7269 6e74 6564 2062 7920  ring printed by 
+00030720: 6063 6f63 6f6e 7574 202d 7660 0a0a 2323  `coconut -v`..##
+00030730: 2323 2060 6175 746f 5f63 6f6d 7069 6c61  ## `auto_compila
+00030740: 7469 6f6e 600a 0a2a 2a63 6f63 6f6e 7574  tion`..**coconut
+00030750: 2e61 7069 2e61 7574 6f5f 636f 6d70 696c  .api.auto_compil
+00030760: 6174 696f 6e2a 2a28 5f6f 6e5f 3d60 5472  ation**(_on_=`Tr
+00030770: 7565 6029 0a0a 5475 726e 7320 5b61 7574  ue`)..Turns [aut
+00030780: 6f6d 6174 6963 2063 6f6d 7069 6c61 7469  omatic compilati
+00030790: 6f6e 5d28 2361 7574 6f6d 6174 6963 2d63  on](#automatic-c
+000307a0: 6f6d 7069 6c61 7469 6f6e 2920 6f6e 206f  ompilation) on o
+000307b0: 7220 6f66 662e 2054 6869 7320 6675 6e63  r off. This func
+000307c0: 7469 6f6e 2069 7320 6361 6c6c 6564 2061  tion is called a
+000307d0: 7574 6f6d 6174 6963 616c 6c79 2077 6865  utomatically whe
+000307e0: 6e20 6063 6f63 6f6e 7574 2e61 7069 6020  n `coconut.api` 
+000307f0: 6973 2069 6d70 6f72 7465 642e 0a0a 2323  is imported...##
+00030800: 2323 2060 7573 655f 636f 636f 6e75 745f  ## `use_coconut_
+00030810: 6272 6561 6b70 6f69 6e74 600a 0a2a 2a63  breakpoint`..**c
+00030820: 6f63 6f6e 7574 2e61 7069 2e75 7365 5f63  oconut.api.use_c
+00030830: 6f63 6f6e 7574 5f62 7265 616b 706f 696e  oconut_breakpoin
+00030840: 742a 2a28 5f6f 6e5f 3d60 5472 7565 6029  t**(_on_=`True`)
+00030850: 0a0a 5377 6974 6368 6573 2074 6865 205b  ..Switches the [
+00030860: 6062 7265 616b 706f 696e 7460 2062 7569  `breakpoint` bui
+00030870: 6c74 2d69 6e5d 2868 7474 7073 3a2f 2f77  lt-in](https://w
+00030880: 7777 2e70 7974 686f 6e2e 6f72 672f 6465  ww.python.org/de
+00030890: 762f 7065 7073 2f70 6570 2d30 3535 332f  v/peps/pep-0553/
+000308a0: 2920 7768 6963 6820 436f 636f 6e75 7420  ) which Coconut 
+000308b0: 6d61 6b65 7320 756e 6976 6572 7361 6c6c  makes universall
+000308c0: 7920 6176 6169 6c61 626c 6520 746f 2075  y available to u
+000308d0: 7365 205b 6063 6f63 6f6e 7574 2e65 6d62  se [`coconut.emb
+000308e0: 6564 605d 2823 636f 636f 6e75 742d 656d  ed`](#coconut-em
+000308f0: 6265 6429 2069 6e73 7465 6164 206f 6620  bed) instead of 
+00030900: 5b60 7064 622e 7365 745f 7472 6163 6560  [`pdb.set_trace`
+00030910: 5d28 6874 7470 733a 2f2f 646f 6373 2e70  ](https://docs.p
+00030920: 7974 686f 6e2e 6f72 672f 332f 6c69 6272  ython.org/3/libr
+00030930: 6172 792f 7064 622e 6874 6d6c 2370 6462  ary/pdb.html#pdb
+00030940: 2e73 6574 5f74 7261 6365 2920 286f 7220  .set_trace) (or 
+00030950: 756e 646f 6573 2074 6861 7420 7377 6974  undoes that swit
+00030960: 6368 2069 6620 606f 6e3d 4661 6c73 6560  ch if `on=False`
+00030970: 292e 2054 6869 7320 6675 6e63 7469 6f6e  ). This function
+00030980: 2069 7320 6361 6c6c 6564 2061 7574 6f6d   is called autom
+00030990: 6174 6963 616c 6c79 2077 6865 6e20 6063  atically when `c
+000309a0: 6f63 6f6e 7574 2e61 7069 6020 6973 2069  oconut.api` is i
+000309b0: 6d70 6f72 7465 642e 0a0a 2323 2323 2060  mported...#### `
+000309c0: 436f 636f 6e75 7445 7863 6570 7469 6f6e  CoconutException
+000309d0: 600a 0a49 6620 616e 2065 7272 6f72 2069  `..If an error i
+000309e0: 7320 656e 636f 756e 7465 7265 6420 696e  s encountered in
+000309f0: 2061 2061 7069 2066 756e 6374 696f 6e2c   a api function,
+00030a00: 2061 2060 436f 636f 6e75 7445 7863 6570   a `CoconutExcep
+00030a10: 7469 6f6e 6020 696e 7374 616e 6365 206d  tion` instance m
+00030a20: 6179 2062 6520 7261 6973 6564 2e20 6063  ay be raised. `c
+00030a30: 6f63 6f6e 7574 2e61 7069 2e43 6f63 6f6e  oconut.api.Cocon
+00030a40: 7574 4578 6365 7074 696f 6e60 2069 7320  utException` is 
+00030a50: 7072 6f76 6964 6564 2074 6f20 616c 6c6f  provided to allo
+00030a60: 7720 6361 7463 6869 6e67 2073 7563 6820  w catching such 
+00030a70: 6572 726f 7273 2e0a 0a23 2323 2060 636f  errors...### `co
+00030a80: 636f 6e75 742e 5f5f 636f 636f 6e75 745f  conut.__coconut_
+00030a90: 5f60 0a0a 4974 2069 7320 736f 6d65 7469  _`..It is someti
+00030aa0: 6d65 7320 7573 6566 756c 2074 6f20 6265  mes useful to be
+00030ab0: 2061 626c 6520 746f 2061 6363 6573 7320   able to access 
+00030ac0: 436f 636f 6e75 7420 6275 696c 742d 696e  Coconut built-in
+00030ad0: 7320 6672 6f6d 2070 7572 6520 5079 7468  s from pure Pyth
+00030ae0: 6f6e 2e20 546f 2061 6363 6f6d 706c 6973  on. To accomplis
+00030af0: 6820 7468 6973 2c20 436f 636f 6e75 7420  h this, Coconut 
+00030b00: 7072 6f76 6964 6573 2060 636f 636f 6e75  provides `coconu
+00030b10: 742e 5f5f 636f 636f 6e75 745f 5f60 2c20  t.__coconut__`, 
+00030b20: 7768 6963 6820 6265 6861 7665 7320 6578  which behaves ex
+00030b30: 6163 746c 7920 6c69 6b65 2074 6865 2060  actly like the `
+00030b40: 5f5f 636f 636f 6e75 745f 5f2e 7079 6020  __coconut__.py` 
+00030b50: 6865 6164 6572 2066 696c 6520 696e 636c  header file incl
+00030b60: 7564 6564 2077 6865 6e20 436f 636f 6e75  uded when Coconu
+00030b70: 7420 6973 2063 6f6d 7069 6c65 6420 696e  t is compiled in
+00030b80: 2070 6163 6b61 6765 206d 6f64 652e 0a0a   package mode...
+00030b90: 416c 6c20 436f 636f 6e75 7420 6275 696c  All Coconut buil
+00030ba0: 742d 696e 7320 6172 6520 6163 6365 7373  t-ins are access
+00030bb0: 6962 6c65 2066 726f 6d20 6063 6f63 6f6e  ible from `cocon
+00030bc0: 7574 2e5f 5f63 6f63 6f6e 7574 5f5f 602e  ut.__coconut__`.
+00030bd0: 2054 6865 2072 6563 6f6d 6d65 6e64 6564   The recommended
+00030be0: 2077 6179 2074 6f20 696d 706f 7274 2074   way to import t
+00030bf0: 6865 6d20 6973 2074 6f20 7573 6520 6066  hem is to use `f
+00030c00: 726f 6d20 636f 636f 6e75 742e 5f5f 636f  rom coconut.__co
+00030c10: 636f 6e75 745f 5f20 696d 706f 7274 6020  conut__ import` 
+00030c20: 616e 6420 696d 706f 7274 2077 6861 7465  and import whate
+00030c30: 7665 7220 6275 696c 742d 696e 7320 796f  ver built-ins yo
+00030c40: 7527 6c6c 2062 6520 7573 696e 672e 0a0a  u'll be using...
+00030c50: 2323 2323 2320 4578 616d 706c 650a 0a60  ##### Example..`
+00030c60: 6060 636f 636f 6e75 745f 7079 7468 6f6e  ``coconut_python
+00030c70: 0a66 726f 6d20 636f 636f 6e75 742e 5f5f  .from coconut.__
+00030c80: 636f 636f 6e75 745f 5f20 696d 706f 7274  coconut__ import
+00030c90: 2070 6172 616c 6c65 6c5f 6d61 700a 6060   parallel_map.``
+00030ca0: 600a                                     `.
```

### Comparing `coconut-develop-3.0.2.post0.dev6/FAQ.md` & `coconut-develop-3.0.2.post0.dev7/FAQ.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/HELP.md` & `coconut-develop-3.0.2.post0.dev7/HELP.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/LICENSE.txt` & `coconut-develop-3.0.2.post0.dev7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/PKG-INFO` & `coconut-develop-3.0.2.post0.dev7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,100 @@
 Metadata-Version: 2.1
 Name: coconut-develop
-Version: 3.0.2.post0.dev6
+Version: 3.0.2.post0.dev7
 Summary: Simple, elegant, Pythonic functional programming.
 Home-page: http://coconut-lang.org
 Author: Evan Hubinger
 Author-email: evanjhub@gmail.com
 License: Apache 2.0
+Description: |logo| Coconut
+        ==============
+        
+        ..
+            <insert toctree here>
+        
+        .. |logo| image:: https://github.com/evhub/coconut/raw/gh-pages/favicon-32x32.png
+        
+        .. image:: https://opencollective.com/coconut/backers/badge.svg
+            :alt: Backers on Open Collective
+            :target: #backers
+        .. image:: https://opencollective.com/coconut/sponsors/badge.svg
+            :alt: Sponsors on Open Collective
+            :target: #sponsors
+        .. image:: https://badges.gitter.im/evhub/coconut.svg
+            :alt: Join the chat at https://gitter.im/evhub/coconut
+            :target: https://gitter.im/evhub/coconut?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+        
+        Coconut (`coconut-lang.org`__) is a variant of Python_ that **adds on top of Python syntax** new features for simple, elegant, Pythonic **functional programming**.
+        
+        __ Coconut_
+        .. _Coconut: http://coconut-lang.org/
+        
+        Coconut is developed on GitHub_ and hosted on PyPI_. Installing Coconut is as easy as opening a command prompt and entering::
+        
+            pip install coconut
+        
+        To help you get started, check out these links for more information about Coconut:
+        
+        - Tutorial_: If you're new to Coconut, a good place to start is Coconut's **tutorial**.
+        - Documentation_: If you're looking for info about a specific feature, check out Coconut's **documentation**.
+        - `Online Interpreter`_: If you want to try Coconut in your browser, check out Coconut's **online interpreter**.
+        - FAQ_: If you have general questions about Coconut—like who Coconut is built for and whether or not you should use it—Coconut's frequently asked questions are often the best place to start.
+        - `Create a New Issue <https://github.com/evhub/coconut/issues/new>`_: If you're having a problem with Coconut, creating a new issue detailing the problem will allow it to be addressed as soon as possible.
+        - Gitter_: For any questions, concerns, or comments about anything Coconut-related, ask around at Coconut's Gitter, a GitHub-integrated chat room for Coconut developers.
+        - Releases_: Want to know what's been added in recent Coconut versions? Check out the release log for all the new features and fixes.
+        
+        .. _Python: https://www.python.org/
+        .. _PyPI: https://pypi.python.org/pypi/coconut
+        .. _Tutorial: http://coconut.readthedocs.io/en/latest/HELP.html
+        .. _Documentation: http://coconut.readthedocs.io/en/latest/DOCS.html
+        .. _`Online Interpreter`: https://cs121-team-panda.github.io/coconut-interpreter
+        .. _FAQ: http://coconut.readthedocs.io/en/latest/FAQ.html
+        .. _GitHub: https://github.com/evhub/coconut
+        .. _Gitter: https://gitter.im/evhub/coconut
+        .. _Releases: https://github.com/evhub/coconut/releases
+        
+        Credits
+        +++++++
+        
+        Contributors
+        ------------
+        
+        This project exists thanks to all the people who contribute! `Become a contributor`__.
+        
+        .. image:: https://opencollective.com/coconut/contributors.svg?width=890&button=false
+            :target: https://github.com/evhub/coconut/graphs/contributors
+        
+        __ Contributor_
+        .. _Contributor: http://coconut.readthedocs.io/en/develop/CONTRIBUTING.html
+        
+        Backers
+        -------
+        
+        Thank you to all our backers! `Become a backer`__.
+        
+        .. image:: https://opencollective.com/coconut/backers.svg?width=890
+            :target: https://opencollective.com/coconut#backers
+        
+        __ Backer_
+        .. _Backer: https://opencollective.com/coconut#backer
+        
+        Sponsors
+        --------
+        
+        Support Coconut by becoming a sponsor. Your logo will show up here with a link to your website. `Become a sponsor`__.
+        
+        .. image:: https://opencollective.com/XX/sponsor/0/avatar.svg
+            :target: https://opencollective.com/coconut/sponsor/0/website
+        
+        __ Sponsor_
+        .. _Sponsor: https://opencollective.com/coconut#sponsor
+        
 Keywords: functional,programming,language,compiler,pattern,pattern-matching,algebraic,data type,data types,lambda,lambdas,lazy,evaluation,lazy list,lazy lists,tail,recursion,call,recursive,infix,function,composition,compose,partial,application,currying,curry,pipeline,pipe,unicode,operator,operators,frozenset,literal,syntax,destructuring,assignment,fold,datamaker,prepattern,iterator,none,coalesce,coalescing,statement,lru_cache,memoization,backport,typing,embed,PEP 622,overrides,islice,itertools,functools,TYPE_CHECKING,Expected,breakpoint,help,reduce,takewhile,dropwhile,tee,count,makedata,consume,parallel_map,addpattern,recursive_iterator,concurrent_map,fmap,starmap,reiterable,scan,groupsof,memoize,zip_longest,override,flatten,ident,call,safe_call,flip,const,lift,all_equal,collectby,multi_enumerate,cartesian_product,multiset,cycle,windowsof,and_then,and_then_await,py_chr,py_dict,py_hex,py_input,py_int,py_map,py_object,py_oct,py_open,py_print,py_range,py_str,py_super,py_zip,py_filter,py_reversed,py_enumerate,py_raw_input,py_xrange,py_repr,py_breakpoint,_namedtuple_of,reveal_type,reveal_locals,MatchError,__fmap__,__iter_getitem__,data,match,case,cases,where,addpattern,then,operator,type,copyclosure,λ
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Interpreters
@@ -47,91 +131,7 @@
 Provides-Extra: xonsh
 Provides-Extra: jupyter
 Provides-Extra: all
 Provides-Extra: ipython
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: dev
-License-File: LICENSE.txt
-
-|logo| Coconut
-==============
-
-..
-    <insert toctree here>
-
-.. |logo| image:: https://github.com/evhub/coconut/raw/gh-pages/favicon-32x32.png
-
-.. image:: https://opencollective.com/coconut/backers/badge.svg
-    :alt: Backers on Open Collective
-    :target: #backers
-.. image:: https://opencollective.com/coconut/sponsors/badge.svg
-    :alt: Sponsors on Open Collective
-    :target: #sponsors
-.. image:: https://badges.gitter.im/evhub/coconut.svg
-    :alt: Join the chat at https://gitter.im/evhub/coconut
-    :target: https://gitter.im/evhub/coconut?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-
-Coconut (`coconut-lang.org`__) is a variant of Python_ that **adds on top of Python syntax** new features for simple, elegant, Pythonic **functional programming**.
-
-__ Coconut_
-.. _Coconut: http://coconut-lang.org/
-
-Coconut is developed on GitHub_ and hosted on PyPI_. Installing Coconut is as easy as opening a command prompt and entering::
-
-    pip install coconut
-
-To help you get started, check out these links for more information about Coconut:
-
-- Tutorial_: If you're new to Coconut, a good place to start is Coconut's **tutorial**.
-- Documentation_: If you're looking for info about a specific feature, check out Coconut's **documentation**.
-- `Online Interpreter`_: If you want to try Coconut in your browser, check out Coconut's **online interpreter**.
-- FAQ_: If you have general questions about Coconut—like who Coconut is built for and whether or not you should use it—Coconut's frequently asked questions are often the best place to start.
-- `Create a New Issue <https://github.com/evhub/coconut/issues/new>`_: If you're having a problem with Coconut, creating a new issue detailing the problem will allow it to be addressed as soon as possible.
-- Gitter_: For any questions, concerns, or comments about anything Coconut-related, ask around at Coconut's Gitter, a GitHub-integrated chat room for Coconut developers.
-- Releases_: Want to know what's been added in recent Coconut versions? Check out the release log for all the new features and fixes.
-
-.. _Python: https://www.python.org/
-.. _PyPI: https://pypi.python.org/pypi/coconut
-.. _Tutorial: http://coconut.readthedocs.io/en/latest/HELP.html
-.. _Documentation: http://coconut.readthedocs.io/en/latest/DOCS.html
-.. _`Online Interpreter`: https://cs121-team-panda.github.io/coconut-interpreter
-.. _FAQ: http://coconut.readthedocs.io/en/latest/FAQ.html
-.. _GitHub: https://github.com/evhub/coconut
-.. _Gitter: https://gitter.im/evhub/coconut
-.. _Releases: https://github.com/evhub/coconut/releases
-
-Credits
-+++++++
-
-Contributors
-------------
-
-This project exists thanks to all the people who contribute! `Become a contributor`__.
-
-.. image:: https://opencollective.com/coconut/contributors.svg?width=890&button=false
-    :target: https://github.com/evhub/coconut/graphs/contributors
-
-__ Contributor_
-.. _Contributor: http://coconut.readthedocs.io/en/develop/CONTRIBUTING.html
-
-Backers
--------
-
-Thank you to all our backers! `Become a backer`__.
-
-.. image:: https://opencollective.com/coconut/backers.svg?width=890
-    :target: https://opencollective.com/coconut#backers
-
-__ Backer_
-.. _Backer: https://opencollective.com/coconut#backer
-
-Sponsors
---------
-
-Support Coconut by becoming a sponsor. Your logo will show up here with a link to your website. `Become a sponsor`__.
-
-.. image:: https://opencollective.com/XX/sponsor/0/avatar.svg
-    :target: https://opencollective.com/coconut/sponsor/0/website
-
-__ Sponsor_
-.. _Sponsor: https://opencollective.com/coconut#sponsor
```

### Comparing `coconut-develop-3.0.2.post0.dev6/README.rst` & `coconut-develop-3.0.2.post0.dev7/README.rst`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/__coconut__/__init__.py` & `coconut-develop-3.0.2.post0.dev7/__coconut__/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/__coconut__/__init__.pyi` & `coconut-develop-3.0.2.post0.dev7/__coconut__/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/_coconut/__init__.py` & `coconut-develop-3.0.2.post0.dev7/_coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/_coconut/__init__.pyi` & `coconut-develop-3.0.2.post0.dev7/_coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/__coconut__.py` & `coconut-develop-3.0.2.post0.dev7/coconut/__coconut__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/__coconut__.pyi` & `coconut-develop-3.0.2.post0.dev7/coconut/__coconut__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/__init__.py` & `coconut-develop-3.0.2.post0.dev7/coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/__init__.pyi` & `coconut-develop-3.0.2.post0.dev7/coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/__main__.py` & `coconut-develop-3.0.2.post0.dev7/coconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/_pyparsing.py` & `coconut-develop-3.0.2.post0.dev7/coconut/_pyparsing.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/api.py` & `coconut-develop-3.0.2.post0.dev7/coconut/api.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/api.pyi` & `coconut-develop-3.0.2.post0.dev7/coconut/api.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/command/__init__.py` & `coconut-develop-3.0.2.post0.dev7/coconut/command/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/command/cli.py` & `coconut-develop-3.0.2.post0.dev7/coconut/command/cli.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/command/command.py` & `coconut-develop-3.0.2.post0.dev7/coconut/command/command.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/command/command.pyi` & `coconut-develop-3.0.2.post0.dev7/coconut/command/command.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/command/mypy.py` & `coconut-develop-3.0.2.post0.dev7/coconut/command/mypy.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/command/util.py` & `coconut-develop-3.0.2.post0.dev7/coconut/command/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/command/watch.py` & `coconut-develop-3.0.2.post0.dev7/coconut/command/watch.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/compiler/__init__.py` & `coconut-develop-3.0.2.post0.dev7/coconut/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/compiler/compiler.py` & `coconut-develop-3.0.2.post0.dev7/coconut/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/compiler/grammar.py` & `coconut-develop-3.0.2.post0.dev7/coconut/compiler/grammar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1386,15 +1386,17 @@
     impl_call_item = condense(
         disallow_keywords(reserved_vars)
         + ~any_string
         + atom_item
         + Optional(power_in_impl_call)
     )
     impl_call = Forward()
-    impl_call_ref = (
+    # we need to disable this inside the xonsh parser
+    impl_call_ref = Forward()
+    unsafe_impl_call_ref = (
         impl_call_item + OneOrMore(impl_call_arg)
     )
 
     factor <<= condense(
         ZeroOrMore(unary) + (
             impl_call
             | await_item + Optional(power)
@@ -2353,16 +2355,21 @@
 
     unsafe_anything_stmt = originalTextFor(regex_item("[^\n]+\n+"))
     unsafe_xonsh_command = originalTextFor(
         (Optional(at) + dollar | bang)
         + ~(lparen + rparen | lbrack + rbrack | lbrace + rbrace)
         + (parens | brackets | braces | unsafe_name)
     )
-    xonsh_parser, _anything_stmt, _xonsh_command = disable_outside(
+    unsafe_xonsh_parser, _impl_call_ref = disable_inside(
         single_parser,
+        unsafe_impl_call_ref,
+    )
+    impl_call_ref <<= _impl_call_ref
+    xonsh_parser, _anything_stmt, _xonsh_command = disable_outside(
+        unsafe_xonsh_parser,
         unsafe_anything_stmt,
         unsafe_xonsh_command,
     )
     anything_stmt <<= _anything_stmt
     xonsh_command <<= _xonsh_command
 
 # end: MAIN GRAMMAR
```

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/compiler/header.py` & `coconut-develop-3.0.2.post0.dev7/coconut/compiler/header.py`

 * *Files 0% similar despite different names*

```diff
@@ -679,17 +679,22 @@
             newline=True,
         ),
         import_asyncio=pycondition(
             (3, 4),
             if_lt='''
 try:
     import trollius as asyncio
-except ImportError:
+except ImportError as trollius_import_error:
     class you_need_to_install_trollius{object}:
         __slots__ = ()
+        @staticmethod
+        def coroutine(func):
+            def raise_import_error(*args, **kwargs):
+                raise trollius_import_error
+            return raise_import_error
     asyncio = you_need_to_install_trollius()
             '''.format(**format_dict),
             if_ge='''
 import asyncio
             ''',
             indent=1,
         ),
```

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/compiler/matching.py` & `coconut-develop-3.0.2.post0.dev7/coconut/compiler/matching.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/compiler/templates/header.py_template` & `coconut-develop-3.0.2.post0.dev7/coconut/compiler/templates/header.py_template`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/compiler/util.py` & `coconut-develop-3.0.2.post0.dev7/coconut/compiler/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/constants.py` & `coconut-develop-3.0.2.post0.dev7/coconut/constants.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/convenience.py` & `coconut-develop-3.0.2.post0.dev7/coconut/convenience.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/convenience.pyi` & `coconut-develop-3.0.2.post0.dev7/coconut/convenience.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/exceptions.py` & `coconut-develop-3.0.2.post0.dev7/coconut/exceptions.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/highlighter.py` & `coconut-develop-3.0.2.post0.dev7/coconut/highlighter.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/icoconut/__init__.py` & `coconut-develop-3.0.2.post0.dev7/coconut/icoconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/icoconut/__main__.py` & `coconut-develop-3.0.2.post0.dev7/coconut/icoconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/icoconut/embed.py` & `coconut-develop-3.0.2.post0.dev7/coconut/icoconut/embed.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/icoconut/root.py` & `coconut-develop-3.0.2.post0.dev7/coconut/icoconut/root.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,23 +154,22 @@
 
     class CoconutSplitter(IPythonInputSplitter, object):
         """IPython splitter for Coconut."""
 
         def __init__(self, *args, **kwargs):
             """Version of __init__ that sets up Coconut code compilation."""
             super(CoconutSplitter, self).__init__(*args, **kwargs)
+            self._original_compile = self._compile
             self._compile = self._coconut_compile
 
         def _coconut_compile(self, source, *args, **kwargs):
             """Version of _compile that checks Coconut code.
             None means that the code should not be run as is.
             Any other value means that it can."""
-            if source.endswith("\n\n"):
-                return True
-            elif should_indent(source):
+            if not source.endswith("\n\n") and should_indent(source):
                 return None
             else:
                 return True
 
     INTERACTIVE_SHELL_CODE = '''
 input_splitter = CoconutSplitter(line_input_checker=True)
 input_transformer_manager = CoconutSplitter(line_input_checker=False)
```

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/integrations.py` & `coconut-develop-3.0.2.post0.dev7/coconut/integrations.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/main.py` & `coconut-develop-3.0.2.post0.dev7/coconut/main.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/requirements.py` & `coconut-develop-3.0.2.post0.dev7/coconut/requirements.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/root.py` & `coconut-develop-3.0.2.post0.dev7/coconut/root.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -----------------------------------------------------------------------------------------------------------------------
 # VERSION:
 # -----------------------------------------------------------------------------------------------------------------------
 
 VERSION = "3.0.2"
 VERSION_NAME = None
 # False for release, int >= 1 for develop
-DEVELOP = 6
+DEVELOP = 7
 ALPHA = False  # for pre releases rather than post releases
 
 assert DEVELOP is False or DEVELOP >= 1, "DEVELOP must be False or an int >= 1"
 assert DEVELOP or not ALPHA, "alpha releases are only for develop"
 
 # -----------------------------------------------------------------------------------------------------------------------
 # UTILITIES:
```

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/terminal.py` & `coconut-develop-3.0.2.post0.dev7/coconut/terminal.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/tests/__init__.py` & `coconut-develop-3.0.2.post0.dev7/coconut/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/tests/__main__.py` & `coconut-develop-3.0.2.post0.dev7/coconut/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/tests/constants_test.py` & `coconut-develop-3.0.2.post0.dev7/coconut/tests/constants_test.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/tests/main_test.py` & `coconut-develop-3.0.2.post0.dev7/coconut/tests/main_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -761,14 +761,17 @@
             p.sendline('echo f"{$ENV_VAR}"; echo f"{$ENV_VAR}"')
             p.expect("ABC")
             p.expect("ABC")
             if not PYPY or PY39:
                 if PY36:
                     p.sendline("echo 123;; 123")
                     p.expect("123;; 123")
+                    p.sendline("echo abc; echo abc")
+                    p.expect("abc")
+                    p.expect("abc")
                 p.sendline('execx("10 |> print")')
                 p.expect("subprocess mode")
             p.sendline("xontrib unload coconut")
             p.expect("$")
             if (not PYPY or PY39) and PY36:
                 p.sendline("1 |> print")
                 p.expect("subprocess mode")
```

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/agnostic/main.coco` & `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/main.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/agnostic/primary.coco` & `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/primary.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/agnostic/specific.coco` & `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/specific.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/agnostic/suite.coco` & `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/suite.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/agnostic/tutorial.coco` & `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/tutorial.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/agnostic/util.coco` & `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/util.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/non_strict/non_strict_test.coco` & `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/non_strict/non_strict_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/target_3/py3_test.coco` & `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_3/py3_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/target_35/py35_test.coco` & `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_35/py35_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/target_36/py36_test.coco` & `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_36/py36_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/tests/src/cocotest/target_sys/target_sys_test.coco` & `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_sys/target_sys_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/tests/src/extras.coco` & `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/extras.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut/util.py` & `coconut-develop-3.0.2.post0.dev7/coconut/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/coconut_develop.egg-info/SOURCES.txt` & `coconut-develop-3.0.2.post0.dev7/coconut_develop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/conf.py` & `coconut-develop-3.0.2.post0.dev7/conf.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/setup.py` & `coconut-develop-3.0.2.post0.dev7/setup.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev6/xontrib/coconut.py` & `coconut-develop-3.0.2.post0.dev7/xontrib/coconut.py`

 * *Files identical despite different names*

