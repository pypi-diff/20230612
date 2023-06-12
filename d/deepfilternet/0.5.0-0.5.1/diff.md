# Comparing `tmp/deepfilternet-0.5.0.tar.gz` & `tmp/deepfilternet-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepfilternet-0.5.0.tar", max compression
+gzip compressed data, was "deepfilternet-0.5.1.tar", max compression
```

## Comparing `deepfilternet-0.5.0.tar` & `deepfilternet-0.5.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      495 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/LICENSE
--rw-r--r--   0        0        0    10837 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/LICENSE-APACHE
--rw-r--r--   0        0        0     1083 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/LICENSE-MIT
--rw-r--r--   0        0        0      171 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/__init__.py
--rw-r--r--   0        0        0     7976 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/checkpoint.py
--rw-r--r--   0        0        0    10763 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/config.py
--rw-r--r--   0        0        0    11383 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/deepfilternet.py
--rw-r--r--   0        0        0    19236 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/deepfilternet2.py
--rw-r--r--   0        0        0    16199 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/deepfilternet3.py
--rw-r--r--   0        0        0    15869 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/deepfilternetmf.py
--rw-r--r--   0        0        0    13645 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/enhance.py
--rw-r--r--   0        0        0    23763 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/evaluation_utils.py
--rw-r--r--   0        0        0     4105 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/io.py
--rw-r--r--   0        0        0     7192 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/logger.py
--rw-r--r--   0        0        0    33521 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/loss.py
--rw-r--r--   0        0        0     1920 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/lr.py
--rw-r--r--   0        0        0      779 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/model.py
--rw-r--r--   0        0        0    36996 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/modules.py
--rw-r--r--   0        0        0    24438 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/multiframe.py
--rw-r--r--   0        0        0     8108 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/dnsmos.py
--rw-r--r--   0        0        0     9489 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/dnsmos_dns5.py
--rw-r--r--   0        0        0     3528 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/dnsmos_v2.py
--rw-r--r--   0        0        0    10613 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/export.py
--rw-r--r--   0        0        0     4376 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/filter_dnsmos.py
--rw-r--r--   0        0        0     2267 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/fix_n_samples_hdf5.py
--rw-r--r--   0        0        0      519 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/list_attrs_in_hdf5.py
--rw-r--r--   0        0        0     1959 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/model_summary.py
--rw-r--r--   0        0        0     2211 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/plot_lrs.py
--rw-r--r--   0        0        0      636 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/plot_spec.py
--rw-r--r--   0        0        0     4194 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/plot_summaries.py
--rwxr-xr-x   0        0        0     8762 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/prepare_data.py
--rw-r--r--   0        0        0      355 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/print_model.py
--rw-r--r--   0        0        0     2423 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/sample_from_hdf5.py
--rw-r--r--   0        0        0     2393 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/split_hdf5.py
--rwxr-xr-x   0        0        0     4608 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/test_df.py
--rw-r--r--   0        0        0     2535 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/test_dns_2020.py
--rw-r--r--   0        0        0     2312 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/test_noisy_dnsmos.py
--rw-r--r--   0        0        0     2592 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/test_voicebank_demand.py
--rw-r--r--   0        0        0     3109 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/trim_silence_hdf5.py
--rw-r--r--   0        0        0    17442 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/sepm.py
--rw-r--r--   0        0        0     9474 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/stoi.py
--rw-r--r--   0        0        0    23584 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/train.py
--rw-r--r--   0        0        0     7430 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/utils.py
--rw-r--r--   0        0        0      884 2023-06-05 11:47:27.021806 deepfilternet-0.5.0/df/version.py
--rw-r--r--   0        0        0     3566 2023-06-05 11:47:27.021806 deepfilternet-0.5.0/df/visualization.py
--rw-r--r--   0        0        0     2450 2023-06-05 11:47:27.021806 deepfilternet-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1707 1970-01-01 00:00:00.000000 deepfilternet-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      495 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/LICENSE
+-rw-r--r--   0        0        0    10837 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/LICENSE-APACHE
+-rw-r--r--   0        0        0     1083 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/LICENSE-MIT
+-rw-r--r--   0        0        0      171 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/df/__init__.py
+-rw-r--r--   0        0        0     7976 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/df/checkpoint.py
+-rw-r--r--   0        0        0    10763 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/df/config.py
+-rw-r--r--   0        0        0    11383 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/df/deepfilternet.py
+-rw-r--r--   0        0        0    19236 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/df/deepfilternet2.py
+-rw-r--r--   0        0        0    16199 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/df/deepfilternet3.py
+-rw-r--r--   0        0        0    15869 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/df/deepfilternetmf.py
+-rw-r--r--   0        0        0    13799 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/df/enhance.py
+-rw-r--r--   0        0        0    23763 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/df/evaluation_utils.py
+-rw-r--r--   0        0        0     4105 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/df/io.py
+-rw-r--r--   0        0        0     7192 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/df/logger.py
+-rw-r--r--   0        0        0    33521 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/df/loss.py
+-rw-r--r--   0        0        0     1920 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/df/lr.py
+-rw-r--r--   0        0        0      779 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/df/model.py
+-rw-r--r--   0        0        0    36996 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/df/modules.py
+-rw-r--r--   0        0        0    24440 2023-06-12 21:43:39.797739 deepfilternet-0.5.1/df/multiframe.py
+-rw-r--r--   0        0        0     8108 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/dnsmos.py
+-rw-r--r--   0        0        0     9489 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/dnsmos_dns5.py
+-rw-r--r--   0        0        0     3528 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/dnsmos_v2.py
+-rw-r--r--   0        0        0    10613 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/export.py
+-rw-r--r--   0        0        0     4376 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/filter_dnsmos.py
+-rw-r--r--   0        0        0     2267 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/fix_n_samples_hdf5.py
+-rw-r--r--   0        0        0      519 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/list_attrs_in_hdf5.py
+-rw-r--r--   0        0        0     1959 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/model_summary.py
+-rw-r--r--   0        0        0     2211 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/plot_lrs.py
+-rw-r--r--   0        0        0      636 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/plot_spec.py
+-rw-r--r--   0        0        0     4194 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/plot_summaries.py
+-rwxr-xr-x   0        0        0     8762 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/prepare_data.py
+-rw-r--r--   0        0        0      355 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/print_model.py
+-rw-r--r--   0        0        0     2423 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/sample_from_hdf5.py
+-rw-r--r--   0        0        0     2393 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/split_hdf5.py
+-rwxr-xr-x   0        0        0     4608 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/test_df.py
+-rw-r--r--   0        0        0     2535 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/test_dns_2020.py
+-rw-r--r--   0        0        0     2312 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/test_noisy_dnsmos.py
+-rw-r--r--   0        0        0     2592 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/test_voicebank_demand.py
+-rw-r--r--   0        0        0     3109 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/scripts/trim_silence_hdf5.py
+-rw-r--r--   0        0        0    17442 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/sepm.py
+-rw-r--r--   0        0        0     9474 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/stoi.py
+-rw-r--r--   0        0        0    23584 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/train.py
+-rw-r--r--   0        0        0     7430 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/utils.py
+-rw-r--r--   0        0        0      884 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/version.py
+-rw-r--r--   0        0        0     3566 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/df/visualization.py
+-rw-r--r--   0        0        0     2450 2023-06-12 21:43:39.801739 deepfilternet-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1707 1970-01-01 00:00:00.000000 deepfilternet-0.5.1/PKG-INFO
```

### Comparing `deepfilternet-0.5.0/LICENSE-APACHE` & `deepfilternet-0.5.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/LICENSE-MIT` & `deepfilternet-0.5.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/checkpoint.py` & `deepfilternet-0.5.1/df/checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/config.py` & `deepfilternet-0.5.1/df/config.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/deepfilternet.py` & `deepfilternet-0.5.1/df/deepfilternet.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/deepfilternet2.py` & `deepfilternet-0.5.1/df/deepfilternet2.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/deepfilternet3.py` & `deepfilternet-0.5.1/df/deepfilternet3.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/deepfilternetmf.py` & `deepfilternet-0.5.1/df/deepfilternetmf.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/enhance.py` & `deepfilternet-0.5.1/df/enhance.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 def main(args):
     model, df_state, suffix = init_df(
         args.model_base_dir,
         post_filter=args.pf,
         log_level=args.log_level,
         config_allow_defaults=True,
         epoch=args.epoch,
+        mask_only=args.no_df_stage,
     )
     suffix = suffix if args.suffix else None
     if args.output_dir is None:
         args.output_dir = "."
     elif not os.path.isdir(args.output_dir):
         os.mkdir(args.output_dir)
     df_sr = ModelParams().sr
@@ -101,14 +102,15 @@
     model_base_dir: Optional[str] = None,
     post_filter: bool = False,
     log_level: str = "INFO",
     log_file: Optional[str] = "enhance.log",
     config_allow_defaults: bool = False,
     epoch: Union[str, int, None] = "best",
     default_model: str = DEFAULT_MODEL,
+    mask_only: bool = False,
 ) -> Tuple[nn.Module, DF, str]:
     """Initializes and loads config, model and deep filtering state.
 
     Args:
         model_base_dir (str): Path to the model directory containing checkpoint and config. If None,
             load the pretrained DeepFilterNet2 model.
         post_filter (bool): Enable post filter for some minor, extra noise reduction.
@@ -157,15 +159,17 @@
         nb_bands=p.nb_erb,
         min_nb_erb_freqs=p.min_nb_freqs,
     )
     checkpoint_dir = os.path.join(model_base_dir, "checkpoints")
     load_cp = epoch is not None and not (isinstance(epoch, str) and epoch.lower() == "none")
     if not load_cp:
         checkpoint_dir = None
-    mask_only = config("mask_only", cast=bool, section="train", default=False, save=False)
+    mask_only = mask_only or config(
+        "mask_only", cast=bool, section="train", default=False, save=False
+    )
     model, epoch = load_model_cp(checkpoint_dir, df_state, epoch=epoch, mask_only=mask_only)
     if (epoch is None or epoch == 0) and load_cp:
         logger.error("Could not find a checkpoint")
         exit(1)
     logger.debug(f"Loaded checkpoint from epoch {epoch}")
     model = model.to(get_device())
     # Set suffix to model name
@@ -357,13 +361,14 @@
     )
     parser.add_argument(
         "--no-suffix",
         action="store_false",
         dest="suffix",
         help="Don't add the model suffix to the enhanced audio files",
     )
+    parser.add_argument("--no-df-stage", action="store_true")
     args = parser.parse_args()
     main(args)
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `deepfilternet-0.5.0/df/evaluation_utils.py` & `deepfilternet-0.5.1/df/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/io.py` & `deepfilternet-0.5.1/df/io.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/logger.py` & `deepfilternet-0.5.1/df/logger.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/loss.py` & `deepfilternet-0.5.1/df/loss.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/lr.py` & `deepfilternet-0.5.1/df/lr.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/model.py` & `deepfilternet-0.5.1/df/model.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/modules.py` & `deepfilternet-0.5.1/df/modules.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/multiframe.py` & `deepfilternet-0.5.1/df/multiframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,28 +120,28 @@
         Rxx (complex Tensor): Correlation matrix of shape [B, C, T, F, N, N]
     """
     x = F.pad(x, (0, 0, n - 1, 0)).unfold(-2, n, 1)
     return torch.einsum("...n,...m->...mn", x, x.conj())
 
 
 def df(spec: Tensor, coefs: Tensor) -> Tensor:
-    """Deep filter implemenation using `torch.einsum`. Requires unfolded spectrogram.
+    """Deep filter implementation using `torch.einsum`. Requires unfolded spectrogram.
 
     Args:
         spec (complex Tensor): Spectrogram of shape [B, C, T, F, N]
         coefs (complex Tensor): Coefficients of shape [B, C, N, T, F]
 
     Returns:
         spec (complex Tensor): Spectrogram of shape [B, C, T, F]
     """
     return torch.einsum("...tfn,...ntf->...tf", spec, coefs)
 
 
 def df_real(spec: Tensor, coefs: Tensor) -> Tensor:
-    """Deep filter implemenation for real valued input Tensors. Requires unfolded spectrograms.
+    """Deep filter implementation for real valued input Tensors. Requires unfolded spectrograms.
 
     Args:
         spec (real-valued Tensor): Spectrogram of shape [B, C, N, T, F, 2].
         coefs (real-valued Tensor): Coefficients of shape [B, C, N, T, F, 2].
 
     Returns:
         spec (real-valued Tensor): Filtered Spectrogram of shape [B, C, T, F, 2]
```

### Comparing `deepfilternet-0.5.0/df/scripts/dnsmos.py` & `deepfilternet-0.5.1/df/scripts/dnsmos.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/dnsmos_dns5.py` & `deepfilternet-0.5.1/df/scripts/dnsmos_dns5.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/dnsmos_v2.py` & `deepfilternet-0.5.1/df/scripts/dnsmos_v2.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/export.py` & `deepfilternet-0.5.1/df/scripts/export.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/filter_dnsmos.py` & `deepfilternet-0.5.1/df/scripts/filter_dnsmos.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/fix_n_samples_hdf5.py` & `deepfilternet-0.5.1/df/scripts/fix_n_samples_hdf5.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/list_attrs_in_hdf5.py` & `deepfilternet-0.5.1/df/scripts/list_attrs_in_hdf5.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/model_summary.py` & `deepfilternet-0.5.1/df/scripts/model_summary.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/plot_lrs.py` & `deepfilternet-0.5.1/df/scripts/plot_lrs.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/plot_spec.py` & `deepfilternet-0.5.1/df/scripts/plot_spec.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/plot_summaries.py` & `deepfilternet-0.5.1/df/scripts/plot_summaries.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/prepare_data.py` & `deepfilternet-0.5.1/df/scripts/prepare_data.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/sample_from_hdf5.py` & `deepfilternet-0.5.1/df/scripts/sample_from_hdf5.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/split_hdf5.py` & `deepfilternet-0.5.1/df/scripts/split_hdf5.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/test_df.py` & `deepfilternet-0.5.1/df/scripts/test_df.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/test_dns_2020.py` & `deepfilternet-0.5.1/df/scripts/test_dns_2020.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/test_noisy_dnsmos.py` & `deepfilternet-0.5.1/df/scripts/test_noisy_dnsmos.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/test_voicebank_demand.py` & `deepfilternet-0.5.1/df/scripts/test_voicebank_demand.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/scripts/trim_silence_hdf5.py` & `deepfilternet-0.5.1/df/scripts/trim_silence_hdf5.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/sepm.py` & `deepfilternet-0.5.1/df/sepm.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/stoi.py` & `deepfilternet-0.5.1/df/stoi.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/train.py` & `deepfilternet-0.5.1/df/train.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/utils.py` & `deepfilternet-0.5.1/df/utils.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/version.py` & `deepfilternet-0.5.1/df/version.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/df/visualization.py` & `deepfilternet-0.5.1/df/visualization.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.0/pyproject.toml` & `deepfilternet-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "DeepFilterNet"
-version = "0.5.0"
+version = "0.5.1"
 description = "Noise supression using deep filtering"
 authors = ["Hendrik Schröter"]
 repository = "https://github.com/Rikorose/DeepFilterNet"
 keywords = ["noise reduction", "neural network"]
 classifiers = [
   "Topic :: Multimedia :: Sound/Audio :: Speech",
   "Topic :: Software Development :: Libraries :: Python Modules",
@@ -19,16 +19,16 @@
   { path = "pretrained_models/DeepFilterNet/config.ini" },
   { path = "pretrained_models/DeepFilterNet/checkpoints/*" },
   { path = "pretrained_models/DeepFilterNet2/config.ini" },
   { path = "pretrained_models/DeepFilterNet2/checkpoints/*" },
 ]
 
 [tool.poetry.dependencies]
-deepfilterlib = "0.5.0"
-deepfilterdataloader = { version = "0.5.0", optional = true }
+deepfilterlib = "0.5.1"
+deepfilterdataloader = { version = "0.5.1", optional = true }
 python = ">=3.8,<4.0"
 numpy = ">=1.22,<2.0"
 loguru = ">=0.5"
 appdirs = "^1.4"
 requests = "^2.27"
 packaging = "^23.0"
 sympy = ">=1.6"
```

### Comparing `deepfilternet-0.5.0/PKG-INFO` & `deepfilternet-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfilternet
-Version: 0.5.0
+Version: 0.5.1
 Summary: Noise supression using deep filtering
 Home-page: https://github.com/Rikorose/DeepFilterNet
 License: MIT
 Keywords: noise reduction,neural network
 Author: Hendrik Schröter
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,16 +20,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Provides-Extra: dnsmos-local
 Provides-Extra: eval
 Provides-Extra: soundfile
 Provides-Extra: train
 Requires-Dist: appdirs (>=1.4,<2.0)
-Requires-Dist: deepfilterdataloader (==0.5.0) ; extra == "train"
-Requires-Dist: deepfilterlib (==0.5.0)
+Requires-Dist: deepfilterdataloader (==0.5.1) ; extra == "train"
+Requires-Dist: deepfilterlib (==0.5.1)
 Requires-Dist: icecream (>=2,<3) ; extra == "train"
 Requires-Dist: loguru (>=0.5)
 Requires-Dist: numpy (>=1.22,<2.0)
 Requires-Dist: onnxruntime (>=1.15,<2.0) ; extra == "dnsmos-local"
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pesq (>=0.0.3,<0.0.5) ; extra == "eval"
 Requires-Dist: pystoi (>=0.3,<0.4) ; extra == "eval"
```

