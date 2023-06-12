# Comparing `tmp/onnx2kerastl-0.0.97.dev1.tar.gz` & `tmp/onnx2kerastl-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2kerastl-0.0.97.dev1.tar", max compression
+gzip compressed data, was "onnx2kerastl-0.0.98.tar", max compression
```

## Comparing `onnx2kerastl-0.0.97.dev1.tar` & `onnx2kerastl-0.0.98.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1067 2023-05-17 10:05:24.840017 onnx2kerastl-0.0.97.dev1/LICENSE
--rw-r--r--   0        0        0       66 2023-05-17 10:05:24.840536 onnx2kerastl-0.0.97.dev1/onnx2kerastl/__init__.py
--rw-r--r--   0        0        0     8121 2023-05-17 10:05:24.840790 onnx2kerastl-0.0.97.dev1/onnx2kerastl/activation_layers.py
--rw-r--r--   0        0        0     1127 2023-05-17 10:05:24.840968 onnx2kerastl-0.0.97.dev1/onnx2kerastl/caffe2_layers.py
--rw-r--r--   0        0        0      780 2023-06-07 15:57:44.568650 onnx2kerastl-0.0.97.dev1/onnx2kerastl/constant_layers.py
--rw-r--r--   0        0        0    14415 2023-06-07 16:25:57.562217 onnx2kerastl-0.0.97.dev1/onnx2kerastl/converter.py
--rw-r--r--   0        0        0    11968 2023-05-17 10:05:24.841507 onnx2kerastl-0.0.97.dev1/onnx2kerastl/convolution_layers.py
--rw-r--r--   0        0        0      584 2023-05-23 13:09:48.518074 onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/__init__.py
--rw-r--r--   0        0        0      236 2023-05-17 10:05:24.841906 onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxabs.py
--rw-r--r--   0        0        0      236 2023-05-17 10:05:24.842046 onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxerf.py
--rw-r--r--   0        0        0      606 2023-05-17 10:05:24.842190 onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
--rw-r--r--   0        0        0     1730 2023-05-17 10:05:24.842337 onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxlstm.py
--rw-r--r--   0        0        0      605 2023-05-17 10:05:24.842473 onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxreducemean.py
--rw-r--r--   0        0        0      238 2023-05-17 10:05:24.842602 onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxsqrt.py
--rw-r--r--   0        0        0     9380 2023-06-07 16:25:57.562862 onnx2kerastl-0.0.97.dev1/onnx2kerastl/elementwise_layers.py
--rw-r--r--   0        0        0      179 2023-05-17 10:05:24.842900 onnx2kerastl-0.0.97.dev1/onnx2kerastl/exceptions.py
--rw-r--r--   0        0        0     3947 2023-05-30 11:43:46.982250 onnx2kerastl-0.0.97.dev1/onnx2kerastl/layers.py
--rw-r--r--   0        0        0     2301 2023-05-30 11:55:17.207286 onnx2kerastl-0.0.97.dev1/onnx2kerastl/linear_layers.py
--rw-r--r--   0        0        0     3791 2023-05-17 10:05:24.843376 onnx2kerastl-0.0.97.dev1/onnx2kerastl/ltsm_layers.py
--rw-r--r--   0        0        0      368 2023-05-17 10:05:24.843508 onnx2kerastl-0.0.97.dev1/onnx2kerastl/main.py
--rw-r--r--   0        0        0     5551 2023-05-17 10:05:24.843673 onnx2kerastl-0.0.97.dev1/onnx2kerastl/normalization_layers.py
--rw-r--r--   0        0        0    16027 2023-06-07 15:57:44.569123 onnx2kerastl-0.0.97.dev1/onnx2kerastl/operation_layers.py
--rw-r--r--   0        0        0     3015 2023-05-17 10:05:24.844012 onnx2kerastl-0.0.97.dev1/onnx2kerastl/padding_layers.py
--rw-r--r--   0        0        0     7464 2023-05-17 10:05:24.844205 onnx2kerastl-0.0.97.dev1/onnx2kerastl/pooling_layers.py
--rw-r--r--   0        0        0    18236 2023-06-08 08:23:24.978235 onnx2kerastl-0.0.97.dev1/onnx2kerastl/reshape_layers.py
--rw-r--r--   0        0        0     5006 2023-06-07 10:11:23.748652 onnx2kerastl-0.0.97.dev1/onnx2kerastl/sampling_layers.py
--rw-r--r--   0        0        0     1655 2023-05-17 10:05:24.844792 onnx2kerastl-0.0.97.dev1/onnx2kerastl/upsampling_layers.py
--rw-r--r--   0        0        0     5822 2023-06-07 16:25:57.564995 onnx2kerastl-0.0.97.dev1/onnx2kerastl/utils.py
--rw-r--r--   0        0        0     1035 2023-06-08 08:23:24.978933 onnx2kerastl-0.0.97.dev1/pyproject.toml
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.97.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-05-24 12:10:46.678537 onnx2kerastl-0.0.98/LICENSE
+-rw-r--r--   0        0        0       66 2022-05-29 07:44:17.204667 onnx2kerastl-0.0.98/onnx2kerastl/__init__.py
+-rw-r--r--   0        0        0     8121 2023-04-25 09:04:27.467793 onnx2kerastl-0.0.98/onnx2kerastl/activation_layers.py
+-rw-r--r--   0        0        0     1127 2022-08-04 13:51:21.421383 onnx2kerastl-0.0.98/onnx2kerastl/caffe2_layers.py
+-rw-r--r--   0        0        0      780 2022-10-03 15:38:22.085235 onnx2kerastl-0.0.98/onnx2kerastl/constant_layers.py
+-rw-r--r--   0        0        0    14415 2023-06-12 12:28:45.565375 onnx2kerastl-0.0.98/onnx2kerastl/converter.py
+-rw-r--r--   0        0        0    11968 2023-05-21 12:48:52.329860 onnx2kerastl-0.0.98/onnx2kerastl/convolution_layers.py
+-rw-r--r--   0        0        0      584 2023-05-21 12:48:52.330876 onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/__init__.py
+-rw-r--r--   0        0        0      236 2022-10-23 09:48:40.399903 onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxabs.py
+-rw-r--r--   0        0        0      236 2022-05-30 13:34:03.376696 onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxerf.py
+-rw-r--r--   0        0        0      606 2022-05-24 12:10:46.680353 onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
+-rw-r--r--   0        0        0     1585 2023-06-12 13:39:46.673928 onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxlstm.py
+-rw-r--r--   0        0        0      605 2022-09-19 17:39:21.485803 onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxreducemean.py
+-rw-r--r--   0        0        0      238 2022-05-30 13:34:03.376950 onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxsqrt.py
+-rw-r--r--   0        0        0     9380 2023-06-12 12:28:45.566760 onnx2kerastl-0.0.98/onnx2kerastl/elementwise_layers.py
+-rw-r--r--   0        0        0      179 2022-08-04 13:51:21.427113 onnx2kerastl-0.0.98/onnx2kerastl/exceptions.py
+-rw-r--r--   0        0        0     3947 2023-06-12 12:28:45.567142 onnx2kerastl-0.0.98/onnx2kerastl/layers.py
+-rw-r--r--   0        0        0     2301 2023-01-19 11:41:57.593097 onnx2kerastl-0.0.98/onnx2kerastl/linear_layers.py
+-rw-r--r--   0        0        0     3664 2023-06-12 13:41:14.046234 onnx2kerastl-0.0.98/onnx2kerastl/ltsm_layers.py
+-rw-r--r--   0        0        0      368 2022-05-24 12:10:46.680940 onnx2kerastl-0.0.98/onnx2kerastl/main.py
+-rw-r--r--   0        0        0     5551 2023-05-21 12:48:52.333310 onnx2kerastl-0.0.98/onnx2kerastl/normalization_layers.py
+-rw-r--r--   0        0        0    16027 2023-06-12 12:28:45.567939 onnx2kerastl-0.0.98/onnx2kerastl/operation_layers.py
+-rw-r--r--   0        0        0     3015 2023-04-25 09:04:27.472631 onnx2kerastl-0.0.98/onnx2kerastl/padding_layers.py
+-rw-r--r--   0        0        0     7464 2023-01-19 11:41:57.596399 onnx2kerastl-0.0.98/onnx2kerastl/pooling_layers.py
+-rw-r--r--   0        0        0    18236 2023-06-12 12:28:45.568511 onnx2kerastl-0.0.98/onnx2kerastl/reshape_layers.py
+-rw-r--r--   0        0        0     5006 2023-06-12 12:28:45.569230 onnx2kerastl-0.0.98/onnx2kerastl/sampling_layers.py
+-rw-r--r--   0        0        0     1655 2023-01-19 11:41:57.597650 onnx2kerastl-0.0.98/onnx2kerastl/upsampling_layers.py
+-rw-r--r--   0        0        0     5822 2023-06-12 12:28:45.570930 onnx2kerastl-0.0.98/onnx2kerastl/utils.py
+-rw-r--r--   0        0        0     1030 2023-06-12 13:41:59.160562 onnx2kerastl-0.0.98/pyproject.toml
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.98/PKG-INFO
```

### Comparing `onnx2kerastl-0.0.97.dev1/LICENSE` & `onnx2kerastl-0.0.98/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/activation_layers.py` & `onnx2kerastl-0.0.98/onnx2kerastl/activation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/caffe2_layers.py` & `onnx2kerastl-0.0.98/onnx2kerastl/caffe2_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/constant_layers.py` & `onnx2kerastl-0.0.98/onnx2kerastl/constant_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/converter.py` & `onnx2kerastl-0.0.98/onnx2kerastl/converter.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/convolution_layers.py` & `onnx2kerastl-0.0.98/onnx2kerastl/convolution_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/__init__.py` & `onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py` & `onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxlstm.py` & `onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxlstm.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,18 +24,15 @@
         if initial_h_state is not None and initial_c_state is not None:
             initial_states = [initial_h_state, initial_c_state]
         else:
             initial_states = None
         res = self.lstm_layer(inputs, initial_state=initial_states, **kwargs)
         if self.return_lstm_state:
             lstm_tensor, h_out, c_out = res
-            lstm_flat = tf.keras.layers.Flatten()(lstm_tensor)
-            h_flat = tf.keras.layers.Flatten()(h_out)
-            c_flat = tf.keras.layers.Flatten()(c_out)
-            concat_output = tf.keras.layers.Concatenate()([lstm_flat, h_flat, c_flat])
+            concat_output = tf.concat([tf.expand_dims(h_out, 1), lstm_tensor, tf.expand_dims(c_out, 1)], axis=1)
             return concat_output
         else:
             return res
 
     def build(self, input_shape):
         self.lstm_layer.build(input_shape)
```

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxreducemean.py` & `onnx2kerastl-0.0.98/onnx2kerastl/customonnxlayer/onnxreducemean.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/elementwise_layers.py` & `onnx2kerastl-0.0.98/onnx2kerastl/elementwise_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/layers.py` & `onnx2kerastl-0.0.98/onnx2kerastl/layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/linear_layers.py` & `onnx2kerastl-0.0.98/onnx2kerastl/linear_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/ltsm_layers.py` & `onnx2kerastl-0.0.98/onnx2kerastl/ltsm_layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,18 +56,17 @@
     bias2 = np.concatenate([weights_b_part2[0:hidden_size], weights_b_part2[2 * hidden_size:3 * hidden_size],
                             weights_b_part2[3 * hidden_size:4 * hidden_size],
                             weights_b_part2[hidden_size:2 * hidden_size]]).transpose()
     bias = bias1 + bias2
     res.node.layer.set_weights([w1, w2, bias])
     tf.keras.backend.set_image_data_format("channels_first")
     if should_return_state:
-        c_out = res[:, -hidden_size:]
-        h_out = res[:, -2*hidden_size:-hidden_size]
-        flat_lstm_tensor = res[:, :-2*hidden_size]
-        lstm_tensor = tf.keras.layers.Reshape((-1, hidden_size))(flat_lstm_tensor)
+        c_out = res[:, -1, :]
+        h_out = res[:, 0, :]
+        lstm_tensor = res[:, 1:-1, :]
         layers[node.output[1]] = c_out
         layers[node.output[2]] = h_out
     else:
         lstm_tensor = res
     lstm_tensor_in_onnx_order = tf.transpose(lstm_tensor, perm=[1, 0, 2])
     lstm_tensor_in_onnx_order = tf.expand_dims(lstm_tensor_in_onnx_order, axis=1)
     layers[node_name] = lstm_tensor_in_onnx_order
```

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/normalization_layers.py` & `onnx2kerastl-0.0.98/onnx2kerastl/normalization_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/operation_layers.py` & `onnx2kerastl-0.0.98/onnx2kerastl/operation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/padding_layers.py` & `onnx2kerastl-0.0.98/onnx2kerastl/padding_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/pooling_layers.py` & `onnx2kerastl-0.0.98/onnx2kerastl/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/reshape_layers.py` & `onnx2kerastl-0.0.98/onnx2kerastl/reshape_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/sampling_layers.py` & `onnx2kerastl-0.0.98/onnx2kerastl/sampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/upsampling_layers.py` & `onnx2kerastl-0.0.98/onnx2kerastl/upsampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/onnx2kerastl/utils.py` & `onnx2kerastl-0.0.98/onnx2kerastl/utils.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.97.dev1/pyproject.toml` & `onnx2kerastl-0.0.98/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onnx2kerastl"
-version = "0.0.97.dev1"
+version = "0.0.98"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
```

### Comparing `onnx2kerastl-0.0.97.dev1/PKG-INFO` & `onnx2kerastl-0.0.98/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2kerastl
-Version: 0.0.97.dev1
+Version: 0.0.98
 Summary: 
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

