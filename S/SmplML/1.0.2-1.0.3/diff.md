# Comparing `tmp/SmplML-1.0.2.tar.gz` & `tmp/SmplML-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SmplML-1.0.2.tar", last modified: Mon Jun 12 04:16:35 2023, max compression
+gzip compressed data, was "dist\SmplML-1.0.3.tar", last modified: Mon Jun 12 07:40:45 2023, max compression
```

## Comparing `SmplML-1.0.2.tar` & `SmplML-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 04:16:35.144250 SmplML-1.0.2/
--rw-rw-rw-   0        0        0       91 2023-06-12 04:14:53.000000 SmplML-1.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1086 2023-06-12 03:44:56.000000 SmplML-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       30 2023-06-12 03:44:54.000000 SmplML-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2767 2023-06-12 04:16:35.143238 SmplML-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1755 2023-06-12 04:14:55.000000 SmplML-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 04:16:35.136645 SmplML-1.0.2/SmplML.egg-info/
--rw-rw-rw-   0        0        0     2767 2023-06-12 04:16:34.000000 SmplML-1.0.2/SmplML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-06-12 04:16:35.000000 SmplML-1.0.2/SmplML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 04:16:34.000000 SmplML-1.0.2/SmplML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-12 04:16:34.000000 SmplML-1.0.2/SmplML.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 04:16:34.000000 SmplML-1.0.2/SmplML.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 04:16:35.145232 SmplML-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1433 2023-06-12 04:15:12.000000 SmplML-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:16:35.140752 SmplML-1.0.2/smpl_ml/
--rw-rw-rw-   0        0        0       46 2023-06-12 03:44:49.000000 SmplML-1.0.2/smpl_ml/__init__.py
--rw-rw-rw-   0        0        0     8081 2023-06-12 02:47:59.000000 SmplML-1.0.2/smpl_ml/classification_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:40:45.099145 SmplML-1.0.3/
+-rw-rw-rw-   0        0        0       90 2023-06-12 07:39:23.000000 SmplML-1.0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1086 2023-06-12 07:39:21.000000 SmplML-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-06-12 07:39:19.000000 SmplML-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3432 2023-06-12 07:40:45.097150 SmplML-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2398 2023-06-12 07:39:17.000000 SmplML-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 07:40:45.086819 SmplML-1.0.3/SmplML.egg-info/
+-rw-rw-rw-   0        0        0     3432 2023-06-12 07:40:44.000000 SmplML-1.0.3/SmplML.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-06-12 07:40:44.000000 SmplML-1.0.3/SmplML.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 07:40:44.000000 SmplML-1.0.3/SmplML.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-12 07:40:44.000000 SmplML-1.0.3/SmplML.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 07:40:44.000000 SmplML-1.0.3/SmplML.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 07:40:45.099145 SmplML-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1459 2023-06-12 07:33:16.000000 SmplML-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:40:45.093549 SmplML-1.0.3/smpl_ml/
+-rw-rw-rw-   0        0        0       46 2023-06-12 03:44:49.000000 SmplML-1.0.3/smpl_ml/__init__.py
+-rw-rw-rw-   0        0        0     9514 2023-06-12 07:39:41.000000 SmplML-1.0.3/smpl_ml/smpl_ml.py
```

### Comparing `SmplML-1.0.2/LICENSE` & `SmplML-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SmplML-1.0.2/PKG-INFO` & `SmplML-1.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: SmplML
-Version: 1.0.2
-Summary: SmplML is a user-friendly Python library for streamlined machine learning classification. It offers intuitive modules for data preprocessing, feature engineering, model training, and evaluation. Ideal for beginners and experts alike, SmplML simplifies classification tasks, enabling you to gain valuable insights from your data with ease.
+Version: 1.0.3
+Summary: SmplML is a user-friendly Python library for streamlined machine learning classification. It offers intuitive functions for data preprocessing, model training, and evaluation of both classification and regression tasks. Ideal for beginners and experts alike, SmplML simplifies tasks, enabling you to gain valuable insights from your data with ease.
 Home-page: https://github.com/JhunBrian/SmplML
 Author: Jhun Brian Andam
-Author-email: brianandam123@gmail.com
+Author-email: andam.jhunbrian@gmail.com
 License: MIT
-Keywords: Machine Learning,Classification
+Keywords: Machine Learning,Classification,Regression
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -30,45 +30,79 @@
 - You can install SmpML using pip:
 ```shell
 pip install SimpleML
 ```
 
 ## Usage
 
+### Classification
 ```python
 import seaborn as sns
 import pandas as pd
-from smpl_ml.classification_helpers import TrainClassifier
+from smpl_ml.smpl_ml import TrainModel
+
 from sklearn.neighbors import KNeighborsClassifier
 
 # Load the dataset
 df = sns.load_dataset('penguins')
 
 # Set the target and features
 target = 'species'
 features = df.iloc[:, df.columns != target].columns
 
 # Create the classifier trainer
-trainer = TrainClassifier(df.dropna(), target=target, features=features, model=KNeighborsClassifier())
+clf_trainer = TrainModel(df.dropna(), target=target, features=features, model=KNeighborsClassifier())
 
 # Fit the model
-trainer.fit()
+clf_trainer.fit()
 
 # Evaluate the model
-model = trainer.evaluate()
+clf_model = clf_trainer.evaluate()
 ```
 
 `model` when `verbose` is set to `True` will return a DataFrame of classification metrics.
 
 
 |    | Recall | Specificity | Precision | F1-Score | Accuracy |
 |----|--------|-------------|-----------|----------|----------|
 | Adelie | 0.91   | 0.70        | 0.67      | 0.77     | 0.76     |
 | Chinstrap | 0.38   | 0.92        | 0.62      | 0.47     | 0.76     |
 | Gentoo | 0.86   | 1.00        | 1.00      | 0.92     | 0.76     |
 
+### Regression
+```python
+import seaborn as sns
+import pandas as pd
+from smpl_ml.smpl_ml import TrainModel
+
+from sklearn.neighbors import KNeighborsRegressor
+
+# Load the dataset
+df = sns.load_dataset('iris')
+
+# Set the target and features
+target = 'sepal_length'
+features = df.columns[1:]
+
+# Create the regressor trainer
+reg_trainer = TrainModel(df.dropna(), target=target, features=features, model=KNeighborsRegressor())
+
+# Fit the model
+reg_trainer.fit()
+
+# Evaluate the model
+reg_model = reg_trainer.evaluate()
+```
+
+|   |Metrics|
+|---|-------|
+|MSE|0.11|
+|RMSE|0.34|
+|MAE|0.27|
+|R-Squared|0.74|
+
 Change Log
 ==================
 
-1.0.2 (06/12/2023)
+1.0.3 (06/12/2023)
 ------------------
-Updated README.md
+Added Regression
```

### Comparing `SmplML-1.0.2/README.md` & `SmplML-1.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -13,38 +13,72 @@
 - You can install SmpML using pip:
 ```shell
 pip install SimpleML
 ```
 
 ## Usage
 
+### Classification
 ```python
 import seaborn as sns
 import pandas as pd
-from smpl_ml.classification_helpers import TrainClassifier
+from smpl_ml.smpl_ml import TrainModel
+
 from sklearn.neighbors import KNeighborsClassifier
 
 # Load the dataset
 df = sns.load_dataset('penguins')
 
 # Set the target and features
 target = 'species'
 features = df.iloc[:, df.columns != target].columns
 
 # Create the classifier trainer
-trainer = TrainClassifier(df.dropna(), target=target, features=features, model=KNeighborsClassifier())
+clf_trainer = TrainModel(df.dropna(), target=target, features=features, model=KNeighborsClassifier())
 
 # Fit the model
-trainer.fit()
+clf_trainer.fit()
 
 # Evaluate the model
-model = trainer.evaluate()
+clf_model = clf_trainer.evaluate()
 ```
 
 `model` when `verbose` is set to `True` will return a DataFrame of classification metrics.
 
 
 |    | Recall | Specificity | Precision | F1-Score | Accuracy |
 |----|--------|-------------|-----------|----------|----------|
 | Adelie | 0.91   | 0.70        | 0.67      | 0.77     | 0.76     |
 | Chinstrap | 0.38   | 0.92        | 0.62      | 0.47     | 0.76     |
-| Gentoo | 0.86   | 1.00        | 1.00      | 0.92     | 0.76     |
+| Gentoo | 0.86   | 1.00        | 1.00      | 0.92     | 0.76     |
+
+### Regression
+```python
+import seaborn as sns
+import pandas as pd
+from smpl_ml.smpl_ml import TrainModel
+
+from sklearn.neighbors import KNeighborsRegressor
+
+# Load the dataset
+df = sns.load_dataset('iris')
+
+# Set the target and features
+target = 'sepal_length'
+features = df.columns[1:]
+
+# Create the regressor trainer
+reg_trainer = TrainModel(df.dropna(), target=target, features=features, model=KNeighborsRegressor())
+
+# Fit the model
+reg_trainer.fit()
+
+# Evaluate the model
+reg_model = reg_trainer.evaluate()
+```
+
+|   |Metrics|
+|---|-------|
+|MSE|0.11|
+|RMSE|0.34|
+|MAE|0.27|
+|R-Squared|0.74|
```

### Comparing `SmplML-1.0.2/SmplML.egg-info/PKG-INFO` & `SmplML-1.0.3/SmplML.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: SmplML
-Version: 1.0.2
-Summary: SmplML is a user-friendly Python library for streamlined machine learning classification. It offers intuitive modules for data preprocessing, feature engineering, model training, and evaluation. Ideal for beginners and experts alike, SmplML simplifies classification tasks, enabling you to gain valuable insights from your data with ease.
+Version: 1.0.3
+Summary: SmplML is a user-friendly Python library for streamlined machine learning classification. It offers intuitive functions for data preprocessing, model training, and evaluation of both classification and regression tasks. Ideal for beginners and experts alike, SmplML simplifies tasks, enabling you to gain valuable insights from your data with ease.
 Home-page: https://github.com/JhunBrian/SmplML
 Author: Jhun Brian Andam
-Author-email: brianandam123@gmail.com
+Author-email: andam.jhunbrian@gmail.com
 License: MIT
-Keywords: Machine Learning,Classification
+Keywords: Machine Learning,Classification,Regression
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -30,45 +30,79 @@
 - You can install SmpML using pip:
 ```shell
 pip install SimpleML
 ```
 
 ## Usage
 
+### Classification
 ```python
 import seaborn as sns
 import pandas as pd
-from smpl_ml.classification_helpers import TrainClassifier
+from smpl_ml.smpl_ml import TrainModel
+
 from sklearn.neighbors import KNeighborsClassifier
 
 # Load the dataset
 df = sns.load_dataset('penguins')
 
 # Set the target and features
 target = 'species'
 features = df.iloc[:, df.columns != target].columns
 
 # Create the classifier trainer
-trainer = TrainClassifier(df.dropna(), target=target, features=features, model=KNeighborsClassifier())
+clf_trainer = TrainModel(df.dropna(), target=target, features=features, model=KNeighborsClassifier())
 
 # Fit the model
-trainer.fit()
+clf_trainer.fit()
 
 # Evaluate the model
-model = trainer.evaluate()
+clf_model = clf_trainer.evaluate()
 ```
 
 `model` when `verbose` is set to `True` will return a DataFrame of classification metrics.
 
 
 |    | Recall | Specificity | Precision | F1-Score | Accuracy |
 |----|--------|-------------|-----------|----------|----------|
 | Adelie | 0.91   | 0.70        | 0.67      | 0.77     | 0.76     |
 | Chinstrap | 0.38   | 0.92        | 0.62      | 0.47     | 0.76     |
 | Gentoo | 0.86   | 1.00        | 1.00      | 0.92     | 0.76     |
 
+### Regression
+```python
+import seaborn as sns
+import pandas as pd
+from smpl_ml.smpl_ml import TrainModel
+
+from sklearn.neighbors import KNeighborsRegressor
+
+# Load the dataset
+df = sns.load_dataset('iris')
+
+# Set the target and features
+target = 'sepal_length'
+features = df.columns[1:]
+
+# Create the regressor trainer
+reg_trainer = TrainModel(df.dropna(), target=target, features=features, model=KNeighborsRegressor())
+
+# Fit the model
+reg_trainer.fit()
+
+# Evaluate the model
+reg_model = reg_trainer.evaluate()
+```
+
+|   |Metrics|
+|---|-------|
+|MSE|0.11|
+|RMSE|0.34|
+|MAE|0.27|
+|R-Squared|0.74|
+
 Change Log
 ==================
 
-1.0.2 (06/12/2023)
+1.0.3 (06/12/2023)
 ------------------
-Updated README.md
+Added Regression
```

### Comparing `SmplML-1.0.2/setup.py` & `SmplML-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,28 +11,28 @@
   'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Science/Research',
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
-desc = """SmplML is a user-friendly Python library for streamlined machine learning classification. It offers intuitive modules for data preprocessing, feature engineering, model training, and evaluation. Ideal for beginners and experts alike, SmplML simplifies classification tasks, enabling you to gain valuable insights from your data with ease."""
+desc = """SmplML is a user-friendly Python library for streamlined machine learning classification. It offers intuitive functions for data preprocessing, model training, and evaluation of both classification and regression tasks. Ideal for beginners and experts alike, SmplML simplifies tasks, enabling you to gain valuable insights from your data with ease."""
  
 dependencies = ['pandas', 
                 'numpy', 
                 'scikit-learn']
 
 setup(
   name='SmplML',
-  version='1.0.2',
+  version='1.0.3',
   description=desc,
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/JhunBrian/SmplML',  
   author='Jhun Brian Andam',
-  author_email='brianandam123@gmail.com',
+  author_email='andam.jhunbrian@gmail.com',
   license='MIT', 
   classifiers=classifiers,
-  keywords=['Machine Learning', 'Classification'], 
+  keywords=['Machine Learning', 'Classification', 'Regression'], 
   packages=find_packages(),
   install_requires=dependencies
 )
```

### Comparing `SmplML-1.0.2/smpl_ml/classification_helpers.py` & `SmplML-1.0.3/smpl_ml/smpl_ml.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,48 +9,49 @@
 
     def __str__(self):
         if self.suggestion:
             err = f"Variable '{self.variable_name}' is not initialized yet. {self.suggestion}"
         else:
             err = f"Variable '{self.variable_name}' is not initialized yet."
         return err
-    
+
+
 class Cat2Num:
     """
     Cat2Num: Categorical to Numerical
     """
-
     def __init__(self):
         self.dict_map = {}
-
-    def cat2num(self, df: pd.DataFrame) -> pd.DataFrame:
+        
+    def cat2num(self, df: pd.DataFrame):
         """
         Convert categorical columns in the DataFrame to numerical representation.
 
         Args:
             df (pd.DataFrame): The input DataFrame with categorical columns.
 
         Returns:
             pd.DataFrame: The DataFrame with categorical columns converted to numerical representation.
         """
         df = df.copy()
         for col in df:
+            
             if df[col].dtype == 'object' or df[col].dtype == 'category':
                 if df[col].dtype == 'category':
                     df[col] = df[col].astype('object')
-
+                    
                 self.dict_map[col] = {}
                 unique_values = df[col].unique()
                 for repl, orig in enumerate(unique_values):
                     self.dict_map[col][orig] = repl
                     df[col].replace(orig, repl, inplace=True)
-
+                    
         return df
-
-    def num2cat(self, df: pd.DataFrame) -> pd.DataFrame:
+    
+    def num2cat(self, df: pd.DataFrame):
         """
         Convert numerical representation of categorical columns back to their original values.
 
         Args:
             df (pd.DataFrame): The input DataFrame with numerical representation of categorical columns.
 
         Returns:
@@ -58,23 +59,24 @@
         
         Raises:
             VariableNotInitializedError: If `cat2num()` has not been executed before calling `num2cat()`.
         """
         df = df.copy()
         if self.dict_map == {}:
             raise VariableNotInitializedError("dict_map", suggestion="Try executing 'cat2num()' first.")
-
+            
         for col in df:
             if col in self.dict_map.keys():
                 for orig, repl in self.dict_map[col].items():
                     df[col].replace(repl, orig, inplace=True)
-
+                    
         return df
-    
-def split_data(df: pd.DataFrame, test_size: float = 0.25, shuffle: bool = True, random_state: int = 143) -> tuple:
+
+
+def split_data(df, test_size=0.25, shuffle=True, random_state=143):
     """
     Split the DataFrame into training and testing datasets.
 
     Args:
         df (pd.DataFrame): The input DataFrame to be split.
         test_size (float, optional): The proportion of the DataFrame to be used for testing. Defaults to 0.25.
         shuffle (bool, optional): Whether to shuffle the DataFrame before splitting. Defaults to True.
@@ -82,21 +84,47 @@
 
     Returns:
         tuple: A tuple containing the training and testing datasets.
 
     """
     if shuffle:
         df = df.sample(frac=1, random_state=random_state)
-
+    
     train = df[:-int(len(df) * test_size)]
     test = df[-int(len(df) * test_size):]
     return train, test
 
 
-def metrics(matrix: np.ndarray, class_labels: list) -> pd.DataFrame:
+def reg_metrics(y_true, y_pred):
+    """
+    Calculate performance metrics based on the provided y_true and y_pred.
+
+    Args:
+        y_true (np.ndarray): True data.
+        y_pred (np.ndarray): The rpedicted data.
+
+    Returns:
+        pd.DataFrame: A DataFrame containing performance metrics.
+
+    """
+    mse = np.mean((y_true - y_pred) ** 2)
+    rmse = np.sqrt(mse)
+    mae = np.mean(np.abs(y_true - y_pred))
+    r2 = 1 - (np.sum((y_true - y_pred) ** 2) / np.sum((y_true - np.mean(y_true)) ** 2))
+
+    dataframe = pd.DataFrame(data={'MSE': mse,
+                                   'RMSE': rmse,
+                                   'MAE': mae,
+                                   'R-squared': r2},
+                             index=['Metrics'])
+    
+    return dataframe.T
+
+
+def clf_metrics(matrix, class_labels):
     """
     Calculate performance metrics based on the confusion matrix.
 
     Args:
         matrix (np.ndarray): The confusion matrix.
         class_labels (list): The list of class labels.
 
@@ -123,17 +151,17 @@
                                    'Precision': PPV,
                                    'F1-Score': F1},
                              index=class_labels)
     dataframe.fillna(value=0, inplace=True)
     dataframe['Accuracy'] = np.round(np.sum(TP) / np.sum(matrix), 2)
     return dataframe
 
-class TrainClassifier:
-    def __init__(self, df, target, features, model, test_size=0.25, random_state=143, shuffle=True):
 
+class TrainModel:
+    def __init__(self, df: pd.DataFrame, target: str, features: list, model, test_size=0.25, random_state=143, shuffle=True):
         """
         Initialize the TrainClassifier object.
 
         Args:
             df (pd.DataFrame): The input DataFrame containing the data.
             target (str): The name of the target variable column.
             features (list): The list of feature columns.
@@ -146,22 +174,23 @@
         self.__target = target
         self.__features = features
         self.__model = model
         self.__test_size = test_size
         self.__random_state = random_state
         self.__shuffle = shuffle
         
-        self.__train = None
-        self.__test = None
-        self.__split_data = split_data
         self.__lbl_encoder = Cat2Num()
         self.__split_data = split_data
-        self.__confusion_matrix = confusion_matrix
-        self.__metrics = metrics
-        self.__clf = None
+        self.__reg_metrics = reg_metrics
+        self.__clf_metrics = clf_metrics
+        self.__conf_matrix = confusion_matrix
+        self.__type = None
+        self.__train = None
+        self.__test = None
+        self.__fitted_model = None
         
     def fit(self, verbose=True):
         """
         Fit the machine learning model using the training data.
 
         Args:
             verbose (bool, optional): Whether to display performance metrics. Defaults to True.
@@ -169,45 +198,58 @@
         data = self.__lbl_encoder.cat2num(self.__df)
         train, test = self.__split_data(df=data, 
                                         test_size=self.__test_size, 
                                         shuffle=self.__shuffle, 
                                         random_state=self.__random_state)
         
         X_train, y_train = train[self.__features], train[self.__target]
-        clf = self.__model.fit(X=X_train, y=y_train)
+        model_ = self.__model.fit(X=X_train, y=y_train)
+        y_pred = model_.predict(X_train)
         
-        if verbose:
-            y_pred = clf.predict(X_train)
-            matrix = self.__confusion_matrix(y_train, y_pred)
-            report_df = self.__metrics(matrix, self.__lbl_encoder.dict_map[self.__target].keys())
-            display(report_df)
-                    
+        if self.__df[self.__target].dtype == 'float64':
+            self.__type = 'regression'
+            if verbose:
+                report_df = self.__reg_metrics(y_train, y_pred)
+                display(report_df)
+                
+        else:
+            self.__type = 'classification'
+            if verbose:
+                matrix = self.__conf_matrix(y_train, y_pred)
+                report_df = self.__clf_metrics(matrix, self.__lbl_encoder.dict_map[self.__target].keys())
+                display(report_df)
+            
+        self.__fitted_model = model_
         self.__train = train
         self.__test = test
-        self.__clf = clf
-        
+            
     def evaluate(self, verbose=True):
         """
         Evaluate the trained machine learning model using the test data.
 
         Args:
             verbose (bool, optional): Whether to display performance metrics. Defaults to True.
 
         Returns:
             trained_model: The trained machine learning model.
 
         Raises:
             VariableNotInitializedError: If `fit()` has not been executed before calling `evaluate()`.
         """
-        if self.__clf == None:
+        if self.__fitted_model == None:
             raise VariableNotInitializedError("model", suggestion="Try fitting it first using `fit()` method.")
-            
-        X_test = self.__test[self.__features]
-        y_test = self.__test[self.__target]
-        
-        if verbose:
-            y_pred = self.__clf.predict(X_test)
-            matrix = self.__confusion_matrix(y_test, y_pred)
-            report_df = self.__metrics(matrix, self.__lbl_encoder.dict_map[self.__target].keys())
-            display(report_df)
+
+        X_test, y_test = self.__test[self.__features], self.__test[self.__target]
+        y_pred = self.__fitted_model.predict(X_test)
         
-        return self.__clf
+        if self.__type == 'regression':
+            if verbose:
+                report_df = self.__reg_metrics(y_test, y_pred)
+                display(report_df)
+                
+        elif self.__type == 'classification':
+            if verbose:
+                matrix = self.__conf_matrix(y_test, y_pred)
+                report_df = self.__clf_metrics(matrix, self.__lbl_encoder.dict_map[self.__target].keys())
+                display(report_df)
+                
+        return self.__fitted_model
```

