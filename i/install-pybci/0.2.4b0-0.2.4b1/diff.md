# Comparing `tmp/install-pybci-0.2.4b0.tar.gz` & `tmp/install-pybci-0.2.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-pybci-0.2.4b0.tar", last modified: Mon Jun  5 17:51:32 2023, max compression
+gzip compressed data, was "install-pybci-0.2.4b1.tar", last modified: Mon Jun 12 20:20:57 2023, max compression
```

## Comparing `install-pybci-0.2.4b0.tar` & `install-pybci-0.2.4b1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:51:32.729608 install-pybci-0.2.4b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-06-05 17:51:32.729608 install-pybci-0.2.4b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:51:32.725608 install-pybci-0.2.4b0/install_pybci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-06-05 17:51:32.000000 install-pybci-0.2.4b0/install_pybci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-05 17:51:32.000000 install-pybci-0.2.4b0/install_pybci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:51:32.000000 install-pybci-0.2.4b0/install_pybci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-05 17:51:32.000000 install-pybci-0.2.4b0/install_pybci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 17:51:32.000000 install-pybci-0.2.4b0/install_pybci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:51:32.725608 install-pybci-0.2.4b0/pybci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:51:32.725608 install-pybci-0.2.4b0/pybci/Configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/Configuration/EpochSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/Configuration/FeatureSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:51:32.729608 install-pybci-0.2.4b0/pybci/ThreadClasses/
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/ThreadClasses/AsyncDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/ThreadClasses/ClassifierThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/ThreadClasses/DataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/ThreadClasses/FeatureProcessorThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/ThreadClasses/MarkerThread.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/ThreadClasses/OptimisedDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/ThreadClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:51:32.729608 install-pybci-0.2.4b0/pybci/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/Utils/Classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/Utils/FeatureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/Utils/LSLScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/Utils/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19917 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/pybci.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/pybci/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:51:32.729608 install-pybci-0.2.4b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-05 17:51:03.000000 install-pybci-0.2.4b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:20:57.895265 install-pybci-0.2.4b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-06-12 20:20:57.895265 install-pybci-0.2.4b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:20:57.895265 install-pybci-0.2.4b1/install_pybci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-06-12 20:20:57.000000 install-pybci-0.2.4b1/install_pybci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-12 20:20:57.000000 install-pybci-0.2.4b1/install_pybci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:20:57.000000 install-pybci-0.2.4b1/install_pybci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 20:20:57.000000 install-pybci-0.2.4b1/install_pybci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 20:20:57.000000 install-pybci-0.2.4b1/install_pybci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:20:57.895265 install-pybci-0.2.4b1/pybci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:20:57.895265 install-pybci-0.2.4b1/pybci/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/Configuration/EpochSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/Configuration/FeatureSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:20:57.895265 install-pybci-0.2.4b1/pybci/ThreadClasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/ThreadClasses/AsyncDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/ThreadClasses/ClassifierThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/ThreadClasses/DataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/ThreadClasses/FeatureProcessorThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/ThreadClasses/MarkerThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/ThreadClasses/OptimisedDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/ThreadClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:20:57.895265 install-pybci-0.2.4b1/pybci/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/Utils/Classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/Utils/FeatureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/Utils/LSLScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/Utils/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/pybci.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 20:20:57.895265 install-pybci-0.2.4b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/setup.py
```

### Comparing `install-pybci-0.2.4b0/LICENSE` & `install-pybci-0.2.4b1/LICENSE`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b0/PKG-INFO` & `install-pybci-0.2.4b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.2.4b0
+Version: 0.2.4b1
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
@@ -41,15 +41,15 @@
 
 [Examples of supported LSL hardware here!](https://labstreaminglayer.readthedocs.io/info/supported_devices.html)
 
 ## Basic implementation
 ```python
 import time
 from pybci import PyBCI
-bci = PyBCI() # set default epoch timing, looks for first available lsl stream and all data streams
+bci = PyBCI() # set default epoch timing, looks for first available lsl marker stream and all data streams
 bci.TrainMode() # assume both marker and datastreams available to start training on received epochs
 accuracy = 0
 try:
     while(True): # training based on couple epochs more then min threshold for classifying
         currentMarkers = bci.ReceivedMarkerCount() # check to see how many received epochs, if markers sent to close together will be ignored till done processing
         time.sleep(1) # wait for marker updates
         print("Markers received: " + str(currentMarkers) +" Class accuracy: " + str(accuracy), end="\r")
@@ -75,14 +75,15 @@
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy, is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
 - Update ReadTheDocs!
 - Finish arduino hand grasp demo and video.
+- Tst and likely Fix multimodal after new data thread creation
 - ~~Combine multiple data streams for multi modal bci!~~
 - ~~Add pytorch compatibility!~~ 
 - ~~run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo])~~
 - ~~Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.~~ (Added universal optimised thread to handle all cases)
 - ~~Levels of print debug (info, error, none)~~
 - ~~Retrieve feature data~~
```

### Comparing `install-pybci-0.2.4b0/README.md` & `install-pybci-0.2.4b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 [Examples of supported LSL hardware here!](https://labstreaminglayer.readthedocs.io/info/supported_devices.html)
 
 ## Basic implementation
 ```python
 import time
 from pybci import PyBCI
-bci = PyBCI() # set default epoch timing, looks for first available lsl stream and all data streams
+bci = PyBCI() # set default epoch timing, looks for first available lsl marker stream and all data streams
 bci.TrainMode() # assume both marker and datastreams available to start training on received epochs
 accuracy = 0
 try:
     while(True): # training based on couple epochs more then min threshold for classifying
         currentMarkers = bci.ReceivedMarkerCount() # check to see how many received epochs, if markers sent to close together will be ignored till done processing
         time.sleep(1) # wait for marker updates
         print("Markers received: " + str(currentMarkers) +" Class accuracy: " + str(accuracy), end="\r")
@@ -51,14 +51,15 @@
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy, is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
 - Update ReadTheDocs!
 - Finish arduino hand grasp demo and video.
+- Tst and likely Fix multimodal after new data thread creation
 - ~~Combine multiple data streams for multi modal bci!~~
 - ~~Add pytorch compatibility!~~ 
 - ~~run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo])~~
 - ~~Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.~~ (Added universal optimised thread to handle all cases)
 - ~~Levels of print debug (info, error, none)~~
 - ~~Retrieve feature data~~
```

### Comparing `install-pybci-0.2.4b0/install_pybci.egg-info/PKG-INFO` & `install-pybci-0.2.4b1/install_pybci.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.2.4b0
+Version: 0.2.4b1
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
@@ -41,15 +41,15 @@
 
 [Examples of supported LSL hardware here!](https://labstreaminglayer.readthedocs.io/info/supported_devices.html)
 
 ## Basic implementation
 ```python
 import time
 from pybci import PyBCI
-bci = PyBCI() # set default epoch timing, looks for first available lsl stream and all data streams
+bci = PyBCI() # set default epoch timing, looks for first available lsl marker stream and all data streams
 bci.TrainMode() # assume both marker and datastreams available to start training on received epochs
 accuracy = 0
 try:
     while(True): # training based on couple epochs more then min threshold for classifying
         currentMarkers = bci.ReceivedMarkerCount() # check to see how many received epochs, if markers sent to close together will be ignored till done processing
         time.sleep(1) # wait for marker updates
         print("Markers received: " + str(currentMarkers) +" Class accuracy: " + str(accuracy), end="\r")
@@ -75,14 +75,15 @@
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy, is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
 - Update ReadTheDocs!
 - Finish arduino hand grasp demo and video.
+- Tst and likely Fix multimodal after new data thread creation
 - ~~Combine multiple data streams for multi modal bci!~~
 - ~~Add pytorch compatibility!~~ 
 - ~~run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo])~~
 - ~~Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.~~ (Added universal optimised thread to handle all cases)
 - ~~Levels of print debug (info, error, none)~~
 - ~~Retrieve feature data~~
```

### Comparing `install-pybci-0.2.4b0/install_pybci.egg-info/SOURCES.txt` & `install-pybci-0.2.4b1/install_pybci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b0/pybci/Configuration/EpochSettings.py` & `install-pybci-0.2.4b1/pybci/Configuration/EpochSettings.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b0/pybci/ThreadClasses/AsyncDataReceiverThread.py` & `install-pybci-0.2.4b1/pybci/ThreadClasses/AsyncDataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b0/pybci/ThreadClasses/ClassifierThread.py` & `install-pybci-0.2.4b1/pybci/ThreadClasses/ClassifierThread.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 
 class ClassifierThread(threading.Thread):
     features = np.array([])#[]
     targets = np.array([])
     mode = "train"
     guess = " "
-    epochCounts = {} 
+    epochCountsc = {} 
     def __init__(self, closeEvent,trainTestEvent, featureQueueTest,featureQueueTrain, classifierInfoQueue, classifierInfoRetrieveEvent, 
                  classifierGuessMarkerQueue, classifierGuessMarkerEvent, queryFeaturesQueue, queryFeaturesEvent,
                  logger = Logger(Logger.INFO), numStreamDevices = 1,
                  minRequiredEpochs = 10, clf = None, model = None, torchModel = None):
         super().__init__()
         self.trainTestEvent = trainTestEvent # responsible for tolling between train and test mode
         self.closeEvent = closeEvent # responsible for cosing threads
@@ -24,71 +24,53 @@
         self.classifierInfoQueue = classifierInfoQueue
         self.classifierGuessMarkerQueue = classifierGuessMarkerQueue
         self.classifierGuessMarkerEvent = classifierGuessMarkerEvent
         self.queryFeaturesQueue = queryFeaturesQueue
         self.queryFeaturesEvent = queryFeaturesEvent
         self.numStreamDevices = numStreamDevices
         self.logger = logger
-        #self.features = np.array([])#[]
-        #self.targets = np.array([])
 
     def run(self):
         if self.numStreamDevices > 1:
             tempdatatrain = {}
             tempdatatest = {}
         while not self.closeEvent.is_set():
             if self.trainTestEvent.is_set(): # We're training!
-                try:
-                    featuresSingle, devCount, target, self.epochCounts = self.featureQueueTrain.get_nowait() #[dataFIFOs, self.currentMarker, self.sr, self.dataType]
-                    
-                    if self.numStreamDevices > 1: # Collects multiple data strems feature sets and synchronise here
-                        tempdatatrain[devCount] = featuresSingle
-                        if len(tempdatatrain) == self.numStreamDevices:
-                            flattened_list = [item for sublist in tempdatatrain.values() for item in sublist]
-                            tempdatatrain = {}
+                if self.featureQueueTrain.empty():
+                    if len(self.epochCountsc) > 1: # check if there is more then one test condition
+                        minNumKeyEpochs = min([self.epochCountsc[key][1] for key in self.epochCountsc]) # check minimum viable number of training eochs have been obtained
+                        if minNumKeyEpochs < self.minRequiredEpochs:
+                            pass
+                        else: 
+                            start = time.time()
+                            self.classifier.TrainModel(self.features, self.targets)
+                            if (self.logger.level == Logger.TIMING):
+                                end = time.time()
+                                self.logger.log(Logger.TIMING, f" classifier training time {end - start}")
+                    if self.classifierGuessMarkerEvent.is_set():
+                        self.classifierGuessMarkerQueue.put(self.guess)
+                else:
+                    try:
+                        featuresSingle, devCount, target, self.epochCountsc = self.featureQueueTrain.get_nowait() #[dataFIFOs, self.currentMarker, self.sr, self.dataType]
+                        
+                        if self.numStreamDevices > 1: # Collects multiple data strems feature sets and synchronise here
+                            tempdatatrain[devCount] = featuresSingle
+                            if len(tempdatatrain) == self.numStreamDevices:
+                                flattened_list = [item for sublist in tempdatatrain.values() for item in sublist]
+                                tempdatatrain = {}
+                                self.targets = np.append(self.targets, [target], axis = 0)
+                                self.features = np.append(self.features, [flattened_list], axis = 0)
+                            # need to check if all device data is captured, then flatten and append  
+                        else: # Only one device to collect from
+                            if self.features.shape[0] == 0:
+                                self.features = self.features.reshape((0,) + featuresSingle.shape)
                             self.targets = np.append(self.targets, [target], axis = 0)
-                            #print(self.features.shape)
-                            self.features = np.append(self.features, [flattened_list], axis = 0)
-                        # need to check if all device data is captured, then flatten and append
-                            if len(self.epochCounts) > 1: # check if there is more then one test condition
-                                minNumKeyEpochs = min([self.epochCounts[key][1] for key in self.epochCounts]) # check minimum viable number of training eochs have been obtained
-                                if minNumKeyEpochs < self.minRequiredEpochs:
-                                    pass
-                                else: 
-                                    start = time.time()
-                                    self.classifier.TrainModel(self.features, self.targets)
-                                    if (self.logger.level == Logger.TIMING):
-                                        end = time.time()
-                                        self.logger.log(Logger.TIMING, f" classifier training time {end - start}")
-                            if self.classifierGuessMarkerEvent.is_set():
-                                self.classifierGuessMarkerQueue.put(self.guess)
-                    else: # Only one device to collect from
-                        #self.targets.append(target)
-                        if self.features.shape[0] == 0:
-                            #print("reshaping")
-                            self.features = self.features.reshape((0,) + featuresSingle.shape)
-                        #self.features.append(featuresSingle)
-                        #print("target shape", self.targets.shape)
-                        self.targets = np.append(self.targets, [target], axis = 0)
-                        #print("feature shape ",self.features.shape)
-                        self.features = np.append(self.features, [featuresSingle], axis = 0)
-                        if len(self.epochCounts) > 1: # check if there is more then one test condition
-                            minNumKeyEpochs = min([self.epochCounts[key][1] for key in self.epochCounts]) # check minimum viable number of training eochs have been obtained
-                            if minNumKeyEpochs < self.minRequiredEpochs:
-                                pass
-                            else: 
-                                start = time.time()
-                                self.classifier.TrainModel(self.features, self.targets)
-                                if (self.logger.level == Logger.TIMING):
-                                    end = time.time()
-                                    self.logger.log(Logger.TIMING, f" classifier training time {end - start}")
-                        if self.classifierGuessMarkerEvent.is_set():
-                            self.classifierGuessMarkerQueue.put(self.guess)
-                except queue.Empty:
-                    pass
+                            self.features = np.append(self.features, [featuresSingle], axis = 0)
+                    except queue.Empty:
+                        pass
             else: # We're testing!
                 try:
                     featuresSingle, devCount = self.featureQueueTest.get_nowait() #[dataFIFOs, self.currentMarker, self.sr, self.dataType]
                     if self.numStreamDevices > 1:
                         tempdatatest[devCount] = featuresSingle
                         if len(tempdatatest) == self.numStreamDevices:
                             flattened_list = []
```

### Comparing `install-pybci-0.2.4b0/pybci/ThreadClasses/DataReceiverThread.py` & `install-pybci-0.2.4b1/pybci/ThreadClasses/DataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b0/pybci/ThreadClasses/FeatureProcessorThread.py` & `install-pybci-0.2.4b1/pybci/ThreadClasses/FeatureProcessorThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b0/pybci/ThreadClasses/MarkerThread.py` & `install-pybci-0.2.4b1/pybci/ThreadClasses/MarkerThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b0/pybci/ThreadClasses/OptimisedDataReceiverThread.py` & `install-pybci-0.2.4b1/pybci/ThreadClasses/OptimisedDataReceiverThread.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,24 @@
         else:
             window_length = self.globalEpochSettings.tmin+self.globalEpochSettings.tmax
         minfifoLength = int(self.sr * window_length * (1-self.globalEpochSettings.windowOverlap)) #  sets global window length with overlap as factor for minimum delay in test mode
         dataBuffers = np.zeros((minfifoLength,chCount))
         chs_to_drop = np.ones(chCount, dtype=bool)
         chs_to_drop[self.streamChsDropDict] = False
         #print(chs_to_drop)
-        fifoLength = int(self.sr * (maxTime+2)) # adds two seconds to give more timestamps when buffering  (assuming devices dont timeout for longer then 2.0 seconds, migth be worth making configurable)
+        fifoLength = int(self.sr * (maxTime+20)) # adds twenty seconds to give more timestamps when buffering  (assuming devices dont timeout for longer then 20.0 seconds, migth be worth making configurable)
         permanentDataBuffers = np.zeros((fifoLength, chCount - len(self.streamChsDropDict)))
         permanentTimestampBuffer = np.zeros(fifoLength)
         next_window_time = 0 # sets testing mode window time, duration based on windowlength and overlap
         while not self.closeEvent.is_set():
             _, timestamps = self.dataStreamInlet.pull_chunk(timeout=0.0, max_samples=dataBuffers.shape[0], dest_obj=dataBuffers) # optimised method of getting data to pull_sample, dest_obj saves memory re-allocation
             if timestamps:
+                #print(timestamps)
+                #if self.markerReceived:
+                #    print(self.markerTimestamp)
                 if len(self.streamChsDropDict) == 0:
                     dataBufferView = dataBuffers[:len(timestamps), :] # [:, :len(timestamps)]
                 else:
                     dataBufferView = dataBuffers[:len(timestamps), chs_to_drop] # [:, :len(timestamps)]
                 permanentDataBuffers = np.roll(permanentDataBuffers, shift=-len(timestamps), axis=0)
                 permanentTimestampBuffer = np.roll(permanentTimestampBuffer, shift=-len(timestamps))
                 permanentDataBuffers[-len(timestamps):,:] = dataBufferView
```

### Comparing `install-pybci-0.2.4b0/pybci/Utils/Classifier.py` & `install-pybci-0.2.4b1/pybci/Utils/Classifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,18 +33,22 @@
             self.classifierLibrary = "sklearn"
 
     def TrainModel(self, features, targets):
         x_train, x_test, y_train, y_test = train_test_split(features, targets, shuffle = True, test_size=0.2)
         #print(features.shape)
         #print(x_train.shape)
         if len(features.shape)==3:
-            self.scaler = [StandardScaler() for scaler in range(features.shape[1])] # normalise our data (everything is a 0 or a 1 if you think about it, cheers georgey boy boole)
-            for e in range(features.shape[1]): # this would normalise the channel, maybe better to normalise across other dimension
-                x_train[:,e,:] = self.scaler[e].fit_transform(x_train[:,e,:]) # Compute the mean and standard deviation based on the training data
-                x_test[:,e,:] = self.scaler[e].transform(x_test[:,e,:])  # Scale the test data
+            self.scaler = [StandardScaler() for scaler in range(features.shape[2])] # normalise our data (everything is a 0 or a 1 if you think about it, cheers georgey boy boole)
+            for e in range(features.shape[2]): # this would normalise the channel, maybe better to normalise across other dimension
+                x_train_channel = x_train[:,:,e].reshape(-1, 1)
+                x_test_channel = x_test[:,:,e].reshape(-1, 1)
+                x_train[:,:,e] = self.scaler[e].fit_transform(x_train_channel).reshape(x_train[:,:,e].shape)
+                x_test[:,:,e] = self.scaler[e].transform(x_test_channel).reshape(x_test[:,:,e].shape)
+                #x_train[:,:,e] = self.scaler[e].fit_transform(x_train[:,:,e]) # Compute the mean and standard deviation based on the training data
+                #x_test[:,:,e] = self.scaler[e].transform(x_test[:,:,e])  # Scale the test data
         elif len(features.shape)== 2:    
             self.scaler = StandardScaler() # normalise our data (everything is a 0 or a 1 if you think about it, cheers georgey boy boole)
             x_train = self.scaler.fit_transform(x_train)  # Compute the mean and standard deviation based on the training data
             x_test = self.scaler.transform(x_test)  # Scale the test data
         if all(item == y_train[0] for item in y_train):
             pass
         else:
@@ -60,16 +64,17 @@
                 self.loss, self.accuracy = self.model.evaluate(np.array(x_test), np.array(y_test))
             else:
                 # no classifier library selected, print debug?
                 pass
 
     def TestModel(self, x):
         if len(x.shape)==2:
-            for e in range(x.shape[0]):
-                x[e,:] = self.scaler[e].transform([x[e,:]])[0]
+            for e in range(x.shape[1]):
+                x[:,e] = self.scaler[e].transform(x[:,e].reshape(-1, 1)).reshape(x[:,e].shape)
+                #x[:,e] = self.scaler[e].transform([x[:,e]])[0]
         elif len(x.shape)== 1:       
             x = self.scaler.transform([x])[0]  # Scale the test data
         if self.classifierLibrary == "sklearn":
             x = np.expand_dims(x, axis=0)
             return self.clf.predict(x)
         elif self.classifierLibrary == "tensor":
             x = np.expand_dims(x, axis=0)
```

### Comparing `install-pybci-0.2.4b0/pybci/Utils/FeatureExtractor.py` & `install-pybci-0.2.4b1/pybci/Utils/FeatureExtractor.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b0/pybci/Utils/LSLScanner.py` & `install-pybci-0.2.4b1/pybci/Utils/LSLScanner.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b0/pybci/Utils/Logger.py` & `install-pybci-0.2.4b1/pybci/Utils/Logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 class Logger:
-    INFO = "info"
-    WARNING = "warning"
-    NONE = "none"
-    TIMING = "timing"
+    INFO = "INFO"
+    WARNING = "WARNING"
+    NONE = "NONE"
+    TIMING = "TIMING"
 
     def __init__(self, level=INFO):
         self.level = level
         self.check_level(level)
-
+        #print(self.level)
     def set_level(self, level):
         self.level = level
         self.check_level(level)
 
     def check_level(self,level):
         if level != self.WARNING and level != self.INFO and level != self.NONE and level != self.TIMING :
             print("PyBCI: [INFO] - Invalid or no log level selected, defaulting to info. (options: info, warning, none)")
             level = self.INFO
             self.level = level
 
     def log(self, level, message):
-        if self.level == 'none':
+        if self.level == self.NONE:
             return None
-        if level == 'info':
-            if self.level != 'none' and self.level != 'warning':
+        if level == self.INFO:
+            if self.level != self.NONE and self.level != self.WARNING:
                 print('PyBCI: [INFO] -' + message)
-        elif level == 'warning':
-            if self.level != 'none':
+        elif level == self.WARNING:
+            if self.level != self.NONE:
                 print('PyBCI: [WARNING] -' + message)
-        elif level == 'timing':
-            if self.level == 'timing':
+        elif level == self.TIMING:
+            if self.level == self.TIMING:
                 print('PyBCI: [TIMING] -' + message)
```

### Comparing `install-pybci-0.2.4b0/pybci/pybci.py` & `install-pybci-0.2.4b1/pybci/pybci.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         markerStream: List[str] 
             Allows user to set custom acceptable Marker stream definitions, if None defaults to markerTypes scan
         streamTypes: List[str] 
             Allows user to set custom acceptable EEG type definitions, ignored if dataStreams not None
         markerTypes: List[str] 
             Allows user to set custom acceptable Marker type definitions, ignored if markerStream not None
         loggingLevel: string 
-            Sets PyBCI print level, ('info' prints all statements, 'warning' is only warning messages, and 'none' is no prints from PyBCI)
+            Sets PyBCI print level, ('INFO' prints all statements, 'WARNING' is only warning messages, 'TIMING' gives estimated time for feature extraction, and  classifier training or testing,  'NONE' means no prints from PyBCI)
         globalEpochSettings (GlobalEpochSettings): 
             Sets global timing settings for epochs.
         customEpochSettings: dict 
             Sets individual timing settings for epochs. {markerstring1:IndividualEpochSettings(),markerstring2:IndividualEpochSettings()}
         streamChsDropDict: dict 
             Keys for dict should be respective datastreams with corresponding list of which channels to drop.  {datastreamstring1: list(ints), datastreamstring2: list(ints)}
         streamCustomFeatureExtract: dict
```

### Comparing `install-pybci-0.2.4b0/setup.py` & `install-pybci-0.2.4b1/setup.py`

 * *Files identical despite different names*

