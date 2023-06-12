# Comparing `tmp/MLandPattern-0.2.0.tar.gz` & `tmp/MLandPattern-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLandPattern-0.2.0.tar", last modified: Mon May  8 07:11:29 2023, max compression
+gzip compressed data, was "MLandPattern-0.2.1.tar", last modified: Mon Jun 12 15:36:54 2023, max compression
```

## Comparing `MLandPattern-0.2.0.tar` & `MLandPattern-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-05-08 07:11:29.403112 MLandPattern-0.2.0/
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-05-08 07:11:29.396637 MLandPattern-0.2.0/MLandPattern/
--rw-r--r--   0 pablomunoz   (501) staff       (20)    21860 2023-05-08 07:10:03.000000 MLandPattern-0.2.0/MLandPattern/MLandPattern.py
--rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.2.0/MLandPattern/__init__.py
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-05-08 07:11:29.400802 MLandPattern-0.2.0/MLandPattern.egg-info/
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-05-08 07:11:29.000000 MLandPattern-0.2.0/MLandPattern.egg-info/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-05-08 07:11:29.000000 MLandPattern-0.2.0/MLandPattern.egg-info/SOURCES.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-05-08 07:11:29.000000 MLandPattern-0.2.0/MLandPattern.egg-info/dependency_links.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-05-08 07:11:29.000000 MLandPattern-0.2.0/MLandPattern.egg-info/top_level.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-05-08 07:11:29.402303 MLandPattern-0.2.0/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.2.0/README.md
--rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-05-08 07:11:29.403473 MLandPattern-0.2.0/setup.cfg
--rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-05-08 07:10:11.000000 MLandPattern-0.2.0/setup.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-12 15:36:54.969108 MLandPattern-0.2.1/
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-12 15:36:54.963367 MLandPattern-0.2.1/MLandPattern/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)    21914 2023-06-12 15:34:46.000000 MLandPattern-0.2.1/MLandPattern/MLandPattern.py
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.2.1/MLandPattern/__init__.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-12 15:36:54.967072 MLandPattern-0.2.1/MLandPattern.egg-info/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-12 15:36:54.000000 MLandPattern-0.2.1/MLandPattern.egg-info/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-06-12 15:36:54.000000 MLandPattern-0.2.1/MLandPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-06-12 15:36:54.000000 MLandPattern-0.2.1/MLandPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-06-12 15:36:54.000000 MLandPattern-0.2.1/MLandPattern.egg-info/top_level.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-12 15:36:54.968780 MLandPattern-0.2.1/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.2.1/README.md
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-06-12 15:36:54.969255 MLandPattern-0.2.1/setup.cfg
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-06-12 15:34:54.000000 MLandPattern-0.2.1/setup.py
```

### Comparing `MLandPattern-0.2.0/MLandPattern/MLandPattern.py` & `MLandPattern-0.2.1/MLandPattern/MLandPattern.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,16 +294,17 @@
     """
     Calculates the model of the MultiVariate Gaussian classifier for a set of data, and applyes it to a test dataset
     :param train_date: matrix of the datapoints of a dataset used to train the model
     :param train_labels: row vector with the labels associated with each row of the training dataset
     :param test_data: matrix of the datapoints of a dataset used to test the model
     :param test_labels: row vector with the labels associated with each row of the test dataset
     :param prior_probability: col vector associated with the prior probability for each dimension
-    :return SPost: matrix associated with the class posterior probabilty associated with each class
+    :return S: matrix associated with the probability array
     :return predictions: Vector associated with the prediction of the class for each test data point
+    :return acc: Accuracy of the validation set
     """
     class_labels = np.unique(train_labels)
     cov = multiclass_covariance(train_data, train_labels)
     # print(cov[0])
     multi_mu = multiclass_mean(train_data, train_labels)
     # print(multi_mu[0])
     densities = []
@@ -321,27 +322,28 @@
             if predictions[i] == test_label[i]:
                 acc += 1
         acc/=len(test_label)
         acc = round(acc*100, 2)
         print(f'Accuracy: {acc}%')
         print(f'Error: {(100 - acc)}%')
 
-    return SPost, predictions
+    return S, predictions, acc
 
 
 def MVG_log_classifier(train_data, train_labels, test_data, prior_probability, test_label=[]):
     """
     Calculates the model of the MultiVariate Gaussian classifier on the logarithm dimension for a set of data, and applyes it to a test dataset
     :param train_date: matrix of the datapoints of a dataset used to train the model
     :param train_labels: row vector with the labels associated with each row of the training dataset
     :param test_data: matrix of the datapoints of a dataset used to test the model
     :param test_labels: row vector with the labels associated with each row of the test dataset
     :param prior_probability: col vector associated with the prior probability for each dimension
-    :return SPost: matrix associated with the class posterior probabilty associated with each class
+    :return S: matrix associated with the probability array
     :return predictions: Vector associated with the prediction of the class for each test data point
+    :return acc: Accuracy of the validation set
     """
     class_labels = np.unique(train_labels)
     cov = multiclass_covariance(train_data, train_labels)
     # print(cov[0])
     multi_mu = multiclass_mean(train_data, train_labels)
     # print(multi_mu[0])
     densities = []
@@ -360,27 +362,28 @@
             if predictions[i] == test_label[i]:
                 acc += 1
         acc/=len(test_label)
         acc = round(acc*100, 2)
         print(f'Accuracy: {acc}%')
         print(f'Error: {(100 - acc)}%')
 
-    return SPost, predictions
+    return S, predictions, acc
 
 
 def Naive_classifier(train_data, train_labels, test_data, prior_probability, test_label=[]):
     """
     Calculates the model of the Naive classifier for a set of data, and applyes it to a test dataset
     :param train_date: matrix of the datapoints of a dataset used to train the model
     :param train_labels: row vector with the labels associated with each row of the training dataset
     :param test_data: matrix of the datapoints of a dataset used to test the model
     :param test_labels: row vector with the labels associated with each row of the test dataset
     :param prior_probability: col vector associated with the prior probability for each dimension
-    :return SPost: matrix associated with the class posterior probabilty associated with each class
+    :return S: matrix associated with the probability array
     :return predictions: Vector associated with the prediction of the class for each test data point
+    :return acc: Accuracy of the validation set
     """
     class_labels = np.unique(train_labels)
     cov = multiclass_covariance(train_data, train_labels)
     identity = np.eye(cov.shape[1])
     # print(identity)
     cov = cov*identity
     multi_mu = multiclass_mean(train_data, train_labels)
@@ -400,27 +403,28 @@
             if predictions[i] == test_label[i]:
                 acc += 1
         acc/=len(test_label)
         acc = round(acc*100, 2)
         print(f'Accuracy: {acc}%')
         print(f'Error: {(100 - acc)}%')
 
-    return SPost, predictions
+    return S, predictions, acc
 
 
 def Naive_log_classifier(train_data, train_labels, test_data, prior_probability, test_label=[]):
     """
     Calculates the model of the Naive classifier on the logarithm realm for a set of data, and applyes it to a test dataset
     :param train_date: matrix of the datapoints of a dataset used to train the model
     :param train_labels: row vector with the labels associated with each row of the training dataset
     :param test_data: matrix of the datapoints of a dataset used to test the model
     :param test_labels: row vector with the labels associated with each row of the test dataset
     :param prior_probability: col vector associated with the prior probability for each dimension
-    :return SPost: matrix associated with the class posterior probabilty associated with each class
+    :return S: matrix associated with the probability array
     :return predictions: Vector associated with the prediction of the class for each test data point
+    :return acc: Accuracy of the validation set
     """
     class_labels = np.unique(train_labels)
     cov = multiclass_covariance(train_data, train_labels)
     identity = np.eye(cov.shape[1])
     # print(identity)
     cov = cov*identity
     multi_mu = multiclass_mean(train_data, train_labels)
@@ -441,27 +445,28 @@
             if predictions[i] == test_label[i]:
                 acc += 1
         acc/=len(test_label)
         acc = round(acc*100, 2)
         print(f'Accuracy: {acc}%')
         print(f'Error: {(100 - acc)}%')
 
-    return SPost, predictions
+    return S, predictions, acc
 
 
 def TiedGaussian(train_data, train_labels, test_data, prior_probability, test_label=[]):
     '''
     Calculates the model of the Tied Gaussian classifier for a set of data, and applyes it to a test dataset
     :param train_date: matrix of the datapoints of a dataset used to train the model
     :param train_labels: row vector with the labels associated with each row of the training dataset
     :param test_data: matrix of the datapoints of a dataset used to test the model
     :param test_labels: row vector with the labels associated with each row of the test dataset
     :param prior_probability: col vector associated with the prior probability for each dimension
-    :return SPost: matrix associated with the class posterior probabilty associated with each class
+    :return S: matrix associated with the probability array
     :return predictions: Vector associated with the prediction of the class for each test data point
+    :return acc: Accuracy of the validation set
     '''
     class_labels = np.unique(train_labels)
     with_cov = covariance_within_class(train_data, train_labels)
     multi_mu = multiclass_mean(train_data, train_labels)
     densities = []
     for i in range(class_labels.size):
         densities.append(
@@ -479,28 +484,29 @@
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
         acc /= len(test_label)
         print(f"Accuracy: {acc}")
         print(f"Error: {1 - acc}")
 
-    return SPost, predictions
+    return S, predictions, acc
 
 def Tied_Naive_classifier(
     train_data, train_labels, test_data, prior_probability, test_label=[]
 ):
     '''
     Calculates the model of the Tied Naive classifier for a set of data, and applyes it to a test dataset
     :param train_date: matrix of the datapoints of a dataset used to train the model
     :param train_labels: row vector with the labels associated with each row of the training dataset
     :param test_data: matrix of the datapoints of a dataset used to test the model
     :param test_labels: row vector with the labels associated with each row of the test dataset
     :param prior_probability: col vector associated with the prior probability for each dimension
-    :return SPost: matrix associated with the class posterior probabilty associated with each class
+    :return S: matrix associated with the probability array
     :return predictions: Vector associated with the prediction of the class for each test data point
+    :return acc: Accuracy of the validation set
     '''
     class_labels = np.unique(train_labels)
     cov = covariance_within_class(train_data, train_labels)
     identity = np.eye(cov.shape[1])
     cov = cov * identity
     multi_mu = multiclass_mean(train_data, train_labels)
     densities = []
@@ -519,15 +525,15 @@
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
         acc /= len(test_label)
         print(f"Accuracy: {acc*100}%")
         print(f"Error: {(1 - acc)*100}%")
 
-    return SPost, predictions
+    return S, predictions, acc
 
 
 
 def split_db(D, L, ratio, seed=0):
     '''
     Splits a dataset D into a training set and a validation set, based on the ratio
     :param D: matrix of attributes of the dataset
```

