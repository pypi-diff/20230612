# Comparing `tmp/cs.splink-20230217.tar.gz` & `tmp/cs.splink-20230612.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.splink-20230217.tar", last modified: Fri Feb 17 09:36:25 2023, max compression
+gzip compressed data, was "cs.splink-20230612.tar", last modified: Mon Jun 12 10:32:52 2023, max compression
```

## Comparing `cs.splink-20230217.tar` & `cs.splink-20230612.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 09:36:25.753077 cs.splink-20230217/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-02-17 09:36:08.000000 cs.splink-20230217/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     9113 2023-02-17 09:36:25.753234 cs.splink-20230217/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    15991 2023-02-17 09:36:11.000000 cs.splink-20230217/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 09:36:25.748388 cs.splink-20230217/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 09:36:25.748691 cs.splink-20230217/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 09:36:25.750355 cs.splink-20230217/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    39545 2023-02-17 09:36:00.000000 cs.splink-20230217/lib/python/cs/splink.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 09:36:25.752843 cs.splink-20230217/lib/python/cs.splink.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     9113 2023-02-17 09:36:25.000000 cs.splink-20230217/lib/python/cs.splink.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      345 2023-02-17 09:36:25.000000 cs.splink-20230217/lib/python/cs.splink.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-02-17 09:36:25.000000 cs.splink-20230217/lib/python/cs.splink.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       42 2023-02-17 09:36:25.000000 cs.splink-20230217/lib/python/cs.splink.egg-info/entry_points.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      357 2023-02-17 09:36:25.000000 cs.splink-20230217/lib/python/cs.splink.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-02-17 09:36:25.000000 cs.splink-20230217/lib/python/cs.splink.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     9751 2023-02-17 09:36:16.000000 cs.splink-20230217/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)     1323 2023-02-17 09:36:25.753939 cs.splink-20230217/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-02-17 09:36:11.000000 cs.splink-20230217/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 10:32:52.080432 cs.splink-20230612/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-12 10:32:30.000000 cs.splink-20230612/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     9609 2023-06-12 10:32:52.080601 cs.splink-20230612/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    16254 2023-06-12 10:32:33.000000 cs.splink-20230612/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 10:32:52.074744 cs.splink-20230612/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 10:32:52.075104 cs.splink-20230612/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 10:32:52.077389 cs.splink-20230612/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    42329 2023-06-12 10:32:20.000000 cs.splink-20230612/lib/python/cs/splink.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 10:32:52.080045 cs.splink-20230612/lib/python/cs.splink.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     9609 2023-06-12 10:32:52.000000 cs.splink-20230612/lib/python/cs.splink.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      345 2023-06-12 10:32:52.000000 cs.splink-20230612/lib/python/cs.splink.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-12 10:32:52.000000 cs.splink-20230612/lib/python/cs.splink.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       42 2023-06-12 10:32:52.000000 cs.splink-20230612/lib/python/cs.splink.egg-info/entry_points.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      366 2023-06-12 10:32:52.000000 cs.splink-20230612/lib/python/cs.splink.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-12 10:32:52.000000 cs.splink-20230612/lib/python/cs.splink.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    10263 2023-06-12 10:32:40.000000 cs.splink-20230612/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)     1333 2023-06-12 10:32:52.081332 cs.splink-20230612/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-12 10:32:33.000000 cs.splink-20230612/setup.py
```

### Comparing `cs.splink-20230217/PKG-INFO` & `cs.splink-20230612/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.splink
-Version: 20230217
+Version: 20230612
 Summary: Assorted utility functions for working with data downloaded from Selectronics' SP-LINK programme which communicates with their solar inverter controllers.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
@@ -16,16 +16,18 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted utility functions for working with data
 downloaded from Selectronics' SP-LINK programme
 which communicates with their solar inverter controllers.
 
-*Latest release 20230217*:
-SPLinkCommand.cmd_plot: make the start-time optional, default to 5.
+*Latest release 20230612*:
+* SPLinkCommand: new print_known_datasets method, use in help.
+* SPLinkCommand.cmd_plot: if the start/stop times are out of order, swap them.
+* Assorted internal changes.
 
 I use this to gather and plot data from my solar inverter.
 
 ## Function `main(argv=None)`
 
 SP-Link command line mode.
 
@@ -86,21 +88,25 @@
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             stop-time       Optional stop time, default now.
                             An integer number of days before the current time
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             mode            A named graph mode, implying a group of fields.
+                            Providing '?' or 'help' prints the available
+                            datasets and field names.
         pull [-d dataset,...] [-F rsync-source] [-nx]
           Fetch and import data.
           -d dataset,...
                 Specify the datasets to import.
           -F    Fetch rsync source, default from $SPLINK_FETCH_SOURCE.
           -n    No action; pass -n to rsync. Just more convenient than putting it at the end.
           -x    Delete source files.
+        shell
+          Run a command prompt via cmd.Cmd using this command's subcommands.
 
 ## Class `SPLinkCSVDir(cs.fs.HasFSPath)`
 
 A class for working with SP-Link data downloads,
 referring to a particular `PerformanceData*` download directory.
 
 ## Class `SPLinkData(cs.fs.HasFSPath, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
@@ -142,21 +148,25 @@
 SPLinkDataFileInfo(fspath, sitename, dataset, unixtime, dotext)
 
 *Method `SPLinkDataFileInfo.__new__(_cls, fspath, sitename, dataset, unixtime, dotext)`*:
 Create new instance of SPLinkDataFileInfo(fspath, sitename, dataset, unixtime, dotext)
 
 ## Function `ts2001_unixtime(tzname=None)`
 
-Convert an SP-Link seconds-since-2001-01-01-local-time offset
-into a UNIX time.
+Return the SP-Link 2001-01-01-local-time epoch as a UNIX time.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* SPLinkCommand: new print_known_datasets method, use in help.
+* SPLinkCommand.cmd_plot: if the start/stop times are out of order, swap them.
+* Assorted internal changes.
+
 *Release 20230217*:
 SPLinkCommand.cmd_plot: make the start-time optional, default to 5.
 
 *Release 20220918*:
 * SPLinkData.plot: rename `key_specs` keyword parameter to mandatory posiitional `data_specs` parameter.
 * SPLinkData.resolve: accept multiple specification strings.
 * New SPLinkData.plot_data_from_spec(start,stop,data_spec,...) method to return a list of PlotSeries instances.
```

### Comparing `cs.splink-20230217/README.md` & `cs.splink-20230612/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Assorted utility functions for working with data
 downloaded from Selectronics' SP-LINK programme
 which communicates with their solar inverter controllers.
 
-*Latest release 20230217*:
-SPLinkCommand.cmd_plot: make the start-time optional, default to 5.
+*Latest release 20230612*:
+* SPLinkCommand: new print_known_datasets method, use in help.
+* SPLinkCommand.cmd_plot: if the start/stop times are out of order, swap them.
+* Assorted internal changes.
 
 I use this to gather and plot data from my solar inverter.
 
 ## Function `main(argv=None)`
 
 SP-Link command line mode.
 
@@ -68,24 +70,27 @@
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             stop-time       Optional stop time, default now.
                             An integer number of days before the current time
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             mode            A named graph mode, implying a group of fields.
+                            Providing '?' or 'help' prints the available
+                            datasets and field names.
         pull [-d dataset,...] [-F rsync-source] [-nx]
           Fetch and import data.
           -d dataset,...
                 Specify the datasets to import.
           -F    Fetch rsync source, default from $SPLINK_FETCH_SOURCE.
           -n    No action; pass -n to rsync. Just more convenient than putting it at the end.
           -x    Delete source files.
+        shell
+          Run a command prompt via cmd.Cmd using this command's subcommands.
 
-*Method `SPLinkCommand.apply_defaults(self)`*:
-Set the default `spdpath`.
+*`SPLinkCommand.Options`*
 
 *Method `SPLinkCommand.apply_opt(self, opt, val)`*:
 Handle an individual global command line option.
 
 *Method `SPLinkCommand.cmd_export(self, argv)`*:
 Usage: {cmd} dataset
 Export the named dataset in the original CSV form.
@@ -136,28 +141,33 @@
                   or any datetime specification recognised by
                   dateutil.parser.parse.
   stop-time       Optional stop time, default now.
                   An integer number of days before the current time
                   or any datetime specification recognised by
                   dateutil.parser.parse.
   mode            A named graph mode, implying a group of fields.
+                  Providing '?' or 'help' prints the available
+                  datasets and field names.
 
 *Method `SPLinkCommand.cmd_pull(self, argv)`*:
 Usage: {cmd} [-d dataset,...] [-F rsync-source] [-nx]
 Fetch and import data.
 -d dataset,...
       Specify the datasets to import.
 -F    Fetch rsync source, default from ${DEFAULT_FETCH_SOURCE_ENVVAR}.
 -n    No action; pass -n to rsync. Just more convenient than putting it at the end.
 -x    Delete source files.
 
 *Method `SPLinkCommand.popdata(self, start: float, stop: float, argv: List[str], argname: str = 'data-spec', *, utcoffset: float, **kw) -> List[cs.timeseries.PlotSeries]`*:
 Pop a data specification from the command line,
 return a list of `PlotSeries` instances derived from it.
 
+*Method `SPLinkCommand.print_known_datasets(self, file=None)`*:
+Print the known datasets and their fields to `file`.
+
 *Method `SPLinkCommand.run_context(self)`*:
 Define `self.options` attributes:
 * `tz`: the default local timezone
 * `spd`: the `SPLinkData` instance for `options.spdpath`
 
 ## Class `SPLinkCSVDir(cs.fs.HasFSPath)`
 
@@ -232,21 +242,14 @@
 Return an informational `dict` containing salient information
 about this `SPLinkData`, handy for use with `pformat()` or `pprint()`.
 
 *Method `SPLinkData.parse_dataset_filename(path)`*:
 Parse the filename part of `path` and derive an `SPLinkDataFileInfo`.
 Raises `ValueError` if the filename cannot be recognised.
 
-*Method `SPLinkData.plot(self, start, stop, data_specs, *, utcoffset, figure=None, ax=None, ax_title=None, key_map=None, color_map=None, event_labels=None, mode_patterns=None, stacked=False, upd=None, runstate=None)`*:
-The core logic of the `SPLinkCommand.cmd_plot` method
-to plot arbitrary parameters against a time range.
-
-`data_specs` is an iterable of `PlotSeries` instances or `str`
-data specifications.
-
 *Method `SPLinkData.plot_data_from_spec(self, start: float, stop: float, data_spec: str, *, utcoffset: float, mode_patterns=None) -> List[cs.timeseries.PlotSeries]`*:
 Decode `data_spec` into a list of `PlotSeries` instances.
 
 *Method `SPLinkData.resolve(self, *specs)`*:
 Resolve field specs into an iterable of `(timeseries,key)`.
 
 *Method `SPLinkData.startup_shutdown(self)`*:
@@ -315,21 +318,25 @@
 Alias for field number 1
 
 *Property `SPLinkDataFileInfo.unixtime`*:
 Alias for field number 3
 
 ## Function `ts2001_unixtime(tzname=None)`
 
-Convert an SP-Link seconds-since-2001-01-01-local-time offset
-into a UNIX time.
+Return the SP-Link 2001-01-01-local-time epoch as a UNIX time.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* SPLinkCommand: new print_known_datasets method, use in help.
+* SPLinkCommand.cmd_plot: if the start/stop times are out of order, swap them.
+* Assorted internal changes.
+
 *Release 20230217*:
 SPLinkCommand.cmd_plot: make the start-time optional, default to 5.
 
 *Release 20220918*:
 * SPLinkData.plot: rename `key_specs` keyword parameter to mandatory posiitional `data_specs` parameter.
 * SPLinkData.resolve: accept multiple specification strings.
 * New SPLinkData.plot_data_from_spec(start,stop,data_spec,...) method to return a list of PlotSeries instances.
```

### Comparing `cs.splink-20230217/lib/python/cs/splink.py` & `cs.splink-20230612/lib/python/cs/splink.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
     I use this to gather and plot data from my solar inverter.
 '''
 
 from collections import defaultdict, namedtuple
 from contextlib import contextmanager
 import csv
+from dataclasses import dataclass, field
 from datetime import datetime
 from functools import partial
 from getopt import GetoptError
 from itertools import chain, cycle
 import os
 from os.path import (
     basename,
@@ -27,50 +28,50 @@
     relpath,
     splitext,
 )
 from pprint import pprint
 import shlex
 import sys
 import time
-from typing import List
+from typing import List, Optional
 
 import arrow
 from dateutil.tz import tzlocal
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from typeguard import typechecked
 
 from cs.context import stackattrs
 from cs.csvutils import csv_import
 from cs.deco import cachedmethod
 from cs.fs import HasFSPath, fnmatchdir, needdir, shortpath
-from cs.fstags import FSTags
+from cs.fstags import FSTags, DEFAULT_FSTAGS
 from cs.lex import s
 from cs.logutils import warning, error
 from cs.mplutils import axes, remove_decorations, print_figure, save_figure, FigureSize
 from cs.pfx import Pfx, pfx, pfx_call, pfx_method
 from cs.progress import progressbar
 from cs.psutils import run
-from cs.resources import MultiOpenMixin
+from cs.resources import MultiOpenMixin, RunState, uses_runstate
 from cs.sqltags import SQLTags
 from cs.tagset import TagSet
 from cs.timeseries import (
     Epoch,
     PlotSeries as PS,
     TimeSeriesBaseCommand,
     TimeSeriesDataDir,
     TimespanPolicyYearly,
     as_datetime64s,
     plot_events,
     timerange,
     tzfor,
 )
-from cs.upd import Upd, print  # pylint: disable=redefined-builtin
+from cs.upd import Upd, uses_upd, print  # pylint: disable=redefined-builtin
 
-__version__ = '20230217'
+__version__ = '20230612'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
     ],
@@ -88,14 +89,15 @@
         'cs.progress',
         'cs.psutils',
         'cs.resources',
         'cs.sqltags',
         'cs.tagset',
         'cs.timeseries',
         'cs.upd',
+        'matplotlib',
         'python-dateutil',
         'typeguard',
     ],
     'entry_points': {
         'console_scripts': [
             'splink = cs.splink:main',
         ],
@@ -122,16 +124,15 @@
 
 def main(argv=None):
   ''' SP-Link command line mode.
   '''
   return SPLinkCommand(argv).run()
 
 def ts2001_unixtime(tzname=None):
-  ''' Convert an SP-Link seconds-since-2001-01-01-local-time offset
-      into a UNIX time.
+  ''' Return the SP-Link 2001-01-01-local-time epoch as a UNIX time.
   '''
   if tzname is None:
     tzname = 'local'
   a2001 = arrow.get(datetime(2001, 1, 1, 0, 0, 0), tzname)
   unixtime = a2001.timestamp()
   return unixtime
 
@@ -566,15 +567,17 @@
     if not plot_data:
       raise ValueError(
           "no fields were resolved by data_spec=%r" % (data_spec,)
       )
     return plot_data
 
   # pylint: disable=too-many-branches,too-many-locals
+  @uses_upd
   @timerange
+  @uses_runstate
   def plot(
       self,
       start,
       stop,
       data_specs,
       *,
       utcoffset,
@@ -582,31 +585,29 @@
       ax=None,
       ax_title=None,
       key_map=None,  # labels from keys
       color_map=None,  # colors for keys
       event_labels=None,
       mode_patterns=None,
       stacked=False,
-      upd=None,
-      runstate=None,
+      upd: Upd,
+      runstate: RunState,
   ):
     ''' The core logic of the `SPLinkCommand.cmd_plot` method
         to plot arbitrary parameters against a time range.
 
         `data_specs` is an iterable of `PlotSeries` instances or `str`
         data specifications.
     '''
     ax = axes(figure, ax)
     figure = ax.figure
     if event_labels is None:
       event_labels = DEFAULT_PLOT_EVENT_LABELS
     if mode_patterns is None:
       mode_patterns = DEFAULT_PLOT_MODE_PATTERNS
-    if upd is None:
-      upd = Upd()
     if key_map is None:
       key_map = {}
     if color_map is None:
       color_map = {}
     plot_data = list(
         chain(
             *(
@@ -658,15 +659,15 @@
             indices,
             *map(lambda ps: ps.series, plot_ps),
             labels=map(lambda ps: key_map.get(ps.label, ps.label), plot_ps),
             colors=map(lambda ps: ps.extra['color'], plot_ps),
         )
       else:
         for label, series, extra in plot_ps:
-          if runstate and runstate.canclled:
+          if runstate.cancelled:
             break
           ax.plot(indices, series, label=label, **extra)
       if ax_title is not None:
         ax.set_title(ax_title)
     return figure
 
 class SPLinkCommand(TimeSeriesBaseCommand):
@@ -692,23 +693,26 @@
       'ALL_DATASETS': ' '.join(sorted(ALL_DATASETS)),
       'TIMESERIES_DATASETS': ' '.join(sorted(SPLinkData.TIMESERIES_DATASETS)),
       'DEFAULT_SPDPATH': DEFAULT_SPDPATH,
       'DEFAULT_SPDPATH_ENVVAR': DEFAULT_SPDPATH_ENVVAR,
       'DEFAULT_FETCH_SOURCE_ENVVAR': DEFAULT_FETCH_SOURCE_ENVVAR,
   }
 
-  def apply_defaults(self):
-    ''' Set the default `spdpath`.
-    '''
-    self.options.fetch_source = os.environ.get(
-        self.DEFAULT_FETCH_SOURCE_ENVVAR
+  @dataclass
+  class Options(TimeSeriesBaseCommand.Options):
+    fetch_source: Optional[str] = field(
+        default_factory=lambda: os.environ.
+        get(SPLinkCommand.DEFAULT_FETCH_SOURCE_ENVVAR)
     )
-    self.options.fstags = FSTags()
-    self.options.spdpath = os.environ.get(
-        self.DEFAULT_SPDPATH_ENVVAR, self.DEFAULT_SPDPATH
+    fstags: FSTags = field(default_factory=lambda: DEFAULT_FSTAGS)
+    spdpath: str = field(
+        default_factory=lambda: os.environ.get(
+            SPLinkCommand.DEFAULT_SPDPATH_ENVVAR,
+            SPLinkCommand.DEFAULT_SPDPATH,
+        )
     )
 
   def apply_opt(self, opt, val):
     ''' Handle an individual global command line option.
     '''
     options = self.options
     if opt == '-d':
@@ -716,14 +720,25 @@
         raise GetoptError("not a directory: %r" % (val,))
       options.spdpath = val
     elif opt == '-n':
       options.doit = False
     else:
       raise RuntimeError("unhandled pre-option")
 
+  def print_known_datasets(self, file=None):
+    ''' Print the known datasets and their fields to `file`.
+    '''
+    spd = self.options.spd
+    print("Known datasets:")
+    for dsname in spd.TIMESERIES_DATASETS:
+      tsd = getattr(spd, dsname)
+      print(" ", dsname, file=file)
+      for key in sorted(tsd.keys()):
+        print("   ", key, file=file)
+
   @timerange
   @typechecked
   def popdata(
       self,
       start: float,
       stop: float,
       argv: List[str],
@@ -1007,14 +1022,16 @@
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             stop-time       Optional stop time, default now.
                             An integer number of days before the current time
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             mode            A named graph mode, implying a group of fields.
+                            Providing '?' or 'help' prints the available
+                            datasets and field names.
     '''
     options = self.options
     options.bare = False
     options.show_image = False
     options.imgpath = None
     options.stacked = False
     options.event_labels = None
@@ -1026,172 +1043,207 @@
         f='force',
         o_='imgpath',
         show='show_image',
         stacked=None,
         tz_=('tz', tzfor),
     )
     tz = options.tz
+    if len(argv) == 1 and argv[0] in ('?', 'help'):
+      self.print_known_datasets()
+      return 0
     # start time
     if not argv:
       argv = ['5']
     start = self.poptime(argv, 'start-time')
     # check for optional stop-time, default now
     if argv:
       try:
         stop = self.poptime(argv, 'stop-time', unpop_on_error=True)
       except GetoptError:
         stop = time.time()
     else:
       stop = time.time()
+    if stop < start:
+      start, stop = stop, start
+    if len(argv) == 1 and argv[0] in ('?', 'help'):
+      self.print_known_datasets()
+      return 0
     data_specs = argv if argv else ['POWER']
     bare = options.bare
     force = options.force
     imgpath = options.imgpath
     spd = options.spd
     show_image = options.show_image
     stacked = options.stacked
     event_labels = options.event_labels
     detailed = spd.DetailedData
-    det_data = lambda field: detailed[field].as_pd_series(
+    detail_series_cropped = lambda field: detailed[field].as_pd_series(
         start, stop, pad=True, tz=tz
     )
-    if data_specs == ['POWER']:
-      grid = det_data('ac_input_power_average_kw')
-      grid_in = -grid.clip(upper=0.0)
-      grid_out = grid.clip(lower=0.0)
-      pv = det_data('total_ac_coupled_power_average_kw')
-      battery = det_data('inverter_ac_power_average_kw')
-      battery_drain = -battery.clip(upper=0.0)
-      battery_charge = battery.clip(lower=0.0)
-      battery_state_of_charge = det_data('state_of_charge_sample')
-      load = det_data('load_ac_power_average_kw')
-      figure, (power_ax, usage_ax) = plt.subplots(
-          2,
-          1,
-          figsize=(FigureSize.DEFAULT_DX, FigureSize.DEFAULT_DY * 1),
-          label=f'Power: {spd}',
-      )
-      # stack the power consumption
-      spd.plot(
-          start,
-          stop,
-          [
-              PS(
-                  'load [load_ac_power_average_kw]',
-                  load,
-                  dict(color='grey'),
-              ),
-              PS(
-                  'battery charge [inverter_ac_power_average_kw]',
-                  battery_charge,
-                  dict(color='blue'),
-              ),
-              PS(
-                  'grid out [ac_input_power_average_kw]',
-                  grid_out,
-                  dict(color='green'),
-              ),
-          ],
-          ax=usage_ax,
-          ax_title="Power Usage",
-          stacked=True,
-          tz=tz,
-      )
-      ax2 = usage_ax.twinx()
-      spd.plot(
-          start,
-          stop,
-          [
-              PS(
-                  'battery % [state_of_charge_sample]',
-                  battery_state_of_charge,
-                  dict(color='orange'),
-              ),
-          ],
-          ax=ax2,
-          tz=tz,
-      )
-      usage_ax.legend()
-      ax2.legend()
-      # stack the power sources
-      spd.plot(
-          start,
-          stop,
-          [
-              PS(
-                  'pv [total_ac_coupled_power_average_kw]',
-                  pv,
-                  dict(color='yellow'),
+    # list of graph specifications
+    had_failed_specs = False
+    graphs = {}
+    for data_spec in data_specs:
+      with Pfx("specification %r", data_spec):
+        if data_spec == 'POWER':
+          grid = detail_series_cropped('ac_input_power_average_kw')
+          grid_in = -grid.clip(upper=0.0)
+          grid_out = grid.clip(lower=0.0)
+          pv = detail_series_cropped('total_ac_coupled_power_average_kw')
+          battery = detail_series_cropped('inverter_ac_power_average_kw')
+          battery_drain = -battery.clip(upper=0.0)
+          battery_charge = battery.clip(lower=0.0)
+          battery_state_of_charge = detail_series_cropped(
+              'state_of_charge_sample'
+          )
+          load = detail_series_cropped('load_ac_power_average_kw')
+          figure, (power_ax, usage_ax) = plt.subplots(
+              2,
+              1,
+              figsize=(FigureSize.DEFAULT_DX, FigureSize.DEFAULT_DY * 1),
+              label=f'Power: {spd}',
+          )
+          graphs["Power Usage"] = [
+              # stack the power consumption
+              dict(
+                  data=[
+                      PS(
+                          'load [load_ac_power_average_kw]',
+                          load,
+                          dict(color='grey'),
+                      ),
+                      PS(
+                          'battery charge [inverter_ac_power_average_kw]',
+                          battery_charge,
+                          dict(color='blue'),
+                      ),
+                      PS(
+                          'grid out [ac_input_power_average_kw]',
+                          grid_out,
+                          dict(color='green'),
+                      ),
+                  ],
+                  stacked=True,
               ),
-              PS(
-                  'battery drain [-inverter_ac_power_average_kw]',
-                  battery_drain,
-                  dict(color='blue'),
+              # overlay the load as a line
+              dict(
+                  data=[
+                      PS(
+                          'load [load_ac_power_average_kw]',
+                          load,
+                          dict(color='black'),
+                      ),
+                  ],
               ),
-              PS(
-                  'grid in [-ac_input_power_average_kw]',
-                  grid_in,
-                  dict(color='red'),
+              dict(
+                  data=[
+                      PS(
+                          'battery % [state_of_charge_sample]',
+                          battery_state_of_charge,
+                          dict(color='orange'),
+                      ),
+                  ],
+                  twinx=True,
               ),
-          ],
-          ax=power_ax,
-          ax_title="Power Supply",
-          stacked=True,
-          tz=tz,
-      )
-      ax2 = power_ax.twinx()
-      spd.plot(
-          start,
-          stop,
-          [
-              PS(
-                  'battery % [state_of_charge_sample]',
-                  battery_state_of_charge,
-                  dict(color='orange'),
+          ]
+          graphs["Power Supply"] = [
+              # stack the power sources
+              dict(
+                  data=[
+                      PS(
+                          'pv [total_ac_coupled_power_average_kw]',
+                          pv,
+                          dict(color='yellow'),
+                      ),
+                      PS(
+                          'battery drain [-inverter_ac_power_average_kw]',
+                          battery_drain,
+                          dict(color='blue'),
+                      ),
+                      PS(
+                          'grid in [-ac_input_power_average_kw]',
+                          grid_in,
+                          dict(color='red'),
+                      ),
+                  ],
+                  stacked=True,
               ),
-          ],
-          ax=ax2,
-          tz=tz,
-      )
-      # overlay the load as a line
-      spd.plot(
-          start,
-          stop,
-          [
-              PS(
-                  'load [load_ac_power_average_kw]',
-                  load,
-                  dict(color='black'),
+              dict(
+                  data=[
+                      PS(
+                          'battery % [state_of_charge_sample]',
+                          battery_state_of_charge,
+                          dict(color='orange'),
+                      ),
+                  ],
+                  twinx=True,
               ),
-          ],
-          ax=power_ax,
-          tz=tz,
-      )
-      power_ax.legend()
-      ax2.legend()
+          ]
+        else:
+          graph_n = 1
+          graph_name_1 = graph_name = data_spec
+          while graph_name in graphs:
+            graph_n += 1
+            graph_name = f'{graph_name_1} {graph_n}'
+          try:
+            plot_data = spd.plot_data_from_spec(start, stop, data_spec, tz=tz)
+          except ValueError as e:
+            warning("bad data spec: %s", e)
+            had_failed_specs = True
+          else:
+            graphs[graph_name] = [
+                dict(
+                    data=spd
+                    .plot_data_from_spec(start, stop, data_spec, tz=tz)
+                ),
+            ]
+    if had_failed_specs:
+      warning("some data specifications did not match")
+      self.print_known_datasets(file=sys.stderr)
+    if not graphs:
+      warning("nothing to plot")
+      return 1
+    assert len(graphs) > 0
+    if len(graphs) > 1:
+      label = f'{spd}: {", ".join(graphs.keys())}'
     else:
-      plot_data = []
-      while data_specs:
-        plot_data.extend(self.popdata(start, stop, data_specs, tz=tz))
-      figure = spd.plot(
-          start,
-          stop,
-          plot_data,
-          tz=tz,
-          event_labels=event_labels,
-          stacked=stacked,
-      )
+      label = f'{spd}'
+    figure, axes = plt.subplots(
+        len(graphs),
+        1,
+        figsize=(FigureSize.DEFAULT_DX, FigureSize.DEFAULT_DY * 1),
+        label=label,
+    )
+    if len(graphs) == 1:
+      axes = axes,
+    for ax, (gkey, gplots) in zip(axes, graphs.items()):
+      gtitle = gkey
+      for gplot in gplots:
+        plot_ax = ax
+        if gplot.get('twinx', False):
+          plot_ax = plot_ax.twinx()
+        spd.plot(
+            start,
+            stop,
+            gplot['data'],
+            ax=plot_ax,
+            ax_title=gplot.get('title', gtitle),
+            stacked=gplot.get('stacked', False),
+            tz=tz,
+        )
+        plot_ax.legend()
     if bare:
       remove_decorations(figure)
     if imgpath:
       save_figure(figure, imgpath, force=force)
       if show_image:
         os.system(shlex.join(['open', imgpath]))
     else:
       print_figure(figure)
+    return 0
 
   def cmd_pull(self, argv):
     ''' Usage: {cmd} [-d dataset,...] [-F rsync-source] [-nx]
           Fetch and import data.
           -d dataset,...
                 Specify the datasets to import.
           -F    Fetch rsync source, default from ${DEFAULT_FETCH_SOURCE_ENVVAR}.
```

### Comparing `cs.splink-20230217/lib/python/cs.splink.egg-info/PKG-INFO` & `cs.splink-20230612/lib/python/cs.splink.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.splink
-Version: 20230217
+Version: 20230612
 Summary: Assorted utility functions for working with data downloaded from Selectronics' SP-LINK programme which communicates with their solar inverter controllers.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
@@ -16,16 +16,18 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted utility functions for working with data
 downloaded from Selectronics' SP-LINK programme
 which communicates with their solar inverter controllers.
 
-*Latest release 20230217*:
-SPLinkCommand.cmd_plot: make the start-time optional, default to 5.
+*Latest release 20230612*:
+* SPLinkCommand: new print_known_datasets method, use in help.
+* SPLinkCommand.cmd_plot: if the start/stop times are out of order, swap them.
+* Assorted internal changes.
 
 I use this to gather and plot data from my solar inverter.
 
 ## Function `main(argv=None)`
 
 SP-Link command line mode.
 
@@ -86,21 +88,25 @@
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             stop-time       Optional stop time, default now.
                             An integer number of days before the current time
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             mode            A named graph mode, implying a group of fields.
+                            Providing '?' or 'help' prints the available
+                            datasets and field names.
         pull [-d dataset,...] [-F rsync-source] [-nx]
           Fetch and import data.
           -d dataset,...
                 Specify the datasets to import.
           -F    Fetch rsync source, default from $SPLINK_FETCH_SOURCE.
           -n    No action; pass -n to rsync. Just more convenient than putting it at the end.
           -x    Delete source files.
+        shell
+          Run a command prompt via cmd.Cmd using this command's subcommands.
 
 ## Class `SPLinkCSVDir(cs.fs.HasFSPath)`
 
 A class for working with SP-Link data downloads,
 referring to a particular `PerformanceData*` download directory.
 
 ## Class `SPLinkData(cs.fs.HasFSPath, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
@@ -142,21 +148,25 @@
 SPLinkDataFileInfo(fspath, sitename, dataset, unixtime, dotext)
 
 *Method `SPLinkDataFileInfo.__new__(_cls, fspath, sitename, dataset, unixtime, dotext)`*:
 Create new instance of SPLinkDataFileInfo(fspath, sitename, dataset, unixtime, dotext)
 
 ## Function `ts2001_unixtime(tzname=None)`
 
-Convert an SP-Link seconds-since-2001-01-01-local-time offset
-into a UNIX time.
+Return the SP-Link 2001-01-01-local-time epoch as a UNIX time.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* SPLinkCommand: new print_known_datasets method, use in help.
+* SPLinkCommand.cmd_plot: if the start/stop times are out of order, swap them.
+* Assorted internal changes.
+
 *Release 20230217*:
 SPLinkCommand.cmd_plot: make the start-time optional, default to 5.
 
 *Release 20220918*:
 * SPLinkData.plot: rename `key_specs` keyword parameter to mandatory posiitional `data_specs` parameter.
 * SPLinkData.resolve: accept multiple specification strings.
 * New SPLinkData.plot_data_from_spec(start,stop,data_spec,...) method to return a list of PlotSeries instances.
```

### Comparing `cs.splink-20230217/pyproject.toml` & `cs.splink-20230612/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,57 +5,60 @@
     { name = "Cameron Simpson", email = "cs@cskk.id.au" },
 ]
 keywords = [
     "python3",
 ]
 dependencies = [
     "arrow",
-    "cs.context>=20230212",
+    "cs.context>=20230331",
     "cs.csvutils>=20220606",
-    "cs.deco>=20230212",
-    "cs.fs>=20221221",
-    "cs.fstags>=20230217",
-    "cs.lex>=20230217.1",
+    "cs.deco>=20230331",
+    "cs.fs>=20230401",
+    "cs.fstags>=20230407",
+    "cs.lex>=20230401",
     "cs.logutils>=20230212",
-    "cs.mplutils>=20220918",
-    "cs.pfx>=20221118",
-    "cs.progress>=20230212",
-    "cs.psutils>=20221228",
-    "cs.resources>=20230217",
-    "cs.sqltags>=20230217",
-    "cs.tagset>=20230212",
-    "cs.timeseries>=20230217",
-    "cs.upd>=20230217",
+    "cs.mplutils>=20230407",
+    "cs.pfx>=20230604",
+    "cs.progress>=20230401",
+    "cs.psutils>=20230612",
+    "cs.resources>=20230503",
+    "cs.sqltags>=20230612",
+    "cs.tagset>=20230612",
+    "cs.timeseries>=20230612",
+    "cs.upd>=20230401",
+    "matplotlib",
     "python-dateutil",
     "typeguard",
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20230217"
+version = "20230612"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Assorted utility functions for working with data
 downloaded from Selectronics' SP-LINK programme
 which communicates with their solar inverter controllers.
 
-*Latest release 20230217*:
-SPLinkCommand.cmd_plot: make the start-time optional, default to 5.
+*Latest release 20230612*:
+* SPLinkCommand: new print_known_datasets method, use in help.
+* SPLinkCommand.cmd_plot: if the start/stop times are out of order, swap them.
+* Assorted internal changes.
 
 I use this to gather and plot data from my solar inverter.
 
 ## Function `main(argv=None)`
 
 SP-Link command line mode.
 
@@ -116,21 +119,25 @@
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             stop-time       Optional stop time, default now.
                             An integer number of days before the current time
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             mode            A named graph mode, implying a group of fields.
+                            Providing '?' or 'help' prints the available
+                            datasets and field names.
         pull [-d dataset,...] [-F rsync-source] [-nx]
           Fetch and import data.
           -d dataset,...
                 Specify the datasets to import.
           -F    Fetch rsync source, default from $SPLINK_FETCH_SOURCE.
           -n    No action; pass -n to rsync. Just more convenient than putting it at the end.
           -x    Delete source files.
+        shell
+          Run a command prompt via cmd.Cmd using this command's subcommands.
 
 ## Class `SPLinkCSVDir(cs.fs.HasFSPath)`
 
 A class for working with SP-Link data downloads,
 referring to a particular `PerformanceData*` download directory.
 
 ## Class `SPLinkData(cs.fs.HasFSPath, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin)`
@@ -172,21 +179,25 @@
 SPLinkDataFileInfo(fspath, sitename, dataset, unixtime, dotext)
 
 *Method `SPLinkDataFileInfo.__new__(_cls, fspath, sitename, dataset, unixtime, dotext)`*:
 Create new instance of SPLinkDataFileInfo(fspath, sitename, dataset, unixtime, dotext)
 
 ## Function `ts2001_unixtime(tzname=None)`
 
-Convert an SP-Link seconds-since-2001-01-01-local-time offset
-into a UNIX time.
+Return the SP-Link 2001-01-01-local-time epoch as a UNIX time.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* SPLinkCommand: new print_known_datasets method, use in help.
+* SPLinkCommand.cmd_plot: if the start/stop times are out of order, swap them.
+* Assorted internal changes.
+
 *Release 20230217*:
 SPLinkCommand.cmd_plot: make the start-time optional, default to 5.
 
 *Release 20220918*:
 * SPLinkData.plot: rename `key_specs` keyword parameter to mandatory posiitional `data_specs` parameter.
 * SPLinkData.resolve: accept multiple specification strings.
 * New SPLinkData.plot_data_from_spec(start,stop,data_spec,...) method to return a list of PlotSeries instances.
```

