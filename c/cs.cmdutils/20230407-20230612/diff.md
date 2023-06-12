# Comparing `tmp/cs.cmdutils-20230407.tar.gz` & `tmp/cs.cmdutils-20230612.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.cmdutils-20230407.tar", last modified: Thu Apr  6 23:58:21 2023, max compression
+gzip compressed data, was "cs.cmdutils-20230612.tar", last modified: Mon Jun 12 03:20:37 2023, max compression
```

## Comparing `cs.cmdutils-20230407.tar` & `cs.cmdutils-20230612.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-06 23:58:21.818657 cs.cmdutils-20230407/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-04-06 23:57:26.000000 cs.cmdutils-20230407/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    15574 2023-04-06 23:58:21.818962 cs.cmdutils-20230407/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    26014 2023-04-06 23:57:36.000000 cs.cmdutils-20230407/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-06 23:58:21.812249 cs.cmdutils-20230407/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-06 23:58:21.812630 cs.cmdutils-20230407/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-06 23:58:21.815290 cs.cmdutils-20230407/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    45753 2023-04-06 23:57:14.000000 cs.cmdutils-20230407/lib/python/cs/cmdutils.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-06 23:58:21.817962 cs.cmdutils-20230407/lib/python/cs.cmdutils.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    15574 2023-04-06 23:58:21.000000 cs.cmdutils-20230407/lib/python/cs.cmdutils.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      310 2023-04-06 23:58:21.000000 cs.cmdutils-20230407/lib/python/cs.cmdutils.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-04-06 23:58:21.000000 cs.cmdutils-20230407/lib/python/cs.cmdutils.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      172 2023-04-06 23:58:21.000000 cs.cmdutils-20230407/lib/python/cs.cmdutils.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-04-06 23:58:21.000000 cs.cmdutils-20230407/lib/python/cs.cmdutils.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    15987 2023-04-06 23:58:09.000000 cs.cmdutils-20230407/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)     1104 2023-04-06 23:58:21.819711 cs.cmdutils-20230407/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-04-06 23:57:36.000000 cs.cmdutils-20230407/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:20:37.031528 cs.cmdutils-20230612/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-12 03:19:41.000000 cs.cmdutils-20230612/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    15180 2023-06-12 03:20:37.031683 cs.cmdutils-20230612/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    25620 2023-06-12 03:19:52.000000 cs.cmdutils-20230612/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:20:37.027063 cs.cmdutils-20230612/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:20:37.027402 cs.cmdutils-20230612/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:20:37.029373 cs.cmdutils-20230612/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    45450 2023-06-12 03:19:32.000000 cs.cmdutils-20230612/lib/python/cs/cmdutils.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:20:37.031237 cs.cmdutils-20230612/lib/python/cs.cmdutils.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    15180 2023-06-12 03:20:37.000000 cs.cmdutils-20230612/lib/python/cs.cmdutils.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      310 2023-06-12 03:20:37.000000 cs.cmdutils-20230612/lib/python/cs.cmdutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-12 03:20:37.000000 cs.cmdutils-20230612/lib/python/cs.cmdutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      172 2023-06-12 03:20:37.000000 cs.cmdutils-20230612/lib/python/cs.cmdutils.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-12 03:20:37.000000 cs.cmdutils-20230612/lib/python/cs.cmdutils.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    15593 2023-06-12 03:20:26.000000 cs.cmdutils-20230612/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)     1104 2023-06-12 03:20:37.032360 cs.cmdutils-20230612/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-12 03:19:52.000000 cs.cmdutils-20230612/setup.py
```

### Comparing `cs.cmdutils-20230407/PKG-INFO` & `cs.cmdutils-20230612/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.cmdutils
-Version: 20230407
+Version: 20230612
 Summary: Convenience functions for working with the Cmd module, the BaseCommand class for constructing command line programmes, and other command line related stuff.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -17,22 +17,17 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Convenience functions for working with the Cmd module,
 the BaseCommand class for constructing command line programmes,
 and other command line related stuff.
 
-*Latest release 20230407*:
-* BaseCommand: use @uses_runstate when preparing the command, store as self.options.runstate.
-* Make BaseCommandOptions a data class.
-* Drop any pretence at python 2 support, we're long past that.
-* BaseCommand: new cmdloop method to run a cmd.Cmd instance to run subcommand interactively.
-* BaseCommand: rename shell to repl, add cmd_shell to call cmdloop().
-* Drop BaseCommand.apply_defaults in favour of the Options dataclass.
-* BaseCommand: do setup_logging before initiating the Options instance.
+*Latest release 20230612*:
+* BaseCommand.cmdloop: fix intro parameter.
+* Other small fixes.
 
 ## Class `BaseCommand`
 
 A base class for handling nestable command lines.
 
 This class provides the basic parse and dispatch mechanisms
 for command lines.
@@ -125,15 +120,15 @@
 
 Editorial: why not arparse?
 Primarily because when incorrectly invoked
 an argparse command line prints the help/usage messgae
 and aborts the whole programme with `SystemExit`.
 But also, I find the whole argparse `add_argument` thing cumbersome.
 
-*Method `BaseCommand.__init__(self, argv=None, *, cmd=None, options=None, runstate: Optional[cs.resources.RunState], **kw_options)`*:
+*Method `BaseCommand.__init__(self, argv=None, *, cmd=None, options=None, **kw_options)`*:
 Initialise the command line.
 Raises `GetoptError` for unrecognised options.
 
 Parameters:
 * `argv`:
   optional command line arguments
   including the main command name if `cmd` is not specified.
@@ -245,14 +240,18 @@
         def do_something(...):
             ... do something ...
 
 # Release Log
 
 
 
+*Release 20230612*:
+* BaseCommand.cmdloop: fix intro parameter.
+* Other small fixes.
+
 *Release 20230407*:
 * BaseCommand: use @uses_runstate when preparing the command, store as self.options.runstate.
 * Make BaseCommandOptions a data class.
 * Drop any pretence at python 2 support, we're long past that.
 * BaseCommand: new cmdloop method to run a cmd.Cmd instance to run subcommand interactively.
 * BaseCommand: rename shell to repl, add cmd_shell to call cmdloop().
 * Drop BaseCommand.apply_defaults in favour of the Options dataclass.
```

### Comparing `cs.cmdutils-20230407/README.md` & `cs.cmdutils-20230612/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 Convenience functions for working with the Cmd module,
 the BaseCommand class for constructing command line programmes,
 and other command line related stuff.
 
-*Latest release 20230407*:
-* BaseCommand: use @uses_runstate when preparing the command, store as self.options.runstate.
-* Make BaseCommandOptions a data class.
-* Drop any pretence at python 2 support, we're long past that.
-* BaseCommand: new cmdloop method to run a cmd.Cmd instance to run subcommand interactively.
-* BaseCommand: rename shell to repl, add cmd_shell to call cmdloop().
-* Drop BaseCommand.apply_defaults in favour of the Options dataclass.
-* BaseCommand: do setup_logging before initiating the Options instance.
+*Latest release 20230612*:
+* BaseCommand.cmdloop: fix intro parameter.
+* Other small fixes.
 
 ## Class `BaseCommand`
 
 A base class for handling nestable command lines.
 
 This class provides the basic parse and dispatch mechanisms
 for command lines.
@@ -106,15 +101,15 @@
 
 Editorial: why not arparse?
 Primarily because when incorrectly invoked
 an argparse command line prints the help/usage messgae
 and aborts the whole programme with `SystemExit`.
 But also, I find the whole argparse `add_argument` thing cumbersome.
 
-*Method `BaseCommand.__init__(self, argv=None, *, cmd=None, options=None, runstate: Optional[cs.resources.RunState], **kw_options)`*:
+*Method `BaseCommand.__init__(self, argv=None, *, cmd=None, options=None, **kw_options)`*:
 Initialise the command line.
 Raises `GetoptError` for unrecognised options.
 
 Parameters:
 * `argv`:
   optional command line arguments
   including the main command name if `cmd` is not specified.
@@ -200,15 +195,15 @@
 or for all subcommands if no names are specified.
 -l  Long help even if no subcommand-names provided.
 
 *Method `BaseCommand.cmd_shell(self, argv)`*:
 Usage: {cmd}
 Run a command prompt via cmd.Cmd using this command's subcommands.
 
-*Method `BaseCommand.cmdloop(intor=None)`*:
+*Method `BaseCommand.cmdloop(intro=None)`*:
 Use `cmd.Cmd` to run a command loop which calls the `cmd_`* methods.
 
 *Method `BaseCommand.getopt_error_handler(cmd, options, e, usage, subcmd=None)`*:
 The `getopt_error_handler` method
 is used to control the handling of `GetoptError`s raised
 during the command line parse
 or during the `main` or `cmd_`*subcmd*` calls.
@@ -546,14 +541,18 @@
         def do_something(...):
             ... do something ...
 
 # Release Log
 
 
 
+*Release 20230612*:
+* BaseCommand.cmdloop: fix intro parameter.
+* Other small fixes.
+
 *Release 20230407*:
 * BaseCommand: use @uses_runstate when preparing the command, store as self.options.runstate.
 * Make BaseCommandOptions a data class.
 * Drop any pretence at python 2 support, we're long past that.
 * BaseCommand: new cmdloop method to run a cmd.Cmd instance to run subcommand interactively.
 * BaseCommand: rename shell to repl, add cmd_shell to call cmdloop().
 * Drop BaseCommand.apply_defaults in favour of the Options dataclass.
```

### Comparing `cs.cmdutils-20230407/lib/python/cs/cmdutils.py` & `cs.cmdutils-20230612/lib/python/cs/cmdutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,25 @@
 # pylint: disable=too-many-lines
 
 ''' Convenience functions for working with the Cmd module,
     the BaseCommand class for constructing command line programmes,
     and other command line related stuff.
 '''
 
-from abc import ABC, abstractmethod
+from abc import ABC
 from cmd import Cmd
 from code import interact
 from collections import namedtuple
 from contextlib import contextmanager
 from dataclasses import dataclass
-from functools import partial
 from getopt import getopt, GetoptError
 from inspect import isclass, ismethod
 from os.path import basename
 try:
-  import readline
+  import readline  # pylint: disable=unused-import
 except ImportError:
   pass
 import shlex
 from signal import SIGHUP, SIGINT, SIGTERM
 import sys
 from typing import Callable, List, Mapping, Optional
 
@@ -42,15 +41,15 @@
 from cs.logutils import setup_logging, warning, exception
 from cs.pfx import Pfx, pfx_call, pfx_method
 from cs.py.doc import obj_docstring
 from cs.resources import RunState, uses_runstate
 from cs.typingutils import subtype
 from cs.upd import Upd
 
-__version__ = '20230407'
+__version__ = '20230612'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -440,24 +439,15 @@
         'Command line usage:\n\n    ' + usage_message.replace('\n', '\n    ')
     )
     cls_doc = obj_docstring(cls)
     cls_doc = cls_doc + '\n\n' + usage_doc if cls_doc else usage_doc
     cls.__doc__ = cls_doc
 
   # pylint: disable=too-many-branches,too-many-statements,too-many-locals
-  @uses_runstate
-  def __init__(
-      self,
-      argv=None,
-      *,
-      cmd=None,
-      options=None,
-      runstate: Optional[RunState],
-      **kw_options
-  ):
+  def __init__(self, argv=None, *, cmd=None, options=None, **kw_options):
     ''' Initialise the command line.
         Raises `GetoptError` for unrecognised options.
 
         Parameters:
         * `argv`:
           optional command line arguments
           including the main command name if `cmd` is not specified.
@@ -524,23 +514,20 @@
       argv = list(argv)
       if cmd is None:
         argv0 = argv.pop(0)
       else:
         argv0 = cmd
     if cmd is None:
       cmd = basename(argv0)
-    if runstate is None:
-      runstate = RunState(cmd)
     self.cmd = cmd
     log_level = getattr(options, 'log_level', None)
     loginfo = setup_logging(cmd, level=log_level)
     # post: argv is list of arguments after the command name
     self.loginfo = loginfo
     options = self.options = self.Options()
-    options.runstate = runstate
     options.runstate_signals = self.DEFAULT_SIGNALS
     # override the default options
     for option, value in kw_options.items():
       setattr(options, option, value)
     self._argv = argv
     self._run = lambda subcmd, command, argv: 2
     self._subcmd = None
@@ -1104,20 +1091,20 @@
           subcmd=self._subcmd,
       ):
         self._printed_usage = True
         return 2
       raise
 
   @classmethod
-  def cmdloop(cls, intor=None):
+  def cmdloop(cls, intro=None):
     ''' Use `cmd.Cmd` to run a command loop which calls the `cmd_`* methods.
     '''
     # TODO: get intro from usage/help
     cmdobj = BaseCommandCmd(cls)
-    cmdobj.cmdloop()
+    cmdobj.cmdloop(intro)
 
   # pylint: disable=unused-argument
   @staticmethod
   def getopt_error_handler(cmd, options, e, usage, subcmd=None):  # pylint: disable=unused-argument
     ''' The `getopt_error_handler` method
         is used to control the handling of `GetoptError`s raised
         during the command line parse
@@ -1169,18 +1156,15 @@
                     yield
                 finally:
                   ... any unconditional cleanup ...
     '''
     # redundant try/finally to remind subclassers of correct structure
     try:
       options = self.options
-      if runstate is None:
-        runstate = getattr(options, 'runstate', None)
-        if runstate is None:
-          runstate = RunState(self.cmd)
+      assert not hasattr(options, 'runstate')
       handle_signal = getattr(
           self, 'handle_signal', lambda *_: runstate.cancel()
       )
       upd = getattr(options, 'upd', self.loginfo.upd) or Upd()
       with stackattrs(self, cmd=self._subcmd or self.cmd):
         with stackattrs(
             options,
@@ -1266,15 +1250,21 @@
               """ Usage: {cmd}
                     Run an interactive Python prompt with some predefined local names.
               """
               return self.repl(*argv)
     '''
     options = self.options
     if banner is None:
-      banner = f'{self.cmd}: {options.sqltags}'
+      banner = self.cmd
+      try:
+        sqltags = options.sqltags
+      except AttributeError:
+        pass
+      else:
+        banner += f': {sqltags}'
     if local is None:
       local = dict(self.__dict__)
       local.update(options.__dict__)
       local.update(argv=argv, cmd=self.cmd, options=options, self=self)
     try:
       # pylint: disable=import-outside-toplevel
       from bpython import embed
@@ -1303,26 +1293,24 @@
   def __init__(self, command_class: BaseCommandSubType):
     super().__init__()
     self.command_class = command_class
 
   @typechecked
   def _doarg(self, subcmd: str, arg: str):
     cls = self.command_class
-    argv = trace(shlex.split)(arg)
-    command = trace(cls)([cls.__name__, subcmd] + argv)
+    argv = shlex.split(arg)
+    command = cls([cls.__name__, subcmd] + argv)
     with stackattrs(command, _subcmd=subcmd):
       command.run()
 
   def __getattr__(self, attr):
     cls = self.command_class
     subcmd = cutprefix(attr, 'do_')
     if subcmd is not attr:
       method_name = cls.SUBCOMMAND_METHOD_PREFIX + subcmd
-      X("method_name=%s", method_name)
       if hasattr(cls, method_name):
 
         def do_cmdsub(arg):
-          return trace(self._doarg)(subcmd, arg)
+          return self._doarg(subcmd, arg)
 
         return do_cmdsub
-        return trace(docmd(partial(self._doarg, subcmd)))
     raise AttributeError("%s.%s" % (self.__class__.__name__, attr))
```

### Comparing `cs.cmdutils-20230407/lib/python/cs.cmdutils.egg-info/PKG-INFO` & `cs.cmdutils-20230612/lib/python/cs.cmdutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.cmdutils
-Version: 20230407
+Version: 20230612
 Summary: Convenience functions for working with the Cmd module, the BaseCommand class for constructing command line programmes, and other command line related stuff.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -17,22 +17,17 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Convenience functions for working with the Cmd module,
 the BaseCommand class for constructing command line programmes,
 and other command line related stuff.
 
-*Latest release 20230407*:
-* BaseCommand: use @uses_runstate when preparing the command, store as self.options.runstate.
-* Make BaseCommandOptions a data class.
-* Drop any pretence at python 2 support, we're long past that.
-* BaseCommand: new cmdloop method to run a cmd.Cmd instance to run subcommand interactively.
-* BaseCommand: rename shell to repl, add cmd_shell to call cmdloop().
-* Drop BaseCommand.apply_defaults in favour of the Options dataclass.
-* BaseCommand: do setup_logging before initiating the Options instance.
+*Latest release 20230612*:
+* BaseCommand.cmdloop: fix intro parameter.
+* Other small fixes.
 
 ## Class `BaseCommand`
 
 A base class for handling nestable command lines.
 
 This class provides the basic parse and dispatch mechanisms
 for command lines.
@@ -125,15 +120,15 @@
 
 Editorial: why not arparse?
 Primarily because when incorrectly invoked
 an argparse command line prints the help/usage messgae
 and aborts the whole programme with `SystemExit`.
 But also, I find the whole argparse `add_argument` thing cumbersome.
 
-*Method `BaseCommand.__init__(self, argv=None, *, cmd=None, options=None, runstate: Optional[cs.resources.RunState], **kw_options)`*:
+*Method `BaseCommand.__init__(self, argv=None, *, cmd=None, options=None, **kw_options)`*:
 Initialise the command line.
 Raises `GetoptError` for unrecognised options.
 
 Parameters:
 * `argv`:
   optional command line arguments
   including the main command name if `cmd` is not specified.
@@ -245,14 +240,18 @@
         def do_something(...):
             ... do something ...
 
 # Release Log
 
 
 
+*Release 20230612*:
+* BaseCommand.cmdloop: fix intro parameter.
+* Other small fixes.
+
 *Release 20230407*:
 * BaseCommand: use @uses_runstate when preparing the command, store as self.options.runstate.
 * Make BaseCommandOptions a data class.
 * Drop any pretence at python 2 support, we're long past that.
 * BaseCommand: new cmdloop method to run a cmd.Cmd instance to run subcommand interactively.
 * BaseCommand: rename shell to repl, add cmd_shell to call cmdloop().
 * Drop BaseCommand.apply_defaults in favour of the Options dataclass.
```

### Comparing `cs.cmdutils-20230407/pyproject.toml` & `cs.cmdutils-20230612/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,52 +8,47 @@
     "python2",
     "python3",
 ]
 dependencies = [
     "cs.context>=20230331",
     "cs.lex>=20230401",
     "cs.logutils>=20230212",
-    "cs.pfx>=20230331",
+    "cs.pfx>=20230604",
     "cs.py.doc>=20220311",
-    "cs.resources>=20230331",
+    "cs.resources>=20230503",
     "cs.typingutils>=20230331",
     "cs.upd>=20230401",
     "typeguard",
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20230407"
+version = "20230612"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Convenience functions for working with the Cmd module,
 the BaseCommand class for constructing command line programmes,
 and other command line related stuff.
 
-*Latest release 20230407*:
-* BaseCommand: use @uses_runstate when preparing the command, store as self.options.runstate.
-* Make BaseCommandOptions a data class.
-* Drop any pretence at python 2 support, we're long past that.
-* BaseCommand: new cmdloop method to run a cmd.Cmd instance to run subcommand interactively.
-* BaseCommand: rename shell to repl, add cmd_shell to call cmdloop().
-* Drop BaseCommand.apply_defaults in favour of the Options dataclass.
-* BaseCommand: do setup_logging before initiating the Options instance.
+*Latest release 20230612*:
+* BaseCommand.cmdloop: fix intro parameter.
+* Other small fixes.
 
 ## Class `BaseCommand`
 
 A base class for handling nestable command lines.
 
 This class provides the basic parse and dispatch mechanisms
 for command lines.
@@ -146,15 +141,15 @@
 
 Editorial: why not arparse?
 Primarily because when incorrectly invoked
 an argparse command line prints the help/usage messgae
 and aborts the whole programme with `SystemExit`.
 But also, I find the whole argparse `add_argument` thing cumbersome.
 
-*Method `BaseCommand.__init__(self, argv=None, *, cmd=None, options=None, runstate: Optional[cs.resources.RunState], **kw_options)`*:
+*Method `BaseCommand.__init__(self, argv=None, *, cmd=None, options=None, **kw_options)`*:
 Initialise the command line.
 Raises `GetoptError` for unrecognised options.
 
 Parameters:
 * `argv`:
   optional command line arguments
   including the main command name if `cmd` is not specified.
@@ -266,14 +261,18 @@
         def do_something(...):
             ... do something ...
 
 # Release Log
 
 
 
+*Release 20230612*:
+* BaseCommand.cmdloop: fix intro parameter.
+* Other small fixes.
+
 *Release 20230407*:
 * BaseCommand: use @uses_runstate when preparing the command, store as self.options.runstate.
 * Make BaseCommandOptions a data class.
 * Drop any pretence at python 2 support, we're long past that.
 * BaseCommand: new cmdloop method to run a cmd.Cmd instance to run subcommand interactively.
 * BaseCommand: rename shell to repl, add cmd_shell to call cmdloop().
 * Drop BaseCommand.apply_defaults in favour of the Options dataclass.
```

### Comparing `cs.cmdutils-20230407/setup.cfg` & `cs.cmdutils-20230612/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.cmdutils
-version = 20230407
+version = 20230612
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = Convenience functions for working with the Cmd module, the BaseCommand class for constructing command line programmes, and other command line related stuff.
 keywords = python2, python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers = 
@@ -21,17 +21,17 @@
 [options]
 package_dir = 
 	= lib/python
 install_requires = 
 	cs.context>=20230331
 	cs.lex>=20230401
 	cs.logutils>=20230212
-	cs.pfx>=20230331
+	cs.pfx>=20230604
 	cs.py.doc>=20220311
-	cs.resources>=20230331
+	cs.resources>=20230503
 	cs.typingutils>=20230331
 	cs.upd>=20230401
 	typeguard
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

