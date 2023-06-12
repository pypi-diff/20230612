# Comparing `tmp/torchbones-1.2.3.tar.gz` & `tmp/torchbones-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.2.3.tar", last modified: Mon Jun 12 20:55:02 2023, max compression
+gzip compressed data, was "torchbones-1.2.4.tar", last modified: Mon Jun 12 20:59:20 2023, max compression
```

## Comparing `torchbones-1.2.3.tar` & `torchbones-1.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-12 20:55:02.024489 torchbones-1.2.3/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      202 2023-06-12 20:55:02.024489 torchbones-1.2.3/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-12 20:55:02.024489 torchbones-1.2.3/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-12 20:54:38.000000 torchbones-1.2.3/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-12 20:55:02.014489 torchbones-1.2.3/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.2.3/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    17154 2023-06-09 16:49:56.000000 torchbones-1.2.3/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-12 20:55:02.024489 torchbones-1.2.3/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      202 2023-06-12 20:55:01.000000 torchbones-1.2.3/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-12 20:55:01.000000 torchbones-1.2.3/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-12 20:55:01.000000 torchbones-1.2.3/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-12 20:55:01.000000 torchbones-1.2.3/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-12 20:55:01.000000 torchbones-1.2.3/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-12 20:59:20.274487 torchbones-1.2.4/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      202 2023-06-12 20:59:20.274487 torchbones-1.2.4/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-12 20:59:20.274487 torchbones-1.2.4/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-12 20:59:16.000000 torchbones-1.2.4/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-12 20:59:20.264487 torchbones-1.2.4/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.2.4/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    17205 2023-06-12 20:59:10.000000 torchbones-1.2.4/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-12 20:59:20.274487 torchbones-1.2.4/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      202 2023-06-12 20:59:20.000000 torchbones-1.2.4/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-12 20:59:20.000000 torchbones-1.2.4/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-12 20:59:20.000000 torchbones-1.2.4/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-12 20:59:20.000000 torchbones-1.2.4/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-12 20:59:20.000000 torchbones-1.2.4/torchbones.egg-info/top_level.txt
```

### Comparing `torchbones-1.2.3/torchbones/main.py` & `torchbones-1.2.4/torchbones/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
     
 class Model:
     def __init__(self, *args, **kwargs):
         self.lins, self.activation, self.optim,  self.batch_size, self.lr, self.indata, self.truth, self.cost =args
         
         keys = ('convs', 'csizes','lr_decay',  'saving', 'run_num', 'new_tar', 'save_weights',
-                'lr_min','dropout', 'resnet', 'train_frac', 'test_set', 'cov', 'max_batch' )
+                'lr_min','dropout', 'resnet', 'train_frac', 'test_set', 'cov', 'max_batch', 'check' )
         for kwarg in kwargs.keys():
             if kwarg not in keys:
                 raise Exception(kwarg + ' is not a valid key. Valid keys: ', keys )
         
         self.cov = kwargs.get('cov', 1)
         self.convs = kwargs.get('convs', [])
         self.csizes = kwargs.get('csizes', [])
@@ -150,15 +150,16 @@
         if self.save_tar and not self.saving:
             raise Exception('Saving must be enabled to save model weights')
         if self.save and not os.path.exists(val_file):
             pickle.dump(self.params(), open(val_file, 'wb'))
             
         self.run_num = kwargs.get('run_num', None)
         self.new_tar = kwargs.get('new_tar', False)
-        self.check()
+        if kwargs.get('check', True):
+            self.check()
         if self.run_num:
             vals = pickle.load(open(val_file,'rb')).loc[self.run_num]
             self.epoch = vals['epochs']
             self.err = vals['test loss']
             self.lr = vals['learning rate']
             print('Weights from run ', str(self.run_num), ' loaded.')
         else: self.epoch = 0
```

