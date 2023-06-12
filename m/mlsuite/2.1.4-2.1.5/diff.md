# Comparing `tmp/mlsuite-2.1.4.tar.gz` & `tmp/mlsuite-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlsuite-2.1.4.tar", last modified: Sun Apr 23 08:48:48 2023, max compression
+gzip compressed data, was "mlsuite-2.1.5.tar", last modified: Mon Jun 12 06:44:47 2023, max compression
```

## Comparing `mlsuite-2.1.4.tar` & `mlsuite-2.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-04-23 08:48:48.148092 mlsuite-2.1.4/
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1067 2022-08-30 02:42:20.000000 mlsuite-2.1.4/LICENSE
-drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-04-23 08:48:48.133675 mlsuite-2.1.4/MLsuite/
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     8137 2023-04-23 08:21:53.000000 mlsuite-2.1.4/MLsuite/MLArguments.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)    26629 2023-02-15 07:37:37.000000 mlsuite-2.1.4/MLsuite/MLEstimators.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     1931 2022-07-07 10:04:52.000000 mlsuite-2.1.4/MLsuite/MLLogging.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     2197 2023-04-07 02:10:21.000000 mlsuite-2.1.4/MLsuite/MLOpenWrite.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)      836 2022-09-06 09:45:06.000000 mlsuite-2.1.4/MLsuite/MLPipeline.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     4438 2022-09-13 08:33:47.000000 mlsuite-2.1.4/MLsuite/MLPredicting.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)    26665 2023-04-23 08:05:06.000000 mlsuite-2.1.4/MLsuite/MLSupervising.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     3424 2022-07-07 10:04:52.000000 mlsuite-2.1.4/MLsuite/MLUtilities.py
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)       17 2022-09-06 06:29:23.000000 mlsuite-2.1.4/MLsuite/__init__.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     2118 2022-12-14 01:57:48.000000 mlsuite-2.1.4/MLsuite/main.py
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1285 2023-04-23 08:48:48.146534 mlsuite-2.1.4/PKG-INFO
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     3421 2023-04-23 08:21:06.000000 mlsuite-2.1.4/README.md
-drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-04-23 08:48:48.143899 mlsuite-2.1.4/mlsuite.egg-info/
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1285 2023-04-23 08:48:47.000000 mlsuite-2.1.4/mlsuite.egg-info/PKG-INFO
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)      414 2023-04-23 08:48:47.000000 mlsuite-2.1.4/mlsuite.egg-info/SOURCES.txt
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)        1 2023-04-23 08:48:47.000000 mlsuite-2.1.4/mlsuite.egg-info/dependency_links.txt
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)      115 2023-04-23 08:48:47.000000 mlsuite-2.1.4/mlsuite.egg-info/requires.txt
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)        8 2023-04-23 08:48:47.000000 mlsuite-2.1.4/mlsuite.egg-info/top_level.txt
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)      455 2022-09-06 10:51:20.000000 mlsuite-2.1.4/mlsuite.py
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)       38 2023-04-23 08:48:48.148654 mlsuite-2.1.4/setup.cfg
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     1823 2023-04-23 08:12:39.000000 mlsuite-2.1.4/setup.py
+drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-06-12 06:44:47.309284 mlsuite-2.1.5/
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1067 2022-08-30 02:42:20.000000 mlsuite-2.1.5/LICENSE
+drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-06-12 06:44:47.292789 mlsuite-2.1.5/MLsuite/
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     8860 2023-06-12 05:35:05.000000 mlsuite-2.1.5/MLsuite/MLArguments.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)    26629 2023-04-28 08:19:34.000000 mlsuite-2.1.5/MLsuite/MLEstimators.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     1931 2022-07-07 10:04:52.000000 mlsuite-2.1.5/MLsuite/MLLogging.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     2197 2023-04-07 02:10:21.000000 mlsuite-2.1.5/MLsuite/MLOpenWrite.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)      836 2022-09-06 09:45:06.000000 mlsuite-2.1.5/MLsuite/MLPipeline.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     4450 2023-06-12 03:50:49.000000 mlsuite-2.1.5/MLsuite/MLPredicting.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)    28223 2023-06-12 06:43:29.000000 mlsuite-2.1.5/MLsuite/MLSupervising.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     3424 2022-07-07 10:04:52.000000 mlsuite-2.1.5/MLsuite/MLUtilities.py
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)       17 2022-09-06 06:29:23.000000 mlsuite-2.1.5/MLsuite/__init__.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     2118 2022-12-14 01:57:48.000000 mlsuite-2.1.5/MLsuite/main.py
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1285 2023-06-12 06:44:47.307899 mlsuite-2.1.5/PKG-INFO
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     3762 2023-06-12 06:43:42.000000 mlsuite-2.1.5/README.md
+drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-06-12 06:44:47.305323 mlsuite-2.1.5/mlsuite.egg-info/
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1285 2023-06-12 06:44:47.000000 mlsuite-2.1.5/mlsuite.egg-info/PKG-INFO
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)      414 2023-06-12 06:44:47.000000 mlsuite-2.1.5/mlsuite.egg-info/SOURCES.txt
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)        1 2023-06-12 06:44:47.000000 mlsuite-2.1.5/mlsuite.egg-info/dependency_links.txt
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)      115 2023-06-12 06:44:47.000000 mlsuite-2.1.5/mlsuite.egg-info/requires.txt
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)        8 2023-06-12 06:44:47.000000 mlsuite-2.1.5/mlsuite.egg-info/top_level.txt
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)      455 2022-09-06 10:51:20.000000 mlsuite-2.1.5/mlsuite.py
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)       38 2023-06-12 06:44:47.309947 mlsuite-2.1.5/setup.cfg
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     1823 2023-06-12 05:36:57.000000 mlsuite-2.1.5/setup.py
```

### Comparing `mlsuite-2.1.4/LICENSE` & `mlsuite-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.4/MLsuite/MLArguments.py` & `mlsuite-2.1.5/MLsuite/MLArguments.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     parser = argparse.ArgumentParser(
                 formatter_class=argparse.RawDescriptionHelpFormatter,
                 prefix_chars='-+',
                 conflict_handler='resolve',
                 description="\nThe traditional machine learning analysis based on sklearn package:\n",
                 epilog='''\
 Example:
-1. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -p data.predict.txt -o testdt/ -m DT
-2. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -p data.predict.txt -o testdt/ -m DT -f (10 times sample grouping and 10 models)
-3. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -o testdt/ -m DT
-4. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT
-5. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT -f (10 times sample grouping and 10 models)
-6. python mlsuite.py Predict -p data.predict.txt   -g group.new.txt -x modelpath/ -y predictdt/ -m DT.''')
+1. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -p data.predict.txt -o testdt/ -m DT -pn 0.9 (The cumulative contribution ratio of PCA is 0.9.)
+2. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -p data.predict.txt -o testdt/ -m DT -pn 0.9 -f (10 times sample grouping and 10 models)
+3. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -o testdt/ -m DT -pn 0.9
+4. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT -pn 0.9
+5. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT -pn 0.9 -f (10 times sample grouping and 10 models)
+6. python mlsuite.py Predict -p data.predict.txt   -g group.new.txt -x modelpath/ -y predictdt/ -m DT -pn 0.9.''')
 
     parser.add_argument('-V','--version',action ='version',
-                version='mlsuite version 2.1.4')
+                version='mlsuite version 2.1.5')
     subparsers = parser.add_subparsers(dest="commands",
                     help='machine learning models help.')
     ### Fitting module
     P_fitting  = subparsers.add_parser('Fitting',conflict_handler='resolve', add_help=False)
     P_fitting.add_argument("-f", "--fit_10", action="store_true", default=False,
                     help='''fitting modeling by 10 times sample spliting''')
     P_fitting.add_argument("-i", "--input",type=str,
@@ -79,14 +79,20 @@
 **SSS..................StratifiedShuffleSplit()
 **SKF..................StratifiedKFold()
 **RSKF.................RepeatedStratifiedKFold()
 **RKF..................RepeatedKFold()
 **LPO..................LeavePOut()
 **LOU..................LeaveOneOut()
 ''')
+    P_fitting.add_argument("-pn", "--pc_number", type=float, default=0,
+                    help='''select PC numbers, default is 0 that means not to do PCA analysis, >1 means selecting PC numbers,
+                            >0 and <1 means select the number of components such that the amount of variance that needs to be
+                            explained is greater than the percentage specified by pc_number.''')
+    P_fitting.add_argument("-am", "--Addmode", type=str, default='LinearSVM',
+                    help='''use additional model to adjust modeling in RF, GBDT and XGB estimators. N means no addition.''')
     P_fitting.add_argument("-rd", "--random",type=int, default=123456,
                     help="the random seeds for cross validation when using StratifiedShuffleSplit.")
     P_fitting.add_argument("-tz", "--testS",type=float, default=0.3,
                     help="the test size for cross validation when using StratifiedShuffleSplit.")
     P_fitting.add_argument("-sc", "--SearchCV",type=str, nargs='?', default='GSCV', choices=['GSCV','RSCV',],
                     help="the hyperparameters optimization method. You also can set it none to discard the method.")
     P_fitting.add_argument("-rt", "--Repeatime", type=int, default=1,
```

### Comparing `mlsuite-2.1.4/MLsuite/MLEstimators.py` & `mlsuite-2.1.5/MLsuite/MLEstimators.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.4/MLsuite/MLLogging.py` & `mlsuite-2.1.5/MLsuite/MLLogging.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.4/MLsuite/MLOpenWrite.py` & `mlsuite-2.1.5/MLsuite/MLOpenWrite.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.4/MLsuite/MLPipeline.py` & `mlsuite-2.1.5/MLsuite/MLPipeline.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.4/MLsuite/MLPredicting.py` & `mlsuite-2.1.5/MLsuite/MLPredicting.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,18 +35,18 @@
             assign = 1
         elif self.arg.refit == 'latest':
             assign = max(modelnu)
         else:
             assign = int(self.arg.refit)
         return '%s%s.pkl' % (comples, assign)
 
-    def Predict_X(self, DFall, _Y_name):
+    def Predict_X(self, DFall, _Y_name, Xa):
         Best_Model = joblib.load(self.GetLatest(_Y_name))
         CVRlt = HyperparamOptimal(arg=self.arg, log=self.log, model=self.arg.model, y_variable_type=self.Type, y_variable_class=self.MClass)
-        Y_PRED, Y_Eval = CVRlt.Predicting_C(Best_Model, DFall, _Y_name)
+        Y_PRED, Y_Eval = CVRlt.Predicting_C(Best_Model, DFall, _Y_name, Xa)
         ### All_Pred_predict
         merge_opt = MergeAllResult(log=self.log)
         merge_opt.CVMerge(Y_PRED, label='Predict')
         Openf('%s%s_Class_%s_detials.xls'%(self.arg.output, _Y_name, 'Predict'), (merge_opt.allTest), index=True, index_label='sample').openv()
         Openf('%s%s_Class_%s_summary.xls'%(self.arg.output, _Y_name, 'Predict'), (merge_opt.ALL_Result), index=True, index_label='sample').openv()
         Openf('%s%s_Class_%s_summary_statistics.xls'%(self.arg.output, _Y_name, 'Predict'), (merge_opt.EvalueA), index=True, index_label='Score').openv()
         ### All_evaluate_score_
@@ -65,15 +65,15 @@
 
     ### load data
     (group, RYa, CYa, Xa, Xg) = OpenM(args, Log).openg()
     YType = group[(group.Variables.isin(RYa + CYa))][['Variables', 'Type']]
     Predt_set = OpenM(args, Log).openp()
     for Yi,Typi in YType.values:
         Log.CIF(('%s: Supervised Predicting' % Yi).center(45, '*'))
-        Supervised(args, Log, Type=Typi, MClass=2).Predict_X(Predt_set, Yi)
+        Supervised(args, Log, Type=Typi, MClass=2).Predict_X(Predt_set, Yi, Xa)
         Log.CIF(('%s: Supervised Predicting Finish' % Yi).center(45, '*'))
     Log.CIF('Supervisor Predicting Finish'.center(45, '*'))
 
 
 if __name__ == "__main__":
     from MLLogging import Logger
     from MLArguments import Args
```

### Comparing `mlsuite-2.1.4/MLsuite/MLSupervising.py` & `mlsuite-2.1.5/MLsuite/MLSupervising.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from .MLUtilities import MyThread, _predict_proba_lr, CrossvalidationSplit, Check_Label, Check_Binar
 from .MLEstimators import ML
 from .MLOpenWrite import OpenM, Openf
 from sklearn.model_selection import GridSearchCV, RandomizedSearchCV
 from sklearn.metrics import (accuracy_score, f1_score, recall_score, precision_score,
                              balanced_accuracy_score, roc_auc_score, average_precision_score)
+from sklearn.decomposition import PCA
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.calibration import CalibratedClassifierCV
 from scipy.sparse import vstack
 import os
 import numpy as np
 import pandas as pd
 import re
@@ -64,15 +65,15 @@
         self.Type = y_variable_type
         self.MClass = y_variable_class
         self.score = score
     
     def Pdecorator(self):
         # sample split
         if self.Type == 'C':
-            self.SSS = CrossvalidationSplit(n_splits=9, test_size=self.arg.GStestS, CVt='SSS', random_state=self.arg.random)
+            self.SSS = CrossvalidationSplit(n_splits=10, test_size=self.arg.GStestS, CVt='SSS', random_state=self.arg.random)
         elif self.Type == 'R':
             self.SSS = CrossvalidationSplit(n_splits=3, n_repeats=3, CVt='RSKF', random_state=self.arg.random)
         else:
             self.SSS = ''
         # get estimator and parameters
         self.estimator = ML(self.model, Type=self.Type).GetPara().estimator
         if self.arg.SearchCV:
@@ -140,15 +141,15 @@
         # print best parameters
         if hasattr(clf, 'best_estimator_'):
             self.log += HyperparamOptimal.logRecord('info','%s best parameters in %s: \n%s\n', self.model, self.arg.SearchCV, clf.best_estimator_.get_params())
             self.clf = clf.best_estimator_
         else:
             self.log += HyperparamOptimal.logRecord('info','%s best parameters: \n%s\n', self.model, clf.get_params())
             self.clf = clf
-    
+
     # obj: refitting the models by the entire train data
     @staticmethod
     def re_fit(clf, x_matrix, y_matrix, model, log):
         new_clf = clf.fit(x_matrix, y_matrix)
         log += HyperparamOptimal.logRecord('info', '%s model has been refitted by input train data.\n', model)
         return new_clf
     
@@ -278,52 +279,59 @@
                                                  
     def getModelResult(self, x_matrix='N'):
         if x_matrix=='N':
             self.x = HyperparamOptimal.MergeTrainTest(train=self.x_train, test=self.x_test)
         else:
             self.x = x_matrix
         self.y = HyperparamOptimal.MergeTrainTest(train=self.y_train, test=self.y_test)
-        self.new_clf = HyperparamOptimal.re_fit(clf=self.clf, x_matrix=self.x, y_matrix=self.y, model=self.model, log=self.log)
-        self.clf_C = HyperparamOptimal.CalibratedClassifierCV(clf=self.new_clf, CV=self.SSS, method=self.arg.calibme, x_matrix=self.x, y_matrix=self.y)
-        predict_G, self.log = HyperparamOptimal.GetPredict(clf=self.new_clf, x_matrix=self.x, mclass=self.MClass, log=self.log)
+        # self.new_clf = HyperparamOptimal.re_fit(clf=self.clf, x_matrix=self.x, y_matrix=self.y, model=self.model, log=self.log)
+        self.clf_C = HyperparamOptimal.CalibratedClassifierCV(clf=self.clf, CV=self.SSS, method=self.arg.calibme, x_matrix=self.x_train, y_matrix=self.y_train)
+        predict_G, self.log = HyperparamOptimal.GetPredict(clf=self.clf, x_matrix=self.x, mclass=self.MClass, log=self.log)
         predict_C, self.log = HyperparamOptimal.GetPredict(clf=self.clf_C, x_matrix=self.x, mclass=self.MClass, log=self.log)
         predict = pd.DataFrame(np.c_[self.y, predict_G, predict_C], index=self.y.index)
         predict.columns = ['TRUE', 'Pred_%s'%self.model] + ['%s_Prob_%s'%(x, self.model) for x in range(self.MClass)] + \
                             ['Pred_C_%s'%self.model] + ['%s_Prob_C_%s'%(x, self.model) for x in range(self.MClass)]
-        coef, self.log = HyperparamOptimal.GetCoef(model=self.model, clf=self.new_clf, mclass=self.MClass, log=self.log, index=self.x.columns)
-        Best_MD = [{'model':self.model, 'clf':self.new_clf, 'features':self.x.columns.tolist()},
+        coef, self.log = HyperparamOptimal.GetCoef(model=self.model, clf=self.clf, mclass=self.MClass, log=self.log, index=self.x.columns)
+        Best_MD = [{'model':self.model, 'clf':self.clf, 'features':self.x.columns.tolist()},
                    {'model':'C_'+self.model, 'clf':self.clf_C, 'features':self.x.columns.tolist()}]
         return(predict, coef, Best_MD)
 
     # obj: predict the testing dataset by 13 models
-    def Predicting_C(self, best_model, pDFall, y_name):
+    def Predicting_C(self, best_model, pDFall, y_name, xa):
         Y_TRUE  = pDFall[y_name].to_frame(name='TRUE')
         Y_PRED , Y_Eval = [], []
         for _k, _cv in enumerate(best_model):
             y_pred = [Y_TRUE]
             for _i, _m in enumerate(_cv):
                 model = _m['model']
                 clf = _m['clf']
                 model_x_names = _m['features']
-                x_pred = pDFall[model_x_names]
+                if 'pca_clf' in _m:
+                    pca_clf = _m['pca_clf']
+                    tmp = pd.DataFrame(pca_clf.transform(pDFall[xa]), index=pDFall.index)
+                    tmp.columns = ["PC"+str(j) for j in range(1, tmp.shape[1]+1)]
+                    x_pred = tmp[model_x_names]
+                else:
+                    x_pred = pDFall[model_x_names]
                 if 'leaf' in _m.keys():
                     leaf = _m['leaf']
                     x_pred, OHE = HyperparamOptimal.OneHot(self.model, _cv[0]['clf'], x_pred, leaf)
                 log = ''
                 _prepro, log = HyperparamOptimal.GetPredict(clf, x_pred, self.MClass, log)
                 self.log.NIF(log)
                 _prepro = pd.DataFrame(_prepro,
                                        index=pDFall.index,
                                        columns = ['Pred_%s' % model] + ['%s_Prob_%s'%(x, model) for x in range(self.MClass)]
                                        )
                 y_pred.append(_prepro)
             y_pred  = pd.concat(y_pred, axis=1)
+            Openf('%s%s_Class_%s_predict.xls'%(self.arg.output, y_name, "Test_"+str(_k+1)), (y_pred), index=True, index_label='sample').openv()
             y_predv = y_pred[~y_pred['TRUE'].isna()]
             self.log.CIF(('%s %s Model Predicting Parameters'% (y_name, self.model)).center(45, '-'))
-            if y_predv.shape[0] > 2:
+            if y_predv['TRUE'].nunique() >= 2:
                 Pred_Mel = HyperparamOptimal.GetScore(df=y_predv, label='Predict')
                 self.log.CIF("%s Modeling evaluation: \n%s" % (self.model, Pred_Mel))
             else:
                 Pred_Mel = pd.DataFrame()
             self.log.CIF(('Completed %2d%%'% ((_k+1)*100/len(best_model))).center(45, '-'))
             Y_PRED.append(y_pred)
             Y_Eval.append(Pred_Mel)
@@ -412,32 +420,32 @@
  
 ### define some functions
 def modeling(arg, x_train, x_test, y_train, y_test, Typi, mclass, _k, _n, allGroup):
     log = ''
     hyper = HyperparamOptimal(arg, log, model=arg.model, y_variable_type=Typi, y_variable_class=mclass)
     hyper.Hyperparemet(x_train, x_test, y_train, y_test)
     predict, coef, Best_MD = hyper.getModelResult()
-    Openf('%s%s_Class_%s_predict.xls'%(arg.output, 'Group', str(_n+1)), (predict), index=True, index_label='sample').openv()
     logText = hyper.log
     # addmodel
     if (arg.model in ['GBDT', 'XGB', 'RF']) and (arg.Addmode !='N'):
         log_add = ''
         x_train_add, OHE = HyperparamOptimal.OneHot(model=arg.model, clf=hyper.clf, x_matrix=x_train)
         x_test_add,  OHE = HyperparamOptimal.OneHot(model=arg.model, clf=hyper.clf, x_matrix=x_test, OHE=OHE)
-        x_matrix_add, OHE_merge = HyperparamOptimal.OneHot(model=arg.model, clf=hyper.new_clf, x_matrix=hyper.x)
         hyper_add = HyperparamOptimal(arg, log_add, model=arg.Addmode, y_variable_type=Typi, y_variable_class=mclass)
         hyper_add.Hyperparemet(x_train_add, x_test_add, y_train, y_test)
-        predict_add, coef_add, Best_MD_add = hyper_add.getModelResult(x_matrix=x_matrix_add)
+        predict_add, coef_add, Best_MD_add = hyper_add.getModelResult()
         predict = pd.concat([predict, predict_add], axis=1)
-        Best_MD_add[0].update({'leaf':OHE_merge})
-        Best_MD_add[1].update({'leaf':OHE_merge})
+        Best_MD_add[0].update({'leaf':OHE})
+        Best_MD_add[1].update({'leaf':OHE})
         Best_MD += Best_MD_add
     # statistic    
-    if len(y_test)>2 and mclass<=2:
-        score = HyperparamOptimal.GetScore(predict.loc[y_train.index], label='Train')
+    if y_test.nunique() >= 2 and mclass<=2:
+        score_train = HyperparamOptimal.GetScore(predict.loc[y_train.index], label='Train')
+        score_validation = HyperparamOptimal.GetScore(predict.loc[y_test.index], label='Validation')
+        score = pd.concat([score_train, score_validation], axis=1)
     else:
         score = pd.DataFrame()
     logText += HyperparamOptimal.logRecord('info', '%s Modeling evaluation: \n%s\n', arg.model, score)
     logText += HyperparamOptimal.logRecord('info', ('Modeling has been Completed %2d%%%%' % ((_k+1)*(_n+1)*100/(arg.Repeatime*allGroup))).center(45, '-'))
     logText += "\n"
     return(predict, coef, score, Best_MD, logText)
 
@@ -465,25 +473,40 @@
         # threads = []
         for repeat in range(args.Repeatime):
             for i in range(len(sample_group_index)):
                 train_index, test_index = sample_group_index[i]
                 train , test = DFall.iloc[train_index, :], DFall.iloc[test_index, :]
                 x_train, y_train = train[Xi], train[Yi]
                 x_test , y_test  = test[Xi], test[Yi]
+                if args.pc_number != 0:
+                    if args.pc_number >= 1:
+                        pc_number = int(args.pc_number)
+                    else:
+                        pc_number = args.pc_number
+                    pca_clf = PCA(n_components=pc_number).fit(x_train)
+                    x_train = pd.DataFrame(pca_clf.transform(x_train), index=x_train.index)
+                    x_test = pd.DataFrame(pca_clf.transform(x_test), index=x_test.index)
+                    x_train.columns = ["PC"+str(j) for j in range(1, x_train.shape[1]+1)]
+                    x_test.columns = ["PC"+str(j) for j in range(1, x_test.shape[1]+1)]
             #    t = MyThread(modeling, (args, x_train, x_test, y_train, y_test, Typi, DFall[Yi].nunique(), repeat, i, len(sample_group_index)))
             #    threads.append(t)
             #for i in range(len(sample_group_index)):
             #    threads[i].setDaemon(True)
             #    threads[i].start()
             #for i in range(len(sample_group_index)):
             #    threads[i].join()
             #for i in range(len(sample_group_index)):
             #    full_predict, coef, score, MD, logText = threads[i].get_result()
                 full_predict, coef, score, MD, logText = modeling(args, x_train, x_test, y_train, y_test, Typi, DFall[Yi].nunique(), repeat, i, len(sample_group_index))
+                Openf('%s%s_Class_%s_predict.xls'%(args.output, Yi, "Train_"+str(i+1)), (full_predict.loc[y_train.index, ]), index=True, index_label='sample').openv()
+                Openf('%s%s_Class_%s_predict.xls'%(args.output, Yi, "Validation_"+str(i+1)), (full_predict.loc[y_test.index, ]), index=True, index_label='sample').openv()
                 allPredict.append(full_predict)
+                if args.pc_number != 0:
+                    for j in range(0, len(MD)):
+                        MD[j].update({'pca_clf':pca_clf})
                 allMD.append(MD)
                 if not coef.empty:
                     allCoef.append(coef)
                 if not score.empty:
                     allScore.append(score)
                 Log.NIF(logText)
             Log.CIF('Modeling has been Completed'.center(45, '-'))
@@ -495,15 +518,15 @@
         matp.ModelScore(allScore)
         Openf('%s%s_Class_%s_detials.xls'%(args.output, Yi, 'Train'), (matp.allTest), index=True, index_label='sample').openv()
         Openf('%s%s_Class_%s_summary.xls'%(args.output, Yi, 'Train'), (matp.ALL_Result), index=True, index_label='sample').openv()
         Openf('%s%s_Class_%s_summary_statistics.xls'%(args.output, Yi, 'Train'), (matp.EvalueA), index=True, index_label='Score').openv()
         Openf('%s%s_Class_features_importance.xls' %(args.output, Yi), (matp.All_import)).openv()
         Openf('%s%s_Class_%s_metrics_pvalues.xls'%(args.output, Yi, 'Train'), (matp.All_pvalues), index=True, index_label='Score').openv()
         joblib.dump(DFall[Xi+[Yi]], '%s%s_Class_traintest_set.pkl' %(args.MODELF, Yi), compress=1)
-        joblib.dump(allMD , '%s%s_Class_best_estimator_1.pkl' %(args.MODELF, Yi), compress=1)
+        joblib.dump(allMD, '%s%s_Class_best_estimator_1.pkl' %(args.MODELF, Yi), compress=1)
     Log.CIF(('%s: Supervised MODELing Finish' % Yi).center(45, '*'))
    
 if __name__ == "__main__":
     from MLLogging import Logger
     from MLArguments import Args
     args = Args()
     args.commands = "Fitting"
```

### Comparing `mlsuite-2.1.4/MLsuite/MLUtilities.py` & `mlsuite-2.1.5/MLsuite/MLUtilities.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.4/MLsuite/main.py` & `mlsuite-2.1.5/MLsuite/main.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.4/PKG-INFO` & `mlsuite-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlsuite
-Version: 2.1.4
+Version: 2.1.5
 Summary: The traditional machine learning analysis based on sklearn package
 Home-page: https://git.genecast.com.cn/narwhal/mlsuite
 Author: suxing li
 Author-email: li.suxing@genecast.com.cn
 Maintainer: suxing li
 Maintainer-email: li.suxing@genecast.com.cn
 Platform: all
```

### Comparing `mlsuite-2.1.4/README.md` & `mlsuite-2.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # mlsuite
 
 ## Install
 
 ```
-pip install mlsuite==2.1.4
+pip install mlsuite==2.1.5
 pip install https://github.com/JamesRitchie/scikit-rvm/archive/master.zip
 ```
 
 ## Usage
 
 Notice: used pyhton3, not python2
 
@@ -24,22 +24,25 @@
 
 optional arguments:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
 
 Example:
 
-1. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -p data.predict.txt -o testdt/ -m DT
-2. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -p data.predict.txt -o testdt/ -m DT -f (10 times sample grouping and 10 models)
-3. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -o testdt/ -m DT
-4. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT
-5. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT -f (10 times sample grouping and 10 models)
-6. python mlsuite.py Predict -p data.predict.txt   -g group.new.txt -x modelpath/ -y predictdt/ -m DT.
+1. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -p data.predict.txt -o testdt/ -m DT -pn 0.9 (The cumulative contribution ratio of PCA is 0.9.)
+2. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -p data.predict.txt -o testdt/ -m DT -pn 0.9 -f (10 times sample grouping and 10 models)
+3. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -o testdt/ -m DT -pn 0.9
+4. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT -pn 0.9
+5. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT -pn 0.9 -f (10 times sample grouping and 10 models)
+6. python mlsuite.py Predict -p data.predict.txt   -g group.new.txt -x modelpath/ -y predictdt/ -m DT -pn 0.9.
 
 ## Update log
+### v2.1.5
+1. "Fitting" module has been added "-pn|--pc_number" arguments, which the spliting training data was reduced dimensions by PCA, and assign the number of PCs (integer, [1,Inf)) or the cumulative contribution ratio (float, (0, 1)).
+
 ### v2.1.4
 1. "Fitting" module has been added "-f|--fit_10" arguments, which the input training dataset was splited into 10 train/test groups, and got 10 models.
 
 ### v2.1.3
 1. pandas's parameter "line_terminator" had changed into "lineterminator" in the 2.0.0 version, so drop "line_terminator" in "MLOpenWrite.py" script.
 2. fixed same packages' version:
 ```
```

### Comparing `mlsuite-2.1.4/mlsuite.egg-info/PKG-INFO` & `mlsuite-2.1.5/mlsuite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlsuite
-Version: 2.1.4
+Version: 2.1.5
 Summary: The traditional machine learning analysis based on sklearn package
 Home-page: https://git.genecast.com.cn/narwhal/mlsuite
 Author: suxing li
 Author-email: li.suxing@genecast.com.cn
 Maintainer: suxing li
 Maintainer-email: li.suxing@genecast.com.cn
 Platform: all
```

### Comparing `mlsuite-2.1.4/setup.py` & `mlsuite-2.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages, setup
 from glob import glob
 from os.path import dirname, join
 import os
 
 setup(
     name='mlsuite',
-    version='2.1.4',
+    version='2.1.5',
     description='The traditional machine learning analysis based on sklearn package',
     author='suxing li',
     author_email='li.suxing@genecast.com.cn',
     maintainer='suxing li',
     maintainer_email='li.suxing@genecast.com.cn',
     packages=find_packages(where='.', exclude=(), include=('*',)),
     include_package_data=True,
```

