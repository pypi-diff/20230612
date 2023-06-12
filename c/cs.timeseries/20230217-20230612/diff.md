# Comparing `tmp/cs.timeseries-20230217.tar.gz` & `tmp/cs.timeseries-20230612.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.timeseries-20230217.tar", last modified: Fri Feb 17 09:34:28 2023, max compression
+gzip compressed data, was "cs.timeseries-20230612.tar", last modified: Mon Jun 12 04:53:18 2023, max compression
```

## Comparing `cs.timeseries-20230217.tar` & `cs.timeseries-20230612.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 09:34:28.106492 cs.timeseries-20230217/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-02-17 09:34:13.000000 cs.timeseries-20230217/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    25059 2023-02-17 09:34:28.106658 cs.timeseries-20230217/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    53059 2023-02-17 09:34:15.000000 cs.timeseries-20230217/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 09:34:28.101153 cs.timeseries-20230217/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 09:34:28.101474 cs.timeseries-20230217/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 09:34:28.103480 cs.timeseries-20230217/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)   115475 2023-02-17 09:34:04.000000 cs.timeseries-20230217/lib/python/cs/timeseries.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 09:34:28.106255 cs.timeseries-20230217/lib/python/cs.timeseries.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    25059 2023-02-17 09:34:28.000000 cs.timeseries-20230217/lib/python/cs.timeseries.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      373 2023-02-17 09:34:28.000000 cs.timeseries-20230217/lib/python/cs.timeseries.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-02-17 09:34:28.000000 cs.timeseries-20230217/lib/python/cs.timeseries.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       44 2023-02-17 09:34:28.000000 cs.timeseries-20230217/lib/python/cs.timeseries.egg-info/entry_points.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      497 2023-02-17 09:34:28.000000 cs.timeseries-20230217/lib/python/cs.timeseries.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-02-17 09:34:28.000000 cs.timeseries-20230217/lib/python/cs.timeseries.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    25848 2023-02-17 09:34:19.000000 cs.timeseries-20230217/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)     1467 2023-02-17 09:34:28.107376 cs.timeseries-20230217/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-02-17 09:34:15.000000 cs.timeseries-20230217/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:53:18.440624 cs.timeseries-20230612/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-12 04:53:00.000000 cs.timeseries-20230612/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    25694 2023-06-12 04:53:18.440793 cs.timeseries-20230612/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    53543 2023-06-12 04:53:03.000000 cs.timeseries-20230612/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:53:18.435791 cs.timeseries-20230612/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:53:18.436131 cs.timeseries-20230612/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:53:18.438191 cs.timeseries-20230612/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)   114991 2023-06-12 04:52:37.000000 cs.timeseries-20230612/lib/python/cs/timeseries.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:53:18.440342 cs.timeseries-20230612/lib/python/cs.timeseries.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    25694 2023-06-12 04:53:18.000000 cs.timeseries-20230612/lib/python/cs.timeseries.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      373 2023-06-12 04:53:18.000000 cs.timeseries-20230612/lib/python/cs.timeseries.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-12 04:53:18.000000 cs.timeseries-20230612/lib/python/cs.timeseries.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       44 2023-06-12 04:53:18.000000 cs.timeseries-20230612/lib/python/cs.timeseries.egg-info/entry_points.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      491 2023-06-12 04:53:18.000000 cs.timeseries-20230612/lib/python/cs.timeseries.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-12 04:53:18.000000 cs.timeseries-20230612/lib/python/cs.timeseries.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    26477 2023-06-12 04:53:09.000000 cs.timeseries-20230612/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)     1461 2023-06-12 04:53:18.441460 cs.timeseries-20230612/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-12 04:53:03.000000 cs.timeseries-20230612/setup.py
```

### Comparing `cs.timeseries-20230217/PKG-INFO` & `cs.timeseries-20230612/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.timeseries
-Version: 20230217
+Version: 20230612
 Summary: Efficient portable machine native columnar file storage of time series data for double float and signed 64-bit integers.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
@@ -16,17 +16,19 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 Provides-Extra: pandas
 
 Efficient portable machine native columnar file storage of time
 series data for double float and signed 64-bit integers.
 
-*Latest release 20230217*:
-* TimeSeriesFile.save_to: use atomic_filename() to create the updated file.
-* Other small fixes and updates.
+*Latest release 20230612*:
+* Epoch.promote: do not special case None, let Optional[Epoch] type annoations handle that.
+* Mark PlotSeries.promote as incomplete (raises RuntimeError).
+* TimespanPolicy.promote: use cls.from_name() instead of TimespanPolicy.from_name().
+* Assorted other small updates.
 
 The core purpose is to provide time series data storage; there
 are assorted convenience methods to export arbitrary subsets
 of the data for use by other libraries in common forms, such
 as dataframes or series, numpy arrays and simple lists.
 There are also some simple plot methods for plotting graphs.
 
@@ -115,15 +117,15 @@
 * `utcoffset`: optional UTC offset for presentation
 Other keyword parameters are passed to `Axes.scatter`.
 
 ## Class `PlotSeries(PlotSeries, builtins.tuple, cs.deco.Promotable)`
 
 Information about a series to be plotted:
 - `label`: the label for this series
-- `series`: an series
+- `series`: a `Series`
 - `extra`: a `dict` of extra information such as plot styling
 
 ## Class `TimePartition(TimePartition, builtins.tuple, TimeStepsMixin)`
 
 A `namedtuple` for a slice of time with the following attributes:
 * `epoch`: the reference `Epoch`
 * `name`: the name for this slice
@@ -228,14 +230,16 @@
                             dateutil.parser.parse.
             stop-time       Optional stop time, default now.
                             An integer number of days before the current time
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             glob|fields     If glob is supplied, constrain the keys of
                             a TimeSeriesDataDir by the glob.
+        shell
+          Run a command prompt via cmd.Cmd using this command's subcommands.
 
 ## Class `TimeSeriesCommand(TimeSeriesBaseCommand, cs.cmdutils.BaseCommand)`
 
 Command line interface to `TimeSeries` data files.
 
 Command line usage:
 
@@ -292,14 +296,16 @@
                             dateutil.parser.parse.
             stop-time       Optional stop time, default now.
                             An integer number of days before the current time
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             glob|fields     If glob is supplied, constrain the keys of
                             a TimeSeriesDataDir by the glob.
+        shell
+          Run a command prompt via cmd.Cmd using this command's subcommands.
         test [testnames...]
           Run some tests of functionality.
 
 ## Class `TimeSeriesDataDir(TimeSeriesMapping, builtins.dict, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin, cs.fs.HasFSPath, cs.configutils.HasConfigIni, HasEpochMixin, TimeStepsMixin)`
 
 A directory containing a collection of `TimeSeriesPartitioned` subdirectories.
 
@@ -354,15 +360,15 @@
 
 Presently the mode used is triggered by the access method.
 Using the `peek` and `poke` methods uses `mmap` by default.
 Other accesses default to use the in-memory mode.
 Access to the `.array` property forces use of the `array` mode.
 Poll/update operations should usually choose to use `peek`/`poke`.
 
-*Method `TimeSeriesFile.__init__(self, fspath: str, typecode: Optional[cs.timeseries.TypeCode] = None, *, epoch: Optional[cs.timeseries.Epoch] = None, fill=None, fstags=None)`*:
+*Method `TimeSeriesFile.__init__(self, fspath: str, typecode: Optional[cs.timeseries.TypeCode] = None, *, epoch: Optional[cs.timeseries.Epoch] = None, fill=None, fstags: cs.fstags.FSTags)`*:
 Prepare a new time series stored in the file at `fspath`
 containing machine native data for the time series values.
 
 Parameters:
 * `fspath`: the filename of the data file
 * `typecode` optional expected `array.typecode` value of the data;
   if specified and the data file exists, they must match;
@@ -411,15 +417,15 @@
 A collection of `TimeSeries` files in a subdirectory.
 We have one of these for each `TimeSeriesDataDir` key.
 
 This class manages a collection of files
 named by the partition from a `TimespanPolicy`,
 which dictates which partition holds the datum for a UNIX time.
 
-*Method `TimeSeriesPartitioned.__init__(self, dirpath: str, typecode: Optional[cs.timeseries.TypeCode] = None, *, epoch: Optional[cs.timeseries.Epoch] = None, policy, fstags: Optional[cs.fstags.FSTags] = None)`*:
+*Method `TimeSeriesPartitioned.__init__(self, dirpath: str, typecode: Optional[cs.timeseries.TypeCode] = None, *, epoch: Optional[cs.timeseries.Epoch] = None, policy, fstags: cs.fstags.FSTags)`*:
 Initialise the `TimeSeriesPartitioned` instance.
 
 Parameters:
 * `dirpath`: the directory filesystem path,
   known as `.fspath` within the instance
 * `typecode`: the `array` type code for the data
 * `epoch`: the time series `Epoch`
@@ -510,14 +516,20 @@
 `dateutil.tz.gettz()`, the local system timezone.
 Otherwise it returns `dateutil.tz.gettz(tzspec)`.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* Epoch.promote: do not special case None, let Optional[Epoch] type annoations handle that.
+* Mark PlotSeries.promote as incomplete (raises RuntimeError).
+* TimespanPolicy.promote: use cls.from_name() instead of TimespanPolicy.from_name().
+* Assorted other small updates.
+
 *Release 20230217*:
 * TimeSeriesFile.save_to: use atomic_filename() to create the updated file.
 * Other small fixes and updates.
 
 *Release 20220918*:
 * TimeSeriesMapping.as_pd_dataframe: rename `keys` to `df_data`, and accept either a time series key or a `(key,series)` tuple.
 * TimeSeriesMapping.as_pd_dataframe: default `key_map`: annotate columns with their original CSV headers if present.
```

### Comparing `cs.timeseries-20230217/README.md` & `cs.timeseries-20230612/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Efficient portable machine native columnar file storage of time
 series data for double float and signed 64-bit integers.
 
-*Latest release 20230217*:
-* TimeSeriesFile.save_to: use atomic_filename() to create the updated file.
-* Other small fixes and updates.
+*Latest release 20230612*:
+* Epoch.promote: do not special case None, let Optional[Epoch] type annoations handle that.
+* Mark PlotSeries.promote as incomplete (raises RuntimeError).
+* TimespanPolicy.promote: use cls.from_name() instead of TimespanPolicy.from_name().
+* Assorted other small updates.
 
 The core purpose is to provide time series data storage; there
 are assorted convenience methods to export arbitrary subsets
 of the data for use by other libraries in common forms, such
 as dataframes or series, numpy arrays and simple lists.
 There are also some simple plot methods for plotting graphs.
 
@@ -114,17 +116,15 @@
 and a `step` defining the width of a time slot.
 
 *Method `Epoch.info_dict(self, d=None)`*:
 Return an informational `dict` containing salient information
 about this `Epoch`, handy for use with `pformat()` or `pprint()`.
 
 *Method `Epoch.promote(epochy)`*:
-Promote `epochy` to an `Epoch` (except for `None`).
-
-`None` remains `None`.
+Promote `epochy` to an `Epoch`.
 
 An `Epoch` remains unchanged.
 
 An `int` or `float` argument will be used as the `step` in
 an `Epoch` starting at `0`.
 
 A 2-tuple of `(start,step)` will be used to construct a new `Epoch` directly.
@@ -172,15 +172,15 @@
 * `utcoffset`: optional UTC offset for presentation
 Other keyword parameters are passed to `Axes.scatter`.
 
 ## Class `PlotSeries(PlotSeries, builtins.tuple, cs.deco.Promotable)`
 
 Information about a series to be plotted:
 - `label`: the label for this series
-- `series`: an series
+- `series`: a `Series`
 - `extra`: a `dict` of extra information such as plot styling
 
 *Method `PlotSeries.promote(data, tsmap=None, extra=None)`*:
 Promote `data` to a `PlotSeries`.
 
 ## Class `TimePartition(TimePartition, builtins.tuple, TimeStepsMixin)`
 
@@ -301,22 +301,21 @@
 to the expected length.
 
 If `astart` is an offset before the start of the array
 raise an `IndexError` unless `prepad` is true,
 in which case the list of values will be prepended
 with enough of `self.fill` to reach the array start.
 
-*Method `TimeSeries.plot(self, start, stop, *, figure=None, ax=None, label=None, runstate=None, utcoffset, **plot_kw) -> matplotlib.axes._axes.Axes`*:
+*Method `TimeSeries.plot(self, start, stop, *, figure=None, ax=None, label=None, utcoffset, **plot_kw) -> matplotlib.axes._axes.Axes`*:
 Convenience shim for `DataFrame.plot` to plot data from
 `start` to `stop`.  Return the plot `Axes`.
 
 Parameters:
 * `start`,`stop`: the time range
 * `label`: optional label for the graph
-* `runstate`: optional `RunState`, ignored in this implementation
 * `utcoffset`: optional timestamp skew from UTC in seconds
 * `figure`,`ax`: optional arguments as for `cs.mplutils.axes`
 Other keyword parameters are passed to `DataFrame.plot`.
 
 *Method `TimeSeries.slice(self, start, stop, pad=False, prepad=False)`*:
 Return a slice of the underlying array
 for the times `start:stop`.
@@ -379,14 +378,16 @@
                             dateutil.parser.parse.
             stop-time       Optional stop time, default now.
                             An integer number of days before the current time
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             glob|fields     If glob is supplied, constrain the keys of
                             a TimeSeriesDataDir by the glob.
+        shell
+          Run a command prompt via cmd.Cmd using this command's subcommands.
 
 *Method `TimeSeriesBaseCommand.cmd_fetch(self, argv)`*:
 Usage: {cmd} ...
 Fetch raw data files from the primary source to a local spool.
 To be implemented in subclasses.
 
 *Method `TimeSeriesBaseCommand.cmd_import(self, argv)`*:
@@ -491,17 +492,21 @@
                             dateutil.parser.parse.
             stop-time       Optional stop time, default now.
                             An integer number of days before the current time
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             glob|fields     If glob is supplied, constrain the keys of
                             a TimeSeriesDataDir by the glob.
+        shell
+          Run a command prompt via cmd.Cmd using this command's subcommands.
         test [testnames...]
           Run some tests of functionality.
 
+*`TimeSeriesCommand.Options`*
+
 *Method `TimeSeriesCommand.apply_preargv(self, argv)`*:
 Parse a leading time series filesystem path from `argv`,
 set `self.options.ts` to the time series,
 return modified `argv`.
 
 *Method `TimeSeriesCommand.cmd_dump(self, argv)`*:
 Usage: {cmd}
@@ -616,15 +621,15 @@
 
 Presently the mode used is triggered by the access method.
 Using the `peek` and `poke` methods uses `mmap` by default.
 Other accesses default to use the in-memory mode.
 Access to the `.array` property forces use of the `array` mode.
 Poll/update operations should usually choose to use `peek`/`poke`.
 
-*Method `TimeSeriesFile.__init__(self, fspath: str, typecode: Optional[cs.timeseries.TypeCode] = None, *, epoch: Optional[cs.timeseries.Epoch] = None, fill=None, fstags=None)`*:
+*Method `TimeSeriesFile.__init__(self, fspath: str, typecode: Optional[cs.timeseries.TypeCode] = None, *, epoch: Optional[cs.timeseries.Epoch] = None, fill=None, fstags: cs.fstags.FSTags)`*:
 Prepare a new time series stored in the file at `fspath`
 containing machine native data for the time series values.
 
 Parameters:
 * `fspath`: the filename of the data file
 * `typecode` optional expected `array.typecode` value of the data;
   if specified and the data file exists, they must match;
@@ -795,15 +800,15 @@
 Create a new entry for `key` if missing.
 This implementation looks up the rules.
 
 *Method `TimeSeriesMapping.__setitem__(self, key: str, ts)`*:
 Insert a time series into this `TimeSeriesMapping`.
 `key` may not already be present.
 
-*Method `TimeSeriesMapping.as_pd_dataframe(self, start=None, stop=None, df_data: Optional[Iterable[Union[str, Tuple[str, Any]]]] = None, *, key_map=None, runstate=None, utcoffset=None)`*:
+*Method `TimeSeriesMapping.as_pd_dataframe(self, start=None, stop=None, df_data: Optional[Iterable[Union[str, Tuple[str, Any]]]] = None, *, key_map=None, runstate: cs.resources.RunState, utcoffset=None)`*:
 Return a `numpy.DataFrame` containing the specified data.
 
 Parameters:
 * `start`: start time of the data
 * `stop`: end time of the data
 * `df_data`: optional iterable of data, default from `self.keys()`;
   each item may either be a time series name
@@ -821,26 +826,25 @@
 The `array` type code for `key`.
 This default method returns `'d'` (float64).
 
 *Method `TimeSeriesMapping.make_ts(self, key)`*:
 Return the `TimeSeries` for `key`,
 creating it if necessary.
 
-*Method `TimeSeriesMapping.plot(self, start, stop, plot_data=None, *, figure=None, ax=None, label=None, runstate=None, utcoffset, stacked=False, kind=None, **plot_kw) -> matplotlib.axes._axes.Axes`*:
+*Method `TimeSeriesMapping.plot(self, start, stop, plot_data=None, *, figure=None, ax=None, label=None, runstate: cs.resources.RunState, utcoffset, stacked=False, kind=None, **plot_kw) -> matplotlib.axes._axes.Axes`*:
 Convenience shim for `DataFrame.plot` to plot data from
 `start` to `stop` for each timeseries in `plot_data`.
 Return the plot `Axes`.
 
 Parameters:
 * `start`: optional start, default `self.start`
 * `stop`: optional stop, default `self.stop`
 * `plot_data`: optional iterable of plot data,
   default `sorted(self.keys())`
 * `label`: optional label for the graph
-* `runstate`: optional `RunState` to allow interruption
 * `figure`,`ax`: optional arguments as for `cs.mplutils.axes`
 Other keyword parameters are passed to `DataFrame.plot`.
 
 The plot data items are either
 a key for a timeseries from this `TimeSeriesMapping`
 or a `(label,series)` 2-tuple being a label and timeseries data.
 
@@ -891,15 +895,15 @@
 A collection of `TimeSeries` files in a subdirectory.
 We have one of these for each `TimeSeriesDataDir` key.
 
 This class manages a collection of files
 named by the partition from a `TimespanPolicy`,
 which dictates which partition holds the datum for a UNIX time.
 
-*Method `TimeSeriesPartitioned.__init__(self, dirpath: str, typecode: Optional[cs.timeseries.TypeCode] = None, *, epoch: Optional[cs.timeseries.Epoch] = None, policy, fstags: Optional[cs.fstags.FSTags] = None)`*:
+*Method `TimeSeriesPartitioned.__init__(self, dirpath: str, typecode: Optional[cs.timeseries.TypeCode] = None, *, epoch: Optional[cs.timeseries.Epoch] = None, policy, fstags: cs.fstags.FSTags)`*:
 Initialise the `TimeSeriesPartitioned` instance.
 
 Parameters:
 * `dirpath`: the directory filesystem path,
   known as `.fspath` within the instance
 * `typecode`: the `array` type code for the data
 * `epoch`: the time series `Epoch`
@@ -948,15 +952,15 @@
 Return the time span name from a `TimeSeriesFile` filename.
 
 *Method `TimeSeriesPartitioned.partitioned_spans(self, start, stop)`*:
 Generator yielding a sequence of `TimePartition`s covering
 the range `start:stop` such that `start` falls within the first
 partition via `self.policy`.
 
-*Method `TimeSeriesPartitioned.plot(self, start, stop, *, figure=None, ax=None, label=None, runstate=None, **plot_kw) -> matplotlib.axes._axes.Axes`*:
+*Method `TimeSeriesPartitioned.plot(self, start, stop, *, figure=None, ax=None, label=None, **plot_kw) -> matplotlib.axes._axes.Axes`*:
 Convenience shim for `DataFrame.plot` to plot data from
 `start` to `stop`.
 Return the plot `Axes`.
 
 Parameters:
 * `start`,`stop`: the time range
 * `figure`,`ax`: optional arguments as for `cs.mplutils.axes`
@@ -1006,17 +1010,16 @@
 * `span_for_time`: return a `TimePartition` from a UNIX time
 * `span_for_name`: return a `TimePartition` from a partition name
 
 *Method `TimespanPolicy.__init__(self, epoch: cs.timeseries.Epoch)`*:
 Initialise the policy.
 
 *Method `TimespanPolicy.from_name(policy_name: str, epoch: Optional[cs.timeseries.Epoch] = None, **policy_kw)`*:
-Factory method to return a new `TimespanPolicy` instance
-from the policy name,
-which indexes `TimespanPolicy.FACTORIES`.
+Factory method to return a new `cls` instance from the policy name,
+which indexes `cls.FACTORIES`.
 
 *Method `TimespanPolicy.name_for_time(self, when)`*:
 Return a time span name for the UNIX time `when`.
 
 *Method `TimespanPolicy.partitioned_spans(self, start, stop)`*:
 Generator yielding a sequence of `TimePartition`s covering
 the range `start:stop` such that `start` falls within the first
@@ -1234,14 +1237,20 @@
 `dateutil.tz.gettz()`, the local system timezone.
 Otherwise it returns `dateutil.tz.gettz(tzspec)`.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* Epoch.promote: do not special case None, let Optional[Epoch] type annoations handle that.
+* Mark PlotSeries.promote as incomplete (raises RuntimeError).
+* TimespanPolicy.promote: use cls.from_name() instead of TimespanPolicy.from_name().
+* Assorted other small updates.
+
 *Release 20230217*:
 * TimeSeriesFile.save_to: use atomic_filename() to create the updated file.
 * Other small fixes and updates.
 
 *Release 20220918*:
 * TimeSeriesMapping.as_pd_dataframe: rename `keys` to `df_data`, and accept either a time series key or a `(key,series)` tuple.
 * TimeSeriesMapping.as_pd_dataframe: default `key_map`: annotate columns with their original CSV headers if present.
```

### Comparing `cs.timeseries-20230217/lib/python/cs/timeseries.py` & `cs.timeseries-20230612/lib/python/cs/timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     data; see my `cs.splink` module which is built on this module.
 '''
 
 from abc import ABC, abstractmethod
 from array import array, typecodes  # pylint: disable=no-name-in-module
 from collections import defaultdict, namedtuple
 from contextlib import contextmanager
+from dataclasses import dataclass
 from datetime import datetime, timedelta, tzinfo
 from fnmatch import fnmatch
 from functools import partial
 from getopt import GetoptError
 from math import nan  # pylint: disable=no-name-in-module
 from mmap import (
     mmap,
@@ -87,27 +88,27 @@
 from cs.cmdutils import BaseCommand
 from cs.configutils import HasConfigIni
 from cs.context import stackattrs
 from cs.csvutils import csv_import
 from cs.deco import cachedmethod, decorator, promote, Promotable
 from cs.fileutils import atomic_filename
 from cs.fs import HasFSPath, fnmatchdir, needdir, shortpath
-from cs.fstags import FSTags
+from cs.fstags import FSTags, uses_fstags
 from cs.lex import is_identifier, s, r
 from cs.logutils import warning
 from cs.mappings import column_name_to_identifier
 from cs.mplutils import axes, remove_decorations, print_figure, save_figure
 from cs.pfx import Pfx, pfx, pfx_call, pfx_method
 from cs.progress import progressbar
 from cs.py.modules import import_extra
-from cs.resources import MultiOpenMixin
+from cs.resources import MultiOpenMixin, RunState, uses_runstate
 from cs.result import CancellationError
 from cs.upd import Upd, UpdProxy, print  # pylint: disable=redefined-builtin
 
-__version__ = '20230217'
+__version__ = '20230612'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
     ],
@@ -436,21 +437,15 @@
     if isinstance(ts, TimeSeries):
       # a single timeseries, no key
       if argv:
         raise GetoptError(
             "fields:%r should not be suppplied for a %s" % (argv, s(ts))
         )
       ax = ts.plot(
-          start,
-          stop,
-          ax=ax,
-          runstate=runstate,
-          tz=tz,
-          figsize=(plot_dx, plot_dy),
-          **plot_kw
+          start, stop, ax=ax, tz=tz, figsize=(plot_dx, plot_dy), **plot_kw
       )  # pylint: disable=missing-kwoa
     elif isinstance(ts, TimeSeriesMapping):
       # multiple timeseries each with their own key
       if argv:
         keys = ts.keys(argv)
         if not keys:
           raise GetoptError(
@@ -465,15 +460,14 @@
           subplots=options.multi,
           sharex=options.multi,
       )
       ax = ts.plot(
           start,
           stop,
           keys,
-          runstate=runstate,
           tz=tz,
           ax=ax,
           **plot_kw,
       )  # pylint: too-many-function-args.disable=missing-kwoa
       figure = (ax[0] if options.multi else ax).figure
     else:
       raise RuntimeError("unhandled type %s" % (s(ts),))
@@ -508,17 +502,18 @@
   DATE_CONV_MAP = {
       'int': int,
       'float': float,
       'date': lambda d: pfx_call(arrow.get, d, tzinfo='local').timestamp(),
       'iso8601': lambda d: pfx_call(arrow.get, d, tzinfo='local').timestamp(),
   }
 
-  def apply_defaults(self):
-    self.options.ts_step = None  # the time series step
-    self.options.ts = None
+  @dataclass
+  class Options(BaseCommand.Options):
+    ts_step: Optional[float] = None  # the time series step
+    ts: Optional["TimeSeries"] = None
 
   def apply_opt(self, opt, val):
     if opt == '-s':
       try:
         ts_step = pfx_call(float, val)
       except ValueError as e:
         raise GetoptError("not a floating point value: %s" % (e,)) from e
@@ -1005,15 +1000,15 @@
     yaxis.append(value_func(event))
   ax.scatter(xaxis, yaxis, **scatter_kw)
   return ax
 
 class PlotSeries(namedtuple('PlotSeries', 'label series extra'), Promotable):
   ''' Information about a series to be plotted:
       - `label`: the label for this series
-      - `series`: an series
+      - `series`: a `Series`
       - `extra`: a `dict` of extra information such as plot styling
   '''
 
   @classmethod
   @timerange
   def promote(cls, data, tsmap=None, extra=None):
     ''' Promote `data` to a `PlotSeries`.
@@ -1215,17 +1210,15 @@
   def typecode(self):
     ''' The `array` typecode for the times from this `Epoch`.
     '''
     return TypeCode(type(self.start))
 
   @classmethod
   def promote(cls, epochy):
-    ''' Promote `epochy` to an `Epoch` (except for `None`).
-
-        `None` remains `None`.
+    ''' Promote `epochy` to an `Epoch`.
 
         An `Epoch` remains unchanged.
 
         An `int` or `float` argument will be used as the `step` in
         an `Epoch` starting at `0`.
 
         A 2-tuple of `(start,step)` will be used to construct a new `Epoch` directly.
@@ -1455,25 +1448,23 @@
       self,
       start,
       stop,
       *,
       figure=None,
       ax=None,
       label=None,
-      runstate=None,  # pylint: disable=unused-argument
       utcoffset,
       **plot_kw,
   ) -> Axes:
     ''' Convenience shim for `DataFrame.plot` to plot data from
         `start` to `stop`.  Return the plot `Axes`.
 
         Parameters:
         * `start`,`stop`: the time range
         * `label`: optional label for the graph
-        * `runstate`: optional `RunState`, ignored in this implementation
         * `utcoffset`: optional timestamp skew from UTC in seconds
         * `figure`,`ax`: optional arguments as for `cs.mplutils.axes`
         Other keyword parameters are passed to `DataFrame.plot`.
     '''
     pd = import_extra('pandas', DISTINFO)
     ax = axes(figure, ax)
     if label is None:
@@ -1650,24 +1641,25 @@
       Poll/update operations should usually choose to use `peek`/`poke`.
   '''
 
   DOTEXT = '.csts'
 
   # pylint: disable=too-many-branches,too-many-statements
   @pfx_method
+  @uses_fstags
   @promote
   @typechecked
   def __init__(
       self,
       fspath: str,
       typecode: Optional[TypeCode] = None,
       *,
       epoch: Optional[Epoch] = None,
       fill=None,
-      fstags=None,
+      fstags: FSTags,
   ):
     ''' Prepare a new time series stored in the file at `fspath`
         containing machine native data for the time series values.
 
         Parameters:
         * `fspath`: the filename of the data file
         * `typecode` optional expected `array.typecode` value of the data;
@@ -1680,19 +1672,17 @@
           if not specified then the data file must exist
           and the `epoch` will be obtained from its header
         * `fill`: optional default fill values for `pad_to`;
           if unspecified, fill with `0` for `'q'`
           and `float('nan')` for `'d'`
     '''
     HasFSPath.__init__(self, fspath)
-    if fstags is None:
-      fstags = FSTags()
     self.fstags = fstags
     try:
-      header, = TimeSeriesFileHeader.scan_fspath(self.fspath, max_count=1)
+      header, = TimeSeriesFileHeader.scan(self.fspath, max_count=1)
     except FileNotFoundError:
       # a missing file is ok, other exceptions are not
       ok = True
       if typecode is None:
         ok = False
         warning("no typecode supplied and no data file %r", fspath)
       if epoch is None:
@@ -2253,17 +2243,16 @@
   # pylint: disable=keyword-arg-before-vararg
   @classmethod
   @promote
   @typechecked
   def from_name(
       cls, policy_name: str, epoch: Optional[Epoch] = None, **policy_kw
   ):
-    ''' Factory method to return a new `TimespanPolicy` instance
-        from the policy name,
-        which indexes `TimespanPolicy.FACTORIES`.
+    ''' Factory method to return a new `cls` instance from the policy name,
+        which indexes `cls.FACTORIES`.
     '''
     if cls is not TimespanPolicy:
       raise TypeError(
           "TimespanPolicy.from_name is not meaningful from a subclass (%s)" %
           (cls.__name__,)
       )
     policy = cls.FACTORIES[policy_name](epoch=epoch, **policy_kw)
@@ -2287,15 +2276,15 @@
           "TimespanPolicy.promote is not meaningful from a subclass (%s)" %
           (cls.__name__,)
       )
     if not isinstance(policy, TimespanPolicy):
       if epoch is None:
         raise ValueError("epoch may not be None if promotion is required")
       if isinstance(policy, str):
-        policy = TimespanPolicy.from_name(policy, epoch=epoch, **policy_kw)
+        policy = cls.from_name(policy, epoch=epoch, **policy_kw)
       elif isinstance(policy, type) and issubclass(policy, TimespanPolicy):
         policy = policy(epoch=epoch, **policy_kw)
       else:
         raise TypeError(
             "%s.promote: do not know how to promote %s" %
             (cls.__name__, r(policy))
         )
@@ -2687,23 +2676,24 @@
   def key_typecode(self, key):
     ''' The `array` type code for `key`.
         This default method returns `'d'` (float64).
     '''
     return 'd'
 
   @pfx
+  @uses_runstate
   @typechecked
   def as_pd_dataframe(
       self,
       start=None,
       stop=None,
       df_data: Optional[Iterable[Union[str, Tuple[str, Any]]]] = None,
       *,
       key_map=None,
-      runstate=None,
+      runstate: RunState,
       utcoffset=None,
   ):
     ''' Return a `numpy.DataFrame` containing the specified data.
 
         Parameters:
         * `start`: start time of the data
         * `stop`: end time of the data
@@ -2732,15 +2722,15 @@
       utcoffset = 0.0
     # we require the indices to ensure that the dataframe covers
     # the entire time range
     indices = as_datetime64s(self.range(start, stop), utcoffset=utcoffset)
     data_dict = {}
     with UpdProxy(prefix="gather fields: ") as proxy:
       for data in progressbar(df_data, "gather fields"):
-        if runstate and runstate.cancelled:
+        if runstate.cancelled:
           raise CancellationError
         pfx_context = (
             data
             if isinstance(data, str) else f'{data[0]}:{type(data[1]).__name__}'
         )
         proxy.text = pfx_context
         with Pfx(pfx_context):
@@ -2749,15 +2739,15 @@
             key = data
             ts = self[key]
             series = ts.as_pd_series(start, stop, utcoffset=utcoffset)
           else:
             key, series = data
           data_key = key_map.get(key, key)
           data_dict[data_key] = series
-    if runstate and runstate.cancelled:
+    if runstate.cancelled:
       raise CancellationError
     return pfx_call(
         pd.DataFrame,
         data=data_dict,
         index=indices,
         copy=False,
     )
@@ -2789,25 +2779,26 @@
       key_map = {column: self.csv_header(column) for column in columns}
     df = self.as_pd_dataframe(start, stop, columns, key_map=key_map)
     if df_mangle:
       df_mangle(df)
     df.to_csv(f, **to_csv_kw)
 
   @timerange
+  @uses_runstate
   @typechecked
   def plot(
       self,
       start,
       stop,
       plot_data=None,
       *,
       figure=None,
       ax=None,
       label=None,
-      runstate=None,
+      runstate: RunState,
       utcoffset,
       stacked=False,
       kind=None,
       **plot_kw,
   ) -> Axes:
     ''' Convenience shim for `DataFrame.plot` to plot data from
         `start` to `stop` for each timeseries in `plot_data`.
@@ -2815,15 +2806,14 @@
 
         Parameters:
         * `start`: optional start, default `self.start`
         * `stop`: optional stop, default `self.stop`
         * `plot_data`: optional iterable of plot data,
           default `sorted(self.keys())`
         * `label`: optional label for the graph
-        * `runstate`: optional `RunState` to allow interruption
         * `figure`,`ax`: optional arguments as for `cs.mplutils.axes`
         Other keyword parameters are passed to `DataFrame.plot`.
 
         The plot data items are either
         a key for a timeseries from this `TimeSeriesMapping`
         or a `(label,series)` 2-tuple being a label and timeseries data.
     '''
@@ -2836,15 +2826,15 @@
     df = self.as_pd_dataframe(
         start,
         stop,
         plot_data,
         runstate=runstate,
         utcoffset=utcoffset,
     )
-    if runstate and runstate.cancelled:
+    if runstate.cancelled:
       raise CancellationError
     return df.plot(ax=ax, kind=kind, stacked=stacked, **plot_kw)
 
   @pfx_method
   def read_csv(self, csvpath, column_name_map=None, **pd_read_csv_kw):
     ''' Shim for `pandas.read_csv` to read a CSV file and save the contents
         in this `TimeSeriesMapping`.
@@ -2925,29 +2915,28 @@
   # particularly we do not want to create the data dir with a
   # subclass and then not find the config reading with the generic
   # class
   CONFIG_SECTION_NAME = 'TimeSeriesDataDir'
 
   # pylint: disable=too-many-branches,too-many-statements
   @pfx_method
+  @uses_fstags
   @promote
   @typechecked
   def __init__(
       self,
       fspath,
       *,
       epoch: Optional[Epoch] = None,
       policy=None,  # :TimespanPolicy
       tz: Optional[str] = None,
-      fstags: Optional[FSTags] = None,
+      fstags: FSTags,
   ):
     HasConfigIni.__init__(self, self.CONFIG_SECTION_NAME)
     HasFSPath.__init__(self, fspath)
-    if fstags is None:
-      fstags = FSTags()
     self.fstags = fstags
     config = self.config
     if not isdirpath(fspath):
       # new data dir, create it and save config
       pfx_call(needdir, fspath)
       config.start = epoch.start
       config.step = epoch.step
@@ -3109,24 +3098,25 @@
       We have one of these for each `TimeSeriesDataDir` key.
 
       This class manages a collection of files
       named by the partition from a `TimespanPolicy`,
       which dictates which partition holds the datum for a UNIX time.
   '''
 
+  @uses_fstags
   @promote
   @typechecked
   def __init__(
       self,
       dirpath: str,
       typecode: Optional[TypeCode] = None,
       *,
       epoch: Optional[Epoch] = None,
       policy,  # :TimespanPolicy,
-      fstags: Optional[FSTags] = None,
+      fstags: FSTags,
   ):
     ''' Initialise the `TimeSeriesPartitioned` instance.
 
         Parameters:
         * `dirpath`: the directory filesystem path,
           known as `.fspath` within the instance
         * `typecode`: the `array` type code for the data
@@ -3150,29 +3140,27 @@
         This class does not set these tags (that would presume write
         access to the parent directory or its `.fstags` file)
         when a `TimeSeriesPartitioned` is made by a `TimeSeriesDataDir`
         instance it sets these flags.
     '''
     policy = TimespanPolicy.promote(policy, epoch)
     HasFSPath.__init__(self, dirpath)
-    if fstags is None:
-      fstags = FSTags()
     if typecode is None:
       typecode = TypeCode(self.tags.typecode)
     policy = TimespanPolicy.promote(policy, epoch=epoch)
     assert isinstance(policy, ArrowBasedTimespanPolicy)
     TimeSeries.__init__(self, policy.epoch, typecode)
     self.policy = policy
     self.fstags = fstags
     self._ts_by_partition = {}
 
   def __str__(self):
     return "%s(%s,%r,%s,%s)" % (
         type(self).__name__,
-        shortpath(self.fspath),
+        getattr(self, 'shortpath', 'NO_FSPATH'),
         getattr(self, 'typecode', 'NO_TYPECODE_YET'),
         getattr(self, 'epoch', 'NO_EPOCH_YET'),
         getattr(self, 'policy', 'NO_POLICY_YET'),
     )
 
   __repr__ = __str__
 
@@ -3411,15 +3399,14 @@
       self,
       start,
       stop,
       *,
       figure=None,
       ax=None,
       label=None,
-      runstate=None,
       **plot_kw,
   ) -> Axes:
     ''' Convenience shim for `DataFrame.plot` to plot data from
         `start` to `stop`.
         Return the plot `Axes`.
 
         Parameters:
@@ -3428,21 +3415,15 @@
         * `label`: optional label for the graph
         Other keyword parameters are passed to `Axes.plot`
         or `DataFrame.plot` for new axes.
     '''
     if label is None:
       label = self.tags.get('csv.header')
     return super().plot(
-        start,
-        stop,
-        figure=figure,
-        ax=ax,
-        label=label,
-        runstate=runstate,
-        **plot_kw
+        start, stop, figure=figure, ax=ax, label=label, **plot_kw
     )
 
 @promote
 @typechecked
 def timeseries_from_path(
     tspath: str, epoch: Optional[Epoch] = None, typecode=None
 ):
```

### Comparing `cs.timeseries-20230217/lib/python/cs.timeseries.egg-info/PKG-INFO` & `cs.timeseries-20230612/lib/python/cs.timeseries.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.timeseries
-Version: 20230217
+Version: 20230612
 Summary: Efficient portable machine native columnar file storage of time series data for double float and signed 64-bit integers.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
@@ -16,17 +16,19 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 Provides-Extra: pandas
 
 Efficient portable machine native columnar file storage of time
 series data for double float and signed 64-bit integers.
 
-*Latest release 20230217*:
-* TimeSeriesFile.save_to: use atomic_filename() to create the updated file.
-* Other small fixes and updates.
+*Latest release 20230612*:
+* Epoch.promote: do not special case None, let Optional[Epoch] type annoations handle that.
+* Mark PlotSeries.promote as incomplete (raises RuntimeError).
+* TimespanPolicy.promote: use cls.from_name() instead of TimespanPolicy.from_name().
+* Assorted other small updates.
 
 The core purpose is to provide time series data storage; there
 are assorted convenience methods to export arbitrary subsets
 of the data for use by other libraries in common forms, such
 as dataframes or series, numpy arrays and simple lists.
 There are also some simple plot methods for plotting graphs.
 
@@ -115,15 +117,15 @@
 * `utcoffset`: optional UTC offset for presentation
 Other keyword parameters are passed to `Axes.scatter`.
 
 ## Class `PlotSeries(PlotSeries, builtins.tuple, cs.deco.Promotable)`
 
 Information about a series to be plotted:
 - `label`: the label for this series
-- `series`: an series
+- `series`: a `Series`
 - `extra`: a `dict` of extra information such as plot styling
 
 ## Class `TimePartition(TimePartition, builtins.tuple, TimeStepsMixin)`
 
 A `namedtuple` for a slice of time with the following attributes:
 * `epoch`: the reference `Epoch`
 * `name`: the name for this slice
@@ -228,14 +230,16 @@
                             dateutil.parser.parse.
             stop-time       Optional stop time, default now.
                             An integer number of days before the current time
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             glob|fields     If glob is supplied, constrain the keys of
                             a TimeSeriesDataDir by the glob.
+        shell
+          Run a command prompt via cmd.Cmd using this command's subcommands.
 
 ## Class `TimeSeriesCommand(TimeSeriesBaseCommand, cs.cmdutils.BaseCommand)`
 
 Command line interface to `TimeSeries` data files.
 
 Command line usage:
 
@@ -292,14 +296,16 @@
                             dateutil.parser.parse.
             stop-time       Optional stop time, default now.
                             An integer number of days before the current time
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             glob|fields     If glob is supplied, constrain the keys of
                             a TimeSeriesDataDir by the glob.
+        shell
+          Run a command prompt via cmd.Cmd using this command's subcommands.
         test [testnames...]
           Run some tests of functionality.
 
 ## Class `TimeSeriesDataDir(TimeSeriesMapping, builtins.dict, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin, cs.fs.HasFSPath, cs.configutils.HasConfigIni, HasEpochMixin, TimeStepsMixin)`
 
 A directory containing a collection of `TimeSeriesPartitioned` subdirectories.
 
@@ -354,15 +360,15 @@
 
 Presently the mode used is triggered by the access method.
 Using the `peek` and `poke` methods uses `mmap` by default.
 Other accesses default to use the in-memory mode.
 Access to the `.array` property forces use of the `array` mode.
 Poll/update operations should usually choose to use `peek`/`poke`.
 
-*Method `TimeSeriesFile.__init__(self, fspath: str, typecode: Optional[cs.timeseries.TypeCode] = None, *, epoch: Optional[cs.timeseries.Epoch] = None, fill=None, fstags=None)`*:
+*Method `TimeSeriesFile.__init__(self, fspath: str, typecode: Optional[cs.timeseries.TypeCode] = None, *, epoch: Optional[cs.timeseries.Epoch] = None, fill=None, fstags: cs.fstags.FSTags)`*:
 Prepare a new time series stored in the file at `fspath`
 containing machine native data for the time series values.
 
 Parameters:
 * `fspath`: the filename of the data file
 * `typecode` optional expected `array.typecode` value of the data;
   if specified and the data file exists, they must match;
@@ -411,15 +417,15 @@
 A collection of `TimeSeries` files in a subdirectory.
 We have one of these for each `TimeSeriesDataDir` key.
 
 This class manages a collection of files
 named by the partition from a `TimespanPolicy`,
 which dictates which partition holds the datum for a UNIX time.
 
-*Method `TimeSeriesPartitioned.__init__(self, dirpath: str, typecode: Optional[cs.timeseries.TypeCode] = None, *, epoch: Optional[cs.timeseries.Epoch] = None, policy, fstags: Optional[cs.fstags.FSTags] = None)`*:
+*Method `TimeSeriesPartitioned.__init__(self, dirpath: str, typecode: Optional[cs.timeseries.TypeCode] = None, *, epoch: Optional[cs.timeseries.Epoch] = None, policy, fstags: cs.fstags.FSTags)`*:
 Initialise the `TimeSeriesPartitioned` instance.
 
 Parameters:
 * `dirpath`: the directory filesystem path,
   known as `.fspath` within the instance
 * `typecode`: the `array` type code for the data
 * `epoch`: the time series `Epoch`
@@ -510,14 +516,20 @@
 `dateutil.tz.gettz()`, the local system timezone.
 Otherwise it returns `dateutil.tz.gettz(tzspec)`.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* Epoch.promote: do not special case None, let Optional[Epoch] type annoations handle that.
+* Mark PlotSeries.promote as incomplete (raises RuntimeError).
+* TimespanPolicy.promote: use cls.from_name() instead of TimespanPolicy.from_name().
+* Assorted other small updates.
+
 *Release 20230217*:
 * TimeSeriesFile.save_to: use atomic_filename() to create the updated file.
 * Other small fixes and updates.
 
 *Release 20220918*:
 * TimeSeriesMapping.as_pd_dataframe: rename `keys` to `df_data`, and accept either a time series key or a `(key,series)` tuple.
 * TimeSeriesMapping.as_pd_dataframe: default `key_map`: annotate columns with their original CSV headers if present.
```

### Comparing `cs.timeseries-20230217/pyproject.toml` & `cs.timeseries-20230612/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,64 +5,66 @@
     { name = "Cameron Simpson", email = "cs@cskk.id.au" },
 ]
 keywords = [
     "python3",
 ]
 dependencies = [
     "arrow",
-    "cs.binary>=20230212",
-    "cs.buffer>=20230212.2",
-    "cs.cmdutils>=20230212",
+    "cs.binary>=20230401",
+    "cs.buffer>=20230401",
+    "cs.cmdutils>=20230612",
     "cs.configutils>=20220430",
-    "cs.context>=20230212",
+    "cs.context>=20230331",
     "cs.csvutils>=20220606",
     "cs.deco>=20221106.1",
     "cs.fileutils>=20210731",
-    "cs.fs>=20221221",
-    "cs.fstags>=20230217",
-    "cs.lex>=20230217.1",
+    "cs.fs>=20230401",
+    "cs.fstags>=20230407",
+    "cs.lex>=20230401",
     "cs.logutils>=20230212",
-    "cs.mappings>=20220912.4",
-    "cs.mplutils>=20220918",
-    "cs.pfx>=20221118",
-    "cs.progress>=20230212",
+    "cs.mappings>=20230612",
+    "cs.mplutils>=20230407",
+    "cs.pfx>=20230604",
+    "cs.progress>=20230401",
     "cs.py.modules>=20220606",
-    "cs.resources>=20230217",
-    "cs.result>=20230212",
-    "cs.upd>=20230217",
+    "cs.resources>=20230503",
+    "cs.result>=20230331",
+    "cs.upd>=20230401",
     "icontract",
     "matplotlib",
     "numpy",
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
 Efficient portable machine native columnar file storage of time
 series data for double float and signed 64-bit integers.
 
-*Latest release 20230217*:
-* TimeSeriesFile.save_to: use atomic_filename() to create the updated file.
-* Other small fixes and updates.
+*Latest release 20230612*:
+* Epoch.promote: do not special case None, let Optional[Epoch] type annoations handle that.
+* Mark PlotSeries.promote as incomplete (raises RuntimeError).
+* TimespanPolicy.promote: use cls.from_name() instead of TimespanPolicy.from_name().
+* Assorted other small updates.
 
 The core purpose is to provide time series data storage; there
 are assorted convenience methods to export arbitrary subsets
 of the data for use by other libraries in common forms, such
 as dataframes or series, numpy arrays and simple lists.
 There are also some simple plot methods for plotting graphs.
 
@@ -151,15 +153,15 @@
 * `utcoffset`: optional UTC offset for presentation
 Other keyword parameters are passed to `Axes.scatter`.
 
 ## Class `PlotSeries(PlotSeries, builtins.tuple, cs.deco.Promotable)`
 
 Information about a series to be plotted:
 - `label`: the label for this series
-- `series`: an series
+- `series`: a `Series`
 - `extra`: a `dict` of extra information such as plot styling
 
 ## Class `TimePartition(TimePartition, builtins.tuple, TimeStepsMixin)`
 
 A `namedtuple` for a slice of time with the following attributes:
 * `epoch`: the reference `Epoch`
 * `name`: the name for this slice
@@ -264,14 +266,16 @@
                             dateutil.parser.parse.
             stop-time       Optional stop time, default now.
                             An integer number of days before the current time
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             glob|fields     If glob is supplied, constrain the keys of
                             a TimeSeriesDataDir by the glob.
+        shell
+          Run a command prompt via cmd.Cmd using this command's subcommands.
 
 ## Class `TimeSeriesCommand(TimeSeriesBaseCommand, cs.cmdutils.BaseCommand)`
 
 Command line interface to `TimeSeries` data files.
 
 Command line usage:
 
@@ -328,14 +332,16 @@
                             dateutil.parser.parse.
             stop-time       Optional stop time, default now.
                             An integer number of days before the current time
                             or any datetime specification recognised by
                             dateutil.parser.parse.
             glob|fields     If glob is supplied, constrain the keys of
                             a TimeSeriesDataDir by the glob.
+        shell
+          Run a command prompt via cmd.Cmd using this command's subcommands.
         test [testnames...]
           Run some tests of functionality.
 
 ## Class `TimeSeriesDataDir(TimeSeriesMapping, builtins.dict, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin, cs.fs.HasFSPath, cs.configutils.HasConfigIni, HasEpochMixin, TimeStepsMixin)`
 
 A directory containing a collection of `TimeSeriesPartitioned` subdirectories.
 
@@ -390,15 +396,15 @@
 
 Presently the mode used is triggered by the access method.
 Using the `peek` and `poke` methods uses `mmap` by default.
 Other accesses default to use the in-memory mode.
 Access to the `.array` property forces use of the `array` mode.
 Poll/update operations should usually choose to use `peek`/`poke`.
 
-*Method `TimeSeriesFile.__init__(self, fspath: str, typecode: Optional[cs.timeseries.TypeCode] = None, *, epoch: Optional[cs.timeseries.Epoch] = None, fill=None, fstags=None)`*:
+*Method `TimeSeriesFile.__init__(self, fspath: str, typecode: Optional[cs.timeseries.TypeCode] = None, *, epoch: Optional[cs.timeseries.Epoch] = None, fill=None, fstags: cs.fstags.FSTags)`*:
 Prepare a new time series stored in the file at `fspath`
 containing machine native data for the time series values.
 
 Parameters:
 * `fspath`: the filename of the data file
 * `typecode` optional expected `array.typecode` value of the data;
   if specified and the data file exists, they must match;
@@ -447,15 +453,15 @@
 A collection of `TimeSeries` files in a subdirectory.
 We have one of these for each `TimeSeriesDataDir` key.
 
 This class manages a collection of files
 named by the partition from a `TimespanPolicy`,
 which dictates which partition holds the datum for a UNIX time.
 
-*Method `TimeSeriesPartitioned.__init__(self, dirpath: str, typecode: Optional[cs.timeseries.TypeCode] = None, *, epoch: Optional[cs.timeseries.Epoch] = None, policy, fstags: Optional[cs.fstags.FSTags] = None)`*:
+*Method `TimeSeriesPartitioned.__init__(self, dirpath: str, typecode: Optional[cs.timeseries.TypeCode] = None, *, epoch: Optional[cs.timeseries.Epoch] = None, policy, fstags: cs.fstags.FSTags)`*:
 Initialise the `TimeSeriesPartitioned` instance.
 
 Parameters:
 * `dirpath`: the directory filesystem path,
   known as `.fspath` within the instance
 * `typecode`: the `array` type code for the data
 * `epoch`: the time series `Epoch`
@@ -546,14 +552,20 @@
 `dateutil.tz.gettz()`, the local system timezone.
 Otherwise it returns `dateutil.tz.gettz(tzspec)`.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* Epoch.promote: do not special case None, let Optional[Epoch] type annoations handle that.
+* Mark PlotSeries.promote as incomplete (raises RuntimeError).
+* TimespanPolicy.promote: use cls.from_name() instead of TimespanPolicy.from_name().
+* Assorted other small updates.
+
 *Release 20230217*:
 * TimeSeriesFile.save_to: use atomic_filename() to create the updated file.
 * Other small fixes and updates.
 
 *Release 20220918*:
 * TimeSeriesMapping.as_pd_dataframe: rename `keys` to `df_data`, and accept either a time series key or a `(key,series)` tuple.
 * TimeSeriesMapping.as_pd_dataframe: default `key_map`: annotate columns with their original CSV headers if present.
```

### Comparing `cs.timeseries-20230217/setup.cfg` & `cs.timeseries-20230612/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.timeseries
-version = 20230217
+version = 20230612
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = Efficient portable machine native columnar file storage of time series data for double float and signed 64-bit integers.
 keywords = python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers = 
@@ -18,34 +18,34 @@
 long_description_content_type = text/markdown
 
 [options]
 package_dir = 
 	= lib/python
 install_requires = 
 	arrow
-	cs.binary>=20230212
-	cs.buffer>=20230212.2
-	cs.cmdutils>=20230212
+	cs.binary>=20230401
+	cs.buffer>=20230401
+	cs.cmdutils>=20230612
 	cs.configutils>=20220430
-	cs.context>=20230212
+	cs.context>=20230331
 	cs.csvutils>=20220606
 	cs.deco>=20221106.1
 	cs.fileutils>=20210731
-	cs.fs>=20221221
-	cs.fstags>=20230217
-	cs.lex>=20230217.1
+	cs.fs>=20230401
+	cs.fstags>=20230407
+	cs.lex>=20230401
 	cs.logutils>=20230212
-	cs.mappings>=20220912.4
-	cs.mplutils>=20220918
-	cs.pfx>=20221118
-	cs.progress>=20230212
+	cs.mappings>=20230612
+	cs.mplutils>=20230407
+	cs.pfx>=20230604
+	cs.progress>=20230401
 	cs.py.modules>=20220606
-	cs.resources>=20230217
-	cs.result>=20230212
-	cs.upd>=20230217
+	cs.resources>=20230503
+	cs.result>=20230331
+	cs.upd>=20230401
 	icontract
 	matplotlib
 	numpy
 	python-dateutil
 	typeguard
 
 [options.entry_points]
```

