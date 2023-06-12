# Comparing `tmp/jjuke-0.0.0.8.tar.gz` & `tmp/jjuke-0.0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jjuke-0.0.0.8.tar", last modified: Fri May 26 18:57:30 2023, max compression
+gzip compressed data, was "dist/jjuke-0.0.1.0.tar", last modified: Mon Jun 12 07:07:22 2023, max compression
```

## Comparing `jjuke-0.0.0.8.tar` & `jjuke-0.0.1.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      162 2023-05-11 12:21:10.000000 jjuke-0.0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke/
--rw-r--r--   0 root         (0) root         (0)      121 2023-05-26 18:56:46.000000 jjuke-0.0.0.8/jjuke/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2967 2023-05-26 18:56:26.000000 jjuke-0.0.0.8/jjuke/logger.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-05-24 07:55:24.000000 jjuke-0.0.0.8/jjuke/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke/metrics/
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-25 18:10:12.000000 jjuke-0.0.0.8/jjuke/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11621 2023-05-25 18:09:59.000000 jjuke-0.0.0.8/jjuke/metrics/evaluation_metrics.py
--rw-r--r--   0 root         (0) root         (0)     2967 2023-05-24 13:00:20.000000 jjuke-0.0.0.8/jjuke/metrics/pointcloud.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke/module/
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/module/__init__.py
--rw-r--r--   0 root         (0) root         (0)      534 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/module/func.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/module/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke/module/loss/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/module/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-05-24 07:55:26.000000 jjuke-0.0.0.8/jjuke/module/loss/focal.py
--rw-r--r--   0 root         (0) root         (0)      362 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/module/loss/utils.py
--rw-r--r--   0 root         (0) root         (0)     4318 2023-05-24 07:55:25.000000 jjuke-0.0.0.8/jjuke/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke/pointcloud/
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-26 07:37:06.000000 jjuke-0.0.0.8/jjuke/pointcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9538 2023-05-26 07:37:15.000000 jjuke-0.0.0.8/jjuke/pointcloud/transform.py
--rw-r--r--   0 root         (0) root         (0)    15015 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/sched.py
--rw-r--r--   0 root         (0) root         (0)    25202 2023-05-24 07:55:25.000000 jjuke-0.0.0.8/jjuke/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke/utils/
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2493 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/data.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/dist.py
--rw-r--r--   0 root         (0) root         (0)      457 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/ema.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/indexing.py
--rw-r--r--   0 root         (0) root         (0)     9553 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/interp1d.py
--rw-r--r--   0 root         (0) root         (0)      259 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/io.py
--rw-r--r--   0 root         (0) root         (0)     7370 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/optim.py
--rw-r--r--   0 root         (0) root         (0)     5673 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/utils.py
--rw-r--r--   0 root         (0) root         (0)     9062 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/vis3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke.egg-info/
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      831 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      622 2023-05-26 18:56:40.000000 jjuke-0.0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:07:22.000000 jjuke-0.0.1.0/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-12 07:07:22.000000 jjuke-0.0.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      152 2023-06-12 07:04:38.000000 jjuke-0.0.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:07:22.000000 jjuke-0.0.1.0/jjuke/
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-12 07:06:24.000000 jjuke-0.0.1.0/jjuke/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-06-12 06:43:37.000000 jjuke-0.0.1.0/jjuke/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-05-24 07:55:24.000000 jjuke-0.0.1.0/jjuke/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:07:22.000000 jjuke-0.0.1.0/jjuke/metrics/
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-25 18:10:12.000000 jjuke-0.0.1.0/jjuke/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11621 2023-05-25 18:09:59.000000 jjuke-0.0.1.0/jjuke/metrics/evaluation_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-05-24 13:00:20.000000 jjuke-0.0.1.0/jjuke/metrics/pointcloud.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:07:22.000000 jjuke-0.0.1.0/jjuke/module/
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-11 12:09:23.000000 jjuke-0.0.1.0/jjuke/module/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      534 2023-05-11 12:09:23.000000 jjuke-0.0.1.0/jjuke/module/func.py
+-rw-r--r--   0 root         (0) root         (0)      730 2023-06-12 06:50:46.000000 jjuke-0.0.1.0/jjuke/module/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:07:22.000000 jjuke-0.0.1.0/jjuke/module/loss/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-11 12:09:23.000000 jjuke-0.0.1.0/jjuke/module/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-06-12 06:51:59.000000 jjuke-0.0.1.0/jjuke/module/loss/focal.py
+-rw-r--r--   0 root         (0) root         (0)      356 2023-06-12 06:51:08.000000 jjuke-0.0.1.0/jjuke/module/loss/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4318 2023-05-24 07:55:25.000000 jjuke-0.0.1.0/jjuke/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:07:22.000000 jjuke-0.0.1.0/jjuke/pointcloud/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-26 07:37:06.000000 jjuke-0.0.1.0/jjuke/pointcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9538 2023-05-26 07:37:15.000000 jjuke-0.0.1.0/jjuke/pointcloud/transform.py
+-rw-r--r--   0 root         (0) root         (0)    15015 2023-05-11 12:09:23.000000 jjuke-0.0.1.0/jjuke/sched.py
+-rw-r--r--   0 root         (0) root         (0)    25202 2023-05-24 07:55:25.000000 jjuke-0.0.1.0/jjuke/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:07:22.000000 jjuke-0.0.1.0/jjuke/utils/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-11 12:09:23.000000 jjuke-0.0.1.0/jjuke/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-06-12 06:51:55.000000 jjuke-0.0.1.0/jjuke/utils/data.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-11 12:09:23.000000 jjuke-0.0.1.0/jjuke/utils/dist.py
+-rw-r--r--   0 root         (0) root         (0)      457 2023-05-11 12:09:23.000000 jjuke-0.0.1.0/jjuke/utils/ema.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-06-12 06:51:50.000000 jjuke-0.0.1.0/jjuke/utils/indexing.py
+-rw-r--r--   0 root         (0) root         (0)     9553 2023-05-11 12:09:23.000000 jjuke-0.0.1.0/jjuke/utils/interp1d.py
+-rw-r--r--   0 root         (0) root         (0)      259 2023-05-11 12:09:23.000000 jjuke-0.0.1.0/jjuke/utils/io.py
+-rw-r--r--   0 root         (0) root         (0)     7370 2023-05-11 12:09:23.000000 jjuke-0.0.1.0/jjuke/utils/optim.py
+-rw-r--r--   0 root         (0) root         (0)     9294 2023-06-12 06:53:09.000000 jjuke-0.0.1.0/jjuke/utils/utils.py
+-rw-r--r--   0 root         (0) root         (0)    22463 2023-06-12 06:40:16.000000 jjuke-0.0.1.0/jjuke/utils/vis3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:07:22.000000 jjuke-0.0.1.0/jjuke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-12 07:07:22.000000 jjuke-0.0.1.0/jjuke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      831 2023-06-12 07:07:22.000000 jjuke-0.0.1.0/jjuke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 07:07:22.000000 jjuke-0.0.1.0/jjuke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-12 07:07:22.000000 jjuke-0.0.1.0/jjuke.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 18:57:30.000000 jjuke-0.0.1.0/jjuke.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      128 2023-06-12 07:07:22.000000 jjuke-0.0.1.0/jjuke.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-12 07:07:22.000000 jjuke-0.0.1.0/jjuke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 07:07:22.000000 jjuke-0.0.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      702 2023-06-12 07:05:54.000000 jjuke-0.0.1.0/setup.py
```

### Comparing `jjuke-0.0.0.8/jjuke/logger.py` & `jjuke-0.0.1.0/jjuke/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from datetime import datetime
 from functools import reduce
 from pathlib import Path
 
-__all__ = ["CustomLogger", "timenow", "basicConfig", "getLogger"]
+__all__ = ["CustomLogger", "timenow"]
 
 
 class CustomLogger:
     def __init__(self, log_dir="./exps", filemode="a", isTrain=True, use_color=True, lock=False):
         self.log_dir = log_dir
         self.lock = lock
         
@@ -86,18 +86,7 @@
 
 def timenow(braket=False):
     n = datetime.now()
     if braket:
         return f"[{n.year}-{n.month:02d}-{n.day:02d} {n.hour:02d}:{n.minute:02d}:{n.second:02d}]"
     else:
         return f"{n.year}-{n.month:02d}-{n.day:02d} {n.hour:02d}:{n.minute:02d}:{n.second:02d}"
-
-
-_logger = CustomLogger()
-
-
-def basicConfig(filename, lock=False):
-    _logger.__init__(filename, lock=lock)
-
-
-def getLogger():
-    return _logger
```

### Comparing `jjuke-0.0.0.8/jjuke/main.py` & `jjuke-0.0.1.0/jjuke/main.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.8/jjuke/metrics/evaluation_metrics.py` & `jjuke-0.0.1.0/jjuke/metrics/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.8/jjuke/metrics/pointcloud.py` & `jjuke-0.0.1.0/jjuke/metrics/pointcloud.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.8/jjuke/module/func.py` & `jjuke-0.0.1.0/jjuke/module/func.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.8/jjuke/module/init.py` & `jjuke-0.0.1.0/jjuke/module/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import torch as th
+import torch
 import torch.nn as nn
 import torch.nn.init as init
 from timm.models.layers import trunc_normal_
 
 _module_list = (nn.Conv1d, nn.Conv2d, nn.Conv3d, nn.Linear, nn.ConvTranspose1d, nn.ConvTranspose2d, nn.ConvTranspose3d)
```

### Comparing `jjuke-0.0.0.8/jjuke/module/loss/focal.py` & `jjuke-0.0.1.0/jjuke/module/loss/focal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import torch as th
+import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import Tensor
 
 from jjuke.module.loss.utils import _reduce
 
 __all__ = ["focal_loss", "FocalLoss"]
@@ -14,15 +14,15 @@
     - logits: b c ...
     - targets: b ... (long)
 
     CE(p) = -\log(p)
     FL(p) = -(1 - p)^\gamma \log(p)
     """
     ce = F.cross_entropy(logits, targets, reduction="none")  # b ...
-    scale = th.pow(1 - th.exp(-ce), gamma)
+    scale = torch.pow(1 - torch.exp(-ce), gamma)
     loss = scale * ce
     return _reduce(loss, reduction)
 
 
 class FocalLoss(nn.Module):
     def __init__(self, gamma: float) -> None:
         super().__init__()
```

### Comparing `jjuke-0.0.0.8/jjuke/options.py` & `jjuke-0.0.1.0/jjuke/options.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.8/jjuke/pointcloud/transform.py` & `jjuke-0.0.1.0/jjuke/pointcloud/transform.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.8/jjuke/sched.py` & `jjuke-0.0.1.0/jjuke/sched.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.8/jjuke/trainer.py` & `jjuke-0.0.1.0/jjuke/trainer.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.8/jjuke/utils/data.py` & `jjuke-0.0.1.0/jjuke/utils/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from math import inf
 from typing import Sequence, Union
 
-import torch as th
+import torch
 import torch.distributed as dist
 from torch.utils.data import DataLoader, Dataset, DistributedSampler
 
 __all__ = ["first", "build_dataloaders", "ChainDataset", "SubDataset", "infinite_dataloader"]
 
 
 def first(xs):
@@ -20,15 +20,15 @@
     ddp=None,
     shuffle=False,
     pin_memory=None,
     persistent_workers=None,
     **kwargs,
 ) -> Union[DataLoader, Sequence[DataLoader]]:
     if pin_memory is None:
-        pin_memory = th.cuda.is_available()
+        pin_memory = torch.cuda.is_available()
     if persistent_workers is None:
         persistent_workers = num_workers > 0
     dl_kwargs = dict(
         batch_size=batch_size,
         num_workers=num_workers,
         pin_memory=pin_memory,
         persistent_workers=persistent_workers,
```

### Comparing `jjuke-0.0.0.8/jjuke/utils/dist.py` & `jjuke-0.0.1.0/jjuke/utils/dist.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.8/jjuke/utils/indexing.py` & `jjuke-0.0.1.0/jjuke/utils/indexing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Sequence
 
-import torch as th
+import torch
 
 
 def discrete_grid_sample(p, x):
     """
     - p: b n 3
     - x: b d r r r
     """
@@ -13,29 +13,29 @@
     p = p[:, None, :].repeat(1, x.size(1), 1)  # b d n
     y = x.flatten(2).gather(-1, p)  # b d n
     y = y.transpose_(1, 2).contiguous()  # b n d
     return y
 
 
 def random_sample(x, n, dim=-1):
-    idx = th.randperm(x.size(dim))[:n]
+    idx = torch.randperm(x.size(dim))[:n]
     if dim < 0:
         dim = x.dim() + dim
     u = [slice(None) for _ in range(dim)] + [idx]
     return x[u]
 
 
 def batched_randperm(shape, dim=-1, device="cpu"):
     """adapted from https://discuss.pyth.org/t/batch-version-of-torch-randperm/111121/2"""
-    idx = th.argsort(th.rand(shape, device=device), dim=dim)
+    idx = torch.argsort(torch.rand(shape, device=device), dim=dim)
     return idx
 
 
-def unsqueeze_as(x, y) -> th.Tensor:
-    if isinstance(y, th.Tensor):
+def unsqueeze_as(x, y) -> torch.Tensor:
+    if isinstance(y, torch.Tensor):
         d = y.dim()
     else:
         d = len(y)
     return x.view(list(x.shape) + [1] * (d - x.dim()))
 
 
 def cumprod(x: Sequence):
```

### Comparing `jjuke-0.0.0.8/jjuke/utils/interp1d.py` & `jjuke-0.0.1.0/jjuke/utils/interp1d.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.8/jjuke/utils/optim.py` & `jjuke-0.0.1.0/jjuke/utils/optim.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.8/jjuke.egg-info/SOURCES.txt` & `jjuke-0.0.1.0/jjuke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.8/setup.py` & `jjuke-0.0.1.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from setuptools import find_packages, setup
 
 setup(
     name="jjuke",
-    version="0.0.0.8",
+    version="0.0.1.0",
     description="utilities for AI models with Pytorch by JJukE",
     author="JJukE",
     author_email="psj9156@gmail.com",
     url="https://github.com/JJukE/JJuk_E.git",
     packages=find_packages(),
     zip_safe=False,
     install_requires=[
         "torch",
         "numpy",
+        "trimesh",
+        "open3d==0.9.0.0",
+        "open3d-python==0.7.0.0",
         "scikit-image",
         "point_cloud_utils",
         "PyMCubes",
         "omegaconf",
         "easydict",
         "tqdm",
         "timm"
```

