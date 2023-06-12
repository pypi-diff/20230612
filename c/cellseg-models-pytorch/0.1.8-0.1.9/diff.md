# Comparing `tmp/cellseg_models_pytorch-0.1.8.tar.gz` & `tmp/cellseg_models_pytorch-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellseg_models_pytorch-0.1.8.tar", max compression
+gzip compressed data, was "cellseg_models_pytorch-0.1.9.tar", max compression
```

## Comparing `cellseg_models_pytorch-0.1.8.tar` & `cellseg_models_pytorch-0.1.9.tar`

### file list

```diff
@@ -1,194 +1,194 @@
--rw-r--r--   0        0        0     1065 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/LICENSE
--rw-r--r--   0        0        0    14372 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/README.md
--rw-r--r--   0        0        0      298 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/__init__.py
--rw-r--r--   0        0        0      299 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datamodules/__init__.py
--rw-r--r--   0        0        0     2424 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datamodules/_basemodule.py
--rw-r--r--   0        0        0     1991 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datamodules/custom_datamodule.py
--rw-r--r--   0        0        0     5077 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datamodules/downloader.py
--rw-r--r--   0        0        0    14355 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datamodules/lizard_datamodule.py
--rw-r--r--   0        0        0    11261 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datamodules/pannuke_datamodule.py
--rw-r--r--   0        0        0        0 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datamodules/tests/__init__.py
--rw-r--r--   0        0        0      195 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/__init__.py
--rw-r--r--   0        0        0     5927 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/_base_dataset.py
--rw-r--r--   0        0        0      145 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/dataset_writers/__init__.py
--rw-r--r--   0        0        0     5714 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/dataset_writers/_base_writer.py
--rw-r--r--   0        0        0     4232 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/dataset_writers/folder_writer.py
--rw-r--r--   0        0        0     6512 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/dataset_writers/hdf5_writer.py
--rw-r--r--   0        0        0     6669 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/folder_dataset_train.py
--rw-r--r--   0        0        0     5585 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/hdf5_dataset.py
--rw-r--r--   0        0        0        0 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/tests/__init__.py
--rw-r--r--   0        0        0   124358 2022-10-18 16:01:10.732021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/tests/data/imgs/patch1.png
--rw-r--r--   0        0        0   134238 2022-10-18 16:01:10.736021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/tests/data/imgs/patch2.png
--rw-r--r--   0        0        0   131893 2022-10-18 16:01:10.736021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/tests/data/imgs/patch3.png
--rw-r--r--   0        0        0   788008 2022-10-18 16:01:10.740021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/tests/data/masks/patch1.mat
--rw-r--r--   0        0        0   789416 2022-10-18 16:01:10.740021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/tests/data/masks/patch2.mat
--rw-r--r--   0        0        0   789984 2022-10-18 16:01:10.740021 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/tests/data/masks/patch3.mat
--rw-r--r--   0        0        0  1854220 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/tests/data/tiny_test.h5
--rw-r--r--   0        0        0     1366 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/tests/test_dataset.py
--rw-r--r--   0        0        0      108 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/__init__.py
--rw-r--r--   0        0        0     4263 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/decoder.py
--rw-r--r--   0        0        0     9300 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/decoder_stage.py
--rw-r--r--   0        0        0       62 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/long_skips/__init__.py
--rw-r--r--   0        0        0     1533 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/long_skips/longskip_module.py
--rw-r--r--   0        0        0       52 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/long_skips/merging/__init__.py
--rw-r--r--   0        0        0     1582 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/long_skips/merging/cat.py
--rw-r--r--   0        0        0     1412 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/long_skips/merging/merge_block.py
--rw-r--r--   0        0        0     2877 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/long_skips/merging/sum.py
--rw-r--r--   0        0        0     2724 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/long_skips/unet.py
--rw-r--r--   0        0        0    15051 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/long_skips/unet3p.py
--rw-r--r--   0        0        0     9798 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/long_skips/unetpp.py
--rw-r--r--   0        0        0        0 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/tests/__init__.py
--rw-r--r--   0        0        0     5755 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/tests/test_decoders.py
--rw-r--r--   0        0        0      423 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/tests/test_merge.py
--rw-r--r--   0        0        0      397 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/__init__.py
--rw-r--r--   0        0        0    14250 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/_base_inferer.py
--rw-r--r--   0        0        0     1992 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/folder_dataset.py
--rw-r--r--   0        0        0     6282 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/post_processor.py
--rw-r--r--   0        0        0     6734 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/predictor.py
--rw-r--r--   0        0        0     6173 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/resize_inferer.py
--rw-r--r--   0        0        0     8897 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/sliding_window_inferer.py
--rw-r--r--   0        0        0        0 2022-10-18 16:01:10.756022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/tests/__init__.py
--rw-r--r--   0        0        0   523557 2022-10-18 16:01:10.760022 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/tests/data/test1.png
--rw-r--r--   0        0        0   488842 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/tests/data/test2.png
--rw-r--r--   0        0        0     1651 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/tests/test_inference.py
--rw-r--r--   0        0        0      702 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/__init__.py
--rw-r--r--   0        0        0      686 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/__init__.py
--rw-r--r--   0        0        0     2872 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/ce.py
--rw-r--r--   0        0        0     3051 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/dice.py
--rw-r--r--   0        0        0     3396 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/focal.py
--rw-r--r--   0        0        0     2084 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/grad_mse.py
--rw-r--r--   0        0        0     3019 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/iou.py
--rw-r--r--   0        0        0     2918 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/mse.py
--rw-r--r--   0        0        0     3397 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/sce.py
--rw-r--r--   0        0        0     5322 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/ssim.py
--rw-r--r--   0        0        0     3448 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/tversky.py
--rw-r--r--   0        0        0     1802 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/joint_loss.py
--rw-r--r--   0        0        0     2051 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/loss_module.py
--rw-r--r--   0        0        0     2992 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/multitask_loss.py
--rw-r--r--   0        0        0      657 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/tests/test_jointloss.py
--rw-r--r--   0        0        0     2546 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/tests/test_losses.py
--rw-r--r--   0        0        0      781 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/tests/test_multitask_loss.py
--rw-r--r--   0        0        0     5900 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/weighted_base_loss.py
--rw-r--r--   0        0        0      798 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/metrics/__init__.py
--rw-r--r--   0        0        0     3514 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/metrics/binary_metrics.py
--rw-r--r--   0        0        0    14556 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/metrics/functional.py
--rw-r--r--   0        0        0        0 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/metrics/tests/__init__.py
--rw-r--r--   0        0        0     2218 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/metrics/tests/test_binary_metrics.py
--rw-r--r--   0        0        0     5411 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/metrics/tests/test_instance_metrics.py
--rw-r--r--   0        0        0      924 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/metrics/tests/test_semantic_metrics.py
--rw-r--r--   0        0        0      771 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/__init__.py
--rw-r--r--   0        0        0        0 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/base/__init__.py
--rw-r--r--   0        0        0     5211 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/base/_base_model.py
--rw-r--r--   0        0        0     1468 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/base/_initialization.py
--rw-r--r--   0        0        0     5573 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/base/_multitask_unet.py
--rw-r--r--   0        0        0     1138 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/base/_seg_head.py
--rw-r--r--   0        0        0      929 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/base/_timm_encoder.py
--rw-r--r--   0        0        0     1558 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/cellpose/_conf.py
--rw-r--r--   0        0        0    11482 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/cellpose/cellpose.py
--rw-r--r--   0        0        0     3708 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/hovernet/_conf.py
--rw-r--r--   0        0        0    11476 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/hovernet/hovernet.py
--rw-r--r--   0        0        0     1478 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/stardist/_conf.py
--rw-r--r--   0        0        0    12287 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/stardist/stardist.py
--rw-r--r--   0        0        0        0 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/tests/__init__.py
--rw-r--r--   0        0        0     2496 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/tests/test_models.py
--rw-r--r--   0        0        0      306 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/__init__.py
--rw-r--r--   0        0        0      960 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/act/__init__.py
--rw-r--r--   0        0        0     1949 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/act/mish.py
--rw-r--r--   0        0        0     1722 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/act/swish.py
--rw-r--r--   0        0        0     9412 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/attention_modules.py
--rw-r--r--   0        0        0     4356 2022-10-18 16:01:10.764023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/base_modules.py
--rw-r--r--   0        0        0      245 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/conv/__init__.py
--rw-r--r--   0        0        0     1924 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/conv/scaled_ws_conv.py
--rw-r--r--   0        0        0     1577 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/conv/ws_conv.py
--rw-r--r--   0        0        0    32050 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/conv_base.py
--rw-r--r--   0        0        0     7253 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/conv_block.py
--rw-r--r--   0        0        0     7876 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/conv_layer.py
--rw-r--r--   0        0        0     4125 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/misc_modules.py
--rw-r--r--   0        0        0      420 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/norm/__init__.py
--rw-r--r--   0        0        0     1937 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/norm/bcn.py
--rw-r--r--   0        0        0      933 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/norm/gn.py
--rw-r--r--   0        0        0      794 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/norm/ln.py
--rw-r--r--   0        0        0        0 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/tests/__init__.py
--rw-r--r--   0        0        0      698 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/tests/test_attention.py
--rw-r--r--   0        0        0     1336 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/tests/test_basemodules.py
--rw-r--r--   0        0        0     1211 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/tests/test_conv_blocks.py
--rw-r--r--   0        0        0     1243 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/tests/test_convlayer.py
--rw-r--r--   0        0        0     1085 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/tests/test_miscmodules.py
--rw-r--r--   0        0        0      292 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/upsample/__init__.py
--rw-r--r--   0        0        0     1415 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/upsample/fixed_unpool.py
--rw-r--r--   0        0        0     2446 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/optimizers/__init__.py
--rw-r--r--   0        0        0        0 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/optimizers/tests/__init__.py
--rw-r--r--   0        0        0      750 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/optimizers/tests/test_optim_setup.py
--rw-r--r--   0        0        0     1105 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/optimizers/utils.py
--rw-r--r--   0        0        0     1417 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/__init__.py
--rw-r--r--   0        0        0        0 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/__init__.py
--rw-r--r--   0        0        0     9348 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/cellpose/_old_cellpose.py
--rw-r--r--   0        0        0     6343 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/cellpose/cellpose.py
--rw-r--r--   0        0        0     5649 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/cellpose/integrator.py
--rw-r--r--   0        0        0     4133 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/cellpose/utils.py
--rw-r--r--   0        0        0     2357 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/dcan.py
--rw-r--r--   0        0        0     1529 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/dran.py
--rw-r--r--   0        0        0     5014 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/drfns.py
--rw-r--r--   0        0        0     3709 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/hovernet.py
--rw-r--r--   0        0        0     6175 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/omnipose.py
--rw-r--r--   0        0        0    10332 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/stardist.py
--rw-r--r--   0        0        0        0 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/tests/__init__.py
--rw-r--r--   0        0        0     3452 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/tests/test_postproc.py
--rw-r--r--   0        0        0        0 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/__init__.py
--rw-r--r--   0        0        0      115 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/callbacks/__init__.py
--rw-r--r--   0        0        0     5610 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/callbacks/metric_callbacks.py
--rw-r--r--   0        0        0    16536 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/callbacks/wandb_callbacks.py
--rw-r--r--   0        0        0      104 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/functional/__init__.py
--rw-r--r--   0        0        0     3790 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/functional/train_metrics.py
--rw-r--r--   0        0        0       95 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/lit/__init__.py
--rw-r--r--   0        0        0    12493 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/lit/lightning_experiment.py
--rw-r--r--   0        0        0        0 2022-10-18 16:01:10.768023 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/tests/__init__.py
--rw-r--r--   0        0        0  6554360 2022-10-18 16:01:10.784024 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/tests/data/sem_target_batch8.pt
--rw-r--r--   0        0        0  6554360 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/tests/data/type_target_batch8.pt
--rw-r--r--   0        0        0      596 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/tests/test_metrics.py
--rw-r--r--   0        0        0     1486 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/tests/test_training.py
--rw-r--r--   0        0        0        0 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/__init__.py
--rw-r--r--   0        0        0     2734 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/albu_transforms/__init__.py
--rw-r--r--   0        0        0     4704 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/albu_transforms/_composition.py
--rw-r--r--   0        0        0     5326 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/albu_transforms/img_transforms.py
--rw-r--r--   0        0        0    10230 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/albu_transforms/inst_transforms.py
--rw-r--r--   0        0        0     4293 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/albu_transforms/norm_transforms.py
--rw-r--r--   0        0        0      575 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/functional/__init__.py
--rw-r--r--   0        0        0     5111 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/functional/cellpose.py
--rw-r--r--   0        0        0     2113 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/functional/contour.py
--rw-r--r--   0        0        0     3088 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/functional/dist.py
--rw-r--r--   0        0        0     3069 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/functional/edge_weights.py
--rw-r--r--   0        0        0     4408 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/functional/hovernet.py
--rw-r--r--   0        0        0     7331 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/functional/omnipose.py
--rw-r--r--   0        0        0     9676 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/functional/stardist.py
--rw-r--r--   0        0        0        0 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/tests/__init__.py
--rw-r--r--   0        0        0     1348 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/tests/test_full_pipeline.py
--rw-r--r--   0        0        0     1609 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/tests/test_img_transforms.py
--rw-r--r--   0        0        0     2995 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/tests/test_inst_transforms.py
--rw-r--r--   0        0        0      714 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/tests/test_norm_transforms.py
--rw-r--r--   0        0        0     2989 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/__init__.py
--rw-r--r--   0        0        0     4757 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/file_manager.py
--rw-r--r--   0        0        0     5550 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/img_utils.py
--rw-r--r--   0        0        0    15320 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/latency_benchmark.py
--rw-r--r--   0        0        0    29813 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/mask_utils.py
--rw-r--r--   0        0        0    12316 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/patching.py
--rw-r--r--   0        0        0     1817 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/save_utils.py
--rw-r--r--   0        0        0    10483 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/seg_benchmark.py
--rw-r--r--   0        0        0     6527 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tensor_img_utlls.py
--rw-r--r--   0        0        0     3833 2022-10-18 16:01:10.800025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tensor_kernels.py
--rw-r--r--   0        0        0     6706 2022-10-18 16:01:10.804025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tensor_utils.py
--rw-r--r--   0        0        0        0 2022-10-18 16:01:10.804025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/__init__.py
--rw-r--r--   0        0        0   510600 2022-10-18 16:01:10.804025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/data/HE.png
--rw-r--r--   0        0        0     1835 2022-10-18 16:01:10.804025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_img_utils.py
--rw-r--r--   0        0        0      701 2022-10-18 16:01:10.804025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_kernels.py
--rw-r--r--   0        0        0     1178 2022-10-18 16:01:10.804025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_latency_benchmarker.py
--rw-r--r--   0        0        0    11935 2022-10-18 16:01:10.804025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_mask_utils.py
--rw-r--r--   0        0        0     2818 2022-10-18 16:01:10.804025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_patching.py
--rw-r--r--   0        0        0      656 2022-10-18 16:01:10.804025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_seg_benchmark.py
--rw-r--r--   0        0        0     1118 2022-10-18 16:01:10.804025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_tensor_img_utils.py
--rw-r--r--   0        0        0     1810 2022-10-18 16:01:10.804025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_tensor_utils.py
--rw-r--r--   0        0        0      819 2022-10-18 16:01:10.804025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_thresholding.py
--rw-r--r--   0        0        0     4088 2022-10-18 16:01:10.804025 cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/thresholding.py
--rw-r--r--   0        0        0     2692 2022-10-18 16:01:10.848028 cellseg_models_pytorch-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    18117 1970-01-01 00:00:00.000000 cellseg_models_pytorch-0.1.8/setup.py
--rw-r--r--   0        0        0    15902 1970-01-01 00:00:00.000000 cellseg_models_pytorch-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-10-21 08:36:56.265349 cellseg_models_pytorch-0.1.9/LICENSE
+-rw-r--r--   0        0        0    14372 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/README.md
+-rw-r--r--   0        0        0      298 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/__init__.py
+-rw-r--r--   0        0        0      299 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datamodules/__init__.py
+-rw-r--r--   0        0        0     2424 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datamodules/_basemodule.py
+-rw-r--r--   0        0        0     1991 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datamodules/custom_datamodule.py
+-rw-r--r--   0        0        0     5077 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datamodules/downloader.py
+-rw-r--r--   0        0        0    14355 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datamodules/lizard_datamodule.py
+-rw-r--r--   0        0        0    11261 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datamodules/pannuke_datamodule.py
+-rw-r--r--   0        0        0        0 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datamodules/tests/__init__.py
+-rw-r--r--   0        0        0      195 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/__init__.py
+-rw-r--r--   0        0        0     5927 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/_base_dataset.py
+-rw-r--r--   0        0        0      145 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/dataset_writers/__init__.py
+-rw-r--r--   0        0        0     5713 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/dataset_writers/_base_writer.py
+-rw-r--r--   0        0        0     4232 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/dataset_writers/folder_writer.py
+-rw-r--r--   0        0        0     6512 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/dataset_writers/hdf5_writer.py
+-rw-r--r--   0        0        0     6668 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/folder_dataset_train.py
+-rw-r--r--   0        0        0     5585 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/hdf5_dataset.py
+-rw-r--r--   0        0        0        0 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/tests/__init__.py
+-rw-r--r--   0        0        0   124358 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/tests/data/imgs/patch1.png
+-rw-r--r--   0        0        0   134238 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/tests/data/imgs/patch2.png
+-rw-r--r--   0        0        0   131893 2022-10-21 08:36:56.269349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/tests/data/imgs/patch3.png
+-rw-r--r--   0        0        0   788008 2022-10-21 08:36:56.273349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/tests/data/masks/patch1.mat
+-rw-r--r--   0        0        0   789416 2022-10-21 08:36:56.273349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/tests/data/masks/patch2.mat
+-rw-r--r--   0        0        0   789984 2022-10-21 08:36:56.277349 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/tests/data/masks/patch3.mat
+-rw-r--r--   0        0        0  1854220 2022-10-21 08:36:56.289348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/tests/data/tiny_test.h5
+-rw-r--r--   0        0        0     1366 2022-10-21 08:36:56.289348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/tests/test_dataset.py
+-rw-r--r--   0        0        0      108 2022-10-21 08:36:56.289348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/__init__.py
+-rw-r--r--   0        0        0     4263 2022-10-21 08:36:56.289348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/decoder.py
+-rw-r--r--   0        0        0     9300 2022-10-21 08:36:56.289348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/decoder_stage.py
+-rw-r--r--   0        0        0       62 2022-10-21 08:36:56.289348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/long_skips/__init__.py
+-rw-r--r--   0        0        0     1533 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/long_skips/longskip_module.py
+-rw-r--r--   0        0        0       52 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/long_skips/merging/__init__.py
+-rw-r--r--   0        0        0     1582 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/long_skips/merging/cat.py
+-rw-r--r--   0        0        0     1412 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/long_skips/merging/merge_block.py
+-rw-r--r--   0        0        0     2877 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/long_skips/merging/sum.py
+-rw-r--r--   0        0        0     2724 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/long_skips/unet.py
+-rw-r--r--   0        0        0    15051 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/long_skips/unet3p.py
+-rw-r--r--   0        0        0     9798 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/long_skips/unetpp.py
+-rw-r--r--   0        0        0        0 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/tests/__init__.py
+-rw-r--r--   0        0        0     5755 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/tests/test_decoders.py
+-rw-r--r--   0        0        0      423 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/tests/test_merge.py
+-rw-r--r--   0        0        0      397 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/__init__.py
+-rw-r--r--   0        0        0    13158 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/_base_inferer.py
+-rw-r--r--   0        0        0     1992 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/folder_dataset.py
+-rw-r--r--   0        0        0     6282 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/post_processor.py
+-rw-r--r--   0        0        0     6734 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/predictor.py
+-rw-r--r--   0        0        0     6024 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/resize_inferer.py
+-rw-r--r--   0        0        0     8821 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/sliding_window_inferer.py
+-rw-r--r--   0        0        0        0 2022-10-21 08:36:56.293348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/tests/__init__.py
+-rw-r--r--   0        0        0   523557 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/tests/data/test1.png
+-rw-r--r--   0        0        0   488842 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/tests/data/test2.png
+-rw-r--r--   0        0        0     1651 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/tests/test_inference.py
+-rw-r--r--   0        0        0      702 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/__init__.py
+-rw-r--r--   0        0        0      686 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/__init__.py
+-rw-r--r--   0        0        0     2872 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/ce.py
+-rw-r--r--   0        0        0     3051 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/dice.py
+-rw-r--r--   0        0        0     3396 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/focal.py
+-rw-r--r--   0        0        0     2084 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/grad_mse.py
+-rw-r--r--   0        0        0     3019 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/iou.py
+-rw-r--r--   0        0        0     2918 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/mse.py
+-rw-r--r--   0        0        0     3397 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/sce.py
+-rw-r--r--   0        0        0     5322 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/ssim.py
+-rw-r--r--   0        0        0     3448 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/tversky.py
+-rw-r--r--   0        0        0     1802 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/joint_loss.py
+-rw-r--r--   0        0        0     2051 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/loss_module.py
+-rw-r--r--   0        0        0     2992 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/multitask_loss.py
+-rw-r--r--   0        0        0      657 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/tests/test_jointloss.py
+-rw-r--r--   0        0        0     2546 2022-10-21 08:36:56.297348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/tests/test_losses.py
+-rw-r--r--   0        0        0      781 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/tests/test_multitask_loss.py
+-rw-r--r--   0        0        0     5900 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/weighted_base_loss.py
+-rw-r--r--   0        0        0      798 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/metrics/__init__.py
+-rw-r--r--   0        0        0     3514 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/metrics/binary_metrics.py
+-rw-r--r--   0        0        0    14556 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/metrics/functional.py
+-rw-r--r--   0        0        0        0 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/metrics/tests/__init__.py
+-rw-r--r--   0        0        0     2218 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/metrics/tests/test_binary_metrics.py
+-rw-r--r--   0        0        0     5411 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/metrics/tests/test_instance_metrics.py
+-rw-r--r--   0        0        0      924 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/metrics/tests/test_semantic_metrics.py
+-rw-r--r--   0        0        0      771 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/base/__init__.py
+-rw-r--r--   0        0        0     5211 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/base/_base_model.py
+-rw-r--r--   0        0        0     1468 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/base/_initialization.py
+-rw-r--r--   0        0        0     5573 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/base/_multitask_unet.py
+-rw-r--r--   0        0        0     1138 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/base/_seg_head.py
+-rw-r--r--   0        0        0      929 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/base/_timm_encoder.py
+-rw-r--r--   0        0        0     1558 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/cellpose/_conf.py
+-rw-r--r--   0        0        0    11482 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/cellpose/cellpose.py
+-rw-r--r--   0        0        0     3708 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/hovernet/_conf.py
+-rw-r--r--   0        0        0    11476 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/hovernet/hovernet.py
+-rw-r--r--   0        0        0     1478 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/stardist/_conf.py
+-rw-r--r--   0        0        0    12287 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/stardist/stardist.py
+-rw-r--r--   0        0        0        0 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/tests/__init__.py
+-rw-r--r--   0        0        0     2496 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/tests/test_models.py
+-rw-r--r--   0        0        0      306 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/__init__.py
+-rw-r--r--   0        0        0      960 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/act/__init__.py
+-rw-r--r--   0        0        0     1949 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/act/mish.py
+-rw-r--r--   0        0        0     1722 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/act/swish.py
+-rw-r--r--   0        0        0     9412 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/attention_modules.py
+-rw-r--r--   0        0        0     4356 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/base_modules.py
+-rw-r--r--   0        0        0      245 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/conv/__init__.py
+-rw-r--r--   0        0        0     1924 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/conv/scaled_ws_conv.py
+-rw-r--r--   0        0        0     1577 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/conv/ws_conv.py
+-rw-r--r--   0        0        0    32050 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/conv_base.py
+-rw-r--r--   0        0        0     7253 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/conv_block.py
+-rw-r--r--   0        0        0     7876 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/conv_layer.py
+-rw-r--r--   0        0        0     4125 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/misc_modules.py
+-rw-r--r--   0        0        0      420 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/norm/__init__.py
+-rw-r--r--   0        0        0     1937 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/norm/bcn.py
+-rw-r--r--   0        0        0      933 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/norm/gn.py
+-rw-r--r--   0        0        0      794 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/norm/ln.py
+-rw-r--r--   0        0        0        0 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/tests/__init__.py
+-rw-r--r--   0        0        0      698 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/tests/test_attention.py
+-rw-r--r--   0        0        0     1336 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/tests/test_basemodules.py
+-rw-r--r--   0        0        0     1211 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/tests/test_conv_blocks.py
+-rw-r--r--   0        0        0     1243 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/tests/test_convlayer.py
+-rw-r--r--   0        0        0     1085 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/tests/test_miscmodules.py
+-rw-r--r--   0        0        0      292 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/upsample/__init__.py
+-rw-r--r--   0        0        0     1415 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/upsample/fixed_unpool.py
+-rw-r--r--   0        0        0     2446 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/optimizers/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/optimizers/tests/__init__.py
+-rw-r--r--   0        0        0      750 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/optimizers/tests/test_optim_setup.py
+-rw-r--r--   0        0        0     1105 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/optimizers/utils.py
+-rw-r--r--   0        0        0     1417 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/__init__.py
+-rw-r--r--   0        0        0     9348 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/cellpose/_old_cellpose.py
+-rw-r--r--   0        0        0     6343 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/cellpose/cellpose.py
+-rw-r--r--   0        0        0     5649 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/cellpose/integrator.py
+-rw-r--r--   0        0        0     4133 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/cellpose/utils.py
+-rw-r--r--   0        0        0     2357 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/dcan.py
+-rw-r--r--   0        0        0     1529 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/dran.py
+-rw-r--r--   0        0        0     5014 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/drfns.py
+-rw-r--r--   0        0        0     3709 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/hovernet.py
+-rw-r--r--   0        0        0     6175 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/omnipose.py
+-rw-r--r--   0        0        0    10332 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/stardist.py
+-rw-r--r--   0        0        0        0 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/tests/__init__.py
+-rw-r--r--   0        0        0     3451 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/tests/test_postproc.py
+-rw-r--r--   0        0        0        0 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/__init__.py
+-rw-r--r--   0        0        0      115 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/callbacks/__init__.py
+-rw-r--r--   0        0        0     5610 2022-10-21 08:36:56.301348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/callbacks/metric_callbacks.py
+-rw-r--r--   0        0        0    16536 2022-10-21 08:36:56.305348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/callbacks/wandb_callbacks.py
+-rw-r--r--   0        0        0      104 2022-10-21 08:36:56.305348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/functional/__init__.py
+-rw-r--r--   0        0        0     3790 2022-10-21 08:36:56.305348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/functional/train_metrics.py
+-rw-r--r--   0        0        0       95 2022-10-21 08:36:56.305348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/lit/__init__.py
+-rw-r--r--   0        0        0    12493 2022-10-21 08:36:56.305348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/lit/lightning_experiment.py
+-rw-r--r--   0        0        0        0 2022-10-21 08:36:56.305348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/tests/__init__.py
+-rw-r--r--   0        0        0  6554360 2022-10-21 08:36:56.317348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/tests/data/sem_target_batch8.pt
+-rw-r--r--   0        0        0  6554360 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/tests/data/type_target_batch8.pt
+-rw-r--r--   0        0        0      596 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/tests/test_metrics.py
+-rw-r--r--   0        0        0     1486 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/tests/test_training.py
+-rw-r--r--   0        0        0        0 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/__init__.py
+-rw-r--r--   0        0        0     2734 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/albu_transforms/__init__.py
+-rw-r--r--   0        0        0     4704 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/albu_transforms/_composition.py
+-rw-r--r--   0        0        0     5326 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/albu_transforms/img_transforms.py
+-rw-r--r--   0        0        0    10230 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/albu_transforms/inst_transforms.py
+-rw-r--r--   0        0        0     4293 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/albu_transforms/norm_transforms.py
+-rw-r--r--   0        0        0      575 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/functional/__init__.py
+-rw-r--r--   0        0        0     5111 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/functional/cellpose.py
+-rw-r--r--   0        0        0     2113 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/functional/contour.py
+-rw-r--r--   0        0        0     3088 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/functional/dist.py
+-rw-r--r--   0        0        0     3069 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/functional/edge_weights.py
+-rw-r--r--   0        0        0     4408 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/functional/hovernet.py
+-rw-r--r--   0        0        0     7331 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/functional/omnipose.py
+-rw-r--r--   0        0        0     9676 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/functional/stardist.py
+-rw-r--r--   0        0        0        0 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/tests/__init__.py
+-rw-r--r--   0        0        0     1348 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/tests/test_full_pipeline.py
+-rw-r--r--   0        0        0     1609 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/tests/test_img_transforms.py
+-rw-r--r--   0        0        0     2995 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/tests/test_inst_transforms.py
+-rw-r--r--   0        0        0      714 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/tests/test_norm_transforms.py
+-rw-r--r--   0        0        0     2989 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/__init__.py
+-rw-r--r--   0        0        0    18716 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/file_manager.py
+-rw-r--r--   0        0        0     5550 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/img_utils.py
+-rw-r--r--   0        0        0    15320 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/latency_benchmark.py
+-rw-r--r--   0        0        0    29822 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/mask_utils.py
+-rw-r--r--   0        0        0    12316 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/patching.py
+-rw-r--r--   0        0        0    10481 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/seg_benchmark.py
+-rw-r--r--   0        0        0     6527 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tensor_img_utlls.py
+-rw-r--r--   0        0        0     3833 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tensor_kernels.py
+-rw-r--r--   0        0        0     6706 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tensor_utils.py
+-rw-r--r--   0        0        0        0 2022-10-21 08:36:56.333348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/__init__.py
+-rw-r--r--   0        0        0   510600 2022-10-21 08:36:56.337348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/data/HE.png
+-rw-r--r--   0        0        0      433 2022-10-21 08:36:56.337348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_filehandler.py
+-rw-r--r--   0        0        0     1835 2022-10-21 08:36:56.337348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_img_utils.py
+-rw-r--r--   0        0        0      701 2022-10-21 08:36:56.337348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_kernels.py
+-rw-r--r--   0        0        0     1232 2022-10-21 08:36:56.337348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_latency_benchmarker.py
+-rw-r--r--   0        0        0    11934 2022-10-21 08:36:56.337348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_mask_utils.py
+-rw-r--r--   0        0        0     2818 2022-10-21 08:36:56.337348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_patching.py
+-rw-r--r--   0        0        0      656 2022-10-21 08:36:56.337348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_seg_benchmark.py
+-rw-r--r--   0        0        0     1118 2022-10-21 08:36:56.337348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_tensor_img_utils.py
+-rw-r--r--   0        0        0     1810 2022-10-21 08:36:56.337348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_tensor_utils.py
+-rw-r--r--   0        0        0      819 2022-10-21 08:36:56.337348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_thresholding.py
+-rw-r--r--   0        0        0     4088 2022-10-21 08:36:56.337348 cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/thresholding.py
+-rw-r--r--   0        0        0     2852 2022-10-21 08:36:56.381347 cellseg_models_pytorch-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    18200 1970-01-01 00:00:00.000000 cellseg_models_pytorch-0.1.9/setup.py
+-rw-r--r--   0        0        0    16029 1970-01-01 00:00:00.000000 cellseg_models_pytorch-0.1.9/PKG-INFO
```

### Comparing `cellseg_models_pytorch-0.1.8/LICENSE` & `cellseg_models_pytorch-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/README.md` & `cellseg_models_pytorch-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datamodules/_basemodule.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datamodules/_basemodule.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datamodules/custom_datamodule.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datamodules/custom_datamodule.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datamodules/downloader.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datamodules/downloader.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datamodules/lizard_datamodule.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datamodules/lizard_datamodule.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datamodules/pannuke_datamodule.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datamodules/pannuke_datamodule.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/_base_dataset.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/_base_dataset.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/dataset_writers/_base_writer.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/dataset_writers/_base_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         img_path: Union[str, Path],
         mask_path: Union[str, Path],
         pre_proc: Callable = None,
     ) -> Dict[str, np.ndarray]:
         """Read one image and corresponding masks and do tiling on them."""
         # im, masks = self._get_arrays()
         im = FileHandler.read_img(img_path)
-        masks = FileHandler.read_mask(mask_path, return_all=True)
+        masks = FileHandler.read_mat(mask_path, return_all=True)
 
         if pre_proc is not None:
             masks = pre_proc(masks)
 
         inst = None
         types = None
         sem = None
```

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/dataset_writers/folder_writer.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/dataset_writers/folder_writer.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/dataset_writers/hdf5_writer.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/dataset_writers/hdf5_writer.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/folder_dataset_train.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/folder_dataset_train.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
         Raises
         ------
             KeyError: If a mask that does not exist in a given .mat file.
         """
         out = OrderedDict()
         out["image"] = FileHandler.read_img(self.fnames_imgs[ix])
-        masks = FileHandler.read_mask(self.fnames_masks[ix], return_all=True)
+        masks = FileHandler.read_mat(self.fnames_masks[ix], return_all=True)
 
         try:
             out["inst"] = masks["inst_map"]
         except KeyError:
             raise KeyError(
                 f"The file {self.fnames_masks[ix]} does not contain key `inst_map`."
             )
```

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/hdf5_dataset.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/hdf5_dataset.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/tests/data/imgs/patch1.png` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/tests/data/imgs/patch1.png`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/tests/data/imgs/patch2.png` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/tests/data/imgs/patch2.png`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/tests/data/imgs/patch3.png` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/tests/data/imgs/patch3.png`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/tests/data/masks/patch1.mat` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/tests/data/masks/patch1.mat`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/tests/data/masks/patch2.mat` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/tests/data/masks/patch2.mat`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/tests/data/masks/patch3.mat` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/tests/data/masks/patch3.mat`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/tests/data/tiny_test.h5` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/tests/data/tiny_test.h5`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/datasets/tests/test_dataset.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/datasets/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/decoder.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/decoder.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/decoder_stage.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/decoder_stage.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/long_skips/longskip_module.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/long_skips/longskip_module.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/long_skips/merging/cat.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/long_skips/merging/cat.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/long_skips/merging/merge_block.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/long_skips/merging/merge_block.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/long_skips/merging/sum.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/long_skips/merging/sum.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/long_skips/unet.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/long_skips/unet.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/long_skips/unet3p.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/long_skips/unet3p.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/long_skips/unetpp.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/long_skips/unetpp.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/decoders/tests/test_decoders.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/decoders/tests/test_decoders.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/_base_inferer.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/_base_inferer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,22 @@
+import warnings
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from itertools import chain
 from pathlib import Path
 from typing import Callable, Dict, List, Tuple, Union
 
 import numpy as np
 import torch
 import torch.nn as nn
 import yaml
-from pathos.multiprocessing import ThreadPool as Pool
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
-from ..utils import tensor_to_ndarray
-from ..utils.save_utils import mask2mat
+from ..utils import FileHandler, tensor_to_ndarray
 from .folder_dataset import FolderDataset
 from .post_processor import PostProcessor
 from .predictor import Predictor
 
 
 class BaseInferer(ABC):
     def __init__(
@@ -29,22 +28,22 @@
         patch_size: Tuple[int, int],
         instance_postproc: str,
         padding: int = None,
         batch_size: int = 8,
         normalization: str = None,
         device: str = "cuda",
         n_devices: int = 1,
-        save_masks: bool = True,
         save_intermediate: bool = False,
         save_dir: Union[Path, str] = None,
+        save_format: str = ".mat",
         checkpoint_path: Union[Path, str] = None,
         n_images: int = None,
         type_post_proc: Callable = None,
         sem_post_proc: Callable = None,
-        **postproc_kwargs,
+        **kwargs,
     ) -> None:
         """Inference for an image folder.
 
         Parameters
         ----------
             model : nn.Module
                 A segmentation model.
@@ -73,66 +72,75 @@
                 Apply img normalization at forward pass (Same as during training).
                 One of: "dataset", "minmax", "norm", "percentile", None.
             device : str, default="cuda"
                 The device of the input and model. One of: "cuda", "cpu"
             n_devices : int, default=1
                 Number of devices (cpus/gpus) used for inference.
                 The model will be copied into these devices.
-            save_masks : bool, default=False
-                If True, the resulting segmentation masks will be saved into `out_masks`
-                variable.
-            save_intermediate : bool, default=False
-                If True, intermediate soft masks will be saved into `soft_masks` var.
             save_dir : bool, optional
                 Path to save directory. If None, no masks will be saved to disk as .mat
-                files. If not None, overrides `save_masks`, thus for every batch the
-                segmentation results are saved into disk and the intermediate results
-                are flushed.
+                or .json files. Instead the masks will be saved in `self.out_masks`.
+            save_intermediate : bool, default=False
+                If True, intermediate soft masks will be saved into `soft_masks` var.
+            save_format : str, default=".mat"
+                The file format for the saved output masks. One of (".mat", ".json").
+                The ".json" option will save masks into geojson format.
             checkpoint_path : Path | str, optional
                 Path to the model weight checkpoints.
             n_images : int, optional
                 First n-number of images used from the `input_folder`.
             type_post_proc : Callable, optional
                 A post-processing function for the type maps. If not None, overrides
                 the default.
             sem_post_proc : Callable, optional
                 A post-processing function for the semantc seg maps. If not None,
                 overrides the default.
-            **postproc_kwargs:
-                Arbitrary keyword arguments for the post-processing.
+            **kwargs:
+                Arbitrary keyword arguments expecially for post-processing and saving.
         """
         # basic inits
         self.model = model
         self.out_heads = self._get_out_info()  # the names and num channels of out heads
         self.batch_size = batch_size
         self.patch_size = patch_size
         self.padding = padding
         self.out_activations = out_activations
         self.out_boundary_weights = out_boundary_weights
         self.head_kwargs = self._check_and_set_head_args()
+        self.kwargs = kwargs
 
         self.save_dir = Path(save_dir) if save_dir is not None else None
-        self.save_masks = save_masks
         self.save_intermediate = save_intermediate
+        self.save_format = save_format
 
         # dataloader
         self.path = Path(input_folder)
+
         folder_ds = FolderDataset(self.path, n_images=n_images)
+        if self.save_dir is None and len(folder_ds.fnames) > 40:
+            warnings.warn(
+                "`save_dir` is None. Thus, the outputs are be saved in `out_masks` "
+                "class variable. If the input folder contains many images, running "
+                "inference will likely flood the memory depending on the size and "
+                "number of the images. Consider saving outputs to disk by providing "
+                "`save_dir` argument."
+            )
+
         self.dataloader = DataLoader(
             folder_ds, batch_size=batch_size, shuffle=False, pin_memory=True
         )
 
         # Set post processor
         self.postprocessor = PostProcessor(
             instance_postproc,
             inst_key=self.model.inst_key,
             aux_key=self.model.aux_key,
             type_post_proc=type_post_proc,
             sem_post_proc=sem_post_proc,
-            **postproc_kwargs,
+            **kwargs,
         )
 
         # load weights and set devices
         if checkpoint_path is not None:
             ckpt = torch.load(
                 checkpoint_path, map_location=lambda storage, loc: storage
             )
@@ -184,18 +192,24 @@
     @abstractmethod
     def _infer_batch(self):
         raise NotImplementedError
 
     def infer(self) -> None:
         """Run inference and post-processing for the images.
 
-        NOTE: Saves outputs in `self.out_masks` or to disk (.mat) files.
-
-        `self.out_masks` is a nested dict: E.g.
-            {"image1": {"inst": [H, W], "type": [H, W], "sem": [H, W]}}
+        NOTE:
+        - Saves outputs in `self.out_masks` or to disk (.mat/.json) files.
+        - If `save_intermediate` is set to True, also intermiediate model outputs are
+            saved to `self.soft_masks`
+        - `self.out_masks` and `self.soft_masks` are nested dicts: E.g.
+                {"sample1": {"inst": [H, W], "type": [H, W], "sem": [H, W]}}
+        - If masks are saved to geojson .json files, more key word arguments
+            need to be given at class initialization. Namely: `geo_format`,
+            `classes_type`, `classes_sem`, `offsets`. See more in the
+            `FileHandler.save_masks` docs.
         """
         self.soft_masks = {}
         self.out_masks = {}
         self.elapsed = []
         self.rate = []
         with tqdm(self.dataloader, unit="batch") as loader:
             with torch.no_grad():
@@ -219,97 +233,33 @@
                     self.rate.append(loader.format_dict["rate"])
 
                     if self.save_intermediate:
                         for n, m in zip(names, soft_masks):
                             self.soft_masks[n] = m
 
                     if self.save_dir is None:
-                        if self.save_masks:
-                            for n, m in zip(names, seg_results):
-                                self.out_masks[n] = m
+                        for n, m in zip(names, seg_results):
+                            self.out_masks[n] = m
                     else:
                         loader.set_postfix_str("Saving results to disk")
                         if self.batch_size > 1:
-                            self.save_parallel(seg_results, names, self.save_dir)
+                            fnames = [Path(self.save_dir) / n for n in names]
+                            FileHandler.save_masks_parallel(
+                                maps=seg_results,
+                                fnames=fnames,
+                                **{**self.kwargs, "format": self.save_format},
+                            )
                         else:
                             for n, m in zip(names, seg_results):
-                                self.save_mask(m, n, self.save_dir)
-
-    @staticmethod
-    def save_mask(
-        maps: Dict[str, np.ndarray],
-        fname: str,
-        save_dir: Union[str, Path],
-        format: str = ".mat",
-    ) -> None:
-        """Save model outputs to .mat or geojson.
-
-        Parameters
-        ----------
-            maps : Dict[str, np.ndarray]
-                model output names mapped to model outputs.
-                E.g. {"sem": np.ndarray, "type": np.ndarray, "inst": np.ndarray}
-            fname : str
-                Name for the output-file.
-            save_dir : Path or str
-                Path to the save directory.
-            format : str
-                One of ".mat" or "geojson"
-        """
-        allowed = (".mat", ".json")
-        if format not in allowed:
-            raise ValueError(
-                f"Illegal file-format. Got: {format}. Allowed formats: {allowed}"
-            )
-
-        if format == ".mat":
-            mask2mat(fname, save_dir, **maps)
-        else:
-            pass
-
-        return True
-
-    @staticmethod
-    def save_parallel(
-        maps: List[Dict[str, np.ndarray]],
-        fnames: List[str],
-        save_dir: Union[Path, str],
-        format: str = ".mat",
-        progress_bar: bool = False,
-    ) -> None:
-        """Save the model output masks to a folder. (multi-threaded).
-
-        Parameters
-        ----------
-            maps : List[Dict[str, np.ndarray]]
-                The model output map dictionaries in a list.
-            fnames : List[str]
-                Name for the output-files. (In the same order with `maps`)
-            save_dir : Path or str
-                Path to the save directory.
-            format : str
-                One of ".mat" or "geojson"
-            progress_bar : bool, default=False
-                If True, a tqdm progress bar is shown.
-        """
-        args = tuple(zip(maps, fnames, [save_dir] * len(maps), [format] * len(maps)))
-
-        with Pool() as pool:
-            if progress_bar:
-                it = tqdm(pool.imap(BaseInferer._save_mask, args), total=len(maps))
-            else:
-                it = pool.imap(BaseInferer._save_mask, args)
-
-            for _ in it:
-                pass
-
-    @staticmethod
-    def _save_mask(args: Tuple[Dict[str, np.ndarray], str, str]) -> None:
-        """Unpacks the args for `save_mask` to enable multi-threading."""
-        return BaseInferer.save_mask(*args)
+                                fname = Path(self.save_dir) / n
+                                FileHandler.save_masks(
+                                    fname=fname,
+                                    maps=m,
+                                    **{**self.kwargs, "format": self.save_format},
+                                )
 
     def _strip_state_dict(self, ckpt: Dict) -> OrderedDict:
         """Strip te first 'model.' (generated by lightning) from the state dict keys."""
         state_dict = OrderedDict()
         for k, w in ckpt["state_dict"].items():
             if "num_batches_track" not in k:
                 new_key = k.strip("model")[1:]
```

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/folder_dataset.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/folder_dataset.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/post_processor.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/post_processor.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/predictor.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/predictor.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/resize_inferer.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/resize_inferer.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,22 +18,22 @@
         resize: Tuple[int, int],
         instance_postproc: str,
         padding: int = None,
         batch_size: int = 8,
         normalization: str = None,
         device: str = "cuda",
         n_devices: int = 1,
-        save_masks: bool = True,
         save_intermediate: bool = False,
         save_dir: Union[Path, str] = None,
+        save_format: str = ".mat",
         checkpoint_path: Union[Path, str] = None,
         n_images: int = None,
         type_post_proc: Callable = None,
         sem_post_proc: Callable = None,
-        **postproc_kwargs,
+        **kwargs,
     ) -> None:
         """Resize inference for a folder of images.
 
         Resizes the image before inputting to the model.
 
         NOTE: This class assumes that all the images in the input folder
         have the same shape. If the images have different shapes,
@@ -69,57 +69,54 @@
                 Apply img normalization (Same as during training). One of "dataset",
                 "minmax", "norm", "percentile", None.
             device : str, default="cuda"
                 The device of the input and model. One of: "cuda", "cpu"
             n_devices : int, default=1
                 Number of devices (cpus/gpus) used for inference.
                 The model will be copied into these devices.
-            save_masks : bool, default=False
-                If True, the resulting segmentation masks will be saved into `out_masks`
-                variable.
             save_intermediate : bool, default=False
                 If True, intermediate soft masks will be saved into `soft_masks` var.
-            save_dir : bool, optional
-                Path to save directory. If None, no masks will be saved to disk as .mat
-                files. If not None, overrides `save_masks`, thus for every batch the
-                segmentation results are saved into disk and the intermediate results
-                are flushed.
+            save_intermediate : bool, default=False
+                If True, intermediate soft masks will be saved into `soft_masks` var.
+            save_format : str, default=".mat"
+                The file format for the saved output masks. One of (".mat", ".json").
+                The ".json" option will save masks into geojson format.
             checkpoint_path : Path | str, optional
                 Path to the model weight checkpoints.
             n_images : int, optional
                 First n-number of images used from the `input_folder`.
             type_post_proc : Callable, optional
                 A post-processing function for the type maps. If not None, overrides
                 the default.
             sem_post_proc : Callable, optional
                 A post-processing function for the semantc seg maps. If not None,
                 overrides the default.
-            **postproc_kwargs:
-                Arbitrary keyword arguments for the post-processing.
+            **kwargs:
+                Arbitrary keyword arguments expecially for post-processing and saving.
         """
         super().__init__(
             model=model,
             input_folder=input_folder,
             out_activations=out_activations,
             out_boundary_weights=out_boundary_weights,
             patch_size=resize,
             padding=padding,
             batch_size=batch_size,
             normalization=normalization,
             instance_postproc=instance_postproc,
             device=device,
             n_devices=n_devices,
-            save_masks=save_masks,
             save_intermediate=save_intermediate,
             save_dir=save_dir,
+            save_format=save_format,
             checkpoint_path=checkpoint_path,
             n_images=n_images,
             type_post_proc=type_post_proc,
             sem_post_proc=sem_post_proc,
-            **postproc_kwargs,
+            **kwargs,
         )
 
     def _infer_batch(self, input_batch: torch.Tensor) -> Dict[str, torch.Tensor]:
         """Infer one batch of images."""
         inp_shape = tuple(input_batch.shape[2:])
 
         if self.padding:
```

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/sliding_window_inferer.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/sliding_window_inferer.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,22 +21,22 @@
         patch_size: Tuple[int, int],
         instance_postproc: str,
         padding: int = None,
         batch_size: int = 8,
         normalization: str = None,
         device: str = "cuda",
         n_devices: int = 1,
-        save_masks: bool = True,
         save_intermediate: bool = False,
         save_dir: Union[Path, str] = None,
+        save_format: str = ".mat",
         checkpoint_path: Union[Path, str] = None,
         n_images: int = None,
         type_post_proc: Callable = None,
         sem_post_proc: Callable = None,
-        **postproc_kwargs,
+        **kwargs,
     ) -> None:
         """Sliding window inference for a folder of images.
 
         NOTE: This class assumes that all the images in the input folder
         have the same shape. If the images have different shapes,
         `batch_size` needs to be set to 1 for this to work.
 
@@ -71,57 +71,55 @@
                 Apply img normalization (Same as during training). One of "dataset",
                 "minmax", "norm", "percentile", None.
             device : str, default="cuda"
                 The device of the input and model. One of: "cuda", "cpu"
             n_devices : int, default=1
                 Number of devices (cpus/gpus) used for inference.
                 The model will be copied into these devices.
-            save_masks : bool, default=False
-                If True, the resulting segmentation masks will be saved into `out_masks`
-                variable.
             save_intermediate : bool, default=False
                 If True, intermediate soft masks will be saved into `soft_masks` var.
             save_dir : bool, optional
                 Path to save directory. If None, no masks will be saved to disk as .mat
-                files. If not None, overrides `save_masks`, thus for every batch the
-                segmentation results are saved into disk and the intermediate results
-                are flushed.
+                or .json files. Instead the masks will be saved in `self.out_masks`.
+            save_format : str, default=".mat"
+                The file format for the saved output masks. One of (".mat", ".json").
+                The ".json" option will save masks into geojson format.
             checkpoint_path : Path | str, optional
                 Path to the model weight checkpoints.
             n_images : int, optional
                 First n-number of images used from the `ìnput_folder`.
             type_post_proc : Callable, optional
                 A post-processing function for the type maps. If not None, overrides
                 the default.
             sem_post_proc : Callable, optional
                 A post-processing function for the semantc seg maps. If not None,
                 overrides the default.
-            **postproc_kwargs:
-                Arbitrary keyword arguments for the post-processing.
+            **kwargs:
+                Arbitrary keyword arguments expecially for post-processing and saving.
         """
         super().__init__(
             model=model,
             input_folder=input_folder,
             out_activations=out_activations,
             out_boundary_weights=out_boundary_weights,
             patch_size=patch_size,
             padding=padding,
             batch_size=batch_size,
             normalization=normalization,
             instance_postproc=instance_postproc,
             device=device,
-            save_masks=save_masks,
             save_intermediate=save_intermediate,
             save_dir=save_dir,
+            save_format=save_format,
             checkpoint_path=checkpoint_path,
             n_images=n_images,
             n_devices=n_devices,
             type_post_proc=type_post_proc,
             sem_post_proc=sem_post_proc,
-            **postproc_kwargs,
+            **kwargs,
         )
 
         self.stride = stride
 
     def _get_margins(
         self, first_endpoint: int, img_size: int, stride: int, pad: int = None
     ) -> Tuple[int, int]:
```

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/tests/data/test1.png` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/tests/data/test1.png`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/tests/data/test2.png` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/tests/data/test2.png`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/inference/tests/test_inference.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/inference/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/__init__.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/__init__.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/__init__.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/ce.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/ce.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/dice.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/dice.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/focal.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/focal.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/grad_mse.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/grad_mse.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/iou.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/iou.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/mse.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/mse.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/sce.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/sce.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/ssim.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/ssim.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/criterions/tversky.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/criterions/tversky.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/joint_loss.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/joint_loss.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/loss_module.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/loss_module.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/multitask_loss.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/multitask_loss.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/tests/test_jointloss.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/tests/test_jointloss.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/tests/test_losses.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/tests/test_losses.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/tests/test_multitask_loss.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/tests/test_multitask_loss.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/losses/weighted_base_loss.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/losses/weighted_base_loss.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/metrics/__init__.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/metrics/binary_metrics.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/metrics/binary_metrics.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/metrics/functional.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/metrics/functional.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/metrics/tests/test_binary_metrics.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/metrics/tests/test_binary_metrics.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/metrics/tests/test_instance_metrics.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/metrics/tests/test_instance_metrics.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/metrics/tests/test_semantic_metrics.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/metrics/tests/test_semantic_metrics.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/__init__.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/base/_base_model.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/base/_base_model.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/base/_initialization.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/base/_initialization.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/base/_multitask_unet.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/base/_multitask_unet.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/base/_seg_head.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/base/_seg_head.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/base/_timm_encoder.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/base/_timm_encoder.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/cellpose/_conf.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/cellpose/_conf.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/cellpose/cellpose.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/cellpose/cellpose.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/hovernet/_conf.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/hovernet/_conf.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/hovernet/hovernet.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/hovernet/hovernet.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/stardist/_conf.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/stardist/_conf.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/stardist/stardist.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/stardist/stardist.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/models/tests/test_models.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/models/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/act/__init__.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/act/__init__.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/act/mish.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/act/mish.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/act/swish.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/act/swish.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/attention_modules.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/attention_modules.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/base_modules.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/base_modules.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/conv/scaled_ws_conv.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/conv/scaled_ws_conv.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/conv/ws_conv.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/conv/ws_conv.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/conv_base.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/conv_base.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/conv_block.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/conv_block.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/conv_layer.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/conv_layer.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/misc_modules.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/misc_modules.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/norm/bcn.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/norm/bcn.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/norm/gn.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/norm/gn.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/norm/ln.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/norm/ln.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/tests/test_attention.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/tests/test_basemodules.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/tests/test_basemodules.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/tests/test_conv_blocks.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/tests/test_conv_blocks.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/tests/test_convlayer.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/tests/test_convlayer.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/tests/test_miscmodules.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/tests/test_miscmodules.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/modules/upsample/fixed_unpool.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/modules/upsample/fixed_unpool.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/optimizers/__init__.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/optimizers/tests/test_optim_setup.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/optimizers/tests/test_optim_setup.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/optimizers/utils.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/optimizers/utils.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/__init__.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/__init__.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/cellpose/_old_cellpose.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/cellpose/_old_cellpose.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/cellpose/cellpose.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/cellpose/cellpose.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/cellpose/integrator.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/cellpose/integrator.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/cellpose/utils.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/cellpose/utils.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/dcan.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/dcan.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/dran.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/dran.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/drfns.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/drfns.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/hovernet.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/hovernet.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/omnipose.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/omnipose.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/functional/stardist.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/functional/stardist.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/postproc/tests/test_postproc.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/postproc/tests/test_postproc.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,14 @@
 
     assert rebuild.dtype == "int32"
     assert rebuild.shape == inst_map.shape
 
 
 def test_postproc_stardist(mask_patch_dir):
     mask_path = sorted(mask_patch_dir.glob("*"))[0]
-    inst_map = FileHandler.read_mask(mask_path)
+    inst_map = FileHandler.read_mat(mask_path)
     stardist = gen_stardist_maps(inst_map, 32)
     dist = gen_dist_maps(inst_map)
     rebuild = post_proc_stardist(dist, stardist)
 
     assert rebuild.dtype == "int32"
     assert rebuild.shape == inst_map.shape
```

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/callbacks/metric_callbacks.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/callbacks/metric_callbacks.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/callbacks/wandb_callbacks.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/callbacks/wandb_callbacks.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/functional/train_metrics.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/functional/train_metrics.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/lit/lightning_experiment.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/lit/lightning_experiment.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/tests/data/sem_target_batch8.pt` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/tests/data/sem_target_batch8.pt`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/tests/data/type_target_batch8.pt` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/tests/data/type_target_batch8.pt`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/tests/test_metrics.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/training/tests/test_training.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/training/tests/test_training.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/albu_transforms/__init__.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/albu_transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/albu_transforms/_composition.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/albu_transforms/_composition.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/albu_transforms/img_transforms.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/albu_transforms/img_transforms.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/albu_transforms/inst_transforms.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/albu_transforms/inst_transforms.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/albu_transforms/norm_transforms.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/albu_transforms/norm_transforms.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/functional/__init__.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/functional/cellpose.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/functional/cellpose.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/functional/contour.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/functional/contour.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/functional/dist.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/functional/dist.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/functional/edge_weights.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/functional/edge_weights.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/functional/hovernet.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/functional/hovernet.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/functional/omnipose.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/functional/omnipose.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/functional/stardist.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/functional/stardist.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/tests/test_full_pipeline.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/tests/test_full_pipeline.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/tests/test_img_transforms.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/tests/test_img_transforms.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/tests/test_inst_transforms.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/tests/test_inst_transforms.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/transforms/tests/test_norm_transforms.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/transforms/tests/test_norm_transforms.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/__init__.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/img_utils.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/img_utils.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/latency_benchmark.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/latency_benchmark.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/mask_utils.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/mask_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,17 @@
     -------
         np.ndarray:
             The instance labelled mask without duplicated indices.
             Shape (H, W).
     """
     current_max_id = np.amax(inst_map)
     inst_list = list(np.unique(inst_map))
-    inst_list.remove(0)  # 0 is background
+    if 0 in inst_list:
+        inst_list.remove(0)
+
     for inst_id in inst_list:
         inst = np.array(inst_map == inst_id, np.uint8)
         remapped_ids = ndi.label(inst)[0]
         remapped_ids[remapped_ids > 1] += current_max_id
         inst_map[remapped_ids > 1] = remapped_ids[remapped_ids > 1]
         current_max_id = np.amax(inst_map)
```

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/patching.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/patching.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/seg_benchmark.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/seg_benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,16 +230,16 @@
     def _read_files(self) -> List[Tuple[np.ndarray, np.ndarray, str]]:
         """Read in the files from the input folders."""
         preds = sorted(self.pred_dir.glob("*"))
         trues = sorted(self.true_dir.glob("*"))
 
         masks = []
         for truef, predf in zip(trues, preds):
-            true = FileHandler.read_mask(truef, return_all=True)
-            pred = FileHandler.read_mask(predf, return_all=True)
+            true = FileHandler.read_mat(truef, return_all=True)
+            pred = FileHandler.read_mat(predf, return_all=True)
             name = truef.name
             masks.append((true, pred, name))
 
         return masks
 
     def run_inst_benchmark(
         self, how: str = "binary", metrics: Tuple[str, ...] = ("pq",)
```

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tensor_img_utlls.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tensor_img_utlls.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tensor_kernels.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tensor_kernels.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tensor_utils.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/data/HE.png` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/data/HE.png`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_img_utils.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_img_utils.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_kernels.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_latency_benchmarker.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_latency_benchmarker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from cellseg_models_pytorch.inference import ResizeInferer
-from cellseg_models_pytorch.models import cellpose_plus
-from cellseg_models_pytorch.utils.latency_benchmark import LatencyBenchmarker
+# from cellseg_models_pytorch.inference import ResizeInferer
+# from cellseg_models_pytorch.models import cellpose_plus
+# from cellseg_models_pytorch.utils.latency_benchmark import LatencyBenchmarker
 
 
-def test_latency_benchmark(img_dir):
-    model = cellpose_plus(sem_classes=3, type_classes=3, long_skip="unet")
+# def test_latency_benchmark(img_dir):
+#     model = cellpose_plus(sem_classes=3, type_classes=3, long_skip="unet")
 
-    inferer = ResizeInferer(
-        model,
-        img_dir,
-        out_activations={"sem": "softmax", "type": "softmax", "cellpose": "tanh"},
-        out_boundary_weights={"sem": False, "type": False, "cellpose": True},
-        resize=(256, 256),
-        padding=80,
-        instance_postproc="hovernet",
-        batch_size=1,
-        save_intermediate=True,
-        device="cpu",
-        parallel=False,
-    )
-    inferer.infer()
+#     inferer = ResizeInferer(
+#         model,
+#         img_dir,
+#         out_activations={"sem": "softmax", "type": "softmax", "cellpose": "tanh"},
+#         out_boundary_weights={"sem": False, "type": False, "cellpose": True},
+#         resize=(256, 256),
+#         padding=80,
+#         instance_postproc="hovernet",
+#         batch_size=1,
+#         save_intermediate=True,
+#         device="cpu",
+#         parallel=False,
+#     )
+#     inferer.infer()
 
-    bm = LatencyBenchmarker(inferer)
+#     bm = LatencyBenchmarker(inferer)
 
-    bm.postproc_latency("inst", reps_per_img=1)
-    bm.postproc_latency("type", reps_per_img=1)
-    bm.postproc_latency("sem", reps_per_img=1)
-    bm.inference_latency(reps=1, warmup_reps=0)
-    bm.inference_postproc_latency(reps=1)
-    # bm.model_latency(input_size=(64, 64), reps=1, warmup_reps=0, device="cpu")
-    # bm.model_throughput(input_size=(64, 64), reps=1, warmup_reps=0, device="cpu")
+#     bm.postproc_latency("inst", reps_per_img=1)
+#     bm.postproc_latency("type", reps_per_img=1)
+#     bm.postproc_latency("sem", reps_per_img=1)
+#     bm.inference_latency(reps=1, warmup_reps=0)
+#     bm.inference_postproc_latency(reps=1)
+#     # bm.model_latency(input_size=(64, 64), reps=1, warmup_reps=0, device="cpu")
+#     # bm.model_throughput(input_size=(64, 64), reps=1, warmup_reps=0, device="cpu")
```

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_mask_utils.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_mask_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
     ],
 )
 def test_conoturs(img_patch_dir, mask_patch_dir, func, fill_contours, classes, colors):
     im_path = sorted(img_patch_dir.glob("*"))[0]
     mask_path = sorted(mask_patch_dir.glob("*"))[0]
 
     img = FileHandler.read_img(im_path)
-    masks = FileHandler.read_mask(mask_path, return_all=True)
+    masks = FileHandler.read_mat(mask_path, return_all=True)
     cont = func(
         masks["inst_map"],
         img,
         masks["type_map"],
         fill_contours=fill_contours,
         classes=classes,
         colors=colors,
```

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_patching.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_patching.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_seg_benchmark.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_seg_benchmark.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_tensor_img_utils.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_tensor_img_utils.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_tensor_utils.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_tensor_utils.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/tests/test_thresholding.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/tests/test_thresholding.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/cellseg_models_pytorch/utils/thresholding.py` & `cellseg_models_pytorch-0.1.9/cellseg_models_pytorch/utils/thresholding.py`

 * *Files identical despite different names*

### Comparing `cellseg_models_pytorch-0.1.8/pyproject.toml` & `cellseg_models_pytorch-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 [tool.poetry]
 name = "cellseg_models_pytorch"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python library for 2D cell/nuclei instance segmentation models written with PyTorch."
 authors = ["Okunator <oskari.lehtonen@helsinki.fi>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/okunator/cellseg_models.pytorch"
 repository = "https://github.com/okunator/cellseg_models.pytorch"
 keywords = ["cell segmentation", "nuclei segmentation", "pytorch", "pytorch-lightning"]
 
 
 [tool.poetry.dependencies]
 python = "^3.7.1,<3.11"
-torch = "^1.8"
-torchvision = "^0.9"
+torch = "^1.8.1"
+torchvision = "^0.9.1"
 numpy = "^1.21"
 scipy = "^1.7"
 scikit-image = "^0.19"
 pathos = "^0.2.8"
 opencv-python = "^4.2.0.32"
 timm = ">=0.5.4,<0.7.0"
 numba = "^0.55.2"
 tqdm = "^4.64.0"
 scikit-learn = "^1.0.2"
 pytorch-lightning = {version = "^1.6.0", optional = true}
 torch-optimizer = {version = "^0.3.0", optional = true}
 tables = {version = "^3.6.0", optional = true}
 albumentations = {version = "^1.0.0", optional = true}
 requests = {version = "^2.28.0", optional = true}
-
+geojson = {version = "^2.5.0", optional = true}
+torchmetrics = {version = "^0.10.0", optional = true}
 
 [tool.poetry.extras]
-all = ["pytorch-lightning", "tables", "requests", "albumentations", "torch-optimizer"]
-
+all = [
+    "pytorch-lightning",
+    "tables",
+    "requests",
+    "albumentations",
+    "geojson",
+    "torch-optimizer",
+    "torchmetrics"
+]
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 pytest-xdist = "^2.5.0"
 flake8 = "^4.0.1"
 flake8-docstrings = "^1.6.0"
@@ -66,15 +74,15 @@
 multi_line_output = 3
 
 [tool.black]
 line-length = 88
 
 [tool.flake8]
 max-line-length = 88
-extend-ignore = "E203,D103,D104,"
+extend-ignore = "E203,D103,D104"
 max-complexity = 10
 exclude = ".git,__pycache__,docs/source/conftest.py,old,build,dist,test,tests"
 
 [tool.coverage.run]
 source = ["cellseg_models_pytorch"]
 
 [tool.coverage.report]
```

### Comparing `cellseg_models_pytorch-0.1.8/setup.py` & `cellseg_models_pytorch-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,28 +63,30 @@
  'numpy>=1.21,<2.0',
  'opencv-python>=4.2.0.32,<5.0.0.0',
  'pathos>=0.2.8,<0.3.0',
  'scikit-image>=0.19,<0.20',
  'scikit-learn>=1.0.2,<2.0.0',
  'scipy>=1.7,<2.0',
  'timm>=0.5.4,<0.7.0',
- 'torch>=1.8,<2.0',
- 'torchvision>=0.9,<0.10',
+ 'torch>=1.8.1,<2.0.0',
+ 'torchvision>=0.9.1,<0.10.0',
  'tqdm>=4.64.0,<5.0.0']
 
 extras_require = \
 {'all': ['pytorch-lightning>=1.6.0,<2.0.0',
          'torch-optimizer>=0.3.0,<0.4.0',
          'tables>=3.6.0,<4.0.0',
          'albumentations>=1.0.0,<2.0.0',
-         'requests>=2.28.0,<3.0.0']}
+         'requests>=2.28.0,<3.0.0',
+         'geojson>=2.5.0,<3.0.0',
+         'torchmetrics>=0.10.0,<0.11.0']}
 
 setup_kwargs = {
     'name': 'cellseg-models-pytorch',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Python library for 2D cell/nuclei instance segmentation models written with PyTorch.',
     'long_description': '<div align="center">\n\n![Logo](./images/logo.png)\n\n**Python library for 2D cell/nuclei instance segmentation models written with [PyTorch](https://pytorch.org/).**\n\n[![Generic badge](https://img.shields.io/badge/License-MIT-<COLOR>.svg?style=for-the-badge)](https://github.com/okunator/cellseg_models.pytorch/blob/master/LICENSE)\n[![PyTorch - Version](https://img.shields.io/badge/PYTORCH-1.8+-red?style=for-the-badge&logo=pytorch)](https://pytorch.org/)\n[![Python - Version](https://img.shields.io/badge/PYTHON-3.7+-red?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)\n<br>\n[![Github Test](https://img.shields.io/github/workflow/status/okunator/cellseg_models.pytorch/Tests?label=Tests&logo=github&style=for-the-badge)](https://github.com/okunator/cellseg_models.pytorch/actions/workflows/tests.yml)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)\n[![Codecov](https://img.shields.io/codecov/c/github/okunator/cellseg_models.pytorch?logo=codecov&style=for-the-badge&token=oGSj7FZ1lm)](https://codecov.io/gh/okunator/cellseg_models.pytorch)\n<br>\n[![Pypi](https://img.shields.io/pypi/v/cellseg-models-pytorch?color=blue&logo=pypi&style=for-the-badge)](https://pypi.org/project/cellseg-models-pytorch/)\n<br>\n[![DOI](https://zenodo.org/badge/450787123.svg)](https://zenodo.org/badge/latestdoi/450787123)\n\n</div>\n\n<div align="center">\n\n</div>\n\n## Introduction\n\nContains multi-task encoder-decoder architectures along with dedicated post-processing methods for segmenting cell/nuclei instances. As the name suggests, this library is heavily inspired by [segmentation_models.pytorch](https://github.com/qubvel/segmentation_models.pytorch) library for semantic segmentation.\n\n<br><br>\n\n![Architecture](./images/architecture_overview.png)\n\n## Installation\n\n**Basic installation**\n\n```shell\npip install cellseg-models-pytorch\n```\n\n**To install extra dependencies (training utilities and datamodules for open-source datasets) use**\n\n```shell\npip install cellseg-models-pytorch[all]\n```\n\n## Features\n\n- High level API to define cell/nuclei instance segmentation models.\n- 4 cell/nuclei instance segmentation models and more to come.\n- Pre-trained backbones/encoders from the [timm](https://github.com/rwightman/pytorch-image-models) library.\n- All the architectures can be augmented to output semantic segmentation outputs along with instance semgentation outputs (panoptic segmentation).\n- A lot of flexibility to modify the components of the model architectures.\n- Optimized inference methods.\n- Popular training losses and benchmarking metrics.\n- Simple model training with [pytorch-lightning](https://www.pytorchlightning.ai/).\n- Popular optimizers for training (provided by [pytorch-optimizer](https://github.com/jettify/pytorch-optimizer)).\n\n## Models\n\n| Model                      | Paper                                                                          |\n| -------------------------- | ------------------------------------------------------------------------------ |\n| [[1](#Citation)] HoVer-Net | https://www.sciencedirect.com/science/article/pii/S1361841519301045?via%3Dihub |\n| [[2](#Citation)] Cellpose  | https://www.nature.com/articles/s41592-020-01018-x                             |\n| [[3](#Citation)] Omnipose  | https://www.biorxiv.org/content/10.1101/2021.11.03.467199v2                    |\n| [[4](#Citation)] Stardist  | https://arxiv.org/abs/1806.03535                                               |\n\n## Datasets\n\n| Dataset                       | Paper                                                                                            |\n| ----------------------------- | ------------------------------------------------------------------------------------------------ |\n| [[5, 6](#References)] Pannuke | https://arxiv.org/abs/2003.10778 , https://link.springer.com/chapter/10.1007/978-3-030-23937-4_2 |\n| [[7](#References)] Lizard     | http://arxiv.org/abs/2108.11195                                                                  |\n\n## Notebook examples\n\n- [Training Stardist with Pannuke](https://github.com/okunator/cellseg_models.pytorch/blob/main/examples/pannuke_nuclei_segmentation_stardist.ipynb). Train the Stardist model with constant sized Pannuke patches.\n- [Training Cellpose with Lizard](https://github.com/okunator/cellseg_models.pytorch/blob/main/examples/lizard_nuclei_segmentation_cellpose.ipynb). Train the Cellpose model with Lizard dataset that is composed of varying sized images.\n\n## Code Examples\n\n**Define Cellpose for cell segmentation.**\n\n```python\nimport cellseg_models_pytorch as csmp\nimport torch\n\nmodel = csmp.models.cellpose_base(type_classes=5) # num of cell types in training data=5.\nx = torch.rand([1, 3, 256, 256])\n\n# NOTE: these outputs still need post-processing to obtain instance segmentation masks.\ny = model(x) # {"cellpose": [1, 2, 256, 256], "type": [1, 5, 256, 256]}\n```\n\n**Define Cellpose for cell and tissue area segmentation (Panoptic segmentation).**\n\n```python\nimport cellseg_models_pytorch as csmp\nimport torch\n\nmodel = csmp.models.cellpose_plus(type_classes=5, sem_classes=3) # num cell types and tissue types\nx = torch.rand([1, 3, 256, 256])\n\n# NOTE: these outputs still need post-processing to obtain instance and semantic segmentation masks.\ny = model(x) # {"cellpose": [1, 2, 256, 256], "type": [1, 5, 256, 256], "sem": [1, 3, 256, 256]}\n```\n\n**Define panoptic Cellpose model with more flexibility.**\n\n```python\nimport cellseg_models_pytorch as csmp\n\nmodel = csmp.CellPoseUnet(\n    decoders=("cellpose", "sem"), # cellpose and semantic decoders\n    heads={"cellpose": {"cellpose": 2, "type": 5}, "sem": {"sem": 3}}, # three output heads\n    depth=5, # encoder depth\n    out_channels=(256, 128, 64, 32, 16), # number of out channels at each decoder stage\n    layer_depths=(4, 4, 4, 4, 4), # number of conv blocks at each decoder layer\n    style_channels=256, # Number of style vector channels\n    enc_name="resnet50", # timm encoder\n    enc_pretrain=True, # imagenet pretrained encoder\n    long_skip="unetpp", # use unet++ long skips. ("unet", "unetpp", "unet3p")\n    merge_policy="sum", # ("cat", "sum")\n    short_skip="residual", # residual short skips. ("basic", "residual", "dense")\n    normalization="bcn", # batch-channel-normalization. ("bcn", "bn", "gn", "ln", "in")\n    activation="gelu", # gelu activation instead of relu. Several options for this.\n    convolution="wsconv", # weight standardized conv. ("wsconv", "conv", "scaled_wsconv")\n    attention="se", # squeeze-and-excitation attention. ("se", "gc", "scse", "eca")\n    pre_activate=False, # normalize and activation after convolution.\n)\n\nx = torch.rand([1, 3, 256, 256])\n# NOTE: these outputs still need post-processing to obtain instance and semantic segmentation masks.\ny = model(x) # {"cellpose": [1, 2, 256, 256], "type": [1, 5, 256, 256], "sem": [1, 3, 256, 256]}\n```\n\n**Run HoVer-Net inference and post-processing with a sliding window approach.**\n\n```python\nimport cellseg_models_pytorch as csmp\n\nmodel = csmp.models.hovernet_base(type_classes=5)\n# returns {"hovernet": [B, 2, H, W], "type": [B, 5, H, W], "inst": [B, 2, H, W]}\n\n# Sliding window inference for big images using overlapping patches\ninferer = csmp.inference.SlidingWindowInferer(\n    model=model,\n    input_folder="/path/to/images/",\n    checkpoint_path="/path/to/model/weights/",\n    out_activations={"hovernet": "tanh", "type": "softmax", "inst": "softmax"},\n    out_boundary_weights={"hovernet": True, "type": False, "inst": False}, # smooths boundary effects\n    instance_postproc="hovernet", # THE POST-PROCESSING METHOD\n    patch_size=(256, 256),\n    stride=128,\n    padding=80,\n    batch_size=8,\n    normalization="percentile", # same normalization as in training\n)\n\ninferer.infer() # Run sliding window inference.\n\ninferer.out_masks\n# {"image1" :{"inst": [H, W], "type": [H, W]}, ..., "imageN" :{"inst": [H, W], "type": [H, W]}}\n```\n\n## Models API\n\n### Class API\n\nThe class API enables the most flexibility in defining different model architectures. It allows for defining a multitude of hard-parameter sharing multi-task encoder-decoder architectures with (relatively) low effort. The class API is borrowing a lot from [segmentation_models.pytorch](https://github.com/qubvel/segmentation_models.pytorch) models API.\n\n**Model classes**:\n\n- `csmp.CellPoseUnet`\n- `csmp.StarDistUnet`\n- `csmp.HoverNet`\n\n**All of the models contain**:\n\n- `model.encoder` - pretrained [timm](https://github.com/rwightman/pytorch-image-models) backbone for feature extraction.\n- `model.{decoder_name}_decoder` - Models can have multiple decoders with unique names.\n- `model.{head_name}_seg_head` - Model decoders can have multiple segmentation heads with unique names.\n- `model.forward(x)` - forward pass.\n\n**Defining your own multi-task architecture**\n\nFor example, to define a multi-task architecture that has `resnet50` encoder, four decoders, and 5 output heads with `CellPoseUnet` architectural components, we could do this:\n\n```python\nimport cellseg_models_pytorch as csmp\nimport torch\n\nmodel = csmp.CellPoseUnet(\n    decoders=("cellpose", "dist", "contour", "sem"),\n    heads={\n        "cellpose": {"type": 5, "cellpose": 2},\n        "dist": {"dist": 1},\n        "contour": {"contour": 1},\n        "sem": {"sem": 4}\n    },\n)\n\nx = torch.rand([1, 3, 256, 256])\nmodel(x)\n# {\n#   "cellpose": [1, 2, 256, 256],\n#   "type": [1, 5, 256, 256],\n#   "dist": [1, 1, 256, 256],\n#   "contour": [1, 1, 256, 256],\n#   "sem": [1, 4, 256, 256]\n# }\n```\n\n### Function API\n\nWith the function API, you can build models with low effort by calling the below listed functions. Under the hood, the function API simply calls the above classes with pre-defined decoder and head names. The training and post-processing tools of this library are built around these names, thus, it is recommended to use the function API, although, it is a bit more rigid than the class API. Basically, the function API only lacks the ability to define the output-tasks of the model, but allows for all the rest as the class API.\n\n| Model functions                        | Output names                              | Task                             |\n| -------------------------------------- | ----------------------------------------- | -------------------------------- |\n| `csmp.models.cellpose_base`            | `"type"`, `"cellpose"`,                   | **instance segmentation**        |\n| `csmp.models.cellpose_plus`            | `"type"`, `"cellpose"`, `"sem"`,          | **panoptic segmentation**        |\n| `csmp.models.omnipose_base`            | `"type"`, `"omnipose"`                    | **instance segmentation**        |\n| `csmp.models.omnipose_plus`            | `"type"`, `"omnipose"`, `"sem"`,          | **panoptic segmentation**        |\n| `csmp.models.hovernet_base`            | `"type"`, `"inst"`, `"hovernet"`          | **instance segmentation**        |\n| `csmp.models.hovernet_plus`            | `"type"`, `"inst"`, `"hovernet"`, `"sem"` | **panoptic segmentation**        |\n| `csmp.models.hovernet_small`           | `"type"`,`"hovernet"`                     | **instance segmentation**        |\n| `csmp.models.hovernet_small_plus`      | `"type"`, `"hovernet"`, `"sem"`           | **panoptic segmentation**        |\n| `csmp.models.stardist_base`            | `"stardist"`, `"dist"`                    | **binary instance segmentation** |\n| `csmp.models.stardist_base_multiclass` | `"stardist"`, `"dist"`, `"type"`          | **instance segmentation**        |\n| `csmp.models.stardist_plus`            | `"stardist"`, `"dist"`, `"type"`, `"sem"` | **panoptic segmentation**        |\n\n## References\n\n- [1] S. Graham, Q. D. Vu, S. E. A. Raza, A. Azam, Y-W. Tsang, J. T. Kwak and N. Rajpoot. "HoVer-Net: Simultaneous Segmentation and Classification of Nuclei in Multi-Tissue Histology Images." Medical Image Analysis, Sept. 2019.\n- [2] Stringer, C.; Wang, T.; Michaelos, M. & Pachitariu, M. Cellpose: a generalist algorithm for cellular segmentation Nature Methods, 2021, 18, 100-106\n- [3] Cutler, K. J., Stringer, C., Wiggins, P. A., & Mougous, J. D. (2022). Omnipose: a high-precision morphology-independent solution for bacterial cell segmentation. bioRxiv. doi:10.1101/2021.11.03.467199\n- [4] Uwe Schmidt, Martin Weigert, Coleman Broaddus, & Gene Myers (2018). Cell Detection with Star-Convex Polygons. In Medical Image Computing and Computer Assisted Intervention - MICCAI 2018 - 21st International Conference, Granada, Spain, September 16-20, 2018, Proceedings, Part II (pp. 265–273).\n- [5] Gamper, J., Koohbanani, N., Benet, K., Khuram, A., & Rajpoot, N. (2019) PanNuke: an open pan-cancer histology dataset for nuclei instance segmentation and classification. In European Congress on Digital Pathology (pp. 11-19).\n- [6] Gamper, J., Koohbanani, N., Graham, S., Jahanifar, M., Khurram, S., Azam, A.,Hewitt, K., & Rajpoot, N. (2020). PanNuke Dataset Extension, Insights and Baselines. arXiv preprint arXiv:2003.10778.\n- [7] Graham, S., Jahanifar, M., Azam, A., Nimir, M., Tsang, Y.W., Dodd, K., Hero, E., Sahota, H., Tank, A., Benes, K., & others (2021). Lizard: A Large-Scale Dataset for Colonic Nuclear Instance Segmentation and Classification. In Proceedings of the IEEE/CVF International Conference on Computer Vision (pp. 684-693).\n\n## Citation\n\n```bibtex\n@misc{csmp2022,\n    title={{cellseg_models.pytorch}: Cell/Nuclei Segmentation Models and Benchmark.},\n    author={Oskari Lehtonen},\n    howpublished = {\\url{https://github.com/okunator/cellseg_models.pytorch}},\n    doi = {10.5281/zenodo.7064617}\n    year={2022}\n}\n```\n\n## Licence\n\nThis project is distributed under [MIT License](https://github.com/okunator/cellseg_models.pytorch/blob/main/LICENSE)\n\nThe project contains code from the original cell segmentation and 3rd-party libraries that have permissive licenses:\n\n- [timm](https://github.com/rwightman/pytorch-image-models) (Apache-2)\n- [HoVer-Net](https://github.com/vqdang/hover_net) (MIT)\n- [Cellpose](https://github.com/MouseLand/cellpose) (BSD-3)\n- [Stardist](https://github.com/stardist/stardist) (BSD-3)\n\nIf you find this library useful in your project, it is your responsibility to ensure you comply with the conditions of any dependent licenses. Please create an issue if you think something is missing regarding the licenses.\n',
     'author': 'Okunator',
     'author_email': 'oskari.lehtonen@helsinki.fi',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/okunator/cellseg_models.pytorch',
```

### Comparing `cellseg_models_pytorch-0.1.8/PKG-INFO` & `cellseg_models_pytorch-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: cellseg-models-pytorch
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python library for 2D cell/nuclei instance segmentation models written with PyTorch.
 Home-page: https://github.com/okunator/cellseg_models.pytorch
 License: MIT
 Keywords: cell segmentation,nuclei segmentation,pytorch,pytorch-lightning
 Author: Okunator
 Author-email: oskari.lehtonen@helsinki.fi
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: all
 Requires-Dist: albumentations (>=1.0.0,<2.0.0); extra == "all"
+Requires-Dist: geojson (>=2.5.0,<3.0.0); extra == "all"
 Requires-Dist: numba (>=0.55.2,<0.56.0)
 Requires-Dist: numpy (>=1.21,<2.0)
 Requires-Dist: opencv-python (>=4.2.0.32,<5.0.0.0)
 Requires-Dist: pathos (>=0.2.8,<0.3.0)
 Requires-Dist: pytorch-lightning (>=1.6.0,<2.0.0); extra == "all"
 Requires-Dist: requests (>=2.28.0,<3.0.0); extra == "all"
 Requires-Dist: scikit-image (>=0.19,<0.20)
 Requires-Dist: scikit-learn (>=1.0.2,<2.0.0)
 Requires-Dist: scipy (>=1.7,<2.0)
 Requires-Dist: tables (>=3.6.0,<4.0.0); extra == "all"
 Requires-Dist: timm (>=0.5.4,<0.7.0)
-Requires-Dist: torch (>=1.8,<2.0)
+Requires-Dist: torch (>=1.8.1,<2.0.0)
 Requires-Dist: torch-optimizer (>=0.3.0,<0.4.0); extra == "all"
-Requires-Dist: torchvision (>=0.9,<0.10)
+Requires-Dist: torchmetrics (>=0.10.0,<0.11.0); extra == "all"
+Requires-Dist: torchvision (>=0.9.1,<0.10.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Project-URL: Repository, https://github.com/okunator/cellseg_models.pytorch
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 ![Logo](./images/logo.png)
```

