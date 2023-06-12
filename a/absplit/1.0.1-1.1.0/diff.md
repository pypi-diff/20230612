# Comparing `tmp/absplit-1.0.1.tar.gz` & `tmp/absplit-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absplit-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absplit-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absplit-1.0.1.tar` & `absplit-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4958 2023-06-05 23:23:06.124000 absplit-1.0.1/.gitignore
--rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      291 2023-06-05 23:23:06.142000 absplit-1.0.1/.idea/genetic_algorithm.iml
--rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      303 2023-06-05 23:23:06.158000 absplit-1.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.0.1/LICENSE
--rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.0.1/MANIFEST.in
--rw-r--r--   0        0        0     7015 2023-06-06 00:11:28.620000 absplit-1.0.1/README.md
--rw-r--r--   0        0        0       62 2023-06-06 00:11:28.566000 absplit-1.0.1/absplit/__init__.py
--rw-r--r--   0        0        0     8775 2023-06-05 23:23:06.210000 absplit-1.0.1/absplit/data.py
--rw-r--r--   0        0        0    21344 2023-06-05 23:49:01.136000 absplit-1.0.1/absplit/ga.py
--rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.0.1/absplit/param.py
--rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.0.1/images/logo.jpeg
--rw-r--r--   0        0        0     1531 2023-06-06 00:11:28.664000 absplit-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       50 2023-06-05 23:23:06.260000 absplit-1.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-1.0.1/tests/test_data.py
--rw-r--r--   0        0        0     2099 2023-06-05 23:50:53.798000 absplit-1.0.1/tests/test_ga.py
--rw-r--r--   0        0        0     8064 1970-01-01 00:00:00.000000 absplit-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4958 2023-06-05 23:23:06.124000 absplit-1.1.0/.gitignore
+-rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.1.0/.idea/.gitignore
+-rw-r--r--   0        0        0      331 2023-06-12 08:10:41.536000 absplit-1.1.0/.idea/genetic_algorithm.iml
+-rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.1.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      305 2023-06-12 08:10:39.408000 absplit-1.1.0/.idea/misc.xml
+-rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.1.0/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.1.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.1.0/LICENSE
+-rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.1.0/MANIFEST.in
+-rw-r--r--   0        0        0     7015 2023-06-12 08:39:50.161000 absplit-1.1.0/README.md
+-rw-r--r--   0        0        0       62 2023-06-12 08:39:50.092000 absplit-1.1.0/absplit/__init__.py
+-rw-r--r--   0        0        0     8275 2023-06-11 11:49:29.241000 absplit-1.1.0/absplit/data.py
+-rw-r--r--   0        0        0    23169 2023-06-12 08:36:15.539000 absplit-1.1.0/absplit/ga.py
+-rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.1.0/absplit/param.py
+-rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.1.0/images/logo.jpeg
+-rw-r--r--   0        0        0     1531 2023-06-12 08:39:50.213000 absplit-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-05 23:23:06.260000 absplit-1.1.0/requirements.txt
+-rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-1.1.0/tests/test_data.py
+-rw-r--r--   0        0        0     2125 2023-06-12 08:32:24.989000 absplit-1.1.0/tests/test_ga.py
+-rw-r--r--   0        0        0     8064 1970-01-01 00:00:00.000000 absplit-1.1.0/PKG-INFO
```

### Comparing `absplit-1.0.1/.gitignore` & `absplit-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `absplit-1.0.1/LICENSE` & `absplit-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `absplit-1.0.1/README.md` & `absplit-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
 Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-1.0.1-blue.svg)
+![version](https://img.shields.io/badge/version-1.1.0-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                **** ABSplit ****
  Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 1.0.1-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.1.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Installation
    3. Tutorials
           o Do_it_yourself
    4. Usage
```

### Comparing `absplit-1.0.1/absplit/data.py` & `absplit-1.1.0/absplit/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,32 +95,14 @@
         for col in self.remainder_cols:
             dtype = self._df_stacked[col].dtype
             if not dtype == 'object':
                 print(f'Column \'{col}\' will be treated as a variable to split on. Normally additional splitting'
                       f'columns are of type object, this is type {dtype}, this could cause problems in splitting. '
                       'Please check your kwargs are correct and remove any metrics you dont intend on splitting on.')
 
-    # groups = np.array([(solution == i).astype(int) for i in range(3)])
-    # # print(groups.shape)
-    #
-    # w = np.array([1, 0.5, 1])
-    # costs = (groups @ all_metrics_global)
-    # # print(costs.shape)
-    # costs *= w.reshape(1, -1, 1)
-    # # print(costs.shape)
-    #
-    # # print(costs.shape)
-    # # return
-    # diffs = np.roll(costs, -1, axis=0) - costs
-    # mse = ((diffs ** 2).mean(axis=1)).sum()
-    #
-    # # Fitness
-    # fitness = 1.0 / np.abs(mse + 1e-10)  # Add small sum to prevent divide by zero
-    # return fitness
-
     def _extract_metadata(self):
         """Extracts metadata used for 3D transformation from unstacked dataframe, builds transformation tuple
 
         Returns:
             None
         """
 
@@ -154,15 +136,15 @@
         """Unstack date column if date columns is passed
 
         Returns:
             pd.DataFrame
         """
 
         self._df_unstacked = self._df_unstacked.unstack(self.date_col, fill_value=0) if self.date_col \
-            else self._df_stacked
+            else self._df_unstacked
 
     def _scale(self):
         """Standardise all metrics so all metrics weighted as equally as possible
 
         Returns:
             pd.DataFrame
         """
@@ -171,15 +153,15 @@
             scaler = self._pre_fit_scaler
         else:
             scaler = preprocessing.MinMaxScaler()
             scaler.fit(self._df_stacked[self.metrics])
 
         self._df_unstacked = self._df_stacked.copy()
         if self._scaler_flag:
-            self._df_unstacked [self.metrics] = scaler.transform(self._df_stacked[self.metrics])
+            self._df_unstacked[self.metrics] = scaler.transform(self._df_stacked[self.metrics])
 
     def filter(self, index):
         """Takes empty dataframe index 'index' and inner joins on unstacked data to return a filtered version.
 
         Used when splitting out sample and population dataframes from concatenated dataframe when using
         Match class
 
@@ -222,8 +204,9 @@
             pd.DataFrame
         """
 
         if solution is None:
             solution = np.array([None])
         df_assigned = self.index.copy()
         df_assigned.insert(loc=0, column='bin', value=solution.reshape(-1, 1))
+        df_assigned['bin'] = df_assigned['bin'].astype(str)
         return df_assigned
```

### Comparing `absplit-1.0.1/absplit/ga.py` & `absplit-1.1.0/absplit/ga.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from absplit.param import ParamMixin
 from absplit.data import Data
+from abc import ABC, abstractmethod
 import pandas as pd
 import pygad
 import logging
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 from sklearn import preprocessing
+from itertools import combinations
+
 
 logger = logging.getLogger(__name__)
 
 
 class GAInstance:
     """Manages initialisation and running of pygad genetic algorithm instance
 
@@ -122,15 +125,15 @@
                           f'discrete genetic algorith, and so you\'re not allowed to modify this')
                     continue
                 if not callable(value):
                     print(f'[Updating] {key} to {value}')
                 self.params[key] = value
 
 
-class SplitBase(ParamMixin):
+class SplitBase(ParamMixin, ABC):
     """Base class for genetic algorithm orchestration.
 
     Manages applying different weights to costs, using multiple runs, extracting and visualising results.
 
     Attributes:
         _runs (int): Number of runs of the genetic algorithm to try
         _ga_params (object): GAParams object
@@ -174,20 +177,22 @@
         self._splits_num = len(self._splits)
         self._ga_params = GAParams(splits=splits, **ga_params)
         self._best_score = -1
         self._metric_weights = metric_weights
         self._df = None
         self._population = None
         self._df_result = None  # Final results dataframe
-        self._ga = None  # genetic algorithm instance
+        self._df_dist = None  # Group count distribution
+        self._df_agg = None  # Group aggregated data
+        self._ga = None  # Genetic algorithm instance
         self._df_vis = None  # Visualisation dataframe
+        self._df_rmse = None  # RMSE between groups
         self._best_ga = None
         self._solution = None
 
-
         self._cost_weighting()
 
     def _cost_weighting(self):
         """Set relative cost weights for each metric. Defaults to 1 unless specified.
 
         Used if you want the genetic algorithm to penalise the MSE cost of some metrics
         over others. Particularly useful if one metric is quite volatile, as the MSE cost can
@@ -240,86 +245,141 @@
                 self._best_score = self._ga.fitness
 
         if self._solution is None:
             raise ValueError('Solution is None')
 
         # Assign solution to index
         self._df_result = self._population.assign(self._solution)
+        self._build_distributions()
+        self._build_df_vis()
+        self._build_aggregation()
+        self._build_rmse()
 
         logger.debug('Split complete')
 
+    @abstractmethod
+    def _build_df_vis(self):
+        pass
+
     def fitness(self, title=None):
         """Plots the fitness-generation graph
 
         Returns:
             None
         """
 
         if self._best_ga:
             self._best_ga.ga.plot_fitness(title=title)
         else:
             print('No solution available, please use .run() first')
 
+    def _build_distributions(self):
+        """Build dataframe that contains data on the count distributions of each group
+
+        Sets:
+            _df_dist
+        """
+        self._df_dist = self._df_result['bin'].value_counts().to_frame('count')
+        self._df_dist.index.name = 'bin'
+        self._df_dist['pct'] = (self._df_dist['count'] / self._df_dist['count'].sum()).round(4)
+        return self._df_dist.sort_index()
+
+    def _build_rmse(self):
+        df_agg = self._df_agg.copy()
+
+        if self.date_col is None:
+            df_agg.index = [0]*df_agg.shape[0]
+
+        df_ = df_agg.pivot(index=self.date_col, columns='bin', values=self.metrics)
+        df_.columns = df_.columns.map('_'.join).str.lower()
+
+        groups = self._df_agg['bin'].unique()
+        combinations_lst = list(combinations(groups, 2))
+
+        df_lst = []
+
+        for metric in self.metrics:
+            df_metric = pd.DataFrame()
+            for a, b in combinations_lst:
+                # print(metric, a, b)
+                col_a = f'{metric}_{a}'
+                col_b = f'{metric}_{b}'
+                rmse = np.sqrt(((df_[col_a] - df_[col_b]) ** 2).mean())
+                # print(mse)
+                df_metric.loc[a, b] = rmse
+                df_metric.loc[b, a] = rmse
+            df_metric = df_metric.reindex(sorted(df_metric.columns), axis=1)
+            columns = pd.MultiIndex.from_tuples([(metric, col) for col in df_metric.columns])
+            df_metric.columns = columns
+            df_lst.append(df_metric)
+
+        self._df_rmse = pd.concat(df_lst, axis=1)
+        self._df_rmse.columns.name = 'bin'
+        self._df_rmse.index.name = 'bin'
+
     @property
     def results(self):
         """Returns compiled dataframe of solutions
 
         Returns:
             pd.DataFrame
         """
-
         return self._df_result
 
-    def visualise(self, column=None):
-        """Visualise metrics for both bins and there comparative performances
+    @property
+    def distributions(self):
+        """Returns distributions dataframe
 
-        Returns:
-            None
+        Returns
+            pd.DataFrame
         """
+        return self._df_dist
 
-        # Default to all metric columns if no columns specified
-        if column:
-            if isinstance(column, str):
-                column = [column]
-            vis_metrics = column
-        else:
-            vis_metrics = self.metrics
+    @property
+    def rmse(self):
+        return self._df_rmse
 
-        if self.results is None:
-            print('Must use .run() before visualising')
-            return
+    @property
+    def aggregations(self):
+        return self._df_agg
+
+    def _build_aggregation(self):
+        """Aggregates data by bins
+
+        Sets:
+            _df_agg
+        """
 
         # Aggregate by bin
         group_cols = ['bin']
         group_cols += [self.date_col] if self.date_col else []
-        df = self._df_vis.groupby(group_cols)[vis_metrics].sum().reset_index()
+        self._df_agg = self._df_vis.groupby(group_cols)[self.metrics].sum().reset_index()
 
-        if not len(df):
-            logger.warning(f'Failed vis')
-            return
+    def visualise(self):
+        """Visualise metrics for both bins and there comparative performances
 
-        sns.set_style('darkgrid')
+        Returns:
+            None
+        """
 
-        # Chart sizing
-        figsize = (min(20, len(vis_metrics)*8), 5) if self.date_col else (8, 5)
-        fig, ax = plt.subplots(1, len(vis_metrics), figsize=figsize)
+        sns.set_style('darkgrid')
+        figsize = (min(20, len(self.metrics) * 8), 5) if self.date_col else (8, 5)
+        fig, ax = plt.subplots(1, len(self.metrics), figsize=figsize)
         if not hasattr(ax, '__iter__'):
             ax = [ax]
 
         # Plot each metric
-        for i, metric in enumerate(vis_metrics):
+        for i, metric in enumerate(self.metrics):
 
             # If over time, plot line graph, else bar
             if self.date_col:
-                palette = ["C0", "C1", "k"][:self._splits_num]
-
-                sns.lineplot(data=df, x=self.date_col, y=metric, hue='bin', ax=ax[i], palette='Dark2')
+                sns.lineplot(data=self._df_agg, x=self.date_col, y=metric, hue='bin', ax=ax[i], palette='Dark2')
             else:
-                df['metric'] = metric
-                sns.barplot(data=df, x='metric', y=metric, hue='bin', ax=ax[i])
+                self._df_agg['metric'] = metric
+                sns.barplot(data=self._df_agg, x='metric', y=metric, hue='bin', ax=ax[i])
 
             ax[i].set_title(f'{metric.title()}')
             ax[i].tick_params(axis='x', labelrotation=45)
 
         plt.show()
 
 
@@ -359,28 +419,21 @@
             metric_weights (dict): Weights for each metric in the data (default: {})
             **kwargs: Additional keyword arguments
         """
         super().__init__(ga_params=ga_params, metric_weights=metric_weights, **kwargs)
         self.df = df
         self._population = Data(self.df.copy(), **kwargs)
 
-    def visualise(self, column=None):
-        """Visualizes the A/B split results.
-
-        Returns:
-            None
-        """
-
+    def _build_df_vis(self):
         # Merge solution results (_df_results) onto input data (metrics) so that data can be visualised
         self._df_vis = self._population.stacked.merge(
             self._df_result,
             left_index=True,
             right_index=True
         )
-        super().visualise(column=column)
 
     def __repr__(self):
         lst_str = [f"'{col}', " for col in self.all_spec_columns]
         return f'ABSplit([{lst_str}])'
 
 
 class MatchDataProc:
@@ -512,42 +565,34 @@
         Returns:
             None
         """
         # Run genetic algorithm
         super().run()
 
         # Filter on only bin == 1
-        self._df_result = self._df_result[self._df_result['bin'] == 1]
+        self._df_result = self._df_result[self._df_result['bin'] == '1']
 
         # Get sample index, set as bin 0, concat to _df_results (which are all bin 1)
         index_cols = self._sample.index.index.names
         df_match = self._df_samp[index_cols].drop_duplicates().set_index(index_cols)
-        df_match['bin'] = 0
+        df_match['bin'] = '0'
         self._df_result = pd.concat([self._df_result, df_match], axis=0).sort_index()
 
-    def visualise(self, column=None):
-        """Visualizes sample and results side by side
-
-        Returns:
-            None
-        """
-
+    def _build_df_vis(self):
         # Concat to form entire population
         self._df_vis = pd.concat([self._population.stacked, self._sample.stacked], axis=0)
 
         # Inner join to filter out all but sample and match
         self._df_vis = self._df_vis.merge(
             self._df_result,
             left_index=True,
             right_index=True,
             how='inner'
         )
 
-        super().visualise(column=column)
-
     def __repr__(self):
         lst_str = [f"'{col}', " for col in self.all_spec_columns]
         return f'Match([{lst_str}])'
 
 
 def fitness_func_absplit(ga_instance, solution, solution_idx):
     """Fitness function for ABSplit
@@ -556,21 +601,24 @@
     global metric_weights_global
     global splits_global
     global size_penalty_global
 
     # Generate binary array, 1 row of 0s and 1s for each group (where solution == 1/2/3 etc)
     groups = np.array([(solution == i).astype(int) for i in range(len(splits_global))])
 
+    # print(groups.shape)
+
     # Size penalty
     # Calculate all_metrics mean * number of days * number of metrics
     mean = np.mean(all_metrics_global) * all_metrics_global.shape[0] * all_metrics_global.shape[2]
     # Get size cost for each group
     mean_group = (groups * mean).sum(1) * splits_global
     # Calculate group differences, sum
-    size_cost = (np.abs(np.roll(mean_group, -1) - mean_group).sum()) * size_penalty_global
+    size_cost = (np.abs(np.roll(mean_group, -1) - mean_group).sum()) * size_penalty_global / len(splits_global)
+    # return
 
     # Metric cost
     costs = (groups @ all_metrics_global) * splits_global.reshape((1, -1, 1)) * metric_weights_global.reshape(-1, 1, 1)
     diffs = np.roll(costs, -1, axis=1) - costs
     mse = ((diffs ** 2).mean(axis=1)).sum()
     mse = mse + size_cost
```

### Comparing `absplit-1.0.1/absplit/param.py` & `absplit-1.1.0/absplit/param.py`

 * *Files identical despite different names*

### Comparing `absplit-1.0.1/images/logo.jpeg` & `absplit-1.1.0/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `absplit-1.0.1/pyproject.toml` & `absplit-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "absplit"
-version = "1.0.1"
+version = "1.1.0"
 description = "Generates A/B test groups"
 readme = "README.md"
 authors = [{name = "Cormac Rynne", email = "cormac.ry@gmail.com"}]
 license = {file = "LICENSE"}
 repository = "https://github.com/cormac-rynne/absplit"
 requires-python = "<=3.11"
 classifiers = [
```

### Comparing `absplit-1.0.1/tests/test_data.py` & `absplit-1.1.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `absplit-1.0.1/tests/test_ga.py` & `absplit-1.1.0/tests/test_ga.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,21 +30,21 @@
 ab.run()
 
 # Results
 data_dct1 = {
     'country': {0: 'UK', 1: 'UK', 2: 'UK', 3: 'UK', 4: 'UK'},
     'region': {0: 'x', 1: 'y', 2: 'y', 3: 'z', 4: 'z'},
     'city': {0: 'e', 1: 'c', 2: 'd', 3: 'a', 4: 'b'},
-    'bin': {0: 1, 1: 0, 2: 0, 3: 1, 4: 1}
+    'bin': {0: '1', 1: '0', 2: '0', 3: '1', 4: '1'}
 }
 data_dct2 = {
     'country': {0: 'UK', 1: 'UK', 2: 'UK', 3: 'UK', 4: 'UK'},
     'region': {0: 'x', 1: 'y', 2: 'y', 3: 'z', 4: 'z'},
     'city': {0: 'e', 1: 'c', 2: 'd', 3: 'a', 4: 'b'},
-    'bin': {0: 0, 1: 1, 2: 1, 3: 0, 4: 0}
+    'bin': {0: '0', 1: '1', 2: '1', 3: '0', 4: '0'}
 }
 df_data1 = pd.DataFrame(data_dct1)
 df_data2 = pd.DataFrame(data_dct2)
 
 
 def test_ab_results():
     """GA output ab.results"""
@@ -70,9 +70,9 @@
     sample=df_sample,
     **kwargs
 )
 m.run()
 
 
 def test_match_results():
-    dct = {'bin': {('UK', 'w', 'f'): 0, ('UK', 'z', 'a'): 1, ('UK', 'z', 'b'): 1}}
+    dct = {'bin': {('UK', 'w', 'f'): '0', ('UK', 'z', 'a'): '1', ('UK', 'z', 'b'): '1'}}
     assert m.results.to_dict() == dct
```

### Comparing `absplit-1.0.1/PKG-INFO` & `absplit-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absplit
-Version: 1.0.1
+Version: 1.1.0
 Summary: Generates A/B test groups
 Keywords: absplit,a/b test,ab test,ab split,split,set formation,group formation
 Author-email: Cormac Rynne <cormac.ry@gmail.com>
 Requires-Python: <=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -31,15 +31,15 @@
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
 Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-1.0.1-blue.svg)
+![version](https://img.shields.io/badge/version-1.1.0-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: absplit Version: 1.0.1 Summary: Generates A/B test
+Metadata-Version: 2.1 Name: absplit Version: 1.1.0 Summary: Generates A/B test
 groups Keywords: absplit,a/b test,ab test,ab split,split,set formation,group
 formation Author-email: Cormac Rynne
 ry@gmail.com> Requires-Python: <=3.11 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -15,15 +15,15 @@
 Libraries :: Python Modules Requires-Dist: pygad==3.0.1 Requires-Dist: scikit-
 learn Requires-Dist: numpy Requires-Dist: pandas Requires-Dist: seaborn
 Project-URL: Home, https://github.com/cormac-rynne/absplit
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                **** ABSplit ****
  Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 1.0.1-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.1.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Installation
    3. Tutorials
           o Do_it_yourself
    4. Usage
```

