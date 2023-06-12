# Comparing `tmp/dtorch-0.0.3.tar.gz` & `tmp/dtorch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtorch-0.0.3.tar", last modified: Wed Jun  7 08:43:01 2023, max compression
+gzip compressed data, was "dtorch-0.0.4.tar", last modified: Mon Jun 12 12:10:01 2023, max compression
```

## Comparing `dtorch-0.0.3.tar` & `dtorch-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-07 08:43:01.488733 dtorch-0.0.3/
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1067 2023-06-06 07:48:12.000000 dtorch-0.0.3/LICENSE
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2639 2023-06-07 08:43:01.488733 dtorch-0.0.3/PKG-INFO
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2131 2023-06-07 08:42:05.000000 dtorch-0.0.3/README.md
-drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-07 08:43:01.488733 dtorch-0.0.3/dtorch/
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      176 2023-06-06 10:00:04.000000 dtorch-0.0.3/dtorch/__init__.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1146 2023-06-06 10:00:04.000000 dtorch-0.0.3/dtorch/dataset.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    13723 2023-06-06 10:00:04.000000 dtorch-0.0.3/dtorch/derivatives.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1979 2023-06-06 10:00:04.000000 dtorch-0.0.3/dtorch/einops.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     8970 2023-06-06 10:00:04.000000 dtorch-0.0.3/dtorch/functionnal.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    10586 2023-06-06 10:00:04.000000 dtorch-0.0.3/dtorch/jtensors.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2691 2023-06-06 10:00:04.000000 dtorch-0.0.3/dtorch/loss.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    11642 2023-06-06 10:00:04.000000 dtorch-0.0.3/dtorch/nn.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      218 2023-06-06 10:00:04.000000 dtorch-0.0.3/dtorch/operation_class.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      940 2023-06-06 10:00:04.000000 dtorch-0.0.3/dtorch/operations.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2698 2023-06-06 10:00:04.000000 dtorch-0.0.3/dtorch/optim.py
-drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-07 08:43:01.488733 dtorch-0.0.3/dtorch.egg-info/
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2639 2023-06-07 08:43:01.000000 dtorch-0.0.3/dtorch.egg-info/PKG-INFO
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      360 2023-06-07 08:43:01.000000 dtorch-0.0.3/dtorch.egg-info/SOURCES.txt
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        1 2023-06-07 08:43:01.000000 dtorch-0.0.3/dtorch.egg-info/dependency_links.txt
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        7 2023-06-07 08:43:01.000000 dtorch-0.0.3/dtorch.egg-info/top_level.txt
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      616 2023-06-07 08:42:31.000000 dtorch-0.0.3/pyproject.toml
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)       38 2023-06-07 08:43:01.488733 dtorch-0.0.3/setup.cfg
+drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-12 12:10:01.642850 dtorch-0.0.4/
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1067 2023-06-06 07:48:12.000000 dtorch-0.0.4/LICENSE
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2642 2023-06-12 12:10:01.642850 dtorch-0.0.4/PKG-INFO
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2134 2023-06-07 09:47:40.000000 dtorch-0.0.4/README.md
+drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-12 12:10:01.642850 dtorch-0.0.4/dtorch/
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      203 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/__init__.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1146 2023-06-06 10:00:04.000000 dtorch-0.0.4/dtorch/dataset.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    16603 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/derivatives.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2096 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/einops.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    17143 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/functionnal.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    12424 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/jtensors.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2679 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/loss.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    13038 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/nn.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      218 2023-06-08 10:17:42.000000 dtorch-0.0.4/dtorch/operation_class.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      940 2023-06-06 10:00:04.000000 dtorch-0.0.4/dtorch/operations.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     7914 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/optim.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1606 2023-06-12 11:58:25.000000 dtorch-0.0.4/dtorch/typing.py
+drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-12 12:10:01.642850 dtorch-0.0.4/dtorch.egg-info/
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2642 2023-06-12 12:10:01.000000 dtorch-0.0.4/dtorch.egg-info/PKG-INFO
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      377 2023-06-12 12:10:01.000000 dtorch-0.0.4/dtorch.egg-info/SOURCES.txt
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        1 2023-06-12 12:10:01.000000 dtorch-0.0.4/dtorch.egg-info/dependency_links.txt
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        7 2023-06-12 12:10:01.000000 dtorch-0.0.4/dtorch.egg-info/top_level.txt
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      616 2023-06-12 11:58:25.000000 dtorch-0.0.4/pyproject.toml
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)       38 2023-06-12 12:10:01.642850 dtorch-0.0.4/setup.cfg
```

### Comparing `dtorch-0.0.3/LICENSE` & `dtorch-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.3/PKG-INFO` & `dtorch-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: A scientific package made a fellow student
 Author-email: Just1truc <hyppoduc@gmail.com>
 Project-URL: Homepage, https://github.com/Just1truc/dtorch
 Project-URL: Bug Tracker, https://github.com/Just1truc/dtorch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 # DTorch
 
 A direct link to the package : [here](https://pypi.org/project/dtorch/)
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Just1truc/dtorch/main/.asset/2023-06-07-09%2038%2034-screenshot.png" data-canonical-src="https://raw.githubusercontent.com/Just1truc/dtorch/main/.asset/2023-06-07-09%2038%2034-screenshot.png" width="200" height="200"/></p>
 
-DTorch is a package made a student at Epitech to improve his understanding of **pytorch** and better his knowledge of ia.
+DTorch is a package made by a student at Epitech to improve his understanding of **pytorch** and better his knowledge of ia.
 It is built on top of **numpy** which is a scientific framework for math between matrices.
 
 This project run on cpu but still have decent computation time making it usable for model building, optimization and saving/loading.
 
 The tensors created can work with numpy but remember that the gradients will **not be calculated** if the operation are not in the range of control of the library. Therefore, a usage of the packages methods on the tensors if preferable.
 
 **Cuda** support may appear in the future and similarly for the dkldnn library that seems to be an excellent when working on CPU.
```

### Comparing `dtorch-0.0.3/README.md` & `dtorch-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # DTorch
 
 A direct link to the package : [here](https://pypi.org/project/dtorch/)
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Just1truc/dtorch/main/.asset/2023-06-07-09%2038%2034-screenshot.png" data-canonical-src="https://raw.githubusercontent.com/Just1truc/dtorch/main/.asset/2023-06-07-09%2038%2034-screenshot.png" width="200" height="200"/></p>
 
-DTorch is a package made a student at Epitech to improve his understanding of **pytorch** and better his knowledge of ia.
+DTorch is a package made by a student at Epitech to improve his understanding of **pytorch** and better his knowledge of ia.
 It is built on top of **numpy** which is a scientific framework for math between matrices.
 
 This project run on cpu but still have decent computation time making it usable for model building, optimization and saving/loading.
 
 The tensors created can work with numpy but remember that the gradients will **not be calculated** if the operation are not in the range of control of the library. Therefore, a usage of the packages methods on the tensors if preferable.
 
 **Cuda** support may appear in the future and similarly for the dkldnn library that seems to be an excellent when working on CPU.
```

### Comparing `dtorch-0.0.3/dtorch/dataset.py` & `dtorch-0.0.4/dtorch/dataset.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.3/dtorch/derivatives.py` & `dtorch-0.0.4/dtorch/derivatives.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,41 @@
 """ imports """
 import dtorch.jtensors
 import numpy as np
 from typing import Tuple
 
 
+def as_strided_deriv(base_tensor, *tensors):
+
+    # TODO: fix this
+
+    tensor : dtorch.jtensors.JTensors = tensors[0]
+    shape : Tuple[int] = tensors[1]
+    strides : Tuple[int] = tensors[2]
+
+    if (tensor.require_grads):
+        indexes = np.lib.stride_tricks.as_strided(np.arange(tensor().size), shape=shape, strides=strides)
+        res = np.bincount(indexes.ravel(), base_tensor().ravel())
+        res.resize(tensor.shape)
+        restrided_base_tensor = np.lib.stride_tricks.as_strided(base_tensor(), shape=tensor.shape, strides=tensor.stride)
+        if (tensor.isLeaf()):
+            tensor.grad += dtorch.jtensors.JTensors(res)
+        else:
+            tensor.grad = dtorch.jtensors.JTensors(res)
+        tensor.backward(tensor.grad, forced=True)
+
 """ Complex """
 
 def unsqueeze_backward(base_tensor, *tensors):
     
     tensor : dtorch.jtensors.JTensors = tensors[0]
     dim : int = tensors[1]
 
     if (tensor.require_grads):
-        grad = dtorch.jtensors.JTensors(np.sum(base_tensor(), axis=dim, keepdims=1))
+        grad = dtorch.jtensors.JTensors(np.squeeze(np.sum(base_tensor(), axis=dim, keepdims=True), axis=dim))
         if (tensor.isLeaf()):
             tensor.grad += grad
         else:
             tensor.grad = grad
         tensor.backward(tensor.grad, forced=True)
 
 
@@ -52,15 +71,15 @@
 
     tensor : dtorch.jtensors.JTensors = tensors[0]
 
     if (tensor.require_grads):
         if (tensor.isLeaf()):
             tensor.grad += dtorch.jtensors.JTensors(base_tensor() * (1 / (2 * np.sqrt(tensor()))))
         else:
-            tensor.grad = dtorch.jtensors.JTensors(base_tensor() * (1 / tensor()))
+            tensor.grad = dtorch.jtensors.JTensors(base_tensor() * (1 / (2 * np.sqrt(tensor()))))
         tensor.backward(tensor.grad, forced=True)
 
 
 def real_max_deriv(base_tensor, *tensors):
 
     tensor : dtorch.jtensors.JTensors = tensors[0]
 
@@ -109,36 +128,43 @@
 # just a matrix on what parameters depend on
 def matmul_deriv(base_tensor, *tensors):
     left : dtorch.jtensors.JTensors = tensors[0]
     right : dtorch.jtensors.JTensors = tensors[1]
 
     if (left.require_grads):
         if (left.isLeaf()):
-            left.grad += dtorch.jtensors.JTensors(np.matmul(base_tensor(), right().T))
+            left.grad += dtorch.jtensors.JTensors(np.matmul(base_tensor(), np.swapaxes(right(), -1, -2)).reshape(left.shape))
         else:
-            left.grad = dtorch.jtensors.JTensors(np.matmul(base_tensor(), right().T))
+            left.grad = dtorch.jtensors.JTensors(np.matmul(base_tensor(), np.swapaxes(right(), -2, -1)).reshape(left.shape))
         left.backward(left.grad, forced=True)
 
     if (right.require_grads):
         if (right.isLeaf()):
-            right.grad += dtorch.jtensors.JTensors(np.matmul(left().T, base_tensor()))
+            right.grad += dtorch.jtensors.JTensors(np.matmul(np.swapaxes(left(), -1, -2), base_tensor()).reshape(right.shape))
         else:
-            right.grad = dtorch.jtensors.JTensors(np.matmul(left().T, base_tensor()))
+            right.grad = dtorch.jtensors.JTensors(np.matmul(np.swapaxes(left(), -1, -2), base_tensor()).reshape(right.shape))
         right.backward(right.grad, forced=True)
 
 
 def sum_deriv(base_tensor, *tensors):
     from_tensor : dtorch.jtensors.JTensors = tensors[0]
+    axis : Tuple[int] = tensors[1]
 
     if (from_tensor.require_grads):
-        tensor = dtorch.jtensors.JTensors(np.lib.stride_tricks.as_strided(np.ones(from_tensor.shape()), shape=from_tensor.shape(), strides=from_tensor.stride()))
+        #tensor = dtorch.jtensors.JTensors(np.lib.stride_tricks.as_strided(np.ones(from_tensor.shape), shape=from_tensor.shape, strides=from_tensor.stride))
+        k = base_tensor.numpy().copy()
+        if (axis is not None):
+            o = np.array(from_tensor.shape)
+            o[list(axis)] = np.ones(len(axis), dtype=int)
+            k = k.reshape(tuple(o))
+        k = np.broadcast_to(k, from_tensor.shape)
         if (from_tensor.isLeaf()):
-            from_tensor.grad += dtorch.jtensors.JTensors(base_tensor() * tensor())
+            from_tensor.grad += dtorch.jtensors.JTensors(k)
         else:
-            from_tensor.grad = dtorch.jtensors.JTensors(base_tensor() * tensor())
+            from_tensor.grad = dtorch.jtensors.JTensors(k)
         from_tensor.backward(from_tensor.grad, forced=True)
 
 
 """ Basics """
 
 def exp_deriv(base_tensor, *tensors):
 
@@ -160,55 +186,81 @@
         if (tensor.isLeaf()):
             tensor.grad += dtorch.jtensors.JTensors(base_tensor() *  (1 / (tensor())))
         else:
             tensor.grad = dtorch.jtensors.JTensors(base_tensor() *  (1 / (tensor())))
         tensor.backward(tensor.grad, forced=True)
 
 
-def mul_deriv(base_tensor, *tensors):
-
-    unpacked_tensors : list[dtorch.jtensors.JTensors | float | int] = list(tensors)
-    is_tensor : bool = isinstance(unpacked_tensors[1], dtorch.jtensors.JTensors)
-
-    if (unpacked_tensors[0].require_grads):
-        if (unpacked_tensors[0].isLeaf()):
-            unpacked_tensors[0].grad += dtorch.jtensors.JTensors(base_tensor() * (unpacked_tensors[1]() if is_tensor else unpacked_tensors[1]))
-        else:
-            unpacked_tensors[0].grad = dtorch.jtensors.JTensors(base_tensor() * (unpacked_tensors[1]() if is_tensor else unpacked_tensors[1]))
-        unpacked_tensors[0].backward(unpacked_tensors[0].grad, forced = True)
-    
-    if (is_tensor and unpacked_tensors[1].require_grads):
-        if (unpacked_tensors[1].isLeaf()):
-            unpacked_tensors[1].grad += dtorch.jtensors.JTensors(base_tensor() * unpacked_tensors[0]())
-        else:
-            unpacked_tensors[1].grad = dtorch.jtensors.JTensors(base_tensor() * unpacked_tensors[0]())
-        unpacked_tensors[1].backward(unpacked_tensors[1].grad, forced = True)
-
-
 def dimensionToSum(left : Tuple[int], right : Tuple[int]) -> Tuple[int]:
 
     left = list(left)
     right = list(right)
     r = 0
     l = 0
+    to_sum_left = []
 
-    while (r < len(right)):
+    while (l < len(left)):
+        if (r >= len(right)):
+            l += 1
+            to_sum_left.append(len(left) - l)
+            continue
         if (right[-1 - r] == 1):
             r += 1
+            l += 1
+            to_sum_left.append(len(left) - l)
             continue
         if (left[-1 -l] == 1):
             l += 1
+            r += 1
             continue
         if (left[-1 -l] == right[-1 -r]):
             r += 1
             l += 1
             continue
-        break
+        l += 1
+        r += 1
+        to_sum_left.append(len(left) - l)
+
+    return tuple(to_sum_left)
+
+
+def mul_deriv(base_tensor, *tensors):
+
+    unpacked_tensors : list[dtorch.jtensors.JTensors] = list(tensors)
+    is_tensor : bool = isinstance(unpacked_tensors[1], dtorch.jtensors.JTensors)
+    #if (is_tensor):
+    #    left_size : int = len(list(filter(lambda x : x > 1, unpacked_tensors[0].shape)))
+    #    right_size : int = len(list(filter(lambda x : x > 1, unpacked_tensors[1].shape)))
+    
+    #print("pouete", base_tensor.shape)
+    #print("proutgot", unpacked_tensors[0].shape, unpacked_tensors[1].shape if is_tensor else unpacked_tensors[1])
+    if (unpacked_tensors[0].require_grads):
+        right_data = unpacked_tensors[1]() if is_tensor else unpacked_tensors[1]
+        #grad = dtorch.jtensors.JTensors((np.sum(right_data * base_tensor(), axis=dimensionToSum((right_data * base_tensor()).shape, unpacked_tensors[0].shape)).reshape(*unpacked_tensors[0].shape)
+        #                                                        if is_tensor and left_size < right_size
+        #                                                        else (right_data * base_tensor.numpy()).reshape(*unpacked_tensors[0].shape)))
+        axis = dimensionToSum((right_data * base_tensor()).shape, unpacked_tensors[0].shape)
+        grad = dtorch.jtensors.JTensors(np.sum(right_data * base_tensor(), axis=axis).reshape(*unpacked_tensors[0].shape))
+        if (unpacked_tensors[0].isLeaf()):
+            unpacked_tensors[0].grad += grad
+        else:
+            unpacked_tensors[0].grad = grad
+        unpacked_tensors[0].backward(unpacked_tensors[0].grad, forced = True)
 
-    return tuple([i for i in range(len(left) - l)])
+    if (is_tensor and unpacked_tensors[1].require_grads):
+        #grad = dtorch.jtensors.JTensors((np.sum(unpacked_tensors[0]() * base_tensor(), axis=dimensionToSum((unpacked_tensors[0]() * base_tensor()).shape, unpacked_tensors[1].shape)).reshape(*unpacked_tensors[1].shape)
+        #                                                       if right_size < left_size
+        #                                                    else (base_tensor.numpy() * unpacked_tensors[0]()).reshape(*unpacked_tensors[1].shape)))
+        axis = dimensionToSum((unpacked_tensors[0]() * base_tensor()).shape, unpacked_tensors[1].shape)
+        grad = dtorch.jtensors.JTensors(np.sum(unpacked_tensors[0]() * base_tensor(), axis=axis).reshape(*unpacked_tensors[1].shape))
+        if (unpacked_tensors[1].isLeaf()):
+            unpacked_tensors[1].grad += grad
+        else:
+            unpacked_tensors[1].grad = grad
+        unpacked_tensors[1].backward(unpacked_tensors[1].grad, forced = True)
 
 
 def tanh_deriv(base_tensor, *tensors):
 
     tensor : dtorch.jtensors.JTensors = tensors[0]
 
     if (tensor.require_grads):
@@ -222,15 +274,15 @@
 def to_list_deriv(base_tensor, *tensors):
 
     index : int = tensors[0]
     tensor : dtorch.jtensors.JTensors = tensors[1]
 
     if (tensor.require_grads):
         if (tensor.grad is None):
-            tensor.grad = dtorch.jtensors.JTensors(np.zeros(tensor.shape()))
+            tensor.grad = dtorch.jtensors.JTensors(np.zeros(tensor.shape))
         if (tensor.isLeaf()):
             tensor.grad[index] += base_tensor()
         else:
             tensor.grad[index] = base_tensor()
         tensor.backward(tensor.grad, forced=True)
 
 
@@ -260,31 +312,31 @@
             tensors[i].backward(tensors[i].grad, forced=True)
 
 
 def add_deriv(base_tensor, *tensors):
 
     unpacked_tensors : list[dtorch.jtensors.JTensors] = list(tensors)
     is_tensor : bool = isinstance(unpacked_tensors[1], dtorch.jtensors.JTensors)
-    left_size : int = len(list(filter(lambda x : x > 1, unpacked_tensors[0].shape())))
-    right_size : int = len(list(filter(lambda x : x > 1, unpacked_tensors[1].shape())))
+    left_size : int = len(list(filter(lambda x : x > 1, unpacked_tensors[0].shape)))
+    right_size : int = len(list(filter(lambda x : x > 1, unpacked_tensors[1].shape)))
 
     if (unpacked_tensors[0].require_grads):
-        grad = dtorch.jtensors.JTensors(np.sum(base_tensor(), axis=dimensionToSum(unpacked_tensors[1].shape(), unpacked_tensors[0].shape())).reshape(*unpacked_tensors[0].shape())
+        grad = dtorch.jtensors.JTensors(np.sum(base_tensor(), axis=dimensionToSum(unpacked_tensors[1].shape, unpacked_tensors[0].shape)).reshape(*unpacked_tensors[0].shape)
                                                                 if left_size < right_size
-                                                                else base_tensor.numpy().reshape(*unpacked_tensors[0].shape()))
+                                                                else base_tensor.numpy().reshape(*unpacked_tensors[0].shape))
         if (unpacked_tensors[0].isLeaf()):
             unpacked_tensors[0].grad += grad
         else:
             unpacked_tensors[0].grad = grad
         unpacked_tensors[0].backward(unpacked_tensors[0].grad, forced = True)
 
     if (is_tensor and unpacked_tensors[1].require_grads):
-        grad = dtorch.jtensors.JTensors(np.sum(base_tensor(), axis=dimensionToSum(unpacked_tensors[0].shape(), unpacked_tensors[1].shape())).reshape(*unpacked_tensors[1].shape())
+        grad = dtorch.jtensors.JTensors(np.sum(base_tensor(), axis=dimensionToSum(unpacked_tensors[0].shape, unpacked_tensors[1].shape)).reshape(*unpacked_tensors[1].shape)
                                                                if right_size < left_size
-                                                               else base_tensor.numpy().reshape(*unpacked_tensors[1].shape()))
+                                                               else base_tensor.numpy().reshape(*unpacked_tensors[1].shape))
         if (unpacked_tensors[1].isLeaf()):
             unpacked_tensors[1].grad += grad
         else:
             unpacked_tensors[1].grad = grad
         unpacked_tensors[1].backward(unpacked_tensors[1].grad, forced = True)
 
 
@@ -313,32 +365,32 @@
 
 
 def sub_deriv(base_tensor, *tensors):
     # need to be fixed
 
     unpacked_tensors : list[dtorch.jtensors.JTensors] = list(tensors)
     is_tensor : bool = isinstance(unpacked_tensors[1], dtorch.jtensors.JTensors)
-    left_size : int = len(list(filter(lambda x : x > 1, unpacked_tensors[0].shape())))
-    right_size : int = len(list(filter(lambda x : x > 1, unpacked_tensors[1].shape())))
+    left_size : int = len(list(filter(lambda x : x > 1, unpacked_tensors[0].shape)))
+    right_size : int = len(list(filter(lambda x : x > 1, unpacked_tensors[1].shape)))
 
     if (unpacked_tensors[0].require_grads):
-        grad = dtorch.jtensors.JTensors(np.sum(base_tensor(), axis=dimensionToSum(unpacked_tensors[1].shape(), unpacked_tensors[0].shape())).reshape(*unpacked_tensors[0].shape())
+        grad = dtorch.jtensors.JTensors(np.sum(base_tensor(), axis=dimensionToSum(unpacked_tensors[1].shape, unpacked_tensors[0].shape)).reshape(*unpacked_tensors[0].shape)
                                                                 if left_size < right_size
-                                                                else base_tensor.numpy().reshape(*unpacked_tensors[0].shape()))
+                                                                else base_tensor.numpy().reshape(*unpacked_tensors[0].shape))
         if (unpacked_tensors[0].isLeaf()):
             unpacked_tensors[0].grad += grad
         else:
             unpacked_tensors[0].grad = grad
         # probleme diagnostiqué : le numpy.ones empeche le passage du relu. A repenser
         unpacked_tensors[0].backward(unpacked_tensors[0].grad, forced = True)
 
     if (is_tensor and unpacked_tensors[1].require_grads):
-        grad = dtorch.jtensors.JTensors(-1 * (np.sum(base_tensor(), axis=dimensionToSum(unpacked_tensors[0].shape(), unpacked_tensors[1].shape())).reshape(*unpacked_tensors[1].shape())
+        grad = dtorch.jtensors.JTensors(-1 * (np.sum(base_tensor(), axis=dimensionToSum(unpacked_tensors[0].shape, unpacked_tensors[1].shape)).reshape(*unpacked_tensors[1].shape)
                                                                if right_size < left_size
-                                                               else base_tensor.numpy().reshape(*unpacked_tensors[1].shape())))
+                                                               else base_tensor.numpy().reshape(*unpacked_tensors[1].shape)))
         if (unpacked_tensors[1].isLeaf()):
             unpacked_tensors[1].grad += grad
         else:
             unpacked_tensors[1].grad = grad
         unpacked_tensors[1].backward(unpacked_tensors[1].grad, forced = True)
```

### Comparing `dtorch-0.0.3/dtorch/einops.py` & `dtorch-0.0.4/dtorch/einops.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """ imports """
 import dtorch.jtensors
 import numpy as np
+from dtorch.typing import types
 
 def rearrange_backward(base_tensor, *args):
     tensor : dtorch.jtensors.JTensors = args[0]
 
     indexes : list = args[1]
-    old_shape = tuple([base_tensor.shape()[i] for i in indexes])
+    old_shape = tuple([base_tensor.shape[i] for i in indexes])
     old_stride = tuple([base_tensor.numpy().strides[i] for i in indexes])
 
     if (tensor.require_grads):
         tensor.grad += dtorch.jtensors.JTensors(np.lib.stride_tricks.as_strided(base_tensor(), old_shape, old_stride))
         tensor.backward(tensor.grad, forced=True)
 
 """ no composition of axis yet """
+@types(tensor=dtorch.jtensors.JTensors, pattern=str, return_type=dtorch.jtensors.JTensors)
 def rearrange(tensor: dtorch.jtensors.JTensors, pattern : str):
 
     dims : list = []
     o = 0
     for i in range(len(pattern.split('->')[0])):
         o += 1
         if (pattern[i] == ' '):
@@ -36,18 +38,18 @@
         if (pattern[i] == '...'):
             raise Exception("... not implemented")
         res_dims.append(pattern[i])
 
     if len(dims) != len(res_dims):
         raise Exception("Invalid pattern")
     
-    if len(dims) != len(tensor.shape()):
+    if len(dims) != len(tensor.shape):
         raise Exception("Tensor and pattern have different dimensions")
     
-    old_shape = tensor.shape()
+    old_shape = tensor.shape
     indexes = [dims.index(i) for i in res_dims]
     shape = tuple([old_shape[i] for i in indexes])
     stride = tuple([tensor.numpy().strides[i] for i in indexes])
     return dtorch.jtensors.JTensors(
         np.lib.stride_tricks.as_strided(tensor(), shape = shape, strides = stride),
         require_grads = tensor.require_grads,
         operation=dtorch.operations.CrossOperationBackward(
```

### Comparing `dtorch-0.0.3/dtorch/jtensors.py` & `dtorch-0.0.4/dtorch/jtensors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 """ imports """
-from typing import Tuple, Any
+from typing import Tuple, Any, Optional
+from dtorch.typing import types, DtAny
 
 import numpy as np
 
 import dtorch.operations
 from dtorch.derivatives import *
 
 """ Code """
 
 class JTensors:
 
     """ Private """
 
-    def __init__(self, array : np.ndarray | list[float], require_grads : bool = False, operation = None):
+    def __init__(self,
+                 array : np.ndarray | list[float] | float,
+                 require_grads : bool = False,
+                 dtype : type | np.dtype = np.float64,
+                 operation = None):
 
         assert (isinstance(array, (np.ndarray, list, float))), "Invalid parameter for argument of jtensor"
 
         if (isinstance(array, list)):
-            self.__list : np.ndarray = np.array(array)
+            self.__list : np.ndarray = np.array(array, dtype=dtype)
         elif (isinstance(array, float)):
-            self.__list : np.ndarray = np.array([array])
+            self.__list : np.ndarray = np.array([array], dtype=dtype)
         else:
             self.__list : np.ndarray = array
+            self.__list = self.__list.astype(dtype)
 
         self.__operation : dtorch.operations.Operation = None
         if (require_grads):
             self.__operation : dtorch.operations.Operation = operation
         self.require_grads : bool = require_grads
         self.grad : JTensors = None
         self.__name : str = None
 
 
     def __call__(self):
 
         return self.__list
-    
+
 
     def __getitem__(self, key : int):
 
         return self.__list[key]
     
 
     def __setitem__(self, key : int, value : float):
@@ -106,15 +112,15 @@
         assert (isinstance(other, (JTensors, int, float))), "Invalid type for operation with jtensor"
         # consider operating by a direct value (int, float, ...)
 
         res : JTensors | int | float = other
         if (isinstance(other, JTensors)):
             res = other.__list
 
-        require_grad : bool =  self.require_grads or (isinstance(other, JTensors) and other.require_grads)
+        require_grad : bool = self.require_grads or (isinstance(other, JTensors) and other.require_grads)
 
         return JTensors(
             self.__list * res,
             require_grads=require_grad,
             operation=dtorch.operations.CrossOperationBackward(mul_deriv, "MulJBackward", self, other)
             if require_grad else None
         )
@@ -235,28 +241,101 @@
         if (base_tensor is None):
             base_tensor = JTensors([1])
             
         if (self.__operation is not None):
             self.__operation.backward(base_tensor)
 
 
+    @property
+    def ndims(self) -> int:
+
+        """number of dimensions of the tensor
+
+        Returns:
+            int: the number of dims
+        """
+
+        return len(self.__list.shape)
+    
+
+    @property
+    def dtype(self) -> np.dtype:
+
+        """return the dtype of the tensor
+
+        Returns:
+            np.dtype: the dtype
+        """
+
+        return self.__list.dtype
+    
+
+    @dtype.setter
+    def dtype(self, dtype : np.dtype) -> None:
+
+        """set the dtype of the tensor
+
+        Args:
+            dtype (np.dtype): the dtype to set
+        """
+
+        self.__list = self.__list.astype(dtype)
+    
+
+    @property
+    def T(self) -> Any:
+        
+        """return the transpose of the tensor
+
+        Returns:
+            Any: the transpose
+        """
+
+        return dtorch.functionnal.transpose(self)
+
+
+    @property
+    def itemsize(self) -> int:
+
+        """return the itemsize of the tensor
+
+        Returns:
+            int: the itemsize
+        """
+
+        return self.__list.itemsize
+    
+
+    @property
+    def size(self) -> int:
+
+        """number of elements in the tensor
+
+        Returns:
+            int: the number of elements
+        """
+
+        return self.__list.size
+
+
     def isLeaf(self) -> bool:
         """
         """
 
         return self.__operation == None
 
 
     def numpy(self):
         """return the numpy array
         """
 
         return self.__list
 
 
+    @property
     def shape(self) -> Tuple[int]:
         """return the shape of the tensor
 
         Returns:
             Tuple[int]: tensor's shape
         """
 
@@ -271,14 +350,15 @@
     def reshape(self, *shape) -> Any:
         """reshape the tensor
         """
 
         return dtorch.functionnal.reshape(self, shape)
     
 
+    @property
     def stride(self) -> Tuple[int]:
         """return the stride of the tensor
 
         Returns:
             Tuple[int]: tensor's stride
         """
 
@@ -315,16 +395,32 @@
             require_grads=self.require_grads,
             operation=dtorch.operations.CrossOperationBackward(
                 real_max_deriv,
                 "MaxJBackward1",
                 self
             ) if self.require_grads else None
         )
+
+
+    def sum(self, axis : Optional[Tuple[int]] = None, keepdims : bool = False) -> Any:
+
+        return dtorch.functionnal.sum(self, axis, keepdims)
     
 
+    def rearrange(self, pattern : str) -> Any:
+
+        """rearrange the tensor
+
+        Returns:
+            Any: the rearranged tensor
+        """
+
+        return dtorch.einops.rearrange(self, pattern)
+
+
     def shuffle(self) -> Any:
 
         np.random.shuffle(self.__list)
         return self
 
 
     def norm(self) -> Any:
```

### Comparing `dtorch-0.0.3/dtorch/loss.py` & `dtorch-0.0.4/dtorch/loss.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,21 +25,21 @@
         assert (reduction == 'mean' or reduction == 'sum'), "Invalid reduction provided"
 
         self.__reduction : str = reduction
 
 
     def __call__(self, outputs : dtorch.jtensors.JTensors, target : dtorch.jtensors.JTensors) -> dtorch.jtensors.JTensors:
 
-        assert (outputs.shape() == target.shape())
+        assert (outputs.shape == target.shape)
 
-        #print("mse:", outputs.shape(), outputs.stride())
-        #print(((target - outputs) ** 2).stride())
+        #print("mse:", outputs.shape, outputs.stride)
+        #print(((target - outputs) ** 2).stride)
         res : dtorch.jtensors.JTensors = dtorch.functionnal.sum((target - outputs) ** 2)
         if (self.__reduction == 'mean'):
-            scl_nb = np.prod(outputs.shape())
+            scl_nb = np.prod(outputs.shape)
             return res / int(scl_nb)
         return res
     
 
 class BCELoss:
 
     def __init__(self, reduction : str = 'mean') -> None:
```

### Comparing `dtorch-0.0.3/dtorch/operations.py` & `dtorch-0.0.4/dtorch/operations.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.3/dtorch.egg-info/PKG-INFO` & `dtorch-0.0.4/dtorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: A scientific package made a fellow student
 Author-email: Just1truc <hyppoduc@gmail.com>
 Project-URL: Homepage, https://github.com/Just1truc/dtorch
 Project-URL: Bug Tracker, https://github.com/Just1truc/dtorch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 # DTorch
 
 A direct link to the package : [here](https://pypi.org/project/dtorch/)
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Just1truc/dtorch/main/.asset/2023-06-07-09%2038%2034-screenshot.png" data-canonical-src="https://raw.githubusercontent.com/Just1truc/dtorch/main/.asset/2023-06-07-09%2038%2034-screenshot.png" width="200" height="200"/></p>
 
-DTorch is a package made a student at Epitech to improve his understanding of **pytorch** and better his knowledge of ia.
+DTorch is a package made by a student at Epitech to improve his understanding of **pytorch** and better his knowledge of ia.
 It is built on top of **numpy** which is a scientific framework for math between matrices.
 
 This project run on cpu but still have decent computation time making it usable for model building, optimization and saving/loading.
 
 The tensors created can work with numpy but remember that the gradients will **not be calculated** if the operation are not in the range of control of the library. Therefore, a usage of the packages methods on the tensors if preferable.
 
 **Cuda** support may appear in the future and similarly for the dkldnn library that seems to be an excellent when working on CPU.
```

### Comparing `dtorch-0.0.3/pyproject.toml` & `dtorch-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["dtorch"]
 
 [project]
 name = "dtorch"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Just1truc", email="hyppoduc@gmail.com" },
 ]
 description = "A scientific package made a fellow student"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

