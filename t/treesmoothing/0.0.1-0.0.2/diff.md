# Comparing `tmp/treesmoothing-0.0.1.tar.gz` & `tmp/treesmoothing-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treesmoothing-0.0.1.tar", last modified: Mon Jun 12 14:04:31 2023, max compression
+gzip compressed data, was "treesmoothing-0.0.2.tar", last modified: Mon Jun 12 14:32:03 2023, max compression
```

## Comparing `treesmoothing-0.0.1.tar` & `treesmoothing-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-06-12 14:04:31.183594 treesmoothing-0.0.1/
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     1089 2023-06-07 07:24:04.000000 treesmoothing-0.0.1/LICENSE
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     8180 2023-06-12 14:04:31.183594 treesmoothing-0.0.1/PKG-INFO
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     6942 2023-06-07 07:57:34.000000 treesmoothing-0.0.1/README.md
--rw-rw-r--   0 bastian   (1000) bastian   (1000)       38 2023-06-12 14:04:31.183594 treesmoothing-0.0.1/setup.cfg
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     1575 2023-06-12 13:57:17.000000 treesmoothing-0.0.1/setup.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-06-12 14:04:31.183594 treesmoothing-0.0.1/treesmoothing/
--rw-rw-r--   0 bastian   (1000) bastian   (1000)       43 2023-06-12 14:00:27.000000 treesmoothing-0.0.1/treesmoothing/__init__.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     8217 2023-06-05 13:26:08.000000 treesmoothing-0.0.1/treesmoothing/beta.py
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      132 2023-06-12 14:03:37.000000 treesmoothing-0.0.1/treesmoothing/core.py
-drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-06-12 14:04:31.183594 treesmoothing-0.0.1/treesmoothing.egg-info/
--rw-rw-r--   0 bastian   (1000) bastian   (1000)     8180 2023-06-12 14:04:31.000000 treesmoothing-0.0.1/treesmoothing.egg-info/PKG-INFO
--rw-rw-r--   0 bastian   (1000) bastian   (1000)      280 2023-06-12 14:04:31.000000 treesmoothing-0.0.1/treesmoothing.egg-info/SOURCES.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)        1 2023-06-12 14:04:31.000000 treesmoothing-0.0.1/treesmoothing.egg-info/dependency_links.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)       57 2023-06-12 14:04:31.000000 treesmoothing-0.0.1/treesmoothing.egg-info/requires.txt
--rw-rw-r--   0 bastian   (1000) bastian   (1000)       14 2023-06-12 14:04:31.000000 treesmoothing-0.0.1/treesmoothing.egg-info/top_level.txt
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-06-12 14:32:03.608429 treesmoothing-0.0.2/
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     1089 2023-06-07 07:24:04.000000 treesmoothing-0.0.2/LICENSE
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     8349 2023-06-12 14:32:03.608429 treesmoothing-0.0.2/PKG-INFO
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     7111 2023-06-12 14:24:07.000000 treesmoothing-0.0.2/README.md
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)       38 2023-06-12 14:32:03.608429 treesmoothing-0.0.2/setup.cfg
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     1575 2023-06-12 14:31:58.000000 treesmoothing-0.0.2/setup.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-06-12 14:32:03.608429 treesmoothing-0.0.2/treesmoothing/
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)       43 2023-06-12 14:00:27.000000 treesmoothing-0.0.2/treesmoothing/__init__.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     8217 2023-06-05 13:26:08.000000 treesmoothing-0.0.2/treesmoothing/beta.py
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      132 2023-06-12 14:03:37.000000 treesmoothing-0.0.2/treesmoothing/core.py
+drwxrwxr-x   0 bastian   (1000) bastian   (1000)        0 2023-06-12 14:32:03.608429 treesmoothing-0.0.2/treesmoothing.egg-info/
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)     8349 2023-06-12 14:32:03.000000 treesmoothing-0.0.2/treesmoothing.egg-info/PKG-INFO
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)      280 2023-06-12 14:32:03.000000 treesmoothing-0.0.2/treesmoothing.egg-info/SOURCES.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)        1 2023-06-12 14:32:03.000000 treesmoothing-0.0.2/treesmoothing.egg-info/dependency_links.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)       57 2023-06-12 14:32:03.000000 treesmoothing-0.0.2/treesmoothing.egg-info/requires.txt
+-rw-rw-r--   0 bastian   (1000) bastian   (1000)       14 2023-06-12 14:32:03.000000 treesmoothing-0.0.2/treesmoothing.egg-info/top_level.txt
```

### Comparing `treesmoothing-0.0.1/LICENSE` & `treesmoothing-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `treesmoothing-0.0.1/PKG-INFO` & `treesmoothing-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treesmoothing
-Version: 0.0.1
+Version: 0.0.2
 Summary: Bayesian post-hoc regularization for random forests
 Home-page: https://github.com/pievos101/TreeSmoothing
 Author: Bastian Pfeifer and Arne Gevaert
 Author-email: bastian.pfeifer@medunigraz.at
 License: MIT
 Keywords: Random Forest,Post-hoc Regularization
 Platform: UNKNOWN
@@ -54,15 +54,29 @@
     - `alpha`: alpha hyperparameter
     - `beta`: beta hyperparameter
     - `random_state`: random state for reproducibility
 - Other functions: `fit(X, y)`, `predict(X)`, `predict_proba(X)`, `score(X, y)` work just like with any other `sklearn` estimator.
 
 
 ## Usage
-Import of main function
+
+Install the Python package treesmoothing via pip
+
+```python
+pip install treesmoothing
+```
+
+and import the ShrinkageClassifier as 
+
+```python
+from treesmoothing import ShrinkageClassifier
+```
+
+or import of main function from source 
+
 ```python
 from beta import ShrinkageClassifier
 ```
 
 Other imports
 
 ```python
@@ -91,21 +105,20 @@
 #sc = "balanced_accuracy"
 sc = "roc_auc"
 
 # number of trees 
 ntrees = 10
 
 # Read in data set
-X, y, feature_names = get_clean_dataset(id, data_source=source)
+X, y, feature_names = get_clean_dataset('breast_cancer', data_source='imodels')
 
 # train-test split
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.20)
 
 scores = {}
-print(ds_name)
 
 scores["vanilla"] = []
 scores["hs"] = []
 scores["beta"] = []
 ```
 
 ### Vanilla Random Forest 
@@ -167,15 +180,15 @@
 
 param_grid = {
 "alpha": [1500, 1000, 800, 500, 100, 50, 30, 10, 1],
 "beta": [1500, 1000, 800, 500, 100, 50, 30, 10, 1],
 "shrink_mode": ["beta"]}
 
 grid_search = GridSearchCV(ShrinkageClassifier
-(RandomForestClassifie(n_estimators=ntrees)), param_grid, cv=5,
+(RandomForestClassifier(n_estimators=ntrees)), param_grid, cv=5,
 n_jobs=-1, scoring=sc)
 
 grid_search.fit(X, y)
 
 best_params = grid_search.best_params_
 print(best_params)
 clf = ShrinkageClassifier(RandomForestClassifier(n_estimators=ntrees),shrink_mode=shrink_mode, 
@@ -186,17 +199,18 @@
     pred_beta = clf.predict(X_test)
     scores[shrink_mode].append(balanced_accuracy_score(y_test, pred_beta))      
 if sc == "roc_auc":
     pred_beta = clf.predict_proba(X_test)[:,1]
     scores[shrink_mode].append(roc_auc_score(y_test, pred_beta))    
 ```
 
+Print the results
+
 ```python
-RES = np.vstack([scores['vanilla'],scores['hs'],scores['beta']])
-print(RES)
+print(scores)
 ```
 
 ## Acknowledgement 
 The TreeSmoothing Python code was written by Bastian Pfeifer and Arne Gevaert. 
 It is based on the Hierarchical Shrinkage implementation within the Python package imodels (https://github.com/csinva/imodels).
 
 ## Citation
```

### Comparing `treesmoothing-0.0.1/README.md` & `treesmoothing-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,29 @@
     - `alpha`: alpha hyperparameter
     - `beta`: beta hyperparameter
     - `random_state`: random state for reproducibility
 - Other functions: `fit(X, y)`, `predict(X)`, `predict_proba(X)`, `score(X, y)` work just like with any other `sklearn` estimator.
 
 
 ## Usage
-Import of main function
+
+Install the Python package treesmoothing via pip
+
+```python
+pip install treesmoothing
+```
+
+and import the ShrinkageClassifier as 
+
+```python
+from treesmoothing import ShrinkageClassifier
+```
+
+or import of main function from source 
+
 ```python
 from beta import ShrinkageClassifier
 ```
 
 Other imports
 
 ```python
@@ -60,21 +74,20 @@
 #sc = "balanced_accuracy"
 sc = "roc_auc"
 
 # number of trees 
 ntrees = 10
 
 # Read in data set
-X, y, feature_names = get_clean_dataset(id, data_source=source)
+X, y, feature_names = get_clean_dataset('breast_cancer', data_source='imodels')
 
 # train-test split
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.20)
 
 scores = {}
-print(ds_name)
 
 scores["vanilla"] = []
 scores["hs"] = []
 scores["beta"] = []
 ```
 
 ### Vanilla Random Forest 
@@ -136,15 +149,15 @@
 
 param_grid = {
 "alpha": [1500, 1000, 800, 500, 100, 50, 30, 10, 1],
 "beta": [1500, 1000, 800, 500, 100, 50, 30, 10, 1],
 "shrink_mode": ["beta"]}
 
 grid_search = GridSearchCV(ShrinkageClassifier
-(RandomForestClassifie(n_estimators=ntrees)), param_grid, cv=5,
+(RandomForestClassifier(n_estimators=ntrees)), param_grid, cv=5,
 n_jobs=-1, scoring=sc)
 
 grid_search.fit(X, y)
 
 best_params = grid_search.best_params_
 print(best_params)
 clf = ShrinkageClassifier(RandomForestClassifier(n_estimators=ntrees),shrink_mode=shrink_mode, 
@@ -155,17 +168,18 @@
     pred_beta = clf.predict(X_test)
     scores[shrink_mode].append(balanced_accuracy_score(y_test, pred_beta))      
 if sc == "roc_auc":
     pred_beta = clf.predict_proba(X_test)[:,1]
     scores[shrink_mode].append(roc_auc_score(y_test, pred_beta))    
 ```
 
+Print the results
+
 ```python
-RES = np.vstack([scores['vanilla'],scores['hs'],scores['beta']])
-print(RES)
+print(scores)
 ```
 
 ## Acknowledgement 
 The TreeSmoothing Python code was written by Bastian Pfeifer and Arne Gevaert. 
 It is based on the Hierarchical Shrinkage implementation within the Python package imodels (https://github.com/csinva/imodels).
 
 ## Citation
```

### Comparing `treesmoothing-0.0.1/setup.py` & `treesmoothing-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 """
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='treesmoothing',
-    version='0.0.1',
+    version='0.0.2',
     author='Bastian Pfeifer and Arne Gevaert',
     license='MIT',
     author_email='bastian.pfeifer@medunigraz.at',
     description='Bayesian post-hoc regularization for random forests',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/pievos101/TreeSmoothing',
```

### Comparing `treesmoothing-0.0.1/treesmoothing/beta.py` & `treesmoothing-0.0.2/treesmoothing/beta.py`

 * *Files identical despite different names*

### Comparing `treesmoothing-0.0.1/treesmoothing.egg-info/PKG-INFO` & `treesmoothing-0.0.2/treesmoothing.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treesmoothing
-Version: 0.0.1
+Version: 0.0.2
 Summary: Bayesian post-hoc regularization for random forests
 Home-page: https://github.com/pievos101/TreeSmoothing
 Author: Bastian Pfeifer and Arne Gevaert
 Author-email: bastian.pfeifer@medunigraz.at
 License: MIT
 Keywords: Random Forest,Post-hoc Regularization
 Platform: UNKNOWN
@@ -54,15 +54,29 @@
     - `alpha`: alpha hyperparameter
     - `beta`: beta hyperparameter
     - `random_state`: random state for reproducibility
 - Other functions: `fit(X, y)`, `predict(X)`, `predict_proba(X)`, `score(X, y)` work just like with any other `sklearn` estimator.
 
 
 ## Usage
-Import of main function
+
+Install the Python package treesmoothing via pip
+
+```python
+pip install treesmoothing
+```
+
+and import the ShrinkageClassifier as 
+
+```python
+from treesmoothing import ShrinkageClassifier
+```
+
+or import of main function from source 
+
 ```python
 from beta import ShrinkageClassifier
 ```
 
 Other imports
 
 ```python
@@ -91,21 +105,20 @@
 #sc = "balanced_accuracy"
 sc = "roc_auc"
 
 # number of trees 
 ntrees = 10
 
 # Read in data set
-X, y, feature_names = get_clean_dataset(id, data_source=source)
+X, y, feature_names = get_clean_dataset('breast_cancer', data_source='imodels')
 
 # train-test split
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.20)
 
 scores = {}
-print(ds_name)
 
 scores["vanilla"] = []
 scores["hs"] = []
 scores["beta"] = []
 ```
 
 ### Vanilla Random Forest 
@@ -167,15 +180,15 @@
 
 param_grid = {
 "alpha": [1500, 1000, 800, 500, 100, 50, 30, 10, 1],
 "beta": [1500, 1000, 800, 500, 100, 50, 30, 10, 1],
 "shrink_mode": ["beta"]}
 
 grid_search = GridSearchCV(ShrinkageClassifier
-(RandomForestClassifie(n_estimators=ntrees)), param_grid, cv=5,
+(RandomForestClassifier(n_estimators=ntrees)), param_grid, cv=5,
 n_jobs=-1, scoring=sc)
 
 grid_search.fit(X, y)
 
 best_params = grid_search.best_params_
 print(best_params)
 clf = ShrinkageClassifier(RandomForestClassifier(n_estimators=ntrees),shrink_mode=shrink_mode, 
@@ -186,17 +199,18 @@
     pred_beta = clf.predict(X_test)
     scores[shrink_mode].append(balanced_accuracy_score(y_test, pred_beta))      
 if sc == "roc_auc":
     pred_beta = clf.predict_proba(X_test)[:,1]
     scores[shrink_mode].append(roc_auc_score(y_test, pred_beta))    
 ```
 
+Print the results
+
 ```python
-RES = np.vstack([scores['vanilla'],scores['hs'],scores['beta']])
-print(RES)
+print(scores)
 ```
 
 ## Acknowledgement 
 The TreeSmoothing Python code was written by Bastian Pfeifer and Arne Gevaert. 
 It is based on the Hierarchical Shrinkage implementation within the Python package imodels (https://github.com/csinva/imodels).
 
 ## Citation
```

