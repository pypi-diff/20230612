# Comparing `tmp/stockstats-0.5.2.tar.gz` & `tmp/stockstats-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockstats-0.5.2.tar", last modified: Fri Feb 10 17:38:36 2023, max compression
+gzip compressed data, was "stockstats-0.5.3.tar", last modified: Mon Jun 12 15:56:09 2023, max compression
```

## Comparing `stockstats-0.5.2.tar` & `stockstats-0.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 17:38:36.978948 stockstats-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-02-10 17:38:25.000000 stockstats-0.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-10 17:38:25.000000 stockstats-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    24350 2023-02-10 17:38:36.978948 stockstats-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23419 2023-02-10 17:38:25.000000 stockstats-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-10 17:38:25.000000 stockstats-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-10 17:38:36.978948 stockstats-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-02-10 17:38:25.000000 stockstats-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 17:38:36.978948 stockstats-0.5.2/stockstats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24350 2023-02-10 17:38:36.000000 stockstats-0.5.2/stockstats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-02-10 17:38:36.000000 stockstats-0.5.2/stockstats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 17:38:36.000000 stockstats-0.5.2/stockstats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-10 17:38:36.000000 stockstats-0.5.2/stockstats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-10 17:38:36.000000 stockstats-0.5.2/stockstats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    46256 2023-02-10 17:38:25.000000 stockstats-0.5.2/stockstats.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-10 17:38:25.000000 stockstats-0.5.2/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:56:09.599066 stockstats-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-12 15:55:43.000000 stockstats-0.5.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 15:55:43.000000 stockstats-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25456 2023-06-12 15:56:09.599066 stockstats-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24525 2023-06-12 15:55:43.000000 stockstats-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 15:55:43.000000 stockstats-0.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-12 15:56:09.599066 stockstats-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-06-12 15:55:43.000000 stockstats-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:56:09.599066 stockstats-0.5.3/stockstats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25456 2023-06-12 15:56:09.000000 stockstats-0.5.3/stockstats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-12 15:56:09.000000 stockstats-0.5.3/stockstats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:56:09.000000 stockstats-0.5.3/stockstats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 15:56:09.000000 stockstats-0.5.3/stockstats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 15:56:09.000000 stockstats-0.5.3/stockstats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    48422 2023-06-12 15:55:43.000000 stockstats-0.5.3/stockstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 15:55:43.000000 stockstats-0.5.3/test-requirements.txt
```

### Comparing `stockstats-0.5.2/LICENSE.txt` & `stockstats-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stockstats-0.5.2/PKG-INFO` & `stockstats-0.5.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockstats
-Version: 0.5.2
+Version: 0.5.3
 Summary: DataFrame with inline stock statistics support.
 Home-page: https://github.com/jealous/stockstats
 Author: Cedric Zhuang
 Author-email: jealous@163.com
 License: BSD
 Keywords: stock statistics indicator
 Platform: any
@@ -25,15 +25,15 @@
 
 # Stock Statistics/Indicators Calculation Helper
 
 [![build & test](https://github.com/jealous/stockstats/actions/workflows/build-test.yml/badge.svg)](https://github.com/jealous/stockstats/actions/workflows/build-test.yml)
 [![codecov](https://codecov.io/gh/jealous/stockstats/branch/master/graph/badge.svg?token=IFMD1pVJ7T)](https://codecov.io/gh/jealous/stockstats)
 [![pypi](https://img.shields.io/pypi/v/stockstats.svg)](https://pypi.python.org/pypi/stockstats)
 
-VERSION: 0.5.2
+VERSION: 0.5.3
 
 ## Introduction
 
 Supply a wrapper ``StockDataFrame`` for ``pandas.DataFrame`` with inline stock
 statistics/indicators support.
 
 Supported statistics/indicators are:
@@ -75,14 +75,16 @@
 * VWMA: Volume Weighted Moving Average
 * CHOP: Choppiness Index
 * KAMA: Kaufman's Adaptive Moving Average
 * PPO: Percentage Price Oscillator
 * StochRSI: Stochastic RSI
 * WT: LazyBear's Wave Trend
 * Supertrend: with the Upper Band and Lower Band
+* Aroon: Aroon Oscillator
+* Z: Z-Score
 
 ## Installation
 
 ```pip install stockstats```
 
 ## Compatibility
 
@@ -674,14 +676,52 @@
 Use the pattern `<A>_x_<B>` to check when A crosses B.
 
 Examples:
 * `kdjk_x_kdjd` returns a series that marks the cross of KDJK and KDJD
 * `kdjk_xu_kdjd` returns a series that marks where KDJK crosses up KDJD
 * `kdjk_xd_kdjd` returns a series that marks where KDJD crosses down KDJD
 
+#### [Aroon Oscillator](https://www.investopedia.com/terms/a/aroonoscillator.asp)
+
+The Aroon Oscillator measures the strength of a trend and 
+the likelihood that it will continue.
+
+The default window is 25.
+
+* Aroon Oscillator = Aroon Up - Aroon Down
+* Aroon Up = 100 * (n - periods since n-period high) / n
+* Aroon Down = 100 * (n - periods since n-period low) / n
+* n = window size
+
+Examples:
+* `df['aroon']` returns Aroon oscillator with a window of 25
+* `df['aroon_14']` returns Aroon oscillator with a window of 14
+
+#### [Z-Score](https://www.investopedia.com/terms/z/zscore.asp)
+
+Z-score is a statistical measurement that describes a value's relationship to 
+the mean of a group of values. 
+
+There is no default column name or window for Z-Score.
+
+The statistical formula for a value's z-score is calculated using
+the following formula:
+
+```z = ( x - μ ) / σ```
+
+Where:
+
+* `z` = Z-score
+* `x` = the value being evaluated
+* `μ` = the mean
+* `σ` = the standard deviation
+
+Examples:
+* `df['close_75_z']` returns the Z-Score of close price with a window of 75
+
 ## Issues
 
 We use [Github Issues](https://github.com/jealous/stockstats/issues) to track
 the issues or bugs.
 
 ## Others
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stockstats-0.5.2/README.md` & `stockstats-0.5.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Stock Statistics/Indicators Calculation Helper
 
 [![build & test](https://github.com/jealous/stockstats/actions/workflows/build-test.yml/badge.svg)](https://github.com/jealous/stockstats/actions/workflows/build-test.yml)
 [![codecov](https://codecov.io/gh/jealous/stockstats/branch/master/graph/badge.svg?token=IFMD1pVJ7T)](https://codecov.io/gh/jealous/stockstats)
 [![pypi](https://img.shields.io/pypi/v/stockstats.svg)](https://pypi.python.org/pypi/stockstats)
 
-VERSION: 0.5.2
+VERSION: 0.5.3
 
 ## Introduction
 
 Supply a wrapper ``StockDataFrame`` for ``pandas.DataFrame`` with inline stock
 statistics/indicators support.
 
 Supported statistics/indicators are:
@@ -50,14 +50,16 @@
 * VWMA: Volume Weighted Moving Average
 * CHOP: Choppiness Index
 * KAMA: Kaufman's Adaptive Moving Average
 * PPO: Percentage Price Oscillator
 * StochRSI: Stochastic RSI
 * WT: LazyBear's Wave Trend
 * Supertrend: with the Upper Band and Lower Band
+* Aroon: Aroon Oscillator
+* Z: Z-Score
 
 ## Installation
 
 ```pip install stockstats```
 
 ## Compatibility
 
@@ -649,14 +651,52 @@
 Use the pattern `<A>_x_<B>` to check when A crosses B.
 
 Examples:
 * `kdjk_x_kdjd` returns a series that marks the cross of KDJK and KDJD
 * `kdjk_xu_kdjd` returns a series that marks where KDJK crosses up KDJD
 * `kdjk_xd_kdjd` returns a series that marks where KDJD crosses down KDJD
 
+#### [Aroon Oscillator](https://www.investopedia.com/terms/a/aroonoscillator.asp)
+
+The Aroon Oscillator measures the strength of a trend and 
+the likelihood that it will continue.
+
+The default window is 25.
+
+* Aroon Oscillator = Aroon Up - Aroon Down
+* Aroon Up = 100 * (n - periods since n-period high) / n
+* Aroon Down = 100 * (n - periods since n-period low) / n
+* n = window size
+
+Examples:
+* `df['aroon']` returns Aroon oscillator with a window of 25
+* `df['aroon_14']` returns Aroon oscillator with a window of 14
+
+#### [Z-Score](https://www.investopedia.com/terms/z/zscore.asp)
+
+Z-score is a statistical measurement that describes a value's relationship to 
+the mean of a group of values. 
+
+There is no default column name or window for Z-Score.
+
+The statistical formula for a value's z-score is calculated using
+the following formula:
+
+```z = ( x - μ ) / σ```
+
+Where:
+
+* `z` = Z-score
+* `x` = the value being evaluated
+* `μ` = the mean
+* `σ` = the standard deviation
+
+Examples:
+* `df['close_75_z']` returns the Z-Score of close price with a window of 75
+
 ## Issues
 
 We use [Github Issues](https://github.com/jealous/stockstats/issues) to track
 the issues or bugs.
 
 ## Others
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stockstats-0.5.2/setup.py` & `stockstats-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `stockstats-0.5.2/stockstats.egg-info/PKG-INFO` & `stockstats-0.5.3/stockstats.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockstats
-Version: 0.5.2
+Version: 0.5.3
 Summary: DataFrame with inline stock statistics support.
 Home-page: https://github.com/jealous/stockstats
 Author: Cedric Zhuang
 Author-email: jealous@163.com
 License: BSD
 Keywords: stock statistics indicator
 Platform: any
@@ -25,15 +25,15 @@
 
 # Stock Statistics/Indicators Calculation Helper
 
 [![build & test](https://github.com/jealous/stockstats/actions/workflows/build-test.yml/badge.svg)](https://github.com/jealous/stockstats/actions/workflows/build-test.yml)
 [![codecov](https://codecov.io/gh/jealous/stockstats/branch/master/graph/badge.svg?token=IFMD1pVJ7T)](https://codecov.io/gh/jealous/stockstats)
 [![pypi](https://img.shields.io/pypi/v/stockstats.svg)](https://pypi.python.org/pypi/stockstats)
 
-VERSION: 0.5.2
+VERSION: 0.5.3
 
 ## Introduction
 
 Supply a wrapper ``StockDataFrame`` for ``pandas.DataFrame`` with inline stock
 statistics/indicators support.
 
 Supported statistics/indicators are:
@@ -75,14 +75,16 @@
 * VWMA: Volume Weighted Moving Average
 * CHOP: Choppiness Index
 * KAMA: Kaufman's Adaptive Moving Average
 * PPO: Percentage Price Oscillator
 * StochRSI: Stochastic RSI
 * WT: LazyBear's Wave Trend
 * Supertrend: with the Upper Band and Lower Band
+* Aroon: Aroon Oscillator
+* Z: Z-Score
 
 ## Installation
 
 ```pip install stockstats```
 
 ## Compatibility
 
@@ -674,14 +676,52 @@
 Use the pattern `<A>_x_<B>` to check when A crosses B.
 
 Examples:
 * `kdjk_x_kdjd` returns a series that marks the cross of KDJK and KDJD
 * `kdjk_xu_kdjd` returns a series that marks where KDJK crosses up KDJD
 * `kdjk_xd_kdjd` returns a series that marks where KDJD crosses down KDJD
 
+#### [Aroon Oscillator](https://www.investopedia.com/terms/a/aroonoscillator.asp)
+
+The Aroon Oscillator measures the strength of a trend and 
+the likelihood that it will continue.
+
+The default window is 25.
+
+* Aroon Oscillator = Aroon Up - Aroon Down
+* Aroon Up = 100 * (n - periods since n-period high) / n
+* Aroon Down = 100 * (n - periods since n-period low) / n
+* n = window size
+
+Examples:
+* `df['aroon']` returns Aroon oscillator with a window of 25
+* `df['aroon_14']` returns Aroon oscillator with a window of 14
+
+#### [Z-Score](https://www.investopedia.com/terms/z/zscore.asp)
+
+Z-score is a statistical measurement that describes a value's relationship to 
+the mean of a group of values. 
+
+There is no default column name or window for Z-Score.
+
+The statistical formula for a value's z-score is calculated using
+the following formula:
+
+```z = ( x - μ ) / σ```
+
+Where:
+
+* `z` = Z-score
+* `x` = the value being evaluated
+* `μ` = the mean
+* `σ` = the standard deviation
+
+Examples:
+* `df['close_75_z']` returns the Z-Score of close price with a window of 75
+
 ## Issues
 
 We use [Github Issues](https://github.com/jealous/stockstats/issues) to track
 the issues or bugs.
 
 ## Others
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stockstats-0.5.2/stockstats.py` & `stockstats-0.5.3/stockstats.py`

 * *Files 2% similar despite different names*

```diff
@@ -599,14 +599,82 @@
                 else:
                     st[i] = ub[i]
 
         self['supertrend_ub'] = ub
         self['supertrend_lb'] = lb
         self['supertrend'] = st
 
+    def _get_aroon(self, window=None):
+        """ Aroon Oscillator
+
+        The Aroon Oscillator measures the strength of a trend and
+        the likelihood that it will continue.
+
+        The default window is 25.
+
+        * Aroon Oscillator = Aroon Up - Aroon Down
+        * Aroon Up = 100 * (n - periods since n-period high) / n
+        * Aroon Down = 100 * (n - periods since n-period low) / n
+        * n = window size
+        """
+        if window is None:
+            window = 25
+            column_name = 'aroon'
+        else:
+            window = self.get_int_positive(window)
+            column_name = 'aroon_{}'.format(window)
+
+        def _window_pct(s):
+            n = float(window)
+            return (n - (n - (s + 1))) / n * 100
+
+        high_since = self['high'].rolling(
+            min_periods=1,
+            window=window,
+            center=False).apply(np.argmax)
+        low_since = self['low'].rolling(
+            min_periods=1,
+            window=window,
+            center=False).apply(np.argmin)
+
+        aroon_up = _window_pct(high_since)
+        aroon_down = _window_pct(low_since)
+        self[column_name] = aroon_up - aroon_down
+
+    def _get_z(self, column, window):
+        """ Z score
+
+        Z-score is a statistical measurement that describes a value's
+        relationship to the mean of a group of values.
+
+        The statistical formula for a value's z-score is calculated using
+        the following formula:
+
+        z = ( x - μ ) / σ
+
+        Where:
+
+        * z = Z-score
+        * x = the value being evaluated
+        * μ = the mean
+        * σ = the standard deviation
+        """
+        window = self.get_int_positive(window)
+        column_name = '{}_{}_z'.format(column, window)
+        col = self[column]
+        mean = col.rolling(
+            min_periods=1,
+            window=window,
+            center=False).mean()
+        std = col.rolling(
+            min_periods=1,
+            window=window,
+            center=False).std()
+        self[column_name] = ((col - mean) / std).fillna(0.0)
+
     def _atr(self, window):
         tr = self._tr()
         return self._smma(tr, window)
 
     def _get_atr(self, window=None):
         """ Average True Range
 
@@ -1274,14 +1342,15 @@
             ('log-ret',): self._get_log_ret,
             ('mfi',): self._get_mfi,
             ('wt1', 'wt2'): self._get_wave_trend,
             ('wr',): self._get_wr,
             ('supertrend',
              'supertrend_lb',
              'supertrend_ub'): self._get_supertrend,
+            ('aroon',): self._get_aroon,
         }
 
     def __init_not_exist_column(self, key):
         for names, handler in self.handler.items():
             if key in names:
                 handler()
                 return
```

