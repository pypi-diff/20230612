# Comparing `tmp/conplex_dti-0.1.0.tar.gz` & `tmp/conplex_dti-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conplex_dti-0.1.0.tar", max compression
+gzip compressed data, was "conplex_dti-0.1.1.tar", max compression
```

## Comparing `conplex_dti-0.1.0.tar` & `conplex_dti-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1074 2023-03-11 16:53:19.162872 conplex_dti-0.1.0/LICENSE
--rw-r--r--   0        0        0      252 2023-03-11 17:33:37.635915 conplex_dti-0.1.0/README.md
--rw-r--r--   0        0        0     3510 2023-03-11 20:51:35.491076 conplex_dti-0.1.0/conplex_dti/MAIN_OLD.txt
--rw-r--r--   0        0        0      395 2023-03-11 17:10:21.584137 conplex_dti-0.1.0/conplex_dti/__init__.py
--rw-r--r--   0        0        0     1003 2023-04-26 19:08:24.982701 conplex_dti-0.1.0/conplex_dti/__main__.py
--rw-r--r--   0        0        0    23714 2023-03-11 20:28:46.529821 conplex_dti-0.1.0/conplex_dti/architectures.py
--rw-r--r--   0        0        0       77 2023-03-11 20:53:29.086748 conplex_dti-0.1.0/conplex_dti/cli/__init__.py
--rw-r--r--   0        0        0    17358 2023-04-26 19:32:18.804335 conplex_dti-0.1.0/conplex_dti/cli/train.py
--rw-r--r--   0        0        0      171 2023-03-11 20:33:16.557111 conplex_dti-0.1.0/conplex_dti/dataset/__init__.py
--rw-r--r--   0        0        0    24261 2023-04-26 19:32:40.233497 conplex_dti-0.1.0/conplex_dti/dataset/datamodules.py
--rw-r--r--   0        0        0      396 2023-03-11 20:36:53.100580 conplex_dti-0.1.0/conplex_dti/featurizer/__init__.py
--rw-r--r--   0        0        0     7731 2023-03-11 20:58:20.270334 conplex_dti-0.1.0/conplex_dti/featurizer/base.py
--rw-r--r--   0        0        0    11422 2023-03-11 20:28:46.233946 conplex_dti-0.1.0/conplex_dti/featurizer/molecule.py
--rw-r--r--   0        0        0    11536 2023-03-11 20:28:46.340599 conplex_dti-0.1.0/conplex_dti/featurizer/protein.py
--rw-r--r--   0        0        0        0 2023-03-11 17:54:11.289513 conplex_dti-0.1.0/conplex_dti/model/__init__.py
--rw-r--r--   0        0        0    23788 2023-03-11 21:37:21.488366 conplex_dti-0.1.0/conplex_dti/model/architectures.py
--rw-r--r--   0        0        0     2125 2023-03-11 20:35:20.124923 conplex_dti-0.1.0/conplex_dti/model/margin.py
--rw-r--r--   0        0        0     4025 2023-03-11 20:35:12.640083 conplex_dti-0.1.0/conplex_dti/utils.py
--rw-r--r--   0        0        0     4178 2023-04-26 19:49:57.912542 conplex_dti-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1854 1970-01-01 00:00:00.000000 conplex_dti-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-11 16:53:19.162872 conplex_dti-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3544 2023-04-27 21:09:41.869490 conplex_dti-0.1.1/README.md
+-rw-r--r--   0        0        0     3510 2023-04-27 20:13:59.889524 conplex_dti-0.1.1/conplex_dti/MAIN_OLD.txt
+-rw-r--r--   0        0        0      399 2023-06-12 15:18:13.332699 conplex_dti-0.1.1/conplex_dti/__init__.py
+-rw-r--r--   0        0        0     1070 2023-06-12 15:38:30.887853 conplex_dti-0.1.1/conplex_dti/__main__.py
+-rw-r--r--   0        0        0    23714 2023-04-27 20:13:59.892315 conplex_dti-0.1.1/conplex_dti/architectures.py
+-rw-r--r--   0        0        0      166 2023-04-27 20:13:59.893555 conplex_dti-0.1.1/conplex_dti/cli/__init__.py
+-rw-r--r--   0        0        0     1316 2023-04-27 20:13:59.894669 conplex_dti-0.1.1/conplex_dti/cli/download.py
+-rw-r--r--   0        0        0    19418 2023-06-12 15:34:12.673595 conplex_dti-0.1.1/conplex_dti/cli/train.py
+-rw-r--r--   0        0        0      171 2023-04-27 20:13:59.897366 conplex_dti-0.1.1/conplex_dti/dataset/__init__.py
+-rw-r--r--   0        0        0    24290 2023-04-27 21:07:43.467420 conplex_dti-0.1.1/conplex_dti/dataset/datamodules.py
+-rw-r--r--   0        0        0      421 2023-04-27 20:13:59.900173 conplex_dti-0.1.1/conplex_dti/featurizer/__init__.py
+-rw-r--r--   0        0        0     7731 2023-04-27 20:13:59.901288 conplex_dti-0.1.1/conplex_dti/featurizer/base.py
+-rw-r--r--   0        0        0    11422 2023-04-27 20:13:59.902654 conplex_dti-0.1.1/conplex_dti/featurizer/molecule.py
+-rw-r--r--   0        0        0    11493 2023-04-27 21:09:39.865982 conplex_dti-0.1.1/conplex_dti/featurizer/protein.py
+-rw-r--r--   0        0        0        0 2023-04-27 20:13:59.904417 conplex_dti-0.1.1/conplex_dti/model/__init__.py
+-rw-r--r--   0        0        0    23789 2023-04-27 20:13:59.906381 conplex_dti-0.1.1/conplex_dti/model/architectures.py
+-rw-r--r--   0        0        0     2125 2023-04-27 20:13:59.907393 conplex_dti-0.1.1/conplex_dti/model/margin.py
+-rw-r--r--   0        0        0     4022 2023-04-27 20:13:59.908432 conplex_dti-0.1.1/conplex_dti/utils.py
+-rw-r--r--   0        0        0     4177 2023-06-12 15:17:57.003372 conplex_dti-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5146 1970-01-01 00:00:00.000000 conplex_dti-0.1.1/PKG-INFO
```

### Comparing `conplex_dti-0.1.0/LICENSE` & `conplex_dti-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.0/conplex_dti/MAIN_OLD.txt` & `conplex_dti-0.1.1/conplex_dti/MAIN_OLD.txt`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.0/conplex_dti/__main__.py` & `conplex_dti-0.1.1/conplex_dti/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 """
 ConPLex: DTI Prediction
 """
 
-from conplex_dti import cli, version
 import argparse
 
-def main():
+from conplex_dti import __version__, cli
+
 
+def main():
     parser = argparse.ArgumentParser(description=__doc__)
 
     parser.add_argument(
-        "-v", "--version", action="version", version=f"ConPLex {version}"
+        "-v", "--version", action="version", version=f"ConPLex {__version__}"
     )
     # parser.add_argument(
     #     "-c",
     #     "--citation",
     #     action=CitationAction,
     #     nargs=0,
     #     help="show program's citation and exit",
     # )
 
     subparsers = parser.add_subparsers(title="ConPLex Commands", dest="cmd")
     subparsers.required = True
 
     modules = {
         "train": (cli.train, cli.train_parser),
+        "download": (cli.download, cli.download_parser),
         # "embed": embed,
         # "evaluate": evaluate,
         # "predict": predict,
     }
 
     for name, (main_func, args_func) in modules.items():
         sp = subparsers.add_parser(name, description=main_func.__doc__)
@@ -36,8 +38,8 @@
         sp.set_defaults(main_func=main_func)
 
     args = parser.parse_args()
     args.main_func(args)
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `conplex_dti-0.1.0/conplex_dti/architectures.py` & `conplex_dti-0.1.1/conplex_dti/architectures.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.0/conplex_dti/cli/train.py` & `conplex_dti-0.1.1/conplex_dti/cli/train.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,163 +1,232 @@
+import typing as T
+
 import copy
-from time import time
+import json
 import os
+from argparse import ArgumentParser
+from pathlib import Path
+from time import time
+
 import numpy as np
 import pandas as pd
 import torch
-import json
+import torchmetrics
+from omegaconf import OmegaConf
 from torch import nn
 from torch.autograd import Variable
 from torch.utils import data
 from tqdm.auto import tqdm
-import typing as T
-import torchmetrics
-
-from argparse import ArgumentParser
 
 import wandb
-from omegaconf import OmegaConf
-from pathlib import Path
 
-from ..model import architectures as model_types
-from ..model.margin import MarginScheduledLossFunction
 from ..dataset import (
-    get_task_dir,
     DTIDataModule,
-    TDCDataModule,
     DUDEDataModule,
     EnzPredDataModule,
-)
-from ..utils import (
-    set_random_seed,
-    config_logger,
-    get_logger,
+    TDCDataModule,
+    get_task_dir,
 )
 from ..featurizer import get_featurizer
+from ..model import architectures as model_types
+from ..model.margin import MarginScheduledLossFunction
+from ..utils import config_logger, get_logger, set_random_seed
 
 logg = get_logger()
 
+
 def add_args(parser: ArgumentParser):
+    parser.add_argument("--run-id", required=True, help="Experiment ID", dest="run_id")
     parser.add_argument(
-        "--run-id", required=True,help="Experiment ID", dest="run_id"
-    )
-    parser.add_argument(
-        "--config", help="YAML config file", default="configs/default_config.yaml"
+        "--config",
+        required=True,
+        help="YAML config file",
+        default="configs/default_config.yaml",
     )
 
-    parser.add_argument(
+    # Logging and Paths
+    log_group = parser.add_argument_group("Logging and Paths")
+
+    log_group.add_argument(
         "--wandb-proj",
         help="Weights and Biases Project",
         dest="wandb_proj",
     )
-    parser.add_argument(
+    log_group.add_argument(
+        "--wandb_save",
+        help="Log to Weights and Biases",
+        dest="wandb_save",
+        action="store_true",
+    )
+    log_group.add_argument(
+        "--log-file",
+        help="Log file",
+        dest="log_file",
+    )
+    log_group.add_argument(
+        "--model-save-dir",
+        help="Model save directory",
+        dest="model_save_dir",
+    )
+    log_group.add_argument(
+        "--data-cache-dir",
+        help="Data cache directory",
+        dest="data_cache_dir",
+    )
+
+    # Miscellaneous
+    misc_group = parser.add_argument_group("Miscellaneous")
+    misc_group.add_argument(
+        "--r", "--replicate", type=int, help="Replicate", dest="replicate"
+    )
+    misc_group.add_argument(
+        "--d", "--device", type=int, help="CUDA device", dest="device"
+    )
+    misc_group.add_argument(
+        "--verbosity", type=int, help="Level at which to log", dest="verbosity"
+    )
+    misc_group.add_argument(
+        "--checkpoint", default=None, help="Model weights to start from"
+    )
+
+    # Task and Dataset
+    task_group = parser.add_argument_group("Task and Dataset")
+
+    task_group.add_argument(
         "--task",
         choices=[
             "biosnap",
             "bindingdb",
             "davis",
             "biosnap_prot",
             "biosnap_mol",
             "dti_dg",
         ],
         type=str,
         help="Task name. Could be biosnap, bindingdb, davis, biosnap_prot, biosnap_mol.",
     )
+    task_group.add_argument(
+        "--contrastive-split",
+        type=str,
+        help="Contrastive split",
+        dest="contrastive_split",
+        choices=["within", "between"],
+    )
 
-    parser.add_argument(
+    # Model and Featurizers
+    model_group = parser.add_argument_group("Model and Featurizers")
+
+    model_group.add_argument(
         "--drug-featurizer", help="Drug featurizer", dest="drug_featurizer"
     )
-    parser.add_argument(
+    model_group.add_argument(
         "--target-featurizer", help="Target featurizer", dest="target_featurizer"
     )
-    parser.add_argument(
-        "--distance-metric",
-        help="Distance in embedding space to supervise with",
-        dest="distance_metric",
+    model_group.add_argument(
+        "--model-architecture", help="Model architecture", dest="model_architecture"
     )
-    parser.add_argument("--epochs", type=int, help="number of total epochs to run")
-    parser.add_argument("-b", "--batch-size", type=int, help="batch size")
-    parser.add_argument(
+    model_group.add_argument(
+        "--latent-dimension", help="Latent dimension", dest="latent_dimension"
+    )
+    model_group.add_argument(
+        "--latent-distance", help="Latent distance", dest="latent_distance"
+    )
+    # Training
+    train_group = parser.add_argument_group("Training")
+
+    train_group.add_argument("--epochs", type=int, help="number of total epochs to run")
+    train_group.add_argument("-b", "--batch-size", type=int, help="batch size")
+    train_group.add_argument(
+        "--cb", "--contrastive-batch-size", type=int, help="contrastive batch size"
+    )
+    train_group.add_argument("--shuffle", type=bool, help="shuffle data")
+    train_group.add_argument("--num-workers", type=int, help="number of workers")
+    train_group.add_argument("--every-n-val", type=int, help="validate every n epochs")
+
+    train_group.add_argument(
         "--lr",
         "--learning-rate",
         type=float,
         help="initial learning rate",
         dest="lr",
     )
-    parser.add_argument(
+    train_group.add_argument(
+        "--lr-t0", type=int, help="number of epochs to reset learning rate"
+    )
+    train_group.add_argument(
+        "--contrastive", type=bool, help="run contrastive training"
+    )
+    train_group.add_argument(
         "--clr", type=float, help="initial learning rate", dest="clr"
     )
-    parser.add_argument(
-        "--r", "--replicate", type=int, help="Replicate", dest="replicate"
+    train_group.add_argument(
+        "--clr-t0", type=int, help="number of epochs to reset learning rate"
     )
-    parser.add_argument(
-        "--d", "--device", type=int, help="CUDA device", dest="device"
+    train_group.add_argument(
+        "--margin-fn", type=str, help="margin function", dest="margin_fn"
     )
-    parser.add_argument(
-        "--verbosity", type=int, help="Level at which to log", dest="verbosity"
+    train_group.add_argument(
+        "--margin-max", type=float, help="margin max", dest="margin_max"
     )
-    parser.add_argument(
-        "--checkpoint", default=None, help="Model weights to start from"
+    train_group.add_argument(
+        "--margin-t0", type=int, help="number of epochs to reset margin"
     )
+
     return parser
 
 
 def test(model, data_generator, metrics, device=None, classify=True):
-
     if device is None:
         device = torch.device("cpu")
 
     metric_dict = {}
 
     for k, met_class in metrics.items():
         if classify:
-            met_instance = met_class(task = "binary")
+            met_instance = met_class(task="binary")
         else:
             met_instance = met_class()
         met_instance.to(device)
         met_instance.reset()
         metric_dict[k] = met_instance
 
     model.eval()
 
-    for i, batch in tqdm(enumerate(data_generator), total=len(data_generator)):
-
+    for _, batch in tqdm(enumerate(data_generator), total=len(data_generator)):
         pred, label = step(model, batch, device)
         if classify:
             label = label.int()
         else:
             label = label.float()
 
         for _, met_instance in metric_dict.items():
             met_instance(pred, label)
 
     results = {}
-    for (k, met_instance) in metric_dict.items():
+    for k, met_instance in metric_dict.items():
         res = met_instance.compute()
         results[k] = res
 
     for met_instance in metric_dict.values():
         met_instance.to("cpu")
 
     return results
 
 
 def step(model, batch, device=None):
-
     if device is None:
         device = torch.device("cpu")
 
     drug, target, label = batch  # target is (D + N_pool)
     pred = model(drug.to(device), target.to(device))
     label = Variable(torch.from_numpy(np.array(label)).float()).to(device)
     return pred, label
 
 
 def contrastive_step(model, batch, device=None):
-
     if device is None:
         device = torch.device("cpu")
 
     anchor, positive, negative = batch
 
     anchor_projection = model.target_projector(anchor.to(device))
     positive_projection = model.drug_projector(positive.to(device))
@@ -200,20 +269,18 @@
 
     # Set random state
     logg.debug(f"Setting random state {config.replicate}")
     set_random_seed(config.replicate)
 
     # Load DataModule
     logg.info("Preparing DataModule")
-    task_dir = get_task_dir(config.task, database_root = config.data_cache_dir)
+    task_dir = get_task_dir(config.task, database_root=config.data_cache_dir)
 
     drug_featurizer = get_featurizer(config.drug_featurizer, save_dir=task_dir)
-    target_featurizer = get_featurizer(
-        config.target_featurizer, save_dir=task_dir
-    )
+    target_featurizer = get_featurizer(config.target_featurizer, save_dir=task_dir)
 
     if config.task == "dti_dg":
         config.classify = False
         config.latent_activation = "GELU"
         config.watch_metric = "val/pcc"
         datamodule = TDCDataModule(
             task_dir,
@@ -316,18 +383,16 @@
         contrastive_loss_fct = MarginScheduledLossFunction(
             M_0=config.margin_max,
             N_epoch=config.epochs,
             N_restart=config.margin_t0,
             update_fn=config.margin_fn,
         )
         opt_contrastive = torch.optim.AdamW(model.parameters(), lr=config.clr)
-        lr_scheduler_contrastive = (
-            torch.optim.lr_scheduler.CosineAnnealingWarmRestarts(
-                opt_contrastive, T_0=config.clr_t0
-            )
+        lr_scheduler_contrastive = torch.optim.lr_scheduler.CosineAnnealingWarmRestarts(
+            opt_contrastive, T_0=config.clr_t0
         )
 
     # Metrics
     logg.info("Initializing metrics")
     max_metric = 0
     model_max = copy.deepcopy(model)
 
@@ -377,25 +442,21 @@
         model.train()
         epoch_time_start = time()
 
         # Main Step
         for i, batch in tqdm(
             enumerate(training_generator), total=len(training_generator)
         ):
-            pred, label = step(
-                model, batch, device
-            )  # batch is (2048, 1024, 1)
+            pred, label = step(model, batch, device)  # batch is (2048, 1024, 1)
 
             loss = loss_fct(pred, label)
 
             wandb_log(
                 {
-                    "train/step": (
-                        epo * len(training_generator) * config.batch_size
-                    )
+                    "train/step": (epo * len(training_generator) * config.batch_size)
                     + (i * config.batch_size),
                     "train/loss": loss,
                 },
                 do_wandb,
             )
 
             opt.zero_grad()
@@ -419,22 +480,17 @@
         # Contrastive Step
         if config.contrastive:
             logg.info(f"Training contrastive at Epoch {epo + 1}")
             for i, batch in tqdm(
                 enumerate(contrastive_generator),
                 total=len(contrastive_generator),
             ):
+                anchor, positive, negative = contrastive_step(model, batch, device)
 
-                anchor, positive, negative = contrastive_step(
-                    model, batch, device
-                )
-
-                contrastive_loss = contrastive_loss_fct(
-                    anchor, positive, negative
-                )
+                contrastive_loss = contrastive_loss_fct(anchor, positive, negative)
 
                 wandb_log(
                     {
                         "train/c_step": (
                             epo
                             * len(training_generator)
                             * config.contrastive_batch_size
@@ -463,24 +519,21 @@
 
             logg.info(
                 f"Training at Contrastive Epoch {epo + 1} with loss {contrastive_loss.cpu().detach().numpy():8f}"
             )
             logg.info(
                 f"Updating contrastive learning rate to {lr_scheduler_contrastive.get_lr()[0]:8f}"
             )
-            logg.info(
-                f"Updating contrastive margin to {contrastive_loss_fct.margin}"
-            )
+            logg.info(f"Updating contrastive margin to {contrastive_loss_fct.margin}")
 
         epoch_time_end = time()
 
         # Validation
         if epo % config.every_n_val == 0:
             with torch.set_grad_enabled(False):
-
                 val_results = test(
                     model,
                     validation_generator,
                     val_metrics,
                     device,
                     config.classify,
                 )
@@ -504,17 +557,15 @@
                     torch.save(
                         model_max.state_dict(),
                         model_save_path,
                     )
                     logg.info(f"Saving checkpoint model to {model_save_path}")
 
                     if do_wandb:
-                        art = wandb.Artifact(
-                            f"dti-{config.run_id}", type="model"
-                        )
+                        art = wandb.Artifact(f"dti-{config.run_id}", type="model")
                         art.add_file(model_save_path, model_save_path.name)
                         wandb.log_artifact(art, aliases=["best"])
 
                 logg.info(f"Validation at Epoch {epo + 1}")
                 for k, v in val_results.items():
                     if not k.startswith("_"):
                         logg.info(f"{k}: {v}")
@@ -543,31 +594,27 @@
             wandb_log(test_results, do_wandb)
 
             logg.info("Final Testing")
             for k, v in test_results.items():
                 if not k.startswith("_"):
                     logg.info(f"{k}: {v}")
 
-            model_save_path = Path(
-                f"{save_dir}/{config.run_id}_best_model.pt"
-            )
+            model_save_path = Path(f"{save_dir}/{config.run_id}_best_model.pt")
             torch.save(
                 model_max.state_dict(),
                 model_save_path,
             )
             logg.info(f"Saving final model to {model_save_path}")
 
             if do_wandb:
-                art = wandb.Artifact(
-                    f"dti-{config.run_id}", type="model"
-                )
+                art = wandb.Artifact(f"dti-{config.run_id}", type="model")
                 art.add_file(model_save_path, model_save_path.name)
                 wandb.log_artifact(art, aliases=["best"])
 
     except Exception as e:
         logg.error(f"Testing failed with exception {e}")
 
     return model_max
 
+
 if __name__ == "__main__":
     best_model = main()
-
```

### Comparing `conplex_dti-0.1.0/conplex_dti/dataset/datamodules.py` & `conplex_dti-0.1.1/conplex_dti/dataset/datamodules.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import sys
 from functools import lru_cache
 from pathlib import Path
 
 import pandas as pd
 import pytorch_lightning as pl
 import torch
-import torch.nn as nn
 from numpy.random import choice
 from sklearn.model_selection import KFold, train_test_split
 from tdc.benchmark_group import dti_dg_group
 from torch.nn.utils.rnn import pad_sequence
 from torch.utils.data import DataLoader, Dataset
 
 from ..featurizer import Featurizer
@@ -28,14 +27,16 @@
     """
     Get the path to data for each benchmark data set
 
     :param task_name: Name of benchmark
     :type task_name: str
     """
 
+    database_root = Path(database_root).resolve()
+
     task_paths = {
         "biosnap": database_root / "/BIOSNAP/full_data",
         "biosnap_prot": database_root / "BIOSNAP/unseen_protein",
         "biosnap_mol": database_root / "BIOSNAP/unseen_drug",
         "bindingdb": database_root / "BindingDB",
         "davis": database_root / "DAVIS",
         "dti_dg": database_root / "TDC",
```

### Comparing `conplex_dti-0.1.0/conplex_dti/featurizer/base.py` & `conplex_dti-0.1.1/conplex_dti/featurizer/base.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.0/conplex_dti/featurizer/molecule.py` & `conplex_dti-0.1.1/conplex_dti/featurizer/molecule.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.0/conplex_dti/featurizer/protein.py` & `conplex_dti-0.1.1/conplex_dti/featurizer/protein.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 from pathlib import Path
 
 import torch
 
 from ..utils import get_logger
 from .base import Featurizer
 
-# from dscript.language_model import lm_embed
-# from dscript.pretrained import get_pretrained
-
 logg = get_logger()
 
 MODEL_CACHE_DIR = Path(
     os.path.join(os.path.dirname(os.path.abspath(__file__)), "..", "..", "models")
 )
 FOLDSEEK_DEFAULT_PATH = Path(
     "/afs/csail.mit.edu/u/r/rsingh/work/corals/data-scratch1/ConPLex_foldseek_embeddings/r1_foldseekrep_encoding.p"
@@ -26,14 +23,15 @@
 
 os.makedirs(MODEL_CACHE_DIR, exist_ok=True)
 
 
 class BeplerBergerFeaturizer(Featurizer):
     def __init__(self, save_dir: Path = Path().absolute()):
         super().__init__("BeplerBerger", 6165, save_dir)
+        from dscript.language_model import lm_embed
 
         self._max_len = 800
         self._embed = lm_embed
 
     def _transform(self, seq):
         if len(seq) > self._max_len:
             seq = seq[: self._max_len]
```

### Comparing `conplex_dti-0.1.0/conplex_dti/model/architectures.py` & `conplex_dti-0.1.1/conplex_dti/model/architectures.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,14 +153,15 @@
 
         distance = self.activator(drug_projection, target_projection)
         return distance.squeeze()
 
 
 SimpleCoembeddingNoSigmoid = SimpleCoembedding
 
+
 class SimpleCoembeddingSigmoid(nn.Module):
     def __init__(
         self,
         drug_shape=2048,
         target_shape=1024,
         latent_dimension=1024,
         latent_activation=nn.ReLU,
```

### Comparing `conplex_dti-0.1.0/conplex_dti/model/margin.py` & `conplex_dti-0.1.1/conplex_dti/model/margin.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.0/conplex_dti/utils.py` & `conplex_dti-0.1.1/conplex_dti/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 import typing as T
 
 import logging as lg
 import multiprocessing as mp
-import os
 import sys
 from functools import partial
 from pathlib import Path
 
 import h5py
 import numpy as np
-import pandas as pd
 import torch
-import torch.nn as nn
 from omegaconf import OmegaConf
 from rdkit import Chem, DataStructs
 from rdkit.Chem import AllChem
-from torch.utils.data import DataLoader, Dataset
 from tqdm import tqdm
 
 logLevels = {0: lg.ERROR, 1: lg.WARNING, 2: lg.INFO, 3: lg.DEBUG}
 LOGGER_NAME = "DTI"
 
 
-def get_logger():
-    return lg.getLogger(LOGGER_NAME)
+def get_logger(logger_name: str = None) -> lg.Logger:
+    if logger_name is None:
+        logger_name = LOGGER_NAME
+    return lg.getLogger(logger_name)
 
 
 logg = get_logger()
 
 
 def config_logger(
     file: T.Union[Path, None],
```

### Comparing `conplex_dti-0.1.0/pyproject.toml` & `conplex_dti-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "conplex-dti"
-version = "0.1.0"
+version = "0.1.1"
 description = "Adapting protein language models and contrastive learning for DTI prediction."
 readme = "README.md"
 authors = ["samsledje <samsl@mit.edu>"]
 license = "MIT"
 repository = "https://github.com/samsledje/ConPLex"
 homepage = "https://github.com/samsledje/ConPLex"
 
@@ -98,15 +98,14 @@
 )/
 '''
 
 [tool.isort]
 # https://github.com/timothycrosley/isort/
 py_version = 39
 line_length = 88
-
 known_typing = ["typing", "types", "typing_extensions", "mypy", "mypy_extensions"]
 sections = ["FUTURE", "TYPING", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
 include_trailing_comma = true
 profile = "black"
 multi_line_output = 3
 indent = 4
 color_output = true
```

