# Comparing `tmp/controlnet_v11_utils-0.0.7.tar.gz` & `tmp/controlnet_v11_utils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ivan.rodkin/lab/ControlNet-v1-1-nightly/dist/.tmp-m9hekxhc/controlnet_v11_utils-0.0.7.tar", last modified: Mon Jun 12 19:17:04 2023, max compression
+gzip compressed data, was "/home/ivan.rodkin/lab/ControlNet-v1-1-nightly/dist/.tmp-uiq2tcjw/controlnet_v11_utils-0.0.8.tar", last modified: Mon Jun 12 19:21:40 2023, max compression
```

## Comparing `controlnet_v11_utils-0.0.7.tar` & `controlnet_v11_utils-0.0.8.tar`

### file list

```diff
@@ -1,508 +1,555 @@
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.879886 controlnet_v11_utils-0.0.7/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       64 2023-06-12 19:17:04.879886 controlnet_v11_utils-0.0.7/PKG-INFO
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    31985 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/README.md
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.349882 controlnet_v11_utils-0.0.7/annotator/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:15:50.000000 controlnet_v11_utils-0.0.7/annotator/__init__.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.349882 controlnet_v11_utils-0.0.7/annotator/canny/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      155 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/canny/__init__.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.349882 controlnet_v11_utils-0.0.7/annotator/hed/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4028 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/hed/__init__.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.349882 controlnet_v11_utils-0.0.7/annotator/lineart/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4060 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/lineart/__init__.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.349882 controlnet_v11_utils-0.0.7/annotator/lineart_anime/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6882 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/lineart_anime/__init__.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.359882 controlnet_v11_utils-0.0.7/annotator/midas/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      899 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/midas/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5213 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/midas/api.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.369882 controlnet_v11_utils-0.0.7/annotator/midas/midas/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/midas/midas/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      367 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/midas/midas/base_model.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9242 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/midas/midas/blocks.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3154 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/midas/midas/dpt_depth.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2709 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/midas/midas/midas_net.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5207 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/midas/midas/midas_net_custom.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7869 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/midas/midas/transforms.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    14625 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/midas/midas/vit.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4582 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/midas/utils.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.369882 controlnet_v11_utils-0.0.7/annotator/mlsd/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1529 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/mlsd/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    24049 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/mlsd/utils.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.369882 controlnet_v11_utils-0.0.7/annotator/normalbae/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2119 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/normalbae/__init__.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.369882 controlnet_v11_utils-0.0.7/annotator/oneformer/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1664 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1525 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/api.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.369882 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      258 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/__init__.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.379883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/checkpoint/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      347 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/checkpoint/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    17841 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/checkpoint/c2_model_loading.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5705 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/checkpoint/catalog.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6352 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/checkpoint/detection_checkpoint.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.389883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/config/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      619 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/config/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7890 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/config/compat.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9251 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/config/config.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    29723 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/config/defaults.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3035 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/config/instantiate.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    16698 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/config/lazy.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.389883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      644 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7398 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/benchmark.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    21351 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/build.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7244 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/catalog.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11179 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/common.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8189 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/dataset_mapper.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.409883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      523 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10194 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/builtin.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    21841 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/builtin_meta.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    13287 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/cityscapes.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7881 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/cityscapes_panoptic.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    23565 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/coco.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9077 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/coco_panoptic.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9743 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/lvis.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)   223757 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/lvis_v0_5_categories.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)   219177 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/lvis_v1_categories.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    39414 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/lvis_v1_category_image_count.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3188 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/pascal_voc.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      169 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/register_coco.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    23252 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/detection_utils.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.419883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/samplers/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      412 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/samplers/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11809 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/samplers/distributed_sampler.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1944 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/samplers/grouped_batch_sampler.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.419883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/transforms/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      486 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/transforms/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    14116 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/transforms/augmentation.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    27335 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/transforms/augmentation_impl.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    12629 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/transforms/transform.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.429883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/engine/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      340 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/engine/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    27122 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/engine/defaults.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    25625 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/engine/hooks.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3946 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/engine/launch.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    16024 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/engine/train_loop.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.439883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      671 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8429 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/cityscapes_evaluation.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    30551 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/coco_evaluation.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8196 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/evaluator.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5098 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/fast_eval_api.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15106 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/lvis_evaluation.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7580 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/panoptic_evaluation.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10916 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/pascal_voc_evaluation.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7648 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/rotated_coco_evaluation.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11471 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/sem_seg_evaluation.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2614 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/testing.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.449883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      673 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9250 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/api.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    22359 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/c10.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7594 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/caffe2_export.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6674 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/caffe2_inference.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    17114 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/caffe2_modeling.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5113 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/caffe2_patch.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11847 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/flatten.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    38328 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/shared.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5028 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/torchscript.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11666 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/torchscript_patch.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.469883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      874 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5764 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/aspp.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    12151 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/batch_norm.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3024 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/blocks.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    17018 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/deform_conv.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4202 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/losses.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10879 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/mask_ops.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6611 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/nms.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3098 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/roi_align.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3752 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/roi_align_rotated.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      652 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/rotated_boxes.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      537 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/shape_spec.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5552 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/wrappers.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.469883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/model_zoo/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      449 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/model_zoo/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11343 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/model_zoo/model_zoo.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.479883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1608 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15519 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/anchor_generator.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.489883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      598 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2532 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/backbone.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1055 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/build.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10380 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/fpn.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    16081 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/mvit.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    16676 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/regnet.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    23678 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/resnet.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    25222 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/swin.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6360 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/utils.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    19471 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/vit.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15163 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/box_regression.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6284 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/matcher.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.499883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/meta_arch/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      508 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/meta_arch/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      854 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/meta_arch/build.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11988 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/meta_arch/dense_detector.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    13273 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/meta_arch/fcos.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10447 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/meta_arch/panoptic_fpn.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    14036 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/meta_arch/rcnn.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    18346 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/meta_arch/retinanet.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9986 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/meta_arch/semantic_seg.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10929 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/mmdet_wrapper.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11569 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/poolers.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4065 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/postprocessing.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.509883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/proposal_generator/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      231 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/proposal_generator/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      856 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/proposal_generator/build.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8168 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/proposal_generator/proposal_utils.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    23934 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/proposal_generator/rpn.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8887 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/proposal_generator/rrpn.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.519883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/roi_heads/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      768 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/roi_heads/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4137 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/roi_heads/box_head.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    13070 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/roi_heads/cascade_rcnn.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    25510 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/roi_heads/fast_rcnn.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11256 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/roi_heads/keypoint_head.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    12289 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/roi_heads/mask_head.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    37801 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/roi_heads/roi_heads.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11255 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2354 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/sampling.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    12496 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/test_time_augmentation.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.519883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/projects/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1177 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/projects/__init__.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.529883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/projects/deeplab/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      244 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/projects/deeplab/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      953 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/projects/deeplab/build_solver.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1157 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/projects/deeplab/config.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1776 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/projects/deeplab/loss.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2405 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/projects/deeplab/lr_scheduler.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5857 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/projects/deeplab/resnet.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    14886 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/projects/deeplab/semantic_seg.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.529883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/solver/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      336 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/solver/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    12200 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/solver/build.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8906 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/solver/lr_scheduler.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.539883 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/structures/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      665 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/structures/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    14429 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/structures/boxes.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5540 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/structures/image_list.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6613 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/structures/instances.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9008 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/structures/keypoints.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    19853 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/structures/masks.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    19044 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/structures/rotated_boxes.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.549884 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/tracking/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      580 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/tracking/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2256 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/tracking/base_tracker.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11918 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/tracking/bbox_iou_tracker.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7526 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/tracking/hungarian_tracker.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4182 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1126 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/tracking/utils.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5388 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.569884 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       51 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6037 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/analysis.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8585 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/collect_env.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4096 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/colormap.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7237 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/comm.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1852 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/develop.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5644 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/env.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    18977 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/events.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1237 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/file_io.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7827 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/logger.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2583 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/memory.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1874 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/registry.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1072 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/serialize.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    18683 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/testing.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2543 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/tracing.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11356 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/video_visualizer.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    51237 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/visualizer.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.569884 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      202 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8345 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/config.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.579884 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       74 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4395 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/build.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.579884 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/dataset_mappers/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        1 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/dataset_mappers/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    13854 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/dataset_mappers/coco_unified_new_baseline_dataset_mapper.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8947 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/dataset_mappers/dataset_mapper.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15595 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/dataset_mappers/oneformer_unified_dataset_mapper.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.589884 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/datasets/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      190 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/datasets/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5079 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/datasets/register_ade20k_instance.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    20089 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/datasets/register_ade20k_panoptic.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8356 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/datasets/register_cityscapes_panoptic.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1730 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/datasets/register_coco_panoptic2instance.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15764 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/datasets/register_coco_panoptic_annos_semseg.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7352 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/tokenizer.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.599884 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/evaluation/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      132 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/evaluation/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8719 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/evaluation/cityscapes_evaluation.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    24346 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/evaluation/coco_evaluator.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    30721 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/evaluation/detection_coco_evaluator.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8474 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/evaluation/evaluator.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5034 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/evaluation/instance_evaluation.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.599884 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      246 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/__init__.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.609884 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/backbone/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       51 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/backbone/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11107 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/backbone/dinat.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    27510 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/backbone/swin.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8270 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/matcher.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.609884 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/meta_arch/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        1 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/meta_arch/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6060 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/meta_arch/oneformer_head.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.609884 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/pixel_decoder/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       51 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/pixel_decoder/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    12468 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/pixel_decoder/fpn.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15424 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/pixel_decoder/msdeformattn.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.619884 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/transformer_decoder/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      139 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/transformer_decoder/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    20487 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/transformer_decoder/oneformer_transformer_decoder.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2709 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/transformer_decoder/position_encoding.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9225 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/transformer_decoder/text_transformer.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    12282 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/transformer_decoder/transformer.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    21159 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/oneformer_model.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.629884 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/utils/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       95 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/utils/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3885 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/utils/box_ops.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4029 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/utils/events.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7486 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/utils/misc.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4836 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/utils/pos_embed.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.629884 controlnet_v11_utils-0.0.7/annotator/openpose/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4280 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/openpose/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10856 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/openpose/body.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    13510 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/openpose/face.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3307 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/openpose/hand.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8745 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/openpose/model.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10551 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/openpose/util.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.639884 controlnet_v11_utils-0.0.7/annotator/pidinet/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1489 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/pidinet/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    20928 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/pidinet/model.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.639884 controlnet_v11_utils-0.0.7/annotator/shuffle/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2230 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/shuffle/__init__.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.639884 controlnet_v11_utils-0.0.7/annotator/uniformer/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1134 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/__init__.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.639884 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      352 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/__init__.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.639884 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/arraymisc/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      133 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/arraymisc/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1824 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/arraymisc/quantization.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.649884 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2438 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1990 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/alexnet.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.669884 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1732 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2508 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/activation.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4681 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/context_block.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1446 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/conv.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2514 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8760 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/conv_module.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5417 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/conv_ws.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4142 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2172 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/drop.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15999 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/generalized_attention.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1097 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/hsigmoid.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      651 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/hswish.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11012 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/non_local.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5154 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/norm.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1127 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/padding.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2487 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/plugin.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      658 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/registry.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      577 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/scale.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      485 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/swish.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    24639 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/transformer.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2880 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/upsample.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6961 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/wrappers.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1089 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/builder.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9955 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/resnet.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.679884 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/utils/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1023 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/utils/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    22104 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/utils/flops_counter.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1881 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2327 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/utils/sync_bn.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    26006 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/utils/weight_init.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6053 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/vgg.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.679884 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/engine/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      266 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/engine/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7196 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/engine/test.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.689885 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      478 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    41933 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/file_client.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.699885 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/handlers/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      278 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/handlers/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      993 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/handlers/base.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1068 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/handlers/json_handler.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      817 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/handlers/pickle_handler.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      665 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/handlers/yaml_handler.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5520 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/io.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3458 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/parse.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.709885 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/image/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1725 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/image/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9907 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/image/colorspace.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    25196 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/image/geometric.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9572 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/image/io.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1410 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/image/misc.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    14999 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/image/photometric.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.759885 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4506 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4344 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/assign_score_withk.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1695 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/ball_query.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2508 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/bbox.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3725 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/border_align.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1609 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/box_iou_rotated.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9873 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/carafe.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3041 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/cc_attention.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1795 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/contour_expand.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4697 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/corner_pool.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6697 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/correlation.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15603 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/deform_conv.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7410 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/deform_roi_pool.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1467 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/deprecated_wrappers.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6582 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/focal_loss.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2550 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/furthest_point_sample.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10031 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/fused_bias_leakyrelu.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1607 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/gather_points.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8135 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/group_points.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      887 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/info.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2988 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/iou3d.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2599 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/knn.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3761 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/masked_conv.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5403 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/merge_cells.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10574 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/modulated_deform_conv.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15175 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/multi_scale_deform_attn.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    16237 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/nms.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3113 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/pixel_group.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    12291 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/point_sample.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5241 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/points_in_boxes.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6063 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/points_sampler.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2773 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/psa_mask.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8519 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/roi_align.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6434 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/roi_align_rotated.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2517 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/roi_pool.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4256 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/roiaware_pool3d.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2990 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/roipoint_pool3d.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5804 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/saconv.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5201 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/scatter_points.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11267 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/sync_bn.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2147 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/three_interpolate.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1515 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/three_nn.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2141 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/tin_shift.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11804 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/upfirdn2d.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5286 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/voxelize.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.769885 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      505 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2830 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/_functions.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3665 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/collate.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2365 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/data_container.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3912 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/data_parallel.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4857 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/distributed.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2837 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/distributed_deprecated.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      332 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/registry.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2307 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/scatter_gather.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      708 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/utils.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.779885 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2859 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7502 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/base_module.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    20846 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/base_runner.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      666 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/builder.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    25136 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/checkpoint.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1928 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/default_constructor.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5395 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/dist_utils.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7565 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/epoch_based_runner.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15784 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/fp16_utils.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.799885 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1396 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7317 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/checkpoint.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      269 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/closure.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3599 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/ema.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    22448 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/evaluation.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2761 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/hook.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      446 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/iter_timer.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.809885 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      522 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5451 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/base.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1761 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/dvclive.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2838 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/mlflow.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3077 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/neptune.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4378 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/pavi.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2077 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/tensorboard.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10684 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/text.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1694 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/wandb.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    26034 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/lr_updater.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      657 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/memory.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    21296 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/momentum_updater.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    21654 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/optimizer.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8041 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/profiler.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      847 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/sampler_seed.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      707 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/sync_buffer.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11062 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/iter_based_runner.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1192 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/log_buffer.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.809885 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/optimizer/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      370 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/optimizer/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1346 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/optimizer/builder.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11803 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/optimizer/default_constructor.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1598 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/priority.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2936 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/utils.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.839885 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3915 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    26263 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/config.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3367 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/env.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2021 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/ext_loader.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3986 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/logging.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11447 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/misc.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      899 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/parrots_jit.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3536 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/parrots_wrapper.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3414 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/path.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7105 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/progressbar.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11041 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/registry.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4289 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/testing.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2993 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/timer.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      795 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/trace.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2673 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/version_utils.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1177 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/version.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.839885 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/video/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      570 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/video/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10209 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/video/io.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9728 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/video/optflow.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5291 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/video/processing.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.849885 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/visualization/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      338 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/visualization/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1381 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/visualization/color.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5145 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/visualization/image.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3389 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/visualization/optflow.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.849885 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv_custom/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       95 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv_custom/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    19091 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv_custom/checkpoint.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2543 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/util.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.849885 controlnet_v11_utils-0.0.7/annotator/zoe/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1671 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/annotator/zoe/__init__.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.859886 controlnet_v11_utils-0.0.7/cldm/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:16:01.000000 controlnet_v11_utils-0.0.7/cldm/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    19200 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/cldm/cldm.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    16397 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/cldm/ddim_hacked.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3567 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/cldm/hack.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3182 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/cldm/logger.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      836 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/cldm/model.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.859886 controlnet_v11_utils-0.0.7/config/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       20 2023-06-12 19:10:48.000000 controlnet_v11_utils-0.0.7/config/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       20 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.7/config/config.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.869886 controlnet_v11_utils-0.0.7/controlnet_v11_utils.egg-info/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       64 2023-06-12 19:17:04.000000 controlnet_v11_utils-0.0.7/controlnet_v11_utils.egg-info/PKG-INFO
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    21260 2023-06-12 19:17:04.000000 controlnet_v11_utils-0.0.7/controlnet_v11_utils.egg-info/SOURCES.txt
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        1 2023-06-12 19:17:04.000000 controlnet_v11_utils-0.0.7/controlnet_v11_utils.egg-info/dependency_links.txt
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       39 2023-06-12 19:17:04.000000 controlnet_v11_utils-0.0.7/controlnet_v11_utils.egg-info/top_level.txt
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.869886 controlnet_v11_utils-0.0.7/ldm/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:16:26.000000 controlnet_v11_utils-0.0.7/ldm/__init__.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.869886 controlnet_v11_utils-0.0.7/ldm/data/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.7/ldm/data/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      629 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.7/ldm/data/util.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7227 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.7/ldm/util.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.869886 controlnet_v11_utils-0.0.7/models/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:16:42.000000 controlnet_v11_utils-0.0.7/models/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       38 2023-06-12 19:17:04.879886 controlnet_v11_utils-0.0.7/setup.cfg
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      149 2023-06-12 19:16:51.000000 controlnet_v11_utils-0.0.7/setup.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:17:04.869886 controlnet_v11_utils-0.0.7/share/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       18 2023-06-12 19:10:32.000000 controlnet_v11_utils-0.0.7/share/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      155 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.7/share/share.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.771556 controlnet_v11_utils-0.0.8/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       64 2023-06-12 19:21:40.771556 controlnet_v11_utils-0.0.8/PKG-INFO
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    31985 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/README.md
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.191552 controlnet_v11_utils-0.0.8/annotator/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:15:50.000000 controlnet_v11_utils-0.0.8/annotator/__init__.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.191552 controlnet_v11_utils-0.0.8/annotator/canny/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      155 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/canny/__init__.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.191552 controlnet_v11_utils-0.0.8/annotator/hed/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4028 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/hed/__init__.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.191552 controlnet_v11_utils-0.0.8/annotator/lineart/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4060 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/lineart/__init__.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.191552 controlnet_v11_utils-0.0.8/annotator/lineart_anime/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6882 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/lineart_anime/__init__.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.201552 controlnet_v11_utils-0.0.8/annotator/midas/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      899 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/midas/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5213 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/midas/api.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.211552 controlnet_v11_utils-0.0.8/annotator/midas/midas/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/midas/midas/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      367 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/midas/midas/base_model.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9242 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/midas/midas/blocks.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3154 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/midas/midas/dpt_depth.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2709 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/midas/midas/midas_net.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5207 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/midas/midas/midas_net_custom.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7869 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/midas/midas/transforms.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    14625 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/midas/midas/vit.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4582 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/midas/utils.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.211552 controlnet_v11_utils-0.0.8/annotator/mlsd/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1529 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/mlsd/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    24049 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/mlsd/utils.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.211552 controlnet_v11_utils-0.0.8/annotator/normalbae/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2119 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/normalbae/__init__.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.211552 controlnet_v11_utils-0.0.8/annotator/oneformer/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1664 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1525 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/api.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.221552 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      258 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/__init__.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.221552 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/checkpoint/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      347 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/checkpoint/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    17841 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/checkpoint/c2_model_loading.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5705 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/checkpoint/catalog.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6352 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/checkpoint/detection_checkpoint.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.231552 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/config/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      619 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/config/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7890 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/config/compat.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9251 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/config/config.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    29723 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/config/defaults.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3035 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/config/instantiate.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    16698 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/config/lazy.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.231552 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      644 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7398 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/benchmark.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    21351 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/build.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7244 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/catalog.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11179 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/common.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8189 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/dataset_mapper.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.251552 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      523 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10194 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/builtin.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    21841 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/builtin_meta.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    13287 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/cityscapes.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7881 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/cityscapes_panoptic.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    23565 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/coco.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9077 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/coco_panoptic.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9743 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/lvis.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)   223757 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/lvis_v0_5_categories.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)   219177 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/lvis_v1_categories.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    39414 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3188 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/pascal_voc.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      169 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/register_coco.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    23252 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/detection_utils.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.261552 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/samplers/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      412 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/samplers/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11809 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/samplers/distributed_sampler.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1944 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/samplers/grouped_batch_sampler.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.261552 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/transforms/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      486 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/transforms/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    14116 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/transforms/augmentation.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    27335 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/transforms/augmentation_impl.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    12629 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/transforms/transform.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.271552 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/engine/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      340 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/engine/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    27122 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/engine/defaults.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    25625 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/engine/hooks.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3946 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/engine/launch.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    16024 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/engine/train_loop.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.281553 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      671 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8429 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/cityscapes_evaluation.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    30551 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/coco_evaluation.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8196 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/evaluator.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5098 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/fast_eval_api.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15106 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/lvis_evaluation.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7580 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/panoptic_evaluation.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10916 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/pascal_voc_evaluation.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7648 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/rotated_coco_evaluation.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11471 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/sem_seg_evaluation.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2614 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/testing.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.291553 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      673 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9250 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/api.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    22359 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/c10.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7594 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/caffe2_export.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6674 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/caffe2_inference.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    17114 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/caffe2_modeling.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5113 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/caffe2_patch.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11847 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/flatten.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    38328 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/shared.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5028 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/torchscript.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11666 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/torchscript_patch.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.311553 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      874 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5764 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/aspp.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    12151 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/batch_norm.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3024 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/blocks.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    17018 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/deform_conv.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4202 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/losses.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10879 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/mask_ops.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6611 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/nms.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3098 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/roi_align.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3752 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/roi_align_rotated.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      652 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/rotated_boxes.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      537 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/shape_spec.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5552 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/wrappers.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.311553 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/model_zoo/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      449 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/model_zoo/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11343 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/model_zoo/model_zoo.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.321553 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1608 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15519 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/anchor_generator.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.341553 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      598 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2532 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/backbone.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1055 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/build.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10380 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/fpn.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    16081 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/mvit.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    16676 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/regnet.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    23678 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/resnet.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    25222 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/swin.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6360 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/utils.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    19471 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/vit.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15163 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/box_regression.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6284 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/matcher.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.341553 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/meta_arch/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      508 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/meta_arch/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      854 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/meta_arch/build.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11988 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/meta_arch/dense_detector.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    13273 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/meta_arch/fcos.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10447 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    14036 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/meta_arch/rcnn.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    18346 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/meta_arch/retinanet.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9986 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/meta_arch/semantic_seg.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10929 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/mmdet_wrapper.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11569 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/poolers.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4065 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/postprocessing.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.351553 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/proposal_generator/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      231 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/proposal_generator/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      856 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/proposal_generator/build.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8168 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/proposal_generator/proposal_utils.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    23934 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/proposal_generator/rpn.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8887 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/proposal_generator/rrpn.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.361553 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/roi_heads/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      768 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/roi_heads/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4137 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/roi_heads/box_head.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    13070 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    25510 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/roi_heads/fast_rcnn.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11256 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/roi_heads/keypoint_head.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    12289 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/roi_heads/mask_head.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    37801 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/roi_heads/roi_heads.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11255 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2354 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/sampling.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    12496 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/test_time_augmentation.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.361553 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/projects/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1177 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/projects/__init__.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.371553 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/projects/deeplab/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      244 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/projects/deeplab/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      953 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/projects/deeplab/build_solver.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1157 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/projects/deeplab/config.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1776 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/projects/deeplab/loss.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2405 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/projects/deeplab/lr_scheduler.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5857 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/projects/deeplab/resnet.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    14886 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/projects/deeplab/semantic_seg.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.371553 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/solver/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      336 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/solver/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    12200 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/solver/build.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8906 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/solver/lr_scheduler.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.381553 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/structures/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      665 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/structures/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    14429 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/structures/boxes.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5540 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/structures/image_list.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6613 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/structures/instances.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9008 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/structures/keypoints.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    19853 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/structures/masks.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    19044 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/structures/rotated_boxes.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.391553 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/tracking/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      580 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/tracking/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2256 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/tracking/base_tracker.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11918 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/tracking/bbox_iou_tracker.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7526 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/tracking/hungarian_tracker.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4182 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1126 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/tracking/utils.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5388 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.411553 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       51 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6037 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/analysis.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8585 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/collect_env.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4096 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/colormap.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7237 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/comm.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1852 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/develop.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5644 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/env.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    18977 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/events.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1237 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/file_io.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7827 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/logger.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2583 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/memory.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1874 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/registry.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1072 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/serialize.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    18683 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/testing.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2543 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/tracing.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11356 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/video_visualizer.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    51237 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/visualizer.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.421553 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      202 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8345 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/config.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.421553 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       74 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4395 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/build.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.421553 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/dataset_mappers/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        1 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/dataset_mappers/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    13854 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/dataset_mappers/coco_unified_new_baseline_dataset_mapper.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8947 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/dataset_mappers/dataset_mapper.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15595 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/dataset_mappers/oneformer_unified_dataset_mapper.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.431553 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/datasets/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      190 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/datasets/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5079 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/datasets/register_ade20k_instance.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    20089 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/datasets/register_ade20k_panoptic.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8356 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/datasets/register_cityscapes_panoptic.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1730 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/datasets/register_coco_panoptic2instance.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15764 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/datasets/register_coco_panoptic_annos_semseg.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7352 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/tokenizer.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.441553 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/evaluation/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      132 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/evaluation/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8719 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/evaluation/cityscapes_evaluation.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    24346 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/evaluation/coco_evaluator.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    30721 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/evaluation/detection_coco_evaluator.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8474 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/evaluation/evaluator.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5034 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/evaluation/instance_evaluation.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.441553 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      246 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/__init__.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.451554 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/backbone/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       51 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/backbone/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11107 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/backbone/dinat.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    27510 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/backbone/swin.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8270 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/matcher.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.451554 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/meta_arch/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        1 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/meta_arch/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6060 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/meta_arch/oneformer_head.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.451554 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/pixel_decoder/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       51 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/pixel_decoder/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    12468 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/pixel_decoder/fpn.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15424 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/pixel_decoder/msdeformattn.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.461554 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/transformer_decoder/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      139 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/transformer_decoder/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    20487 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/transformer_decoder/oneformer_transformer_decoder.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2709 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/transformer_decoder/position_encoding.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9225 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/transformer_decoder/text_transformer.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    12282 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/transformer_decoder/transformer.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    21159 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/oneformer_model.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.471554 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/utils/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       95 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/utils/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3885 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/utils/box_ops.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4029 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/utils/events.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7486 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/utils/misc.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4836 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/utils/pos_embed.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.471554 controlnet_v11_utils-0.0.8/annotator/openpose/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4280 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/openpose/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10856 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/openpose/body.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    13510 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/openpose/face.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3307 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/openpose/hand.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8745 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/openpose/model.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10551 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/openpose/util.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.481554 controlnet_v11_utils-0.0.8/annotator/pidinet/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1489 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/pidinet/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    20928 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/pidinet/model.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.481554 controlnet_v11_utils-0.0.8/annotator/shuffle/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2230 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/shuffle/__init__.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.481554 controlnet_v11_utils-0.0.8/annotator/uniformer/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1134 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/__init__.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.481554 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      352 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/__init__.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.491554 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/arraymisc/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      133 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/arraymisc/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1824 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/arraymisc/quantization.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.491554 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2438 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1990 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/alexnet.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.521554 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1732 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2508 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/activation.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4681 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/context_block.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1446 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/conv.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2514 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8760 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/conv_module.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5417 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/conv_ws.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4142 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2172 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/drop.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15999 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/generalized_attention.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1097 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/hsigmoid.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      651 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/hswish.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11012 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/non_local.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5154 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/norm.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1127 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/padding.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2487 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/plugin.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      658 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/registry.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      577 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/scale.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      485 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/swish.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    24639 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/transformer.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2880 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/upsample.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6961 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/wrappers.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1089 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/builder.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9955 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/resnet.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.521554 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/utils/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1023 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/utils/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    22104 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/utils/flops_counter.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1881 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2327 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/utils/sync_bn.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    26006 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/utils/weight_init.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6053 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/vgg.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.531554 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/engine/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      266 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/engine/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7196 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/engine/test.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.531554 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      478 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    41933 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/file_client.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.541554 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/handlers/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      278 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/handlers/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      993 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/handlers/base.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1068 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/handlers/json_handler.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      817 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      665 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5520 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/io.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3458 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/parse.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.541554 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/image/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1725 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/image/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9907 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/image/colorspace.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    25196 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/image/geometric.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9572 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/image/io.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1410 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/image/misc.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    14999 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/image/photometric.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.601554 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4506 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4344 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/assign_score_withk.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1695 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/ball_query.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2508 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/bbox.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3725 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/border_align.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1609 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/box_iou_rotated.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9873 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/carafe.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3041 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/cc_attention.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1795 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/contour_expand.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4697 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/corner_pool.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6697 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/correlation.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15603 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/deform_conv.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7410 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/deform_roi_pool.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1467 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/deprecated_wrappers.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6582 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/focal_loss.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2550 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/furthest_point_sample.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10031 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/fused_bias_leakyrelu.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1607 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/gather_points.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8135 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/group_points.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      887 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/info.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2988 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/iou3d.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2599 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/knn.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3761 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/masked_conv.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5403 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/merge_cells.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10574 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/modulated_deform_conv.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15175 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/multi_scale_deform_attn.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    16237 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/nms.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3113 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/pixel_group.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    12291 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/point_sample.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5241 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/points_in_boxes.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6063 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/points_sampler.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2773 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/psa_mask.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8519 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/roi_align.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6434 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/roi_align_rotated.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2517 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/roi_pool.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4256 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/roiaware_pool3d.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2990 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/roipoint_pool3d.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5804 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/saconv.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5201 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/scatter_points.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11267 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/sync_bn.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2147 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/three_interpolate.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1515 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/three_nn.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2141 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/tin_shift.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11804 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/upfirdn2d.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5286 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/voxelize.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.611554 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      505 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2830 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/_functions.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3665 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/collate.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2365 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/data_container.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3912 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/data_parallel.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4857 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/distributed.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2837 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/distributed_deprecated.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      332 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/registry.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2307 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/scatter_gather.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      708 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/utils.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.631555 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2859 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7502 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/base_module.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    20846 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/base_runner.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      666 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/builder.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    25136 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/checkpoint.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1928 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/default_constructor.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5395 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/dist_utils.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7565 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/epoch_based_runner.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    15784 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/fp16_utils.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.651555 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1396 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7317 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/checkpoint.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      269 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/closure.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3599 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/ema.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    22448 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/evaluation.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2761 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/hook.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      446 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/iter_timer.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.661555 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      522 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5451 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/base.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1761 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/dvclive.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2838 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/mlflow.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3077 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/neptune.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4378 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/pavi.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2077 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/tensorboard.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10684 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/text.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1694 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/wandb.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    26034 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/lr_updater.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      657 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/memory.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    21296 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/momentum_updater.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    21654 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/optimizer.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8041 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/profiler.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      847 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/sampler_seed.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      707 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/sync_buffer.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11062 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/iter_based_runner.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1192 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/log_buffer.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.661555 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/optimizer/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      370 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/optimizer/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1346 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/optimizer/builder.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11803 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/optimizer/default_constructor.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1598 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/priority.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2936 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/utils.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.681555 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3915 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    26263 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/config.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3367 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/env.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2021 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/ext_loader.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3986 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/logging.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11447 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/misc.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      899 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/parrots_jit.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3536 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/parrots_wrapper.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3414 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/path.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7105 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/progressbar.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11041 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/registry.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4289 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/testing.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2993 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/timer.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      795 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/trace.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2673 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/version_utils.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1177 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/version.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.691555 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/video/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      570 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/video/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    10209 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/video/io.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9728 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/video/optflow.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5291 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/video/processing.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.691555 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/visualization/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      338 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/visualization/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1381 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/visualization/color.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5145 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/visualization/image.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3389 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/visualization/optflow.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.691555 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv_custom/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       95 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv_custom/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    19091 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv_custom/checkpoint.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2543 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/util.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.691555 controlnet_v11_utils-0.0.8/annotator/zoe/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     1671 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/annotator/zoe/__init__.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.701555 controlnet_v11_utils-0.0.8/cldm/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:16:01.000000 controlnet_v11_utils-0.0.8/cldm/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    19200 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/cldm/cldm.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    16397 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/cldm/ddim_hacked.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3567 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/cldm/hack.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3182 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/cldm/logger.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      836 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/cldm/model.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.711555 controlnet_v11_utils-0.0.8/config/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       20 2023-06-12 19:10:48.000000 controlnet_v11_utils-0.0.8/config/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       20 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.8/config/config.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.711555 controlnet_v11_utils-0.0.8/controlnet_v11_utils.egg-info/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       64 2023-06-12 19:21:40.000000 controlnet_v11_utils-0.0.8/controlnet_v11_utils.egg-info/PKG-INFO
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    22566 2023-06-12 19:21:40.000000 controlnet_v11_utils-0.0.8/controlnet_v11_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        1 2023-06-12 19:21:40.000000 controlnet_v11_utils-0.0.8/controlnet_v11_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       39 2023-06-12 19:21:40.000000 controlnet_v11_utils-0.0.8/controlnet_v11_utils.egg-info/top_level.txt
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.711555 controlnet_v11_utils-0.0.8/ldm/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:16:26.000000 controlnet_v11_utils-0.0.8/ldm/__init__.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.721555 controlnet_v11_utils-0.0.8/ldm/data/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/data/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      629 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/data/util.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.721555 controlnet_v11_utils-0.0.8/ldm/models/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:20:28.000000 controlnet_v11_utils-0.0.8/ldm/models/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     8560 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/models/autoencoder.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.721555 controlnet_v11_utils-0.0.8/ldm/models/diffusion/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/models/diffusion/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    17304 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/models/diffusion/ddim.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    84659 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/models/diffusion/ddpm.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.731555 controlnet_v11_utils-0.0.8/ldm/models/diffusion/dpm_solver/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       37 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/models/diffusion/dpm_solver/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    65969 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/models/diffusion/dpm_solver/dpm_solver.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2990 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/models/diffusion/dpm_solver/sampler.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    12927 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/models/diffusion/plms.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      753 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/models/diffusion/sampling_util.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.731555 controlnet_v11_utils-0.0.8/ldm/modules/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:04.000000 controlnet_v11_utils-0.0.8/ldm/modules/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    11806 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/attention.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.741555 controlnet_v11_utils-0.0.8/ldm/modules/diffusionmodules/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/diffusionmodules/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    34384 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/diffusionmodules/model.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    30364 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/diffusionmodules/openaimodel.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3424 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/diffusionmodules/upscaling.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9868 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/diffusionmodules/util.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.741555 controlnet_v11_utils-0.0.8/ldm/modules/distributions/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/distributions/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2970 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/distributions/distributions.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3110 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/ema.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.741555 controlnet_v11_utils-0.0.8/ldm/modules/encoders/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/encoders/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7611 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/encoders/modules.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.751555 controlnet_v11_utils-0.0.8/ldm/modules/image_degradation/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      208 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/image_degradation/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    25198 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/image_degradation/bsrgan.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    22341 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/image_degradation/bsrgan_light.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    29024 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/image_degradation/utils_image.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.751555 controlnet_v11_utils-0.0.8/ldm/modules/midas/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/midas/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5338 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/midas/api.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.761556 controlnet_v11_utils-0.0.8/ldm/modules/midas/midas/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/midas/midas/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      367 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/midas/midas/base_model.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     9242 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/midas/midas/blocks.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     3154 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/midas/midas/dpt_depth.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     2709 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/midas/midas/midas_net.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5207 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/midas/midas/midas_net_custom.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7869 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/midas/midas/transforms.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    14625 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/midas/midas/vit.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4582 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/modules/midas/utils.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     7227 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/ldm/util.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.761556 controlnet_v11_utils-0.0.8/models/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:16:42.000000 controlnet_v11_utils-0.0.8/models/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       38 2023-06-12 19:21:40.771556 controlnet_v11_utils-0.0.8/setup.cfg
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      149 2023-06-12 19:21:24.000000 controlnet_v11_utils-0.0.8/setup.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:21:40.771556 controlnet_v11_utils-0.0.8/share/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       18 2023-06-12 19:10:32.000000 controlnet_v11_utils-0.0.8/share/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      155 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.8/share/share.py
```

### Comparing `controlnet_v11_utils-0.0.7/README.md` & `controlnet_v11_utils-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/hed/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/hed/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/lineart/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/lineart/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/lineart_anime/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/lineart_anime/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/midas/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/midas/api.py` & `controlnet_v11_utils-0.0.8/annotator/midas/api.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/midas/midas/blocks.py` & `controlnet_v11_utils-0.0.8/annotator/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/midas/midas/dpt_depth.py` & `controlnet_v11_utils-0.0.8/annotator/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/midas/midas/midas_net.py` & `controlnet_v11_utils-0.0.8/annotator/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/midas/midas/midas_net_custom.py` & `controlnet_v11_utils-0.0.8/annotator/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/midas/midas/transforms.py` & `controlnet_v11_utils-0.0.8/annotator/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/midas/midas/vit.py` & `controlnet_v11_utils-0.0.8/annotator/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/midas/utils.py` & `controlnet_v11_utils-0.0.8/annotator/midas/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/mlsd/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/mlsd/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/mlsd/utils.py` & `controlnet_v11_utils-0.0.8/annotator/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/normalbae/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/normalbae/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/api.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/api.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/checkpoint/c2_model_loading.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/checkpoint/c2_model_loading.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/checkpoint/catalog.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/checkpoint/catalog.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/checkpoint/detection_checkpoint.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/checkpoint/detection_checkpoint.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/config/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/config/compat.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/config/compat.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/config/config.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/config/config.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/config/defaults.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/config/defaults.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/config/instantiate.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/config/instantiate.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/config/lazy.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/config/lazy.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/benchmark.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/benchmark.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/build.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/build.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/catalog.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/catalog.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/common.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/common.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/dataset_mapper.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/builtin.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/builtin_meta.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/cityscapes.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/cityscapes_panoptic.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/coco.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/coco_panoptic.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/lvis.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/lvis_v0_5_categories.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/lvis_v1_categories.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/lvis_v1_category_image_count.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/datasets/pascal_voc.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/detection_utils.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/samplers/distributed_sampler.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/samplers/grouped_batch_sampler.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/transforms/augmentation.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/transforms/augmentation_impl.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/data/transforms/transform.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/engine/defaults.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/engine/defaults.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/engine/hooks.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/engine/hooks.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/engine/launch.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/engine/launch.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/engine/train_loop.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/engine/train_loop.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/cityscapes_evaluation.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/cityscapes_evaluation.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/coco_evaluation.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/coco_evaluation.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/evaluator.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/fast_eval_api.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/fast_eval_api.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/lvis_evaluation.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/lvis_evaluation.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/panoptic_evaluation.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/panoptic_evaluation.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/pascal_voc_evaluation.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/pascal_voc_evaluation.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/rotated_coco_evaluation.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/rotated_coco_evaluation.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/sem_seg_evaluation.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/sem_seg_evaluation.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/evaluation/testing.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/evaluation/testing.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/api.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/api.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/c10.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/c10.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/caffe2_export.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/caffe2_export.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/caffe2_inference.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/caffe2_inference.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/caffe2_modeling.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/caffe2_modeling.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/caffe2_patch.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/caffe2_patch.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/flatten.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/flatten.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/shared.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/shared.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/torchscript.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/torchscript.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/export/torchscript_patch.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/export/torchscript_patch.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/aspp.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/aspp.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/batch_norm.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/blocks.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/deform_conv.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/losses.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/losses.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/mask_ops.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/mask_ops.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/nms.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/nms.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/roi_align.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/roi_align.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/roi_align_rotated.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/rotated_boxes.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/shape_spec.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/layers/wrappers.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/model_zoo/model_zoo.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/model_zoo/model_zoo.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/anchor_generator.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/backbone.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/build.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/build.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/fpn.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/fpn.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/mvit.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/mvit.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/regnet.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/resnet.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/swin.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/swin.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/utils.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/backbone/vit.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/backbone/vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/box_regression.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/box_regression.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/matcher.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/meta_arch/build.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/meta_arch/dense_detector.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/meta_arch/dense_detector.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/meta_arch/fcos.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/meta_arch/fcos.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/meta_arch/panoptic_fpn.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/meta_arch/panoptic_fpn.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/meta_arch/rcnn.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/meta_arch/rcnn.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/meta_arch/retinanet.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/meta_arch/retinanet.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/meta_arch/semantic_seg.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/meta_arch/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/mmdet_wrapper.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/poolers.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/poolers.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/postprocessing.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/postprocessing.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/proposal_generator/build.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/proposal_generator/build.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/proposal_generator/proposal_utils.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/proposal_generator/proposal_utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/proposal_generator/rpn.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/proposal_generator/rpn.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/proposal_generator/rrpn.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/proposal_generator/rrpn.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/roi_heads/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/roi_heads/box_head.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/roi_heads/box_head.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/roi_heads/cascade_rcnn.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/roi_heads/cascade_rcnn.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/roi_heads/fast_rcnn.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/roi_heads/fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/roi_heads/keypoint_head.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/roi_heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/roi_heads/mask_head.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/roi_heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/roi_heads/roi_heads.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/roi_heads/roi_heads.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/roi_heads/rotated_fast_rcnn.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/roi_heads/rotated_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/sampling.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/sampling.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/modeling/test_time_augmentation.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/modeling/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/projects/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/projects/deeplab/build_solver.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/projects/deeplab/build_solver.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/projects/deeplab/config.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/projects/deeplab/config.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/projects/deeplab/loss.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/projects/deeplab/loss.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/projects/deeplab/lr_scheduler.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/projects/deeplab/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/projects/deeplab/resnet.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/projects/deeplab/resnet.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/projects/deeplab/semantic_seg.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/projects/deeplab/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/solver/build.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/solver/build.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/solver/lr_scheduler.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/solver/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/structures/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/structures/boxes.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/structures/image_list.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/structures/instances.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/structures/instances.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/structures/keypoints.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/structures/masks.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/structures/masks.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/structures/rotated_boxes.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/tracking/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/tracking/base_tracker.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/tracking/base_tracker.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/tracking/bbox_iou_tracker.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/tracking/bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/tracking/hungarian_tracker.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/tracking/hungarian_tracker.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/tracking/utils.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/analysis.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/collect_env.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/colormap.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/comm.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/comm.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/develop.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/develop.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/env.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/env.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/events.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/events.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/file_io.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/logger.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/memory.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/memory.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/registry.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/serialize.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/testing.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/tracing.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/tracing.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/video_visualizer.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/video_visualizer.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/detectron2/utils/visualizer.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/detectron2/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/config.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/config.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/build.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/build.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/dataset_mappers/coco_unified_new_baseline_dataset_mapper.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/dataset_mappers/coco_unified_new_baseline_dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/dataset_mappers/dataset_mapper.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/dataset_mappers/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/dataset_mappers/oneformer_unified_dataset_mapper.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/dataset_mappers/oneformer_unified_dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/datasets/register_ade20k_instance.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/datasets/register_ade20k_instance.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/datasets/register_ade20k_panoptic.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/datasets/register_ade20k_panoptic.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/datasets/register_cityscapes_panoptic.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/datasets/register_cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/datasets/register_coco_panoptic2instance.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/datasets/register_coco_panoptic2instance.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/datasets/register_coco_panoptic_annos_semseg.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/datasets/register_coco_panoptic_annos_semseg.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/data/tokenizer.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/data/tokenizer.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/evaluation/cityscapes_evaluation.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/evaluation/cityscapes_evaluation.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/evaluation/coco_evaluator.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/evaluation/coco_evaluator.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/evaluation/detection_coco_evaluator.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/evaluation/detection_coco_evaluator.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/evaluation/evaluator.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/evaluation/instance_evaluation.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/evaluation/instance_evaluation.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/backbone/dinat.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/backbone/dinat.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/backbone/swin.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/backbone/swin.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/matcher.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/meta_arch/oneformer_head.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/meta_arch/oneformer_head.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/pixel_decoder/fpn.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/pixel_decoder/fpn.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/pixel_decoder/msdeformattn.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/pixel_decoder/msdeformattn.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/transformer_decoder/oneformer_transformer_decoder.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/transformer_decoder/oneformer_transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/transformer_decoder/position_encoding.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/transformer_decoder/position_encoding.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/transformer_decoder/text_transformer.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/transformer_decoder/text_transformer.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/modeling/transformer_decoder/transformer.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/modeling/transformer_decoder/transformer.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/oneformer_model.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/oneformer_model.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/utils/box_ops.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/utils/box_ops.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/utils/events.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/utils/events.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/utils/misc.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/utils/misc.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/oneformer/oneformer/utils/pos_embed.py` & `controlnet_v11_utils-0.0.8/annotator/oneformer/oneformer/utils/pos_embed.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/openpose/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/openpose/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/openpose/body.py` & `controlnet_v11_utils-0.0.8/annotator/openpose/body.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/openpose/face.py` & `controlnet_v11_utils-0.0.8/annotator/openpose/face.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/openpose/hand.py` & `controlnet_v11_utils-0.0.8/annotator/openpose/hand.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/openpose/model.py` & `controlnet_v11_utils-0.0.8/annotator/openpose/model.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/openpose/util.py` & `controlnet_v11_utils-0.0.8/annotator/openpose/util.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/pidinet/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/pidinet/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/pidinet/model.py` & `controlnet_v11_utils-0.0.8/annotator/pidinet/model.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/shuffle/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/arraymisc/quantization.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/arraymisc/quantization.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/alexnet.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/activation.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/context_block.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/conv.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/conv.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/conv_module.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/conv_module.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/conv_ws.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/drop.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/generalized_attention.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/hsigmoid.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/hswish.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/non_local.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/norm.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/norm.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/padding.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/padding.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/plugin.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/plugin.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/registry.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/registry.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/scale.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/transformer.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/upsample.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/upsample.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/bricks/wrappers.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/bricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/builder.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/builder.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/resnet.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/utils/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/utils/flops_counter.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/utils/fuse_conv_bn.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/utils/sync_bn.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/utils/sync_bn.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/utils/weight_init.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/cnn/vgg.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/engine/test.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/engine/test.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/file_client.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/handlers/base.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/handlers/json_handler.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/handlers/pickle_handler.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/handlers/yaml_handler.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/io.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/io.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/fileio/parse.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/image/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/image/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/image/colorspace.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/image/geometric.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/image/geometric.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/image/io.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/image/io.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/image/misc.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/image/misc.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/image/photometric.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/image/photometric.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/assign_score_withk.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/assign_score_withk.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/ball_query.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/ball_query.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/bbox.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/border_align.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/border_align.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/box_iou_rotated.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/box_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/carafe.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/carafe.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/cc_attention.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/cc_attention.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/contour_expand.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/contour_expand.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/corner_pool.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/corner_pool.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/correlation.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/correlation.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/deform_conv.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/deform_roi_pool.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/deform_roi_pool.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/deprecated_wrappers.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/deprecated_wrappers.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/focal_loss.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/focal_loss.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/furthest_point_sample.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/furthest_point_sample.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/fused_bias_leakyrelu.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/fused_bias_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/gather_points.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/gather_points.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/group_points.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/group_points.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/info.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/info.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/iou3d.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/iou3d.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/knn.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/knn.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/masked_conv.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/masked_conv.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/merge_cells.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/merge_cells.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/modulated_deform_conv.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/modulated_deform_conv.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/multi_scale_deform_attn.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/multi_scale_deform_attn.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/nms.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/nms.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/pixel_group.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/pixel_group.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/point_sample.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/point_sample.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/points_in_boxes.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/points_in_boxes.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/points_sampler.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/points_sampler.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/psa_mask.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/psa_mask.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/roi_align.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/roi_align.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/roi_align_rotated.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/roi_pool.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/roi_pool.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/roiaware_pool3d.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/roiaware_pool3d.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/roipoint_pool3d.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/roipoint_pool3d.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/saconv.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/saconv.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/scatter_points.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/scatter_points.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/sync_bn.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/sync_bn.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/three_interpolate.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/three_interpolate.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/three_nn.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/three_nn.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/tin_shift.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/tin_shift.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/upfirdn2d.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/ops/voxelize.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/ops/voxelize.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/_functions.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/_functions.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/collate.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/data_container.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/data_container.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/data_parallel.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/distributed.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/distributed_deprecated.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/distributed_deprecated.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/scatter_gather.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/parallel/utils.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/base_module.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/base_module.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/base_runner.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/builder.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/builder.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/checkpoint.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/default_constructor.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/default_constructor.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/dist_utils.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/dist_utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/epoch_based_runner.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/epoch_based_runner.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/fp16_utils.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/fp16_utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/checkpoint.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/ema.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/ema.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/evaluation.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/evaluation.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/hook.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/base.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/base.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/dvclive.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/dvclive.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/mlflow.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/mlflow.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/neptune.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/neptune.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/pavi.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/pavi.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/tensorboard.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/text.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/text.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/logger/wandb.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/logger/wandb.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/lr_updater.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/lr_updater.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/memory.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/momentum_updater.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/momentum_updater.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/optimizer.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/profiler.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/profiler.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/sampler_seed.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/sampler_seed.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/hooks/sync_buffer.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/hooks/sync_buffer.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/iter_based_runner.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/iter_based_runner.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/log_buffer.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/log_buffer.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/optimizer/builder.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/optimizer/default_constructor.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/priority.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/priority.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/runner/utils.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/runner/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/config.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/config.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/env.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/env.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/ext_loader.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/logging.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/logging.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/misc.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/misc.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/parrots_jit.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/parrots_wrapper.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/path.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/path.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/progressbar.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/registry.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/registry.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/testing.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/testing.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/timer.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/timer.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/trace.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/trace.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/utils/version_utils.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/version.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/version.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/video/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/video/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/video/io.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/video/io.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/video/optflow.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/video/optflow.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/video/processing.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/video/processing.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/visualization/color.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/visualization/color.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/visualization/image.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/visualization/image.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv/visualization/optflow.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv/visualization/optflow.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/uniformer/mmcv_custom/checkpoint.py` & `controlnet_v11_utils-0.0.8/annotator/uniformer/mmcv_custom/checkpoint.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/util.py` & `controlnet_v11_utils-0.0.8/annotator/util.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/annotator/zoe/__init__.py` & `controlnet_v11_utils-0.0.8/annotator/zoe/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/cldm/cldm.py` & `controlnet_v11_utils-0.0.8/cldm/cldm.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/cldm/ddim_hacked.py` & `controlnet_v11_utils-0.0.8/cldm/ddim_hacked.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/cldm/hack.py` & `controlnet_v11_utils-0.0.8/cldm/hack.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/cldm/logger.py` & `controlnet_v11_utils-0.0.8/cldm/logger.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/cldm/model.py` & `controlnet_v11_utils-0.0.8/cldm/model.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/controlnet_v11_utils.egg-info/SOURCES.txt` & `controlnet_v11_utils-0.0.8/controlnet_v11_utils.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -421,10 +421,47 @@
 controlnet_v11_utils.egg-info/SOURCES.txt
 controlnet_v11_utils.egg-info/dependency_links.txt
 controlnet_v11_utils.egg-info/top_level.txt
 ldm/__init__.py
 ldm/util.py
 ldm/data/__init__.py
 ldm/data/util.py
+ldm/models/__init__.py
+ldm/models/autoencoder.py
+ldm/models/diffusion/__init__.py
+ldm/models/diffusion/ddim.py
+ldm/models/diffusion/ddpm.py
+ldm/models/diffusion/plms.py
+ldm/models/diffusion/sampling_util.py
+ldm/models/diffusion/dpm_solver/__init__.py
+ldm/models/diffusion/dpm_solver/dpm_solver.py
+ldm/models/diffusion/dpm_solver/sampler.py
+ldm/modules/__init__.py
+ldm/modules/attention.py
+ldm/modules/ema.py
+ldm/modules/diffusionmodules/__init__.py
+ldm/modules/diffusionmodules/model.py
+ldm/modules/diffusionmodules/openaimodel.py
+ldm/modules/diffusionmodules/upscaling.py
+ldm/modules/diffusionmodules/util.py
+ldm/modules/distributions/__init__.py
+ldm/modules/distributions/distributions.py
+ldm/modules/encoders/__init__.py
+ldm/modules/encoders/modules.py
+ldm/modules/image_degradation/__init__.py
+ldm/modules/image_degradation/bsrgan.py
+ldm/modules/image_degradation/bsrgan_light.py
+ldm/modules/image_degradation/utils_image.py
+ldm/modules/midas/__init__.py
+ldm/modules/midas/api.py
+ldm/modules/midas/utils.py
+ldm/modules/midas/midas/__init__.py
+ldm/modules/midas/midas/base_model.py
+ldm/modules/midas/midas/blocks.py
+ldm/modules/midas/midas/dpt_depth.py
+ldm/modules/midas/midas/midas_net.py
+ldm/modules/midas/midas/midas_net_custom.py
+ldm/modules/midas/midas/transforms.py
+ldm/modules/midas/midas/vit.py
 models/__init__.py
 share/__init__.py
 share/share.py
```

### Comparing `controlnet_v11_utils-0.0.7/ldm/data/util.py` & `controlnet_v11_utils-0.0.8/ldm/data/util.py`

 * *Files identical despite different names*

### Comparing `controlnet_v11_utils-0.0.7/ldm/util.py` & `controlnet_v11_utils-0.0.8/ldm/util.py`

 * *Files identical despite different names*

