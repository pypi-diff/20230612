# Comparing `tmp/argcomplete-3.1.0.tar.gz` & `tmp/argcomplete-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argcomplete-3.1.0.tar", last modified: Sat Jun 10 20:52:29 2023, max compression
+gzip compressed data, was "argcomplete-3.1.1.tar", last modified: Sun Jun 11 23:38:19 2023, max compression
```

## Comparing `argcomplete-3.1.0.tar` & `argcomplete-3.1.1.tar`

### file list

```diff
@@ -1,71 +1,69 @@
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.866948 argcomplete-3.1.0/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.857466 argcomplete-3.1.0/.github/
--rw-r--r--   0 kislyuk    (501) staff       (20)       18 2022-08-21 15:59:43.000000 argcomplete-3.1.0/.github/FUNDING.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.857724 argcomplete-3.1.0/.github/workflows/
--rw-r--r--   0 kislyuk    (501) staff       (20)      924 2023-04-22 14:28:37.000000 argcomplete-3.1.0/.github/workflows/ci.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)      474 2023-03-18 19:32:22.000000 argcomplete-3.1.0/.gitignore
--rw-r--r--   0 kislyuk    (501) staff       (20)       35 2016-06-14 14:20:26.000000 argcomplete-3.1.0/Authors.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)    12880 2023-06-10 20:52:11.000000 argcomplete-3.1.0/Changes.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)    10174 2016-06-14 14:20:26.000000 argcomplete-3.1.0/LICENSE.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)       79 2022-08-21 15:59:43.000000 argcomplete-3.1.0/MANIFEST.in
--rw-r--r--   0 kislyuk    (501) staff       (20)      766 2023-05-07 04:23:05.000000 argcomplete-3.1.0/Makefile
--rw-r--r--   0 kislyuk    (501) staff       (20)      387 2023-03-21 02:49:58.000000 argcomplete-3.1.0/NOTICE
--rw-r--r--   0 kislyuk    (501) staff       (20)    16334 2023-06-10 20:52:29.867092 argcomplete-3.1.0/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)    14690 2023-06-10 20:45:18.000000 argcomplete-3.1.0/README.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)      705 2023-03-05 19:47:13.000000 argcomplete-3.1.0/SECURITY.md
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.860163 argcomplete-3.1.0/argcomplete/
--rw-r--r--   0 kislyuk    (501) staff       (20)      693 2023-03-21 02:49:58.000000 argcomplete-3.1.0/argcomplete/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2719 2023-06-10 20:45:18.000000 argcomplete-3.1.0/argcomplete/_check_console_script.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2600 2023-03-18 19:32:22.000000 argcomplete-3.1.0/argcomplete/_check_module.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.861117 argcomplete-3.1.0/argcomplete/bash_completion.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)     8165 2023-06-10 20:45:18.000000 argcomplete-3.1.0/argcomplete/bash_completion.d/_python-argcomplete
--rw-r--r--   0 kislyuk    (501) staff       (20)     3980 2023-03-26 15:30:13.000000 argcomplete-3.1.0/argcomplete/completers.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      112 2023-03-19 18:35:55.000000 argcomplete-3.1.0/argcomplete/exceptions.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    26975 2023-03-26 15:30:13.000000 argcomplete-3.1.0/argcomplete/finders.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      866 2023-03-19 18:46:34.000000 argcomplete-3.1.0/argcomplete/io.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2131 2023-03-21 02:49:58.000000 argcomplete-3.1.0/argcomplete/lexers.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.861555 argcomplete-3.1.0/argcomplete/packages/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2023-03-19 10:11:13.000000 argcomplete-3.1.0/argcomplete/packages/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    15846 2023-03-19 18:59:55.000000 argcomplete-3.1.0/argcomplete/packages/_argparse.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    12766 2023-03-18 19:32:22.000000 argcomplete-3.1.0/argcomplete/packages/_shlex.py
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2023-03-18 19:32:22.000000 argcomplete-3.1.0/argcomplete/py.typed
--rw-r--r--   0 kislyuk    (501) staff       (20)     7012 2023-04-22 14:28:37.000000 argcomplete-3.1.0/argcomplete/shell_integration.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.861020 argcomplete-3.1.0/argcomplete.egg-info/
--rw-r--r--   0 kislyuk    (501) staff       (20)    16334 2023-06-10 20:52:29.000000 argcomplete-3.1.0/argcomplete.egg-info/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)     1323 2023-06-10 20:52:29.000000 argcomplete-3.1.0/argcomplete.egg-info/SOURCES.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-06-10 20:52:29.000000 argcomplete-3.1.0/argcomplete.egg-info/dependency_links.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-06-10 20:52:19.000000 argcomplete-3.1.0/argcomplete.egg-info/not-zip-safe
--rw-r--r--   0 kislyuk    (501) staff       (20)       96 2023-06-10 20:52:29.000000 argcomplete-3.1.0/argcomplete.egg-info/requires.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)       12 2023-06-10 20:52:29.000000 argcomplete-3.1.0/argcomplete.egg-info/top_level.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)     2214 2023-06-10 20:45:18.000000 argcomplete-3.1.0/common.mk
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.861786 argcomplete-3.1.0/contrib/
--rw-r--r--   0 kislyuk    (501) staff       (20)     2888 2023-04-22 14:28:37.000000 argcomplete-3.1.0/contrib/README.rst
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.863021 argcomplete-3.1.0/docs/
--rw-r--r--   0 kislyuk    (501) staff       (20)       56 2023-05-06 23:05:14.000000 argcomplete-3.1.0/docs/changelog.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)     1162 2023-05-07 04:24:09.000000 argcomplete-3.1.0/docs/conf.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.863337 argcomplete-3.1.0/docs/examples/
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      721 2022-09-14 03:21:59.000000 argcomplete-3.1.0/docs/examples/describe_github_user.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    14171 2022-08-21 15:59:43.000000 argcomplete-3.1.0/docs/fish_help_string.png
--rw-r--r--   0 kislyuk    (501) staff       (20)      293 2023-05-06 23:04:09.000000 argcomplete-3.1.0/docs/index.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)        8 2023-05-06 23:03:19.000000 argcomplete-3.1.0/docs/toc.html
--rw-r--r--   0 kislyuk    (501) staff       (20)     2083 2023-06-10 20:45:18.000000 argcomplete-3.1.0/pyproject.toml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.863855 argcomplete-3.1.0/scripts/
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     4710 2023-06-10 20:45:18.000000 argcomplete-3.1.0/scripts/activate-global-python-argcomplete
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     2608 2023-06-10 20:45:18.000000 argcomplete-3.1.0/scripts/python-argcomplete-check-easy-install-script
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     1997 2023-04-22 14:28:37.000000 argcomplete-3.1.0/scripts/register-python-argcomplete
--rw-r--r--   0 kislyuk    (501) staff       (20)      143 2023-06-10 20:52:29.867442 argcomplete-3.1.0/setup.cfg
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      408 2023-06-10 20:45:18.000000 argcomplete-3.1.0/setup.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.866106 argcomplete-3.1.0/test/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-06-14 14:20:26.000000 argcomplete-3.1.0/test/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      139 2016-06-16 15:02:13.000000 argcomplete-3.1.0/test/__init__.pyc
--rw-r--r--   0 kislyuk    (501) staff       (20)       31 2023-03-05 19:47:13.000000 argcomplete-3.1.0/test/inputrc
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     1764 2023-06-10 20:45:18.000000 argcomplete-3.1.0/test/prog
--rwxr-xr-x   0 kislyuk    (501) staff       (20)    59360 2023-05-06 22:57:27.000000 argcomplete-3.1.0/test/test.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    31570 2016-10-16 02:47:39.000000 argcomplete-3.1.0/test/test.pyc
--rw-r--r--   0 kislyuk    (501) staff       (20)     3183 2023-03-18 19:32:22.000000 argcomplete-3.1.0/test/test_contrib_shells.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.866590 argcomplete-3.1.0/test/test_package/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2023-03-05 19:47:13.000000 argcomplete-3.1.0/test/test_package/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      299 2022-09-14 03:21:59.000000 argcomplete-3.1.0/test/test_package/setup.py
--rw-r--r--   0 kislyuk    (501) staff       (20)       94 2022-09-14 03:21:59.000000 argcomplete-3.1.0/test/test_package/test_module.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-06-10 20:52:29.866822 argcomplete-3.1.0/test/test_package/test_package/
--rw-r--r--   0 kislyuk    (501) staff       (20)      289 2022-09-14 03:21:59.000000 argcomplete-3.1.0/test/test_package/test_package/__init__.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-06-11 23:38:19.719662 argcomplete-3.1.1/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-06-11 23:38:19.666544 argcomplete-3.1.1/.github/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       18 2021-06-26 14:08:42.000000 argcomplete-3.1.1/.github/FUNDING.yml
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-06-11 23:38:19.667503 argcomplete-3.1.1/.github/workflows/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      924 2023-04-23 21:34:49.000000 argcomplete-3.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      474 2023-03-06 19:37:04.000000 argcomplete-3.1.1/.gitignore
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       35 2021-06-26 14:08:42.000000 argcomplete-3.1.1/Authors.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    13027 2023-06-11 23:37:42.000000 argcomplete-3.1.1/Changes.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    10174 2021-06-26 14:08:42.000000 argcomplete-3.1.1/LICENSE.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       79 2021-06-26 14:08:42.000000 argcomplete-3.1.1/MANIFEST.in
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      766 2023-06-03 15:24:48.000000 argcomplete-3.1.1/Makefile
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      387 2023-03-21 01:42:51.000000 argcomplete-3.1.1/NOTICE
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    16334 2023-06-11 23:38:19.720147 argcomplete-3.1.1/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    14690 2023-06-10 20:21:43.000000 argcomplete-3.1.1/README.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      705 2023-03-05 05:26:24.000000 argcomplete-3.1.1/SECURITY.md
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-06-11 23:38:19.678867 argcomplete-3.1.1/argcomplete/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      693 2023-03-21 01:39:54.000000 argcomplete-3.1.1/argcomplete/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2719 2023-06-05 16:46:08.000000 argcomplete-3.1.1/argcomplete/_check_console_script.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2600 2023-03-17 18:26:27.000000 argcomplete-3.1.1/argcomplete/_check_module.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-06-11 23:38:19.683069 argcomplete-3.1.1/argcomplete/bash_completion.d/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8413 2023-06-11 23:31:03.000000 argcomplete-3.1.1/argcomplete/bash_completion.d/_python-argcomplete
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3980 2023-03-29 02:42:12.000000 argcomplete-3.1.1/argcomplete/completers.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      112 2023-03-19 19:40:27.000000 argcomplete-3.1.1/argcomplete/exceptions.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    27230 2023-06-11 23:35:19.000000 argcomplete-3.1.1/argcomplete/finders.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      866 2023-03-19 19:40:27.000000 argcomplete-3.1.1/argcomplete/io.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2131 2023-03-21 01:39:33.000000 argcomplete-3.1.1/argcomplete/lexers.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-06-11 23:38:19.698250 argcomplete-3.1.1/argcomplete/packages/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-03-19 19:40:27.000000 argcomplete-3.1.1/argcomplete/packages/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    15846 2023-03-19 19:40:27.000000 argcomplete-3.1.1/argcomplete/packages/_argparse.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    12766 2023-03-19 19:40:27.000000 argcomplete-3.1.1/argcomplete/packages/_shlex.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-03-17 19:10:26.000000 argcomplete-3.1.1/argcomplete/py.typed
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     7080 2023-06-11 23:34:29.000000 argcomplete-3.1.1/argcomplete/shell_integration.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-06-11 23:38:19.682597 argcomplete-3.1.1/argcomplete.egg-info/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    16334 2023-06-11 23:38:19.000000 argcomplete-3.1.1/argcomplete.egg-info/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1291 2023-06-11 23:38:19.000000 argcomplete-3.1.1/argcomplete.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2023-06-11 23:38:19.000000 argcomplete-3.1.1/argcomplete.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2023-06-11 23:37:54.000000 argcomplete-3.1.1/argcomplete.egg-info/not-zip-safe
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       96 2023-06-11 23:38:19.000000 argcomplete-3.1.1/argcomplete.egg-info/requires.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       12 2023-06-11 23:38:19.000000 argcomplete-3.1.1/argcomplete.egg-info/top_level.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2214 2023-06-11 23:26:52.000000 argcomplete-3.1.1/common.mk
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-06-11 23:38:19.699242 argcomplete-3.1.1/contrib/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2888 2023-04-23 21:34:49.000000 argcomplete-3.1.1/contrib/README.rst
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-06-11 23:38:19.705174 argcomplete-3.1.1/docs/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       56 2023-06-03 15:24:48.000000 argcomplete-3.1.1/docs/changelog.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1162 2023-06-03 15:24:48.000000 argcomplete-3.1.1/docs/conf.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-06-11 23:38:19.706356 argcomplete-3.1.1/docs/examples/
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)      721 2023-03-04 23:22:21.000000 argcomplete-3.1.1/docs/examples/describe_github_user.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    14171 2021-06-26 14:08:42.000000 argcomplete-3.1.1/docs/fish_help_string.png
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      293 2023-06-03 15:24:48.000000 argcomplete-3.1.1/docs/index.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        8 2023-06-03 15:24:48.000000 argcomplete-3.1.1/docs/toc.html
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2074 2023-06-11 23:26:52.000000 argcomplete-3.1.1/pyproject.toml
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-06-11 23:38:19.710281 argcomplete-3.1.1/scripts/
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     4710 2023-06-10 20:21:43.000000 argcomplete-3.1.1/scripts/activate-global-python-argcomplete
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     2608 2023-06-10 20:21:43.000000 argcomplete-3.1.1/scripts/python-argcomplete-check-easy-install-script
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1997 2023-04-23 21:34:49.000000 argcomplete-3.1.1/scripts/register-python-argcomplete
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      143 2023-06-11 23:38:19.721526 argcomplete-3.1.1/setup.cfg
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)      408 2023-06-11 23:26:52.000000 argcomplete-3.1.1/setup.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-06-11 23:38:19.715016 argcomplete-3.1.1/test/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2021-06-26 14:08:42.000000 argcomplete-3.1.1/test/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       31 2023-03-04 23:22:21.000000 argcomplete-3.1.1/test/inputrc
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1764 2023-06-10 20:21:43.000000 argcomplete-3.1.1/test/prog
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    59360 2023-04-23 21:44:19.000000 argcomplete-3.1.1/test/test.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3183 2023-03-17 17:41:01.000000 argcomplete-3.1.1/test/test_contrib_shells.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-06-11 23:38:19.717888 argcomplete-3.1.1/test/test_package/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2023-03-04 23:22:21.000000 argcomplete-3.1.1/test/test_package/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      299 2023-03-04 23:22:21.000000 argcomplete-3.1.1/test/test_package/setup.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       94 2023-03-04 23:22:21.000000 argcomplete-3.1.1/test/test_package/test_module.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-06-11 23:38:19.718923 argcomplete-3.1.1/test/test_package/test_package/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      289 2023-03-04 23:22:21.000000 argcomplete-3.1.1/test/test_package/test_package/__init__.py
```

### Comparing `argcomplete-3.1.0/.github/workflows/ci.yml` & `argcomplete-3.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/Changes.rst` & `argcomplete-3.1.1/Changes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Changes for v3.1.1 (2023-06-11)
+===============================
+
+-  Search through asdf shims
+
+-  Use \` as escape character in PowerShell (#434)
+
 Changes for v3.1.0 (2023-06-10)
 ===============================
 
 -  setup.py -> pyproject.toml migration start (#427)
 
 -  Improve user install logic in activate-global-python-argcomplete
    (#437)
```

### Comparing `argcomplete-3.1.0/LICENSE.rst` & `argcomplete-3.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/Makefile` & `argcomplete-3.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/PKG-INFO` & `argcomplete-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argcomplete
-Version: 3.1.0
+Version: 3.1.1
 Summary: Bash tab completion for argparse
 Home-page: https://github.com/kislyuk/argcomplete
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Project-URL: Documentation, https://kislyuk.github.io/argcomplete
 Project-URL: Source Code, https://github.com/kislyuk/argcomplete
```

### Comparing `argcomplete-3.1.0/README.rst` & `argcomplete-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/SECURITY.md` & `argcomplete-3.1.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/argcomplete/__init__.py` & `argcomplete-3.1.1/argcomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/argcomplete/_check_console_script.py` & `argcomplete-3.1.1/argcomplete/_check_console_script.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/argcomplete/_check_module.py` & `argcomplete-3.1.1/argcomplete/_check_module.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/argcomplete/bash_completion.d/_python-argcomplete` & `argcomplete-3.1.1/argcomplete/bash_completion.d/_python-argcomplete`

 * *Files 4% similar despite different names*

```diff
@@ -53,20 +53,20 @@
     else
         _BASH_REMATCH=( "${BASH_REMATCH[@]}" )
     fi
 }
 
 # This function scans the beginning of an executable file provided as the first
 # argument ($1) for certain indicators, specified by the second argument ($2),
-# or the "target".  There are three possible targets: "interpreter",
+# or the "target". There are three possible targets: "interpreter",
 # "magic_string", and "easy_install". If the target is "interpreter", the
 # function matches the interpreter line, alongside any optional interpreter
 # arguments. If the target is "magic_string", a match is attempted for the
-# "PYTHON_ARGCOMPLETE_OK" magic string, indicating that the file should be
-# searched.  If the target is "easy_install", the function matches either
+# "PYTHON_ARGCOMPLETE_OK" magic string, indicating that the file should be run
+# to get completions. If the target is "easy_install", the function matches either
 # "PBR Generated" or any of the "EASY-INSTALL" scripts (either SCRIPT,
 # ENTRY-SCRIPT, or DEV-SCRIPT). In all cases, only the first kilobyte of
 # the file is searched. The regex matches are returned in BASH_REMATCH,
 # indexed starting at 1, regardless of the shell in use.
 __python_argcomplete_scan_head() {
     local file="$1"
     local target="$2"
@@ -84,14 +84,15 @@
     fi
 
     local regex
 
     case "$target" in
             magic_string) regex='PYTHON_ARGCOMPLETE_OK' ;;
             easy_install) regex="(PBR Generated)|(EASY-INSTALL-(SCRIPT|ENTRY-SCRIPT|DEV-SCRIPT))" ;;
+            asdf) regex="asdf exec " ;;
             interpreter) regex='^#!(.*)$' ;;
     esac
 
     local ret=""
     if [[ "$REPLY" =~ $regex ]]; then
         ret=1
     fi
@@ -166,14 +167,17 @@
         fi
     elif __python_argcomplete_which "$executable" >/dev/null 2>&1; then
         local SCRIPT_NAME=$(__python_argcomplete_which "$executable")
         __python_argcomplete_scan_head_noerr "$SCRIPT_NAME" interpreter
         if (__python_argcomplete_which pyenv && [[ "$SCRIPT_NAME" = $(pyenv root)/shims/* ]]) >/dev/null 2>&1; then
             local SCRIPT_NAME=$(pyenv which "$executable")
         fi
+        if (__python_argcomplete_which asdf && __python_argcomplete_scan_head_noerr "$SCRIPT_NAME" asdf) >/dev/null 2>&1; then
+            local SCRIPT_NAME=$(asdf which "$executable")
+        fi
         if __python_argcomplete_scan_head_noerr "$SCRIPT_NAME" magic_string; then
             ARGCOMPLETE=1
         elif __python_argcomplete_scan_head_noerr "$SCRIPT_NAME" interpreter; then
             __python_argcomplete_upshift_bash_rematch
             local interpreter="${_BASH_REMATCH[2]}"
 
             if [[ -n "${ZSH_VERSION-}" ]]; then
```

### Comparing `argcomplete-3.1.0/argcomplete/completers.py` & `argcomplete-3.1.1/argcomplete/completers.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/argcomplete/finders.py` & `argcomplete-3.1.1/argcomplete/finders.py`

 * *Files 1% similar despite different names*

```diff
@@ -515,16 +515,22 @@
             special_chars = ""
         elif cword_prequote == "'":
             # Nothing can be escaped in single quotes, so we need to close
             # the string, escape the single quote, then open a new string.
             special_chars = ""
             completions = [c.replace("'", r"'\''") for c in completions]
 
+        # PowerShell uses ` as escape character.
+        if os.environ.get("_ARGCOMPLETE_SHELL") == "powershell":
+            escape_char = '`'
+            special_chars = special_chars.replace('`', '')
+        else:
+            escape_char = "\\"
         for char in special_chars:
-            completions = [c.replace(char, "\\" + char) for c in completions]
+            completions = [c.replace(char, escape_char + char) for c in completions]
 
         if self.append_space:
             # Similar functionality in bash was previously turned off by supplying the "-o nospace" option to complete.
             # Now it is conditionally disabled using "compopt -o nospace" if the match ends in a continuation character.
             # This code is retained for environments where this isn't done natively.
             continuation_chars = "=/:"
             if len(completions) == 1 and completions[0][-1] not in continuation_chars:
```

### Comparing `argcomplete-3.1.0/argcomplete/io.py` & `argcomplete-3.1.1/argcomplete/io.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/argcomplete/lexers.py` & `argcomplete-3.1.1/argcomplete/lexers.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/argcomplete/packages/_argparse.py` & `argcomplete-3.1.1/argcomplete/packages/_argparse.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/argcomplete/packages/_shlex.py` & `argcomplete-3.1.1/argcomplete/packages/_shlex.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/argcomplete/shell_integration.py` & `argcomplete-3.1.1/argcomplete/shell_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,21 +101,22 @@
     $env:ARGCOMPLETE_USE_TEMPFILES = 1
     $env:_ARGCOMPLETE_STDOUT_FILENAME = $completion_file
     $env:COMP_LINE = $wordToComplete
     $env:COMP_POINT = $cursorPosition
     $env:_ARGCOMPLETE = 1
     $env:_ARGCOMPLETE_SUPPRESS_SPACE = 0
     $env:_ARGCOMPLETE_IFS = "`n"
+    $env:_ARGCOMPLETE_SHELL = "powershell"
     %(argcomplete_script)s 2>&1 | Out-Null
 
     Get-Content $completion_file | ForEach-Object {
         [System.Management.Automation.CompletionResult]::new($_, $_, "ParameterValue", $_)
     }
     rm $completion_file
-    Remove-Item Env:\_ARGCOMPLETE_STDOUT_FILENAME, Env:\ARGCOMPLETE_USE_TEMPFILES, Env:\COMP_LINE, Env:\COMP_POINT, Env:\_ARGCOMPLETE, Env:\_ARGCOMPLETE_SUPPRESS_SPACE, Env:\_ARGCOMPLETE_IFS
+    Remove-Item Env:\_ARGCOMPLETE_STDOUT_FILENAME, Env:\ARGCOMPLETE_USE_TEMPFILES, Env:\COMP_LINE, Env:\COMP_POINT, Env:\_ARGCOMPLETE, Env:\_ARGCOMPLETE_SUPPRESS_SPACE, Env:\_ARGCOMPLETE_IFS, Env:\_ARGCOMPLETE_SHELL
 }
 """  # noqa: E501
 
 shell_codes = {"bash": bashcode, "tcsh": tcshcode, "fish": fishcode, "powershell": powershell_code}
 
 
 def shellcode(executables, use_defaults=True, shell="bash", complete_arguments=None, argcomplete_script=None):
```

### Comparing `argcomplete-3.1.0/argcomplete.egg-info/PKG-INFO` & `argcomplete-3.1.1/argcomplete.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argcomplete
-Version: 3.1.0
+Version: 3.1.1
 Summary: Bash tab completion for argparse
 Home-page: https://github.com/kislyuk/argcomplete
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Project-URL: Documentation, https://kislyuk.github.io/argcomplete
 Project-URL: Source Code, https://github.com/kislyuk/argcomplete
```

### Comparing `argcomplete-3.1.0/argcomplete.egg-info/SOURCES.txt` & `argcomplete-3.1.1/argcomplete.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,15 @@
 docs/index.rst
 docs/toc.html
 docs/examples/describe_github_user.py
 scripts/activate-global-python-argcomplete
 scripts/python-argcomplete-check-easy-install-script
 scripts/register-python-argcomplete
 test/__init__.py
-test/__init__.pyc
 test/inputrc
 test/prog
 test/test.py
-test/test.pyc
 test/test_contrib_shells.py
 test/test_package/__init__.py
 test/test_package/setup.py
 test/test_package/test_module.py
 test/test_package/test_package/__init__.py
```

### Comparing `argcomplete-3.1.0/common.mk` & `argcomplete-3.1.1/common.mk`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/contrib/README.rst` & `argcomplete-3.1.1/contrib/README.rst`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/docs/conf.py` & `argcomplete-3.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/docs/examples/describe_github_user.py` & `argcomplete-3.1.1/docs/examples/describe_github_user.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/docs/fish_help_string.png` & `argcomplete-3.1.1/docs/fish_help_string.png`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/pyproject.toml` & `argcomplete-3.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=67.7.2", "wheel", "setuptools_scm[toml]>=6.2"]
+requires = ["setuptools>=67.7.2", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "argcomplete"
 description = "Bash tab completion for argparse"
 readme = "README.rst"
 requires-python = ">=3.6"
```

### Comparing `argcomplete-3.1.0/scripts/activate-global-python-argcomplete` & `argcomplete-3.1.1/scripts/activate-global-python-argcomplete`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/scripts/python-argcomplete-check-easy-install-script` & `argcomplete-3.1.1/scripts/python-argcomplete-check-easy-install-script`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/scripts/register-python-argcomplete` & `argcomplete-3.1.1/scripts/register-python-argcomplete`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/test/prog` & `argcomplete-3.1.1/test/prog`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/test/test.py` & `argcomplete-3.1.1/test/test.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.1.0/test/test_contrib_shells.py` & `argcomplete-3.1.1/test/test_contrib_shells.py`

 * *Files identical despite different names*

