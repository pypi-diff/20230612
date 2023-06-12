# Comparing `tmp/vocos-0.0.1.tar.gz` & `tmp/vocos-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocos-0.0.1.tar", last modified: Sun Jun 11 20:02:59 2023, max compression
+gzip compressed data, was "vocos-0.0.2.tar", last modified: Mon Jun 12 16:58:46 2023, max compression
```

## Comparing `vocos-0.0.1.tar` & `vocos-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:02:59.989894 vocos-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-11 20:02:53.000000 vocos-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-11 20:02:59.989894 vocos-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-11 20:02:53.000000 vocos-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 20:02:59.989894 vocos-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-11 20:02:53.000000 vocos-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:02:59.985894 vocos-0.0.1/vocos/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-11 20:02:53.000000 vocos-0.0.1/vocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-11 20:02:53.000000 vocos-0.0.1/vocos/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-06-11 20:02:53.000000 vocos-0.0.1/vocos/discriminators.py
--rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-06-11 20:02:53.000000 vocos-0.0.1/vocos/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-11 20:02:53.000000 vocos-0.0.1/vocos/feature_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-11 20:02:53.000000 vocos-0.0.1/vocos/heads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-11 20:02:53.000000 vocos-0.0.1/vocos/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-11 20:02:53.000000 vocos-0.0.1/vocos/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-11 20:02:53.000000 vocos-0.0.1/vocos/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-06-11 20:02:53.000000 vocos-0.0.1/vocos/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-11 20:02:53.000000 vocos-0.0.1/vocos/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-11 20:02:53.000000 vocos-0.0.1/vocos/spectral_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:02:59.989894 vocos-0.0.1/vocos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-11 20:02:59.000000 vocos-0.0.1/vocos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-11 20:02:59.000000 vocos-0.0.1/vocos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 20:02:59.000000 vocos-0.0.1/vocos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-11 20:02:59.000000 vocos-0.0.1/vocos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-11 20:02:59.000000 vocos-0.0.1/vocos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:58:46.802756 vocos-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-12 16:58:40.000000 vocos-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-12 16:58:46.802756 vocos-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-12 16:58:40.000000 vocos-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:58:46.806756 vocos-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-12 16:58:40.000000 vocos-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:58:46.802756 vocos-0.0.2/vocos/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/discriminators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/heads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-12 16:58:40.000000 vocos-0.0.2/vocos/spectral_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:58:46.802756 vocos-0.0.2/vocos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-12 16:58:46.000000 vocos-0.0.2/vocos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-12 16:58:46.000000 vocos-0.0.2/vocos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:58:46.000000 vocos-0.0.2/vocos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-12 16:58:46.000000 vocos-0.0.2/vocos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 16:58:46.000000 vocos-0.0.2/vocos.egg-info/top_level.txt
```

### Comparing `vocos-0.0.1/LICENSE` & `vocos-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vocos-0.0.1/PKG-INFO` & `vocos-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocos
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fourier-based neural vocoder for high-quality audio synthesis
 Home-page: https://github.com/charactr-platform/vocos
 Author: Hubert Siuzdak
 Author-email: huberts@charactr.com
 Description-Content-Type: text/markdown
 Provides-Extra: train
 License-File: LICENSE
```

### Comparing `vocos-0.0.1/README.md` & `vocos-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vocos-0.0.1/setup.py` & `vocos-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.1/vocos/dataset.py` & `vocos-0.0.2/vocos/dataset.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.1/vocos/discriminators.py` & `vocos-0.0.2/vocos/discriminators.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.1/vocos/experiment.py` & `vocos-0.0.2/vocos/experiment.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.1/vocos/feature_extractors.py` & `vocos-0.0.2/vocos/feature_extractors.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.1/vocos/heads.py` & `vocos-0.0.2/vocos/heads.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.1/vocos/helpers.py` & `vocos-0.0.2/vocos/helpers.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.1/vocos/loss.py` & `vocos-0.0.2/vocos/loss.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.1/vocos/models.py` & `vocos-0.0.2/vocos/models.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.1/vocos/modules.py` & `vocos-0.0.2/vocos/modules.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.1/vocos/pretrained.py` & `vocos-0.0.2/vocos/pretrained.py`

 * *Files 25% similar despite different names*

```diff
@@ -72,24 +72,70 @@
                 for key, value in model.feature_extractor.encodec.state_dict().items()
             }
             state_dict.update(encodec_parameters)
         model.load_state_dict(state_dict)
         model.eval()
         return model
 
+    @torch.inference_mode()
     def forward(self, audio_input: torch.Tensor, **kwargs: Any) -> torch.Tensor:
         """
         Method to run a copy-synthesis from audio waveform. The feature extractor first processes the audio input,
         which is then passed through the backbone and the head to reconstruct the audio output.
+
+        Args:
+            audio_input (Tensor): The input tensor representing the audio waveform of shape (B, T),
+                                        where B is the batch size and L is the waveform length.
+
+
+        Returns:
+            Tensor: The output tensor representing the reconstructed audio waveform of shape (B, T).
         """
         features = self.feature_extractor(audio_input, **kwargs)
         audio_output = self.decode(features, **kwargs)
         return audio_output
 
+    @torch.inference_mode()
     def decode(self, features_input: torch.Tensor, **kwargs: Any) -> torch.Tensor:
         """
         Method to decode audio waveform from already calculated features. The features input is passed through
         the backbone and the head to reconstruct the audio output.
+
+        Args:
+            features_input (Tensor): The input tensor of features of shape (B, C, L), where B is the batch size,
+                                     C denotes the feature dimension, and L is the sequence length.
+
+        Returns:
+            Tensor: The output tensor representing the reconstructed audio waveform of shape (B, T).
         """
         x = self.backbone(features_input, **kwargs)
         audio_output = self.head(x)
         return audio_output
+
+    @torch.inference_mode()
+    def codes_to_features(self, codes: torch.Tensor) -> torch.Tensor:
+        """
+        Transforms an input sequence of discrete tokens (codes) into feature embeddings using the feature extractor's
+        codebook weights.
+
+        Args:
+            codes (Tensor): The input tensor. Expected shape is (K, L) or (K, B, L),
+                            where K is the number of codebooks, B is the batch size and L is the sequence length.
+
+        Returns:
+            Tensor: Features of shape (B, C, L), where B is the batch size, C denotes the feature dimension,
+                    and L is the sequence length.
+        """
+        assert isinstance(
+            self.feature_extractor, EncodecFeatures
+        ), "Feature extractor should be an instance of EncodecFeatures"
+
+        if codes.dim() == 2:
+            codes = codes.unsqueeze(1)
+
+        n_bins = self.feature_extractor.encodec.quantizer.bins
+        offsets = torch.arange(0, n_bins * len(codes), n_bins, device=codes.device)
+        embeddings_idxs = codes + offsets.view(-1, 1, 1)
+        features = torch.nn.functional.embedding(embeddings_idxs, self.feature_extractor.codebook_weights).sum(dim=0)
+        features = features.transpose(1, 2)
+
+        return features
```

### Comparing `vocos-0.0.1/vocos/spectral_ops.py` & `vocos-0.0.2/vocos/spectral_ops.py`

 * *Files identical despite different names*

### Comparing `vocos-0.0.1/vocos.egg-info/PKG-INFO` & `vocos-0.0.2/vocos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocos
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fourier-based neural vocoder for high-quality audio synthesis
 Home-page: https://github.com/charactr-platform/vocos
 Author: Hubert Siuzdak
 Author-email: huberts@charactr.com
 Description-Content-Type: text/markdown
 Provides-Extra: train
 License-File: LICENSE
```

