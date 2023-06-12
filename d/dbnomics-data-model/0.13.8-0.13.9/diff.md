# Comparing `tmp/dbnomics-data-model-0.13.8.tar.gz` & `tmp/dbnomics-data-model-0.13.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dbnomics-data-model-0.13.8.tar", last modified: Tue Feb  4 16:52:17 2020, max compression
+gzip compressed data, was "dist/dbnomics-data-model-0.13.9.tar", last modified: Wed Feb 12 18:10:37 2020, max compression
```

## Comparing `dbnomics-data-model-0.13.8.tar` & `dbnomics-data-model-0.13.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-04 16:52:17.000000 dbnomics-data-model-0.13.8/
--rw-rw-rw-   0 root         (0) root         (0)       48 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    15306 2020-02-04 16:52:17.000000 dbnomics-data-model-0.13.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12174 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-04 16:52:17.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2788 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)     1964 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    33835 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/observations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-04 16:52:17.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/schemas/
--rw-rw-rw-   0 root         (0) root         (0)     2424 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/schemas/category_tree.json
--rw-rw-rw-   0 root         (0) root         (0)     3523 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/schemas/dataset.json
--rw-rw-rw-   0 root         (0) root         (0)     1145 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/schemas/definitions.json
--rw-rw-rw-   0 root         (0) root         (0)     1012 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/schemas/provider.json
--rw-rw-rw-   0 root         (0) root         (0)     4321 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/schemas/series.json
--rw-rw-rw-   0 root         (0) root         (0)     4082 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/series.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-04 16:52:17.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/storages/
--rw-rw-rw-   0 root         (0) root         (0)     3801 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/storages/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9151 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/storages/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     1190 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/storages/files.py
--rw-rw-rw-   0 root         (0) root         (0)     8326 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/storages/filesystem.py
--rw-rw-rw-   0 root         (0) root         (0)     9203 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/storages/git.py
--rwxrwxrwx   0 root         (0) root         (0)    31187 2020-02-04 16:52:02.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/validate_storage.py
--rw-rw-rw-   0 root         (0) root         (0)     2437 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/dbnomics_data_model/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-04 16:52:17.000000 dbnomics-data-model-0.13.8/dbnomics_data_model.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15306 2020-02-04 16:52:17.000000 dbnomics-data-model-0.13.8/dbnomics_data_model.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2020-02-04 16:52:17.000000 dbnomics-data-model-0.13.8/dbnomics_data_model.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-02-04 16:52:17.000000 dbnomics-data-model-0.13.8/dbnomics_data_model.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       81 2020-02-04 16:52:17.000000 dbnomics-data-model-0.13.8/dbnomics_data_model.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       92 2020-02-04 16:52:17.000000 dbnomics-data-model-0.13.8/dbnomics_data_model.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2020-02-04 16:52:17.000000 dbnomics-data-model-0.13.8/dbnomics_data_model.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      202 2020-02-04 16:52:17.000000 dbnomics-data-model-0.13.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2574 2020-02-04 16:52:02.000000 dbnomics-data-model-0.13.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-04 16:52:17.000000 dbnomics-data-model-0.13.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4104 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/tests/test_filesystem.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2020-02-04 12:11:52.000000 dbnomics-data-model-0.13.8/tests/test_misc_errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-12 18:10:37.000000 dbnomics-data-model-0.13.9/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    15306 2020-02-12 18:10:37.000000 dbnomics-data-model-0.13.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    12174 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-12 18:10:37.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2788 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)     1964 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    36462 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/observations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-12 18:10:37.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)     2424 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/schemas/category_tree.json
+-rw-rw-rw-   0 root         (0) root         (0)     3523 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/schemas/dataset.json
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/schemas/definitions.json
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/schemas/provider.json
+-rw-rw-rw-   0 root         (0) root         (0)     4321 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/schemas/series.json
+-rw-rw-rw-   0 root         (0) root         (0)     4082 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/series.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-12 18:10:37.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/storages/
+-rw-rw-rw-   0 root         (0) root         (0)     3801 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/storages/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9151 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/storages/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1190 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/storages/files.py
+-rw-rw-rw-   0 root         (0) root         (0)     8326 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/storages/filesystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     9203 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/storages/git.py
+-rwxrwxrwx   0 root         (0) root         (0)    31187 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/validate_storage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2437 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/dbnomics_data_model/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-12 18:10:37.000000 dbnomics-data-model-0.13.9/dbnomics_data_model.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15306 2020-02-12 18:10:37.000000 dbnomics-data-model-0.13.9/dbnomics_data_model.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2020-02-12 18:10:37.000000 dbnomics-data-model-0.13.9/dbnomics_data_model.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-02-12 18:10:37.000000 dbnomics-data-model-0.13.9/dbnomics_data_model.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2020-02-12 18:10:37.000000 dbnomics-data-model-0.13.9/dbnomics_data_model.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2020-02-12 18:10:37.000000 dbnomics-data-model-0.13.9/dbnomics_data_model.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2020-02-12 18:10:37.000000 dbnomics-data-model-0.13.9/dbnomics_data_model.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      202 2020-02-12 18:10:37.000000 dbnomics-data-model-0.13.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2574 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-12 18:10:37.000000 dbnomics-data-model-0.13.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4104 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/tests/test_filesystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2020-02-12 18:10:16.000000 dbnomics-data-model-0.13.9/tests/test_misc_errors.py
```

### Comparing `dbnomics-data-model-0.13.8/PKG-INFO` & `dbnomics-data-model-0.13.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnomics-data-model
-Version: 0.13.8
+Version: 0.13.9
 Summary: DBnomics data model
 Home-page: https://git.nomics.world/dbnomics/dbnomics-data-model
 Author: DBnomics Team
 Author-email: contact@nomics.world
 License: https://www.gnu.org/licenses/agpl-3.0.en.html
 Description: # DBnomics data model
```

### Comparing `dbnomics-data-model-0.13.8/README.md` & `dbnomics-data-model-0.13.9/README.md`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model/datasets.py` & `dbnomics-data-model-0.13.9/dbnomics_data_model/datasets.py`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model/exceptions.py` & `dbnomics-data-model-0.13.9/dbnomics_data_model/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model/observations.py` & `dbnomics-data-model-0.13.9/dbnomics_data_model/observations.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,14 +55,15 @@
             Frequency.WEEKLY: "W",
             Frequency.DAILY: "D",
         }[self]
 
 
 day_range_re = "0[1-9]|[1-2][0-9]|3[0-1]"  # 01-31
 month_range_re = "0[1-9]|1[0-2]"  # 01-12
+# Cf https://docs.python.org/3/library/datetime.html#datetime.date.isocalendar
 week_range_re = "0[1-9]|[1-4][0-9]|5[0-3]"  # 01-53
 
 
 period_format_strict_regex_list = [
     (Frequency.ANNUAL, re.compile(r"^(\d{4})$")),
     (Frequency.BI_ANNUAL, re.compile(r"^(\d{4})-S([1-2])$")),
     (Frequency.BI_MONTHLY, re.compile(r"^(\d{4})-B([1-6])$")),
@@ -192,16 +193,17 @@
         for periods_dates, values in periods_dates_and_values_list
     ]
 
 
 def detect_frequency(period1, period2):
     """Return a tuple like `(frequency, normalize_period)` for the given `period`.
 
-    `normalize_period` can be `None` if periods are already normalized,
-    or a function taking a period as `str` and returning a normalized period as `str`.
+    If periods are already normalized or if `period1` and `period2` are not start days
+    of the inferred frequency, `normalize_period` will be `None`.
+    Otherwise it will be a function taking a period `str` and returning a normalized period `str`.
 
     When the format of the periods is "daily", the frequency can be different,
     depending on the interval between the days (e.g. the frequency can be "quarterly" if the interval is 3 months).
     That's the purpose of this function, compared to `detect_period_format` which takes one period only.
 
     See also: `detect_period_format`, `detect_period_format_strict`
 
@@ -244,33 +246,49 @@
     (<Frequency.QUARTERLY: 'quarterly'>, ...)
     >>> detect_frequency('1919-03-31', '1919-06-30')  # doctest: +ELLIPSIS
     (<Frequency.QUARTERLY: 'quarterly'>, ...)
     >>> detect_frequency('2014-01-01', '2014-03-01')  # doctest: +ELLIPSIS
     (<Frequency.BI_MONTHLY: 'bi-monthly'>, ...)
     >>> detect_frequency('2014-01-01', '2014-02-01')  # doctest: +ELLIPSIS
     (<Frequency.MONTHLY: 'monthly'>, ...)
-    >>> detect_frequency('2014-01-01', '2014-01-08')  # doctest: +ELLIPSIS
+    >>> detect_frequency('2014-01-15', '2014-02-15')  # doctest: +ELLIPSIS
+    (<Frequency.MONTHLY: 'monthly'>, None)
+    >>> detect_frequency('2014-01-01', '2014-01-31')  # doctest: +ELLIPSIS
+    (<Frequency.DAILY: 'daily'>, None)
+    >>> detect_frequency('2014-01-06', '2014-01-13')  # doctest: +ELLIPSIS
     (<Frequency.WEEKLY: 'weekly'>, ...)
+    >>> detect_frequency('2014-01-07', '2014-01-14')  # doctest: +ELLIPSIS
+    (<Frequency.WEEKLY: 'weekly'>, None)
+    >>> detect_frequency('2014-01-06', '2014-01-14')  # doctest: +ELLIPSIS
+    (<Frequency.DAILY: 'daily'>, None)
+    >>> detect_frequency('2014-01-03', '2014-01-11')  # doctest: +ELLIPSIS
+    (<Frequency.DAILY: 'daily'>, None)
 
     # Invalid or different period formats:
     >>> detect_frequency('2014', '2015-02')
     (None, None)
     >>> detect_frequency('2014', '2014Z2')
     (None, None)
     >>> detect_frequency('2014Z2', '2014')
     (None, None)
     >>> detect_frequency('2014Z2', '2014Z2')
     (None, None)
     """
 
-    def make_normalize_period(frequency):
+    def make_normalize_period(frequency: Frequency, date_1: date, date_2: date):
         def normalize_period(period):
             period_date = datetime.fromisoformat(period)
             return start_day_to_period(period_date, frequency)
-        return normalize_period
+
+        return (
+            normalize_period
+            if is_start_day(date_1, frequency) and is_start_day(date_2, frequency)
+            else None
+        )
+
 
     period1_format, normalize_period = detect_period_format(period1)
     period2_format, _ = detect_period_format(period2)
 
     if period1_format != period2_format:
         log.error("The 2 periods do not have the same format {!r}".format(
             ((period1, period1_format), (period2, period2_format))))
@@ -279,26 +297,26 @@
     elif period1_format == Frequency.DAILY:
         # Measure the interval between the two periods.
         date_1 = datetime.fromisoformat(period1)
         date_2 = datetime.fromisoformat(period2)
         date_diff = relativedelta(date_2, date_1)
         if date_diff.days == 1:
             return (Frequency.DAILY, None)
-        elif date_diff.weeks == 1:
-            return (Frequency.WEEKLY, make_normalize_period(Frequency.WEEKLY))
+        elif date_diff.days == 7:
+            return (Frequency.WEEKLY, make_normalize_period(Frequency.WEEKLY, date_1, date_2))
         elif date_diff.months == 1:
-            return (Frequency.MONTHLY, make_normalize_period(Frequency.MONTHLY))
+            return (Frequency.MONTHLY, make_normalize_period(Frequency.MONTHLY, date_1, date_2))
         elif date_diff.months == 2:
-            return (Frequency.BI_MONTHLY, make_normalize_period(Frequency.BI_MONTHLY))
+            return (Frequency.BI_MONTHLY, make_normalize_period(Frequency.BI_MONTHLY, date_1, date_2))
         elif date_diff.months == 3:
-            return (Frequency.QUARTERLY, make_normalize_period(Frequency.QUARTERLY))
+            return (Frequency.QUARTERLY, make_normalize_period(Frequency.QUARTERLY, date_1, date_2))
         elif date_diff.months == 6:
-            return (Frequency.BI_ANNUAL, make_normalize_period(Frequency.BI_ANNUAL))
+            return (Frequency.BI_ANNUAL, make_normalize_period(Frequency.BI_ANNUAL, date_1, date_2))
         elif date_diff.years == 1:
-            return (Frequency.ANNUAL, make_normalize_period(Frequency.ANNUAL))
+            return (Frequency.ANNUAL, make_normalize_period(Frequency.ANNUAL, date_1, date_2))
         else:
             # No specific interval detected, keep daily.
             return (Frequency.DAILY, None)
 
     return (period1_format, normalize_period)
 
 
@@ -591,14 +609,18 @@
     (<Frequency.ANNUAL: 'annual'>, [['PERIOD', 'VALUE', 'FLAG'], ['2010', 1.0, ''], ['2011', 2.0, 'E']])
     >>> normalize_observations([['PERIOD', 'VALUE', 'FLAG'], ['2010', 1, None], ['2011', 2, 'E']])
     (<Frequency.ANNUAL: 'annual'>, [['PERIOD', 'VALUE', 'FLAG'], ['2010', 1.0, ''], ['2011', 2.0, 'E']])
 
     # Period format different than frequency:
     >>> normalize_observations([['PERIOD', 'VALUE'], ['2010-01-01', 1], ['2010-04-01', 2]])
     (<Frequency.QUARTERLY: 'quarterly'>, [['PERIOD', 'VALUE'], ['2010-Q1', 1.0], ['2010-Q2', 2.0]])
+    >>> normalize_observations([['PERIOD', 'VALUE'], ['2010-01-01', 1], ['2010-01-08', 2]])
+    (<Frequency.WEEKLY: 'weekly'>, [['PERIOD', 'VALUE'], ['2010-01-01', 1.0], ['2010-01-08', 2.0]])
+    >>> normalize_observations([['PERIOD', 'VALUE'], ['2010-01-04', 1], ['2010-01-11', 2]])
+    (<Frequency.WEEKLY: 'weekly'>, [['PERIOD', 'VALUE'], ['2010-W01', 1.0], ['2010-W02', 2.0]])
     """
     if not observations:
         return (None, [])
 
     header = observations[0]
     if len(observations) < 2:
         return (None, observations)
@@ -625,18 +647,38 @@
 
     rows = observations[1:]
     normalized_rows = list(map(normalize_row, rows))
 
     return (frequency, [header] + normalized_rows)
 
 
+def is_start_day(date: date, frequency: Frequency):
+    if frequency == Frequency.ANNUAL:
+        return date.day == 1 and date.month == 1
+    elif frequency == Frequency.BI_ANNUAL:
+        return date.day == 1 and date.month in {1, 7}
+    elif frequency == Frequency.QUARTERLY:
+        return date.day == 1 and date.month in {1, 4, 7, 10}
+    elif frequency == Frequency.BI_MONTHLY:
+        return date.day == 1 and date.month in {1, 3, 5, 7, 9, 11}
+    elif frequency == Frequency.MONTHLY:
+        return date.day == 1
+    elif frequency == Frequency.WEEKLY:
+        return date.isoweekday() == 1  # monday
+    elif frequency == Frequency.DAILY:
+        return True
+
+    raise ValueError("Unsupported frequency: {}".format(frequency))
+
+
 def period_to_start_day(period):
     """Return the start day of `period` as ISO-8601 date string.
 
     >>> period_to_start_day("")
+    >>> period_to_start_day("2000-W00")
     >>> period_to_start_day("2001")
     datetime.date(2001, 1, 1)
     >>> period_to_start_day("2001-S1")
     datetime.date(2001, 1, 1)
     >>> period_to_start_day("2001-S2")
     datetime.date(2001, 7, 1)
     >>> period_to_start_day("2001-B1")
@@ -692,88 +734,97 @@
                 assert index in range(1, 5)
                 month = index * 3 - 2
                 return date(int(year), month, 1)
             elif period_format == Frequency.MONTHLY:
                 year, month = match.groups()
                 return date(int(year), int(month), 1)
             elif period_format == Frequency.WEEKLY:
-                return datetime.strptime("{}-1".format(period), "%Y-W%W-%w").date()
+                return datetime.strptime("{}-1".format(period), "%G-W%V-%u").date()
             elif period_format == Frequency.DAILY:
                 year, month, day = match.groups()
                 return date(int(year), int(month), int(day))
             else:
                 assert False, period_format
 
     return None
 
 
 def start_day_to_period(period_date: date, frequency: Frequency):
-    """Return a period as `str` from `period_date` start day given `frequency`.
+    """Simplfy the `str` representation of `period_date` based on `frequency`.
+
+    If `period_date` is the start day of the period defined by `frequency`,
+    return a simpler representation of `period_date` as `str`,
+    otherwise return `period_date` as ISO format.
 
     >>> start_day_to_period(date(2000, 1, 1), Frequency.ANNUAL)
     '2000'
     >>> start_day_to_period(date(2000, 1, 1), Frequency.BI_ANNUAL)
     '2000-S1'
+    >>> start_day_to_period(date(2000, 7, 1), Frequency.BI_ANNUAL)
+    '2000-S2'
     >>> start_day_to_period(date(2000, 1, 1), Frequency.BI_MONTHLY)
     '2000-B1'
     >>> start_day_to_period(date(2000, 1, 1), Frequency.QUARTERLY)
     '2000-Q1'
     >>> start_day_to_period(date(2000, 4, 1), Frequency.QUARTERLY)
     '2000-Q2'
     >>> start_day_to_period(date(2000, 1, 1), Frequency.MONTHLY)
     '2000-01'
-    >>> start_day_to_period(date(2000, 1, 1), Frequency.WEEKLY)
-    '2000-W00'
+    >>> start_day_to_period(date(2000, 1, 3), Frequency.WEEKLY)
+    '2000-W01'
     >>> start_day_to_period(date(2000, 1, 1), Frequency.DAILY)
     '2000-01-01'
 
     # `period_date` is not the start day:
     >>> start_day_to_period(date(2000, 2, 3), Frequency.ANNUAL)
-    '2000'
+    '2000-02-03'
     >>> start_day_to_period(date(2000, 2, 3), Frequency.BI_ANNUAL)
-    '2000-S1'
+    '2000-02-03'
     >>> start_day_to_period(date(2000, 6, 8), Frequency.BI_ANNUAL)
-    '2000-S1'
+    '2000-06-08'
     >>> start_day_to_period(date(2000, 8, 21), Frequency.BI_ANNUAL)
-    '2000-S2'
+    '2000-08-21'
     >>> start_day_to_period(date(2000, 12, 31), Frequency.BI_ANNUAL)
-    '2000-S2'
+    '2000-12-31'
     >>> start_day_to_period(date(2000, 2, 3), Frequency.BI_MONTHLY)
-    '2000-B1'
+    '2000-02-03'
     >>> start_day_to_period(date(2000, 3, 7), Frequency.BI_MONTHLY)
-    '2000-B2'
+    '2000-03-07'
     >>> start_day_to_period(date(2000, 2, 3), Frequency.QUARTERLY)
-    '2000-Q1'
+    '2000-02-03'
     >>> start_day_to_period(date(2000, 4, 6), Frequency.QUARTERLY)
-    '2000-Q2'
+    '2000-04-06'
     >>> start_day_to_period(date(2000, 2, 3), Frequency.MONTHLY)
-    '2000-02'
+    '2000-02-03'
     >>> start_day_to_period(date(2000, 5, 8), Frequency.MONTHLY)
-    '2000-05'
+    '2000-05-08'
+    >>> start_day_to_period(date(2000, 1, 1), Frequency.WEEKLY)
+    '2000-01-01'
     >>> start_day_to_period(date(2000, 2, 3), Frequency.WEEKLY)
-    '2000-W05'
+    '2000-02-03'
     """
+    if not is_start_day(period_date, frequency):
+        return period_date.isoformat()
+
     if frequency == Frequency.ANNUAL:
         return period_date.strftime("%Y")
     elif frequency == Frequency.BI_ANNUAL:
         return "{}-S{}".format(period_date.year, math.ceil(period_date.month / 6))
     elif frequency == Frequency.QUARTERLY:
         return "{}-Q{}".format(period_date.year, math.ceil(period_date.month / 3))
     elif frequency == Frequency.BI_MONTHLY:
         return "{}-B{}".format(period_date.year, math.ceil(period_date.month / 2))
     elif frequency == Frequency.MONTHLY:
         return period_date.strftime("%Y-%m")
     elif frequency == Frequency.WEEKLY:
-        return period_date.strftime("%Y-W%W")
+        return period_date.strftime("%G-W%V")
     elif frequency == Frequency.DAILY:
         return period_date.isoformat()
-    else:
-        assert False, frequency
 
-    assert False, "Should never reach this line"
+    raise ValueError("Unsupported frequency: {}".format(frequency))
 
 
 def value_to_float(value):
     """Try to convert a value to a `float`. Otherwise return "NA" if empty, or else original value.
 
     >>> value_to_float(None)
     'NA'
```

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model/schemas/category_tree.json` & `dbnomics-data-model-0.13.9/dbnomics_data_model/schemas/category_tree.json`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model/schemas/dataset.json` & `dbnomics-data-model-0.13.9/dbnomics_data_model/schemas/dataset.json`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model/schemas/definitions.json` & `dbnomics-data-model-0.13.9/dbnomics_data_model/schemas/definitions.json`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model/schemas/provider.json` & `dbnomics-data-model-0.13.9/dbnomics_data_model/schemas/provider.json`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model/schemas/series.json` & `dbnomics-data-model-0.13.9/dbnomics_data_model/schemas/series.json`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model/series.py` & `dbnomics-data-model-0.13.9/dbnomics_data_model/series.py`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model/storages/__init__.py` & `dbnomics-data-model-0.13.9/dbnomics_data_model/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model/storages/abstract.py` & `dbnomics-data-model-0.13.9/dbnomics_data_model/storages/abstract.py`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model/storages/files.py` & `dbnomics-data-model-0.13.9/dbnomics_data_model/storages/files.py`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model/storages/filesystem.py` & `dbnomics-data-model-0.13.9/dbnomics_data_model/storages/filesystem.py`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model/storages/git.py` & `dbnomics-data-model-0.13.9/dbnomics_data_model/storages/git.py`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model/validate_storage.py` & `dbnomics-data-model-0.13.9/dbnomics_data_model/validate_storage.py`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model/validators.py` & `dbnomics-data-model-0.13.9/dbnomics_data_model/validators.py`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model.egg-info/PKG-INFO` & `dbnomics-data-model-0.13.9/dbnomics_data_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnomics-data-model
-Version: 0.13.8
+Version: 0.13.9
 Summary: DBnomics data model
 Home-page: https://git.nomics.world/dbnomics/dbnomics-data-model
 Author: DBnomics Team
 Author-email: contact@nomics.world
 License: https://www.gnu.org/licenses/agpl-3.0.en.html
 Description: # DBnomics data model
```

### Comparing `dbnomics-data-model-0.13.8/dbnomics_data_model.egg-info/SOURCES.txt` & `dbnomics-data-model-0.13.9/dbnomics_data_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/setup.py` & `dbnomics-data-model-0.13.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 readme_filepath = script_dir / 'README.md'
 with readme_filepath.open('rt', encoding='utf-8') as fd:
     README = fd.read()
 
 
 setup(
     name='dbnomics-data-model',
-    version='0.13.8',
+    version='0.13.9',
 
     author='DBnomics Team',
     author_email='contact@nomics.world',
     classifiers=[classifier for classifier in classifiers.split('\n') if classifier],
     description="DBnomics data model",
     long_description=README,
     long_description_content_type="text/markdown",
```

### Comparing `dbnomics-data-model-0.13.8/tests/test_filesystem.py` & `dbnomics-data-model-0.13.9/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `dbnomics-data-model-0.13.8/tests/test_misc_errors.py` & `dbnomics-data-model-0.13.9/tests/test_misc_errors.py`

 * *Files identical despite different names*

