# Comparing `tmp/ocnn-2.2.0.tar.gz` & `tmp/ocnn-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocnn-2.2.0.tar", last modified: Thu Feb  9 01:11:28 2023, max compression
+gzip compressed data, was "ocnn-2.2.1.tar", last modified: Mon Jun 12 07:10:17 2023, max compression
```

## Comparing `ocnn-2.2.0.tar` & `ocnn-2.2.1.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-02-09 01:11:28.373432 ocnn-2.2.0/
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     1093 2022-10-25 07:14:38.000000 ocnn-2.2.0/LICENSE
--rw-rw-r--   0 wangps    (1001) wangps    (1001)       25 2022-10-25 07:14:38.000000 ocnn-2.2.0/MANIFEST.in
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     3129 2023-02-09 01:11:28.373432 ocnn-2.2.0/PKG-INFO
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     2667 2023-02-01 02:11:12.000000 ocnn-2.2.0/README.md
-drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-02-09 01:11:28.369432 ocnn-2.2.0/ocnn/
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      558 2023-02-09 01:07:15.000000 ocnn-2.2.0/ocnn/__init__.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     5036 2022-12-01 07:10:03.000000 ocnn-2.2.0/ocnn/dataset.py
-drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-02-09 01:11:28.373432 ocnn-2.2.0/ocnn/models/
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      600 2022-10-25 07:14:38.000000 ocnn-2.2.0/ocnn/models/__init__.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     6028 2022-10-25 07:14:38.000000 ocnn-2.2.0/ocnn/models/autoencoder.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     6429 2022-12-25 05:57:42.000000 ocnn-2.2.0/ocnn/models/hrnet.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     1708 2022-10-25 07:14:38.000000 ocnn-2.2.0/ocnn/models/lenet.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     1976 2022-10-25 07:14:38.000000 ocnn-2.2.0/ocnn/models/resnet.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     2503 2022-10-25 07:14:38.000000 ocnn-2.2.0/ocnn/models/segnet.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     4018 2022-12-01 11:07:36.000000 ocnn-2.2.0/ocnn/models/unet.py
-drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-02-09 01:11:28.373432 ocnn-2.2.0/ocnn/modules/
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      800 2022-10-25 07:14:38.000000 ocnn-2.2.0/ocnn/modules/__init__.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     7433 2022-10-25 07:14:38.000000 ocnn-2.2.0/ocnn/modules/modules.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     4424 2022-10-25 07:14:38.000000 ocnn-2.2.0/ocnn/modules/resblocks.py
-drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-02-09 01:11:28.373432 ocnn-2.2.0/ocnn/nn/
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     1540 2022-12-01 06:36:57.000000 ocnn-2.2.0/ocnn/nn/__init__.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     2084 2022-10-25 07:14:38.000000 ocnn-2.2.0/ocnn/nn/octree2col.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     1474 2023-02-01 02:11:12.000000 ocnn-2.2.0/ocnn/nn/octree2vox.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)    14057 2023-02-01 02:11:12.000000 ocnn-2.2.0/ocnn/nn/octree_conv.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     1908 2022-10-25 07:14:38.000000 ocnn-2.2.0/ocnn/nn/octree_drop.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     6672 2022-10-25 07:14:38.000000 ocnn-2.2.0/ocnn/nn/octree_dwconv.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     6912 2022-10-25 07:14:38.000000 ocnn-2.2.0/ocnn/nn/octree_interp.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     1818 2022-10-25 07:14:38.000000 ocnn-2.2.0/ocnn/nn/octree_norm.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     1281 2022-10-25 07:14:38.000000 ocnn-2.2.0/ocnn/nn/octree_pad.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     6356 2022-12-15 13:29:27.000000 ocnn-2.2.0/ocnn/nn/octree_pool.py
-drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-02-09 01:11:28.373432 ocnn-2.2.0/ocnn/octree/
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      576 2022-10-25 07:14:38.000000 ocnn-2.2.0/ocnn/octree/__init__.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)    20759 2022-11-02 08:04:29.000000 ocnn-2.2.0/ocnn/octree/octree.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)    10076 2022-12-25 09:49:28.000000 ocnn-2.2.0/ocnn/octree/points.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     3821 2023-02-02 08:39:40.000000 ocnn-2.2.0/ocnn/octree/shuffled_key.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     4949 2022-12-01 06:36:57.000000 ocnn-2.2.0/ocnn/utils.py
-drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-02-09 01:11:28.369432 ocnn-2.2.0/ocnn.egg-info/
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     3129 2023-02-09 01:11:28.000000 ocnn-2.2.0/ocnn.egg-info/PKG-INFO
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      817 2023-02-09 01:11:28.000000 ocnn-2.2.0/ocnn.egg-info/SOURCES.txt
--rw-rw-r--   0 wangps    (1001) wangps    (1001)        1 2023-02-09 01:11:28.000000 ocnn-2.2.0/ocnn.egg-info/dependency_links.txt
--rw-rw-r--   0 wangps    (1001) wangps    (1001)        1 2023-02-09 01:11:28.000000 ocnn-2.2.0/ocnn.egg-info/not-zip-safe
--rw-rw-r--   0 wangps    (1001) wangps    (1001)       12 2023-02-09 01:11:28.000000 ocnn-2.2.0/ocnn.egg-info/requires.txt
--rw-rw-r--   0 wangps    (1001) wangps    (1001)        5 2023-02-09 01:11:28.000000 ocnn-2.2.0/ocnn.egg-info/top_level.txt
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      107 2023-02-09 01:11:28.373432 ocnn-2.2.0/setup.cfg
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     1158 2023-02-09 01:07:15.000000 ocnn-2.2.0/setup.py
+drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-06-12 07:10:17.611613 ocnn-2.2.1/
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     1093 2022-10-25 07:14:38.000000 ocnn-2.2.1/LICENSE
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)       25 2022-10-25 07:14:38.000000 ocnn-2.2.1/MANIFEST.in
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     3129 2023-06-12 07:10:17.611613 ocnn-2.2.1/PKG-INFO
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     2667 2023-02-01 02:11:12.000000 ocnn-2.2.1/README.md
+drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-06-12 07:10:17.603613 ocnn-2.2.1/ocnn/
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      558 2023-06-12 07:08:34.000000 ocnn-2.2.1/ocnn/__init__.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     5036 2022-12-01 07:10:03.000000 ocnn-2.2.1/ocnn/dataset.py
+drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-06-12 07:10:17.607613 ocnn-2.2.1/ocnn/models/
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      638 2023-03-17 07:35:52.000000 ocnn-2.2.1/ocnn/models/__init__.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     6077 2023-03-17 07:35:52.000000 ocnn-2.2.1/ocnn/models/autoencoder.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     6492 2023-06-12 02:38:53.000000 ocnn-2.2.1/ocnn/models/hrnet.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     1708 2022-10-25 07:14:38.000000 ocnn-2.2.1/ocnn/models/lenet.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     3209 2023-03-17 07:35:52.000000 ocnn-2.2.1/ocnn/models/ounet.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     1976 2022-10-25 07:14:38.000000 ocnn-2.2.1/ocnn/models/resnet.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     2503 2022-10-25 07:14:38.000000 ocnn-2.2.1/ocnn/models/segnet.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     4018 2022-12-01 11:07:36.000000 ocnn-2.2.1/ocnn/models/unet.py
+drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-06-12 07:10:17.607613 ocnn-2.2.1/ocnn/modules/
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      800 2022-10-25 07:14:38.000000 ocnn-2.2.1/ocnn/modules/__init__.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     7433 2022-10-25 07:14:38.000000 ocnn-2.2.1/ocnn/modules/modules.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     4424 2022-10-25 07:14:38.000000 ocnn-2.2.1/ocnn/modules/resblocks.py
+drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-06-12 07:10:17.611613 ocnn-2.2.1/ocnn/nn/
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     1665 2023-05-12 03:55:04.000000 ocnn-2.2.1/ocnn/nn/__init__.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     2084 2022-10-25 07:14:38.000000 ocnn-2.2.1/ocnn/nn/octree2col.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     1474 2023-02-01 02:11:12.000000 ocnn-2.2.1/ocnn/nn/octree2vox.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     1650 2023-03-23 01:57:43.000000 ocnn-2.2.1/ocnn/nn/octree_align.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)    14057 2023-02-01 02:11:12.000000 ocnn-2.2.1/ocnn/nn/octree_conv.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     1908 2022-10-25 07:14:38.000000 ocnn-2.2.1/ocnn/nn/octree_drop.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     6672 2022-10-25 07:14:38.000000 ocnn-2.2.1/ocnn/nn/octree_dwconv.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     6912 2022-10-25 07:14:38.000000 ocnn-2.2.1/ocnn/nn/octree_interp.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     2890 2023-05-12 03:55:04.000000 ocnn-2.2.1/ocnn/nn/octree_norm.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     1281 2022-10-25 07:14:38.000000 ocnn-2.2.1/ocnn/nn/octree_pad.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     6464 2023-04-03 00:43:37.000000 ocnn-2.2.1/ocnn/nn/octree_pool.py
+drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-06-12 07:10:17.611613 ocnn-2.2.1/ocnn/octree/
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      576 2022-10-25 07:14:38.000000 ocnn-2.2.1/ocnn/octree/__init__.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)    21497 2023-05-12 00:22:04.000000 ocnn-2.2.1/ocnn/octree/octree.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)    10076 2022-12-25 09:49:28.000000 ocnn-2.2.1/ocnn/octree/points.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     3821 2023-02-02 08:39:40.000000 ocnn-2.2.1/ocnn/octree/shuffled_key.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     4949 2022-12-01 06:36:57.000000 ocnn-2.2.1/ocnn/utils.py
+drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-06-12 07:10:17.607613 ocnn-2.2.1/ocnn.egg-info/
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     3129 2023-06-12 07:10:17.000000 ocnn-2.2.1/ocnn.egg-info/PKG-INFO
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      862 2023-06-12 07:10:17.000000 ocnn-2.2.1/ocnn.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)        1 2023-06-12 07:10:17.000000 ocnn-2.2.1/ocnn.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)        1 2023-02-09 01:11:28.000000 ocnn-2.2.1/ocnn.egg-info/not-zip-safe
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)       12 2023-06-12 07:10:17.000000 ocnn-2.2.1/ocnn.egg-info/requires.txt
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)        5 2023-06-12 07:10:17.000000 ocnn-2.2.1/ocnn.egg-info/top_level.txt
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      107 2023-06-12 07:10:17.611613 ocnn-2.2.1/setup.cfg
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     1158 2023-06-12 07:08:34.000000 ocnn-2.2.1/setup.py
```

### Comparing `ocnn-2.2.0/LICENSE` & `ocnn-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/PKG-INFO` & `ocnn-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocnn
-Version: 2.2.0
+Version: 2.2.1
 Summary: Octree-based Sparse Convolutional Neural Networks
 Home-page: https://github.com/octree-nn/ocnn-pytorch
 Author: Peng-Shuai Wang
 Author-email: wangps@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ocnn-2.2.0/README.md` & `ocnn-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/__init__.py` & `ocnn-2.2.1/ocnn/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from . import octree
 from . import nn
 from . import modules
 from . import models
 from . import dataset
 from . import utils
 
-__version__ = '2.2.0'
+__version__ = '2.2.1'
 
 __all__ = [
     'octree',
     'nn',
     'modules',
     'models',
     'dataset',
```

### Comparing `ocnn-2.2.0/ocnn/dataset.py` & `ocnn-2.2.1/ocnn/dataset.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/models/autoencoder.py` & `ocnn-2.2.1/ocnn/models/autoencoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,39 +22,39 @@
     depth (int): The depth of the octree.
     full_depth (int): The full depth of the octree.
     feature (str): The feature type of the input signal. For details of this
         argument, please refer to :class:`ocnn.modules.InputFeature`.
   '''
 
   def __init__(self, channel_in: int, channel_out: int, depth: int,
-               full_depth: int = 2, feature: str = 'ND'):
+               full_depth: int = 2, feature: str = 'ND', code_channel: int = 128):
     super().__init__()
     self.channel_in = channel_in
     self.channel_out = channel_out
     self.depth = depth
     self.full_depth = full_depth
     self.feature = feature
     self.resblk_num = 2
-    self.shape_code_channel = 128
     self.channels = [512, 512, 256, 256, 128, 128, 32, 32, 16, 16]
+    self.code_channel = code_channel if code_channel > 0 else self.channels[full_depth]
 
     # encoder
     self.conv1 = ocnn.modules.OctreeConvBnRelu(
         channel_in, self.channels[depth], nempty=False)
     self.encoder_blks = torch.nn.ModuleList([ocnn.modules.OctreeResBlocks(
         self.channels[d], self.channels[d], self.resblk_num, nempty=False)
         for d in range(depth, full_depth-1, -1)])
     self.downsample = torch.nn.ModuleList([ocnn.modules.OctreeConvBnRelu(
         self.channels[d], self.channels[d-1], kernel_size=[2], stride=2,
         nempty=False) for d in range(depth, full_depth, -1)])
     self.proj = torch.nn.Linear(
-        self.channels[full_depth], self.shape_code_channel, bias=True)
+        self.channels[full_depth], self.code_channel, bias=True)
 
     # decoder
-    self.channels[full_depth] = self.shape_code_channel  # update `channels`
+    self.channels[full_depth] = self.code_channel  # update `channels`
     self.upsample = torch.nn.ModuleList([ocnn.modules.OctreeDeconvBnRelu(
         self.channels[d-1], self.channels[d], kernel_size=[2], stride=2,
         nempty=False) for d in range(full_depth+1, depth+1)])
     self.decoder_blks = torch.nn.ModuleList([ocnn.modules.OctreeResBlocks(
         self.channels[d], self.channels[d], self.resblk_num, nempty=False)
         for d in range(full_depth, depth+1)])
 
@@ -73,15 +73,15 @@
     '''
 
     octree_feature = ocnn.modules.InputFeature(self.feature, nempty=False)
     out = octree_feature(octree)
     assert out.size(1) == self.channel_in
     return out
 
-  def ae_encoder(self, octree: Octree):
+  def encoder(self, octree: Octree):
     r''' The encoder network of the AutoEncoder.
     '''
 
     convs = dict()
     depth, full_depth = self.depth, self.full_depth
     data = self.get_input_feature(octree)
     convs[depth] = self.conv1(data, octree, depth)
@@ -90,16 +90,16 @@
       if d > full_depth:
         convs[d-1] = self.downsample[i](convs[d], octree, d)
 
     # NOTE: here tanh is used to constrain the shape code in [-1, 1]
     shape_code = self.proj(convs[full_depth]).tanh()
     return shape_code
 
-  def ae_decoder(self, shape_code: torch.Tensor, octree: Octree,
-                 update_octree: bool = False):
+  def decoder(self, shape_code: torch.Tensor, octree: Octree,
+              update_octree: bool = False):
     r''' The decoder network of the AutoEncoder.
     '''
 
     logits = dict()
     deconv = shape_code
     depth, full_depth = self.depth, self.full_depth
     for i, d in enumerate(range(full_depth, depth+1)):
@@ -132,15 +132,15 @@
     r''' Decodes the shape code to an output octree.
 
     Args:
       shape_code (torch.Tensor): The shape code for decoding.
     '''
 
     octree_out = self.init_octree(shape_code)
-    out = self.ae_decoder(shape_code, octree_out, update_octree=True)
+    out = self.decoder(shape_code, octree_out, update_octree=True)
     return out
 
   def init_octree(self, shape_code: torch.Tensor):
     r''' Initialize a full octree for decoding.
 
     Args:
       shape_code (torch.Tensor): The shape code for decoding, used to getting 
@@ -154,12 +154,12 @@
     for d in range(self.full_depth+1):
       octree.octree_grow_full(depth=d)
     return octree
 
   def forward(self, octree: Octree, update_octree: bool):
     r''''''
 
-    shape_code = self.ae_encoder(octree)
+    shape_code = self.encoder(octree)
     if update_octree:
       octree = self.init_octree(shape_code)
-    out = self.ae_decoder(shape_code, octree, update_octree)
+    out = self.decoder(shape_code, octree, update_octree)
     return out
```

### Comparing `ocnn-2.2.0/ocnn/models/hrnet.py` & `ocnn-2.2.1/ocnn/models/hrnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,20 +136,21 @@
     #     ocnn.modules.FcBnRelu(512, 256),
     #     torch.nn.Dropout(p=0.5),
     #     torch.nn.Linear(256, out_channels))
 
   def forward(self, data: List[torch.Tensor], octree: Octree, depth: int):
     full_depth = 2
     num = len(data)
+    outs = [x for x in data]  # avoid modifying the input data
     for i in range(num):
       depth_i = depth - i
       for d in range(depth_i, full_depth, -1):
-        data[i] = ocnn.nn.octree_max_pool(data[i], octree, d, self.nempty)
+        outs[i] = ocnn.nn.octree_max_pool(outs[i], octree, d, self.nempty)
 
-    out = torch.cat(data, dim=1)
+    out = torch.cat(outs, dim=1)
     out = self.conv1x1(out)
     out = self.global_pool(out, octree, full_depth)
     logit = self.header(out)
     return logit
 
 
 class HRNet(torch.nn.Module):
```

### Comparing `ocnn-2.2.0/ocnn/models/lenet.py` & `ocnn-2.2.1/ocnn/models/lenet.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/models/resnet.py` & `ocnn-2.2.1/ocnn/models/resnet.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/models/segnet.py` & `ocnn-2.2.1/ocnn/models/segnet.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/models/unet.py` & `ocnn-2.2.1/ocnn/models/unet.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/modules/__init__.py` & `ocnn-2.2.1/ocnn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/modules/modules.py` & `ocnn-2.2.1/ocnn/modules/modules.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/modules/resblocks.py` & `ocnn-2.2.1/ocnn/modules/resblocks.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/nn/__init__.py` & `ocnn-2.2.1/ocnn/nn/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,17 @@
                             OctreeInterp, OctreeUpsample)
 from .octree_pool import (octree_max_pool, OctreeMaxPool,
                           octree_max_unpool, OctreeMaxUnpool,
                           octree_global_pool, OctreeGlobalPool,
                           octree_avg_pool, OctreeAvgPool,)
 from .octree_conv import OctreeConv, OctreeDeconv
 from .octree_dwconv import OctreeDWConv
-from .octree_norm import OctreeInstanceNorm, OctreeBatchNorm
+from .octree_norm import OctreeBatchNorm, OctreeGroupNorm, OctreeInstanceNorm
 from .octree_drop import OctreeDropPath
+from .octree_align import search_value, octree_align
 
 
 __all__ = [
     'octree2voxel',
     'octree2col', 'col2octree',
     'octree_pad', 'octree_depad',
     'octree_nearest_pts', 'octree_linear_pts',
@@ -29,12 +30,13 @@
     'octree_global_pool', 'octree_avg_pool',
     'Octree2Voxel',
     'OctreeMaxPool', 'OctreeMaxUnpool',
     'OctreeGlobalPool', 'OctreeAvgPool',
     'OctreeConv', 'OctreeDeconv',
     'OctreeDWConv',
     'OctreeInterp', 'OctreeUpsample',
-    'OctreeInstanceNorm', 'OctreeBatchNorm',
+    'OctreeInstanceNorm', 'OctreeBatchNorm', 'OctreeGroupNorm',
     'OctreeDropPath',
+    'search_value', 'octree_align',
 ]
 
 classes = __all__
```

### Comparing `ocnn-2.2.0/ocnn/nn/octree2col.py` & `ocnn-2.2.1/ocnn/nn/octree2col.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/nn/octree2vox.py` & `ocnn-2.2.1/ocnn/nn/octree2vox.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/nn/octree_conv.py` & `ocnn-2.2.1/ocnn/nn/octree_conv.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/nn/octree_drop.py` & `ocnn-2.2.1/ocnn/nn/octree_drop.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/nn/octree_dwconv.py` & `ocnn-2.2.1/ocnn/nn/octree_dwconv.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/nn/octree_interp.py` & `ocnn-2.2.1/ocnn/nn/octree_interp.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/nn/octree_norm.py` & `ocnn-2.2.1/ocnn/nn/octree_norm.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,25 +11,28 @@
 from ocnn.octree import Octree
 from ocnn.utils import scatter_add
 
 
 OctreeBatchNorm = torch.nn.BatchNorm1d
 
 
-class OctreeInstanceNorm(torch.nn.Module):
-  r''' An instance normalization layer for the octree.
+class OctreeGroupNorm(torch.nn.Module):
+  r''' An group normalization layer for the octree.
   '''
 
-  def __init__(self, in_channels: int, nempty: bool = False):
+  def __init__(self, in_channels: int, group: int, nempty: bool = False):
     super().__init__()
-
     self.eps = 1e-5
     self.nempty = nempty
+    self.group = group
     self.in_channels = in_channels
 
+    assert in_channels % group == 0
+    self.channels_per_group = in_channels // group
+
     self.weights = torch.nn.Parameter(torch.Tensor(1, in_channels))
     self.bias = torch.nn.Parameter(torch.Tensor(1, in_channels))
     self.reset_parameters()
 
   def reset_parameters(self):
     torch.nn.init.ones_(self.weights)
     torch.nn.init.zeros_(self.bias)
@@ -37,20 +40,47 @@
   def forward(self, data: torch.Tensor, octree: Octree, depth: int):
     r''''''
 
     batch_size = octree.batch_size
     batch_id = octree.batch_id(depth, self.nempty)
     ones = data.new_ones([data.shape[0], 1])
     count = scatter_add(ones, batch_id, dim=0, dim_size=batch_size)
-    norm = 1.0 / (count + self.eps)  # there might be 0 element in some shapes
+    count = count * self.channels_per_group  # element number in each group
+    inv_count = 1.0 / (count + self.eps)  # there might be 0 element sometimes
 
-    mean = scatter_add(data, batch_id, dim=0, dim_size=batch_size) * norm
+    mean = scatter_add(data, batch_id, dim=0, dim_size=batch_size) * inv_count
+    mean = self._adjust_for_group(mean)
     out = data - mean.index_select(0, batch_id)
-    var = scatter_add(out * out, batch_id, dim=0, dim_size=batch_size) * norm
+
+    var = scatter_add(out**2, batch_id, dim=0, dim_size=batch_size) * inv_count
+    var = self._adjust_for_group(var)
     inv_std = 1.0 / (var + self.eps).sqrt()
     out = out * inv_std.index_select(0, batch_id)
 
     out = out * self.weights + self.bias
     return out
 
+  def _adjust_for_group(self, tensor: torch.Tensor):
+    r''' Adjust the tensor for the group.
+    '''
+
+    if self.channels_per_group > 1:
+      tensor = (tensor.reshape(-1, self.group, self.channels_per_group)
+                      .sum(-1, keepdim=True)
+                      .repeat(1, 1, self.channels_per_group)
+                      .reshape(-1, self.in_channels))
+    return tensor
+
+  def extra_repr(self) -> str:
+    return ('in_channels={}, group={}, nempty={}').format(
+            self.in_channels, self.group, self.nempty)  # noqa
+
+
+class OctreeInstanceNorm(OctreeGroupNorm):
+  r''' An instance normalization layer for the octree.
+  '''
+
+  def __init__(self, in_channels: int, nempty: bool = False):
+    super().__init__(in_channels=in_channels, group=in_channels, nempty=nempty)
+
   def extra_repr(self) -> str:
     return ('in_channels={}, nempty={}').format(self.in_channels, self.nempty)
```

### Comparing `ocnn-2.2.0/ocnn/nn/octree_pad.py` & `ocnn-2.2.1/ocnn/nn/octree_pad.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/nn/octree_pool.py` & `ocnn-2.2.1/ocnn/nn/octree_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,17 @@
 
 class OctreeMaxUnpool(OctreePoolBase):
   r''' Performs octree max unpooling.
 
   Please refer to :func:`octree_max_unpool` for details.
   '''
 
+  def __init__(self, nempty: bool = False):
+    super().__init__(kernel_size=[2], stride=2, nempty=nempty)
+
   def forward(self, data: torch.Tensor, indices: torch.Tensor, octree: Octree,
               depth: int):
     r''''''
 
     return octree_max_unpool(data, indices, octree, depth, self.nempty)
```

### Comparing `ocnn-2.2.0/ocnn/octree/__init__.py` & `ocnn-2.2.1/ocnn/octree/__init__.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/octree/octree.py` & `ocnn-2.2.1/ocnn/octree/octree.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     .. note::
       Currently, the batch size of the point cloud must be 1.
     '''
 
     self.device = point_cloud.device
     assert point_cloud.batch_size == self.batch_size, 'Inconsistent batch_size'
 
-    # normalize points from [-1, 1] to [0, 2^depth]. #[Lable:S]
+    # normalize points from [-1, 1] to [0, 2^depth]. #[L:Scale]
     scale = 2 ** (self.depth - 1)
     points = (point_cloud.points + 1.0) * scale
 
     # get the shuffled key and sort
     x, y, z = points[:, 0], points[:, 1], points[:, 2]
     b = None if self.batch_size == 1 else point_cloud.batch_id.view(-1)
     key = xyz2key(x, y, z, b, self.depth)
@@ -207,15 +207,15 @@
     children[nempty_idx] = torch.arange(
         node_key.numel(), dtype=torch.int32, device=self.device)
     self.children[d] = children
     self.nnum_nempty[d] = node_key.numel()
 
     # average the signal for the last octree layer
     d = self.depth
-    points = scatter_add(points, idx, dim=0)  # points is rescaled in [Lable:S]
+    points = scatter_add(points, idx, dim=0)  # points is rescaled in [L:Scale]
     self.points[d] = points / counts.unsqueeze(1)
     if point_cloud.normals is not None:
       normals = scatter_add(point_cloud.normals, idx, dim=0)
       self.normals[d] = F.normalize(normals)
     if point_cloud.features is not None:
       features = scatter_add(point_cloud.features, idx, dim=0)
       self.features[d] = features / counts.unsqueeze(1)
@@ -403,15 +403,15 @@
       nempty (bool): If True, only returns the neighborhoods of the non-empty
           octree nodes.
     '''
 
     if stride == 1:
       neigh = self.neighs[depth]
     elif stride == 2:
-      # clone neigh to avoid self.neigh[depth] being modified (such as in L282)
+      # clone neigh to avoid self.neigh[depth] being modified
       neigh = self.neighs[depth][::8].clone()
     else:
       raise ValueError('Unsupported stride {}'.format(stride))
 
     if nempty:
       child = self.children[depth]
       if stride == 1:
@@ -449,23 +449,43 @@
 
     # features
     if self.features[depth] is not None:
       features.append(self.features[depth])
 
     return torch.cat(features, dim=1)
 
-  def to_points(self):
+  def to_points(self, rescale: bool = True):
     r''' Converts averaged points in the octree to a point cloud.
+
+    Args:
+      rescale (bool): rescale the xyz coordinates to [-1, 1] if True.
     '''
 
-    d = self.depth
-    scale = 2 ** (1-d)
-    # normalize to [-1, 1] since the average points are in range [0, 2^d]
-    points = self.points[d] * scale - 1.0
-    return Points(points, self.normals[d], self.features[d])
+    depth = self.depth
+    batch_size = self.batch_size
+
+    # by default, use the average points generated when building the octree
+    # from the input point cloud
+    xyz = self.points[depth]
+    batch_id = self.batch_id(depth, nempty=True)
+
+    # xyz is None when the octree is predicted by a neural network
+    if xyz is None:
+      x, y, z, batch_id = self.xyzb(depth, nempty=True)
+      xyz = torch.stack([x, y, z], dim=1) + 0.5
+
+    # normalize xyz to [-1, 1] since the average points are in range [0, 2^d]
+    if rescale:
+      scale = 2 ** (1 - depth)
+      xyz = self.points[depth] * scale - 1.0
+
+    # construct Points
+    out = Points(xyz, self.normals[depth], self.features[depth],
+                 batch_id=batch_id, batch_size=batch_size)
+    return out
 
   def to(self, device: Union[torch.device, str], non_blocking: bool = False):
     r''' Moves the octree to a specified device.
 
     Args:
       device (torch.device or str): The destination device.
       non_blocking (bool): If True and the source is in pinned memory, the copy
@@ -553,16 +573,16 @@
       key = octrees[i].keys[d] & ((1 << 48) - 1)  # clear the highest bits
       keys[i] = key | (i << 48)
     octree.keys[d] = torch.cat(keys, dim=0)
 
     # children
     children = [None] * octree.batch_size
     for i in range(octree.batch_size):
-      child = octrees[i].children[d]
-      mask = child >= 0
+      child = octrees[i].children[d].clone()  # !! `clone` is used here to avoid
+      mask = child >= 0                       # !! modifying the original octrees
       child[mask] = child[mask] + nnum_cum[d, i]
       children[i] = child
     octree.children[d] = torch.cat(children, dim=0)
 
     # features
     if octrees[0].features[d] is not None and d == octree.depth:
       features = [octrees[i].features[d] for i in range(octree.batch_size)]
```

### Comparing `ocnn-2.2.0/ocnn/octree/points.py` & `ocnn-2.2.1/ocnn/octree/points.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/octree/shuffled_key.py` & `ocnn-2.2.1/ocnn/octree/shuffled_key.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn/utils.py` & `ocnn-2.2.1/ocnn/utils.py`

 * *Files identical despite different names*

### Comparing `ocnn-2.2.0/ocnn.egg-info/PKG-INFO` & `ocnn-2.2.1/ocnn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocnn
-Version: 2.2.0
+Version: 2.2.1
 Summary: Octree-based Sparse Convolutional Neural Networks
 Home-page: https://github.com/octree-nn/ocnn-pytorch
 Author: Peng-Shuai Wang
 Author-email: wangps@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ocnn-2.2.0/ocnn.egg-info/SOURCES.txt` & `ocnn-2.2.1/ocnn.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,23 +12,25 @@
 ocnn.egg-info/not-zip-safe
 ocnn.egg-info/requires.txt
 ocnn.egg-info/top_level.txt
 ocnn/models/__init__.py
 ocnn/models/autoencoder.py
 ocnn/models/hrnet.py
 ocnn/models/lenet.py
+ocnn/models/ounet.py
 ocnn/models/resnet.py
 ocnn/models/segnet.py
 ocnn/models/unet.py
 ocnn/modules/__init__.py
 ocnn/modules/modules.py
 ocnn/modules/resblocks.py
 ocnn/nn/__init__.py
 ocnn/nn/octree2col.py
 ocnn/nn/octree2vox.py
+ocnn/nn/octree_align.py
 ocnn/nn/octree_conv.py
 ocnn/nn/octree_drop.py
 ocnn/nn/octree_dwconv.py
 ocnn/nn/octree_interp.py
 ocnn/nn/octree_norm.py
 ocnn/nn/octree_pad.py
 ocnn/nn/octree_pool.py
```

### Comparing `ocnn-2.2.0/setup.py` & `ocnn-2.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (c) 2022 Peng-Shuai Wang <wangps@hotmail.com>
 # Licensed under The MIT License [see LICENSE for details]
 # Written by Peng-Shuai Wang
 # --------------------------------------------------------
 
 from setuptools import setup, find_packages
 
-__version__ = '2.2.0'
+__version__ = '2.2.1'
 
 with open("README.md", "r", encoding="utf-8") as fid:
   long_description = fid.read()
 
 setup(
     name='ocnn',
     version=__version__,
```

