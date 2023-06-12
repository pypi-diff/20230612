# Comparing `tmp/SmplML-1.0.3.tar.gz` & `tmp/SmplML-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SmplML-1.0.3.tar", last modified: Mon Jun 12 07:40:45 2023, max compression
+gzip compressed data, was "dist\SmplML-1.0.4.tar", last modified: Mon Jun 12 08:09:49 2023, max compression
```

## Comparing `SmplML-1.0.3.tar` & `SmplML-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 07:40:45.099145 SmplML-1.0.3/
--rw-rw-rw-   0        0        0       90 2023-06-12 07:39:23.000000 SmplML-1.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1086 2023-06-12 07:39:21.000000 SmplML-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       30 2023-06-12 07:39:19.000000 SmplML-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3432 2023-06-12 07:40:45.097150 SmplML-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2398 2023-06-12 07:39:17.000000 SmplML-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 07:40:45.086819 SmplML-1.0.3/SmplML.egg-info/
--rw-rw-rw-   0        0        0     3432 2023-06-12 07:40:44.000000 SmplML-1.0.3/SmplML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-06-12 07:40:44.000000 SmplML-1.0.3/SmplML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 07:40:44.000000 SmplML-1.0.3/SmplML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-12 07:40:44.000000 SmplML-1.0.3/SmplML.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 07:40:44.000000 SmplML-1.0.3/SmplML.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 07:40:45.099145 SmplML-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1459 2023-06-12 07:33:16.000000 SmplML-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:40:45.093549 SmplML-1.0.3/smpl_ml/
--rw-rw-rw-   0        0        0       46 2023-06-12 03:44:49.000000 SmplML-1.0.3/smpl_ml/__init__.py
--rw-rw-rw-   0        0        0     9514 2023-06-12 07:39:41.000000 SmplML-1.0.3/smpl_ml/smpl_ml.py
+drwxrwxrwx   0        0        0        0 2023-06-12 08:09:49.140933 SmplML-1.0.4/
+-rw-rw-rw-   0        0        0       90 2023-06-12 08:08:56.000000 SmplML-1.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1086 2023-06-12 07:39:21.000000 SmplML-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-06-12 07:39:19.000000 SmplML-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3868 2023-06-12 08:09:49.139599 SmplML-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2857 2023-06-12 08:09:31.000000 SmplML-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 08:09:49.131367 SmplML-1.0.4/SmplML.egg-info/
+-rw-rw-rw-   0        0        0     3868 2023-06-12 08:09:48.000000 SmplML-1.0.4/SmplML.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-06-12 08:09:48.000000 SmplML-1.0.4/SmplML.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 08:09:48.000000 SmplML-1.0.4/SmplML.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-12 08:09:48.000000 SmplML-1.0.4/SmplML.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 08:09:48.000000 SmplML-1.0.4/SmplML.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 08:09:49.141936 SmplML-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1436 2023-06-12 08:08:47.000000 SmplML-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 08:09:49.137083 SmplML-1.0.4/smpl_ml/
+-rw-rw-rw-   0        0        0       46 2023-06-12 03:44:49.000000 SmplML-1.0.4/smpl_ml/__init__.py
+-rw-rw-rw-   0        0        0     9514 2023-06-12 08:09:04.000000 SmplML-1.0.4/smpl_ml/smpl_ml.py
```

### Comparing `SmplML-1.0.3/LICENSE` & `SmplML-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SmplML-1.0.3/PKG-INFO` & `SmplML-1.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: SmplML
-Version: 1.0.3
-Summary: SmplML is a user-friendly Python library for streamlined machine learning classification. It offers intuitive functions for data preprocessing, model training, and evaluation of both classification and regression tasks. Ideal for beginners and experts alike, SmplML simplifies tasks, enabling you to gain valuable insights from your data with ease.
+Version: 1.0.4
+Summary: SmplML is a user-friendly Python module for streamlined machine learning classification and regression. It offers intuitive functionality for data preprocessing, model training, and evaluation. Ideal for beginners and experts alike, SmplML simplifies ML tasks, enabling you to gain valuable insights from your data with ease.
 Home-page: https://github.com/JhunBrian/SmplML
 Author: Jhun Brian Andam
 Author-email: andam.jhunbrian@gmail.com
 License: MIT
 Keywords: Machine Learning,Classification,Regression
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# SmplML / SimpleML: Simplified Machine Learning for Classification
+# SmplML / SimpleML: Simplified Machine Learning for Classification and Regression
 
-SmplML is a user-friendly Python library for streamlined machine learning classification. It offers intuitive modules for data preprocessing, model training, and evaluation. Ideal for beginners and experts alike, EasyML simplifies classification tasks, enabling you to gain valuable insights from your data with ease.
+SmplML is a user-friendly Python module for streamlined machine learning classification and regression. It offers intuitive functionality for data preprocessing, model training, and evaluation. Ideal for beginners and experts alike, SmplML simplifies ML tasks, enabling you to gain valuable insights from your data with ease.
 
 ## Features
 
 - Data preprocessing: Easily handle encoding categorical variables.
-- Model training: Train various classification models with just a few lines of code.
+- Model training: Train various classification and regression models with just a few lines of code.
 - Model evaluation: Evaluate model performance using common metrics and visualizations.
+- This module is designed to seamlessly handle various scikit-learn models, making it flexible for handling sklearn-like model formats.
 
 ## Installation
 
 - You can install SmpML using pip:
 ```shell
 pip install SimpleML
 ```
 
 ## Usage
+The `TrainModel` class is designed to handle both classification and regression tasks. It determines the task type based on the `target` parameter. If the `target` has a `float` data type, the class automatically redirects the procedures to regression; otherwise, it assumes a classification task.
 
 ### Classification
 ```python
 import seaborn as sns
 import pandas as pd
 from smpl_ml.smpl_ml import TrainModel
 
@@ -55,15 +57,15 @@
 # Fit the model
 clf_trainer.fit()
 
 # Evaluate the model
 clf_model = clf_trainer.evaluate()
 ```
 
-`model` when `verbose` is set to `True` will return a DataFrame of classification metrics.
+`model` when `verbose` is set to `True` will return a DataFrame of metrics.
 
 
 |    | Recall | Specificity | Precision | F1-Score | Accuracy |
 |----|--------|-------------|-----------|----------|----------|
 | Adelie | 0.91   | 0.70        | 0.67      | 0.77     | 0.76     |
 | Chinstrap | 0.38   | 0.92        | 0.62      | 0.47     | 0.76     |
 | Gentoo | 0.86   | 1.00        | 1.00      | 0.92     | 0.76     |
@@ -99,10 +101,10 @@
 |RMSE|0.34|
 |MAE|0.27|
 |R-Squared|0.74|
 
 Change Log
 ==================
 
-1.0.3 (06/12/2023)
+1.0.4 (06/12/2023)
 ------------------
 Added Regression
```

### Comparing `SmplML-1.0.3/README.md` & `SmplML-1.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-# SmplML / SimpleML: Simplified Machine Learning for Classification
+# SmplML / SimpleML: Simplified Machine Learning for Classification and Regression
 
-SmplML is a user-friendly Python library for streamlined machine learning classification. It offers intuitive modules for data preprocessing, model training, and evaluation. Ideal for beginners and experts alike, EasyML simplifies classification tasks, enabling you to gain valuable insights from your data with ease.
+SmplML is a user-friendly Python module for streamlined machine learning classification and regression. It offers intuitive functionality for data preprocessing, model training, and evaluation. Ideal for beginners and experts alike, SmplML simplifies ML tasks, enabling you to gain valuable insights from your data with ease.
 
 ## Features
 
 - Data preprocessing: Easily handle encoding categorical variables.
-- Model training: Train various classification models with just a few lines of code.
+- Model training: Train various classification and regression models with just a few lines of code.
 - Model evaluation: Evaluate model performance using common metrics and visualizations.
+- This module is designed to seamlessly handle various scikit-learn models, making it flexible for handling sklearn-like model formats.
 
 ## Installation
 
 - You can install SmpML using pip:
 ```shell
 pip install SimpleML
 ```
 
 ## Usage
+The `TrainModel` class is designed to handle both classification and regression tasks. It determines the task type based on the `target` parameter. If the `target` has a `float` data type, the class automatically redirects the procedures to regression; otherwise, it assumes a classification task.
 
 ### Classification
 ```python
 import seaborn as sns
 import pandas as pd
 from smpl_ml.smpl_ml import TrainModel
 
@@ -38,15 +40,15 @@
 # Fit the model
 clf_trainer.fit()
 
 # Evaluate the model
 clf_model = clf_trainer.evaluate()
 ```
 
-`model` when `verbose` is set to `True` will return a DataFrame of classification metrics.
+`model` when `verbose` is set to `True` will return a DataFrame of metrics.
 
 
 |    | Recall | Specificity | Precision | F1-Score | Accuracy |
 |----|--------|-------------|-----------|----------|----------|
 | Adelie | 0.91   | 0.70        | 0.67      | 0.77     | 0.76     |
 | Chinstrap | 0.38   | 0.92        | 0.62      | 0.47     | 0.76     |
 | Gentoo | 0.86   | 1.00        | 1.00      | 0.92     | 0.76     |
```

### Comparing `SmplML-1.0.3/SmplML.egg-info/PKG-INFO` & `SmplML-1.0.4/SmplML.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: SmplML
-Version: 1.0.3
-Summary: SmplML is a user-friendly Python library for streamlined machine learning classification. It offers intuitive functions for data preprocessing, model training, and evaluation of both classification and regression tasks. Ideal for beginners and experts alike, SmplML simplifies tasks, enabling you to gain valuable insights from your data with ease.
+Version: 1.0.4
+Summary: SmplML is a user-friendly Python module for streamlined machine learning classification and regression. It offers intuitive functionality for data preprocessing, model training, and evaluation. Ideal for beginners and experts alike, SmplML simplifies ML tasks, enabling you to gain valuable insights from your data with ease.
 Home-page: https://github.com/JhunBrian/SmplML
 Author: Jhun Brian Andam
 Author-email: andam.jhunbrian@gmail.com
 License: MIT
 Keywords: Machine Learning,Classification,Regression
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# SmplML / SimpleML: Simplified Machine Learning for Classification
+# SmplML / SimpleML: Simplified Machine Learning for Classification and Regression
 
-SmplML is a user-friendly Python library for streamlined machine learning classification. It offers intuitive modules for data preprocessing, model training, and evaluation. Ideal for beginners and experts alike, EasyML simplifies classification tasks, enabling you to gain valuable insights from your data with ease.
+SmplML is a user-friendly Python module for streamlined machine learning classification and regression. It offers intuitive functionality for data preprocessing, model training, and evaluation. Ideal for beginners and experts alike, SmplML simplifies ML tasks, enabling you to gain valuable insights from your data with ease.
 
 ## Features
 
 - Data preprocessing: Easily handle encoding categorical variables.
-- Model training: Train various classification models with just a few lines of code.
+- Model training: Train various classification and regression models with just a few lines of code.
 - Model evaluation: Evaluate model performance using common metrics and visualizations.
+- This module is designed to seamlessly handle various scikit-learn models, making it flexible for handling sklearn-like model formats.
 
 ## Installation
 
 - You can install SmpML using pip:
 ```shell
 pip install SimpleML
 ```
 
 ## Usage
+The `TrainModel` class is designed to handle both classification and regression tasks. It determines the task type based on the `target` parameter. If the `target` has a `float` data type, the class automatically redirects the procedures to regression; otherwise, it assumes a classification task.
 
 ### Classification
 ```python
 import seaborn as sns
 import pandas as pd
 from smpl_ml.smpl_ml import TrainModel
 
@@ -55,15 +57,15 @@
 # Fit the model
 clf_trainer.fit()
 
 # Evaluate the model
 clf_model = clf_trainer.evaluate()
 ```
 
-`model` when `verbose` is set to `True` will return a DataFrame of classification metrics.
+`model` when `verbose` is set to `True` will return a DataFrame of metrics.
 
 
 |    | Recall | Specificity | Precision | F1-Score | Accuracy |
 |----|--------|-------------|-----------|----------|----------|
 | Adelie | 0.91   | 0.70        | 0.67      | 0.77     | 0.76     |
 | Chinstrap | 0.38   | 0.92        | 0.62      | 0.47     | 0.76     |
 | Gentoo | 0.86   | 1.00        | 1.00      | 0.92     | 0.76     |
@@ -99,10 +101,10 @@
 |RMSE|0.34|
 |MAE|0.27|
 |R-Squared|0.74|
 
 Change Log
 ==================
 
-1.0.3 (06/12/2023)
+1.0.4 (06/12/2023)
 ------------------
 Added Regression
```

### Comparing `SmplML-1.0.3/setup.py` & `SmplML-1.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,23 @@
   'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Science/Research',
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
-desc = """SmplML is a user-friendly Python library for streamlined machine learning classification. It offers intuitive functions for data preprocessing, model training, and evaluation of both classification and regression tasks. Ideal for beginners and experts alike, SmplML simplifies tasks, enabling you to gain valuable insights from your data with ease."""
+desc = """SmplML is a user-friendly Python module for streamlined machine learning classification and regression. It offers intuitive functionality for data preprocessing, model training, and evaluation. Ideal for beginners and experts alike, SmplML simplifies ML tasks, enabling you to gain valuable insights from your data with ease."""
  
 dependencies = ['pandas', 
                 'numpy', 
                 'scikit-learn']
 
 setup(
   name='SmplML',
-  version='1.0.3',
+  version='1.0.4',
   description=desc,
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/JhunBrian/SmplML',  
   author='Jhun Brian Andam',
   author_email='andam.jhunbrian@gmail.com',
   license='MIT',
```

### Comparing `SmplML-1.0.3/smpl_ml/smpl_ml.py` & `SmplML-1.0.4/smpl_ml/smpl_ml.py`

 * *Files identical despite different names*

