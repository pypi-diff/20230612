# Comparing `tmp/cs.psutils-20221228.tar.gz` & `tmp/cs.psutils-20230612.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.psutils-20221228.tar", last modified: Tue Dec 27 23:41:59 2022, max compression
+gzip compressed data, was "cs.psutils-20230612.tar", last modified: Mon Jun 12 03:16:36 2023, max compression
```

## Comparing `cs.psutils-20221228.tar` & `cs.psutils-20230612.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-12-27 23:41:59.730325 cs.psutils-20221228/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2022-12-27 23:41:28.000000 cs.psutils-20221228/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     8053 2022-12-27 23:41:59.730475 cs.psutils-20221228/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     7169 2022-12-27 23:41:33.000000 cs.psutils-20221228/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-12-27 23:41:59.725649 cs.psutils-20221228/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-12-27 23:41:59.725951 cs.psutils-20221228/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-12-27 23:41:59.727914 cs.psutils-20221228/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    12516 2022-12-27 23:41:20.000000 cs.psutils-20221228/lib/python/cs/psutils.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-12-27 23:41:59.730001 cs.psutils-20221228/lib/python/cs.psutils.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     8053 2022-12-27 23:41:59.000000 cs.psutils-20221228/lib/python/cs.psutils.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      304 2022-12-27 23:41:59.000000 cs.psutils-20221228/lib/python/cs.psutils.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2022-12-27 23:41:59.000000 cs.psutils-20221228/lib/python/cs.psutils.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       39 2022-12-27 23:41:59.000000 cs.psutils-20221228/lib/python/cs.psutils.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2022-12-27 23:41:59.000000 cs.psutils-20221228/lib/python/cs.psutils.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     8248 2022-12-27 23:41:49.000000 cs.psutils-20221228/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)      897 2022-12-27 23:41:59.731171 cs.psutils-20221228/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2022-12-27 23:41:33.000000 cs.psutils-20221228/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:16:36.804571 cs.psutils-20230612/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-12 03:16:06.000000 cs.psutils-20230612/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     7640 2023-06-12 03:16:36.804704 cs.psutils-20230612/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6804 2023-06-12 03:16:11.000000 cs.psutils-20230612/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:16:36.799026 cs.psutils-20230612/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:16:36.799438 cs.psutils-20230612/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:16:36.801692 cs.psutils-20230612/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    11812 2023-06-12 03:15:57.000000 cs.psutils-20230612/lib/python/cs/psutils.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:16:36.804220 cs.psutils-20230612/lib/python/cs.psutils.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     7640 2023-06-12 03:16:36.000000 cs.psutils-20230612/lib/python/cs.psutils.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      304 2023-06-12 03:16:36.000000 cs.psutils-20230612/lib/python/cs.psutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-12 03:16:36.000000 cs.psutils-20230612/lib/python/cs.psutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       39 2023-06-12 03:16:36.000000 cs.psutils-20230612/lib/python/cs.psutils.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-12 03:16:36.000000 cs.psutils-20230612/lib/python/cs.psutils.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     7838 2023-06-12 03:16:28.000000 cs.psutils-20230612/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)      860 2023-06-12 03:16:36.805380 cs.psutils-20230612/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-12 03:16:11.000000 cs.psutils-20230612/setup.py
```

### Comparing `cs.psutils-20221228/PKG-INFO` & `cs.psutils-20230612/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: cs.psutils
-Version: 20221228
+Version: 20230612
 Summary: Assorted process and subprocess management functions.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted process and subprocess management functions.
 
-*Latest release 20221228*:
-* signal_handlers: bugfix iteration of sig_hnds.
-* Use cs.gimmicks instead of cs.logutils.
-* Drop use of cs.upd, fixes circular import; users of run() may need to call "with Upd().above()" themselves.
+*Latest release 20230612*:
+* pipefrom: default stdin=DEVNULL.
+* Make many parameters keyword only.
 
 ## Function `groupargv(pre_argv, argv, post_argv=(), max_argv=None, encode=False)`
 
 Distribute the array `argv` over multiple arrays
 to fit within `MAX_ARGV`.
 Return a list of argv lists.
 
@@ -56,39 +54,28 @@
 * `path`: the path to the process id file.
 * `pid`: the process id to store in the pid file,
   default from `os.etpid`.
 
 Writes the process id file at the start
 and removes the process id file at the end.
 
-## Function `pipefrom(argv, quiet=False, binary=False, keep_stdin=False, **kw)`
+## Function `pipefrom(argv, *, quiet=False, text=True, stdin=-3, **popen_kw)`
 
-Pipe text from a command.
-Optionally trace invocation.
-Return the `Popen` object with `.stdout` decoded as text.
+Pipe text (usually) from a command using `subprocess.Popen`.
+Return the `Popen` object with `.stdout` as a pipe.
 
 Parameters:
 * `argv`: the command argument list
-* `binary`: if true (default false)
-  return the raw stdout instead of a text wrapper
 * `quiet`: optional flag, default `False`;
+  if true, print the command to `stderr`
+* `text`: optional flag, default `True`; passed to `Popen`.
+* `stdin`: optional value for `Popen`'s `stdin`, default `DEVNULL`
+Other keyword arguments are passed to `Popen`.
 
-  if `trace` is `True`, recite invocation to stderr
-  otherwise presume that `trace` is a stream
-  to which to recite the invocation.
-* `keep_stdin`: if true (default `False`)
-  do not attach the command's standard input to the null device.
-  The default behaviour is to do so,
-  preventing commands from accidentally
-  consuming the main process' input stream.
-
-Other keyword arguments are passed to the `io.TextIOWrapper`
-which wraps the command's output.
-
-## Function `pipeto(argv, quiet=False, **kw)`
+## Function `pipeto(argv, *, quiet=False, **kw)`
 
 Pipe text to a command.
 Optionally trace invocation.
 Return the Popen object with .stdin encoded as text.
 
 Parameters:
 * `argv`: the command argument list
@@ -175,14 +162,18 @@
 * `path`: the path to the pid file.
 * `pid`: the process id to write, defautl from `os.getpid`.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* pipefrom: default stdin=DEVNULL.
+* Make many parameters keyword only.
+
 *Release 20221228*:
 * signal_handlers: bugfix iteration of sig_hnds.
 * Use cs.gimmicks instead of cs.logutils.
 * Drop use of cs.upd, fixes circular import; users of run() may need to call "with Upd().above()" themselves.
 
 *Release 20221118*:
 run: do not print cp.stdout.
```

### Comparing `cs.psutils-20221228/README.md` & `cs.psutils-20230612/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Assorted process and subprocess management functions.
 
-*Latest release 20221228*:
-* signal_handlers: bugfix iteration of sig_hnds.
-* Use cs.gimmicks instead of cs.logutils.
-* Drop use of cs.upd, fixes circular import; users of run() may need to call "with Upd().above()" themselves.
+*Latest release 20230612*:
+* pipefrom: default stdin=DEVNULL.
+* Make many parameters keyword only.
 
 ## Function `groupargv(pre_argv, argv, post_argv=(), max_argv=None, encode=False)`
 
 Distribute the array `argv` over multiple arrays
 to fit within `MAX_ARGV`.
 Return a list of argv lists.
 
@@ -36,39 +35,28 @@
 * `path`: the path to the process id file.
 * `pid`: the process id to store in the pid file,
   default from `os.etpid`.
 
 Writes the process id file at the start
 and removes the process id file at the end.
 
-## Function `pipefrom(argv, quiet=False, binary=False, keep_stdin=False, **kw)`
+## Function `pipefrom(argv, *, quiet=False, text=True, stdin=-3, **popen_kw)`
 
-Pipe text from a command.
-Optionally trace invocation.
-Return the `Popen` object with `.stdout` decoded as text.
+Pipe text (usually) from a command using `subprocess.Popen`.
+Return the `Popen` object with `.stdout` as a pipe.
 
 Parameters:
 * `argv`: the command argument list
-* `binary`: if true (default false)
-  return the raw stdout instead of a text wrapper
 * `quiet`: optional flag, default `False`;
+  if true, print the command to `stderr`
+* `text`: optional flag, default `True`; passed to `Popen`.
+* `stdin`: optional value for `Popen`'s `stdin`, default `DEVNULL`
+Other keyword arguments are passed to `Popen`.
 
-  if `trace` is `True`, recite invocation to stderr
-  otherwise presume that `trace` is a stream
-  to which to recite the invocation.
-* `keep_stdin`: if true (default `False`)
-  do not attach the command's standard input to the null device.
-  The default behaviour is to do so,
-  preventing commands from accidentally
-  consuming the main process' input stream.
-
-Other keyword arguments are passed to the `io.TextIOWrapper`
-which wraps the command's output.
-
-## Function `pipeto(argv, quiet=False, **kw)`
+## Function `pipeto(argv, *, quiet=False, **kw)`
 
 Pipe text to a command.
 Optionally trace invocation.
 Return the Popen object with .stdin encoded as text.
 
 Parameters:
 * `argv`: the command argument list
@@ -155,14 +143,18 @@
 * `path`: the path to the pid file.
 * `pid`: the process id to write, defautl from `os.getpid`.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* pipefrom: default stdin=DEVNULL.
+* Make many parameters keyword only.
+
 *Release 20221228*:
 * signal_handlers: bugfix iteration of sig_hnds.
 * Use cs.gimmicks instead of cs.logutils.
 * Drop use of cs.upd, fixes circular import; users of run() may need to call "with Upd().above()" themselves.
 
 *Release 20221118*:
 run: do not print cp.stdout.
```

### Comparing `cs.psutils-20221228/lib/python/cs/psutils.py` & `cs.psutils-20230612/lib/python/cs/psutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,21 +15,20 @@
 from subprocess import PIPE, Popen, run as subprocess_run
 import sys
 import time
 
 from cs.gimmicks import trace, warning, DEVNULL
 from cs.pfx import pfx_call
 
-__version__ = '20221228'
+__version__ = '20230612'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
     ],
     'install_requires': [
         'cs.gimmicks>=devnull',
         'cs.pfx',
     ],
 }
@@ -229,53 +228,31 @@
     warning(
         "run fails, exit code %s from %s",
         cp.returncode,
         shlex.join(cp.args),
     )
   return cp
 
-def pipefrom(argv, quiet=False, binary=False, keep_stdin=False, **kw):
-  ''' Pipe text from a command.
-      Optionally trace invocation.
-      Return the `Popen` object with `.stdout` decoded as text.
+def pipefrom(argv, *, quiet=False, text=True, stdin=DEVNULL, **popen_kw):
+  ''' Pipe text (usually) from a command using `subprocess.Popen`.
+      Return the `Popen` object with `.stdout` as a pipe.
 
       Parameters:
       * `argv`: the command argument list
-      * `binary`: if true (default false)
-        return the raw stdout instead of a text wrapper
       * `quiet`: optional flag, default `False`;
-
-        if `trace` is `True`, recite invocation to stderr
-        otherwise presume that `trace` is a stream
-        to which to recite the invocation.
-      * `keep_stdin`: if true (default `False`)
-        do not attach the command's standard input to the null device.
-        The default behaviour is to do so,
-        preventing commands from accidentally
-        consuming the main process' input stream.
-
-      Other keyword arguments are passed to the `io.TextIOWrapper`
-      which wraps the command's output.
+        if true, print the command to `stderr`
+      * `text`: optional flag, default `True`; passed to `Popen`.
+      * `stdin`: optional value for `Popen`'s `stdin`, default `DEVNULL`
+      Other keyword arguments are passed to `Popen`.
   '''
   if not quiet:
     print_argv(*argv, indent="+ ", end=" |\n", file=sys.stderr)
-  popen_kw = {}
-  if not keep_stdin:
-    popen_kw['stdin'] = DEVNULL
-  P = Popen(argv, stdout=PIPE, **popen_kw)  # pylint: disable=consider-using-with
-  if binary:
-    if kw:
-      raise ValueError(
-          "binary mode: extra keyword arguments not supported: %r" % (kw,)
-      )
-  else:
-    P.stdout = io.TextIOWrapper(P.stdout, **kw)
-  return P
+  return Popen(argv, stdout=PIPE, text=text, stdin=stdin, **popen_kw)
 
-def pipeto(argv, quiet=False, **kw):
+def pipeto(argv, *, quiet=False, **kw):
   ''' Pipe text to a command.
       Optionally trace invocation.
       Return the Popen object with .stdin encoded as text.
 
       Parameters:
       * `argv`: the command argument list
       * `trace`: if true (default `False`),
```

### Comparing `cs.psutils-20221228/lib/python/cs.psutils.egg-info/PKG-INFO` & `cs.psutils-20230612/lib/python/cs.psutils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: cs.psutils
-Version: 20221228
+Version: 20230612
 Summary: Assorted process and subprocess management functions.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted process and subprocess management functions.
 
-*Latest release 20221228*:
-* signal_handlers: bugfix iteration of sig_hnds.
-* Use cs.gimmicks instead of cs.logutils.
-* Drop use of cs.upd, fixes circular import; users of run() may need to call "with Upd().above()" themselves.
+*Latest release 20230612*:
+* pipefrom: default stdin=DEVNULL.
+* Make many parameters keyword only.
 
 ## Function `groupargv(pre_argv, argv, post_argv=(), max_argv=None, encode=False)`
 
 Distribute the array `argv` over multiple arrays
 to fit within `MAX_ARGV`.
 Return a list of argv lists.
 
@@ -56,39 +54,28 @@
 * `path`: the path to the process id file.
 * `pid`: the process id to store in the pid file,
   default from `os.etpid`.
 
 Writes the process id file at the start
 and removes the process id file at the end.
 
-## Function `pipefrom(argv, quiet=False, binary=False, keep_stdin=False, **kw)`
+## Function `pipefrom(argv, *, quiet=False, text=True, stdin=-3, **popen_kw)`
 
-Pipe text from a command.
-Optionally trace invocation.
-Return the `Popen` object with `.stdout` decoded as text.
+Pipe text (usually) from a command using `subprocess.Popen`.
+Return the `Popen` object with `.stdout` as a pipe.
 
 Parameters:
 * `argv`: the command argument list
-* `binary`: if true (default false)
-  return the raw stdout instead of a text wrapper
 * `quiet`: optional flag, default `False`;
+  if true, print the command to `stderr`
+* `text`: optional flag, default `True`; passed to `Popen`.
+* `stdin`: optional value for `Popen`'s `stdin`, default `DEVNULL`
+Other keyword arguments are passed to `Popen`.
 
-  if `trace` is `True`, recite invocation to stderr
-  otherwise presume that `trace` is a stream
-  to which to recite the invocation.
-* `keep_stdin`: if true (default `False`)
-  do not attach the command's standard input to the null device.
-  The default behaviour is to do so,
-  preventing commands from accidentally
-  consuming the main process' input stream.
-
-Other keyword arguments are passed to the `io.TextIOWrapper`
-which wraps the command's output.
-
-## Function `pipeto(argv, quiet=False, **kw)`
+## Function `pipeto(argv, *, quiet=False, **kw)`
 
 Pipe text to a command.
 Optionally trace invocation.
 Return the Popen object with .stdin encoded as text.
 
 Parameters:
 * `argv`: the command argument list
@@ -175,14 +162,18 @@
 * `path`: the path to the pid file.
 * `pid`: the process id to write, defautl from `os.getpid`.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* pipefrom: default stdin=DEVNULL.
+* Make many parameters keyword only.
+
 *Release 20221228*:
 * signal_handlers: bugfix iteration of sig_hnds.
 * Use cs.gimmicks instead of cs.logutils.
 * Drop use of cs.upd, fixes circular import; users of run() may need to call "with Upd().above()" themselves.
 
 *Release 20221118*:
 run: do not print cp.stdout.
```

### Comparing `cs.psutils-20221228/pyproject.toml` & `cs.psutils-20230612/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,42 +6,40 @@
 ]
 keywords = [
     "python2",
     "python3",
 ]
 dependencies = [
     "cs.gimmicks>=20220429",
-    "cs.pfx>=20221118",
+    "cs.pfx>=20230604",
 ]
 classifiers = [
     "Programming Language :: Python",
-    "Programming Language :: Python :: 2",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20221228"
+version = "20230612"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Assorted process and subprocess management functions.
 
-*Latest release 20221228*:
-* signal_handlers: bugfix iteration of sig_hnds.
-* Use cs.gimmicks instead of cs.logutils.
-* Drop use of cs.upd, fixes circular import; users of run() may need to call \"with Upd().above()\" themselves.
+*Latest release 20230612*:
+* pipefrom: default stdin=DEVNULL.
+* Make many parameters keyword only.
 
 ## Function `groupargv(pre_argv, argv, post_argv=(), max_argv=None, encode=False)`
 
 Distribute the array `argv` over multiple arrays
 to fit within `MAX_ARGV`.
 Return a list of argv lists.
 
@@ -70,39 +68,28 @@
 * `path`: the path to the process id file.
 * `pid`: the process id to store in the pid file,
   default from `os.etpid`.
 
 Writes the process id file at the start
 and removes the process id file at the end.
 
-## Function `pipefrom(argv, quiet=False, binary=False, keep_stdin=False, **kw)`
+## Function `pipefrom(argv, *, quiet=False, text=True, stdin=-3, **popen_kw)`
 
-Pipe text from a command.
-Optionally trace invocation.
-Return the `Popen` object with `.stdout` decoded as text.
+Pipe text (usually) from a command using `subprocess.Popen`.
+Return the `Popen` object with `.stdout` as a pipe.
 
 Parameters:
 * `argv`: the command argument list
-* `binary`: if true (default false)
-  return the raw stdout instead of a text wrapper
 * `quiet`: optional flag, default `False`;
+  if true, print the command to `stderr`
+* `text`: optional flag, default `True`; passed to `Popen`.
+* `stdin`: optional value for `Popen`'s `stdin`, default `DEVNULL`
+Other keyword arguments are passed to `Popen`.
 
-  if `trace` is `True`, recite invocation to stderr
-  otherwise presume that `trace` is a stream
-  to which to recite the invocation.
-* `keep_stdin`: if true (default `False`)
-  do not attach the command's standard input to the null device.
-  The default behaviour is to do so,
-  preventing commands from accidentally
-  consuming the main process' input stream.
-
-Other keyword arguments are passed to the `io.TextIOWrapper`
-which wraps the command's output.
-
-## Function `pipeto(argv, quiet=False, **kw)`
+## Function `pipeto(argv, *, quiet=False, **kw)`
 
 Pipe text to a command.
 Optionally trace invocation.
 Return the Popen object with .stdin encoded as text.
 
 Parameters:
 * `argv`: the command argument list
@@ -189,14 +176,18 @@
 * `path`: the path to the pid file.
 * `pid`: the process id to write, defautl from `os.getpid`.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* pipefrom: default stdin=DEVNULL.
+* Make many parameters keyword only.
+
 *Release 20221228*:
 * signal_handlers: bugfix iteration of sig_hnds.
 * Use cs.gimmicks instead of cs.logutils.
 * Drop use of cs.upd, fixes circular import; users of run() may need to call \"with Upd().above()\" themselves.
 
 *Release 20221118*:
 run: do not print cp.stdout.
```

### Comparing `cs.psutils-20221228/setup.cfg` & `cs.psutils-20230612/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 [metadata]
 name = cs.psutils
-version = 20221228
+version = 20230612
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = Assorted process and subprocess management functions.
 keywords = python2, python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers = 
 	Programming Language :: Python
-	Programming Language :: Python :: 2
 	Programming Language :: Python :: 3
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries :: Python Modules
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 package_dir = 
 	= lib/python
 install_requires = 
 	cs.gimmicks>=20220429
-	cs.pfx>=20221118
+	cs.pfx>=20230604
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

