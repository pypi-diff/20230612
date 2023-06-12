# Comparing `tmp/AutoCarver-4.4.0.tar.gz` & `tmp/AutoCarver-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-4.4.0.tar", last modified: Sun Jun 11 09:49:42 2023, max compression
+gzip compressed data, was "AutoCarver-4.4.1.tar", last modified: Mon Jun 12 12:14:28 2023, max compression
```

## Comparing `AutoCarver-4.4.0.tar` & `AutoCarver-4.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:49:42.932103 AutoCarver-4.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:49:42.932103 AutoCarver-4.4.0/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)    23484 2023-06-11 09:49:33.000000 AutoCarver-4.4.0/AutoCarver/AutoCarver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-11 09:49:33.000000 AutoCarver-4.4.0/AutoCarver/Converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    51578 2023-06-11 09:49:33.000000 AutoCarver-4.4.0/AutoCarver/Discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27407 2023-06-11 09:49:33.000000 AutoCarver-4.4.0/AutoCarver/FeatureSelector.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 09:49:33.000000 AutoCarver-4.4.0/AutoCarver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:49:42.932103 AutoCarver-4.4.0/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-06-11 09:49:42.000000 AutoCarver-4.4.0/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-11 09:49:42.000000 AutoCarver-4.4.0/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 09:49:42.000000 AutoCarver-4.4.0/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-11 09:49:42.000000 AutoCarver-4.4.0/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-11 09:49:33.000000 AutoCarver-4.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-06-11 09:49:42.932103 AutoCarver-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17418 2023-06-11 09:49:33.000000 AutoCarver-4.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 09:49:42.932103 AutoCarver-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-11 09:49:33.000000 AutoCarver-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:14:28.942246 AutoCarver-4.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:14:28.942246 AutoCarver-4.4.1/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)    24410 2023-06-12 12:14:19.000000 AutoCarver-4.4.1/AutoCarver/AutoCarver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-12 12:14:19.000000 AutoCarver-4.4.1/AutoCarver/Converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52397 2023-06-12 12:14:19.000000 AutoCarver-4.4.1/AutoCarver/Discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27508 2023-06-12 12:14:19.000000 AutoCarver-4.4.1/AutoCarver/FeatureSelector.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 12:14:19.000000 AutoCarver-4.4.1/AutoCarver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:14:28.942246 AutoCarver-4.4.1/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-06-12 12:14:28.000000 AutoCarver-4.4.1/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-12 12:14:28.000000 AutoCarver-4.4.1/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:14:28.000000 AutoCarver-4.4.1/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 12:14:28.000000 AutoCarver-4.4.1/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-12 12:14:19.000000 AutoCarver-4.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-06-12 12:14:28.942246 AutoCarver-4.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17418 2023-06-12 12:14:19.000000 AutoCarver-4.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 12:14:28.942246 AutoCarver-4.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-12 12:14:19.000000 AutoCarver-4.4.1/setup.py
```

### Comparing `AutoCarver-4.4.0/AutoCarver/AutoCarver.py` & `AutoCarver-4.4.1/AutoCarver/AutoCarver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 from .Discretizers import GroupedList, GroupedListDiscretizer, is_equal
 from IPython.display import display_html
-from matplotlib.pyplot import subplots, show
+from matplotlib.axes import Axes
+from matplotlib.figure import Figure
+from matplotlib.pyplot import subplots
 from matplotlib.ticker import PercentFormatter
-from numpy import sort, nan, inf, float32, where, isin, argsort, array, append, quantile, linspace, argmin, sqrt, random
-from pandas import DataFrame, Series, isna, qcut, notna, unique, concat, crosstab
+from numpy import sqrt
+from pandas import DataFrame, Series, notna, unique, crosstab
 from pandas.api.types import is_string_dtype
 from scipy.stats import chi2_contingency
 from seaborn import color_palette, despine
 from tqdm.notebook import tqdm
 from typing import Any, Dict, List, Tuple
 
 
 class AutoCarver(GroupedListDiscretizer):
-    """ Automatic carving of continuous, categorical and categorical ordinal features 
-    that maximizes association with a binary target.
+    """ Automatic carving of continuous, categorical and categorical ordinal
+    features that maximizes association with a binary target.
 
-    Modalities/values of features are carved/regrouped according to a computed specific
-    order defined based on their types:
+    Modalities/values of features are carved/regrouped according to a computed
+    specific order defined based on their types:
      - [Qualitative features] grouped based on modality target rate.
-     - [Qualitative ordinal features] grouped based on specified modality order.
+     - [Qualitative ordinal features] grouped based on specified modality order
      - [Quantitative features] grouped based on the order of their values.
-    Uses Tschurpow's T to find the optimal carving (regrouping) of modalities/values
-    of features.
+    Uses Tschurpow's T to find the optimal carving (regrouping) of modalities/
+    values of features.
 
     Parameters
     ----------
     values_orders: dict, default {}
         Dictionnary of features and list of their respective values' order.
-        Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
+        Exemple: for an `age` feature, `values_orders` could be
+        `{'age': ['0-18', '18-30', '30-50', '50+']}`.
 
     sort_by: str, default 'tschuprowt'
-        Association measure used to find the optimal group modality combination.
+        Association measure used to find the optimal group modality combination
         Implemented: ['cramerv', 'tschuprowt']
 
     max_n_mod: int, default 5
-        Maximum number of modalities for the carved features (excluding `numpy.nan`).
-         - All possible combinations of less than `max_n_mod` groups of modalities will be tested. 
-        Recommandation: `max_n_mod` should be set from 4 (faster) to 6 (preciser).
+        Maximum number of modalities for the carved features (excluding `nan`).
+         - All possible combinations of less than `max_n_mod` groups of
+           modalities will be tested.
+        Recommandation: `max_n_mod` should be set from 4 (faster) to 6
+        (preciser).
 
     keep_nans: bool, default False
         Whether or not to group `numpy.nan` to other modalities/values.
 
     Examples
     ----------
 
@@ -59,26 +64,30 @@
     # specifying orders of categorical ordinal features
     values_orders = {
         'age': ['0-18', '18-30', '30-50', '50+'],
         'grade': ['A', 'B', 'C', 'D', 'J', 'K', 'NN']
     }
 
     # pre-processing of features into categorical ordinal features
-    discretizer = Discretizer(selected_quanti, selected_quali, min_freq=0.02, q=20, values_orders=values_orders)
+    discretizer = Discretizer(
+        selected_quanti, selected_quali, min_freq=0.02, q=20,
+        values_orders=values_orders
+    )
     X_train = discretizer.fit_transform(X_train, y_train)
     X_test = discretizer.transform(X_test)
 
     # storing Discretizer
     pipe = [('Discretizer', discretizer)]
 
-    # updating features' values orders (at this step every features are qualitative ordinal)
+    # updating features' values orders (every features are qualitative ordinal)
     values_orders = discretizer.values_orders
 
     # intiating AutoCarver
-    auto_carver = AutoCarver(values_orders, sort_by='cramerv', max_n_mod=5, sample_size=0.01)
+    auto_carver = AutoCarver(
+        values_orders, sort_by='cramerv', max_n_mod=5, sample_size=0.01)
 
     # fitting on training sample
     # a test sample can be specified to evaluate carving robustness
     X_train = auto_carver.fit_transform(X_train, y_train, X_test, y_test)
 
     # applying transformation on test sample
     X_test = auto_carver.transform(X_test)
@@ -91,34 +100,49 @@
     pipe = Pipeline(pipe)
 
     # applying pipe to a validation set or in production
     X_val = pipe.transform(X_val)
 
     """
    
-    def __init__(self, values_orders: Dict[str, Any], *, sort_by: str='tschuprowt',
-                 copy: bool=False, max_n_mod: int=5, dropna: bool=True,
-                 verbose: bool=True, str_nan: str='__NAN__') -> None:
+    def __init__(
+            self,
+            values_orders: Dict[str, Any],
+            *,
+            max_n_mod: int=5,
+            sort_by: str='tschuprowt',
+            str_nan: str='__NAN__',
+            dropna: bool=True,
+            copy: bool=False,
+            verbose: bool=True
+        ) -> None:
         
         self.features = list(values_orders.keys())
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.non_viable_features: List[str] = []  # list of features non viable features
         self.max_n_mod = max_n_mod  # maximum number of modality per feature
         self.dropna = dropna  # whether or not to group NaNs with other modalities
         
         # association measure used to find the best groups
-        implemented = ['tschuprowt', 'cramerv']
-        assert sort_by in implemented, f"Measure {sort_by} is not yet implemented. Choose from: {', '.join(implemented)}."
+        measures = ['tschuprowt', 'cramerv']
+        assert sort_by in measures, f"""{sort_by} not yet implemented. Choose
+                                        from: {', '.join(measures)}."""
         self.sort_by = sort_by
 
         self.copy = copy
         self.verbose = verbose
         self.str_nan = str_nan
     
-    def prepare_data(self, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None) -> Tuple[DataFrame, Series, DataFrame, Series]:
+    def prepare_data(
+            self,
+            X: DataFrame,
+            y: Series,
+            X_test: DataFrame=None,
+            y_test: Series=None
+        ) -> Tuple[DataFrame, Series, DataFrame, Series]:
         """ Checks validity of provided data"""
         
         # preparing train sample
         # checking for binary target
         y_values = unique(y)
         assert (0 in y_values) & (1 in y_values), "y must be a binary Series (int or float, not object)"
         assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
@@ -149,15 +173,21 @@
         
             # checking for quantitative columns
             is_object = X_test[self.features].dtypes.apply(is_string_dtype)
             assert all(is_object), f"Non-string features in X_test: {', '.join(is_object[~is_object].index)}, consider using Discretizer."
             
         return Xc, y, Xtestc, y_test
     
-    def fit(self, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None) -> None:
+    def fit(
+            self,
+            X: DataFrame,
+            y: Series,
+            X_test: DataFrame=None,
+            y_test: Series=None
+        ) -> None:
 
         # preparing datasets and checking for wrong values
         Xc, y, Xtestc, y_test = self.prepare_data(X, y, X_test, y_test)
         
         # automatic carving of each feature
         for n, feature in tqdm(enumerate(self.features), total=len(self.features), disable=self.verbose):
 
@@ -175,15 +205,22 @@
         # discretizing features based on each feature's values_order
         super().__init__(self.values_orders, str_nan=self.str_nan, copy=self.copy, output=float)
         super().fit(X, y)
 
         return self
 
 
-    def get_best_combination(self, feature: str, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None) -> Dict[str, Any]:
+    def get_best_combination(
+            self,
+            feature: str,
+            X: DataFrame,
+            y: Series,
+            X_test: DataFrame=None,
+            y_test: Series=None
+        ) -> Dict[str, Any]:
         """ Carves a feature"""
 
         # computing crosstabs
         # crosstab on TRAIN
         xtab = nan_crosstab(X[feature], y, self.str_nan)
 
         # crosstab on TEST
@@ -217,29 +254,38 @@
 
         # printing the new group statistics
         if self.verbose and best_groups:
             self.display_xtabs(feature, 'Fitted', xtab, xtab_test)
 
         return best_groups
 
-    def insert_nan(self, feature: str, xtab: DataFrame) -> GroupedList:
+    def insert_nan(
+            self,
+            feature: str,
+            xtab: DataFrame
+        ) -> GroupedList:
         """ Inserts NaNs in the order"""
 
         # accessing order for specified feature
         order = self.values_orders.get(feature)
 
         # adding nans at the end of the order
         if self.str_nan not in order:
             order = order.append(self.str_nan)
 
             # updating values_orders
             self.values_orders.update({feature: order})
 
-
-    def update_order(self, feature: str, best_groups: GroupedList, xtab: DataFrame, xtab_test: DataFrame=None) -> Tuple[DataFrame, DataFrame]:
+    def update_order(
+            self,
+            feature: str,
+            best_groups: GroupedList,
+            xtab: DataFrame,
+            xtab_test: DataFrame=None
+        ) -> Tuple[DataFrame, DataFrame]:
         """ Updates the values_orders and xtabs according to the best_groups"""
 
         # updating values_orders with best_combination 
         self.values_orders.update({feature: best_groups})
 
         # update of the TRAIN crosstab
         best_combi = list(map(best_groups.get_group, xtab.index))
@@ -248,15 +294,21 @@
         # update of the TEST crosstab
         if xtab_test is not None:
             best_combi = list(map(best_groups.get_group, xtab_test.index))
             xtab_test = xtab_test.groupby(best_combi, dropna=False).sum()
         
         return xtab, xtab_test
     
-    def display_xtabs(self, feature: str, caption: str, xtab: DataFrame, xtab_test: DataFrame=None) -> None:
+    def display_xtabs(
+            self,
+            feature: str,
+            caption: str,
+            xtab: DataFrame,
+            xtab_test: DataFrame=None
+        ) -> None:
         """ Pretty display of frequency and target rate per modality on the same line. """
         
         # known_order per feature
         known_order = self.values_orders.get(feature)
         
         # target rate and frequency on TRAIN
         train_stats = stats_xtab(xtab, known_order)
@@ -281,24 +333,31 @@
             test_style = test_style.set_table_attributes("style='display:inline'")  # printing in notebook
             test_style = test_style.set_caption(f'{caption} distribution on X_test:')  # title
             html += ' ' + test_style._repr_html_()
 
         # displaying html of colored DataFrame
         display_html(html, raw=True)
 
-def groupedlist_combination(combination: List[List[Any]], order: GroupedList) -> GroupedList:
+def groupedlist_combination(
+        combination: List[List[Any]],
+        order: GroupedList
+    ) -> GroupedList:
     """ Converts a list of combination to a GroupedList"""
     
     order_copy = GroupedList(order)
     for combi in combination:
         order_copy.group_list(combi, combi[0])
     
     return order_copy
 
-def stats_xtab(xtab: DataFrame, known_order: List[Any]=None, known_labels: List[Any]=None) -> DataFrame:
+def stats_xtab(
+        xtab: DataFrame,
+        known_order: List[Any]=None,
+        known_labels: List[Any]=None
+    ) -> DataFrame:
     """ Computes column (target) rate per row (modality) and row frequency"""
     
     # target rate and frequency statistics per modality
     stats = DataFrame({
         # target rate per modality
         'target_rate': xtab[1].divide(xtab.sum(axis=1)),
         # frequency per modality
@@ -339,15 +398,18 @@
     
     # sorting statistics
     stats = stats.reindex(order, fill_value=0)
     stats['labels'] = labels
     
     return stats
 
-def apply_combination(xtab: DataFrame, combination: GroupedList) -> Dict[str, Any]:
+def apply_combination(
+        xtab: DataFrame,
+        combination: GroupedList
+    ) -> Dict[str, Any]:
     """ applies a modality combination to a crosstab """
 
     # initiating association dict
     association = {'combination': combination}
 
     # grouping modalities in the initial crosstab
     groups = list(map(combination.get_group, xtab.index))
@@ -355,15 +417,23 @@
     association.update({'combi_xtab': combi_xtab})
 
     # measuring association with the target
     association.update(association_xtab(combi_xtab))
 
     return association
 
-def best_combination(order: GroupedList, max_n_mod: int, sort_by: str, xtab_train: DataFrame, xtab_dev: DataFrame=None, dropna: bool=True, str_nan: str=None):
+def best_combination(
+        order: GroupedList,
+        max_n_mod: int,
+        sort_by: str,
+        xtab_train: DataFrame,
+        xtab_dev: DataFrame=None,
+        dropna: bool=True,
+        str_nan: str=None
+    ) -> Dict[str, Any]:
     """ Finds the best combination of groups of feature's values:
      - Most associated combination on train sample 
      - Stable target rate of combination on test sample.
     """
     
     # copying crosstabs
     xtab = xtab_train
@@ -427,15 +497,20 @@
             if viability:
 
                 association.update({'combi_xtab_test': combi_xtab_test})
 
                 return association
 
 
-def get_all_combinations(values: GroupedList, max_n_mod: int=None, raw: bool=False) -> List[GroupedList]:
+def get_all_combinations(
+        values: GroupedList,
+        max_n_mod: int=None,
+        raw: bool=False
+    ) -> List[GroupedList]:
+    """ Returns all possible triangular combinations"""
 
     # maximum number of classes
     q = len(values)
 
     # desired max number of classes
     if max_n_mod is None:
         max_n_mod = q
@@ -450,15 +525,19 @@
     
     # converting back to GroupedList
     if not raw:
         combinations = [groupedlist_combination(combination, values) for combination in combinations]
 
     return combinations
 
-def get_all_nan_combinations(order: GroupedList, str_nan: str, max_n_mod: int) -> List[GroupedList]:
+def get_all_nan_combinations(
+        order: GroupedList,
+        str_nan: str,
+        max_n_mod: int
+    ) -> List[GroupedList]:
     """ all possible combinations of modalities with numpy.nan"""
     
     # computing all non-NaN combinations
     # case 0: several modalities -> several combinations
     if len(order) > 1:
         combinations = get_all_combinations(order, max_n_mod-1, raw=True)
     # case 1: unique or no modality -> two combinations
@@ -489,15 +568,20 @@
     
     # converting back to GroupedList
     new_combinations = [groupedlist_combination(combination, order) for combination in new_combinations] 
 
     return new_combinations
 
 
-def consecutive_combinations(n_remaining: int, start: int, end: int, grp_for_this_step: list=None):
+def consecutive_combinations(
+        n_remaining: int,
+        start: int,
+        end: int,
+        grp_for_this_step: list=None
+    ) -> None:
     """HELPER finds all consecutive combinations between start and end.    """
 
     # Import de la liste globale
     global __li_of_res__
 
     # initiating group
     if not grp_for_this_step:
@@ -517,26 +601,26 @@
     else:
         
         ### Parcours de toutes les valeurs possibles de fin pour le i-ème groupe du groupement à x quantiles ###
         for i in range(start, end):
 
             consecutive_combinations(n_remaining-1, i+1, end, grp_for_this_step + [(start, i)])
             
-def get_combinations(n_class, q):
+def get_combinations(n_class: int, q: int) -> List[List[str]]:
     """HELPER recupération des combinaisons possibles de q quantiles pour n_class."""
     
     globals()['__li_of_res__'] = []
 
     consecutive_combinations(n_class-1, 0, q-1)
     
     combinations = [list(map(lambda u: (str(u[0]).zfill(len(str(q-1))), str(u[1]).zfill(len(str(q-1)))), l)) for l in __li_of_res__]
     
     return combinations
 
-def association_xtab(xtab: DataFrame):
+def association_xtab(xtab: DataFrame) -> Dict[str, float]:
     """ Computes measures of association between feature x and feature2. """
 
     # numnber of observations
     n_obs = xtab.sum().sum()
 
     # number of values taken by the features
     n_mod_x, n_mod_y = len(xtab.index), len(xtab.columns)
@@ -556,27 +640,31 @@
     if dof_mods > 0:
         tschuprowt = sqrt(chi2 / n_obs / dof_mods)
 
     results = {'cramerv': cramerv, 'tschuprowt': tschuprowt}
     
     return results
 
-def nan_crosstab(x: Series, y: Series, str_nan: str='__NAN__'):
+def nan_crosstab(
+        x: Series,
+        y: Series,
+        str_nan: str='__NAN__'
+    ):
     """ Crosstab that keeps nans as a specific value"""
     
     # keeping NaNs as a specific modality
     x_filled = x.fillna(str_nan)  # filling NaNs
 
     # computing initial crosstabs
     xtab = crosstab(x_filled, y)
     
     return xtab
 
 
-def plot_stats(stats):
+def plot_stats(stats: DataFrame) -> Tuple[Figure, Axes]:
     """ Barplot of the volume and target rate"""
     
     x = [0] + [elt for e in stats['frequency'].cumsum()[:-1] for elt in [e] * 2] + [1]
     y2 = [elt for e in list(stats['target_rate']) for elt in [e]*2]
     s = list(stats.index)
     scaled_y2 = [(y-min(y2)) / (max(y2) - min(y2)) for y in y2]
     c = color_palette("coolwarm", as_cmap=True)(scaled_y2)
```

### Comparing `AutoCarver-4.4.0/AutoCarver/Converters.py` & `AutoCarver-4.4.1/AutoCarver/Converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-4.4.0/AutoCarver/Discretizers.py` & `AutoCarver-4.4.1/AutoCarver/Discretizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .Converters import StringConverter
 from IPython.display import display_html
 from numpy import sort, nan, inf, float32, where, isin, argsort, array, select, append, quantile, linspace, argmin
 from pandas import DataFrame, Series, isna, qcut, notna, unique
 from pandas.api.types import is_numeric_dtype, is_string_dtype
 from sklearn.base import BaseEstimator, TransformerMixin
 from typing import Any, Dict, List
 from warnings import warn
@@ -210,17 +211,23 @@
                 repr += [f'{values[-1]}'[:char_limit]+' to '+f'{values[0]}'[:char_limit]]
                 
         return repr
 
 
 class GroupedListDiscretizer(BaseEstimator, TransformerMixin):
     
-    def __init__(self, values_orders: Dict[str, Any], *, 
-        copy: bool=False, output: type= float,
-        str_nan: str=None, verbose: bool=False) -> None:
+    def __init__(
+            self,
+            values_orders: Dict[str, Any],
+            *,
+            copy: bool=False,
+            output: type= float,
+            str_nan: str=None,
+            verbose: bool=False
+        ) -> None:
         
         self.features = list(values_orders.keys())
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.copy = copy
         self.output = output
         self.verbose = verbose
         self.str_nan = str_nan
@@ -295,48 +302,64 @@
         [Qualitative ordinal features] dict of features values and list of orders of their values.
          - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
         (smallest frequency or closest target rate), between the superior and inferior values (described
         by the `values_orders`).
         Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
     """
     
-    def __init__(self, features: List[str], min_freq: float, *,
-                 values_orders: Dict[str, Any]={}, copy: bool=False, 
-                 verbose: bool=False) -> None:
+    def __init__(
+            self,
+            features: List[str],
+            min_freq: float,
+            *,
+            values_orders: Dict[str, Any]={},
+            copy: bool=False,
+            verbose: bool=False
+        ) -> None:
     
         self.features = features[:]
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.ordinal_features = [f for f in values_orders if f in features]  # ignores non qualitative features
         self.non_ordinal_features = [f for f in features if f not in self.ordinal_features]
         self.min_freq = min_freq
         self.pipe: List[BaseEstimator] = []
         self.copy = copy
         self.verbose = verbose
         
     def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
         """ Checking data for bucketization"""
-        
+
+        # copying dataframe
+        Xc = X.copy()
+
         # checking for quantitative columns
-        is_object = X[self.features].dtypes.apply(is_string_dtype)
-        assert all(is_object), f"Non-string features: {', '.join(is_object[~is_object].index)}, consider using Converters.StringConverter."
-        
+        is_object = Xc[self.features].dtypes.apply(is_string_dtype)
+        if not all(is_object):  # non qualitative features detected
+
+            if self.verbose:
+                print(f"""Non-string features: {', '.join(is_object[~is_object].index)}, will be converted using Converters.StringConverter.""")
+
+            # converting specified features into qualitative features
+            stringer = StringConverter(features=self.features)
+            Xc = stringer.fit_transform(Xc)
+
+            # append the string converter to the feature engineering pipeline
+            self.pipe += [('StringConverter', stringer)]
+
         # checking for binary target
         y_values = unique(y)
         assert (0 in y_values) & (1 in y_values), "y must be a binary Series (int or float, not object)"
         assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
-        
+
         # checking that all unique values in X are in values_orders
-        uniques = X[self.features].apply(nan_unique)
+        uniques = Xc[self.features].apply(nan_unique)
         for feature in self.ordinal_features:
             missing = [val for val in uniques[feature] if val not in self.values_orders[feature]]
             assert len(missing)==0, f"The ordering for {', '.join(missing)} of feature '{feature}' must be specified in values_orders (str-only)."
-        
-        # copying dataframe
-        Xc = X.copy()
-        
+
         return Xc
 
     def fit(self, X: DataFrame, y: Series) -> None:
         """ Learning TRAIN distribution"""
         
         # checking data before bucketization
         Xc = self.prepare_data(X, y)
@@ -402,16 +425,23 @@
         cut into proportionaly less quantiles (`q:=max(round(non_frequent * q), 1)`). 
         Exemple: if q=10 and the value numpy.nan represent 50 % of the observed values, non-NaNs will be 
         cut in q=5 quantiles.
         Recommandation: `q` should be set from 10 (faster) to 20 (preciser).
 
     """
     
-    def __init__(self, features: List[str], q: int, *, values_orders: Dict[str, Any]={}, copy: bool=False, 
-                 verbose: bool=False) -> None:
+    def __init__(
+            self,
+            features: List[str],
+            q: int,
+            *,
+            values_orders: Dict[str, Any]={},
+            copy: bool=False,
+            verbose: bool=False
+        ) -> None:
         
         self.features = features[:]
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
         self.q = q
         self.pipe: List[BaseEstimator] = []
         self.copy = copy
         self.verbose = verbose
@@ -524,16 +554,24 @@
         [Qualitative ordinal features] dict of features values and list of orders of their values.
          - [Qualitative ordinal features] Less frequent modalities are grouped to the closest modality 
         (smallest frequency or closest target rate), between the superior and inferior values (described
         by the `values_orders`).
         Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
     """
 
-    def __init__(self, quanti_features: List[str], quali_features: List[str], min_freq: float, *, 
-                 values_orders: Dict[str, Any]={}, copy: bool=False, verbose: bool=False) -> None:
+    def __init__(
+            self,
+            quanti_features: List[str],
+            quali_features: List[str],
+            min_freq: float,
+            *,
+            values_orders: Dict[str, Any]={},
+            copy: bool=False,
+            verbose: bool=False
+        ) -> None:
 
         self.features = quanti_features[:] + quali_features[:]
         self.quanti_features = quanti_features[:]
         assert len(list(set(quanti_features))) == len(quanti_features), "Column duplicates in quanti_features"
         self.quali_features = quali_features[:]
         assert len(list(set(quali_features))) == len(quali_features), "Column duplicates in quali_features"
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
@@ -602,16 +640,25 @@
 
         return Xc
 
 
 
 class ChainedDiscretizer(GroupedListDiscretizer):
     
-    def __init__(self, features: List[str], min_freq: float, chained_orders: List[GroupedList], *, 
-                 remove_unknown: bool=False, str_nan: str='__NAN__', copy: bool=False, verbose: bool=False) -> None:       
+    def __init__(
+            self,
+            features: List[str],
+            min_freq: float,
+            chained_orders: List[GroupedList],
+            *,
+            remove_unknown: bool=False,
+            str_nan: str='__NAN__',
+            copy: bool=False,
+            verbose: bool=False
+        ) -> None:       
         
         self.min_freq = min_freq
         self.features = features[:]
         self.chained_orders = [GroupedList(order) for order in chained_orders]
         self.copy = copy
         self.verbose = verbose
```

### Comparing `AutoCarver-4.4.0/AutoCarver/FeatureSelector.py` & `AutoCarver-4.4.1/AutoCarver/FeatureSelector.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,16 +71,25 @@
         To be used with: `vif_filter`
     ascending, bool default False
         According to this measure:
          - True: Lower values of the measure are to be considered as more associated to the target
          - False: Higher values of the measure are to be considered as more associated to the target
     """
     
-    def __init__(self, features: List[str], n_best: int, measures: List[Callable]=list(), filters: List[Callable]=list(),
-                 sample_size: float=1., copy: bool=True, verbose: bool=True, **params) -> None:
+    def __init__(
+            self,
+            features: List[str],
+            n_best: int,
+            measures: List[Callable]=list(),
+            filters: List[Callable]=list(),
+            sample_size: float=1.,
+            copy: bool=True,
+            verbose: bool=True,
+            **params
+        ) -> None:
         
         self.features = features[:]
         self.n_best = n_best
         assert n_best <= len(features), "Must set n_best <= len(features)"
         self.best_features = features[:]
         self.sample_size = sample_size
```

### Comparing `AutoCarver-4.4.0/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-4.4.1/AutoCarver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 4.4.0
+Version: 4.4.1
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `AutoCarver-4.4.0/LICENSE` & `AutoCarver-4.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-4.4.0/PKG-INFO` & `AutoCarver-4.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 4.4.0
+Version: 4.4.1
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `AutoCarver-4.4.0/README.md` & `AutoCarver-4.4.1/README.md`

 * *Files identical despite different names*

### Comparing `AutoCarver-4.4.0/setup.py` & `AutoCarver-4.4.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name='AutoCarver',
-    version='4.4.0',
+    version='4.4.1',
     author='Mario DEFRANCE',
     author_email='defrancemario@gmail.com',
     description='Automatic Bucketizing of Features with Optimal Association',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mdefrance/AutoCarver',
-    project_urls = {
+    project_urls={
         "Bug Tracker": "https://github.com/mdefrance/AutoCarver/issues"
     },
     license='MIT',
     packages=['AutoCarver'],
     classifiers=[
-        'Development Status :: 4 - Beta',  # ou 4 - Beta ou 5 - Production/Stable
+        # ou 4 - Beta ou 5 - Production/Stable
+        'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         "Operating System :: Unix",
```

