# Comparing `tmp/bmcook-0.1.1.1.tar.gz` & `tmp/bmcook-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmcook-0.1.1.1.tar", last modified: Tue Nov 15 06:27:12 2022, max compression
+gzip compressed data, was "bmcook-0.1.2.tar", last modified: Mon Jun 12 03:47:11 2023, max compression
```

## Comparing `bmcook-0.1.1.1.tar` & `bmcook-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2022-11-15 06:27:12.168515 bmcook-0.1.1.1/
--rw-r--r--   0 gongbaitao   (501) staff       (20)    11337 2022-09-05 05:06:36.000000 bmcook-0.1.1.1/LICENSE
--rw-r--r--   0 gongbaitao   (501) staff       (20)      238 2022-11-15 06:27:12.168309 bmcook-0.1.1.1/PKG-INFO
--rw-r--r--   0 gongbaitao   (501) staff       (20)    10438 2022-11-07 10:03:38.000000 bmcook-0.1.1.1/README.md
-drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2022-11-15 06:27:12.162089 bmcook-0.1.1.1/bmcook/
--rw-r--r--   0 gongbaitao   (501) staff       (20)      230 2022-10-27 09:22:48.000000 bmcook-0.1.1.1/bmcook/__init__.py
-drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2022-11-15 06:27:12.163352 bmcook-0.1.1.1/bmcook/distilling/
--rw-r--r--   0 gongbaitao   (501) staff       (20)    10974 2022-10-27 09:18:10.000000 bmcook-0.1.1.1/bmcook/distilling/__init__.py
-drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2022-11-15 06:27:12.163630 bmcook-0.1.1.1/bmcook/moe/
--rw-r--r--   0 gongbaitao   (501) staff       (20)     4037 2022-10-27 09:17:57.000000 bmcook-0.1.1.1/bmcook/moe/__init__.py
-drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2022-11-15 06:27:12.164302 bmcook-0.1.1.1/bmcook/pruning/
--rw-r--r--   0 gongbaitao   (501) staff       (20)    10055 2022-10-27 09:17:57.000000 bmcook-0.1.1.1/bmcook/pruning/__init__.py
--rw-r--r--   0 gongbaitao   (501) staff       (20)     5165 2022-10-27 09:17:59.000000 bmcook-0.1.1.1/bmcook/pruning/prune_func.py
-drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2022-11-15 06:27:12.167272 bmcook-0.1.1.1/bmcook/pruning/sprune/
--rw-r--r--   0 gongbaitao   (501) staff       (20)       65 2022-10-27 09:17:58.000000 bmcook-0.1.1.1/bmcook/pruning/sprune/__init__.py
--rw-r--r--   0 gongbaitao   (501) staff       (20)    10984 2022-10-27 09:17:58.000000 bmcook-0.1.1.1/bmcook/pruning/sprune/do_prune.py
--rw-r--r--   0 gongbaitao   (501) staff       (20)     8431 2022-10-27 09:17:58.000000 bmcook-0.1.1.1/bmcook/pruning/sprune/engine.py
--rw-r--r--   0 gongbaitao   (501) staff       (20)     3718 2022-10-27 09:17:59.000000 bmcook-0.1.1.1/bmcook/pruning/sprune/func.py
--rw-r--r--   0 gongbaitao   (501) staff       (20)    12522 2022-10-27 09:17:59.000000 bmcook-0.1.1.1/bmcook/pruning/sprune/plugin.py
--rw-r--r--   0 gongbaitao   (501) staff       (20)    11702 2022-10-27 09:17:59.000000 bmcook-0.1.1.1/bmcook/pruning/sprune/utils.py
-drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2022-11-15 06:27:12.167428 bmcook-0.1.1.1/bmcook/quant/
--rw-r--r--   0 gongbaitao   (501) staff       (20)     1876 2022-11-07 09:49:02.000000 bmcook-0.1.1.1/bmcook/quant/__init__.py
--rw-r--r--   0 gongbaitao   (501) staff       (20)     7610 2022-10-27 09:23:51.000000 bmcook-0.1.1.1/bmcook/store.py
--rw-r--r--   0 gongbaitao   (501) staff       (20)     8666 2022-11-07 09:53:04.000000 bmcook-0.1.1.1/bmcook/trainer.py
-drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2022-11-15 06:27:12.168052 bmcook-0.1.1.1/bmcook/utils/
--rw-r--r--   0 gongbaitao   (501) staff       (20)        0 2022-10-27 09:18:01.000000 bmcook-0.1.1.1/bmcook/utils/__init__.py
--rw-r--r--   0 gongbaitao   (501) staff       (20)      689 2022-10-27 09:18:01.000000 bmcook-0.1.1.1/bmcook/utils/arguments.py
--rw-r--r--   0 gongbaitao   (501) staff       (20)     1579 2022-10-27 09:18:01.000000 bmcook-0.1.1.1/bmcook/utils/config.py
-drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2022-11-15 06:27:12.163061 bmcook-0.1.1.1/bmcook.egg-info/
--rw-r--r--   0 gongbaitao   (501) staff       (20)      238 2022-11-15 06:27:12.000000 bmcook-0.1.1.1/bmcook.egg-info/PKG-INFO
--rw-r--r--   0 gongbaitao   (501) staff       (20)      629 2022-11-15 06:27:12.000000 bmcook-0.1.1.1/bmcook.egg-info/SOURCES.txt
--rw-r--r--   0 gongbaitao   (501) staff       (20)        1 2022-11-15 06:27:12.000000 bmcook-0.1.1.1/bmcook.egg-info/dependency_links.txt
--rw-r--r--   0 gongbaitao   (501) staff       (20)       21 2022-11-15 06:27:12.000000 bmcook-0.1.1.1/bmcook.egg-info/requires.txt
--rw-r--r--   0 gongbaitao   (501) staff       (20)        7 2022-11-15 06:27:12.000000 bmcook-0.1.1.1/bmcook.egg-info/top_level.txt
--rw-r--r--   0 gongbaitao   (501) staff       (20)       38 2022-11-15 06:27:12.168561 bmcook-0.1.1.1/setup.cfg
--rw-r--r--   0 gongbaitao   (501) staff       (20)      513 2022-11-15 06:27:03.000000 bmcook-0.1.1.1/setup.py
+drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2023-06-12 03:47:11.420142 bmcook-0.1.2/
+-rw-r--r--   0 gongbaitao   (501) staff       (20)      249 2023-06-12 03:47:11.419916 bmcook-0.1.2/PKG-INFO
+-rw-r--r--   0 gongbaitao   (501) staff       (20)    10655 2023-05-27 18:14:41.000000 bmcook-0.1.2/README.md
+drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2023-06-12 03:47:11.413248 bmcook-0.1.2/bmcook/
+-rw-r--r--   0 gongbaitao   (501) staff       (20)      263 2023-05-27 17:17:45.000000 bmcook-0.1.2/bmcook/__init__.py
+drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2023-06-12 03:47:11.414911 bmcook-0.1.2/bmcook/distilling/
+-rw-r--r--   0 gongbaitao   (501) staff       (20)     9195 2023-05-27 17:17:45.000000 bmcook-0.1.2/bmcook/distilling/__init__.py
+drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2023-06-12 03:47:11.415227 bmcook-0.1.2/bmcook/moe/
+-rw-r--r--   0 gongbaitao   (501) staff       (20)     4046 2023-05-27 17:17:45.000000 bmcook-0.1.2/bmcook/moe/__init__.py
+drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2023-06-12 03:47:11.416027 bmcook-0.1.2/bmcook/pruning/
+-rw-r--r--   0 gongbaitao   (501) staff       (20)     9703 2023-05-27 17:54:39.000000 bmcook-0.1.2/bmcook/pruning/__init__.py
+-rw-r--r--   0 gongbaitao   (501) staff       (20)     5165 2023-05-27 17:17:45.000000 bmcook-0.1.2/bmcook/pruning/prune_func.py
+drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2023-06-12 03:47:11.417390 bmcook-0.1.2/bmcook/pruning/sprune/
+-rw-r--r--   0 gongbaitao   (501) staff       (20)       81 2023-05-27 17:20:11.000000 bmcook-0.1.2/bmcook/pruning/sprune/__init__.py
+-rw-r--r--   0 gongbaitao   (501) staff       (20)     6625 2023-05-27 17:20:12.000000 bmcook-0.1.2/bmcook/pruning/sprune/engine.py
+-rw-r--r--   0 gongbaitao   (501) staff       (20)     2279 2023-05-27 17:20:12.000000 bmcook-0.1.2/bmcook/pruning/sprune/func.py
+drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2023-06-12 03:47:11.418459 bmcook-0.1.2/bmcook/pruning/sprune/plugin/
+-rw-r--r--   0 gongbaitao   (501) staff       (20)       63 2023-05-27 17:20:11.000000 bmcook-0.1.2/bmcook/pruning/sprune/plugin/__init__.py
+-rw-r--r--   0 gongbaitao   (501) staff       (20)     5708 2023-05-27 17:20:11.000000 bmcook-0.1.2/bmcook/pruning/sprune/plugin/plugin.py
+-rw-r--r--   0 gongbaitao   (501) staff       (20)    12918 2023-05-27 17:20:11.000000 bmcook-0.1.2/bmcook/pruning/sprune/plugin/unit.py
+-rw-r--r--   0 gongbaitao   (501) staff       (20)     3454 2023-05-27 17:20:11.000000 bmcook-0.1.2/bmcook/pruning/sprune/plugin/unitlist.py
+-rw-r--r--   0 gongbaitao   (501) staff       (20)     2603 2023-05-27 17:20:12.000000 bmcook-0.1.2/bmcook/pruning/sprune/utils.py
+drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2023-06-12 03:47:11.418759 bmcook-0.1.2/bmcook/quant/
+-rw-r--r--   0 gongbaitao   (501) staff       (20)     2561 2023-05-27 17:17:45.000000 bmcook-0.1.2/bmcook/quant/__init__.py
+-rw-r--r--   0 gongbaitao   (501) staff       (20)     4737 2023-05-27 18:45:40.000000 bmcook-0.1.2/bmcook/store.py
+-rw-r--r--   0 gongbaitao   (501) staff       (20)     5267 2023-05-27 17:55:11.000000 bmcook-0.1.2/bmcook/trainer.py
+drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2023-06-12 03:47:11.419581 bmcook-0.1.2/bmcook/utils/
+-rw-r--r--   0 gongbaitao   (501) staff       (20)        0 2023-05-27 17:17:45.000000 bmcook-0.1.2/bmcook/utils/__init__.py
+-rw-r--r--   0 gongbaitao   (501) staff       (20)      689 2023-05-27 17:17:45.000000 bmcook-0.1.2/bmcook/utils/arguments.py
+-rw-r--r--   0 gongbaitao   (501) staff       (20)     1579 2023-05-27 17:17:45.000000 bmcook-0.1.2/bmcook/utils/config.py
+drwxr-xr-x   0 gongbaitao   (501) staff       (20)        0 2023-06-12 03:47:11.414618 bmcook-0.1.2/bmcook.egg-info/
+-rw-r--r--   0 gongbaitao   (501) staff       (20)      249 2023-06-12 03:47:11.000000 bmcook-0.1.2/bmcook.egg-info/PKG-INFO
+-rw-r--r--   0 gongbaitao   (501) staff       (20)      713 2023-06-12 03:47:11.000000 bmcook-0.1.2/bmcook.egg-info/SOURCES.txt
+-rw-r--r--   0 gongbaitao   (501) staff       (20)        1 2023-06-12 03:47:11.000000 bmcook-0.1.2/bmcook.egg-info/dependency_links.txt
+-rw-r--r--   0 gongbaitao   (501) staff       (20)       21 2023-06-12 03:47:11.000000 bmcook-0.1.2/bmcook.egg-info/requires.txt
+-rw-r--r--   0 gongbaitao   (501) staff       (20)        7 2023-06-12 03:47:11.000000 bmcook-0.1.2/bmcook.egg-info/top_level.txt
+-rw-r--r--   0 gongbaitao   (501) staff       (20)       38 2023-06-12 03:47:11.420199 bmcook-0.1.2/setup.cfg
+-rw-r--r--   0 gongbaitao   (501) staff       (20)      507 2023-06-12 03:18:58.000000 bmcook-0.1.2/setup.py
```

### Comparing `bmcook-0.1.1.1/README.md` & `bmcook-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 	<a>
 		 <img alt="version" src="https://img.shields.io/badge/version-0.1.0-blue">
 	</a>
 </p>    
 
 ## What's New
 
+- 2023/5/27 Support structured pruning of Decoder-only models, and the compression of [CPM-Live](https://github.com/OpenBMB/CPM-Live/tree/master) models。
 - 2022/5/17 Support PLMs in [model-center](https://github.com/OpenBMB/ModelCenter).
 - 2022/3/29 (**BMCook 0.1.0**) Now we publicly release the first version of BMCook.
 
 <div id="overview"></div>
 
 ## Overview
 
@@ -235,23 +236,25 @@
      --model gpt2-base \
      --start-lr 1e-4 \
      --cook-config configs/gpt2-combine.json \
 ```
 
 ## Performances
 
-Based on GPT-J, we evaluate different combinations of compression techniques. The corpus is OpenWebText. We also train a small GPT-J with 0.7B parameters based on this corpus from scratch, GPT-J (0.7B).
+Based on T5-3B, we evaluate different combinations of compression techniques. The corpus for compression is the Pile. The evaluation datasets includes SST-2, MNLI, and SQuAD. Specifically, we freeze the compressed models and adopt adapter-tuning.
 
-|                        |     LM Loss    |     Relative Performance    |     Speedup    |
+|                        |     Average Performance    |     Relative Performance    |     Speedup    |
 |------------------------|----------------|-----------------------------|----------------|
-|     GPT-J              |           3.37 |                        -    |          1x    |
-|     GPT-J (0.7B)       |           4.06 |                       83.0% |         ~10x   |
-|     GPT-J (P+D)        |           3.57 |                       94.4% |          2x    |
-|     GPT-J (P+D+Q)      |           3.58 |                       94.1% |          8x    |
-|     GPT-J (P+D+Q+M)    |           3.69 |                       91.3% |          10x   |
+|     T5-3B              |           0.9258 |                        -    |          1x    |
+|     T5-Base       |           0.8796 |                       95.0% |         7x   |
+|     T5-3B (P+D)        |           0.9150 |                       98.8% |          2x    |
+|     T5-3B (P+D+Q)      |           0.9126 |                       98.6% |          8x    |
+|     T5-3B (P+D+Q+M)    |           0.9017 |                       97.4% |          12x   |
+
+
 
 D denotes knowledge distillation. P denotes pruning. Q denotes quantization. M denotes MoEfication.
 
 ## Comparisons
 
 |                 | Model Quantization | Model Pruning | Knowledge Distillation | Model MoEfication |
 |-----------------|--------------------|---------------|------------------------|-------------------|
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
                  ****** [docs/_static/logo.png] BMCook ******
                      **Model Compression for Big Models**
    Overview â¢ Documentation â¢ Installation â¢ Usage â¢ Quick_Start â¢
                                  ç®ä½ä¸­æ
                            [doc] [github] [version]
-## What's New - 2022/5/17 Support PLMs in [model-center](https://github.com/
-OpenBMB/ModelCenter). - 2022/3/29 (**BMCook 0.1.0**) Now we publicly release
-the first version of BMCook.
+## What's New - 2023/5/27 Support structured pruning of Decoder-only models,
+and the compression of [CPM-Live](https://github.com/OpenBMB/CPM-Live/tree/
+master) modelsã - 2022/5/17 Support PLMs in [model-center](https://
+github.com/OpenBMB/ModelCenter). - 2022/3/29 (**BMCook 0.1.0**) Now we publicly
+release the first version of BMCook.
 ## Overview BMCook is a model compression toolkit for large-scale pre-trained
 language models (PLMs), which integrates multiple model compression methods.
 You can combine them in any way to achieve the desired speedup. Specifically,
 we implement the following four model compression methods, knowledge
 distillation, model pruning, model quantization, and model MoEfication. It has
 following features: - **Various Supported Methods.** Compared to existing
 compression toolkits, BMCook supports all mainstream acceleration methods for
@@ -88,31 +90,31 @@
 MoEfication toolkit)ï¼ ``` torchrun --nnodes=1 --nproc_per_node=1 --rdzv_id=1
 --rdzv_backend=c10d --rdzv_endpoint=localhost train.py \ --save-dir results/
 gpt2-moe \ --model gpt2-base \ --start-lr 1e-4 \ --cook-config configs/gpt2-
 moe.json \ ``` Combine quantization, pruning and knowledge distillationï¼ ```
 torchrun --nnodes=1 --nproc_per_node=1 --rdzv_id=1 --rdzv_backend=c10d --
 rdzv_endpoint=localhost train.py \ --save-dir results/gpt2-combine \ --model
 gpt2-base \ --start-lr 1e-4 \ --cook-config configs/gpt2-combine.json \ ``` ##
-Performances Based on GPT-J, we evaluate different combinations of compression
-techniques. The corpus is OpenWebText. We also train a small GPT-J with 0.7B
-parameters based on this corpus from scratch, GPT-J (0.7B). | | LM Loss |
-Relative Performance | Speedup | |------------------------|----------------|---
---------------------------|----------------| | GPT-J | 3.37 | - | 1x | | GPT-J
-(0.7B) | 4.06 | 83.0% | ~10x | | GPT-J (P+D) | 3.57 | 94.4% | 2x | | GPT-J
-(P+D+Q) | 3.58 | 94.1% | 8x | | GPT-J (P+D+Q+M) | 3.69 | 91.3% | 10x | D
-denotes knowledge distillation. P denotes pruning. Q denotes quantization. M
-denotes MoEfication. ## Comparisons | | Model Quantization | Model Pruning |
-Knowledge Distillation | Model MoEfication | |-----------------|---------------
------|---------------|------------------------|-------------------| |
-[TextPruner](https://github.com/airaria/TextPruner) | - | â | - | - | |
-[TensorFlow Lite](https://www.tensorflow.org/lite) | â | â | - | - | |
-[PyTorch](https://pytorch.org/) | â | â | - | - | | [TextBrewer](https://
-github.com/airaria/TextBrewer) | - | â | â | - | | BMCook | â | â | â
-| â | ## Community We welcome everyone to contribute codes following our
-[contributing guidelines](https://github.com/OpenBMB/BMCook/blob/main/
-CONTRIBUTING.md). You can also find us on other platforms: - QQ Group:
-735930538 - WeChat Official Account: OpenBMB - Website: https://www.openbmb.org
-- Weibo: http://weibo.cn/OpenBMB - Twitter: https://twitter.com/OpenBMB ##
-License The package is released under the [Apache 2.0](https://github.com/
-OpenBMB/BMCook/blob/main/LICENSE) License. ## Contributors We thank Zhengyan
-Zhang, Baitao Gong, Yingfa Chen, Guoyang Zeng, Jie Zhou, and Zhi Zheng for the
-contribution. More contributors are welcome!
+Performances Based on T5-3B, we evaluate different combinations of compression
+techniques. The corpus for compression is the Pile. The evaluation datasets
+includes SST-2, MNLI, and SQuAD. Specifically, we freeze the compressed models
+and adopt adapter-tuning. | | Average Performance | Relative Performance |
+Speedup | |------------------------|----------------|--------------------------
+---|----------------| | T5-3B | 0.9258 | - | 1x | | T5-Base | 0.8796 | 95.0% |
+7x | | T5-3B (P+D) | 0.9150 | 98.8% | 2x | | T5-3B (P+D+Q) | 0.9126 | 98.6% |
+8x | | T5-3B (P+D+Q+M) | 0.9017 | 97.4% | 12x | D denotes knowledge
+distillation. P denotes pruning. Q denotes quantization. M denotes MoEfication.
+## Comparisons | | Model Quantization | Model Pruning | Knowledge Distillation
+| Model MoEfication | |-----------------|--------------------|---------------|-
+-----------------------|-------------------| | [TextPruner](https://github.com/
+airaria/TextPruner) | - | â | - | - | | [TensorFlow Lite](https://
+www.tensorflow.org/lite) | â | â | - | - | | [PyTorch](https://pytorch.org/
+) | â | â | - | - | | [TextBrewer](https://github.com/airaria/TextBrewer) |
+- | â | â | - | | BMCook | â | â | â | â | ## Community We welcome
+everyone to contribute codes following our [contributing guidelines](https://
+github.com/OpenBMB/BMCook/blob/main/CONTRIBUTING.md). You can also find us on
+other platforms: - QQ Group: 735930538 - WeChat Official Account: OpenBMB -
+Website: https://www.openbmb.org - Weibo: http://weibo.cn/OpenBMB - Twitter:
+https://twitter.com/OpenBMB ## License The package is released under the
+[Apache 2.0](https://github.com/OpenBMB/BMCook/blob/main/LICENSE) License. ##
+Contributors We thank Zhengyan Zhang, Baitao Gong, Yingfa Chen, Guoyang Zeng,
+Jie Zhou, and Zhi Zheng for the contribution. More contributors are welcome!
```

### Comparing `bmcook-0.1.1.1/bmcook/distilling/__init__.py` & `bmcook-0.1.2/bmcook/distilling/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,152 +1,103 @@
 import types
+import torch
 import bmtrain as bmt
 import torch.nn.functional as F
-import model_center
+import model_center.layer as Layer
 
 
 class BMDistill:
     '''
     BMDistill provide additional training objectives for knowledge distillation, which further improves the performance of compressed models.
     '''
 
     @classmethod
-    def set_forward(cls, student, teacher, foward_fn, config):
+    def set_forward(cls, student, teacher, forward_fn, config, target_linear = Layer.Linear):
         '''
         Modify the forward function of the student model to compute additional knowledge distillation loss.
 
-        `foward_fn` should have the following arguments: `foward_fn(model, enc_input, enc_length, dec_input, dec_length, targets, loss_func)`. These arguments are general for existing Transformers. For decoder-only model, `enc_input` and `enc_length` can be set to None. For encoder-only model, `dec_input` and `dec_length` can be set to None. Similarly, `student` and `teacher` models also have the following arguments: `model(enc_input, enc_length, dec_input, dec_length)`.
+        `forward_fn` should have the following arguments: `forward_fn(model, enc_input, enc_length, dec_input, dec_length, targets, loss_func)`. These arguments are general for existing Transformers. For decoder-only model, `enc_input` and `enc_length` can be set to None. For encoder-only model, `dec_input` and `dec_length` can be set to None. Similarly, `student` and `teacher` models also have the following arguments: `model(enc_input, enc_length, dec_input, dec_length)`.
 
         :param student: Student model.
         :param teacher: Teacher model.
-        :param foward_fn: Forward function of the student model.
+        :param forward_fn: Forward function of the student model.
         :param config: ConfigParser object.
-        :return: Modified forward function, whose return values are the original return values of `foward_fn` and additional knowledge distillation loss.
+        :return: Modified forward function, whose return values are the original return values of `forward_fn` and additional knowledge distillation loss.
         '''
 
         distill_config = config.get('distillation')
         if distill_config['ce_scale'] + distill_config['mse_hidn_scale'] + distill_config['mse_att_scale'] == 0:
             # if all scales are zero, return the original forward function
-            return foward_fn
+            return forward_fn
 
         if distill_config['mse_hidn_scale'] > 0:
             # if mse_hidn_scale is not zero, get the module mapping from the teacher model to the student model
             s_module_map, t_module_map = get_module_map(distill_config['mse_hidn_module'])
             update_forward(student, teacher, s_module_map, t_module_map)
 
-        if cls.version:
-            def forward(model, loss_func, targets, *model_args, **model_kwargs):
+        target_linear = Layer.Linear if target_linear is None else target_linear
 
-                with bmt.inspect.inspect_tensor() as inspector:
-                    outputs = foward_fn(
-                        model, loss_func, targets, *model_args, **model_kwargs)
+        def forward(model, loss_func, targets, *model_args, **model_kwargs):
+            with bmt.inspect.inspect_tensor() as inspector:
+                outputs = forward_fn(
+                    model, loss_func, targets, *model_args, **model_kwargs
+                )
+                with torch.no_grad():
                     outputs_t = teacher(*model_args, **model_kwargs)
 
-                records = {}
-                for record in inspector._summary:
-                    records[record['name']] = record['tensor']
-
-                loss = outputs[0]
-                model_outputs = outputs[1]
-                logits_s = model_outputs
-
-
-                # Compute loss and d_loss
-                d_loss = 0.0
-                if distill_config['ce_scale'] > 0:
-                    temp = distill_config['ce_temp']
-                    logits_t = outputs_t.detach()
-                    prob_t = F.softmax(logits_t / temp, dim=-1)
-                    log_prob_s = F.log_softmax(logits_s / temp, dim=-1)
-                    d_loss += -(prob_t * log_prob_s).sum(dim=1).mean() * distill_config['ce_scale']
-            
-                # MSE loss 
-                if distill_config['mse_hidn_scale'] > 0:
-                    for module_name in s_module_map:
-                        t_module_name = s_module_map[module_name]['t']['name']
-                        student_t = records[module_name+'_student']
-                        teacher_t = records[t_module_name+'_teacher'].detach()
-
-                        if distill_config['mse_hidn_proj']:
-                            if 'mapping' not in s_module_map[module_name]:
-                                t_dim = teacher_t.size(-1)
-                                s_dim = student_t.size(-1)
-                                # May be different on different devices
-                                
-                                s_module_map[module_name]['mapping'] = model_center.layer.Linear(t_dim, s_dim, init_std=0.02)
-                                bmt.init_parameters(s_module_map[module_name]['mapping'])
-                                s_module_map[module_name]['mapping'].to(teacher_t.device)
-                                bmt.synchronize()
-                            
-                            teacher_t = s_module_map[module_name]['mapping'](teacher_t)
-                            
-                        cur_loss = (student_t - teacher_t).pow(2).mean() * distill_config['mse_hidn_scale']
-                        d_loss += cur_loss
-                
-                loss = loss + d_loss
-
-                # update loss & append distillation loss
-                outputs[0] = loss
-                outputs[4] = d_loss
-                return outputs
-        else:
-            def forward(model, loss_func, targets, *model_args, **model_kwargs):
-
-                with bmt.inspect.inspect_tensor() as inspector:
-                    outputs = foward_fn(
-                        model, loss_func, targets, *model_args, **model_kwargs)    
-                    outputs_t = teacher(*model_args, **model_kwargs)
-
-
-                records = {}
-                for record in inspector._summary:
-                    records[record['name']] = record['tensor']
-
-                loss = outputs[0]
-                model_outputs = outputs[1]
-                logits_s = model_outputs
-
-                # Compute loss and d_loss
-                d_loss = 0.0
-                if distill_config['ce_scale'] > 0:
-                    temp = distill_config['ce_temp']
-                    logits_t = outputs_t.logits.detach()
-                    prob_t = F.softmax(logits_t / temp, dim=-1)
-                    log_prob_s = F.log_softmax(logits_s / temp, dim=-1)
-                    d_loss += -(prob_t * log_prob_s).sum(dim=1).mean() * distill_config['ce_scale']
-            
-                # MSE loss 
-                if distill_config['mse_hidn_scale'] > 0:
-                    for module_name in s_module_map:
-                        t_module_name = s_module_map[module_name]['t']['name']
-                        student_t = records[module_name+'_student']
-                        teacher_t = records[t_module_name+'_teacher'].detach()
-
-                        if distill_config['mse_hidn_proj']:
-                            if 'mapping' not in s_module_map[module_name]:
-                                t_dim = teacher_t.size(-1)
-                                s_dim = student_t.size(-1)
-                                # May be different on different devices
-                                
-                                s_module_map[module_name]['mapping'] = model_center.layer.Linear(t_dim, s_dim, init_std=0.02)
-                                bmt.init_parameters(s_module_map[module_name]['mapping'])
-                                s_module_map[module_name]['mapping'].to(teacher_t.device)
-                                bmt.synchronize()
-                            
-                            teacher_t = s_module_map[module_name]['mapping'](teacher_t)
+            records = {}
+            for record in inspector._summary:
+                records[record['name']] = record['tensor']
+
+            loss = outputs.loss
+            model_outputs = outputs.original_output
+            logits_s = model_outputs.logits
+
+            # Compute loss and d_loss
+            d_loss = 0.0
+            if distill_config['ce_scale'] > 0:
+                temp = distill_config['ce_temp']
+                logits_t = outputs_t[0].detach()
+                prob_t = F.softmax(logits_t / temp, dim=-1)
+                log_prob_s = F.log_softmax(logits_s / temp, dim=-1)
+                d_loss += -(prob_t * log_prob_s).sum(dim=1).mean() * distill_config['ce_scale']
+        
+            # MSE loss 
+            if distill_config['mse_hidn_scale'] > 0:
+                for module_name in s_module_map:
+                    t_module_name = s_module_map[module_name]['t']['name']
+                    student_t = records[module_name+'_student']
+                    teacher_t = records[t_module_name+'_teacher'].detach()
+
+                    if distill_config['mse_hidn_proj']:
+                        if 'mapping' not in s_module_map[module_name]:
+                            t_dim = teacher_t.size(-1)
+                            s_dim = student_t.size(-1)
+                            # May be different on different devices
                             
-                        cur_loss = (student_t - teacher_t).pow(2).mean() * distill_config['mse_hidn_scale']
-                        d_loss += cur_loss
-                
-                loss = loss + d_loss
-
-                # update loss & append distillation loss
-                outputs[0] = loss
-                outputs[4] = d_loss
-                return outputs
+                            s_module_map[module_name]['mapping'] = target_linear(t_dim, s_dim, init_std=0.02)
+                            bmt.init_parameters(s_module_map[module_name]['mapping'])
+                            s_module_map[module_name]['mapping'].to(teacher_t.device)
+                            bmt.synchronize()
+                        
+                        teacher_t = s_module_map[module_name]['mapping'](teacher_t)
+
+                    #normalize
+                    student_t_norm = student_t / (student_t.norm(dim=-1)).mean()
+                    teacher_t_norm = teacher_t / (teacher_t.norm(dim=-1)).mean()
+                    
+                    cur_loss = (student_t_norm - teacher_t_norm).pow(2).mean() * distill_config['mse_hidn_scale']
+                    d_loss += cur_loss
+            
+            loss = loss + d_loss
+
+            # update loss & append distillation loss
+            outputs.loss = loss
+            outputs.d_loss = d_loss
+            return outputs
         return forward
 
 def get_module_info(info):
     '''
     Parse module info. For example, "[post]encoder.output_layernorm" is parsed to {'name': 'encoder.output_layernorm', 'type': 'post'}, which means the output of the 'encoder.output_layernorm' module is used for distillation. Meanwhile, "[pre]encoder.output_layernorm" is parsed to {'name': 'encoder.output_layernorm', 'type': 'pre'}, which means the input of the 'encoder.output_layernorm' module is used for distillation.
 
     :param info: Module info.
@@ -186,42 +137,56 @@
 
     '''
 
     select_keys = set()
     for k, v in student.named_modules():
         if k in s_module_map:
             select_keys.add(k)
-            v.forward_old = v.forward
+            if isinstance(v, bmt.CheckpointBlock):
+                v.forward_old = v._module.forward
+            else:
+                v.forward_old = v.forward
             v.inspect_name = k+'_student'
-            
+
             if s_module_map[k]['s']['type'] == 'pre':
-                def _forward(module_self, x):
+                def _forward(module_self, x, *args, **kwargs):
                     bmt.inspect.record_tensor(x, module_self.inspect_name)
-                    return module_self.forward_old(x)
-            
+                    return module_self.forward_old(x, *args, **kwargs)
+
             elif s_module_map[k]['s']['type'] == 'post':
-                def _forward(module_self, x):
-                    x = module_self.forward_old(x)
+                def _forward(module_self, x, *args, **kwargs):
+                    x = module_self.forward_old(x, *args, **kwargs)
+                    assert isinstance(x, torch.Tensor)
                     bmt.inspect.record_tensor(x, module_self.inspect_name)
                     return x
-            
-            v.forward = types.MethodType(_forward, v)
+
+            if isinstance(v, bmt.CheckpointBlock):
+                v._module.forward = types.MethodType(_forward, v)
+            else:
+                v.forward = types.MethodType(_forward, v)
 
     for k, v in teacher.named_modules():
         if k in t_module_map:
             select_keys.add(k)
-            v.forward_old = v.forward
+            if isinstance(v, bmt.CheckpointBlock):
+                v.forward_old = v._module.forward
+            else:
+                v.forward_old = v.forward
             v.inspect_name = k+'_teacher'
 
             if t_module_map[k]['t']['type'] == 'pre':
-                def _forward(module_self, x):
+                def _forward(module_self, x, *args, **kwargs):
                     bmt.inspect.record_tensor(x, module_self.inspect_name)
-                    return module_self.forward_old(x)
+                    return module_self.forward_old(x, *args, **kwargs)
 
             elif t_module_map[k]['t']['type'] == 'post':
-                def _forward(module_self, x):
-                    x = module_self.forward_old(x)
+                def _forward(module_self, x, *args, **kwargs):
+                    x = module_self.forward_old(x, *args, **kwargs)
+                    assert isinstance(x, torch.Tensor)
                     bmt.inspect.record_tensor(x, module_self.inspect_name)
                     return x
-            
-            v.forward = types.MethodType(_forward, v)
-    bmt.print_rank('Selected modules for hidden state MSE: {}'.format(select_keys))                        
+
+            if isinstance(v, bmt.CheckpointBlock):
+                v._module.forward = types.MethodType(_forward, v)
+            else:
+                v.forward = types.MethodType(_forward, v)
+    bmt.print_rank('Selected modules for hidden state MSE: {}'.format(select_keys))
```

### Comparing `bmcook-0.1.1.1/bmcook/moe/__init__.py` & `bmcook-0.1.2/bmcook/moe/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                     model, loss_func, targets, *model_args, **model_kwargs)
             
             records = {}
             for record in inspector._summary:
                 if 'moe_hidden' in record['name']:
                     records[record['name']] = record['tensor']
             
-            outputs[5] = records
+            outputs.moe_records = records
             return outputs
         return forward
 
     # @staticmethod
     # def moefy(model, num_expert, topk, checkpoint=None):
     #     '''
     #     Replace the feed-forward modules in PLMs with MoE modules according to the results of MoEfication from the checkpoint file.
```

### Comparing `bmcook-0.1.1.1/bmcook/pruning/__init__.py` & `bmcook-0.1.2/bmcook/pruning/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from collections import defaultdict
+import os
 import types
 import torch
 import bmtrain as bmt
-import os
-import json
+from collections import defaultdict
 from bmtrain.block_layer import storage_type_cuda, round_up
 from .prune_func import m4n2_1d, m4n2_2d_greedy
-from .sprune import SPruneEngine, SPrunePlugin
+from .sprune import SPruneEngine, SPrunePlugin, SPruneStrategy
 
 
 def get_trivial_mask(p):
     return torch.ones_like(p)
 
 def get_masks(ordered_parameters, func=get_trivial_mask, targets=[]):
     ordered_masks = []
@@ -97,18 +96,20 @@
         checkpoint = prune_config['pruning_mask_path'] if 'pruning_mask_path' in prune_config else None
         if prune_config['mask_method'] == 'm4n2_1d':
             func = m4n2_1d
         elif prune_config['mask_method'] == 'm4n2_2d':
             func = m4n2_2d_greedy
         elif prune_config['mask_method'] == 'sprune':
             sprune_config = prune_config['sprune']
-            plugin = SPrunePlugin(model)
-            cls.sprune_engine = SPruneEngine(sprune_config, plugin)
+            strategy = SPruneStrategy(config=sprune_config)
+            plugin = SPrunePlugin(sprune_config["training_mask"], model)
+            cls.sprune_engine = SPruneEngine(strategy, plugin, saved_path=sprune_config["mask_path"])
             cls._sprune = True
-            return
+            cls.lag_loss, cls.sparsity = None, None
+            return 
         else:
             raise ValueError("Unknown mask method: {}".format(prune_config['mask_method']))
 
 
         if checkpoint is not None:
             if os.path.exists(checkpoint):
                 storaged_masks = torch.load(checkpoint, map_location='cpu')
@@ -160,36 +161,14 @@
 
         if storaged_masks is None and checkpoint is not None and bmt.global_var.config["rank"] == 0:
             torch.save(storaged_masks_, checkpoint)
 
         cls._masks = _masks
 
     @classmethod
-    def set_forward_sprune(cls, forward_fn):
-        r"""
-        Modify the CookTrainer.forward
-
-        :param forward_fn: func CookTrainer.forward to modify.
-        :return: new forward modified
-        """
-        if cls._sprune is True:
-            def forward(model, loss_func, targets, *model_args, **model_kwargs):
-                outputs = forward_fn(model, loss_func, targets, *model_args, **model_kwargs)
-                loss = outputs[0]
-
-                lag_loss, sparsity = cls.sprune_engine.update()
-                loss += lag_loss
-                
-                outputs[0], outputs[2], outputs[3] = loss, lag_loss, sparsity
-                return outputs
-        else:
-            forward = forward_fn
-        return forward
-
-    @classmethod
     def set_optim_for_pruning(cls, optimizer):
         '''
         Modify the step function of the optimizer to avoid the update of the pruned weights, i.e., setting corresponding gradients and parameters to zeros.
 
         :param optimizer: Optimizer to modify.
         :return: Modified optimizer.
         '''
@@ -223,23 +202,26 @@
                             for k in p:
                                 p[k].mul_(mask[k])
                         else:
                             tmp_mask = torch.tensor(mask, dtype=p.dtype, device=p.device)
                             p.mul_(tmp_mask)
                 return rval
             cls._optimizer.step = types.MethodType(_step, cls._optimizer)
-        else:
+        elif cls.sprune_engine.is_training:
             cls._optimizer.zero_grad_old = optimizer.zero_grad
 
             def _step(opt_self, *args, **kwargs):
+                lag_loss, sparsity = cls.sprune_engine.update()
+                lag_loss.backward()
                 rval = opt_self.step_old(*args, **kwargs)
                 cls.sprune_engine.sp_optimizer.step()
                 cls.sprune_engine.lagrangian_optimizer.step()
+                bmt.print_rank("sparsity: {:.4f} | lag_loss: {:.4f}".format(sparsity, lag_loss))
                 return rval
             cls._optimizer.step = types.MethodType(_step, cls._optimizer)
 
             def _zero_grad(opt_self, *args, **kwargs):
                 rval = opt_self.zero_grad_old(*args, **kwargs)
                 cls.sprune_engine.sp_optimizer.zero_grad()
                 cls.sprune_engine.lagrangian_optimizer.zero_grad()
                 return rval
-            cls._optimizer.zero_grad = types.MethodType(_zero_grad, cls._optimizer)
+            cls._optimizer.zero_grad = types.MethodType(_zero_grad, cls._optimizer)
```

### Comparing `bmcook-0.1.1.1/bmcook/pruning/prune_func.py` & `bmcook-0.1.2/bmcook/pruning/prune_func.py`

 * *Files identical despite different names*

### Comparing `bmcook-0.1.1.1/bmcook/pruning/sprune/engine.py` & `bmcook-0.1.2/bmcook/pruning/sprune/engine.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,188 +1,150 @@
 import torch
 import bmtrain as bmt
-from typing import Dict
+from typing import Dict, Optional
 from torch.nn.parameter import Parameter
-from .func import determinate_mask, sample, binarize
-from .plugin import SPrunePlugin
-from .utils import get_params_from_block
+from .func import determinate_mask, sample, binarize, from_sparsity
+from .plugin import SPrunePlugin, UnitList
+from .utils import inspect_checkpoint_block
 
 
 class SPruneStrategy:
     def __init__(self, config: Dict) -> None:
         self.criterion = config['criterion']
         assert self.criterion == 'l0', "BMCook sprune do not support other criterions besides l0 yet."
-        self.fixed_mask_path = config['fixed_mask_path']
+        self.mask_path = config['mask_path']
         self.training_mask = config['training_mask']
-        self.mask_mode = config['mask_mode']
+        self.is_training = config['is_training']
         self.target_mode = config['target_mode']
         self.target_sparsity = config['target_sparsity']
+        self.start_sparsity = config['start_sparsity']
+        self.hard_binarize = config['hard_binarize']
+        self.tuning = config['tuning']
+        if self.is_training is False:
+            self.iterative = self.tuning['iterative']
+            self.interval = self.tuning['interval']
+            self.ratio = self.tuning['ratio']
 
 
-class SPruneEngine:
+class SPruneEngine(bmt.DistributedModule):
     r"""
     SPruneEngine is used for the mask computation and update of SPrunePlugin.
 
     The engine design is based on L0 regularization method and a lagrangian term. For L0 regularization details, see paper
         "Learning Sparse Neural Networks through L_0 Regularization" <https://openreview.net/forum?id=H1Y8hhg0b>.
         For lagrangian term in PLM structure pruning, see paper "Structured Pruning of Large Language Models" 
         <https://arxiv.org/abs/1910.04732>.
     """
-    def __init__(self, config: Dict, plugin: SPrunePlugin) -> None:
+    def __init__(self, strategy: SPruneStrategy, plugin: SPrunePlugin, saved_path: str) -> None:
         r"""Init the SpruneEngine from a SPrunePlugin. It will initilize all the :class:`torch.nn.Parameter`
         used for learning the sprune mask, and create the optimizer for l0 regularization.
 
         Args:
             config: `(Dict)`, the sprune config.
             plugin: `(SPrunePlugin)`, the SPrunePlugin.
         """
         super().__init__()
-        self.strategy = SPruneStrategy(config)
+        self.strategy = strategy
         self.target_sparsity = self.strategy.target_sparsity
+        self.is_training = self.strategy.is_training
         self.plugin = plugin
-        self.training = True
-
-        self.lambda_1 = Parameter(torch.tensor(0.1, dtype=torch.float, device='cuda'))
-        self.lambda_2 = Parameter(torch.tensor(0.1, dtype=torch.float, device='cuda'))
-        self.training_loga = {}
-        for mask in self.strategy.training_mask:
-            shape = self.plugin.info_to_engine['shape'][mask]
-            self.training_loga[mask+'_loga'] = Parameter(torch.empty(shape[0], dtype=torch.float, device='cuda').normal_(0., 1e-2))
+        self.loga_param = None
+        
+        if self.is_training:
+            #TODO from sparsity to loga
+            start_loga = from_sparsity(self.strategy.start_sparsity)
+
+            self.lambda_1 = Parameter(torch.tensor(0., dtype=torch.float, device='cuda'))
+            self.lambda_2 = Parameter(torch.tensor(0., dtype=torch.float, device='cuda'))
+
+            for name, unitlist in self.plugin.named_lists():
+                for i, unit in enumerate(unitlist):
+                    setattr(self, f"{name}-{i}-loga", Parameter(torch.ones_like(unit.mask, dtype=torch.float).normal_(start_loga, 0.01)))
+            self.loga_param = [(n, p) for n, p in self.named_parameters() if '-loga' in n]
+            self.lambda_param = [self.lambda_1, self.lambda_2]
+            self.create_sprune_optimizer()
 
-        self.create_sprune_optimizer()
+        else:
+            self.target_mask = torch.load(saved_path)
+            if not self.strategy.iterative:
+                for k, _ in self.plugin.named_lists():
+                    if k in self.target_mask:
+                        cur_unitlist = getattr(self.plugin, k)
+                        cur_unitlist.load_mask(self.target_mask[k])
+            else:
+                self.interval = self.strategy.interval
+                self.iter_pruner = self.base_iterative_prune()
 
     def create_sprune_optimizer(self):
         r"""Create the sprune optimizer and lagrangian optimizer, making the learning of loga and 
         lagrangian terms to be an adversarial game.
         
         sprune optimizer will manage the loga parameters.
 
         lagrangian optimizer will manage the lagrangian terms.
         """
         l0_params = [{
-                        "params": [p for _, p in self.training_loga.items()],
+                        "params": [p for (_, p) in self.loga_param],
                         "weight_decay": 0.0,
                         "lr": 0.1
                         }]
-        self.sp_optimizer = torch.optim.AdamW(l0_params)
+        self.sp_optimizer = torch.optim.AdamW(l0_params) if self.is_training else None
 
         lagrangian_params = [{
-                    "params": [self.lambda_1, self.lambda_2],
+                    "params": self.lambda_param,
                     "weight_decay": 0.0,
                     "lr": -0.1
                 }]
-        self.lagrangian_optimizer = torch.optim.AdamW(lagrangian_params)
+        self.lagrangian_optimizer = torch.optim.AdamW(lagrangian_params) if self.is_training else None
     
     def update(self):
         r"""
         update the sprune parameters and lagrangian parameters.
         """
-        if self.training:
-            info_list = self.update_plugin_mask(training=True)
-            loss, sparsity = self.loss(info_list)
+        if self.is_training:
+            sparsity = self.forward(True)
+            loss = self.get_loss(sparsity)
             if torch.abs(sparsity - self.target_sparsity) < 5e-5:
                 bmt.print_rank("binarize the mask and begin finetune...")
-                info_list = self.update_plugin_mask(training=False)
-                self.lambda_1.requires_grad_(False)
-                self.lambda_2.requires_grad_(False)
-                for v in self.training_loga.values():
+                sparsity = self.forward(False)
+                for v in self.parameters():
                     v.requires_grad_(False)
-                self.training = False
+                self.is_training = False
+            return loss, sparsity
         else:
-            info_list = self.update_plugin_mask(training=False)
-            loss, sparsity = self.loss(info_list)
-        return loss, sparsity
-
-    def step(self):
-        r"""run :method:`.step()` of sprune optimizer and lagrangian optimizer"""
-        self.sp_optimizer.step()
-        self.lagrangian_optimizer.step()
-    
-    def zero_grad(self):
-        r"""run :method:`.zero_grad()` of sprune optimizer and lagrangian optimizer"""
-        self.sp_optimizer.zero_grad()
-        self.lagrangian_optimizer.zero_grad()
-
-    def loss(self, info_list):
-        r"""calculate the lagrangian loss. It can be calculated in sparsity(`float`) or dimension(`int`)"""
-        if self.strategy.target_mode == 'sparsity':
-            return self.lagrangian_loss_sparsity(info_list, layer_constraint=False)
-        elif self.strategy.target_mode == 'dimension':
-            return self.lagrangian_loss_dimension()
-
-    def update_plugin_mask(self, training: bool = True):
-        r"""update the mask managed in plugin"""
-        info_list = {}
-        for k, v in self.training_loga.items():
-            module = k.split('_loga')[0]
+            return torch.tensor(0), torch.tensor(-1000)
 
+    def forward(self, training: bool = True):
+        for (k, v) in self.loga_param:
+            list_name, unit_index, _ = k.split('-')
             mask = sample(v) if training is True else binarize(v)
             train_mask = determinate_mask(v)
-            assert mask.size(0) == train_mask.size(0)
-            
-            for index in range(mask.size(0)):
-                self.plugin.__dict__[module][index]['mask'] = mask[index].clone().detach()
-                
-                param = self.plugin.__dict__[module][index]['param']
-                index_all = self.plugin.__dict__[module][index]['index']
-
-                if index_all not in info_list:
-                    info_list[index_all] = {'module': [module], 'param': [param], 'score': [train_mask[index]]}
-                else:
-                    if module in info_list[index_all]['module']:
-                        module_correct = 'cross_' + module
-                    else:
-                        module_correct = module
-                    info_list[index_all]['module'].append(module_correct)
-                    info_list[index_all]['param'].append(param)
-                    info_list[index_all]['score'].append(train_mask[index])
-
-        return info_list
-
-    def lagrangian_loss_sparsity(self, info_list, layer_constraint: bool = False):
-        r"""The func 'lagrangian_loss_sparsity' is to calculate the lagrangian loss to get the target sparsity"""
-        expected_sparsity = get_params_from_block(info_list)
+            unit_list = getattr(self.plugin, list_name)
+            unit_list[int(unit_index)].mask = mask.half().clone().detach()
+            unit_list[int(unit_index)].density = train_mask.sum()
+
+        param_exp, param_all = 0, 0
+        for transformer_unit in self.plugin:
+            param_exp += transformer_unit.get_param_exp()
+            param_all += transformer_unit.get_param_all()
+
+        expected_sparsity = 1 - param_exp / param_all
+
+        return expected_sparsity
+    
+    def get_loss(self, expected_sparsity):
         loss_sparsity = expected_sparsity - self.target_sparsity
-        if layer_constraint:
-            loss_sparsity = torch.mean(torch.abs(loss_sparsity))
-            expected_sparsity = torch.mean(expected_sparsity)
-
-        lagrangian_loss = self.lambda_1 * loss_sparsity + self.lambda_2 * (loss_sparsity ** 2)
-
-        return lagrangian_loss, expected_sparsity
-
-    def lagrangian_loss_dimension(self):
-        r"""calculate the lagrangian loss to get the target dimension"""
-        dimension_score = determinate_mask(self.training_loga)
-        all_dimension = dimension_score.size(1)
-        
-        expected_dimension = torch.sum(dimension_score, -1)
-        loss_dimension = torch.sum((self.target_dimension - expected_dimension) / all_dimension)
+        sp_loss = self.lambda_1 * loss_sparsity + self.lambda_2 * (loss_sparsity ** 2)
+        return sp_loss
+
+    def save_masks(self, file_name: str):
+        if self.loga_param is not None:
+            for (k, v) in self.loga_param:
+                list_name, unit_index, _ = k.split('-')
+                mask = determinate_mask(v)
+                unit_list = getattr(self.plugin, list_name)
+                unit_list[int(unit_index)].mask = mask.half().clone().detach()
         
-        lagrangian_loss = self.lambda_1 * loss_dimension + self.lambda_2 * (loss_dimension ** 2)
+        for _, unit_list in self.plugin.named_lists():
+            unit_list.binarize_mask(hard_binarize=self.strategy.hard_binarize, target_s=self.strategy.target_sparsity)
         
-        return lagrangian_loss, expected_dimension
-
-    def get_model_sparsity(self, layer_constraint: bool = False):
-        r"""calculate the current sparsity to calculate lagrangian loss."""
-        if not layer_constraint:
-            total_res = 0
-            num_res = 0
-            for k, v in self.training_loga.items():
-                # layer-wise
-                for layer_index in range(v.size(0)):
-                    param = self.plugin.__dict__[k.split('_loga')[0]][layer_index]['param']
-                    v_cur = v[layer_index]
-
-                    total_res +=  torch.sum(determinate_mask(v_cur)) * param * 3
-                    num_res   +=  v_cur.numel() * param * 3
-            ratio = total_res / num_res
-        else:
-            ratio = []
-            for k, v in self.training_loga.items():
-                # layer-wise
-                for layer_index in range(v.size(0)):
-                    param = self.plugin.__dict__[k.split('_loga')[0]][layer_index]['param']
-                    v_cur = v[layer_index]
-                    ratio.append(torch.sum(determinate_mask(v_cur)) / v_cur.numel())
-                ratio = torch.stack(ratio)
-        return 1 - ratio  # return sparsity
+        self.plugin.save_masks(file_name)
```

### Comparing `bmcook-0.1.1.1/bmcook/pruning/sprune/func.py` & `bmcook-0.1.2/bmcook/pruning/sprune/func.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,59 @@
 import torch
 import math
 from torch import Tensor
 
+from typing import Optional
+
 gamma, zeta, epsilon = -.1, 1.1, 1e-6
 beta = 2./3.
-
-def cdf_concrete_dist(eps: Tensor, loga: Tensor):
-    r"""Implements the CDF of the 'stretched' concrete distribution"""
-    xn = (eps - gamma) / (zeta - gamma)
-    s = torch.sigmoid((torch.log(xn / (1 - xn)) * beta - loga))
-    z = s.clamp(min=0., max=1.)
-    return z
-
-
-def hard_concrete_dist(loga: Tensor):
-    r"""Implements the gard concrete distribution. For details, see paper 
-    'Learning Sparse Neural Networks through L_0 Regularization' <https://openreview.net/forum?id=H1Y8hhg0b>."""
-    u = torch.FloatTensor(*loga.shape).uniform_(epsilon, 1-epsilon).to(loga.device)
-    s = torch.sigmoid((torch.log(u / (1 - u)) + loga) / beta)
-    s_shift = s * (zeta - gamma) + gamma
-    z = s_shift.clamp(min=0., max=1.).to(device='cuda', dtype=torch.half) 
-    return z
+zero_point = torch.tensor((0 - gamma) / (zeta - gamma))
 
 def l0_norm_term(loga: Tensor):
     r"""calculate the l0 norm term. For details, see paper
     'Structured Pruning of Large Language Models' <https://arxiv.org/abs/1910.04732>"""
     x = loga - beta * (math.log(- gamma / zeta))
     loss = torch.sigmoid(x).sum()
     return loss
 
+def from_sparsity(s: float):
+    sig_input = -math.log((1 / s) - 1)
+    loga = - sig_input + torch.log(zero_point / (1 - zero_point)) * beta
+    return loga
+
 def determinate_mask(loga: Tensor):
-    sig = torch.sigmoid(loga)
-    s = sig * (zeta - gamma) + gamma
-    out = s.clamp(min=0., max=1.)
+    r"""Drop the stochastic sampling in func:sample, used for evaluation when training sprune mask"""
+    sig = torch.sigmoid(torch.log(zero_point / (1 - zero_point)) * beta - loga)
+    s = 1 - sig
+    out = s.clamp(min=epsilon, max=1-epsilon)
     return out
 
 def sample(loga: Tensor):
-    eps = torch.FloatTensor(*loga.shape).uniform_(epsilon, 1-epsilon).to(loga.device)
+    r"""Implements the gard concrete distribution. For details, see paper 
+    'Learning Sparse Neural Networks through L_0 Regularization' <https://openreview.net/forum?id=H1Y8hhg0b>."""
+    eps = loga.new_empty(loga.size()).uniform_(epsilon, 1-epsilon)
     s = torch.sigmoid((torch.log(eps / (1 - eps)) + loga) / beta)
-    s = s * (zeta - gamma) + gamma
-    z = s.clamp(min=0., max=1.)
-    z_ = z.to(device='cuda', dtype=torch.half)  # remove from the computation graph of sp_module
-    return z_
+    z = s.clamp(min=epsilon, max=1-epsilon) # remove from the computation graph of sp_module
+    return z
 
-def binarize(loga: Tensor):
+def binarize(loga: torch.FloatTensor, hard_binarize: bool = False, target_s: Optional[float] = None):
+    r"""According to the score mask, to get 0-1 mask for actual pruning."""
+    dtype, device = torch.half, loga.device
     mask = determinate_mask(loga)
-    expected_num_nonzeros = torch.sum(mask, -1)
-    total_num_nonzeros = loga.size(-1)
-    expected_num_zeros = total_num_nonzeros - expected_num_nonzeros
-    if loga.dim() == 1:
-        num_zeros = round(expected_num_zeros.item())
-        soft_mask = torch.ones_like(loga, dtype=torch.half)
-        if num_zeros > 0:
-            if soft_mask.ndim == 0:
-                soft_mask = torch.tensor(0).to(loga.device)
-            else:
-                _, indices = torch.topk(loga, k=num_zeros, largest=False)  # return values, indices
-                soft_mask[indices] = 0.  # set zero
-        res = soft_mask.to(device='cuda')  # remove from the computation graph of sp_module
-    else:
-        res = []
-        for index in range(loga.size(0)):
-            num_zero = round(expected_num_zeros[index].item())
-            cur_layer = loga[index]
-            soft_mask = torch.ones_like(cur_layer, dtype=torch.half)
-            if num_zero > 0:
-                if soft_mask.ndim == 0:
-                    soft_mask = torch.tensor(0).to(cur_layer.device)
-                else:
-                    _, indices = torch.topk(mask[index], k=num_zero, largest=False)  # 返回values, indices
-                    soft_mask[indices] = 0.  # 置零
-            res.append(soft_mask)
-        res = torch.stack(res)
-    return res
 
+    if not hard_binarize:
+        expected_num_nonzeros = mask.sum()
+        total_num_nonzeros = loga.size(-1)
+        num_zeros = round((total_num_nonzeros - expected_num_nonzeros).item())
+    else:
+        num_zeros = round(torch.tensor(mask.numel() * target_s).item())
 
-def binarize_mask_1d(loga: Tensor):
-    expected_num_nonzeros = torch.sum(1 - cdf_concrete_dist(torch.tensor(0.), loga), -1)
-    expected_num_zeros = loga.size(1) - expected_num_nonzeros
-    
-    num_zeros = round(expected_num_zeros)
-    soft_mask = torch.ones_like(loga)
+    soft_mask = torch.ones_like(loga, dtype=dtype, device=device)
     if num_zeros > 0:
         if soft_mask.ndim == 0:
-            soft_mask = torch.tensor(0).to(loga.device)
+            soft_mask = torch.tensor(0, device=device)
         else:
-            _, indices = torch.topk(loga, k=num_zeros, largest=False)  # return values, indices
+            _, indices = torch.topk(mask, k=num_zeros, largest=False)  # return values, indices
             soft_mask[indices] = 0.  # set zero
-    soft_mask = soft_mask.to(device='cuda', dtype=torch.half)  # remove from the computation graph of sp_module
-    return soft_mask
+    res = soft_mask
+    
+    return res
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bmcook-0.1.1.1/bmcook/utils/arguments.py` & `bmcook-0.1.2/bmcook/utils/arguments.py`

 * *Files identical despite different names*

### Comparing `bmcook-0.1.1.1/bmcook/utils/config.py` & `bmcook-0.1.2/bmcook/utils/config.py`

 * *Files identical despite different names*

### Comparing `bmcook-0.1.1.1/bmcook.egg-info/SOURCES.txt` & `bmcook-0.1.2/bmcook.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 bmcook/__init__.py
 bmcook/store.py
 bmcook/trainer.py
 bmcook.egg-info/PKG-INFO
 bmcook.egg-info/SOURCES.txt
@@ -10,16 +9,18 @@
 bmcook.egg-info/requires.txt
 bmcook.egg-info/top_level.txt
 bmcook/distilling/__init__.py
 bmcook/moe/__init__.py
 bmcook/pruning/__init__.py
 bmcook/pruning/prune_func.py
 bmcook/pruning/sprune/__init__.py
-bmcook/pruning/sprune/do_prune.py
 bmcook/pruning/sprune/engine.py
 bmcook/pruning/sprune/func.py
-bmcook/pruning/sprune/plugin.py
 bmcook/pruning/sprune/utils.py
+bmcook/pruning/sprune/plugin/__init__.py
+bmcook/pruning/sprune/plugin/plugin.py
+bmcook/pruning/sprune/plugin/unit.py
+bmcook/pruning/sprune/plugin/unitlist.py
 bmcook/quant/__init__.py
 bmcook/utils/__init__.py
 bmcook/utils/arguments.py
 bmcook/utils/config.py
```

